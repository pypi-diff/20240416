# Comparing `tmp/AIPyS-0.0.6.tar.gz` & `tmp/AIPyS-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AIPyS-0.0.6.tar", last modified: Tue Apr 16 12:59:24 2024, max compression
+gzip compressed data, was "AIPyS-0.0.7.tar", last modified: Tue Apr 16 13:00:09 2024, max compression
```

## Comparing `AIPyS-0.0.6.tar` & `AIPyS-0.0.7.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 12:59:24.742752 AIPyS-0.0.6/
-drwxrwxrwx   0        0        0        0 2024-04-16 12:59:24.076301 AIPyS-0.0.6/AIPyS/
-drwxrwxrwx   0        0        0        0 2024-04-16 12:59:24.303152 AIPyS-0.0.6/AIPyS/CLI/
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.6/AIPyS/CLI/__init__.py
--rw-rw-rw-   0        0        0     7580 2024-04-15 18:55:22.000000 AIPyS-0.0.6/AIPyS/CLI/aipys.py
--rw-rw-rw-   0        0        0     1284 2024-04-15 18:53:26.000000 AIPyS-0.0.6/AIPyS/CLI/area_analysis.py
--rw-rw-rw-   0        0        0     3292 2024-04-16 12:57:00.000000 AIPyS-0.0.6/AIPyS/CLI/loadParameters.py
--rw-rw-rw-   0        0        0     2761 2024-03-01 16:45:08.000000 AIPyS-0.0.6/AIPyS/CLI/promptParameters.py
--rw-rw-rw-   0        0        0     9375 2024-04-09 18:42:35.000000 AIPyS-0.0.6/AIPyS/CLI/set_parameters.py
--rw-rw-rw-   0        0        0      854 2024-02-29 17:57:58.000000 AIPyS-0.0.6/AIPyS/CLI/test.py
--rw-rw-rw-   0        0        0     1500 2024-03-02 13:49:57.000000 AIPyS-0.0.6/AIPyS/DataLoad.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.6/AIPyS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 12:59:24.031741 AIPyS-0.0.6/AIPyS/classification/
-drwxrwxrwx   0        0        0        0 2024-04-16 12:59:24.360182 AIPyS-0.0.6/AIPyS/classification/CNN/
--rw-rw-rw-   0        0        0     2501 2024-03-02 20:04:55.000000 AIPyS-0.0.6/AIPyS/classification/CNN/CNN_deploy.py
--rw-rw-rw-   0        0        0     5086 2024-02-28 23:19:26.000000 AIPyS-0.0.6/AIPyS/classification/CNN/Taining_data_orgenizer.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.6/AIPyS/classification/CNN/__init__.py
--rw-rw-rw-   0        0        0     1908 2024-02-28 23:19:26.000000 AIPyS-0.0.6/AIPyS/classification/CNN/mapSgRNA.py
--rw-rw-rw-   0        0        0    18474 2024-02-28 23:19:26.000000 AIPyS-0.0.6/AIPyS/classification/CNN/model_builder.py
--rw-rw-rw-   0        0        0     8897 2024-02-28 23:19:26.000000 AIPyS-0.0.6/AIPyS/classification/CNN/model_evaluation_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-16 12:59:24.408975 AIPyS-0.0.6/AIPyS/classification/bayes/
--rw-rw-rw-   0        0        0     2596 2024-02-28 23:19:26.000000 AIPyS-0.0.6/AIPyS/classification/bayes/BayesianModels.py
--rw-rw-rw-   0        0        0     6221 2024-03-02 14:10:27.000000 AIPyS-0.0.6/AIPyS/classification/bayes/Baysian_deploy.py
--rw-rw-rw-   0        0        0     7817 2024-04-11 17:07:53.000000 AIPyS-0.0.6/AIPyS/classification/bayes/Baysian_training.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.6/AIPyS/classification/bayes/DisplayImageFrame.py
--rw-rw-rw-   0        0        0     6145 2024-02-29 21:52:44.000000 AIPyS-0.0.6/AIPyS/classification/bayes/GranulaityMesure.py
--rw-rw-rw-   0        0        0    18111 2024-04-15 19:16:12.000000 AIPyS-0.0.6/AIPyS/classification/bayes/GranularityDataGen.py
--rw-rw-rw-   0        0        0     5065 2024-02-28 23:19:26.000000 AIPyS-0.0.6/AIPyS/classification/bayes/GranularityDeploy.py
--rw-rw-rw-   0        0        0     2024 2024-02-28 23:19:26.000000 AIPyS-0.0.6/AIPyS/classification/bayes/RunningWindow.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.6/AIPyS/classification/bayes/__init__.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:37:34.000000 AIPyS-0.0.6/AIPyS/draft.py
-drwxrwxrwx   0        0        0        0 2024-04-16 12:59:24.033032 AIPyS-0.0.6/AIPyS/segmentation/
-drwxrwxrwx   0        0        0        0 2024-04-16 12:59:24.475174 AIPyS-0.0.6/AIPyS/segmentation/cellpose/
--rw-rw-rw-   0        0        0     2283 2024-02-28 23:19:56.000000 AIPyS-0.0.6/AIPyS/segmentation/cellpose/AIPS_cellpose.py
--rw-rw-rw-   0        0        0     1666 2024-04-12 18:30:36.000000 AIPyS-0.0.6/AIPyS/segmentation/cellpose/AIPS_cellpse_video_gen.py
--rw-rw-rw-   0        0        0     2450 2024-03-02 12:03:05.000000 AIPyS-0.0.6/AIPyS/segmentation/cellpose/StackObjects_cellpose.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.6/AIPyS/segmentation/cellpose/__init__.py
--rw-rw-rw-   0        0        0     4727 2024-04-15 18:01:11.000000 AIPyS-0.0.6/AIPyS/segmentation/cellpose/plotObjectAreas.py
-drwxrwxrwx   0        0        0        0 2024-04-16 12:59:24.481882 AIPyS-0.0.6/AIPyS/segmentation/parametric/
--rw-rw-rw-   0        0        0     3564 2024-02-28 23:19:27.000000 AIPyS-0.0.6/AIPyS/segmentation/parametric/GlobalSeg.py
--rw-rw-rw-   0        0        0     2426 2024-02-28 23:19:56.000000 AIPyS-0.0.6/AIPyS/segmentation/parametric/ImageSeqGlobSeg.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.6/AIPyS/segmentation/parametric/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 12:59:24.557616 AIPyS-0.0.6/AIPyS/supportFunctions/
--rw-rw-rw-   0        0        0     6856 2024-03-02 13:11:22.000000 AIPyS-0.0.6/AIPyS/supportFunctions/AIPS_file_display.py
--rw-rw-rw-   0        0        0    13755 2024-04-15 18:45:15.000000 AIPyS-0.0.6/AIPyS/supportFunctions/AIPS_functions.py
--rw-rw-rw-   0        0        0    10310 2024-02-28 23:19:27.000000 AIPyS-0.0.6/AIPyS/supportFunctions/AIPS_granularity.py
--rw-rw-rw-   0        0        0    14491 2024-02-28 23:19:27.000000 AIPyS-0.0.6/AIPyS/supportFunctions/AIPS_module.py
--rw-rw-rw-   0        0        0     4250 2024-02-28 23:19:27.000000 AIPyS-0.0.6/AIPyS/supportFunctions/AIPS_simulate.py
--rw-rw-rw-   0        0        0     7362 2024-02-28 23:19:27.000000 AIPyS-0.0.6/AIPyS/supportFunctions/Display_composit.py
--rw-rw-rw-   0        0        0     1252 2024-02-28 23:19:27.000000 AIPyS-0.0.6/AIPyS/supportFunctions/GranularityFunc.py
--rw-rw-rw-   0        0        0    16340 2024-02-28 23:19:27.000000 AIPyS-0.0.6/AIPyS/supportFunctions/Granularity_cellprofiler.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.6/AIPyS/supportFunctions/__init__.py
--rw-rw-rw-   0        0        0     8046 2024-02-28 23:19:27.000000 AIPyS-0.0.6/AIPyS/supportFunctions/display_and_xml.py
--rw-rw-rw-   0        0        0      421 2024-02-29 19:41:05.000000 AIPyS-0.0.6/AIPyS/supportFunctions/unpack_h5.py
-drwxrwxrwx   0        0        0        0 2024-04-16 12:59:24.689499 AIPyS-0.0.6/AIPyS.egg-info/
--rw-rw-rw-   0        0        0     3838 2024-04-16 12:59:23.000000 AIPyS-0.0.6/AIPyS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2209 2024-04-16 12:59:23.000000 AIPyS-0.0.6/AIPyS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 12:59:23.000000 AIPyS-0.0.6/AIPyS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2024-04-16 12:59:23.000000 AIPyS-0.0.6/AIPyS.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      338 2024-04-16 12:59:23.000000 AIPyS-0.0.6/AIPyS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-16 12:59:23.000000 AIPyS-0.0.6/AIPyS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2024-04-04 15:36:53.000000 AIPyS-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     3838 2024-04-16 12:59:24.742752 AIPyS-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-16 12:59:24.742752 AIPyS-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1407 2024-04-16 12:58:21.000000 AIPyS-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-16 12:59:24.040378 AIPyS-0.0.6/web_app/
-drwxrwxrwx   0        0        0        0 2024-04-16 12:59:24.592117 AIPyS-0.0.6/web_app/AreasViz/
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.6/web_app/AreasViz/__init__.py
--rw-rw-rw-   0        0        0     4059 2024-04-15 18:20:48.000000 AIPyS-0.0.6/web_app/AreasViz/app.py
-drwxrwxrwx   0        0        0        0 2024-04-16 12:59:24.622325 AIPyS-0.0.6/web_app/Image_labeling/
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.6/web_app/Image_labeling/__init__.py
--rw-rw-rw-   0        0        0     6622 2024-04-11 19:13:34.000000 AIPyS-0.0.6/web_app/Image_labeling/app.py
--rw-rw-rw-   0        0        0     1786 2024-02-28 23:19:27.000000 AIPyS-0.0.6/web_app/Image_labeling/draft.py
-drwxrwxrwx   0        0        0        0 2024-04-16 12:59:24.655640 AIPyS-0.0.6/web_app/TableViz/
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.6/web_app/TableViz/__init__.py
--rw-rw-rw-   0        0        0     4054 2024-03-01 12:56:00.000000 AIPyS-0.0.6/web_app/TableViz/app.py
--rw-rw-rw-   0        0        0     2320 2024-02-28 23:19:27.000000 AIPyS-0.0.6/web_app/TableViz/distplot.py
-drwxrwxrwx   0        0        0        0 2024-04-16 12:59:24.681723 AIPyS-0.0.6/web_app/measure_length/
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.6/web_app/measure_length/__init__.py
--rw-rw-rw-   0        0        0     4549 2024-02-29 19:09:36.000000 AIPyS-0.0.6/web_app/measure_length/app.py
+drwxrwxrwx   0        0        0        0 2024-04-16 13:00:09.713719 AIPyS-0.0.7/
+drwxrwxrwx   0        0        0        0 2024-04-16 13:00:08.967889 AIPyS-0.0.7/AIPyS/
+drwxrwxrwx   0        0        0        0 2024-04-16 13:00:09.256641 AIPyS-0.0.7/AIPyS/CLI/
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.7/AIPyS/CLI/__init__.py
+-rw-rw-rw-   0        0        0     7580 2024-04-15 18:55:22.000000 AIPyS-0.0.7/AIPyS/CLI/aipys.py
+-rw-rw-rw-   0        0        0     1284 2024-04-15 18:53:26.000000 AIPyS-0.0.7/AIPyS/CLI/area_analysis.py
+-rw-rw-rw-   0        0        0     3292 2024-04-16 12:57:00.000000 AIPyS-0.0.7/AIPyS/CLI/loadParameters.py
+-rw-rw-rw-   0        0        0     2761 2024-03-01 16:45:08.000000 AIPyS-0.0.7/AIPyS/CLI/promptParameters.py
+-rw-rw-rw-   0        0        0     9375 2024-04-09 18:42:35.000000 AIPyS-0.0.7/AIPyS/CLI/set_parameters.py
+-rw-rw-rw-   0        0        0      854 2024-02-29 17:57:58.000000 AIPyS-0.0.7/AIPyS/CLI/test.py
+-rw-rw-rw-   0        0        0     1500 2024-03-02 13:49:57.000000 AIPyS-0.0.7/AIPyS/DataLoad.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.7/AIPyS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 13:00:08.923088 AIPyS-0.0.7/AIPyS/classification/
+drwxrwxrwx   0        0        0        0 2024-04-16 13:00:09.302346 AIPyS-0.0.7/AIPyS/classification/CNN/
+-rw-rw-rw-   0        0        0     2501 2024-03-02 20:04:55.000000 AIPyS-0.0.7/AIPyS/classification/CNN/CNN_deploy.py
+-rw-rw-rw-   0        0        0     5086 2024-02-28 23:19:26.000000 AIPyS-0.0.7/AIPyS/classification/CNN/Taining_data_orgenizer.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.7/AIPyS/classification/CNN/__init__.py
+-rw-rw-rw-   0        0        0     1908 2024-02-28 23:19:26.000000 AIPyS-0.0.7/AIPyS/classification/CNN/mapSgRNA.py
+-rw-rw-rw-   0        0        0    18474 2024-02-28 23:19:26.000000 AIPyS-0.0.7/AIPyS/classification/CNN/model_builder.py
+-rw-rw-rw-   0        0        0     8897 2024-02-28 23:19:26.000000 AIPyS-0.0.7/AIPyS/classification/CNN/model_evaluation_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-16 13:00:09.363614 AIPyS-0.0.7/AIPyS/classification/bayes/
+-rw-rw-rw-   0        0        0     2596 2024-02-28 23:19:26.000000 AIPyS-0.0.7/AIPyS/classification/bayes/BayesianModels.py
+-rw-rw-rw-   0        0        0     6221 2024-03-02 14:10:27.000000 AIPyS-0.0.7/AIPyS/classification/bayes/Baysian_deploy.py
+-rw-rw-rw-   0        0        0     7817 2024-04-11 17:07:53.000000 AIPyS-0.0.7/AIPyS/classification/bayes/Baysian_training.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.7/AIPyS/classification/bayes/DisplayImageFrame.py
+-rw-rw-rw-   0        0        0     6145 2024-02-29 21:52:44.000000 AIPyS-0.0.7/AIPyS/classification/bayes/GranulaityMesure.py
+-rw-rw-rw-   0        0        0    18111 2024-04-15 19:16:12.000000 AIPyS-0.0.7/AIPyS/classification/bayes/GranularityDataGen.py
+-rw-rw-rw-   0        0        0     5065 2024-02-28 23:19:26.000000 AIPyS-0.0.7/AIPyS/classification/bayes/GranularityDeploy.py
+-rw-rw-rw-   0        0        0     2024 2024-02-28 23:19:26.000000 AIPyS-0.0.7/AIPyS/classification/bayes/RunningWindow.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.7/AIPyS/classification/bayes/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:37:34.000000 AIPyS-0.0.7/AIPyS/draft.py
+drwxrwxrwx   0        0        0        0 2024-04-16 13:00:08.925080 AIPyS-0.0.7/AIPyS/segmentation/
+drwxrwxrwx   0        0        0        0 2024-04-16 13:00:09.443907 AIPyS-0.0.7/AIPyS/segmentation/cellpose/
+-rw-rw-rw-   0        0        0     2283 2024-02-28 23:19:56.000000 AIPyS-0.0.7/AIPyS/segmentation/cellpose/AIPS_cellpose.py
+-rw-rw-rw-   0        0        0     1666 2024-04-12 18:30:36.000000 AIPyS-0.0.7/AIPyS/segmentation/cellpose/AIPS_cellpse_video_gen.py
+-rw-rw-rw-   0        0        0     2450 2024-03-02 12:03:05.000000 AIPyS-0.0.7/AIPyS/segmentation/cellpose/StackObjects_cellpose.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.7/AIPyS/segmentation/cellpose/__init__.py
+-rw-rw-rw-   0        0        0     4727 2024-04-15 18:01:11.000000 AIPyS-0.0.7/AIPyS/segmentation/cellpose/plotObjectAreas.py
+drwxrwxrwx   0        0        0        0 2024-04-16 13:00:09.456527 AIPyS-0.0.7/AIPyS/segmentation/parametric/
+-rw-rw-rw-   0        0        0     3564 2024-02-28 23:19:27.000000 AIPyS-0.0.7/AIPyS/segmentation/parametric/GlobalSeg.py
+-rw-rw-rw-   0        0        0     2426 2024-02-28 23:19:56.000000 AIPyS-0.0.7/AIPyS/segmentation/parametric/ImageSeqGlobSeg.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.7/AIPyS/segmentation/parametric/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 13:00:09.544976 AIPyS-0.0.7/AIPyS/supportFunctions/
+-rw-rw-rw-   0        0        0     6856 2024-03-02 13:11:22.000000 AIPyS-0.0.7/AIPyS/supportFunctions/AIPS_file_display.py
+-rw-rw-rw-   0        0        0    13755 2024-04-15 18:45:15.000000 AIPyS-0.0.7/AIPyS/supportFunctions/AIPS_functions.py
+-rw-rw-rw-   0        0        0    10310 2024-02-28 23:19:27.000000 AIPyS-0.0.7/AIPyS/supportFunctions/AIPS_granularity.py
+-rw-rw-rw-   0        0        0    14491 2024-02-28 23:19:27.000000 AIPyS-0.0.7/AIPyS/supportFunctions/AIPS_module.py
+-rw-rw-rw-   0        0        0     4250 2024-02-28 23:19:27.000000 AIPyS-0.0.7/AIPyS/supportFunctions/AIPS_simulate.py
+-rw-rw-rw-   0        0        0     7362 2024-02-28 23:19:27.000000 AIPyS-0.0.7/AIPyS/supportFunctions/Display_composit.py
+-rw-rw-rw-   0        0        0     1252 2024-02-28 23:19:27.000000 AIPyS-0.0.7/AIPyS/supportFunctions/GranularityFunc.py
+-rw-rw-rw-   0        0        0    16340 2024-02-28 23:19:27.000000 AIPyS-0.0.7/AIPyS/supportFunctions/Granularity_cellprofiler.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.7/AIPyS/supportFunctions/__init__.py
+-rw-rw-rw-   0        0        0     8046 2024-02-28 23:19:27.000000 AIPyS-0.0.7/AIPyS/supportFunctions/display_and_xml.py
+-rw-rw-rw-   0        0        0      421 2024-02-29 19:41:05.000000 AIPyS-0.0.7/AIPyS/supportFunctions/unpack_h5.py
+drwxrwxrwx   0        0        0        0 2024-04-16 13:00:09.662222 AIPyS-0.0.7/AIPyS.egg-info/
+-rw-rw-rw-   0        0        0     3838 2024-04-16 13:00:08.000000 AIPyS-0.0.7/AIPyS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2209 2024-04-16 13:00:08.000000 AIPyS-0.0.7/AIPyS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 13:00:08.000000 AIPyS-0.0.7/AIPyS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2024-04-16 13:00:08.000000 AIPyS-0.0.7/AIPyS.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      338 2024-04-16 13:00:08.000000 AIPyS-0.0.7/AIPyS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-16 13:00:08.000000 AIPyS-0.0.7/AIPyS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2024-04-04 15:36:53.000000 AIPyS-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     3838 2024-04-16 13:00:09.713719 AIPyS-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-16 13:00:09.713719 AIPyS-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1407 2024-04-16 12:59:53.000000 AIPyS-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 13:00:08.929326 AIPyS-0.0.7/web_app/
+drwxrwxrwx   0        0        0        0 2024-04-16 13:00:09.564283 AIPyS-0.0.7/web_app/AreasViz/
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.7/web_app/AreasViz/__init__.py
+-rw-rw-rw-   0        0        0     4059 2024-04-15 18:20:48.000000 AIPyS-0.0.7/web_app/AreasViz/app.py
+drwxrwxrwx   0        0        0        0 2024-04-16 13:00:09.598511 AIPyS-0.0.7/web_app/Image_labeling/
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.7/web_app/Image_labeling/__init__.py
+-rw-rw-rw-   0        0        0     6622 2024-04-11 19:13:34.000000 AIPyS-0.0.7/web_app/Image_labeling/app.py
+-rw-rw-rw-   0        0        0     1786 2024-02-28 23:19:27.000000 AIPyS-0.0.7/web_app/Image_labeling/draft.py
+drwxrwxrwx   0        0        0        0 2024-04-16 13:00:09.636484 AIPyS-0.0.7/web_app/TableViz/
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.7/web_app/TableViz/__init__.py
+-rw-rw-rw-   0        0        0     4054 2024-03-01 12:56:00.000000 AIPyS-0.0.7/web_app/TableViz/app.py
+-rw-rw-rw-   0        0        0     2320 2024-02-28 23:19:27.000000 AIPyS-0.0.7/web_app/TableViz/distplot.py
+drwxrwxrwx   0        0        0        0 2024-04-16 13:00:09.662222 AIPyS-0.0.7/web_app/measure_length/
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.7/web_app/measure_length/__init__.py
+-rw-rw-rw-   0        0        0     4549 2024-02-29 19:09:36.000000 AIPyS-0.0.7/web_app/measure_length/app.py
```

### Comparing `AIPyS-0.0.6/AIPyS/CLI/aipys.py` & `AIPyS-0.0.7/AIPyS/CLI/aipys.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/AIPyS/CLI/area_analysis.py` & `AIPyS-0.0.7/AIPyS/CLI/area_analysis.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/AIPyS/CLI/loadParameters.py` & `AIPyS-0.0.7/AIPyS/CLI/loadParameters.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/AIPyS/CLI/promptParameters.py` & `AIPyS-0.0.7/AIPyS/CLI/promptParameters.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/AIPyS/CLI/set_parameters.py` & `AIPyS-0.0.7/AIPyS/CLI/set_parameters.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/AIPyS/CLI/test.py` & `AIPyS-0.0.7/AIPyS/CLI/test.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/AIPyS/DataLoad.py` & `AIPyS-0.0.7/AIPyS/DataLoad.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/AIPyS/classification/CNN/CNN_deploy.py` & `AIPyS-0.0.7/AIPyS/classification/CNN/CNN_deploy.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/AIPyS/classification/CNN/Taining_data_orgenizer.py` & `AIPyS-0.0.7/AIPyS/classification/CNN/Taining_data_orgenizer.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/AIPyS/classification/CNN/mapSgRNA.py` & `AIPyS-0.0.7/AIPyS/classification/CNN/mapSgRNA.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/AIPyS/classification/CNN/model_builder.py` & `AIPyS-0.0.7/AIPyS/classification/CNN/model_builder.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/AIPyS/classification/CNN/model_evaluation_utils.py` & `AIPyS-0.0.7/AIPyS/classification/CNN/model_evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/AIPyS/classification/bayes/BayesianModels.py` & `AIPyS-0.0.7/AIPyS/classification/bayes/BayesianModels.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/AIPyS/classification/bayes/Baysian_deploy.py` & `AIPyS-0.0.7/AIPyS/classification/bayes/Baysian_deploy.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/AIPyS/classification/bayes/Baysian_training.py` & `AIPyS-0.0.7/AIPyS/classification/bayes/Baysian_training.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/AIPyS/classification/bayes/GranulaityMesure.py` & `AIPyS-0.0.7/AIPyS/classification/bayes/GranulaityMesure.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/AIPyS/classification/bayes/GranularityDataGen.py` & `AIPyS-0.0.7/AIPyS/classification/bayes/GranularityDataGen.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/AIPyS/classification/bayes/GranularityDeploy.py` & `AIPyS-0.0.7/AIPyS/classification/bayes/GranularityDeploy.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/AIPyS/classification/bayes/RunningWindow.py` & `AIPyS-0.0.7/AIPyS/classification/bayes/RunningWindow.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/AIPyS/segmentation/cellpose/AIPS_cellpose.py` & `AIPyS-0.0.7/AIPyS/segmentation/cellpose/AIPS_cellpose.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/AIPyS/segmentation/cellpose/AIPS_cellpse_video_gen.py` & `AIPyS-0.0.7/AIPyS/segmentation/cellpose/AIPS_cellpse_video_gen.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/AIPyS/segmentation/cellpose/StackObjects_cellpose.py` & `AIPyS-0.0.7/AIPyS/segmentation/cellpose/StackObjects_cellpose.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/AIPyS/segmentation/cellpose/plotObjectAreas.py` & `AIPyS-0.0.7/AIPyS/segmentation/cellpose/plotObjectAreas.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/AIPyS/segmentation/parametric/GlobalSeg.py` & `AIPyS-0.0.7/AIPyS/segmentation/parametric/GlobalSeg.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/AIPyS/segmentation/parametric/ImageSeqGlobSeg.py` & `AIPyS-0.0.7/AIPyS/segmentation/parametric/ImageSeqGlobSeg.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/AIPyS/supportFunctions/AIPS_file_display.py` & `AIPyS-0.0.7/AIPyS/supportFunctions/AIPS_file_display.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/AIPyS/supportFunctions/AIPS_functions.py` & `AIPyS-0.0.7/AIPyS/supportFunctions/AIPS_functions.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/AIPyS/supportFunctions/AIPS_granularity.py` & `AIPyS-0.0.7/AIPyS/supportFunctions/AIPS_granularity.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/AIPyS/supportFunctions/AIPS_module.py` & `AIPyS-0.0.7/AIPyS/supportFunctions/AIPS_module.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/AIPyS/supportFunctions/AIPS_simulate.py` & `AIPyS-0.0.7/AIPyS/supportFunctions/AIPS_simulate.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/AIPyS/supportFunctions/Display_composit.py` & `AIPyS-0.0.7/AIPyS/supportFunctions/Display_composit.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/AIPyS/supportFunctions/GranularityFunc.py` & `AIPyS-0.0.7/AIPyS/supportFunctions/GranularityFunc.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/AIPyS/supportFunctions/Granularity_cellprofiler.py` & `AIPyS-0.0.7/AIPyS/supportFunctions/Granularity_cellprofiler.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/AIPyS/supportFunctions/display_and_xml.py` & `AIPyS-0.0.7/AIPyS/supportFunctions/display_and_xml.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/AIPyS.egg-info/PKG-INFO` & `AIPyS-0.0.7/AIPyS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AIPyS
-Version: 0.0.6
+Version: 0.0.7
 Summary: AI Powered Photoswitchable Screen
 Home-page: 
 Author: Gil Kanfer
 Author-email: gil.kanfer.il@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `AIPyS-0.0.6/AIPyS.egg-info/SOURCES.txt` & `AIPyS-0.0.7/AIPyS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/LICENSE` & `AIPyS-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/PKG-INFO` & `AIPyS-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AIPyS
-Version: 0.0.6
+Version: 0.0.7
 Summary: AI Powered Photoswitchable Screen
 Home-page: 
 Author: Gil Kanfer
 Author-email: gil.kanfer.il@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `AIPyS-0.0.6/setup.py` & `AIPyS-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name="AIPyS",
-    version="0.0.6",
+    version="0.0.7",
     packages=find_packages(include=['AIPyS','AIPyS.CLI','AIPyS.classification.bayes','AIPyS.classification.CNN',
                                     'AIPyS.segmentation.cellpose','AIPyS.segmentation.parametric','AIPyS.supportFunctions',
                                     'web_app.Image_labeling','web_app.measure_length','web_app.measure_length','web_app.TableViz', 'web_app.AreasViz',]),
     install_requires=required,
     entry_points={
         'console_scripts': [
            'aipys=AIPyS.CLI.aipys:main',
```

### Comparing `AIPyS-0.0.6/web_app/AreasViz/app.py` & `AIPyS-0.0.7/web_app/AreasViz/app.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/web_app/Image_labeling/app.py` & `AIPyS-0.0.7/web_app/Image_labeling/app.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/web_app/Image_labeling/draft.py` & `AIPyS-0.0.7/web_app/Image_labeling/draft.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/web_app/TableViz/app.py` & `AIPyS-0.0.7/web_app/TableViz/app.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/web_app/TableViz/distplot.py` & `AIPyS-0.0.7/web_app/TableViz/distplot.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.6/web_app/measure_length/app.py` & `AIPyS-0.0.7/web_app/measure_length/app.py`

 * *Files identical despite different names*

