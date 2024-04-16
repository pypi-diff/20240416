# Comparing `tmp/stelar_spatiotemporal-0.0.7.tar.gz` & `tmp/stelar_spatiotemporal-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/STELAR_spatiotemporal/STELAR_spatiotemporal/dist/.tmp-efcsk8ud/stelar_spatiotemporal-0.0.7.tar", last modified: Thu Nov  2 12:26:07 2023, max compression
+gzip compressed data, was "/home/runner/work/STELAR_spatiotemporal/STELAR_spatiotemporal/dist/.tmp-8lb394fv/stelar_spatiotemporal-0.0.9.tar", last modified: Thu Dec 21 09:50:32 2023, max compression
```

## Comparing `stelar_spatiotemporal-0.0.7.tar` & `stelar_spatiotemporal-0.0.9.tar`

### file list

```diff
@@ -1,130 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 12:26:07.000000 stelar_spatiotemporal-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2023-11-02 12:26:07.000000 stelar_spatiotemporal-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      993 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-02 12:26:07.000000 stelar_spatiotemporal-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-11-02 12:26:01.000000 stelar_spatiotemporal-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 12:26:07.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 12:26:07.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 12:26:07.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/base/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/base/base_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     7181 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/base/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/base/base_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/base/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/execute.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 12:26:07.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/input/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5071 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/input/eopatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/input/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/input/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8133 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/input/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/input/random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 12:26:07.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/models/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/models/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5252 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/models/classification_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    17287 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/models/classification_temp_nets.py
--rw-r--r--   0 runner    (1001) docker     (127)    15982 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/models/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8428 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/models/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)    11919 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/models/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5784 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/models/pse_tae_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7023 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/models/segmentation_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    27399 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/models/segmentation_unets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7250 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/models/transformer_encoder_layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 12:26:07.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/tasks/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/tasks/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/tasks/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 12:26:07.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/utils/tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 12:26:07.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 12:26:07.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8739 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    24295 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/core/core_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    36600 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/core/eodata.py
--rw-r--r--   0 runner    (1001) docker     (127)    13456 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/core/eodata_io.py
--rw-r--r--   0 runner    (1001) docker     (127)    12068 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/core/eodata_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)    13571 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/core/eoexecution.py
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/core/eotask.py
--rw-r--r--   0 runner    (1001) docker     (127)    19973 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/core/eoworkflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/core/fs_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7005 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/core/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    23656 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/core/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 12:26:07.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/coregistration/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/coregistration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20643 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/coregistration/coregistration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5594 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/coregistration/coregistration_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 12:26:07.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/features/
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4063 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/features/bands_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     5929 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/features/blob.py
--rw-r--r--   0 runner    (1001) docker     (127)     6898 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/features/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     4085 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/features/doubly_logistic_approximation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/features/feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8650 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/features/feature_manipulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8660 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/features/haralick.py
--rw-r--r--   0 runner    (1001) docker     (127)     5262 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/features/hog.py
--rw-r--r--   0 runner    (1001) docker     (127)    30698 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/features/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/features/local_binary_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)    19019 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/features/radiometric_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)    11146 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/features/temporal_features.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 12:26:07.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/geometry/
--rw-r--r--   0 runner    (1001) docker     (127)      548 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/geometry/morphology.py
--rw-r--r--   0 runner    (1001) docker     (127)    17979 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/geometry/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     6923 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/geometry/superpixel.py
--rw-r--r--   0 runner    (1001) docker     (127)    22809 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/geometry/transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 12:26:07.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/io/
--rw-r--r--   0 runner    (1001) docker     (127)      541 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11157 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/io/geometry_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     6665 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/io/geopedia.py
--rw-r--r--   0 runner    (1001) docker     (127)    21300 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/io/local_io.py
--rw-r--r--   0 runner    (1001) docker     (127)    11163 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/io/meteoblue.py
--rw-r--r--   0 runner    (1001) docker     (127)    29932 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/io/sentinelhub_process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 12:26:07.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/mask/
--rw-r--r--   0 runner    (1001) docker     (127)      377 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/mask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25398 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/mask/cloud_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/mask/mask_counting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6176 2023-11-02 12:25:53.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/mask/masking.py
--rw-r--r--   0 runner    (1001) docker     (127)    14529 2023-11-02 12:25:54.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/mask/snow_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2023-11-02 12:25:54.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/mask/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 12:26:07.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/ml_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2023-11-02 12:25:54.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/ml_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16460 2023-11-02 12:25:54.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/ml_tools/classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5254 2023-11-02 12:25:54.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/ml_tools/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2023-11-02 12:25:54.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/ml_tools/train_test_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2023-11-02 12:25:54.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/ml_tools/truth_transformations.py
--rw-r--r--   0 runner    (1001) docker     (127)     8454 2023-11-02 12:25:54.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/ml_tools/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     8318 2023-11-02 12:25:54.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/ml_tools/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 12:26:07.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2023-11-02 12:25:54.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6275 2023-11-02 12:25:54.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/visualization/eoexecutor_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)    14051 2023-11-02 12:25:54.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/visualization/eopatch_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2023-11-02 12:25:54.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/visualization/eoworkflow_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8464 2023-11-02 12:25:54.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/visualization/xarray_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4157 2023-11-02 12:25:54.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eopatch_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2023-11-02 12:25:54.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     8521 2023-11-02 12:25:54.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 12:26:07.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2023-11-02 12:25:54.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15546 2023-11-02 12:25:54.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/preprocessing/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    15211 2023-11-02 12:25:54.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/preprocessing/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)     5475 2023-11-02 12:25:54.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/preprocessing/vista_preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 12:26:07.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2023-11-02 12:25:54.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2023-11-02 12:25:54.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/segmentation/bands_data_package.py
--rw-r--r--   0 runner    (1001) docker     (127)    15639 2023-11-02 12:25:54.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/segmentation/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 12:26:07.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2023-11-02 12:26:07.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5373 2023-11-02 12:26:07.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-02 12:26:07.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      161 2023-11-02 12:26:07.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-02 12:26:07.000000 stelar_spatiotemporal-0.0.7/stelar_spatiotemporal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:50:32.000000 stelar_spatiotemporal-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2023-12-21 09:50:32.000000 stelar_spatiotemporal-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-21 09:50:32.000000 stelar_spatiotemporal-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-12-21 09:50:27.000000 stelar_spatiotemporal-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:50:32.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:50:32.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:50:32.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/base/base_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7181 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/base/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/base/base_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/base/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/execute.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:50:32.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/input/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5071 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/input/eopatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/input/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/input/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8133 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/input/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/input/random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:50:32.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/models/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5252 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/models/classification_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17287 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/models/classification_temp_nets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15982 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8428 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/models/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11919 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/models/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5784 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/models/pse_tae_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7023 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/models/segmentation_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27399 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/models/segmentation_unets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7250 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/models/transformer_encoder_layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:50:32.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/tasks/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/tasks/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/tasks/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:50:32.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/utils/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:50:32.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:50:32.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8739 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24295 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/core/core_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36600 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/core/eodata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13456 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/core/eodata_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12068 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/core/eodata_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13571 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/core/eoexecution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/core/eotask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19973 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/core/eoworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/core/fs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7005 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/core/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23656 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/core/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:50:32.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/coregistration/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/coregistration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20643 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/coregistration/coregistration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5594 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/coregistration/coregistration_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:50:32.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/features/bands_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5929 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/features/blob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6898 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/features/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4085 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/features/doubly_logistic_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/features/feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8650 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/features/feature_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8660 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/features/haralick.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5262 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/features/hog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30698 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/features/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/features/local_binary_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19019 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/features/radiometric_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11146 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/features/temporal_features.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:50:32.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/geometry/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17979 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/geometry/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6923 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/geometry/superpixel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22809 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/geometry/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:50:32.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11157 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/io/geometry_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6665 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/io/geopedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21300 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/io/local_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11163 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/io/meteoblue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29932 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/io/sentinelhub_process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:50:32.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/mask/
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/mask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25398 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/mask/cloud_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/mask/mask_counting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6176 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/mask/masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14529 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/mask/snow_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/mask/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:50:32.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/ml_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/ml_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16460 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/ml_tools/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5254 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/ml_tools/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/ml_tools/train_test_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/ml_tools/truth_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8454 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/ml_tools/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8318 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/ml_tools/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:50:32.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6275 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/visualization/eoexecutor_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14051 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/visualization/eopatch_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/visualization/eoworkflow_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8464 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/visualization/xarray_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4157 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eopatch_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:50:32.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/imputation/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/imputation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8596 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/imputation/imputation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8519 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:50:32.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15546 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/preprocessing/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15408 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/preprocessing/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5475 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/preprocessing/vista_preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:50:32.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/segmentation/bands_data_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15639 2023-12-21 09:50:21.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/segmentation/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:50:32.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2023-12-21 09:50:32.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5465 2023-12-21 09:50:32.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-21 09:50:32.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2023-12-21 09:50:32.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-21 09:50:32.000000 stelar_spatiotemporal-0.0.9/stelar_spatiotemporal.egg-info/top_level.txt
```

### Comparing `stelar_spatiotemporal-0.0.7/LICENSE` & `stelar_spatiotemporal-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/PKG-INFO` & `stelar_spatiotemporal-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stelar_spatiotemporal
-Version: 0.0.7
+Version: 0.0.9
 Summary: Spatiotemporal data processing for the STELAR project
 Author: Jens d'Hondt
 Author-email: j.e.d.hondt@tue.nl
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
@@ -13,15 +13,15 @@
 
 This package is part of the EU STELAR project and provides tools for processing spatiotemporal data. The package includes functionality for field delineation (i.e., segmentation) of satellite images, extracting LAI timseries out of the images, and interpolating cloud covers, among others.
 
 ## Installation
 
 To install the package, simply run:
 ```
-pip install git+https://github.com/JdHondt/STELAR_spatiotemporal.git@master
+pip install git+https://github.com/stelar-eu/STELAR_spatiotemporal.git@master
 ```
 
 ## Usage
 
 To use the package, import it in your Python code:
 
 ```python
```

### Comparing `stelar_spatiotemporal-0.0.7/README.md` & `stelar_spatiotemporal-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 This package is part of the EU STELAR project and provides tools for processing spatiotemporal data. The package includes functionality for field delineation (i.e., segmentation) of satellite images, extracting LAI timseries out of the images, and interpolating cloud covers, among others.
 
 ## Installation
 
 To install the package, simply run:
 ```
-pip install git+https://github.com/JdHondt/STELAR_spatiotemporal.git@master
+pip install git+https://github.com/stelar-eu/STELAR_spatiotemporal.git@master
 ```
 
 ## Usage
 
 To use the package, import it in your Python code:
 
 ```python
```

### Comparing `stelar_spatiotemporal-0.0.7/setup.py` & `stelar_spatiotemporal-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     LONG_DESCRIPTION = "\\n" + fh.read()
 
 setup(
     name='stelar_spatiotemporal',
-    version='0.0.7',
+    version='0.0.9',
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     author="Jens d'Hondt",
     author_email="j.e.d.hondt@tue.nl",
     packages=find_packages(),
     install_requires=[
         "pystac",
```

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/base/base_model.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/base/base_model.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/base/base_task.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/base/base_task.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/base/configuration.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/base/configuration.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/execute.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/execute.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/input/eopatch.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/input/eopatch.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/input/hdf5.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/input/hdf5.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/input/numpy.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/input/numpy.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/input/operations.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/input/operations.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/input/random.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/input/random.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/models/callbacks.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/models/callbacks.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/models/classification_base.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/models/classification_base.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/models/classification_temp_nets.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/models/classification_temp_nets.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/models/layers.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/models/layers.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/models/losses.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/models/losses.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/models/metrics.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/models/metrics.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/models/pse_tae_layers.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/models/pse_tae_layers.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/models/segmentation_base.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/models/segmentation_base.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/models/segmentation_unets.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/models/segmentation_unets.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/models/transformer_encoder_layers.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/models/transformer_encoder_layers.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/tasks/evaluate.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/tasks/evaluate.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/tasks/predict.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/tasks/predict.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/tasks/train.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/tasks/train.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/utils/tf_utils.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/utils/tf_utils.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eoflow/utils/utils.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eoflow/utils/utils.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/core/__init__.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/core/__init__.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/core/constants.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/core/constants.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/core/core_tasks.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/core/core_tasks.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/core/eodata.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/core/eodata.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/core/eodata_io.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/core/eodata_io.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/core/eodata_merge.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/core/eodata_merge.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/core/eoexecution.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/core/eoexecution.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/core/eotask.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/core/eotask.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/core/eoworkflow.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/core/eoworkflow.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/core/fs_utils.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/core/fs_utils.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/core/graph.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/core/graph.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/core/utilities.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/core/utilities.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/coregistration/coregistration.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/coregistration/coregistration.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/coregistration/coregistration_utilities.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/coregistration/coregistration_utilities.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/features/__init__.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/features/__init__.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/features/bands_extraction.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/features/bands_extraction.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/features/blob.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/features/blob.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/features/clustering.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/features/clustering.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/features/doubly_logistic_approximation.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/features/doubly_logistic_approximation.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/features/feature_extractor.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/features/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/features/feature_manipulation.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/features/feature_manipulation.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/features/haralick.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/features/haralick.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/features/hog.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/features/hog.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/features/interpolation.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/features/interpolation.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/features/local_binary_pattern.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/features/local_binary_pattern.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/features/radiometric_normalization.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/features/radiometric_normalization.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/features/temporal_features.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/features/temporal_features.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/geometry/__init__.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/geometry/morphology.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/geometry/morphology.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/geometry/sampling.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/geometry/sampling.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/geometry/superpixel.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/geometry/superpixel.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/geometry/transformations.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/geometry/transformations.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/io/__init__.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/io/__init__.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/io/geometry_io.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/io/geometry_io.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/io/geopedia.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/io/geopedia.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/io/local_io.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/io/local_io.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/io/meteoblue.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/io/meteoblue.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/io/sentinelhub_process.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/io/sentinelhub_process.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/mask/cloud_mask.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/mask/cloud_mask.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/mask/mask_counting.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/mask/mask_counting.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/mask/masking.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/mask/masking.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/mask/snow_mask.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/mask/snow_mask.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/mask/utilities.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/mask/utilities.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/ml_tools/__init__.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/ml_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/ml_tools/classifier.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/ml_tools/classifier.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/ml_tools/postprocessing.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/ml_tools/postprocessing.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/ml_tools/train_test_split.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/ml_tools/train_test_split.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/ml_tools/truth_transformations.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/ml_tools/truth_transformations.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/ml_tools/utilities.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/ml_tools/utilities.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/ml_tools/validator.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/ml_tools/validator.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/visualization/eoexecutor_visualization.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/visualization/eoexecutor_visualization.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/visualization/eopatch_visualization.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/visualization/eopatch_visualization.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/visualization/eoworkflow_visualization.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/visualization/eoworkflow_visualization.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eolearn/visualization/xarray_utils.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eolearn/visualization/xarray_utils.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/eopatch_functions.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/eopatch_functions.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/io.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/io.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/lib.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,25 +125,25 @@
     rescaled = (rescaled - np.min(rescaled)) / (np.max(rescaled) - np.min(rescaled))
 
     # assert np.sum(~np.isfinite(rescaled)) == 0
 
     return rescaled
 
 
-def export_eopatch_to_tiff(eop_path:str, out_path:str, feature:tuple, nodata:int=0, channel_pos:int=-1):
+def export_eopatch_to_tiff(eop_path:str, out_path:str, feature:tuple, nodata:int=0, channel_pos:int=0):
     eopatch = EOPatch.load(eop_path, lazy_loading=True)
 
     image_array = eopatch[feature].squeeze()
 
     if len(image_array.shape) > 3:
         raise ValueError(f"Feature {feature} has more than 3 dimensions, make sure to select either a single timestamp or a single band")
     
     if len(image_array.shape) == 2:
-        image_array = image_array[..., np.newaxis]
-        channel_pos = -1
+        image_array = image_array[np.newaxis, ...]
+        channel_pos = 0
 
     # Get image dimensions
     img_shape = list(image_array.shape)
     channel_count = img_shape[channel_pos]
 
     # Width and height are the other two dimensions
     img_shape.pop(channel_pos)
```

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/preprocessing/preprocessing.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/preprocessing/preprocessing.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/preprocessing/timeseries.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/preprocessing/timeseries.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import shutil
 from shapely.geometry import Polygon
 import rasterio
 from rasterio.mask import mask as mask_func
 import geopandas as gpd
 from typing import Union
 import fiona
+import time
 
 from ..eolearn.core import EOPatch, FeatureType, OverwritePermission
 from ..lib import check_types, multiprocess_map, export_eopatch_to_tiff, df_to_csv_manual, load_bbox, get_filesystem
 from .preprocessing import split_array_into_patchlets, split_patch_into_patchlets, combine_dates_for_eopatch
 
 
 def get_px_csv_path(outdir:str, prefix:str, x:str, y:str):
@@ -241,15 +242,15 @@
 def load_fields(field_path:str, nrows:int = None, min_area:int = 0, max_area:int = 500000):
     # Get the filesystem
     filesystem = get_filesystem(field_path)
 
     # Read fields with fiona and store as a geopandas dataframe
     lines = []
     c = 0
-    with fiona.open(filesystem.open(field_path)) as fields_file:
+    with fiona.open(filesystem.open(field_path, 'rb')) as fields_file:
         for line in fields_file:
             # Get feature
             feature = line['geometry']
 
             # Get area
             area = Polygon(feature['coordinates'][0]).area
 
@@ -352,32 +353,37 @@
                 fields = load_fields(fields_path, min_area=minarea, max_area=maxarea) 
         else:
                 fields = load_fields(fields_path, nrows=nfields, min_area=minarea, max_area=maxarea)
 
         for i, eop_path in enumerate(eop_paths):
                 print(f"Processing eopatch {i+1}/{len(eop_paths)}")
 
+                start = time.time()
+
                 # 0. Get the datetimes
                 eop = EOPatch.load(eop_path, lazy_loading=True)
                 datetimes = eop.timestamp
 
                 # 1. Save the eopatches as tiff if necessary
-                print(f"1. Temporarily saving eopatch as tiff", end="\r")
+                print(f"1. Temporarily saving eopatch as tiff")
                 tiff_path = os.path.join(tif_dir, os.path.basename(eop_path) + ".tiff")
                 if not os.path.exists(tiff_path):
                         export_eopatch_to_tiff(eop_path, tiff_path, feature=(FeatureType.DATA, "LAI"), nodata=0, channel_pos=0)
+                print(f"Time taken: {time.time() - start} seconds")
 
+                start = time.time()
                 # 3. For each field, mask the tiff, get median and save timeseries as csv
-                print(f"3. Masking tiff and saving timeseries", end="\r")
+                print(f"2. Masking tiff and saving timeseries")
                 outpath = os.path.join(outdir, "lai_field_timeseries.csv")
                 field_to_csv(fields, tiff_path, datetimes, outpath, n_jobs=n_jobs)
+                print(f"Time taken: {time.time() - start} seconds")
                 
                 # 4. Delete the temporary tiff
                 if delete_tmp:
-                        print(f"4. Deleting temporary tiff", end="\r")
+                        print(f"4. Deleting temporary tiff")
                         os.remove(tiff_path)
 
 
 def lai_to_csv_field_append(npy_path:str, bbox_path:str, fields_path:str, outdir:str, n_jobs:int=8):
     tmp_eop_path = "tmp_eop"
     timestamp = dt.datetime.strptime(os.path.basename(npy_path).replace(".npy",""), "%Y_%m_%d")
```

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/preprocessing/vista_preprocessing.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/preprocessing/vista_preprocessing.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/segmentation/bands_data_package.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/segmentation/bands_data_package.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal/segmentation/segmentation.py` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal/segmentation/segmentation.py`

 * *Files identical despite different names*

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal.egg-info/PKG-INFO` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stelar-spatiotemporal
-Version: 0.0.7
+Version: 0.0.9
 Summary: Spatiotemporal data processing for the STELAR project
 Author: Jens d'Hondt
 Author-email: j.e.d.hondt@tue.nl
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
@@ -13,15 +13,15 @@
 
 This package is part of the EU STELAR project and provides tools for processing spatiotemporal data. The package includes functionality for field delineation (i.e., segmentation) of satellite images, extracting LAI timseries out of the images, and interpolating cloud covers, among others.
 
 ## Installation
 
 To install the package, simply run:
 ```
-pip install git+https://github.com/JdHondt/STELAR_spatiotemporal.git@master
+pip install git+https://github.com/stelar-eu/STELAR_spatiotemporal.git@master
 ```
 
 ## Usage
 
 To use the package, import it in your Python code:
 
 ```python
```

### Comparing `stelar_spatiotemporal-0.0.7/stelar_spatiotemporal.egg-info/SOURCES.txt` & `stelar_spatiotemporal-0.0.9/stelar_spatiotemporal.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -95,14 +95,16 @@
 stelar_spatiotemporal/eolearn/ml_tools/utilities.py
 stelar_spatiotemporal/eolearn/ml_tools/validator.py
 stelar_spatiotemporal/eolearn/visualization/__init__.py
 stelar_spatiotemporal/eolearn/visualization/eoexecutor_visualization.py
 stelar_spatiotemporal/eolearn/visualization/eopatch_visualization.py
 stelar_spatiotemporal/eolearn/visualization/eoworkflow_visualization.py
 stelar_spatiotemporal/eolearn/visualization/xarray_utils.py
+stelar_spatiotemporal/imputation/__init__.py
+stelar_spatiotemporal/imputation/imputation.py
 stelar_spatiotemporal/preprocessing/__init__.py
 stelar_spatiotemporal/preprocessing/preprocessing.py
 stelar_spatiotemporal/preprocessing/timeseries.py
 stelar_spatiotemporal/preprocessing/vista_preprocessing.py
 stelar_spatiotemporal/segmentation/__init__.py
 stelar_spatiotemporal/segmentation/bands_data_package.py
 stelar_spatiotemporal/segmentation/segmentation.py
```

