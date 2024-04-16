# Comparing `tmp/nncore-0.4.1.tar.gz` & `tmp/nncore-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nncore-0.4.1.tar", last modified: Sun Apr 14 14:43:50 2024, max compression
+gzip compressed data, was "nncore-0.4.2.tar", last modified: Tue Apr 16 13:20:13 2024, max compression
```

## Comparing `nncore-0.4.1.tar` & `nncore-0.4.2.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.131383 nncore-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-14 14:43:42.000000 nncore-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-04-14 14:43:50.131383 nncore-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-04-14 14:43:42.000000 nncore-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.115383 nncore-0.4.1/nncore/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.115383 nncore-0.4.1/nncore/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/dataset/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/dataset/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/dataset/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.115383 nncore-0.4.1/nncore/engine/
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/engine/buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/engine/builder.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9026 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/engine/comm.py
--rw-r--r--   0 runner    (1001) docker     (127)    21729 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/engine/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.119383 nncore-0.4.1/nncore/engine/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/engine/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/engine/hooks/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/engine/hooks/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/engine/hooks/closure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/engine/hooks/eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/engine/hooks/lr_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/engine/hooks/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/engine/hooks/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/engine/hooks/precise_bn.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/engine/hooks/sampler_seed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/engine/hooks/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11191 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/engine/hooks/writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8474 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/engine/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.119383 nncore-0.4.1/nncore/image/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/image/colorspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/image/geometric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/image/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/image/normalize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.119383 nncore-0.4.1/nncore/io/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.119383 nncore-0.4.1/nncore/io/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/io/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/io/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/io/handlers/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/io/handlers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/io/handlers/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/io/handlers/pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/io/handlers/txt.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/io/handlers/xml.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/io/handlers/yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/io/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.123383 nncore-0.4.1/nncore/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.123383 nncore-0.4.1/nncore/nn/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/blocks/activation.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/blocks/conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     8154 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/blocks/msg_pass.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/blocks/norm.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/blocks/scale.py
--rw-r--r--   0 runner    (1001) docker     (127)    30450 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/blocks/transformer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4505 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.123383 nncore-0.4.1/nncore/nn/bundle/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/bundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/bundle/bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.123383 nncore-0.4.1/nncore/nn/losses/
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/losses/bce.py
--rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/losses/contrastive.py
--rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/losses/focal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/losses/ghm.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6311 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/losses/lasso.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/losses/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.123383 nncore-0.4.1/nncore/nn/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/modules/conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/modules/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/modules/msg_pass.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9821 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/nn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.123383 nncore-0.4.1/nncore/ops/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/ops/bbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/ops/matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/ops/temporal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.127383 nncore-0.4.1/nncore/optim/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/optim/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/optim/lamb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.127383 nncore-0.4.1/nncore/parallel/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/parallel/collate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/parallel/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/parallel/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.127383 nncore-0.4.1/nncore/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/utils/binder.py
--rw-r--r--   0 runner    (1001) docker     (127)    14654 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/utils/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     9214 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/utils/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.127383 nncore-0.4.1/nncore/video/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-04-14 14:43:42.000000 nncore-0.4.1/nncore/video/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.131383 nncore-0.4.1/nncore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-04-14 14:43:50.000000 nncore-0.4.1/nncore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-14 14:43:50.000000 nncore-0.4.1/nncore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 14:43:50.000000 nncore-0.4.1/nncore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-14 14:43:50.000000 nncore-0.4.1/nncore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-14 14:43:50.000000 nncore-0.4.1/nncore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-14 14:43:50.131383 nncore-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-14 14:43:42.000000 nncore-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:43:50.131383 nncore-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-14 14:43:42.000000 nncore-0.4.1/tests/test_binder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-14 14:43:42.000000 nncore-0.4.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-14 14:43:42.000000 nncore-0.4.1/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-14 14:43:42.000000 nncore-0.4.1/tests/test_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-14 14:43:42.000000 nncore-0.4.1/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-14 14:43:42.000000 nncore-0.4.1/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-14 14:43:42.000000 nncore-0.4.1/tests/test_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-14 14:43:42.000000 nncore-0.4.1/tests/test_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:20:13.716007 nncore-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-16 13:20:03.000000 nncore-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-04-16 13:20:13.716007 nncore-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-04-16 13:20:03.000000 nncore-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:20:13.696007 nncore-0.4.2/nncore/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:20:13.700007 nncore-0.4.2/nncore/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/dataset/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/dataset/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/dataset/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:20:13.700007 nncore-0.4.2/nncore/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/engine/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/engine/builder.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9026 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/engine/comm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22210 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/engine/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:20:13.704007 nncore-0.4.2/nncore/engine/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/engine/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/engine/hooks/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/engine/hooks/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/engine/hooks/closure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/engine/hooks/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/engine/hooks/lr_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/engine/hooks/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/engine/hooks/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/engine/hooks/precise_bn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/engine/hooks/sampler_seed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/engine/hooks/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11191 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/engine/hooks/writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8474 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/engine/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:20:13.704007 nncore-0.4.2/nncore/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/image/colorspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/image/geometric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/image/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/image/normalize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:20:13.704007 nncore-0.4.2/nncore/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:20:13.704007 nncore-0.4.2/nncore/io/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/io/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/io/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/io/handlers/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/io/handlers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/io/handlers/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/io/handlers/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/io/handlers/txt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/io/handlers/xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/io/handlers/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/io/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:20:13.708007 nncore-0.4.2/nncore/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:20:13.708007 nncore-0.4.2/nncore/nn/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/nn/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/nn/blocks/activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/nn/blocks/conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8154 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/nn/blocks/msg_pass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/nn/blocks/norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/nn/blocks/scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30450 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/nn/blocks/transformer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4505 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/nn/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:20:13.708007 nncore-0.4.2/nncore/nn/bundle/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/nn/bundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/nn/bundle/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/nn/init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:20:13.708007 nncore-0.4.2/nncore/nn/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/nn/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/nn/losses/bce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6824 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/nn/losses/contrastive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/nn/losses/focal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/nn/losses/ghm.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6311 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/nn/losses/lasso.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/nn/losses/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:20:13.712007 nncore-0.4.2/nncore/nn/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/nn/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/nn/modules/conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/nn/modules/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/nn/modules/msg_pass.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9866 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/nn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:20:13.712007 nncore-0.4.2/nncore/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/ops/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/ops/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/ops/temporal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:20:13.712007 nncore-0.4.2/nncore/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/optim/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/optim/lamb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:20:13.712007 nncore-0.4.2/nncore/parallel/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/parallel/collate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/parallel/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/parallel/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:20:13.716007 nncore-0.4.2/nncore/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/utils/binder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14654 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/utils/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9214 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/utils/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:20:13.716007 nncore-0.4.2/nncore/video/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-04-16 13:20:03.000000 nncore-0.4.2/nncore/video/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:20:13.716007 nncore-0.4.2/nncore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-04-16 13:20:13.000000 nncore-0.4.2/nncore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-16 13:20:13.000000 nncore-0.4.2/nncore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 13:20:13.000000 nncore-0.4.2/nncore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-16 13:20:13.000000 nncore-0.4.2/nncore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 13:20:13.000000 nncore-0.4.2/nncore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-16 13:20:13.716007 nncore-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-16 13:20:03.000000 nncore-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:20:13.716007 nncore-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-16 13:20:03.000000 nncore-0.4.2/tests/test_binder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-16 13:20:03.000000 nncore-0.4.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-16 13:20:03.000000 nncore-0.4.2/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-16 13:20:03.000000 nncore-0.4.2/tests/test_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-16 13:20:03.000000 nncore-0.4.2/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-16 13:20:03.000000 nncore-0.4.2/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-16 13:20:03.000000 nncore-0.4.2/tests/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-16 13:20:03.000000 nncore-0.4.2/tests/test_registry.py
```

### Comparing `nncore-0.4.1/LICENSE` & `nncore-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/PKG-INFO` & `nncore-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nncore
-Version: 0.4.1
+Version: 0.4.2
 Summary: A lightweight machine learning toolkit for researchers.
 Home-page: https://github.com/yeliudev/nncore
 Author: Ye Liu
 Author-email: yeliudev@outlook.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nncore Version: 0.4.1 Summary: A lightweight
+Metadata-Version: 2.1 Name: nncore Version: 0.4.2 Summary: A lightweight
 machine learning toolkit for researchers. Home-page: https://github.com/
 yeliudev/nncore Author: Ye Liu Author-email: yeliudev@outlook.com License: MIT
 Classifier: Development Status :: 4 - Beta Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
```

### Comparing `nncore-0.4.1/README.md` & `nncore-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/dataset/builder.py` & `nncore-0.4.2/nncore/dataset/builder.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/dataset/wrapper.py` & `nncore-0.4.2/nncore/dataset/wrapper.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/engine/__init__.py` & `nncore-0.4.2/nncore/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/engine/buffer.py` & `nncore-0.4.2/nncore/engine/buffer.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/engine/builder.py` & `nncore-0.4.2/nncore/engine/builder.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/engine/comm.py` & `nncore-0.4.2/nncore/engine/comm.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/engine/engine.py` & `nncore-0.4.2/nncore/engine/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -462,19 +462,19 @@
         self._call_hook('before_val_epoch')
 
         for data in nncore.ProgressBar(self.data_loader):
             self.val_iter(data)
 
         self._call_hook('after_val_epoch')
 
-    def test_epoch(self):
+    def test_epoch(self, split='test'):
         self._mode = 'test'
         self.model.eval()
         self.buffer.pop('_out', None)
-        self.data_loader = self.data_loaders[self._mode]
+        self.data_loader = self.data_loaders[split]
 
         if callable(getattr(self.data_loader.dataset, 'set_state', None)):
             self.data_loader.dataset.set_state(self._mode)
 
         for data in nncore.ProgressBar(self.data_loader):
             self.test_iter(data)
 
@@ -508,18 +508,14 @@
                 self.logger.info('Validating...')
                 self.val_epoch()
 
         self._call_hook('after_stage')
         self._stage += 1
 
     def evaluate(self):
-        """
-        Perform evaluation. This methods is expected to be called after
-        validation or testing.
-        """
         blob = self.buffer.pop('_out')
         blob = gather(blob)
 
         if is_main_process():
             blob = nncore.interleave(blob)[:len(self.data_loader.dataset)]
 
             cfg = self.cur_stage.get('validation')
@@ -534,36 +530,54 @@
                 blob, logger=self.logger, **cfg)
         else:
             output = dict()
 
         sync()
         return output
 
-    def launch(self, eval=False, **kwargs):
+    def eval_mode(self, mode):
+        if isinstance(mode, bool):
+            splits = ('test', )
+        elif mode in ('val', 'test'):
+            splits = (mode, )
+        elif mode == 'both':
+            splits = ('val', 'test')
+        else:
+            raise ValueError("eval mode '{}' not found".format(mode))
+
+        output = dict()
+        for split in splits:
+            self.logger.info('Inferencing on {} split...'.format(split))
+            self.test_epoch(split=split)
+            out = self.evaluate()
+            if out:
+                self.logger.info(
+                    'Evaluation results on {} split: '.format(split) +
+                    ', '.join(['{}: {}'.format(k, v) for k, v in out.items()]))
+            output[split] = out
+            self.reset_states()
+
+        return output
+
+    def launch(self, eval=None, **kwargs):
         """
         Launch the engine.
 
         Args:
-            eval (bool, optional): Whether to run evaluation only. Default:
-                ``False``.
+            eval (str | bool | None, optional): Run evaluation only and
+                specify the split to use. Default: ``None``.
         """
         self._kwargs = kwargs
 
         if eval:
-            self.logger.info('Evaluating...')
-            self.test_epoch()
-            output = self.evaluate()
-            self.logger.info(
-                'Evaluation results: ' +
-                ', '.join(['{}: {}'.format(k, v) for k, v in output.items()]))
-            return output
+            return self.eval_mode(eval)
 
         self.logger.info('Distributed: {}, AMP: {}, Debug: {}'.format(
-            f'{get_world_size()} processes' if is_distributed() else False,
-            self.get_amp_type(), self.debug))
+            '{} processes'.format(get_world_size())
+            if is_distributed() else False, self.get_amp_type(), self.debug))
         self.logger.info('Launch engine, host: {}, work_dir: {}'.format(
             nncore.get_host_info(), self.work_dir))
 
         self._call_hook('before_launch')
 
         while self._stage < self._max_stages:
             self.run_stage()
```

### Comparing `nncore-0.4.1/nncore/engine/hooks/__init__.py` & `nncore-0.4.2/nncore/engine/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/engine/hooks/base.py` & `nncore-0.4.2/nncore/engine/hooks/base.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/engine/hooks/checkpoint.py` & `nncore-0.4.2/nncore/engine/hooks/checkpoint.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/engine/hooks/closure.py` & `nncore-0.4.2/nncore/engine/hooks/closure.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/engine/hooks/eval.py` & `nncore-0.4.2/nncore/engine/hooks/eval.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/engine/hooks/lr_updater.py` & `nncore-0.4.2/nncore/engine/hooks/lr_updater.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/engine/hooks/memory.py` & `nncore-0.4.2/nncore/engine/hooks/memory.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/engine/hooks/optimizer.py` & `nncore-0.4.2/nncore/engine/hooks/optimizer.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/engine/hooks/precise_bn.py` & `nncore-0.4.2/nncore/engine/hooks/precise_bn.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/engine/hooks/timer.py` & `nncore-0.4.2/nncore/engine/hooks/timer.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/engine/hooks/writer.py` & `nncore-0.4.2/nncore/engine/hooks/writer.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/engine/utils.py` & `nncore-0.4.2/nncore/engine/utils.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/image/__init__.py` & `nncore-0.4.2/nncore/image/__init__.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/image/colorspace.py` & `nncore-0.4.2/nncore/image/colorspace.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/image/geometric.py` & `nncore-0.4.2/nncore/image/geometric.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/image/io.py` & `nncore-0.4.2/nncore/image/io.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/image/normalize.py` & `nncore-0.4.2/nncore/image/normalize.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/io/handlers/base.py` & `nncore-0.4.2/nncore/io/handlers/base.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/io/handlers/hdf5.py` & `nncore-0.4.2/nncore/io/handlers/hdf5.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/io/handlers/json.py` & `nncore-0.4.2/nncore/io/handlers/json.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/io/handlers/numpy.py` & `nncore-0.4.2/nncore/io/handlers/numpy.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/io/handlers/pickle.py` & `nncore-0.4.2/nncore/io/handlers/pickle.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/io/handlers/txt.py` & `nncore-0.4.2/nncore/io/handlers/txt.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/io/handlers/xml.py` & `nncore-0.4.2/nncore/io/handlers/xml.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/io/handlers/yaml.py` & `nncore-0.4.2/nncore/io/handlers/yaml.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/io/io.py` & `nncore-0.4.2/nncore/io/io.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/nn/__init__.py` & `nncore-0.4.2/nncore/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/nn/blocks/__init__.py` & `nncore-0.4.2/nncore/nn/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/nn/blocks/activation.py` & `nncore-0.4.2/nncore/nn/blocks/activation.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/nn/blocks/conv.py` & `nncore-0.4.2/nncore/nn/blocks/conv.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/nn/blocks/msg_pass.py` & `nncore-0.4.2/nncore/nn/blocks/msg_pass.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/nn/blocks/norm.py` & `nncore-0.4.2/nncore/nn/blocks/norm.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/nn/blocks/scale.py` & `nncore-0.4.2/nncore/nn/blocks/scale.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/nn/blocks/transformer.py` & `nncore-0.4.2/nncore/nn/blocks/transformer.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/nn/builder.py` & `nncore-0.4.2/nncore/nn/builder.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/nn/bundle/bundle.py` & `nncore-0.4.2/nncore/nn/bundle/bundle.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/nn/init.py` & `nncore-0.4.2/nncore/nn/init.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/nn/losses/__init__.py` & `nncore-0.4.2/nncore/nn/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/nn/losses/bce.py` & `nncore-0.4.2/nncore/nn/losses/bce.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/nn/losses/contrastive.py` & `nncore-0.4.2/nncore/nn/losses/contrastive.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,31 +4,29 @@
 
 import torch
 import torch.distributed as dist
 import torch.nn as nn
 import torch.nn.functional as F
 
 import nncore
-from nncore.engine import comm
 from nncore.ops import cosine_similarity
 from ..builder import LOSSES
 from ..bundle import Parameter
 from .utils import weighted_loss
 
 
 class _AllGather(torch.autograd.Function):
 
     @staticmethod
     def forward(ctx, tensor, group=None):
-        rank, world_size = comm.get_dist_info()
-
         ctx.size = tensor.size(-2)
-        ctx.rank = rank
+        ctx.rank = dist.get_rank(group=group)
         ctx.group = group
 
+        world_size = dist.get_world_size(group=group)
         gathered = [torch.zeros_like(tensor) for _ in range(world_size)]
         dist.all_gather(gathered, tensor, group=group)
 
         gathered = torch.cat(gathered, dim=-2)
         return gathered
 
     @staticmethod
@@ -75,16 +73,16 @@
         scale = a.new_tensor([math.log(1 / temperature)])
 
     scale = scale.exp().clamp(max=max_scale)
 
     n = a.size(-2)
     t = torch.arange(n, device=a.device)
 
-    if dist and comm.is_distributed():
-        rank = comm.get_rank(group=group)
+    if dist and dist.is_initialized():
+        rank = dist.get_rank(group=group)
 
         s, e = n * rank, n * (rank + 1)
         t += s
 
         a = _AllGather.apply(a)
         b = _AllGather.apply(b)
```

### Comparing `nncore-0.4.1/nncore/nn/losses/focal.py` & `nncore-0.4.2/nncore/nn/losses/focal.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/nn/losses/ghm.py` & `nncore-0.4.2/nncore/nn/losses/ghm.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/nn/losses/lasso.py` & `nncore-0.4.2/nncore/nn/losses/lasso.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/nn/losses/utils.py` & `nncore-0.4.2/nncore/nn/losses/utils.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/nn/modules/conv.py` & `nncore-0.4.2/nncore/nn/modules/conv.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/nn/modules/linear.py` & `nncore-0.4.2/nncore/nn/modules/linear.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/nn/modules/msg_pass.py` & `nncore-0.4.2/nncore/nn/modules/msg_pass.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/nn/utils.py` & `nncore-0.4.2/nncore/nn/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,35 +157,35 @@
         bn.running_mean = bn_rm[i]
         bn.running_var = bn_rv[i]
         bn.momentum = bn_mo[i]
 
 
 def publish_model(checkpoint,
                   out='model.pth',
-                  keys_to_keep=['state_dict', 'meta'],
+                  keys_to_keep=['state_dict'],
                   device='cpu',
                   meta=None,
                   hash_type='sha256',
                   hash_len=8):
     """
     Publish a model by removing needless data in the checkpoint, moving the
     weights to the specified device, and hashing the output model file.
 
     Args:
         checkpoint (dict | str): The checkpoint or path to the checkpoint.
         out (str, optional): Path to the output checkpoint file. Default:
             ``'model.pth'``.
         keys_to_keep (list[str], optional): The list of keys to be kept from
-            the checkpoint. Default: ``['state_dict', 'meta']``.
+            the checkpoint. Default: ``['state_dict']``.
         device (:obj:`torch.device` | str): The destination device. Default:
             ``'cpu'``.
         meta (dict | None, optional): The meta data to be saved. Note that the
             key ``nncore_version`` and ``create_time`` are reserved by the
             method. Default: ``None``.
-        hash_type (str, optional): Type of the hash algorithm. Currently
+        hash_type (str | None, optional): Type of the hash algorithm. Currently
             supported algorithms include ``'md5'``, ``'sha1'``, ``'sha224'``,
             ``'sha256'``, ``'sha384'``, ``'sha512'``, ``'blake2b'``,
             ``'blake2s'``, ``'sha3_224'``, ``'sha3_256'``, ``'sha3_384'``,
             ``'sha3_512'``, ``'shake_128'``, and ``'shake_256'``. Default:
             ``'sha256'``.
         hash_len (int, optional): Length of the hash value. Default: ``8``.
     """
@@ -204,21 +204,22 @@
         create_time=nncore.get_time_str(),
         **meta or dict())
     model['meta'] = _meta
 
     model = move_to_device(model, device=device)
     torch.save(model, out)
 
-    with open(out, 'rb') as f:
-        hasher = hashlib.new(hash_type, data=f.read())
-        hash_value = hasher.hexdigest()[:hash_len]
-
-    name, ext = nncore.split_ext(out)
-    hashed = '{}-{}.{}'.format(name, hash_value, ext).rstrip('.')
-    nncore.rename(out, hashed)
+    if hash_type is not None:
+        with open(out, 'rb') as f:
+            hasher = hashlib.new(hash_type, data=f.read())
+            hash_value = hasher.hexdigest()[:hash_len]
+
+        name, ext = nncore.split_ext(out)
+        hashed = '{}-{}.{}'.format(name, hash_value, ext).rstrip('.')
+        nncore.rename(out, hashed)
 
 
 def model_soup(model1, model2, out='model.pth', device='cpu'):
     """
     Combine two models by calculating the element-wise average of their weight
     matrices (i.e. cooking model soups [1]). The output model is expected to
     have better performance compaired with the original ones.
```

### Comparing `nncore-0.4.1/nncore/ops/__init__.py` & `nncore-0.4.2/nncore/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/ops/bbox.py` & `nncore-0.4.2/nncore/ops/bbox.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/ops/matrix.py` & `nncore-0.4.2/nncore/ops/matrix.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/ops/temporal.py` & `nncore-0.4.2/nncore/ops/temporal.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/optim/builder.py` & `nncore-0.4.2/nncore/optim/builder.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/optim/lamb.py` & `nncore-0.4.2/nncore/optim/lamb.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/parallel/collate.py` & `nncore-0.4.2/nncore/parallel/collate.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/parallel/container.py` & `nncore-0.4.2/nncore/parallel/container.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/parallel/parallel.py` & `nncore-0.4.2/nncore/parallel/parallel.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/utils/__init__.py` & `nncore-0.4.2/nncore/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/utils/binder.py` & `nncore-0.4.2/nncore/utils/binder.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/utils/config.py` & `nncore-0.4.2/nncore/utils/config.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/utils/data.py` & `nncore-0.4.2/nncore/utils/data.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/utils/env.py` & `nncore-0.4.2/nncore/utils/env.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/utils/logger.py` & `nncore-0.4.2/nncore/utils/logger.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/utils/misc.py` & `nncore-0.4.2/nncore/utils/misc.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/utils/network.py` & `nncore-0.4.2/nncore/utils/network.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/utils/path.py` & `nncore-0.4.2/nncore/utils/path.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/utils/progress.py` & `nncore-0.4.2/nncore/utils/progress.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,16 +126,16 @@
 
             if self._num_tasks is not None:
                 perc = self._completed / self._num_tasks
                 eta = int(ela * (1 - perc) / perc + 0.5)
                 eta_str = self._get_time_str(math.ceil(eta))
                 end_str = '\n' if self._num_tasks == self._completed else ''
                 if self._percentage:
-                    msg = self._pb.format(f'{round(perc*100, 1)}%', ela_str,
-                                          eta_str, end_str)
+                    msg = self._pb.format('{}%'.format(round(perc * 100, 1)),
+                                          ela_str, eta_str, end_str)
                 else:
                     msg = self._wb.format(self._completed, self._num_tasks,
                                           fps, ela_str, eta_str, end_str)
                 bar_width = self._get_bar_width(msg)
                 mark_width = int(bar_width * perc)
                 chars = '>' * mark_width + ' ' * (bar_width - mark_width)
                 msg = msg.format(chars)
```

### Comparing `nncore-0.4.1/nncore/utils/registry.py` & `nncore-0.4.2/nncore/utils/registry.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/utils/timer.py` & `nncore-0.4.2/nncore/utils/timer.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore/video/io.py` & `nncore-0.4.2/nncore/video/io.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/nncore.egg-info/PKG-INFO` & `nncore-0.4.2/nncore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nncore
-Version: 0.4.1
+Version: 0.4.2
 Summary: A lightweight machine learning toolkit for researchers.
 Home-page: https://github.com/yeliudev/nncore
 Author: Ye Liu
 Author-email: yeliudev@outlook.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nncore Version: 0.4.1 Summary: A lightweight
+Metadata-Version: 2.1 Name: nncore Version: 0.4.2 Summary: A lightweight
 machine learning toolkit for researchers. Home-page: https://github.com/
 yeliudev/nncore Author: Ye Liu Author-email: yeliudev@outlook.com License: MIT
 Classifier: Development Status :: 4 - Beta Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
```

### Comparing `nncore-0.4.1/nncore.egg-info/SOURCES.txt` & `nncore-0.4.2/nncore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/setup.cfg` & `nncore-0.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/setup.py` & `nncore-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/tests/test_config.py` & `nncore-0.4.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/tests/test_data.py` & `nncore-0.4.2/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/tests/test_io.py` & `nncore-0.4.2/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/tests/test_logger.py` & `nncore-0.4.2/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/tests/test_path.py` & `nncore-0.4.2/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `nncore-0.4.1/tests/test_registry.py` & `nncore-0.4.2/tests/test_registry.py`

 * *Files identical despite different names*

