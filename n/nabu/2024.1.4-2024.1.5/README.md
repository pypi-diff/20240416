# Comparing `tmp/nabu-2024.1.4.tar.gz` & `tmp/nabu-2024.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nabu-2024.1.4.tar", last modified: Tue Apr  9 17:51:44 2024, max compression
+gzip compressed data, was "nabu-2024.1.5.tar", last modified: Tue Apr 16 08:27:48 2024, max compression
```

## Comparing `nabu-2024.1.4.tar` & `nabu-2024.1.5.tar`

### file list

```diff
@@ -1,370 +1,370 @@
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.760004 nabu-2024.1.4/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1066 2024-02-22 07:28:34.000000 nabu-2024.1.4/LICENSE
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5207 2024-04-09 17:51:44.760004 nabu-2024.1.4/PKG-INFO
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1614 2021-05-20 09:15:33.000000 nabu-2024.1.4/README.md
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.732005 nabu-2024.1.4/doc/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3787 2024-02-22 07:28:34.000000 nabu-2024.1.4/doc/conf.py
--rwxr-xr-x   0 pierre    (1000) pierre    (1000)     1143 2021-08-26 14:35:51.000000 nabu-2024.1.4/doc/create_conf_doc.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      730 2021-04-19 08:16:31.000000 nabu-2024.1.4/doc/doc_config.py
--rwxr-xr-x   0 pierre    (1000) pierre    (1000)     1012 2020-09-24 07:10:31.000000 nabu-2024.1.4/doc/get_mathjax.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.732005 nabu-2024.1.4/nabu/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      270 2024-04-09 17:50:55.000000 nabu-2024.1.4/nabu/__init__.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.732005 nabu-2024.1.4/nabu/app/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2020-02-16 18:41:31.000000 nabu-2024.1.4/nabu/app/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3246 2023-04-27 12:39:24.000000 nabu-2024.1.4/nabu/app/bootstrap.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2148 2024-02-22 07:28:34.000000 nabu-2024.1.4/nabu/app/bootstrap_stitching.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    11217 2024-03-07 14:48:11.000000 nabu-2024.1.4/nabu/app/cast_volume.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    22109 2024-02-22 07:28:34.000000 nabu-2024.1.4/nabu/app/cli_configs.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3341 2023-04-27 12:39:24.000000 nabu-2024.1.4/nabu/app/compare_volumes.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5132 2024-02-22 07:28:34.000000 nabu-2024.1.4/nabu/app/composite_cor.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2130 2023-11-08 17:09:41.000000 nabu-2024.1.4/nabu/app/correct_rot.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     6199 2023-11-08 17:09:41.000000 nabu-2024.1.4/nabu/app/create_distortion_map_from_poly.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    15217 2023-11-08 17:09:41.000000 nabu-2024.1.4/nabu/app/diag_to_pix.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    17111 2023-12-12 07:29:33.000000 nabu-2024.1.4/nabu/app/diag_to_rot.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5450 2023-04-27 12:39:24.000000 nabu-2024.1.4/nabu/app/double_flatfield.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     8919 2023-11-14 07:22:14.000000 nabu-2024.1.4/nabu/app/generate_header.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     7930 2023-12-01 20:01:03.000000 nabu-2024.1.4/nabu/app/histogram.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4055 2024-03-12 08:31:26.000000 nabu-2024.1.4/nabu/app/multicor.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4976 2023-04-27 12:39:24.000000 nabu-2024.1.4/nabu/app/nx_z_splitter.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4586 2024-02-22 07:28:34.000000 nabu-2024.1.4/nabu/app/parse_reconstruction_log.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5495 2024-01-16 09:04:06.000000 nabu-2024.1.4/nabu/app/prepare_weights_double.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3968 2024-01-16 09:05:41.000000 nabu-2024.1.4/nabu/app/reconstruct.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4454 2023-11-08 17:08:57.000000 nabu-2024.1.4/nabu/app/reconstruct_helical.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     6586 2024-02-22 07:28:34.000000 nabu-2024.1.4/nabu/app/reduce_dark_flat.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     6445 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/app/rotate.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3507 2023-04-27 12:39:24.000000 nabu-2024.1.4/nabu/app/shrink_dataset.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3310 2024-02-22 07:28:34.000000 nabu-2024.1.4/nabu/app/stitching.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.732005 nabu-2024.1.4/nabu/app/tests/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2641 2023-12-12 07:29:33.000000 nabu-2024.1.4/nabu/app/tests/test_reduce_dark_flat.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1178 2023-11-08 17:08:57.000000 nabu-2024.1.4/nabu/app/utils.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3368 2023-11-08 17:08:57.000000 nabu-2024.1.4/nabu/app/validator.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.736004 nabu-2024.1.4/nabu/cuda/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2021-05-26 09:53:09.000000 nabu-2024.1.4/nabu/cuda/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      241 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/cuda/convolution.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      194 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/cuda/fft.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3381 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/cuda/kernel.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      216 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/cuda/medfilt.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      216 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/cuda/padding.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2605 2023-12-07 08:34:31.000000 nabu-2024.1.4/nabu/cuda/processing.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.736004 nabu-2024.1.4/nabu/cuda/src/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     7188 2024-03-28 14:29:32.000000 nabu-2024.1.4/nabu/cuda/src/ElementOp.cu
--rw-r--r--   0 pierre    (1000) pierre    (1000)     6257 2024-01-16 09:04:06.000000 nabu-2024.1.4/nabu/cuda/src/backproj.cu
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1851 2021-05-20 15:41:47.000000 nabu-2024.1.4/nabu/cuda/src/backproj_polar.cu
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2898 2020-02-16 18:41:31.000000 nabu-2024.1.4/nabu/cuda/src/boundary.h
--rw-r--r--   0 pierre    (1000) pierre    (1000)     7353 2020-08-05 14:37:44.000000 nabu-2024.1.4/nabu/cuda/src/convolution.cu
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2220 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/cuda/src/dfi_fftshift.cu
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2058 2023-02-07 09:23:45.000000 nabu-2024.1.4/nabu/cuda/src/flatfield.cu
--rw-r--r--   0 pierre    (1000) pierre    (1000)      547 2023-11-14 07:22:14.000000 nabu-2024.1.4/nabu/cuda/src/fourier_wavelets.cu
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2902 2023-11-08 17:08:57.000000 nabu-2024.1.4/nabu/cuda/src/halftomo.cu
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3955 2023-04-27 12:39:24.000000 nabu-2024.1.4/nabu/cuda/src/helical_padding.cu
--rw-r--r--   0 pierre    (1000) pierre    (1000)      808 2020-10-27 10:43:16.000000 nabu-2024.1.4/nabu/cuda/src/histogram.cu
--rw-r--r--   0 pierre    (1000) pierre    (1000)      839 2021-08-12 07:07:29.000000 nabu-2024.1.4/nabu/cuda/src/interpolation.cu
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2449 2021-08-12 07:07:29.000000 nabu-2024.1.4/nabu/cuda/src/medfilt.cu
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2028 2024-03-28 14:29:51.000000 nabu-2024.1.4/nabu/cuda/src/normalization.cu
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4420 2023-12-12 07:29:33.000000 nabu-2024.1.4/nabu/cuda/src/padding.cu
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3750 2023-04-27 12:39:24.000000 nabu-2024.1.4/nabu/cuda/src/proj.cu
--rw-r--r--   0 pierre    (1000) pierre    (1000)      657 2021-03-04 08:50:36.000000 nabu-2024.1.4/nabu/cuda/src/rotation.cu
--rw-r--r--   0 pierre    (1000) pierre    (1000)      476 2023-11-14 07:22:14.000000 nabu-2024.1.4/nabu/cuda/src/transpose.cu
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.736004 nabu-2024.1.4/nabu/cuda/tests/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2020-02-16 18:41:31.000000 nabu-2024.1.4/nabu/cuda/tests/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     9741 2023-12-05 12:36:09.000000 nabu-2024.1.4/nabu/cuda/utils.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.736004 nabu-2024.1.4/nabu/estimation/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      379 2023-02-07 09:23:45.000000 nabu-2024.1.4/nabu/estimation/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    21584 2024-01-16 09:04:06.000000 nabu-2024.1.4/nabu/estimation/alignment.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    68104 2024-02-22 07:28:34.000000 nabu-2024.1.4/nabu/estimation/cor.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     6394 2023-12-01 20:01:03.000000 nabu-2024.1.4/nabu/estimation/cor_sino.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4701 2023-03-04 19:02:16.000000 nabu-2024.1.4/nabu/estimation/distortion.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    15765 2023-02-07 09:23:45.000000 nabu-2024.1.4/nabu/estimation/focus.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.736004 nabu-2024.1.4/nabu/estimation/tests/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2021-05-20 09:15:33.000000 nabu-2024.1.4/nabu/estimation/tests/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2491 2023-02-07 09:23:45.000000 nabu-2024.1.4/nabu/estimation/tests/test_alignment.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    21268 2024-02-22 07:28:34.000000 nabu-2024.1.4/nabu/estimation/tests/test_cor.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4170 2023-02-07 09:23:45.000000 nabu-2024.1.4/nabu/estimation/tests/test_focus.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1658 2023-02-07 09:23:45.000000 nabu-2024.1.4/nabu/estimation/tests/test_tilt.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2999 2023-02-07 09:23:45.000000 nabu-2024.1.4/nabu/estimation/tests/test_translation.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     8647 2023-11-08 17:08:57.000000 nabu-2024.1.4/nabu/estimation/tilt.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     8581 2023-11-08 17:08:57.000000 nabu-2024.1.4/nabu/estimation/translation.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1401 2023-02-07 09:23:45.000000 nabu-2024.1.4/nabu/estimation/utils.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.740005 nabu-2024.1.4/nabu/io/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      176 2024-04-09 17:50:55.000000 nabu-2024.1.4/nabu/io/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    15638 2024-03-07 14:48:11.000000 nabu-2024.1.4/nabu/io/cast_volume.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    11744 2023-03-04 19:02:16.000000 nabu-2024.1.4/nabu/io/detector_distortion.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    23083 2024-04-09 17:50:55.000000 nabu-2024.1.4/nabu/io/reader.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4477 2023-03-04 19:02:16.000000 nabu-2024.1.4/nabu/io/reader_helical.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.740005 nabu-2024.1.4/nabu/io/tests/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2020-08-05 06:12:22.000000 nabu-2024.1.4/nabu/io/tests/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    10391 2023-11-08 17:08:57.000000 nabu-2024.1.4/nabu/io/tests/test_cast_volume.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     6341 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/io/tests/test_detector_distortion.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     7188 2024-04-09 17:50:55.000000 nabu-2024.1.4/nabu/io/tests/test_writers.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3838 2024-04-09 17:50:55.000000 nabu-2024.1.4/nabu/io/tiffwriter_zmm.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     9223 2024-03-28 12:42:51.000000 nabu-2024.1.4/nabu/io/utils.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    31417 2024-04-09 17:50:55.000000 nabu-2024.1.4/nabu/io/writer.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.740005 nabu-2024.1.4/nabu/misc/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2020-02-16 18:41:31.000000 nabu-2024.1.4/nabu/misc/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2920 2023-02-07 09:23:45.000000 nabu-2024.1.4/nabu/misc/binning.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      205 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/misc/fftshift.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      604 2023-02-07 09:23:45.000000 nabu-2024.1.4/nabu/misc/filters.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5691 2023-03-04 19:02:16.000000 nabu-2024.1.4/nabu/misc/fourier_filters.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      209 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/misc/histogram.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      238 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/misc/histogram_cuda.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      194 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/misc/kernel_base.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2713 2023-02-07 09:23:45.000000 nabu-2024.1.4/nabu/misc/padding.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      216 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/misc/padding_base.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      214 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/misc/processing_base.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      205 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/misc/rotation.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      225 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/misc/rotation_cuda.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.740005 nabu-2024.1.4/nabu/misc/tests/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2020-02-16 18:41:31.000000 nabu-2024.1.4/nabu/misc/tests/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1884 2023-02-07 09:23:45.000000 nabu-2024.1.4/nabu/misc/tests/test_binning.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2389 2023-11-08 17:08:57.000000 nabu-2024.1.4/nabu/misc/tests/test_interpolation.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      209 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/misc/transpose.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      195 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/misc/unsharp.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      221 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/misc/unsharp_cuda.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      238 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/misc/unsharp_opencl.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3906 2023-02-07 09:23:45.000000 nabu-2024.1.4/nabu/misc/utils.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.740005 nabu-2024.1.4/nabu/opencl/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2020-02-16 18:41:31.000000 nabu-2024.1.4/nabu/opencl/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      208 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/opencl/fft.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4736 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/opencl/kernel.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1263 2023-11-08 17:08:57.000000 nabu-2024.1.4/nabu/opencl/memcpy.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      224 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/opencl/padding.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2122 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/opencl/processing.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.740005 nabu-2024.1.4/nabu/opencl/src/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1258 2023-04-27 12:39:24.000000 nabu-2024.1.4/nabu/opencl/src/ElementOp.cl
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5559 2024-01-16 09:04:06.000000 nabu-2024.1.4/nabu/opencl/src/backproj.cl
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1726 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/opencl/src/fftshift.cl
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1386 2023-11-08 17:08:57.000000 nabu-2024.1.4/nabu/opencl/src/halftomo.cl
--rw-r--r--   0 pierre    (1000) pierre    (1000)      460 2023-12-12 07:29:33.000000 nabu-2024.1.4/nabu/opencl/src/padding.cl
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2486 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/opencl/src/roll.cl
--rw-r--r--   0 pierre    (1000) pierre    (1000)      450 2023-11-14 07:22:14.000000 nabu-2024.1.4/nabu/opencl/src/transpose.cl
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.740005 nabu-2024.1.4/nabu/opencl/tests/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2023-04-27 12:39:24.000000 nabu-2024.1.4/nabu/opencl/tests/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    10141 2023-11-08 17:08:57.000000 nabu-2024.1.4/nabu/opencl/utils.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.744005 nabu-2024.1.4/nabu/pipeline/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2021-08-12 07:07:29.000000 nabu-2024.1.4/nabu/pipeline/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     9221 2023-11-08 17:08:57.000000 nabu-2024.1.4/nabu/pipeline/config.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    16300 2023-11-30 13:44:11.000000 nabu-2024.1.4/nabu/pipeline/config_validators.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     6520 2023-03-28 09:40:32.000000 nabu-2024.1.4/nabu/pipeline/datadump.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     9263 2024-04-09 17:50:57.000000 nabu-2024.1.4/nabu/pipeline/dataset_validator.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      920 2023-03-04 19:02:16.000000 nabu-2024.1.4/nabu/pipeline/detector_distortion_provider.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    41374 2024-04-09 17:50:55.000000 nabu-2024.1.4/nabu/pipeline/estimators.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     6086 2024-04-09 17:50:55.000000 nabu-2024.1.4/nabu/pipeline/fallback_utils.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.744005 nabu-2024.1.4/nabu/pipeline/fullfield/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2021-08-12 07:07:29.000000 nabu-2024.1.4/nabu/pipeline/fullfield/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    36919 2024-04-04 13:57:15.000000 nabu-2024.1.4/nabu/pipeline/fullfield/chunked.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5645 2023-12-05 12:36:09.000000 nabu-2024.1.4/nabu/pipeline/fullfield/chunked_cuda.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     9935 2024-02-22 07:28:34.000000 nabu-2024.1.4/nabu/pipeline/fullfield/computations.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3055 2023-03-04 19:02:16.000000 nabu-2024.1.4/nabu/pipeline/fullfield/dataset_validator.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    30358 2024-02-22 07:28:34.000000 nabu-2024.1.4/nabu/pipeline/fullfield/nabu_config.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    36107 2024-04-09 17:50:57.000000 nabu-2024.1.4/nabu/pipeline/fullfield/processconfig.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    36627 2023-12-01 20:01:03.000000 nabu-2024.1.4/nabu/pipeline/fullfield/reconstruction.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.744005 nabu-2024.1.4/nabu/pipeline/helical/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2022-06-24 07:40:44.000000 nabu-2024.1.4/nabu/pipeline/helical/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      640 2023-11-08 17:08:57.000000 nabu-2024.1.4/nabu/pipeline/helical/dataset_validator.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5845 2024-01-16 09:04:06.000000 nabu-2024.1.4/nabu/pipeline/helical/fbp.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    10234 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/pipeline/helical/filtering.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    26308 2024-02-22 07:28:34.000000 nabu-2024.1.4/nabu/pipeline/helical/gridded_accumulator.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    68449 2024-04-09 17:50:55.000000 nabu-2024.1.4/nabu/pipeline/helical/helical_chunked_regridded.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3863 2023-12-01 20:01:03.000000 nabu-2024.1.4/nabu/pipeline/helical/helical_chunked_regridded_cuda.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    24060 2024-04-09 17:50:55.000000 nabu-2024.1.4/nabu/pipeline/helical/helical_reconstruction.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1439 2023-02-07 09:23:45.000000 nabu-2024.1.4/nabu/pipeline/helical/helical_utils.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     8042 2023-11-08 17:08:57.000000 nabu-2024.1.4/nabu/pipeline/helical/nabu_config.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2775 2023-11-08 17:08:57.000000 nabu-2024.1.4/nabu/pipeline/helical/processconfig.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    25044 2023-11-08 17:08:57.000000 nabu-2024.1.4/nabu/pipeline/helical/span_strategy.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.744005 nabu-2024.1.4/nabu/pipeline/helical/tests/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2022-06-24 07:40:44.000000 nabu-2024.1.4/nabu/pipeline/helical/tests/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     6416 2024-02-22 07:28:34.000000 nabu-2024.1.4/nabu/pipeline/helical/tests/test_accumulator.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    14569 2023-08-01 07:42:15.000000 nabu-2024.1.4/nabu/pipeline/helical/tests/test_pipeline_elements_full.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2721 2023-03-04 19:02:16.000000 nabu-2024.1.4/nabu/pipeline/helical/tests/test_strategy.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1555 2024-04-09 17:50:55.000000 nabu-2024.1.4/nabu/pipeline/helical/utils.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3981 2023-03-04 19:02:16.000000 nabu-2024.1.4/nabu/pipeline/helical/weight_balancer.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3479 2024-02-22 07:28:34.000000 nabu-2024.1.4/nabu/pipeline/params.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     8216 2023-11-14 16:50:06.000000 nabu-2024.1.4/nabu/pipeline/processconfig.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.744005 nabu-2024.1.4/nabu/pipeline/tests/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3410 2024-04-09 15:10:05.000000 nabu-2024.1.4/nabu/pipeline/tests/test_chunk_reader.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     8392 2024-02-22 07:28:34.000000 nabu-2024.1.4/nabu/pipeline/tests/test_estimators.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3462 2023-11-08 17:08:57.000000 nabu-2024.1.4/nabu/pipeline/utils.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     7501 2024-04-09 17:50:55.000000 nabu-2024.1.4/nabu/pipeline/writer.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.744005 nabu-2024.1.4/nabu/pipeline/xrdct/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2021-08-12 07:07:29.000000 nabu-2024.1.4/nabu/pipeline/xrdct/__init__.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.748005 nabu-2024.1.4/nabu/preproc/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      284 2023-02-07 09:23:45.000000 nabu-2024.1.4/nabu/preproc/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      379 2023-02-07 09:23:45.000000 nabu-2024.1.4/nabu/preproc/alignment.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5145 2023-11-08 17:08:57.000000 nabu-2024.1.4/nabu/preproc/ccd.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     6068 2023-12-12 07:29:33.000000 nabu-2024.1.4/nabu/preproc/ccd_cuda.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    14657 2023-11-14 07:22:14.000000 nabu-2024.1.4/nabu/preproc/ctf.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5245 2024-04-09 17:50:55.000000 nabu-2024.1.4/nabu/preproc/ctf_cuda.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3309 2023-03-04 19:02:16.000000 nabu-2024.1.4/nabu/preproc/distortion.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     8213 2024-04-09 17:50:55.000000 nabu-2024.1.4/nabu/preproc/double_flatfield.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     6153 2024-02-22 07:28:34.000000 nabu-2024.1.4/nabu/preproc/double_flatfield_cuda.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2279 2023-03-04 19:02:16.000000 nabu-2024.1.4/nabu/preproc/double_flatfield_variable_region.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    19202 2023-03-28 09:40:32.000000 nabu-2024.1.4/nabu/preproc/flatfield.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5331 2023-12-12 07:29:33.000000 nabu-2024.1.4/nabu/preproc/flatfield_cuda.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3155 2023-03-28 09:40:32.000000 nabu-2024.1.4/nabu/preproc/flatfield_variable_region.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    16383 2024-04-09 17:50:55.000000 nabu-2024.1.4/nabu/preproc/phase.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5057 2024-04-09 17:50:55.000000 nabu-2024.1.4/nabu/preproc/phase_cuda.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3424 2023-02-07 09:23:45.000000 nabu-2024.1.4/nabu/preproc/shift.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4165 2024-01-16 09:04:06.000000 nabu-2024.1.4/nabu/preproc/shift_cuda.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.748005 nabu-2024.1.4/nabu/preproc/tests/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2020-02-16 18:41:31.000000 nabu-2024.1.4/nabu/preproc/tests/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2249 2023-02-07 09:23:45.000000 nabu-2024.1.4/nabu/preproc/tests/test_ccd_corr.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     9848 2023-11-14 07:22:14.000000 nabu-2024.1.4/nabu/preproc/tests/test_ctf.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2873 2023-11-08 17:08:57.000000 nabu-2024.1.4/nabu/preproc/tests/test_double_flatfield.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    23498 2023-03-04 19:02:16.000000 nabu-2024.1.4/nabu/preproc/tests/test_flatfield.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2182 2024-04-09 17:50:55.000000 nabu-2024.1.4/nabu/preproc/tests/test_paganin.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2867 2024-01-16 09:04:06.000000 nabu-2024.1.4/nabu/preproc/tests/test_vshift.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.748005 nabu-2024.1.4/nabu/processing/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/processing/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    15313 2023-12-12 07:29:33.000000 nabu-2024.1.4/nabu/processing/convolution_cuda.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5656 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/processing/fft_base.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     8918 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/processing/fft_cuda.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1386 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/processing/fft_opencl.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4880 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/processing/fftshift.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    11316 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/processing/histogram.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3277 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/processing/histogram_cuda.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4251 2024-04-09 17:50:55.000000 nabu-2024.1.4/nabu/processing/kernel_base.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5691 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/processing/medfilt_cuda.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      895 2023-12-12 07:29:33.000000 nabu-2024.1.4/nabu/processing/muladd.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2445 2023-12-12 07:29:33.000000 nabu-2024.1.4/nabu/processing/muladd_cuda.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2874 2023-12-12 07:29:33.000000 nabu-2024.1.4/nabu/processing/padding_base.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2689 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/processing/padding_cuda.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3049 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/processing/padding_opencl.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4412 2024-01-16 09:04:06.000000 nabu-2024.1.4/nabu/processing/processing_base.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2263 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/processing/roll_opencl.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1836 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/processing/rotation.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2746 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/processing/rotation_cuda.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.752004 nabu-2024.1.4/nabu/processing/tests/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/processing/tests/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     9827 2023-12-01 20:01:03.000000 nabu-2024.1.4/nabu/processing/tests/test_fft.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2559 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/processing/tests/test_fftshift.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2283 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/processing/tests/test_histogram.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2722 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/processing/tests/test_medfilt.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1927 2023-12-12 07:29:33.000000 nabu-2024.1.4/nabu/processing/tests/test_muladd.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     8736 2024-02-22 14:03:48.000000 nabu-2024.1.4/nabu/processing/tests/test_padding.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2352 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/processing/tests/test_roll.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2737 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/processing/tests/test_rotation.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2760 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/processing/tests/test_transpose.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4391 2023-12-14 18:31:26.000000 nabu-2024.1.4/nabu/processing/tests/test_unsharp.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4410 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/processing/transpose.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2682 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/processing/unsharp.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2127 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/processing/unsharp_cuda.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2637 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/processing/unsharp_opencl.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.752004 nabu-2024.1.4/nabu/reconstruction/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      163 2023-02-07 09:23:45.000000 nabu-2024.1.4/nabu/reconstruction/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    11028 2023-11-08 17:08:57.000000 nabu-2024.1.4/nabu/reconstruction/cone.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4829 2024-01-16 09:04:06.000000 nabu-2024.1.4/nabu/reconstruction/fbp.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    16833 2024-02-22 07:28:34.000000 nabu-2024.1.4/nabu/reconstruction/fbp_base.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3274 2024-02-22 07:28:34.000000 nabu-2024.1.4/nabu/reconstruction/fbp_opencl.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     7984 2024-04-09 17:50:55.000000 nabu-2024.1.4/nabu/reconstruction/filtering.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3673 2023-12-12 07:29:33.000000 nabu-2024.1.4/nabu/reconstruction/filtering_cuda.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3957 2023-11-30 07:55:23.000000 nabu-2024.1.4/nabu/reconstruction/filtering_opencl.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     9099 2023-12-02 12:30:42.000000 nabu-2024.1.4/nabu/reconstruction/projection.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     7299 2023-02-07 09:23:45.000000 nabu-2024.1.4/nabu/reconstruction/reconstructor.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1644 2023-11-08 17:08:57.000000 nabu-2024.1.4/nabu/reconstruction/reconstructor_cuda.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     9527 2023-12-05 12:36:09.000000 nabu-2024.1.4/nabu/reconstruction/rings.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    13514 2024-04-09 17:50:55.000000 nabu-2024.1.4/nabu/reconstruction/rings_cuda.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    17026 2023-11-08 17:08:57.000000 nabu-2024.1.4/nabu/reconstruction/sinogram.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    10623 2023-12-12 07:29:33.000000 nabu-2024.1.4/nabu/reconstruction/sinogram_cuda.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1403 2023-11-08 17:08:57.000000 nabu-2024.1.4/nabu/reconstruction/sinogram_opencl.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.752004 nabu-2024.1.4/nabu/reconstruction/tests/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2020-02-16 18:41:31.000000 nabu-2024.1.4/nabu/reconstruction/tests/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    11813 2023-02-07 09:23:45.000000 nabu-2024.1.4/nabu/reconstruction/tests/test_cone.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     8299 2023-12-12 07:29:33.000000 nabu-2024.1.4/nabu/reconstruction/tests/test_deringer.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    10053 2024-02-22 07:28:34.000000 nabu-2024.1.4/nabu/reconstruction/tests/test_fbp.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4782 2024-04-09 17:50:55.000000 nabu-2024.1.4/nabu/reconstruction/tests/test_filtering.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4171 2023-11-08 17:08:57.000000 nabu-2024.1.4/nabu/reconstruction/tests/test_halftomo.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     6033 2023-04-27 12:39:24.000000 nabu-2024.1.4/nabu/reconstruction/tests/test_projector.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3221 2023-02-07 09:23:45.000000 nabu-2024.1.4/nabu/reconstruction/tests/test_reconstructor.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3692 2023-02-07 09:23:45.000000 nabu-2024.1.4/nabu/reconstruction/tests/test_sino_normalization.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.752004 nabu-2024.1.4/nabu/resources/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2020-02-16 18:41:31.000000 nabu-2024.1.4/nabu/resources/__init__.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.752004 nabu-2024.1.4/nabu/resources/cli/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2020-02-16 18:41:31.000000 nabu-2024.1.4/nabu/resources/cli/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      170 2021-10-01 06:59:16.000000 nabu-2024.1.4/nabu/resources/cor.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    17004 2024-02-22 07:28:34.000000 nabu-2024.1.4/nabu/resources/dataset_analyzer.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5701 2024-04-09 17:50:55.000000 nabu-2024.1.4/nabu/resources/gpu.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3758 2023-02-07 09:23:45.000000 nabu-2024.1.4/nabu/resources/logger.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     9221 2023-11-08 17:09:41.000000 nabu-2024.1.4/nabu/resources/nxflatfield.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.752004 nabu-2024.1.4/nabu/resources/templates/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2022-11-24 08:53:51.000000 nabu-2024.1.4/nabu/resources/templates/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      394 2023-03-04 19:02:16.000000 nabu-2024.1.4/nabu/resources/templates/bm05_pag.conf
--rw-r--r--   0 pierre    (1000) pierre    (1000)      842 2023-03-04 19:02:16.000000 nabu-2024.1.4/nabu/resources/templates/id16_ctf.conf
--rw-r--r--   0 pierre    (1000) pierre    (1000)      773 2023-02-07 09:23:45.000000 nabu-2024.1.4/nabu/resources/templates/id16_holo.conf
--rw-r--r--   0 pierre    (1000) pierre    (1000)      384 2022-11-24 08:53:51.000000 nabu-2024.1.4/nabu/resources/templates/id19_pag.conf
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.756004 nabu-2024.1.4/nabu/resources/tests/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2020-09-08 07:42:25.000000 nabu-2024.1.4/nabu/resources/tests/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4297 2023-11-08 17:08:57.000000 nabu-2024.1.4/nabu/resources/tests/test_nxflatfield.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2155 2023-03-04 19:02:16.000000 nabu-2024.1.4/nabu/resources/tests/test_units.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5725 2023-11-08 17:08:57.000000 nabu-2024.1.4/nabu/resources/utils.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.756004 nabu-2024.1.4/nabu/stitching/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2023-02-07 09:23:45.000000 nabu-2024.1.4/nabu/stitching/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     6752 2023-11-14 07:22:14.000000 nabu-2024.1.4/nabu/stitching/alignment.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    51333 2024-04-09 17:50:55.000000 nabu-2024.1.4/nabu/stitching/config.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      130 2023-11-08 17:09:41.000000 nabu-2024.1.4/nabu/stitching/definitions.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5889 2023-11-30 13:44:03.000000 nabu-2024.1.4/nabu/stitching/frame_composition.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    15700 2023-12-05 12:36:09.000000 nabu-2024.1.4/nabu/stitching/overlap.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2069 2023-11-30 14:27:36.000000 nabu-2024.1.4/nabu/stitching/sample_normalization.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     8906 2023-11-08 17:09:41.000000 nabu-2024.1.4/nabu/stitching/slurm_utils.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.756004 nabu-2024.1.4/nabu/stitching/tests/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2023-11-08 17:08:57.000000 nabu-2024.1.4/nabu/stitching/tests/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2735 2023-12-01 20:01:03.000000 nabu-2024.1.4/nabu/stitching/tests/test_alignment.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     8490 2023-11-30 14:27:36.000000 nabu-2024.1.4/nabu/stitching/tests/test_config.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     6043 2023-11-08 17:08:57.000000 nabu-2024.1.4/nabu/stitching/tests/test_frame_composition.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2588 2023-12-05 12:36:09.000000 nabu-2024.1.4/nabu/stitching/tests/test_overlap.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1348 2023-11-30 14:27:36.000000 nabu-2024.1.4/nabu/stitching/tests/test_sample_normalization.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4950 2023-11-08 17:08:57.000000 nabu-2024.1.4/nabu/stitching/tests/test_slurm_utils.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      641 2023-12-01 20:01:03.000000 nabu-2024.1.4/nabu/stitching/tests/test_utils.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    42582 2024-03-12 08:31:26.000000 nabu-2024.1.4/nabu/stitching/tests/test_z_stitching.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    23651 2023-11-14 07:22:14.000000 nabu-2024.1.4/nabu/stitching/utils.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)   103400 2024-03-28 12:42:51.000000 nabu-2024.1.4/nabu/stitching/z_stitching.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1417 2023-11-08 17:08:57.000000 nabu-2024.1.4/nabu/tests.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    13298 2023-11-14 07:22:14.000000 nabu-2024.1.4/nabu/testutils.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.756004 nabu-2024.1.4/nabu/thirdparty/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2020-02-16 18:41:31.000000 nabu-2024.1.4/nabu/thirdparty/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    13872 2023-11-08 17:08:57.000000 nabu-2024.1.4/nabu/thirdparty/algotom_convert_sino.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4500 2023-08-10 08:00:22.000000 nabu-2024.1.4/nabu/thirdparty/pore3d_deringer_munch.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    22810 2023-12-05 12:36:09.000000 nabu-2024.1.4/nabu/thirdparty/tomocupy_remove_stripe.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     8634 2020-02-16 18:41:31.000000 nabu-2024.1.4/nabu/thirdparty/tomopy_phase.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5611 2021-05-20 15:41:47.000000 nabu-2024.1.4/nabu/thirdparty/tomwer_load_flats_darks.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    23767 2024-04-09 17:50:55.000000 nabu-2024.1.4/nabu/utils.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.760004 nabu-2024.1.4/nabu.egg-info/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5207 2024-04-09 17:51:44.000000 nabu-2024.1.4/nabu.egg-info/PKG-INFO
--rw-r--r--   0 pierre    (1000) pierre    (1000)     9851 2024-04-09 17:51:44.000000 nabu-2024.1.4/nabu.egg-info/SOURCES.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2024-04-09 17:51:44.000000 nabu-2024.1.4/nabu.egg-info/dependency_links.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1288 2024-04-09 17:51:44.000000 nabu-2024.1.4/nabu.egg-info/entry_points.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)      215 2024-04-09 17:51:44.000000 nabu-2024.1.4/nabu.egg-info/requires.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)       14 2024-04-09 17:51:44.000000 nabu-2024.1.4/nabu.egg-info/top_level.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4206 2024-03-28 12:43:07.000000 nabu-2024.1.4/pyproject.toml
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-09 17:51:44.760004 nabu-2024.1.4/sandbox/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1937 2022-01-20 15:02:07.000000 nabu-2024.1.4/sandbox/align_test.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3909 2020-02-16 18:41:31.000000 nabu-2024.1.4/sandbox/app.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1254 2021-09-24 11:43:07.000000 nabu-2024.1.4/sandbox/binning_cython.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5576 2021-06-15 12:16:55.000000 nabu-2024.1.4/sandbox/circ_sm.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3694 2021-06-10 10:06:32.000000 nabu-2024.1.4/sandbox/composite_image.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4852 2022-04-13 13:45:10.000000 nabu-2024.1.4/sandbox/convert_id15.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1271 2021-04-07 09:14:58.000000 nabu-2024.1.4/sandbox/do_test_ctf.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      958 2021-02-23 12:43:56.000000 nabu-2024.1.4/sandbox/esrf_envs.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1215 2021-03-15 07:57:07.000000 nabu-2024.1.4/sandbox/fbp_polar.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    12543 2020-06-15 10:39:20.000000 nabu-2024.1.4/sandbox/fbp_tilt.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2795 2021-10-07 10:08:42.000000 nabu-2024.1.4/sandbox/interleaved.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1103 2021-06-07 13:45:18.000000 nabu-2024.1.4/sandbox/interp_sinos_halftomo.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      333 2021-06-09 15:36:43.000000 nabu-2024.1.4/sandbox/linear_interp.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1759 2020-07-24 07:30:55.000000 nabu-2024.1.4/sandbox/merge_recs.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1640 2021-03-10 14:25:00.000000 nabu-2024.1.4/sandbox/moduleutils.py
--rwxr-xr-x   0 pierre    (1000) pierre    (1000)     7734 2020-07-21 10:06:42.000000 nabu-2024.1.4/sandbox/nbreconstruct.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      995 2020-07-06 08:31:17.000000 nabu-2024.1.4/sandbox/pag_margin.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4094 2024-01-16 13:32:19.000000 nabu-2024.1.4/sandbox/parse.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1475 2023-03-30 13:51:47.000000 nabu-2024.1.4/sandbox/plot.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2423 2020-06-17 07:06:52.000000 nabu-2024.1.4/sandbox/proj3D.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2037 2020-06-04 12:41:27.000000 nabu-2024.1.4/sandbox/rec_bm05.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3681 2020-07-10 12:57:45.000000 nabu-2024.1.4/sandbox/rec_thread.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1383 2021-04-22 06:48:32.000000 nabu-2024.1.4/sandbox/shift_bilinear2.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5845 2020-06-16 11:40:32.000000 nabu-2024.1.4/sandbox/sinotilt.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1608 2021-02-23 12:42:38.000000 nabu-2024.1.4/sandbox/sysutils.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1848 2022-01-15 08:13:05.000000 nabu-2024.1.4/sandbox/test_mp_queue.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     6830 2020-06-15 11:08:58.000000 nabu-2024.1.4/sandbox/tilt.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1620 2020-06-13 18:29:52.000000 nabu-2024.1.4/sandbox/utils.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     6751 2021-05-03 10:59:48.000000 nabu-2024.1.4/sandbox/vo.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2998 2020-05-18 07:12:51.000000 nabu-2024.1.4/sandbox/workers.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     8076 2020-10-22 10:27:49.000000 nabu-2024.1.4/sandbox/xrdrec_pyFAI_data.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)       38 2024-04-09 17:51:44.760004 nabu-2024.1.4/setup.cfg
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.942163 nabu-2024.1.5/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1066 2024-02-22 07:28:34.000000 nabu-2024.1.5/LICENSE
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     5207 2024-04-16 08:27:48.938163 nabu-2024.1.5/PKG-INFO
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1614 2021-05-20 09:15:33.000000 nabu-2024.1.5/README.md
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.910163 nabu-2024.1.5/doc/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3787 2024-02-22 07:28:34.000000 nabu-2024.1.5/doc/conf.py
+-rwxr-xr-x   0 pierre    (1000) pierre    (1000)     1143 2021-08-26 14:35:51.000000 nabu-2024.1.5/doc/create_conf_doc.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      730 2021-04-19 08:16:31.000000 nabu-2024.1.5/doc/doc_config.py
+-rwxr-xr-x   0 pierre    (1000) pierre    (1000)     1012 2020-09-24 07:10:31.000000 nabu-2024.1.5/doc/get_mathjax.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.910163 nabu-2024.1.5/nabu/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      270 2024-04-16 08:27:28.000000 nabu-2024.1.5/nabu/__init__.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.914163 nabu-2024.1.5/nabu/app/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2020-02-16 18:41:31.000000 nabu-2024.1.5/nabu/app/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3246 2023-04-27 12:39:24.000000 nabu-2024.1.5/nabu/app/bootstrap.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2148 2024-02-22 07:28:34.000000 nabu-2024.1.5/nabu/app/bootstrap_stitching.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    11217 2024-03-07 14:48:11.000000 nabu-2024.1.5/nabu/app/cast_volume.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    22109 2024-02-22 07:28:34.000000 nabu-2024.1.5/nabu/app/cli_configs.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3341 2023-04-27 12:39:24.000000 nabu-2024.1.5/nabu/app/compare_volumes.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     5132 2024-02-22 07:28:34.000000 nabu-2024.1.5/nabu/app/composite_cor.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2130 2023-11-08 17:09:41.000000 nabu-2024.1.5/nabu/app/correct_rot.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     6199 2023-11-08 17:09:41.000000 nabu-2024.1.5/nabu/app/create_distortion_map_from_poly.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    15217 2023-11-08 17:09:41.000000 nabu-2024.1.5/nabu/app/diag_to_pix.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    17111 2023-12-12 07:29:33.000000 nabu-2024.1.5/nabu/app/diag_to_rot.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     5450 2023-04-27 12:39:24.000000 nabu-2024.1.5/nabu/app/double_flatfield.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     8919 2023-11-14 07:22:14.000000 nabu-2024.1.5/nabu/app/generate_header.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     7930 2023-12-01 20:01:03.000000 nabu-2024.1.5/nabu/app/histogram.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4055 2024-03-12 08:31:26.000000 nabu-2024.1.5/nabu/app/multicor.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4976 2023-04-27 12:39:24.000000 nabu-2024.1.5/nabu/app/nx_z_splitter.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4586 2024-02-22 07:28:34.000000 nabu-2024.1.5/nabu/app/parse_reconstruction_log.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     5495 2024-01-16 09:04:06.000000 nabu-2024.1.5/nabu/app/prepare_weights_double.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3968 2024-01-16 09:05:41.000000 nabu-2024.1.5/nabu/app/reconstruct.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4454 2023-11-08 17:08:57.000000 nabu-2024.1.5/nabu/app/reconstruct_helical.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     6586 2024-02-22 07:28:34.000000 nabu-2024.1.5/nabu/app/reduce_dark_flat.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     6445 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/app/rotate.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3507 2023-04-27 12:39:24.000000 nabu-2024.1.5/nabu/app/shrink_dataset.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3310 2024-02-22 07:28:34.000000 nabu-2024.1.5/nabu/app/stitching.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.914163 nabu-2024.1.5/nabu/app/tests/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2641 2023-12-12 07:29:33.000000 nabu-2024.1.5/nabu/app/tests/test_reduce_dark_flat.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1178 2023-11-08 17:08:57.000000 nabu-2024.1.5/nabu/app/utils.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3368 2023-11-08 17:08:57.000000 nabu-2024.1.5/nabu/app/validator.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.914163 nabu-2024.1.5/nabu/cuda/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2021-05-26 09:53:09.000000 nabu-2024.1.5/nabu/cuda/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      241 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/cuda/convolution.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      194 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/cuda/fft.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3381 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/cuda/kernel.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      216 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/cuda/medfilt.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      216 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/cuda/padding.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2605 2023-12-07 08:34:31.000000 nabu-2024.1.5/nabu/cuda/processing.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.914163 nabu-2024.1.5/nabu/cuda/src/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     7188 2024-03-28 14:29:32.000000 nabu-2024.1.5/nabu/cuda/src/ElementOp.cu
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     6257 2024-01-16 09:04:06.000000 nabu-2024.1.5/nabu/cuda/src/backproj.cu
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1851 2021-05-20 15:41:47.000000 nabu-2024.1.5/nabu/cuda/src/backproj_polar.cu
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2898 2020-02-16 18:41:31.000000 nabu-2024.1.5/nabu/cuda/src/boundary.h
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     7353 2020-08-05 14:37:44.000000 nabu-2024.1.5/nabu/cuda/src/convolution.cu
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2220 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/cuda/src/dfi_fftshift.cu
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2058 2023-02-07 09:23:45.000000 nabu-2024.1.5/nabu/cuda/src/flatfield.cu
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      547 2023-11-14 07:22:14.000000 nabu-2024.1.5/nabu/cuda/src/fourier_wavelets.cu
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2902 2023-11-08 17:08:57.000000 nabu-2024.1.5/nabu/cuda/src/halftomo.cu
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3955 2023-04-27 12:39:24.000000 nabu-2024.1.5/nabu/cuda/src/helical_padding.cu
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      808 2020-10-27 10:43:16.000000 nabu-2024.1.5/nabu/cuda/src/histogram.cu
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      839 2021-08-12 07:07:29.000000 nabu-2024.1.5/nabu/cuda/src/interpolation.cu
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2449 2021-08-12 07:07:29.000000 nabu-2024.1.5/nabu/cuda/src/medfilt.cu
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2028 2024-03-28 14:29:51.000000 nabu-2024.1.5/nabu/cuda/src/normalization.cu
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4420 2023-12-12 07:29:33.000000 nabu-2024.1.5/nabu/cuda/src/padding.cu
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3750 2023-04-27 12:39:24.000000 nabu-2024.1.5/nabu/cuda/src/proj.cu
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      657 2021-03-04 08:50:36.000000 nabu-2024.1.5/nabu/cuda/src/rotation.cu
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      476 2023-11-14 07:22:14.000000 nabu-2024.1.5/nabu/cuda/src/transpose.cu
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.914163 nabu-2024.1.5/nabu/cuda/tests/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2020-02-16 18:41:31.000000 nabu-2024.1.5/nabu/cuda/tests/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     9741 2023-12-05 12:36:09.000000 nabu-2024.1.5/nabu/cuda/utils.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.918163 nabu-2024.1.5/nabu/estimation/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      379 2023-02-07 09:23:45.000000 nabu-2024.1.5/nabu/estimation/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    21584 2024-01-16 09:04:06.000000 nabu-2024.1.5/nabu/estimation/alignment.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    68104 2024-02-22 07:28:34.000000 nabu-2024.1.5/nabu/estimation/cor.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     6394 2023-12-01 20:01:03.000000 nabu-2024.1.5/nabu/estimation/cor_sino.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4701 2023-03-04 19:02:16.000000 nabu-2024.1.5/nabu/estimation/distortion.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    15765 2023-02-07 09:23:45.000000 nabu-2024.1.5/nabu/estimation/focus.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.918163 nabu-2024.1.5/nabu/estimation/tests/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2021-05-20 09:15:33.000000 nabu-2024.1.5/nabu/estimation/tests/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2491 2023-02-07 09:23:45.000000 nabu-2024.1.5/nabu/estimation/tests/test_alignment.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    21268 2024-02-22 07:28:34.000000 nabu-2024.1.5/nabu/estimation/tests/test_cor.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4170 2023-02-07 09:23:45.000000 nabu-2024.1.5/nabu/estimation/tests/test_focus.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1658 2023-02-07 09:23:45.000000 nabu-2024.1.5/nabu/estimation/tests/test_tilt.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2999 2023-02-07 09:23:45.000000 nabu-2024.1.5/nabu/estimation/tests/test_translation.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     8647 2023-11-08 17:08:57.000000 nabu-2024.1.5/nabu/estimation/tilt.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     8581 2023-11-08 17:08:57.000000 nabu-2024.1.5/nabu/estimation/translation.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1401 2023-02-07 09:23:45.000000 nabu-2024.1.5/nabu/estimation/utils.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.918163 nabu-2024.1.5/nabu/io/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      176 2024-04-16 08:13:10.000000 nabu-2024.1.5/nabu/io/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    15638 2024-03-07 14:48:11.000000 nabu-2024.1.5/nabu/io/cast_volume.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    11744 2023-03-04 19:02:16.000000 nabu-2024.1.5/nabu/io/detector_distortion.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    23083 2024-04-16 08:13:10.000000 nabu-2024.1.5/nabu/io/reader.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4477 2023-03-04 19:02:16.000000 nabu-2024.1.5/nabu/io/reader_helical.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.918163 nabu-2024.1.5/nabu/io/tests/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2020-08-05 06:12:22.000000 nabu-2024.1.5/nabu/io/tests/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    10391 2023-11-08 17:08:57.000000 nabu-2024.1.5/nabu/io/tests/test_cast_volume.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     6341 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/io/tests/test_detector_distortion.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     7188 2024-04-16 08:13:10.000000 nabu-2024.1.5/nabu/io/tests/test_writers.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3838 2024-04-16 08:13:10.000000 nabu-2024.1.5/nabu/io/tiffwriter_zmm.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     9223 2024-03-28 12:42:51.000000 nabu-2024.1.5/nabu/io/utils.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    31417 2024-04-16 08:13:10.000000 nabu-2024.1.5/nabu/io/writer.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.918163 nabu-2024.1.5/nabu/misc/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2020-02-16 18:41:31.000000 nabu-2024.1.5/nabu/misc/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2920 2023-02-07 09:23:45.000000 nabu-2024.1.5/nabu/misc/binning.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      205 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/misc/fftshift.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      604 2023-02-07 09:23:45.000000 nabu-2024.1.5/nabu/misc/filters.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     5691 2023-03-04 19:02:16.000000 nabu-2024.1.5/nabu/misc/fourier_filters.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      209 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/misc/histogram.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      238 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/misc/histogram_cuda.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      194 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/misc/kernel_base.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2713 2023-02-07 09:23:45.000000 nabu-2024.1.5/nabu/misc/padding.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      216 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/misc/padding_base.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      214 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/misc/processing_base.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      205 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/misc/rotation.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      225 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/misc/rotation_cuda.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.922164 nabu-2024.1.5/nabu/misc/tests/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2020-02-16 18:41:31.000000 nabu-2024.1.5/nabu/misc/tests/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1884 2023-02-07 09:23:45.000000 nabu-2024.1.5/nabu/misc/tests/test_binning.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2389 2023-11-08 17:08:57.000000 nabu-2024.1.5/nabu/misc/tests/test_interpolation.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      209 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/misc/transpose.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      195 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/misc/unsharp.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      221 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/misc/unsharp_cuda.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      238 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/misc/unsharp_opencl.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3906 2023-02-07 09:23:45.000000 nabu-2024.1.5/nabu/misc/utils.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.922164 nabu-2024.1.5/nabu/opencl/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2020-02-16 18:41:31.000000 nabu-2024.1.5/nabu/opencl/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      208 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/opencl/fft.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4736 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/opencl/kernel.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1263 2023-11-08 17:08:57.000000 nabu-2024.1.5/nabu/opencl/memcpy.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      224 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/opencl/padding.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2122 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/opencl/processing.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.922164 nabu-2024.1.5/nabu/opencl/src/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1258 2023-04-27 12:39:24.000000 nabu-2024.1.5/nabu/opencl/src/ElementOp.cl
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     5559 2024-01-16 09:04:06.000000 nabu-2024.1.5/nabu/opencl/src/backproj.cl
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1726 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/opencl/src/fftshift.cl
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1386 2023-11-08 17:08:57.000000 nabu-2024.1.5/nabu/opencl/src/halftomo.cl
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      460 2023-12-12 07:29:33.000000 nabu-2024.1.5/nabu/opencl/src/padding.cl
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2486 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/opencl/src/roll.cl
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      450 2023-11-14 07:22:14.000000 nabu-2024.1.5/nabu/opencl/src/transpose.cl
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.922164 nabu-2024.1.5/nabu/opencl/tests/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2023-04-27 12:39:24.000000 nabu-2024.1.5/nabu/opencl/tests/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    10141 2023-11-08 17:08:57.000000 nabu-2024.1.5/nabu/opencl/utils.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.922164 nabu-2024.1.5/nabu/pipeline/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2021-08-12 07:07:29.000000 nabu-2024.1.5/nabu/pipeline/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     9221 2023-11-08 17:08:57.000000 nabu-2024.1.5/nabu/pipeline/config.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    16300 2023-11-30 13:44:11.000000 nabu-2024.1.5/nabu/pipeline/config_validators.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     6520 2023-03-28 09:40:32.000000 nabu-2024.1.5/nabu/pipeline/datadump.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     9263 2024-04-09 17:50:57.000000 nabu-2024.1.5/nabu/pipeline/dataset_validator.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      920 2023-03-04 19:02:16.000000 nabu-2024.1.5/nabu/pipeline/detector_distortion_provider.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    41374 2024-04-16 08:21:13.000000 nabu-2024.1.5/nabu/pipeline/estimators.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     6086 2024-04-16 08:21:13.000000 nabu-2024.1.5/nabu/pipeline/fallback_utils.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.922164 nabu-2024.1.5/nabu/pipeline/fullfield/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2021-08-12 07:07:29.000000 nabu-2024.1.5/nabu/pipeline/fullfield/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    36919 2024-04-04 13:57:15.000000 nabu-2024.1.5/nabu/pipeline/fullfield/chunked.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     5645 2023-12-05 12:36:09.000000 nabu-2024.1.5/nabu/pipeline/fullfield/chunked_cuda.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     9935 2024-02-22 07:28:34.000000 nabu-2024.1.5/nabu/pipeline/fullfield/computations.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3055 2023-03-04 19:02:16.000000 nabu-2024.1.5/nabu/pipeline/fullfield/dataset_validator.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    30358 2024-02-22 07:28:34.000000 nabu-2024.1.5/nabu/pipeline/fullfield/nabu_config.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    36107 2024-04-16 08:21:13.000000 nabu-2024.1.5/nabu/pipeline/fullfield/processconfig.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    36627 2023-12-01 20:01:03.000000 nabu-2024.1.5/nabu/pipeline/fullfield/reconstruction.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.926164 nabu-2024.1.5/nabu/pipeline/helical/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2022-06-24 07:40:44.000000 nabu-2024.1.5/nabu/pipeline/helical/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      640 2023-11-08 17:08:57.000000 nabu-2024.1.5/nabu/pipeline/helical/dataset_validator.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     5845 2024-01-16 09:04:06.000000 nabu-2024.1.5/nabu/pipeline/helical/fbp.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    10234 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/pipeline/helical/filtering.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    26308 2024-02-22 07:28:34.000000 nabu-2024.1.5/nabu/pipeline/helical/gridded_accumulator.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    68449 2024-04-16 08:21:13.000000 nabu-2024.1.5/nabu/pipeline/helical/helical_chunked_regridded.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3863 2023-12-01 20:01:03.000000 nabu-2024.1.5/nabu/pipeline/helical/helical_chunked_regridded_cuda.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    24060 2024-04-16 08:21:13.000000 nabu-2024.1.5/nabu/pipeline/helical/helical_reconstruction.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1439 2023-02-07 09:23:45.000000 nabu-2024.1.5/nabu/pipeline/helical/helical_utils.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     8042 2023-11-08 17:08:57.000000 nabu-2024.1.5/nabu/pipeline/helical/nabu_config.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2775 2023-11-08 17:08:57.000000 nabu-2024.1.5/nabu/pipeline/helical/processconfig.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    25044 2023-11-08 17:08:57.000000 nabu-2024.1.5/nabu/pipeline/helical/span_strategy.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.926164 nabu-2024.1.5/nabu/pipeline/helical/tests/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2022-06-24 07:40:44.000000 nabu-2024.1.5/nabu/pipeline/helical/tests/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     6416 2024-02-22 07:28:34.000000 nabu-2024.1.5/nabu/pipeline/helical/tests/test_accumulator.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    14569 2023-08-01 07:42:15.000000 nabu-2024.1.5/nabu/pipeline/helical/tests/test_pipeline_elements_full.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2721 2023-03-04 19:02:16.000000 nabu-2024.1.5/nabu/pipeline/helical/tests/test_strategy.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1555 2024-04-16 08:13:10.000000 nabu-2024.1.5/nabu/pipeline/helical/utils.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3981 2023-03-04 19:02:16.000000 nabu-2024.1.5/nabu/pipeline/helical/weight_balancer.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3479 2024-02-22 07:28:34.000000 nabu-2024.1.5/nabu/pipeline/params.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     8216 2023-11-14 16:50:06.000000 nabu-2024.1.5/nabu/pipeline/processconfig.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.926164 nabu-2024.1.5/nabu/pipeline/tests/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3410 2024-04-09 15:10:05.000000 nabu-2024.1.5/nabu/pipeline/tests/test_chunk_reader.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     8392 2024-02-22 07:28:34.000000 nabu-2024.1.5/nabu/pipeline/tests/test_estimators.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3462 2023-11-08 17:08:57.000000 nabu-2024.1.5/nabu/pipeline/utils.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     7558 2024-04-16 08:21:19.000000 nabu-2024.1.5/nabu/pipeline/writer.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.926164 nabu-2024.1.5/nabu/pipeline/xrdct/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2021-08-12 07:07:29.000000 nabu-2024.1.5/nabu/pipeline/xrdct/__init__.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.926164 nabu-2024.1.5/nabu/preproc/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      284 2023-02-07 09:23:45.000000 nabu-2024.1.5/nabu/preproc/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      379 2023-02-07 09:23:45.000000 nabu-2024.1.5/nabu/preproc/alignment.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     5145 2023-11-08 17:08:57.000000 nabu-2024.1.5/nabu/preproc/ccd.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     6068 2023-12-12 07:29:33.000000 nabu-2024.1.5/nabu/preproc/ccd_cuda.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    14657 2023-11-14 07:22:14.000000 nabu-2024.1.5/nabu/preproc/ctf.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     5245 2024-04-16 08:21:13.000000 nabu-2024.1.5/nabu/preproc/ctf_cuda.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3309 2023-03-04 19:02:16.000000 nabu-2024.1.5/nabu/preproc/distortion.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     8213 2024-04-16 08:13:10.000000 nabu-2024.1.5/nabu/preproc/double_flatfield.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     6153 2024-02-22 07:28:34.000000 nabu-2024.1.5/nabu/preproc/double_flatfield_cuda.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2279 2023-03-04 19:02:16.000000 nabu-2024.1.5/nabu/preproc/double_flatfield_variable_region.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    19202 2023-03-28 09:40:32.000000 nabu-2024.1.5/nabu/preproc/flatfield.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     5331 2023-12-12 07:29:33.000000 nabu-2024.1.5/nabu/preproc/flatfield_cuda.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3155 2023-03-28 09:40:32.000000 nabu-2024.1.5/nabu/preproc/flatfield_variable_region.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    16383 2024-04-16 08:13:10.000000 nabu-2024.1.5/nabu/preproc/phase.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     5057 2024-04-16 08:13:10.000000 nabu-2024.1.5/nabu/preproc/phase_cuda.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3424 2023-02-07 09:23:45.000000 nabu-2024.1.5/nabu/preproc/shift.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4165 2024-01-16 09:04:06.000000 nabu-2024.1.5/nabu/preproc/shift_cuda.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.926164 nabu-2024.1.5/nabu/preproc/tests/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2020-02-16 18:41:31.000000 nabu-2024.1.5/nabu/preproc/tests/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2249 2023-02-07 09:23:45.000000 nabu-2024.1.5/nabu/preproc/tests/test_ccd_corr.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     9848 2023-11-14 07:22:14.000000 nabu-2024.1.5/nabu/preproc/tests/test_ctf.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2873 2023-11-08 17:08:57.000000 nabu-2024.1.5/nabu/preproc/tests/test_double_flatfield.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    23498 2023-03-04 19:02:16.000000 nabu-2024.1.5/nabu/preproc/tests/test_flatfield.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2182 2024-04-16 08:13:10.000000 nabu-2024.1.5/nabu/preproc/tests/test_paganin.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2867 2024-01-16 09:04:06.000000 nabu-2024.1.5/nabu/preproc/tests/test_vshift.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.930163 nabu-2024.1.5/nabu/processing/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/processing/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    15313 2023-12-12 07:29:33.000000 nabu-2024.1.5/nabu/processing/convolution_cuda.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     5656 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/processing/fft_base.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     8918 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/processing/fft_cuda.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1386 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/processing/fft_opencl.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4880 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/processing/fftshift.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    11316 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/processing/histogram.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3277 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/processing/histogram_cuda.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4251 2024-04-16 08:21:13.000000 nabu-2024.1.5/nabu/processing/kernel_base.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     5691 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/processing/medfilt_cuda.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      895 2023-12-12 07:29:33.000000 nabu-2024.1.5/nabu/processing/muladd.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2445 2023-12-12 07:29:33.000000 nabu-2024.1.5/nabu/processing/muladd_cuda.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2874 2023-12-12 07:29:33.000000 nabu-2024.1.5/nabu/processing/padding_base.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2689 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/processing/padding_cuda.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3049 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/processing/padding_opencl.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4412 2024-01-16 09:04:06.000000 nabu-2024.1.5/nabu/processing/processing_base.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2263 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/processing/roll_opencl.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1836 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/processing/rotation.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2746 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/processing/rotation_cuda.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.930163 nabu-2024.1.5/nabu/processing/tests/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/processing/tests/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     9827 2023-12-01 20:01:03.000000 nabu-2024.1.5/nabu/processing/tests/test_fft.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2559 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/processing/tests/test_fftshift.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2283 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/processing/tests/test_histogram.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2722 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/processing/tests/test_medfilt.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1927 2023-12-12 07:29:33.000000 nabu-2024.1.5/nabu/processing/tests/test_muladd.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     8736 2024-02-22 14:03:48.000000 nabu-2024.1.5/nabu/processing/tests/test_padding.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2352 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/processing/tests/test_roll.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2737 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/processing/tests/test_rotation.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2760 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/processing/tests/test_transpose.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4391 2023-12-14 18:31:26.000000 nabu-2024.1.5/nabu/processing/tests/test_unsharp.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4410 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/processing/transpose.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2682 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/processing/unsharp.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2127 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/processing/unsharp_cuda.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2637 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/processing/unsharp_opencl.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.930163 nabu-2024.1.5/nabu/reconstruction/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      163 2023-02-07 09:23:45.000000 nabu-2024.1.5/nabu/reconstruction/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    11028 2023-11-08 17:08:57.000000 nabu-2024.1.5/nabu/reconstruction/cone.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4829 2024-01-16 09:04:06.000000 nabu-2024.1.5/nabu/reconstruction/fbp.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    16833 2024-02-22 07:28:34.000000 nabu-2024.1.5/nabu/reconstruction/fbp_base.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3274 2024-02-22 07:28:34.000000 nabu-2024.1.5/nabu/reconstruction/fbp_opencl.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     7984 2024-04-16 08:13:10.000000 nabu-2024.1.5/nabu/reconstruction/filtering.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3673 2023-12-12 07:29:33.000000 nabu-2024.1.5/nabu/reconstruction/filtering_cuda.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3957 2023-11-30 07:55:23.000000 nabu-2024.1.5/nabu/reconstruction/filtering_opencl.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     9099 2023-12-02 12:30:42.000000 nabu-2024.1.5/nabu/reconstruction/projection.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     7299 2023-02-07 09:23:45.000000 nabu-2024.1.5/nabu/reconstruction/reconstructor.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1644 2023-11-08 17:08:57.000000 nabu-2024.1.5/nabu/reconstruction/reconstructor_cuda.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     9527 2023-12-05 12:36:09.000000 nabu-2024.1.5/nabu/reconstruction/rings.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    13514 2024-04-16 08:13:10.000000 nabu-2024.1.5/nabu/reconstruction/rings_cuda.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    17026 2023-11-08 17:08:57.000000 nabu-2024.1.5/nabu/reconstruction/sinogram.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    10623 2023-12-12 07:29:33.000000 nabu-2024.1.5/nabu/reconstruction/sinogram_cuda.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1403 2023-11-08 17:08:57.000000 nabu-2024.1.5/nabu/reconstruction/sinogram_opencl.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.934163 nabu-2024.1.5/nabu/reconstruction/tests/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2020-02-16 18:41:31.000000 nabu-2024.1.5/nabu/reconstruction/tests/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    11813 2023-02-07 09:23:45.000000 nabu-2024.1.5/nabu/reconstruction/tests/test_cone.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     8299 2023-12-12 07:29:33.000000 nabu-2024.1.5/nabu/reconstruction/tests/test_deringer.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    10053 2024-02-22 07:28:34.000000 nabu-2024.1.5/nabu/reconstruction/tests/test_fbp.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4782 2024-04-16 08:13:10.000000 nabu-2024.1.5/nabu/reconstruction/tests/test_filtering.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4171 2023-11-08 17:08:57.000000 nabu-2024.1.5/nabu/reconstruction/tests/test_halftomo.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     6033 2023-04-27 12:39:24.000000 nabu-2024.1.5/nabu/reconstruction/tests/test_projector.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3221 2023-02-07 09:23:45.000000 nabu-2024.1.5/nabu/reconstruction/tests/test_reconstructor.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3692 2023-02-07 09:23:45.000000 nabu-2024.1.5/nabu/reconstruction/tests/test_sino_normalization.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.934163 nabu-2024.1.5/nabu/resources/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2020-02-16 18:41:31.000000 nabu-2024.1.5/nabu/resources/__init__.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.934163 nabu-2024.1.5/nabu/resources/cli/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2020-02-16 18:41:31.000000 nabu-2024.1.5/nabu/resources/cli/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      170 2021-10-01 06:59:16.000000 nabu-2024.1.5/nabu/resources/cor.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    17004 2024-02-22 07:28:34.000000 nabu-2024.1.5/nabu/resources/dataset_analyzer.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     5701 2024-04-16 08:21:13.000000 nabu-2024.1.5/nabu/resources/gpu.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3758 2023-02-07 09:23:45.000000 nabu-2024.1.5/nabu/resources/logger.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     9221 2023-11-08 17:09:41.000000 nabu-2024.1.5/nabu/resources/nxflatfield.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.934163 nabu-2024.1.5/nabu/resources/templates/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2022-11-24 08:53:51.000000 nabu-2024.1.5/nabu/resources/templates/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      394 2023-03-04 19:02:16.000000 nabu-2024.1.5/nabu/resources/templates/bm05_pag.conf
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      842 2023-03-04 19:02:16.000000 nabu-2024.1.5/nabu/resources/templates/id16_ctf.conf
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      773 2023-02-07 09:23:45.000000 nabu-2024.1.5/nabu/resources/templates/id16_holo.conf
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      384 2022-11-24 08:53:51.000000 nabu-2024.1.5/nabu/resources/templates/id19_pag.conf
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.934163 nabu-2024.1.5/nabu/resources/tests/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2020-09-08 07:42:25.000000 nabu-2024.1.5/nabu/resources/tests/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4297 2023-11-08 17:08:57.000000 nabu-2024.1.5/nabu/resources/tests/test_nxflatfield.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2155 2023-03-04 19:02:16.000000 nabu-2024.1.5/nabu/resources/tests/test_units.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     5725 2023-11-08 17:08:57.000000 nabu-2024.1.5/nabu/resources/utils.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.934163 nabu-2024.1.5/nabu/stitching/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2023-02-07 09:23:45.000000 nabu-2024.1.5/nabu/stitching/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     6752 2023-11-14 07:22:14.000000 nabu-2024.1.5/nabu/stitching/alignment.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    51333 2024-04-16 08:21:13.000000 nabu-2024.1.5/nabu/stitching/config.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      130 2023-11-08 17:09:41.000000 nabu-2024.1.5/nabu/stitching/definitions.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     5889 2023-11-30 13:44:03.000000 nabu-2024.1.5/nabu/stitching/frame_composition.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    15700 2023-12-05 12:36:09.000000 nabu-2024.1.5/nabu/stitching/overlap.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2069 2023-11-30 14:27:36.000000 nabu-2024.1.5/nabu/stitching/sample_normalization.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     8906 2023-11-08 17:09:41.000000 nabu-2024.1.5/nabu/stitching/slurm_utils.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.934163 nabu-2024.1.5/nabu/stitching/tests/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2023-11-08 17:08:57.000000 nabu-2024.1.5/nabu/stitching/tests/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2735 2023-12-01 20:01:03.000000 nabu-2024.1.5/nabu/stitching/tests/test_alignment.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     8490 2023-11-30 14:27:36.000000 nabu-2024.1.5/nabu/stitching/tests/test_config.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     6043 2023-11-08 17:08:57.000000 nabu-2024.1.5/nabu/stitching/tests/test_frame_composition.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2588 2023-12-05 12:36:09.000000 nabu-2024.1.5/nabu/stitching/tests/test_overlap.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1348 2023-11-30 14:27:36.000000 nabu-2024.1.5/nabu/stitching/tests/test_sample_normalization.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4950 2023-11-08 17:08:57.000000 nabu-2024.1.5/nabu/stitching/tests/test_slurm_utils.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      641 2023-12-01 20:01:03.000000 nabu-2024.1.5/nabu/stitching/tests/test_utils.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    42582 2024-03-12 08:31:26.000000 nabu-2024.1.5/nabu/stitching/tests/test_z_stitching.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    23651 2023-11-14 07:22:14.000000 nabu-2024.1.5/nabu/stitching/utils.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)   103400 2024-03-28 12:42:51.000000 nabu-2024.1.5/nabu/stitching/z_stitching.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1417 2023-11-08 17:08:57.000000 nabu-2024.1.5/nabu/tests.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    13298 2023-11-14 07:22:14.000000 nabu-2024.1.5/nabu/testutils.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.938163 nabu-2024.1.5/nabu/thirdparty/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2020-02-16 18:41:31.000000 nabu-2024.1.5/nabu/thirdparty/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    13872 2023-11-08 17:08:57.000000 nabu-2024.1.5/nabu/thirdparty/algotom_convert_sino.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4500 2023-08-10 08:00:22.000000 nabu-2024.1.5/nabu/thirdparty/pore3d_deringer_munch.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    22810 2023-12-05 12:36:09.000000 nabu-2024.1.5/nabu/thirdparty/tomocupy_remove_stripe.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     8634 2020-02-16 18:41:31.000000 nabu-2024.1.5/nabu/thirdparty/tomopy_phase.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     5611 2021-05-20 15:41:47.000000 nabu-2024.1.5/nabu/thirdparty/tomwer_load_flats_darks.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    23767 2024-04-16 08:13:10.000000 nabu-2024.1.5/nabu/utils.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.938163 nabu-2024.1.5/nabu.egg-info/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     5207 2024-04-16 08:27:48.000000 nabu-2024.1.5/nabu.egg-info/PKG-INFO
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     9851 2024-04-16 08:27:48.000000 nabu-2024.1.5/nabu.egg-info/SOURCES.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2024-04-16 08:27:48.000000 nabu-2024.1.5/nabu.egg-info/dependency_links.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1288 2024-04-16 08:27:48.000000 nabu-2024.1.5/nabu.egg-info/entry_points.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      215 2024-04-16 08:27:48.000000 nabu-2024.1.5/nabu.egg-info/requires.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)       14 2024-04-16 08:27:48.000000 nabu-2024.1.5/nabu.egg-info/top_level.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4206 2024-03-28 12:43:07.000000 nabu-2024.1.5/pyproject.toml
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2024-04-16 08:27:48.938163 nabu-2024.1.5/sandbox/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1937 2022-01-20 15:02:07.000000 nabu-2024.1.5/sandbox/align_test.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3909 2020-02-16 18:41:31.000000 nabu-2024.1.5/sandbox/app.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1254 2021-09-24 11:43:07.000000 nabu-2024.1.5/sandbox/binning_cython.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     5576 2021-06-15 12:16:55.000000 nabu-2024.1.5/sandbox/circ_sm.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3694 2021-06-10 10:06:32.000000 nabu-2024.1.5/sandbox/composite_image.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4852 2022-04-13 13:45:10.000000 nabu-2024.1.5/sandbox/convert_id15.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1271 2021-04-07 09:14:58.000000 nabu-2024.1.5/sandbox/do_test_ctf.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      958 2021-02-23 12:43:56.000000 nabu-2024.1.5/sandbox/esrf_envs.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1215 2021-03-15 07:57:07.000000 nabu-2024.1.5/sandbox/fbp_polar.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    12543 2020-06-15 10:39:20.000000 nabu-2024.1.5/sandbox/fbp_tilt.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2795 2021-10-07 10:08:42.000000 nabu-2024.1.5/sandbox/interleaved.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1103 2021-06-07 13:45:18.000000 nabu-2024.1.5/sandbox/interp_sinos_halftomo.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      333 2021-06-09 15:36:43.000000 nabu-2024.1.5/sandbox/linear_interp.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1759 2020-07-24 07:30:55.000000 nabu-2024.1.5/sandbox/merge_recs.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1640 2021-03-10 14:25:00.000000 nabu-2024.1.5/sandbox/moduleutils.py
+-rwxr-xr-x   0 pierre    (1000) pierre    (1000)     7734 2020-07-21 10:06:42.000000 nabu-2024.1.5/sandbox/nbreconstruct.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      995 2020-07-06 08:31:17.000000 nabu-2024.1.5/sandbox/pag_margin.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4094 2024-01-16 13:32:19.000000 nabu-2024.1.5/sandbox/parse.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1475 2023-03-30 13:51:47.000000 nabu-2024.1.5/sandbox/plot.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2423 2020-06-17 07:06:52.000000 nabu-2024.1.5/sandbox/proj3D.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2037 2020-06-04 12:41:27.000000 nabu-2024.1.5/sandbox/rec_bm05.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3681 2020-07-10 12:57:45.000000 nabu-2024.1.5/sandbox/rec_thread.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1383 2021-04-22 06:48:32.000000 nabu-2024.1.5/sandbox/shift_bilinear2.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     5845 2020-06-16 11:40:32.000000 nabu-2024.1.5/sandbox/sinotilt.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1608 2021-02-23 12:42:38.000000 nabu-2024.1.5/sandbox/sysutils.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1848 2022-01-15 08:13:05.000000 nabu-2024.1.5/sandbox/test_mp_queue.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     6830 2020-06-15 11:08:58.000000 nabu-2024.1.5/sandbox/tilt.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1620 2020-06-13 18:29:52.000000 nabu-2024.1.5/sandbox/utils.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     6751 2021-05-03 10:59:48.000000 nabu-2024.1.5/sandbox/vo.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2998 2020-05-18 07:12:51.000000 nabu-2024.1.5/sandbox/workers.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     8076 2020-10-22 10:27:49.000000 nabu-2024.1.5/sandbox/xrdrec_pyFAI_data.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)       38 2024-04-16 08:27:48.942163 nabu-2024.1.5/setup.cfg
```

### Comparing `nabu-2024.1.4/LICENSE` & `nabu-2024.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/PKG-INFO` & `nabu-2024.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nabu
-Version: 2024.1.4
+Version: 2024.1.5
 Summary: Nabu - Tomography software
 Author-email: Pierre Paleo <pierre.paleo@esrf.fr>, Henri Payno <henri.payno@esrf.fr>, Alessandro Mirone <mirone@esrf.fr>, Jérôme Lesaint <jerome.lesaint@esrf.fr>
 Maintainer-email: Pierre Paleo <pierre.paleo@esrf.fr>
 License: MIT License
         
         Copyright (c) 2020-2024 ESRF
```

### Comparing `nabu-2024.1.4/README.md` & `nabu-2024.1.5/README.md`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/doc/conf.py` & `nabu-2024.1.5/doc/conf.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/doc/create_conf_doc.py` & `nabu-2024.1.5/doc/create_conf_doc.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/doc/doc_config.py` & `nabu-2024.1.5/doc/doc_config.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/doc/get_mathjax.py` & `nabu-2024.1.5/doc/get_mathjax.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/app/bootstrap.py` & `nabu-2024.1.5/nabu/app/bootstrap.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/app/bootstrap_stitching.py` & `nabu-2024.1.5/nabu/app/bootstrap_stitching.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/app/cast_volume.py` & `nabu-2024.1.5/nabu/app/cast_volume.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/app/cli_configs.py` & `nabu-2024.1.5/nabu/app/cli_configs.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/app/compare_volumes.py` & `nabu-2024.1.5/nabu/app/compare_volumes.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/app/composite_cor.py` & `nabu-2024.1.5/nabu/app/composite_cor.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/app/correct_rot.py` & `nabu-2024.1.5/nabu/app/correct_rot.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/app/create_distortion_map_from_poly.py` & `nabu-2024.1.5/nabu/app/create_distortion_map_from_poly.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/app/diag_to_pix.py` & `nabu-2024.1.5/nabu/app/diag_to_pix.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/app/diag_to_rot.py` & `nabu-2024.1.5/nabu/app/diag_to_rot.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/app/double_flatfield.py` & `nabu-2024.1.5/nabu/app/double_flatfield.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/app/generate_header.py` & `nabu-2024.1.5/nabu/app/generate_header.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/app/histogram.py` & `nabu-2024.1.5/nabu/app/histogram.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/app/multicor.py` & `nabu-2024.1.5/nabu/app/multicor.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/app/nx_z_splitter.py` & `nabu-2024.1.5/nabu/app/nx_z_splitter.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/app/parse_reconstruction_log.py` & `nabu-2024.1.5/nabu/app/parse_reconstruction_log.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/app/prepare_weights_double.py` & `nabu-2024.1.5/nabu/app/prepare_weights_double.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/app/reconstruct.py` & `nabu-2024.1.5/nabu/app/reconstruct.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/app/reconstruct_helical.py` & `nabu-2024.1.5/nabu/app/reconstruct_helical.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/app/reduce_dark_flat.py` & `nabu-2024.1.5/nabu/app/reduce_dark_flat.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/app/rotate.py` & `nabu-2024.1.5/nabu/app/rotate.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/app/shrink_dataset.py` & `nabu-2024.1.5/nabu/app/shrink_dataset.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/app/stitching.py` & `nabu-2024.1.5/nabu/app/stitching.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/app/tests/test_reduce_dark_flat.py` & `nabu-2024.1.5/nabu/app/tests/test_reduce_dark_flat.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/app/utils.py` & `nabu-2024.1.5/nabu/app/utils.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/app/validator.py` & `nabu-2024.1.5/nabu/app/validator.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/cuda/kernel.py` & `nabu-2024.1.5/nabu/cuda/kernel.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/cuda/processing.py` & `nabu-2024.1.5/nabu/cuda/processing.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/cuda/src/ElementOp.cu` & `nabu-2024.1.5/nabu/cuda/src/ElementOp.cu`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/cuda/src/backproj.cu` & `nabu-2024.1.5/nabu/cuda/src/backproj.cu`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/cuda/src/backproj_polar.cu` & `nabu-2024.1.5/nabu/cuda/src/backproj_polar.cu`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/cuda/src/boundary.h` & `nabu-2024.1.5/nabu/cuda/src/boundary.h`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/cuda/src/convolution.cu` & `nabu-2024.1.5/nabu/cuda/src/convolution.cu`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/cuda/src/dfi_fftshift.cu` & `nabu-2024.1.5/nabu/cuda/src/dfi_fftshift.cu`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/cuda/src/flatfield.cu` & `nabu-2024.1.5/nabu/cuda/src/flatfield.cu`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/cuda/src/fourier_wavelets.cu` & `nabu-2024.1.5/nabu/cuda/src/fourier_wavelets.cu`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/cuda/src/halftomo.cu` & `nabu-2024.1.5/nabu/cuda/src/halftomo.cu`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/cuda/src/helical_padding.cu` & `nabu-2024.1.5/nabu/cuda/src/helical_padding.cu`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/cuda/src/histogram.cu` & `nabu-2024.1.5/nabu/cuda/src/histogram.cu`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/cuda/src/interpolation.cu` & `nabu-2024.1.5/nabu/cuda/src/interpolation.cu`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/cuda/src/medfilt.cu` & `nabu-2024.1.5/nabu/cuda/src/medfilt.cu`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/cuda/src/normalization.cu` & `nabu-2024.1.5/nabu/cuda/src/normalization.cu`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/cuda/src/padding.cu` & `nabu-2024.1.5/nabu/cuda/src/padding.cu`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/cuda/src/proj.cu` & `nabu-2024.1.5/nabu/cuda/src/proj.cu`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/cuda/src/rotation.cu` & `nabu-2024.1.5/nabu/cuda/src/rotation.cu`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/cuda/utils.py` & `nabu-2024.1.5/nabu/cuda/utils.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/estimation/alignment.py` & `nabu-2024.1.5/nabu/estimation/alignment.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/estimation/cor.py` & `nabu-2024.1.5/nabu/estimation/cor.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/estimation/cor_sino.py` & `nabu-2024.1.5/nabu/estimation/cor_sino.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/estimation/distortion.py` & `nabu-2024.1.5/nabu/estimation/distortion.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/estimation/focus.py` & `nabu-2024.1.5/nabu/estimation/focus.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/estimation/tests/test_alignment.py` & `nabu-2024.1.5/nabu/estimation/tests/test_alignment.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/estimation/tests/test_cor.py` & `nabu-2024.1.5/nabu/estimation/tests/test_cor.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/estimation/tests/test_focus.py` & `nabu-2024.1.5/nabu/estimation/tests/test_focus.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/estimation/tests/test_tilt.py` & `nabu-2024.1.5/nabu/estimation/tests/test_tilt.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/estimation/tests/test_translation.py` & `nabu-2024.1.5/nabu/estimation/tests/test_translation.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/estimation/tilt.py` & `nabu-2024.1.5/nabu/estimation/tilt.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/estimation/translation.py` & `nabu-2024.1.5/nabu/estimation/translation.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/estimation/utils.py` & `nabu-2024.1.5/nabu/estimation/utils.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/io/cast_volume.py` & `nabu-2024.1.5/nabu/io/cast_volume.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/io/detector_distortion.py` & `nabu-2024.1.5/nabu/io/detector_distortion.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/io/reader.py` & `nabu-2024.1.5/nabu/io/reader.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/io/reader_helical.py` & `nabu-2024.1.5/nabu/io/reader_helical.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/io/tests/test_cast_volume.py` & `nabu-2024.1.5/nabu/io/tests/test_cast_volume.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/io/tests/test_detector_distortion.py` & `nabu-2024.1.5/nabu/io/tests/test_detector_distortion.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/io/tests/test_writers.py` & `nabu-2024.1.5/nabu/io/tests/test_writers.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/io/tiffwriter_zmm.py` & `nabu-2024.1.5/nabu/io/tiffwriter_zmm.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/io/utils.py` & `nabu-2024.1.5/nabu/io/utils.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/io/writer.py` & `nabu-2024.1.5/nabu/io/writer.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/misc/binning.py` & `nabu-2024.1.5/nabu/misc/binning.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/misc/filters.py` & `nabu-2024.1.5/nabu/misc/filters.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/misc/fourier_filters.py` & `nabu-2024.1.5/nabu/misc/fourier_filters.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/misc/padding.py` & `nabu-2024.1.5/nabu/misc/padding.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/misc/tests/test_binning.py` & `nabu-2024.1.5/nabu/misc/tests/test_binning.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/misc/tests/test_interpolation.py` & `nabu-2024.1.5/nabu/misc/tests/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/misc/utils.py` & `nabu-2024.1.5/nabu/misc/utils.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/opencl/kernel.py` & `nabu-2024.1.5/nabu/opencl/kernel.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/opencl/memcpy.py` & `nabu-2024.1.5/nabu/opencl/memcpy.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/opencl/processing.py` & `nabu-2024.1.5/nabu/opencl/processing.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/opencl/src/ElementOp.cl` & `nabu-2024.1.5/nabu/opencl/src/ElementOp.cl`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/opencl/src/backproj.cl` & `nabu-2024.1.5/nabu/opencl/src/backproj.cl`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/opencl/src/fftshift.cl` & `nabu-2024.1.5/nabu/opencl/src/fftshift.cl`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/opencl/src/halftomo.cl` & `nabu-2024.1.5/nabu/opencl/src/halftomo.cl`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/opencl/src/roll.cl` & `nabu-2024.1.5/nabu/opencl/src/roll.cl`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/opencl/utils.py` & `nabu-2024.1.5/nabu/opencl/utils.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/pipeline/config.py` & `nabu-2024.1.5/nabu/pipeline/config.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/pipeline/config_validators.py` & `nabu-2024.1.5/nabu/pipeline/config_validators.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/pipeline/datadump.py` & `nabu-2024.1.5/nabu/pipeline/datadump.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/pipeline/dataset_validator.py` & `nabu-2024.1.5/nabu/pipeline/dataset_validator.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/pipeline/detector_distortion_provider.py` & `nabu-2024.1.5/nabu/pipeline/detector_distortion_provider.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/pipeline/estimators.py` & `nabu-2024.1.5/nabu/pipeline/estimators.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/pipeline/fallback_utils.py` & `nabu-2024.1.5/nabu/pipeline/fallback_utils.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/pipeline/fullfield/chunked.py` & `nabu-2024.1.5/nabu/pipeline/fullfield/chunked.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/pipeline/fullfield/chunked_cuda.py` & `nabu-2024.1.5/nabu/pipeline/fullfield/chunked_cuda.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/pipeline/fullfield/computations.py` & `nabu-2024.1.5/nabu/pipeline/fullfield/computations.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/pipeline/fullfield/dataset_validator.py` & `nabu-2024.1.5/nabu/pipeline/fullfield/dataset_validator.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/pipeline/fullfield/nabu_config.py` & `nabu-2024.1.5/nabu/pipeline/fullfield/nabu_config.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/pipeline/fullfield/processconfig.py` & `nabu-2024.1.5/nabu/pipeline/fullfield/processconfig.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/pipeline/fullfield/reconstruction.py` & `nabu-2024.1.5/nabu/pipeline/fullfield/reconstruction.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/pipeline/helical/dataset_validator.py` & `nabu-2024.1.5/nabu/pipeline/helical/dataset_validator.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/pipeline/helical/fbp.py` & `nabu-2024.1.5/nabu/pipeline/helical/fbp.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/pipeline/helical/filtering.py` & `nabu-2024.1.5/nabu/pipeline/helical/filtering.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/pipeline/helical/gridded_accumulator.py` & `nabu-2024.1.5/nabu/pipeline/helical/gridded_accumulator.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/pipeline/helical/helical_chunked_regridded.py` & `nabu-2024.1.5/nabu/pipeline/helical/helical_chunked_regridded.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/pipeline/helical/helical_chunked_regridded_cuda.py` & `nabu-2024.1.5/nabu/pipeline/helical/helical_chunked_regridded_cuda.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/pipeline/helical/helical_reconstruction.py` & `nabu-2024.1.5/nabu/pipeline/helical/helical_reconstruction.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/pipeline/helical/helical_utils.py` & `nabu-2024.1.5/nabu/pipeline/helical/helical_utils.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/pipeline/helical/nabu_config.py` & `nabu-2024.1.5/nabu/pipeline/helical/nabu_config.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/pipeline/helical/processconfig.py` & `nabu-2024.1.5/nabu/pipeline/helical/processconfig.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/pipeline/helical/span_strategy.py` & `nabu-2024.1.5/nabu/pipeline/helical/span_strategy.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/pipeline/helical/tests/test_accumulator.py` & `nabu-2024.1.5/nabu/pipeline/helical/tests/test_accumulator.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/pipeline/helical/tests/test_pipeline_elements_full.py` & `nabu-2024.1.5/nabu/pipeline/helical/tests/test_pipeline_elements_full.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/pipeline/helical/tests/test_strategy.py` & `nabu-2024.1.5/nabu/pipeline/helical/tests/test_strategy.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/pipeline/helical/utils.py` & `nabu-2024.1.5/nabu/pipeline/helical/utils.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/pipeline/helical/weight_balancer.py` & `nabu-2024.1.5/nabu/pipeline/helical/weight_balancer.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/pipeline/params.py` & `nabu-2024.1.5/nabu/pipeline/params.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/pipeline/processconfig.py` & `nabu-2024.1.5/nabu/pipeline/processconfig.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/pipeline/tests/test_chunk_reader.py` & `nabu-2024.1.5/nabu/pipeline/tests/test_chunk_reader.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/pipeline/tests/test_estimators.py` & `nabu-2024.1.5/nabu/pipeline/tests/test_estimators.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/pipeline/utils.py` & `nabu-2024.1.5/nabu/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/pipeline/writer.py` & `nabu-2024.1.5/nabu/pipeline/writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,16 +132,17 @@
         elif self.file_format in ["vol", "bigtiff"]:
             writer_kwargs = {
                 "file_path": path.join(
                     self.output_dir, self.file_prefix + "." + self.file_format.replace("bigtiff", "tiff")
                 ),
                 "overwrite": self.overwrite,
                 "append": self.extra_options.get("single_output_file_initialized", False),
-                "hst_metadata": self.extra_options.get("raw_vol_metadata", {}),
             }
+            if self.file_format == "vol":
+                writer_kwargs["hst_metadata"] = self.extra_options.get("raw_vol_metadata", {})
         else:
             raise ValueError("Unsupported file format: %s" % self.file_format)
         self._h5_entry = self.metadata.get("entry", "entry")
         self.writer = self._writer_classes[self.file_format](**writer_kwargs)
         self.fname = self.get_fname(self.writer)
         if path.exists(self.fname):
             err = "File already exists: %s" % self.fname
```

### Comparing `nabu-2024.1.4/nabu/preproc/ccd.py` & `nabu-2024.1.5/nabu/preproc/ccd.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/preproc/ccd_cuda.py` & `nabu-2024.1.5/nabu/preproc/ccd_cuda.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/preproc/ctf.py` & `nabu-2024.1.5/nabu/preproc/ctf.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/preproc/ctf_cuda.py` & `nabu-2024.1.5/nabu/preproc/ctf_cuda.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/preproc/distortion.py` & `nabu-2024.1.5/nabu/preproc/distortion.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/preproc/double_flatfield.py` & `nabu-2024.1.5/nabu/preproc/double_flatfield.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/preproc/double_flatfield_cuda.py` & `nabu-2024.1.5/nabu/preproc/double_flatfield_cuda.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/preproc/double_flatfield_variable_region.py` & `nabu-2024.1.5/nabu/preproc/double_flatfield_variable_region.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/preproc/flatfield.py` & `nabu-2024.1.5/nabu/preproc/flatfield.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/preproc/flatfield_cuda.py` & `nabu-2024.1.5/nabu/preproc/flatfield_cuda.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/preproc/flatfield_variable_region.py` & `nabu-2024.1.5/nabu/preproc/flatfield_variable_region.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/preproc/phase.py` & `nabu-2024.1.5/nabu/preproc/phase.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/preproc/phase_cuda.py` & `nabu-2024.1.5/nabu/preproc/phase_cuda.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/preproc/shift.py` & `nabu-2024.1.5/nabu/preproc/shift.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/preproc/shift_cuda.py` & `nabu-2024.1.5/nabu/preproc/shift_cuda.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/preproc/tests/test_ccd_corr.py` & `nabu-2024.1.5/nabu/preproc/tests/test_ccd_corr.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/preproc/tests/test_ctf.py` & `nabu-2024.1.5/nabu/preproc/tests/test_ctf.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/preproc/tests/test_double_flatfield.py` & `nabu-2024.1.5/nabu/preproc/tests/test_double_flatfield.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/preproc/tests/test_flatfield.py` & `nabu-2024.1.5/nabu/preproc/tests/test_flatfield.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/preproc/tests/test_paganin.py` & `nabu-2024.1.5/nabu/preproc/tests/test_paganin.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/preproc/tests/test_vshift.py` & `nabu-2024.1.5/nabu/preproc/tests/test_vshift.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/processing/convolution_cuda.py` & `nabu-2024.1.5/nabu/processing/convolution_cuda.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/processing/fft_base.py` & `nabu-2024.1.5/nabu/processing/fft_base.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/processing/fft_cuda.py` & `nabu-2024.1.5/nabu/processing/fft_cuda.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/processing/fft_opencl.py` & `nabu-2024.1.5/nabu/processing/fft_opencl.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/processing/fftshift.py` & `nabu-2024.1.5/nabu/processing/fftshift.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/processing/histogram.py` & `nabu-2024.1.5/nabu/processing/histogram.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/processing/histogram_cuda.py` & `nabu-2024.1.5/nabu/processing/histogram_cuda.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/processing/kernel_base.py` & `nabu-2024.1.5/nabu/processing/kernel_base.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/processing/medfilt_cuda.py` & `nabu-2024.1.5/nabu/processing/medfilt_cuda.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/processing/muladd.py` & `nabu-2024.1.5/nabu/processing/muladd.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/processing/muladd_cuda.py` & `nabu-2024.1.5/nabu/processing/muladd_cuda.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/processing/padding_base.py` & `nabu-2024.1.5/nabu/processing/padding_base.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/processing/padding_cuda.py` & `nabu-2024.1.5/nabu/processing/padding_cuda.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/processing/padding_opencl.py` & `nabu-2024.1.5/nabu/processing/padding_opencl.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/processing/processing_base.py` & `nabu-2024.1.5/nabu/processing/processing_base.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/processing/roll_opencl.py` & `nabu-2024.1.5/nabu/processing/roll_opencl.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/processing/rotation.py` & `nabu-2024.1.5/nabu/processing/rotation.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/processing/rotation_cuda.py` & `nabu-2024.1.5/nabu/processing/rotation_cuda.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/processing/tests/test_fft.py` & `nabu-2024.1.5/nabu/processing/tests/test_fft.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/processing/tests/test_fftshift.py` & `nabu-2024.1.5/nabu/processing/tests/test_fftshift.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/processing/tests/test_histogram.py` & `nabu-2024.1.5/nabu/processing/tests/test_histogram.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/processing/tests/test_medfilt.py` & `nabu-2024.1.5/nabu/processing/tests/test_medfilt.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/processing/tests/test_muladd.py` & `nabu-2024.1.5/nabu/processing/tests/test_muladd.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/processing/tests/test_padding.py` & `nabu-2024.1.5/nabu/processing/tests/test_padding.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/processing/tests/test_roll.py` & `nabu-2024.1.5/nabu/processing/tests/test_roll.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/processing/tests/test_rotation.py` & `nabu-2024.1.5/nabu/processing/tests/test_rotation.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/processing/tests/test_transpose.py` & `nabu-2024.1.5/nabu/processing/tests/test_transpose.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/processing/tests/test_unsharp.py` & `nabu-2024.1.5/nabu/processing/tests/test_unsharp.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/processing/transpose.py` & `nabu-2024.1.5/nabu/processing/transpose.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/processing/unsharp.py` & `nabu-2024.1.5/nabu/processing/unsharp.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/processing/unsharp_cuda.py` & `nabu-2024.1.5/nabu/processing/unsharp_cuda.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/processing/unsharp_opencl.py` & `nabu-2024.1.5/nabu/processing/unsharp_opencl.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/reconstruction/cone.py` & `nabu-2024.1.5/nabu/reconstruction/cone.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/reconstruction/fbp.py` & `nabu-2024.1.5/nabu/reconstruction/fbp.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/reconstruction/fbp_base.py` & `nabu-2024.1.5/nabu/reconstruction/fbp_base.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/reconstruction/fbp_opencl.py` & `nabu-2024.1.5/nabu/reconstruction/fbp_opencl.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/reconstruction/filtering.py` & `nabu-2024.1.5/nabu/reconstruction/filtering.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/reconstruction/filtering_cuda.py` & `nabu-2024.1.5/nabu/reconstruction/filtering_cuda.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/reconstruction/filtering_opencl.py` & `nabu-2024.1.5/nabu/reconstruction/filtering_opencl.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/reconstruction/projection.py` & `nabu-2024.1.5/nabu/reconstruction/projection.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/reconstruction/reconstructor.py` & `nabu-2024.1.5/nabu/reconstruction/reconstructor.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/reconstruction/reconstructor_cuda.py` & `nabu-2024.1.5/nabu/reconstruction/reconstructor_cuda.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/reconstruction/rings.py` & `nabu-2024.1.5/nabu/reconstruction/rings.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/reconstruction/rings_cuda.py` & `nabu-2024.1.5/nabu/reconstruction/rings_cuda.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/reconstruction/sinogram.py` & `nabu-2024.1.5/nabu/reconstruction/sinogram.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/reconstruction/sinogram_cuda.py` & `nabu-2024.1.5/nabu/reconstruction/sinogram_cuda.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/reconstruction/sinogram_opencl.py` & `nabu-2024.1.5/nabu/reconstruction/sinogram_opencl.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/reconstruction/tests/test_cone.py` & `nabu-2024.1.5/nabu/reconstruction/tests/test_cone.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/reconstruction/tests/test_deringer.py` & `nabu-2024.1.5/nabu/reconstruction/tests/test_deringer.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/reconstruction/tests/test_fbp.py` & `nabu-2024.1.5/nabu/reconstruction/tests/test_fbp.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/reconstruction/tests/test_filtering.py` & `nabu-2024.1.5/nabu/reconstruction/tests/test_filtering.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/reconstruction/tests/test_halftomo.py` & `nabu-2024.1.5/nabu/reconstruction/tests/test_halftomo.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/reconstruction/tests/test_projector.py` & `nabu-2024.1.5/nabu/reconstruction/tests/test_projector.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/reconstruction/tests/test_reconstructor.py` & `nabu-2024.1.5/nabu/reconstruction/tests/test_reconstructor.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/reconstruction/tests/test_sino_normalization.py` & `nabu-2024.1.5/nabu/reconstruction/tests/test_sino_normalization.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/resources/dataset_analyzer.py` & `nabu-2024.1.5/nabu/resources/dataset_analyzer.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/resources/gpu.py` & `nabu-2024.1.5/nabu/resources/gpu.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/resources/logger.py` & `nabu-2024.1.5/nabu/resources/logger.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/resources/nxflatfield.py` & `nabu-2024.1.5/nabu/resources/nxflatfield.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/resources/templates/id16_ctf.conf` & `nabu-2024.1.5/nabu/resources/templates/id16_ctf.conf`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/resources/templates/id16_holo.conf` & `nabu-2024.1.5/nabu/resources/templates/id16_holo.conf`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/resources/tests/test_nxflatfield.py` & `nabu-2024.1.5/nabu/resources/tests/test_nxflatfield.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/resources/tests/test_units.py` & `nabu-2024.1.5/nabu/resources/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/resources/utils.py` & `nabu-2024.1.5/nabu/resources/utils.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/stitching/alignment.py` & `nabu-2024.1.5/nabu/stitching/alignment.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/stitching/config.py` & `nabu-2024.1.5/nabu/stitching/config.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/stitching/frame_composition.py` & `nabu-2024.1.5/nabu/stitching/frame_composition.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/stitching/overlap.py` & `nabu-2024.1.5/nabu/stitching/overlap.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/stitching/sample_normalization.py` & `nabu-2024.1.5/nabu/stitching/sample_normalization.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/stitching/slurm_utils.py` & `nabu-2024.1.5/nabu/stitching/slurm_utils.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/stitching/tests/test_alignment.py` & `nabu-2024.1.5/nabu/stitching/tests/test_alignment.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/stitching/tests/test_config.py` & `nabu-2024.1.5/nabu/stitching/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/stitching/tests/test_frame_composition.py` & `nabu-2024.1.5/nabu/stitching/tests/test_frame_composition.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/stitching/tests/test_overlap.py` & `nabu-2024.1.5/nabu/stitching/tests/test_overlap.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/stitching/tests/test_sample_normalization.py` & `nabu-2024.1.5/nabu/stitching/tests/test_sample_normalization.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/stitching/tests/test_slurm_utils.py` & `nabu-2024.1.5/nabu/stitching/tests/test_slurm_utils.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/stitching/tests/test_utils.py` & `nabu-2024.1.5/nabu/stitching/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/stitching/tests/test_z_stitching.py` & `nabu-2024.1.5/nabu/stitching/tests/test_z_stitching.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/stitching/utils.py` & `nabu-2024.1.5/nabu/stitching/utils.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/stitching/z_stitching.py` & `nabu-2024.1.5/nabu/stitching/z_stitching.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/tests.py` & `nabu-2024.1.5/nabu/tests.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/testutils.py` & `nabu-2024.1.5/nabu/testutils.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/thirdparty/algotom_convert_sino.py` & `nabu-2024.1.5/nabu/thirdparty/algotom_convert_sino.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/thirdparty/pore3d_deringer_munch.py` & `nabu-2024.1.5/nabu/thirdparty/pore3d_deringer_munch.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/thirdparty/tomocupy_remove_stripe.py` & `nabu-2024.1.5/nabu/thirdparty/tomocupy_remove_stripe.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/thirdparty/tomopy_phase.py` & `nabu-2024.1.5/nabu/thirdparty/tomopy_phase.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/thirdparty/tomwer_load_flats_darks.py` & `nabu-2024.1.5/nabu/thirdparty/tomwer_load_flats_darks.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu/utils.py` & `nabu-2024.1.5/nabu/utils.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu.egg-info/PKG-INFO` & `nabu-2024.1.5/nabu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nabu
-Version: 2024.1.4
+Version: 2024.1.5
 Summary: Nabu - Tomography software
 Author-email: Pierre Paleo <pierre.paleo@esrf.fr>, Henri Payno <henri.payno@esrf.fr>, Alessandro Mirone <mirone@esrf.fr>, Jérôme Lesaint <jerome.lesaint@esrf.fr>
 Maintainer-email: Pierre Paleo <pierre.paleo@esrf.fr>
 License: MIT License
         
         Copyright (c) 2020-2024 ESRF
```

### Comparing `nabu-2024.1.4/nabu.egg-info/SOURCES.txt` & `nabu-2024.1.5/nabu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/nabu.egg-info/entry_points.txt` & `nabu-2024.1.5/nabu.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/pyproject.toml` & `nabu-2024.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/sandbox/align_test.py` & `nabu-2024.1.5/sandbox/align_test.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/sandbox/app.py` & `nabu-2024.1.5/sandbox/app.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/sandbox/binning_cython.py` & `nabu-2024.1.5/sandbox/binning_cython.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/sandbox/circ_sm.py` & `nabu-2024.1.5/sandbox/circ_sm.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/sandbox/composite_image.py` & `nabu-2024.1.5/sandbox/composite_image.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/sandbox/convert_id15.py` & `nabu-2024.1.5/sandbox/convert_id15.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/sandbox/do_test_ctf.py` & `nabu-2024.1.5/sandbox/do_test_ctf.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/sandbox/esrf_envs.py` & `nabu-2024.1.5/sandbox/esrf_envs.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/sandbox/fbp_polar.py` & `nabu-2024.1.5/sandbox/fbp_polar.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/sandbox/fbp_tilt.py` & `nabu-2024.1.5/sandbox/fbp_tilt.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/sandbox/interleaved.py` & `nabu-2024.1.5/sandbox/interleaved.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/sandbox/interp_sinos_halftomo.py` & `nabu-2024.1.5/sandbox/interp_sinos_halftomo.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/sandbox/merge_recs.py` & `nabu-2024.1.5/sandbox/merge_recs.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/sandbox/moduleutils.py` & `nabu-2024.1.5/sandbox/moduleutils.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/sandbox/nbreconstruct.py` & `nabu-2024.1.5/sandbox/nbreconstruct.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/sandbox/pag_margin.py` & `nabu-2024.1.5/sandbox/pag_margin.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/sandbox/parse.py` & `nabu-2024.1.5/sandbox/parse.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/sandbox/plot.py` & `nabu-2024.1.5/sandbox/plot.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/sandbox/proj3D.py` & `nabu-2024.1.5/sandbox/proj3D.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/sandbox/rec_bm05.py` & `nabu-2024.1.5/sandbox/rec_bm05.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/sandbox/rec_thread.py` & `nabu-2024.1.5/sandbox/rec_thread.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/sandbox/shift_bilinear2.py` & `nabu-2024.1.5/sandbox/shift_bilinear2.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/sandbox/sinotilt.py` & `nabu-2024.1.5/sandbox/sinotilt.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/sandbox/sysutils.py` & `nabu-2024.1.5/sandbox/sysutils.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/sandbox/test_mp_queue.py` & `nabu-2024.1.5/sandbox/test_mp_queue.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/sandbox/tilt.py` & `nabu-2024.1.5/sandbox/tilt.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/sandbox/utils.py` & `nabu-2024.1.5/sandbox/utils.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/sandbox/vo.py` & `nabu-2024.1.5/sandbox/vo.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/sandbox/workers.py` & `nabu-2024.1.5/sandbox/workers.py`

 * *Files identical despite different names*

### Comparing `nabu-2024.1.4/sandbox/xrdrec_pyFAI_data.py` & `nabu-2024.1.5/sandbox/xrdrec_pyFAI_data.py`

 * *Files identical despite different names*

