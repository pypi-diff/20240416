# Comparing `tmp/thingsvision-2.5.3.tar.gz` & `tmp/thingsvision-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thingsvision-2.5.3.tar", last modified: Mon Apr  8 11:03:26 2024, max compression
+gzip compressed data, was "thingsvision-2.5.4.tar", last modified: Tue Apr 16 08:06:45 2024, max compression
```

## Comparing `thingsvision-2.5.3.tar` & `thingsvision-2.5.4.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.384412 thingsvision-2.5.3/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1097 2021-01-22 09:49:59.000000 thingsvision-2.5.3/LICENSE
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    16318 2024-04-08 11:03:26.384090 thingsvision-2.5.3/PKG-INFO
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    15715 2024-04-08 11:02:58.000000 thingsvision-2.5.3/README.md
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       38 2024-04-08 11:03:26.384488 thingsvision-2.5.3/setup.cfg
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1747 2023-04-30 10:17:04.000000 thingsvision-2.5.3/setup.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.352435 thingsvision-2.5.3/tests/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-02-02 09:19:53.000000 thingsvision-2.5.3/tests/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.353834 thingsvision-2.5.3/tests/extractor/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.5.3/tests/extractor/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.355668 thingsvision-2.5.3/tests/extractor/extraction/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.5.3/tests/extractor/extraction/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2452 2024-04-06 10:03:37.000000 thingsvision-2.5.3/tests/extractor/extraction/test_custom_model.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3196 2024-04-01 11:22:39.000000 thingsvision-2.5.3/tests/extractor/extraction/test_model_extractor.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1954 2024-04-06 10:03:24.000000 thingsvision-2.5.3/tests/extractor/extraction/test_pretrained_model.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2977 2024-04-06 10:04:01.000000 thingsvision-2.5.3/tests/extractor/extraction/test_torch_vs_tensorflow.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4459 2024-04-01 11:29:46.000000 thingsvision-2.5.3/tests/extractor/test_load_extractor.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1487 2023-02-22 09:56:38.000000 thingsvision-2.5.3/tests/extractor/test_transformations.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    11484 2024-04-08 11:02:58.000000 thingsvision-2.5.3/tests/helper.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4447 2023-02-22 09:56:38.000000 thingsvision-2.5.3/tests/test_features.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3719 2022-08-31 09:02:04.000000 thingsvision-2.5.3/tests/test_rest.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.356855 thingsvision-2.5.3/thingsvision/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      103 2022-11-09 16:59:35.000000 thingsvision-2.5.3/thingsvision/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       22 2024-04-08 11:02:58.000000 thingsvision-2.5.3/thingsvision/_version.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.358808 thingsvision-2.5.3/thingsvision/core/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-23 10:25:59.000000 thingsvision-2.5.3/thingsvision/core/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.359574 thingsvision-2.5.3/thingsvision/core/cka/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       21 2022-08-22 09:49:44.000000 thingsvision-2.5.3/thingsvision/core/cka/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1974 2022-08-22 09:49:44.000000 thingsvision-2.5.3/thingsvision/core/cka/base.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.362224 thingsvision-2.5.3/thingsvision/core/extraction/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      176 2024-04-01 11:36:55.000000 thingsvision-2.5.3/thingsvision/core/extraction/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    10749 2024-04-04 09:43:21.000000 thingsvision-2.5.3/thingsvision/core/extraction/base.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    17334 2024-04-08 11:02:58.000000 thingsvision-2.5.3/thingsvision/core/extraction/extractors.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     8452 2024-04-04 09:43:21.000000 thingsvision-2.5.3/thingsvision/core/extraction/helpers.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3134 2024-04-04 09:43:21.000000 thingsvision-2.5.3/thingsvision/core/extraction/tensorflow.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     8530 2024-04-08 11:02:58.000000 thingsvision-2.5.3/thingsvision/core/extraction/torch.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.362996 thingsvision-2.5.3/thingsvision/core/rsa/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       59 2022-08-22 09:49:44.000000 thingsvision-2.5.3/thingsvision/core/rsa/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-29 15:24:25.000000 thingsvision-2.5.3/thingsvision/core/rsa/base.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4651 2022-08-31 09:02:04.000000 thingsvision-2.5.3/thingsvision/core/rsa/helpers.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.369261 thingsvision-2.5.3/thingsvision/custom_models/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      286 2023-08-04 09:46:20.000000 thingsvision-2.5.3/thingsvision/custom_models/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      620 2023-07-11 09:50:14.000000 thingsvision-2.5.3/thingsvision/custom_models/alexnet_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      627 2023-07-11 09:50:14.000000 thingsvision-2.5.3/thingsvision/custom_models/alexnet_salobjsub.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.371580 thingsvision-2.5.3/thingsvision/custom_models/cornet/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1474 2022-08-22 09:49:44.000000 thingsvision-2.5.3/thingsvision/custom_models/cornet/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3588 2022-08-22 09:49:44.000000 thingsvision-2.5.3/thingsvision/custom_models/cornet/cornet_r.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3682 2022-08-22 09:49:44.000000 thingsvision-2.5.3/thingsvision/custom_models/cornet/cornet_rt.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4203 2022-08-22 09:49:44.000000 thingsvision-2.5.3/thingsvision/custom_models/cornet/cornet_s.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-08-22 09:49:44.000000 thingsvision-2.5.3/thingsvision/custom_models/cornet/cornet_z.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      287 2023-01-18 14:03:54.000000 thingsvision-2.5.3/thingsvision/custom_models/custom.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.372557 thingsvision-2.5.3/thingsvision/custom_models/dreamsim/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       31 2023-08-04 09:46:20.000000 thingsvision-2.5.3/thingsvision/custom_models/dreamsim/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1999 2024-03-19 09:46:42.000000 thingsvision-2.5.3/thingsvision/custom_models/dreamsim/dreamsim.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.373538 thingsvision-2.5.3/thingsvision/custom_models/harmonization/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       41 2023-03-06 11:11:47.000000 thingsvision-2.5.3/thingsvision/custom_models/harmonization/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1366 2023-03-06 11:11:52.000000 thingsvision-2.5.3/thingsvision/custom_models/harmonization/harmonization.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      629 2023-08-04 09:17:34.000000 thingsvision-2.5.3/thingsvision/custom_models/inception_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      453 2023-07-26 10:09:51.000000 thingsvision-2.5.3/thingsvision/custom_models/official_clip.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1033 2023-07-11 09:50:14.000000 thingsvision-2.5.3/thingsvision/custom_models/openclip.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      623 2023-08-04 09:16:38.000000 thingsvision-2.5.3/thingsvision/custom_models/resnet50_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      614 2023-08-04 09:31:47.000000 thingsvision-2.5.3/thingsvision/custom_models/vgg16_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      621 2023-08-04 09:46:20.000000 thingsvision-2.5.3/thingsvision/custom_models/vgg16bn_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     5980 2024-03-19 09:46:42.000000 thingsvision-2.5.3/thingsvision/thingsvision.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.374049 thingsvision-2.5.3/thingsvision/utils/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-26 11:38:32.000000 thingsvision-2.5.3/thingsvision/utils/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.374860 thingsvision-2.5.3/thingsvision/utils/alignment/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       31 2024-03-28 13:19:33.000000 thingsvision-2.5.3/thingsvision/utils/alignment/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2633 2024-03-28 13:33:43.000000 thingsvision-2.5.3/thingsvision/utils/alignment/transforms.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.375392 thingsvision-2.5.3/thingsvision/utils/checkpointing/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      522 2023-07-26 10:09:51.000000 thingsvision-2.5.3/thingsvision/utils/checkpointing/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.378414 thingsvision-2.5.3/thingsvision/utils/data/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-11-15 12:25:36.000000 thingsvision-2.5.3/thingsvision/utils/data/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1778 2022-11-15 12:25:36.000000 thingsvision-2.5.3/thingsvision/utils/data/data_loader.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7808 2022-11-15 12:25:36.000000 thingsvision-2.5.3/thingsvision/utils/data/dataset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2969 2022-08-25 08:25:51.000000 thingsvision-2.5.3/thingsvision/utils/data/helpers.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.379288 thingsvision-2.5.3/thingsvision/utils/imagenet/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2355 2022-08-22 09:49:44.000000 thingsvision-2.5.3/thingsvision/utils/imagenet/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.379838 thingsvision-2.5.3/thingsvision/utils/models/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2023-08-09 09:09:13.000000 thingsvision-2.5.3/thingsvision/utils/models/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.381332 thingsvision-2.5.3/thingsvision/utils/models/dino/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       62 2024-04-05 17:27:52.000000 thingsvision-2.5.3/thingsvision/utils/models/dino/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2396 2023-08-08 13:01:35.000000 thingsvision-2.5.3/thingsvision/utils/models/dino/utils.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    11168 2023-08-08 13:01:35.000000 thingsvision-2.5.3/thingsvision/utils/models/dino/vision_transformer.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.382720 thingsvision-2.5.3/thingsvision/utils/models/mae/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      116 2024-04-08 11:02:58.000000 thingsvision-2.5.3/thingsvision/utils/models/mae/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2157 2024-04-08 11:02:58.000000 thingsvision-2.5.3/thingsvision/utils/models/mae/utils.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2108 2024-04-08 11:02:58.000000 thingsvision-2.5.3/thingsvision/utils/models/mae/vit_mae.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.383406 thingsvision-2.5.3/thingsvision/utils/storing/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       67 2022-08-22 09:49:44.000000 thingsvision-2.5.3/thingsvision/utils/storing/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7325 2023-02-22 09:56:38.000000 thingsvision-2.5.3/thingsvision/utils/storing/helpers.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-08 11:03:26.358587 thingsvision-2.5.3/thingsvision.egg-info/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    16318 2024-04-08 11:03:26.000000 thingsvision-2.5.3/thingsvision.egg-info/PKG-INFO
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2773 2024-04-08 11:03:26.000000 thingsvision-2.5.3/thingsvision.egg-info/SOURCES.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       39 2024-04-08 11:03:26.000000 thingsvision-2.5.3/thingsvision.egg-info/dependency_links.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       64 2024-04-08 11:03:26.000000 thingsvision-2.5.3/thingsvision.egg-info/entry_points.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      332 2024-04-08 11:03:26.000000 thingsvision-2.5.3/thingsvision.egg-info/requires.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       19 2024-04-08 11:03:26.000000 thingsvision-2.5.3/thingsvision.egg-info/top_level.txt
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.896856 thingsvision-2.5.4/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1097 2021-01-22 09:49:59.000000 thingsvision-2.5.4/LICENSE
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    16350 2024-04-16 08:06:45.896520 thingsvision-2.5.4/PKG-INFO
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    15747 2024-04-09 09:52:31.000000 thingsvision-2.5.4/README.md
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       38 2024-04-16 08:06:45.896971 thingsvision-2.5.4/setup.cfg
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1747 2023-04-30 10:17:04.000000 thingsvision-2.5.4/setup.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.881827 thingsvision-2.5.4/tests/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-02-02 09:19:53.000000 thingsvision-2.5.4/tests/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.882452 thingsvision-2.5.4/tests/extractor/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.5.4/tests/extractor/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.883501 thingsvision-2.5.4/tests/extractor/extraction/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.5.4/tests/extractor/extraction/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2452 2024-04-06 10:03:37.000000 thingsvision-2.5.4/tests/extractor/extraction/test_custom_model.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3196 2024-04-01 11:22:39.000000 thingsvision-2.5.4/tests/extractor/extraction/test_model_extractor.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1954 2024-04-06 10:03:24.000000 thingsvision-2.5.4/tests/extractor/extraction/test_pretrained_model.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2977 2024-04-06 10:04:01.000000 thingsvision-2.5.4/tests/extractor/extraction/test_torch_vs_tensorflow.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4459 2024-04-01 11:29:46.000000 thingsvision-2.5.4/tests/extractor/test_load_extractor.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1487 2023-02-22 09:56:38.000000 thingsvision-2.5.4/tests/extractor/test_transformations.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    11484 2024-04-08 11:02:58.000000 thingsvision-2.5.4/tests/helper.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4447 2023-02-22 09:56:38.000000 thingsvision-2.5.4/tests/test_features.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3719 2022-08-31 09:02:04.000000 thingsvision-2.5.4/tests/test_rest.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.884148 thingsvision-2.5.4/thingsvision/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      103 2022-11-09 16:59:35.000000 thingsvision-2.5.4/thingsvision/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       22 2024-04-16 08:06:05.000000 thingsvision-2.5.4/thingsvision/_version.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.885660 thingsvision-2.5.4/thingsvision/core/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-23 10:25:59.000000 thingsvision-2.5.4/thingsvision/core/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.886042 thingsvision-2.5.4/thingsvision/core/cka/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       21 2022-08-22 09:49:44.000000 thingsvision-2.5.4/thingsvision/core/cka/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1974 2022-08-22 09:49:44.000000 thingsvision-2.5.4/thingsvision/core/cka/base.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.887430 thingsvision-2.5.4/thingsvision/core/extraction/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      176 2024-04-01 11:36:55.000000 thingsvision-2.5.4/thingsvision/core/extraction/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    10749 2024-04-04 09:43:21.000000 thingsvision-2.5.4/thingsvision/core/extraction/base.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    17334 2024-04-08 11:02:58.000000 thingsvision-2.5.4/thingsvision/core/extraction/extractors.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     8452 2024-04-04 09:43:21.000000 thingsvision-2.5.4/thingsvision/core/extraction/helpers.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3134 2024-04-04 09:43:21.000000 thingsvision-2.5.4/thingsvision/core/extraction/tensorflow.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     8530 2024-04-08 11:02:58.000000 thingsvision-2.5.4/thingsvision/core/extraction/torch.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.888128 thingsvision-2.5.4/thingsvision/core/rsa/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       59 2022-08-22 09:49:44.000000 thingsvision-2.5.4/thingsvision/core/rsa/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-29 15:24:25.000000 thingsvision-2.5.4/thingsvision/core/rsa/base.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4651 2022-08-31 09:02:04.000000 thingsvision-2.5.4/thingsvision/core/rsa/helpers.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.890391 thingsvision-2.5.4/thingsvision/custom_models/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      286 2023-08-04 09:46:20.000000 thingsvision-2.5.4/thingsvision/custom_models/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      620 2023-07-11 09:50:14.000000 thingsvision-2.5.4/thingsvision/custom_models/alexnet_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      627 2023-07-11 09:50:14.000000 thingsvision-2.5.4/thingsvision/custom_models/alexnet_salobjsub.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.891612 thingsvision-2.5.4/thingsvision/custom_models/cornet/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1474 2022-08-22 09:49:44.000000 thingsvision-2.5.4/thingsvision/custom_models/cornet/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3588 2022-08-22 09:49:44.000000 thingsvision-2.5.4/thingsvision/custom_models/cornet/cornet_r.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3682 2022-08-22 09:49:44.000000 thingsvision-2.5.4/thingsvision/custom_models/cornet/cornet_rt.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4203 2022-08-22 09:49:44.000000 thingsvision-2.5.4/thingsvision/custom_models/cornet/cornet_s.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-08-22 09:49:44.000000 thingsvision-2.5.4/thingsvision/custom_models/cornet/cornet_z.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      287 2023-01-18 14:03:54.000000 thingsvision-2.5.4/thingsvision/custom_models/custom.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.892058 thingsvision-2.5.4/thingsvision/custom_models/dreamsim/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       31 2023-08-04 09:46:20.000000 thingsvision-2.5.4/thingsvision/custom_models/dreamsim/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1999 2024-03-19 09:46:42.000000 thingsvision-2.5.4/thingsvision/custom_models/dreamsim/dreamsim.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.892474 thingsvision-2.5.4/thingsvision/custom_models/harmonization/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       41 2023-03-06 11:11:47.000000 thingsvision-2.5.4/thingsvision/custom_models/harmonization/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1366 2023-03-06 11:11:52.000000 thingsvision-2.5.4/thingsvision/custom_models/harmonization/harmonization.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      629 2023-08-04 09:17:34.000000 thingsvision-2.5.4/thingsvision/custom_models/inception_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      453 2023-07-26 10:09:51.000000 thingsvision-2.5.4/thingsvision/custom_models/official_clip.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1033 2023-07-11 09:50:14.000000 thingsvision-2.5.4/thingsvision/custom_models/openclip.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      623 2023-08-04 09:16:38.000000 thingsvision-2.5.4/thingsvision/custom_models/resnet50_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      614 2023-08-04 09:31:47.000000 thingsvision-2.5.4/thingsvision/custom_models/vgg16_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      621 2023-08-04 09:46:20.000000 thingsvision-2.5.4/thingsvision/custom_models/vgg16bn_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     5992 2024-04-16 08:05:49.000000 thingsvision-2.5.4/thingsvision/thingsvision.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.892692 thingsvision-2.5.4/thingsvision/utils/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-26 11:38:32.000000 thingsvision-2.5.4/thingsvision/utils/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.893068 thingsvision-2.5.4/thingsvision/utils/alignment/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       31 2024-03-28 13:19:33.000000 thingsvision-2.5.4/thingsvision/utils/alignment/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2633 2024-03-28 13:33:43.000000 thingsvision-2.5.4/thingsvision/utils/alignment/transforms.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.893280 thingsvision-2.5.4/thingsvision/utils/checkpointing/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      522 2023-07-26 10:09:51.000000 thingsvision-2.5.4/thingsvision/utils/checkpointing/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.894135 thingsvision-2.5.4/thingsvision/utils/data/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-11-15 12:25:36.000000 thingsvision-2.5.4/thingsvision/utils/data/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1778 2022-11-15 12:25:36.000000 thingsvision-2.5.4/thingsvision/utils/data/data_loader.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7808 2022-11-15 12:25:36.000000 thingsvision-2.5.4/thingsvision/utils/data/dataset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2969 2022-08-25 08:25:51.000000 thingsvision-2.5.4/thingsvision/utils/data/helpers.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.894352 thingsvision-2.5.4/thingsvision/utils/imagenet/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2355 2022-08-22 09:49:44.000000 thingsvision-2.5.4/thingsvision/utils/imagenet/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.894565 thingsvision-2.5.4/thingsvision/utils/models/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2023-08-09 09:09:13.000000 thingsvision-2.5.4/thingsvision/utils/models/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.895148 thingsvision-2.5.4/thingsvision/utils/models/dino/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       62 2024-04-05 17:27:52.000000 thingsvision-2.5.4/thingsvision/utils/models/dino/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2396 2023-08-08 13:01:35.000000 thingsvision-2.5.4/thingsvision/utils/models/dino/utils.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    11168 2023-08-08 13:01:35.000000 thingsvision-2.5.4/thingsvision/utils/models/dino/vision_transformer.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.895779 thingsvision-2.5.4/thingsvision/utils/models/mae/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      116 2024-04-08 11:02:58.000000 thingsvision-2.5.4/thingsvision/utils/models/mae/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2157 2024-04-08 11:02:58.000000 thingsvision-2.5.4/thingsvision/utils/models/mae/utils.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2108 2024-04-08 11:02:58.000000 thingsvision-2.5.4/thingsvision/utils/models/mae/vit_mae.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.896203 thingsvision-2.5.4/thingsvision/utils/storing/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       67 2022-08-22 09:49:44.000000 thingsvision-2.5.4/thingsvision/utils/storing/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7325 2023-02-22 09:56:38.000000 thingsvision-2.5.4/thingsvision/utils/storing/helpers.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.885451 thingsvision-2.5.4/thingsvision.egg-info/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    16350 2024-04-16 08:06:45.000000 thingsvision-2.5.4/thingsvision.egg-info/PKG-INFO
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2773 2024-04-16 08:06:45.000000 thingsvision-2.5.4/thingsvision.egg-info/SOURCES.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       39 2024-04-16 08:06:45.000000 thingsvision-2.5.4/thingsvision.egg-info/dependency_links.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       64 2024-04-16 08:06:45.000000 thingsvision-2.5.4/thingsvision.egg-info/entry_points.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      332 2024-04-16 08:06:45.000000 thingsvision-2.5.4/thingsvision.egg-info/requires.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       19 2024-04-16 08:06:45.000000 thingsvision-2.5.4/thingsvision.egg-info/top_level.txt
```

### Comparing `thingsvision-2.5.3/LICENSE` & `thingsvision-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/PKG-INFO` & `thingsvision-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thingsvision
-Version: 2.5.3
+Version: 2.5.4
 Summary: Extracting image features from state-of-the-art neural networks for Computer Vision made easy
 Home-page: https://github.com/ViCCo-Group/thingsvision
 Author: Lukas Muttenthaler
 Author-email: muttenthaler@cbs.mpg.de
 License: MIT License
 Keywords: feature extraction
 Classifier: Programming Language :: Python :: 3.8
@@ -88,20 +88,22 @@
 Neural networks come from different sources. With `thingsvision`, you can extract image representations of all models from:
 - [torchvision](https://pytorch.org/vision/0.8/models.html)
 - [Keras](https://www.tensorflow.org/api_docs/python/tf/keras/applications)
 - [timm](https://github.com/rwightman/pytorch-image-models)
 - `ssl` (self-supervised learning models)
   - `simclr-rn50`, `mocov2-rn50`, `barlowtwins-rn50`, `pirl-rn50`
   - `jigsaw-rn50`, `rotnet-rn50`, `swav-rn50`, `vicreg-rn50`
-  - `dino-rn50`, `dino-xcit-{small/medium}-{12/24}-p{8/16}`, `dino-vit-{tiny/small/base}-p{8/16}`, `dinov2-vit-{small/base/large/giant}-p14`
+  - `dino-rn50`, `dino-xcit-{small/medium}-{12/24}-p{8/16}`
+  - `dino-vit-{tiny/small/base}-p{8/16}`
+  - `dinov2-vit-{small/base/large/giant}-p14`
   - `mae-vit-{base/large}-p16`, `mae-vit-huge-p14`<br>
 - [OpenCLIP](https://github.com/mlfoundations/open_clip) models (CLIP trained on LAION-{400M/2B/5B})
 - [CLIP](https://github.com/openai/CLIP) models (CLIP trained on WiT)
 - a few custom models (Alexnet, VGG-16, Resnet50, and Inception_v3) trained on [Ecoset](https://www.pnas.org/doi/10.1073/pnas.2011417118) rather than ImageNet and one Alexnet model pretrained on ImageNet and fine-tuned on [SalObjSub](https://cs-people.bu.edu/jmzhang/sos.html)<br>
-- each of the many [CORnet](https://github.com/dicarlolab/CORnet) versions
+- each of the many [CORnet](https://github.com/dicarlolab/CORnet) versions (recurrent vision models)
 - [Harmonization](https://arxiv.org/abs/2211.04533) models (see [Harmonization repo](https://github.com/serre-lab/harmonization)). The default variant is `ViT_B16`. Other available models are `ResNet50`, `VGG16`, `EfficientNetB0`, `tiny_ConvNeXT`, `tiny_MaxViT`, and `LeViT_small`<br> 
 - [DreamSim](https://dreamsim-nights.github.io/) models  (see [DreamSim repo](https://github.com/ssundaram21/dreamsim)). The default variant is `open_clip_vitb32`. Other available models are `clip_vitb32`, `dino_vitb16`, and an `ensemble`. See the [docs](https://vicco-group.github.io/thingsvision/AvailableModels.html#dreamsim) for more information
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 <!-- Getting Started -->
@@ -155,15 +157,15 @@
 - `thingsvision show-model`
 - `thingsvision extract-features`
 
 Example calls might look as follows:
 
 ```bash
 thingsvision show-model --model-name "alexnet" --source "torchvision"
-thingsvision extract_features --image-root "./data" --model-name "alexnet" --module-name "features.10" --batch-size 32 --device "cuda" --source "torchvision" --file-format "npy" --out-path "./features"
+thingsvision extract-features --image-root "./data" --model-name "alexnet" --module-name "features.10" --batch-size 32 --device "cuda" --source "torchvision" --file-format "npy" --out-path "./features"
 ```
 
 See `thingsvision show-model -h` and `thingsvision extract-features -h` for a list of all possible arguments. Note that the CLI provides just the basic extraction functionalities but is probably enough for most users that don't want to dive too deep into various models and modules. If you need more fine-grained control over the extraction itself, we recommend to use the python package directly and write your own Python script.
 
 #### Python commands
 
 To do this start by importing all the necessary components and instantiating a `thingsvision` extractor. Here we're using `CLIP` from the official clip repo as the model to extract features from and also load the model to GPU for faster inference,
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thingsvision Version: 2.5.3 Summary: Extracting
+Metadata-Version: 2.1 Name: thingsvision Version: 2.5.4 Summary: Extracting
 image features from state-of-the-art neural networks for Computer Vision made
 easy Home-page: https://github.com/ViCCo-Group/thingsvision Author: Lukas
 Muttenthaler Author-email: muttenthaler@cbs.mpg.de License: MIT License
 Keywords: feature extraction Classifier: Programming Language :: Python :: 3.8
 Classifier: Natural Language :: English Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Requires-Python:
 >=3.8 Description-Content-Type: text/markdown License-File: LICENSE
@@ -42,29 +42,29 @@
 ### :file_cabinet: Model collection Neural networks come from different
 sources. With `thingsvision`, you can extract image representations of all
 models from: - [torchvision](https://pytorch.org/vision/0.8/models.html) -
 [Keras](https://www.tensorflow.org/api_docs/python/tf/keras/applications) -
 [timm](https://github.com/rwightman/pytorch-image-models) - `ssl` (self-
 supervised learning models) - `simclr-rn50`, `mocov2-rn50`, `barlowtwins-rn50`,
 `pirl-rn50` - `jigsaw-rn50`, `rotnet-rn50`, `swav-rn50`, `vicreg-rn50` - `dino-
-rn50`, `dino-xcit-{small/medium}-{12/24}-p{8/16}`, `dino-vit-{tiny/small/base}-
-p{8/16}`, `dinov2-vit-{small/base/large/giant}-p14` - `mae-vit-{base/large}-
-p16`, `mae-vit-huge-p14`
+rn50`, `dino-xcit-{small/medium}-{12/24}-p{8/16}` - `dino-vit-{tiny/small/
+base}-p{8/16}` - `dinov2-vit-{small/base/large/giant}-p14` - `mae-vit-{base/
+large}-p16`, `mae-vit-huge-p14`
 - [OpenCLIP](https://github.com/mlfoundations/open_clip) models (CLIP trained
 on LAION-{400M/2B/5B}) - [CLIP](https://github.com/openai/CLIP) models (CLIP
 trained on WiT) - a few custom models (Alexnet, VGG-16, Resnet50, and
 Inception_v3) trained on [Ecoset](https://www.pnas.org/doi/10.1073/
 pnas.2011417118) rather than ImageNet and one Alexnet model pretrained on
 ImageNet and fine-tuned on [SalObjSub](https://cs-people.bu.edu/jmzhang/
 sos.html)
-- each of the many [CORnet](https://github.com/dicarlolab/CORnet) versions -
-[Harmonization](https://arxiv.org/abs/2211.04533) models (see [Harmonization
-repo](https://github.com/serre-lab/harmonization)). The default variant is
-`ViT_B16`. Other available models are `ResNet50`, `VGG16`, `EfficientNetB0`,
-`tiny_ConvNeXT`, `tiny_MaxViT`, and `LeViT_small`
+- each of the many [CORnet](https://github.com/dicarlolab/CORnet) versions
+(recurrent vision models) - [Harmonization](https://arxiv.org/abs/2211.04533)
+models (see [Harmonization repo](https://github.com/serre-lab/harmonization)).
+The default variant is `ViT_B16`. Other available models are `ResNet50`,
+`VGG16`, `EfficientNetB0`, `tiny_ConvNeXT`, `tiny_MaxViT`, and `LeViT_small`
 - [DreamSim](https://dreamsim-nights.github.io/) models (see [DreamSim repo]
 (https://github.com/ssundaram21/dreamsim)). The default variant is
 `open_clip_vitb32`. Other available models are `clip_vitb32`, `dino_vitb16`,
 and an `ensemble`. See the [docs](https://vicco-group.github.io/thingsvision/
 AvailableModels.html#dreamsim) for more information
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## :running: Getting Started ### :computer: Setting up your environment ####
@@ -97,15 +97,15 @@
 ### :mag: Basic usage #### Command Line Interface (CLI) `thingsvision` was
 designed to simplify feature extraction. If you have some folder of images
 (e.g., `./images`) and want to extract features for each of these images
 without opening a Jupyter Notebook instance or writing a Python script, it's
 probably easiest to use our CLI. The interface includes two options, -
 `thingsvision show-model` - `thingsvision extract-features` Example calls might
 look as follows: ```bash thingsvision show-model --model-name "alexnet" --
-source "torchvision" thingsvision extract_features --image-root "./data" --
+source "torchvision" thingsvision extract-features --image-root "./data" --
 model-name "alexnet" --module-name "features.10" --batch-size 32 --device
 "cuda" --source "torchvision" --file-format "npy" --out-path "./features" ```
 See `thingsvision show-model -h` and `thingsvision extract-features -h` for a
 list of all possible arguments. Note that the CLI provides just the basic
 extraction functionalities but is probably enough for most users that don't
 want to dive too deep into various models and modules. If you need more fine-
 grained control over the extraction itself, we recommend to use the python
```

### Comparing `thingsvision-2.5.3/README.md` & `thingsvision-2.5.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -71,20 +71,22 @@
 Neural networks come from different sources. With `thingsvision`, you can extract image representations of all models from:
 - [torchvision](https://pytorch.org/vision/0.8/models.html)
 - [Keras](https://www.tensorflow.org/api_docs/python/tf/keras/applications)
 - [timm](https://github.com/rwightman/pytorch-image-models)
 - `ssl` (self-supervised learning models)
   - `simclr-rn50`, `mocov2-rn50`, `barlowtwins-rn50`, `pirl-rn50`
   - `jigsaw-rn50`, `rotnet-rn50`, `swav-rn50`, `vicreg-rn50`
-  - `dino-rn50`, `dino-xcit-{small/medium}-{12/24}-p{8/16}`, `dino-vit-{tiny/small/base}-p{8/16}`, `dinov2-vit-{small/base/large/giant}-p14`
+  - `dino-rn50`, `dino-xcit-{small/medium}-{12/24}-p{8/16}`
+  - `dino-vit-{tiny/small/base}-p{8/16}`
+  - `dinov2-vit-{small/base/large/giant}-p14`
   - `mae-vit-{base/large}-p16`, `mae-vit-huge-p14`<br>
 - [OpenCLIP](https://github.com/mlfoundations/open_clip) models (CLIP trained on LAION-{400M/2B/5B})
 - [CLIP](https://github.com/openai/CLIP) models (CLIP trained on WiT)
 - a few custom models (Alexnet, VGG-16, Resnet50, and Inception_v3) trained on [Ecoset](https://www.pnas.org/doi/10.1073/pnas.2011417118) rather than ImageNet and one Alexnet model pretrained on ImageNet and fine-tuned on [SalObjSub](https://cs-people.bu.edu/jmzhang/sos.html)<br>
-- each of the many [CORnet](https://github.com/dicarlolab/CORnet) versions
+- each of the many [CORnet](https://github.com/dicarlolab/CORnet) versions (recurrent vision models)
 - [Harmonization](https://arxiv.org/abs/2211.04533) models (see [Harmonization repo](https://github.com/serre-lab/harmonization)). The default variant is `ViT_B16`. Other available models are `ResNet50`, `VGG16`, `EfficientNetB0`, `tiny_ConvNeXT`, `tiny_MaxViT`, and `LeViT_small`<br> 
 - [DreamSim](https://dreamsim-nights.github.io/) models  (see [DreamSim repo](https://github.com/ssundaram21/dreamsim)). The default variant is `open_clip_vitb32`. Other available models are `clip_vitb32`, `dino_vitb16`, and an `ensemble`. See the [docs](https://vicco-group.github.io/thingsvision/AvailableModels.html#dreamsim) for more information
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 <!-- Getting Started -->
@@ -138,15 +140,15 @@
 - `thingsvision show-model`
 - `thingsvision extract-features`
 
 Example calls might look as follows:
 
 ```bash
 thingsvision show-model --model-name "alexnet" --source "torchvision"
-thingsvision extract_features --image-root "./data" --model-name "alexnet" --module-name "features.10" --batch-size 32 --device "cuda" --source "torchvision" --file-format "npy" --out-path "./features"
+thingsvision extract-features --image-root "./data" --model-name "alexnet" --module-name "features.10" --batch-size 32 --device "cuda" --source "torchvision" --file-format "npy" --out-path "./features"
 ```
 
 See `thingsvision show-model -h` and `thingsvision extract-features -h` for a list of all possible arguments. Note that the CLI provides just the basic extraction functionalities but is probably enough for most users that don't want to dive too deep into various models and modules. If you need more fine-grained control over the extraction itself, we recommend to use the python package directly and write your own Python script.
 
 #### Python commands
 
 To do this start by importing all the necessary components and instantiating a `thingsvision` extractor. Here we're using `CLIP` from the official clip repo as the model to extract features from and also load the model to GPU for faster inference,
```

#### html2text {}

```diff
@@ -34,29 +34,29 @@
 ### :file_cabinet: Model collection Neural networks come from different
 sources. With `thingsvision`, you can extract image representations of all
 models from: - [torchvision](https://pytorch.org/vision/0.8/models.html) -
 [Keras](https://www.tensorflow.org/api_docs/python/tf/keras/applications) -
 [timm](https://github.com/rwightman/pytorch-image-models) - `ssl` (self-
 supervised learning models) - `simclr-rn50`, `mocov2-rn50`, `barlowtwins-rn50`,
 `pirl-rn50` - `jigsaw-rn50`, `rotnet-rn50`, `swav-rn50`, `vicreg-rn50` - `dino-
-rn50`, `dino-xcit-{small/medium}-{12/24}-p{8/16}`, `dino-vit-{tiny/small/base}-
-p{8/16}`, `dinov2-vit-{small/base/large/giant}-p14` - `mae-vit-{base/large}-
-p16`, `mae-vit-huge-p14`
+rn50`, `dino-xcit-{small/medium}-{12/24}-p{8/16}` - `dino-vit-{tiny/small/
+base}-p{8/16}` - `dinov2-vit-{small/base/large/giant}-p14` - `mae-vit-{base/
+large}-p16`, `mae-vit-huge-p14`
 - [OpenCLIP](https://github.com/mlfoundations/open_clip) models (CLIP trained
 on LAION-{400M/2B/5B}) - [CLIP](https://github.com/openai/CLIP) models (CLIP
 trained on WiT) - a few custom models (Alexnet, VGG-16, Resnet50, and
 Inception_v3) trained on [Ecoset](https://www.pnas.org/doi/10.1073/
 pnas.2011417118) rather than ImageNet and one Alexnet model pretrained on
 ImageNet and fine-tuned on [SalObjSub](https://cs-people.bu.edu/jmzhang/
 sos.html)
-- each of the many [CORnet](https://github.com/dicarlolab/CORnet) versions -
-[Harmonization](https://arxiv.org/abs/2211.04533) models (see [Harmonization
-repo](https://github.com/serre-lab/harmonization)). The default variant is
-`ViT_B16`. Other available models are `ResNet50`, `VGG16`, `EfficientNetB0`,
-`tiny_ConvNeXT`, `tiny_MaxViT`, and `LeViT_small`
+- each of the many [CORnet](https://github.com/dicarlolab/CORnet) versions
+(recurrent vision models) - [Harmonization](https://arxiv.org/abs/2211.04533)
+models (see [Harmonization repo](https://github.com/serre-lab/harmonization)).
+The default variant is `ViT_B16`. Other available models are `ResNet50`,
+`VGG16`, `EfficientNetB0`, `tiny_ConvNeXT`, `tiny_MaxViT`, and `LeViT_small`
 - [DreamSim](https://dreamsim-nights.github.io/) models (see [DreamSim repo]
 (https://github.com/ssundaram21/dreamsim)). The default variant is
 `open_clip_vitb32`. Other available models are `clip_vitb32`, `dino_vitb16`,
 and an `ensemble`. See the [docs](https://vicco-group.github.io/thingsvision/
 AvailableModels.html#dreamsim) for more information
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## :running: Getting Started ### :computer: Setting up your environment ####
@@ -89,15 +89,15 @@
 ### :mag: Basic usage #### Command Line Interface (CLI) `thingsvision` was
 designed to simplify feature extraction. If you have some folder of images
 (e.g., `./images`) and want to extract features for each of these images
 without opening a Jupyter Notebook instance or writing a Python script, it's
 probably easiest to use our CLI. The interface includes two options, -
 `thingsvision show-model` - `thingsvision extract-features` Example calls might
 look as follows: ```bash thingsvision show-model --model-name "alexnet" --
-source "torchvision" thingsvision extract_features --image-root "./data" --
+source "torchvision" thingsvision extract-features --image-root "./data" --
 model-name "alexnet" --module-name "features.10" --batch-size 32 --device
 "cuda" --source "torchvision" --file-format "npy" --out-path "./features" ```
 See `thingsvision show-model -h` and `thingsvision extract-features -h` for a
 list of all possible arguments. Note that the CLI provides just the basic
 extraction functionalities but is probably enough for most users that don't
 want to dive too deep into various models and modules. If you need more fine-
 grained control over the extraction itself, we recommend to use the python
```

### Comparing `thingsvision-2.5.3/setup.py` & `thingsvision-2.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/tests/extractor/extraction/test_custom_model.py` & `thingsvision-2.5.4/tests/extractor/extraction/test_custom_model.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/tests/extractor/extraction/test_model_extractor.py` & `thingsvision-2.5.4/tests/extractor/extraction/test_model_extractor.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/tests/extractor/extraction/test_pretrained_model.py` & `thingsvision-2.5.4/tests/extractor/extraction/test_pretrained_model.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/tests/extractor/extraction/test_torch_vs_tensorflow.py` & `thingsvision-2.5.4/tests/extractor/extraction/test_torch_vs_tensorflow.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/tests/extractor/test_load_extractor.py` & `thingsvision-2.5.4/tests/extractor/test_load_extractor.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/tests/extractor/test_transformations.py` & `thingsvision-2.5.4/tests/extractor/test_transformations.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/tests/helper.py` & `thingsvision-2.5.4/tests/helper.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/tests/test_features.py` & `thingsvision-2.5.4/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/tests/test_rest.py` & `thingsvision-2.5.4/tests/test_rest.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/thingsvision/core/cka/base.py` & `thingsvision-2.5.4/thingsvision/core/cka/base.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/thingsvision/core/extraction/base.py` & `thingsvision-2.5.4/thingsvision/core/extraction/base.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/thingsvision/core/extraction/extractors.py` & `thingsvision-2.5.4/thingsvision/core/extraction/extractors.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/thingsvision/core/extraction/helpers.py` & `thingsvision-2.5.4/thingsvision/core/extraction/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/thingsvision/core/extraction/tensorflow.py` & `thingsvision-2.5.4/thingsvision/core/extraction/tensorflow.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/thingsvision/core/extraction/torch.py` & `thingsvision-2.5.4/thingsvision/core/extraction/torch.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/thingsvision/core/rsa/helpers.py` & `thingsvision-2.5.4/thingsvision/core/rsa/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/thingsvision/custom_models/alexnet_ecoset.py` & `thingsvision-2.5.4/thingsvision/custom_models/alexnet_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/thingsvision/custom_models/alexnet_salobjsub.py` & `thingsvision-2.5.4/thingsvision/custom_models/alexnet_salobjsub.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/thingsvision/custom_models/cornet/__init__.py` & `thingsvision-2.5.4/thingsvision/custom_models/cornet/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/thingsvision/custom_models/cornet/cornet_r.py` & `thingsvision-2.5.4/thingsvision/custom_models/cornet/cornet_r.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/thingsvision/custom_models/cornet/cornet_rt.py` & `thingsvision-2.5.4/thingsvision/custom_models/cornet/cornet_rt.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/thingsvision/custom_models/cornet/cornet_s.py` & `thingsvision-2.5.4/thingsvision/custom_models/cornet/cornet_s.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/thingsvision/custom_models/cornet/cornet_z.py` & `thingsvision-2.5.4/thingsvision/custom_models/cornet/cornet_z.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/thingsvision/custom_models/dreamsim/dreamsim.py` & `thingsvision-2.5.4/thingsvision/custom_models/dreamsim/dreamsim.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/thingsvision/custom_models/harmonization/harmonization.py` & `thingsvision-2.5.4/thingsvision/custom_models/harmonization/harmonization.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/thingsvision/custom_models/inception_ecoset.py` & `thingsvision-2.5.4/thingsvision/custom_models/inception_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/thingsvision/custom_models/openclip.py` & `thingsvision-2.5.4/thingsvision/custom_models/openclip.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/thingsvision/custom_models/resnet50_ecoset.py` & `thingsvision-2.5.4/thingsvision/custom_models/resnet50_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/thingsvision/custom_models/vgg16_ecoset.py` & `thingsvision-2.5.4/thingsvision/custom_models/vgg16_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/thingsvision/custom_models/vgg16bn_ecoset.py` & `thingsvision-2.5.4/thingsvision/custom_models/vgg16bn_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/thingsvision/thingsvision.py` & `thingsvision-2.5.4/thingsvision/thingsvision.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,20 @@
     common_parser.add_argument(
         "--device",
         type=device_type,
         default="cuda",
         help="""Device to use for the extractor. Options are 'cpu', 'cuda', or 'cuda:x', 
                 where x is the GPU index. (default: cuda)""",
     )
+    common_parser.add_argument(
+        "--model-parameters",
+        type=str,
+        default=None,
+        help="For CLIP, OpenCLIP, DreamSIM, and DINO models a model_parameters dictionary has to be defined. (default: None)",
+    )
 
     subparsers = parent_parser.add_subparsers(
         title="Subcommands",
         description="Valid subcommands are",
         help="Additional help available is available within  each subcommand",
         dest="command",
     )
@@ -90,20 +96,14 @@
         default="./features",
         help="Path to directory where features should be stored. (default: ./features)",
     )
     parser_extract.add_argument(
         "--flatten-acts", action="store_true", help="Flatten activations before saving them to disk."
     )
     parser_extract.add_argument(
-        "--model-parameters",
-        type=str,
-        default=None,
-        help="For CLIP, OpenCLIP, DreamSIM, and DINO models a model_parameters dictionary has to be defined. (default: None)",
-    )
-    parser_extract.add_argument(
         "--module-name",
         type=str,
         default="features.10",
         help="Name of the module to use for feature extraction. (default: features.10)",
     )
     parser_extract.add_argument(
         "--file-format",
@@ -155,26 +155,26 @@
         source=args.source, 
         pretrained=True,
         device=args.device,
         model_parameters=args.model_parameters,
     )
 
     if args.command == "show-model":
-        extractor.show_model()
+        print(extractor.show_model())
         sys.exit(1)
 
     if args.command == "extract-features":
         dataset = ImageDataset(
             root=args.image_root,
             out_path=args.out_path,
             backend=extractor.get_backend(),
             transforms=extractor.get_transformations(),
         )
         batches = DataLoader(
-            dataset=dataset, batch_size=args.batch_size, backend=extractor.backend
+            dataset=dataset, batch_size=args.batch_size, backend=extractor.get_backend()
         )
 
         features = extractor.extract_features(
             batches=batches,
             module_name=args.module_name,
             flatten_acts=args.flatten_acts,
             output_type=args.output_type,
```

### Comparing `thingsvision-2.5.3/thingsvision/utils/alignment/transforms.py` & `thingsvision-2.5.4/thingsvision/utils/alignment/transforms.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/thingsvision/utils/checkpointing/__init__.py` & `thingsvision-2.5.4/thingsvision/utils/checkpointing/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/thingsvision/utils/data/__init__.py` & `thingsvision-2.5.4/thingsvision/utils/data/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/thingsvision/utils/data/data_loader.py` & `thingsvision-2.5.4/thingsvision/utils/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/thingsvision/utils/data/dataset.py` & `thingsvision-2.5.4/thingsvision/utils/data/dataset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/thingsvision/utils/data/helpers.py` & `thingsvision-2.5.4/thingsvision/utils/data/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/thingsvision/utils/imagenet/__init__.py` & `thingsvision-2.5.4/thingsvision/utils/imagenet/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/thingsvision/utils/models/dino/utils.py` & `thingsvision-2.5.4/thingsvision/utils/models/dino/utils.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/thingsvision/utils/models/dino/vision_transformer.py` & `thingsvision-2.5.4/thingsvision/utils/models/dino/vision_transformer.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/thingsvision/utils/models/mae/utils.py` & `thingsvision-2.5.4/thingsvision/utils/models/mae/utils.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/thingsvision/utils/models/mae/vit_mae.py` & `thingsvision-2.5.4/thingsvision/utils/models/mae/vit_mae.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/thingsvision/utils/storing/helpers.py` & `thingsvision-2.5.4/thingsvision/utils/storing/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.3/thingsvision.egg-info/PKG-INFO` & `thingsvision-2.5.4/thingsvision.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thingsvision
-Version: 2.5.3
+Version: 2.5.4
 Summary: Extracting image features from state-of-the-art neural networks for Computer Vision made easy
 Home-page: https://github.com/ViCCo-Group/thingsvision
 Author: Lukas Muttenthaler
 Author-email: muttenthaler@cbs.mpg.de
 License: MIT License
 Keywords: feature extraction
 Classifier: Programming Language :: Python :: 3.8
@@ -88,20 +88,22 @@
 Neural networks come from different sources. With `thingsvision`, you can extract image representations of all models from:
 - [torchvision](https://pytorch.org/vision/0.8/models.html)
 - [Keras](https://www.tensorflow.org/api_docs/python/tf/keras/applications)
 - [timm](https://github.com/rwightman/pytorch-image-models)
 - `ssl` (self-supervised learning models)
   - `simclr-rn50`, `mocov2-rn50`, `barlowtwins-rn50`, `pirl-rn50`
   - `jigsaw-rn50`, `rotnet-rn50`, `swav-rn50`, `vicreg-rn50`
-  - `dino-rn50`, `dino-xcit-{small/medium}-{12/24}-p{8/16}`, `dino-vit-{tiny/small/base}-p{8/16}`, `dinov2-vit-{small/base/large/giant}-p14`
+  - `dino-rn50`, `dino-xcit-{small/medium}-{12/24}-p{8/16}`
+  - `dino-vit-{tiny/small/base}-p{8/16}`
+  - `dinov2-vit-{small/base/large/giant}-p14`
   - `mae-vit-{base/large}-p16`, `mae-vit-huge-p14`<br>
 - [OpenCLIP](https://github.com/mlfoundations/open_clip) models (CLIP trained on LAION-{400M/2B/5B})
 - [CLIP](https://github.com/openai/CLIP) models (CLIP trained on WiT)
 - a few custom models (Alexnet, VGG-16, Resnet50, and Inception_v3) trained on [Ecoset](https://www.pnas.org/doi/10.1073/pnas.2011417118) rather than ImageNet and one Alexnet model pretrained on ImageNet and fine-tuned on [SalObjSub](https://cs-people.bu.edu/jmzhang/sos.html)<br>
-- each of the many [CORnet](https://github.com/dicarlolab/CORnet) versions
+- each of the many [CORnet](https://github.com/dicarlolab/CORnet) versions (recurrent vision models)
 - [Harmonization](https://arxiv.org/abs/2211.04533) models (see [Harmonization repo](https://github.com/serre-lab/harmonization)). The default variant is `ViT_B16`. Other available models are `ResNet50`, `VGG16`, `EfficientNetB0`, `tiny_ConvNeXT`, `tiny_MaxViT`, and `LeViT_small`<br> 
 - [DreamSim](https://dreamsim-nights.github.io/) models  (see [DreamSim repo](https://github.com/ssundaram21/dreamsim)). The default variant is `open_clip_vitb32`. Other available models are `clip_vitb32`, `dino_vitb16`, and an `ensemble`. See the [docs](https://vicco-group.github.io/thingsvision/AvailableModels.html#dreamsim) for more information
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 <!-- Getting Started -->
@@ -155,15 +157,15 @@
 - `thingsvision show-model`
 - `thingsvision extract-features`
 
 Example calls might look as follows:
 
 ```bash
 thingsvision show-model --model-name "alexnet" --source "torchvision"
-thingsvision extract_features --image-root "./data" --model-name "alexnet" --module-name "features.10" --batch-size 32 --device "cuda" --source "torchvision" --file-format "npy" --out-path "./features"
+thingsvision extract-features --image-root "./data" --model-name "alexnet" --module-name "features.10" --batch-size 32 --device "cuda" --source "torchvision" --file-format "npy" --out-path "./features"
 ```
 
 See `thingsvision show-model -h` and `thingsvision extract-features -h` for a list of all possible arguments. Note that the CLI provides just the basic extraction functionalities but is probably enough for most users that don't want to dive too deep into various models and modules. If you need more fine-grained control over the extraction itself, we recommend to use the python package directly and write your own Python script.
 
 #### Python commands
 
 To do this start by importing all the necessary components and instantiating a `thingsvision` extractor. Here we're using `CLIP` from the official clip repo as the model to extract features from and also load the model to GPU for faster inference,
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thingsvision Version: 2.5.3 Summary: Extracting
+Metadata-Version: 2.1 Name: thingsvision Version: 2.5.4 Summary: Extracting
 image features from state-of-the-art neural networks for Computer Vision made
 easy Home-page: https://github.com/ViCCo-Group/thingsvision Author: Lukas
 Muttenthaler Author-email: muttenthaler@cbs.mpg.de License: MIT License
 Keywords: feature extraction Classifier: Programming Language :: Python :: 3.8
 Classifier: Natural Language :: English Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Requires-Python:
 >=3.8 Description-Content-Type: text/markdown License-File: LICENSE
@@ -42,29 +42,29 @@
 ### :file_cabinet: Model collection Neural networks come from different
 sources. With `thingsvision`, you can extract image representations of all
 models from: - [torchvision](https://pytorch.org/vision/0.8/models.html) -
 [Keras](https://www.tensorflow.org/api_docs/python/tf/keras/applications) -
 [timm](https://github.com/rwightman/pytorch-image-models) - `ssl` (self-
 supervised learning models) - `simclr-rn50`, `mocov2-rn50`, `barlowtwins-rn50`,
 `pirl-rn50` - `jigsaw-rn50`, `rotnet-rn50`, `swav-rn50`, `vicreg-rn50` - `dino-
-rn50`, `dino-xcit-{small/medium}-{12/24}-p{8/16}`, `dino-vit-{tiny/small/base}-
-p{8/16}`, `dinov2-vit-{small/base/large/giant}-p14` - `mae-vit-{base/large}-
-p16`, `mae-vit-huge-p14`
+rn50`, `dino-xcit-{small/medium}-{12/24}-p{8/16}` - `dino-vit-{tiny/small/
+base}-p{8/16}` - `dinov2-vit-{small/base/large/giant}-p14` - `mae-vit-{base/
+large}-p16`, `mae-vit-huge-p14`
 - [OpenCLIP](https://github.com/mlfoundations/open_clip) models (CLIP trained
 on LAION-{400M/2B/5B}) - [CLIP](https://github.com/openai/CLIP) models (CLIP
 trained on WiT) - a few custom models (Alexnet, VGG-16, Resnet50, and
 Inception_v3) trained on [Ecoset](https://www.pnas.org/doi/10.1073/
 pnas.2011417118) rather than ImageNet and one Alexnet model pretrained on
 ImageNet and fine-tuned on [SalObjSub](https://cs-people.bu.edu/jmzhang/
 sos.html)
-- each of the many [CORnet](https://github.com/dicarlolab/CORnet) versions -
-[Harmonization](https://arxiv.org/abs/2211.04533) models (see [Harmonization
-repo](https://github.com/serre-lab/harmonization)). The default variant is
-`ViT_B16`. Other available models are `ResNet50`, `VGG16`, `EfficientNetB0`,
-`tiny_ConvNeXT`, `tiny_MaxViT`, and `LeViT_small`
+- each of the many [CORnet](https://github.com/dicarlolab/CORnet) versions
+(recurrent vision models) - [Harmonization](https://arxiv.org/abs/2211.04533)
+models (see [Harmonization repo](https://github.com/serre-lab/harmonization)).
+The default variant is `ViT_B16`. Other available models are `ResNet50`,
+`VGG16`, `EfficientNetB0`, `tiny_ConvNeXT`, `tiny_MaxViT`, and `LeViT_small`
 - [DreamSim](https://dreamsim-nights.github.io/) models (see [DreamSim repo]
 (https://github.com/ssundaram21/dreamsim)). The default variant is
 `open_clip_vitb32`. Other available models are `clip_vitb32`, `dino_vitb16`,
 and an `ensemble`. See the [docs](https://vicco-group.github.io/thingsvision/
 AvailableModels.html#dreamsim) for more information
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## :running: Getting Started ### :computer: Setting up your environment ####
@@ -97,15 +97,15 @@
 ### :mag: Basic usage #### Command Line Interface (CLI) `thingsvision` was
 designed to simplify feature extraction. If you have some folder of images
 (e.g., `./images`) and want to extract features for each of these images
 without opening a Jupyter Notebook instance or writing a Python script, it's
 probably easiest to use our CLI. The interface includes two options, -
 `thingsvision show-model` - `thingsvision extract-features` Example calls might
 look as follows: ```bash thingsvision show-model --model-name "alexnet" --
-source "torchvision" thingsvision extract_features --image-root "./data" --
+source "torchvision" thingsvision extract-features --image-root "./data" --
 model-name "alexnet" --module-name "features.10" --batch-size 32 --device
 "cuda" --source "torchvision" --file-format "npy" --out-path "./features" ```
 See `thingsvision show-model -h` and `thingsvision extract-features -h` for a
 list of all possible arguments. Note that the CLI provides just the basic
 extraction functionalities but is probably enough for most users that don't
 want to dive too deep into various models and modules. If you need more fine-
 grained control over the extraction itself, we recommend to use the python
```

### Comparing `thingsvision-2.5.3/thingsvision.egg-info/SOURCES.txt` & `thingsvision-2.5.4/thingsvision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

