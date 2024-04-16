# Comparing `tmp/ego4d-1.7.1.tar.gz` & `tmp/ego4d-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ego4d-1.7.1.tar", last modified: Fri Mar 29 02:54:29 2024, max compression
+gzip compressed data, was "ego4d-1.7.2.tar", last modified: Tue Apr 16 20:04:20 2024, max compression
```

## Comparing `ego4d-1.7.1.tar` & `ego4d-1.7.2.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxrwxr-x   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-03-29 02:54:29.154527 ego4d-1.7.1/
--rw-r--r--   0 miguelmartin (1185200870) miguelmartin (1185200870)      293 2024-03-29 02:54:29.153059 ego4d-1.7.1/PKG-INFO
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     6349 2024-03-29 02:32:12.000000 ego4d-1.7.1/README.md
-drwxrwxr-x   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-03-29 02:54:28.847176 ego4d-1.7.1/ego4d/
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)       95 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/__init__.py
-drwxrwxr-x   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-03-29 02:54:28.920723 ego4d-1.7.1/ego4d/cli/
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)       95 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/cli/__init__.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     8264 2024-02-29 01:38:22.000000 ego4d-1.7.1/ego4d/cli/cli.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)    11147 2024-03-26 02:59:01.000000 ego4d-1.7.1/ego4d/cli/config.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     5166 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/cli/config_test.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)    14827 2024-02-29 01:38:22.000000 ego4d-1.7.1/ego4d/cli/download.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)      181 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/cli/e2e_test.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)      605 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/cli/integrity.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     7966 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/cli/manifest.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     6175 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/cli/manifest_test.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)      650 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/cli/progressbar.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)      994 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/cli/s3path.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)      954 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/cli/s3path_test.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)      752 2024-03-13 03:26:30.000000 ego4d-1.7.1/ego4d/cli/universities.py
-drwxrwxr-x   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-03-29 02:54:28.926010 ego4d-1.7.1/ego4d/egoexo/
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-02-29 04:07:27.000000 ego4d-1.7.1/ego4d/egoexo/__init__.py
-drwxrwxr-x   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-03-29 02:54:28.931720 ego4d-1.7.1/ego4d/egoexo/download/
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-02-29 04:07:27.000000 ego4d-1.7.1/ego4d/egoexo/download/__init__.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)      356 2024-03-27 16:24:45.000000 ego4d-1.7.1/ego4d/egoexo/download/cli.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     1290 2024-03-26 02:59:01.000000 ego4d-1.7.1/ego4d/egoexo/expert_commentary.py
-drwxrwxr-x   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-03-29 02:54:28.966568 ego4d-1.7.1/ego4d/features/
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/features/__init__.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/features/audio.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)    10748 2024-03-27 16:24:45.000000 ego4d-1.7.1/ego4d/features/config.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     9457 2024-03-27 00:19:38.000000 ego4d-1.7.1/ego4d/features/dataset.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)    10748 2024-02-29 01:38:22.000000 ego4d-1.7.1/ego4d/features/extract_features.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     6245 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/features/inference.py
-drwxrwxr-x   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-03-29 02:54:28.994287 ego4d-1.7.1/ego4d/features/models/
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/features/models/__init__.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)      247 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/features/models/common.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     1988 2024-03-27 00:19:38.000000 ego4d-1.7.1/ego4d/features/models/maws.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     1806 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/features/models/mel_spectrogram.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     2147 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/features/models/mvit.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     2271 2024-03-27 00:19:38.000000 ego4d-1.7.1/ego4d/features/models/omnivore.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     2857 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/features/models/slowfast.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     2489 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/features/models/speechbrain_asr.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     3229 2024-03-27 00:19:38.000000 ego4d-1.7.1/ego4d/features/profile_extract.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     8628 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/features/slurm.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     1832 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/features/visualize_dataloader.py
-drwxrwxr-x   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-03-29 02:54:29.006080 ego4d-1.7.1/ego4d/internal/
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/internal/__init__.py
-drwxrwxr-x   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-03-29 02:54:29.012561 ego4d-1.7.1/ego4d/internal/colmap/
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/internal/colmap/__init__.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)    21202 2024-02-29 01:38:22.000000 ego4d-1.7.1/ego4d/internal/colmap/preprocess.py
-drwxrwxr-x   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-03-29 02:54:29.029957 ego4d-1.7.1/ego4d/internal/download/
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-02-29 04:07:27.000000 ego4d-1.7.1/ego4d/internal/download/__init__.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)    19246 2024-03-29 02:46:52.000000 ego4d-1.7.1/ego4d/internal/download/cli.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     1351 2024-03-29 02:32:12.000000 ego4d-1.7.1/ego4d/internal/download/manifest.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)    33101 2024-03-29 02:47:24.000000 ego4d-1.7.1/ego4d/internal/download/manifest_gen.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     3584 2024-03-27 16:24:45.000000 ego4d-1.7.1/ego4d/internal/downscale.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     7481 2024-03-29 02:47:41.000000 ego4d-1.7.1/ego4d/internal/s3.py
-drwxrwxr-x   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-03-29 02:54:29.058786 ego4d-1.7.1/ego4d/internal/validation/
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/internal/validation/__init__.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     1503 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/internal/validation/cli.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     6717 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/internal/validation/config.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     2782 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/internal/validation/credential_s3.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     5548 2024-02-29 01:38:22.000000 ego4d-1.7.1/ego4d/internal/validation/ffmpeg_utils.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)    22398 2024-03-26 02:59:01.000000 ego4d-1.7.1/ego4d/internal/validation/manifest.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)    66771 2024-03-26 02:59:01.000000 ego4d-1.7.1/ego4d/internal/validation/validate.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     5572 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/internal/validation/validate_test.py
-drwxrwxr-x   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-03-29 02:54:29.077813 ego4d-1.7.1/ego4d/research/
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/research/__init__.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     6490 2024-03-26 03:15:57.000000 ego4d-1.7.1/ego4d/research/chunk.py
-drwxrwxr-x   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-03-29 02:54:29.110835 ego4d-1.7.1/ego4d/research/clep/
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/research/clep/__init__.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     2326 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/research/clep/config.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     6775 2024-03-26 02:59:01.000000 ego4d-1.7.1/ego4d/research/clep/dataset.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     1266 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/research/clep/model.py
-drwxrwxr-x   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-03-29 02:54:29.134451 ego4d-1.7.1/ego4d/research/clep/preprocess/
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/research/clep/preprocess/__init__.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     4563 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/research/clep/preprocess/cc.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     3217 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/research/clep/preprocess/charades.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     1464 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/research/clep/preprocess/common.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     6177 2024-03-27 00:19:38.000000 ego4d-1.7.1/ego4d/research/clep/preprocess/ego4d_data.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     4674 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/research/clep/preprocess/kinetics.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     1324 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/research/clep/run_preprocess.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)    10763 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/research/clep/train.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     2598 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/research/clep/utils.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     4067 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/research/clep/val.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     1199 2023-10-24 20:27:36.000000 ego4d-1.7.1/ego4d/research/common.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     5699 2024-03-27 00:19:38.000000 ego4d-1.7.1/ego4d/research/dataset.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     8855 2024-03-26 03:15:57.000000 ego4d-1.7.1/ego4d/research/readers.py
-drwxrwxr-x   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-03-29 02:54:29.144189 ego4d-1.7.1/ego4d/research/util/
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-02-29 01:38:22.000000 ego4d-1.7.1/ego4d/research/util/__init__.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     5038 2024-02-29 01:38:22.000000 ego4d-1.7.1/ego4d/research/util/lzstring.py
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     1486 2024-02-29 01:38:22.000000 ego4d-1.7.1/ego4d/research/util/masks.py
-drwxrwxr-x   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-03-29 02:54:29.148601 ego4d-1.7.1/ego4d.egg-info/
--rw-r--r--   0 miguelmartin (1185200870) miguelmartin (1185200870)      293 2024-03-29 02:54:28.000000 ego4d-1.7.1/ego4d.egg-info/PKG-INFO
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     2511 2024-03-29 02:54:28.000000 ego4d-1.7.1/ego4d.egg-info/SOURCES.txt
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)        1 2024-03-29 02:54:28.000000 ego4d-1.7.1/ego4d.egg-info/dependency_links.txt
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)      199 2024-03-29 02:54:28.000000 ego4d-1.7.1/ego4d.egg-info/entry_points.txt
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)       41 2024-03-29 02:54:28.000000 ego4d-1.7.1/ego4d.egg-info/requires.txt
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)        6 2024-03-29 02:54:28.000000 ego4d-1.7.1/ego4d.egg-info/top_level.txt
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)       83 2023-10-24 20:27:36.000000 ego4d-1.7.1/pyproject.toml
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)      107 2024-03-29 02:54:29.157818 ego4d-1.7.1/setup.cfg
--rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)      887 2024-03-29 02:35:31.000000 ego4d-1.7.1/setup.py
+drwxrwxr-x   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-04-16 20:04:20.306816 ego4d-1.7.2/
+-rw-r--r--   0 miguelmartin (1185200870) miguelmartin (1185200870)      293 2024-04-16 20:04:20.305153 ego4d-1.7.2/PKG-INFO
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     6349 2024-03-29 02:32:12.000000 ego4d-1.7.2/README.md
+drwxrwxr-x   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-04-16 20:04:19.920993 ego4d-1.7.2/ego4d/
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)       95 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/__init__.py
+drwxrwxr-x   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-04-16 20:04:20.010265 ego4d-1.7.2/ego4d/cli/
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)       95 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/cli/__init__.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     8264 2024-02-29 01:38:22.000000 ego4d-1.7.2/ego4d/cli/cli.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)    11147 2024-03-26 02:59:01.000000 ego4d-1.7.2/ego4d/cli/config.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     5166 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/cli/config_test.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)    14827 2024-02-29 01:38:22.000000 ego4d-1.7.2/ego4d/cli/download.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)      181 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/cli/e2e_test.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)      605 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/cli/integrity.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     7966 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/cli/manifest.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     6175 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/cli/manifest_test.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)      650 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/cli/progressbar.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)      994 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/cli/s3path.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)      954 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/cli/s3path_test.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)      752 2024-03-13 03:26:30.000000 ego4d-1.7.2/ego4d/cli/universities.py
+drwxrwxr-x   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-04-16 20:04:20.018556 ego4d-1.7.2/ego4d/egoexo/
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-02-29 04:07:27.000000 ego4d-1.7.2/ego4d/egoexo/__init__.py
+drwxrwxr-x   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-04-16 20:04:20.026859 ego4d-1.7.2/ego4d/egoexo/download/
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-02-29 04:07:27.000000 ego4d-1.7.2/ego4d/egoexo/download/__init__.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)      356 2024-03-27 16:24:45.000000 ego4d-1.7.2/ego4d/egoexo/download/cli.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     1290 2024-03-26 02:59:01.000000 ego4d-1.7.2/ego4d/egoexo/expert_commentary.py
+drwxrwxr-x   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-04-16 20:04:20.068322 ego4d-1.7.2/ego4d/features/
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/features/__init__.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/features/audio.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)    10748 2024-03-27 16:24:45.000000 ego4d-1.7.2/ego4d/features/config.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     9457 2024-03-27 00:19:38.000000 ego4d-1.7.2/ego4d/features/dataset.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)    10748 2024-02-29 01:38:22.000000 ego4d-1.7.2/ego4d/features/extract_features.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     6245 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/features/inference.py
+drwxrwxr-x   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-04-16 20:04:20.108695 ego4d-1.7.2/ego4d/features/models/
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/features/models/__init__.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)      247 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/features/models/common.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     1988 2024-03-27 00:19:38.000000 ego4d-1.7.2/ego4d/features/models/maws.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     1806 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/features/models/mel_spectrogram.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     2147 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/features/models/mvit.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     2271 2024-03-27 00:19:38.000000 ego4d-1.7.2/ego4d/features/models/omnivore.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     2857 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/features/models/slowfast.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     2489 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/features/models/speechbrain_asr.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     3229 2024-03-27 00:19:38.000000 ego4d-1.7.2/ego4d/features/profile_extract.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     8628 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/features/slurm.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     1832 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/features/visualize_dataloader.py
+drwxrwxr-x   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-04-16 20:04:20.122561 ego4d-1.7.2/ego4d/internal/
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/internal/__init__.py
+drwxrwxr-x   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-04-16 20:04:20.132367 ego4d-1.7.2/ego4d/internal/colmap/
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/internal/colmap/__init__.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)    21202 2024-02-29 01:38:22.000000 ego4d-1.7.2/ego4d/internal/colmap/preprocess.py
+drwxrwxr-x   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-04-16 20:04:20.149728 ego4d-1.7.2/ego4d/internal/download/
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-02-29 04:07:27.000000 ego4d-1.7.2/ego4d/internal/download/__init__.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)    19856 2024-04-16 20:03:51.000000 ego4d-1.7.2/ego4d/internal/download/cli.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     1351 2024-03-29 04:14:59.000000 ego4d-1.7.2/ego4d/internal/download/manifest.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)    33106 2024-04-16 20:03:51.000000 ego4d-1.7.2/ego4d/internal/download/manifest_gen.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     3584 2024-03-27 16:24:45.000000 ego4d-1.7.2/ego4d/internal/downscale.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     7481 2024-03-29 04:14:59.000000 ego4d-1.7.2/ego4d/internal/s3.py
+drwxrwxr-x   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-04-16 20:04:20.187703 ego4d-1.7.2/ego4d/internal/validation/
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/internal/validation/__init__.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     1503 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/internal/validation/cli.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     6717 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/internal/validation/config.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     2782 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/internal/validation/credential_s3.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     5548 2024-02-29 01:38:22.000000 ego4d-1.7.2/ego4d/internal/validation/ffmpeg_utils.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)    22398 2024-03-26 02:59:01.000000 ego4d-1.7.2/ego4d/internal/validation/manifest.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)    66771 2024-04-05 01:12:56.000000 ego4d-1.7.2/ego4d/internal/validation/validate.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     5572 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/internal/validation/validate_test.py
+drwxrwxr-x   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-04-16 20:04:20.209744 ego4d-1.7.2/ego4d/research/
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/research/__init__.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     6971 2024-04-16 20:03:51.000000 ego4d-1.7.2/ego4d/research/chunk.py
+drwxrwxr-x   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-04-16 20:04:20.251016 ego4d-1.7.2/ego4d/research/clep/
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/research/clep/__init__.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     2326 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/research/clep/config.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     6775 2024-04-05 01:13:08.000000 ego4d-1.7.2/ego4d/research/clep/dataset.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     1266 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/research/clep/model.py
+drwxrwxr-x   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-04-16 20:04:20.279699 ego4d-1.7.2/ego4d/research/clep/preprocess/
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/research/clep/preprocess/__init__.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     4563 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/research/clep/preprocess/cc.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     3217 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/research/clep/preprocess/charades.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     1464 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/research/clep/preprocess/common.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     6177 2024-03-27 00:19:38.000000 ego4d-1.7.2/ego4d/research/clep/preprocess/ego4d_data.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     4674 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/research/clep/preprocess/kinetics.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     1324 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/research/clep/run_preprocess.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)    10763 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/research/clep/train.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     2598 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/research/clep/utils.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     4067 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/research/clep/val.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     1199 2023-10-24 20:27:36.000000 ego4d-1.7.2/ego4d/research/common.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     5699 2024-03-27 00:19:38.000000 ego4d-1.7.2/ego4d/research/dataset.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     8855 2024-03-26 03:15:57.000000 ego4d-1.7.2/ego4d/research/readers.py
+drwxrwxr-x   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-04-16 20:04:20.294063 ego4d-1.7.2/ego4d/research/util/
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-02-29 01:38:22.000000 ego4d-1.7.2/ego4d/research/util/__init__.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     5038 2024-02-29 01:38:22.000000 ego4d-1.7.2/ego4d/research/util/lzstring.py
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     1486 2024-02-29 01:38:22.000000 ego4d-1.7.2/ego4d/research/util/masks.py
+drwxrwxr-x   0 miguelmartin (1185200870) miguelmartin (1185200870)        0 2024-04-16 20:04:20.299817 ego4d-1.7.2/ego4d.egg-info/
+-rw-r--r--   0 miguelmartin (1185200870) miguelmartin (1185200870)      293 2024-04-16 20:04:19.000000 ego4d-1.7.2/ego4d.egg-info/PKG-INFO
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)     2511 2024-04-16 20:04:19.000000 ego4d-1.7.2/ego4d.egg-info/SOURCES.txt
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)        1 2024-04-16 20:04:19.000000 ego4d-1.7.2/ego4d.egg-info/dependency_links.txt
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)      199 2024-04-16 20:04:19.000000 ego4d-1.7.2/ego4d.egg-info/entry_points.txt
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)       41 2024-04-16 20:04:19.000000 ego4d-1.7.2/ego4d.egg-info/requires.txt
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)        6 2024-04-16 20:04:19.000000 ego4d-1.7.2/ego4d.egg-info/top_level.txt
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)       83 2023-10-24 20:27:36.000000 ego4d-1.7.2/pyproject.toml
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)      107 2024-04-16 20:04:20.310862 ego4d-1.7.2/setup.cfg
+-rw-rw-r--   0 miguelmartin (1185200870) miguelmartin (1185200870)      887 2024-04-16 20:03:51.000000 ego4d-1.7.2/setup.py
```

### Comparing `ego4d-1.7.1/README.md` & `ego4d-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/cli/cli.py` & `ego4d-1.7.2/ego4d/cli/cli.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/cli/config.py` & `ego4d-1.7.2/ego4d/cli/config.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/cli/config_test.py` & `ego4d-1.7.2/ego4d/cli/config_test.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/cli/download.py` & `ego4d-1.7.2/ego4d/cli/download.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/cli/integrity.py` & `ego4d-1.7.2/ego4d/cli/integrity.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/cli/manifest.py` & `ego4d-1.7.2/ego4d/cli/manifest.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/cli/manifest_test.py` & `ego4d-1.7.2/ego4d/cli/manifest_test.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/cli/progressbar.py` & `ego4d-1.7.2/ego4d/cli/progressbar.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/cli/s3path.py` & `ego4d-1.7.2/ego4d/cli/s3path.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/cli/s3path_test.py` & `ego4d-1.7.2/ego4d/cli/s3path_test.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/cli/universities.py` & `ego4d-1.7.2/ego4d/cli/universities.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/egoexo/expert_commentary.py` & `ego4d-1.7.2/ego4d/egoexo/expert_commentary.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/features/config.py` & `ego4d-1.7.2/ego4d/features/config.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/features/dataset.py` & `ego4d-1.7.2/ego4d/features/dataset.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/features/extract_features.py` & `ego4d-1.7.2/ego4d/features/extract_features.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/features/inference.py` & `ego4d-1.7.2/ego4d/features/inference.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/features/models/maws.py` & `ego4d-1.7.2/ego4d/features/models/maws.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/features/models/mel_spectrogram.py` & `ego4d-1.7.2/ego4d/features/models/mel_spectrogram.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/features/models/mvit.py` & `ego4d-1.7.2/ego4d/features/models/mvit.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/features/models/omnivore.py` & `ego4d-1.7.2/ego4d/features/models/omnivore.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/features/models/slowfast.py` & `ego4d-1.7.2/ego4d/features/models/slowfast.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/features/models/speechbrain_asr.py` & `ego4d-1.7.2/ego4d/features/models/speechbrain_asr.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/features/profile_extract.py` & `ego4d-1.7.2/ego4d/features/profile_extract.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/features/slurm.py` & `ego4d-1.7.2/ego4d/features/slurm.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/features/visualize_dataloader.py` & `ego4d-1.7.2/ego4d/features/visualize_dataloader.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/internal/colmap/preprocess.py` & `ego4d-1.7.2/ego4d/internal/colmap/preprocess.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/internal/download/cli.py` & `ego4d-1.7.2/ego4d/internal/download/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import argparse
 import os
 import sys
 import threading
 import traceback
-from collections import defaultdict
 from concurrent.futures import ThreadPoolExecutor
 from typing import Callable, List, Optional, Tuple, TypeVar
 
 from ego4d.cli.progressbar import DownloadProgressBar
 from ego4d.cli.universities import UNIV_TO_BUCKET
 
 from ego4d.internal.download.manifest import (
@@ -241,14 +240,28 @@
     for part in tqdm(parts):
         manifest_path = _s3_path_join(_s3_path_join(release_dir, part), "manifest.json")
         if not pathmgr.exists(manifest_path):
             part_errs.append(part)
             continue
 
         ms = manifest_loads(pathmgr.open(manifest_path).read())
+        valid_benchmark_names = {b for m in ms for b in m.benchmarks or []}
+        invalid_benchmarks = (
+            args.benchmarks - valid_benchmark_names if args.benchmarks else set()
+        )
+        if len(invalid_benchmarks) > 0:
+            print(f"Provided invalid benchmarks: {invalid_benchmarks}")
+            print("Valid benchmark names include: ")
+            print()
+            for b in valid_benchmark_names:
+                print(b)
+            print()
+            print("Quitting ...")
+            sys.exit(3)
+
         for m in ms:
             num_paths += len(m.paths)
             if not _manifest_ok(m, args):
                 continue
 
             all_paths.extend([p for p in m.paths if _path_ok(p, args)])
     print("Done", flush=True)
@@ -345,15 +358,15 @@
     )
     if len(curr_stats_failures) > 0:
         print(f"WARN: {len(curr_stats_failures)} failed to stat")
 
     ps_to_dl = {
         path: size
         for path, size in path_size_pairs
-        if (path, size) not in existing_paths
+        if (path, size) not in existing_paths and size > 0
     }
     if len(ps_to_dl) == 0 and not args.force:
         print("Everything has been downloaded. Bye.")
         sys.exit(0)
 
     if args.force:
         print("Forcing everything to be re-downloaded ...")
@@ -375,49 +388,50 @@
     else:
         confirm = True
 
     if not confirm:
         print("Aborting...")
         sys.exit(0)
 
-    print("Preparing output directories ...")
-    all_out_dirs = {
-        os.path.join(out_dir, os.path.dirname(x.relative_path)) for x in all_paths
-    }
-    for x in tqdm(all_out_dirs):
-        os.makedirs(x, exist_ok=True)
-
     if args.delete:
         print("Scanning for files to delete ...")
         files_that_exist = []
         for dirpath, _, filenames in os.walk(out_dir):
             files_that_exist.extend([os.path.join(dirpath, f) for f in filenames])
 
         files_that_exist = set(files_that_exist)
         files_to_delete = files_that_exist - {
             os.path.join(out_dir, x[0].relative_path) for x in path_size_pairs
         }
-        response = input(
-            f"Will delete: {len(files_to_delete)} files (there is {len(files_that_exist)} total files) "
-            f"Continue? (y/[n]): "
-        )
-        if not delete_yes:
-            if response.lower() in ["yes", "y"]:
-                confirm = True
+        if len(files_to_delete) > 0:
+            response = input(
+                f"Will delete: {len(files_to_delete)} files (there is {len(files_that_exist)} total files) "
+                f"Continue? (y/[n]): "
+            )
+            if not delete_yes:
+                if response.lower() in ["yes", "y"]:
+                    confirm = True
+                else:
+                    confirm = False
             else:
-                confirm = False
-        else:
-            confirm = True
+                confirm = True
+
+            if not confirm:
+                print("Aborting...")
+                sys.exit(0)
 
-        if not confirm:
-            print("Aborting...")
-            sys.exit(0)
+            for f in tqdm(files_to_delete):
+                os.remove(f)
 
-        for f in tqdm(files_to_delete):
-            os.remove(f)
+    print("Preparing output directories ...")
+    all_out_dirs = {
+        os.path.join(out_dir, os.path.dirname(x.relative_path)) for x in all_paths
+    }
+    for x in tqdm(all_out_dirs):
+        os.makedirs(x, exist_ok=True)
 
     print("Downloading ...")
     assert all(size is not None for size in ps_to_dl.values())
     paths_to_fetch = [
         (path, size) for path, size in ps_to_dl.items() if size is not None
     ]
     total_bytes_to_fetch = sum(size for _, size in paths_to_fetch)
```

### Comparing `ego4d-1.7.1/ego4d/internal/download/manifest.py` & `ego4d-1.7.2/ego4d/internal/download/manifest.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/internal/download/manifest_gen.py` & `ego4d-1.7.2/ego4d/internal/download/manifest_gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -623,16 +623,19 @@
                 "camera_pose": [],
             },
             "take_uid_as_key": True,
         },
     }
     if not dev_release:
         egopose_base_dir = os.path.join(release_dir, "annotations/ego_pose/")
-        for split in ["train", "val"]:
+        for split in ["train", "val", "test"]:
             for part in ["body", "hand", "camera_pose"]:
+                if part in ("body", "hand") and split == "test":
+                    continue
+
                 subdir = os.path.join(egopose_base_dir, split, part)
                 print(subdir)
 
                 annotation_files = []
 
                 # go over each potential manifest --part
                 for manifest_key, metadata in egopose_part_subdirs.items():
@@ -843,15 +846,15 @@
         "capture_point_cloud": "[Point clouds](data/mps/#point-clouds) for each capture",
         "downscaled_takes/448": "[Downscaled takes](data/downscaled_takes/) at 448px on the shortest side",
         "features/omnivore_video": "Omnivore video [features](/data/features)",
         "features/maws_clip_2b": "[MAWS CLIP](https://github.com/facebookresearch/maws) ([ViT-2b](https://github.com/facebookresearch/maws?tab=readme-ov-file#maws-pretrained-models)) [features](/data/features) for each frame of video",
         "ego_pose_pseudo_gt": "Pseudo-ground truth data for [Ego Pose](/annotations/ego_pose/)",
         "expert_commentary": "[Commentaries](/annotations/expert_commentary) for each expert (audio recordings)",
         "all": "All data within the release (you can use `--parts all`) ",
-        "default": "The default set of data in the release",
+        "default": "The default set of data in the release (you can use `--parts default` or provide no parts)",
     }
 
     manifests_by_name = {}
     for m_name in tqdm(manifests):
         m_path = os.path.join(release_dir, m_name, "manifest.json")
         m = manifest_loads(pathmgr.open(m_path).read())
         manifests_by_name[m_name] = m
@@ -891,13 +894,11 @@
     print("| -----|-----------|-------------|")
     for k, v in file_size_by_mname.items():
         assert k in manifest_descs
         size = v / 10**9
         if k in default:
             print(f"| **{k}** | {size:.3f} | {manifest_descs[k]} |")
         else:
-            print(f"| {k} | {size:.3f} | {v} |")
-    print(f"| *all* | {all_file_size/10**9:.3f} | {manifest_descs['all']} |")
-    print(f"| **default ** | {default_size/10**9:.3f} | {manifest_descs['default']} |")
+            print(f"| {k} | {size:.3f} | {manifest_descs[k]} |")
 
 
 print_manifest_stats(release_dir)
```

### Comparing `ego4d-1.7.1/ego4d/internal/downscale.py` & `ego4d-1.7.2/ego4d/internal/downscale.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/internal/s3.py` & `ego4d-1.7.2/ego4d/internal/s3.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/internal/validation/cli.py` & `ego4d-1.7.2/ego4d/internal/validation/cli.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/internal/validation/config.py` & `ego4d-1.7.2/ego4d/internal/validation/config.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/internal/validation/credential_s3.py` & `ego4d-1.7.2/ego4d/internal/validation/credential_s3.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/internal/validation/ffmpeg_utils.py` & `ego4d-1.7.2/ego4d/internal/validation/ffmpeg_utils.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/internal/validation/manifest.py` & `ego4d-1.7.2/ego4d/internal/validation/manifest.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/internal/validation/validate.py` & `ego4d-1.7.2/ego4d/internal/validation/validate.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/internal/validation/validate_test.py` & `ego4d-1.7.2/ego4d/internal/validation/validate_test.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/research/chunk.py` & `ego4d-1.7.2/ego4d/research/chunk.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,32 +28,37 @@
     audio_frames_pts: Optional[List[int]]
 
     video_frames_sec: List[Fraction]
     audio_frames_sec: Optional[List[Fraction]]
 
     video_timebase: Fraction
     audio_timebase: Fraction
+    audio_sample_rate: int
+    video_fps: Fraction
 
 
 def split_av_frames(
     video_path: str,
     window_size_sec: int = 5,
-    subsample_n_frames: Optional[int] = 30,  # 6 fps
+    subsample_n_frames: Optional[int] = None,
     limit: int = -1,
 ) -> Iterator[VideoChunk]:
     with av.open(video_path) as container:
         has_audio = len(container.streams.audio) > 0
         has_audio = False
 
         streams_to_decode = {"video": 0}
         video_tb = container.streams.video[0].time_base
+        video_fps = container.streams.video[0].framerate
         audio_tb = None
+        audio_sample_rate = None
         if has_audio:
             streams_to_decode["audio"] = 0
             audio_tb = container.streams.audio[0].time_base
+            audio_sample_rate = container.streams.audio[0].sample_rate
 
         vf_buffer = {}
         af_buffer = {}
         curr_window_start_sec = 0
         curr_window_end_sec = curr_window_start_sec + window_size_sec
         i = 0
         for frame in container.decode(**streams_to_decode):
@@ -106,14 +111,16 @@
                         audio_frames_sec=(
                             [x * audio_tb for x in af_frames_pts]
                             if af_frames_pts is not None
                             else None
                         ),
                         video_timebase=video_tb,
                         audio_timebase=audio_tb,
+                        video_fps=video_fps,
+                        audio_sample_rate=audio_sample_rate,
                     )
                 vf_buffer = {}
                 af_buffer = {}
             else:
                 if t_pts_sec < curr_window_start_sec:
                     raise AssertionError("packets from previous window")
 
@@ -161,14 +168,17 @@
         ),
         "has_audio": has_audio,
         "num_frames": chunk.video_frames.shape[0],
         "num_audio_frames": chunk.audio_frames.shape[0] if has_audio else 0,
         "frame_height": chunk.video_frames.shape[2],
         "frame_width": chunk.video_frames.shape[3],
         "is_audio_mono": is_audio_mono,
+        "video_fps_numeratator": chunk.video_fps.numerator,
+        "video_fps_denom": chunk.video_fps.denominator,
+        "audio_sample_rate": chunk.audio_sample_rate,
     }
     json.dump(metadata, pathmgr.open(metadata_path, "w"), indent=2)
 
     # TODO: is torch.save better?
     np.save(pathmgr.open(video_path, "wb"), chunk.video_frames)
     if has_audio:
         np.save(pathmgr.open(audio_path, "wb"), chunk.audio_frames)
```

### Comparing `ego4d-1.7.1/ego4d/research/clep/config.py` & `ego4d-1.7.2/ego4d/research/clep/config.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/research/clep/dataset.py` & `ego4d-1.7.2/ego4d/research/clep/dataset.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/research/clep/model.py` & `ego4d-1.7.2/ego4d/research/clep/model.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/research/clep/preprocess/cc.py` & `ego4d-1.7.2/ego4d/research/clep/preprocess/cc.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/research/clep/preprocess/charades.py` & `ego4d-1.7.2/ego4d/research/clep/preprocess/charades.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/research/clep/preprocess/common.py` & `ego4d-1.7.2/ego4d/research/clep/preprocess/common.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/research/clep/preprocess/ego4d_data.py` & `ego4d-1.7.2/ego4d/research/clep/preprocess/ego4d_data.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/research/clep/preprocess/kinetics.py` & `ego4d-1.7.2/ego4d/research/clep/preprocess/kinetics.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/research/clep/run_preprocess.py` & `ego4d-1.7.2/ego4d/research/clep/run_preprocess.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/research/clep/train.py` & `ego4d-1.7.2/ego4d/research/clep/train.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/research/clep/utils.py` & `ego4d-1.7.2/ego4d/research/clep/utils.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/research/clep/val.py` & `ego4d-1.7.2/ego4d/research/clep/val.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/research/common.py` & `ego4d-1.7.2/ego4d/research/common.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/research/dataset.py` & `ego4d-1.7.2/ego4d/research/dataset.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/research/readers.py` & `ego4d-1.7.2/ego4d/research/readers.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/research/util/lzstring.py` & `ego4d-1.7.2/ego4d/research/util/lzstring.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d/research/util/masks.py` & `ego4d-1.7.2/ego4d/research/util/masks.py`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/ego4d.egg-info/SOURCES.txt` & `ego4d-1.7.2/ego4d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ego4d-1.7.1/setup.py` & `ego4d-1.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates. All Rights Reserved.
 
 from setuptools import find_packages, setup
 
 setup(
     name="ego4d",
-    version="1.7.1",
+    version="1.7.2",
     author="FAIR",
     author_email="info@ego4d-data.org",
     description="Ego4D Dataset CLI",
     url="https://github.com/facebookresearch/Ego4d/",
     install_requires=[
         "boto3",
         "tqdm",
```

