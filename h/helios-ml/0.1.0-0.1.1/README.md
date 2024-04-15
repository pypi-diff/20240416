# Comparing `tmp/helios-ml-0.1.0.tar.gz` & `tmp/helios_ml-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helios-ml-0.1.0.tar", last modified: Sat Apr 13 01:49:05 2024, max compression
+gzip compressed data, was "helios_ml-0.1.1.tar", last modified: Mon Apr 15 22:25:56 2024, max compression
```

## Comparing `helios-ml-0.1.0.tar` & `helios_ml-0.1.1.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 01:49:05.434610 helios-ml-0.1.0/
-drwxrwxrwx   0        0        0        0 2024-04-13 01:49:05.369379 helios-ml-0.1.0/.github/
-drwxrwxrwx   0        0        0        0 2024-04-13 01:49:05.380100 helios-ml-0.1.0/.github/workflows/
--rw-rw-rw-   0        0        0     1112 2024-04-13 01:32:20.000000 helios-ml-0.1.0/.github/workflows/publish.yml
--rw-rw-rw-   0        0        0     1461 2024-04-13 01:32:20.000000 helios-ml-0.1.0/.github/workflows/tests.yml
--rw-rw-rw-   0        0        0      245 2024-04-13 01:32:20.000000 helios-ml-0.1.0/.gitignore
--rw-rw-rw-   0        0        0      779 2024-04-13 01:32:20.000000 helios-ml-0.1.0/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0     1511 2024-04-13 01:32:20.000000 helios-ml-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     5196 2024-04-13 01:49:05.434610 helios-ml-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3705 2024-04-13 01:32:20.000000 helios-ml-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-13 01:49:05.369379 helios-ml-0.1.0/data/
-drwxrwxrwx   0        0        0        0 2024-04-13 01:49:05.380100 helios-ml-0.1.0/data/logo/
--rw-rw-rw-   0        0        0    20058 2024-04-13 01:32:20.000000 helios-ml-0.1.0/data/logo/logo-background.png
--rw-rw-rw-   0        0        0    14627 2024-04-13 01:32:20.000000 helios-ml-0.1.0/data/logo/logo-transparent.png
-drwxrwxrwx   0        0        0        0 2024-04-13 01:49:05.369379 helios-ml-0.1.0/examples/
-drwxrwxrwx   0        0        0        0 2024-04-13 01:49:05.380100 helios-ml-0.1.0/examples/cifar10/
--rw-rw-rw-   0        0        0    11400 2024-04-13 01:32:20.000000 helios-ml-0.1.0/examples/cifar10/cifar10.py
--rw-rw-rw-   0        0        0     2234 2024-04-13 01:32:20.000000 helios-ml-0.1.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-13 01:49:05.384609 helios-ml-0.1.0/requirements/
--rw-rw-rw-   0        0        0      409 2024-04-13 01:32:20.000000 helios-ml-0.1.0/requirements/ci.txt
--rw-rw-rw-   0        0        0      300 2024-04-13 01:32:20.000000 helios-ml-0.1.0/requirements/default.txt
--rw-rw-rw-   0        0        0      440 2024-04-13 01:32:20.000000 helios-ml-0.1.0/requirements/dev.txt
--rw-rw-rw-   0        0        0       42 2024-04-13 01:49:05.434610 helios-ml-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-13 01:49:05.374385 helios-ml-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-13 01:49:05.384609 helios-ml-0.1.0/src/helios/
--rw-rw-rw-   0        0        0       53 2024-04-13 01:32:20.000000 helios-ml-0.1.0/src/helios/__init__.py
--rw-rw-rw-   0        0        0      155 2024-04-13 01:32:20.000000 helios-ml-0.1.0/src/helios/_version.py
-drwxrwxrwx   0        0        0        0 2024-04-13 01:49:05.384609 helios-ml-0.1.0/src/helios/core/
--rw-rw-rw-   0        0        0      446 2024-04-13 01:32:20.000000 helios-ml-0.1.0/src/helios/core/__init__.py
--rw-rw-rw-   0        0        0      254 2024-04-13 01:32:20.000000 helios-ml-0.1.0/src/helios/core/cuda.py
--rw-rw-rw-   0        0        0     5408 2024-04-13 01:32:20.000000 helios-ml-0.1.0/src/helios/core/distributed.py
--rw-rw-rw-   0        0        0    17253 2024-04-13 01:32:20.000000 helios-ml-0.1.0/src/helios/core/logging.py
--rw-rw-rw-   0        0        0     4345 2024-04-13 01:32:20.000000 helios-ml-0.1.0/src/helios/core/rng.py
--rw-rw-rw-   0        0        0    13227 2024-04-13 01:32:20.000000 helios-ml-0.1.0/src/helios/core/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-13 01:49:05.384609 helios-ml-0.1.0/src/helios/data/
--rw-rw-rw-   0        0        0      530 2024-04-13 01:32:20.000000 helios-ml-0.1.0/src/helios/data/__init__.py
--rw-rw-rw-   0        0        0    12646 2024-04-13 01:32:20.000000 helios-ml-0.1.0/src/helios/data/datamodule.py
--rw-rw-rw-   0        0        0     5263 2024-04-13 01:32:20.000000 helios-ml-0.1.0/src/helios/data/functional.py
--rw-rw-rw-   0        0        0     7733 2024-04-13 01:32:20.000000 helios-ml-0.1.0/src/helios/data/samplers.py
--rw-rw-rw-   0        0        0     2332 2024-04-13 01:32:20.000000 helios-ml-0.1.0/src/helios/data/transforms.py
-drwxrwxrwx   0        0        0        0 2024-04-13 01:49:05.394604 helios-ml-0.1.0/src/helios/losses/
--rw-rw-rw-   0        0        0      261 2024-04-13 01:32:20.000000 helios-ml-0.1.0/src/helios/losses/__init__.py
--rw-rw-rw-   0        0        0      545 2024-04-13 01:32:20.000000 helios-ml-0.1.0/src/helios/losses/utils.py
--rw-rw-rw-   0        0        0     1504 2024-04-13 01:32:20.000000 helios-ml-0.1.0/src/helios/losses/weighted_loss.py
-drwxrwxrwx   0        0        0        0 2024-04-13 01:49:05.396150 helios-ml-0.1.0/src/helios/metrics/
--rw-rw-rw-   0        0        0      488 2024-04-13 01:32:20.000000 helios-ml-0.1.0/src/helios/metrics/__init__.py
--rw-rw-rw-   0        0        0    13882 2024-04-13 01:32:20.000000 helios-ml-0.1.0/src/helios/metrics/functional.py
--rw-rw-rw-   0        0        0     7376 2024-04-13 01:32:20.000000 helios-ml-0.1.0/src/helios/metrics/metrics.py
-drwxrwxrwx   0        0        0        0 2024-04-13 01:49:05.396150 helios-ml-0.1.0/src/helios/model/
--rw-rw-rw-   0        0        0      286 2024-04-13 01:32:20.000000 helios-ml-0.1.0/src/helios/model/__init__.py
--rw-rw-rw-   0        0        0    12625 2024-04-13 01:32:20.000000 helios-ml-0.1.0/src/helios/model/model.py
--rw-rw-rw-   0        0        0     1465 2024-04-13 01:32:20.000000 helios-ml-0.1.0/src/helios/model/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-13 01:49:05.396150 helios-ml-0.1.0/src/helios/nn/
--rw-rw-rw-   0        0        0      330 2024-04-13 01:32:20.000000 helios-ml-0.1.0/src/helios/nn/__init__.py
--rw-rw-rw-   0        0        0     1847 2024-04-13 01:32:20.000000 helios-ml-0.1.0/src/helios/nn/swa_utils.py
--rw-rw-rw-   0        0        0     1750 2024-04-13 01:32:20.000000 helios-ml-0.1.0/src/helios/nn/utils.py
--rw-rw-rw-   0        0        0     1857 2024-04-13 01:32:20.000000 helios-ml-0.1.0/src/helios/onnx.py
-drwxrwxrwx   0        0        0        0 2024-04-13 01:49:05.396150 helios-ml-0.1.0/src/helios/optim/
--rw-rw-rw-   0        0        0      226 2024-04-13 01:32:20.000000 helios-ml-0.1.0/src/helios/optim/__init__.py
--rw-rw-rw-   0        0        0      923 2024-04-13 01:32:20.000000 helios-ml-0.1.0/src/helios/optim/utils.py
--rw-rw-rw-   0        0        0        0 2024-04-13 01:32:20.000000 helios-ml-0.1.0/src/helios/py.typed
-drwxrwxrwx   0        0        0        0 2024-04-13 01:49:05.396150 helios-ml-0.1.0/src/helios/scheduler/
--rw-rw-rw-   0        0        0      364 2024-04-13 01:32:20.000000 helios-ml-0.1.0/src/helios/scheduler/__init__.py
--rw-rw-rw-   0        0        0     4896 2024-04-13 01:32:20.000000 helios-ml-0.1.0/src/helios/scheduler/schedulers.py
--rw-rw-rw-   0        0        0      962 2024-04-13 01:32:20.000000 helios-ml-0.1.0/src/helios/scheduler/utils.py
--rw-rw-rw-   0        0        0    35393 2024-04-13 01:32:20.000000 helios-ml-0.1.0/src/helios/trainer.py
-drwxrwxrwx   0        0        0        0 2024-04-13 01:49:05.434610 helios-ml-0.1.0/src/helios_ml.egg-info/
--rw-rw-rw-   0        0        0     5196 2024-04-13 01:49:05.000000 helios-ml-0.1.0/src/helios_ml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1884 2024-04-13 01:49:05.000000 helios-ml-0.1.0/src/helios_ml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 01:49:05.000000 helios-ml-0.1.0/src/helios_ml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      436 2024-04-13 01:49:05.000000 helios-ml-0.1.0/src/helios_ml.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-13 01:49:05.000000 helios-ml-0.1.0/src/helios_ml.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-13 01:49:05.428104 helios-ml-0.1.0/test/
--rw-rw-rw-   0        0        0        0 2024-04-13 01:32:20.000000 helios-ml-0.1.0/test/__init__.py
--rw-rw-rw-   0        0        0     2425 2024-04-13 01:32:20.000000 helios-ml-0.1.0/test/conftest.py
-drwxrwxrwx   0        0        0        0 2024-04-13 01:49:05.428104 helios-ml-0.1.0/test/registry_test/
--rw-rw-rw-   0        0        0       70 2024-04-13 01:32:20.000000 helios-ml-0.1.0/test/registry_test/__init__.py
--rw-rw-rw-   0        0        0       49 2024-04-13 01:32:20.000000 helios-ml-0.1.0/test/registry_test/extra.py
--rw-rw-rw-   0        0        0      102 2024-04-13 01:32:20.000000 helios-ml-0.1.0/test/registry_test/foo.py
--rw-rw-rw-   0        0        0      139 2024-04-13 01:32:20.000000 helios-ml-0.1.0/test/registry_test/func_registry.py
-drwxrwxrwx   0        0        0        0 2024-04-13 01:49:05.434610 helios-ml-0.1.0/test/registry_test/nested/
--rw-rw-rw-   0        0        0        0 2024-04-13 01:32:20.000000 helios-ml-0.1.0/test/registry_test/nested/__init__.py
--rw-rw-rw-   0        0        0      103 2024-04-13 01:32:20.000000 helios-ml-0.1.0/test/registry_test/nested/bar.py
--rw-rw-rw-   0        0        0       63 2024-04-13 01:32:20.000000 helios-ml-0.1.0/test/registry_test/nested/extra.py
--rw-rw-rw-   0        0        0        0 2024-04-13 01:32:20.000000 helios-ml-0.1.0/test/registry_test/py.typed
--rw-rw-rw-   0        0        0     4751 2024-04-13 01:32:20.000000 helios-ml-0.1.0/test/test_core.py
--rw-rw-rw-   0        0        0     7923 2024-04-13 01:32:20.000000 helios-ml-0.1.0/test/test_data.py
--rw-rw-rw-   0        0        0      730 2024-04-13 01:32:20.000000 helios-ml-0.1.0/test/test_losses.py
--rw-rw-rw-   0        0        0      574 2024-04-13 01:32:20.000000 helios-ml-0.1.0/test/test_metrics.py
--rw-rw-rw-   0        0        0     2108 2024-04-13 01:32:20.000000 helios-ml-0.1.0/test/test_model.py
--rw-rw-rw-   0        0        0     1144 2024-04-13 01:32:20.000000 helios-ml-0.1.0/test/test_nn.py
--rw-rw-rw-   0        0        0     1000 2024-04-13 01:32:20.000000 helios-ml-0.1.0/test/test_onnx.py
--rw-rw-rw-   0        0        0      316 2024-04-13 01:32:20.000000 helios-ml-0.1.0/test/test_optim.py
--rw-rw-rw-   0        0        0      508 2024-04-13 01:32:20.000000 helios-ml-0.1.0/test/test_scheduler.py
--rw-rw-rw-   0        0        0    11800 2024-04-13 01:32:20.000000 helios-ml-0.1.0/test/test_trainer.py
-drwxrwxrwx   0        0        0        0 2024-04-13 01:49:05.434610 helios-ml-0.1.0/tools/
--rw-rw-rw-   0        0        0     1642 2024-04-13 01:32:20.000000 helios-ml-0.1.0/tools/generate_requirements.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:25:56.469020 helios_ml-0.1.1/
+drwxrwxrwx   0        0        0        0 2024-04-15 22:25:56.431492 helios_ml-0.1.1/.github/
+drwxrwxrwx   0        0        0        0 2024-04-15 22:25:56.437004 helios_ml-0.1.1/.github/workflows/
+-rw-rw-rw-   0        0        0     1108 2024-04-15 22:25:46.000000 helios_ml-0.1.1/.github/workflows/publish.yml
+-rw-rw-rw-   0        0        0     1482 2024-04-15 21:39:15.000000 helios_ml-0.1.1/.github/workflows/tests.yml
+-rw-rw-rw-   0        0        0      245 2024-04-12 23:20:25.000000 helios_ml-0.1.1/.gitignore
+-rw-rw-rw-   0        0        0      779 2024-04-12 23:17:15.000000 helios_ml-0.1.1/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0     1511 2024-04-12 23:17:15.000000 helios_ml-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     7527 2024-04-15 22:25:56.469020 helios_ml-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5351 2024-04-15 21:38:28.000000 helios_ml-0.1.1/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-15 22:25:56.431492 helios_ml-0.1.1/data/
+drwxrwxrwx   0        0        0        0 2024-04-15 22:25:56.438004 helios_ml-0.1.1/data/logo/
+-rw-rw-rw-   0        0        0    20058 2024-04-12 23:17:15.000000 helios_ml-0.1.1/data/logo/logo-background.png
+-rw-rw-rw-   0        0        0    14627 2024-04-12 23:17:15.000000 helios_ml-0.1.1/data/logo/logo-transparent.png
+drwxrwxrwx   0        0        0        0 2024-04-15 22:25:56.431492 helios_ml-0.1.1/examples/
+drwxrwxrwx   0        0        0        0 2024-04-15 22:25:56.438004 helios_ml-0.1.1/examples/cifar10/
+-rw-rw-rw-   0        0        0    11404 2024-04-15 20:22:47.000000 helios_ml-0.1.1/examples/cifar10/cifar10.py
+-rw-rw-rw-   0        0        0     2779 2024-04-15 22:19:34.000000 helios_ml-0.1.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-15 22:25:56.439005 helios_ml-0.1.1/requirements/
+-rw-rw-rw-   0        0        0      409 2024-04-15 22:21:21.000000 helios_ml-0.1.1/requirements/ci.txt
+-rw-rw-rw-   0        0        0      300 2024-04-15 22:21:21.000000 helios_ml-0.1.1/requirements/default.txt
+-rw-rw-rw-   0        0        0      440 2024-04-15 22:21:21.000000 helios_ml-0.1.1/requirements/dev.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 22:25:56.469020 helios_ml-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-15 22:25:56.434492 helios_ml-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-15 22:25:56.440006 helios_ml-0.1.1/src/helios/
+-rw-rw-rw-   0        0        0       53 2024-04-12 23:57:34.000000 helios_ml-0.1.1/src/helios/__init__.py
+-rw-rw-rw-   0        0        0      155 2024-04-12 23:59:10.000000 helios_ml-0.1.1/src/helios/_version.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:25:56.442003 helios_ml-0.1.1/src/helios/core/
+-rw-rw-rw-   0        0        0      446 2024-04-12 23:17:15.000000 helios_ml-0.1.1/src/helios/core/__init__.py
+-rw-rw-rw-   0        0        0      254 2024-04-12 23:17:15.000000 helios_ml-0.1.1/src/helios/core/cuda.py
+-rw-rw-rw-   0        0        0     5408 2024-04-12 23:17:15.000000 helios_ml-0.1.1/src/helios/core/distributed.py
+-rw-rw-rw-   0        0        0    17255 2024-04-15 20:21:06.000000 helios_ml-0.1.1/src/helios/core/logging.py
+-rw-rw-rw-   0        0        0     4342 2024-04-15 20:21:39.000000 helios_ml-0.1.1/src/helios/core/rng.py
+-rw-rw-rw-   0        0        0    13539 2024-04-15 20:22:04.000000 helios_ml-0.1.1/src/helios/core/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:25:56.444003 helios_ml-0.1.1/src/helios/data/
+-rw-rw-rw-   0        0        0      530 2024-04-12 23:17:15.000000 helios_ml-0.1.1/src/helios/data/__init__.py
+-rw-rw-rw-   0        0        0    12644 2024-04-15 20:20:56.000000 helios_ml-0.1.1/src/helios/data/datamodule.py
+-rw-rw-rw-   0        0        0     5263 2024-04-12 23:17:15.000000 helios_ml-0.1.1/src/helios/data/functional.py
+-rw-rw-rw-   0        0        0     7733 2024-04-12 23:17:15.000000 helios_ml-0.1.1/src/helios/data/samplers.py
+-rw-rw-rw-   0        0        0     2332 2024-04-12 23:17:15.000000 helios_ml-0.1.1/src/helios/data/transforms.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:25:56.445003 helios_ml-0.1.1/src/helios/losses/
+-rw-rw-rw-   0        0        0      261 2024-04-12 23:17:15.000000 helios_ml-0.1.1/src/helios/losses/__init__.py
+-rw-rw-rw-   0        0        0      545 2024-04-12 23:17:15.000000 helios_ml-0.1.1/src/helios/losses/utils.py
+-rw-rw-rw-   0        0        0     1504 2024-04-12 23:17:15.000000 helios_ml-0.1.1/src/helios/losses/weighted_loss.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:25:56.446003 helios_ml-0.1.1/src/helios/metrics/
+-rw-rw-rw-   0        0        0      488 2024-04-12 23:17:15.000000 helios_ml-0.1.1/src/helios/metrics/__init__.py
+-rw-rw-rw-   0        0        0    13882 2024-04-12 23:17:15.000000 helios_ml-0.1.1/src/helios/metrics/functional.py
+-rw-rw-rw-   0        0        0     7376 2024-04-12 23:17:15.000000 helios_ml-0.1.1/src/helios/metrics/metrics.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:25:56.447003 helios_ml-0.1.1/src/helios/model/
+-rw-rw-rw-   0        0        0      286 2024-04-12 23:17:15.000000 helios_ml-0.1.1/src/helios/model/__init__.py
+-rw-rw-rw-   0        0        0    12625 2024-04-12 23:17:15.000000 helios_ml-0.1.1/src/helios/model/model.py
+-rw-rw-rw-   0        0        0     1465 2024-04-12 23:17:15.000000 helios_ml-0.1.1/src/helios/model/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:25:56.448004 helios_ml-0.1.1/src/helios/nn/
+-rw-rw-rw-   0        0        0      330 2024-04-12 23:17:15.000000 helios_ml-0.1.1/src/helios/nn/__init__.py
+-rw-rw-rw-   0        0        0     1847 2024-04-12 23:17:15.000000 helios_ml-0.1.1/src/helios/nn/swa_utils.py
+-rw-rw-rw-   0        0        0     1750 2024-04-12 23:17:15.000000 helios_ml-0.1.1/src/helios/nn/utils.py
+-rw-rw-rw-   0        0        0     1857 2024-04-12 23:17:15.000000 helios_ml-0.1.1/src/helios/onnx.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:25:56.449004 helios_ml-0.1.1/src/helios/optim/
+-rw-rw-rw-   0        0        0      226 2024-04-12 23:17:15.000000 helios_ml-0.1.1/src/helios/optim/__init__.py
+-rw-rw-rw-   0        0        0      923 2024-04-12 23:17:15.000000 helios_ml-0.1.1/src/helios/optim/utils.py
+-rw-rw-rw-   0        0        0        0 2024-04-12 23:17:15.000000 helios_ml-0.1.1/src/helios/py.typed
+drwxrwxrwx   0        0        0        0 2024-04-15 22:25:56.450003 helios_ml-0.1.1/src/helios/scheduler/
+-rw-rw-rw-   0        0        0      364 2024-04-12 23:17:15.000000 helios_ml-0.1.1/src/helios/scheduler/__init__.py
+-rw-rw-rw-   0        0        0     4896 2024-04-12 23:17:15.000000 helios_ml-0.1.1/src/helios/scheduler/schedulers.py
+-rw-rw-rw-   0        0        0      962 2024-04-12 23:17:15.000000 helios_ml-0.1.1/src/helios/scheduler/utils.py
+-rw-rw-rw-   0        0        0    35395 2024-04-15 20:22:13.000000 helios_ml-0.1.1/src/helios/trainer.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:25:56.467517 helios_ml-0.1.1/src/helios_ml.egg-info/
+-rw-rw-rw-   0        0        0     7527 2024-04-15 22:25:56.000000 helios_ml-0.1.1/src/helios_ml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1885 2024-04-15 22:25:56.000000 helios_ml-0.1.1/src/helios_ml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 22:25:56.000000 helios_ml-0.1.1/src/helios_ml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      436 2024-04-15 22:25:56.000000 helios_ml-0.1.1/src/helios_ml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-15 22:25:56.000000 helios_ml-0.1.1/src/helios_ml.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 22:25:56.464516 helios_ml-0.1.1/test/
+-rw-rw-rw-   0        0        0        0 2024-04-12 23:17:15.000000 helios_ml-0.1.1/test/__init__.py
+-rw-rw-rw-   0        0        0     2425 2024-04-12 23:17:15.000000 helios_ml-0.1.1/test/conftest.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:25:56.466516 helios_ml-0.1.1/test/registry_test/
+-rw-rw-rw-   0        0        0       70 2024-04-12 23:17:15.000000 helios_ml-0.1.1/test/registry_test/__init__.py
+-rw-rw-rw-   0        0        0       49 2024-04-12 23:17:15.000000 helios_ml-0.1.1/test/registry_test/extra.py
+-rw-rw-rw-   0        0        0      102 2024-04-12 23:17:15.000000 helios_ml-0.1.1/test/registry_test/foo.py
+-rw-rw-rw-   0        0        0      139 2024-04-12 23:17:15.000000 helios_ml-0.1.1/test/registry_test/func_registry.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:25:56.467517 helios_ml-0.1.1/test/registry_test/nested/
+-rw-rw-rw-   0        0        0        0 2024-04-12 23:17:15.000000 helios_ml-0.1.1/test/registry_test/nested/__init__.py
+-rw-rw-rw-   0        0        0      103 2024-04-12 23:17:15.000000 helios_ml-0.1.1/test/registry_test/nested/bar.py
+-rw-rw-rw-   0        0        0       63 2024-04-12 23:17:15.000000 helios_ml-0.1.1/test/registry_test/nested/extra.py
+-rw-rw-rw-   0        0        0        0 2024-04-12 23:17:15.000000 helios_ml-0.1.1/test/registry_test/py.typed
+-rw-rw-rw-   0        0        0     4751 2024-04-12 23:17:15.000000 helios_ml-0.1.1/test/test_core.py
+-rw-rw-rw-   0        0        0     7923 2024-04-12 23:17:15.000000 helios_ml-0.1.1/test/test_data.py
+-rw-rw-rw-   0        0        0      730 2024-04-12 23:17:15.000000 helios_ml-0.1.1/test/test_losses.py
+-rw-rw-rw-   0        0        0      574 2024-04-12 23:17:15.000000 helios_ml-0.1.1/test/test_metrics.py
+-rw-rw-rw-   0        0        0     2108 2024-04-12 23:17:15.000000 helios_ml-0.1.1/test/test_model.py
+-rw-rw-rw-   0        0        0     1144 2024-04-12 23:17:15.000000 helios_ml-0.1.1/test/test_nn.py
+-rw-rw-rw-   0        0        0     1000 2024-04-12 23:17:15.000000 helios_ml-0.1.1/test/test_onnx.py
+-rw-rw-rw-   0        0        0      316 2024-04-12 23:17:15.000000 helios_ml-0.1.1/test/test_optim.py
+-rw-rw-rw-   0        0        0      508 2024-04-12 23:17:15.000000 helios_ml-0.1.1/test/test_scheduler.py
+-rw-rw-rw-   0        0        0    11800 2024-04-12 23:17:15.000000 helios_ml-0.1.1/test/test_trainer.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:25:56.467517 helios_ml-0.1.1/tools/
+-rw-rw-rw-   0        0        0     1642 2024-04-12 23:17:15.000000 helios_ml-0.1.1/tools/generate_requirements.py
```

### Comparing `helios-ml-0.1.0/.github/workflows/publish.yml` & `helios_ml-0.1.1/.github/workflows/publish.yml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 permissions:
   contents: read
 
 jobs:
   publish:
     runs-on: ubuntu-latest
     environment:
-      name: testpypi
+      name: pypi
       url: https://pypi.org/project/helios-ml
     permissions:
       id-token: write
     steps:
       - name: Checkout
         uses: actions/checkout@v3
```

### Comparing `helios-ml-0.1.0/.github/workflows/tests.yml` & `helios_ml-0.1.1/.github/workflows/tests.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 name: "Tests"
 
 on:
   push:
     branches: [ master ]
     paths-ignore:
       - 'README.md'
+      - 'README.rst'
       - '.pre-commit-config.yaml'
       - 'data/**'
       - "LICENSE"
   pull_request:
     branches: [ master ]
     paths-ignore:
       - 'README.md'
```

### Comparing `helios-ml-0.1.0/.pre-commit-config.yaml` & `helios_ml-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `helios-ml-0.1.0/LICENSE` & `helios_ml-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `helios-ml-0.1.0/data/logo/logo-background.png` & `helios_ml-0.1.1/data/logo/logo-background.png`

 * *Files identical despite different names*

### Comparing `helios-ml-0.1.0/data/logo/logo-transparent.png` & `helios_ml-0.1.1/data/logo/logo-transparent.png`

 * *Files identical despite different names*

### Comparing `helios-ml-0.1.0/examples/cifar10/cifar10.py` & `helios_ml-0.1.1/examples/cifar10/cifar10.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     def prepare_data(self) -> None:
         """Download all necessary data."""
         torchvision.datasets.CIFAR10(root=self._root, train=True, download=True)
         torchvision.datasets.CIFAR10(root=self._root, train=False, download=True)
 
     def setup(self) -> None:
         """Create the datasets."""
-        # Use the ToTensor transform from Pyro to automate the conversion from images to
+        # Use the ToTensor transform from Helios to automate the conversion from images to
         # tensors.
         transforms = T.Compose(
             [hld.transforms.ToTensor(), T.Normalize((0.5, 0.5, 0.5), (0.5, 0.5, 0.5))]
         )
         params = hld.DataLoaderParams()
         params.batch_size = 4
         params.shuffle = True
@@ -116,16 +116,16 @@
     def setup(self, fast_init: bool = False) -> None:
         """Create the network, loss, and optimizer."""
         # Note that when we create the network and loss function, we immediately move them
         # to the current device, which has been set by the trainer.
         self._net = Net().to(self.device)
         self._criterion = nn.CrossEntropyLoss().to(self.device)
 
-        # Note that SGD is shipped as part of the default optimizers from Pyro, so we can
-        # directly request it from create_optimizer instead of building it ourselves.
+        # Note that SGD is shipped as part of the default optimizers from Helios, so we
+        # can directly request it from create_optimizer instead of building it ourselves.
         self._optimizer = hlo.create_optimizer(
             "SGD", self._net.parameters(), lr=0.001, momentum=0.9
         )
 
     def load_state_dict(
         self, state_dict: dict[str, typing.Any], fast_init: bool = False
     ) -> None:
```

### Comparing `helios-ml-0.1.0/pyproject.toml` & `helios_ml-0.1.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,41 @@
 [build-system]
 requires = ["setuptools>=64", "setuptools-scm>=8"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "helios-ml"
-authors = [{name = "Mauricio A. Rovira Galvez"}]
-description = "A Torch-based package for training AI networks"
+authors = [{name = "Mauricio A. Rovira Galvez", email = "maroviragalvez@outlook.com"}]
+readme = "README.rst"
+license = {text = "BSD-3-Clause"}
+description = "A light-weight system for training AI networks using PyTorch"
+classifiers = [
+    "Intended Audience :: Science/Research",
+    "Intended Audience :: Developers",
+    "Topic :: Software Development",
+    "Topic :: Scientific/Engineering :: Artificial Intelligence",
+    "License :: OSI Approved :: BSD License",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+]
 requires-python = ">= 3.11"
 dependencies = [
     "tqdm>=4.66.2",
     "opencv-python>=4.9.0.80",
     "protobuf>=3.19.6, !=4.24.0, <5.0.0",
     "tensorboard>=2.16.2",
     "torch>=2.2.1",
     "torchvision>=0.17.1",
     "onnx>=1.16.0",
     "onnxruntime>=1.17.1",
     "matplotlib>=3.8.4"
 ]
 
-dynamic = ["version", "readme"]
+dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
     "mypy>=1.8.0",
     "ruff>=0.3.4",
     "pytest>=8.1.1",
     "pre-commit>=3.6.2",
@@ -38,29 +50,28 @@
     "ruff>=0.3.4",
     "pytest>=8.1.1",
     "types-Pillow>=10.2.0.20240311",
     "types-tqdm>=4.66.0.20240106",
     "build>=1.2.1"
 ]
 
+[project.urls]
+homepage = "https://github.com/marovira/helios-ml"
+source = "https://github.com/marovira/helios-ml"
+issues = "https://github.com/marovira/helios-ml/issues"
+"release notes" = "https://github.com/marovira/helios-ml/releases"
+
 [tool.setuptools_scm]
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
-[tool.setuptools.dynamic]
-readme = {file = ["README.md"]}
-
 [tool.setuptools.package-data]
 pkgname = ["py.typed"]
 
-[project.urls]
-Homepage = "https://github.com/marovira/pyro-ml"
-Issues = "https://github.com/marovira/pyro-ml/issues"
-
 [tool.mypy]
 warn_unused_configs = true
 
 [[tool.mypy.overrides]]
 module = "torchvision.*"
 ignore_missing_imports = true
```

### Comparing `helios-ml-0.1.0/src/helios/core/distributed.py` & `helios_ml-0.1.1/src/helios/core/distributed.py`

 * *Files identical despite different names*

### Comparing `helios-ml-0.1.0/src/helios/core/logging.py` & `helios_ml-0.1.1/src/helios/core/logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
     Args:
         log_file (pathlib.Path): path to the log file.
     """
 
     def __init__(self: "RootLogger"):
         """Create the root logger with stream output as default."""
-        self._logger = logging.getLogger("pyro")
+        self._logger = logging.getLogger("helios")
         self._rank = get_global_rank()
         self._format_str = "[%(asctime)s] [%(levelname)s]: %(message)s"
         self._log_file: pathlib.Path | None = None
 
         stream_handler = logging.StreamHandler()
         stream_handler.setFormatter(logging.Formatter(self._format_str))
         stream_handler.setLevel(logging.WARNING)
```

### Comparing `helios-ml-0.1.0/src/helios/core/rng.py` & `helios_ml-0.1.1/src/helios/core/rng.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import torch
 from numpy import random as npr
 
 _DEFAULT_RNG_SEED = 6691
 
 
 def get_default_seed() -> int:
-    """Return the default Pyro seed."""
+    """Return the default seed."""
     return _DEFAULT_RNG_SEED
 
 
 class DefaultNumpyRNG:
     """
     Default RNG from Numpy.
 
@@ -89,17 +89,17 @@
     return _get_safe_default_rng()
 
 
 def seed_rngs(seed: int | None = None, skip_torch: bool = False) -> None:
     """
     Seed the default RNGs with the given seed.
 
-    If no seed is given, then the default seed from Pyro will be used. The RNGs that will
-    be seeded are: PyTorch (+ CUDA if available), stdlib random, and the default Numpy
-    generator.
+    If no seed is given, then the default seed from Helios will be used. The RNGs that
+    will be seeded are: PyTorch (+ CUDA if available), stdlib random, and the default
+    Numpy generator.
     The skip_torch flag is intended to be used when seeding worker processes for
     dataloaders. In those cases, the RNGs for PyTorch have already been seeded, so we
     shouldn't be re-seeding them.
 
     Args:
         seed (int | None): optional value to seed the random generators with.
         skip_torch (bool): if True, torch RNGs won't be seeded.
```

### Comparing `helios-ml-0.1.0/src/helios/core/utils.py` & `helios_ml-0.1.1/src/helios/core/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,39 +14,43 @@
 
 T = typing.TypeVar("T")
 T_Any = typing.TypeVar("T_Any", bound=typing.Any)
 
 
 def get_env_info_str() -> str:
     """
-    Return a string with the pyro header and the environment information.
+    Return a string with the Helios header and the environment information.
 
     Returns:
         str: the message string.
     """
     msg = r"""
-#===========================================#
-  _____   __     __  _____     ____
- |  __ \  \ \   / / |  __ \   / __ \
- | |__) |  \ \_/ /  | |__) | | |  | |
- |  ___/    \   /   |  _  /  | |  | |
- | |         | |    | | \ \  | |__| |
- |_|         |_|    |_|  \_\  \____/
+#===========================================================================#
+          _______  _       _________ _______  _______
+|\     /|(  ____ \( \      \__   __/(  ___  )(  ____ \
+| )   ( || (    \/| (         ) (   | (   ) || (    \/
+| (___) || (__    | |         | |   | |   | || (_____
+|  ___  ||  __)   | |         | |   | |   | |(_____  )
+| (   ) || (      | |         | |   | |   | |      ) |
+| )   ( || (____/\| (____/\___) (___| (___) |/\____) |
+|/     \|(_______/(_______/\_______/(_______)\_______)
     """
     msg += (
         "\nEnvironment info: "
-        f"\n\tPyro: {__version__}"
+        f"\n\tHelios: {__version__}"
         f"\n\tPyTorch: {torch.__version__}"
         f"\n\tTorchVision: {torchvision.__version__}"
         f"\n\tOS: {platform.platform()}"
         f"\n\tPython: {sys.version_info[0]}.{sys.version_info[1]}.{sys.version_info[3]}"
     )
     if torch.cuda.is_available():
         msg += f"\n\tCUDA version: {torch.version.cuda}"
-    msg += "\n#===========================================#\n\n"
+    msg += "\n"
+    msg += "#===========================================================================#"
+    msg += "\n\n"
     return msg
 
 
 def get_from_optional(opt_var: T | None, raise_on_empty: bool = False) -> T:
     """
     Ensure the given variable is not None and return it.
 
@@ -360,17 +364,17 @@
             |---some_funcs.py <- Doesn't register anything.
             |---sub_package/
             |   |---__init__.py
             |   |---another_type.py <- Registers
             |   |---another_func.py <- Doesn't register.
 
         We can then do the following inside `main.py`:
-            import pyro.core as pyc
+            import helios.core as hlc
             ...
-            pyc.update_all_registries(Path.cwd() / "my_package", recurse=True)
+            hlc.update_all_registries(Path.cwd() / "my_package", recurse=True)
 
         The function will recursively walk through `my_package` and import the following:
             * my_package.some_class
             * my_package.sub_package.another_type
         After the function returns, the corresponding registries will have been populated
         with the types and they can be used elsewhere in the code.
```

### Comparing `helios-ml-0.1.0/src/helios/data/__init__.py` & `helios_ml-0.1.1/src/helios/data/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-ml-0.1.0/src/helios/data/datamodule.py` & `helios_ml-0.1.1/src/helios/data/datamodule.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,17 +232,17 @@
     Base class that groups together the creation of the main training datasets.
 
     The use of this class is to standardize the way datasets and their respective
     dataloaders are created, thereby allowing consistent settings across models.
     Ex:
         ```py
         from torchvision.datasets import CIFAR10
-        from pyro import data
+        from helios import data
 
-        class MyDataModule(data.PyroDataModule):
+        class MyDataModule(data.DataModule):
             def prepare_data(self) -> None:
                 # Use this function to prepare the data for your datasets. This will be
                 # called before the distributed processes are created (if using) so you
                 # should not set any state here.
                 CIFAR10(download=True) # download the dataset only.
 
             def setup(self) -> None:
```

### Comparing `helios-ml-0.1.0/src/helios/data/functional.py` & `helios_ml-0.1.1/src/helios/data/functional.py`

 * *Files identical despite different names*

### Comparing `helios-ml-0.1.0/src/helios/data/samplers.py` & `helios_ml-0.1.1/src/helios/data/samplers.py`

 * *Files identical despite different names*

### Comparing `helios-ml-0.1.0/src/helios/data/transforms.py` & `helios_ml-0.1.1/src/helios/data/transforms.py`

 * *Files identical despite different names*

### Comparing `helios-ml-0.1.0/src/helios/losses/utils.py` & `helios_ml-0.1.1/src/helios/losses/utils.py`

 * *Files identical despite different names*

### Comparing `helios-ml-0.1.0/src/helios/losses/weighted_loss.py` & `helios_ml-0.1.1/src/helios/losses/weighted_loss.py`

 * *Files identical despite different names*

### Comparing `helios-ml-0.1.0/src/helios/metrics/functional.py` & `helios_ml-0.1.1/src/helios/metrics/functional.py`

 * *Files identical despite different names*

### Comparing `helios-ml-0.1.0/src/helios/metrics/metrics.py` & `helios_ml-0.1.1/src/helios/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `helios-ml-0.1.0/src/helios/model/model.py` & `helios_ml-0.1.1/src/helios/model/model.py`

 * *Files identical despite different names*

### Comparing `helios-ml-0.1.0/src/helios/model/utils.py` & `helios_ml-0.1.1/src/helios/model/utils.py`

 * *Files identical despite different names*

### Comparing `helios-ml-0.1.0/src/helios/nn/swa_utils.py` & `helios_ml-0.1.1/src/helios/nn/swa_utils.py`

 * *Files identical despite different names*

### Comparing `helios-ml-0.1.0/src/helios/nn/utils.py` & `helios_ml-0.1.1/src/helios/nn/utils.py`

 * *Files identical despite different names*

### Comparing `helios-ml-0.1.0/src/helios/onnx.py` & `helios_ml-0.1.1/src/helios/onnx.py`

 * *Files identical despite different names*

### Comparing `helios-ml-0.1.0/src/helios/optim/utils.py` & `helios_ml-0.1.1/src/helios/optim/utils.py`

 * *Files identical despite different names*

### Comparing `helios-ml-0.1.0/src/helios/scheduler/schedulers.py` & `helios_ml-0.1.1/src/helios/scheduler/schedulers.py`

 * *Files identical despite different names*

### Comparing `helios-ml-0.1.0/src/helios/scheduler/utils.py` & `helios_ml-0.1.1/src/helios/scheduler/utils.py`

 * *Files identical despite different names*

### Comparing `helios-ml-0.1.0/src/helios/trainer.py` & `helios_ml-0.1.1/src/helios/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -539,15 +539,15 @@
                 self._log_path.mkdir(parents=True, exist_ok=True)
             if self._run_path is not None:
                 self._run_path.mkdir(parents=True, exist_ok=True)
 
     def _print_header(
         self, chkpt_path: pathlib.Path | None, for_training: bool = True
     ) -> None:
-        """Print the Pyro header with system info to the logs."""
+        """Print the Helios header with system info to the logs."""
         root_logger = logging.get_root_logger()
 
         print(core.get_env_info_str())
 
         if for_training:
             if chkpt_path is not None:
                 msg = f"Resuming training from checkpoint {str(chkpt_path)}"
```

### Comparing `helios-ml-0.1.0/src/helios_ml.egg-info/SOURCES.txt` & `helios_ml-0.1.1/src/helios_ml.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 .gitignore
 .pre-commit-config.yaml
 LICENSE
-README.md
+README.rst
 pyproject.toml
 .github/workflows/publish.yml
 .github/workflows/tests.yml
 data/logo/logo-background.png
 data/logo/logo-transparent.png
 examples/cifar10/cifar10.py
 requirements/ci.txt
```

### Comparing `helios-ml-0.1.0/test/conftest.py` & `helios_ml-0.1.1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `helios-ml-0.1.0/test/test_core.py` & `helios_ml-0.1.1/test/test_core.py`

 * *Files identical despite different names*

### Comparing `helios-ml-0.1.0/test/test_data.py` & `helios_ml-0.1.1/test/test_data.py`

 * *Files identical despite different names*

### Comparing `helios-ml-0.1.0/test/test_losses.py` & `helios_ml-0.1.1/test/test_losses.py`

 * *Files identical despite different names*

### Comparing `helios-ml-0.1.0/test/test_metrics.py` & `helios_ml-0.1.1/test/test_metrics.py`

 * *Files identical despite different names*

### Comparing `helios-ml-0.1.0/test/test_model.py` & `helios_ml-0.1.1/test/test_model.py`

 * *Files identical despite different names*

### Comparing `helios-ml-0.1.0/test/test_nn.py` & `helios_ml-0.1.1/test/test_nn.py`

 * *Files identical despite different names*

### Comparing `helios-ml-0.1.0/test/test_onnx.py` & `helios_ml-0.1.1/test/test_onnx.py`

 * *Files identical despite different names*

### Comparing `helios-ml-0.1.0/test/test_trainer.py` & `helios_ml-0.1.1/test/test_trainer.py`

 * *Files identical despite different names*

### Comparing `helios-ml-0.1.0/tools/generate_requirements.py` & `helios_ml-0.1.1/tools/generate_requirements.py`

 * *Files identical despite different names*

