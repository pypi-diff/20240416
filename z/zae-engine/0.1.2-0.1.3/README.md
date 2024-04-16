# Comparing `tmp/zae_engine-0.1.2.tar.gz` & `tmp/zae_engine-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zae_engine-0.1.2.tar", max compression
+gzip compressed data, was "zae_engine-0.1.3.tar", max compression
```

## Comparing `zae_engine-0.1.2.tar` & `zae_engine-0.1.3.tar`

### file list

```diff
@@ -1,75 +1,74 @@
--rw-r--r--   0        0        0     2007 2024-03-18 02:01:14.925084 zae_engine-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       39 2024-03-18 00:46:13.767730 zae_engine-0.1.2/zae_cli/__init__.py
--rw-r--r--   0        0        0     1317 2024-03-18 00:46:13.768238 zae_engine-0.1.2/zae_cli/cli.py
--rw-r--r--   0        0        0     4135 2024-03-18 00:46:13.768238 zae_engine-0.1.2/zae_cli/example_script.py
--rw-r--r--   0        0        0      727 2024-03-18 00:46:13.768238 zae_engine-0.1.2/zae_cli/io.py
--rw-r--r--   0        0        0     3601 2024-03-18 00:46:13.768238 zae_engine-0.1.2/zae_cli/tree_builder.py
--rw-r--r--   0        0        0      221 2024-03-18 00:46:13.768238 zae_engine-0.1.2/zae_engine/__init__.py
--rw-r--r--   0        0        0       47 2023-10-25 08:01:07.685942 zae_engine-0.1.2/zae_engine/data_pipeline/__init__.py
--rw-r--r--   0        0        0      216 2023-10-26 01:47:49.645644 zae_engine-0.1.2/zae_engine/data_pipeline/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2634 2023-10-26 01:47:49.645644 zae_engine-0.1.2/zae_engine/data_pipeline/__pycache__/_fileio.cpython-310.pyc
--rw-r--r--   0        0        0     6796 2024-02-06 07:49:15.003844 zae_engine-0.1.2/zae_engine/data_pipeline/__pycache__/collate.cpython-310.pyc
--rw-r--r--   0        0        0     2651 2023-10-25 08:01:07.685942 zae_engine-0.1.2/zae_engine/data_pipeline/_fileio.py
--rw-r--r--   0        0        0     7678 2024-02-06 02:01:08.594408 zae_engine-0.1.2/zae_engine/data_pipeline/collate.py
--rw-r--r--   0        0        0        0 2023-10-25 08:01:07.686939 zae_engine-0.1.2/zae_engine/data_pipeline/resource/__init__.py
--rw-r--r--   0        0        0      151 2023-10-13 05:26:24.577765 zae_engine-0.1.2/zae_engine/data_pipeline/resource/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    10000 2023-10-25 08:01:07.686939 zae_engine-0.1.2/zae_engine/data_pipeline/resource/sample_data.dat
--rw-r--r--   0        0        0      115 2023-10-25 08:01:07.686939 zae_engine-0.1.2/zae_engine/data_pipeline/resource/sample_data.hea
--rw-r--r--   0        0        0      178 2023-10-25 08:01:07.686939 zae_engine-0.1.2/zae_engine/data_pipeline/resource/sample_data.zae
--rw-r--r--   0        0        0       92 2024-02-06 01:49:00.431862 zae_engine-0.1.2/zae_engine/inference/__init__.py
--rw-r--r--   0        0        0      240 2024-02-06 07:49:04.128830 zae_engine-0.1.2/zae_engine/inference/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3747 2024-02-06 07:49:04.130853 zae_engine-0.1.2/zae_engine/inference/__pycache__/beat.cpython-310.pyc
--rw-r--r--   0        0        0     6402 2024-02-06 07:49:16.782915 zae_engine-0.1.2/zae_engine/inference/__pycache__/sec10.cpython-310.pyc
--rw-r--r--   0        0        0     3165 2024-02-06 02:01:08.594408 zae_engine-0.1.2/zae_engine/inference/beat.py
--rw-r--r--   0        0        0     5404 2024-02-06 02:01:08.594408 zae_engine-0.1.2/zae_engine/inference/sec10.py
--rw-r--r--   0        0        0      108 2023-08-22 05:18:53.112758 zae_engine-0.1.2/zae_engine/loss/__init__.py
--rw-r--r--   0        0        0      265 2023-10-13 05:21:20.139025 zae_engine-0.1.2/zae_engine/loss/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3067 2023-10-26 01:53:01.317426 zae_engine-0.1.2/zae_engine/loss/__pycache__/_loss.cpython-310.pyc
--rw-r--r--   0        0        0     3192 2023-10-25 08:01:07.686939 zae_engine-0.1.2/zae_engine/loss/_loss.py
--rw-r--r--   0        0        0      319 2024-02-06 02:01:08.594937 zae_engine-0.1.2/zae_engine/measure/__init__.py
--rw-r--r--   0        0        0      464 2024-02-06 07:49:16.956139 zae_engine-0.1.2/zae_engine/measure/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     9902 2024-02-06 07:49:16.958140 zae_engine-0.1.2/zae_engine/measure/__pycache__/_measure.cpython-310.pyc
--rw-r--r--   0        0        0    11758 2024-02-06 02:01:08.594937 zae_engine-0.1.2/zae_engine/measure/_measure.py
--rw-r--r--   0        0        0      211 2024-02-06 02:01:08.594937 zae_engine-0.1.2/zae_engine/models/__init__.py
--rw-r--r--   0        0        0      362 2024-02-06 07:49:04.131829 zae_engine-0.1.2/zae_engine/models/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2035 2024-02-06 07:49:04.132830 zae_engine-0.1.2/zae_engine/models/__pycache__/benchmark.cpython-310.pyc
--rw-r--r--   0        0        0    15157 2024-02-06 07:49:04.136342 zae_engine-0.1.2/zae_engine/models/__pycache__/build.cpython-310.pyc
--rw-r--r--   0        0        0     3666 2023-10-25 10:00:41.514047 zae_engine-0.1.2/zae_engine/models/__pycache__/utility.cpython-310.pyc
--rw-r--r--   0        0        0     2521 2024-02-06 01:49:00.432895 zae_engine-0.1.2/zae_engine/models/benchmark.py
--rw-r--r--   0        0        0    18698 2024-03-18 00:46:13.768744 zae_engine-0.1.2/zae_engine/models/build.py
--rw-r--r--   0        0        0      173 2023-08-22 05:18:53.113750 zae_engine-0.1.2/zae_engine/models/resource/.env
--rw-r--r--   0        0        0        0 2023-08-22 05:18:53.113750 zae_engine-0.1.2/zae_engine/models/resource/__init__.py
--rw-r--r--   0        0        0      153 2023-10-13 05:26:24.577765 zae_engine-0.1.2/zae_engine/models/resource/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3846 2023-10-25 08:01:07.687937 zae_engine-0.1.2/zae_engine/models/utility.py
--rw-r--r--   0        0        0      126 2023-08-22 05:18:53.114750 zae_engine-0.1.2/zae_engine/nn_night/__init__.py
--rw-r--r--   0        0        0      211 2023-10-12 10:51:08.636534 zae_engine-0.1.2/zae_engine/nn_night/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1064 2023-10-12 10:51:08.637658 zae_engine-0.1.2/zae_engine/nn_night/__pycache__/_activation.cpython-310.pyc
--rw-r--r--   0        0        0     1871 2023-10-12 10:51:08.638683 zae_engine-0.1.2/zae_engine/nn_night/__pycache__/_layer.cpython-310.pyc
--rw-r--r--   0        0        0     8070 2023-10-25 10:00:41.498447 zae_engine-0.1.2/zae_engine/nn_night/__pycache__/_module.cpython-310.pyc
--rw-r--r--   0        0        0      597 2023-08-22 05:18:53.114750 zae_engine-0.1.2/zae_engine/nn_night/_activation.py
--rw-r--r--   0        0        0     1736 2023-08-22 05:18:53.114750 zae_engine-0.1.2/zae_engine/nn_night/_layer.py
--rw-r--r--   0        0        0     7702 2023-10-25 08:01:07.687937 zae_engine-0.1.2/zae_engine/nn_night/_module.py
--rw-r--r--   0        0        0      337 2024-02-06 02:01:08.595563 zae_engine-0.1.2/zae_engine/operation/__init__.py
--rw-r--r--   0        0        0      426 2024-02-06 07:49:16.723406 zae_engine-0.1.2/zae_engine/operation/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     8941 2024-02-06 07:49:16.726406 zae_engine-0.1.2/zae_engine/operation/__pycache__/_operation.cpython-310.pyc
--rw-r--r--   0        0        0    10306 2024-02-06 01:49:00.433405 zae_engine-0.1.2/zae_engine/operation/_operation.py
--rw-r--r--   0        0        0        0 2023-10-25 08:01:07.688932 zae_engine-0.1.2/zae_engine/scripts/__init__.py
--rw-r--r--   0        0        0     3532 2023-10-25 08:01:07.688932 zae_engine-0.1.2/zae_engine/scripts/example_script.py
--rw-r--r--   0        0        0       53 2023-08-22 05:18:53.119737 zae_engine-0.1.2/zae_engine/trainer/__init__.py
--rw-r--r--   0        0        0      207 2023-10-13 05:01:18.404200 zae_engine-0.1.2/zae_engine/trainer/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    12599 2024-02-07 00:38:41.182459 zae_engine-0.1.2/zae_engine/trainer/__pycache__/_trainer.cpython-310.pyc
--rw-r--r--   0        0        0     3828 2023-11-02 07:34:59.267084 zae_engine-0.1.2/zae_engine/trainer/__pycache__/mpu_utils.cpython-310.pyc
--rw-r--r--   0        0        0    12698 2024-03-18 00:46:13.769358 zae_engine-0.1.2/zae_engine/trainer/_trainer.py
--rw-r--r--   0        0        0     2963 2023-08-22 05:18:53.119737 zae_engine-0.1.2/zae_engine/trainer/mpu_utils.py
--rw-r--r--   0        0        0       50 2023-08-22 05:18:53.119737 zae_engine-0.1.2/zae_engine/trainer/utils/__init__.py
--rw-r--r--   0        0        0      196 2023-10-13 05:01:18.404200 zae_engine-0.1.2/zae_engine/trainer/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     5660 2023-10-13 05:01:18.404200 zae_engine-0.1.2/zae_engine/trainer/utils/__pycache__/_callback.cpython-310.pyc
--rw-r--r--   0        0        0     2524 2024-02-06 07:49:06.904855 zae_engine-0.1.2/zae_engine/trainer/utils/__pycache__/_logger.cpython-310.pyc
--rw-r--r--   0        0        0     5723 2023-08-22 05:18:53.119737 zae_engine-0.1.2/zae_engine/trainer/utils/_callback.py
--rw-r--r--   0        0        0     2164 2024-03-18 00:46:13.769358 zae_engine-0.1.2/zae_engine/trainer/utils/_logger.py
--rw-r--r--   0        0        0       19 2024-03-18 00:46:13.769358 zae_engine-0.1.2/zae_engine/utils/__init__.py
--rw-r--r--   0        0        0      162 2024-03-12 06:07:08.919387 zae_engine-0.1.2/zae_engine/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      892 2024-02-06 07:49:16.984655 zae_engine-0.1.2/zae_engine/utils/__pycache__/io.cpython-310.pyc
--rw-r--r--   0        0        0      727 2024-03-18 00:46:13.769860 zae_engine-0.1.2/zae_engine/utils/io.py
--rw-r--r--   0        0        0     1118 2024-02-06 02:01:08.595563 zae_engine-0.1.2/zae_engine/zae_engine.py
--rw-r--r--   0        0        0     1686 1970-01-01 00:00:00.000000 zae_engine-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2171 2024-04-16 01:27:10.985783 zae_engine-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       20 2024-04-16 01:26:56.056447 zae_engine-0.1.3/zae_cli/__init__.py
+-rw-r--r--   0        0        0     1312 2024-04-16 01:26:56.056447 zae_engine-0.1.3/zae_cli/cli.py
+-rw-r--r--   0        0        0     3978 2024-04-16 01:26:56.056447 zae_engine-0.1.3/zae_cli/example_script.py
+-rw-r--r--   0        0        0     5346 2024-04-16 01:26:56.056447 zae_engine-0.1.3/zae_cli/tree_builder.py
+-rw-r--r--   0        0        0      221 2024-03-22 02:49:57.138724 zae_engine-0.1.3/zae_engine/__init__.py
+-rw-r--r--   0        0        0       47 2023-10-25 08:01:07.685942 zae_engine-0.1.3/zae_engine/data_pipeline/__init__.py
+-rw-r--r--   0        0        0      216 2023-10-26 01:47:49.645644 zae_engine-0.1.3/zae_engine/data_pipeline/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2634 2023-10-26 01:47:49.645644 zae_engine-0.1.3/zae_engine/data_pipeline/__pycache__/_fileio.cpython-310.pyc
+-rw-r--r--   0        0        0     6796 2024-03-22 09:37:52.311184 zae_engine-0.1.3/zae_engine/data_pipeline/__pycache__/collate.cpython-310.pyc
+-rw-r--r--   0        0        0    10000 2024-04-16 01:26:56.056447 zae_engine-0.1.3/zae_engine/data_pipeline/__sample/sample_data.dat
+-rw-r--r--   0        0        0      115 2024-04-16 01:26:56.056447 zae_engine-0.1.3/zae_engine/data_pipeline/__sample/sample_data.hea
+-rw-r--r--   0        0        0      178 2024-04-16 01:26:56.056447 zae_engine-0.1.3/zae_engine/data_pipeline/__sample/sample_data.zae
+-rw-r--r--   0        0        0     2649 2024-04-16 01:26:56.056447 zae_engine-0.1.3/zae_engine/data_pipeline/_fileio.py
+-rw-r--r--   0        0        0     7678 2024-03-22 02:49:57.138724 zae_engine-0.1.3/zae_engine/data_pipeline/collate.py
+-rw-r--r--   0        0        0      160 2024-04-03 05:59:23.010944 zae_engine-0.1.3/zae_engine/data_pipeline/resource/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0       92 2024-02-06 01:49:00.431862 zae_engine-0.1.3/zae_engine/inference/__init__.py
+-rw-r--r--   0        0        0      240 2024-02-06 07:49:04.128830 zae_engine-0.1.3/zae_engine/inference/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3747 2024-03-22 09:37:26.872146 zae_engine-0.1.3/zae_engine/inference/__pycache__/beat.cpython-310.pyc
+-rw-r--r--   0        0        0     6402 2024-03-22 09:38:38.576140 zae_engine-0.1.3/zae_engine/inference/__pycache__/sec10.cpython-310.pyc
+-rw-r--r--   0        0        0     3165 2024-03-22 02:49:57.139227 zae_engine-0.1.3/zae_engine/inference/beat.py
+-rw-r--r--   0        0        0     5404 2024-03-22 02:49:57.139227 zae_engine-0.1.3/zae_engine/inference/sec10.py
+-rw-r--r--   0        0        0      108 2023-08-22 05:18:53.112758 zae_engine-0.1.3/zae_engine/loss/__init__.py
+-rw-r--r--   0        0        0      265 2023-10-13 05:21:20.139025 zae_engine-0.1.3/zae_engine/loss/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3067 2023-10-26 01:53:01.317426 zae_engine-0.1.3/zae_engine/loss/__pycache__/_loss.cpython-310.pyc
+-rw-r--r--   0        0        0     3192 2023-10-25 08:01:07.686939 zae_engine-0.1.3/zae_engine/loss/_loss.py
+-rw-r--r--   0        0        0      319 2024-03-22 02:49:57.139227 zae_engine-0.1.3/zae_engine/measure/__init__.py
+-rw-r--r--   0        0        0      464 2024-03-22 09:38:39.300978 zae_engine-0.1.3/zae_engine/measure/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     9902 2024-03-22 09:38:39.300978 zae_engine-0.1.3/zae_engine/measure/__pycache__/_measure.cpython-310.pyc
+-rw-r--r--   0        0        0    11758 2024-03-22 02:49:57.139227 zae_engine-0.1.3/zae_engine/measure/_measure.py
+-rw-r--r--   0        0        0      211 2024-03-22 02:49:57.139750 zae_engine-0.1.3/zae_engine/models/__init__.py
+-rw-r--r--   0        0        0      362 2024-03-22 09:37:26.872146 zae_engine-0.1.3/zae_engine/models/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2035 2024-02-06 07:49:04.132830 zae_engine-0.1.3/zae_engine/models/__pycache__/benchmark.cpython-310.pyc
+-rw-r--r--   0        0        0    15157 2024-04-01 02:27:03.418596 zae_engine-0.1.3/zae_engine/models/__pycache__/build.cpython-310.pyc
+-rw-r--r--   0        0        0     3666 2023-10-25 10:00:41.514047 zae_engine-0.1.3/zae_engine/models/__pycache__/utility.cpython-310.pyc
+-rw-r--r--   0        0        0     2521 2024-02-06 01:49:00.432895 zae_engine-0.1.3/zae_engine/models/benchmark.py
+-rw-r--r--   0        0        0    18698 2024-03-22 09:50:46.101618 zae_engine-0.1.3/zae_engine/models/build.py
+-rw-r--r--   0        0        0      173 2023-08-22 05:18:53.113750 zae_engine-0.1.3/zae_engine/models/resource/.env
+-rw-r--r--   0        0        0        0 2023-08-22 05:18:53.113750 zae_engine-0.1.3/zae_engine/models/resource/__init__.py
+-rw-r--r--   0        0        0      153 2023-10-13 05:26:24.577765 zae_engine-0.1.3/zae_engine/models/resource/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3846 2023-10-25 08:01:07.687937 zae_engine-0.1.3/zae_engine/models/utility.py
+-rw-r--r--   0        0        0      126 2023-08-22 05:18:53.114750 zae_engine-0.1.3/zae_engine/nn_night/__init__.py
+-rw-r--r--   0        0        0      211 2023-10-12 10:51:08.636534 zae_engine-0.1.3/zae_engine/nn_night/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1064 2023-10-12 10:51:08.637658 zae_engine-0.1.3/zae_engine/nn_night/__pycache__/_activation.cpython-310.pyc
+-rw-r--r--   0        0        0     1871 2023-10-12 10:51:08.638683 zae_engine-0.1.3/zae_engine/nn_night/__pycache__/_layer.cpython-310.pyc
+-rw-r--r--   0        0        0     8070 2023-10-25 10:00:41.498447 zae_engine-0.1.3/zae_engine/nn_night/__pycache__/_module.cpython-310.pyc
+-rw-r--r--   0        0        0      597 2023-08-22 05:18:53.114750 zae_engine-0.1.3/zae_engine/nn_night/_activation.py
+-rw-r--r--   0        0        0     1736 2023-08-22 05:18:53.114750 zae_engine-0.1.3/zae_engine/nn_night/_layer.py
+-rw-r--r--   0        0        0     7702 2023-10-25 08:01:07.687937 zae_engine-0.1.3/zae_engine/nn_night/_module.py
+-rw-r--r--   0        0        0      337 2024-03-22 02:49:57.139750 zae_engine-0.1.3/zae_engine/operation/__init__.py
+-rw-r--r--   0        0        0      426 2024-03-22 09:38:38.514376 zae_engine-0.1.3/zae_engine/operation/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     8941 2024-02-06 07:49:16.726406 zae_engine-0.1.3/zae_engine/operation/__pycache__/_operation.cpython-310.pyc
+-rw-r--r--   0        0        0    10306 2024-02-06 01:49:00.433405 zae_engine-0.1.3/zae_engine/operation/_operation.py
+-rw-r--r--   0        0        0        0 2023-10-25 08:01:07.688932 zae_engine-0.1.3/zae_engine/scripts/__init__.py
+-rw-r--r--   0        0        0      145 2024-04-03 05:59:23.020824 zae_engine-0.1.3/zae_engine/scripts/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3390 2024-04-15 06:26:54.244400 zae_engine-0.1.3/zae_engine/scripts/__pycache__/example_script.cpython-310.pyc
+-rw-r--r--   0        0        0     3532 2024-03-22 09:50:36.415710 zae_engine-0.1.3/zae_engine/scripts/example_script.py
+-rw-r--r--   0        0        0       53 2023-08-22 05:18:53.119737 zae_engine-0.1.3/zae_engine/trainer/__init__.py
+-rw-r--r--   0        0        0      207 2023-10-13 05:01:18.404200 zae_engine-0.1.3/zae_engine/trainer/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    12867 2024-04-02 00:44:05.737349 zae_engine-0.1.3/zae_engine/trainer/__pycache__/_trainer.cpython-310.pyc
+-rw-r--r--   0        0        0     3828 2023-11-02 07:34:59.267084 zae_engine-0.1.3/zae_engine/trainer/__pycache__/mpu_utils.cpython-310.pyc
+-rw-r--r--   0        0        0    13307 2024-04-16 01:26:56.056447 zae_engine-0.1.3/zae_engine/trainer/_trainer.py
+-rw-r--r--   0        0        0     2963 2023-08-22 05:18:53.119737 zae_engine-0.1.3/zae_engine/trainer/mpu_utils.py
+-rw-r--r--   0        0        0       50 2023-08-22 05:18:53.119737 zae_engine-0.1.3/zae_engine/trainer/utils/__init__.py
+-rw-r--r--   0        0        0      196 2023-10-13 05:01:18.404200 zae_engine-0.1.3/zae_engine/trainer/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     5660 2023-10-13 05:01:18.404200 zae_engine-0.1.3/zae_engine/trainer/utils/__pycache__/_callback.cpython-310.pyc
+-rw-r--r--   0        0        0     2524 2024-03-22 09:37:31.411211 zae_engine-0.1.3/zae_engine/trainer/utils/__pycache__/_logger.cpython-310.pyc
+-rw-r--r--   0        0        0     5723 2023-08-22 05:18:53.119737 zae_engine-0.1.3/zae_engine/trainer/utils/_callback.py
+-rw-r--r--   0        0        0     2164 2024-03-22 02:49:57.140295 zae_engine-0.1.3/zae_engine/trainer/utils/_logger.py
+-rw-r--r--   0        0        0       19 2024-03-22 02:49:57.140295 zae_engine-0.1.3/zae_engine/utils/__init__.py
+-rw-r--r--   0        0        0      162 2024-03-22 09:38:39.332191 zae_engine-0.1.3/zae_engine/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      892 2024-03-22 09:38:39.332191 zae_engine-0.1.3/zae_engine/utils/__pycache__/io.cpython-310.pyc
+-rw-r--r--   0        0        0      727 2024-03-22 02:49:57.140295 zae_engine-0.1.3/zae_engine/utils/io.py
+-rw-r--r--   0        0        0     1868 1970-01-01 00:00:00.000000 zae_engine-0.1.3/PKG-INFO
```

### Comparing `zae_engine-0.1.2/pyproject.toml` & `zae_engine-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'zae-engine'
-version = '0.1.2'
+version = '0.1.3'
 description = 'Deep learning engine powered by zae-park.'
 authors = ["zae-park <tom941105@gmail.com>"]
 packages = [
     {include = "zae_engine", from='.'},
     {include = "zae_cli", from='.'},
 ]
 
@@ -36,36 +36,45 @@
 neurokit2 = "^0.2.6"
 nibabel = "^5.1.0"
 minio = "^7.1.17"
 pytest = "^7.4.2"
 pandas = "^2.1.2"
 openpyxl = "^3.1.2"
 #tf2onnx = { git = "https://github.com/onnx/tensorflow-onnx.git" }
-onnx = "1.14.1"
+#onnx = "1.14.1"
 click = "^8.1.7"
 pillow = "^10.1.0"
 wandb = "^0.16.2"
+genbadge = "^1.1.1"
+pytest-cov = "^5.0.0"
+codecov = "^2.1.13"
+sphinx = "^7.2.6"
+sphinx-rtd-theme = "^2.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
 python = ">=3.10.0,<3.12"
 pytest = "^7.4.2"
 torchvision = [
     { platform = "win32", url = "https://download.pytorch.org/whl/cu117/torchvision-0.15.1%2Bcu117-cp310-cp310-win_amd64.whl" },
     { platform = "linux", url = "https://download.pytorch.org/whl/cu117/torchvision-0.15.1%2Bcu117-cp310-cp310-linux_x86_64.whl" },
 ]
 torch = [
     { platform = "win32", url = "https://download.pytorch.org/whl/cu117/torch-2.0.0%2Bcu117-cp310-cp310-win_amd64.whl" },
     { platform = "linux", url = "https://download.pytorch.org/whl/cu117/torch-2.0.0%2Bcu117-cp310-cp310-linux_x86_64.whl" },
 ]
+coverage = "^7.4.4"
 
 [build-system]
 requires = ["poetry>=1.5"]
 build-backend = "poetry.masonry.api"
 
 [tool.black]
 line-length = 120
 target-version = ['py310']
 
 [tool.poetry.scripts]
 zae = "zae_cli.cli:cli_run"
-zae-test = "zae_cli.cli:zae_print"
+zae-test = "zae_cli.cli:zae_print"
+
+[tool.pydoc-markdown]
+
```

### Comparing `zae_engine-0.1.2/zae_cli/cli.py` & `zae_engine-0.1.3/zae_cli/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import shutil
 
 import click
 
-from .tree_builder import TreeBuilder
+from tree_builder import TreeBuilder
 
 
 # Package structure will be changed in the future.
 # zae_cli
 #   | ---- main
 #   | ---- tree - tree_builder.py
 #   | ---- example - generator.py example_script.py
@@ -24,25 +24,26 @@
 @click.option(
     "path",
     "-p",
     type=click.Path(exists=False),
     help="The destination path where example file will be created when the `example` command.",
 )
 def cli_run(command: str, path: str = ""):
-    print("CLI in cli dir")
     if command == "tree":
         TreeBuilder.print_tree(os.path.join(os.path.dirname(os.path.abspath(__file__)), "../zae_engine"))
+
     elif command == "example":
         if not path:
             path = os.path.join(os.getcwd(), "zae_example.py")
         shutil.copy(os.path.join(os.path.dirname(os.path.abspath(__file__)), "example_script.py"), path)
         print(f"Generate snippet file. {path} python")
     elif command == "hello":
         zae_print()
     else:
         print(f'Invalid command "{command}".')
 
 
-if __name__ == "__main__":
-    # python -m zae_cli.cli
-    print("module run")
-    cli_run(["snippet"])
+# if __name__ == "__main__":
+#     os.system("zae tree")
+# python -m zae_cli.cli
+# print("module run")
+# cli_run(["snippet"])
```

### Comparing `zae_engine-0.1.2/zae_cli/example_script.py` & `zae_engine-0.1.3/zae_cli/example_script.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,36 @@
+import os
+import datetime
 from collections import namedtuple
-import random
-import time
-import glob
-import torch
-import torch.nn as nn
-from torchvision.transforms import Resize
-from torch.utils.data import Dataset, DataLoader, ConcatDataset
-import torch.nn.functional as F
-from tqdm import tqdm
-import onnx
-import tf2onnx
 
-import os
+import numpy as np
 from sklearn.datasets import fetch_openml
 from sklearn.model_selection import train_test_split
-import numpy as np
-import matplotlib.pyplot as plt
-from glob import glob
-import tensorflow as tf
-from PIL import Image
-from tensorflow import keras
-from keras import layers
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+from torch.utils.data import Dataset, DataLoader
 
 from zae_engine import trainer, models, measure, data_pipeline
 from zae_engine.operation import draw_confusion_matrix, print_confusion_matrix
 
 
-class ExDataset(data.Dataset):
+class ExDataset(Dataset):
     def __init__(self, x, y, _type: type = tuple):
-        self.x = torch.tensor(x, dtype=torch.float32).unsqueeze(0)
-        self.y = torch.tensor(y, dtype=torch.float32)
+        self.x = torch.tensor(x.to_numpy().reshape(-1, 28, 28), dtype=torch.float32).unsqueeze(1)
+        self.y = torch.tensor(y.to_numpy(), dtype=torch.float32).unsqueeze(1)
+        self.eye = np.eye(len(y.unique()))
         self._type = _type
 
     def __len__(self):
         return len(self.x)
 
     def __getitem__(self, i):
         x, y = self.x[i], self.y[i]
+        y = self.eye[y.int()]
         if self._type == tuple:
             return (x, y)
         elif self._type == dict:
             return {"x": x, "y": y}
         elif self._type == namedtuple:
             return namedtuple("item", ["x", "y"])(x, y)
         else:
@@ -57,16 +47,16 @@
         depth: int = 3,
         order: int = 1,
         stride: list or tuple = (2, 2),
     ):
         super().__init__(
             ch_in=ch_in, ch_out=ch_out, width=width, kernel_size=kernel_size, depth=depth, order=order, stride=stride
         )
-        self.pool = nn.AdaptiveAvgPool2d(128)
-        self.head = nn.Linear(128, ch_out)
+        self.pool = nn.Sequential(nn.Flatten(), nn.AdaptiveAvgPool1d(32))
+        self.head = nn.Linear(32, ch_out)
 
     def forward(self, x):
         out = self.body(x)
         out = self.pool(out)
         return self.head(out)
 
 
@@ -75,46 +65,45 @@
         super(ExTrainer, self).__init__(model, device, mode, optimizer, scheduler)
 
     def train_step(self, batch):
         x, y = batch
         proba = self.model(x).softmax(1)
         predict = proba.argmax(1)
         loss = F.cross_entropy(proba, y)
-        return {"loss": loss, "output": predict, "acc": measure.accuracy(y.argmax(1), predict)}
+
+        acc = measure.accuracy(self._to_cpu(y.argmax(1)), self._to_cpu(predict))
+        return {"loss": loss, "output": predict, "acc": acc}
 
     def test_step(self, batch):
         return self.train_step(batch)
 
 
 def main():
     kickoff_time = datetime.datetime.now()
-    epochs = 100
+    epochs = 2
     batch_size = 32
     learning_rate = 1e-4
     device = torch.device(f"cuda:{0}" if torch.cuda.is_available() else "cpu")
 
     mnist = fetch_openml("mnist_784")
-    x, y = mnist.data, mnist.target
+    x, y = mnist.data, mnist.target.astype(int)
 
-    x_train, x, y_train, y = train_test_split(x, y, test_size=0.2, random_state=1111, stratify=True)
-    x_valid, x_test, y_valid, y_test = train_test_split(x, y, test_size=0.5, random_state=1111, stratify=True)
+    x_train, x, y_train, y = train_test_split(x, y, test_size=0.2, random_state=1111, stratify=y)
+    x_valid, x_test, y_valid, y_test = train_test_split(x, y, test_size=0.5, random_state=1111, stratify=y)
 
-    train_loader = data.DataLoader(dataset=ExDataset(x_train, y_train), batch_size=batch_size)
-    valid_loader = data.DataLoader(dataset=ExDataset(x_valid, y_valid), batch_size=batch_size * 2)
-    test_loader = data.DataLoader(dataset=ExDataset(x_test, y_test), batch_size=batch_size * 2)
+    train_loader = DataLoader(dataset=ExDataset(x_train, y_train), batch_size=batch_size)
+    valid_loader = DataLoader(dataset=ExDataset(x_valid, y_valid), batch_size=batch_size * 2)
+    test_loader = DataLoader(dataset=ExDataset(x_test, y_test), batch_size=batch_size * 2)
 
     model = ExModel()
     opt = torch.optim.Adam(params=model.parameters(), lr=learning_rate)
-    scheduler = torch.optim.lr_scheduler.LambdaLR(optimizer=opt, lr_lambda=epochs)
+    scheduler = torch.optim.lr_scheduler.LambdaLR(optimizer=opt, lr_lambda=lambda x: 0.9**epochs)
 
     trainer = ExTrainer(model, device=device, optimizer=opt, scheduler=scheduler)
 
-    if not os.path.exists(out_path):
-        os.mkdir(out_path)
-
     trainer.run(n_epoch=epochs, loader=train_loader, valid_loader=valid_loader)
 
     test_result = np.stack(trainer.inference(loader=test_loader))
     confusion_mat = draw_confusion_matrix(y_test, test_result, num_classes=10)
     print_confusion_matrix(confusion_mat)
 
     elapsed_time = datetime.datetime.now() - kickoff_time
```

### Comparing `zae_engine-0.1.2/zae_cli/io.py` & `zae_engine-0.1.3/zae_engine/utils/io.py`

 * *Files identical despite different names*

### Comparing `zae_engine-0.1.2/zae_cli/tree_builder.py` & `zae_engine-0.1.3/zae_cli/tree_builder.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,100 @@
 import os
+import ast
 import pathlib
+from collections import defaultdict
 from importlib import import_module
 from inspect import isclass, isfunction, isroutine, getmembers
 
 from rich import print
 from rich.filesize import decimal
 from rich.markup import escape
 from rich.text import Text
 from rich.tree import Tree
 
 
+def get_methods_from_abspath(abs_path):
+    with open(abs_path, "r", encoding="utf-8") as file:
+        tree = ast.parse(file.read(), filename=abs_path)
+
+    defined_methods_with_classes = defaultdict(list)
+    current_class = None
+
+    for node in ast.walk(tree):
+        if isinstance(node, ast.ClassDef):
+            current_class = node.name
+            defined_methods_with_classes[current_class] = []
+        elif isinstance(node, ast.FunctionDef):
+            # Check if the function is not a dunder
+            if node.name.startswith("__") or node.name.endswith("__") or "wrap" in node.name:
+                continue
+            # Check if the function is in a class
+            if current_class:
+                defined_methods_with_classes[current_class].append(node.name)
+            # Check if the function is standalone and not in a class
+            else:
+                defined_methods_with_classes["standalone"].append(node.name)
+
+    return defined_methods_with_classes
+
+
 class TreeBuilder:
-    START_IGNORE = ['.', '__', 'test']
+    START_IGNORE = [".", "__", "test"]
     _tree = None
 
     def __init__(self, root: str):
         self.tree = None
         self.set_tree(root)
         self.walk_in(pathlib.Path(root), self.tree)
 
     def set_tree(self, root):
-        self.tree = Tree(f":open_file_folder: [link file://{root}]{root}",
-                         guide_style="bold bright_blue")
+        self.tree = Tree(f":open_file_folder: [link file://{root}]{root}", guide_style="bold bright_blue")
 
     def walk_in(self, root, tree):
         paths = self.get_path(root)
         for path in paths:
             if self.is_valid(path):
                 if path.is_dir():
                     # if current path is directory, add branch to tree and walk in to.
                     branch = tree.add(
                         f"[bold magenta]:open_file_folder: [link file://{path}]{escape(path.name)}",
-                        style="", guide_style="")
+                        style="",
+                        guide_style="",
+                    )
                     self.walk_in(path, branch)
-                elif path.name.endswith('.py'):
+                elif path.name.endswith(".py"):
                     # if current path is script, add branch to tree and find routine.
                     branch = tree.add(
-                        f"[bold magenta]🐍 [link file://{path}]{escape(path.name)}",
-                        style="", guide_style="")
+                        f"[bold magenta]🐍 [link file://{path}]{escape(path.name)}", style="", guide_style=""
+                    )
 
-                    bag = getmembers(import_module(path.__str__().replace('\\', '.')[:-3]))
-                    for n, v in bag:
+                    print(path)
+                    # bag = getmembers(import_module(path.name[:-3]))
+                    bag = get_methods_from_abspath(str(path.resolve()))
+                    # bag = getmembers(import_module(path.__str__().replace("\\", ".")[:-3]))
+                    for n, v in bag.items():
                         if os.path.splitext(n)[-1]:
                             self.add_leaf(path.name, branch)
                         else:
-                            if isroutine(v):
-                                if isfunction(v):
-                                    self.add_leaf(n, branch, icon='📄 ')
-                                    # self.add_leaf(n, branch, icon='⬛ ')
-                            elif isclass(v):
-                                    self.add_leaf(n, branch, icon='📘 ')
-                                    # self.add_leaf(n, branch, icon='◼ ')
+                            if n == "standalone":
+                                for func_name in v:
+                                    self.add_leaf(func_name, branch, icon="📄 ")
                             else:
-                                pass
+                                # for cls_name in v:
+                                self.add_leaf(n, branch, icon="📘 ")
+
+                            # if isroutine(v):
+                            #     if isfunction(v):
+                            #         self.add_leaf(n, branch, icon="📘 ")
+                            #         # self.add_leaf(n, branch, icon='⬛ ')
+                            # elif isclass(v):
+                            #     self.add_leaf(n, branch, icon="📘 ")
+                            #     # self.add_leaf(n, branch, icon='◼ ')
+                            # else:
+                            #     pass
 
     def add_branch(self, path, branch):
         text_filename = Text(path.name, "green")
         text_filename.highlight_regex(r"\..*$", "bold red")
         text_filename.stylize(f"link file://{path}")
         file_size = path.stat().st_size
         text_filename.append(f" ({decimal(file_size)})", "blue")
@@ -85,11 +123,10 @@
     @classmethod
     def print_tree(cls, path):
         if cls._tree is None:
             cls._tree = cls(path)
         print(cls._tree.tree)
 
 
-if __name__ == '__main__':
-    TreeBuilder.print_tree('./zae_engine')
-
-
+if __name__ == "__main__":
+    # res = get_methods_from_abspath("Z:\\dev-zae\\zae-engine\\zae_cli\\../zae_engine\\data_pipeline\\collate.py")
+    TreeBuilder.print_tree("../zae_engine")
```

### Comparing `zae_engine-0.1.2/zae_engine/data_pipeline/__pycache__/_fileio.cpython-310.pyc` & `zae_engine-0.1.3/zae_engine/data_pipeline/__pycache__/_fileio.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zae_engine-0.1.2/zae_engine/data_pipeline/__pycache__/collate.cpython-310.pyc` & `zae_engine-0.1.3/zae_engine/data_pipeline/__pycache__/collate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Feb  6 02:01:08 2024 UTC, .py size: 7678 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 e492 c165 fe1d 0000  o..........e....
+00000000: 6f0d 0d0a 0000 0000 d5f1 fc65 fe1d 0000  o..........e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6400 6402 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 6d07 5a07 0100 6400 6403 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6404 6c0a 6d0b 5a0b 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6405 6c0c 5a0d 6400 6406 6c0e 6d0f 5a0f  d.l.Z.d.d.l.m.Z.
```

### Comparing `zae_engine-0.1.2/zae_engine/data_pipeline/_fileio.py` & `zae_engine-0.1.3/zae_engine/data_pipeline/_fileio.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         If this parameter is not specified, run for 10 second data.
     :return:
         If beat_idx was given, return recording, r-peak index, and beat type for beat_idx'th beat.
         If not, return recording, label sequence for 10 sec data.
     """
     lookup = {"N": 1, "A": 2}
 
-    ex_path = os.path.join(os.path.dirname(__file__), "resource/sample_data")
+    ex_path = os.path.join(os.path.dirname(__file__), "sample/sample_data")
     recording = wfdb.rdsamp(ex_path, return_res=32)[0].squeeze()  # nd-array, [2500, ]
     anno = wfdb.rdann(ex_path, "zae")
     samp, sym = anno.sample.tolist(), anno.symbol
     if sym[0] != "*":
         samp.insert(0, 0)
         sym.insert(0, "*")
     if sym[-1] != "*":
```

### Comparing `zae_engine-0.1.2/zae_engine/data_pipeline/collate.py` & `zae_engine-0.1.3/zae_engine/data_pipeline/collate.py`

 * *Files identical despite different names*

### Comparing `zae_engine-0.1.2/zae_engine/data_pipeline/resource/sample_data.dat` & `zae_engine-0.1.3/zae_engine/data_pipeline/__sample/sample_data.dat`

 * *Files identical despite different names*

### Comparing `zae_engine-0.1.2/zae_engine/inference/__pycache__/beat.cpython-310.pyc` & `zae_engine-0.1.3/zae_engine/inference/__pycache__/beat.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Feb  6 02:01:08 2024 UTC, .py size: 3165 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 e492 c165 5d0c 0000  o..........e]...
+00000000: 6f0d 0d0a 0000 0000 d5f1 fc65 5d0c 0000  o..........e]...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6403 6c07 5a08 6400 6403 6c09  ..d.d.l.Z.d.d.l.
 00000060: 5a09 6400 6404 6c0a 6d0b 5a0b 6d0c 5a0c  Z.d.d.l.m.Z.m.Z.
 00000070: 0100 6400 6405 6c0d 6d0e 5a0e 6d0f 5a0f  ..d.d.l.m.Z.m.Z.
@@ -52,29 +52,29 @@
 00000330: 7429 03da 056d 6f64 656c da06 6465 7669  t)...model..devi
 00000340: 6365 da04 6d6f 6465 4e29 12da 036c 656e  ce..modeN)...len
 00000350: da05 7368 6170 65da 0574 6f72 6368 7217  ..shape..torchr.
 00000360: 0000 00da 0463 7564 61da 0c69 735f 6176  .....cuda..is_av
 00000370: 6169 6c61 626c 65da 0b45 4347 5f64 6174  ailable..ECG_dat
 00000380: 6173 6574 da07 7265 7368 6170 6572 0800  aset..reshaper..
 00000390: 0000 da03 436f 6cda 0477 7261 7072 0900  ....Col..wrapr..
-000003a0: 0000 da11 6265 6174 5f73 6567 6d65 6e74  ....beat_segment
+000003a0: 0000 5a11 6265 6174 5f73 6567 6d65 6e74  ..Z.beat_segment
 000003b0: 6174 696f 6eda 0c54 7261 696e 6572 5f73  ation..Trainer_s
 000003c0: 7467 31da 026e 70da 0b63 6f6e 6361 7465  tg1..np..concate
 000003d0: 6e61 7465 da09 696e 6665 7265 6e63 65da  nate..inference.
 000003e0: 0661 7267 6d61 7829 0672 0c00 0000 7217  .argmax).r....r.
 000003f0: 0000 005a 1169 6e66 6572 656e 6365 5f64  ...Z.inference_d
 00000400: 6174 6173 6574 5a10 696e 6665 7265 6e63  atasetZ.inferenc
 00000410: 655f 6c6f 6164 6572 7216 0000 005a 0874  e_loaderr....Z.t
-00000420: 7261 696e 6572 31a9 0072 2800 0000 fa32  rainer1..r(....2
+00000420: 7261 696e 6572 31a9 0072 2700 0000 fa32  rainer1..r'....2
 00000430: 5a3a 5c64 6576 2d7a 6165 5c7a 6165 2d65  Z:\dev-zae\zae-e
 00000440: 6e67 696e 655c 7a61 655f 656e 6769 6e65  ngine\zae_engine
 00000450: 5c69 6e66 6572 656e 6365 5c62 6561 742e  \inference\beat.
 00000460: 7079 da04 636f 7265 0c00 0000 7312 0000  py..core....s...
 00000470: 0024 0618 0112 0102 0114 0106 ff0a 050e  .$..............
-00000480: 0116 0172 2a00 0000 6300 0000 0000 0000  ...r*...c.......
+00000480: 0116 0172 2900 0000 6300 0000 0000 0000  ...r)...c.......
 00000490: 0000 0000 0000 0000 0002 0000 0040 0000  .............@..
 000004a0: 0073 2c00 0000 6500 5a01 6400 5a02 6401  .s,...e.Z.d.Z.d.
 000004b0: 6402 8400 5a03 6403 6404 8400 5a04 6405  d...Z.d.d...Z.d.
 000004c0: 6406 8400 5a05 6407 6408 8400 5a06 6409  d...Z.d.d...Z.d.
 000004d0: 5300 290a 721e 0000 0063 0100 0000 0000  S.).r....c......
 000004e0: 0000 0000 0000 0200 0000 0400 0000 4b00  ..............K.
 000004f0: 0000 73d2 0000 007c 017c 005f 0074 016a  ..s....|.|._.t.j
@@ -94,142 +94,142 @@
 000005d0: 00a9 01da 0564 7479 7065 da01 79da 0266  .....dtype..y..f
 000005e0: 6eda 0272 70da 056f 6e6f 6666 7218 0000  n..rp..onoffr...
 000005f0: 00da 007a 0709 2023 206f 6620 7a12 2064  ...z.. # of z. d
 00000600: 6174 615f 7069 7065 6c69 6e65 3a20 2564  ata_pipeline: %d
 00000610: 290f da06 6b77 6172 6773 721b 0000 00da  )...kwargsr.....
 00000620: 0674 656e 736f 72da 0766 6c6f 6174 3332  .tensor..float32
 00000630: 720c 0000 00da 0461 7474 72da 046c 6f6e  r......attr..lon
-00000640: 6772 2d00 0000 722e 0000 0072 2f00 0000  gr-...r....r/...
-00000650: 7230 0000 00da 046b 6579 7372 1800 0000  r0.....keysr....
+00000640: 6772 2c00 0000 722d 0000 0072 2e00 0000  gr,...r-...r....
+00000650: 722f 0000 00da 046b 6579 7372 1800 0000  r/.....keysr....
 00000660: da05 7072 696e 7472 1900 0000 2902 da04  ..printr....)...
-00000670: 7365 6c66 7232 0000 0072 2800 0000 7228  selfr2...r(...r(
-00000680: 0000 0072 2900 0000 da08 5f5f 696e 6974  ...r).....__init
+00000670: 7365 6c66 7231 0000 0072 2700 0000 7227  selfr1...r'...r'
+00000680: 0000 0072 2800 0000 da08 5f5f 696e 6974  ...r(.....__init
 00000690: 5f5f 2100 0000 7310 0000 0006 0116 0128  __!...s........(
 000006a0: 011c 011c 011c 011a 0220 017a 1445 4347  ......... .z.ECG
 000006b0: 5f64 6174 6173 6574 2e5f 5f69 6e69 745f  _dataset.__init_
 000006c0: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
 000006d0: 0000 0200 0000 4300 0000 730a 0000 0074  ......C...s....t
 000006e0: 007c 006a 0183 0153 00a9 014e 2902 7219  .|.j...S...N).r.
-000006f0: 0000 0072 0c00 0000 a901 7239 0000 0072  ...r......r9...r
-00000700: 2800 0000 7228 0000 0072 2900 0000 da07  (...r(...r).....
+000006f0: 0000 0072 0c00 0000 a901 7238 0000 0072  ...r......r8...r
+00000700: 2700 0000 7227 0000 0072 2800 0000 da07  '...r'...r(.....
 00000710: 5f5f 6c65 6e5f 5f2c 0000 0073 0200 0000  __len__,...s....
 00000720: 0a01 7a13 4543 475f 6461 7461 7365 742e  ..z.ECG_dataset.
 00000730: 5f5f 6c65 6e5f 5f63 0200 0000 0000 0000  __len__c........
 00000740: 0000 0000 0200 0000 0300 0000 4300 0000  ............C...
 00000750: 731c 0000 007c 017c 006a 00a0 01a1 0076  s....|.|.j.....v
 00000760: 0072 0c7c 006a 007c 0119 0053 0064 0053  .r.|.j.|...S.d.S
-00000770: 0072 3b00 0000 2902 7232 0000 0072 3700  .r;...).r2...r7.
-00000780: 0000 2902 7239 0000 00da 0876 6172 5f6e  ..).r9.....var_n
-00000790: 616d 6572 2800 0000 7228 0000 0072 2900  amer(...r(...r).
-000007a0: 0000 7235 0000 002f 0000 0073 0600 0000  ..r5.../...s....
+00000770: 0072 3a00 0000 2902 7231 0000 0072 3600  .r:...).r1...r6.
+00000780: 0000 2902 7238 0000 00da 0876 6172 5f6e  ..).r8.....var_n
+00000790: 616d 6572 2700 0000 7227 0000 0072 2800  amer'...r'...r(.
+000007a0: 0000 7234 0000 002f 0000 0073 0600 0000  ..r4.../...s....
 000007b0: 0e01 0a01 04ff 7a10 4543 475f 6461 7461  ......z.ECG_data
 000007c0: 7365 742e 6174 7472 6302 0000 0000 0000  set.attrc.......
 000007d0: 0000 0000 0003 0000 0004 0000 0043 0000  .............C..
 000007e0: 0073 a400 0000 7400 6400 8301 7d02 7c00  .s....t.d...}.|.
 000007f0: 6a01 7c01 1900 a002 6401 a101 7c02 6402  j.|.....d...|.d.
 00000800: 3c00 7c00 6a03 6400 7501 721b 7c00 6a03  <.|.j.d.u.r.|.j.
 00000810: 7c01 1900 a002 6401 a101 6e01 6400 7c02  |.....d...n.d.|.
 00000820: 6403 3c00 7c00 6a04 6400 7501 7229 7c00  d.<.|.j.d.u.r)|.
 00000830: 6a04 7c01 1900 6e01 6400 7c02 6404 3c00  j.|...n.d.|.d.<.
 00000840: 7c00 6a05 6400 7501 723f 7406 6a07 7c00  |.j.d.u.r?t.j.|.
 00000850: 6a05 7c01 1900 7406 6a08 6405 8d02 7c02  j.|...t.j.d...|.
 00000860: 6406 3c00 7c00 6a09 7250 7c00 6a09 6400  d.<.|.j.rP|.j.d.
 00000870: 7501 724c 7c00 6a09 7c01 1900 6e01 6400  u.rL|.j.|...n.d.
 00000880: 7c02 6407 3c00 7c02 5300 2908 4e72 0100  |.d.<.|.S.).Nr..
-00000890: 0000 720c 0000 0072 2d00 0000 722e 0000  ..r....r-...r...
-000008a0: 0072 2b00 0000 722f 0000 0072 3000 0000  .r+...r/...r0...
+00000890: 0000 720c 0000 0072 2c00 0000 722d 0000  ..r....r,...r-..
+000008a0: 0072 2a00 0000 722e 0000 0072 2f00 0000  .r*...r....r/...
 000008b0: 290a 7202 0000 0072 0c00 0000 da09 756e  ).r....r......un
-000008c0: 7371 7565 657a 6572 2d00 0000 722e 0000  squeezer-...r...
-000008d0: 0072 2f00 0000 721b 0000 0072 3300 0000  .r/...r....r3...
-000008e0: 7236 0000 0072 3000 0000 2903 7239 0000  r6...r0...).r9..
+000008c0: 7371 7565 657a 6572 2c00 0000 722d 0000  squeezer,...r-..
+000008d0: 0072 2e00 0000 721b 0000 0072 3200 0000  .r....r....r2...
+000008e0: 7235 0000 0072 2f00 0000 2903 7238 0000  r5...r/...).r8..
 000008f0: 00da 0369 6478 5a0a 6261 7463 685f 6469  ...idxZ.batch_di
-00000900: 6374 7228 0000 0072 2800 0000 7229 0000  ctr(...r(...r)..
+00000900: 6374 7227 0000 0072 2700 0000 7228 0000  ctr'...r'...r(..
 00000910: 00da 0b5f 5f67 6574 6974 656d 5f5f 3300  ...__getitem__3.
 00000920: 0000 7312 0000 0008 0114 0122 011c 010a  ..s........"....
 00000930: 011a 0106 011c 0104 017a 1745 4347 5f64  .........z.ECG_d
 00000940: 6174 6173 6574 2e5f 5f67 6574 6974 656d  ataset.__getitem
 00000950: 5f5f 4e29 07da 085f 5f6e 616d 655f 5fda  __N)...__name__.
 00000960: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-00000970: 7561 6c6e 616d 655f 5f72 3a00 0000 723d  ualname__r:...r=
-00000980: 0000 0072 3500 0000 7241 0000 0072 2800  ...r5...rA...r(.
-00000990: 0000 7228 0000 0072 2800 0000 7229 0000  ..r(...r(...r)..
+00000970: 7561 6c6e 616d 655f 5f72 3900 0000 723c  ualname__r9...r<
+00000980: 0000 0072 3400 0000 7240 0000 0072 2700  ...r4...r@...r'.
+00000990: 0000 7227 0000 0072 2700 0000 7228 0000  ..r'...r'...r(..
 000009a0: 0072 1e00 0000 2000 0000 730a 0000 0008  .r.... ...s.....
 000009b0: 0008 0108 0b08 030c 0472 1e00 0000 6300  .........r....c.
 000009c0: 0000 0000 0000 0000 0000 0000 0000 0005  ................
 000009d0: 0000 0000 0000 0073 4800 0000 6500 5a01  .......sH...e.Z.
 000009e0: 6400 5a02 640b 6402 6503 6403 6504 6a05  d.Z.d.d.e.d.e.j.
 000009f0: 6a06 6604 8700 6601 6404 6405 840d 5a07  j.f...f.d.d...Z.
 00000a00: 6406 6508 6602 6407 6408 8404 5a09 6406  d.e.f.d.d...Z.d.
 00000a10: 6508 6602 6409 640a 8404 5a0a 8700 0400  e.f.d.d...Z.....
-00000a20: 5a0b 5300 290c 7223 0000 004e 7218 0000  Z.S.).r#...Nr...
+00000a20: 5a0b 5300 290c 7222 0000 004e 7218 0000  Z.S.).r"...Nr...
 00000a30: 00da 096f 7074 696d 697a 6572 6306 0000  ...optimizerc...
 00000a40: 0000 0000 0000 0000 0006 0000 0007 0000  ................
 00000a50: 0003 0000 0073 2200 0000 7400 7401 7c00  .....s"...t.t.|.
 00000a60: 8302 a002 7c01 7c02 7c03 7c04 7c05 a105  ....|.|.|.|.|...
 00000a70: 0100 6401 7c00 5f03 6400 5300 2902 4ee9  ..d.|._.d.S.).N.
-00000a80: 2000 0000 2904 da05 7375 7065 7272 2300   ...)...superr#.
-00000a90: 0000 723a 0000 00da 0f6d 696e 695f 6261  ..r:.....mini_ba
-00000aa0: 7463 685f 7369 7a65 2906 7239 0000 0072  tch_size).r9...r
-00000ab0: 1600 0000 7217 0000 0072 1800 0000 7245  ....r....r....rE
+00000a80: 2000 0000 2904 da05 7375 7065 7272 2200   ...)...superr".
+00000a90: 0000 7239 0000 00da 0f6d 696e 695f 6261  ..r9.....mini_ba
+00000aa0: 7463 685f 7369 7a65 2906 7238 0000 0072  tch_size).r8...r
+00000ab0: 1600 0000 7217 0000 0072 1800 0000 7244  ....r....r....rD
 00000ac0: 0000 00da 0973 6368 6564 756c 6572 a901  .....scheduler..
-00000ad0: da09 5f5f 636c 6173 735f 5f72 2800 0000  ..__class__r(...
-00000ae0: 7229 0000 0072 3a00 0000 4000 0000 7304  r)...r:...@...s.
+00000ad0: da09 5f5f 636c 6173 735f 5f72 2700 0000  ..__class__r'...
+00000ae0: 7228 0000 0072 3900 0000 4000 0000 7304  r(...r9...@...s.
 00000af0: 0000 0018 010a 017a 1554 7261 696e 6572  .......z.Trainer
 00000b00: 5f73 7467 312e 5f5f 696e 6974 5f5f da05  _stg1.__init__..
 00000b10: 6261 7463 6863 0200 0000 0000 0000 0000  batchc..........
 00000b20: 0000 0200 0000 0100 0000 4300 0000 7304  ..........C...s.
-00000b30: 0000 0064 0053 0072 3b00 0000 7228 0000  ...d.S.r;...r(..
-00000b40: 0029 0272 3900 0000 724c 0000 0072 2800  .).r9...rL...r(.
-00000b50: 0000 7228 0000 0072 2900 0000 da0a 7472  ..r(...r).....tr
+00000b30: 0000 0064 0053 0072 3a00 0000 7227 0000  ...d.S.r:...r'..
+00000b40: 0029 0272 3800 0000 724b 0000 0072 2700  .).r8...rK...r'.
+00000b50: 0000 7227 0000 0072 2800 0000 da0a 7472  ..r'...r(.....tr
 00000b60: 6169 6e5f 7374 6570 4400 0000 7302 0000  ain_stepD...s...
 00000b70: 0004 017a 1754 7261 696e 6572 5f73 7467  ...z.Trainer_stg
 00000b80: 312e 7472 6169 6e5f 7374 6570 6302 0000  1.train_stepc...
 00000b90: 0000 0000 0000 0000 0005 0000 0005 0000  ................
 00000ba0: 0003 0000 0073 3a00 0000 7c01 6401 1900  .....s:...|.d...
 00000bb0: 7d02 7c02 6a00 8800 6a01 6402 6403 8d02  }.|.j...j.d.d...
 00000bc0: 7d03 7402 a003 8700 6601 6404 6405 8408  }.t.....f.d.d...
 00000bd0: 7c03 4400 8301 a101 7d04 6402 7c04 6406  |.D.....}.d.|.d.
 00000be0: 9c02 5300 2907 4e72 0c00 0000 7201 0000  ..S.).Nr....r...
 00000bf0: 0029 01da 0364 696d 6301 0000 0000 0000  .)...dimc.......
 00000c00: 0000 0000 0002 0000 0005 0000 0013 0000  ................
 00000c10: 0073 1600 0000 6700 7c00 5d07 7d01 8800  .s....g.|.].}...
-00000c20: a000 7c01 a101 9102 7102 5300 7228 0000  ..|.....q.S.r(..
+00000c20: a000 7c01 a101 9102 7102 5300 7227 0000  ..|.....q.S.r'..
 00000c30: 0029 0172 1600 0000 2902 da02 2e30 5a03  .).r....)....0Z.
-00000c40: 6d5f 7872 3c00 0000 7228 0000 0072 2900  m_xr<...r(...r).
+00000c40: 6d5f 7872 3b00 0000 7227 0000 0072 2800  m_xr;...r'...r(.
 00000c50: 0000 da0a 3c6c 6973 7463 6f6d 703e 4a00  ....<listcomp>J.
 00000c60: 0000 7302 0000 0016 007a 2a54 7261 696e  ..s......z*Train
 00000c70: 6572 5f73 7467 312e 7465 7374 5f73 7465  er_stg1.test_ste
 00000c80: 702e 3c6c 6f63 616c 733e 2e3c 6c69 7374  p.<locals>.<list
 00000c90: 636f 6d70 3e29 02da 046c 6f73 73da 066f  comp>)...loss..o
-00000ca0: 7574 7075 7429 0472 1000 0000 7248 0000  utput).r....rH..
-00000cb0: 0072 1b00 0000 da03 6361 7429 0572 3900  .r......cat).r9.
-00000cc0: 0000 724c 0000 0072 0c00 0000 5a06 6d69  ..rL...r....Z.mi
-00000cd0: 6e69 5f78 da03 6f75 7472 2800 0000 723c  ni_x..outr(...r<
-00000ce0: 0000 0072 2900 0000 da09 7465 7374 5f73  ...r).....test_s
+00000ca0: 7574 7075 7429 0472 1000 0000 7247 0000  utput).r....rG..
+00000cb0: 0072 1b00 0000 da03 6361 7429 0572 3800  .r......cat).r8.
+00000cc0: 0000 724b 0000 0072 0c00 0000 5a06 6d69  ..rK...r....Z.mi
+00000cd0: 6e69 5f78 da03 6f75 7472 2700 0000 723b  ni_x..outr'...r;
+00000ce0: 0000 0072 2800 0000 da09 7465 7374 5f73  ...r(.....test_s
 00000cf0: 7465 7047 0000 0073 0800 0000 0801 1001  tepG...s........
 00000d00: 1801 0a01 7a16 5472 6169 6e65 725f 7374  ....z.Trainer_st
 00000d10: 6731 2e74 6573 745f 7374 6570 2902 4e4e  g1.test_step).NN
-00000d20: 290c 7242 0000 0072 4300 0000 7244 0000  ).rB...rC...rD..
+00000d20: 290c 7241 0000 0072 4200 0000 7243 0000  ).rA...rB...rC..
 00000d30: 00da 0373 7472 721b 0000 00da 056f 7074  ...strr......opt
-00000d40: 696d da09 4f70 7469 6d69 7a65 7272 3a00  im..Optimizerr:.
-00000d50: 0000 da04 6469 6374 724d 0000 0072 5500  ....dictrM...rU.
+00000d40: 696d da09 4f70 7469 6d69 7a65 7272 3900  im..Optimizerr9.
+00000d50: 0000 da04 6469 6374 724c 0000 0072 5400  ....dictrL...rT.
 00000d60: 0000 da0d 5f5f 636c 6173 7363 656c 6c5f  ....__classcell_
-00000d70: 5f72 2800 0000 7228 0000 0072 4a00 0000  _r(...r(...rJ...
-00000d80: 7229 0000 0072 2300 0000 3f00 0000 7308  r)...r#...?...s.
-00000d90: 0000 0008 001c 010e 0416 0372 2300 0000  ...........r#...
+00000d70: 5f72 2700 0000 7227 0000 0072 4900 0000  _r'...r'...rI...
+00000d80: 7228 0000 0072 2200 0000 3f00 0000 7308  r(...r"...?...s.
+00000d90: 0000 0008 001c 010e 0416 0372 2200 0000  ...........r"...
 00000da0: 2919 da0b 636f 6c6c 6563 7469 6f6e 7372  )...collectionsr
 00000db0: 0200 0000 da06 7479 7069 6e67 7203 0000  ......typingr...
 00000dc0: 0072 0400 0000 7205 0000 0072 0600 0000  .r....r....r....
-00000dd0: da05 6e75 6d70 7972 2400 0000 721b 0000  ..numpyr$...r...
+00000dd0: da05 6e75 6d70 7972 2300 0000 721b 0000  ..numpyr#...r...
 00000de0: 00da 1074 6f72 6368 2e75 7469 6c73 2e64  ...torch.utils.d
-00000df0: 6174 6172 0700 0000 7208 0000 005a 0a7a  atar....r....Z.z
+00000df0: 6174 6172 0700 0000 7208 0000 00da 0a7a  atar....r......z
 00000e00: 6165 5f65 6e67 696e 6572 0900 0000 720a  ae_enginer....r.
 00000e10: 0000 005a 207a 6165 5f65 6e67 696e 652e  ...Z zae_engine.
 00000e20: 6461 7461 5f70 6970 656c 696e 652e 636f  data_pipeline.co
 00000e30: 6c6c 6174 6572 0b00 0000 7220 0000 00da  llater....r ....
 00000e40: 076e 6461 7272 6179 da06 5465 6e73 6f72  .ndarray..Tensor
-00000e50: 722a 0000 0072 1e00 0000 da07 5472 6169  r*...r......Trai
-00000e60: 6e65 7272 2300 0000 7228 0000 0072 2800  nerr#...r(...r(.
-00000e70: 0000 7228 0000 0072 2900 0000 da08 3c6d  ..r(...r).....<m
+00000e50: 7229 0000 0072 1e00 0000 da07 5472 6169  r)...r......Trai
+00000e60: 6e65 7272 2200 0000 7227 0000 0072 2700  nerr"...r'...r'.
+00000e70: 0000 7227 0000 0072 2800 0000 da08 3c6d  ..r'...r(.....<m
 00000e80: 6f64 756c 653e 0100 0000 7314 0000 000c  odule>....s.....
 00000e90: 0018 0108 0208 0110 0110 020c 011a 0310  ................
 00000ea0: 1416 1f                                  ...
```

### Comparing `zae_engine-0.1.2/zae_engine/inference/__pycache__/sec10.cpython-310.pyc` & `zae_engine-0.1.3/zae_engine/inference/__pycache__/sec10.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Feb  6 02:01:08 2024 UTC, .py size: 5404 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 e492 c165 1c15 0000  o..........e....
+00000000: 6f0d 0d0a 0000 0000 d5f1 fc65 1c15 0000  o..........e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 fe00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 0100 6400 6403 6c09  m.Z.m.Z...d.d.l.
 00000060: 5a0a 6400 6403 6c0b 5a0b 6400 6404 6c0c  Z.d.d.l.Z.d.d.l.
 00000070: 6d0d 5a0e 0100 6400 6405 6c0f 6d10 5a10  m.Z...d.d.l.m.Z.
@@ -55,127 +55,127 @@
 00000360: 746f 7263 68da 0664 6576 6963 65da 0463  torch..device..c
 00000370: 7564 61da 0c69 735f 6176 6169 6c61 626c  uda..is_availabl
 00000380: 65da 0c53 6563 3130 5472 6169 6e65 72da  e..Sec10Trainer.
 00000390: 0969 6e66 6572 656e 6365 da02 6e70 da0b  .inference..np..
 000003a0: 636f 6e63 6174 656e 6174 65da 086c 6f67  concatenate..log
 000003b0: 5f74 6573 74da 0772 6573 6861 7065 2909  _test..reshape).
 000003c0: 720f 0000 0072 1000 0000 da07 636f 6c6c  r....r......coll
-000003d0: 6174 6572 1200 0000 5a0a 6578 5f6c 6f61  ater....Z.ex_loa
+000003d0: 6174 6572 1200 0000 da0a 6578 5f6c 6f61  ater......ex_loa
 000003e0: 6465 7231 da05 6d6f 6465 6c72 2300 0000  der1..modelr#...
 000003f0: da07 7472 6169 6e65 72da 0672 6573 756c  ..trainer..resul
-00000400: 74a9 0072 3000 0000 fa33 5a3a 5c64 6576  t..r0....3Z:\dev
+00000400: 74a9 0072 3100 0000 fa33 5a3a 5c64 6576  t..r1....3Z:\dev
 00000410: 2d7a 6165 5c7a 6165 2d65 6e67 696e 655c  -zae\zae-engine\
 00000420: 7a61 655f 656e 6769 6e65 5c69 6e66 6572  zae_engine\infer
 00000430: 656e 6365 5c73 6563 3130 2e70 79da 0463  ence\sec10.py..c
 00000440: 6f72 650f 0000 0073 1600 0000 2401 0601  ore....s....$...
 00000450: 0802 1401 1002 1801 0c01 0a01 1002 1001  ................
-00000460: 0401 7232 0000 00da 0862 616e 6470 6173  ..r2.....bandpas
+00000460: 0401 7233 0000 00da 0862 616e 6470 6173  ..r3.....bandpas
 00000470: 73da 0b73 616d 706c 655f 7261 7465 da05  s..sample_rate..
 00000480: 6274 7970 6563 0300 0000 0000 0000 0000  btypec..........
 00000490: 0000 0400 0000 0700 0000 4300 0000 7374  ..........C...st
 000004a0: 0000 007c 0164 0114 007d 037c 0264 026b  ...|.d...}.|.d.k
 000004b0: 0272 1e74 006a 0167 0074 006a 0264 0364  .r.t.j.g.t.j.d.d
 000004c0: 017c 031b 0064 047c 031b 0067 027c 0264  .|...d.|...g.|.d
 000004d0: 058d 03a2 017c 0091 0152 008e 007d 007c  .....|...R...}.|
 000004e0: 0264 066b 0272 3874 006a 0167 0074 006a  .d.k.r8t.j.g.t.j
 000004f0: 0264 0364 077c 031b 0064 087c 031b 0067  .d.d.|...d.|...g
 00000500: 027c 0264 058d 03a2 017c 0091 0152 008e  .|.d.....|...R..
 00000510: 007d 007c 0053 0029 0a7a 1166 696c 7465  .}.|.S.).z.filte
 00000520: 7220 6563 6720 7369 676e 616c e700 0000  r ecg signal....
-00000530: 0000 00e0 3f72 3300 0000 7218 0000 00e9  ....?r3...r.....
-00000540: 3200 0000 a901 7235 0000 00da 0862 616e  2.....r5.....ban
+00000530: 0000 00e0 3f72 3400 0000 7218 0000 00e9  ....?r4...r.....
+00000540: 3200 0000 a901 7236 0000 00da 0862 616e  2.....r6.....ban
 00000550: 6473 746f 7067 3333 3333 33f3 4d40 67cd  dstopg33333.M@g.
 00000560: cccc cccc 0c4e 404e 2903 da03 7369 67da  .....N@N)...sig.
 00000570: 0866 696c 7466 696c 74da 0662 7574 7465  .filtfilt..butte
-00000580: 7229 0472 0f00 0000 7234 0000 0072 3500  r).r....r4...r5.
-00000590: 0000 da03 6e79 7172 3000 0000 7230 0000  ....nyqr0...r0..
-000005a0: 0072 3100 0000 da0d 6669 6c74 6572 5f73  .r1.....filter_s
+00000580: 7229 0472 0f00 0000 7235 0000 0072 3600  r).r....r5...r6.
+00000590: 0000 da03 6e79 7172 3100 0000 7231 0000  ....nyqr1...r1..
+000005a0: 0072 3200 0000 da0d 6669 6c74 6572 5f73  .r2.....filter_s
 000005b0: 6967 6e61 6c20 0000 0073 0c00 0000 0802  ignal ...s......
-000005c0: 0801 2c01 0801 2c01 0401 723e 0000 0063  ..,...,...r>...c
+000005c0: 0801 2c01 0801 2c01 0401 723f 0000 0063  ..,...,...r?...c
 000005d0: 0100 0000 0000 0000 0000 0000 0400 0000  ................
 000005e0: 0700 0000 4300 0000 7354 0000 0074 0083  ....C...sT...t..
 000005f0: 007d 0167 007d 027c 0044 005d 1b7d 037c  .}.g.}.|.D.].}.|
 00000600: 01a0 0174 02a0 037c 0364 01a1 02a1 0101  ...t...|.d......
 00000610: 007c 01a0 0474 02a0 037c 0364 01a1 02a1  .|...t...|.d....
 00000620: 01a0 05a1 007d 037c 02a0 067c 03a1 0101  .....}.|...|....
 00000630: 0071 0774 02a0 077c 02a1 017d 007c 0053  .q.t...|...}.|.S
 00000640: 0029 024e 7215 0000 0029 0872 0a00 0000  .).Nr....).r....
 00000650: da03 6669 7472 2800 0000 da0b 6578 7061  ..fitr(.....expa
 00000660: 6e64 5f64 696d 73da 0974 7261 6e73 666f  nd_dims..transfo
 00000670: 726d da07 7371 7565 657a 65da 0661 7070  rm..squeeze..app
 00000680: 656e 64da 0561 7272 6179 2904 720f 0000  end..array).r...
 00000690: 00da 0673 6361 6c65 72da 0562 6174 6368  ...scaler..batch
-000006a0: 5a08 7375 6273 6574 5f78 7230 0000 0072  Z.subset_xr0...r
-000006b0: 3000 0000 7231 0000 00da 0c73 6361 6c65  0...r1.....scale
+000006a0: 5a08 7375 6273 6574 5f78 7231 0000 0072  Z.subset_xr1...r
+000006b0: 3100 0000 7232 0000 00da 0c73 6361 6c65  1...r2.....scale
 000006c0: 5f73 6967 6e61 6c2a 0000 0073 1000 0000  _signal*...s....
 000006d0: 0601 0401 0801 1201 1601 0c01 0a01 0401  ................
-000006e0: 7247 0000 0063 0000 0000 0000 0000 0000  rG...c..........
+000006e0: 7248 0000 0063 0000 0000 0000 0000 0000  rH...c..........
 000006f0: 0000 0000 0000 0600 0000 0000 0000 734e  ..............sN
 00000700: 0000 0065 005a 0164 005a 0287 0066 0164  ...e.Z.d.Z...f.d
 00000710: 0164 0284 085a 0364 0365 0465 0565 0666  .d...Z.d.e.e.e.f
 00000720: 0219 0064 0465 0765 0865 096a 0a66 0219  ...d.e.e.e.j.f..
 00000730: 0066 0464 0564 0684 045a 0b64 0365 0666  .f.d.d...Z.d.e.f
 00000740: 0264 0764 0884 045a 0c87 0004 005a 0d53  .d.d...Z.....Z.S
 00000750: 0029 0972 2600 0000 6304 0000 0000 0000  .).r&...c.......
 00000760: 0000 0000 0004 0000 0005 0000 0003 0000  ................
 00000770: 0073 1e00 0000 7400 7401 7c00 8302 a002  .s....t.t.|.....
 00000780: 7c01 7c02 7c03 a103 0100 6401 7c00 5f03  |.|.|.....d.|._.
 00000790: 6400 5300 2902 4ee9 2000 0000 2904 da05  d.S.).N. ...)...
 000007a0: 7375 7065 7272 2600 0000 da08 5f5f 696e  superr&.....__in
 000007b0: 6974 5f5f da0f 6d69 6e69 5f62 6174 6368  it__..mini_batch
-000007c0: 5f73 697a 6529 04da 0473 656c 6672 2d00  _size)...selfr-.
+000007c0: 5f73 697a 6529 04da 0473 656c 6672 2e00  _size)...selfr..
 000007d0: 0000 7223 0000 00da 046d 6f64 65a9 01da  ..r#.....mode...
-000007e0: 095f 5f63 6c61 7373 5f5f 7230 0000 0072  .__class__r0...r
-000007f0: 3100 0000 724a 0000 0036 0000 0073 0400  1...rJ...6...s..
+000007e0: 095f 5f63 6c61 7373 5f5f 7231 0000 0072  .__class__r1...r
+000007f0: 3200 0000 724b 0000 0036 0000 0073 0400  2...rK...6...s..
 00000800: 0000 1401 0a01 7a15 5365 6331 3054 7261  ......z.Sec10Tra
-00000810: 696e 6572 2e5f 5f69 6e69 745f 5f72 4600  iner.__init__rF.
+00000810: 696e 6572 2e5f 5f69 6e69 745f 5f72 4700  iner.__init__rG.
 00000820: 0000 da06 7265 7475 726e 6302 0000 0000  ....returnc.....
 00000830: 0000 0000 0000 0002 0000 0001 0000 0043  ...............C
 00000840: 0000 0073 0400 0000 6400 5300 a901 4e72  ...s....d.S...Nr
-00000850: 3000 0000 2902 724c 0000 0072 4600 0000  0...).rL...rF...
-00000860: 7230 0000 0072 3000 0000 7231 0000 00da  r0...r0...r1....
+00000850: 3100 0000 2902 724d 0000 0072 4700 0000  1...).rM...rG...
+00000860: 7231 0000 0072 3100 0000 7232 0000 00da  r1...r1...r2....
 00000870: 0a74 7261 696e 5f73 7465 703a 0000 0073  .train_step:...s
 00000880: 0200 0000 0401 7a17 5365 6331 3054 7261  ......z.Sec10Tra
 00000890: 696e 6572 2e74 7261 696e 5f73 7465 7063  iner.train_stepc
 000008a0: 0200 0000 0000 0000 0000 0000 0500 0000  ................
 000008b0: 0500 0000 0300 0000 733a 0000 007c 0164  ........s:...|.d
 000008c0: 0119 007d 027c 026a 0088 006a 0164 0264  ...}.|.j...j.d.d
 000008d0: 038d 027d 0374 02a0 0387 0066 0164 0464  ...}.t.....f.d.d
 000008e0: 0584 087c 0344 0083 01a1 017d 0464 027c  ...|.D.....}.d.|
 000008f0: 0464 069c 0253 0029 074e 720f 0000 0072  .d...S.).Nr....r
 00000900: 0100 0000 2901 da03 6469 6d63 0100 0000  ....)...dimc....
 00000910: 0000 0000 0000 0000 0200 0000 0500 0000  ................
 00000920: 1300 0000 7324 0000 0067 007c 005d 0e7d  ....s$...g.|.].}
 00000930: 0188 00a0 007c 01a1 01a0 0164 00a1 01a0  .....|.....d....
 00000940: 02a1 00a0 03a1 0091 0271 0253 0029 0172  .........q.S.).r
-00000950: 1c00 0000 2904 722d 0000 00da 0661 7267  ....).r-.....arg
+00000950: 1c00 0000 2904 722e 0000 00da 0661 7267  ....).r......arg
 00000960: 6d61 78da 0664 6574 6163 6872 1900 0000  max..detachr....
-00000970: 2902 da02 2e30 da03 6d5f 78a9 0172 4c00  )....0..m_x..rL.
-00000980: 0000 7230 0000 0072 3100 0000 da0a 3c6c  ..r0...r1.....<l
+00000970: 2902 da02 2e30 da03 6d5f 78a9 0172 4d00  )....0..m_x..rM.
+00000980: 0000 7231 0000 0072 3200 0000 da0a 3c6c  ..r1...r2.....<l
 00000990: 6973 7463 6f6d 703e 4000 0000 7302 0000  istcomp>@...s...
 000009a0: 0024 007a 2a53 6563 3130 5472 6169 6e65  .$.z*Sec10Traine
 000009b0: 722e 7465 7374 5f73 7465 702e 3c6c 6f63  r.test_step.<loc
 000009c0: 616c 733e 2e3c 6c69 7374 636f 6d70 3e29  als>.<listcomp>)
 000009d0: 02da 046c 6f73 7372 1b00 0000 2904 da05  ...lossr....)...
-000009e0: 7370 6c69 7472 4b00 0000 7222 0000 00da  splitrK...r"....
-000009f0: 0363 6174 2905 724c 0000 0072 4600 0000  .cat).rL...rF...
+000009e0: 7370 6c69 7472 4c00 0000 7222 0000 00da  splitrL...r"....
+000009f0: 0363 6174 2905 724d 0000 0072 4700 0000  .cat).rM...rG...
 00000a00: 720f 0000 00da 066d 696e 695f 78da 036f  r......mini_x..o
-00000a10: 7574 7230 0000 0072 5800 0000 7231 0000  utr0...rX...r1..
+00000a10: 7574 7231 0000 0072 5900 0000 7232 0000  utr1...rY...r2..
 00000a20: 00da 0974 6573 745f 7374 6570 3d00 0000  ...test_step=...
 00000a30: 7308 0000 0008 0110 0118 010a 017a 1653  s............z.S
 00000a40: 6563 3130 5472 6169 6e65 722e 7465 7374  ec10Trainer.test
 00000a50: 5f73 7465 7029 0eda 085f 5f6e 616d 655f  _step)...__name_
 00000a60: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00000a70: 5f71 7561 6c6e 616d 655f 5f72 4a00 0000  _qualname__rJ...
+00000a70: 5f71 7561 6c6e 616d 655f 5f72 4b00 0000  _qualname__rK...
 00000a80: 7203 0000 00da 0574 7570 6c65 da04 6469  r......tuple..di
 00000a90: 6374 7204 0000 00da 0373 7472 7222 0000  ctr......strr"..
-00000aa0: 00da 0654 656e 736f 7272 5200 0000 725f  ...TensorrR...r_
+00000aa0: 00da 0654 656e 736f 7272 5300 0000 7260  ...TensorrS...r`
 00000ab0: 0000 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
-00000ac0: 5f5f 7230 0000 0072 3000 0000 724e 0000  __r0...r0...rN..
-00000ad0: 0072 3100 0000 7226 0000 0035 0000 0073  .r1...r&...5...s
+00000ac0: 5f5f 7231 0000 0072 3100 0000 724f 0000  __r1...r1...rO..
+00000ad0: 0072 3200 0000 7226 0000 0035 0000 0073  .r2...r&...5...s
 00000ae0: 0800 0000 0800 0c01 2404 1603 7226 0000  ........$...r&..
 00000af0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
 00000b00: 0000 0c00 0000 0000 0000 73dc 0000 0065  ..........s....e
 00000b10: 005a 0164 005a 0209 0109 0209 0309 0409  .Z.d.Z..........
 00000b20: 0564 1f64 0665 0365 0419 0064 0765 0365  .d.d.e.e...d.e.e
 00000b30: 0519 0064 0865 0365 0665 0719 0019 0064  ...d.e.e.e.....d
 00000b40: 0965 0365 0519 0064 0a65 0365 0819 0066  .e.e...d.e.e...f
@@ -187,78 +187,78 @@
 00000ba0: 0d65 0b64 0e65 0b66 0464 1764 1884 0483  .e.d.e.f.d.d....
 00000bb0: 015a 1064 0d65 0665 0a19 0064 0e65 0b65  .Z.d.e.e...d.e.e
 00000bc0: 1165 126a 1366 0219 0066 0464 1964 1a84  .e.j.f...f.d.d..
 00000bd0: 045a 1464 2164 1c65 1566 0264 1d64 1e84  .Z.d!d.e.f.d.d..
 00000be0: 055a 1687 0004 005a 1753 0029 2272 1f00  .Z.....Z.S.)"r..
 00000bf0: 0000 a903 da05 6368 756e 6bda 0966 696c  ......chunk..fil
 00000c00: 7465 7269 6e67 da07 7363 616c 696e 6772  tering..scalingr
-00000c10: 1700 0000 a902 7236 0000 0072 3700 0000  ......r6...r7...
+00000c10: 1700 0000 a902 7237 0000 0072 3800 0000  ......r7...r8...
 00000c20: e9fa 0000 0054 da08 7365 7175 656e 6365  .....T..sequence
 00000c30: da05 6e5f 636c 73da 0663 7574 6f66 66da  ..n_cls..cutoff.
 00000c40: 0d73 616d 706c 696e 675f 7261 7465 da03  .sampling_rate..
 00000c50: 686f 7463 0600 0000 0000 0000 0000 0000  hotc............
 00000c60: 0600 0000 0400 0000 0300 0000 732a 0000  ............s*..
 00000c70: 0074 0083 00a0 017c 017c 02a1 0201 007c  .t.....|.|.....|
 00000c80: 047c 005f 027c 037c 005f 037c 057c 005f  .|._.|.|._.|.|._
-00000c90: 047c 027c 005f 0564 0053 0072 5100 0000  .|.|._.d.S.rQ...
-00000ca0: 2906 7249 0000 0072 4a00 0000 7271 0000  ).rI...rJ...rq..
-00000cb0: 0072 7000 0000 da06 6973 5f68 6f74 726f  .rp.....is_hotro
-00000cc0: 0000 0029 0672 4c00 0000 726e 0000 0072  ...).rL...rn...r
-00000cd0: 6f00 0000 7270 0000 0072 7100 0000 7272  o...rp...rq...rr
-00000ce0: 0000 0072 4e00 0000 7230 0000 0072 3100  ...rN...r0...r1.
-00000cf0: 0000 724a 0000 0045 0000 0073 0a00 0000  ..rJ...E...s....
+00000c90: 047c 027c 005f 0564 0053 0072 5200 0000  .|.|._.d.S.rR...
+00000ca0: 2906 724a 0000 0072 4b00 0000 7272 0000  ).rJ...rK...rr..
+00000cb0: 0072 7100 0000 da06 6973 5f68 6f74 7270  .rq.....is_hotrp
+00000cc0: 0000 0029 0672 4d00 0000 726f 0000 0072  ...).rM...ro...r
+00000cd0: 7000 0000 7271 0000 0072 7200 0000 7273  p...rq...rr...rs
+00000ce0: 0000 0072 4f00 0000 7231 0000 0072 3200  ...rO...r1...r2.
+00000cf0: 0000 724b 0000 0045 0000 0073 0a00 0000  ..rK...E...s....
 00000d00: 0e08 0601 0601 0601 0a01 7a15 5365 6331  ..........z.Sec1
 00000d10: 3043 6f6c 6c61 7465 2e5f 5f69 6e69 745f  0Collate.__init_
-00000d20: 5f72 4600 0000 7250 0000 0063 0200 0000  _rF...rP...c....
+00000d20: 5f72 4700 0000 7251 0000 0063 0200 0000  _rG...rQ...c....
 00000d30: 0000 0000 0000 0000 0400 0000 0500 0000  ................
 00000d40: 4300 0000 734e 0000 007c 0164 0119 007d  C...sN...|.d...}
 00000d50: 027c 026a 0064 0219 0064 0316 007d 037c  .|.j.d...d...}.|
 00000d60: 0364 046b 0372 1a7c 0264 0064 0085 0264  .d.k.r.|.d.d...d
 00000d70: 007c 030b 0085 0266 0219 007d 027c 02a0  .|.....f...}.|..
 00000d80: 0164 027c 006a 0264 0514 00a1 027c 0164  .d.|.j.d.....|.d
 00000d90: 013c 007c 0153 0029 064e 720f 0000 0072  .<.|.S.).Nr....r
 00000da0: 1c00 0000 69c4 0900 0072 0100 0000 e90a  ....i....r......
 00000db0: 0000 0029 0372 1e00 0000 722b 0000 0072  ...).r....r+...r
-00000dc0: 7100 0000 2904 724c 0000 0072 4600 0000  q...).rL...rF...
-00000dd0: 720f 0000 00da 066d 6f64 756c 6f72 3000  r......modulor0.
-00000de0: 0000 7230 0000 0072 3100 0000 7269 0000  ..r0...r1...ri..
+00000dc0: 7200 0000 2904 724d 0000 0072 4700 0000  r...).rM...rG...
+00000dd0: 720f 0000 00da 066d 6f64 756c 6f72 3100  r......modulor1.
+00000de0: 0000 7231 0000 0072 3200 0000 726a 0000  ..r1...r2...rj..
 00000df0: 0053 0000 0073 0c00 0000 0801 0e01 0801  .S...s..........
 00000e00: 1601 1601 0401 7a12 5365 6331 3043 6f6c  ......z.Sec10Col
 00000e10: 6c61 7465 2e63 6875 6e6b 6302 0000 0000  late.chunkc.....
 00000e20: 0000 0000 0000 0003 0000 0003 0000 0043  ...............C
 00000e30: 0000 0073 2200 0000 7400 a001 7c00 6a02  ...s"...t...|.j.
 00000e40: a101 7d02 7c02 7c01 6401 1900 6701 1900  ..}.|.|.d...g...
 00000e50: 7c01 6401 3c00 7c01 5300 2902 4eda 0179  |.d.<.|.S.).N..y
-00000e60: 2903 7228 0000 00da 0365 7965 726f 0000  ).r(.....eyero..
-00000e70: 0029 0372 4c00 0000 7246 0000 005a 0c6f  .).rL...rF...Z.o
-00000e80: 6e65 686f 745f 7461 626c 6572 3000 0000  nehot_tabler0...
-00000e90: 7230 0000 0072 3100 0000 7272 0000 005b  r0...r1...rr...[
+00000e60: 2903 7228 0000 00da 0365 7965 7270 0000  ).r(.....eyerp..
+00000e70: 0029 0372 4d00 0000 7247 0000 005a 0c6f  .).rM...rG...Z.o
+00000e80: 6e65 686f 745f 7461 626c 6572 3100 0000  nehot_tabler1...
+00000e90: 7231 0000 0072 3200 0000 7273 0000 005b  r1...r2...rs...[
 00000ea0: 0000 0073 0600 0000 0c01 1201 0401 7a10  ...s..........z.
 00000eb0: 5365 6331 3043 6f6c 6c61 7465 2e68 6f74  Sec10Collate.hot
 00000ec0: 46da 0d62 616e 6470 6173 735f 6f6e 6c79  F..bandpass_only
 00000ed0: 6303 0000 0000 0000 0000 0000 0004 0000  c...............
 00000ee0: 0005 0000 0043 0000 0073 4800 0000 7400  .....C...sH...t.
 00000ef0: 7c01 6401 1900 7c00 6a01 8302 7d03 7c02  |.d...|.j...}.|.
 00000f00: 7213 7402 a003 7c03 a101 7c01 6401 3c00  r.t...|...|.d.<.
 00000f10: 7c01 5300 7400 7c03 7c00 6a01 6402 6403  |.S.t.|.|.j.d.d.
 00000f20: 8d03 7d03 7402 a003 7c03 a101 7c01 6401  ..}.t...|...|.d.
-00000f30: 3c00 7c01 5300 2904 4e72 0f00 0000 7239  <.|.S.).Nr....r9
-00000f40: 0000 0072 3800 0000 2904 723e 0000 0072  ...r8...).r>...r
-00000f50: 7100 0000 7228 0000 0072 4400 0000 2904  q...r(...rD...).
-00000f60: 724c 0000 0072 4600 0000 7278 0000 0072  rL...rF...rx...r
-00000f70: 0f00 0000 7230 0000 0072 3000 0000 7231  ....r0...r0...r1
-00000f80: 0000 0072 6a00 0000 6000 0000 730e 0000  ...rj...`...s...
+00000f30: 3c00 7c01 5300 2904 4e72 0f00 0000 723a  <.|.S.).Nr....r:
+00000f40: 0000 0072 3900 0000 2904 723f 0000 0072  ...r9...).r?...r
+00000f50: 7200 0000 7228 0000 0072 4500 0000 2904  r...r(...rE...).
+00000f60: 724d 0000 0072 4700 0000 7279 0000 0072  rM...rG...ry...r
+00000f70: 0f00 0000 7231 0000 0072 3100 0000 7232  ....r1...r1...r2
+00000f80: 0000 0072 6b00 0000 6000 0000 730e 0000  ...rk...`...s...
 00000f90: 0010 0104 020e 0104 0110 020e 0104 017a  ...............z
 00000fa0: 1653 6563 3130 436f 6c6c 6174 652e 6669  .Sec10Collate.fi
 00000fb0: 6c74 6572 696e 6763 0100 0000 0000 0000  lteringc........
 00000fc0: 0000 0000 0100 0000 0300 0000 4300 0000  ............C...
 00000fd0: 7314 0000 0074 007c 0064 0119 0083 017c  s....t.|.d.....|
 00000fe0: 0064 013c 007c 0053 0029 024e 720f 0000  .d.<.|.S.).Nr...
-00000ff0: 0029 0172 4700 0000 2901 7246 0000 0072  .).rG...).rF...r
-00001000: 3000 0000 7230 0000 0072 3100 0000 726b  0...r0...r1...rk
+00000ff0: 0029 0172 4800 0000 2901 7247 0000 0072  .).rH...).rG...r
+00001000: 3100 0000 7231 0000 0072 3200 0000 726c  1...r1...r2...rl
 00001010: 0000 006b 0000 0073 0400 0000 1002 0401  ...k...s........
 00001020: 7a14 5365 6331 3043 6f6c 6c61 7465 2e73  z.Sec10Collate.s
 00001030: 6361 6c69 6e67 6302 0000 0000 0000 0000  calingc.........
 00001040: 0000 0005 0000 0006 0000 0043 0000 0073  ...........C...s
 00001050: 0201 0000 6700 6700 6401 9c02 7d02 7c01  ....g.g.d...}.|.
 00001060: 4400 5d51 7d03 7c00 6a00 4400 5d21 7d04  D.]Q}.|.j.D.]!}.
 00001070: 7c04 6402 6b02 7218 7c00 a001 7c03 a101  |.d.k.r.|...|...
@@ -272,62 +272,62 @@
 000010f0: 0100 7c02 6407 1900 a007 7c03 6407 1900  ..|.d.....|.d...
 00001100: a101 0100 7107 7409 a00a 7c02 6407 1900  ....q.t...|.d...
 00001110: a101 7c02 6407 3c00 740b a00c 7c02 6407  ..|.d.<.t...|.d.
 00001120: 1900 a101 a00d a100 a00e 6408 a101 7c02  ..........d...|.
 00001130: 6407 3c00 7c02 6406 1900 727b 7409 a00a  d.<.|.d...r{t...
 00001140: 7c02 6406 1900 a101 6e01 6700 7c02 6406  |.d.....n.g.|.d.
 00001150: 3c00 7c02 5300 2909 4ea9 0272 0f00 0000  <.|.S.).N..r....
-00001160: 7276 0000 0072 6900 0000 726a 0000 0072  rv...ri...rj...r
-00001170: 6b00 0000 7218 0000 0072 7600 0000 720f  k...r....rv...r.
-00001180: 0000 0072 1500 0000 290f 726e 0000 0072  ...r....).rn...r
-00001190: 6900 0000 726a 0000 0072 6b00 0000 721d  i...rj...rk...r.
-000011a0: 0000 00da 046b 6579 7372 7300 0000 7243  .....keysrs...rC
-000011b0: 0000 0072 7200 0000 7228 0000 0072 2900  ...rr...r(...r).
+00001160: 7277 0000 0072 6a00 0000 726b 0000 0072  rw...rj...rk...r
+00001170: 6c00 0000 7218 0000 0072 7700 0000 720f  l...r....rw...r.
+00001180: 0000 0072 1500 0000 290f 726f 0000 0072  ...r....).ro...r
+00001190: 6a00 0000 726b 0000 0072 6c00 0000 721d  j...rk...rl...r.
+000011a0: 0000 00da 046b 6579 7372 7400 0000 7244  .....keysrt...rD
+000011b0: 0000 0072 7300 0000 7228 0000 0072 2900  ...rs...r(...r).
 000011c0: 0000 7222 0000 00da 0a66 726f 6d5f 6e75  ..r".....from_nu
 000011d0: 6d70 79da 0566 6c6f 6174 da09 756e 7371  mpy..float..unsq
-000011e0: 7565 657a 6529 0572 4c00 0000 7246 0000  ueeze).rL...rF..
+000011e0: 7565 657a 6529 0572 4d00 0000 7247 0000  ueeze).rM...rG..
 000011f0: 00da 0762 6174 6368 6573 da01 62da 0373  ...batches..b..s
-00001200: 6571 7230 0000 0072 3000 0000 7231 0000  eqr0...r0...r1..
+00001200: 6571 7231 0000 0072 3100 0000 7232 0000  eqr1...r1...r2..
 00001210: 00da 085f 5f63 616c 6c5f 5f70 0000 0073  ...__call__p...s
 00001220: 2600 0000 0a01 0801 0a01 0801 0c01 0801  &...............
 00001230: 0c01 0801 0c01 0402 1001 0601 1a01 1202  ................
 00001240: 1401 1201 1c01 1e01 0401 7a15 5365 6331  ..........z.Sec1
 00001250: 3043 6f6c 6c61 7465 2e5f 5f63 616c 6c5f  0Collate.__call_
 00001260: 5f4e da04 6675 6e63 6302 0000 0000 0000  _N..funcc.......
 00001270: 0000 0000 0003 0000 0004 0000 0003 0000  ................
 00001280: 0073 2600 0000 8800 6400 7500 7207 7c00  .s&.....d.u.r.|.
 00001290: 6a00 8900 7401 8800 8301 8700 6601 6401  j...t.......f.d.
 000012a0: 6402 8408 8301 7d02 7c02 5300 2903 4e63  d.....}.|.S.).Nc
 000012b0: 0000 0000 0000 0000 0000 0000 0200 0000  ................
 000012c0: 0400 0000 1f00 0000 730e 0000 0088 007c  ........s......|
-000012d0: 0069 007c 01a4 018e 0153 0072 5100 0000  .i.|.....S.rQ...
-000012e0: 7230 0000 0029 02da 0461 7267 73da 066b  r0...)...args..k
-000012f0: 7761 7267 73a9 0172 8200 0000 7230 0000  wargs..r....r0..
-00001300: 0072 3100 0000 da0c 7772 6170 7065 645f  .r1.....wrapped_
+000012d0: 0069 007c 01a4 018e 0153 0072 5200 0000  .i.|.....S.rR...
+000012e0: 7231 0000 0029 02da 0461 7267 73da 066b  r1...)...args..k
+000012f0: 7761 7267 73a9 0172 8300 0000 7231 0000  wargs..r....r1..
+00001300: 0072 3200 0000 da0c 7772 6170 7065 645f  .r2.....wrapped_
 00001310: 6675 6e63 8b00 0000 7302 0000 000e 027a  func....s......z
 00001320: 2753 6563 3130 436f 6c6c 6174 652e 7772  'Sec10Collate.wr
 00001330: 6170 2e3c 6c6f 6361 6c73 3e2e 7772 6170  ap.<locals>.wrap
-00001340: 7065 645f 6675 6e63 2902 7281 0000 0072  ped_func).r....r
-00001350: 0200 0000 2903 724c 0000 0072 8200 0000  ....).rL...r....
-00001360: 7286 0000 0072 3000 0000 7285 0000 0072  r....r0...r....r
-00001370: 3100 0000 7221 0000 0087 0000 0073 0a00  1...r!.......s..
+00001340: 7065 645f 6675 6e63 2902 7282 0000 0072  ped_func).r....r
+00001350: 0200 0000 2903 724d 0000 0072 8300 0000  ....).rM...r....
+00001360: 7287 0000 0072 3100 0000 7286 0000 0072  r....r1...r....r
+00001370: 3200 0000 7221 0000 0087 0000 0073 0a00  2...r!.......s..
 00001380: 0000 0801 0601 0602 0e01 0403 7a11 5365  ............z.Se
 00001390: 6331 3043 6f6c 6c61 7465 2e77 7261 7029  c10Collate.wrap)
-000013a0: 0572 6800 0000 7217 0000 0072 6c00 0000  .rh...r....rl...
-000013b0: 726d 0000 0054 2901 4672 5100 0000 2918  rm...T).FrQ...).
-000013c0: 7260 0000 0072 6100 0000 7262 0000 0072  r`...ra...rb...r
-000013d0: 0500 0000 7263 0000 00da 0369 6e74 7206  ....rc.....intr.
-000013e0: 0000 0072 7c00 0000 da04 626f 6f6c 724a  ...r|.....boolrJ
-000013f0: 0000 0072 6400 0000 7204 0000 0072 6900  ...rd...r....ri.
-00001400: 0000 7272 0000 0072 6a00 0000 da0c 7374  ..rr...rj.....st
-00001410: 6174 6963 6d65 7468 6f64 726b 0000 0072  aticmethodrk...r
-00001420: 6500 0000 7222 0000 0072 6600 0000 7281  e...r"...rf...r.
-00001430: 0000 0072 0700 0000 7221 0000 0072 6700  ...r....r!...rg.
-00001440: 0000 7230 0000 0072 3000 0000 724e 0000  ..r0...r0...rN..
-00001450: 0072 3100 0000 721f 0000 0044 0000 0073  .r1...r....D...s
+000013a0: 0572 6900 0000 7217 0000 0072 6d00 0000  .ri...r....rm...
+000013b0: 726e 0000 0054 2901 4672 5200 0000 2918  rn...T).FrR...).
+000013c0: 7261 0000 0072 6200 0000 7263 0000 0072  ra...rb...rc...r
+000013d0: 0500 0000 7264 0000 00da 0369 6e74 7206  ....rd.....intr.
+000013e0: 0000 0072 7d00 0000 da04 626f 6f6c 724b  ...r}.....boolrK
+000013f0: 0000 0072 6500 0000 7204 0000 0072 6a00  ...re...r....rj.
+00001400: 0000 7273 0000 0072 6b00 0000 da0c 7374  ..rs...rk.....st
+00001410: 6174 6963 6d65 7468 6f64 726c 0000 0072  aticmethodrl...r
+00001420: 6600 0000 7222 0000 0072 6700 0000 7282  f...r"...rg...r.
+00001430: 0000 0072 0700 0000 7221 0000 0072 6800  ...r....r!...rh.
+00001440: 0000 7231 0000 0072 3100 0000 724f 0000  ..r1...r1...rO..
+00001450: 0072 3200 0000 721f 0000 0044 0000 0073  .r2...r....D...s
 00001460: 3000 0000 0800 0203 0201 0201 0201 0201  0...............
 00001470: 04fa 0602 02fe 0603 02fd 0a04 02fc 0605  ................
 00001480: 02fb 0606 0efa 120e 1208 1c05 020b 1401  ................
 00001490: 2004 1817 721f 0000 0063 0000 0000 0000   ...r....c......
 000014a0: 0000 0000 0000 0000 0000 0800 0000 4000  ..............@.
 000014b0: 0000 733e 0000 0065 005a 0164 005a 0264  ..s>...e.Z.d.Z.d
 000014c0: 0a64 0265 036a 0464 0365 0565 0665 0765  .d.e.j.d.e.e.e.e
@@ -337,65 +337,65 @@
 00001500: 6367 5f73 6574 da09 6c61 6265 6c5f 7365  cg_set..label_se
 00001510: 7463 0300 0000 0000 0000 0000 0000 0300  tc..............
 00001520: 0000 0400 0000 4300 0000 732a 0000 0074  ......C...s*...t
 00001530: 007c 016a 0183 0164 016b 0272 0d7c 01a0  .|.j...d.k.r.|..
 00001540: 0264 0164 02a1 026e 017c 017c 005f 037c  .d.d...n.|.|._.|
 00001550: 027c 005f 0464 0053 0029 034e 7215 0000  .|._.d.S.).Nr...
 00001560: 0072 1c00 0000 2905 721d 0000 0072 1e00  .r....).r....r..
-00001570: 0000 722b 0000 0072 8a00 0000 728b 0000  ..r+...r....r...
-00001580: 0029 0372 4c00 0000 728a 0000 0072 8b00  .).rL...r....r..
-00001590: 0000 7230 0000 0072 3000 0000 7231 0000  ..r0...r0...r1..
-000015a0: 0072 4a00 0000 9300 0000 7304 0000 0020  .rJ.......s.... 
+00001570: 0000 722b 0000 0072 8b00 0000 728c 0000  ..r+...r....r...
+00001580: 0029 0372 4d00 0000 728b 0000 0072 8c00  .).rM...r....r..
+00001590: 0000 7231 0000 0072 3100 0000 7232 0000  ..r1...r1...r2..
+000015a0: 0072 4b00 0000 9300 0000 7304 0000 0020  .rK.......s.... 
 000015b0: 010a 017a 1553 6563 3130 4461 7461 7365  ...z.Sec10Datase
 000015c0: 742e 5f5f 696e 6974 5f5f 6301 0000 0000  t.__init__c.....
 000015d0: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
 000015e0: 0000 0073 0a00 0000 7400 7c00 6a01 8301  ...s....t.|.j...
-000015f0: 5300 7251 0000 0029 0272 1d00 0000 728a  S.rQ...).r....r.
-00001600: 0000 0072 5800 0000 7230 0000 0072 3000  ...rX...r0...r0.
-00001610: 0000 7231 0000 00da 075f 5f6c 656e 5f5f  ..r1.....__len__
+000015f0: 5300 7252 0000 0029 0272 1d00 0000 728b  S.rR...).r....r.
+00001600: 0000 0072 5900 0000 7231 0000 0072 3100  ...rY...r1...r1.
+00001610: 0000 7232 0000 00da 075f 5f6c 656e 5f5f  ..r2.....__len__
 00001620: 9700 0000 7302 0000 000a 017a 1453 6563  ....s......z.Sec
 00001630: 3130 4461 7461 7365 742e 5f5f 6c65 6e5f  10Dataset.__len_
 00001640: 5f63 0200 0000 0000 0000 0000 0000 0400  _c..............
 00001650: 0000 0400 0000 4300 0000 7338 0000 007c  ......C...s8...|
 00001660: 006a 007c 0119 00a0 0164 0164 02a1 027d  .j.|.....d.d...}
 00001670: 027c 006a 0264 0075 0172 187c 006a 027c  .|.j.d.u.r.|.j.|
 00001680: 0119 007d 037c 027c 0364 039c 0253 0064  ...}.|.|.d...S.d
 00001690: 047c 0269 0153 0029 054e 7215 0000 0072  .|.i.S.).Nr....r
-000016a0: 1c00 0000 7279 0000 0072 0f00 0000 2903  ....ry...r....).
-000016b0: 728a 0000 0072 2b00 0000 728b 0000 0029  r....r+...r....)
-000016c0: 0472 4c00 0000 da03 6964 78da 0365 6367  .rL.....idx..ecg
-000016d0: da05 6c61 6265 6c72 3000 0000 7230 0000  ..labelr0...r0..
-000016e0: 0072 3100 0000 da0b 5f5f 6765 7469 7465  .r1.....__getite
+000016a0: 1c00 0000 727a 0000 0072 0f00 0000 2903  ....rz...r....).
+000016b0: 728b 0000 0072 2b00 0000 728c 0000 0029  r....r+...r....)
+000016c0: 0472 4d00 0000 da03 6964 78da 0365 6367  .rM.....idx..ecg
+000016d0: da05 6c61 6265 6c72 3100 0000 7231 0000  ..labelr1...r1..
+000016e0: 0072 3200 0000 da0b 5f5f 6765 7469 7465  .r2.....__getite
 000016f0: 6d5f 5f9a 0000 0073 0a00 0000 1201 0a01  m__....s........
 00001700: 0a01 0a01 0802 7a18 5365 6331 3044 6174  ......z.Sec10Dat
 00001710: 6173 6574 2e5f 5f67 6574 6974 656d 5f5f  aset.__getitem__
-00001720: 7251 0000 0029 0c72 6000 0000 7261 0000  rQ...).r`...ra..
-00001730: 0072 6200 0000 7228 0000 00da 076e 6461  .rb...r(.....nda
+00001720: 7252 0000 0029 0c72 6100 0000 7262 0000  rR...).ra...rb..
+00001730: 0072 6300 0000 7228 0000 00da 076e 6461  .rc...r(.....nda
 00001740: 7272 6179 7205 0000 0072 0300 0000 7206  rrayr....r....r.
-00001750: 0000 0072 0800 0000 724a 0000 0072 8c00  ...r....rJ...r..
-00001760: 0000 7290 0000 0072 3000 0000 7230 0000  ..r....r0...r0..
-00001770: 0072 3000 0000 7231 0000 0072 2000 0000  .r0...r1...r ...
+00001750: 0000 0072 0800 0000 724b 0000 0072 8d00  ...r....rK...r..
+00001760: 0000 7291 0000 0072 3100 0000 7231 0000  ..r....r1...r1..
+00001770: 0072 3100 0000 7232 0000 0072 2000 0000  .r1...r2...r ...
 00001780: 9200 0000 7308 0000 0008 0022 0108 040c  ....s......"....
-00001790: 0372 2000 0000 2901 7233 0000 0029 24da  .r ...).r3...)$.
+00001790: 0372 2000 0000 2901 7234 0000 0029 24da  .r ...).r4...)$.
 000017a0: 0966 756e 6374 6f6f 6c73 7202 0000 00da  .functoolsr.....
 000017b0: 0674 7970 696e 6772 0300 0000 7204 0000  .typingr....r...
 000017c0: 0072 0500 0000 7206 0000 0072 0700 0000  .r....r....r....
 000017d0: 7208 0000 00da 056e 756d 7079 7228 0000  r......numpyr(..
 000017e0: 0072 2200 0000 da05 7363 6970 7972 0900  .r".....scipyr..
-000017f0: 0000 723a 0000 005a 1573 6b6c 6561 726e  ..r:...Z.sklearn
+000017f0: 0000 723b 0000 005a 1573 6b6c 6561 726e  ..r;...Z.sklearn
 00001800: 2e70 7265 7072 6f63 6573 7369 6e67 720a  .preprocessingr.
 00001810: 0000 00da 1074 6f72 6368 2e75 7469 6c73  .....torch.utils
-00001820: 2e64 6174 6172 0b00 0000 720c 0000 005a  .datar....r....Z
+00001820: 2e64 6174 6172 0b00 0000 720c 0000 00da  .datar....r.....
 00001830: 0a7a 6165 5f65 6e67 696e 65da 207a 6165  .zae_engine. zae
 00001840: 5f65 6e67 696e 652e 6461 7461 5f70 6970  _engine.data_pip
 00001850: 656c 696e 652e 636f 6c6c 6174 6572 0d00  eline.collater..
 00001860: 0000 da17 7a61 655f 656e 6769 6e65 2e6d  ....zae_engine.m
 00001870: 6f64 656c 732e 6275 696c 6472 0e00 0000  odels.buildr....
-00001880: 7291 0000 0072 8700 0000 7232 0000 0072  r....r....r2...r
-00001890: 6500 0000 723e 0000 0072 4700 0000 722e  e...r>...rG...r.
+00001880: 7292 0000 0072 8800 0000 7233 0000 0072  r....r....r3...r
+00001890: 6600 0000 723f 0000 0072 4800 0000 722f  f...r?...rH...r/
 000018a0: 0000 00da 0754 7261 696e 6572 7226 0000  .....Trainerr&..
-000018b0: 0072 1f00 0000 7220 0000 0072 3000 0000  .r....r ...r0...
-000018c0: 7230 0000 0072 3000 0000 7231 0000 00da  r0...r0...r1....
+000018b0: 0072 1f00 0000 7220 0000 0072 3100 0000  .r....r ...r1...
+000018c0: 7231 0000 0072 3100 0000 7232 0000 00da  r1...r1...r2....
 000018d0: 083c 6d6f 6475 6c65 3e01 0000 0073 2000  .<module>....s .
 000018e0: 0000 0c00 2001 0802 0801 0c01 0c01 1001  .... ...........
 000018f0: 0802 0c01 0c01 1403 1e11 100a 140b 100f  ................
 00001900: 144e                                     .N
```

### Comparing `zae_engine-0.1.2/zae_engine/inference/beat.py` & `zae_engine-0.1.3/zae_engine/inference/beat.py`

 * *Files identical despite different names*

### Comparing `zae_engine-0.1.2/zae_engine/inference/sec10.py` & `zae_engine-0.1.3/zae_engine/inference/sec10.py`

 * *Files identical despite different names*

### Comparing `zae_engine-0.1.2/zae_engine/loss/__pycache__/_loss.cpython-310.pyc` & `zae_engine-0.1.3/zae_engine/loss/__pycache__/_loss.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zae_engine-0.1.2/zae_engine/loss/_loss.py` & `zae_engine-0.1.3/zae_engine/loss/_loss.py`

 * *Files identical despite different names*

### Comparing `zae_engine-0.1.2/zae_engine/measure/__pycache__/_measure.cpython-310.pyc` & `zae_engine-0.1.3/zae_engine/measure/__pycache__/_measure.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Feb  6 02:01:08 2024 UTC, .py size: 11758 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 e492 c165 ee2d 0000  o..........e.-..
+00000000: 6f0d 0d0a 0000 0000 d5f1 fc65 ee2d 0000  o..........e.-..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000d 0000 0040 0000 0073 c801 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 0100 6400 6402 6c06  m.Z.m.Z...d.d.l.
 00000050: 5a07 6400 6402 6c08 5a08 6400 6403 6c09  Z.d.d.l.Z.d.d.l.
 00000060: 6d0a 5a0a 0100 6400 6404 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
 00000070: 0100 6507 a00d 6507 6a0e a101 6a0f 5a10  ..e...e.j...j.Z.
```

### Comparing `zae_engine-0.1.2/zae_engine/measure/_measure.py` & `zae_engine-0.1.3/zae_engine/measure/_measure.py`

 * *Files identical despite different names*

### Comparing `zae_engine-0.1.2/zae_engine/models/__pycache__/benchmark.cpython-310.pyc` & `zae_engine-0.1.3/zae_engine/models/__pycache__/benchmark.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zae_engine-0.1.2/zae_engine/models/__pycache__/build.cpython-310.pyc` & `zae_engine-0.1.3/zae_engine/models/__pycache__/build.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Feb  6 02:03:49 2024 UTC, .py size: 18698 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8593 c165 0a49 0000  o..........e.I..
+00000000: 6f0d 0d0a 0000 0000 7654 fd65 0a49 0000  o.......vT.e.I..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 be00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6401 6c07 5a08 6400 6401 6c09  ..d.d.l.Z.d.d.l.
 00000060: 5a09 6400 6401 6c0a 6d0b 5a0b 0100 6400  Z.d.d.l.m.Z...d.
 00000070: 6401 6c0c 6d0b 0200 0100 6d0d 5a0e 0100  d.l.m.....m.Z...
@@ -929,15 +929,15 @@
 00003a00: 0302 fd02 0402 fc02 0502 fb02 0602 fa02  ................
 00003a10: 070a f902 3602 0202 fe02 0302 fd02 0402  ....6...........
 00003a20: fc02 0502 fb02 060a fa10 2672 8700 0000  ..........&r....
 00003a30: 291a da03 7379 73da 0674 7970 696e 6772  )...sys..typingr
 00003a40: 0200 0000 7203 0000 0072 0400 0000 7205  ....r....r....r.
 00003a50: 0000 0072 0600 0000 da05 6e75 6d70 7972  ...r......numpyr
 00003a60: 4800 0000 726e 0000 00da 0874 6f72 6368  H...rn.....torch
-00003a70: 2e6e 6e72 2300 0000 5a13 746f 7263 682e  .nnr#...Z.torch.
+00003a70: 2e6e 6e72 2300 0000 da13 746f 7263 682e  .nnr#.....torch.
 00003a80: 6e6e 2e66 756e 6374 696f 6e61 6cda 0a66  nn.functional..f
 00003a90: 756e 6374 696f 6e61 6c72 ba00 0000 7207  unctionalr....r.
 00003aa0: 0000 00da 0a7a 6165 5f65 6e67 696e 6572  .....zae_enginer
 00003ab0: 0800 0000 7241 0000 00da 197a 6165 5f65  ....rA.....zae_e
 00003ac0: 6e67 696e 652e 6d6f 6465 6c73 2e75 7469  ngine.models.uti
 00003ad0: 6c69 7479 7209 0000 0072 bf00 0000 720a  lityr....r....r.
 00003ae0: 0000 0072 5c00 0000 7277 0000 0072 8700  ...r\...rw...r..
```

### Comparing `zae_engine-0.1.2/zae_engine/models/__pycache__/utility.cpython-310.pyc` & `zae_engine-0.1.3/zae_engine/models/__pycache__/utility.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zae_engine-0.1.2/zae_engine/models/benchmark.py` & `zae_engine-0.1.3/zae_engine/models/benchmark.py`

 * *Files identical despite different names*

### Comparing `zae_engine-0.1.2/zae_engine/models/build.py` & `zae_engine-0.1.3/zae_engine/models/build.py`

 * *Files identical despite different names*

### Comparing `zae_engine-0.1.2/zae_engine/models/utility.py` & `zae_engine-0.1.3/zae_engine/models/utility.py`

 * *Files identical despite different names*

### Comparing `zae_engine-0.1.2/zae_engine/nn_night/__pycache__/_activation.cpython-310.pyc` & `zae_engine-0.1.3/zae_engine/nn_night/__pycache__/_activation.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zae_engine-0.1.2/zae_engine/nn_night/__pycache__/_layer.cpython-310.pyc` & `zae_engine-0.1.3/zae_engine/nn_night/__pycache__/_layer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zae_engine-0.1.2/zae_engine/nn_night/__pycache__/_module.cpython-310.pyc` & `zae_engine-0.1.3/zae_engine/nn_night/__pycache__/_module.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zae_engine-0.1.2/zae_engine/nn_night/_activation.py` & `zae_engine-0.1.3/zae_engine/nn_night/_activation.py`

 * *Files identical despite different names*

### Comparing `zae_engine-0.1.2/zae_engine/nn_night/_layer.py` & `zae_engine-0.1.3/zae_engine/nn_night/_layer.py`

 * *Files identical despite different names*

### Comparing `zae_engine-0.1.2/zae_engine/nn_night/_module.py` & `zae_engine-0.1.3/zae_engine/nn_night/_module.py`

 * *Files identical despite different names*

### Comparing `zae_engine-0.1.2/zae_engine/operation/__pycache__/_operation.cpython-310.pyc` & `zae_engine-0.1.3/zae_engine/operation/__pycache__/_operation.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zae_engine-0.1.2/zae_engine/operation/_operation.py` & `zae_engine-0.1.3/zae_engine/operation/_operation.py`

 * *Files identical despite different names*

### Comparing `zae_engine-0.1.2/zae_engine/scripts/example_script.py` & `zae_engine-0.1.3/zae_engine/scripts/example_script.py`

 * *Files identical despite different names*

### Comparing `zae_engine-0.1.2/zae_engine/trainer/__pycache__/_trainer.cpython-310.pyc` & `zae_engine-0.1.3/zae_engine/trainer/__pycache__/_trainer.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Feb  7 00:16:33 2024 UTC, .py size: 12698 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,788 +1,805 @@
-00000000: 6f0d 0d0a 0000 0000 e1cb c265 9a31 0000  o..........e.1..
+00000000: 6f0d 0d0a 0000 0000 de21 0a66 fb33 0000  o........!.f.3..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 8600 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 8e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 0100 6400  m.Z.m.Z.m.Z...d.
-00000070: 6401 6c0c 5a0c 6400 6401 6c0d 5a0e 6400  d.l.Z.d.d.l.Z.d.
-00000080: 6401 6c0f 5a0f 6405 6406 6c10 6d11 5a11  d.l.Z.d.d.l.m.Z.
-00000090: 0100 4700 6407 6408 8400 6408 6502 8303  ..G.d.d...d.e...
-000000a0: 5a12 4700 6409 640a 8400 640a 8302 5a13  Z.G.d.d...d...Z.
-000000b0: 6401 5300 290b e900 0000 004e 2902 da03  d.S.)......N)...
-000000c0: 4142 43da 0e61 6273 7472 6163 746d 6574  ABC..abstractmet
-000000d0: 686f 6429 01da 0b64 6566 6175 6c74 6469  hod)...defaultdi
-000000e0: 6374 2905 da05 5475 706c 65da 0444 6963  ct)...Tuple..Dic
-000000f0: 74da 0555 6e69 6f6e da08 4f70 7469 6f6e  t..Union..Option
-00000100: 616c da08 4974 6572 6162 6c65 e901 0000  al..Iterable....
-00000110: 0029 01da 0d4e 6570 7475 6e65 4c6f 6767  .)...NeptuneLogg
-00000120: 6572 6300 0000 0000 0000 0000 0000 0000  erc.............
-00000130: 0000 0012 0000 0040 0000 0073 4002 0000  .......@...s@...
-00000140: 6500 5a01 6400 5a02 6401 5a03 0902 0902  e.Z.d.Z.d.Z.....
-00000150: 0903 0902 6446 6404 6504 6a05 6405 6506  ....dFd.e.j.d.e.
-00000160: 6406 6507 6504 6a08 6a09 1900 6407 6507  d.e.e.j.j...d.e.
-00000170: 6408 650a 6409 6507 650b 6506 650c 650d  d.e.d.e.e.e.e.e.
-00000180: 650b 6602 1900 6602 1900 1900 660c 640a  e.f...f.....f.d.
-00000190: 640b 8405 5a0e 640c 650f 6504 6a10 640d  d...Z.d.e.e.j.d.
-000001a0: 6602 1900 7035 6504 6a10 6602 640e 640f  f...p5e.j.f.d.d.
-000001b0: 8404 5a11 640c 650f 650c 6504 6a10 6504  ..Z.d.e.e.e.j.e.
-000001c0: 6a12 6a13 6602 1900 1900 704e 650c 6504  j.j.f.....pNe.e.
-000001d0: 6a10 6504 6a12 6a13 6602 1900 6602 6410  j.e.j.j.f...f.d.
-000001e0: 6411 8404 5a14 6447 6448 6413 6414 8405  d...Z.dGdHd.d...
-000001f0: 5a15 6415 6416 8400 5a16 6449 6417 6517  Z.d.d...Z.dId.e.
-00000200: 640c 6402 6604 6418 6419 8405 5a18 641a  d.d.f.d.d...Z.d.
-00000210: 641b 8400 5a19 6448 641c 641d 8404 5a1a  d...Z.dHd.d...Z.
-00000220: 641e 650c 651b 650b 6602 1900 640c 6402  d.e.e.e.f...d.d.
-00000230: 6604 641f 6420 8404 5a1c 651d 641e 650c  f.d.d ..Z.e.d.e.
-00000240: 651b 650b 6602 1900 640c 651e 6506 6504  e.e.f...d.e.e.e.
-00000250: 6a10 6602 1900 6604 6421 6422 8404 8301  j.f...f.d!d"....
-00000260: 5a1f 651d 641e 650c 651b 650b 6602 1900  Z.e.d.e.e.e.f...
-00000270: 640c 651e 6506 6504 6a10 6602 1900 6604  d.e.e.e.j.f...f.
-00000280: 6423 6424 8404 8301 5a20 6425 651e 6506  d#d$....Z d%e.e.
-00000290: 6504 6a10 6602 1900 640c 6402 6604 6426  e.j.f...d.d.f.d&
-000002a0: 6427 8404 5a21 6449 6405 6506 640c 6402  d'..Z!dId.e.d.d.
-000002b0: 6604 6428 6429 8405 5a22 642a 6517 642b  f.d(d)..Z"d*e.d+
-000002c0: 6523 640c 6402 6606 642c 642d 8404 5a24  e#d.d.f.d,d-..Z$
-000002d0: 6448 642e 642f 8404 5a25 6430 6517 6431  dHd.d/..Z%d0e.d1
-000002e0: 6517 640c 6402 6606 6432 6433 8404 5a26  e.d.d.f.d2d3..Z&
-000002f0: 6434 6506 640c 6402 6604 6435 6436 8404  d4e.d.d.f.d5d6..
-00000300: 5a27 644a 6434 6506 6438 6528 640c 6402  Z'dJd4e.d8e(d.d.
-00000310: 6606 6439 643a 8405 5a29 6409 651e 6506  f.d9d:..Z)d.e.e.
-00000320: 650c 650d 650b 6602 1900 6602 1900 640c  e.e.e.f...f...d.
-00000330: 651e 6506 650c 650d 6402 6602 1900 6602  e.e.e.e.d.f...f.
-00000340: 1900 6604 643b 643c 8404 5a2a 644b 643e  ..f.d;d<..Z*dKd>
-00000350: 6506 643f 6506 640c 6402 6606 6440 6441  e.d?e.d.d.f.d@dA
-00000360: 8405 5a2b 6448 6442 6443 8404 5a2c 640c  ..Z+dHdBdC..Z,d.
-00000370: 652d 6602 6444 6445 8404 5a2e 6402 5300  e-f.dDdE..Z.d.S.
-00000380: 294c da07 5472 6169 6e65 7261 f501 0000  )L..Trainera....
-00000390: 0a20 2020 2041 6273 7472 6163 7420 636c  .    Abstract cl
-000003a0: 6173 7320 666f 7220 6578 7065 7269 6d65  ass for experime
-000003b0: 6e74 7320 7769 7468 2032 2061 6273 7472  nts with 2 abstr
-000003c0: 6163 7420 6d65 7468 6f64 7320 7472 6169  act methods trai
-000003d0: 6e5f 7374 6570 2061 6e64 2074 6573 745f  n_step and test_
-000003e0: 7374 6570 2e0a 2020 2020 4e6f 7465 2074  step..    Note t
-000003f0: 6861 7420 626f 7468 2074 6865 2074 7261  hat both the tra
-00000400: 696e 5f73 7465 7020 616e 6420 7465 7374  in_step and test
-00000410: 5f73 7465 7020 6172 6520 7265 6365 6976  _step are receiv
-00000420: 6520 6261 7463 6820 616e 6420 7265 7475  e batch and retu
-00000430: 726e 2061 2064 6963 7469 6f6e 6172 792e  rn a dictionary.
-00000440: 0a20 2020 204d 6f72 6520 6465 7461 696c  .    More detail
-00000450: 2061 626f 7574 2074 686f 7365 2061 7265   about those are
-00000460: 2069 6e20 6561 6368 206d 6574 686f 6427   in each method'
-00000470: 7320 646f 6373 7472 696e 672e 0a0a 2020  s docstring...  
-00000480: 2020 3a70 6172 616d 206d 6f64 656c 3a20    :param model: 
-00000490: 6e6e 2e4d 6f64 756c 650a 2020 2020 3a70  nn.Module.    :p
-000004a0: 6172 616d 2064 6576 6963 653a 2074 6f72  aram device: tor
-000004b0: 6368 2e64 6576 6963 650a 2020 2020 3a70  ch.device.    :p
-000004c0: 6172 616d 206d 6f64 653a 2073 7472 0a20  aram mode: str. 
-000004d0: 2020 203a 7061 7261 6d20 6f70 7469 6d69     :param optimi
-000004e0: 7a65 723a 2073 7472 2c20 6f70 7469 6f6e  zer: str, option
-000004f0: 616c 0a20 2020 203a 7061 7261 6d20 7363  al.    :param sc
-00000500: 6865 6475 6c65 723a 2073 7472 2c20 6f70  heduler: str, op
-00000510: 7469 6f6e 616c 0a20 2020 203a 6361 6c6c  tional.    :call
-00000520: 6261 636b 733a 2055 6e69 6f6e 5b43 616c  backs: Union[Cal
-00000530: 6c61 626c 652c 2049 7465 7261 626c 655d  lable, Iterable]
-00000540: 2c20 6f70 7469 6f6e 616c 0a20 2020 203a  , optional.    :
-00000550: 6361 6c6c 6261 636b 5f73 7465 703a 2069  callback_step: i
-00000560: 6e74 2c20 6f70 7469 6f6e 616c 0a20 2020  nt, optional.   
-00000570: 203a 6361 6c6c 6261 636b 5f65 706f 6368   :callback_epoch
-00000580: 0a20 2020 204e a900 da06 6465 7669 6365  .    N....device
-00000590: da04 6d6f 6465 da09 6f70 7469 6d69 7a65  ..mode..optimize
-000005a0: 72da 0973 6368 6564 756c 6572 da09 6361  r..scheduler..ca
-000005b0: 6c6c 6261 636b 73da 0a77 6562 5f6c 6f67  llbacks..web_log
-000005c0: 6765 7263 0800 0000 0000 0000 0000 0000  gerc............
-000005d0: 0800 0000 0400 0000 4300 0000 73aa 0000  ........C...s...
-000005e0: 0064 017c 026a 0076 0072 0b74 016a 02a0  .d.|.j.v.r.t.j..
-000005f0: 037c 02a1 0101 007c 027c 005f 0464 025c  .|.....|.|._.d.\
-00000600: 037c 005f 057c 005f 067c 005f 0764 025c  .|._.|._.|._.d.\
-00000610: 037c 005f 087c 005f 097c 005f 0a7c 037c  .|._.|._.|._.|.|
-00000620: 005f 0b7c 047c 005f 0c7c 057c 005f 0d7c  ._.|.|._.|.|._.|
-00000630: 00a0 0e7c 01a1 017c 005f 0f74 1074 1183  ...|...|._.t.t..
-00000640: 0174 1074 1183 0102 027c 005f 127c 005f  .t.t.....|._.|._
-00000650: 1374 016a 1474 1074 1183 0102 027c 005f  .t.j.t.t.....|._
-00000660: 157c 005f 167c 067c 005f 1774 1883 007c  .|._.|.|._.t...|
-00000670: 005f 197c 0772 537c 00a0 1a7c 07a1 017c  ._.|.rS|...|...|
-00000680: 005f 1b64 0053 0064 0053 0029 034e da04  ._.d.S.d.S.).N..
-00000690: 6375 6461 2903 4e4e 4e29 1cda 0474 7970  cuda).NNN)...typ
-000006a0: 65da 0574 6f72 6368 7214 0000 00da 0a73  e..torchr......s
-000006b0: 6574 5f64 6576 6963 6572 0e00 0000 da06  et_devicer......
-000006c0: 6c6f 6164 6572 da06 6e5f 6461 7461 da0a  loader..n_data..
-000006d0: 6261 7463 685f 7369 7a65 da0c 7661 6c69  batch_size..vali
-000006e0: 645f 6c6f 6164 6572 da0c 6e5f 7661 6c69  d_loader..n_vali
-000006f0: 645f 6461 7461 da10 7661 6c69 645f 6261  d_data..valid_ba
-00000700: 7463 685f 7369 7a65 720f 0000 0072 1000  tch_sizer....r..
-00000710: 0000 7211 0000 00da 0a5f 746f 5f64 6576  ..r......_to_dev
-00000720: 6963 65da 056d 6f64 656c 7204 0000 00da  ice..modelr.....
-00000730: 046c 6973 74da 096c 6f67 5f74 7261 696e  .list..log_train
-00000740: da08 6c6f 675f 7465 7374 da03 696e 66da  ..log_test..inf.
-00000750: 0b6c 6f73 735f 6275 6666 6572 da0d 7765  .loss_buffer..we
-00000760: 6967 6874 5f62 7566 6665 7272 1200 0000  ight_bufferr....
-00000770: da0f 5072 6f67 7265 7373 4368 6563 6b65  ..ProgressChecke
-00000780: 72da 1070 726f 6772 6573 735f 6368 6563  r..progress_chec
-00000790: 6b65 72da 1063 6865 636b 5f77 6562 5f6c  ker..check_web_l
-000007a0: 6f67 6765 7272 1300 0000 2908 da04 7365  oggerr....)...se
-000007b0: 6c66 721f 0000 0072 0e00 0000 720f 0000  lfr....r....r...
-000007c0: 0072 1000 0000 7211 0000 0072 1200 0000  .r....r....r....
-000007d0: 7213 0000 0072 0d00 0000 720d 0000 00fa  r....r....r.....
-000007e0: 345a 3a5c 6465 762d 7a61 655c 7a61 652d  4Z:\dev-zae\zae-
-000007f0: 656e 6769 6e65 5c7a 6165 5f65 6e67 696e  engine\zae_engin
-00000800: 655c 7472 6169 6e65 725c 5f74 7261 696e  e\trainer\_train
-00000810: 6572 2e70 79da 085f 5f69 6e69 745f 5f1d  er.py..__init__.
-00000820: 0000 0073 2000 0000 0a0a 0c01 0601 1001  ...s ...........
-00000830: 1001 0601 0601 0601 0c01 1601 1401 0601  ................
-00000840: 0801 0401 1001 04ff 7a10 5472 6169 6e65  ........z.Traine
-00000850: 722e 5f5f 696e 6974 5f5f da06 7265 7475  r.__init__..retu
-00000860: 726e 2e63 0100 0000 0000 0000 0000 0000  rn.c............
-00000870: 0300 0000 0400 0000 0700 0000 736a 0000  ............sj..
-00000880: 0074 007c 0183 0164 016b 0272 2a7c 0164  .t.|...d.k.r*|.d
-00000890: 0219 007d 0274 017c 0274 026a 0383 0272  ...}.t.|.t.j...r
-000008a0: 2864 037c 02a0 04a1 0076 0072 1c7c 02a0  (d.|.....v.r.|..
-000008b0: 05a1 00a0 06a1 0053 0064 047c 02a0 04a1  .......S.d.|....
-000008c0: 0076 0072 267c 02a0 07a1 0053 007c 0253  .v.r&|.....S.|.S
-000008d0: 007c 0253 0074 0887 0066 0164 0564 0684  .|.S.t...f.d.d..
-000008e0: 087c 0144 0083 0183 0153 0029 087a cf0a  .|.D.....S.).z..
-000008f0: 2020 2020 2020 2020 4361 7374 2067 6976          Cast giv
-00000900: 656e 2061 7267 756d 656e 7473 2074 6f20  en arguments to 
-00000910: 6370 752e 0a20 2020 2020 2020 203a 7061  cpu..        :pa
-00000920: 7261 6d20 6172 6773 3a20 5369 6e67 6c65  ram args: Single
-00000930: 2061 7267 756d 656e 7420 6f72 2076 6172   argument or var
-00000940: 6961 626c 652d 6c65 6e67 7468 2073 6571  iable-length seq
-00000950: 7565 6e63 6520 6f66 2061 7267 756d 656e  uence of argumen
-00000960: 7473 2e0a 2020 2020 2020 2020 3a72 6574  ts..        :ret
-00000970: 7572 6e3a 2053 696e 676c 6520 6172 6775  urn: Single argu
-00000980: 6d65 6e74 206f 7220 7661 7269 6162 6c65  ment or variable
-00000990: 2d6c 656e 6774 6820 7365 7175 656e 6365  -length sequence
-000009a0: 206f 6620 6172 6775 6d65 6e74 7320 696e   of arguments in
-000009b0: 2063 7075 2e0a 2020 2020 2020 2020 720a   cpu..        r.
-000009c0: 0000 0072 0100 0000 da06 6465 7461 6368  ...r......detach
-000009d0: da04 6974 656d 6301 0000 0000 0000 0000  ..itemc.........
-000009e0: 0000 0002 0000 0005 0000 0013 0000 0073  ...............s
-000009f0: 1600 0000 6700 7c00 5d07 7d01 8800 a000  ....g.|.].}.....
-00000a00: 7c01 a101 9102 7102 5300 720d 0000 0029  |.....q.S.r....)
-00000a10: 01da 075f 746f 5f63 7075 a902 da02 2e30  ..._to_cpu.....0
-00000a20: da01 61a9 0172 2900 0000 720d 0000 0072  ..a..r)...r....r
-00000a30: 2a00 0000 da0a 3c6c 6973 7463 6f6d 703e  *.....<listcomp>
-00000a40: 4400 0000 7302 0000 0016 007a 2354 7261  D...s......z#Tra
-00000a50: 696e 6572 2e5f 746f 5f63 7075 2e3c 6c6f  iner._to_cpu.<lo
-00000a60: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
-00000a70: 4e29 09da 036c 656e da0a 6973 696e 7374  N)...len..isinst
-00000a80: 616e 6365 7216 0000 00da 0654 656e 736f  ancer......Tenso
-00000a90: 72da 075f 5f64 6972 5f5f 722d 0000 00da  r..__dir__r-....
-00000aa0: 0363 7075 722e 0000 00da 0574 7570 6c65  .cpur......tuple
-00000ab0: 2903 7229 0000 00da 0461 7267 7372 3200  ).r).....argsr2.
-00000ac0: 0000 720d 0000 0072 3300 0000 722a 0000  ..r....r3...r*..
-00000ad0: 0072 2f00 0000 3700 0000 730c 0000 000c  .r/...7...s.....
-00000ae0: 0608 010c 0130 0104 0216 027a 0f54 7261  .....0.....z.Tra
-00000af0: 696e 6572 2e5f 746f 5f63 7075 6301 0000  iner._to_cpuc...
-00000b00: 0000 0000 0000 0000 0003 0000 0004 0000  ................
-00000b10: 000f 0000 0073 6c00 0000 7c01 7227 7400  .....sl...|.r't.
-00000b20: 7c01 8301 6401 6b02 721c 6402 7c01 6403  |...d.k.r.d.|.d.
-00000b30: 1900 a001 a100 7600 7218 7c01 6403 1900  ......v.r.|.d...
-00000b40: a002 8800 6a03 a101 5300 7c01 6403 1900  ....j...S.|.d...
-00000b50: 5300 7404 8700 6601 6404 6405 8408 7c01  S.t...f.d.d...|.
-00000b60: 4400 8301 8301 5300 7c02 7234 8700 6601  D.....S.|.r4..f.
-00000b70: 6406 6407 8408 7c02 a005 a100 4400 8301  d.d...|.....D...
-00000b80: 5300 6408 5300 2909 7ad5 0a20 2020 2020  S.d.S.).z..     
-00000b90: 2020 2043 6173 7420 6769 7665 6e20 6172     Cast given ar
-00000ba0: 6775 6d65 6e74 7320 746f 2064 6576 6963  guments to devic
-00000bb0: 652e 0a20 2020 2020 2020 203a 7061 7261  e..        :para
-00000bc0: 6d20 6172 6773 3a20 5369 6e67 6c65 2061  m args: Single a
-00000bd0: 7267 756d 656e 7420 6f72 2076 6172 6961  rgument or varia
-00000be0: 626c 652d 6c65 6e67 7468 2073 6571 7565  ble-length seque
-00000bf0: 6e63 6520 6f66 2061 7267 756d 656e 7473  nce of arguments
-00000c00: 2e0a 2020 2020 2020 2020 3a72 6574 7572  ..        :retur
-00000c10: 6e3a 2053 696e 676c 6520 6172 6775 6d65  n: Single argume
-00000c20: 6e74 206f 7220 7661 7269 6162 6c65 2d6c  nt or variable-l
-00000c30: 656e 6774 6820 7365 7175 656e 6365 206f  ength sequence o
-00000c40: 6620 6172 6775 6d65 6e74 7320 696e 2064  f arguments in d
-00000c50: 6576 6963 652e 0a20 2020 2020 2020 2072  evice..        r
-00000c60: 0a00 0000 da02 746f 7201 0000 0063 0100  ......tor....c..
-00000c70: 0000 0000 0000 0000 0000 0200 0000 0500  ................
-00000c80: 0000 1300 0000 7328 0000 0067 007c 005d  ......s(...g.|.]
-00000c90: 107d 0164 007c 01a0 00a1 0076 0072 107c  .}.d.|.....v.r.|
-00000ca0: 01a0 0188 006a 02a1 016e 017c 0191 0271  .....j...n.|...q
-00000cb0: 0253 00a9 0172 3c00 0000 a903 7238 0000  .S...r<.....r8..
-00000cc0: 0072 3c00 0000 720e 0000 0072 3000 0000  .r<...r....r0...
-00000cd0: 7233 0000 0072 0d00 0000 722a 0000 0072  r3...r....r*...r
-00000ce0: 3400 0000 5200 0000 7302 0000 0028 007a  4...R...s....(.z
-00000cf0: 2654 7261 696e 6572 2e5f 746f 5f64 6576  &Trainer._to_dev
-00000d00: 6963 652e 3c6c 6f63 616c 733e 2e3c 6c69  ice.<locals>.<li
-00000d10: 7374 636f 6d70 3e63 0100 0000 0000 0000  stcomp>c........
-00000d20: 0000 0000 0300 0000 0600 0000 1300 0000  ................
-00000d30: 732e 0000 0069 007c 005d 135c 027d 017d  s....i.|.].\.}.}
-00000d40: 027c 0164 007c 02a0 00a1 0076 0072 137c  .|.d.|.....v.r.|
-00000d50: 02a0 0188 006a 02a1 016e 017c 0293 0271  .....j...n.|...q
-00000d60: 0253 0072 3d00 0000 723e 0000 0029 0372  .S.r=...r>...).r
-00000d70: 3100 0000 da01 6bda 0176 7233 0000 0072  1.....k..vr3...r
-00000d80: 0d00 0000 722a 0000 00da 0a3c 6469 6374  ....r*.....<dict
-00000d90: 636f 6d70 3e54 0000 0073 0200 0000 2e00  comp>T...s......
-00000da0: 7a26 5472 6169 6e65 722e 5f74 6f5f 6465  z&Trainer._to_de
-00000db0: 7669 6365 2e3c 6c6f 6361 6c73 3e2e 3c64  vice.<locals>.<d
-00000dc0: 6963 7463 6f6d 703e 4e29 0672 3500 0000  ictcomp>N).r5...
-00000dd0: 7238 0000 0072 3c00 0000 720e 0000 0072  r8...r<...r....r
-00000de0: 3a00 0000 da05 6974 656d 7329 0372 2900  :.....items).r).
-00000df0: 0000 723b 0000 00da 066b 7761 7267 7372  ..r;.....kwargsr
-00000e00: 0d00 0000 7233 0000 0072 2a00 0000 721e  ....r3...r*...r.
-00000e10: 0000 0046 0000 0073 0e00 0000 0408 0c01  ...F...s........
-00000e20: 2801 1602 0401 1601 04ff 7a12 5472 6169  (.........z.Trai
-00000e30: 6e65 722e 5f74 6f5f 6465 7669 6365 4663  ner._to_deviceFc
-00000e40: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00000e50: 0300 0000 4300 0000 7382 0000 007c 0172  ....C...s....|.r
-00000e60: 237c 006a 0064 0175 0172 0d7c 006a 006a  #|.j.d.u.r.|.j.j
-00000e70: 01a0 02a1 006e 0164 027c 005f 037c 006a  .....n.d.|._.|.j
-00000e80: 0464 0175 0172 1e7c 006a 046a 01a0 02a1  .d.u.r.|.j.j....
-00000e90: 007c 005f 0564 0153 0064 027c 005f 0564  .|._.d.S.d.|._.d
-00000ea0: 0153 007c 006a 0664 036b 0272 377c 006a  .S.|.j.d.k.r7|.j
-00000eb0: 0464 0175 0172 377c 0004 006a 057c 006a  .d.u.r7|...j.|.j
-00000ec0: 0738 0002 005f 0564 0153 007c 0004 006a  .8..._.d.S.|...j
-00000ed0: 037c 006a 0838 0002 005f 0364 0153 0029  .|.j.8..._.d.S.)
-00000ee0: 047a 350a 2020 2020 2020 2020 436f 756e  .z5.        Coun
-00000ef0: 7420 7468 6520 6e75 6d62 6572 206f 6620  t the number of 
-00000f00: 6461 7461 2069 6e20 6c6f 6164 6572 2e0a  data in loader..
-00000f10: 2020 2020 2020 2020 4e72 0100 0000 da04          Nr......
-00000f20: 7465 7374 2909 7218 0000 00da 0764 6174  test).r......dat
-00000f30: 6173 6574 da07 5f5f 6c65 6e5f 5f72 1900  aset..__len__r..
-00000f40: 0000 721b 0000 0072 1c00 0000 720f 0000  ..r....r....r...
-00000f50: 0072 1d00 0000 721a 0000 0029 0272 2900  .r....r....).r).
-00000f60: 0000 da07 696e 6974 6961 6c72 0d00 0000  ....initialr....
-00000f70: 720d 0000 0072 2a00 0000 da0b 5f64 6174  r....r*....._dat
-00000f80: 615f 636f 756e 7456 0000 0073 0c00 0000  a_countV...s....
-00000f90: 0404 1c01 2601 1402 1401 1402 7a13 5472  ....&.......z.Tr
-00000fa0: 6169 6e65 722e 5f64 6174 615f 636f 756e  ainer._data_coun
-00000fb0: 7463 0100 0000 0000 0000 0000 0000 0100  tc..............
-00000fc0: 0000 0200 0000 4300 0000 733a 0000 007c  ......C...s:...|
-00000fd0: 006a 0064 0175 0172 097c 006a 006a 016e  .j.d.u.r.|.j.j.n
-00000fe0: 0164 027c 005f 017c 006a 0264 0175 0172  .d.|._.|.j.d.u.r
-00000ff0: 187c 006a 026a 017c 005f 0364 0153 0064  .|.j.j.|._.d.S.d
-00001000: 027c 005f 0364 0153 0029 037a 2d0a 2020  .|._.d.S.).z-.  
-00001010: 2020 2020 2020 4368 6563 6b20 6261 7463        Check batc
-00001020: 6820 7369 7a65 206f 6620 6c6f 6164 6572  h size of loader
-00001030: 2e0a 2020 2020 2020 2020 4e72 0100 0000  ..        Nr....
-00001040: 2904 7218 0000 0072 1a00 0000 721b 0000  ).r....r....r...
-00001050: 0072 1d00 0000 7233 0000 0072 0d00 0000  .r....r3...r....
-00001060: 720d 0000 0072 2a00 0000 da11 5f63 6865  r....r*....._che
-00001070: 636b 5f62 6174 6368 5f73 697a 6563 0000  ck_batch_sizec..
-00001080: 0073 0400 0000 1804 2201 7a19 5472 6169  .s......".z.Trai
-00001090: 6e65 722e 5f63 6865 636b 5f62 6174 6368  ner._check_batch
-000010a0: 5f73 697a 65da 076e 5f65 706f 6368 6304  _size..n_epochc.
-000010b0: 0000 0000 0000 0000 0000 0007 0000 0005  ................
-000010c0: 0000 004b 0000 0073 c600 0000 7c02 7c03  ...K...s....|.|.
-000010d0: 0202 7c00 5f00 7c00 5f01 7c00 a002 a100  ..|._.|._.|.....
-000010e0: 0100 7403 7c01 8301 4400 5d51 7d05 7404  ..t.|...D.]Q}.t.
-000010f0: 6401 7c05 6402 1700 1600 8301 0100 7c00  d.|.d.........|.
-00001100: 6a05 6403 6404 8d01 0100 7c00 a006 7c02  j.d.d.....|...|.
-00001110: a101 0100 7c03 7233 7c00 a007 a100 0100  ....|.r3|.......
-00001120: 7c00 a006 7c03 a101 0100 7c00 a007 a100  |...|.....|.....
-00001130: 0100 7c00 6a08 6405 6b02 7260 7409 a00a  ..|.j.d.k.r`t...
-00001140: 7c03 7241 7c00 6a0b 6406 1900 6e04 7c00  |.rA|.j.d...n.|.
-00001150: 6a0c 6406 1900 a101 a00d a100 7d06 7c00  j.d.........}.|.
-00001160: 6a0e 7c05 6402 1700 7c06 6407 8d02 0100  j.|.d...|.d.....
-00001170: 7c00 6a0f 6a10 6409 6900 7c04 a401 8e01  |.j.j.d.i.|.....
-00001180: 0100 7c00 6a11 a012 a100 0100 710f 6408  ..|.j.......q.d.
-00001190: 5300 290a 7ae9 0a20 2020 2020 2020 2052  S.).z..        R
-000011a0: 756e 2066 6f72 2061 2067 6976 656e 206c  un for a given l
-000011b0: 6f61 6465 722e 0a20 2020 2020 2020 2049  oader..        I
-000011c0: 6620 7661 6c69 645f 6c6f 6164 6572 2069  f valid_loader i
-000011d0: 7320 6e6f 7420 4e6f 6e65 2c20 7468 6520  s not None, the 
-000011e0: 6d6f 6465 6c20 6576 616c 7561 7465 7320  model evaluates 
-000011f0: 7468 6520 6461 7461 2069 6e20 7661 6c69  the data in vali
-00001200: 645f 6c6f 6164 6572 2066 6f72 2065 7665  d_loader for eve
-00001210: 7279 2065 706f 6368 2e0a 2020 2020 2020  ry epoch..      
-00001220: 2020 3a70 6172 616d 206e 5f65 706f 6368    :param n_epoch
-00001230: 3a0a 2020 2020 2020 2020 3a70 6172 616d  :.        :param
-00001240: 206c 6f61 6465 723a 0a20 2020 2020 2020   loader:.       
-00001250: 203a 7061 7261 6d20 7661 6c69 645f 6c6f   :param valid_lo
-00001260: 6164 6572 3a0a 2020 2020 2020 2020 3a72  ader:.        :r
-00001270: 6574 7572 6e3a 0a20 2020 2020 2020 207a  eturn:.        z
-00001280: 0845 706f 6368 2025 6472 0a00 0000 5429  .Epoch %dr....T)
-00001290: 0172 4700 0000 da05 7472 6169 6eda 046c  .rG.....train..l
-000012a0: 6f73 7329 02da 0963 7572 5f65 706f 6368  oss)...cur_epoch
-000012b0: da08 6375 725f 6c6f 7373 4e72 0d00 0000  ..cur_lossNr....
-000012c0: 2913 7218 0000 0072 1b00 0000 7249 0000  ).r....r....rI..
-000012d0: 00da 0572 616e 6765 da05 7072 696e 7472  ...range..printr
-000012e0: 4800 0000 da09 7275 6e5f 6570 6f63 68da  H.....run_epoch.
-000012f0: 0674 6f67 676c 6572 0f00 0000 da02 6e70  .toggler......np
-00001300: da04 6d65 616e 7222 0000 0072 2100 0000  ..meanr"...r!...
-00001310: 722e 0000 00da 0c63 6865 636b 5f62 6574  r......check_bet
-00001320: 7465 7272 1100 0000 da04 7374 6570 7227  terr......stepr'
-00001330: 0000 00da 0c75 7064 6174 655f 6570 6f63  .....update_epoc
-00001340: 6829 0772 2900 0000 724a 0000 0072 1800  h).r)...rJ...r..
-00001350: 0000 721b 0000 0072 4300 0000 da01 6572  ..r....rC.....er
-00001360: 4e00 0000 720d 0000 0072 0d00 0000 722a  N...r....r....r*
-00001370: 0000 00da 0372 756e 6a00 0000 7322 0000  .....runj...s"..
-00001380: 000e 0908 010c 0110 010c 010a 0104 0108  ................
-00001390: 010a 0108 010a 0122 0112 0112 010a 0102  ......."........
-000013a0: 8004 f47a 0b54 7261 696e 6572 2e72 756e  ...z.Trainer.run
-000013b0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-000013c0: 0003 0000 0043 0000 0073 2200 0000 7c00  .....C...s"...|.
-000013d0: 6a00 720d 7c00 6a00 4400 5d08 7d01 7c01  j.r.|.j.D.].}.|.
-000013e0: 7c00 8301 0100 7106 6400 5300 6400 5300  |.....q.d.S.d.S.
-000013f0: a901 4e29 0172 1200 0000 2902 7229 0000  ..N).r....).r)..
-00001400: 00da 0263 6272 0d00 0000 720d 0000 0072  ...cbr....r....r
-00001410: 2a00 0000 da0c 7275 6e5f 6361 6c6c 6261  *.....run_callba
-00001420: 636b 8300 0000 730a 0000 0006 010a 010a  ck....s.........
-00001430: 0104 fe04 017a 1454 7261 696e 6572 2e72  .....z.Trainer.r
-00001440: 756e 5f63 616c 6c62 6163 6b63 0200 0000  un_callbackc....
-00001450: 0000 0000 0000 0000 0400 0000 0500 0000  ................
-00001460: 4300 0000 7346 0000 007c 00a0 00a1 0001  C...sF...|......
-00001470: 0074 017c 0183 0144 005d 185c 027d 027d  .t.|...D.].\.}.}
-00001480: 037c 00a0 027c 03a1 0101 007c 00a0 03a1  .|...|.....|....
-00001490: 0001 007c 006a 047c 0264 0117 0074 057c  ...|.j.|.d...t.|
-000014a0: 0183 0164 028d 0201 0071 0864 0053 0029  ...d.....q.d.S.)
-000014b0: 034e 720a 0000 0029 02da 0963 7572 5f62  .Nr....)...cur_b
-000014c0: 6174 6368 da09 6e75 6d5f 6261 7463 6829  atch..num_batch)
-000014d0: 06da 096c 6f67 5f72 6573 6574 da09 656e  ...log_reset..en
-000014e0: 756d 6572 6174 65da 0972 756e 5f62 6174  umerate..run_bat
-000014f0: 6368 7248 0000 00da 0970 7269 6e74 5f6c  chrH.....print_l
-00001500: 6f67 7235 0000 0029 0472 2900 0000 7218  ogr5...).r)...r.
-00001510: 0000 00da 0169 da05 6261 7463 6872 0d00  .....i..batchr..
-00001520: 0000 720d 0000 0072 2a00 0000 7251 0000  ..r....r*...rQ..
-00001530: 0088 0000 0073 0c00 0000 0801 1001 0a01  .....s..........
-00001540: 0801 1801 04fd 7a11 5472 6169 6e65 722e  ......z.Trainer.
-00001550: 7275 6e5f 6570 6f63 6872 6400 0000 6302  run_epochrd...c.
-00001560: 0000 0000 0000 0000 0000 0003 0000 0008  ................
-00001570: 0000 0043 0000 0073 de00 0000 7400 7c01  ...C...s....t.|.
-00001580: 7401 8302 720d 7c00 6a02 6407 6900 7c01  t...r.|.j.d.i.|.
-00001590: a401 8e01 6e04 7c00 6a02 7c01 8e00 7d01  ....n.|.j.|...}.
-000015a0: 7c00 6a03 6401 6b02 7232 7c00 6a04 a005  |.j.d.k.r2|.j...
-000015b0: a100 0100 7c00 6a06 a007 a100 0100 7c00  ....|.j.......|.
-000015c0: a008 7c01 a101 7d02 7c02 6402 1900 a009  ..|...}.|.d.....
-000015d0: a100 0100 7c00 6a06 a00a a100 0100 6e2d  ....|.j.......n-
-000015e0: 7c00 6a03 6403 6b02 7256 7c00 6a04 a00b  |.j.d.k.rV|.j...
-000015f0: a100 0100 740c a00d a100 8f0d 0100 7c00  ....t.........|.
-00001600: a00e 7c01 a101 7d02 5700 6404 0400 0400  ..|...}.W.d.....
-00001610: 8303 0100 6e12 3100 7350 7701 0100 0100  ....n.1.sPw.....
-00001620: 0100 5900 0100 6e09 740f 6405 7c00 6a03  ..Y...n.t.d.|.j.
-00001630: 9b00 6406 9d03 8301 8201 7c00 a010 7c02  ..d.......|...|.
-00001640: a101 0100 7c00 6a11 a012 a100 0100 7c00  ....|.j.......|.
-00001650: a013 a100 0100 6404 5300 2908 7a2d 0a20  ......d.S.).z-. 
-00001660: 2020 2020 2020 2052 756e 2066 6f72 2061         Run for a
-00001670: 2062 6174 6368 2028 6e6f 7420 6570 6f63   batch (not epoc
-00001680: 6829 0a20 2020 2020 2020 2072 4b00 0000  h).        rK...
-00001690: 724c 0000 0072 4400 0000 4efa 1055 6e65  rL...rD...N..Une
-000016a0: 7870 6563 7465 6420 6d6f 6465 20da 012e  xpected mode ...
-000016b0: 720d 0000 0029 1472 3600 0000 da04 6469  r....).r6.....di
-000016c0: 6374 721e 0000 0072 0f00 0000 721f 0000  ctr....r....r...
-000016d0: 0072 4b00 0000 7210 0000 00da 097a 6572  .rK...r......zer
-000016e0: 6f5f 6772 6164 da0a 7472 6169 6e5f 7374  o_grad..train_st
-000016f0: 6570 da08 6261 636b 7761 7264 7256 0000  ep..backwardrV..
-00001700: 00da 0465 7661 6c72 1600 0000 da07 6e6f  ...evalr......no
-00001710: 5f67 7261 64da 0974 6573 745f 7374 6570  _grad..test_step
-00001720: da0a 5661 6c75 6545 7272 6f72 da07 6c6f  ..ValueError..lo
-00001730: 6767 696e 6772 2700 0000 da0b 7570 6461  ggingr'.....upda
-00001740: 7465 5f73 7465 7072 5c00 0000 2903 7229  te_stepr\...).r)
-00001750: 0000 0072 6400 0000 da09 7374 6570 5f64  ...rd.....step_d
-00001760: 6963 7472 0d00 0000 720d 0000 0072 2a00  ictr....r....r*.
-00001770: 0000 7261 0000 008f 0000 0073 2000 0000  ..ra.......s ...
-00001780: 2404 0a01 0a01 0a01 0a01 0c01 0c01 0a02  $...............
-00001790: 0a01 0a01 0c01 1eff 1203 0a02 0a01 0c01  ................
-000017a0: 7a11 5472 6169 6e65 722e 7275 6e5f 6261  z.Trainer.run_ba
-000017b0: 7463 6863 0200 0000 0000 0000 0000 0000  tchc............
-000017c0: 0700 0000 0400 0000 4300 0000 f332 0000  ........C....2..
-000017d0: 007c 015c 037d 027d 037d 047c 00a0 007c  .|.\.}.}.}.|...|
-000017e0: 02a1 017d 0564 0167 0174 017c 0283 0114  ...}.d.g.t.|....
-000017f0: 007d 067c 0674 02a0 037c 05a1 0164 029c  .}.|.t...|...d..
-00001800: 0253 0029 0461 7601 0000 0a20 2020 2020  .S.).av....     
-00001810: 2020 2055 6e75 7365 6420 6475 6d6d 7920     Unused dummy 
-00001820: 6675 6e63 7469 6f6e 2079 6574 2065 7869  function yet exi
-00001830: 7374 2074 6f20 7072 6f76 6964 6520 492f  st to provide I/
-00001840: 4f20 666f 726d 6174 2069 6e66 6f72 6d61  O format informa
-00001850: 7469 6f6e 2e0a 2020 2020 2020 2020 5468  tion..        Th
-00001860: 6520 6261 7463 6820 6973 2061 2070 6172  e batch is a par
-00001870: 7420 6f66 2074 6865 2064 6174 6173 6574  t of the dataset
-00001880: 2069 6e20 7468 6520 6461 7461 6c6f 6164   in the dataload
-00001890: 6572 2066 6574 6368 6564 2076 6961 2020  er fetched via  
-000018a0: 5f5f 6765 7469 7465 6d5f 5f20 6d65 7468  __getitem__ meth
-000018b0: 6f64 2e0a 2020 2020 2020 2020 5468 6520  od..        The 
-000018c0: 6469 6374 696f 6e61 7279 2063 6f6e 7369  dictionary consi
-000018d0: 7374 7320 6f66 207b 2773 7472 273a 2074  sts of {'str': t
-000018e0: 6f72 6368 2e74 656e 736f 7228 7661 6c75  orch.tensor(valu
-000018f0: 6529 7d2c 2061 6e64 206d 7573 7420 696e  e)}, and must in
-00001900: 636c 7564 6520 276c 6f73 7327 2e0a 2020  clude 'loss'..  
-00001910: 2020 2020 2020 4e6f 7465 2074 6861 7420        Note that 
-00001920: 7468 6973 2066 756e 6374 696f 6e20 776f  this function wo
-00001930: 726b 206f 6e6c 7920 696e 2027 7472 6169  rk only in 'trai
-00001940: 6e27 206d 6f64 652c 2068 656e 6365 2062  n' mode, hence b
-00001950: 6163 6b28 2920 6d65 7468 6f64 2069 6e20  ack() method in 
-00001960: 6e6e 2e4d 6f64 756c 6520 6973 206e 6563  nn.Module is nec
-00001970: 6573 7361 7279 2e0a 2020 2020 2020 2020  essary..        
-00001980: e700 0000 0000 0000 00a9 0272 4c00 0000  ...........rL...
-00001990: 7254 0000 004e a904 721f 0000 0072 3500  rT...N..r....r5.
-000019a0: 0000 7216 0000 0072 5400 0000 a907 7229  ..r....rT.....r)
-000019b0: 0000 0072 6400 0000 da01 78da 0179 da02  ...rd.....x..y..
-000019c0: 666e da07 6f75 7470 7574 7372 4c00 0000  fn..outputsrL...
-000019d0: 720d 0000 0072 0d00 0000 722a 0000 0072  r....r....r*...r
-000019e0: 6900 0000 a600 0000 f308 0000 000a 080a  i...............
-000019f0: 010e 0110 017a 1254 7261 696e 6572 2e74  .....z.Trainer.t
-00001a00: 7261 696e 5f73 7465 7063 0200 0000 0000  rain_stepc......
-00001a10: 0000 0000 0000 0700 0000 0400 0000 4300  ..............C.
-00001a20: 0000 7272 0000 0029 0461 4601 0000 0a20  ..rr...).aF.... 
-00001a30: 2020 2020 2020 2055 6e75 7365 6420 6475         Unused du
-00001a40: 6d6d 7920 6675 6e63 7469 6f6e 2079 6574  mmy function yet
-00001a50: 2065 7869 7374 2074 6f20 7072 6f76 6964   exist to provid
-00001a60: 6520 492f 4f20 666f 726d 6174 2069 6e66  e I/O format inf
-00001a70: 6f72 6d61 7469 6f6e 2e0a 2020 2020 2020  ormation..      
-00001a80: 2020 5468 6520 6261 7463 6820 6973 2061    The batch is a
-00001a90: 2070 6172 7420 6f66 2074 6865 2064 6174   part of the dat
-00001aa0: 6173 6574 2069 6e20 7468 6520 6461 7461  aset in the data
-00001ab0: 6c6f 6164 6572 2066 6574 6368 6564 2076  loader fetched v
-00001ac0: 6961 2020 5f5f 6765 7469 7465 6d5f 5f20  ia  __getitem__ 
-00001ad0: 6d65 7468 6f64 2e0a 2020 2020 2020 2020  method..        
-00001ae0: 5468 6520 6469 6374 696f 6e61 7279 2063  The dictionary c
-00001af0: 6f6e 7369 7374 7320 6f66 207b 2773 7472  onsists of {'str
-00001b00: 273a 2074 6f72 6368 2e74 656e 736f 7228  ': torch.tensor(
-00001b10: 7661 6c75 6529 7d2c 2061 6e64 206d 7573  value)}, and mus
-00001b20: 7420 696e 636c 7564 6520 276c 6f73 7327  t include 'loss'
-00001b30: 2e0a 2020 2020 2020 2020 4e6f 7465 2074  ..        Note t
-00001b40: 6861 7420 7468 6973 2066 756e 6374 696f  hat this functio
-00001b50: 6e20 776f 726b 206f 6e6c 7920 696e 2027  n work only in '
-00001b60: 7465 7374 2720 6d6f 6465 2e0a 2020 2020  test' mode..    
-00001b70: 2020 2020 7273 0000 0072 7400 0000 4e72      rs...rt...Nr
-00001b80: 7500 0000 7276 0000 0072 0d00 0000 720d  u...rv...r....r.
-00001b90: 0000 0072 2a00 0000 726d 0000 00b3 0000  ...r*...rm......
-00001ba0: 0072 7b00 0000 7a11 5472 6169 6e65 722e  .r{...z.Trainer.
-00001bb0: 7465 7374 5f73 7465 7072 7100 0000 6302  test_steprq...c.
-00001bc0: 0000 0000 0000 0000 0000 0004 0000 0006  ................
-00001bd0: 0000 0043 0000 0073 6a00 0000 7c01 a000  ...C...sj...|...
-00001be0: a100 4400 5d2e 5c02 7d02 7d03 7c00 6a01  ..D.].\.}.}.|.j.
-00001bf0: 6401 6b02 7219 7c00 6a02 7c02 1900 a003  d.k.r.|.j.|.....
-00001c00: 7c00 a004 7c03 a101 a101 0100 7104 7c00  |...|.......q.|.
-00001c10: 6a01 6402 6b02 722a 7c00 6a05 7c02 1900  j.d.k.r*|.j.|...
-00001c20: a003 7c00 a004 7c03 a101 a101 0100 7104  ..|...|.......q.
-00001c30: 7406 6403 7c00 6a01 9b00 6404 9d03 8301  t.d.|.j...d.....
-00001c40: 8201 6400 5300 2905 4e72 4b00 0000 7244  ..d.S.).NrK...rD
-00001c50: 0000 0072 6500 0000 7266 0000 0029 0772  ...re...rf...).r
-00001c60: 4200 0000 720f 0000 0072 2100 0000 da06  B...r....r!.....
-00001c70: 6170 7065 6e64 722f 0000 0072 2200 0000  appendr/...r"...
-00001c80: 726e 0000 0029 0472 2900 0000 7271 0000  rn...).r)...rq..
-00001c90: 0072 3f00 0000 7240 0000 0072 0d00 0000  .r?...r@...r....
-00001ca0: 720d 0000 0072 2a00 0000 726f 0000 00c0  r....r*...ro....
-00001cb0: 0000 0073 0e00 0000 1001 0a01 1801 0a01  ...s............
-00001cc0: 1801 1202 04fa 7a0f 5472 6169 6e65 722e  ......z.Trainer.
-00001cd0: 6c6f 6767 696e 6763 0200 0000 0000 0000  loggingc........
-00001ce0: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
-00001cf0: 7326 0000 007c 0172 077c 017c 005f 0064  s&...|.r.|.|._.d
-00001d00: 0353 007c 006a 0064 016b 0272 0e64 026e  .S.|.j.d.k.r.d.n
-00001d10: 0164 017c 005f 0064 0353 0029 047a 460a  .d.|._.d.S.).zF.
-00001d20: 2020 2020 2020 2020 5377 6974 6368 696e          Switchin
-00001d30: 6720 6d6f 6465 2069 6e20 696e 7374 616e  g mode in instan
-00001d40: 6365 2e0a 2020 2020 2020 2020 3a70 6172  ce..        :par
-00001d50: 616d 206d 6f64 653a 2073 7472 0a20 2020  am mode: str.   
-00001d60: 2020 2020 2072 4b00 0000 7244 0000 004e       rK...rD...N
-00001d70: 2901 720f 0000 0029 0272 2900 0000 720f  ).r....).r)...r.
-00001d80: 0000 0072 0d00 0000 720d 0000 0072 2a00  ...r....r....r*.
-00001d90: 0000 7252 0000 00c9 0000 0073 0600 0000  ..rR.......s....
-00001da0: 0405 0a01 1802 7a0e 5472 6169 6e65 722e  ......z.Trainer.
-00001db0: 746f 6767 6c65 724d 0000 0072 4e00 0000  togglerM...rN...
-00001dc0: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
-00001dd0: 0004 0000 0043 0000 0073 3800 0000 7c02  .....C...s8...|.
-00001de0: 7c00 6a00 6b04 7207 6401 5300 7c00 6a01  |.j.k.r.d.S.|.j.
-00001df0: 6402 1900 a002 7c01 a101 0100 7c00 6a01  d.....|.....|.j.
-00001e00: 6403 1900 a002 7c00 6a03 a004 a100 a101  d.....|.j.......
-00001e10: 0100 6401 5300 2904 7aa0 0a20 2020 2020  ..d.S.).z..     
-00001e20: 2020 2043 6f6d 7061 7265 2074 6865 2063     Compare the c
-00001e30: 7572 7265 6e74 206d 6f64 656c 2061 6e64  urrent model and
-00001e40: 2074 6865 2069 6e2d 6275 6666 6572 206d   the in-buffer m
-00001e50: 6f64 656c 2e0a 2020 2020 2020 2020 5468  odel..        Th
-00001e60: 6520 6372 6974 6572 696f 6e20 6973 206c  e criterion is l
-00001e70: 6f73 732e 0a20 2020 2020 2020 203a 7061  oss..        :pa
-00001e80: 7261 6d20 6375 725f 6570 6f63 683a 2069  ram cur_epoch: i
-00001e90: 6e74 0a20 2020 2020 2020 203a 7061 7261  nt.        :para
-00001ea0: 6d20 6375 725f 6c6f 7373 3a20 666c 6f61  m cur_loss: floa
-00001eb0: 740a 2020 2020 2020 2020 4eda 0565 706f  t.        N..epo
-00001ec0: 6368 da06 7765 6967 6874 2905 7224 0000  ch..weight).r$..
-00001ed0: 0072 2500 0000 727c 0000 0072 1f00 0000  .r%...r|...r....
-00001ee0: da0a 7374 6174 655f 6469 6374 2903 7229  ..state_dict).r)
-00001ef0: 0000 0072 4d00 0000 724e 0000 0072 0d00  ...rM...rN...r..
-00001f00: 0000 720d 0000 0072 2a00 0000 7255 0000  ..r....r*...rU..
-00001f10: 00d3 0000 0073 0800 0000 0a07 0401 1001  .....s..........
-00001f20: 1a01 7a14 5472 6169 6e65 722e 6368 6563  ..z.Trainer.chec
-00001f30: 6b5f 6265 7474 6572 6301 0000 0000 0000  k_betterc.......
-00001f40: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
-00001f50: 0073 1800 0000 7c00 6a00 a001 a100 0100  .s....|.j.......
-00001f60: 7c00 6a02 a001 a100 0100 6401 5300 2902  |.j.......d.S.).
-00001f70: 7a20 0a20 2020 2020 2020 2043 6c65 6172  z .        Clear
-00001f80: 2074 6865 206c 6f67 2e0a 2020 2020 2020   the log..      
-00001f90: 2020 4e29 0372 2100 0000 da05 636c 6561    N).r!.....clea
-00001fa0: 7272 2200 0000 7233 0000 0072 0d00 0000  rr"...r3...r....
-00001fb0: 720d 0000 0072 2a00 0000 725f 0000 00df  r....r*...r_....
-00001fc0: 0000 0073 0400 0000 0a04 0e01 7a11 5472  ...s........z.Tr
-00001fd0: 6169 6e65 722e 6c6f 675f 7265 7365 7472  ainer.log_resetr
-00001fe0: 5d00 0000 725e 0000 0063 0300 0000 0000  ]...r^...c......
-00001ff0: 0000 0000 0000 0b00 0000 0800 0000 4300  ..............C.
-00002000: 0000 73bc 0000 007c 006a 0064 016b 0272  ..s....|.j.d.k.r
-00002010: 087c 006a 016e 027c 006a 027d 037c 006a  .|.j.n.|.j.}.|.j
-00002020: 0372 167c 006a 036a 0464 0219 0064 0319  .r.|.j.j.d...d..
-00002030: 006e 0164 027d 047c 017c 026b 027d 057c  .n.d.}.|.|.k.}.|
-00002040: 0572 2064 006e 0274 056a 067d 067c 0572  .r d.n.t.j.}.|.r
-00002050: 2764 046e 0164 057d 0764 067c 019b 0064  'd.n.d.}.d.|...d
-00002060: 077c 029b 009d 047d 087c 03a0 07a1 0044  .|.....}.|.....D
-00002070: 005d 175c 027d 097d 0a64 087c 0976 0072  .].\.}.}.d.|.v.r
-00002080: 3e71 357c 0864 097c 099b 0064 0a74 08a0  >q5|.d.|...d.t..
-00002090: 097c 0aa1 0164 0b9b 049d 0437 007d 0871  .|...d.....7.}.q
-000020a0: 357c 0864 0c7c 0464 0d9b 049d 0237 007d  5|.d.|.d.....7.}
-000020b0: 0874 0a7c 087c 077c 0664 0e8d 0301 0064  .t.|.|.|.d.....d
-000020c0: 0053 0029 0f4e 724b 0000 0072 0100 0000  .S.).NrK...r....
-000020d0: da02 6c72 da01 0ada 007a 0a0d 0909 4261  ..lr.....z....Ba
-000020e0: 7463 683a 20fa 012f da06 6f75 7470 7574  tch: ../..output
-000020f0: da01 097a 023a 207a 032e 3666 7a05 094c  ...z.: z..6fz..L
-00002100: 523a 207a 032e 3365 2902 da03 656e 64da  R: z..3e)...end.
-00002110: 0466 696c 6529 0b72 0f00 0000 7221 0000  .file).r....r!..
-00002120: 0072 2200 0000 7210 0000 00da 0c70 6172  .r"...r......par
-00002130: 616d 5f67 726f 7570 73da 0373 7973 da06  am_groups..sys..
-00002140: 7374 6465 7272 7242 0000 0072 5300 0000  stderrrB...rS...
-00002150: 7254 0000 0072 5000 0000 290b 7229 0000  rT...rP...).r)..
-00002160: 0072 5d00 0000 725e 0000 00da 036c 6f67  .r]...r^.....log
-00002170: 5a02 4c52 5a06 6973 5f65 6e64 da04 6469  Z.LRZ.is_end..di
-00002180: 7370 7287 0000 005a 076c 6f67 5f73 7472  spr....Z.log_str
-00002190: 723f 0000 0072 4000 0000 720d 0000 0072  r?...r@...r....r
-000021a0: 0d00 0000 722a 0000 0072 6200 0000 e600  ....r*...rb.....
-000021b0: 0000 7318 0000 0016 011a 0108 010e 010c  ..s.............
-000021c0: 0110 0210 0108 0102 011e 0110 0112 017a  ...............z
-000021d0: 1154 7261 696e 6572 2e70 7269 6e74 5f6c  .Trainer.print_l
-000021e0: 6f67 da08 6669 6c65 6e61 6d65 6302 0000  og..filenamec...
-000021f0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00002200: 0043 0000 0073 1600 0000 7400 a001 7c00  .C...s....t...|.
-00002210: 6a02 a003 a100 7c01 a102 0100 6400 5300  j.....|.....d.S.
-00002220: 725a 0000 0029 0472 1600 0000 da04 7361  rZ...).r......sa
-00002230: 7665 721f 0000 0072 7f00 0000 2902 7229  ver....r....).r)
-00002240: 0000 0072 8e00 0000 720d 0000 0072 0d00  ...r....r....r..
-00002250: 0000 722a 0000 00da 0a73 6176 655f 6d6f  ..r*.....save_mo
-00002260: 6465 6cf5 0000 0073 0200 0000 1601 7a12  del....s......z.
-00002270: 5472 6169 6e65 722e 7361 7665 5f6d 6f64  Trainer.save_mod
-00002280: 656c 54da 0673 7472 6963 7463 0300 0000  elT..strictc....
-00002290: 0000 0000 0000 0000 0500 0000 0a00 0000  ................
-000022a0: 4300 0000 73a4 0000 007a 1f7c 0172 0e74  C...s....z.|.r.t
-000022b0: 006a 017c 0174 00a0 0264 01a1 0164 028d  .j.|.t...d...d..
-000022c0: 027d 036e 077c 006a 0364 0319 0064 0419  .}.n.|.j.d...d..
-000022d0: 007d 037c 006a 046a 057c 037c 0264 058d  .}.|.j.j.|.|.d..
-000022e0: 0201 0057 0064 0753 0004 0074 0679 3a01  ...W.d.S...t.y:.
-000022f0: 007d 0401 007a 0f74 0764 067c 019b 009d  .}...z.t.d.|....
-00002300: 027c 0483 0201 0057 0059 0064 077d 047e  .|.....W.Y.d.}.~
-00002310: 0464 0753 0064 077d 047e 0477 0104 0074  .d.S.d.}.~.w...t
-00002320: 0879 5101 007d 0401 007a 0c74 0764 087c  .yQ..}...z.t.d.|
-00002330: 0483 0201 0057 0059 0064 077d 047e 0464  .....W.Y.d.}.~.d
-00002340: 0753 0064 077d 047e 0477 0177 0029 0961  .S.d.}.~.w.w.).a
-00002350: 0401 0000 0a20 2020 2020 2020 2055 7064  .....        Upd
-00002360: 6174 6520 6d6f 6465 6c27 7320 7765 6967  ate model's weig
-00002370: 6874 732e 0a20 2020 2020 2020 2049 6620  hts..        If 
-00002380: 6669 6c65 6e61 6d65 2069 7320 4e6f 6e65  filename is None
-00002390: 2c20 6d6f 6465 6c20 7570 6461 7465 6420  , model updated 
-000023a0: 7769 7468 206c 6174 6573 7420 7765 6967  with latest weig
-000023b0: 6874 2062 7566 6665 7220 696e 2074 6865  ht buffer in the
-000023c0: 2069 6e73 7461 6e63 652e 0a20 2020 2020   instance..     
-000023d0: 2020 2049 6620 6e6f 742c 2074 6865 206d     If not, the m
-000023e0: 6f64 656c 2069 7320 7570 6461 7465 6420  odel is updated 
-000023f0: 7769 7468 2077 6569 6768 7473 206c 6f61  with weights loa
-00002400: 6465 6420 6672 6f6d 2074 6865 2066 696c  ded from the fil
-00002410: 656e 616d 652e 0a20 2020 2020 2020 203a  ename..        :
-00002420: 7061 7261 6d20 6669 6c65 6e61 6d65 3a20  param filename: 
-00002430: 7374 720a 2020 2020 2020 2020 3a70 6172  str.        :par
-00002440: 616d 2073 7472 6963 743a 2062 6f6f 6c0a  am strict: bool.
-00002450: 2020 2020 2020 2020 7239 0000 0029 01da          r9...)..
-00002460: 0c6d 6170 5f6c 6f63 6174 696f 6e72 7e00  .map_locationr~.
-00002470: 0000 e9ff ffff ff29 0172 9100 0000 7a11  .......).r....z.
-00002480: 4361 6e6e 6f74 2066 696e 6420 6669 6c65  Cannot find file
-00002490: 204e 7a28 5468 6572 6520 6973 206e 6f20   Nz(There is no 
-000024a0: 7765 6967 6874 2069 6e20 6275 6666 6572  weight in buffer
-000024b0: 206f 6620 7472 6169 6e65 722e 2909 7216   of trainer.).r.
-000024c0: 0000 00da 046c 6f61 6472 0e00 0000 7225  .....loadr....r%
-000024d0: 0000 0072 1f00 0000 da0f 6c6f 6164 5f73  ...r......load_s
-000024e0: 7461 7465 5f64 6963 74da 1146 696c 654e  tate_dict..FileN
-000024f0: 6f74 466f 756e 6445 7272 6f72 7250 0000  otFoundErrorrP..
-00002500: 00da 0a49 6e64 6578 4572 726f 7229 0572  ...IndexError).r
-00002510: 2900 0000 728e 0000 0072 9100 0000 da07  )...r....r......
-00002520: 7765 6967 6874 7372 5800 0000 720d 0000  weightsrX...r...
-00002530: 0072 0d00 0000 722a 0000 00da 0d61 7070  .r....r*.....app
-00002540: 6c79 5f77 6569 6768 7473 f800 0000 7318  ly_weights....s.
-00002550: 0000 0002 0804 0116 010e 0216 010e 011e  ................
-00002560: 0108 800e 0118 0108 8002 ff7a 1554 7261  ...........z.Tra
-00002570: 696e 6572 2e61 7070 6c79 5f77 6569 6768  iner.apply_weigh
-00002580: 7473 6302 0000 0000 0000 0000 0000 0005  tsc.............
-00002590: 0000 0005 0000 0043 0000 0073 7e00 0000  .......C...s~...
-000025a0: 7400 6401 8301 7d02 7c01 a001 a100 4400  t.d...}.|.....D.
-000025b0: 5d34 5c02 7d03 7d04 7c03 a002 a100 6402  ]4\.}.}.|.....d.
-000025c0: 7600 7224 7403 7c04 7404 8302 721f 7405  v.r$t.|.t...r.t.
-000025d0: 6a06 6406 6900 7c04 a401 8e01 6e01 7c04  j.d.i.|.....n.|.
-000025e0: 7c02 6403 3c00 7108 7c03 a002 a100 6404  |.d.<.q.|.....d.
-000025f0: 7600 723c 7403 7c04 7404 8302 7237 7c00  v.r<t.|.t...r7|.
-00002600: 6a07 6406 6900 7c04 a401 8e01 6e01 7c04  j.d.i.|.....n.|.
-00002610: 7c02 6405 3c00 7108 7108 7c02 5300 2907  |.d.<.q.q.|.S.).
-00002620: 7ac2 0a20 2020 2020 2020 2043 6865 636b  z..        Check
-00002630: 2067 6976 656e 2077 6562 5f6c 6f67 6765   given web_logge
-00002640: 7220 6973 2072 756e 6e65 7220 6f62 6a65  r is runner obje
-00002650: 6374 206f 7220 7275 6e6e 6572 2070 6172  ct or runner par
-00002660: 616d 732e 0a20 2020 2020 2020 2049 6620  ams..        If 
-00002670: 7275 6e6e 6572 2070 6172 616d 7320 6172  runner params ar
-00002680: 6520 7072 6f76 6964 6564 2c20 696e 6974  e provided, init
-00002690: 206e 6577 2072 756e 6e65 7220 6f62 6a65   new runner obje
-000026a0: 6374 2075 7369 6e67 2074 686f 7365 2e0a  ct using those..
-000026b0: 2020 2020 2020 2020 3a70 6172 616d 2077          :param w
-000026c0: 6562 5f6c 6f67 6765 723a 0a20 2020 2020  eb_logger:.     
-000026d0: 2020 203a 7265 7475 726e 3a0a 2020 2020     :return:.    
-000026e0: 2020 2020 4e29 02da 0577 616e 6462 7a03      N)...wandbz.
-000026f0: 7726 6272 9a00 0000 2905 da07 6e65 7074  w&br....)...nept
-00002700: 756e 657a 0a6e 6570 7475 6e65 2e61 695a  unez.neptune.aiZ
-00002710: 096e 6570 7475 6e65 6169 7a0a 6e65 7074  .neptuneaiz.nept
-00002720: 756e 652d 6169 5a03 6e65 7072 9b00 0000  une-aiZ.nepr....
-00002730: 720d 0000 0029 0872 0400 0000 7242 0000  r....).r....rB..
-00002740: 00da 056c 6f77 6572 7236 0000 0072 6700  ...lowerr6...rg.
-00002750: 0000 729a 0000 00da 0469 6e69 74da 0869  ..r......init..i
-00002760: 6e69 745f 746b 6e29 0572 2900 0000 7213  nit_tkn).r)...r.
-00002770: 0000 005a 0b6c 6f67 6765 725f 6469 6374  ...Z.logger_dict
-00002780: 723f 0000 0072 4000 0000 720d 0000 0072  r?...r@...r....r
-00002790: 0d00 0000 722a 0000 0072 2800 0000 0b01  ....r*...r(.....
-000027a0: 0000 7310 0000 0008 0710 010c 0124 010c  ..s..........$..
-000027b0: 0124 0102 0304 017a 1854 7261 696e 6572  .$.....z.Trainer
-000027c0: 2e63 6865 636b 5f77 6562 5f6c 6f67 6765  .check_web_logge
-000027d0: 7272 8300 0000 da0c 7072 6f6a 6563 745f  rr......project_
-000027e0: 6e61 6d65 da07 6170 695f 746b 6e63 0300  name..api_tknc..
-000027f0: 0000 0000 0000 0000 0000 0400 0000 0400  ................
-00002800: 0000 4b00 0000 7318 0000 0074 007c 017c  ..K...s....t.|.|
-00002810: 0266 0269 007c 03a4 018e 017c 005f 0164  .f.i.|.....|._.d
-00002820: 0153 0029 0261 3b01 0000 0a20 2020 2020  .S.).a;....     
-00002830: 2020 2049 6e69 7469 616c 697a 6520 6e65     Initialize ne
-00002840: 7074 756e 6520 6c6f 6767 6572 2077 6974  ptune logger wit
-00002850: 6820 6769 7665 6e20 7072 6f6a 6563 7420  h given project 
-00002860: 6e61 6d65 2061 6e64 2074 6f6b 656e 2e0a  name and token..
-00002870: 2020 2020 2020 2020 5573 6167 653a 0a20          Usage:. 
-00002880: 2020 2020 2020 2020 2020 2074 7261 696e             train
-00002890: 6572 2e69 6e69 745f 746b 6e28 5052 4f4a  er.init_tkn(PROJ
-000028a0: 4543 545f 4e41 4d45 2c20 4150 495f 544f  ECT_NAME, API_TO
-000028b0: 4b45 4e29 0a20 2020 2020 2020 203a 7061  KEN).        :pa
-000028c0: 7261 6d20 7072 6f6a 6563 745f 6e61 6d65  ram project_name
-000028d0: 3a20 7374 720a 2020 2020 2020 2020 3a70  : str.        :p
-000028e0: 6172 616d 2061 7069 5f74 6b6e 3a20 7374  aram api_tkn: st
-000028f0: 720a 2020 2020 2020 2020 3a70 6172 616d  r.        :param
-00002900: 206b 7761 7267 733a 2065 7874 7261 2068   kwargs: extra h
-00002910: 6173 6861 626c 6520 666f 7220 7472 6163  ashable for trac
-00002920: 6b69 6e67 206d 6f64 656c 2028 6f72 206f  king model (or o
-00002930: 7074 2c20 7363 6865 6475 6c65 722c 2065  pt, scheduler, e
-00002940: 7463 2e2e 2e29 0a20 2020 2020 2020 203a  tc...).        :
-00002950: 7265 7475 726e 3a20 4e6f 6e65 0a20 2020  return: None.   
-00002960: 2020 2020 204e 2902 720b 0000 0072 1300       N).r....r..
-00002970: 0000 2904 7229 0000 0072 9f00 0000 72a0  ..).r)...r....r.
-00002980: 0000 0072 4300 0000 720d 0000 0072 0d00  ...rC...r....r..
-00002990: 0000 722a 0000 0072 9e00 0000 1d01 0000  ..r*...r........
-000029a0: 7302 0000 0018 0a7a 1054 7261 696e 6572  s......z.Trainer
-000029b0: 2e69 6e69 745f 746b 6e63 0100 0000 0000  .init_tknc......
-000029c0: 0000 0000 0000 0300 0000 0200 0000 4300  ..............C.
-000029d0: 0000 7334 0000 007c 006a 0064 0119 0004  ..s4...|.j.d....
-000029e0: 007d 0172 0b7c 01a0 01a1 0001 007c 006a  .}.r.|.......|.j
-000029f0: 0064 0219 0004 007d 0272 187c 02a0 02a1  .d.....}.r.|....
-00002a00: 0001 0064 0353 0064 0353 0029 047a 3e0a  ...d.S.d.S.).z>.
-00002a10: 2020 2020 2020 2020 456c 696d 696e 6174          Eliminat
-00002a20: 6520 7765 625f 6c6f 6767 6572 732e 0a20  e web_loggers.. 
-00002a30: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
-00002a40: 4e6f 6e65 0a20 2020 2020 2020 2072 9a00  None.        r..
-00002a50: 0000 729b 0000 004e 2903 7213 0000 00da  ..r....N).r.....
-00002a60: 0666 696e 6973 68da 0965 6c69 6d69 6e61  .finish..elimina
-00002a70: 7465 2903 7229 0000 005a 0677 625f 6c6f  te).r)...Z.wb_lo
-00002a80: 675a 066e 705f 6c6f 6772 0d00 0000 720d  gZ.np_logr....r.
-00002a90: 0000 0072 2a00 0000 da0e 656e 645f 7765  ...r*.....end_we
-00002aa0: 625f 6c6f 6767 6572 2901 0000 730a 0000  b_logger)...s...
-00002ab0: 000e 0508 010e 010c 0104 ff7a 1654 7261  ...........z.Tra
-00002ac0: 696e 6572 2e65 6e64 5f77 6562 5f6c 6f67  iner.end_web_log
-00002ad0: 6765 7263 0200 0000 0000 0000 0000 0000  gerc............
-00002ae0: 0200 0000 0400 0000 4300 0000 7330 0000  ........C...s0..
-00002af0: 007c 006a 0072 077c 00a0 01a1 0001 007c  .|.j.r.|.......|
-00002b00: 00a0 0264 01a1 0101 007c 006a 0364 027c  ...d.....|.j.d.|
-00002b10: 0164 038d 0201 007c 006a 0464 0419 0053  .d.....|.j.d...S
-00002b20: 0029 054e 7244 0000 0072 0a00 0000 2902  .).NrD...r....).
-00002b30: 724a 0000 0072 1800 0000 7285 0000 0029  rJ...r....r....)
-00002b40: 0572 1300 0000 72a3 0000 0072 5200 0000  .r....r....rR...
-00002b50: 7259 0000 0072 2200 0000 2902 7229 0000  rY...r"...).r)..
-00002b60: 0072 1800 0000 720d 0000 0072 0d00 0000  .r....r....r....
-00002b70: 722a 0000 00da 0969 6e66 6572 656e 6365  r*.....inference
-00002b80: 3301 0000 730a 0000 0006 0108 010a 010e  3...s...........
-00002b90: 010a 017a 1154 7261 696e 6572 2e69 6e66  ...z.Trainer.inf
-00002ba0: 6572 656e 6365 2904 4e4e 720d 0000 004e  erence).NNr....N
-00002bb0: 2901 4629 0272 2c00 0000 4e72 5a00 0000  ).F).r,...NrZ...
-00002bc0: 2902 4e54 2901 7283 0000 0029 2fda 085f  ).NT).r....)/.._
-00002bd0: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-00002be0: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-00002bf0: 5fda 075f 5f64 6f63 5f5f 7216 0000 0072  _..__doc__r....r
-00002c00: 0e00 0000 da03 7374 7272 0800 0000 da05  ......strr......
-00002c10: 6f70 7469 6dda 094f 7074 696d 697a 6572  optim..Optimizer
-00002c20: 7209 0000 0072 6700 0000 7207 0000 00da  r....rg...r.....
-00002c30: 066f 626a 6563 7472 2b00 0000 7205 0000  .objectr+...r...
-00002c40: 0072 3700 0000 722f 0000 00da 026e 6eda  .r7...r/.....nn.
-00002c50: 064d 6f64 756c 6572 1e00 0000 7248 0000  .Moduler....rH..
-00002c60: 0072 4900 0000 da03 696e 7472 5900 0000  .rI.....intrY...
-00002c70: 725c 0000 0072 5100 0000 723a 0000 0072  r\...rQ...r:...r
-00002c80: 6100 0000 7203 0000 0072 0600 0000 7269  a...r....r....ri
-00002c90: 0000 0072 6d00 0000 726f 0000 0072 5200  ...rm...ro...rR.
-00002ca0: 0000 da05 666c 6f61 7472 5500 0000 725f  ....floatrU...r_
-00002cb0: 0000 0072 6200 0000 7290 0000 00da 0462  ...rb...r......b
-00002cc0: 6f6f 6c72 9900 0000 7228 0000 0072 9e00  oolr....r(...r..
-00002cd0: 0000 72a3 0000 0072 2000 0000 72a4 0000  ..r....r ...r...
-00002ce0: 0072 0d00 0000 720d 0000 0072 0d00 0000  .r....r....r....
-00002cf0: 722a 0000 0072 0c00 0000 0d00 0000 7358  r*...r........sX
-00002d00: 0000 0008 0004 0102 1402 0102 0102 0104  ................
-00002d10: f804 0302 fd02 0402 fc0a 0502 fb02 0602  ................
-00002d20: fa02 0702 f916 080a f81e 1a02 0f26 020a  .............&..
-00002d30: fe0c 1008 0d14 0708 190a 051a 0702 1726  ...............&
-00002d40: 0102 0c26 011c 0c14 0916 0a0a 0c16 0712  ...&............
-00002d50: 0f18 0332 1318 120a 0c12 0a72 0c00 0000  ...2.......r....
-00002d60: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00002d70: 0002 0000 0040 0000 0073 3400 0000 6500  .....@...s4...e.
-00002d80: 5a01 6400 5a02 6401 6402 8400 5a03 6403  Z.d.Z.d.d...Z.d.
-00002d90: 6404 8400 5a04 6405 6406 8400 5a05 6407  d...Z.d.d...Z.d.
-00002da0: 6408 8400 5a06 6409 640a 8400 5a07 640b  d...Z.d.d...Z.d.
-00002db0: 5300 290c 7226 0000 0063 0100 0000 0000  S.).r&...c......
-00002dc0: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
-00002dd0: 0000 7310 0000 0064 017c 005f 0064 017c  ..s....d.|._.d.|
-00002de0: 005f 0164 0053 00a9 024e 720a 0000 0029  ._.d.S...Nr....)
-00002df0: 02da 165f 5072 6f67 7265 7373 4368 6563  ..._ProgressChec
-00002e00: 6b65 725f 5f73 7465 70da 175f 5072 6f67  ker__step.._Prog
-00002e10: 7265 7373 4368 6563 6b65 725f 5f65 706f  ressChecker__epo
-00002e20: 6368 7233 0000 0072 0d00 0000 720d 0000  chr3...r....r...
-00002e30: 0072 2a00 0000 722b 0000 003c 0100 0073  .r*...r+...<...s
-00002e40: 0400 0000 0601 0a01 7a18 5072 6f67 7265  ........z.Progre
-00002e50: 7373 4368 6563 6b65 722e 5f5f 696e 6974  ssChecker.__init
-00002e60: 5f5f 6301 0000 0000 0000 0000 0000 0001  __c.............
-00002e70: 0000 0003 0000 0043 0000 00f3 1200 0000  .......C........
-00002e80: 7c00 0400 6a00 6401 3700 0200 5f00 6400  |...j.d.7..._.d.
-00002e90: 5300 72b2 0000 00a9 0172 b300 0000 7233  S.r......r....r3
-00002ea0: 0000 0072 0d00 0000 720d 0000 0072 2a00  ...r....r....r*.
-00002eb0: 0000 7270 0000 0040 0100 00f3 0200 0000  ..rp...@........
-00002ec0: 1201 7a1b 5072 6f67 7265 7373 4368 6563  ..z.ProgressChec
-00002ed0: 6b65 722e 7570 6461 7465 5f73 7465 7063  ker.update_stepc
-00002ee0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00002ef0: 0300 0000 4300 0000 72b5 0000 0072 b200  ....C...r....r..
-00002f00: 0000 a901 72b4 0000 0072 3300 0000 720d  ....r....r3...r.
-00002f10: 0000 0072 0d00 0000 722a 0000 0072 5700  ...r....r*...rW.
-00002f20: 0000 4301 0000 72b7 0000 007a 1c50 726f  ..C...r....z.Pro
-00002f30: 6772 6573 7343 6865 636b 6572 2e75 7064  gressChecker.upd
-00002f40: 6174 655f 6570 6f63 6863 0100 0000 0000  ate_epochc......
-00002f50: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
-00002f60: 0000 f306 0000 007c 006a 0053 0072 5a00  .......|.j.S.rZ.
-00002f70: 0000 72b6 0000 0072 3300 0000 720d 0000  ..r....r3...r...
-00002f80: 0072 0d00 0000 722a 0000 00da 0867 6574  .r....r*.....get
-00002f90: 5f73 7465 7046 0100 00f3 0200 0000 0601  _stepF..........
-00002fa0: 7a18 5072 6f67 7265 7373 4368 6563 6b65  z.ProgressChecke
-00002fb0: 722e 6765 745f 7374 6570 6301 0000 0000  r.get_stepc.....
-00002fc0: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
-00002fd0: 0000 0072 b900 0000 725a 0000 0072 b800  ...r....rZ...r..
-00002fe0: 0000 7233 0000 0072 0d00 0000 720d 0000  ..r3...r....r...
-00002ff0: 0072 2a00 0000 da09 6765 745f 6570 6f63  .r*.....get_epoc
-00003000: 6849 0100 0072 bb00 0000 7a19 5072 6f67  hI...r....z.Prog
-00003010: 7265 7373 4368 6563 6b65 722e 6765 745f  ressChecker.get_
-00003020: 6570 6f63 684e 2908 72a5 0000 0072 a600  epochN).r....r..
-00003030: 0000 72a7 0000 0072 2b00 0000 7270 0000  ..r....r+...rp..
-00003040: 0072 5700 0000 72ba 0000 0072 bc00 0000  .rW...r....r....
-00003050: 720d 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
-00003060: 2a00 0000 7226 0000 003b 0100 0073 0c00  *...r&...;...s..
-00003070: 0000 0800 0801 0804 0803 0803 0c03 7226  ..............r&
-00003080: 0000 0029 1472 8a00 0000 da03 6162 6372  ...).r......abcr
-00003090: 0200 0000 7203 0000 00da 0b63 6f6c 6c65  ....r......colle
-000030a0: 6374 696f 6e73 7204 0000 00da 0674 7970  ctionsr......typ
-000030b0: 696e 6772 0500 0000 7206 0000 0072 0700  ingr....r....r..
-000030c0: 0000 7208 0000 0072 0900 0000 729a 0000  ..r....r....r...
-000030d0: 00da 056e 756d 7079 7253 0000 0072 1600  ...numpyrS...r..
-000030e0: 0000 da05 7574 696c 7372 0b00 0000 720c  ....utilsr....r.
-000030f0: 0000 0072 2600 0000 720d 0000 0072 0d00  ...r&...r....r..
-00003100: 0000 720d 0000 0072 2a00 0000 da08 3c6d  ..r....r*.....<m
-00003110: 6f64 756c 653e 0100 0000 7318 0000 0008  odule>....s.....
-00003120: 0010 010c 011c 0108 0208 0108 010c 0210  ................
-00003130: 0300 7f00 7f12 30                        ......0
+00000070: 6401 6c0c 5a0c 6400 6401 6c0d 5a0d 6400  d.l.Z.d.d.l.Z.d.
+00000080: 6401 6c0e 5a0f 6400 6401 6c10 5a10 6405  d.l.Z.d.d.l.Z.d.
+00000090: 6406 6c11 6d12 5a12 0100 4700 6407 6408  d.l.m.Z...G.d.d.
+000000a0: 8400 6408 6502 8303 5a13 4700 6409 640a  ..d.e...Z.G.d.d.
+000000b0: 8400 640a 8302 5a14 6401 5300 290b e900  ..d...Z.d.S.)...
+000000c0: 0000 004e 2902 da03 4142 43da 0e61 6273  ...N)...ABC..abs
+000000d0: 7472 6163 746d 6574 686f 6429 01da 0b64  tractmethod)...d
+000000e0: 6566 6175 6c74 6469 6374 2905 da05 5475  efaultdict)...Tu
+000000f0: 706c 65da 0444 6963 74da 0555 6e69 6f6e  ple..Dict..Union
+00000100: da08 4f70 7469 6f6e 616c da08 4974 6572  ..Optional..Iter
+00000110: 6162 6c65 e901 0000 0029 01da 0d4e 6570  able.....)...Nep
+00000120: 7475 6e65 4c6f 6767 6572 6300 0000 0000  tuneLoggerc.....
+00000130: 0000 0000 0000 0000 0000 0014 0000 0040  ...............@
+00000140: 0000 0073 4e02 0000 6500 5a01 6400 5a02  ...sN...e.Z.d.Z.
+00000150: 6401 5a03 0902 0902 0903 0904 0902 6447  d.Z...........dG
+00000160: 6405 6504 6a05 6406 6506 6407 6507 6504  d.e.j.d.e.d.e.e.
+00000170: 6a08 6a09 1900 6408 6507 6409 650a 640a  j.j...d.e.d.e.d.
+00000180: 650b 640b 6507 650c 6506 650d 650e 650c  e.d.e.e.e.e.e.e.
+00000190: 6602 1900 6602 1900 1900 660e 640c 640d  f...f.....f.d.d.
+000001a0: 8405 5a0f 640e 6510 6504 6a11 640f 6602  ..Z.d.e.e.j.d.f.
+000001b0: 1900 7038 6504 6a11 6602 6410 6411 8404  ..p8e.j.f.d.d...
+000001c0: 5a12 640e 6510 650d 6504 6a11 6504 6a13  Z.d.e.e.e.j.e.j.
+000001d0: 6a14 6602 1900 1900 7051 650d 6504 6a11  j.f.....pQe.e.j.
+000001e0: 6504 6a13 6a14 6602 1900 6602 6412 6413  e.j.j.f...f.d.d.
+000001f0: 8404 5a15 6448 6449 6415 6416 8405 5a16  ..Z.dHdId.d...Z.
+00000200: 6417 6418 8400 5a17 644a 6419 6518 640e  d.d...Z.dJd.e.d.
+00000210: 6402 6604 641a 641b 8405 5a19 641c 641d  d.f.d.d...Z.d.d.
+00000220: 8400 5a1a 6449 641e 641f 8404 5a1b 6420  ..Z.dId.d...Z.d 
+00000230: 650d 651c 650c 6602 1900 640e 6402 6604  e.e.e.f...d.d.f.
+00000240: 6421 6422 8404 5a1d 651e 6420 650d 651c  d!d"..Z.e.d e.e.
+00000250: 650c 6602 1900 640e 651f 6506 6504 6a11  e.f...d.e.e.e.j.
+00000260: 6602 1900 6604 6423 6424 8404 8301 5a20  f...f.d#d$....Z 
+00000270: 651e 6420 650d 651c 650c 6602 1900 640e  e.d e.e.e.f...d.
+00000280: 651f 6506 6504 6a11 6602 1900 6604 6425  e.e.e.j.f...f.d%
+00000290: 6426 8404 8301 5a21 6427 651f 6506 6504  d&....Z!d'e.e.e.
+000002a0: 6a11 6602 1900 640e 6402 6604 6428 6429  j.f...d.d.f.d(d)
+000002b0: 8404 5a22 644a 6406 6506 640e 6402 6604  ..Z"dJd.e.d.d.f.
+000002c0: 642a 642b 8405 5a23 642c 6518 642d 6524  d*d+..Z#d,e.d-e$
+000002d0: 640e 6402 6606 642e 642f 8404 5a25 6449  d.d.f.d.d/..Z%dI
+000002e0: 6430 6431 8404 5a26 6432 6518 6433 6518  d0d1..Z&d2e.d3e.
+000002f0: 640e 6510 6506 650c 6602 1900 6606 6434  d.e.e.e.f...f.d4
+00000300: 6435 8404 5a27 6436 6506 640e 6402 6604  d5..Z'd6e.d.d.f.
+00000310: 6437 6438 8404 5a28 644b 6436 6506 6439  d7d8..Z(dKd6e.d9
+00000320: 650a 640e 6402 6606 643a 643b 8405 5a29  e.d.d.f.d:d;..Z)
+00000330: 640b 651f 6506 650d 650e 650c 6602 1900  d.e.e.e.e.e.f...
+00000340: 6602 1900 640e 651f 6506 650d 650e 6402  f...d.e.e.e.e.d.
+00000350: 6602 1900 6602 1900 6604 643c 643d 8404  f...f...f.d<d=..
+00000360: 5a2a 644c 643f 6506 6440 6506 640e 6402  Z*dLd?e.d@e.d.d.
+00000370: 6606 6441 6442 8405 5a2b 6449 6443 6444  f.dAdB..Z+dIdCdD
+00000380: 8404 5a2c 640e 652d 6602 6445 6446 8404  ..Z,d.e-f.dEdF..
+00000390: 5a2e 6402 5300 294d da07 5472 6169 6e65  Z.d.S.)M..Traine
+000003a0: 7261 f501 0000 0a20 2020 2041 6273 7472  ra.....    Abstr
+000003b0: 6163 7420 636c 6173 7320 666f 7220 6578  act class for ex
+000003c0: 7065 7269 6d65 6e74 7320 7769 7468 2032  periments with 2
+000003d0: 2061 6273 7472 6163 7420 6d65 7468 6f64   abstract method
+000003e0: 7320 7472 6169 6e5f 7374 6570 2061 6e64  s train_step and
+000003f0: 2074 6573 745f 7374 6570 2e0a 2020 2020   test_step..    
+00000400: 4e6f 7465 2074 6861 7420 626f 7468 2074  Note that both t
+00000410: 6865 2074 7261 696e 5f73 7465 7020 616e  he train_step an
+00000420: 6420 7465 7374 5f73 7465 7020 6172 6520  d test_step are 
+00000430: 7265 6365 6976 6520 6261 7463 6820 616e  receive batch an
+00000440: 6420 7265 7475 726e 2061 2064 6963 7469  d return a dicti
+00000450: 6f6e 6172 792e 0a20 2020 204d 6f72 6520  onary..    More 
+00000460: 6465 7461 696c 2061 626f 7574 2074 686f  detail about tho
+00000470: 7365 2061 7265 2069 6e20 6561 6368 206d  se are in each m
+00000480: 6574 686f 6427 7320 646f 6373 7472 696e  ethod's docstrin
+00000490: 672e 0a0a 2020 2020 3a70 6172 616d 206d  g...    :param m
+000004a0: 6f64 656c 3a20 6e6e 2e4d 6f64 756c 650a  odel: nn.Module.
+000004b0: 2020 2020 3a70 6172 616d 2064 6576 6963      :param devic
+000004c0: 653a 2074 6f72 6368 2e64 6576 6963 650a  e: torch.device.
+000004d0: 2020 2020 3a70 6172 616d 206d 6f64 653a      :param mode:
+000004e0: 2073 7472 0a20 2020 203a 7061 7261 6d20   str.    :param 
+000004f0: 6f70 7469 6d69 7a65 723a 2073 7472 2c20  optimizer: str, 
+00000500: 6f70 7469 6f6e 616c 0a20 2020 203a 7061  optional.    :pa
+00000510: 7261 6d20 7363 6865 6475 6c65 723a 2073  ram scheduler: s
+00000520: 7472 2c20 6f70 7469 6f6e 616c 0a20 2020  tr, optional.   
+00000530: 203a 6361 6c6c 6261 636b 733a 2055 6e69   :callbacks: Uni
+00000540: 6f6e 5b43 616c 6c61 626c 652c 2049 7465  on[Callable, Ite
+00000550: 7261 626c 655d 2c20 6f70 7469 6f6e 616c  rable], optional
+00000560: 0a20 2020 203a 6361 6c6c 6261 636b 5f73  .    :callback_s
+00000570: 7465 703a 2069 6e74 2c20 6f70 7469 6f6e  tep: int, option
+00000580: 616c 0a20 2020 203a 6361 6c6c 6261 636b  al.    :callback
+00000590: 5f65 706f 6368 0a20 2020 204e 54a9 00da  _epoch.    NT...
+000005a0: 0664 6576 6963 65da 046d 6f64 65da 096f  .device..mode..o
+000005b0: 7074 696d 697a 6572 da09 7363 6865 6475  ptimizer..schedu
+000005c0: 6c65 72da 076c 6f67 5f62 6172 da09 6361  ler..log_bar..ca
+000005d0: 6c6c 6261 636b 73da 0a77 6562 5f6c 6f67  llbacks..web_log
+000005e0: 6765 7263 0900 0000 0000 0000 0000 0000  gerc............
+000005f0: 0900 0000 0400 0000 4300 0000 73b0 0000  ........C...s...
+00000600: 0064 017c 026a 0076 0072 0b74 016a 02a0  .d.|.j.v.r.t.j..
+00000610: 037c 02a1 0101 007c 027c 005f 0464 025c  .|.....|.|._.d.\
+00000620: 037c 005f 057c 005f 067c 005f 0764 025c  .|._.|._.|._.d.\
+00000630: 037c 005f 087c 005f 097c 005f 0a7c 037c  .|._.|._.|._.|.|
+00000640: 005f 0b7c 067c 005f 0c7c 047c 005f 0d7c  ._.|.|._.|.|._.|
+00000650: 057c 005f 0e7c 00a0 0f7c 01a1 017c 005f  .|._.|...|...|._
+00000660: 1074 1174 1283 0174 1174 1283 0102 027c  .t.t...t.t.....|
+00000670: 005f 137c 005f 1474 016a 1574 1174 1283  ._.|._.t.j.t.t..
+00000680: 0102 027c 005f 167c 005f 177c 077c 005f  ...|._.|._.|.|._
+00000690: 1874 1983 007c 005f 1a7c 0872 567c 00a0  .t...|._.|.rV|..
+000006a0: 1b7c 08a1 017c 005f 1c64 0053 0064 0053  .|...|._.d.S.d.S
+000006b0: 0029 034e da04 6375 6461 2903 4e4e 4e29  .).N..cuda).NNN)
+000006c0: 1dda 0474 7970 65da 0574 6f72 6368 7215  ...type..torchr.
+000006d0: 0000 00da 0a73 6574 5f64 6576 6963 6572  .....set_devicer
+000006e0: 0e00 0000 da06 6c6f 6164 6572 da06 6e5f  ......loader..n_
+000006f0: 6461 7461 da0a 6261 7463 685f 7369 7a65  data..batch_size
+00000700: da0c 7661 6c69 645f 6c6f 6164 6572 da0c  ..valid_loader..
+00000710: 6e5f 7661 6c69 645f 6461 7461 da10 7661  n_valid_data..va
+00000720: 6c69 645f 6261 7463 685f 7369 7a65 720f  lid_batch_sizer.
+00000730: 0000 0072 1200 0000 7210 0000 0072 1100  ...r....r....r..
+00000740: 0000 da0a 5f74 6f5f 6465 7669 6365 da05  ...._to_device..
+00000750: 6d6f 6465 6c72 0400 0000 da04 6c69 7374  modelr......list
+00000760: da09 6c6f 675f 7472 6169 6eda 086c 6f67  ..log_train..log
+00000770: 5f74 6573 74da 0369 6e66 da0b 6c6f 7373  _test..inf..loss
+00000780: 5f62 7566 6665 72da 0d77 6569 6768 745f  _buffer..weight_
+00000790: 6275 6666 6572 7213 0000 00da 0f50 726f  bufferr......Pro
+000007a0: 6772 6573 7343 6865 636b 6572 da10 7072  gressChecker..pr
+000007b0: 6f67 7265 7373 5f63 6865 636b 6572 da10  ogress_checker..
+000007c0: 6368 6563 6b5f 7765 625f 6c6f 6767 6572  check_web_logger
+000007d0: 7214 0000 0029 09da 0473 656c 6672 2000  r....)...selfr .
+000007e0: 0000 720e 0000 0072 0f00 0000 7210 0000  ..r....r....r...
+000007f0: 0072 1100 0000 7212 0000 0072 1300 0000  .r....r....r....
+00000800: 7214 0000 0072 0d00 0000 720d 0000 00fa  r....r....r.....
+00000810: 345a 3a5c 6465 762d 7a61 655c 7a61 652d  4Z:\dev-zae\zae-
+00000820: 656e 6769 6e65 5c7a 6165 5f65 6e67 696e  engine\zae_engin
+00000830: 655c 7472 6169 6e65 725c 5f74 7261 696e  e\trainer\_train
+00000840: 6572 2e70 79da 085f 5f69 6e69 745f 5f1e  er.py..__init__.
+00000850: 0000 0073 2200 0000 0a0b 0c01 0601 1001  ...s"...........
+00000860: 1001 0601 0601 0601 0601 0c01 1601 1401  ................
+00000870: 0601 0801 0401 1001 04ff 7a10 5472 6169  ..........z.Trai
+00000880: 6e65 722e 5f5f 696e 6974 5f5f da06 7265  ner.__init__..re
+00000890: 7475 726e 2e63 0100 0000 0000 0000 0000  turn.c..........
+000008a0: 0000 0300 0000 0400 0000 0700 0000 736a  ..............sj
+000008b0: 0000 0074 007c 0183 0164 016b 0272 2a7c  ...t.|...d.k.r*|
+000008c0: 0164 0219 007d 0274 017c 0274 026a 0383  .d...}.t.|.t.j..
+000008d0: 0272 2864 037c 02a0 04a1 0076 0072 1c7c  .r(d.|.....v.r.|
+000008e0: 02a0 05a1 00a0 06a1 0053 0064 047c 02a0  .........S.d.|..
+000008f0: 04a1 0076 0072 267c 02a0 07a1 0053 007c  ...v.r&|.....S.|
+00000900: 0253 007c 0253 0074 0887 0066 0164 0564  .S.|.S.t...f.d.d
+00000910: 0684 087c 0144 0083 0183 0153 0029 087a  ...|.D.....S.).z
+00000920: cf0a 2020 2020 2020 2020 4361 7374 2067  ..        Cast g
+00000930: 6976 656e 2061 7267 756d 656e 7473 2074  iven arguments t
+00000940: 6f20 6370 752e 0a20 2020 2020 2020 203a  o cpu..        :
+00000950: 7061 7261 6d20 6172 6773 3a20 5369 6e67  param args: Sing
+00000960: 6c65 2061 7267 756d 656e 7420 6f72 2076  le argument or v
+00000970: 6172 6961 626c 652d 6c65 6e67 7468 2073  ariable-length s
+00000980: 6571 7565 6e63 6520 6f66 2061 7267 756d  equence of argum
+00000990: 656e 7473 2e0a 2020 2020 2020 2020 3a72  ents..        :r
+000009a0: 6574 7572 6e3a 2053 696e 676c 6520 6172  eturn: Single ar
+000009b0: 6775 6d65 6e74 206f 7220 7661 7269 6162  gument or variab
+000009c0: 6c65 2d6c 656e 6774 6820 7365 7175 656e  le-length sequen
+000009d0: 6365 206f 6620 6172 6775 6d65 6e74 7320  ce of arguments 
+000009e0: 696e 2063 7075 2e0a 2020 2020 2020 2020  in cpu..        
+000009f0: 720a 0000 0072 0100 0000 da06 6465 7461  r....r......deta
+00000a00: 6368 da04 6974 656d 6301 0000 0000 0000  ch..itemc.......
+00000a10: 0000 0000 0002 0000 0005 0000 0013 0000  ................
+00000a20: 0073 1600 0000 6700 7c00 5d07 7d01 8800  .s....g.|.].}...
+00000a30: a000 7c01 a101 9102 7102 5300 720d 0000  ..|.....q.S.r...
+00000a40: 0029 01da 075f 746f 5f63 7075 a902 da02  .)..._to_cpu....
+00000a50: 2e30 da01 61a9 0172 2a00 0000 720d 0000  .0..a..r*...r...
+00000a60: 0072 2b00 0000 da0a 3c6c 6973 7463 6f6d  .r+.....<listcom
+00000a70: 703e 4700 0000 7302 0000 0016 007a 2354  p>G...s......z#T
+00000a80: 7261 696e 6572 2e5f 746f 5f63 7075 2e3c  rainer._to_cpu.<
+00000a90: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+00000aa0: 703e 4e29 09da 036c 656e da0a 6973 696e  p>N)...len..isin
+00000ab0: 7374 616e 6365 7217 0000 00da 0654 656e  stancer......Ten
+00000ac0: 736f 72da 075f 5f64 6972 5f5f 722e 0000  sor..__dir__r...
+00000ad0: 00da 0363 7075 722f 0000 00da 0574 7570  ...cpur/.....tup
+00000ae0: 6c65 2903 722a 0000 00da 0461 7267 7372  le).r*.....argsr
+00000af0: 3300 0000 720d 0000 0072 3400 0000 722b  3...r....r4...r+
+00000b00: 0000 0072 3000 0000 3a00 0000 730c 0000  ...r0...:...s...
+00000b10: 000c 0608 010c 0130 0104 0216 027a 0f54  .......0.....z.T
+00000b20: 7261 696e 6572 2e5f 746f 5f63 7075 6301  rainer._to_cpuc.
+00000b30: 0000 0000 0000 0000 0000 0003 0000 0004  ................
+00000b40: 0000 000f 0000 0073 6c00 0000 7c01 7227  .......sl...|.r'
+00000b50: 7400 7c01 8301 6401 6b02 721c 6402 7c01  t.|...d.k.r.d.|.
+00000b60: 6403 1900 a001 a100 7600 7218 7c01 6403  d.......v.r.|.d.
+00000b70: 1900 a002 8800 6a03 a101 5300 7c01 6403  ......j...S.|.d.
+00000b80: 1900 5300 7404 8700 6601 6404 6405 8408  ..S.t...f.d.d...
+00000b90: 7c01 4400 8301 8301 5300 7c02 7234 8700  |.D.....S.|.r4..
+00000ba0: 6601 6406 6407 8408 7c02 a005 a100 4400  f.d.d...|.....D.
+00000bb0: 8301 5300 6408 5300 2909 7ad5 0a20 2020  ..S.d.S.).z..   
+00000bc0: 2020 2020 2043 6173 7420 6769 7665 6e20       Cast given 
+00000bd0: 6172 6775 6d65 6e74 7320 746f 2064 6576  arguments to dev
+00000be0: 6963 652e 0a20 2020 2020 2020 203a 7061  ice..        :pa
+00000bf0: 7261 6d20 6172 6773 3a20 5369 6e67 6c65  ram args: Single
+00000c00: 2061 7267 756d 656e 7420 6f72 2076 6172   argument or var
+00000c10: 6961 626c 652d 6c65 6e67 7468 2073 6571  iable-length seq
+00000c20: 7565 6e63 6520 6f66 2061 7267 756d 656e  uence of argumen
+00000c30: 7473 2e0a 2020 2020 2020 2020 3a72 6574  ts..        :ret
+00000c40: 7572 6e3a 2053 696e 676c 6520 6172 6775  urn: Single argu
+00000c50: 6d65 6e74 206f 7220 7661 7269 6162 6c65  ment or variable
+00000c60: 2d6c 656e 6774 6820 7365 7175 656e 6365  -length sequence
+00000c70: 206f 6620 6172 6775 6d65 6e74 7320 696e   of arguments in
+00000c80: 2064 6576 6963 652e 0a20 2020 2020 2020   device..       
+00000c90: 2072 0a00 0000 da02 746f 7201 0000 0063   r......tor....c
+00000ca0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00000cb0: 0500 0000 1300 0000 7328 0000 0067 007c  ........s(...g.|
+00000cc0: 005d 107d 0164 007c 01a0 00a1 0076 0072  .].}.d.|.....v.r
+00000cd0: 107c 01a0 0188 006a 02a1 016e 017c 0191  .|.....j...n.|..
+00000ce0: 0271 0253 00a9 0172 3d00 0000 a903 7239  .q.S...r=.....r9
+00000cf0: 0000 0072 3d00 0000 720e 0000 0072 3100  ...r=...r....r1.
+00000d00: 0000 7234 0000 0072 0d00 0000 722b 0000  ..r4...r....r+..
+00000d10: 0072 3500 0000 5500 0000 7302 0000 0028  .r5...U...s....(
+00000d20: 007a 2654 7261 696e 6572 2e5f 746f 5f64  .z&Trainer._to_d
+00000d30: 6576 6963 652e 3c6c 6f63 616c 733e 2e3c  evice.<locals>.<
+00000d40: 6c69 7374 636f 6d70 3e63 0100 0000 0000  listcomp>c......
+00000d50: 0000 0000 0000 0300 0000 0600 0000 1300  ................
+00000d60: 0000 732e 0000 0069 007c 005d 135c 027d  ..s....i.|.].\.}
+00000d70: 017d 027c 0164 007c 02a0 00a1 0076 0072  .}.|.d.|.....v.r
+00000d80: 137c 02a0 0188 006a 02a1 016e 017c 0293  .|.....j...n.|..
+00000d90: 0271 0253 0072 3e00 0000 723f 0000 0029  .q.S.r>...r?...)
+00000da0: 0372 3200 0000 da01 6bda 0176 7234 0000  .r2.....k..vr4..
+00000db0: 0072 0d00 0000 722b 0000 00da 0a3c 6469  .r....r+.....<di
+00000dc0: 6374 636f 6d70 3e57 0000 0073 0200 0000  ctcomp>W...s....
+00000dd0: 2e00 7a26 5472 6169 6e65 722e 5f74 6f5f  ..z&Trainer._to_
+00000de0: 6465 7669 6365 2e3c 6c6f 6361 6c73 3e2e  device.<locals>.
+00000df0: 3c64 6963 7463 6f6d 703e 4e29 0672 3600  <dictcomp>N).r6.
+00000e00: 0000 7239 0000 0072 3d00 0000 720e 0000  ..r9...r=...r...
+00000e10: 0072 3b00 0000 da05 6974 656d 7329 0372  .r;.....items).r
+00000e20: 2a00 0000 723c 0000 00da 066b 7761 7267  *...r<.....kwarg
+00000e30: 7372 0d00 0000 7234 0000 0072 2b00 0000  sr....r4...r+...
+00000e40: 721f 0000 0049 0000 0073 0e00 0000 0408  r....I...s......
+00000e50: 0c01 2801 1602 0401 1601 04ff 7a12 5472  ..(.........z.Tr
+00000e60: 6169 6e65 722e 5f74 6f5f 6465 7669 6365  ainer._to_device
+00000e70: 4663 0200 0000 0000 0000 0000 0000 0200  Fc..............
+00000e80: 0000 0300 0000 4300 0000 7382 0000 007c  ......C...s....|
+00000e90: 0172 237c 006a 0064 0175 0172 0d7c 006a  .r#|.j.d.u.r.|.j
+00000ea0: 006a 01a0 02a1 006e 0164 027c 005f 037c  .j.....n.d.|._.|
+00000eb0: 006a 0464 0175 0172 1e7c 006a 046a 01a0  .j.d.u.r.|.j.j..
+00000ec0: 02a1 007c 005f 0564 0153 0064 027c 005f  ...|._.d.S.d.|._
+00000ed0: 0564 0153 007c 006a 0664 036b 0272 377c  .d.S.|.j.d.k.r7|
+00000ee0: 006a 0464 0175 0172 377c 0004 006a 057c  .j.d.u.r7|...j.|
+00000ef0: 006a 0738 0002 005f 0564 0153 007c 0004  .j.8..._.d.S.|..
+00000f00: 006a 037c 006a 0838 0002 005f 0364 0153  .j.|.j.8..._.d.S
+00000f10: 0029 047a 350a 2020 2020 2020 2020 436f  .).z5.        Co
+00000f20: 756e 7420 7468 6520 6e75 6d62 6572 206f  unt the number o
+00000f30: 6620 6461 7461 2069 6e20 6c6f 6164 6572  f data in loader
+00000f40: 2e0a 2020 2020 2020 2020 4e72 0100 0000  ..        Nr....
+00000f50: da04 7465 7374 2909 7219 0000 00da 0764  ..test).r......d
+00000f60: 6174 6173 6574 da07 5f5f 6c65 6e5f 5f72  ataset..__len__r
+00000f70: 1a00 0000 721c 0000 0072 1d00 0000 720f  ....r....r....r.
+00000f80: 0000 0072 1e00 0000 721b 0000 0029 0272  ...r....r....).r
+00000f90: 2a00 0000 da07 696e 6974 6961 6c72 0d00  *.....initialr..
+00000fa0: 0000 720d 0000 0072 2b00 0000 da0b 5f64  ..r....r+....._d
+00000fb0: 6174 615f 636f 756e 7459 0000 0073 0c00  ata_countY...s..
+00000fc0: 0000 0404 1c01 2601 1402 1401 1402 7a13  ......&.......z.
+00000fd0: 5472 6169 6e65 722e 5f64 6174 615f 636f  Trainer._data_co
+00000fe0: 756e 7463 0100 0000 0000 0000 0000 0000  untc............
+00000ff0: 0100 0000 0200 0000 4300 0000 733a 0000  ........C...s:..
+00001000: 007c 006a 0064 0175 0172 097c 006a 006a  .|.j.d.u.r.|.j.j
+00001010: 016e 0164 027c 005f 017c 006a 0264 0175  .n.d.|._.|.j.d.u
+00001020: 0172 187c 006a 026a 017c 005f 0364 0153  .r.|.j.j.|._.d.S
+00001030: 0064 027c 005f 0364 0153 0029 037a 2d0a  .d.|._.d.S.).z-.
+00001040: 2020 2020 2020 2020 4368 6563 6b20 6261          Check ba
+00001050: 7463 6820 7369 7a65 206f 6620 6c6f 6164  tch size of load
+00001060: 6572 2e0a 2020 2020 2020 2020 4e72 0100  er..        Nr..
+00001070: 0000 2904 7219 0000 0072 1b00 0000 721c  ..).r....r....r.
+00001080: 0000 0072 1e00 0000 7234 0000 0072 0d00  ...r....r4...r..
+00001090: 0000 720d 0000 0072 2b00 0000 da11 5f63  ..r....r+....._c
+000010a0: 6865 636b 5f62 6174 6368 5f73 697a 6566  heck_batch_sizef
+000010b0: 0000 0073 0400 0000 1804 2201 7a19 5472  ...s......".z.Tr
+000010c0: 6169 6e65 722e 5f63 6865 636b 5f62 6174  ainer._check_bat
+000010d0: 6368 5f73 697a 65da 076e 5f65 706f 6368  ch_size..n_epoch
+000010e0: 6304 0000 0000 0000 0000 0000 0008 0000  c...............
+000010f0: 0006 0000 004b 0000 0073 fe00 0000 7c02  .....K...s....|.
+00001100: 7c03 0202 7c00 5f00 7c00 5f01 7c00 a002  |...|._.|._.|...
+00001110: a100 0100 7c00 6a03 7218 7404 6a04 7405  ....|.j.r.t.j.t.
+00001120: 7c01 8301 6401 6402 6403 8d03 6e03 7405  |...d.d.d...n.t.
+00001130: 7c01 8301 7d05 7c05 4400 5d5e 7d06 7c00  |...}.|.D.]^}.|.
+00001140: 6a03 722d 7c05 a006 6404 7c06 6405 1700  j.r-|...d.|.d...
+00001150: 1600 a101 0100 6e08 7407 6404 7c06 6405  ......n.t.d.|.d.
+00001160: 1700 1600 8301 0100 7c00 6a08 6402 6406  ........|.j.d.d.
+00001170: 8d01 0100 7c00 a009 7c02 a101 0100 7c03  ....|...|.....|.
+00001180: 724f 7c00 a00a a100 0100 7c00 a009 7c03  rO|.......|...|.
+00001190: a101 0100 7c00 a00a a100 0100 7c00 6a0b  ....|.......|.j.
+000011a0: 6407 6b02 727c 740c a00d 7c03 725d 7c00  d.k.r|t...|.r]|.
+000011b0: 6a0e 6408 1900 6e04 7c00 6a0f 6408 1900  j.d...n.|.j.d...
+000011c0: a101 a010 a100 7d07 7c00 6a11 7c06 6405  ......}.|.j.|.d.
+000011d0: 1700 7c07 6409 8d02 0100 7c00 6a12 6a13  ..|.d.....|.j.j.
+000011e0: 640b 6900 7c04 a401 8e01 0100 7c00 6a14  d.i.|.......|.j.
+000011f0: a015 a100 0100 711e 640a 5300 290c 7ae9  ......q.d.S.).z.
+00001200: 0a20 2020 2020 2020 2052 756e 2066 6f72  .        Run for
+00001210: 2061 2067 6976 656e 206c 6f61 6465 722e   a given loader.
+00001220: 0a20 2020 2020 2020 2049 6620 7661 6c69  .        If vali
+00001230: 645f 6c6f 6164 6572 2069 7320 6e6f 7420  d_loader is not 
+00001240: 4e6f 6e65 2c20 7468 6520 6d6f 6465 6c20  None, the model 
+00001250: 6576 616c 7561 7465 7320 7468 6520 6461  evaluates the da
+00001260: 7461 2069 6e20 7661 6c69 645f 6c6f 6164  ta in valid_load
+00001270: 6572 2066 6f72 2065 7665 7279 2065 706f  er for every epo
+00001280: 6368 2e0a 2020 2020 2020 2020 3a70 6172  ch..        :par
+00001290: 616d 206e 5f65 706f 6368 3a0a 2020 2020  am n_epoch:.    
+000012a0: 2020 2020 3a70 6172 616d 206c 6f61 6465      :param loade
+000012b0: 723a 0a20 2020 2020 2020 203a 7061 7261  r:.        :para
+000012c0: 6d20 7661 6c69 645f 6c6f 6164 6572 3a0a  m valid_loader:.
+000012d0: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+000012e0: 0a20 2020 2020 2020 2072 0100 0000 54a9  .        r....T.
+000012f0: 02da 0870 6f73 6974 696f 6eda 056c 6561  ...position..lea
+00001300: 7665 7a08 4570 6f63 6820 2564 720a 0000  vez.Epoch %dr...
+00001310: 0029 0172 4800 0000 da05 7472 6169 6eda  .).rH.....train.
+00001320: 046c 6f73 7329 02da 0963 7572 5f65 706f  .loss)...cur_epo
+00001330: 6368 da08 6375 725f 6c6f 7373 4e72 0d00  ch..cur_lossNr..
+00001340: 0000 2916 7219 0000 0072 1c00 0000 724a  ..).r....r....rJ
+00001350: 0000 0072 1200 0000 da04 7471 646d da05  ...r......tqdm..
+00001360: 7261 6e67 65da 0f73 6574 5f64 6573 6372  range..set_descr
+00001370: 6970 7469 6f6e da05 7072 696e 7472 4900  iption..printrI.
+00001380: 0000 da09 7275 6e5f 6570 6f63 68da 0674  ....run_epoch..t
+00001390: 6f67 676c 6572 0f00 0000 da02 6e70 da04  oggler......np..
+000013a0: 6d65 616e 7223 0000 0072 2200 0000 722f  meanr#...r"...r/
+000013b0: 0000 00da 0c63 6865 636b 5f62 6574 7465  .....check_bette
+000013c0: 7272 1100 0000 da04 7374 6570 7228 0000  rr......stepr(..
+000013d0: 00da 0c75 7064 6174 655f 6570 6f63 6829  ...update_epoch)
+000013e0: 0872 2a00 0000 724b 0000 0072 1900 0000  .r*...rK...r....
+000013f0: 721c 0000 0072 4400 0000 da08 7072 6f67  r....rD.....prog
+00001400: 7265 7373 da01 6572 5200 0000 720d 0000  ress..erR...r...
+00001410: 0072 0d00 0000 722b 0000 00da 0372 756e  .r....r+.....run
+00001420: 6d00 0000 7328 0000 000e 0908 0122 0108  m...s(......."..
+00001430: 0106 0114 0110 020c 010a 0104 0108 010a  ................
+00001440: 0108 010a 0122 0112 0112 010a 0102 8004  ....."..........
+00001450: f17a 0b54 7261 696e 6572 2e72 756e 6301  .z.Trainer.runc.
+00001460: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+00001470: 0000 0043 0000 0073 2200 0000 7c00 6a00  ...C...s"...|.j.
+00001480: 720d 7c00 6a00 4400 5d08 7d01 7c01 7c00  r.|.j.D.].}.|.|.
+00001490: 8301 0100 7106 6400 5300 6400 5300 a901  ....q.d.S.d.S...
+000014a0: 4e29 0172 1300 0000 2902 722a 0000 00da  N).r....).r*....
+000014b0: 0263 6272 0d00 0000 720d 0000 0072 2b00  .cbr....r....r+.
+000014c0: 0000 da0c 7275 6e5f 6361 6c6c 6261 636b  ....run_callback
+000014d0: 8a00 0000 730a 0000 0006 010a 010a 0104  ....s...........
+000014e0: fe04 017a 1454 7261 696e 6572 2e72 756e  ...z.Trainer.run
+000014f0: 5f63 616c 6c62 6163 6b63 0200 0000 0000  _callbackc......
+00001500: 0000 0000 0000 0700 0000 0500 0000 4300  ..............C.
+00001510: 0000 7386 0000 007c 00a0 00a1 0001 007c  ..s....|.......|
+00001520: 006a 0172 0f74 026a 027c 0164 0164 0264  .j.r.t.j.|.d.d.d
+00001530: 038d 036e 017c 017d 0274 037c 0283 0144  ...n.|.}.t.|...D
+00001540: 005d 2b5c 027d 037d 047c 00a0 047c 04a1  .]+\.}.}.|...|..
+00001550: 0101 007c 00a0 05a1 0001 007c 006a 067c  ...|.......|.j.|
+00001560: 0364 0117 0074 077c 0183 0164 048d 025c  .d...t.|...d...\
+00001570: 027d 057d 067c 006a 0172 387c 02a0 087c  .}.}.|.j.r8|...|
+00001580: 05a1 0101 0071 1574 097c 0566 0169 007c  .....q.t.|.f.i.|
+00001590: 06a4 018e 0101 0071 1564 0053 0029 054e  .......q.d.S.).N
+000015a0: 720a 0000 0046 724c 0000 0029 02da 0963  r....FrL...)...c
+000015b0: 7572 5f62 6174 6368 da09 6e75 6d5f 6261  ur_batch..num_ba
+000015c0: 7463 6829 0ada 096c 6f67 5f72 6573 6574  tch)...log_reset
+000015d0: 7212 0000 0072 5300 0000 da09 656e 756d  r....rS.....enum
+000015e0: 6572 6174 65da 0972 756e 5f62 6174 6368  erate..run_batch
+000015f0: 7249 0000 00da 0970 7269 6e74 5f6c 6f67  rI.....print_log
+00001600: 7236 0000 0072 5500 0000 7256 0000 0029  r6...rU...rV...)
+00001610: 0772 2a00 0000 7219 0000 0072 5e00 0000  .r*...r....r^...
+00001620: da01 69da 0562 6174 6368 da04 6465 7363  ..i..batch..desc
+00001630: da07 7072 696e 7465 7272 0d00 0000 720d  ..printerr....r.
+00001640: 0000 0072 2b00 0000 7257 0000 008f 0000  ...r+...rW......
+00001650: 0073 1400 0000 0801 1a01 1001 0a01 0801  .s..............
+00001660: 1a01 0601 0c01 1202 04f9 7a11 5472 6169  ..........z.Trai
+00001670: 6e65 722e 7275 6e5f 6570 6f63 6872 6b00  ner.run_epochrk.
+00001680: 0000 6302 0000 0000 0000 0000 0000 0003  ..c.............
+00001690: 0000 0008 0000 0043 0000 0073 de00 0000  .......C...s....
+000016a0: 7400 7c01 7401 8302 720d 7c00 6a02 6407  t.|.t...r.|.j.d.
+000016b0: 6900 7c01 a401 8e01 6e04 7c00 6a02 7c01  i.|.....n.|.j.|.
+000016c0: 8e00 7d01 7c00 6a03 6401 6b02 7232 7c00  ..}.|.j.d.k.r2|.
+000016d0: 6a04 a005 a100 0100 7c00 6a06 a007 a100  j.......|.j.....
+000016e0: 0100 7c00 a008 7c01 a101 7d02 7c02 6402  ..|...|...}.|.d.
+000016f0: 1900 a009 a100 0100 7c00 6a06 a00a a100  ........|.j.....
+00001700: 0100 6e2d 7c00 6a03 6403 6b02 7256 7c00  ..n-|.j.d.k.rV|.
+00001710: 6a04 a00b a100 0100 740c a00d a100 8f0d  j.......t.......
+00001720: 0100 7c00 a00e 7c01 a101 7d02 5700 6404  ..|...|...}.W.d.
+00001730: 0400 0400 8303 0100 6e12 3100 7350 7701  ........n.1.sPw.
+00001740: 0100 0100 0100 5900 0100 6e09 740f 6405  ......Y...n.t.d.
+00001750: 7c00 6a03 9b00 6406 9d03 8301 8201 7c00  |.j...d.......|.
+00001760: a010 7c02 a101 0100 7c00 6a11 a012 a100  ..|.....|.j.....
+00001770: 0100 7c00 a013 a100 0100 6404 5300 2908  ..|.......d.S.).
+00001780: 7a2d 0a20 2020 2020 2020 2052 756e 2066  z-.        Run f
+00001790: 6f72 2061 2062 6174 6368 2028 6e6f 7420  or a batch (not 
+000017a0: 6570 6f63 6829 0a20 2020 2020 2020 2072  epoch).        r
+000017b0: 4f00 0000 7250 0000 0072 4500 0000 4efa  O...rP...rE...N.
+000017c0: 1055 6e65 7870 6563 7465 6420 6d6f 6465  .Unexpected mode
+000017d0: 20da 012e 720d 0000 0029 1472 3700 0000   ...r....).r7...
+000017e0: da04 6469 6374 721f 0000 0072 0f00 0000  ..dictr....r....
+000017f0: 7220 0000 0072 4f00 0000 7210 0000 00da  r ...rO...r.....
+00001800: 097a 6572 6f5f 6772 6164 da0a 7472 6169  .zero_grad..trai
+00001810: 6e5f 7374 6570 da08 6261 636b 7761 7264  n_step..backward
+00001820: 725c 0000 00da 0465 7661 6c72 1700 0000  r\.....evalr....
+00001830: da07 6e6f 5f67 7261 64da 0974 6573 745f  ..no_grad..test_
+00001840: 7374 6570 da0a 5661 6c75 6545 7272 6f72  step..ValueError
+00001850: da07 6c6f 6767 696e 6772 2800 0000 da0b  ..loggingr(.....
+00001860: 7570 6461 7465 5f73 7465 7072 6300 0000  update_steprc...
+00001870: 2903 722a 0000 0072 6b00 0000 da09 7374  ).r*...rk.....st
+00001880: 6570 5f64 6963 7472 0d00 0000 720d 0000  ep_dictr....r...
+00001890: 0072 2b00 0000 7268 0000 009b 0000 0073  .r+...rh.......s
+000018a0: 2000 0000 2404 0a01 0a01 0a01 0a01 0c01   ...$...........
+000018b0: 0c01 0a02 0a01 0a01 0c01 1eff 1203 0a02  ................
+000018c0: 0a01 0c01 7a11 5472 6169 6e65 722e 7275  ....z.Trainer.ru
+000018d0: 6e5f 6261 7463 6863 0200 0000 0000 0000  n_batchc........
+000018e0: 0000 0000 0700 0000 0400 0000 4300 0000  ............C...
+000018f0: f332 0000 007c 015c 037d 027d 037d 047c  .2...|.\.}.}.}.|
+00001900: 00a0 007c 02a1 017d 0564 0167 0174 017c  ...|...}.d.g.t.|
+00001910: 0283 0114 007d 067c 0674 02a0 037c 05a1  .....}.|.t...|..
+00001920: 0164 029c 0253 0029 0461 7601 0000 0a20  .d...S.).av.... 
+00001930: 2020 2020 2020 2055 6e75 7365 6420 6475         Unused du
+00001940: 6d6d 7920 6675 6e63 7469 6f6e 2079 6574  mmy function yet
+00001950: 2065 7869 7374 2074 6f20 7072 6f76 6964   exist to provid
+00001960: 6520 492f 4f20 666f 726d 6174 2069 6e66  e I/O format inf
+00001970: 6f72 6d61 7469 6f6e 2e0a 2020 2020 2020  ormation..      
+00001980: 2020 5468 6520 6261 7463 6820 6973 2061    The batch is a
+00001990: 2070 6172 7420 6f66 2074 6865 2064 6174   part of the dat
+000019a0: 6173 6574 2069 6e20 7468 6520 6461 7461  aset in the data
+000019b0: 6c6f 6164 6572 2066 6574 6368 6564 2076  loader fetched v
+000019c0: 6961 2020 5f5f 6765 7469 7465 6d5f 5f20  ia  __getitem__ 
+000019d0: 6d65 7468 6f64 2e0a 2020 2020 2020 2020  method..        
+000019e0: 5468 6520 6469 6374 696f 6e61 7279 2063  The dictionary c
+000019f0: 6f6e 7369 7374 7320 6f66 207b 2773 7472  onsists of {'str
+00001a00: 273a 2074 6f72 6368 2e74 656e 736f 7228  ': torch.tensor(
+00001a10: 7661 6c75 6529 7d2c 2061 6e64 206d 7573  value)}, and mus
+00001a20: 7420 696e 636c 7564 6520 276c 6f73 7327  t include 'loss'
+00001a30: 2e0a 2020 2020 2020 2020 4e6f 7465 2074  ..        Note t
+00001a40: 6861 7420 7468 6973 2066 756e 6374 696f  hat this functio
+00001a50: 6e20 776f 726b 206f 6e6c 7920 696e 2027  n work only in '
+00001a60: 7472 6169 6e27 206d 6f64 652c 2068 656e  train' mode, hen
+00001a70: 6365 2062 6163 6b28 2920 6d65 7468 6f64  ce back() method
+00001a80: 2069 6e20 6e6e 2e4d 6f64 756c 6520 6973   in nn.Module is
+00001a90: 206e 6563 6573 7361 7279 2e0a 2020 2020   necessary..    
+00001aa0: 2020 2020 e700 0000 0000 0000 00a9 0272      ...........r
+00001ab0: 5000 0000 725a 0000 004e a904 7220 0000  P...rZ...N..r ..
+00001ac0: 0072 3600 0000 7217 0000 0072 5a00 0000  .r6...r....rZ...
+00001ad0: a907 722a 0000 0072 6b00 0000 da01 78da  ..r*...rk.....x.
+00001ae0: 0179 da02 666e da07 6f75 7470 7574 7372  .y..fn..outputsr
+00001af0: 5000 0000 720d 0000 0072 0d00 0000 722b  P...r....r....r+
+00001b00: 0000 0072 7200 0000 b200 0000 f308 0000  ...rr...........
+00001b10: 000a 080a 010e 0110 017a 1254 7261 696e  .........z.Train
+00001b20: 6572 2e74 7261 696e 5f73 7465 7063 0200  er.train_stepc..
+00001b30: 0000 0000 0000 0000 0000 0700 0000 0400  ................
+00001b40: 0000 4300 0000 727b 0000 0029 0461 4601  ..C...r{...).aF.
+00001b50: 0000 0a20 2020 2020 2020 2055 6e75 7365  ...        Unuse
+00001b60: 6420 6475 6d6d 7920 6675 6e63 7469 6f6e  d dummy function
+00001b70: 2079 6574 2065 7869 7374 2074 6f20 7072   yet exist to pr
+00001b80: 6f76 6964 6520 492f 4f20 666f 726d 6174  ovide I/O format
+00001b90: 2069 6e66 6f72 6d61 7469 6f6e 2e0a 2020   information..  
+00001ba0: 2020 2020 2020 5468 6520 6261 7463 6820        The batch 
+00001bb0: 6973 2061 2070 6172 7420 6f66 2074 6865  is a part of the
+00001bc0: 2064 6174 6173 6574 2069 6e20 7468 6520   dataset in the 
+00001bd0: 6461 7461 6c6f 6164 6572 2066 6574 6368  dataloader fetch
+00001be0: 6564 2076 6961 2020 5f5f 6765 7469 7465  ed via  __getite
+00001bf0: 6d5f 5f20 6d65 7468 6f64 2e0a 2020 2020  m__ method..    
+00001c00: 2020 2020 5468 6520 6469 6374 696f 6e61      The dictiona
+00001c10: 7279 2063 6f6e 7369 7374 7320 6f66 207b  ry consists of {
+00001c20: 2773 7472 273a 2074 6f72 6368 2e74 656e  'str': torch.ten
+00001c30: 736f 7228 7661 6c75 6529 7d2c 2061 6e64  sor(value)}, and
+00001c40: 206d 7573 7420 696e 636c 7564 6520 276c   must include 'l
+00001c50: 6f73 7327 2e0a 2020 2020 2020 2020 4e6f  oss'..        No
+00001c60: 7465 2074 6861 7420 7468 6973 2066 756e  te that this fun
+00001c70: 6374 696f 6e20 776f 726b 206f 6e6c 7920  ction work only 
+00001c80: 696e 2027 7465 7374 2720 6d6f 6465 2e0a  in 'test' mode..
+00001c90: 2020 2020 2020 2020 727c 0000 0072 7d00          r|...r}.
+00001ca0: 0000 4e72 7e00 0000 727f 0000 0072 0d00  ..Nr~...r....r..
+00001cb0: 0000 720d 0000 0072 2b00 0000 7276 0000  ..r....r+...rv..
+00001cc0: 00bf 0000 0072 8400 0000 7a11 5472 6169  .....r....z.Trai
+00001cd0: 6e65 722e 7465 7374 5f73 7465 7072 7a00  ner.test_steprz.
+00001ce0: 0000 6302 0000 0000 0000 0000 0000 0004  ..c.............
+00001cf0: 0000 0006 0000 0043 0000 0073 6a00 0000  .......C...sj...
+00001d00: 7c01 a000 a100 4400 5d2e 5c02 7d02 7d03  |.....D.].\.}.}.
+00001d10: 7c00 6a01 6401 6b02 7219 7c00 6a02 7c02  |.j.d.k.r.|.j.|.
+00001d20: 1900 a003 7c00 a004 7c03 a101 a101 0100  ....|...|.......
+00001d30: 7104 7c00 6a01 6402 6b02 722a 7c00 6a05  q.|.j.d.k.r*|.j.
+00001d40: 7c02 1900 a003 7c00 a004 7c03 a101 a101  |.....|...|.....
+00001d50: 0100 7104 7406 6403 7c00 6a01 9b00 6404  ..q.t.d.|.j...d.
+00001d60: 9d03 8301 8201 6400 5300 2905 4e72 4f00  ......d.S.).NrO.
+00001d70: 0000 7245 0000 0072 6e00 0000 726f 0000  ..rE...rn...ro..
+00001d80: 0029 0772 4300 0000 720f 0000 0072 2200  .).rC...r....r".
+00001d90: 0000 da06 6170 7065 6e64 7230 0000 0072  ....appendr0...r
+00001da0: 2300 0000 7277 0000 0029 0472 2a00 0000  #...rw...).r*...
+00001db0: 727a 0000 0072 4000 0000 7241 0000 0072  rz...r@...rA...r
+00001dc0: 0d00 0000 720d 0000 0072 2b00 0000 7278  ....r....r+...rx
+00001dd0: 0000 00cc 0000 0073 0e00 0000 1001 0a01  .......s........
+00001de0: 1801 0a01 1801 1202 04fa 7a0f 5472 6169  ..........z.Trai
+00001df0: 6e65 722e 6c6f 6767 696e 6763 0200 0000  ner.loggingc....
+00001e00: 0000 0000 0000 0000 0200 0000 0200 0000  ................
+00001e10: 4300 0000 7326 0000 007c 0172 077c 017c  C...s&...|.r.|.|
+00001e20: 005f 0064 0353 007c 006a 0064 016b 0272  ._.d.S.|.j.d.k.r
+00001e30: 0e64 026e 0164 017c 005f 0064 0353 0029  .d.n.d.|._.d.S.)
+00001e40: 047a 460a 2020 2020 2020 2020 5377 6974  .zF.        Swit
+00001e50: 6368 696e 6720 6d6f 6465 2069 6e20 696e  ching mode in in
+00001e60: 7374 616e 6365 2e0a 2020 2020 2020 2020  stance..        
+00001e70: 3a70 6172 616d 206d 6f64 653a 2073 7472  :param mode: str
+00001e80: 0a20 2020 2020 2020 2072 4f00 0000 7245  .        rO...rE
+00001e90: 0000 004e 2901 720f 0000 0029 0272 2a00  ...N).r....).r*.
+00001ea0: 0000 720f 0000 0072 0d00 0000 720d 0000  ..r....r....r...
+00001eb0: 0072 2b00 0000 7258 0000 00d5 0000 0073  .r+...rX.......s
+00001ec0: 0600 0000 0405 0a01 1802 7a0e 5472 6169  ..........z.Trai
+00001ed0: 6e65 722e 746f 6767 6c65 7251 0000 0072  ner.togglerQ...r
+00001ee0: 5200 0000 6303 0000 0000 0000 0000 0000  R...c...........
+00001ef0: 0003 0000 0004 0000 0043 0000 0073 3800  .........C...s8.
+00001f00: 0000 7c02 7c00 6a00 6b04 7207 6401 5300  ..|.|.j.k.r.d.S.
+00001f10: 7c00 6a01 6402 1900 a002 7c01 a101 0100  |.j.d.....|.....
+00001f20: 7c00 6a01 6403 1900 a002 7c00 6a03 a004  |.j.d.....|.j...
+00001f30: a100 a101 0100 6401 5300 2904 7aa0 0a20  ......d.S.).z.. 
+00001f40: 2020 2020 2020 2043 6f6d 7061 7265 2074         Compare t
+00001f50: 6865 2063 7572 7265 6e74 206d 6f64 656c  he current model
+00001f60: 2061 6e64 2074 6865 2069 6e2d 6275 6666   and the in-buff
+00001f70: 6572 206d 6f64 656c 2e0a 2020 2020 2020  er model..      
+00001f80: 2020 5468 6520 6372 6974 6572 696f 6e20    The criterion 
+00001f90: 6973 206c 6f73 732e 0a20 2020 2020 2020  is loss..       
+00001fa0: 203a 7061 7261 6d20 6375 725f 6570 6f63   :param cur_epoc
+00001fb0: 683a 2069 6e74 0a20 2020 2020 2020 203a  h: int.        :
+00001fc0: 7061 7261 6d20 6375 725f 6c6f 7373 3a20  param cur_loss: 
+00001fd0: 666c 6f61 740a 2020 2020 2020 2020 4eda  float.        N.
+00001fe0: 0565 706f 6368 da06 7765 6967 6874 2905  .epoch..weight).
+00001ff0: 7225 0000 0072 2600 0000 7285 0000 0072  r%...r&...r....r
+00002000: 2000 0000 da0a 7374 6174 655f 6469 6374   .....state_dict
+00002010: 2903 722a 0000 0072 5100 0000 7252 0000  ).r*...rQ...rR..
+00002020: 0072 0d00 0000 720d 0000 0072 2b00 0000  .r....r....r+...
+00002030: 725b 0000 00df 0000 0073 0800 0000 0a07  r[.......s......
+00002040: 0401 1001 1a01 7a14 5472 6169 6e65 722e  ......z.Trainer.
+00002050: 6368 6563 6b5f 6265 7474 6572 6301 0000  check_betterc...
+00002060: 0000 0000 0000 0000 0001 0000 0002 0000  ................
+00002070: 0043 0000 0073 1800 0000 7c00 6a00 a001  .C...s....|.j...
+00002080: a100 0100 7c00 6a02 a001 a100 0100 6401  ....|.j.......d.
+00002090: 5300 2902 7a20 0a20 2020 2020 2020 2043  S.).z .        C
+000020a0: 6c65 6172 2074 6865 206c 6f67 2e0a 2020  lear the log..  
+000020b0: 2020 2020 2020 4e29 0372 2200 0000 da05        N).r".....
+000020c0: 636c 6561 7272 2300 0000 7234 0000 0072  clearr#...r4...r
+000020d0: 0d00 0000 720d 0000 0072 2b00 0000 7266  ....r....r+...rf
+000020e0: 0000 00eb 0000 0073 0400 0000 0a04 0e01  .......s........
+000020f0: 7a11 5472 6169 6e65 722e 6c6f 675f 7265  z.Trainer.log_re
+00002100: 7365 7472 6400 0000 7265 0000 0063 0300  setrd...re...c..
+00002110: 0000 0000 0000 0000 0000 0b00 0000 0800  ................
+00002120: 0000 4300 0000 73b8 0000 007c 006a 0064  ..C...s....|.j.d
+00002130: 016b 0272 087c 006a 016e 027c 006a 027d  .k.r.|.j.n.|.j.}
+00002140: 037c 006a 0372 167c 006a 036a 0464 0219  .|.j.r.|.j.j.d..
+00002150: 0064 0319 006e 0164 027d 047c 017c 026b  .d...n.d.}.|.|.k
+00002160: 027d 057c 0572 2064 006e 0274 056a 067d  .}.|.r d.n.t.j.}
+00002170: 067c 0572 2764 046e 0164 057d 0764 067c  .|.r'd.n.d.}.d.|
+00002180: 019b 0064 077c 029b 009d 047d 087c 03a0  ...d.|.....}.|..
+00002190: 07a1 0044 005d 175c 027d 097d 0a64 087c  ...D.].\.}.}.d.|
+000021a0: 0976 0072 3e71 357c 0864 097c 099b 0064  .v.r>q5|.d.|...d
+000021b0: 0a74 08a0 097c 0aa1 0164 0b9b 049d 0437  .t...|...d.....7
+000021c0: 007d 0871 357c 0864 0c7c 0464 0d9b 049d  .}.q5|.d.|.d....
+000021d0: 0237 007d 087c 087c 077c 0664 0e9c 0266  .7.}.|.|.|.d...f
+000021e0: 0253 0029 0f4e 724f 0000 0072 0100 0000  .S.).NrO...r....
+000021f0: da02 6c72 da01 0ada 007a 0a0d 0909 4261  ..lr.....z....Ba
+00002200: 7463 683a 20fa 012f da06 6f75 7470 7574  tch: ../..output
+00002210: da01 097a 023a 207a 032e 3666 7a05 094c  ...z.: z..6fz..L
+00002220: 523a 207a 032e 3365 2902 da03 656e 64da  R: z..3e)...end.
+00002230: 0466 696c 6529 0a72 0f00 0000 7222 0000  .file).r....r"..
+00002240: 0072 2300 0000 7210 0000 00da 0c70 6172  .r#...r......par
+00002250: 616d 5f67 726f 7570 73da 0373 7973 da06  am_groups..sys..
+00002260: 7374 6465 7272 7243 0000 0072 5900 0000  stderrrC...rY...
+00002270: 725a 0000 0029 0b72 2a00 0000 7264 0000  rZ...).r*...rd..
+00002280: 0072 6500 0000 da03 6c6f 67da 024c 525a  .re.....log..LRZ
+00002290: 0669 735f 656e 64da 0464 6973 7072 9000  .is_end..dispr..
+000022a0: 0000 5a07 6c6f 675f 7374 7272 4000 0000  ..Z.log_strr@...
+000022b0: 7241 0000 0072 0d00 0000 720d 0000 0072  rA...r....r....r
+000022c0: 2b00 0000 7269 0000 00f2 0000 0073 1800  +...ri.......s..
+000022d0: 0000 1601 1a01 0801 0e01 0c01 1002 1001  ................
+000022e0: 0801 0201 1e01 1001 0e02 7a11 5472 6169  ..........z.Trai
+000022f0: 6e65 722e 7072 696e 745f 6c6f 67da 0866  ner.print_log..f
+00002300: 696c 656e 616d 6563 0200 0000 0000 0000  ilenamec........
+00002310: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
+00002320: 7316 0000 0074 00a0 017c 006a 02a0 03a1  s....t...|.j....
+00002330: 007c 01a1 0201 0064 0053 0072 6100 0000  .|.....d.S.ra...
+00002340: 2904 7217 0000 00da 0473 6176 6572 2000  ).r......saver .
+00002350: 0000 7288 0000 0029 0272 2a00 0000 7298  ..r....).r*...r.
+00002360: 0000 0072 0d00 0000 720d 0000 0072 2b00  ...r....r....r+.
+00002370: 0000 da0a 7361 7665 5f6d 6f64 656c 0201  ....save_model..
+00002380: 0000 7302 0000 0016 017a 1254 7261 696e  ..s......z.Train
+00002390: 6572 2e73 6176 655f 6d6f 6465 6cda 0673  er.save_model..s
+000023a0: 7472 6963 7463 0300 0000 0000 0000 0000  trictc..........
+000023b0: 0000 0500 0000 0a00 0000 4300 0000 73a4  ..........C...s.
+000023c0: 0000 007a 1f7c 0172 0e74 006a 017c 0174  ...z.|.r.t.j.|.t
+000023d0: 00a0 0264 01a1 0164 028d 027d 036e 077c  ...d...d...}.n.|
+000023e0: 006a 0364 0319 0064 0419 007d 037c 006a  .j.d...d...}.|.j
+000023f0: 046a 057c 037c 0264 058d 0201 0057 0064  .j.|.|.d.....W.d
+00002400: 0753 0004 0074 0679 3a01 007d 0401 007a  .S...t.y:..}...z
+00002410: 0f74 0764 067c 019b 009d 027c 0483 0201  .t.d.|.....|....
+00002420: 0057 0059 0064 077d 047e 0464 0753 0064  .W.Y.d.}.~.d.S.d
+00002430: 077d 047e 0477 0104 0074 0879 5101 007d  .}.~.w...t.yQ..}
+00002440: 0401 007a 0c74 0764 087c 0483 0201 0057  ...z.t.d.|.....W
+00002450: 0059 0064 077d 047e 0464 0753 0064 077d  .Y.d.}.~.d.S.d.}
+00002460: 047e 0477 0177 0029 0961 0401 0000 0a20  .~.w.w.).a..... 
+00002470: 2020 2020 2020 2055 7064 6174 6520 6d6f         Update mo
+00002480: 6465 6c27 7320 7765 6967 6874 732e 0a20  del's weights.. 
+00002490: 2020 2020 2020 2049 6620 6669 6c65 6e61         If filena
+000024a0: 6d65 2069 7320 4e6f 6e65 2c20 6d6f 6465  me is None, mode
+000024b0: 6c20 7570 6461 7465 6420 7769 7468 206c  l updated with l
+000024c0: 6174 6573 7420 7765 6967 6874 2062 7566  atest weight buf
+000024d0: 6665 7220 696e 2074 6865 2069 6e73 7461  fer in the insta
+000024e0: 6e63 652e 0a20 2020 2020 2020 2049 6620  nce..        If 
+000024f0: 6e6f 742c 2074 6865 206d 6f64 656c 2069  not, the model i
+00002500: 7320 7570 6461 7465 6420 7769 7468 2077  s updated with w
+00002510: 6569 6768 7473 206c 6f61 6465 6420 6672  eights loaded fr
+00002520: 6f6d 2074 6865 2066 696c 656e 616d 652e  om the filename.
+00002530: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00002540: 6669 6c65 6e61 6d65 3a20 7374 720a 2020  filename: str.  
+00002550: 2020 2020 2020 3a70 6172 616d 2073 7472        :param str
+00002560: 6963 743a 2062 6f6f 6c0a 2020 2020 2020  ict: bool.      
+00002570: 2020 723a 0000 0029 01da 0c6d 6170 5f6c    r:...)...map_l
+00002580: 6f63 6174 696f 6e72 8700 0000 e9ff ffff  ocationr........
+00002590: ff29 0172 9b00 0000 7a11 4361 6e6e 6f74  .).r....z.Cannot
+000025a0: 2066 696e 6420 6669 6c65 204e 7a28 5468   find file Nz(Th
+000025b0: 6572 6520 6973 206e 6f20 7765 6967 6874  ere is no weight
+000025c0: 2069 6e20 6275 6666 6572 206f 6620 7472   in buffer of tr
+000025d0: 6169 6e65 722e 2909 7217 0000 00da 046c  ainer.).r......l
+000025e0: 6f61 6472 0e00 0000 7226 0000 0072 2000  oadr....r&...r .
+000025f0: 0000 da0f 6c6f 6164 5f73 7461 7465 5f64  ....load_state_d
+00002600: 6963 74da 1146 696c 654e 6f74 466f 756e  ict..FileNotFoun
+00002610: 6445 7272 6f72 7256 0000 00da 0a49 6e64  dErrorrV.....Ind
+00002620: 6578 4572 726f 7229 0572 2a00 0000 7298  exError).r*...r.
+00002630: 0000 0072 9b00 0000 da07 7765 6967 6874  ...r......weight
+00002640: 7372 5f00 0000 720d 0000 0072 0d00 0000  sr_...r....r....
+00002650: 722b 0000 00da 0d61 7070 6c79 5f77 6569  r+.....apply_wei
+00002660: 6768 7473 0501 0000 7318 0000 0002 0804  ghts....s.......
+00002670: 0116 010e 0216 010e 011e 0108 800e 0118  ................
+00002680: 0108 8002 ff7a 1554 7261 696e 6572 2e61  .....z.Trainer.a
+00002690: 7070 6c79 5f77 6569 6768 7473 6302 0000  pply_weightsc...
+000026a0: 0000 0000 0000 0000 0005 0000 0005 0000  ................
+000026b0: 0043 0000 0073 7e00 0000 7400 6401 8301  .C...s~...t.d...
+000026c0: 7d02 7c01 a001 a100 4400 5d34 5c02 7d03  }.|.....D.]4\.}.
+000026d0: 7d04 7c03 a002 a100 6402 7600 7224 7403  }.|.....d.v.r$t.
+000026e0: 7c04 7404 8302 721f 7405 6a06 6406 6900  |.t...r.t.j.d.i.
+000026f0: 7c04 a401 8e01 6e01 7c04 7c02 6403 3c00  |.....n.|.|.d.<.
+00002700: 7108 7c03 a002 a100 6404 7600 723c 7403  q.|.....d.v.r<t.
+00002710: 7c04 7404 8302 7237 7c00 6a07 6406 6900  |.t...r7|.j.d.i.
+00002720: 7c04 a401 8e01 6e01 7c04 7c02 6405 3c00  |.....n.|.|.d.<.
+00002730: 7108 7108 7c02 5300 2907 7ac2 0a20 2020  q.q.|.S.).z..   
+00002740: 2020 2020 2043 6865 636b 2067 6976 656e       Check given
+00002750: 2077 6562 5f6c 6f67 6765 7220 6973 2072   web_logger is r
+00002760: 756e 6e65 7220 6f62 6a65 6374 206f 7220  unner object or 
+00002770: 7275 6e6e 6572 2070 6172 616d 732e 0a20  runner params.. 
+00002780: 2020 2020 2020 2049 6620 7275 6e6e 6572         If runner
+00002790: 2070 6172 616d 7320 6172 6520 7072 6f76   params are prov
+000027a0: 6964 6564 2c20 696e 6974 206e 6577 2072  ided, init new r
+000027b0: 756e 6e65 7220 6f62 6a65 6374 2075 7369  unner object usi
+000027c0: 6e67 2074 686f 7365 2e0a 2020 2020 2020  ng those..      
+000027d0: 2020 3a70 6172 616d 2077 6562 5f6c 6f67    :param web_log
+000027e0: 6765 723a 0a20 2020 2020 2020 203a 7265  ger:.        :re
+000027f0: 7475 726e 3a0a 2020 2020 2020 2020 4e29  turn:.        N)
+00002800: 02da 0577 616e 6462 7a03 7726 6272 a400  ...wandbz.w&br..
+00002810: 0000 2905 da07 6e65 7074 756e 657a 0a6e  ..)...neptunez.n
+00002820: 6570 7475 6e65 2e61 695a 096e 6570 7475  eptune.aiZ.neptu
+00002830: 6e65 6169 7a0a 6e65 7074 756e 652d 6169  neaiz.neptune-ai
+00002840: 5a03 6e65 7072 a500 0000 720d 0000 0029  Z.nepr....r....)
+00002850: 0872 0400 0000 7243 0000 00da 056c 6f77  .r....rC.....low
+00002860: 6572 7237 0000 0072 7000 0000 72a4 0000  err7...rp...r...
+00002870: 00da 0469 6e69 74da 0869 6e69 745f 746b  ...init..init_tk
+00002880: 6e29 0572 2a00 0000 7214 0000 005a 0b6c  n).r*...r....Z.l
+00002890: 6f67 6765 725f 6469 6374 7240 0000 0072  ogger_dictr@...r
+000028a0: 4100 0000 720d 0000 0072 0d00 0000 722b  A...r....r....r+
+000028b0: 0000 0072 2900 0000 1801 0000 7310 0000  ...r).......s...
+000028c0: 0008 0710 010c 0124 010c 0124 0102 0304  .......$...$....
+000028d0: 017a 1854 7261 696e 6572 2e63 6865 636b  .z.Trainer.check
+000028e0: 5f77 6562 5f6c 6f67 6765 7272 8c00 0000  _web_loggerr....
+000028f0: da0c 7072 6f6a 6563 745f 6e61 6d65 da07  ..project_name..
+00002900: 6170 695f 746b 6e63 0300 0000 0000 0000  api_tknc........
+00002910: 0000 0000 0400 0000 0400 0000 4b00 0000  ............K...
+00002920: 7318 0000 0074 007c 017c 0266 0269 007c  s....t.|.|.f.i.|
+00002930: 03a4 018e 017c 005f 0164 0153 0029 0261  .....|._.d.S.).a
+00002940: 3b01 0000 0a20 2020 2020 2020 2049 6e69  ;....        Ini
+00002950: 7469 616c 697a 6520 6e65 7074 756e 6520  tialize neptune 
+00002960: 6c6f 6767 6572 2077 6974 6820 6769 7665  logger with give
+00002970: 6e20 7072 6f6a 6563 7420 6e61 6d65 2061  n project name a
+00002980: 6e64 2074 6f6b 656e 2e0a 2020 2020 2020  nd token..      
+00002990: 2020 5573 6167 653a 0a20 2020 2020 2020    Usage:.       
+000029a0: 2020 2020 2074 7261 696e 6572 2e69 6e69       trainer.ini
+000029b0: 745f 746b 6e28 5052 4f4a 4543 545f 4e41  t_tkn(PROJECT_NA
+000029c0: 4d45 2c20 4150 495f 544f 4b45 4e29 0a20  ME, API_TOKEN). 
+000029d0: 2020 2020 2020 203a 7061 7261 6d20 7072         :param pr
+000029e0: 6f6a 6563 745f 6e61 6d65 3a20 7374 720a  oject_name: str.
+000029f0: 2020 2020 2020 2020 3a70 6172 616d 2061          :param a
+00002a00: 7069 5f74 6b6e 3a20 7374 720a 2020 2020  pi_tkn: str.    
+00002a10: 2020 2020 3a70 6172 616d 206b 7761 7267      :param kwarg
+00002a20: 733a 2065 7874 7261 2068 6173 6861 626c  s: extra hashabl
+00002a30: 6520 666f 7220 7472 6163 6b69 6e67 206d  e for tracking m
+00002a40: 6f64 656c 2028 6f72 206f 7074 2c20 7363  odel (or opt, sc
+00002a50: 6865 6475 6c65 722c 2065 7463 2e2e 2e29  heduler, etc...)
+00002a60: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+00002a70: 3a20 4e6f 6e65 0a20 2020 2020 2020 204e  : None.        N
+00002a80: 2902 720b 0000 0072 1400 0000 2904 722a  ).r....r....).r*
+00002a90: 0000 0072 a900 0000 72aa 0000 0072 4400  ...r....r....rD.
+00002aa0: 0000 720d 0000 0072 0d00 0000 722b 0000  ..r....r....r+..
+00002ab0: 0072 a800 0000 2a01 0000 7302 0000 0018  .r....*...s.....
+00002ac0: 0a7a 1054 7261 696e 6572 2e69 6e69 745f  .z.Trainer.init_
+00002ad0: 746b 6e63 0100 0000 0000 0000 0000 0000  tknc............
+00002ae0: 0300 0000 0200 0000 4300 0000 7334 0000  ........C...s4..
+00002af0: 007c 006a 0064 0119 0004 007d 0172 0b7c  .|.j.d.....}.r.|
+00002b00: 01a0 01a1 0001 007c 006a 0064 0219 0004  .......|.j.d....
+00002b10: 007d 0272 187c 02a0 02a1 0001 0064 0353  .}.r.|.......d.S
+00002b20: 0064 0353 0029 047a 3e0a 2020 2020 2020  .d.S.).z>.      
+00002b30: 2020 456c 696d 696e 6174 6520 7765 625f    Eliminate web_
+00002b40: 6c6f 6767 6572 732e 0a20 2020 2020 2020  loggers..       
+00002b50: 203a 7265 7475 726e 3a20 4e6f 6e65 0a20   :return: None. 
+00002b60: 2020 2020 2020 2072 a400 0000 72a5 0000         r....r...
+00002b70: 004e 2903 7214 0000 00da 0666 696e 6973  .N).r......finis
+00002b80: 68da 0965 6c69 6d69 6e61 7465 2903 722a  h..eliminate).r*
+00002b90: 0000 005a 0677 625f 6c6f 675a 066e 705f  ...Z.wb_logZ.np_
+00002ba0: 6c6f 6772 0d00 0000 720d 0000 0072 2b00  logr....r....r+.
+00002bb0: 0000 da0e 656e 645f 7765 625f 6c6f 6767  ....end_web_logg
+00002bc0: 6572 3601 0000 730a 0000 000e 0508 010e  er6...s.........
+00002bd0: 010c 0104 ff7a 1654 7261 696e 6572 2e65  .....z.Trainer.e
+00002be0: 6e64 5f77 6562 5f6c 6f67 6765 7263 0200  nd_web_loggerc..
+00002bf0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00002c00: 0000 4300 0000 7322 0000 007c 00a0 0064  ..C...s"...|...d
+00002c10: 01a1 0101 007c 006a 0164 027c 0164 038d  .....|.j.d.|.d..
+00002c20: 0201 007c 006a 0264 0419 0053 0029 054e  ...|.j.d...S.).N
+00002c30: 7245 0000 0072 0a00 0000 2902 724b 0000  rE...r....).rK..
+00002c40: 0072 1900 0000 728e 0000 0029 0372 5800  .r....r....).rX.
+00002c50: 0000 7260 0000 0072 2300 0000 2902 722a  ..r`...r#...).r*
+00002c60: 0000 0072 1900 0000 720d 0000 0072 0d00  ...r....r....r..
+00002c70: 0000 722b 0000 00da 0969 6e66 6572 656e  ..r+.....inferen
+00002c80: 6365 4001 0000 7306 0000 000a 030e 010a  ce@...s.........
+00002c90: 017a 1154 7261 696e 6572 2e69 6e66 6572  .z.Trainer.infer
+00002ca0: 656e 6365 2905 4e4e 5472 0d00 0000 4e29  ence).NNTr....N)
+00002cb0: 0146 2902 722d 0000 004e 7261 0000 0029  .F).r-...Nra...)
+00002cc0: 024e 5429 0172 8c00 0000 292f da08 5f5f  .NT).r....)/..__
+00002cd0: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+00002ce0: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+00002cf0: da07 5f5f 646f 635f 5f72 1700 0000 720e  ..__doc__r....r.
+00002d00: 0000 00da 0373 7472 7208 0000 00da 056f  .....strr......o
+00002d10: 7074 696d da09 4f70 7469 6d69 7a65 72da  ptim..Optimizer.
+00002d20: 0462 6f6f 6c72 0900 0000 7270 0000 0072  .boolr....rp...r
+00002d30: 0700 0000 da06 6f62 6a65 6374 722c 0000  ......objectr,..
+00002d40: 0072 0500 0000 7238 0000 0072 3000 0000  .r....r8...r0...
+00002d50: da02 6e6e da06 4d6f 6475 6c65 721f 0000  ..nn..Moduler...
+00002d60: 0072 4900 0000 724a 0000 00da 0369 6e74  .rI...rJ.....int
+00002d70: 7260 0000 0072 6300 0000 7257 0000 0072  r`...rc...rW...r
+00002d80: 3b00 0000 7268 0000 0072 0300 0000 7206  ;...rh...r....r.
+00002d90: 0000 0072 7200 0000 7276 0000 0072 7800  ...rr...rv...rx.
+00002da0: 0000 7258 0000 00da 0566 6c6f 6174 725b  ..rX.....floatr[
+00002db0: 0000 0072 6600 0000 7269 0000 0072 9a00  ...rf...ri...r..
+00002dc0: 0000 72a3 0000 0072 2900 0000 72a8 0000  ..r....r)...r...
+00002dd0: 0072 ad00 0000 7221 0000 0072 ae00 0000  .r....r!...r....
+00002de0: 720d 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
+00002df0: 2b00 0000 720c 0000 000e 0000 0073 5e00  +...r........s^.
+00002e00: 0000 0800 0401 0214 0201 0201 0201 0201  ................
+00002e10: 04f7 0403 02fd 0204 02fc 0a05 02fb 0206  ................
+00002e20: 02fa 0207 02f9 0208 02f8 1609 0af7 1e1c  ................
+00002e30: 020f 2602 0afe 0c10 080d 1407 081d 0a05  ..&.............
+00002e40: 1a0c 0217 2601 020c 2601 1c0c 1409 160a  ....&...&.......
+00002e50: 0a0c 1e07 1210 1803 3213 1812 0a0c 120a  ........2.......
+00002e60: 720c 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00002e70: 0000 0000 0000 0200 0000 4000 0000 7334  ..........@...s4
+00002e80: 0000 0065 005a 0164 005a 0264 0164 0284  ...e.Z.d.Z.d.d..
+00002e90: 005a 0364 0364 0484 005a 0464 0564 0684  .Z.d.d...Z.d.d..
+00002ea0: 005a 0564 0764 0884 005a 0664 0964 0a84  .Z.d.d...Z.d.d..
+00002eb0: 005a 0764 0b53 0029 0c72 2700 0000 6301  .Z.d.S.).r'...c.
+00002ec0: 0000 0000 0000 0000 0000 0001 0000 0002  ................
+00002ed0: 0000 0043 0000 0073 1000 0000 6401 7c00  ...C...s....d.|.
+00002ee0: 5f00 6401 7c00 5f01 6400 5300 a902 4e72  _.d.|._.d.S...Nr
+00002ef0: 0a00 0000 2902 da16 5f50 726f 6772 6573  ....)..._Progres
+00002f00: 7343 6865 636b 6572 5f5f 7374 6570 da17  sChecker__step..
+00002f10: 5f50 726f 6772 6573 7343 6865 636b 6572  _ProgressChecker
+00002f20: 5f5f 6570 6f63 6872 3400 0000 720d 0000  __epochr4...r...
+00002f30: 0072 0d00 0000 722b 0000 0072 2c00 0000  .r....r+...r,...
+00002f40: 4901 0000 7304 0000 0006 010a 017a 1850  I...s........z.P
+00002f50: 726f 6772 6573 7343 6865 636b 6572 2e5f  rogressChecker._
+00002f60: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
+00002f70: 0000 0000 0100 0000 0300 0000 4300 0000  ............C...
+00002f80: f312 0000 007c 0004 006a 0064 0137 0002  .....|...j.d.7..
+00002f90: 005f 0064 0053 0072 bc00 0000 a901 72bd  ._.d.S.r......r.
+00002fa0: 0000 0072 3400 0000 720d 0000 0072 0d00  ...r4...r....r..
+00002fb0: 0000 722b 0000 0072 7900 0000 4d01 0000  ..r+...ry...M...
+00002fc0: f302 0000 0012 017a 1b50 726f 6772 6573  .......z.Progres
+00002fd0: 7343 6865 636b 6572 2e75 7064 6174 655f  sChecker.update_
+00002fe0: 7374 6570 6301 0000 0000 0000 0000 0000  stepc...........
+00002ff0: 0001 0000 0003 0000 0043 0000 0072 bf00  .........C...r..
+00003000: 0000 72bc 0000 00a9 0172 be00 0000 7234  ..r......r....r4
+00003010: 0000 0072 0d00 0000 720d 0000 0072 2b00  ...r....r....r+.
+00003020: 0000 725d 0000 0050 0100 0072 c100 0000  ..r]...P...r....
+00003030: 7a1c 5072 6f67 7265 7373 4368 6563 6b65  z.ProgressChecke
+00003040: 722e 7570 6461 7465 5f65 706f 6368 6301  r.update_epochc.
+00003050: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+00003060: 0000 0043 0000 00f3 0600 0000 7c00 6a00  ...C........|.j.
+00003070: 5300 7261 0000 0072 c000 0000 7234 0000  S.ra...r....r4..
+00003080: 0072 0d00 0000 720d 0000 0072 2b00 0000  .r....r....r+...
+00003090: da08 6765 745f 7374 6570 5301 0000 f302  ..get_stepS.....
+000030a0: 0000 0006 017a 1850 726f 6772 6573 7343  .....z.ProgressC
+000030b0: 6865 636b 6572 2e67 6574 5f73 7465 7063  hecker.get_stepc
+000030c0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000030d0: 0100 0000 4300 0000 72c3 0000 0072 6100  ....C...r....ra.
+000030e0: 0000 72c2 0000 0072 3400 0000 720d 0000  ..r....r4...r...
+000030f0: 0072 0d00 0000 722b 0000 00da 0967 6574  .r....r+.....get
+00003100: 5f65 706f 6368 5601 0000 72c5 0000 007a  _epochV...r....z
+00003110: 1950 726f 6772 6573 7343 6865 636b 6572  .ProgressChecker
+00003120: 2e67 6574 5f65 706f 6368 4e29 0872 af00  .get_epochN).r..
+00003130: 0000 72b0 0000 0072 b100 0000 722c 0000  ..r....r....r,..
+00003140: 0072 7900 0000 725d 0000 0072 c400 0000  .ry...r]...r....
+00003150: 72c6 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
+00003160: 0d00 0000 722b 0000 0072 2700 0000 4801  ....r+...r'...H.
+00003170: 0000 730c 0000 0008 0008 0108 0408 0308  ..s.............
+00003180: 030c 0372 2700 0000 2915 7293 0000 00da  ...r'...).r.....
+00003190: 0361 6263 7202 0000 0072 0300 0000 da0b  .abcr....r......
+000031a0: 636f 6c6c 6563 7469 6f6e 7372 0400 0000  collectionsr....
+000031b0: da06 7479 7069 6e67 7205 0000 0072 0600  ..typingr....r..
+000031c0: 0000 7207 0000 0072 0800 0000 7209 0000  ..r....r....r...
+000031d0: 0072 5300 0000 72a4 0000 00da 056e 756d  .rS...r......num
+000031e0: 7079 7259 0000 0072 1700 0000 da05 7574  pyrY...r......ut
+000031f0: 696c 7372 0b00 0000 720c 0000 0072 2700  ilsr....r....r'.
+00003200: 0000 720d 0000 0072 0d00 0000 720d 0000  ..r....r....r...
+00003210: 0072 2b00 0000 da08 3c6d 6f64 756c 653e  .r+.....<module>
+00003220: 0100 0000 731a 0000 0008 0010 010c 011c  ....s...........
+00003230: 0108 0208 0108 0108 010c 0210 0300 7f00  ................
+00003240: 7f12 3c                                  ..<
```

### Comparing `zae_engine-0.1.2/zae_engine/trainer/__pycache__/mpu_utils.cpython-310.pyc` & `zae_engine-0.1.3/zae_engine/trainer/__pycache__/mpu_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zae_engine-0.1.2/zae_engine/trainer/_trainer.py` & `zae_engine-0.1.3/zae_engine/trainer/_trainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import sys
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from typing import Tuple, Dict, Union, Optional, Iterable
 
+import tqdm
 import wandb
 import numpy as np
 import torch
 
 from .utils import NeptuneLogger
 
 
@@ -29,23 +30,25 @@
     def __init__(
         self,
         model,
         device: torch.device,
         mode: str,
         optimizer: Optional[torch.optim.Optimizer] = None,
         scheduler: Optional = None,
+        log_bar: bool = True,
         callbacks: Iterable = (),
         web_logger: Optional[dict[str, Union[object, dict]]] = None,
     ):
         if "cuda" in device.type:
             torch.cuda.set_device(device)  # Not for device in ['cpu', 'mps']
         self.device = device
         self.loader, self.n_data, self.batch_size = None, None, None
         self.valid_loader, self.n_valid_data, self.valid_batch_size = None, None, None
         self.mode = mode
+        self.log_bar = log_bar
         self.optimizer = optimizer
         self.scheduler = scheduler
         self.model = self._to_device(model)
         self.log_train, self.log_test = defaultdict(list), defaultdict(list)
         self.loss_buffer, self.weight_buffer = torch.inf, defaultdict(list)
         self.callbacks = callbacks
         self.progress_checker = ProgressChecker()
@@ -110,16 +113,20 @@
         :param n_epoch:
         :param loader:
         :param valid_loader:
         :return:
         """
         self.loader, self.valid_loader = loader, valid_loader
         self._check_batch_size()
-        for e in range(n_epoch):
-            print("Epoch %d" % (e + 1))
+        progress = tqdm.tqdm(range(n_epoch), position=0, leave=True) if self.log_bar else range(n_epoch)
+        for e in progress:
+            if self.log_bar:
+                progress.set_description("Epoch %d" % (e + 1))
+            else:
+                print("Epoch %d" % (e + 1))
             self._data_count(initial=True)
             self.run_epoch(loader)
             if valid_loader:
                 self.toggle()
                 self.run_epoch(valid_loader)
                 self.toggle()
             if self.mode == "train":
@@ -131,18 +138,23 @@
     def run_callback(self):
         if self.callbacks:
             for cb in self.callbacks:
                 cb(self)  # replace even
 
     def run_epoch(self, loader) -> None:
         self.log_reset()
-        for i, batch in enumerate(loader):
+        progress = tqdm.tqdm(loader, position=1, leave=False) if self.log_bar else loader
+        for i, batch in enumerate(progress):
             self.run_batch(batch)
             self._data_count()
-            self.print_log(cur_batch=i + 1, num_batch=len(loader))
+            desc, printer = self.print_log(cur_batch=i + 1, num_batch=len(loader))
+            if self.log_bar:
+                progress.set_description(desc)
+            else:
+                print(desc, **printer)
 
     def run_batch(self, batch: Union[tuple, dict]) -> None:
         """
         Run for a batch (not epoch)
         """
         batch = self._to_device(**batch) if isinstance(batch, dict) else self._to_device(*batch)
         if self.mode == "train":
@@ -223,28 +235,29 @@
     def log_reset(self) -> None:
         """
         Clear the log.
         """
         self.log_train.clear()
         self.log_test.clear()
 
-    def print_log(self, cur_batch: int, num_batch: int) -> None:
+    def print_log(self, cur_batch: int, num_batch: int) -> Tuple[str, dict]:
         log = self.log_train if self.mode == "train" else self.log_test
         LR = self.optimizer.param_groups[0]["lr"] if self.optimizer else 0
         is_end = cur_batch == num_batch
         disp = None if is_end else sys.stderr
         end = "\n" if is_end else ""
 
         log_str = f"\r\t\tBatch: {cur_batch}/{num_batch}"
         for k, v in log.items():
             if "output" in k:
                 continue
             log_str += f"\t{k}: {np.mean(v):.6f}"
         log_str += f"\tLR: {LR:.3e}"
-        print(log_str, end=end, file=disp)
+        # print(log_str, end=end, file=disp)
+        return log_str, {"end": end, "file": disp}
 
     def save_model(self, filename: str) -> None:
         torch.save(self.model.state_dict(), filename)
 
     def apply_weights(self, filename: str = None, strict: bool = True) -> None:
         """
         Update model's weights.
@@ -301,16 +314,16 @@
         """
         if wb_log := self.web_logger["wandb"]:
             wb_log.finish()
         if np_log := self.web_logger["neptune"]:
             np_log.eliminate()
 
     def inference(self, loader) -> list:
-        if self.web_logger:
-            self.end_web_logger()
+        # if self.web_logger:
+        #     self.end_web_logger()
         self.toggle("test")
         self.run(n_epoch=1, loader=loader)
         return self.log_test["output"]
 
 
 class ProgressChecker:
     def __init__(self):
```

### Comparing `zae_engine-0.1.2/zae_engine/trainer/mpu_utils.py` & `zae_engine-0.1.3/zae_engine/trainer/mpu_utils.py`

 * *Files identical despite different names*

### Comparing `zae_engine-0.1.2/zae_engine/trainer/utils/__pycache__/_callback.cpython-310.pyc` & `zae_engine-0.1.3/zae_engine/trainer/utils/__pycache__/_callback.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `zae_engine-0.1.2/zae_engine/trainer/utils/__pycache__/_logger.cpython-310.pyc` & `zae_engine-0.1.3/zae_engine/trainer/utils/__pycache__/_logger.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Feb  6 02:03:49 2024 UTC, .py size: 2164 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8593 c165 7408 0000  o..........et...
+00000000: 6f0d 0d0a 0000 0000 d5f1 fc65 7408 0000  o..........et...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a03 6400 6403 6c04 6d05 5a06 0100 4700  Z.d.d.l.m.Z...G.
 00000050: 6404 6405 8400 6405 8302 5a07 6402 5300  d.d...d...Z.d.S.
 00000060: 2906 e900 0000 0029 01da 0770 6172 7469  )......)...parti
 00000070: 616c 4e29 01da 1f4e 6570 7475 6e65 496e  alN)...NeptuneIn
```

### Comparing `zae_engine-0.1.2/zae_engine/trainer/utils/_callback.py` & `zae_engine-0.1.3/zae_engine/trainer/utils/_callback.py`

 * *Files identical despite different names*

### Comparing `zae_engine-0.1.2/zae_engine/trainer/utils/_logger.py` & `zae_engine-0.1.3/zae_engine/trainer/utils/_logger.py`

 * *Files identical despite different names*

### Comparing `zae_engine-0.1.2/zae_engine/utils/__pycache__/io.cpython-310.pyc` & `zae_engine-0.1.3/zae_engine/utils/__pycache__/io.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Feb  6 02:03:49 2024 UTC, .py size: 727 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8593 c165 d702 0000  o..........e....
+00000000: 6f0d 0d0a 0000 0000 d5f1 fc65 d702 0000  o..........e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6403 6c02 6d03 5a03 0100 6400  Z.d.d.l.m.Z...d.
 00000050: 6402 6c04 5a05 6400 6402 6c06 5a06 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6402 6c07 5a07 6700 6404 a201 5a08 640a  d.l.Z.g.d...Z.d.
 00000070: 6405 6509 6406 6509 6407 6501 6402 6503  d.e.d.e.d.e.d.e.
```

### Comparing `zae_engine-0.1.2/PKG-INFO` & `zae_engine-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 Metadata-Version: 2.1
 Name: zae-engine
-Version: 0.1.2
+Version: 0.1.3
 Summary: Deep learning engine powered by zae-park.
 Author: zae-park
 Author-email: tom941105@gmail.com
 Requires-Python: >=3.10.0,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.7,<9.0.0)
+Requires-Dist: codecov (>=2.1.13,<3.0.0)
 Requires-Dist: einops (>=0.6.1,<0.7.0)
 Requires-Dist: future (>=0.18.3,<0.19.0)
+Requires-Dist: genbadge (>=1.1.1,<2.0.0)
 Requires-Dist: image-ocr (>=0.0.4,<0.0.5)
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
 Requires-Dist: keras-ocr (==0.8.9)
 Requires-Dist: matplotlib (>=3.7.2,<4.0.0)
 Requires-Dist: minio (>=7.1.17,<8.0.0)
 Requires-Dist: neptune (>=1.8.2,<2.0.0)
 Requires-Dist: neurokit2 (>=0.2.6,<0.3.0)
 Requires-Dist: nibabel (>=5.1.0,<6.0.0)
-Requires-Dist: onnx (==1.14.1)
 Requires-Dist: opencv-python-headless (>=4.8.0.76,<5.0.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.1.2,<3.0.0)
 Requires-Dist: pillow (>=10.1.0,<11.0.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: pytest (>=7.4.2,<8.0.0)
+Requires-Dist: pytest-cov (>=5.0.0,<6.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.5.2,<14.0.0)
 Requires-Dist: scikit-learn (>=1.3.1,<2.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Requires-Dist: segment-anything (>=1.0,<2.0)
+Requires-Dist: sphinx (>=7.2.6,<8.0.0)
+Requires-Dist: sphinx-rtd-theme (>=2.0.0,<3.0.0)
 Requires-Dist: tensorflow (>=2.13.0,<3.0.0)
 Requires-Dist: tensorflow-intel (>=2.14.0,<3.0.0) ; sys_platform == "win64"
 Requires-Dist: tensorflow-io-gcs-filesystem (==0.31.0)
 Requires-Dist: termcolor (==2.2.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: typeguard (>=4.1.2,<5.0.0)
 Requires-Dist: ultralytics (==8.0.155)
```

