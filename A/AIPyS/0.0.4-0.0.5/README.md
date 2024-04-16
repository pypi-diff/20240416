# Comparing `tmp/AIPyS-0.0.4.tar.gz` & `tmp/AIPyS-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AIPyS-0.0.4.tar", last modified: Thu Apr 11 17:14:49 2024, max compression
+gzip compressed data, was "AIPyS-0.0.5.tar", last modified: Mon Apr 15 19:41:12 2024, max compression
```

## Comparing `AIPyS-0.0.4.tar` & `AIPyS-0.0.5.tar`

### file list

```diff
@@ -1,75 +1,80 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 17:14:49.822272 AIPyS-0.0.4/
-drwxrwxrwx   0        0        0        0 2024-04-11 17:14:49.077514 AIPyS-0.0.4/AIPyS/
-drwxrwxrwx   0        0        0        0 2024-04-11 17:14:49.364745 AIPyS-0.0.4/AIPyS/CLI/
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.4/AIPyS/CLI/__init__.py
--rw-rw-rw-   0        0        0     7527 2024-04-09 18:32:27.000000 AIPyS-0.0.4/AIPyS/CLI/aipys.py
--rw-rw-rw-   0        0        0     3666 2024-03-02 14:46:53.000000 AIPyS-0.0.4/AIPyS/CLI/loadParameters.py
--rw-rw-rw-   0        0        0     2761 2024-03-01 16:45:08.000000 AIPyS-0.0.4/AIPyS/CLI/promptParameters.py
--rw-rw-rw-   0        0        0     9375 2024-04-09 18:42:35.000000 AIPyS-0.0.4/AIPyS/CLI/set_parameters.py
--rw-rw-rw-   0        0        0      854 2024-02-29 17:57:58.000000 AIPyS-0.0.4/AIPyS/CLI/test.py
--rw-rw-rw-   0        0        0     1500 2024-03-02 13:49:57.000000 AIPyS-0.0.4/AIPyS/DataLoad.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.4/AIPyS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 17:14:49.019666 AIPyS-0.0.4/AIPyS/classification/
-drwxrwxrwx   0        0        0        0 2024-04-11 17:14:49.405752 AIPyS-0.0.4/AIPyS/classification/CNN/
--rw-rw-rw-   0        0        0     2501 2024-03-02 20:04:55.000000 AIPyS-0.0.4/AIPyS/classification/CNN/CNN_deploy.py
--rw-rw-rw-   0        0        0     5086 2024-02-28 23:19:26.000000 AIPyS-0.0.4/AIPyS/classification/CNN/Taining_data_orgenizer.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.4/AIPyS/classification/CNN/__init__.py
--rw-rw-rw-   0        0        0     1908 2024-02-28 23:19:26.000000 AIPyS-0.0.4/AIPyS/classification/CNN/mapSgRNA.py
--rw-rw-rw-   0        0        0    18474 2024-02-28 23:19:26.000000 AIPyS-0.0.4/AIPyS/classification/CNN/model_builder.py
--rw-rw-rw-   0        0        0     8897 2024-02-28 23:19:26.000000 AIPyS-0.0.4/AIPyS/classification/CNN/model_evaluation_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-11 17:14:49.460605 AIPyS-0.0.4/AIPyS/classification/bayes/
--rw-rw-rw-   0        0        0     2596 2024-02-28 23:19:26.000000 AIPyS-0.0.4/AIPyS/classification/bayes/BayesianModels.py
--rw-rw-rw-   0        0        0     6221 2024-03-02 14:10:27.000000 AIPyS-0.0.4/AIPyS/classification/bayes/Baysian_deploy.py
--rw-rw-rw-   0        0        0     7817 2024-04-11 17:07:53.000000 AIPyS-0.0.4/AIPyS/classification/bayes/Baysian_training.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.4/AIPyS/classification/bayes/DisplayImageFrame.py
--rw-rw-rw-   0        0        0     6145 2024-02-29 21:52:44.000000 AIPyS-0.0.4/AIPyS/classification/bayes/GranulaityMesure.py
--rw-rw-rw-   0        0        0    17734 2024-03-02 12:05:52.000000 AIPyS-0.0.4/AIPyS/classification/bayes/GranularityDataGen.py
--rw-rw-rw-   0        0        0     5065 2024-02-28 23:19:26.000000 AIPyS-0.0.4/AIPyS/classification/bayes/GranularityDeploy.py
--rw-rw-rw-   0        0        0     2024 2024-02-28 23:19:26.000000 AIPyS-0.0.4/AIPyS/classification/bayes/RunningWindow.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.4/AIPyS/classification/bayes/__init__.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:37:34.000000 AIPyS-0.0.4/AIPyS/draft.py
-drwxrwxrwx   0        0        0        0 2024-04-11 17:14:49.024653 AIPyS-0.0.4/AIPyS/segmentation/
-drwxrwxrwx   0        0        0        0 2024-04-11 17:14:49.501496 AIPyS-0.0.4/AIPyS/segmentation/cellpose/
--rw-rw-rw-   0        0        0     2283 2024-02-28 23:19:56.000000 AIPyS-0.0.4/AIPyS/segmentation/cellpose/AIPS_cellpose.py
--rw-rw-rw-   0        0        0     1666 2024-02-29 21:42:22.000000 AIPyS-0.0.4/AIPyS/segmentation/cellpose/AIPS_cellpse_video_gen.py
--rw-rw-rw-   0        0        0     2450 2024-03-02 12:03:05.000000 AIPyS-0.0.4/AIPyS/segmentation/cellpose/StackObjects_cellpose.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.4/AIPyS/segmentation/cellpose/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 17:14:49.527426 AIPyS-0.0.4/AIPyS/segmentation/parametric/
--rw-rw-rw-   0        0        0     3564 2024-02-28 23:19:27.000000 AIPyS-0.0.4/AIPyS/segmentation/parametric/GlobalSeg.py
--rw-rw-rw-   0        0        0     2426 2024-02-28 23:19:56.000000 AIPyS-0.0.4/AIPyS/segmentation/parametric/ImageSeqGlobSeg.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.4/AIPyS/segmentation/parametric/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 17:14:49.614628 AIPyS-0.0.4/AIPyS/supportFunctions/
--rw-rw-rw-   0        0        0     6856 2024-03-02 13:11:22.000000 AIPyS-0.0.4/AIPyS/supportFunctions/AIPS_file_display.py
--rw-rw-rw-   0        0        0    11778 2024-03-02 20:08:24.000000 AIPyS-0.0.4/AIPyS/supportFunctions/AIPS_functions.py
--rw-rw-rw-   0        0        0    10310 2024-02-28 23:19:27.000000 AIPyS-0.0.4/AIPyS/supportFunctions/AIPS_granularity.py
--rw-rw-rw-   0        0        0    14491 2024-02-28 23:19:27.000000 AIPyS-0.0.4/AIPyS/supportFunctions/AIPS_module.py
--rw-rw-rw-   0        0        0     4250 2024-02-28 23:19:27.000000 AIPyS-0.0.4/AIPyS/supportFunctions/AIPS_simulate.py
--rw-rw-rw-   0        0        0     7362 2024-02-28 23:19:27.000000 AIPyS-0.0.4/AIPyS/supportFunctions/Display_composit.py
--rw-rw-rw-   0        0        0     1252 2024-02-28 23:19:27.000000 AIPyS-0.0.4/AIPyS/supportFunctions/GranularityFunc.py
--rw-rw-rw-   0        0        0    16340 2024-02-28 23:19:27.000000 AIPyS-0.0.4/AIPyS/supportFunctions/Granularity_cellprofiler.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.4/AIPyS/supportFunctions/__init__.py
--rw-rw-rw-   0        0        0     8046 2024-02-28 23:19:27.000000 AIPyS-0.0.4/AIPyS/supportFunctions/display_and_xml.py
--rw-rw-rw-   0        0        0      421 2024-02-29 19:41:05.000000 AIPyS-0.0.4/AIPyS/supportFunctions/unpack_h5.py
-drwxrwxrwx   0        0        0        0 2024-04-11 17:14:49.731318 AIPyS-0.0.4/AIPyS.egg-info/
--rw-rw-rw-   0        0        0     3821 2024-04-11 17:14:48.000000 AIPyS-0.0.4/AIPyS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2082 2024-04-11 17:14:48.000000 AIPyS-0.0.4/AIPyS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 17:14:48.000000 AIPyS-0.0.4/AIPyS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2024-04-11 17:14:48.000000 AIPyS-0.0.4/AIPyS.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      337 2024-04-11 17:14:48.000000 AIPyS-0.0.4/AIPyS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-11 17:14:48.000000 AIPyS-0.0.4/AIPyS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2024-04-04 15:36:53.000000 AIPyS-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     3821 2024-04-11 17:14:49.817284 AIPyS-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-11 17:14:49.822272 AIPyS-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1386 2024-04-11 17:09:54.000000 AIPyS-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 17:14:49.031636 AIPyS-0.0.4/web_app/
-drwxrwxrwx   0        0        0        0 2024-04-11 17:14:49.638564 AIPyS-0.0.4/web_app/Image_labeling/
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.4/web_app/Image_labeling/__init__.py
--rw-rw-rw-   0        0        0     6115 2024-03-01 12:33:36.000000 AIPyS-0.0.4/web_app/Image_labeling/app.py
--rw-rw-rw-   0        0        0     1786 2024-02-28 23:19:27.000000 AIPyS-0.0.4/web_app/Image_labeling/draft.py
-drwxrwxrwx   0        0        0        0 2024-04-11 17:14:49.690430 AIPyS-0.0.4/web_app/TableViz/
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.4/web_app/TableViz/__init__.py
--rw-rw-rw-   0        0        0     4054 2024-03-01 12:56:00.000000 AIPyS-0.0.4/web_app/TableViz/app.py
--rw-rw-rw-   0        0        0     2320 2024-02-28 23:19:27.000000 AIPyS-0.0.4/web_app/TableViz/distplot.py
-drwxrwxrwx   0        0        0        0 2024-04-11 17:14:49.728326 AIPyS-0.0.4/web_app/measure_length/
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.4/web_app/measure_length/__init__.py
--rw-rw-rw-   0        0        0     4549 2024-02-29 19:09:36.000000 AIPyS-0.0.4/web_app/measure_length/app.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:41:12.933298 AIPyS-0.0.5/
+drwxrwxrwx   0        0        0        0 2024-04-15 19:41:12.272137 AIPyS-0.0.5/AIPyS/
+drwxrwxrwx   0        0        0        0 2024-04-15 19:41:12.545365 AIPyS-0.0.5/AIPyS/CLI/
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.5/AIPyS/CLI/__init__.py
+-rw-rw-rw-   0        0        0     7580 2024-04-15 18:55:22.000000 AIPyS-0.0.5/AIPyS/CLI/aipys.py
+-rw-rw-rw-   0        0        0     1284 2024-04-15 18:53:26.000000 AIPyS-0.0.5/AIPyS/CLI/area_analysis.py
+-rw-rw-rw-   0        0        0     3666 2024-03-02 14:46:53.000000 AIPyS-0.0.5/AIPyS/CLI/loadParameters.py
+-rw-rw-rw-   0        0        0     2761 2024-03-01 16:45:08.000000 AIPyS-0.0.5/AIPyS/CLI/promptParameters.py
+-rw-rw-rw-   0        0        0     9375 2024-04-09 18:42:35.000000 AIPyS-0.0.5/AIPyS/CLI/set_parameters.py
+-rw-rw-rw-   0        0        0      854 2024-02-29 17:57:58.000000 AIPyS-0.0.5/AIPyS/CLI/test.py
+-rw-rw-rw-   0        0        0     1500 2024-03-02 13:49:57.000000 AIPyS-0.0.5/AIPyS/DataLoad.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.5/AIPyS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:41:12.220780 AIPyS-0.0.5/AIPyS/classification/
+drwxrwxrwx   0        0        0        0 2024-04-15 19:41:12.591930 AIPyS-0.0.5/AIPyS/classification/CNN/
+-rw-rw-rw-   0        0        0     2501 2024-03-02 20:04:55.000000 AIPyS-0.0.5/AIPyS/classification/CNN/CNN_deploy.py
+-rw-rw-rw-   0        0        0     5086 2024-02-28 23:19:26.000000 AIPyS-0.0.5/AIPyS/classification/CNN/Taining_data_orgenizer.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.5/AIPyS/classification/CNN/__init__.py
+-rw-rw-rw-   0        0        0     1908 2024-02-28 23:19:26.000000 AIPyS-0.0.5/AIPyS/classification/CNN/mapSgRNA.py
+-rw-rw-rw-   0        0        0    18474 2024-02-28 23:19:26.000000 AIPyS-0.0.5/AIPyS/classification/CNN/model_builder.py
+-rw-rw-rw-   0        0        0     8897 2024-02-28 23:19:26.000000 AIPyS-0.0.5/AIPyS/classification/CNN/model_evaluation_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:41:12.639644 AIPyS-0.0.5/AIPyS/classification/bayes/
+-rw-rw-rw-   0        0        0     2596 2024-02-28 23:19:26.000000 AIPyS-0.0.5/AIPyS/classification/bayes/BayesianModels.py
+-rw-rw-rw-   0        0        0     6221 2024-03-02 14:10:27.000000 AIPyS-0.0.5/AIPyS/classification/bayes/Baysian_deploy.py
+-rw-rw-rw-   0        0        0     7817 2024-04-11 17:07:53.000000 AIPyS-0.0.5/AIPyS/classification/bayes/Baysian_training.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.5/AIPyS/classification/bayes/DisplayImageFrame.py
+-rw-rw-rw-   0        0        0     6145 2024-02-29 21:52:44.000000 AIPyS-0.0.5/AIPyS/classification/bayes/GranulaityMesure.py
+-rw-rw-rw-   0        0        0    18111 2024-04-15 19:16:12.000000 AIPyS-0.0.5/AIPyS/classification/bayes/GranularityDataGen.py
+-rw-rw-rw-   0        0        0     5065 2024-02-28 23:19:26.000000 AIPyS-0.0.5/AIPyS/classification/bayes/GranularityDeploy.py
+-rw-rw-rw-   0        0        0     2024 2024-02-28 23:19:26.000000 AIPyS-0.0.5/AIPyS/classification/bayes/RunningWindow.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.5/AIPyS/classification/bayes/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:37:34.000000 AIPyS-0.0.5/AIPyS/draft.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:41:12.223773 AIPyS-0.0.5/AIPyS/segmentation/
+drwxrwxrwx   0        0        0        0 2024-04-15 19:41:12.703848 AIPyS-0.0.5/AIPyS/segmentation/cellpose/
+-rw-rw-rw-   0        0        0     2283 2024-02-28 23:19:56.000000 AIPyS-0.0.5/AIPyS/segmentation/cellpose/AIPS_cellpose.py
+-rw-rw-rw-   0        0        0     1666 2024-04-12 18:30:36.000000 AIPyS-0.0.5/AIPyS/segmentation/cellpose/AIPS_cellpse_video_gen.py
+-rw-rw-rw-   0        0        0     2450 2024-03-02 12:03:05.000000 AIPyS-0.0.5/AIPyS/segmentation/cellpose/StackObjects_cellpose.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.5/AIPyS/segmentation/cellpose/__init__.py
+-rw-rw-rw-   0        0        0     4727 2024-04-15 18:01:11.000000 AIPyS-0.0.5/AIPyS/segmentation/cellpose/plotObjectAreas.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:41:12.711985 AIPyS-0.0.5/AIPyS/segmentation/parametric/
+-rw-rw-rw-   0        0        0     3564 2024-02-28 23:19:27.000000 AIPyS-0.0.5/AIPyS/segmentation/parametric/GlobalSeg.py
+-rw-rw-rw-   0        0        0     2426 2024-02-28 23:19:56.000000 AIPyS-0.0.5/AIPyS/segmentation/parametric/ImageSeqGlobSeg.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.5/AIPyS/segmentation/parametric/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:41:12.781718 AIPyS-0.0.5/AIPyS/supportFunctions/
+-rw-rw-rw-   0        0        0     6856 2024-03-02 13:11:22.000000 AIPyS-0.0.5/AIPyS/supportFunctions/AIPS_file_display.py
+-rw-rw-rw-   0        0        0    13755 2024-04-15 18:45:15.000000 AIPyS-0.0.5/AIPyS/supportFunctions/AIPS_functions.py
+-rw-rw-rw-   0        0        0    10310 2024-02-28 23:19:27.000000 AIPyS-0.0.5/AIPyS/supportFunctions/AIPS_granularity.py
+-rw-rw-rw-   0        0        0    14491 2024-02-28 23:19:27.000000 AIPyS-0.0.5/AIPyS/supportFunctions/AIPS_module.py
+-rw-rw-rw-   0        0        0     4250 2024-02-28 23:19:27.000000 AIPyS-0.0.5/AIPyS/supportFunctions/AIPS_simulate.py
+-rw-rw-rw-   0        0        0     7362 2024-02-28 23:19:27.000000 AIPyS-0.0.5/AIPyS/supportFunctions/Display_composit.py
+-rw-rw-rw-   0        0        0     1252 2024-02-28 23:19:27.000000 AIPyS-0.0.5/AIPyS/supportFunctions/GranularityFunc.py
+-rw-rw-rw-   0        0        0    16340 2024-02-28 23:19:27.000000 AIPyS-0.0.5/AIPyS/supportFunctions/Granularity_cellprofiler.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.5/AIPyS/supportFunctions/__init__.py
+-rw-rw-rw-   0        0        0     8046 2024-02-28 23:19:27.000000 AIPyS-0.0.5/AIPyS/supportFunctions/display_and_xml.py
+-rw-rw-rw-   0        0        0      421 2024-02-29 19:41:05.000000 AIPyS-0.0.5/AIPyS/supportFunctions/unpack_h5.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:41:12.898156 AIPyS-0.0.5/AIPyS.egg-info/
+-rw-rw-rw-   0        0        0     3846 2024-04-15 19:41:11.000000 AIPyS-0.0.5/AIPyS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2209 2024-04-15 19:41:12.000000 AIPyS-0.0.5/AIPyS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 19:41:11.000000 AIPyS-0.0.5/AIPyS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2024-04-15 19:41:11.000000 AIPyS-0.0.5/AIPyS.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      346 2024-04-15 19:41:11.000000 AIPyS-0.0.5/AIPyS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-15 19:41:11.000000 AIPyS-0.0.5/AIPyS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2024-04-04 15:36:53.000000 AIPyS-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     3846 2024-04-15 19:41:12.931303 AIPyS-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-15 19:41:12.934295 AIPyS-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1407 2024-04-15 19:40:31.000000 AIPyS-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:41:12.227890 AIPyS-0.0.5/web_app/
+drwxrwxrwx   0        0        0        0 2024-04-15 19:41:12.804087 AIPyS-0.0.5/web_app/AreasViz/
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.5/web_app/AreasViz/__init__.py
+-rw-rw-rw-   0        0        0     4059 2024-04-15 18:20:48.000000 AIPyS-0.0.5/web_app/AreasViz/app.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:41:12.831355 AIPyS-0.0.5/web_app/Image_labeling/
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.5/web_app/Image_labeling/__init__.py
+-rw-rw-rw-   0        0        0     6622 2024-04-11 19:13:34.000000 AIPyS-0.0.5/web_app/Image_labeling/app.py
+-rw-rw-rw-   0        0        0     1786 2024-02-28 23:19:27.000000 AIPyS-0.0.5/web_app/Image_labeling/draft.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:41:12.867120 AIPyS-0.0.5/web_app/TableViz/
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.5/web_app/TableViz/__init__.py
+-rw-rw-rw-   0        0        0     4054 2024-03-01 12:56:00.000000 AIPyS-0.0.5/web_app/TableViz/app.py
+-rw-rw-rw-   0        0        0     2320 2024-02-28 23:19:27.000000 AIPyS-0.0.5/web_app/TableViz/distplot.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:41:12.895165 AIPyS-0.0.5/web_app/measure_length/
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.5/web_app/measure_length/__init__.py
+-rw-rw-rw-   0        0        0     4549 2024-02-29 19:09:36.000000 AIPyS-0.0.5/web_app/measure_length/app.py
```

### Comparing `AIPyS-0.0.4/AIPyS/CLI/aipys.py` & `AIPyS-0.0.5/AIPyS/CLI/aipys.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from AIPyS.classification.bayes.GranularityDataGen import GranularityDataGen_cp
 from AIPyS.classification.bayes.Baysian_training import Baysian_training
 from AIPyS.classification.bayes.Baysian_deploy import BayesDeploy
 from AIPyS.supportFunctions.unpack_h5 import parametersInspec
 from AIPyS.CLI.set_parameters import update_auto_parameters
 
 
+
 # location of parameters file
 user_parameters_path = os.path.join(Path.home(), '.AIPyS', 'parameters.h5')
 
 def run(option):
     if option == "measDia":
         parameters = parametersInspec(option,user_parameters_path)
         image_name = parameters["Image_name"]
@@ -33,29 +34,30 @@
         app.run_server()
     elif option == "cp_seg_video":
         parameters = parametersInspec(option,user_parameters_path)
         files = glob.glob(parameters['data_dir'] + "\\*.tif")
         if parameters['channels']=='greyscale':
             channels = [0,0]
         else:
-            print('chanlles are missing')
+            print('channels are missing')
         CellPoseSeg(diameter =  parameters['diameter'],videoName = parameters['videoName'], model_type = parameters['model_type'], channels = channels,
                     Image_name = files[:parameters['imagesN']], outPath = parameters['outPath'])
     elif option == "cp_gran_video":
         # Placeholder for cp_gran_video option - creates a video of kernel opening
         parameters = parametersInspec(option,user_parameters_path)
         if parameters['channels']=='greyscale':
             channels = [0,0]
         else:
             print('channels are missing')
         GranulaityMesure_cp(start_kernel = parameters['start_kernel'],end_karnel = parameters['end_karnel'],kernel_size = parameters['kernel_size'],
                             extract_pixel = parameters['extract_pixel'],outputImageSize = parameters['outputImageSize'], resize_pixel = parameters['resize_pixel'],
                             videoName = parameters['videoName'], model_type = parameters['model_type'], channels = parameters['channels'],
                             Image_name = parameters['Image_name'], outPath = parameters['outPath'],diameter =  parameters['diameter']) # save video form cell segmentation
     elif option == "cp_gran_table_gen":
+        ### trainingDataPath needs to be updated 
         parameters = parametersInspec(option,user_parameters_path)
         if parameters['channels']=='greyscale':
             channels = [0,0]
         else:
             print('channels are missing')
         pattern = os.path.join(parameters['trainingDataPath'], '**', '*.tif')
         # List all the .tif files
```

### Comparing `AIPyS-0.0.4/AIPyS/CLI/loadParameters.py` & `AIPyS-0.0.5/AIPyS/CLI/loadParameters.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.4/AIPyS/CLI/promptParameters.py` & `AIPyS-0.0.5/AIPyS/CLI/promptParameters.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.4/AIPyS/CLI/set_parameters.py` & `AIPyS-0.0.5/AIPyS/CLI/set_parameters.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.4/AIPyS/CLI/test.py` & `AIPyS-0.0.5/AIPyS/CLI/test.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.4/AIPyS/DataLoad.py` & `AIPyS-0.0.5/AIPyS/DataLoad.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.4/AIPyS/classification/CNN/CNN_deploy.py` & `AIPyS-0.0.5/AIPyS/classification/CNN/CNN_deploy.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.4/AIPyS/classification/CNN/Taining_data_orgenizer.py` & `AIPyS-0.0.5/AIPyS/classification/CNN/Taining_data_orgenizer.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.4/AIPyS/classification/CNN/mapSgRNA.py` & `AIPyS-0.0.5/AIPyS/classification/CNN/mapSgRNA.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.4/AIPyS/classification/CNN/model_builder.py` & `AIPyS-0.0.5/AIPyS/classification/CNN/model_builder.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.4/AIPyS/classification/CNN/model_evaluation_utils.py` & `AIPyS-0.0.5/AIPyS/classification/CNN/model_evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.4/AIPyS/classification/bayes/BayesianModels.py` & `AIPyS-0.0.5/AIPyS/classification/bayes/BayesianModels.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.4/AIPyS/classification/bayes/Baysian_deploy.py` & `AIPyS-0.0.5/AIPyS/classification/bayes/Baysian_deploy.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.4/AIPyS/classification/bayes/Baysian_training.py` & `AIPyS-0.0.5/AIPyS/classification/bayes/Baysian_training.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.4/AIPyS/classification/bayes/GranulaityMesure.py` & `AIPyS-0.0.5/AIPyS/classification/bayes/GranulaityMesure.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.4/AIPyS/classification/bayes/GranularityDataGen.py` & `AIPyS-0.0.5/AIPyS/classification/bayes/GranularityDataGen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from AIPyS.classification.bayes.RunningWindow import RunningWindow
 from AIPyS.supportFunctions.GranularityFunc import openingOperation,resize,imageToRGB
 from AIPyS.supportFunctions.AIPS_file_display import Compsite_display
 from AIPyS.segmentation.cellpose.StackObjects_cellpose import StackObjects_cellpose 
-import numpy as np
+from AIPyS.supportFunctions.AIPS_functions import areaThreshold
 import string
 import cv2
 import pdb
 import random
+import numpy as np
 import skimage
 import os
 import pandas as pd
 import matplotlib.pyplot as plt
 from matplotlib.backends.backend_pdf import PdfPages
 from PIL import Image, ImageEnhance, ImageDraw,ImageFont
 from IPython.display import clear_output
@@ -303,14 +304,19 @@
         dfGran = {'name':[],'ratio':[],'intensity':[],'sd':[],'maskArea':[]}
         c = 0
         for image_path in image_name_list:
             image = skimage.io.imread(image_path)
             image_name = self.generate_random_string(7)
             # Initiate cellpose segmentation
             mask, table = self.cellpose_segmentation(image_input = image)
+            # add MLE cleaning area step if area is smaller then th skip it:
+            th_area = areaThreshold(arr_area = table.area.values)
+            if th_area=="na":
+                #incase MLE fail
+                th_area = 1
             # create original image:
             #print('-' * c, end = '\r')
             clear_output(wait=True)
             for idx, (index, row) in enumerate(table.iterrows()):
                 if idx % 10 == 0:
                     c += 1
                     print('.'*c, end = '\r')
@@ -319,14 +325,16 @@
                     stack_img, stack_mask = self.stackObjects_cellpose_ebimage_parametrs_method(image,mask,table,img_label)
                 except:
                     continue
                 if stack_img is None:
                     continue
                 intensity =  np.mean(stack_img)
                 maskArea = row['area']
+                if maskArea < th_area:
+                    continue
                 sd = self.sdCalc(stack_img,intensity)
                 #image intensity and sd before opening:
                 # # video gen
                 imageDecy = openingOperation(kernel = self.kernelGran, image = stack_img)
                 ratio = np.mean(imageDecy)/intensity
                 dfGran['name'].append(image_name + f'_{idx}.png')
                 dfGran['ratio'].append(ratio)
@@ -339,11 +347,11 @@
                 PIL_image = PIL_image_grey.convert('RGB') # for getting a grey scale with red text
                 draw = ImageDraw.Draw(PIL_image)
                 font_size = 24
                 font = ImageFont.truetype("arial.ttf", font_size)  # Adjust as necessary
                 draw.text((5, 5),f'Imagename:{image_name}_{idx} \n Ratio:{np.round(ratio,4)} \n Area: {np.round(maskArea,4)}', 'red',font=font)
                 PIL_image.save(os.path.join(ImagePath,image_name + '_' + f'{idx}.png'))
         dfGran = pd.DataFrame(dfGran)
-        dfGran['label'] = 0
+        dfGran['label'] = "na"
         dfGran.to_csv(os.path.join(DataPath,'imageseq_data.csv'))
```

### Comparing `AIPyS-0.0.4/AIPyS/classification/bayes/GranularityDeploy.py` & `AIPyS-0.0.5/AIPyS/classification/bayes/GranularityDeploy.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.4/AIPyS/classification/bayes/RunningWindow.py` & `AIPyS-0.0.5/AIPyS/classification/bayes/RunningWindow.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.4/AIPyS/segmentation/cellpose/AIPS_cellpose.py` & `AIPyS-0.0.5/AIPyS/segmentation/cellpose/AIPS_cellpose.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.4/AIPyS/segmentation/cellpose/AIPS_cellpse_video_gen.py` & `AIPyS-0.0.5/AIPyS/segmentation/cellpose/AIPS_cellpse_video_gen.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.4/AIPyS/segmentation/cellpose/StackObjects_cellpose.py` & `AIPyS-0.0.5/AIPyS/segmentation/cellpose/StackObjects_cellpose.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.4/AIPyS/segmentation/parametric/GlobalSeg.py` & `AIPyS-0.0.5/AIPyS/segmentation/parametric/GlobalSeg.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.4/AIPyS/segmentation/parametric/ImageSeqGlobSeg.py` & `AIPyS-0.0.5/AIPyS/segmentation/parametric/ImageSeqGlobSeg.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.4/AIPyS/supportFunctions/AIPS_file_display.py` & `AIPyS-0.0.5/AIPyS/supportFunctions/AIPS_file_display.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.4/AIPyS/supportFunctions/AIPS_functions.py` & `AIPyS-0.0.5/AIPyS/supportFunctions/AIPS_functions.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from skimage.filters import threshold_local
 from scipy.ndimage.morphology import binary_opening
 from skimage import io, filters, measure, color, img_as_ubyte
 import skimage.morphology as sm
 from skimage.segmentation import watershed
 from skimage import measure
 from skimage.exposure import rescale_intensity
+from sklearn.mixture import GaussianMixture
 import os
 import pandas as pd
 from scipy.ndimage.morphology import binary_fill_holes
 import base64
 from datetime import datetime
 import re
 from AIPyS.supportFunctions.display_and_xml import unique_rand
@@ -293,7 +294,52 @@
     :param table: keep all the object which are predicted above the threshold
     :return: ROI image mask of selected objects
     '''
     nmask = np.zeros_like(mask)
     for label in table.index.values:
         nmask[mask == label] = label
     return nmask
+
+def areaThreshold(arr_area):
+    y = np.array(arr_area).reshape(-1, 1)  # Reshape data to 2D array required by GMM
+    # Define the range of components to test
+    n_components = np.arange(1, 3)
+    # Fit GMM models for 1 and 2 components
+    models = [GaussianMixture(n_components=n, random_state=42).fit(y) for n in n_components]
+    # Evaluate models using Bayesian Information Criterion (BIC)
+    BIC_scores = [model.bic(y) for model in models]
+
+    # # Plot BIC scores to visualize the best model
+    # plt.figure(figsize=(8, 4))
+    # plt.plot(n_components, BIC_scores, marker='o')
+    # plt.title('BIC Scores by Number of Components')
+    # plt.xlabel('Number of Components')
+    # plt.ylabel('BIC Score')
+    # plt.xticks(n_components)
+    # plt.show()
+
+    # Select the model with the lowest BIC
+    best_model = models[np.argmin(BIC_scores)]
+
+    # Assuming the best model has two components (as expected)
+    #if best_model.n_components == 2:
+    means = np.sort(best_model.means_.flatten())
+    std_dev = np.sqrt(best_model.covariances_.flatten())
+        # Estimate a potential threshold
+    threshold = (means[0] + means[1]) / 2
+        # print(f"Estimated threshold between populations: {threshold}")
+
+        # # Optionally, plot the distribution and the threshold
+        # plt.hist(y, bins=30, density=True, alpha=0.6, color='g')
+        # xmin, xmax = plt.xlim()
+        # x = np.linspace(xmin, xmax, 100)
+        # for mean, std in zip(means, std_dev):
+        #     p = np.exp(-(x - mean)**2 / (2 * std**2)) / (np.sqrt(2 * np.pi) * std)
+        #     plt.plot(x, p, 'k', linewidth=2)
+        # plt.axvline(x=threshold, color='red', linestyle='dashed', linewidth=2)
+        # plt.title('Fit results and estimated threshold')
+        # plt.show()
+    if isinstance(threshold, (int, float)) and threshold > 0:
+        return threshold
+    else:
+        return "na"
+
```

### Comparing `AIPyS-0.0.4/AIPyS/supportFunctions/AIPS_granularity.py` & `AIPyS-0.0.5/AIPyS/supportFunctions/AIPS_granularity.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.4/AIPyS/supportFunctions/AIPS_module.py` & `AIPyS-0.0.5/AIPyS/supportFunctions/AIPS_module.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.4/AIPyS/supportFunctions/AIPS_simulate.py` & `AIPyS-0.0.5/AIPyS/supportFunctions/AIPS_simulate.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.4/AIPyS/supportFunctions/Display_composit.py` & `AIPyS-0.0.5/AIPyS/supportFunctions/Display_composit.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.4/AIPyS/supportFunctions/GranularityFunc.py` & `AIPyS-0.0.5/AIPyS/supportFunctions/GranularityFunc.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.4/AIPyS/supportFunctions/Granularity_cellprofiler.py` & `AIPyS-0.0.5/AIPyS/supportFunctions/Granularity_cellprofiler.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.4/AIPyS/supportFunctions/display_and_xml.py` & `AIPyS-0.0.5/AIPyS/supportFunctions/display_and_xml.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.4/AIPyS.egg-info/PKG-INFO` & `AIPyS-0.0.5/AIPyS.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AIPyS
-Version: 0.0.4
+Version: 0.0.5
 Summary: AI Powered Photoswitchable Screen
 Home-page: 
 Author: Gil Kanfer
 Author-email: gil.kanfer.il@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,14 +32,15 @@
 Requires-Dist: dash
 Requires-Dist: dash-core-components
 Requires-Dist: dash-html-components
 Requires-Dist: dash-renderer
 Requires-Dist: dash-table
 Requires-Dist: dash-bootstrap-components
 Requires-Dist: dash_canvas
+Requires-Dist: dash_daq
 Requires-Dist: plotly_express
 
 
 ---
 
 # AI Powered Photoswitchable Screen (AIPyS) Version 2
```

### Comparing `AIPyS-0.0.4/AIPyS.egg-info/SOURCES.txt` & `AIPyS-0.0.5/AIPyS.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 AIPyS.egg-info/SOURCES.txt
 AIPyS.egg-info/dependency_links.txt
 AIPyS.egg-info/entry_points.txt
 AIPyS.egg-info/requires.txt
 AIPyS.egg-info/top_level.txt
 AIPyS/CLI/__init__.py
 AIPyS/CLI/aipys.py
+AIPyS/CLI/area_analysis.py
 AIPyS/CLI/loadParameters.py
 AIPyS/CLI/promptParameters.py
 AIPyS/CLI/set_parameters.py
 AIPyS/CLI/test.py
 AIPyS/classification/CNN/CNN_deploy.py
 AIPyS/classification/CNN/Taining_data_orgenizer.py
 AIPyS/classification/CNN/__init__.py
@@ -30,28 +31,31 @@
 AIPyS/classification/bayes/GranularityDeploy.py
 AIPyS/classification/bayes/RunningWindow.py
 AIPyS/classification/bayes/__init__.py
 AIPyS/segmentation/cellpose/AIPS_cellpose.py
 AIPyS/segmentation/cellpose/AIPS_cellpse_video_gen.py
 AIPyS/segmentation/cellpose/StackObjects_cellpose.py
 AIPyS/segmentation/cellpose/__init__.py
+AIPyS/segmentation/cellpose/plotObjectAreas.py
 AIPyS/segmentation/parametric/GlobalSeg.py
 AIPyS/segmentation/parametric/ImageSeqGlobSeg.py
 AIPyS/segmentation/parametric/__init__.py
 AIPyS/supportFunctions/AIPS_file_display.py
 AIPyS/supportFunctions/AIPS_functions.py
 AIPyS/supportFunctions/AIPS_granularity.py
 AIPyS/supportFunctions/AIPS_module.py
 AIPyS/supportFunctions/AIPS_simulate.py
 AIPyS/supportFunctions/Display_composit.py
 AIPyS/supportFunctions/GranularityFunc.py
 AIPyS/supportFunctions/Granularity_cellprofiler.py
 AIPyS/supportFunctions/__init__.py
 AIPyS/supportFunctions/display_and_xml.py
 AIPyS/supportFunctions/unpack_h5.py
+web_app/AreasViz/__init__.py
+web_app/AreasViz/app.py
 web_app/Image_labeling/__init__.py
 web_app/Image_labeling/app.py
 web_app/Image_labeling/draft.py
 web_app/TableViz/__init__.py
 web_app/TableViz/app.py
 web_app/TableViz/distplot.py
 web_app/measure_length/__init__.py
```

### Comparing `AIPyS-0.0.4/LICENSE` & `AIPyS-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.4/PKG-INFO` & `AIPyS-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AIPyS
-Version: 0.0.4
+Version: 0.0.5
 Summary: AI Powered Photoswitchable Screen
 Home-page: 
 Author: Gil Kanfer
 Author-email: gil.kanfer.il@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,14 +32,15 @@
 Requires-Dist: dash
 Requires-Dist: dash-core-components
 Requires-Dist: dash-html-components
 Requires-Dist: dash-renderer
 Requires-Dist: dash-table
 Requires-Dist: dash-bootstrap-components
 Requires-Dist: dash_canvas
+Requires-Dist: dash_daq
 Requires-Dist: plotly_express
 
 
 ---
 
 # AI Powered Photoswitchable Screen (AIPyS) Version 2
```

### Comparing `AIPyS-0.0.4/setup.py` & `AIPyS-0.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name="AIPyS",
-    version="0.0.4",
+    version="0.0.5",
     packages=find_packages(include=['AIPyS','AIPyS.CLI','AIPyS.classification.bayes','AIPyS.classification.CNN',
                                     'AIPyS.segmentation.cellpose','AIPyS.segmentation.parametric','AIPyS.supportFunctions',
-                                    'web_app.Image_labeling','web_app.measure_length','web_app.measure_length','web_app.TableViz']),
+                                    'web_app.Image_labeling','web_app.measure_length','web_app.measure_length','web_app.TableViz', 'web_app.AreasViz',]),
     install_requires=required,
     entry_points={
         'console_scripts': [
            'aipys=AIPyS.CLI.aipys:main',  
            'updateParameters=AIPyS.CLI.set_parameters:main',
             'load-parameters=AIPyS.CLI.loadParameters:main', 
             ],
```

### Comparing `AIPyS-0.0.4/web_app/Image_labeling/app.py` & `AIPyS-0.0.5/web_app/Image_labeling/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #%%
 import dash
 from dash import html
 from dash import dash_table, dcc
 from dash.dependencies import Input, Output
+import dash_daq as daq
 #import dash_core_components as dcc
 from dash import State
 from dash.exceptions import PreventUpdate
 import dash_bootstrap_components as dbc
 import pandas as pd
 import sys
 import numpy as np
@@ -83,16 +84,22 @@
               row_selectable="single",
               editable = True,
               page_size=10,
               page_current = 0,
               page_action='native',
               row_deletable=True,
               cell_selectable=True),
-              dbc.Button('Save data', id='save-button', color="danger", n_clicks=0, active=True),
-              dcc.Loading(html.Div(id='load-csv-file'), type="circle", style={'height': '100%', 'width': '100%'}),
+               html.Div([
+                daq.BooleanSwitch(id='my-boolean-switch',
+                                label="Null label remove",
+                                labelPosition="top",
+                                on=False),
+                dbc.Button('Save data', id='save-button', color="danger", n_clicks=0, active=True),
+                dcc.Loading(html.Div(id='load-csv-file'), type="circle", style={'height': '100%', 'width': '100%'}),
+                          ],style={'display': 'flex', 'flex-direction': 'row'})
           ],style={'flex': '1', 'display': 'flex', 'flex-direction': 'column'}),
           html.Div([
             html.Div(id='img-container')
           ], style={'flex': '1'}),
           html.Div(id='temp-contain'),
   ],style={'display': 'flex', 'flex-direction': 'row'})
 
@@ -124,23 +131,27 @@
       img = openImageToPX(os.path.join(imagePath,img_name))
       return [dcc.Graph(id="disp1",figure=img)]
     raise PreventUpdate
 
   @app.callback(
     Output('load-csv-file', 'children'),
     [Input('save-button', 'n_clicks'),
+     Input('my-boolean-switch','on'),
     State('table', 'data')],
     prevent_initial_call=True,
   )
-  def save_data(n,curr_table):
+  def save_data(n,on,curr_table):
     # Handler for data update; includes save logic as needed
     if n is None:
       return dash.no_update
     else:
       df_curr = pd.DataFrame(curr_table).reset_index()
+      if on:
+        # remove all the rows with no label
+        df_curr = df_curr[df_curr['label'] != 'na']
       df_curr.to_csv(os.path.join(dataPath,'imageseq_data.csv'),index=False)
       return "data is saved"
   return app
```

### Comparing `AIPyS-0.0.4/web_app/Image_labeling/draft.py` & `AIPyS-0.0.5/web_app/Image_labeling/draft.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.4/web_app/TableViz/app.py` & `AIPyS-0.0.5/web_app/TableViz/app.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.4/web_app/TableViz/distplot.py` & `AIPyS-0.0.5/web_app/TableViz/distplot.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.4/web_app/measure_length/app.py` & `AIPyS-0.0.5/web_app/measure_length/app.py`

 * *Files identical despite different names*

