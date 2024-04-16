# Comparing `tmp/swane-0.0.6.tar.gz` & `tmp/swane-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swane-0.0.6.tar", last modified: Mon Aug  7 15:05:13 2023, max compression
+gzip compressed data, was "swane-0.1.0.tar", last modified: Tue Apr 16 15:37:23 2024, max compression
```

## Comparing `swane-0.0.6.tar` & `swane-0.1.0.tar`

### file list

```diff
@@ -1,95 +1,107 @@
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-08-07 15:05:13.622750 swane-0.0.6/
--rw-rw-r--   0 mau       (1000) mau       (1000)     1976 2023-03-29 17:07:54.000000 swane-0.0.6/LICENSE
--rw-rw-r--   0 mau       (1000) mau       (1000)      184 2023-03-29 17:07:54.000000 swane-0.0.6/MANIFEST.in
--rw-rw-r--   0 mau       (1000) mau       (1000)      427 2023-08-07 15:05:13.622750 swane-0.0.6/PKG-INFO
--rw-rw-r--   0 mau       (1000) mau       (1000)     7360 2023-08-07 13:21:41.000000 swane-0.0.6/README.md
--rw-rw-r--   0 mau       (1000) mau       (1000)       38 2023-08-07 15:05:13.626750 swane-0.0.6/setup.cfg
--rw-rw-r--   0 mau       (1000) mau       (1000)     1258 2023-08-07 15:03:55.000000 swane-0.0.6/setup.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-08-07 15:05:13.618750 swane-0.0.6/swane/
--rw-rw-r--   0 mau       (1000) mau       (1000)       46 2023-08-07 15:05:08.000000 swane-0.0.6/swane/__init__.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2068 2023-04-29 14:28:42.000000 swane-0.0.6/swane/__main__.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-08-07 15:05:13.618750 swane-0.0.6/swane/nipype_pipeline/
--rw-rw-r--   0 mau       (1000) mau       (1000)    18907 2023-08-07 13:21:41.000000 swane-0.0.6/swane/nipype_pipeline/MainWorkflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.6/swane/nipype_pipeline/__init__.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-08-07 15:05:13.618750 swane-0.0.6/swane/nipype_pipeline/engine/
--rw-rw-r--   0 mau       (1000) mau       (1000)     7906 2023-06-11 04:41:26.000000 swane-0.0.6/swane/nipype_pipeline/engine/CustomWorkflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2795 2023-04-16 08:37:06.000000 swane-0.0.6/swane/nipype_pipeline/engine/MonitoredMultiProcPlugin.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      405 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/engine/NodeListEntry.py
--rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.6/swane/nipype_pipeline/engine/__init__.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-08-07 15:05:13.622750 swane-0.0.6/swane/nipype_pipeline/nodes/
--rw-rw-r--   0 mau       (1000) mau       (1000)     2537 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/AsymmetryIndex.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2263 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/CustomBEDPOSTX5.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1477 2023-06-12 13:39:18.000000 swane-0.0.6/swane/nipype_pipeline/nodes/CustomDcm2niix.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      489 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/CustomDilateImage.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      661 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/CustomLabel2Vol.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      923 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/CustomProbTrackX2.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2356 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/CustomSliceTimer.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2437 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/DeleteVolumes.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2737 2023-08-07 13:21:41.000000 swane-0.0.6/swane/nipype_pipeline/nodes/FLAT1OutliersMask.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     4520 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/FMRIGenSpec.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2506 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/ForceOrient.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      458 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/FslCluster.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1600 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/FslNVols.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1601 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/GetNiftiTR.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1650 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/MergeTargets.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1849 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/Orient.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1400 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/RandomSeedGenerator.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2741 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/SegmentHA.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     3247 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/SumMultiTracks.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1292 2023-05-29 14:38:12.000000 swane-0.0.6/swane/nipype_pipeline/nodes/SumMultiVols.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1580 2023-05-29 14:38:12.000000 swane-0.0.6/swane/nipype_pipeline/nodes/TTest.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     3025 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/ThrROI.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2378 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/VenousCheck.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2703 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/Zscore.py
--rw-rw-r--   0 mau       (1000) mau       (1000)       25 2023-03-29 17:07:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/__init__.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      178 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/utils.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-08-07 15:05:13.622750 swane-0.0.6/swane/nipype_pipeline/workflows/
--rw-rw-r--   0 mau       (1000) mau       (1000)    14190 2023-08-07 13:21:41.000000 swane-0.0.6/swane/nipype_pipeline/workflows/FLAT1_workflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.6/swane/nipype_pipeline/workflows/__init__.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     7912 2023-08-07 13:21:41.000000 swane-0.0.6/swane/nipype_pipeline/workflows/dti_preproc_workflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)    11783 2023-05-29 14:38:12.000000 swane-0.0.6/swane/nipype_pipeline/workflows/freesurfer_asymmetry_index_workflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     8381 2023-05-29 06:41:18.000000 swane-0.0.6/swane/nipype_pipeline/workflows/freesurfer_workflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)    10956 2023-04-04 03:17:58.000000 swane-0.0.6/swane/nipype_pipeline/workflows/func_map_workflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     3504 2023-04-02 08:01:53.000000 swane-0.0.6/swane/nipype_pipeline/workflows/linear_reg_workflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     3132 2023-08-07 13:21:41.000000 swane-0.0.6/swane/nipype_pipeline/workflows/nonlinear_reg_workflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2180 2023-04-02 07:46:38.000000 swane-0.0.6/swane/nipype_pipeline/workflows/ref_workflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)    19604 2023-07-13 09:03:26.000000 swane-0.0.6/swane/nipype_pipeline/workflows/task_fMRI_workflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)    13725 2023-08-07 13:21:41.000000 swane-0.0.6/swane/nipype_pipeline/workflows/tractography_workflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     6335 2023-04-02 08:03:52.000000 swane-0.0.6/swane/nipype_pipeline/workflows/venous_workflow.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-08-07 15:05:13.622750 swane-0.0.6/swane/slicer/
--rw-rw-r--   0 mau       (1000) mau       (1000)     2971 2023-05-19 05:29:53.000000 swane-0.0.6/swane/slicer/SlicerCheckWorker.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1331 2023-04-15 15:05:28.000000 swane-0.0.6/swane/slicer/SlicerExportWorker.py
--rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.6/swane/slicer/__init__.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      302 2023-04-15 15:05:28.000000 swane-0.0.6/swane/slicer/slicer_script_freesurfer_module_check.py
--rw-rw-r--   0 mau       (1000) mau       (1000)    12647 2023-08-07 13:21:41.000000 swane-0.0.6/swane/slicer/slicer_script_result.py
--rw-rw-r--   0 mau       (1000) mau       (1000)    12511 2023-08-07 13:21:41.000000 swane-0.0.6/swane/strings.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-08-07 15:05:13.622750 swane-0.0.6/swane/ui/
--rw-rw-r--   0 mau       (1000) mau       (1000)     2309 2023-05-11 14:49:48.000000 swane-0.0.6/swane/ui/CustomTreeWidgetItem.py
--rw-rw-r--   0 mau       (1000) mau       (1000)    25003 2023-08-07 14:58:34.000000 swane-0.0.6/swane/ui/MainWindow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      950 2023-05-19 04:43:57.000000 swane-0.0.6/swane/ui/PersistentProgressDialog.py
--rw-rw-r--   0 mau       (1000) mau       (1000)    19245 2023-08-07 13:21:41.000000 swane-0.0.6/swane/ui/PreferencesWindow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)    43097 2023-08-07 14:11:31.000000 swane-0.0.6/swane/ui/PtTab.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1119 2023-05-19 04:43:57.000000 swane-0.0.6/swane/ui/VerticalScrollArea.py
--rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.6/swane/ui/__init__.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-08-07 15:05:13.622750 swane-0.0.6/swane/ui/workers/
--rw-rw-r--   0 mau       (1000) mau       (1000)     4152 2023-03-29 17:07:54.000000 swane-0.0.6/swane/ui/workers/DicomSearchWorker.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      725 2023-03-29 17:07:54.000000 swane-0.0.6/swane/ui/workers/WorkflowGeneratorWorker.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      631 2023-03-29 17:07:54.000000 swane-0.0.6/swane/ui/workers/WorkflowMonitorWorker.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     3829 2023-04-16 08:37:06.000000 swane-0.0.6/swane/ui/workers/WorkflowProcess.py
--rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.6/swane/ui/workers/__init__.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-08-07 15:05:13.622750 swane-0.0.6/swane/utils/
--rw-rw-r--   0 mau       (1000) mau       (1000)     9139 2023-08-07 13:21:41.000000 swane-0.0.6/swane/utils/ConfigManager.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     4390 2023-08-07 13:21:41.000000 swane-0.0.6/swane/utils/DataInput.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     5698 2023-05-19 04:55:32.000000 swane-0.0.6/swane/utils/PreferenceEntry.py
--rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.6/swane/utils/__init__.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1749 2023-03-29 17:07:54.000000 swane-0.0.6/swane/utils/check_dependency.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     3267 2023-03-29 17:07:54.000000 swane-0.0.6/swane/utils/fsl_conflict_handler.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1429 2023-08-07 14:10:46.000000 swane-0.0.6/swane/utils/print_error.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     4385 2023-04-11 10:17:10.000000 swane-0.0.6/swane/utils/shortcut_manager.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-08-07 15:05:13.618750 swane-0.0.6/swane.egg-info/
--rw-rw-r--   0 mau       (1000) mau       (1000)      427 2023-08-07 15:05:13.000000 swane-0.0.6/swane.egg-info/PKG-INFO
--rw-rw-r--   0 mau       (1000) mau       (1000)     3118 2023-08-07 15:05:13.000000 swane-0.0.6/swane.egg-info/SOURCES.txt
--rw-rw-r--   0 mau       (1000) mau       (1000)        1 2023-08-07 15:05:13.000000 swane-0.0.6/swane.egg-info/dependency_links.txt
--rw-rw-r--   0 mau       (1000) mau       (1000)       42 2023-08-07 15:05:13.000000 swane-0.0.6/swane.egg-info/entry_points.txt
--rw-rw-r--   0 mau       (1000) mau       (1000)      165 2023-08-07 15:05:13.000000 swane-0.0.6/swane.egg-info/requires.txt
--rw-rw-r--   0 mau       (1000) mau       (1000)        6 2023-08-07 15:05:13.000000 swane-0.0.6/swane.egg-info/top_level.txt
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2024-04-16 15:37:23.904716 swane-0.1.0/
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1976 2023-12-27 07:46:23.000000 swane-0.1.0/LICENSE
+-rw-rw-r--   0 mau       (1000) mau       (1000)      184 2023-03-29 17:07:54.000000 swane-0.1.0/MANIFEST.in
+-rw-r--r--   0 mau       (1000) mau       (1000)      832 2024-04-16 15:37:23.904716 swane-0.1.0/PKG-INFO
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2953 2023-12-27 07:46:23.000000 swane-0.1.0/README.md
+-rw-rw-r--   0 mau       (1000) mau       (1000)       38 2024-04-16 15:37:23.904716 swane-0.1.0/setup.cfg
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1368 2023-12-11 10:38:23.000000 swane-0.1.0/setup.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2024-04-16 15:37:23.876717 swane-0.1.0/swane/
+-rw-rw-r--   0 mau       (1000) mau       (1000)       48 2024-04-16 15:26:41.000000 swane-0.1.0/swane/__init__.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2084 2023-12-27 07:46:23.000000 swane-0.1.0/swane/__main__.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2024-04-16 15:37:23.880717 swane-0.1.0/swane/config/
+-rw-rw-r--   0 mau       (1000) mau       (1000)    19242 2023-12-28 16:39:57.000000 swane-0.1.0/swane/config/ConfigManager.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      119 2023-12-02 19:33:04.000000 swane-0.1.0/swane/config/PrefCategory.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1724 2023-12-28 16:33:01.000000 swane-0.1.0/swane/config/PreferenceEntry.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-12-02 19:30:26.000000 swane-0.1.0/swane/config/__init__.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1523 2023-12-27 07:46:23.000000 swane-0.1.0/swane/config/config_enums.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    14753 2024-03-25 06:32:26.000000 swane-0.1.0/swane/config/preference_list.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2024-04-16 15:37:23.880717 swane-0.1.0/swane/nipype_pipeline/
+-rw-rw-r--   0 mau       (1000) mau       (1000)    19614 2024-03-25 06:32:26.000000 swane-0.1.0/swane/nipype_pipeline/MainWorkflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.1.0/swane/nipype_pipeline/__init__.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2024-04-16 15:37:23.880717 swane-0.1.0/swane/nipype_pipeline/engine/
+-rw-rw-r--   0 mau       (1000) mau       (1000)     7967 2023-12-27 07:46:23.000000 swane-0.1.0/swane/nipype_pipeline/engine/CustomWorkflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    12511 2024-03-22 11:39:16.000000 swane-0.1.0/swane/nipype_pipeline/engine/MonitoredMultiProcPlugin.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      405 2023-04-06 16:01:54.000000 swane-0.1.0/swane/nipype_pipeline/engine/NodeListEntry.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1318 2023-12-27 07:46:23.000000 swane-0.1.0/swane/nipype_pipeline/engine/WorkflowReport.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-10-16 16:01:20.000000 swane-0.1.0/swane/nipype_pipeline/engine/__init__.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2024-04-16 15:37:23.888716 swane-0.1.0/swane/nipype_pipeline/nodes/
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2537 2023-04-06 16:01:54.000000 swane-0.1.0/swane/nipype_pipeline/nodes/AsymmetryIndex.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2515 2023-12-27 07:46:23.000000 swane-0.1.0/swane/nipype_pipeline/nodes/CropFov.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2263 2023-11-26 16:19:46.000000 swane-0.1.0/swane/nipype_pipeline/nodes/CustomBEDPOSTX5.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2236 2023-12-12 08:54:12.000000 swane-0.1.0/swane/nipype_pipeline/nodes/CustomDcm2niix.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1419 2023-11-29 07:11:21.000000 swane-0.1.0/swane/nipype_pipeline/nodes/CustomEddy.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      661 2023-04-06 16:01:54.000000 swane-0.1.0/swane/nipype_pipeline/nodes/CustomLabel2Vol.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1375 2023-11-26 18:19:58.000000 swane-0.1.0/swane/nipype_pipeline/nodes/CustomProbTrackX2.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2390 2023-12-27 07:46:23.000000 swane-0.1.0/swane/nipype_pipeline/nodes/CustomSliceTimer.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2437 2023-04-06 16:01:54.000000 swane-0.1.0/swane/nipype_pipeline/nodes/DeleteVolumes.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2737 2023-08-07 15:19:23.000000 swane-0.1.0/swane/nipype_pipeline/nodes/FLAT1OutliersMask.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     4611 2023-12-27 07:46:23.000000 swane-0.1.0/swane/nipype_pipeline/nodes/FMRIGenSpec.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2506 2023-04-06 16:01:54.000000 swane-0.1.0/swane/nipype_pipeline/nodes/ForceOrient.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1600 2023-04-06 16:01:54.000000 swane-0.1.0/swane/nipype_pipeline/nodes/FslNVols.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1637 2023-12-27 07:46:23.000000 swane-0.1.0/swane/nipype_pipeline/nodes/GenEddyFiles.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1601 2023-04-06 16:01:54.000000 swane-0.1.0/swane/nipype_pipeline/nodes/GetNiftiTR.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1650 2023-04-06 16:01:54.000000 swane-0.1.0/swane/nipype_pipeline/nodes/MergeTargets.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1849 2023-04-06 16:01:54.000000 swane-0.1.0/swane/nipype_pipeline/nodes/Orient.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1400 2023-04-06 16:01:54.000000 swane-0.1.0/swane/nipype_pipeline/nodes/RandomSeedGenerator.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2727 2023-12-30 08:16:37.000000 swane-0.1.0/swane/nipype_pipeline/nodes/SegmentHA.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     3236 2023-11-26 18:18:50.000000 swane-0.1.0/swane/nipype_pipeline/nodes/SumMultiTracks.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1292 2023-08-07 15:19:23.000000 swane-0.1.0/swane/nipype_pipeline/nodes/SumMultiVols.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1582 2023-12-27 07:46:23.000000 swane-0.1.0/swane/nipype_pipeline/nodes/TTest.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     3025 2023-04-06 16:01:54.000000 swane-0.1.0/swane/nipype_pipeline/nodes/ThrROI.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     3376 2023-12-27 07:46:23.000000 swane-0.1.0/swane/nipype_pipeline/nodes/VenousCheck.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2703 2023-04-06 16:01:54.000000 swane-0.1.0/swane/nipype_pipeline/nodes/Zscore.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)       25 2023-03-29 17:07:54.000000 swane-0.1.0/swane/nipype_pipeline/nodes/__init__.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      178 2023-04-06 16:01:54.000000 swane-0.1.0/swane/nipype_pipeline/nodes/utils.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2024-04-16 15:37:23.892716 swane-0.1.0/swane/nipype_pipeline/workflows/
+-rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.1.0/swane/nipype_pipeline/workflows/__init__.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    10347 2023-12-27 07:46:23.000000 swane-0.1.0/swane/nipype_pipeline/workflows/dti_preproc_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    14090 2024-03-22 08:42:56.000000 swane-0.1.0/swane/nipype_pipeline/workflows/flat1_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    14113 2023-11-22 18:35:13.000000 swane-0.1.0/swane/nipype_pipeline/workflows/freesurfer_asymmetry_index_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     9238 2023-12-30 08:16:37.000000 swane-0.1.0/swane/nipype_pipeline/workflows/freesurfer_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    11706 2023-12-27 07:46:23.000000 swane-0.1.0/swane/nipype_pipeline/workflows/func_map_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     3740 2024-03-22 08:49:25.000000 swane-0.1.0/swane/nipype_pipeline/workflows/linear_reg_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     3132 2023-08-07 15:19:23.000000 swane-0.1.0/swane/nipype_pipeline/workflows/nonlinear_reg_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2837 2023-12-27 07:46:23.000000 swane-0.1.0/swane/nipype_pipeline/workflows/ref_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    19471 2023-12-27 07:46:23.000000 swane-0.1.0/swane/nipype_pipeline/workflows/task_fMRI_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    14082 2023-12-28 16:33:01.000000 swane-0.1.0/swane/nipype_pipeline/workflows/tractography_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     6610 2023-12-27 07:46:23.000000 swane-0.1.0/swane/nipype_pipeline/workflows/venous_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    13681 2023-12-30 08:16:37.000000 swane-0.1.0/swane/strings.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2024-04-16 15:37:23.896716 swane-0.1.0/swane/ui/
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2823 2023-12-27 07:46:23.000000 swane-0.1.0/swane/ui/CustomTreeWidgetItem.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    25210 2023-12-30 08:16:37.000000 swane-0.1.0/swane/ui/MainWindow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1107 2023-12-05 07:20:59.000000 swane-0.1.0/swane/ui/PersistentProgressDialog.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    12060 2023-12-28 16:39:56.000000 swane-0.1.0/swane/ui/PreferenceUIEntry.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    10410 2023-12-27 07:46:23.000000 swane-0.1.0/swane/ui/PreferencesWindow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    49799 2023-12-28 16:33:01.000000 swane-0.1.0/swane/ui/SubjectTab.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1119 2023-08-07 15:19:23.000000 swane-0.1.0/swane/ui/VerticalScrollArea.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.1.0/swane/ui/__init__.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2024-04-16 15:37:23.900716 swane-0.1.0/swane/utils/
+-rw-rw-r--   0 mau       (1000) mau       (1000)     3006 2024-01-17 12:44:19.000000 swane-0.1.0/swane/utils/DataInputList.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     9755 2024-03-25 06:32:26.000000 swane-0.1.0/swane/utils/DependencyManager.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    25445 2023-12-28 16:33:01.000000 swane-0.1.0/swane/utils/Subject.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      840 2023-12-27 07:46:23.000000 swane-0.1.0/swane/utils/SubjectInputStateList.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.1.0/swane/utils/__init__.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      601 2023-12-27 07:46:23.000000 swane-0.1.0/swane/utils/decorators.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     3326 2023-12-27 07:46:23.000000 swane-0.1.0/swane/utils/fsl_conflict_handler.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      427 2023-12-03 18:39:39.000000 swane-0.1.0/swane/utils/last_pid_is_running.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1429 2023-10-25 07:42:31.000000 swane-0.1.0/swane/utils/print_error.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2024-04-16 15:37:23.904716 swane-0.1.0/swane/workers/
+-rw-rw-r--   0 mau       (1000) mau       (1000)     9393 2023-12-27 07:46:23.000000 swane-0.1.0/swane/workers/DicomSearchWorker.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     4629 2023-12-27 07:46:23.000000 swane-0.1.0/swane/workers/SlicerCheckWorker.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1364 2023-12-27 07:46:23.000000 swane-0.1.0/swane/workers/SlicerExportWorker.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      948 2023-12-27 07:46:23.000000 swane-0.1.0/swane/workers/SlicerViewerWorker.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1599 2023-12-27 07:46:23.000000 swane-0.1.0/swane/workers/UpdateCheckWorker.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      887 2023-12-27 07:46:23.000000 swane-0.1.0/swane/workers/WorkflowMonitorWorker.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     7362 2023-12-27 07:46:23.000000 swane-0.1.0/swane/workers/WorkflowProcess.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.1.0/swane/workers/__init__.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      593 2023-12-05 12:29:00.000000 swane-0.1.0/swane/workers/open_results_directory.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      302 2023-08-07 15:19:23.000000 swane-0.1.0/swane/workers/slicer_script_freesurfer_module_check.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      445 2023-12-07 15:17:27.000000 swane-0.1.0/swane/workers/slicer_script_freesurfer_module_install.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    13067 2023-12-27 07:46:23.000000 swane-0.1.0/swane/workers/slicer_script_result.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2024-04-16 15:37:23.904716 swane-0.1.0/swane.egg-info/
+-rw-r--r--   0 mau       (1000) mau       (1000)      832 2024-04-16 15:37:23.000000 swane-0.1.0/swane.egg-info/PKG-INFO
+-rw-rw-r--   0 mau       (1000) mau       (1000)     3536 2024-04-16 15:37:23.000000 swane-0.1.0/swane.egg-info/SOURCES.txt
+-rw-rw-r--   0 mau       (1000) mau       (1000)        1 2024-04-16 15:37:23.000000 swane-0.1.0/swane.egg-info/dependency_links.txt
+-rw-rw-r--   0 mau       (1000) mau       (1000)       42 2024-04-16 15:37:23.000000 swane-0.1.0/swane.egg-info/entry_points.txt
+-rw-rw-r--   0 mau       (1000) mau       (1000)      210 2024-04-16 15:37:23.000000 swane-0.1.0/swane.egg-info/requires.txt
+-rw-rw-r--   0 mau       (1000) mau       (1000)        6 2024-04-16 15:37:23.000000 swane-0.1.0/swane.egg-info/top_level.txt
```

### Comparing `swane-0.0.6/LICENSE` & `swane-0.1.0/LICENSE`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2023 LICE - Commissione Neuroimmagini
+Copyright (c) 2024 LICE - Commissione Neuroimmagini
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `swane-0.0.6/setup.py` & `swane-0.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,33 +10,36 @@
 
 
 setup(name='swane',
       version=get_property('__version__'),
       description='Standardized Workflow for Advanced Neuroimaging in Epilepsy',
       author='LICE - Commissione Neuroimmagini',
       author_email='dev@lice.it',
-      packages=find_packages(),
+      packages=find_packages(exclude=["swane.tests"]),
       classifiers=[
           "Programming Language :: Python :: 3",
           "License :: OSI Approved :: MIT License",
           "Operating System :: MacOS",
           "Operating System :: POSIX :: Linux",
       ],
       license='MIT',
       install_requires=[
           "networkx<3",
           "nipype==1.8.6",
           "Pyside6==6.4.3",
           "pydicom==2.3.1",
           "configparser==5.3.0",
           "psutil==5.9.4",
-          "pyshortcuts==1.8.3",
           "swane_supplement>=0.1.2",
           "matplotlib==3.5.2",
-          "nibabel==5.0.0"
+          "nibabel==5.0.0",
+          "packaging",
+          "PySide6_VerticalQTabWidget==0.0.3",
+          "GPUtil==1.4.0",
+          "numpy"
       ],
       python_requires=">=3.7",
       entry_points={
           'gui_scripts': [
               "swane = swane.__main__:main"
           ]
       }
```

### Comparing `swane-0.0.6/swane/__main__.py` & `swane-0.1.0/swane/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from swane.utils.fsl_conflict_handler import fsl_conflict_check
 
 
 def main():
     import sys
     import os
-    import psutil
     from swane import strings
     import swane_supplement
     from PySide6.QtWidgets import QApplication, QMessageBox
     from PySide6.QtGui import QIcon, QPixmap
     from swane.ui.MainWindow import MainWindow
-    from swane.utils.ConfigManager import ConfigManager
+    from swane.config.ConfigManager import ConfigManager
     from swane import EXIT_CODE_REBOOT
+    from swane.config.config_enums import GlobalPrefCategoryList
+    from swane.utils.last_pid_is_running import last_pid_is_running
 
     # Exit Code definition for automatic reboot
     current_exit_code = EXIT_CODE_REBOOT
 
     while current_exit_code == EXIT_CODE_REBOOT:
         
         # Singleton for SWANe application
@@ -29,26 +30,24 @@
         # SWANe App Name definition
         app.setApplicationDisplayName(strings.APPNAME)
         
         # SWANe Configuration loading
         global_config = ConfigManager()
 
         # Guard to prevent multiple SWANe instances launch
-        last_pid = global_config.getint('MAIN', 'lastPID')
-        if last_pid != os.getpid():
-            try:
-                psutil.Process(last_pid)
-                msg_box = QMessageBox()
-                msg_box.setText(strings.main_multiple_instances_error)
-                msg_box.exec()
-                break
-
-            except (psutil.NoSuchProcess, ValueError):
-                global_config['MAIN']['lastPID'] = str(os.getpid())
-                global_config.save()
+        last_pid = global_config.get_last_pid()
+
+        if last_pid_is_running(last_pid):
+            msg_box = QMessageBox()
+            msg_box.setText(strings.main_multiple_instances_error)
+            msg_box.exec()
+            sys.exit(-1)
+        else:
+            global_config[GlobalPrefCategoryList.MAIN]['last_pid'] = str(os.getpid())
+            global_config.save()
 
         # MainWindow in a varariable to prenvent garbage collector deletion (might cause crash)
         widget = MainWindow(global_config)
         widget.setWindowIcon(QIcon(QPixmap(swane_supplement.appIcon_file)))
         current_exit_code = app.exec()
 
     sys.exit(current_exit_code)
```

### Comparing `swane-0.0.6/swane/nipype_pipeline/MainWorkflow.py` & `swane-0.1.0/swane/nipype_pipeline/MainWorkflow.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,349 +1,336 @@
 import os
 from multiprocessing import cpu_count
 from os.path import abspath
 
 import swane_supplement
-
-from swane.utils.ConfigManager import ConfigManager
-from swane.utils.DataInput import DataInputList
-
+from swane.config.ConfigManager import ConfigManager
+from swane.utils.SubjectInputStateList import SubjectInputStateList
+from swane.utils.DataInputList import DataInputList as DIL, FMRI_NUM
+from swane.config.config_enums import PLANES, CORE_LIMIT, BLOCK_DESIGN, GlobalPrefCategoryList
 from swane.nipype_pipeline.engine.CustomWorkflow import CustomWorkflow
-
 from swane.nipype_pipeline.workflows.linear_reg_workflow import linear_reg_workflow
 from swane.nipype_pipeline.workflows.task_fMRI_workflow import task_fMRI_workflow
 from swane.nipype_pipeline.workflows.nonlinear_reg_workflow import nonlinear_reg_workflow
 from swane.nipype_pipeline.workflows.ref_workflow import ref_workflow
 from swane.nipype_pipeline.workflows.freesurfer_workflow import freesurfer_workflow
-from swane.nipype_pipeline.workflows.FLAT1_workflow import FLAT1_workflow
+from swane.nipype_pipeline.workflows.flat1_workflow import flat1_workflow
 from swane.nipype_pipeline.workflows.func_map_workflow import func_map_workflow
 from swane.nipype_pipeline.workflows.venous_workflow import venous_workflow
 from swane.nipype_pipeline.workflows.dti_preproc_workflow import dti_preproc_workflow
 from swane.nipype_pipeline.workflows.tractography_workflow import tractography_workflow, SIDES
+from swane.config.preference_list import TRACTS
+from swane.utils.DependencyManager import DependencyManager
+from swane.nipype_pipeline.engine.MonitoredMultiProcPlugin import MonitoredMultiProcPlugin
 
 
 DEBUG = False
 
 
 # TODO implementazione error manager
 class MainWorkflow(CustomWorkflow):
-    SCENE_DIR = 'scene'
+    Result_DIR = 'results'
 
-    def add_input_folders(self, global_config: ConfigManager, pt_config: ConfigManager, data_input_list: DataInputList):
+    def __init__(self, name: str, base_dir: str):
+        super().__init__(name, base_dir)
+        self.is_resource_monitor: bool = False
+        self.max_cpu: int = -1
+        self.max_gpu: int = -1
+        self.multicore_node_limit: CORE_LIMIT = CORE_LIMIT.SOFT_CAP
+
+    def add_input_folders(self, global_config: ConfigManager, subject_config: ConfigManager,
+                          dependency_manager: DependencyManager, subject_input_state_list: SubjectInputStateList):
         """
         Create the Workflows and their sub-workflows based on the list of available data inputs 
 
         Parameters
         ----------
         global_config : ConfigManager
             The app global configurations.
-        pt_config : ConfigManager
-            The patient specific configurations.
-        data_input_list : DataInputList
+        subject_config : ConfigManager
+            The subject specific configurations.
+        dependency_manager: DependencyManager
+            The state of application dependency
+        subject_input_state_list : SubjectInputStateList
             The list of all available input data from the DICOM directory.
 
         Returns
         -------
         None.
 
         """
         
-        if not data_input_list.is_ref_loaded:
+        if not subject_input_state_list.is_ref_loaded:
             return
 
         # Check for FreeSurfer requirement and request
-        is_freesurfer = pt_config.is_freesurfer() and pt_config.get_pt_wf_freesurfer()
-        is_hippo_amyg_labels = pt_config.is_freesurfer_matlab() and pt_config.get_pt_wf_hippo()
+        is_freesurfer = dependency_manager.is_freesurfer() and subject_config.get_workflow_freesurfer_pref()
+        is_hippo_amyg_labels = dependency_manager.is_freesurfer_matlab() and subject_config.get_workflow_hippo_pref()
+
         # Check for FLAT1 requirement and request
-        is_FLAT1 = pt_config.getboolean('WF_OPTION', 'FLAT1') and data_input_list[DataInputList.FLAIR3D].loaded
+        is_flat1 = subject_config.getboolean_safe(DIL.T13D, 'flat1') and subject_input_state_list[DIL.FLAIR3D].loaded
         # Check for Asymmetry Index request
-        is_ai = pt_config.getboolean('WF_OPTION', 'ai')
+        is_ai = ((subject_config.getboolean_safe(DIL.PET, 'ai') and subject_input_state_list[DIL.PET].loaded) or
+                 (subject_config.getboolean_safe(DIL.ASL, 'ai') and subject_input_state_list[DIL.ASL].loaded))
         # Check for Tractography request
-        is_tractography = pt_config.getboolean('WF_OPTION', 'tractography')
+        is_tractography = subject_config.getboolean_safe(DIL.DTI, 'tractography')
+        # CPU cores and memory management
+        self.is_resource_monitor = global_config.getboolean_safe(GlobalPrefCategoryList.PERFORMANCE, 'resource_monitor')
+        self.max_cpu = global_config.getint_safe(GlobalPrefCategoryList.PERFORMANCE, 'max_subj_cu')
+        if self.max_cpu < 1:
+            self.max_cpu = cpu_count()
+        self.multicore_node_limit = global_config.getenum_safe(GlobalPrefCategoryList.PERFORMANCE, 'multicore_node_limit')
+        # GPU management
+        self.max_gpu = global_config.getint_safe(GlobalPrefCategoryList.PERFORMANCE, 'max_subj_gpu')
+        if self.max_gpu < 0:
+            self.max_gpu = MonitoredMultiProcPlugin.gpu_count()
+        try:
+            if not dependency_manager.is_cuda():
+                subject_config[DIL.DTI]["cuda"] = "false"
+            else:
+                subject_config[DIL.DTI]["cuda"] = global_config[GlobalPrefCategoryList.PERFORMANCE]["cuda"]
+        except:
+            subject_config[DIL.DTI]["cuda"] = "false"
 
-        # Core management
-        self.max_cpu = global_config.getint('MAIN', 'maxPtCPU')
-        if self.max_cpu > 0:
-            max_node_cpu = max(int(self.max_cpu / 2), 1)
-        else:
-            max_node_cpu = max(int((cpu_count() - 2) / 2), 1)
+        subject_config.sections()
+
+        max_node_cpu = max(int(self.max_cpu / 2), 1)
 
         # 3D T1w
-        ref_dir = data_input_list.get_dicom_dir(DataInputList.T13D)
-        t1 = ref_workflow(data_input_list[DataInputList.T13D].wf_name, ref_dir)
+        ref_dir = subject_input_state_list.get_dicom_dir(DIL.T13D)
+        t1 = ref_workflow(DIL.T13D.value.workflow_name, ref_dir, subject_config[DIL.T13D])
         t1.long_name = "3D T1w analysis"
         self.add_nodes([t1])
 
-        t1.sink_result(self.base_dir, "outputnode", 'ref', self.SCENE_DIR)
-        t1.sink_result(self.base_dir, "outputnode", 'ref_brain', self.SCENE_DIR)
+        t1.sink_result(self.base_dir, "outputnode", 'ref', self.Result_DIR)
+        t1.sink_result(self.base_dir, "outputnode", 'ref_brain', self.Result_DIR)
 
-        if is_ai and (data_input_list[DataInputList.ASL].loaded or data_input_list[DataInputList.PET].loaded):
+        if is_ai:
             # Non linear registration for Asymmetry Index
             sym = nonlinear_reg_workflow("sym")
             sym.long_name = "Symmetric atlas registration"
 
             sym_inputnode = sym.get_node("inputnode")
             sym_template = swane_supplement.sym_template
             sym_inputnode.inputs.atlas = sym_template
             self.connect(t1, "outputnode.ref_brain", sym, "inputnode.in_file")
 
         if is_freesurfer:
             # FreeSurfer analysis
-            freesurfer = freesurfer_workflow("freesurfer", is_hippo_amyg_labels)
+            freesurfer = freesurfer_workflow("freesurfer", is_hippo_amyg_labels, max_cpu=self.max_cpu, multicore_node_limit=self.multicore_node_limit)
             freesurfer.long_name = "Freesurfer analysis"
 
             freesurfer_inputnode = freesurfer.get_node("inputnode")
-            freesurfer_inputnode.inputs.max_node_cpu = max_node_cpu
             freesurfer_inputnode.inputs.subjects_dir = self.base_dir
             self.connect(t1, "outputnode.ref", freesurfer, "inputnode.ref")
 
-            freesurfer.sink_result(self.base_dir, "outputnode", 'pial', self.SCENE_DIR)
-            freesurfer.sink_result(self.base_dir, "outputnode", 'white', self.SCENE_DIR)
-            freesurfer.sink_result(self.base_dir, "outputnode", 'vol_label_file', self.SCENE_DIR)
+            freesurfer.sink_result(self.base_dir, "outputnode", 'pial', self.Result_DIR)
+            freesurfer.sink_result(self.base_dir, "outputnode", 'white', self.Result_DIR)
+            freesurfer.sink_result(self.base_dir, "outputnode", 'vol_label_file', self.Result_DIR)
             if is_hippo_amyg_labels:
                 regex_subs = [("-T1.*.mgz", ".mgz")]
                 freesurfer.sink_result(self.base_dir, "outputnode", 'lh_hippoAmygLabels', 'scene.segmentHA', regex_subs)
                 freesurfer.sink_result(self.base_dir, "outputnode", 'rh_hippoAmygLabels', 'scene.segmentHA', regex_subs)
 
-        if data_input_list[DataInputList.FLAIR3D].loaded:
+        if subject_input_state_list[DIL.FLAIR3D].loaded:
             # 3D Flair analysis
-            flair_dir = data_input_list.get_dicom_dir(DataInputList.FLAIR3D)
-            flair = linear_reg_workflow(data_input_list[DataInputList.FLAIR3D].wf_name, flair_dir)
+            flair_dir = subject_input_state_list.get_dicom_dir(DIL.FLAIR3D)
+            flair = linear_reg_workflow(DIL.FLAIR3D.value.workflow_name, flair_dir, subject_config[DIL.FLAIR3D])
             flair.long_name = "3D Flair analysis"
             self.add_nodes([flair])
 
             flair_inputnode = flair.get_node("inputnode")
-            flair_inputnode.inputs.frac = 0.5
             flair_inputnode.inputs.crop = True
             flair_inputnode.inputs.output_name = "r-flair_brain.nii.gz"
             self.connect(t1, "outputnode.ref_brain", flair, "inputnode.reference")
 
-            flair.sink_result(self.base_dir, "outputnode", 'registered_file', self.SCENE_DIR)
+            flair.sink_result(self.base_dir, "outputnode", 'registered_file', self.Result_DIR)
+
+            # if is_freesurfer:
+            #     from swane.nipype_pipeline.workflows.freesurfer_asymmetry_index_workflow import freesurfer_asymmetry_index_workflow
+            #     flair_ai = freesurfer_asymmetry_index_workflow(name="flair_ai")
+            #     self.connect(flair, "outputnode.registered_file", flair_ai, "inputnode.in_file")
+            #     self.connect(freesurfer, "outputnode.vol_label_file_nii", flair_ai, "inputnode.seg_file")
 
-        if is_FLAT1:
+        if is_flat1:
             # Non linear registration to MNI1mm Atlas for FLAT1
             mni1 = nonlinear_reg_workflow("mni1")
             mni1.long_name = "MNI atlas registration"
 
             mni1_inputnode = mni1.get_node("inputnode")
             mni1_path = abspath(os.path.join(os.environ["FSLDIR"], 'data/standard/MNI152_T1_1mm_brain.nii.gz'))
             mni1_inputnode.inputs.atlas = mni1_path
             self.connect(t1, "outputnode.ref_brain", mni1, "inputnode.in_file")
 
             # FLAT1 analysis
-            FLAT1 = FLAT1_workflow("FLAT1", mni1_path)
-            FLAT1.long_name = "FLAT1 analysis"
+            flat1 = flat1_workflow("FLAT1", mni1_path)
+            flat1.long_name = "FLAT1 analysis"
 
-            self.connect(t1, "outputnode.ref_brain", FLAT1, "inputnode.ref_brain")
-            self.connect(flair, "outputnode.registered_file", FLAT1, "inputnode.flair_brain")
-            self.connect(mni1, "outputnode.fieldcoeff_file", FLAT1, "inputnode.ref_2_mni1_warp")
-            self.connect(mni1, "outputnode.inverse_warp", FLAT1, "inputnode.ref_2_mni1_inverse_warp")
-
-            FLAT1.sink_result(self.base_dir, "outputnode", "extension_z", self.SCENE_DIR)
-            FLAT1.sink_result(self.base_dir, "outputnode", "junction_z", self.SCENE_DIR)
-            FLAT1.sink_result(self.base_dir, "outputnode", "binary_flair", self.SCENE_DIR)
-
-        for plane in DataInputList.PLANES:
-            if DataInputList.FLAIR2D+'_%s' % plane in data_input_list and data_input_list[DataInputList.FLAIR2D+'_%s' % plane].loaded:
-                flair_dir = data_input_list.get_dicom_dir(DataInputList.FLAIR2D+'_%s' % plane)
-                flair2d = linear_reg_workflow(data_input_list[DataInputList.FLAIR2D+'_%s' % plane].wf_name, flair_dir, is_volumetric=False)
-                flair2d.long_name = "2D %s FLAIR analysis" % plane
+            self.connect(t1, "outputnode.ref_brain", flat1, "inputnode.ref_brain")
+            self.connect(flair, "outputnode.registered_file", flat1, "inputnode.flair_brain")
+            self.connect(mni1, "outputnode.fieldcoeff_file", flat1, "inputnode.ref_2_mni1_warp")
+            self.connect(mni1, "outputnode.inverse_warp", flat1, "inputnode.ref_2_mni1_inverse_warp")
+
+            flat1.sink_result(self.base_dir, "outputnode", "extension_z", self.Result_DIR)
+            flat1.sink_result(self.base_dir, "outputnode", "junction_z", self.Result_DIR)
+            flat1.sink_result(self.base_dir, "outputnode", "binary_flair", self.Result_DIR)
+
+        for plane in PLANES:
+            if DIL['FLAIR2D_%s' % plane.name] in subject_input_state_list and subject_input_state_list[DIL['FLAIR2D_%s' % plane.name]].loaded:
+                flair_dir = subject_input_state_list.get_dicom_dir(DIL['FLAIR2D_%s' % plane.name])
+                flair2d = linear_reg_workflow(DIL['FLAIR2D_%s' % plane.name].value.workflow_name, flair_dir, None, is_volumetric=False)
+                flair2d.long_name = "2D %s FLAIR analysis" % plane.value
                 self.add_nodes([flair2d])
 
                 flair2d_tra_inputnode = flair2d.get_node("inputnode")
-                flair2d_tra_inputnode.inputs.frac = 0.5
                 flair2d_tra_inputnode.inputs.crop = False
                 flair2d_tra_inputnode.inputs.output_name = "r-flair2d_%s_brain.nii.gz" % plane
                 self.connect(t1, "outputnode.ref_brain", flair2d, "inputnode.reference")
 
-                flair2d.sink_result(self.base_dir, "outputnode", 'registered_file', self.SCENE_DIR)
+                flair2d.sink_result(self.base_dir, "outputnode", 'registered_file', self.Result_DIR)
 
-        if data_input_list[DataInputList.MDC].loaded:
+        if subject_input_state_list[DIL.MDC].loaded:
             # MDC analysis
-            mdc_dir = data_input_list.get_dicom_dir(DataInputList.MDC)
-            mdc = linear_reg_workflow(data_input_list[DataInputList.MDC].wf_name, mdc_dir)
+            mdc_dir = subject_input_state_list.get_dicom_dir(DIL.MDC)
+            mdc = linear_reg_workflow(DIL.MDC.value.workflow_name, mdc_dir, subject_config[DIL.MDC])
             mdc.long_name = "Post-contrast 3D T1w analysis"
             self.add_nodes([mdc])
 
             mdc_inputnode = mdc.get_node("inputnode")
-            mdc_inputnode.inputs.frac = 0.3
             mdc_inputnode.inputs.crop = True
             mdc_inputnode.inputs.output_name = "r-mdc_brain.nii.gz"
             self.connect(t1, "outputnode.ref_brain", mdc, "inputnode.reference")
 
-            mdc.sink_result(self.base_dir, "outputnode", 'registered_file', self.SCENE_DIR)
+            mdc.sink_result(self.base_dir, "outputnode", 'registered_file', self.Result_DIR)
 
-        if data_input_list[DataInputList.ASL].loaded:
+        if subject_input_state_list[DIL.ASL].loaded:
             # ASL analysis
-            asl_dir = data_input_list.get_dicom_dir(DataInputList.ASL)
-            asl = func_map_workflow(data_input_list[DataInputList.ASL].wf_name, asl_dir, is_freesurfer, is_ai)
+            asl_dir = subject_input_state_list.get_dicom_dir(DIL.ASL)
+            asl = func_map_workflow(DIL.ASL.value.workflow_name, asl_dir, is_freesurfer, subject_config[DIL.ASL])
             asl.long_name = "Arterial Spin Labelling analysis"
 
             self.connect(t1, 'outputnode.ref_brain', asl, 'inputnode.reference')
             self.connect(t1, 'outputnode.ref_mask', asl, 'inputnode.brain_mask')
 
-            asl.sink_result(self.base_dir, "outputnode", 'registered_file', self.SCENE_DIR)
+            asl.sink_result(self.base_dir, "outputnode", 'registered_file', self.Result_DIR)
 
             if is_freesurfer:
                 self.connect(freesurfer, 'outputnode.subjects_dir', asl, 'inputnode.freesurfer_subjects_dir')
                 self.connect(freesurfer, 'outputnode.subject_id', asl, 'inputnode.freesurfer_subject_id')
-                self.connect(freesurfer, 'outputnode.bgtROI', asl, 'inputnode.bgtROI')
+                self.connect(freesurfer, 'outputnode.bgROI', asl, 'inputnode.bgROI')
 
-                asl.sink_result(self.base_dir, "outputnode", 'surf_lh', self.SCENE_DIR)
-                asl.sink_result(self.base_dir, "outputnode", 'surf_rh', self.SCENE_DIR)
-                asl.sink_result(self.base_dir, "outputnode", 'zscore', self.SCENE_DIR)
-                asl.sink_result(self.base_dir, "outputnode", 'zscore_surf_lh', self.SCENE_DIR)
-                asl.sink_result(self.base_dir, "outputnode", 'zscore_surf_rh', self.SCENE_DIR)
+                asl.sink_result(self.base_dir, "outputnode", 'surf_lh', self.Result_DIR)
+                asl.sink_result(self.base_dir, "outputnode", 'surf_rh', self.Result_DIR)
+                asl.sink_result(self.base_dir, "outputnode", 'zscore', self.Result_DIR)
+                asl.sink_result(self.base_dir, "outputnode", 'zscore_surf_lh', self.Result_DIR)
+                asl.sink_result(self.base_dir, "outputnode", 'zscore_surf_rh', self.Result_DIR)
 
-            if is_ai:
+            if subject_config.getboolean_safe(DIL.ASL, 'ai'):
                 self.connect(sym, 'outputnode.fieldcoeff_file', asl, 'inputnode.ref_2_sym_warp')
                 self.connect(sym, 'outputnode.inverse_warp', asl, 'inputnode.ref_2_sym_invwarp')
 
-                asl.sink_result(self.base_dir, "outputnode", 'ai', self.SCENE_DIR)
+                asl.sink_result(self.base_dir, "outputnode", 'ai', self.Result_DIR)
 
                 if is_freesurfer:
-                    asl.sink_result(self.base_dir, "outputnode", 'ai_surf_lh', self.SCENE_DIR)
-                    asl.sink_result(self.base_dir, "outputnode", 'ai_surf_rh', self.SCENE_DIR)
+                    asl.sink_result(self.base_dir, "outputnode", 'ai_surf_lh', self.Result_DIR)
+                    asl.sink_result(self.base_dir, "outputnode", 'ai_surf_rh', self.Result_DIR)
 
-        if data_input_list[DataInputList.PET].loaded:  # and check_input['ct_brain']:
+        if subject_input_state_list[DIL.PET].loaded:  # and check_input['ct_brain']:
             # PET analysis
-            pet_dir = data_input_list.get_dicom_dir(DataInputList.PET)
-            pet = func_map_workflow(data_input_list[DataInputList.PET].wf_name, pet_dir, is_freesurfer, is_ai)
+            pet_dir = subject_input_state_list.get_dicom_dir(DIL.PET)
+            pet = func_map_workflow(DIL.PET.value.workflow_name, pet_dir, is_freesurfer, subject_config[DIL.PET])
             pet.long_name = "Pet analysis"
 
             self.connect(t1, 'outputnode.ref', pet, 'inputnode.reference')
             self.connect(t1, 'outputnode.ref_mask', pet, 'inputnode.brain_mask')
 
-            pet.sink_result(self.base_dir, "outputnode", 'registered_file', self.SCENE_DIR)
+            pet.sink_result(self.base_dir, "outputnode", 'registered_file', self.Result_DIR)
 
             if is_freesurfer:
                 self.connect(freesurfer, 'outputnode.subjects_dir', pet, 'inputnode.freesurfer_subjects_dir')
                 self.connect(freesurfer, 'outputnode.subject_id', pet, 'inputnode.freesurfer_subject_id')
-                self.connect(freesurfer, 'outputnode.bgtROI', pet, 'inputnode.bgtROI')
+                self.connect(freesurfer, 'outputnode.bgROI', pet, 'inputnode.bgROI')
 
-                pet.sink_result(self.base_dir, "outputnode", 'surf_lh', self.SCENE_DIR)
-                pet.sink_result(self.base_dir, "outputnode", 'surf_rh', self.SCENE_DIR)
-                pet.sink_result(self.base_dir, "outputnode", 'zscore', self.SCENE_DIR)
-                pet.sink_result(self.base_dir, "outputnode", 'zscore_surf_lh', self.SCENE_DIR)
-                pet.sink_result(self.base_dir, "outputnode", 'zscore_surf_rh', self.SCENE_DIR)
+                pet.sink_result(self.base_dir, "outputnode", 'surf_lh', self.Result_DIR)
+                pet.sink_result(self.base_dir, "outputnode", 'surf_rh', self.Result_DIR)
+                pet.sink_result(self.base_dir, "outputnode", 'zscore', self.Result_DIR)
+                pet.sink_result(self.base_dir, "outputnode", 'zscore_surf_lh', self.Result_DIR)
+                pet.sink_result(self.base_dir, "outputnode", 'zscore_surf_rh', self.Result_DIR)
 
                 # TODO work in progress for segmentation based asymmetry study
                 # from swane.nipype_pipeline.workflows.freesurfer_asymmetry_index_workflow import freesurfer_asymmetry_index_workflow
                 # pet_ai = freesurfer_asymmetry_index_workflow(name="pet_ai")
                 # self.connect(pet, "outputnode.registered_file", pet_ai, "inputnode.in_file")
                 # self.connect(freesurfer, "outputnode.vol_label_file_nii", pet_ai, "inputnode.seg_file")
 
-            if is_ai:
+            if subject_config.getboolean_safe(DIL.PET, 'ai'):
                 self.connect(sym, 'outputnode.fieldcoeff_file', pet, 'inputnode.ref_2_sym_warp')
                 self.connect(sym, 'outputnode.inverse_warp', pet, 'inputnode.ref_2_sym_invwarp')
 
-                pet.sink_result(self.base_dir, "outputnode", 'ai', self.SCENE_DIR)
+                pet.sink_result(self.base_dir, "outputnode", 'ai', self.Result_DIR)
 
                 if is_freesurfer:
-                    pet.sink_result(self.base_dir, "outputnode", 'ai_surf_lh', self.SCENE_DIR)
-                    pet.sink_result(self.base_dir, "outputnode", 'ai_surf_rh', self.SCENE_DIR)
+                    pet.sink_result(self.base_dir, "outputnode", 'ai_surf_lh', self.Result_DIR)
+                    pet.sink_result(self.base_dir, "outputnode", 'ai_surf_rh', self.Result_DIR)
 
-        if data_input_list[DataInputList.VENOUS].loaded:
+        if subject_input_state_list[DIL.VENOUS].loaded and subject_input_state_list[DIL.VENOUS].volumes + subject_input_state_list[DIL.VENOUS2].volumes == 2:
             # Venous analysis
-            venous_dir = data_input_list.get_dicom_dir(DataInputList.VENOUS)
+            venous_dir = subject_input_state_list.get_dicom_dir(DIL.VENOUS)
             venous2_dir = None
-            if data_input_list[DataInputList.VENOUS2].loaded:
-                venous2_dir = data_input_list.get_dicom_dir(DataInputList.VENOUS2)
-            venous = venous_workflow(data_input_list[DataInputList.VENOUS].wf_name, venous_dir, venous2_dir)
+            if subject_input_state_list[DIL.VENOUS2].loaded:
+                venous2_dir = subject_input_state_list.get_dicom_dir(DIL.VENOUS2)
+            venous = venous_workflow(DIL.VENOUS.value.workflow_name, venous_dir, subject_config[DIL.VENOUS], venous2_dir)
             venous.long_name = "Venous MRA analysis"
 
             self.connect(t1, "outputnode.ref_brain", venous, "inputnode.ref_brain")
 
-            venous.sink_result(self.base_dir, "outputnode", 'veins', self.SCENE_DIR)
+            venous.sink_result(self.base_dir, "outputnode", 'veins', self.Result_DIR)
 
-        if data_input_list[DataInputList.DTI].loaded:
+        if subject_input_state_list[DIL.DTI].loaded:
             # DTI analysis
-            dti_dir = data_input_list.get_dicom_dir(DataInputList.DTI)
+            dti_dir = subject_input_state_list.get_dicom_dir(DIL.DTI)
             mni_dir = abspath(os.path.join(os.environ["FSLDIR"], 'data/standard/MNI152_T1_2mm_brain.nii.gz'))
 
-            dti_preproc = dti_preproc_workflow(data_input_list[DataInputList.DTI].wf_name, dti_dir, mni_dir, is_tractography=is_tractography)
+            dti_preproc = dti_preproc_workflow(DIL.DTI.value.workflow_name, dti_dir, subject_config[DIL.DTI], mni_dir, max_cpu=self.max_cpu, multicore_node_limit=self.multicore_node_limit)
             dti_preproc.long_name = "Diffusion Tensor Imaging preprocessing"
             self.connect(t1, "outputnode.ref_brain", dti_preproc, "inputnode.ref_brain")
 
-            dti_preproc.sink_result(self.base_dir, "outputnode", 'FA', self.SCENE_DIR)
+            dti_preproc.sink_result(self.base_dir, "outputnode", 'FA', self.Result_DIR)
 
             if is_tractography:
-                for tract in pt_config['DEFAULTTRACTS'].keys():
-                    if not pt_config.getboolean('DEFAULTTRACTS', tract):
+                for tract in TRACTS.keys():
+                    try:
+                        if not subject_config.getboolean_safe(DIL.DTI, tract):
+                            continue
+                    except:
                         continue
                     
-                    tract_workflow = tractography_workflow(tract, 5)
-                    tract_workflow.long_name = pt_config.TRACTS[tract][0] + " tractography"
+                    tract_workflow = tractography_workflow(tract, subject_config[DIL.DTI])
                     if tract_workflow is not None:
+                        tract_workflow.long_name = TRACTS[tract][0] + " tractography"
                         self.connect(dti_preproc, "outputnode.fsamples", tract_workflow, "inputnode.fsamples")
                         self.connect(dti_preproc, "outputnode.nodiff_mask_file", tract_workflow, "inputnode.mask")
                         self.connect(dti_preproc, "outputnode.phsamples", tract_workflow, "inputnode.phsamples")
                         self.connect(dti_preproc, "outputnode.thsamples", tract_workflow, "inputnode.thsamples")
                         self.connect(t1, "outputnode.ref_brain", tract_workflow, "inputnode.ref_brain")
                         self.connect(dti_preproc, "outputnode.diff2ref_mat", tract_workflow, "inputnode.diff2ref_mat")
                         self.connect(dti_preproc, "outputnode.ref2diff_mat", tract_workflow, "inputnode.ref2diff_mat")
                         self.connect(dti_preproc, "outputnode.mni2ref_warp", tract_workflow, "inputnode.mni2ref_warp")
 
                         for side in SIDES:
                             tract_workflow.sink_result(self.base_dir, "outputnode", "waytotal_%s" % side,
-                                                             self.SCENE_DIR + ".dti")
+                                                       self.Result_DIR + ".dti")
                             tract_workflow.sink_result(self.base_dir, "outputnode", "fdt_paths_%s" % side,
-                                                             self.SCENE_DIR + ".dti")
+                                                       self.Result_DIR + ".dti")
 
         # Check for Task FMRI sequences
-        for y in range(DataInputList.FMRI_NUM):
+        for y in range(FMRI_NUM):
 
-            if data_input_list[DataInputList.FMRI+'_%d' % y].loaded:
+            if subject_input_state_list[DIL['FMRI_%d' % y]].loaded:
 
-                task_a_name = pt_config['FMRI']["task_%d_name_a" % y]
-                task_b_name = pt_config['FMRI']["task_%d_name_b" % y]
-                task_duration = pt_config['FMRI'].getint('task_%d_duration' % y)
-                rest_duration = pt_config['FMRI'].getint('rest_%d_duration' % y)
-
-                try:
-                    TR = pt_config['FMRI'].getfloat('task_%d_tr' % y)
-                except:
-                    TR = -1
-
-                try:
-                    slice_timing = pt_config['FMRI'].getint('task_%d_st' % y)
-                except:
-                    slice_timing = 0
-
-                try:
-                    nvols = pt_config['FMRI'].getint('task_%d_vols' % y)
-                except:
-                    nvols = -1
-
-                try:
-                    del_start_vols = pt_config['FMRI'].getint('task_%d_del_start_vols' % y)
-                except:
-                    del_start_vols = 0
-
-                try:
-                    del_end_vols = pt_config['FMRI'].getint('task_%d_del_end_vols' % y)
-                except:
-                    del_end_vols = 0
-
-                try:
-                    design_block = pt_config['FMRI'].getint('task_%d_blockdesign' % y)
-                except:
-                    design_block = 0
-
-                dicom_dir = data_input_list.get_dicom_dir(DataInputList.FMRI+'_%d' % y)
-                fMRI = task_fMRI_workflow(data_input_list[DataInputList.FMRI+'_%d' % y].wf_name, dicom_dir, design_block, self.base_dir)
+                dicom_dir = subject_input_state_list.get_dicom_dir(DIL['FMRI_%d' % y])
+                fMRI = task_fMRI_workflow(DIL['FMRI_%d' % y].value.workflow_name, dicom_dir, subject_config[DIL['FMRI_%d' % y]], self.base_dir)
                 fMRI.long_name = "Task fMRI analysis - %d" % y
-                inputnode = fMRI.get_node("inputnode")
-                inputnode.inputs.TR = TR
-                inputnode.inputs.slice_timing = slice_timing
-                inputnode.inputs.nvols = nvols
-                inputnode.inputs.task_a_name = task_a_name
-                inputnode.inputs.task_b_name = task_b_name
-                inputnode.inputs.task_duration = task_duration
-                inputnode.inputs.rest_duration = rest_duration
-                inputnode.inputs.del_start_vols = del_start_vols
-                inputnode.inputs.del_end_vols = del_end_vols
-
                 self.connect(t1, "outputnode.ref_brain", fMRI, "inputnode.ref_BET")
-                fMRI.sink_result(self.base_dir, "outputnode", 'threshold_file_1', self.SCENE_DIR + '.fMRI')
-                if design_block == 1:
-                    fMRI.sink_result(self.base_dir, "outputnode", 'threshold_file_2', self.SCENE_DIR + '.fMRI')
+                fMRI.sink_result(self.base_dir, "outputnode", 'threshold_file_1', self.Result_DIR + '.fMRI')
+                if subject_config.getenum_safe(DIL['FMRI_%d' % y], "block_design") == BLOCK_DESIGN.RARB:
+                    fMRI.sink_result(self.base_dir, "outputnode", 'threshold_file_2', self.Result_DIR + '.fMRI')
```

### Comparing `swane-0.0.6/swane/nipype_pipeline/engine/CustomWorkflow.py` & `swane-0.1.0/swane/nipype_pipeline/engine/CustomWorkflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,34 +35,35 @@
             formatted_name = default_node_name
         else:
             formatted_name = node.name
 
         formatted_name = formatted_name[0].upper() + formatted_name[1:]
         return formatted_name
 
-    def get_node_array(self):
+    def get_node_array(self) -> dict:
         """
         Returns a List of NodeListEntry objects for the Nodes in a Workflow.
         
         """
         
         from networkx import topological_sort
 
         outlist = {}
         for node in topological_sort(self._graph):
             if hasattr(node, "interface") and isinstance(node.interface, IdentityInterface):
                 continue
 
             outlist[node.name] = NodeListEntry()
             outlist[node.name].long_name = self.format_node_name(node)
-            if isinstance(node, Workflow):
+            if isinstance(node, CustomWorkflow):
                 outlist[node.name].node_list = node.get_node_array()
         return outlist
 
-    def sink_result(self, save_path, result_node, result_name, sub_folder, regexp_substitutions=None):
+    def sink_result(self, save_path: str, result_node: str, result_name: str, sub_folder: str,
+                    regexp_substitutions: list[tuple[str, str]] = None):
         """
         Creates a sink_result Node to save the output files of a Workflow.
         
         """
         
         if isinstance(result_node, str):
             result_node = self.get_node(result_node)
@@ -72,17 +73,15 @@
         data_sink.inputs.base_directory = save_path
 
         if regexp_substitutions is not None:
             data_sink.inputs.regexp_substitutions = regexp_substitutions
 
         self.connect(result_node, result_name, data_sink, sub_folder)
 
-    def _get_dot(
-            self, prefix=None, hierarchy=None, colored=False, simple_form=True, level=0
-    ):
+    def _get_dot(self, prefix=None, hierarchy=None, colored=False, simple_form=True, level=0):
         """
         Custom implementation of _get_dot Nipype func to support the long_name Node attribute.
         
         """
         
         import networkx as nx
```

### Comparing `swane-0.0.6/swane/nipype_pipeline/nodes/AsymmetryIndex.py` & `swane-0.1.0/swane/nipype_pipeline/nodes/AsymmetryIndex.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.6/swane/nipype_pipeline/nodes/CustomBEDPOSTX5.py` & `swane-0.1.0/swane/nipype_pipeline/nodes/CustomBEDPOSTX5.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.6/swane/nipype_pipeline/nodes/CustomLabel2Vol.py` & `swane-0.1.0/swane/nipype_pipeline/nodes/CustomLabel2Vol.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.6/swane/nipype_pipeline/nodes/CustomSliceTimer.py` & `swane-0.1.0/swane/nipype_pipeline/nodes/CustomSliceTimer.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,25 +2,23 @@
 
 import shutil
 from nipype.interfaces.fsl import SliceTimer
 from nipype import Node
 from os.path import abspath
 import os
 from nipype.interfaces.base import (traits, TraitedSpec, BaseInterface, BaseInterfaceInputSpec, File)
+from swane.config.config_enums import SLICE_TIMING
 
 
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.BaseInterfaceInputSpec)  -*-
 class CustomSliceTimerInputSpec(BaseInterfaceInputSpec):
     in_file = File(exists=True, mandatory=True, desc='the input image')
     time_repetition = traits.Float(mandatory=True)
     slice_timing = traits.Enum(
-        0,  # None
-        1,  # Regular up
-        2,  # Regular down
-        3,  # intervealed
+        SLICE_TIMING,
         usedefault=True)
 
 
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.TraitedSpec)  -*-
 class CustomSliceTimerOutputSpec(TraitedSpec):
     slice_time_corrected_file = File(desc='the output image')
 
@@ -33,24 +31,24 @@
     """
     
     input_spec = CustomSliceTimerInputSpec
     output_spec = CustomSliceTimerOutputSpec
 
     def _run_interface(self, runtime):
         out_file = self._gen_outfilename()
-        if self.inputs.slice_timing == 0:
+        if self.inputs.slice_timing == SLICE_TIMING.UNKNOWN:
             shutil.copy(self.inputs.in_file, out_file)
         else:
             fmri_timing_correction = Node(SliceTimer(), name="fMRI_timing_correction")
             fmri_timing_correction.inputs.time_repetition = self.inputs.time_repetition
             fmri_timing_correction.inputs.in_file = self.inputs.in_file
             fmri_timing_correction.inputs.out_file = out_file
-            if self.inputs.slice_timing == 2:
+            if self.inputs.slice_timing == SLICE_TIMING.DOWN:
                 fmri_timing_correction.inputs.index_dir = True
-            elif self.inputs.slice_timing == 3:
+            elif self.inputs.slice_timing == SLICE_TIMING.INTERLEAVED:
                 fmri_timing_correction.inputs.interleaved = True
             fmri_timing_correction.run()
 
         return runtime
 
     def _gen_outfilename(self):
         out_file = os.path.basename(self.inputs.in_file)
```

### Comparing `swane-0.0.6/swane/nipype_pipeline/nodes/DeleteVolumes.py` & `swane-0.1.0/swane/nipype_pipeline/nodes/DeleteVolumes.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.6/swane/nipype_pipeline/nodes/FLAT1OutliersMask.py` & `swane-0.1.0/swane/nipype_pipeline/nodes/FLAT1OutliersMask.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.6/swane/nipype_pipeline/nodes/FMRIGenSpec.py` & `swane-0.1.0/swane/nipype_pipeline/nodes/FMRIGenSpec.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # -*- DISCLAIMER: this file contains code derived from Nipype (https://github.com/nipy/nipype/blob/master/LICENSE)  -*-
 
 from nipype.interfaces.base import (traits, BaseInterface, BaseInterfaceInputSpec, TraitedSpec, File, Bunch, isdefined)
+from swane.config.config_enums import BLOCK_DESIGN
 
 
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.BaseInterfaceInputSpec)  -*-
 class FMRIGenSpecInputSpec(BaseInterfaceInputSpec):
     TR = traits.Float(mandatory=True, desc="Repetition Time")
     nvols = traits.Int(mandatory=True, desc="Number of EPI runs")
     task_duration = traits.Int(mandatory=True, desc="Task duration")
     rest_duration = traits.Int(mandatory=True, desc="Rest duration")
-    design_block = traits.Enum(0, 1, usedefault=True)
+    block_design = traits.Enum(BLOCK_DESIGN, usedefault=True)
     task_a_name = traits.String(mandatory=False, desc="Task A name")
     task_b_name = traits.String(mandatory=False, desc="Task A name")
     hpcutoff = traits.Int(mandatory=False, desc="Cutoff for highpass filtering")
     tempMean = File(exists=True, mandatory=True, desc="mean functional image")
 
 
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.TraitedSpec)  -*-
@@ -37,29 +38,29 @@
     input_spec = FMRIGenSpecInputSpec
     output_spec = FMRIGenSpecOutputSpec
 
     def _run_interface(self, runtime):
 
         if isdefined(self.inputs.hpcutoff):
             self.hpcutoff = self.inputs.hpcutoff
-        elif self.inputs.design_block == 0:
+        elif self.inputs.block_design == BLOCK_DESIGN.RARA:
             self.hpcutoff = self.inputs.task_duration + self.inputs.rest_duration
         else:
             self.hpcutoff = (self.inputs.task_duration + self.inputs.rest_duration) *2
 
         self.hp_sigma_vol = self.hpcutoff / (2 * self.inputs.TR)
 
         self.hpstring = '-bptf %f -1 -add %s' % (self.hp_sigma_vol, self.inputs.tempMean)
 
         if not isdefined(self.inputs.task_a_name):
             self.inputs.task_a_name = "TaskA"
         if not isdefined(self.inputs.task_b_name):
             self.inputs.task_b_name = "TaskB"
 
-        if self.inputs.design_block == 0:
+        if self.inputs.block_design == BLOCK_DESIGN.RARA:
             self.contrasts = [['%s_versus_Rest' % self.inputs.task_a_name, 'T', [self.inputs.task_a_name], [1]]]
 
             self.evs_run = Bunch(
                 conditions=[self.inputs.task_a_name],
                 onsets=[list(range(self.inputs.rest_duration, int(self.inputs.TR * self.inputs.nvols),
                                    (self.inputs.task_duration + self.inputs.rest_duration)))],
                 durations=[[self.inputs.task_duration]]
```

### Comparing `swane-0.0.6/swane/nipype_pipeline/nodes/ForceOrient.py` & `swane-0.1.0/swane/nipype_pipeline/nodes/ForceOrient.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.6/swane/nipype_pipeline/nodes/FslNVols.py` & `swane-0.1.0/swane/nipype_pipeline/nodes/FslNVols.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.6/swane/nipype_pipeline/nodes/GetNiftiTR.py` & `swane-0.1.0/swane/nipype_pipeline/nodes/GetNiftiTR.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.6/swane/nipype_pipeline/nodes/MergeTargets.py` & `swane-0.1.0/swane/nipype_pipeline/nodes/MergeTargets.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.6/swane/nipype_pipeline/nodes/Orient.py` & `swane-0.1.0/swane/nipype_pipeline/nodes/Orient.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.6/swane/nipype_pipeline/nodes/RandomSeedGenerator.py` & `swane-0.1.0/swane/nipype_pipeline/nodes/RandomSeedGenerator.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.6/swane/nipype_pipeline/nodes/SegmentHA.py` & `swane-0.1.0/swane/nipype_pipeline/nodes/SegmentHA.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         mandatory=True,
         position=1,
         argstr="%s",
         hash_files=False,
         desc="path to subjects directory",
         genfile=True,
     )
-    num_threads = traits.Int(argstr="")
+    num_cpu = traits.Int(argstr="")
 
 
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.TraitedSpec)  -*-
 class SegmentHAOutputSpec(TraitedSpec):
     lh_hippoAmygLabels = File(desc="Discrete segmentation volumes at subvoxel resolution")
     rh_hippoAmygLabels = File(desc="Discrete segmentation volumes at subvoxel resolution")
 
@@ -60,18 +60,18 @@
 
     def _parse_inputs(self, skip=None):
         """
         Custom implementation of _parse_inputs func to manage multithreading.
 
         """
 
-        if isdefined(self.inputs.num_threads):
-            skip = ["num_threads"]
-            self.n_procs = self.inputs.num_threads
-            self.inputs.environ["ITK_GLOBAL_DEFAULT_NUMBER_OF_THREADS"] = "%d" % self.inputs.num_threads
+        if isdefined(self.inputs.num_cpu):
+            skip = ["num_cpu"]
+            # self.n_procs = self.inputs.num_threads
+            self.inputs.environ["ITK_GLOBAL_DEFAULT_NUMBER_OF_THREADS"] = "%d" % self.inputs.num_cpu
 
         parse = super(SegmentHA, self)._parse_inputs(skip)
 
         # Delete lock file if exists from previous execution
         ex_path = abspath(
             os.path.join(self.inputs.subjects_dir, self.inputs.subject_id, "scripts/IsRunningHPsubT1.lh+rh"))
```

### Comparing `swane-0.0.6/swane/nipype_pipeline/nodes/SumMultiTracks.py` & `swane-0.1.0/swane/nipype_pipeline/nodes/SumMultiTracks.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,32 +30,31 @@
     input_spec = SumMultiTracksInputSpec
     output_spec = SumMultiTracksOutputSpec
 
     def _run_interface(self, runtime):
         self.inputs.out_file = self._gen_outfilename()
         waytotal_sum_file = self._gen_waytotal_outfilename()
 
-        steps = len(self.inputs.path_files) - 1
+        steps = len(self.inputs.path_files)
         sum_loop = [None] * steps
         sum_res = [None] * steps
-
         waytotal_sum = 0
 
         for x in range(steps):
 
             # SUM FTP_PATHS
             sum_loop[x] = BinaryMaths()
             sum_loop[x].inputs.operation = "add"
 
             if x == 0:
                 sum_loop[x].inputs.in_file = self.inputs.path_files[x]
             else:
                 sum_loop[x].inputs.in_file = sum_res[(x - 1)].outputs.out_file
 
-            sum_loop[x].inputs.operand_file = self.inputs.path_files[(x + 1)]
+            sum_loop[x].inputs.operand_file = self.inputs.path_files[x]
 
             if x == (steps - 1):
                 sum_loop[x].inputs.out_file = self.inputs.out_file
 
             sum_res[x] = sum_loop[x].run()
 
             # SUM WAYTOTAL
```

### Comparing `swane-0.0.6/swane/nipype_pipeline/nodes/SumMultiVols.py` & `swane-0.1.0/swane/nipype_pipeline/nodes/SumMultiVols.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.6/swane/nipype_pipeline/nodes/TTest.py` & `swane-0.1.0/swane/nipype_pipeline/nodes/TTest.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     stat_t = traits.Float(desc="T statistics")
     stat_p = traits.Float(desc="P value")
 
 
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.BaseInterface)  -*-
 class TTest(BaseInterface):
     """
-    Reads the num. of volumes from a 4d NIFTI file.
+    Calculate T statistics of two given distributions
 
     """
 
     input_spec = TTestInputSpec
     output_spec = TTestOutputSpec
 
     def _run_interface(self, runtime):
```

### Comparing `swane-0.0.6/swane/nipype_pipeline/nodes/ThrROI.py` & `swane-0.1.0/swane/nipype_pipeline/nodes/ThrROI.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.6/swane/nipype_pipeline/nodes/VenousCheck.py` & `swane-0.1.0/swane/nipype_pipeline/nodes/Zscore.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,75 @@
 # -*- DISCLAIMER: this file contains code derived from Nipype (https://github.com/nipy/nipype/blob/master/LICENSE)  -*-
 
-import shutil
-from nipype.interfaces.base import InputMultiObject
-from nipype.interfaces.fsl import ImageStats
+from nipype.interfaces.fsl import (BinaryMaths, ImageStats, ApplyMask)
 from os.path import abspath
-from nipype.interfaces.base import (BaseInterface, BaseInterfaceInputSpec, TraitedSpec, File)
+import os
+from nipype.interfaces.base import (BaseInterface, BaseInterfaceInputSpec, TraitedSpec, File, isdefined)
 
 
+# NODO PER CALCOLARE Z SCORE DA ROI
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.BaseInterfaceInputSpec)  -*-
-class VenousCheckInputSpec(BaseInterfaceInputSpec):
-    in_files = InputMultiObject(File(exists=True), desc="List of splitted file")
-    out_file_veins = File(desc='the output venous image')
-    out_file_anat = File(desc='the output anatomic image')
+class ZscoreInputSpec(BaseInterfaceInputSpec):
+    in_file = File(exists=True, mandatory=True, desc='the input image')
+    ROI_file = File(exists=True, mandatory=True, desc='the input image')
+    out_file = File(desc='the output image')
 
 
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.TraitedSpec)  -*-
-class VenousCheckOutputSpec(TraitedSpec):
-    out_file_veins = File(desc='the output venous image')
-    out_file_anat = File(desc='the output anatomic image')
+class ZscoreOutputSpec(TraitedSpec):
+    out_file = File(exists=True, desc='the output image')
 
 
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.BaseInterface)  -*-
-class VenousCheck(BaseInterface):
+class Zscore(BaseInterface):
     """
-    Recognises the venous phase from the anatomic image of a phase contrast sequence based on its standard deviation.
+    Calculates the z-score index of an image compared with a ROI.
 
     """
     
-    input_spec = VenousCheckInputSpec
-    output_spec = VenousCheckOutputSpec
+    input_spec = ZscoreInputSpec
+    output_spec = ZscoreOutputSpec
 
     def _run_interface(self, runtime):
-        self.inputs.out_file_veins = abspath("veins.nii.gz")
-        self.inputs.out_file_anat = abspath("veins_anat.nii.gz")
-        s0 = ImageStats()
-        s0.inputs.in_file = self.inputs.in_files[0]
-        s0.inputs.op_string = "-s"
-        res0 = s0.run()
-        s1 = ImageStats()
-        s1.inputs.in_file = self.inputs.in_files[1]
-        s1.inputs.op_string = "-s"
-        res1 = s1.run()
-        if res0.outputs.out_stat < res1.outputs.out_stat:
-            shutil.copy(self.inputs.in_files[0], self.inputs.out_file_veins)
-            shutil.copy(self.inputs.in_files[1], self.inputs.out_file_anat)
-        else:
-            shutil.copy(self.inputs.in_files[1], self.inputs.out_file_veins)
-            shutil.copy(self.inputs.in_files[0], self.inputs.out_file_anat)
+        self.inputs.out_file = self._gen_outfilename()
+
+        mask = ApplyMask()
+        mask.inputs.in_file = self.inputs.in_file
+        mask.inputs.mask_file = self.inputs.ROI_file
+        mask.inputs.out_file = abspath("mask_" + os.path.basename(self.inputs.in_file))
+        res_mask = mask.run()
+
+        mean = ImageStats()
+        mean.inputs.in_file = res_mask.outputs.out_file
+        mean.inputs.op_string = "-M"
+        mean_res = mean.run()
+
+        sd = ImageStats()
+        sd.inputs.in_file = res_mask.outputs.out_file
+        sd.inputs.op_string = "-S"
+        sd_res = sd.run()
+
+        sub = BinaryMaths()
+        sub.inputs.in_file = self.inputs.in_file
+        sub.inputs.operation = "sub"
+        sub.inputs.operand_value = mean_res.outputs.out_stat
+        sub_res = sub.run()
+
+        div = BinaryMaths()
+        div.inputs.in_file = sub_res.outputs.out_file
+        div.inputs.operation = "div"
+        div.inputs.operand_value = sd_res.outputs.out_stat
+        div.inputs.out_file = self.inputs.out_file
+        div.run()
 
         return runtime
 
+    def _gen_outfilename(self):
+        out_file = self.inputs.out_file
+        if not isdefined(out_file) and isdefined(self.inputs.in_file):
+            out_file = "zscore_" + os.path.basename(self.inputs.in_file)
+        return abspath(out_file)
+
     def _list_outputs(self):
         outputs = self.output_spec().get()
-        outputs['out_file_veins'] = abspath("veins.nii.gz")
-        outputs['out_file_anat'] = abspath("veins_anat.nii.gz")
+        outputs['out_file'] = self._gen_outfilename()
         return outputs
```

### Comparing `swane-0.0.6/swane/nipype_pipeline/workflows/FLAT1_workflow.py` & `swane-0.1.0/swane/nipype_pipeline/workflows/flat1_workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import swane_supplement
 
-from nipype.interfaces.fsl import (ApplyWarp, ApplyMask, BinaryMaths, FAST, ImageStats, )
+from nipype.interfaces.fsl import (ApplyWarp, ApplyMask, BinaryMaths, FAST, ImageStats, SpatialFilter)
 from nipype.pipeline.engine import Node
 
 from swane.nipype_pipeline.nodes.utils import getn
 from swane.nipype_pipeline.engine.CustomWorkflow import CustomWorkflow
 from swane.nipype_pipeline.nodes.ThrROI import ThrROI
-from swane.nipype_pipeline.nodes.CustomDilateImage import CustomDilateImage
 from swane.nipype_pipeline.nodes.FLAT1OutliersMask import FLAT1OutliersMask
 
 from nipype.interfaces.utility import IdentityInterface
 
 
-def FLAT1_workflow(name: str, mni1_dir: str, base_dir: str = "/")  -> CustomWorkflow:
+def flat1_workflow(name: str, mni1_dir: str, base_dir: str = "/") -> CustomWorkflow:
     """
     Creation of a junction and extension z-score map based on T13D, FLAIR3D and
     a mean template.
 
     Parameters
     ----------
     name : str
@@ -60,16 +59,15 @@
 
     """
     
     workflow = CustomWorkflow(name=name, base_dir=base_dir)
 
     # Input Node
     inputnode = Node(
-        IdentityInterface(fields=['ref_brain', 'flair_brain', 'ref_2_mni1_warp',
-                                  'ref_2_mni1_inverse_warp']),
+        IdentityInterface(fields=['ref_brain', 'flair_brain', 'ref_2_mni1_warp', 'ref_2_mni1_inverse_warp']),
         name='inputnode')
     
     # Output Node
     outputnode = Node(
         IdentityInterface(fields=['extension_z', 'junction_z', 'binary_flair']),
         name='outputnode')
 
@@ -169,17 +167,17 @@
     binary_flair.long_name = "Mean based masking"
     binary_flair.inputs.out_file = "binary_flair.nii.gz"
     workflow.connect(cortex_mask, "out_file", binary_flair, "in_file")
     workflow.connect(gm_mean, "out_stat", binary_flair, "seg_val_max")
     workflow.connect(wm_mean, "out_stat", binary_flair, "seg_val_min")
 
     # NODE 14: Junction map generation
-    convolution_flair = Node(CustomDilateImage(), name="%s_convolution_flair" % name)
+    convolution_flair = Node(SpatialFilter(), name="%s_convolution_flair" % name)
     convolution_flair.long_name = "junction map generation"
-    convolution_flair.inputs.args = "-fmean"
+    convolution_flair.inputs.operation = "mean"
     convolution_flair.inputs.kernel_shape = "boxv"
     convolution_flair.inputs.kernel_size = 5
     convolution_flair.inputs.out_file = "convolution_flair.nii.gz"
     workflow.connect(binary_flair, "out_file", convolution_flair, "in_file")
 
     # NODE 13: Junction map mean value calculation
     junction_mean = Node(BinaryMaths(), name="%s_junction_mean" % name)
@@ -221,17 +219,17 @@
     normalised_gm_mask.long_name = "Grey matter/cerebellum normalization"
     normalised_gm_mask.inputs.operation = "div"
     normalised_gm_mask.inputs.out_file = "normalised_GM_mask.nii.gz"
     workflow.connect(restore_gm_mask, "out_file", normalised_gm_mask, "in_file")
     workflow.connect(cerebellum_mean, "out_stat", normalised_gm_mask, "operand_value")
 
     # NODE 19: Extension map generation
-    smoothed_image_extension = Node(CustomDilateImage(), name="%s_smoothed_image_extension" % name)
+    smoothed_image_extension = Node(SpatialFilter(), name="%s_smoothed_image_extension" % name)
     smoothed_image_extension.long_name = "extension map generation"
-    smoothed_image_extension.inputs.args = "-fmean"
+    smoothed_image_extension.inputs.operation = "mean"
     smoothed_image_extension.inputs.kernel_shape = "boxv"
     smoothed_image_extension.inputs.kernel_size = 5
     smoothed_image_extension.inputs.out_file = "smoothed_image_extension.nii.gz"
     workflow.connect(normalised_gm_mask, "out_file", smoothed_image_extension, "in_file")
 
     # NODE 20: Extension map mean value calculation
     extension_mean = Node(BinaryMaths(), name="%s_image_extension" % name)
```

### Comparing `swane-0.0.6/swane/nipype_pipeline/workflows/dti_preproc_workflow.py` & `swane-0.1.0/swane/nipype_pipeline/workflows/dti_preproc_workflow.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from nipype.interfaces.fsl import (BET, FLIRT, ConvertXFM, ExtractROI, EddyCorrect, DTIFit, ApplyXFM, FNIRT)
 from nipype.pipeline.engine import Node
-import os
-
+from swane.config.config_enums import CORE_LIMIT
 from swane.nipype_pipeline.engine.CustomWorkflow import CustomWorkflow
 from swane.nipype_pipeline.nodes.CustomDcm2niix import CustomDcm2niix
 from swane.nipype_pipeline.nodes.ForceOrient import ForceOrient
 from swane.nipype_pipeline.nodes.CustomBEDPOSTX5 import CustomBEDPOSTX5
-
+from swane.nipype_pipeline.nodes.GenEddyFiles import GenEddyFiles
+from swane.nipype_pipeline.nodes.CustomEddy import CustomEddy
+from configparser import SectionProxy
 from nipype.interfaces.utility import IdentityInterface
+from multiprocessing import cpu_count
 
 
-def dti_preproc_workflow(name: str, dti_dir: str, mni_dir: str = None, base_dir: str = "/", is_tractography: bool = False) -> CustomWorkflow:
+def dti_preproc_workflow(name: str, dti_dir: str, config: SectionProxy, mni_dir: str = None, base_dir: str = "/",
+                         max_cpu: int = 0, multicore_node_limit: CORE_LIMIT = CORE_LIMIT.SOFT_CAP) -> CustomWorkflow:
     """
     DTI preprocessing workflow with eddy current and motion artifact correction.
     Diffusion metrics calculation and, if needed, bayesian estimation of
     diffusion parameters.
 
     Parameters
     ----------
@@ -22,16 +25,20 @@
         The workflow name.
     dti_dir : path
         The directory path of DTI dicom files.
     mni_dir : path, optional
         The file path of the MNI template. The default is None.
     base_dir : path, optional
         The base directory path relative to parent workflow. The default is "/".
-    is_tractography : bool, optional
-        Enable bayesian estimation of diffusion parameters. The default is False.
+    config: SectionProxy
+        workflow settings.
+    max_cpu : int, optional
+        If greater than 0, limit the core usage of bedpostx. The default is 0.
+    multicore_node_limit: CORE_LIMIT, optional
+        Preference for bedpostX core usage. The default il CORE_LIMIT.SOFT_CAP
         
     Input Node Fields
     ----------
     ref_brain : path
         Betted T13D reference file.
 
     Returns
@@ -70,19 +77,22 @@
     # Output Node
     outputnode = Node(
         IdentityInterface(fields=['nodiff_mask_file', 'FA', 'fsamples', 'phsamples',
                                   'thsamples', 'diff2ref_mat', "ref2diff_mat", "mni2ref_warp",
                                   ]),
         name='outputnode')
 
+    is_cuda = config.getboolean_safe('cuda')
+
     # NODE 1: Conversion dicom -> nifti
     conv = Node(CustomDcm2niix(), name='dti_conv')
     conv.inputs.source_dir = dti_dir
     conv.inputs.out_filename = "dti"
     conv.inputs.bids_format = False
+    conv.inputs.request_dti = True
 
     # NODE 1b: Orienting in radiological convention
     reorient = Node(ForceOrient(), name='dti_reOrient')
     workflow.connect(conv, "converted_files", reorient, "in_file")
 
     # NODE 2: b0 image extraction
     nodif = Node(ExtractROI(), name='dti_nodif')
@@ -96,24 +106,52 @@
     bet = Node(BET(), name='nodif_BET')
     bet.inputs.frac = 0.3
     bet.inputs.robust = True
     bet.inputs.threshold = True
     bet.inputs.mask = True
     workflow.connect(nodif, "roi_file", bet, "in_file")
 
-    # NODE 4: Eddy current and motion artifact correction
-    eddy = Node(EddyCorrect(), name='dti_eddy')
-    eddy.inputs.ref_num = 0
-    eddy.inputs.out_file = "data.nii.gz"
-    workflow.connect(reorient, "out_file", eddy, "in_file")
+    old_eddy_correct = config.getboolean_safe("old_eddy_correct")
+    if old_eddy_correct:
+        # NODE 4a: Generate Eddy files
+        eddy = Node(EddyCorrect(), name='dti_eddy')
+        eddy.inputs.ref_num = 0
+        eddy.inputs.out_file = "data.nii.gz"
+        workflow.connect(reorient, "out_file", eddy, "in_file")
+        eddy_output_name = "eddy_corrected"
+    else:
+        # NODE 4a: Generate Eddy files
+        eddy_files = Node(GenEddyFiles(), name="dti_eddy_files")
+        workflow.connect(conv, "bvals", eddy_files, "bval")
+
+        # NODE 4: Eddy current and motion artifact correction
+        eddy = Node(CustomEddy(), name="dti_eddy")
+        eddy.inputs.use_gpu = is_cuda
+        if not is_cuda:
+            if multicore_node_limit == CORE_LIMIT.HARD_CAP:
+                eddy_cpu = max_cpu
+                eddy.inputs.num_threads = max_cpu
+            elif multicore_node_limit == CORE_LIMIT.SOFT_CAP:
+                eddy_cpu = max_cpu
+            else:
+                eddy_cpu = cpu_count()
+            eddy.inputs.environ = {'OMP_NUM_THREADS': str(eddy_cpu), 'FSL_SKIP_GLOBAL': '1'}
+
+        workflow.connect(reorient, "out_file", eddy, "in_file")
+        workflow.connect(conv, "bvals", eddy, "in_bval")
+        workflow.connect(conv, "bvecs", eddy, "in_bvec")
+        workflow.connect(eddy_files, "acqp", eddy, "in_acqp")
+        workflow.connect(eddy_files, "index", eddy, "in_index")
+        workflow.connect(bet, "mask_file", eddy, "in_mask")
+        eddy_output_name = "out_corrected"
 
     # NODE 5: DTI metrics calculation
     dtifit = Node(DTIFit(), name='dti_dtifit')
     dtifit.long_name = "DTI metrics calculation"
-    workflow.connect(eddy, "eddy_corrected", dtifit, "dwi")
+    workflow.connect(eddy, eddy_output_name, dtifit, "dwi")
     workflow.connect(bet, "mask_file", dtifit, "mask")
     workflow.connect(conv, "bvecs", dtifit, "bvecs")
     workflow.connect(conv, "bvals", dtifit, "bvals")
 
     # NODE 6: b0 image linear registration in reference space
     flirt = Node(FLIRT(), name='diff2ref_FLIRT')
     flirt.long_name = "%s to reference space"
@@ -124,22 +162,25 @@
     flirt.inputs.searchr_z = [-90, 90]
     flirt.inputs.dof = 6
     workflow.connect(bet, "out_file", flirt, "in_file")
     workflow.connect(inputnode, "ref_brain", flirt, "reference")
 
     # NODE 7: FA linear transformation in reference space
     fa_2_ref_flirt = Node(ApplyXFM(), name='FA2ref_FLIRT')
+    fa_2_ref_flirt.long_name = "FA %s in reference space"
     fa_2_ref_flirt.inputs.out_file = "r-FA.nii.gz"
     fa_2_ref_flirt.inputs.interp = "trilinear"
     workflow.connect(dtifit, "FA", fa_2_ref_flirt, "in_file")
     workflow.connect(flirt, "out_matrix_file", fa_2_ref_flirt, "in_matrix_file")
     workflow.connect(inputnode, "ref_brain", fa_2_ref_flirt, "reference")
     
     workflow.connect(fa_2_ref_flirt, 'out_file', outputnode, 'FA')
 
+    is_tractography = config.getboolean_safe('tractography')
+
     if is_tractography:
         # NODE 1: Linear registration
         mni_2_ref_flirt = Node(FLIRT(), name='mni_2_ref_flirt')
         mni_2_ref_flirt.long_name = "atlas %s to diffusion space"
         mni_2_ref_flirt.inputs.searchr_x = [-90, 90]
         mni_2_ref_flirt.inputs.searchr_y = [-90, 90]
         mni_2_ref_flirt.inputs.searchr_z = [-90, 90]
@@ -161,15 +202,24 @@
         # NODE 8: Bayesian estimation of diffusion parameters
         bedpostx = Node(CustomBEDPOSTX5(), name='dti_bedpostx')
         bedpostx.inputs.n_fibres = 2
         bedpostx.inputs.rician = True
         bedpostx.inputs.sample_every = 25
         bedpostx.inputs.n_jumps = 1250
         bedpostx.inputs.burn_in = 1000
-        workflow.connect(eddy, "eddy_corrected", bedpostx, "dwi")
+        bedpostx.inputs.use_gpu = is_cuda
+        if not is_cuda:
+            # if cuda is enabled only 1 process is launched
+            if multicore_node_limit == CORE_LIMIT.SOFT_CAP:
+                bedpostx.inputs.environ = {'FSLSUB_PARALLEL': str(max_cpu)}
+            elif multicore_node_limit == CORE_LIMIT.HARD_CAP:
+                bedpostx.inputs.environ = {'FSLSUB_PARALLEL': str(max_cpu)}
+                bedpostx.inputs.num_threads = max_cpu
+
+        workflow.connect(eddy, eddy_output_name, bedpostx, "dwi")
         workflow.connect(bet, "mask_file", bedpostx, "mask")
         workflow.connect(conv, "bvecs", bedpostx, "bvecs")
         workflow.connect(conv, "bvals", bedpostx, "bvals")
 
         # NODE 9: Linear transformation inverse matrix calculation from diffusion to reference space
         ref2diff_convert = Node(ConvertXFM(), name='ref2diff_convert')
         ref2diff_convert.long_name = "inverse transformation from reference space"
```

### Comparing `swane-0.0.6/swane/nipype_pipeline/workflows/freesurfer_asymmetry_index_workflow.py` & `swane-0.1.0/swane/nipype_pipeline/workflows/freesurfer_asymmetry_index_workflow.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 from nipype.interfaces.fsl import ImageMaths, ImageStats, ApplyMask, BinaryMaths
 
 from nipype import Node, Merge
 
 from swane.nipype_pipeline.engine.CustomWorkflow import CustomWorkflow
 from swane.nipype_pipeline.nodes.TTest import TTest
 from swane.nipype_pipeline.nodes.SumMultiVols import SumMultiVols
-from swane.nipype_pipeline.nodes.Zscore import Zscore
+from swane.nipype_pipeline.nodes.utils import getn
 
 from nipype.interfaces.utility import IdentityInterface
 
-
 lh_labels = [
-    17,      # Left-Hippocampus                        220 216 20  0
-    18,      # Left-Amygdala                           103 255 255 0
+    17,      # Left-Hippocampus                    220 216 20  0
+    18,      # Left-Amygdala                       103 255 255 0
     1000,    # ctx-lh-unknown                      25  5   25  0
     1001,    # ctx-lh-bankssts                     25  100 40  0
     1002,    # ctx-lh-caudalanteriorcingulate      125 100 160 0
     1003,    # ctx-lh-caudalmiddlefrontal          100 25  0   0
     1004,    # ctx-lh-corpuscallosum               120 70  50  0
     1005,    # ctx-lh-cuneus                       220 20  100 0
     1006,    # ctx-lh-entorhinal                   220 20  10  0
@@ -49,52 +48,52 @@
     1032,    # ctx-lh-frontalpole                  100 0   100 0
     1033,    # ctx-lh-temporalpole                 70  70  70  0
     1034,    # ctx-lh-transversetemporal           150 150 200 0
     1035,    # ctx-lh-insula                       255 192 32  0
 ]
 
 labels_rh = [
-    53,     # Right - Hippocampus                       220 216 20  0
-    54,     # Right - Amygdala                          103 255 255 0
+    53,     # Right - Hippocampus                 220 216 20  0
+    54,     # Right - Amygdala                    103 255 255 0
     2000,   # ctx-rh-unknown                      25  5   25  0
-    2001,   #    ctx-rh-bankssts                     25  100 40  0
-    2002,   #    ctx-rh-caudalanteriorcingulate      125 100 160 0
-    2003,   #    ctx-rh-caudalmiddlefrontal          100 25  0   0
-    2004,   #    ctx-rh-corpuscallosum               120 70  50  0
-    2005,   #    ctx-rh-cuneus                       220 20  100 0
-    2006,   #    ctx-rh-entorhinal                   220 20  10  0
-    2007,   #   ctx-rh-fusiform                     180 220 140 0
-    2008,   #    ctx-rh-inferiorparietal             220 60  220 0
-    2009,   #    ctx-rh-inferiortemporal             180 40  120 0
-    2010,   #    ctx-rh-isthmuscingulate             140 20  140 0
-    2011,   #    ctx-rh-lateraloccipital             20  30  140 0
-    2012,   #    ctx-rh-lateralorbitofrontal         35  75  50  0
-    2013,   #    ctx-rh-lingual                      225 140 140 0
-    2014,   #    ctx-rh-medialorbitofrontal          200 35  75  0
-    2015,   #    ctx-rh-middletemporal               160 100 50  0
-    2016,   #   ctx-rh-parahippocampal              20  220 60  0
-    2017,   #    ctx-rh-paracentral                  60  220 60  0
-    2018,   #    ctx-rh-parsopercularis              220 180 140 0
-    2019,   #    ctx-rh-parsorbitalis                20  100 50  0
-    2020,   #    ctx-rh-parstriangularis             220 60  20  0
-    2021,   #    ctx-rh-pericalcarine                120 100 60  0
-    2022,   #    ctx-rh-postcentral                  220 20  20  0
-    2023,   #    ctx-rh-posteriorcingulate           220 180 220 0
-    2024,   #    ctx-rh-precentral                   60  20  220 0
-    2025,   #    ctx-rh-precuneus                    160 140 180 0
-    2026,   #    ctx-rh-rostralanteriorcingulate     80  20  140 0
-    2027,   #    ctx-rh-rostralmiddlefrontal         75  50  125 0
-    2028,   #    ctx-rh-superiorfrontal              20  220 160 0
-    2029,   #    ctx-rh-superiorparietal             20  180 140 0
-    2030,   #    ctx-rh-superiortemporal             140 220 220 0
-    2031,   #    ctx-rh-supramarginal                80  160 20  0
-    2032,   #    ctx-rh-frontalpole                  100 0   100 0
-    2033,   #    ctx-rh-temporalpole                 70  70  70  0
-    2034,   #    ctx-rh-transversetemporal           150 150 200 0
-    2035,   #    ctx-rh-insula                       255 192 32  0
+    2001,   # ctx-rh-bankssts                     25  100 40  0
+    2002,   # ctx-rh-caudalanteriorcingulate      125 100 160 0
+    2003,   # ctx-rh-caudalmiddlefrontal          100 25  0   0
+    2004,   # ctx-rh-corpuscallosum               120 70  50  0
+    2005,   # ctx-rh-cuneus                       220 20  100 0
+    2006,   # ctx-rh-entorhinal                   220 20  10  0
+    2007,   # ctx-rh-fusiform                     180 220 140 0
+    2008,   # ctx-rh-inferiorparietal             220 60  220 0
+    2009,   # ctx-rh-inferiortemporal             180 40  120 0
+    2010,   # ctx-rh-isthmuscingulate             140 20  140 0
+    2011,   # ctx-rh-lateraloccipital             20  30  140 0
+    2012,   # ctx-rh-lateralorbitofrontal         35  75  50  0
+    2013,   # ctx-rh-lingual                      225 140 140 0
+    2014,   # ctx-rh-medialorbitofrontal          200 35  75  0
+    2015,   # ctx-rh-middletemporal               160 100 50  0
+    2016,   # ctx-rh-parahippocampal              20  220 60  0
+    2017,   # ctx-rh-paracentral                  60  220 60  0
+    2018,   # ctx-rh-parsopercularis              220 180 140 0
+    2019,   # ctx-rh-parsorbitalis                20  100 50  0
+    2020,   # ctx-rh-parstriangularis             220 60  20  0
+    2021,   # ctx-rh-pericalcarine                120 100 60  0
+    2022,   # ctx-rh-postcentral                  220 20  20  0
+    2023,   # ctx-rh-posteriorcingulate           220 180 220 0
+    2024,   # ctx-rh-precentral                   60  20  220 0
+    2025,   # ctx-rh-precuneus                    160 140 180 0
+    2026,   # ctx-rh-rostralanteriorcingulate     80  20  140 0
+    2027,   # ctx-rh-rostralmiddlefrontal         75  50  125 0
+    2028,   # ctx-rh-superiorfrontal              20  220 160 0
+    2029,   # ctx-rh-superiorparietal             20  180 140 0
+    2030,   # ctx-rh-superiortemporal             140 220 220 0
+    2031,   # ctx-rh-supramarginal                80  160 20  0
+    2032,   # ctx-rh-frontalpole                  100 0   100 0
+    2033,   # ctx-rh-temporalpole                 70  70  70  0
+    2034,   # ctx-rh-transversetemporal           150 150 200 0
+    2035,   # ctx-rh-insula                       255 192 32  0
 ]
 
 
 def get_symmetric(index):
     if index >= 1000:
         return index+1000
     if index == 17:
@@ -140,20 +139,21 @@
     # Input Node
     inputnode = Node(
         IdentityInterface(fields=['in_file', 'seg_file']),
         name='inputnode')
 
     # Output Node
     outputnode = Node(
-        IdentityInterface(fields=['asymmetry_t', 'asymmetry_p', 'asymmetry_z']),
+        IdentityInterface(fields=['asymmetry_t', 'asymmetry_p', 'asymmetry_z', 'asymmetry_ai']),
         name='outputnode')
 
-    merge_node_t = Node(Merge(len(lh_labels)*2), name="merge_node_t")
+    merge_node_t = Node(Merge(len(lh_labels) * 2), name="merge_node_t")
     merge_node_p = Node(Merge(len(lh_labels) * 2), name="merge_node_p")
     merge_node_z = Node(Merge(len(lh_labels) * 2), name="merge_node_z")
+    merge_node_ai = Node(Merge(len(lh_labels) * 2), name="merge_node_ai")
     index = 1
 
     for lh_label in lh_labels:
 
         rh_label = get_symmetric(lh_label)
         if rh_label == -1:
             continue
@@ -188,14 +188,52 @@
         rh_stats.inputs.op_string = "-M -S -V"
         workflow.connect(rh_apply_mask, "out_file", rh_stats, "in_file")
 
         t_test = Node(TTest(), name="ttest_%d" % lh_label)
         workflow.connect(lh_stats, "out_stat", t_test, "stats_lh")
         workflow.connect(rh_stats, "out_stat", t_test, "stats_rh")
 
+        lh_ai_sum = Node(BinaryMaths(), name="lh_ai_sum_%d" % lh_label)
+        lh_ai_sum.inputs.operation = "add"
+        workflow.connect(inputnode, "in_file", lh_ai_sum, "in_file")
+        workflow.connect(rh_stats, ('out_stat', getn, 0), lh_ai_sum, "operand_value")
+
+        lh_ai_sub = Node(BinaryMaths(), name="lh_ai_sub_%d" % lh_label)
+        lh_ai_sub.inputs.operation = "sub"
+        workflow.connect(inputnode, "in_file", lh_ai_sub, "in_file")
+        workflow.connect(rh_stats, ('out_stat', getn, 0), lh_ai_sub, "operand_value")
+
+        lh_ai = Node(BinaryMaths(), name="lh_ai_%d" % lh_label)
+        lh_ai.inputs.operation = "div"
+        workflow.connect(lh_ai_sub, "out_file", lh_ai, "in_file")
+        workflow.connect(lh_ai_sum, "out_file", lh_ai, "operand_file")
+
+        lh_ai_mask = Node(ApplyMask(), name="lh_ai_applymask_%d" % lh_label)
+        workflow.connect(lh_ai, "out_file", lh_ai_mask, "in_file")
+        workflow.connect(lh_mask, "out_file", lh_ai_mask, "mask_file")
+
+        rh_ai_sum = Node(BinaryMaths(), name="rh_ai_sum_%d" % rh_label)
+        rh_ai_sum.inputs.operation = "add"
+        workflow.connect(inputnode, "in_file", rh_ai_sum, "in_file")
+        workflow.connect(rh_stats, ('out_stat', getn, 0), rh_ai_sum, "operand_value")
+
+        rh_ai_sub = Node(BinaryMaths(), name="rh_ai_sub_%d" % rh_label)
+        rh_ai_sub.inputs.operation = "sub"
+        workflow.connect(inputnode, "in_file", rh_ai_sub, "in_file")
+        workflow.connect(rh_stats, ('out_stat', getn, 0), rh_ai_sub, "operand_value")
+
+        rh_ai = Node(BinaryMaths(), name="rh_ai_%d" % rh_label)
+        rh_ai.inputs.operation = "div"
+        workflow.connect(rh_ai_sub, "out_file", rh_ai, "in_file")
+        workflow.connect(rh_ai_sum, "out_file", rh_ai, "operand_file")
+
+        rh_ai_mask = Node(ApplyMask(), name="rh_ai_applymask_%d" % rh_label)
+        workflow.connect(rh_ai, "out_file", rh_ai_mask, "in_file")
+        workflow.connect(rh_mask, "out_file", rh_ai_mask, "mask_file")
+
         lh_value_t = Node(BinaryMaths(), name="lh_value_t_%d" % lh_label)
         lh_value_t.inputs.operation = "mul"
         workflow.connect(lh_mask, "out_file", lh_value_t, "in_file")
         workflow.connect(t_test, "stat_t", lh_value_t, "operand_value")
 
         rh_value_t = Node(BinaryMaths(), name="rh_value_t_%d" % lh_label)
         rh_value_t.inputs.operation = "mul"
@@ -224,27 +262,33 @@
         workflow.connect(inputnode, "in_file", rh_z, "in_file")
         workflow.connect(lh_stats, ('out_stat', get_z_op_string), rh_z, 'op_string')
         workflow.connect(rh_mask, "out_file", rh_z, "in_file2")
 
         workflow.connect(lh_value_t, "out_file", merge_node_t, 'in%d' % index)
         workflow.connect(lh_value_p, "out_file", merge_node_p, 'in%d' % index)
         workflow.connect(lh_z, "out_file", merge_node_z, 'in%d' % index)
+        workflow.connect(lh_ai_mask, "out_file", merge_node_ai, 'in%d' % index)
         index += 1
         workflow.connect(rh_value_t, "out_file", merge_node_t, 'in%d' % index)
         workflow.connect(lh_value_p, "out_file", merge_node_p, 'in%d' % index)
         workflow.connect(rh_z, "out_file", merge_node_z, 'in%d' % index)
+        workflow.connect(rh_ai_mask, "out_file", merge_node_ai, 'in%d' % index)
         index += 1
 
     sum_masks_t = Node(SumMultiVols(), name="sum_masks_t")
     workflow.connect(merge_node_t, "out", sum_masks_t, "vol_files")
 
     sum_masks_p = Node(SumMultiVols(), name="sum_masks_p")
     workflow.connect(merge_node_p, "out", sum_masks_p, "vol_files")
 
     sum_masks_z = Node(SumMultiVols(), name="sum_masks_z")
     workflow.connect(merge_node_z, "out", sum_masks_z, "vol_files")
 
+    sum_masks_ai = Node(SumMultiVols(), name="sum_masks_ai")
+    workflow.connect(merge_node_ai, "out", sum_masks_ai, "vol_files")
+
     workflow.connect(sum_masks_t, "out_file", outputnode, "asymmetry_t")
     workflow.connect(sum_masks_p, "out_file", outputnode, "asymmetry_p")
     workflow.connect(sum_masks_z, "out_file", outputnode, "asymmetry_z")
+    workflow.connect(sum_masks_ai, "out_file", outputnode, "asymmetry_ai")
 
     return workflow
```

### Comparing `swane-0.0.6/swane/nipype_pipeline/workflows/freesurfer_workflow.py` & `swane-0.1.0/swane/nipype_pipeline/workflows/freesurfer_workflow.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 from nipype.interfaces.freesurfer import ReconAll
 from nipype.interfaces.fsl import BinaryMaths
-
+from multiprocessing import cpu_count
 from nipype.pipeline.engine import Node
-
+from math import trunc
 from swane.nipype_pipeline.nodes.utils import getn
 from swane.nipype_pipeline.engine.CustomWorkflow import CustomWorkflow
 from swane.nipype_pipeline.nodes.SegmentHA import SegmentHA
 from swane.nipype_pipeline.nodes.CustomLabel2Vol import CustomLabel2Vol
 from swane.nipype_pipeline.nodes.ThrROI import ThrROI
-
+from swane.config.config_enums import CORE_LIMIT
 from nipype.interfaces.utility import IdentityInterface
 
 FS_DIR = "FS"
 
 
-def freesurfer_workflow(name: str, is_hippo_amyg_labels: bool, base_dir: str = "/")  -> CustomWorkflow:
+def freesurfer_workflow(name: str, is_hippo_amyg_labels: bool, base_dir: str = "/", max_cpu: int = 0,
+                        multicore_node_limit: CORE_LIMIT = CORE_LIMIT.SOFT_CAP) -> CustomWorkflow:
     """
     Freesurfer cortical reconstruction, white matter ROI, basal ganglia and thalami ROI.
     If needed, segmentation of the hippocampal substructures and the nuclei of the amygdala.
 
     Parameters
     ----------
     name : str
         The workflow name.
     is_hippo_amyg_labels : bool
         Enable segmentation of the hippocampal substructures and the nuclei of the amygdala.
     base_dir : path, optional
         The base directory path relative to parent workflow. The default is "/".
+    max_cpu : int, optional
+        If greater than 0, limit the core usage of bedpostx. The default is 0.
+    multicore_node_limit: CORE_LIMIT, optional
+        Preference for bedpostX core usage. The default il CORE_LIMIT.SOFT_CAP
         
     Input Node Fields
     ----------
-    max_node_cpu : int
-        Max number of cpu to use for the workflow.
     ref : path
         T13D reference file.
     subjects_dir : path
         Directory for Freesurfer analysis.
 
     Returns
     -------
@@ -44,86 +47,90 @@
         
     Output Node Fields
     ----------
     subject_id : string
         Subject name for Freesurfer (defined as FS_DIR="FS").
     subjects_dir : path
         Directory for Freesurfer analysis.
-    bgtROI : path
+    bgROI : path
         Binary ROI for basal ganglia and thalamus.
     wmROI : path
         Binary ROI for cerebral white matter.
     pial : list of strings
         Gray matter/pia mater rh and lh surfaces.
     white : list of strings
         White/gray matter rh and lh surfaces.
     vol_label_file : path
         Aparc parcellation projected into aseg volume in reference space.
+    vol_label_file_nii : path
+        Aparc parcellation projected into aseg volume in reference space and nifti format.
     lh_hippoAmygLabels : path
         Left side labels from segmentation of the hippocampal substructures and the nuclei of the amygdala.
     rh_hippoAmygLabels : path
         Right side labels from segmentation of the hippocampal substructures and the nuclei of the amygdala.
 
     """
     
     workflow = CustomWorkflow(name=name, base_dir=base_dir)
 
     # Input Node
     inputnode = Node(
-        IdentityInterface(fields=['max_node_cpu', 'ref', 'subjects_dir']),
+        IdentityInterface(fields=['ref', 'subjects_dir']),
         name='inputnode')
     
     # Output Node
     outputnode = Node(
-        IdentityInterface(fields=['subject_id', 'subjects_dir', 'bgtROI', 'wmROI',
-                                  'pial', 'white', 'vol_label_file', 'vol_label_file_nii', 'lh_hippoAmygLabels',
-                                  'rh_hippoAmygLabels']),
+        IdentityInterface(fields=['subject_id', 'subjects_dir', 'bgROI', 'wmROI', 'pial', 'white', 'vol_label_file',
+                                  'vol_label_file_nii', 'lh_hippoAmygLabels', 'rh_hippoAmygLabels']),
         name='outputnode')
 
-    def check_fov_dim(nifti):
-        import subprocess
-        for x in range(1, 4, 1):
-            cmd = "echo $( echo $(fslval " + nifti + " dim" + str(x) + ") \\* $(fslval " + nifti + " pixdim" + str(x) + ") | bc)"
-            output = subprocess.run(cmd, shell=True, stdout=subprocess.PIPE).stdout.decode('utf-8')
-            try:
-                fovdim = float(output)
-                if fovdim > 256:
-                    return "-cw256"
-            except:
-                pass
-        return ""
-
     # NODE 1: Freesurfer cortical reconstruction process
-    reconAll = Node(ReconAll(), name='reconAll')
-    reconAll.inputs.subject_id = FS_DIR
-    reconAll.inputs.parallel = True
-    reconAll.inputs.directive = 'all'
-    workflow.add_nodes([reconAll])
-    workflow.connect(inputnode, "max_node_cpu", reconAll, "openmp")
-    workflow.connect(inputnode, "ref", reconAll, "T1_files")
-    workflow.connect(inputnode, ('ref', check_fov_dim), reconAll, 'flags')
-    workflow.connect(inputnode, "subjects_dir", reconAll, "subjects_dir")
+    recon_all = Node(ReconAll(), name='reconAll')
+    recon_all.inputs.subject_id = FS_DIR
+
+    # parallel option split some steps in right and left
+    if max_cpu > 1:
+        recon_all.inputs.parallel = True
+
+    # openmp option apply max cpu tu some steps, resulting in twice cpu usage for rogh/left steps
+    if multicore_node_limit == CORE_LIMIT.NO_LIMIT:
+        # no limit
+        recon_all.inputs.openmp = cpu_count()
+    elif multicore_node_limit == CORE_LIMIT.SOFT_CAP:
+        # for soft cap we accept that parallelized steps use each max_cpu cores, resulting in twice the setting
+        recon_all.inputs.openmp = max_cpu
+        recon_all.n_procs = recon_all.inputs.openmp
+    else:
+        # for hard cap we use half of max_cpu setting, but at least 1
+        recon_all.inputs.openmp = max(trunc(max_cpu/2), 1)
+        recon_all.n_procs = recon_all.inputs.openmp * 2
+
+    recon_all.inputs.directive = 'all'
+    recon_all.inputs.args = "-no-isrunning"
+    workflow.add_nodes([recon_all])
+    workflow.connect(inputnode, "ref", recon_all, "T1_files")
+    workflow.connect(inputnode, "subjects_dir", recon_all, "subjects_dir")
 
     # NODE 2: Aparcaseg linear transformation in reference space
     aparaseg2Volmgz = Node(CustomLabel2Vol(), name="aparaseg2Volmgz")
     aparaseg2Volmgz.long_name = "label %s to reference space"
     aparaseg2Volmgz.inputs.vol_label_file = "./r-aparc_aseg.mgz"
-    workflow.connect(reconAll, "rawavg", aparaseg2Volmgz, "template_file")
-    workflow.connect([(reconAll, aparaseg2Volmgz, [(('aparc_aseg', getn, 0), 'reg_header')])])
-    workflow.connect([(reconAll, aparaseg2Volmgz, [(('aparc_aseg', getn, 0), 'seg_file')])])
-    workflow.connect(reconAll, "subjects_dir", aparaseg2Volmgz, "subjects_dir")
-    workflow.connect(reconAll, "subject_id", aparaseg2Volmgz, "subject_id")
+    workflow.connect(recon_all, "rawavg", aparaseg2Volmgz, "template_file")
+    workflow.connect([(recon_all, aparaseg2Volmgz, [(('aparc_aseg', getn, 0), 'reg_header')])])
+    workflow.connect([(recon_all, aparaseg2Volmgz, [(('aparc_aseg', getn, 0), 'seg_file')])])
+    workflow.connect(recon_all, "subjects_dir", aparaseg2Volmgz, "subjects_dir")
+    workflow.connect(recon_all, "subject_id", aparaseg2Volmgz, "subject_id")
 
     # NODE 3: Aparcaseg conversion mgz -> nifti
     aparaseg2Volnii = Node(CustomLabel2Vol(), name="aparaseg2Volnii")
     aparaseg2Volnii.long_name = "label Nifti conversion"
     aparaseg2Volnii.inputs.vol_label_file = "r-aparc_aseg.nii.gz"
-    workflow.connect(reconAll, "rawavg", aparaseg2Volnii, "template_file")
-    workflow.connect([(reconAll, aparaseg2Volnii, [(('aparc_aseg', getn, 0), 'reg_header')])])
-    workflow.connect([(reconAll, aparaseg2Volnii, [(('aparc_aseg', getn, 0), 'seg_file')])])
+    workflow.connect(recon_all, "rawavg", aparaseg2Volnii, "template_file")
+    workflow.connect([(recon_all, aparaseg2Volnii, [(('aparc_aseg', getn, 0), 'reg_header')])])
+    workflow.connect([(recon_all, aparaseg2Volnii, [(('aparc_aseg', getn, 0), 'seg_file')])])
     workflow.connect(aparaseg2Volnii, "vol_label_file", outputnode, "vol_label_file_nii")
 
     # NODE 4: Left cerebral white matter binary ROI
     lhwmROI = Node(ThrROI(), name='lhwmROI')
     lhwmROI.long_name = "Lh white matter ROI"
     lhwmROI.inputs.seg_val_min = 2
     lhwmROI.inputs.seg_val_max = 2
@@ -143,50 +150,55 @@
     wmROI.long_name = "white matter ROI"
     wmROI.inputs.operation = "add"
     wmROI.inputs.out_file = "wmROI.nii.gz"
     workflow.connect(lhwmROI, "out_file", wmROI, "in_file")
     workflow.connect(rhwmROI, "out_file", wmROI, "operand_file")
 
     # NODE 7: Left basal ganglia and thalamus binary ROI
-    lhbgtROI = Node(ThrROI(), name='lhbgtROI')
-    lhbgtROI.long_name = "Lh BGT ROI"
-    lhbgtROI.inputs.seg_val_min = 10
-    lhbgtROI.inputs.seg_val_max = 13
-    lhbgtROI.inputs.out_file = "lhbgtROI.nii.gz"
-    workflow.connect(aparaseg2Volnii, "vol_label_file", lhbgtROI, "in_file")
+    lhbgROI = Node(ThrROI(), name='lhbgROI')
+    lhbgROI.long_name = "Lh Basal ganglia ROI"
+    lhbgROI.inputs.seg_val_min = 11
+    lhbgROI.inputs.seg_val_max = 13
+    lhbgROI.inputs.out_file = "lhbgROI.nii.gz"
+    workflow.connect(aparaseg2Volnii, "vol_label_file", lhbgROI, "in_file")
 
     # NODE 8: Right basal ganglia and thalamus binary ROI
-    rhbgtROI = Node(ThrROI(), name='rhbgtROI')
-    rhbgtROI.long_name = "Rh BGT ROI"
-    rhbgtROI.inputs.seg_val_min = 49
-    rhbgtROI.inputs.seg_val_max = 52
-    rhbgtROI.inputs.out_file = "rhbgtROI.nii.gz"
-    workflow.connect(aparaseg2Volnii, "vol_label_file", rhbgtROI, "in_file")
+    rhbgROI = Node(ThrROI(), name='rhbgROI')
+    rhbgROI.long_name = "Rh Basal ganglia ROI"
+    rhbgROI.inputs.seg_val_min = 50
+    rhbgROI.inputs.seg_val_max = 52
+    rhbgROI.inputs.out_file = "rhbgROI.nii.gz"
+    workflow.connect(aparaseg2Volnii, "vol_label_file", rhbgROI, "in_file")
 
     # NODE 9: Basal ganglia and thalami binary ROI
-    bgtROI = Node(BinaryMaths(), name='bgtROI')
-    bgtROI.long_name = "BGT ROI"
-    bgtROI.inputs.operation = "add"
-    bgtROI.inputs.out_file = "bgtROI.nii.gz"
-    workflow.connect(lhbgtROI, "out_file", bgtROI, "in_file")
-    workflow.connect(rhbgtROI, "out_file", bgtROI, "operand_file")
+    bgROI = Node(BinaryMaths(), name='bgROI')
+    bgROI.long_name = "Basal ganglia ROI"
+    bgROI.inputs.operation = "add"
+    bgROI.inputs.out_file = "bgROI.nii.gz"
+    workflow.connect(lhbgROI, "out_file", bgROI, "in_file")
+    workflow.connect(rhbgROI, "out_file", bgROI, "operand_file")
 
-    workflow.connect(bgtROI, "out_file", outputnode, "bgtROI")
+    workflow.connect(bgROI, "out_file", outputnode, "bgROI")
     # TODO wmROI work in progress - Not used for now. Maybe useful for SUPERFLAIR
     workflow.connect(wmROI, "out_file", outputnode, "wmROI")
-    workflow.connect(reconAll, "pial", outputnode, "pial")
-    workflow.connect(reconAll, "white", outputnode, "white")
-    workflow.connect(reconAll, "subject_id", outputnode, "subject_id")
-    workflow.connect(reconAll, "subjects_dir", outputnode, "subjects_dir")
+    workflow.connect(recon_all, "pial", outputnode, "pial")
+    workflow.connect(recon_all, "white", outputnode, "white")
+    workflow.connect(recon_all, "subject_id", outputnode, "subject_id")
+    workflow.connect(recon_all, "subjects_dir", outputnode, "subjects_dir")
     workflow.connect(aparaseg2Volmgz, "vol_label_file", outputnode, "vol_label_file")
 
     if is_hippo_amyg_labels:
         # NODE 10: Segmentation of the hippocampal substructures and the nuclei of the amygdala
         segmentHA = Node(SegmentHA(), name="segmentHA")
-        workflow.connect(reconAll, "subjects_dir", segmentHA, "subjects_dir")
-        workflow.connect(reconAll, "subject_id", segmentHA, "subject_id")
-        workflow.connect(inputnode, "max_node_cpu", segmentHA, "num_threads")
-
+        if multicore_node_limit == CORE_LIMIT.NO_LIMIT:
+            segmentHA.inputs.num_cpu = cpu_count()
+        elif multicore_node_limit == CORE_LIMIT.SOFT_CAP:
+            segmentHA.inputs.num_cpu = max_cpu
+        else:
+            segmentHA.inputs.num_cpu = max_cpu
+            segmentHA.n_procs = segmentHA.inputs.num_cpu
+        workflow.connect(recon_all, "subjects_dir", segmentHA, "subjects_dir")
+        workflow.connect(recon_all, "subject_id", segmentHA, "subject_id")
         workflow.connect(segmentHA, "lh_hippoAmygLabels", outputnode, "lh_hippoAmygLabels")
         workflow.connect(segmentHA, "rh_hippoAmygLabels", outputnode, "rh_hippoAmygLabels")
 
     return workflow
```

### Comparing `swane-0.0.6/swane/nipype_pipeline/workflows/func_map_workflow.py` & `swane-0.1.0/swane/nipype_pipeline/workflows/func_map_workflow.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,54 +1,52 @@
 from nipype.interfaces.freesurfer import SampleToSurface
-from nipype.interfaces.fsl import (FLIRT, IsotropicSmooth, ApplyWarp, ApplyMask, SwapDimensions, ApplyXFM)
+from nipype.interfaces.fsl import (FLIRT, IsotropicSmooth, ApplyWarp, ApplyMask, SwapDimensions, ApplyXFM, ImageMaths)
 from nipype.pipeline.engine import Node
 from swane.nipype_pipeline.workflows.tractography_workflow import SIDES
-
 from swane.nipype_pipeline.engine.CustomWorkflow import CustomWorkflow
 from swane.nipype_pipeline.nodes.CustomDcm2niix import CustomDcm2niix
 from swane.nipype_pipeline.nodes.ForceOrient import ForceOrient
 from swane.nipype_pipeline.nodes.AsymmetryIndex import AsymmetryIndex
 from swane.nipype_pipeline.nodes.Zscore import Zscore
-
 from nipype.interfaces.utility import IdentityInterface
-
+from configparser import SectionProxy
 import swane_supplement
 
 
-def func_map_workflow(name: str, dicom_dir: str, is_freesurfer: bool, is_ai: bool, base_dir: str = "/") -> CustomWorkflow:
+def func_map_workflow(name: str, dicom_dir: str, is_freesurfer: bool, config: SectionProxy, base_dir: str = "/") -> CustomWorkflow:
     """
     Analysis for PET or ASL:
         - registration to reference;
         - z-score and asymmetry index maps;
         - projection on FreeSurfer pial surface.
 
     Parameters
     ----------
     name : str
         The workflow name.
     dicom_dir : path
         The file path of the DICOM files.
     is_freesurfer : bool
         True if the reconall is available.
-    is_ai : bool
-        Enables the asymmetry index map calculation.
+    config: SectionProxy
+        workflow settings.
     base_dir : path, optional
         The base directory path relative to parent workflow. The default is "/".
         
     Input Node Fields
     ----------
     reference : path
         The reference image for the registration.
     brain_mask : path
         The brain mask from T13D bet command.
     freesurfer_subjects_dir : path
         The directory from FreeSurfer analysis.
     freesurfer_subject_id : 
         The subject id from FreeSurfer analysis.
-    bgtROI : path
+    bgROI : path
         Basal ganglia and thalami ROI.
     ref_2_sym_warp : path
         Nonlinear registration warp from T13D to symmetric atlas.
     ref_2_sym_invwarp : path
         Nonlinear registration inverse warp from symmetric atlas to T13D.
 
     Returns
@@ -61,15 +59,15 @@
     registered_file : string
         Functional map in T13D reference space.
     surf_lh : path
         If FreeSurfer is available, functional map projection on LH pial surface.
     surf_rh : path
         If FreeSurfer is available, functional map projection on RH pial surface.
     zscore : path
-        If FreeSurfer is available, internal z-score statistics compared to bgt.
+        If FreeSurfer is available, internal z-score statistics compared to basal ganglia.
     zscore_surf_lh : list of strings
         If FreeSurfer is available, z-score projection on LH pial surface.
     zscore_surf_rh : list of strings
         If FreeSurfer is available, z-score projection on RH pial surface.
     ai : path
         If AI is enabled, asymmetry index map.
     ai_surf_lh : path
@@ -79,17 +77,16 @@
 
     """
     
     workflow = CustomWorkflow(name=name, base_dir=base_dir)
     
     # Input Node
     inputnode = Node(
-        IdentityInterface(fields=['reference', 'brain_mask', 'freesurfer_subjects_dir',
-                                  'freesurfer_subject_id', 'bgtROI', 'ref_2_sym_warp',
-                                  'swap_2_sym_warp', 'ref_2_sym_invwarp']),
+        IdentityInterface(fields=['reference', 'brain_mask', 'freesurfer_subjects_dir', 'freesurfer_subject_id',
+                                  'bgROI', 'ref_2_sym_warp', 'ref_2_sym_invwarp']),
         name='inputnode')
     
     # Output Node
     outputnode = Node(
         IdentityInterface(fields=['registered_file', 'surf_lh', 'surf_rh', 'zscore', 'zscore_surf_lh',
                                   'zscore_surf_rh', 'ai', 'ai_surf_lh', 'ai_surf_rh']),
         name='outputnode')
@@ -159,15 +156,15 @@
             workflow.connect(func_surf, "out_file", outputnode, "surf_%s" % side)
 
         # NODE 8: z-score calculation
         zscore = Node(Zscore(), name="%s_zscore" % name)
         zscore.long_name = "internal zscore"
         zscore.inputs.out_file = "r-%s_zscore.nii.gz" % name
         workflow.connect(mask, "out_file", zscore, "in_file")
-        workflow.connect(inputnode, "bgtROI", zscore, "ROI_file")
+        workflow.connect(inputnode, "bgROI", zscore, "ROI_file")
 
         workflow.connect(zscore, "out_file", outputnode, "zscore")
 
         # NODE 10: Projection of z-score on FreeSurfer pial surface
         for side in SIDES:
             zscore_surf_lh = Node(SampleToSurface(), name='%s_zscore_surf_%s' % (name, side))
             zscore_surf_lh.long_name = side + " zscore %s"
@@ -180,22 +177,24 @@
             zscore_surf_lh.inputs.sampling_units = "frac"
             workflow.connect(zscore, "out_file", zscore_surf_lh, "source_file")
             workflow.connect(inputnode, "freesurfer_subjects_dir", zscore_surf_lh, "subjects_dir")
             workflow.connect(inputnode, "freesurfer_subject_id", zscore_surf_lh, "subject_id")
 
             workflow.connect(zscore_surf_lh, "out_file", outputnode, "zscore_surf_%s" % side)
 
+    is_ai = config.getboolean_safe("ai")
+
     if is_ai:
         sym_template = swane_supplement.sym_template
 
         # NODE 11: Nonlinear transformation of the images in symmetric atlas
         func_2_sym_warp = Node(ApplyWarp(), name='%s_2_sym_warp' % name)
         func_2_sym_warp.long_name = "%s to symmetric atlas"
         func_2_sym_warp.inputs.ref_file = sym_template
-        workflow.connect(mask, "out_file", func_2_sym_warp, "in_file")
+        workflow.connect(smooth_2_ref_flirt, "out_file", func_2_sym_warp, "in_file")
         workflow.connect(inputnode, "ref_2_sym_warp", func_2_sym_warp, "field_file")
 
         # NODE 12: RL swap of image in symmetric atlas
         sym_swap = Node(SwapDimensions(), name='%s_sym_swap' % name)
         sym_swap.long_name = "right-left flip"
         sym_swap.inputs.out_file = "%s_sym_swapped.nii.gz" % name
         sym_swap.inputs.new_dims = ("-x", "y", "z")
@@ -204,36 +203,50 @@
         # NODE 13: Asymmetry index calculation
         ai = Node(AsymmetryIndex(), name="%s_ai" % name)
         ai.long_name = "asymmetry index"
         ai.inputs.out_file = "r-%s_ai.nii.gz" % name
         workflow.connect(func_2_sym_warp, "out_file", ai, "in_file")
         workflow.connect(sym_swap, "out_file", ai, "swapped_file")
 
-        # NODE 14: AI Nonlinear transformation to reference space
+        # NODE 14: AI thresholding
+        ai_threshold = Node(ImageMaths(), name='%s_ai_threshold' % name)
+        threshold = config.getint_safe("ai_threshold")
+        threshold = abs(threshold/100)
+        ai_threshold.inputs.op_string = "-thr %f -uthr %f" % (-threshold, threshold)
+        workflow.connect(ai, "out_file", ai_threshold, "in_file")
+
+        # NODE 15: AI Nonlinear transformation to reference space
         ai_2_ref = Node(ApplyWarp(), name="%s_ai_2_ref" % name)
         ai_2_ref.long_name = "asymmetry index %s from symmetric atlas"
         ai_2_ref.inputs.out_file = "r-%s_ai.nii.gz" % name
-        workflow.connect(ai, "out_file", ai_2_ref, "in_file")
+        workflow.connect(ai_threshold, "out_file", ai_2_ref, "in_file")
         workflow.connect(inputnode, "ref_2_sym_invwarp", ai_2_ref, "field_file")
         workflow.connect(inputnode, "reference", ai_2_ref, "ref_file")
 
-        workflow.connect(ai_2_ref, "out_file", outputnode, "ai")
+        # NODE 16: AI scalp removal
+        ai_mask = Node(ApplyMask(), name='%s_ai_mask' % name)
+        ai_mask.long_name = name + " AI %s"
+        ai_mask.inputs.out_file = "r-%s_ai.nii.gz" % name
+        workflow.connect(ai_2_ref, "out_file", ai_mask, "in_file")
+        workflow.connect(inputnode, "brain_mask", ai_mask, "mask_file")
+
+        workflow.connect(ai_mask, "out_file", outputnode, "ai")
 
         if is_freesurfer:
             for side in SIDES:
-                # NODE 15: Projection of AI on FreeSurfer pial surface
+                # NODE 17: Projection of AI on FreeSurfer pial surface
                 ai_surf = Node(SampleToSurface(), name='%s_ai_surf_%s' % (name, side))
                 ai_surf.long_name = side + " asymmetry index %s"
                 ai_surf.inputs.hemi = side
                 ai_surf.inputs.out_file = "%s_ai_surf_%s.mgz" % (name, side)
                 ai_surf.inputs.cortex_mask = True
                 ai_surf.inputs.reg_header = True
                 ai_surf.inputs.sampling_method = "point"
                 ai_surf.inputs.sampling_range = 0.5
                 ai_surf.inputs.sampling_units = "frac"
-                workflow.connect(ai_2_ref, "out_file", ai_surf, "source_file")
+                workflow.connect(ai_mask, "out_file", ai_surf, "source_file")
                 workflow.connect(inputnode, "freesurfer_subjects_dir", ai_surf, "subjects_dir")
                 workflow.connect(inputnode, "freesurfer_subject_id", ai_surf, "subject_id")
 
                 workflow.connect(ai_surf, "out_file", outputnode, "ai_surf_%s" % side)
 
     return workflow
```

### Comparing `swane-0.0.6/swane/nipype_pipeline/workflows/linear_reg_workflow.py` & `swane-0.1.0/swane/nipype_pipeline/workflows/linear_reg_workflow.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from nipype.interfaces.fsl import (BET, FLIRT)
-
 from swane.nipype_pipeline.engine.CustomWorkflow import CustomWorkflow
 from swane.nipype_pipeline.nodes.CustomDcm2niix import CustomDcm2niix
 from swane.nipype_pipeline.nodes.ForceOrient import ForceOrient
-
+from swane.utils.DataInputList import DataInputList
 from nipype import Node
 from nipype.interfaces.utility import IdentityInterface
+from configparser import SectionProxy
 
 
-def linear_reg_workflow(name: str, dicom_dir: str, base_dir: str = "/", is_volumetric: bool = True) -> CustomWorkflow:
+def linear_reg_workflow(name: str, dicom_dir: str, config: SectionProxy, base_dir: str = "/", is_volumetric: bool = True) -> CustomWorkflow:
     """
     Transforms input images in a reference space through a linear registration.
 
     Parameters
     ----------
     name : str
         The workflow name.
     dicom_dir : path
         The file path of the DICOM files.
+    config: SectionProxy
+        workflow settings.
     base_dir : path, optional
         The base directory path relative to parent workflow. The default is "/".
     is_volumetric : bool, optional
         True if input is 3D. The default is True.
 
     Input Node Fields
     ----------
     reference : path
         The reference image for the registration.
-    frac : float
-        Fractional intensity threshold for bet command.
     output_name : str
         The name for registered file.
     crop : bool
         If True, enables 3D images (neck removal).
 
     Returns
     -------
@@ -48,40 +48,43 @@
 
     """
     
     workflow = CustomWorkflow(name=name, base_dir=base_dir)
 
     # Input Node
     inputnode = Node(
-        IdentityInterface(fields=['reference', 'frac', 'output_name', 'crop']),
+        IdentityInterface(fields=['reference', 'output_name', 'crop']),
         name='inputnode')
     
     # Output Node
     outputnode = Node(
         IdentityInterface(fields=['registered_file', 'out_matrix_file']),
         name='outputnode')
 
-
     # NODE 1: Conversion dicom -> nifti
     conversion = Node(CustomDcm2niix(), name='%s_conv' % name)
     conversion.inputs.source_dir = dicom_dir
     conversion.inputs.bids_format = False
     conversion.inputs.out_filename = name
     workflow.connect(inputnode, 'crop', conversion, 'crop')
 
     # NODE 2: Orienting in radiological convention
     reorient = Node(ForceOrient(), name='%s_reorient' % name)
     workflow.connect(conversion, "converted_files", reorient, "in_file")
 
     # NODE 3: Scalp removal
     bet = Node(BET(), '%s_BET' % name)
-    bet.inputs.robust = True
-    bet.inputs.threshold = True
+    if config is not None:
+        bet.inputs.frac = config.getfloat_safe('bet_thr')
+    if config is not None and config.getboolean_safe('bet_bias_correction'):
+        bet.inputs.reduce_bias = True
+    else:
+        bet.inputs.robust = True
+    bet.inputs.mask = True
     workflow.connect(reorient, "out_file", bet, "in_file")
-    workflow.connect(inputnode, "frac", bet, "frac")
 
     # NODE 4: Linear registration to reference space
     flirt_2_ref = Node(FLIRT(), name='%s_2_ref' % name)
     flirt_2_ref.long_name = "%s to reference space"
     flirt_2_ref.inputs.out_matrix_file = "%s_2_ref.mat" % name
 
     if is_volumetric:
```

### Comparing `swane-0.0.6/swane/nipype_pipeline/workflows/nonlinear_reg_workflow.py` & `swane-0.1.0/swane/nipype_pipeline/workflows/nonlinear_reg_workflow.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.6/swane/nipype_pipeline/workflows/ref_workflow.py` & `swane-0.1.0/swane/nipype_pipeline/workflows/ref_workflow.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 from swane.nipype_pipeline.engine.CustomWorkflow import CustomWorkflow
 from swane.nipype_pipeline.nodes.CustomDcm2niix import CustomDcm2niix
 from swane.nipype_pipeline.nodes.ForceOrient import ForceOrient
-
+from swane.nipype_pipeline.nodes.CropFov import CropFov
+from configparser import SectionProxy
+from swane.utils.DataInputList import DataInputList
 from nipype.interfaces.fsl import BET
 from nipype.interfaces.utility import IdentityInterface
 
 from nipype import Node
 
-def ref_workflow(name: str, dicom_dir: str, base_dir: str = "/") -> CustomWorkflow:
+
+def ref_workflow(name: str, dicom_dir: str, config: SectionProxy, base_dir: str = "/") -> CustomWorkflow:
     """
     T13D workflow to use as reference.
 
     Parameters
     ----------
     name : str
         The workflow name.
     dicom_dir : path
         The file path of the DICOM files.
+    config: SectionProxy
+        workflow settings.
     base_dir : path, optional
         The base directory path relative to parent workflow. The default is "/".
 
     Input Node Fields
     ----------
     -
 
@@ -35,39 +40,49 @@
         T13D.
     ref_brain : path
         Betted T13D.
     ref_mask : path
         Brain mask from T13D bet command.
 
     """
-    
+
     workflow = CustomWorkflow(name=name, base_dir=base_dir)
     
     # Output Node
     outputnode = Node(
         IdentityInterface(fields=['ref', 'ref_brain', 'ref_mask']),
         name='outputnode')
 
     # NODE 1: Conversion dicom -> nifti
     ref_conv = Node(CustomDcm2niix(), name='%s_conv' % name)
     ref_conv.inputs.source_dir = dicom_dir
     ref_conv.inputs.crop = True
     ref_conv.inputs.bids_format = False
-    ref_conv.inputs.out_filename = "ref"
+    ref_conv.inputs.out_filename = "converted"
 
     # NODE 2: Orienting in radiological convention
     ref_reOrient = Node(ForceOrient(), name='%s_reOrient' % name)
     workflow.connect(ref_conv, "converted_files", ref_reOrient, "in_file")
 
-    # NODE 3: Scalp removal
-    ref_BET = Node(BET(), name='ref_BET')
-    ref_BET.inputs.frac = 0.5
+    # NODE 3: Crop FOV larger than 256mm for subsequent freesurfer
+    ref_reScale = Node(CropFov(), name='%s_reScale' % name)
+    ref_reScale.long_name = "Crop large FOV"
+    ref_reScale.inputs.max_dim = 256
+    ref_reScale.inputs.out_file = "ref.nii.gz"
+    workflow.connect(ref_reOrient, "out_file", ref_reScale, "in_file")
+
+    # NODE 4: Scalp removal
+    ref_BET = Node(BET(), name='%s_BET' % name)
     ref_BET.inputs.mask = True
-    ref_BET.inputs.robust = True
-    ref_BET.inputs.threshold = True
-    workflow.connect(ref_reOrient, "out_file", ref_BET, "in_file")
+    ref_BET.inputs.frac = config.getfloat_safe('bet_thr')
+    if config.getboolean_safe('bet_bias_correction'):
+        ref_BET.inputs.reduce_bias = True
+    else:
+        ref_BET.inputs.robust = True
+
+    workflow.connect(ref_reScale, "out_file", ref_BET, "in_file")
     
-    workflow.connect(ref_reOrient, "out_file", outputnode, "ref")
+    workflow.connect(ref_reScale, "out_file", outputnode, "ref")
     workflow.connect(ref_BET, "out_file", outputnode, "ref_brain")
     workflow.connect(ref_BET, "mask_file", outputnode, "ref_mask")
 
     return workflow
```

### Comparing `swane-0.0.6/swane/nipype_pipeline/workflows/task_fMRI_workflow.py` & `swane-0.1.0/swane/nipype_pipeline/workflows/task_fMRI_workflow.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,91 +1,76 @@
 from nipype import Node, IdentityInterface, Merge, SelectFiles
 from nipype.algorithms.modelgen import SpecifyModel
 from nipype.algorithms.rapidart import ArtifactDetect
-from nipype.interfaces.fsl import ImageMaths, ExtractROI, MCFLIRT, BET, ImageStats, SUSAN, FLIRT, Level1Design, \
-    FEATModel, FILMGLS, SmoothEstimate
-
+from nipype.interfaces.fsl import (ImageMaths, ExtractROI, MCFLIRT, BET, ImageStats, SUSAN, FLIRT, Level1Design,
+                                   FEATModel, FILMGLS, SmoothEstimate, Cluster, ApplyXFM)
+from configparser import SectionProxy
 from swane.nipype_pipeline.engine.CustomWorkflow import CustomWorkflow
 from swane.nipype_pipeline.nodes.CustomDcm2niix import CustomDcm2niix
 from swane.nipype_pipeline.nodes.FslNVols import FslNVols
-from swane.nipype_pipeline.nodes.FslCluster import FslCluster
 from swane.nipype_pipeline.nodes.FMRIGenSpec import FMRIGenSpec
 from swane.nipype_pipeline.nodes.CustomSliceTimer import CustomSliceTimer
 from swane.nipype_pipeline.nodes.GetNiftiTR import GetNiftiTR
 from swane.nipype_pipeline.nodes.ForceOrient import ForceOrient
 from swane.nipype_pipeline.nodes.DeleteVolumes import DeleteVolumes
+from swane.config.config_enums import BLOCK_DESIGN
 
 
-def task_fMRI_workflow(name: str, dicom_dir: str, design_block: int, base_dir: str = "/") -> CustomWorkflow:
+def task_fMRI_workflow(name: str, dicom_dir: str, config: SectionProxy, base_dir: str = "/") -> CustomWorkflow:
     """
     fMRI first level anlysis for a single task with constant task-rest paradigm.
 
     Parameters
     ----------
     name : str
         The workflow name.
     dicom_dir : path
         The directory path of the DICOM files.
-    design_block : int
-        Task design block:
-            0: rArA...
-            1: rArBrArB...
+    config: SectionProxy
+        workflow settings.
     base_dir : path, optional
         The base directory path relative to parent workflow. The default is "/".
 
     Input Node Fields
     ----------
-    task_a_name : str
-        The name of the task A.
-    task_b_name : str
-        The name of the task B.
-    nvols : int
-        If == -1, automatic detection of EPI volume number, otherwise force to specified number.
-    TR : float
-        If == -1, automatic detection of Repetition Time, otherwise force to specified number.
-    slice_timing : int
-        Slice order for timing correction:
-            0, Unknown, correction disabled
-            1, Regular up
-            2, Regular down
-            3, intervealed
-    task_duration : int
-        Duration of task in seconds.
     ref_BET : path
         Betted T13D.
-    rest_duration : int
-        Duration of rest in second.
-    del_start_vols : int
-        Volumes to delete from start of sequence.
-    del_end_vols : int
-        Volumes to delete from end of sequence.
 
-    Returns
-    -------
-    workflow : CustomWorkflow
-        The fMRI workflow.
-        
     Output Node Fields
     ----------
     threshold_file_1 : path
         Cluster of activation (task A vs rest or Task A vs Task B) in T13D reference space.
     threshold_file_2 : path
         Cluster of activation (task b vs Task) in T13D reference space.
 
+    Returns
+    -------
+    workflow : CustomWorkflow
+        The fMRI workflow.
+
     """
-    
-    #TODO rinominare in workflow
+
     workflow = CustomWorkflow(name=name, base_dir=base_dir)
     
     # Input Node
     inputnode = Node(
         IdentityInterface(
-            fields=['task_a_name', 'task_b_name', 'nvols', 'TR', 'slice_timing', 'task_duration', 'ref_BET',
-                    'rest_duration', 'del_start_vols', 'del_end_vols']),
+            fields=['ref_BET']),
         name='inputnode')
+
+    task_a_name = config["task_a_name"]
+    task_b_name = config["task_b_name"]
+    task_duration = config.getint_safe('task_duration')
+    rest_duration = config.getint_safe('rest_duration')
+    TR = config.getfloat_safe('tr')
+    slice_timing = config.getenum_safe('slice_timing')
+    n_vols = config.getint_safe('n_vols')
+    del_start_vols = config.getint_safe('del_start_vols')
+    del_end_vols = config.getint_safe('del_end_vols')
+    block_design = config.getenum_safe('block_design')
     
     # Output Node
     outputnode = Node(
         IdentityInterface(fields=['threshold_file_1', 'threshold_file_2']),
         name='outputnode')
 
     # NODE 1: Conversion dicom -> nifti
@@ -93,30 +78,30 @@
     conv.inputs.out_filename = name
     conv.inputs.bids_format = False
     conv.inputs.source_dir = dicom_dir
 
     # NODE 2: Get EPI volume numbers
     nvols = Node(FslNVols(), name="%s_nvols" % name)
     nvols.long_name = "EPI volumes count"
-    workflow.connect(inputnode, 'nvols', nvols, 'force_value')
+    nvols.inputs.force_value = n_vols
     workflow.connect(conv, 'converted_files', nvols, 'in_file')
 
     # NODE 3: Get Repetition Time
     getTR = Node(GetNiftiTR(), name="%s_getTR" % name)
     getTR.long_name = "get TR"
-    workflow.connect(inputnode, 'TR', getTR, 'force_value')
+    getTR.inputs.force_value = TR
     workflow.connect(conv, 'converted_files', getTR, 'in_file')
 
     # NODE 4: Delete specified volumes at start and end of sequence
     del_vols = Node(DeleteVolumes(), name="%s_del_vols" % name)
     del_vols.long_name = "Extreme volumes deletion"
+    del_vols.inputs.del_start_vols = del_start_vols
+    del_vols.inputs.del_end_vols = del_end_vols
     workflow.connect(conv, 'converted_files', del_vols, "in_file")
     workflow.connect(nvols, 'nvols', del_vols, "nvols")
-    workflow.connect(inputnode, 'del_start_vols', del_vols, "del_start_vols")
-    workflow.connect(inputnode, 'del_end_vols', del_vols, "del_end_vols")
 
     # NODE 5: Orienting in radiological convention
     reorient = Node(ForceOrient(), name='%s_reorient' % name)
     workflow.connect(del_vols, "out_file", reorient, "in_file")
 
     # NODE 5: Convert functional images to float representation.
     img2float = Node(ImageMaths(), name="%s_img2float" % name)
@@ -151,17 +136,17 @@
     motion_correct.inputs.save_rms = True
     motion_correct.inputs.interpolation = 'spline'
     workflow.connect(img2float, 'out_file', motion_correct, 'in_file')
     workflow.connect(extract_ref, 'roi_file', motion_correct, 'ref_file')
 
     # NODE 8: Perform slice timing correction if needed
     slice_timing_correction = Node(CustomSliceTimer(), name="%s_timing_correction" % name)
+    slice_timing_correction.inputs.slice_timing = slice_timing
     workflow.connect(getTR, 'TR', slice_timing_correction, 'time_repetition')
     workflow.connect(motion_correct, 'out_file', slice_timing_correction, 'in_file')
-    workflow.connect(inputnode, 'slice_timing', slice_timing_correction, 'slice_timing')
 
     # NODE 9: Extract the mean volume of the first functional run
     meanfunc = Node(ImageMaths(), name="%s_meanfunc" % name)
     meanfunc.long_name = "mean image calculation"
     meanfunc.inputs.op_string = '-Tmean'
     meanfunc.inputs.suffix = '_mean'
     workflow.connect(slice_timing_correction, 'slice_time_corrected_file', meanfunc, 'in_file')
@@ -282,19 +267,19 @@
     meanfunc3.long_name = "mean image calculation"
     meanfunc3.inputs.op_string = '-Tmean'
     meanfunc3.inputs.suffix = '_mean'
     workflow.connect(intnorm, 'out_file', meanfunc3, 'in_file')
 
     # NODE 25: Generate the Bunch containing fMRI specifications
     genSpec = Node(FMRIGenSpec(), name="%s_genSpec" % name)
-    genSpec.inputs.design_block = design_block
-    workflow.connect(inputnode, 'task_duration', genSpec, 'task_duration')
-    workflow.connect(inputnode, 'rest_duration', genSpec, 'rest_duration')
-    workflow.connect(inputnode, 'task_a_name', genSpec, 'task_a_name')
-    workflow.connect(inputnode, 'task_b_name', genSpec, 'task_b_name')
+    genSpec.inputs.block_design = block_design
+    genSpec.inputs.task_duration = task_duration
+    genSpec.inputs.rest_duration = rest_duration
+    genSpec.inputs.task_a_name = task_a_name
+    genSpec.inputs.task_b_name = task_b_name
     workflow.connect(getTR, "TR", genSpec, "TR")
     workflow.connect(del_vols, "nvols", genSpec, "nvols")
     workflow.connect(meanfunc3, "out_file", genSpec, "tempMean")
 
     # NODE 26: Perform temporal highpass filtering on the data
     highpass = Node(ImageMaths(), name="%s_highpass" % name)
     highpass.long_name = "Highpass temporal filtering"
@@ -372,37 +357,37 @@
             with open(dofFile, 'r') as file:
                 for line in file.readlines():
                     return int(line)
 
     workflow.connect(modelestimate, ('dof_file', dof_from_file), smoothness, 'dof')
     workflow.connect(dilatemask, 'out_file', smoothness, 'mask_file')
 
-    n_contrasts = 1 + design_block
+    n_contrasts = 1
+    if block_design == BLOCK_DESIGN.RARB:
+        n_contrasts += 1
     cont = 0
     while cont < n_contrasts:
         cont += 1
 
         # NODE 34: Select all result file from filmgls output folder
-        results_select = Node(SelectFiles({'cope': 'cope%d.nii.gz' % cont,
-                                                'zstat': 'zstat%d.nii.gz' % cont}),
-                                   name="%s_results_select_%d" % (name, cont))
+        results_select = Node(SelectFiles({'cope': 'cope%d.nii.gz' % cont, 'zstat': 'zstat%d.nii.gz' % cont}),
+                              name="%s_results_select_%d" % (name, cont))
         results_select.long_name = "contrast %d result selection" % cont
         workflow.connect(modelestimate, 'results_dir', results_select, 'base_directory')
 
-
         # NODE 35: Mask z-stat with the dilated mask
         maskfunc4 = Node(ImageMaths(), name="%s_maskfunc4_%d" % (name, cont))
         maskfunc4.long_name = "Zstat masking"
         maskfunc4.inputs.suffix = '_mask'
         maskfunc4.inputs.op_string = '-mas'
         workflow.connect(results_select, 'zstat', maskfunc4, 'in_file')
         workflow.connect(dilatemask, 'out_file', maskfunc4, 'in_file2')
 
         # NODE 36: Perform clustering on statistical output
-        cluster = Node(FslCluster(), name="%s_cluster_%d" % (name, cont))
+        cluster = Node(Cluster(), name="%s_cluster_%d" % (name, cont))
         cluster.long_name = "contrast " + str(cont) + " %s"
         cluster.inputs.threshold = 3.1
         cluster.inputs.connectivity = 26
         cluster.inputs.pthreshold = 0.05
         cluster.inputs.out_localmax_txt_file = True
 
         # Function to generate the name for the file of output cluster
@@ -410,13 +395,21 @@
             return "r-%s_cluster_%s.nii.gz" % (run_name, contrasts[x-1][0])
 
         workflow.connect([(genSpec, cluster, [(('contrasts', cluster_file_name, name, cont), 'out_threshold_file')])])
         workflow.connect(maskfunc4, 'out_file', cluster, 'in_file')
         workflow.connect(results_select, 'cope', cluster, 'cope_file')
         workflow.connect(smoothness, 'volume', cluster, 'volume')
         workflow.connect(smoothness, 'dlh', cluster, 'dlh')
-        workflow.connect(inputnode, "ref_BET", cluster, "std_space_file")
-        workflow.connect(flirt_2_ref, "out_matrix_file", cluster, "xfm_file")
 
-        workflow.connect(cluster, 'threshold_file', outputnode, 'threshold_file_%s' % cont)
+        # NODE 37: Transformation in ref space
+        cluster_2_ref = Node(ApplyXFM(), name="%s_cluster_%d_to_ref" % (name, cont))
+        cluster_2_ref.long_name = "contrast " + str(cont) + " %s in reference space"
+        cluster_2_ref.inputs.apply_xfm = True
+        workflow.connect(cluster, 'threshold_file', cluster_2_ref, 'in_file')
+        workflow.connect([(genSpec, cluster_2_ref, [(('contrasts', cluster_file_name, name, cont), 'out_file')])])
+        workflow.connect(inputnode, "ref_BET", cluster_2_ref, "reference")
+        workflow.connect(flirt_2_ref, "out_matrix_file", cluster_2_ref, "in_matrix_file")
+
+        # workflow.connect(cluster, 'threshold_file', outputnode, 'threshold_file_%s' % cont)
+        workflow.connect(cluster_2_ref, 'out_file', outputnode, 'threshold_file_%s' % cont)
 
     return workflow
```

### Comparing `swane-0.0.6/swane/nipype_pipeline/workflows/tractography_workflow.py` & `swane-0.1.0/swane/nipype_pipeline/workflows/tractography_workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 import os
 import glob
-
-from nipype import Node, IdentityInterface, MapNode, JoinNode, Merge, Rename
+from nipype import Node, IdentityInterface, MapNode, JoinNode, Merge
 from nipype.interfaces.fsl import ApplyWarp, ImageMaths
-
+from configparser import SectionProxy
 from swane.nipype_pipeline.engine.CustomWorkflow import CustomWorkflow
 from swane.nipype_pipeline.nodes.RandomSeedGenerator import RandomSeedGenerator
 from swane.nipype_pipeline.nodes.CustomProbTrackX2 import CustomProbTrackX2
 from swane.nipype_pipeline.nodes.MergeTargets import MergeTargets
 from swane.nipype_pipeline.nodes.SumMultiTracks import SumMultiTracks
-from swane.utils.ConfigManager import ConfigManager
+from swane.config.preference_list import TRACTS, DEFAULT_N_SAMPLES, XTRACT_DATA_DIR
 
 SIDES = ["lh", "rh"]
 
 
-def tractography_workflow(name: str, threads: int, base_dir: str = "/") -> CustomWorkflow:
+def tractography_workflow(name: str, config: SectionProxy, base_dir: str = "/") -> CustomWorkflow:
     """
     Executes tractography for chosen tract using xtract protocols.
 
     Parameters
     ----------
     name : str
         The workflow and tract name.
-    threads : int
-        The number of parallel threads to use for the analysis.
+    config: SectionProxy
+        The subject workflow preferences.
     base_dir : path, optional
         The base directory path relative to parent workflow. The default is "/".
 
     Input Node Fields
     ----------
+    mask: path
+        The ref brain mask.
     fsamples : path
         Samples from the distribution of anysotropic volume fraction.
     phsamples : path
         Samples from the distribution on phi.
     thsamples : path
         Samples from the distribution on theta.
     ref_brain : path
@@ -63,46 +64,53 @@
         Text file containing a single number corresponding to the total number
         of generated tracts that have not been rejected by inclusion/exclusion
         mask criteria for LH side.
 
     """
 
     # Check if tract is in configuration list
-    if name not in ConfigManager.TRACTS:
+    if name not in TRACTS:
         return None
 
     # Check for existance of xtract data directory and protocol name dicrectory
-    if not os.path.exists(os.path.join(ConfigManager.XTRACT_DATA_DIR, name + "_l")):
+    if not os.path.exists(os.path.join(XTRACT_DATA_DIR, name + "_l")):
         return None
 
     workflow = CustomWorkflow(name='tract_' + name, base_dir=base_dir)
     
     inputnode = Node(
         IdentityInterface(fields=['fsamples', 'mask', 'phsamples', 'thsamples', 'ref_brain',
                                   'diff2ref_mat', "ref2diff_mat", "mni2ref_warp",
                                   ]),
         name='inputnode')
 
     outputnode = Node(
         IdentityInterface(fields=['fdt_paths_rh', 'fdt_paths_lh', 'waytotal_rh', 'waytotal_lh']),
         name='outputnode')
 
+    is_cuda = config.getboolean_safe('cuda')
+    if is_cuda:
+        # if cuda is enabled only 1 process is launched
+        track_threads = 1
+    else:
+        track_threads = config.getint_safe('track_procs')
+
     # NODE 1: Random seed genration for cache preservation
     random_seed = Node(RandomSeedGenerator(), name='random_seed')
-    random_seed.inputs.seeds_n = threads
+    random_seed.inputs.seeds_n = track_threads
     workflow.connect(inputnode, "mask", random_seed, "mask")
 
     try:
-        n_samples = int(ConfigManager.TRACTS[name][2] / threads)
+        n_samples = int(TRACTS[name][2] / track_threads)
     except:
-        n_samples = int(ConfigManager.DEFAULT_N_SAMPLES / threads)
+        n_samples = int(DEFAULT_N_SAMPLES / track_threads)
 
     for side in SIDES:
         # Xtract protocol loading
-        protocol_dir = os.path.join(ConfigManager.XTRACT_DATA_DIR, name + "_" + side[0])
+        protocol_dir = os.path.join(XTRACT_DATA_DIR, name + "_" + side[0])
 
         seed_file = os.path.join(protocol_dir, "seed.nii.gz")
         exclude_file = os.path.join(protocol_dir, "exclude.nii.gz")
         stop_file = os.path.join(protocol_dir, "stop.nii.gz")
         target_files = glob.glob(os.path.join(protocol_dir, "target*"))
 
         invert_file = os.path.join(protocol_dir, "invert")
@@ -159,14 +167,15 @@
         probtrackx = MapNode(CustomProbTrackX2(), name="probtrackx_%s_%s" % (name, side), iterfield=["rseed"])
         probtrackx.long_name = side + " %s"
         probtrackx.inputs.n_samples = n_samples
         probtrackx.inputs.loop_check = True
         probtrackx.inputs.wayorder = is_wayorder
         probtrackx.inputs.rand_fib = 1
         probtrackx.inputs.sample_random_points = 1
+        probtrackx.inputs.use_gpu = is_cuda
         # TODO argomento --ompl che fa??
         probtrackx.inputs.opd = True
         workflow.connect(inputnode, "fsamples", probtrackx, "fsamples")
         workflow.connect(inputnode, "mask", probtrackx, "mask")
         workflow.connect(inputnode, "ref_brain", probtrackx, "seed_ref")
         workflow.connect(inputnode, "phsamples", probtrackx, "phsamples")
         workflow.connect(inputnode, "thsamples", probtrackx, "thsamples")
@@ -194,14 +203,15 @@
             probtrackx_inverted.long_name = side + " inverse %s"
             probtrackx_inverted.inputs.n_samples = n_samples
             probtrackx_inverted.inputs.loop_check = True
             probtrackx_inverted.inputs.wayorder = is_wayorder
             probtrackx_inverted.inputs.rand_fib = 1
             probtrackx_inverted.inputs.sample_random_points = 1
             probtrackx_inverted.inputs.opd = True
+            probtrackx_inverted.inputs.use_gpu = is_cuda
             workflow.connect(inputnode, "fsamples", probtrackx_inverted, "fsamples")
             workflow.connect(inputnode, "mask", probtrackx_inverted, "mask")
             workflow.connect(inputnode, "ref_brain", probtrackx_inverted, "seed_ref")
             workflow.connect(inputnode, "phsamples", probtrackx_inverted, "phsamples")
             workflow.connect(inputnode, "thsamples", probtrackx_inverted, "thsamples")
             workflow.connect(inputnode, "ref2diff_mat", probtrackx_inverted, "xfm")
             workflow.connect(inputnode, "diff2ref_mat", probtrackx_inverted, "inv_xfm")
```

### Comparing `swane-0.0.6/swane/nipype_pipeline/workflows/venous_workflow.py` & `swane-0.1.0/swane/nipype_pipeline/workflows/venous_workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from nipype.interfaces.fsl import (BET, FLIRT, Split, ApplyMask, ImageStats, ImageMaths, ApplyXFM)
 from nipype.interfaces.utility import Merge
 from nipype.pipeline.engine import Node
-
 from swane.nipype_pipeline.engine.CustomWorkflow import CustomWorkflow
 from swane.nipype_pipeline.nodes.CustomDcm2niix import CustomDcm2niix
 from swane.nipype_pipeline.nodes.ForceOrient import ForceOrient
 from swane.nipype_pipeline.nodes.VenousCheck import VenousCheck
-
 from nipype.interfaces.utility import IdentityInterface
+from configparser import SectionProxy
 
 
-def venous_workflow(name: str, venous_dir: str, venous2_dir: str = None, base_dir: str = "/") -> CustomWorkflow:
+def venous_workflow(name: str, venous_dir: str, config: SectionProxy, venous2_dir: str = None, base_dir: str = "/") -> CustomWorkflow:
     """
     Analysis of phase contrasts images (in single or two series) to obtain in skull veins
     in reference space, scaled in 0-100 value.
 
     Parameters
     ----------
     name : str
         The workflow name.
     venous_dir : path
         The directory path of the venous phase contrast DICOM files.
+    config: SectionProxy
+        workflow settings.
     venous2_dir : path
         If veins phase is divided from anatomic phase, use this param to load the second DICOM files directory.
     base_dir : str, optional
         The base directory path relative to parent workflow. The default is "/".
 
     Input Node Fields
     ----------
@@ -63,21 +64,22 @@
 
     # NODE 2a: Orienting in radiological convention
     veins_reOrient = Node(ForceOrient(), name='veins_reOrient')
     workflow.connect(veins_conv, "converted_files", veins_reOrient, "in_file")
 
     # NODE 4: Detect the venous phase from the anatomic phase
     veins_check = Node(VenousCheck(), name='veins_check')
-    veins_check.long_name = "angiographic phase detection"
-
-    # If the phases are in the same sequence
+    veins_check.long_name = "angiographic volume detection"
+    vein_detection_mode = config.getenum_safe("vein_detection_mode")
+    veins_check.inputs.detection_mode = vein_detection_mode
+        # If the phases are in the same sequence
     if venous2_dir is None:
         # NODE 3a: Divide the two phases from the phase contrast
         veins_split = Node(Split(), name='veins_split')
-        veins_split.long_name = "phase splitting"
+        veins_split.long_name = "volumes splitting"
         veins_split.inputs.dimension = 't'
         workflow.connect(veins_reOrient, "out_file", veins_split, "in_file")
 
         workflow.connect(veins_split, "out_files", veins_check, "in_files")
     else:
         # NODE 1b: Conversion dicom -> nifti
         veins2_conv = Node(CustomDcm2niix(), name='veins2_conv')
@@ -87,26 +89,26 @@
 
         # NODE 2b: Orienting in radiological convention
         veins2_reOrient = Node(ForceOrient(), name='veins2_reOrient')
         workflow.connect(veins2_conv, "converted_files", veins2_reOrient, "in_file")
 
         # NODE 3b: Merge the two phases
         veins_merge = Node(Merge(2), name="veins_merge")
-        veins_merge.long_name = "phase merging"
+        veins_merge.long_name = "volumes merging"
         workflow.connect(veins_reOrient, "out_file", veins_merge, "in1")
         workflow.connect(veins2_reOrient, "out_file", veins_merge, "in2")
 
         workflow.connect(veins_merge, "out", veins_check, "in_files")
 
     # NODE 5: Scalp removal and in skull structures segmentation
     bet = Node(BET(), name='veins_bet')
-    bet.inputs.frac = 0.4
     bet.inputs.mask = True
     bet.inputs.threshold = True
     bet.inputs.surfaces = True
+    bet.inputs.frac = config.getfloat_safe('bet_thr')
     workflow.connect(veins_check, "out_file_anat", bet, "in_file")
 
     # NODE 6: Linear registration of anatomic phase to reference space
     anat_flirt = Node(FLIRT(), name='anat_flirt')
     anat_flirt.long_name = "%s to reference space"
     anat_flirt.inputs.out_matrix_file = "veins2ref.mat"
     anat_flirt.inputs.cost = "mutualinfo"
```

### Comparing `swane-0.0.6/swane/slicer/slicer_script_result.py` & `swane-0.1.0/swane/workers/slicer_script_result.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,17 +94,19 @@
     
     file = os.path.join(scene_dir, node_name)
     surf_node = None
     
     if os.path.exists(file):
         try:
             print("SLICERLOADER: Loading surface " + node_name)
-            surf_node = slicer.util.loadNodeFromFile(file, 'FreeSurferModelFile',
-                                                    {"referenceVolumeID": ref_node.GetID()})
-            surf_node.GetDisplayNode().SetColor(0.82, 0.82, 0.82)
+            loaded_nodes = vtk.vtkCollection()
+            surf_node = slicer.app.ioManager().loadNodes("FreeSurfer model", {"fileName": file, "referenceVolumeID": ref_node.GetID()}, loaded_nodes)
+            if surf_node:
+                surf_node = list(loaded_nodes)[0]
+                surf_node.GetDisplayNode().SetColor(0.82, 0.82, 0.82)
         except:
             pass
         
     return surf_node
 
 
 def load_freesurfer_overlay(scene_dir: str, node_name: str, surf_node):
@@ -127,16 +129,15 @@
 
     """
     
     file = os.path.join(scene_dir, node_name)
     if os.path.exists(file):
         try:
             print("SLICERLOADER: Loading surface overlay " + node_name)
-            overlay_node = slicer.util.loadNodeFromFile(file, 'FreeSurferScalarOverlayFile',
-                                                       {"modelNodeId": surf_node.GetID()})
+            overlay_node = slicer.util.loadNodeFromFile(file, 'FreeSurferScalarOverlayFile', {"modelNodeId": surf_node.GetID()})
             overlay_node.GetDisplayNode().SetAndObserveColorNodeID('vtkMRMLColorTableNodeFileColdToHotRainbow.txt')
             overlay_node.GetDisplayNode().SetScalarVisibility(False)
         except:
             pass
 
 
 def load_freesurfer_segmentation_file(seg_file: str):
@@ -152,15 +153,23 @@
     -------
     None.
 
     """
     
     if os.path.exists(seg_file):
         try:
-            slicer.util.loadNodeFromFile(seg_file, 'FreeSurferSegmentationFile')
+
+            # TODO: temporary fix for ubuntu crash
+            if "linux" in sys.platform:
+                slicer.util.loadVolume(seg_file, {"labelmap": True, "colorNodeID": "vtkMRMLColorTableNodeFile"})
+            else:
+                slicer.util.getModuleLogic('FreeSurferImporter').LoadFreeSurferSegmentation(seg_file)
+
+            # slicer.util.loadNodeFromFile(seg_file, 'FreeSurferSegmentationFile')
+
         except:
             pass
 
 
 def load_freesurfer(scene_dir: str, ref_node):
     """
     Loads the FreeSurfer output.
@@ -173,15 +182,15 @@
         The reference node for surface positioning.
 
     Returns
     -------
     None.
 
     """
-    
+
     seg_list = ["r-aparc_aseg.mgz", "segmentHA/lh.hippoAmygLabels.mgz", "segmentHA/rh.hippoAmygLabels.mgz"]
     for file in seg_list:
         seg_file = os.path.join(scene_dir, file)
         load_freesurfer_segmentation_file(seg_file)
 
     lh_pial = load_freesurfer_surf(scene_dir, "lh.pial", ref_node)
     rh_pial = load_freesurfer_surf(scene_dir, "rh.pial", ref_node)
@@ -364,55 +373,55 @@
         my_storage_node.SetFileName(os.path.join(scene_dir, "tracts_" + side + ".seg.nrrd"))
         my_storage_node.WriteData(segmentation_node)
 
 ###############################################################################
 
 # slicerpython execution code
 slicer.mrmlScene.Clear(0)
-sceneDir = os.path.join(os.getcwd(), "scene")
+results_folder = os.getcwd()
 
-if not os.path.isdir(sceneDir):
+if not os.path.isdir(results_folder):
     print("SLICERLOADER: Results folder not found")
 else:
-    refNode = load_anat(sceneDir, "ref")
+    refNode = load_anat(results_folder, "ref")
     if refNode is not None:
 
-        dtiDir = os.path.join(sceneDir, "dti")
+        dtiDir = os.path.join(results_folder, "dti")
         if os.path.isdir(dtiDir):
-            main_tract(dtiDir, sceneDir)
+            main_tract(dtiDir, results_folder)
 
-        lesion_segment(sceneDir)
+        # lesion_segment(sceneDir)
 
         baseList = ['ref_brain', 'r-flair_brain', 'r-mdc_brain', 'r-FA', 'r-flair2d_tra_brain', 'r-flair2d_cor_brain',
                     'r-flair2d_sag_brain', 'r-binary_flair', 'r-junction_z', 'r-extension_z']
 
         for volume in baseList:
-            load_anat(sceneDir, volume)
+            load_anat(results_folder, volume)
 
         colorList = [('r-asl_ai', 'vtkMRMLColorTableNodeFileDivergingBlueRed.txt'),
                      ('r-pet_ai', 'vtkMRMLColorTableNodeFileDivergingBlueRed.txt'),
                      ('r-pet', 'vtkMRMLColorTableNodeFileColdToHotRainbow.txt'),
                      ('r-pet_zscore', 'vtkMRMLColorTableNodeFileColdToHotRainbow.txt'),
                      ('r-asl', 'vtkMRMLColorTableNodeFileColdToHotRainbow.txt'),
                      ('r-asl_zscore', 'vtkMRMLColorTableNodeFileColdToHotRainbow.txt'),
                      ]
 
         for volume in colorList:
-            load_anat(sceneDir, volume[0], volume[1])
+            load_anat(results_folder, volume[0], volume[1])
 
-        load_fmri(sceneDir)
+        load_fmri(results_folder)
 
-        load_vein(sceneDir)
+        load_vein(results_folder)
 
-        load_freesurfer(sceneDir, refNode)
+        load_freesurfer(results_folder, refNode)
 
         ext = "mrb"
         
         #TODO valutare
         # Saving in MRML doesn't work well, disable extension choice for now
-        # if sys.argv[1] is not None and sys.argv[1] == "1":
+        # if sys.argv[1] is not None and sys.argv[1] == "mrml":
         #     ext = "mrml"
 
         print("SLICERLOADER: Saving multimodale scene (some minutes)")
-        slicer.util.saveScene(os.path.join(sceneDir, "scene." + ext))
+        slicer.util.saveScene(os.path.join(results_folder, "scene." + ext))
 
 sys.exit(0)
```

### Comparing `swane-0.0.6/swane/strings.py` & `swane-0.1.0/swane/strings.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,173 +1,172 @@
 # General
 APPNAME = "SWANe"
 app_acronym = "Standardized Workflow for Advanced Neuroimaging in Epilepsy"
 EXECBUTTONTEXT = "Execute " + APPNAME + " Workflow"
+EXECBUTTONTEXT_disabled_tooltip = "Generate Workflow first"
 EXECBUTTONTEXT_STOP = "Stop " + APPNAME + " Workflow"
 GENBUTTONTEXT = "Generate " + APPNAME + " Workflow"
-PTCONFIGBUTTONTEXT = "Workflow preferences"
+SUBJCONFIGBUTTONTEXT = "Workflow preferences"
+INFOCHAR = "\u24D8"
+WF_DIR_SUFFIX = "_nipype"
 
 # Main
 main_multiple_instances_error = "Another instance of " + APPNAME + " is already running!"
 
 # Main Window
 mainwindow_choose_working_dir = "Choose the main working directory before start to use this application"
 mainwindow_working_dir_space_error = "Blank spaces are not allowed in main working dir name or in its parent folder name"
 mainwindow_choose_working_dir_title = 'Select the main working directory'
-mainwindow_select_pt_folder = 'Select a patient folder'
-mainwindow_ptfolder_outside_workingdir_error = "The selected folder is not in " + APPNAME + " main working directory!"
-mainwindow_ptfolder_with_blank_spaces_error = "The selected folder name contains blank spaces!"
-mainwindow_pt_already_loaded_error = "The selected patient was already loaded in " + APPNAME + "!"
-mainwindow_invalid_folder_error = "The selected folder does not contains valid patient data!"
-mainwindow_force_dir_update = "If you are SURE you selected a patient folder, " + APPNAME + "can try to update " \
-                              "it.\nDo you want to update selected patient folder?"
-mainwindow_max_pt_error = "Max patient tab limit reached!"
-mainwindow_new_pt_name = 'Write the name of the new patient:'
-mainwindow_new_pt_title = 'New patient'
-mainwindow_new_pt_created = "New patient created in: "
-mainwindow_new_pt_name_error = "Invalid name: "
-mainwindow_pt_exists_error = "This patient already exists: "
-mainwindow_shortcut_created = "Shortcut created!"
-mainwindow_shortcut_removed = "Shortcut removed!"
+mainwindow_select_subj_folder = 'Select a subject folder'
+mainwindow_subj_folder_outside_workingdir_error = "The selected folder is not in " + APPNAME + " main working directory!"
+mainwindow_subj_folder_with_blank_spaces_error = "The selected folder name contains blank spaces!"
+mainwindow_subj_already_loaded_error = "The selected subject was already loaded in " + APPNAME + "!"
+mainwindow_invalid_folder_error = "The selected folder does not contains valid subject data!"
+mainwindow_force_dir_update = "If you are SURE you selected a subject folder, " + APPNAME + "can try to update " \
+                              "it.\nDo you want to update selected subject folder?"
+mainwindow_max_subj_error = "Max subject tab limit reached!"
+mainwindow_update_available = "New version available (%s). We recommend you to update " + APPNAME + " with:<br><b><center>pip3 install --upgrade swane"
+mainwindow_new_subj_name = 'Write the name of the new subject:'
+mainwindow_new_subj_title = 'New subject'
+mainwindow_new_subj_created = "New subject created: "
+mainwindow_new_subj_name_error = "Invalid name: "
+mainwindow_subj_exists_error = "This subject already exists: "
 mainwindow_home_tab_name = "Home"
-mainwindow_wf_executing_error_1 = "Cannot close a patient during workflow execution!"
+mainwindow_wf_executing_error_1 = "Cannot close a subject during workflow execution!"
 mainwindow_wf_executing_error_2 = "Cannot close " + APPNAME + " during workflow execution!"
 mainwindow_home_label1 = "Welcome to " + APPNAME + "!"
 mainwindow_home_label2 = APPNAME + " (" + app_acronym + ") is a graphic tools for modular neuroimaging processing. " \
                         "With " + APPNAME + " you can easily import and organize DICOM files from multiple sources, " \
                         "generate a pipeline based on available imaging modalities and export results in a " \
                         "multimodal scene."
 mainwindow_home_label3 = APPNAME + " does NOT implement processing software but integrates in a user-friendly " \
                         "interface many external applications, so make sure the check the following dependencies."
 mainwindow_home_label4 = APPNAME + " is not meant for clinical use!\n"
 mainwindow_home_label5 = "\nExternal mandatory dependencies:"
 mainwindow_home_label6 = "\nExternal recommended dependencies:"
 mainwindow_home_label7 = "\nExternal optional dependencies:"
 
 mainwindow_dep_slicer_src = "Searching Slicer installation..."
-mainwindow_dep_slicer_found = "Slicer detected"
-mainwindow_pref_disabled_error = "Prefecences disabled during workflow execution!"
+mainwindow_pref_disabled_error = "Preferences disabled during workflow execution!"
 aboutwindow_python_libs = "Python libraries dependencies: configparser, logging, matplotlib, nipype, pydicom, " \
-                          "pyshortcuts, PySide6, psutil"
+                          "PySide6, psutil, nibabel, networkx"
 
 # Menu
-menu_load_pt = "Load existing patient"
-menu_load_pt_tip = "Load patient data from the main working directory"
-menu_new_pt = "Create new patient"
-menu_new_pt_tip = "Add a new patient in the main working directory"
+menu_load_subj = "Load existing subject"
+menu_load_subj_tip = "Load subject data from the main working directory"
+menu_new_subj = "Create new subject"
+menu_new_subj_tip = "Add a new subject in the main working directory"
 menu_exit = "Exit " + APPNAME
-menu_pref = "Preferences"
-menu_pref_tip = "Edit " + APPNAME + " preferences"
-menu_shortcut = "Toggle shortcuts"
+menu_pref = "Application settings"
+menu_pref_tip = "Edit " + APPNAME + " settings"
+menu_wf_pref = "Default Workflow preferences"
 menu_about = "About " + APPNAME + "..."
 menu_file_name = "File"
 menu_tools_name = "Tools"
 menu_help_name = "Help"
 
-# Patient Tab
-pttab_data_tab_name = "Data load"
-pttab_wf_tab_name = "Workflow execution"
-pttab_results_tab_name = "Results export"
-pttab_wf_executed = APPNAME + " Workflow executed!"
-pttab_wf_executed_with_error = APPNAME + " Workflow finished. Error occurred!"
-pttab_import_button = "Import"
-pttab_clear_button = "Clear"
-pttab_scan_dicom_button = "Scan DICOM folder"
-pttab_selected_series_error = "No series was selected"
-pttab_wrong_type_check = "Do you want to continue importing?"
-pttab_wrong_type_check_msg = "You selected %s images while %s images were expected."
-pttab_dicom_copy = "Copying DICOM files in patient folder..."
-pttab_dicom_check = "Verifying patient folder..."
-pttab_dicom_scan = "Scanning DICOM folder..."
-pttab_pt_loading = "Checking patient DICOM folders..."
-pttab_select_dicom_folder = 'Select a folder to scan for DICOM files'
-pttab_no_dicom_error = "No DICOM file in "
-pttab_multi_pt_error = "Dicom file from more than one patient in "
-pttab_multi_exam_error = "DICOM file from more than one examination in "
-pttab_multi_series_error = "DICOM file from more than one series in "
-pttab_missing_fsl_error = "FSL is required to generate " + APPNAME + " Workflow!"
-pttab_wf_gen_error = "Error generating the Workflow!"
-pttab_old_wf_found = "This patient has already been analyzed by " + APPNAME + """. Do you want to resume the previous analysis? If you want to delete all
+# Subject Tab
+subj_tab_data_tab_name = "Data load"
+subj_tab_wf_tab_name = "Workflow execution"
+subj_tab_results_tab_name = "Results export"
+subj_tab_wf_executed = APPNAME + " Workflow executed!"
+subj_tab_wf_executed_with_error = APPNAME + " Workflow finished. Error occurred!"
+subj_tab_import_button = "Import"
+subj_tab_clear_button = "Clear"
+subj_tab_scan_dicom_button = "Scan DICOM folder"
+subj_tab_selected_series_error = "No series was selected"
+subj_tab_wrong_type_check = "Do you want to continue importing?"
+subj_tab_wrong_type_check_msg = "You selected %s images while %s images were expected."
+subj_tab_wrong_max_vols_check_msg = "The series you selected contains %d volumes while a maximum of %d were expected."
+subj_tab_wrong_min_vols_check_msg = "The series you selected contains %d volumes while a minimum of %d were expected."
+subj_tab_import_copy_error_msg = "Error copying selected series files."
+subj_tab_import_folder_not_empy = "Images are already loaded for this series."
+subj_tab_dicom_copy = "Copying DICOM files in subject folder..."
+subj_tab_dicom_check = "Verifying subject folder..."
+subj_tab_dicom_scan = "Scanning DICOM folder..."
+subj_tab_subj_loading = "Checking subject DICOM folders..."
+subj_tab_select_dicom_folder = 'Select a folder to scan for DICOM files'
+subj_tab_no_dicom_error = "No DICOM file in "
+subj_tab_multi_subj_error = "Dicom file from more than one subject in "
+subj_tab_multi_exam_error = "DICOM file from more than one examination in "
+subj_tab_multi_series_error = "DICOM file from more than one series in "
+subj_tab_missing_fsl_error = "FSL is required to generate " + APPNAME + " Workflow!"
+subj_tab_wf_gen_error = "Error generating the Workflow!"
+subj_tab_old_wf_found = "This subject has already been analyzed by " + APPNAME + """. Do you want to resume the previous analysis? If you want to delete all
 previous analyses and start over press NO, otherwise press YES"""
-pttab_old_wf_resume = "Resume execution"
-pttab_old_wf_reset = "New execution"
-pttab_old_fs_found = "An existing FreeSurfer folder was detected. Do you want to keep or delete the existing folder?"
-pttab_old_fs_resume = "Keep folder"
-pttab_old_fs_reset = "Delete folder"
-pttab_wf_stop = "Do you REALLY want to stop " + APPNAME + " Workflow execution?"
-pttab_results_button = "Export results into Slicer scene"
-pttab_exporting_start = "Exporting results into Slicer scene...\nLoading Slicer environment"
-pttab_exporting_prefix = "Exporting results into Slicer scene...\n"
-pttab_dicom_clearing = "Clearing DICOM files in: "
-pttab_wf_insufficient_resources = "Insufficient system resources (RAM or CPU) to execute workflows"
+subj_tab_old_wf_resume = "Resume execution"
+subj_tab_old_wf_reset = "New execution"
+subj_tab_old_fs_found = "An existing FreeSurfer folder was detected. Do you want to keep or delete the existing folder?"
+subj_tab_old_fs_resume = "Keep folder"
+subj_tab_old_fs_reset = "Delete folder"
+subj_tab_wf_stop = "Do you REALLY want to stop " + APPNAME + " Workflow execution?"
+subj_tab_generate_scene_button = "Create/Update Slicer scene " + INFOCHAR
+subj_tab_generate_scene_button_tooltip = "In case of a new analysis remember to update the Slicer scene"
+subj_tab_generate_scene_button_disabled_tooltip = "Slicer not detected"
+subj_tab_load_scene_button = "Visualize scene into Slicer"
+subj_tab_load_scene_button_tooltip = "Create a Slicer scene first"
+subj_tab_open_results_directory = "Open results folder"
+subj_tab_exporting_start = "Exporting results into Slicer scene...\nLoading Slicer environment"
+subj_tab_exporting_prefix = "Exporting results into Slicer scene...\n"
+subj_tab_dicom_clearing = "Clearing DICOM files in: "
+subj_tab_wf_insufficient_resources = "Insufficient system resources (RAM or CPU) to execute workflows"
+subj_tab_wf_invalid_signal = "Signaling error, workflow will be stopped. Report this error."
+subj_tab_wf_error_oom_gpu = "Process killed: Out of Memory (GPU). Try to reduce GPU process limit in performance preferences"
+subj_tab_wf_error_oom = "Process killed (possible Out of Memory). Try to reduce CPU core limit in performance preferences"
+subj_tab_wf_error_terminated = "Process terminated. This can occur if user manually terminates a running process."
+subj_tab_tabtooltip_exec_disabled_series = "A 3D T1w series is required to enable workflow execution"
+subj_tab_tabtooltip_exec_disabled_dependency = "Mandatory dependencies are required to enable workflow execution"
+subj_tab_tabtooltip_result_disabled = "Complete a workflow first"
+subj_tab_tabtooltip_data_disabled = "Cannot change subject data during workflow execution"
+
+# Wf Preference Window
+wf_pref_window_title_user = ' - Workflow preferences'
 
 # Preference Window
-pref_window_title_global = APPNAME + ' - Preferences'
-pref_window_title_user = ' - Workflow preferences'
-pref_window_global_box_title = "Global settings"
-pref_window_global_box_mwd = "Main working directory"
-pref_window_global_box_slicer = "3D Slicer path"
-pref_window_global_box_default_wf = "Default workflow"
-pref_window_global_box_default_task = "Default fMRI taks duration"
-pref_window_global_box_pt_limit = "Patient tab limit"
-pref_window_global_box_cpu_limit = "CPU per Patient limit"
-pref_window_global_box_default_ext = "Slicer scene extension"
-pref_window_global_box_optional_title = "Optional series settings"
-pref_window_wf_box_title = "Workflow settings"
-pref_window_wf_box_reconall = "FreeSurfer analysis"
-pref_window_wf_box_reconall_disabled_tip = "FreeSurfer not detected"
-pref_window_wf_box_hippo = "FreeSurfer hippocampal subfields"
-pref_window_wf_box_hippo_disabled_tip = "Matlab Runtime not detected"
-pref_window_wf_box_ai = "Asymmetry Index map for ASL and PET"
-pref_window_wf_box_FLAT1 = "FLAT1 analysis"
-pref_window_wf_box_tractography = "DTI tractography"
-pref_window_wf_box_missing_flair3d = "3D Flair missing"
-pref_window_wf_box_missing_dti = "DTI missing"
-pref_window_wf_box_missing_ai = "Asymmetry Index maps can be generated for PET or ASL data"
-pref_window_fmri_box_task_a_name = "Task A name"
-pref_window_fmri_box_task_b_name = "Task B name"
-pref_window_fmri_box_task_duration = "Task duration (sec)"
-pref_window_fmri_box_rest_duration = "Rest duration (sec)"
-pref_window_fmri_box_tr = "TR (sec)"
-pref_window_fmri_box_vols = "Number of EPI runs"
-pref_window_fmri_box_st = "Slice timing"
-pref_window_fmri_box_blockdesign = "Block design"
-pref_window_fmri_box_del_start_vols = "Delete start volumes"
-pref_window_fmri_box_del_end_vols = "Delete end volumes"
-pref_window_tract_box_title = "Tractography settings"
 pref_window_save_button = "Save preferences"
 pref_window_save_restart_button = "Save preferences (" + APPNAME + " will close and restart)"
 pref_window_discard_button = "Discard changes"
 pref_window_dir_error = "Directory does not exists!"
 pref_window_file_error = "File does not exists!"
-pref_window_select_slicer = "Select 3D Slicer executable"
+
+pref_window_reset_global_button = "Reset workflow settings to default"
+pref_window_reset_global_box = "Do you really want to reset global workflow settings to application default?"
+pref_window_reset_subj_button = "Apply default workflow settings"
+pref_window_reset_subj_box = "Do you really want to apply default workflow settings to this subject?"
 
 # Workflow
+check_dep_generic_error = "Dependency check error"
 check_dep_dcm2niix_error = "dcm2niix not detected (<a href='https://github.com/rordenlab/dcm2niix#Install" \
                            "'>installation info</a>)"
 check_dep_dcm2niix_found = "dcm2niix detected (%s)"
 check_dep_fsl_error = "FSL not detected (<a href='https://fsl.fmrib.ox.ac.uk/fsl/fslwiki/FslInstallation" \
                       "'>installation info</a>)"
+check_dep_fsl_wrong_version = "FSL version outdated (found %s, required %s). Please " \
+                              "<a href='https://fsl.fmrib.ox.ac.uk/fsl/fslwiki/FslInstallation'>update</a>"
 check_dep_fsl_found = "FSL detected (%s)"
 check_dep_fs_found = "FreeSurfer detected (%s)"
 check_dep_fs_error1 = "FreeSurfer not detected (<a href='https://surfer.nmr.mgh.harvard.edu/fswiki/DownloadAndInstall" \
                       "'>installation info</a>)"
 check_dep_fs_error2 = "FreeSurfer detected (%s) but without environment configuration"
 check_dep_fs_error3 = "FreeSurfer detected (%s). Matlab Runtime is not installed (<a " \
                       "href='https://surfer.nmr.mgh.harvard.edu/fswiki/MatlabRuntime'>registration instruction</a>)"
 check_dep_fs_error4 = "FreeSurfer detected (%s). License key missing (<a " \
                       "href='https://surfer.nmr.mgh.harvard.edu/registration.html'>registration instruction</a>)"
+check_dep_fs_wrong_version = "FreeSurfer version outdated (found %s, required %s). Please " \
+                              "<a href='https://surfer.nmr.mgh.harvard.edu/fswiki/DownloadAndInstall'>update</a>"
 check_dep_graph_error = "Graphviz not detected (<a href='https://graphviz.org/download/'>Installation info</a>)"
 check_dep_graph_found = "Graphviz detected"
 check_dep_slicer_error1 = "Slicer not detected (<a href='https://slicer.readthedocs.io/en/latest/user_guide" \
                           "/getting_started.html#installing-3d-slicer/'>Installation info</a>)"
 check_dep_slicer_error2 = "Slicer detected but without SlicerFreeSurfer extension (<a " \
                           "href='https://slicer.readthedocs.io/en/latest/user_guide/extensions_manager.html?highlight" \
-                          "=extension%20manager'>Exstensions Manager info</a>)"
-check_dep_slicer_found = "Slicer detected"
+                          "=extension%20manager'>Extensions Manager info</a>)"
+check_dep_slicer_wrong_version = "Slicer version outdated (found %s, required %s). Please " \
+                              "<a href='https://slicer.readthedocs.io/en/latest/user_guide'>update</a>"
+check_dep_slicer_found = "Slicer detected (%s)"
 
 fsl_python_error = APPNAME + " has been executed using fsl Python instead of system Python.\nThis may depend " \
                     "on a conflict in FSL(>=6.0.6) and FreeSurfer(<=7.3.2) configurations in your %s file that " \
                     "impacts on correct functioning of " + APPNAME + " and maybe other applications.\n" + APPNAME + \
                     " can try to fix your configuration file or to restart with system Python interpreter. Otherwise" \
                     " you can exit " + APPNAME + " and fix your configuration manually adding this line to your " \
                     "configuration file:"
@@ -184,15 +183,17 @@
 node_names["FLIRT"] = "linear registration"
 node_names["ApplyXFM"] = "linear transformation"
 node_names["FNIRT"] = "nonlinear registration"
 node_names["ApplyWarp"] = "nonlinear transformation"
 node_names["InvWarp"] = "inverse transformation"
 node_names["DataSink"] = "saving"
 node_names["ApplyMask"] = "masking"
-node_names["EddyCorrect"] = "eddy current correction"
+node_names["EddyCorrect"] = "eddy current correction (old)"
+node_names["CustomEddy"] = "eddy current correction"
+node_names["GenEddyFiles"] = "eddy current correction preparation"
 node_names["CustomBEDPOSTX5"] = "diffusion bayesian estimation"
 node_names["RandomSeedGenerator"] = "random seeds generation"
 node_names["CustomProbTrackX2"] = "probabilistic tractography"
 node_names["SumMultiTracks"] = "Parallel tractography merging"
 node_names["ReconAll"] = "Freesurfer recon-all"
 node_names["CustomLabel2Vol"] = "linear transformation"
 node_names["SegmentHA"] = "hippocampal segmentation"
@@ -202,11 +203,11 @@
 node_names["FMRIGenSpec"] = "functional model generation"
 node_names["ArtifactDetect"] = "outliers detection"
 node_names["SpecifyModel"] = "functional model application"
 node_names["Level1Design"] = "FEAT files generation"
 node_names["FEATModel"] = "design file generation"
 node_names["FILMGLS"] = "General-Linear-Model estimation"
 node_names["SmoothEstimate"] = "smoothness estimation"
-node_names["FslCluster"] = "cluster extraction"
+node_names["Cluster"] = "cluster extraction"
 node_names["SampleToSurface"] = "surface projection"
 node_names["FAST"] = "Tissue segmentation"
-node_names["FLAT1OutliersMask"] = "outliers mask generation"
+node_names["FLAT1OutliersMask"] = "outliers mask generation"
```

### Comparing `swane-0.0.6/swane/ui/CustomTreeWidgetItem.py` & `swane-0.1.0/swane/ui/CustomTreeWidgetItem.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from PySide6.QtWidgets import QWidget, QLabel, QHBoxLayout, QTreeWidgetItem, QSpacerItem
+from PySide6.QtWidgets import QWidget, QLabel, QHBoxLayout, QTreeWidgetItem, QSpacerItem, QTreeWidget
 from PySide6.QtSvgWidgets import QSvgWidget
+from swane import strings
 
 
 class CustomTreeWidgetItem(QTreeWidgetItem):
     """
     Custom implementation of PySide QTreeWidgetItem to define the Workflows Tree items.
 
     """
 
-    def __init__(self, parent, tree, text, art=None):
+    def __init__(self, parent, tree: QTreeWidget, text: str, art: str = None):
         super(CustomTreeWidgetItem, self).__init__(parent)
         
         self.widget = QWidget()
         self.widget.setLayout(QHBoxLayout())
         self.artLabel = QSvgWidget()
         self.artLabel.setFixedWidth(26)
         self.artLabel.setFixedHeight(26)
@@ -25,15 +26,26 @@
         self.widget.layout().addSpacerItem(QSpacerItem(25, 0))
 
         tree.setItemWidget(self, 0, self.widget)
         
         self.completed = False
         self.art = None
 
-    def setText(self, text: str):
+    def setToolTip(self, column, toolTip):
+        """
+        Reimplement base method to add info character .
+
+        """
+        if toolTip == "" and self.get_text().endswith(strings.INFOCHAR):
+            self.set_text(self.get_text()[:-2])
+        elif toolTip != "" and not self.get_text().endswith(strings.INFOCHAR):
+            self.set_text(self.get_text() + " " + strings.INFOCHAR)
+        super().setToolTip(column, toolTip)
+
+    def set_text(self, text: str):
         """
         Set the tree item text.
 
         Parameters
         ----------
         text : str
             The item text.
```

### Comparing `swane-0.0.6/swane/ui/MainWindow.py` & `swane-0.1.0/swane/ui/MainWindow.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,265 +1,292 @@
-from PySide6.QtWidgets import (QMainWindow, QMessageBox, QFileDialog, QInputDialog,
+from PySide6.QtWidgets import (QMainWindow, QMessageBox, QFileDialog, QInputDialog, QStyle,
                                QLineEdit, QTabWidget, QGridLayout, QLabel, QSizePolicy,
-                               QSpacerItem, QWidget, QTabBar, QDialog)
-from swane.utils.check_dependency import (check_dcm2niix, check_fsl, check_freesurfer,
-                                          check_graphviz)
+                               QSpacerItem, QWidget, QTabBar, QDialog, QPushButton, QStyleOptionButton)
 from PySide6.QtGui import QAction, QIcon, QPixmap, QFont, QCloseEvent
-from PySide6.QtCore import QCoreApplication, QThreadPool
+from PySide6.QtCore import QCoreApplication, Qt, QThreadPool
 from PySide6.QtSvgWidgets import QSvgWidget
 import os
-import sys
-
-from swane.ui.PtTab import PtTab
+from swane.utils.DependencyManager import DependencyManager, Dependence, DependenceStatus
+from swane.ui.SubjectTab import SubjectTab
 from swane.ui.PreferencesWindow import PreferencesWindow
 import swane_supplement
 from swane import __version__, EXIT_CODE_REBOOT, strings
-from swane.utils.DataInput import DataInputList
-from swane.utils.shortcut_manager import shortcut_manager
-from swane.slicer.SlicerCheckWorker import SlicerCheckWorker
+from swane.workers.UpdateCheckWorker import UpdateCheckWorker
+from swane.utils.Subject import Subject, SubjectRet
+from swane.config.ConfigManager import ConfigManager
 
 
 class MainWindow(QMainWindow):
     """
     Custom implementation of PySide QMainWindow to define SWANe GUI.
 
     """
        
-    def __init__(self, global_config):
+    def __init__(self, global_config: ConfigManager):
 
-        # GUI configuration setting
-        self.global_config = global_config
-        
         super(MainWindow, self).__init__()
-        
+
+        # GUI configuration setting
+        self.global_config: ConfigManager = global_config
+        self.dependency_manager: DependencyManager = DependencyManager()
+        self.global_config.check_dependencies(self.dependency_manager)
+
         # GUI Icons setting
         self.setWindowIcon(QIcon(QPixmap(swane_supplement.appIcon_file)))
         self.OK_ICON_FILE = swane_supplement.okIcon_file
         self.ERROR_ICON_FILE = swane_supplement.errorIcon_file
         self.WARNING_ICON_FILE = swane_supplement.warnIcon_file
         self.LOADING_MOVIE_FILE = swane_supplement.loadingMovie_file
         self.VOID_SVG_FILE = swane_supplement.voidsvg_file
         self.OK_ICON = QPixmap(self.OK_ICON_FILE)
         self.ERROR_ICON = QPixmap(self.ERROR_ICON_FILE)
         self.WARNING_ICON = QPixmap(self.WARNING_ICON_FILE)
+        self.NON_UNICODE_BUTTON_HEIGHT = MainWindow.get_non_unicode_height()
 
-        # Patient folder configuration checking
-        while self.global_config.get_patients_folder() == "" or not os.path.exists(
-                self.global_config.get_patients_folder()):
+        # subject folder configuration checking
+        while self.global_config.get_main_working_directory() == "":
             msg_box = QMessageBox()
             msg_box.setText(strings.mainwindow_choose_working_dir)
             msg_box.exec()
-            self.set_patients_folder()
+            self.set_main_working_directory()
 
-        # Patient folder configuration setting
-        os.chdir(self.global_config.get_patients_folder())
+        # subject folder configuration setting
+        os.chdir(self.global_config.get_main_working_directory())
 
         self.initialize_ui()
 
-        # SWANe launching icon checking
-        if self.global_config.get_shortcut_path() != '':
-            targets = self.global_config.get_shortcut_path().split("|")
-            new_path = ''
-            change = False
-            for fil in targets:
-                if strings.APPNAME in fil and os.path.exists(fil):
-                    if new_path != '':
-                        new_path = new_path + "|"
-                    new_path = new_path + fil
-                else:
-                    change = True
-            if change:
-                self.global_config.set_shortcut_path(new_path)
-                self.global_config.save()
+        # Check for update
+        update_thread = UpdateCheckWorker()
+        update_thread.signal.last_available.connect(lambda pip_version: self.update_available(pip_version))
+        QThreadPool.globalInstance().start(update_thread)
+
+    def update_available(self, pip_version: str):
+        """
+        Called if UpdateCheckWorker detect a newer version on pip
+        Parameters
+        ----------
+        pip_version: str
+            The version of the update available on pip
+        """
+        msg_box = QMessageBox(parent=self)
+        msg_box.setIcon(QMessageBox.Icon.Information)
+        msg_box.setText(strings.mainwindow_update_available % pip_version)
+        msg_box.exec()
+
+    @staticmethod
+    def get_non_unicode_height() -> int:
+        """
+        Returns
+        -------
+        The pixel height of a generic label WITHOUT unicode character
+        """
+        button = QPushButton()
+        opt = QStyleOptionButton()
+        opt.initFrom(button)
+        text_size = button.fontMetrics().size(Qt.TextShowMnemonic, button.text())
+        return button.style().sizeFromContents(QStyle.CT_PushButton, opt, text_size, button).height()
 
-    def open_pt_dir(self, folder_path: str):
+    def open_subject_tab(self, subject: Subject):
         """
-        Load a checked and valid patient folder.
+        Load a checked and valid subject folder.
 
         Parameters
         ----------
-        folder_path : str
-            The patient folder path.
+        subject : str
+            The subject to load in the tab.
 
         Returns
         -------
         None.
 
         """
         
-        this_tab = PtTab(self.global_config, folder_path,
-                         self, parent=self.main_tab)
-        this_tab.set_main_window(self)
-        self.pt_tabs_array.append(this_tab)
+        this_tab = SubjectTab(self.global_config, subject, main_window=self, parent=self.main_tab)
+        self.subject_tab_array.append(this_tab)
 
-        self.main_tab.addTab(this_tab, os.path.basename(folder_path))
+        self.main_tab.addTab(this_tab, os.path.basename(subject.name))
         self.main_tab.setCurrentWidget(this_tab)
         
-        this_tab.load_pt()
+        this_tab.load_subject()
 
-    def check_pt_limit(self) -> bool:
+    def check_subject_limit(self) -> bool:
         """
-        Check if SWANe can open another patient tab without overcome the limit set by configuration.
+        Check if SWANe can open another subject tab without overcome the limit set by configuration.
 
         Returns
         -------
         bool
             True if SWANe can load another tab, otherwise False.
 
         """
         
-        max_pt = self.global_config.get_max_pt()
-        if max_pt <= 0:
+        max_subjects = self.global_config.get_max_subject_tabs()
+        if max_subjects <= 0:
             return True
-        if len(self.pt_tabs_array) >= max_pt:
+        if len(self.subject_tab_array) >= max_subjects:
             msg_box = QMessageBox()
             msg_box.setIcon(QMessageBox.Icon.Warning)
-            msg_box.setText(strings.mainwindow_max_pt_error)
+            msg_box.setText(strings.mainwindow_max_subj_error)
             msg_box.exec()
             return False
         return True
 
-    def search_pt_dir(self):
+    def search_subject_dir(self, button_state: bool = False, folder_path: str = None):
         """
-        Try to open a patient directory
+        Try to open a subject directory
+
+        Parameters
+        ----------
+        button_state: bool
+            Not used, passed by QPushButton. Default is False
+        folder_path: str
+            The folder to load. Default is None
 
         Returns
         -------
         None.
 
         """
         
-        # Guard to avoid the opening of patient tabs greater than the maximum allowed
-        if not self.check_pt_limit():
+        # Guard to avoid the opening of subject tabs greater than the maximum allowed
+        if not self.check_subject_limit():
             return
 
-        # Open the directory selection dialog 
-        file_dialog = QFileDialog()
-        file_dialog.setDirectory(self.global_config.get_patients_folder())
-        folder_path = file_dialog.getExistingDirectory(self, strings.mainwindow_select_pt_folder)
-        if not os.path.exists(folder_path):
-            return
+        if folder_path is None:
+            # Open the directory selection dialog if a path is not provided
+            file_dialog = QFileDialog()
+            file_dialog.setDirectory(self.global_config.get_main_working_directory())
+            folder_path = file_dialog.getExistingDirectory(self, strings.mainwindow_select_subj_folder)
 
-        # Guard to avoid the opening a directory containing blank spaces
-        if ' ' in folder_path:
+        subject = Subject(self.global_config, dependency_manager=self.dependency_manager)
+
+        # Guard to avoid an already loaded subject directory
+        for tab in self.subject_tab_array:
+            if tab.subject.folder == folder_path:
+                msg_box = QMessageBox()
+                msg_box.setIcon(QMessageBox.Icon.Warning)
+                msg_box.setText(strings.mainwindow_subj_already_loaded_error)
+                msg_box.exec()
+                return
+
+        subject_load_ret = subject.load(folder_path)
+
+        if subject_load_ret == SubjectRet.ValidFolder:
+            self.open_subject_tab(subject)
+        elif subject_load_ret == SubjectRet.FolderNotFound:
+            # User canceled subject load
+            return
+        elif subject_load_ret == SubjectRet.PathBlankSpaces:
+            # Guard to avoid the opening a directory containing blank spaces
             msg_box = QMessageBox()
             msg_box.setIcon(QMessageBox.Icon.Critical)
-            msg_box.setText(strings.mainwindow_ptfolder_with_blank_spaces_error)
+            msg_box.setText(strings.mainwindow_subj_folder_with_blank_spaces_error)
             msg_box.exec()
             return
-
-
-        # Guard to avoid the opening of a directory outside the main patient folder
-        if not os.path.abspath(folder_path).startswith(
-                os.path.abspath(self.global_config.get_patients_folder()) + os.sep):
+        elif subject_load_ret == SubjectRet.FolderOutsideMain:
+            # Guard to avoid the opening of a directory outside the main subject folder
             msg_box = QMessageBox()
             msg_box.setIcon(QMessageBox.Icon.Critical)
-            msg_box.setText(strings.mainwindow_ptfolder_outside_workingdir_error)
+            msg_box.setText(strings.mainwindow_subj_folder_outside_workingdir_error)
             msg_box.exec()
             return
-
-        # Guard to avoid an already loaded patient directory
-        for pt in self.pt_tabs_array:
-            if pt.pt_folder == folder_path:
-                msg_box = QMessageBox()
-                msg_box.setIcon(QMessageBox.Icon.Warning)
-                msg_box.setText(strings.mainwindow_pt_already_loaded_error)
-                msg_box.exec()
-                return
-
-        # Check if selected folder is a valid patient folder
-        if not self.check_pt_dir(folder_path):
+        elif subject_load_ret == SubjectRet.InvalidFolderTree:
+            # Check if selected folder is a valid subject folder
             msg_box = QMessageBox()
             msg_box.setIcon(QMessageBox.Icon.Warning)
             msg_box.setText(strings.mainwindow_invalid_folder_error)
             msg_box.exec()
 
             msg_box2 = QMessageBox()
             msg_box2.setText(strings.mainwindow_force_dir_update)
             msg_box2.setIcon(QMessageBox.Icon.Question)
             msg_box2.setStandardButtons(QMessageBox.StandardButton.Yes | QMessageBox.StandardButton.No)
             msg_box2.button(QMessageBox.StandardButton.Yes).setText("Yes")
             msg_box2.button(QMessageBox.StandardButton.No).setText("No")
             msg_box2.setDefaultButton(QMessageBox.StandardButton.No)
             ret = msg_box2.exec()
-            
-            # A patient folder has a predefined folder tree.
-            # SWANe recognizes a patient folder checking its subfolders.
-            # If a selected folder is not valid, the user may force its conversion into a patient folder.
+
+            # A subject folder has a predefined folder tree.
+            # SWANe recognizes a subject folder checking its subfolders.
+            # If a selected folder is not valid, the user may force its conversion into a subject folder.
             if ret == QMessageBox.StandardButton.Yes:
-                self.update_pt_dir(folder_path)
-            else:
-                return
+                subject.fix_subject_folder_subtree(folder_path)
+                self.search_subject_dir(folder_path=folder_path)
+            return
             
-        self.open_pt_dir(folder_path)
+        return
 
-    def get_suggested_patient_name(self) -> str:
+    def get_suggested_subject_name(self) -> str:
         """
-        Get a default name for the patient folder based the existing patient folders into the main patient directory.
+        Get a default name for the subject folder based the existing subject folders into the main subject directory.
 
         Returns
         -------
         str
-            The suggested patient folder name.
+            The suggested subject folder name.
 
         """
         
         import re
         
-        regex = re.compile('^' + self.global_config.get_patientsprefix() + '\d+$')
+        regex = re.compile('^' + self.global_config.get_subjects_prefix() + '\d+$')
         file_list = []
         
-        for this_dir in os.listdir(self.global_config.get_patients_folder()):
+        for this_dir in os.listdir(self.global_config.get_main_working_directory()):
             if regex.match(this_dir):
                 file_list.append(
-                    int(this_dir.replace(self.global_config.get_patientsprefix(), "")))
+                    int(this_dir.replace(self.global_config.get_subjects_prefix(), "")))
 
         if len(file_list) == 0:
-            return self.global_config.get_patientsprefix() + "1"
+            return self.global_config.get_subjects_prefix() + "1"
         
-        return self.global_config.get_patientsprefix() + str(max(file_list) + 1)
+        return self.global_config.get_subjects_prefix() + str(max(file_list) + 1)
 
-    def choose_new_pt_dir(self):
+    def choose_new_subject_dir(self):
         """
-        Create a new patient folder. The user must specify its name.
+        Create a new subject folder. The user must specify its name.
 
         Returns
         -------
         None.
 
         """
         
-        if not self.check_pt_limit():
+        if not self.check_subject_limit():
             return
 
-        text, ok = QInputDialog.getText(self, strings.mainwindow_new_pt_title, strings.mainwindow_new_pt_name,
-                                        QLineEdit.EchoMode.Normal, self.get_suggested_patient_name())
+        text, ok = QInputDialog.getText(self, strings.mainwindow_new_subj_title, strings.mainwindow_new_subj_name,
+                                        QLineEdit.EchoMode.Normal, self.get_suggested_subject_name())
 
         if not ok:
             return
 
-        pt_name = str(text)
+        subject_name = str(text).replace(" ", "_")
+        subject = Subject(self.global_config, dependency_manager=self.dependency_manager)
+        create_subject_ret = subject.create_new_subject_dir(subject_name)
 
-        if pt_name == "":
+        if create_subject_ret == SubjectRet.FolderNotFound or create_subject_ret == SubjectRet.PathBlankSpaces:
             msg_box = QMessageBox()
-            msg_box.setText(strings.mainwindow_new_pt_name_error + pt_name)
+            msg_box.setText(strings.mainwindow_new_subj_name_error + subject_name)
             msg_box.exec()
             return
-
-        if os.path.exists(os.path.join(self.global_config.get_patients_folder(), pt_name)):
+        elif create_subject_ret == SubjectRet.FolderAlreadyExists:
             msg_box = QMessageBox()
-            msg_box.setText(strings.mainwindow_pt_exists_error + pt_name)
+            msg_box.setText(strings.mainwindow_subj_exists_error + subject_name)
             msg_box.exec()
             return
+        elif create_subject_ret == SubjectRet.ValidFolder:
+            msg_box = QMessageBox()
+            msg_box.setText(strings.mainwindow_new_subj_created + subject_name)
+            msg_box.exec()
+            self.open_subject_tab(subject)
 
-        self.create_new_pt_dir(pt_name.replace(" ", "_"))
-
-    def set_patients_folder(self):
+    def set_main_working_directory(self):
         """
-        Generates the OS directory selection dialog to set the default patient folder
+        Generates the OS directory selection dialog to set the default subject folder
 
         Returns
         -------
         None.
 
         """
         
@@ -270,147 +297,96 @@
 
         if ' ' in folder_path:
             msg_box = QMessageBox()
             msg_box.setText(strings.mainwindow_working_dir_space_error)
             msg_box.exec()
             return
         
-        self.global_config.set_patients_folder(os.path.abspath(folder_path))
-        self.global_config.save()
+        self.global_config.set_main_working_directory(os.path.abspath(folder_path))
         
         os.chdir(folder_path)
 
-    def create_new_pt_dir(self, pt_name: str):
+    def edit_config(self):
         """
-        Create a new patient folder and subfolders.
-
-        Parameters
-        ----------
-        pt_name : str
-            The patient folder name.
+        Open the Global Preferences Window.
 
         Returns
         -------
         None.
 
         """
         
-        base_folder = os.path.abspath(os.path.join(
-            self.global_config.get_patients_folder(), pt_name))
-
-        dicom_folder = os.path.join(base_folder, self.global_config.get_default_dicom_folder())
-
-        for data_input in DataInputList().values():
-            os.makedirs(os.path.join(
-                dicom_folder, data_input.name), exist_ok=True)
-
-        msg_box = QMessageBox()
-        msg_box.setText(strings.mainwindow_new_pt_created + base_folder)
-        msg_box.exec()
-
-        self.open_pt_dir(base_folder)
-
-    def check_pt_dir(self, dir_path: str) -> bool:
-        """
-        Check if a directory is a valid patient folder
-
-        Parameters
-        ----------
-        dir_path : str
-            The directory path to check.
-
-        Returns
-        -------
-        bool
-            True if the directory is a valid patient folder, otherwise False.
+        if self.check_running_workflows():
+            msg_box = QMessageBox()
+            msg_box.setText(strings.mainwindow_pref_disabled_error)
+            msg_box.exec()
+            return
 
-        """
+        preference_window = PreferencesWindow(self.global_config, self.dependency_manager, False)
+        ret = preference_window.exec()
         
-        for data_input in DataInputList().values():
-            if not os.path.exists(os.path.join(dir_path, self.global_config.get_default_dicom_folder(), data_input.name)):
-                return False
+        if ret == EXIT_CODE_REBOOT:
+            self.close()
+            QCoreApplication.exit(EXIT_CODE_REBOOT)
             
-        return True
+        if ret != 0:
+            self.reset_workflows()
 
-    def update_pt_dir(self, dir_path: str):
+    def edit_wf_config(self):
         """
-        Update an existing folder with the patient subfolder structure.
-
-        Parameters
-        ----------
-        dir_path : str
-            The directory path to update into a patient folder.
+        Open the Default Workflow Settings Window.
 
         Returns
         -------
         None.
 
         """
 
-        for data_input in DataInputList().values():
-            if not os.path.exists(
-                    os.path.join(dir_path, self.global_config.get_default_dicom_folder(), data_input.name)):
-                os.makedirs(os.path.join(dir_path, self.global_config.get_default_dicom_folder(), data_input.name),
-                            exist_ok=True)
-
-    def edit_config(self):
-        """
-        Open the Global Preferences Window.
-
-        Returns
-        -------
-        None.
-
-        """
-        
         if self.check_running_workflows():
             msg_box = QMessageBox()
             msg_box.setText(strings.mainwindow_pref_disabled_error)
             msg_box.exec()
             return
-        
-        preference_window = PreferencesWindow(self.global_config, self)
-        ret = preference_window.exec()
-        
-        if ret == EXIT_CODE_REBOOT:
-            self.close()
-            QCoreApplication.exit(EXIT_CODE_REBOOT)
-            
-        if ret != 0:
-            self.reset_workflows()
+
+        wf_preference_window = PreferencesWindow(self.global_config, self.dependency_manager, True)
+        ret = wf_preference_window.exec()
+
+        if ret == -1:
+            self.global_config.reset_to_defaults()
+            self.edit_wf_config()
 
     def check_running_workflows(self) -> bool:
         """
-        Check if SWANe is executing a workflow in any open Patients tab.
+        Check if SWANe is executing a workflow in any open subject tab.
 
         Returns
         -------
         bool
             True if SWANe is executing a workflow, otherwise False.
 
         """
         
-        for pt in self.pt_tabs_array:
-            if pt.is_workflow_process_alive():
+        for subj in self.subject_tab_array:
+            if subj.subject.is_workflow_process_alive():
                 return True
             
         return False
 
     def reset_workflows(self):
         """
         Reset all the generated workflows that are not already running.
 
         Returns
         -------
         None.
 
         """
         
-        for pt in self.pt_tabs_array:
-            pt.reset_workflow()
+        for subj in self.subject_tab_array:
+            subj.reset_workflow()
 
     def about(self):
         """
         Open the About Window.
 
         Returns
         -------
@@ -462,103 +438,101 @@
         self.resize(800, 600)
         self.setWindowTitle(strings.APPNAME + " - " + strings.app_acronym)
 
         self.statusBar().showMessage('')
 
         # Buttons definition
         button_action = QAction(QIcon.fromTheme(
-            "document-open"), strings.menu_load_pt, self)
-        button_action.setStatusTip(strings.menu_load_pt_tip)
-        button_action.triggered.connect(self.search_pt_dir)
+            "document-open"), strings.menu_load_subj, self)
+        button_action.setStatusTip(strings.menu_load_subj_tip)
+        button_action.triggered.connect(self.search_subject_dir)
 
         button_action2 = QAction(QIcon.fromTheme(
-            "document-new"), strings.menu_new_pt, self)
-        button_action2.setStatusTip(strings.menu_new_pt_tip)
-        button_action2.triggered.connect(self.choose_new_pt_dir)
+            "document-new"), strings.menu_new_subj, self)
+        button_action2.setStatusTip(strings.menu_new_subj_tip)
+        button_action2.triggered.connect(self.choose_new_subject_dir)
 
         button_action3 = QAction(QIcon.fromTheme(
             "application-exit"), strings.menu_exit, self)
         button_action3.triggered.connect(self.close)
 
         button_action4 = QAction(QIcon.fromTheme(
             "preferences-other"), strings.menu_pref, self)
         button_action4.setStatusTip(strings.menu_pref_tip)
         button_action4.triggered.connect(self.edit_config)
 
-        button_action6 = QAction(strings.menu_about, self)
-        button_action6.triggered.connect(self.about)
+        button_action5 = QAction(QIcon.fromTheme(
+            "preferences-other"), strings.menu_wf_pref, self)
+        button_action5.triggered.connect(self.edit_wf_config)
+
+        button_action7 = QAction(strings.menu_about, self)
+        button_action7.triggered.connect(self.about)
 
         # Menu definition and population
         menu = self.menuBar()
         menu.setNativeMenuBar(False)
         file_menu = menu.addMenu(strings.menu_file_name)
         file_menu.addAction(button_action)
         file_menu.addAction(button_action2)
         file_menu.addAction(button_action3)
         tool_menu = menu.addMenu(strings.menu_tools_name)
         tool_menu.addAction(button_action4)
-        if sys.platform != "darwin":
-            button_action5 = QAction(strings.menu_shortcut, self)
-            button_action5.triggered.connect(lambda checked=None, global_config=self.global_config: shortcut_manager(global_config))
-
-            tool_menu.addAction(button_action5)
+        tool_menu.addAction(button_action5)
         help_menu = menu.addMenu(strings.menu_help_name)
-        help_menu.addAction(button_action6)
+        help_menu.addAction(button_action7)
         
         # Tab definition
         self.main_tab = QTabWidget(parent=self)
         self.main_tab.setTabsClosable(True)
-        self.main_tab.tabCloseRequested.connect(self.close_pt)
+        self.main_tab.tabCloseRequested.connect(self.close_subject_tab)
         self.setCentralWidget(self.main_tab)
         self.homeTab = QWidget()
         self.main_tab.addTab(self.homeTab, strings.mainwindow_home_tab_name)
 
         # Tab closing option disabled
         self.main_tab.tabBar().setTabButton(0, QTabBar.ButtonPosition.LeftSide, None)
         self.main_tab.tabBar().setTabButton(0, QTabBar.ButtonPosition.RightSide, None)
         
         # Home Tab definition
         self.home_tab_ui()
         
-        self.pt_tabs_array = []
+        self.subject_tab_array = []
 
         self.show()
 
-    def close_pt(self, index: int):
+    def close_subject_tab(self, index: int):
         """
-        Handle the PySide tab closing event for the Patient tab.
+        Handle the PySide tab closing event for the subject tab.
 
         Parameters
         ----------
         index : int
-            The patient tab index into the GUI.
+            The subject tab index into the GUI.
 
         Returns
         -------
         None.
 
         """
         
         # Guard to prevent the Home Tab closing
         if index <= 0:
             return
 
         tab_item = self.main_tab.widget(index)
-        if tab_item.is_workflow_process_alive():
+        if tab_item.subject.is_workflow_process_alive():
             msg_box = QMessageBox()
             msg_box.setText(strings.mainwindow_wf_executing_error_1)
             msg_box.exec()
             return
 
-        tab_item.pt_config.save()
+        tab_item.subject.config.save()
         
-        self.pt_tabs_array.remove(tab_item)
+        self.subject_tab_array.remove(tab_item)
         self.main_tab.removeTab(index)
-        
-        tab_item = None
 
     def closeEvent(self, event: QCloseEvent):
         """
         Prevent the closing of a running workflow tab
 
         Parameters
         ----------
@@ -585,15 +559,15 @@
 
         Returns
         -------
         None.
 
         """
         
-        layout = QGridLayout()
+        self.home_grid_layout = QGridLayout()
 
         bold_font = QFont()
         bold_font.setBold(True)
         title_font = QFont()
         title_font.setBold(True)
         title_font.setPointSize(title_font.pointSize() * 1.5)
         x = 0
@@ -603,152 +577,139 @@
         label_welcome2 = QLabel(strings.mainwindow_home_label2)
         label_welcome2.setWordWrap(True)
         label_welcome3 = QLabel(strings.mainwindow_home_label3)
         label_welcome3.setWordWrap(True)
         label_welcome4 = QLabel(strings.mainwindow_home_label4)
         label_welcome4.setFont(bold_font)
 
-        layout.addWidget(label_welcome1, x, 0, 1, 2)
+        self.home_grid_layout.addWidget(label_welcome1, x, 0, 1, 2)
         x += 1
-        layout.addWidget(label_welcome2, x, 0, 1, 2)
+        self.home_grid_layout.addWidget(label_welcome2, x, 0, 1, 2)
         x += 1
-        layout.addWidget(label_welcome3, x, 0, 1, 2)
+        self.home_grid_layout.addWidget(label_welcome3, x, 0, 1, 2)
         x += 1
-        layout.addWidget(label_welcome4, x, 0, 1, 2)
+        self.home_grid_layout.addWidget(label_welcome4, x, 0, 1, 2)
         x += 1
 
         # Main window dependency check
         label_main_dep = QLabel(strings.mainwindow_home_label5)
         label_main_dep.setSizePolicy(QSizePolicy.Minimum, QSizePolicy.Minimum)
         label_main_dep.setFont(bold_font)
-        layout.addWidget(label_main_dep, x, 0, 1, 2)
+        self.home_grid_layout.addWidget(label_main_dep, x, 0, 1, 2)
         x += 1
 
-        msg, self.dcm2niix = check_dcm2niix()
-        x = self.add_home_entry(layout, msg, self.dcm2niix, x)
+        x = self.add_home_entry(self.dependency_manager.dcm2niix, x)
 
-        msg, self.fsl = check_fsl()
-        x = self.add_home_entry(layout, msg, self.fsl, x)
+        x = self.add_home_entry(self.dependency_manager.fsl, x)
 
         label_main_dep = QLabel(strings.mainwindow_home_label6)
         label_main_dep.setSizePolicy(QSizePolicy.Minimum, QSizePolicy.Minimum)
         label_main_dep.setFont(bold_font)
-        layout.addWidget(label_main_dep, x, 0, 1, 2)
+        self.home_grid_layout.addWidget(label_main_dep, x, 0, 1, 2)
         x += 1
 
-        msg, self.freesurfer = check_freesurfer()
-        x = self.add_home_entry(layout, msg, self.freesurfer[0], x)
+        x = self.add_home_entry(self.dependency_manager.freesurfer, x)
+        self.global_config.freesurfer = self.dependency_manager.is_freesurfer()
 
-        check_slicer = False
-        current_slicer_path = self.global_config.get_slicer_path()
-        if current_slicer_path == '':
-            check_slicer = True
-        elif current_slicer_path[0] == "*":
-            current_slicer_path = current_slicer_path[1:]
-            check_slicer = True
-
-        if not os.path.exists(current_slicer_path):
-            current_slicer_path = ''
-
-        if check_slicer:
-            self.slicerlabel_icon = QSvgWidget()
-            self.slicerlabel_icon.setFixedSize(25, 25)
-            self.slicerlabel_icon.load(self.LOADING_MOVIE_FILE)
-            layout.addWidget(self.slicerlabel_icon, x, 0)
-            self.slicerlabel = QLabel(strings.mainwindow_dep_slicer_src)
-            self.slicerlabel.setOpenExternalLinks(True)
-            self.slicerlabel.setSizePolicy(
-                QSizePolicy.Minimum, QSizePolicy.Minimum)
-            layout.addWidget(self.slicerlabel, x, 1)
-            x += 1
-
-            self.global_config.set_slicer_path('')
-            check_slicer_work = SlicerCheckWorker(current_slicer_path, parent=self)
-            check_slicer_work.signal.slicer.connect(self.slicer_row)
-            QThreadPool.globalInstance().start(check_slicer_work)
+        if DependencyManager.need_slicer_check(self.global_config):
+            self.slicer_x = x
+            x = self.add_home_entry(Dependence(DependenceStatus.CHECKING, strings.mainwindow_dep_slicer_src), x)
+            DependencyManager.check_slicer(self.global_config.get_slicer_path(), self.slicer_row)
         else:
-            self.add_home_entry(layout, strings.mainwindow_dep_slicer_found, True, x)
-        x += 1
+            label = strings.check_dep_slicer_found % self.global_config.get_slicer_version()
+            x = self.add_home_entry(Dependence(DependenceStatus.DETECTED, label), x)
 
         label_main_dep = QLabel(strings.mainwindow_home_label7)
         label_main_dep.setSizePolicy(QSizePolicy.Minimum, QSizePolicy.Minimum)
         label_main_dep.setFont(bold_font)
-        layout.addWidget(label_main_dep, x, 0, 1, 2)
+        self.home_grid_layout.addWidget(label_main_dep, x, 0, 1, 2)
         x += 1
 
-        msg, self.graphviz = check_graphviz()
-        x = self.add_home_entry(layout, msg, self.graphviz, x)
+        x = self.add_home_entry(self.dependency_manager.graphviz, x)
 
-        vertical_spacer = QSpacerItem(
-            20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
-        layout.addItem(vertical_spacer, x, 0, 1, 2)
+        vertical_spacer = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
+        self.home_grid_layout.addItem(vertical_spacer, x, 0, 1, 2)
 
-        self.homeTab.setLayout(layout)
+        self.homeTab.setLayout(self.home_grid_layout)
 
-    def add_home_entry(self, gridlayout: QGridLayout, msg: str, icon: bool, x: int) -> int:
+    def add_home_entry(self, dep: Dependence, x: int) -> int:
         """
         Generates a dependency check label, adding it to an existing layout
 
         Parameters
         ----------
-        gridlayout : QGridLayout
-            The layout to populate with the generated label.
-        msg : str
-            The label text.
-        icon : bool
-            The label check icon.
+        dep : Dependence
+            A Dependence object to be parsed.
         x : int
             The starting grid layout row index.
 
         Returns
         -------
         int
             The next grid layout row index.
 
         """
         
         label_icon = QLabel()
-        label_icon.setFixedSize(25, 25)
         label_icon.setScaledContents(True)
-        
-        if icon:
+
+        if dep.state == DependenceStatus.DETECTED:
             label_icon.setPixmap(self.OK_ICON)
+        elif dep.state == DependenceStatus.WARNING:
+            label_icon.setPixmap(self.WARNING_ICON)
+        elif dep.state == DependenceStatus.CHECKING:
+            label_icon = QSvgWidget()
+            label_icon.load(self.LOADING_MOVIE_FILE)
         else:
             label_icon.setPixmap(self.ERROR_ICON)
-            
-        gridlayout.addWidget(label_icon, x, 0)
-        label = QLabel(msg)
+
+        label_icon.setFixedSize(25, 25)
+
+        old_icon_layout = self.home_grid_layout.itemAtPosition(x, 0)
+        if old_icon_layout is not None:
+            old_icon_layout.widget().deleteLater()
+            self.home_grid_layout.removeItem(old_icon_layout)
+        self.home_grid_layout.addWidget(label_icon, x, 0)
+
+        label = QLabel(dep.label)
         label.setOpenExternalLinks(True)
         label.setSizePolicy(QSizePolicy.Minimum, QSizePolicy.Minimum)
-        gridlayout.addWidget(label, x, 1)
+
+        old_label_layout = self.home_grid_layout.itemAtPosition(x, 1)
+        if old_label_layout is not None:
+            old_label_layout.widget().deleteLater()
+            self.home_grid_layout.removeItem(old_label_layout)
+        self.home_grid_layout.addWidget(label, x, 1)
         
         return x + 1
 
-    def slicer_row(self, slicer_path: str, msg: str, found: bool):
+    def slicer_row(self, slicer_path: str, slicer_version: str, msg: str, state: DependenceStatus):
         """
         Generates the Slicer dependency check label and path, if 3D Slicer is found.
 
         Parameters
         ----------
         slicer_path : str
             The local 3D Slicer path.
+        slicer_version: str
+            The Slicer version found
         msg : str
             The label message.
-        found : bool
-            True if 3d Slicer has been found locally, otherwise False.
+        state: DependenceStatus
+            A state from DependenceStatus.
 
         Returns
         -------
         None.
 
         """
         
-        if found:
+        self.add_home_entry(Dependence(state, msg), self.slicer_x)
+
+        if state is DependenceStatus.DETECTED:
             self.global_config.set_slicer_path(slicer_path)
+            self.global_config.set_slicer_version(slicer_version)
             self.global_config.save()
-            self.slicerlabel_icon.load(self.OK_ICON_FILE)
-        else:
-            self.global_config.set_slicer_path('')
-            self.global_config.save()
-            self.slicerlabel_icon.load(self.ERROR_ICON_FILE)
-            
-        self.slicerlabel.setText(msg)
+
+        for tab in self.subject_tab_array:
+            tab.export_results_button_update_state()
+            tab.load_scene_button_update_state()
```

### Comparing `swane-0.0.6/swane/ui/PersistentProgressDialog.py` & `swane-0.1.0/swane/ui/PersistentProgressDialog.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,14 +14,18 @@
         self.setWindowModality(Qt.WindowModal)
         self.setMinimumDuration(0)
 
     def keyPressEvent(self, event):
         if event.key() != Qt.Key_Escape:
             super(PersistentProgressDialog, self).keyPressEvent(event)
 
-    def increase_value(self, x):
+    def increase_value(self, x, maximum=0):
+        if self.maximum() == 0 and maximum > 0:
+            self.setMaximum(maximum)
+        if not self.isVisible():
+            self.show()
         if self.value() == 0 and self.maximum() > 1:
             x = x+1
         self.setValue(self.value()+x)
 
     def closeEvent(self, event):
         event.ignore()
```

### Comparing `swane-0.0.6/swane/ui/PtTab.py` & `swane-0.1.0/swane/ui/SubjectTab.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,182 +1,176 @@
 import os
-import shutil
-import traceback
-from multiprocessing import Queue
-from threading import Thread
-
-import pydicom
 from PySide6.QtCore import Qt, QThreadPool, QFileSystemWatcher
 from PySide6.QtGui import QFont
 from PySide6.QtSvgWidgets import QSvgWidget
 from PySide6.QtWidgets import (QTabWidget, QWidget, QGridLayout, QLabel, QHeaderView,
-                               QPushButton, QSizePolicy, QHBoxLayout,
+                               QPushButton, QSizePolicy, QHBoxLayout, QSpacerItem,
                                QGroupBox, QVBoxLayout, QMessageBox, QListWidget,
                                QFileDialog, QTreeWidget, QErrorMessage, QFileSystemModel,
                                QTreeView, QComboBox)
 
 from swane import strings
-from swane.slicer.SlicerExportWorker import SlicerExportWorker
-from swane.nipype_pipeline.MainWorkflow import MainWorkflow
-from swane.ui.workers.WorkflowGeneratorWorker import WorkflowGeneratorWorker
-from swane.ui.workers.WorkflowMonitorWorker import WorkflowMonitorWorker
-from swane.ui.workers.WorkflowProcess import WorkflowProcess
+from swane.workers.SlicerExportWorker import SlicerExportWorker
+from swane.workers.SlicerViewerWorker import SlicerViewerWorker
 from swane.ui.CustomTreeWidgetItem import CustomTreeWidgetItem
 from swane.ui.PersistentProgressDialog import PersistentProgressDialog
 from swane.ui.PreferencesWindow import PreferencesWindow
 from swane.ui.VerticalScrollArea import VerticalScrollArea
-from swane.utils.ConfigManager import ConfigManager
-from swane.ui.workers.DicomSearchWorker import DicomSearchWorker
-from swane.nipype_pipeline.workflows.freesurfer_workflow import FS_DIR
-from swane.utils.DataInput import DataInput, DataInputList
-from swane.nipype_pipeline.engine.MonitoredMultiProcPlugin import MonitoredMultiProcPlugin
+from swane.config.ConfigManager import ConfigManager
+from swane.workers.DicomSearchWorker import DicomSearchWorker
+from swane.utils.DataInputList import DataInputList
+from swane.utils.DependencyManager import DependencyManager
+from swane.config.preference_list import WORKFLOW_TYPES
+from swane.nipype_pipeline.engine.WorkflowReport import WorkflowReport, WorkflowSignals
+from swane.utils.Subject import Subject, SubjectRet
+from swane.workers.open_results_directory import open_results_directory
 
 
-class PtTab(QTabWidget):
+class SubjectTab(QTabWidget):
     """
-    Custom implementation of PySide QTabWidget to define a patient tab widget.
+    Custom implementation of PySide QTabWidget to define a subject tab widget.
 
     """
     
     DATATAB = 0
     EXECTAB = 1
     RESULTTAB = 2
-    GRAPH_DIR_NAME = "graph"
-    GRAPH_FILE_PREFIX = "graph_"
-    GRAPH_FILE_EXT = "svg"
-    GRAPH_TYPE = "colored"
-    NODE_MSG_DIVIDER = '.'
 
-    def __init__(self, global_config, pt_folder, main_window, parent=None):
-        super(PtTab, self).__init__(parent)
+    def __init__(self, global_config: ConfigManager, subject: Subject, main_window, parent=None):
+        super(SubjectTab, self).__init__(parent)
         self.global_config = global_config
-        self.pt_folder = pt_folder
-        self.pt_name = os.path.basename(pt_folder)
+        self.subject = subject
         self.main_window = main_window
 
-        self.workflow = None
-        self.workflow_process = None
-        self.node_list = None
-
-        dicom_dir = os.path.join(self.pt_folder, self.global_config.get_default_dicom_folder())
-        self.data_input_list = DataInputList(dicom_dir)
-
         self.data_tab = QWidget()
         self.exec_tab = QWidget()
-        self.slicer_tab = QWidget()
+        self.result_tab = QWidget()
 
-        self.addTab(self.data_tab, strings.pttab_data_tab_name)
-        self.addTab(self.exec_tab, strings.pttab_wf_tab_name)
-        self.addTab(self.slicer_tab, strings.pttab_results_tab_name)
+        self.addTab(self.data_tab, strings.subj_tab_data_tab_name)
+        self.addTab(self.exec_tab, strings.subj_tab_wf_tab_name)
+        self.addTab(self.result_tab, strings.subj_tab_results_tab_name)
 
         self.directory_watcher = QFileSystemWatcher()
         self.directory_watcher.directoryChanged.connect(self.reset_workflow)
 
-        self.start_gen_wf_thread()
+        self.scan_directory_watcher = QFileSystemWatcher()
+        self.scan_directory_watcher.directoryChanged.connect(self.clear_scan_result)
 
-        self.data_tab_ui()
-        self.exec_tab_ui()
-        self.slicer_tab_ui()
-
-        self.setTabEnabled(PtTab.EXECTAB, False)
-        self.setTabEnabled(PtTab.RESULTTAB, False)
-
-    def set_main_window(self, main_window):
-        """
-        Set the Main Window.
+        self.result_directory_watcher = QFileSystemWatcher()
+        self.result_directory_watcher.directoryChanged.connect(self.enable_tab_if_result_dir)
+        self.result_directory_watcher.addPath(self.subject.folder)
 
-        Parameters
-        ----------
-        main_window : MainWindow
-            The Main Window.
+        self.workflow_process = None
+        self.node_list = None
+        self.input_report = {}
+        self.dicom_scan_series_list = []
+        self.importable_series_list = QListWidget()
+        self.workflow_type_combo = None
+        self.generate_workflow_button = None
+        self.node_list_treeWidget = None
+        self.subject_config_button = None
+        self.exec_button = None
+        self.exec_graph = None
+        self.load_scene_button = None
+        self.open_results_directory_button = None
+        self.results_model = None
+        self.result_tree = None
+        self.generate_scene_button = None
 
-        Returns
-        -------
-        None.
+        self.data_tab_ui()
+        self.exec_tab_ui()
+        self.result_tab_ui()
 
-        """
-        
-        self.main_window = main_window
+        self.setTabEnabled(SubjectTab.EXECTAB, False)
+        self.setTabEnabled(SubjectTab.RESULTTAB, False)
 
-    def update_node_list(self, msg: str):
+    def update_node_list(self, wf_report: WorkflowReport):
         """
-        Searches for the node linked to the msg arg.
-        Uses the parsed msng arg to update the node status.
+        Searches for the node linked to the wf_report arg.
+        Uses the wf_report arg to update the node status.
 
         Parameters
         ----------
-        msg : str
+        wf_report : WorkflowReport
             Workflow Monitor Worker message to parse.
 
         Returns
         -------
         None.
 
         """
         
-        if msg == WorkflowMonitorWorker.STOP:
+        if wf_report.signal_type == WorkflowSignals.WORKFLOW_STOP:
+            self.enable_tab_if_result_dir(on_workflow_running=True)
             errors = False
             for key in self.node_list.keys():
                 self.node_list[key].node_holder.setExpanded(False)
                 if not self.node_list[key].node_holder.completed:
                     errors = True
                     for subkey in self.node_list[key].node_list.keys():
                         if self.node_list[key].node_list[subkey].node_holder.art == self.main_window.ERROR_ICON_FILE:
                             self.node_list[key].node_holder.set_art(self.main_window.ERROR_ICON_FILE)
                             break
 
-            self.setTabEnabled(PtTab.DATATAB, True)
-            
+            self.setTabEnabled(SubjectTab.DATATAB, True)
+
+            self.exec_button_set_enabled(False)
+
             if errors:
-                self.exec_button.setText(strings.pttab_wf_executed_with_error)
-                self.node_button.setEnabled(True)
+                self.generate_workflow_button.setEnabled(True)
+                self.subject.workflow = None
+                self.exec_button.setText(strings.subj_tab_wf_executed_with_error)
+                self.exec_button.setToolTip("")
             else:
-                self.exec_button.setText(strings.pttab_wf_executed)
-                
-            self.exec_button.setEnabled(False)
-            self.enable_tab_if_result_dir()
+                self.exec_button.setText(strings.subj_tab_wf_executed)
+                self.exec_button.setToolTip("")
+
+
             
             return
+        elif wf_report.signal_type == WorkflowSignals.INVALID_SIGNAL:
+            # Invalid signal sent from WF to UI, code error intercept
+            try:
+                self.workflow_process.stop_event.set()
+            except:
+                pass
+            msg_box = QMessageBox()
+            msg_box.setText(strings.subj_tab_wf_invalid_signal)
+            msg_box.exec()
 
         # TODO - To be implemented for RAM usage info by each workflow
         # if msg == WorkflowProcess.WORKFLOW_INSUFFICIENT_RESOURCES:
         #     msg_box = QMessageBox()
         #     msg_box.setText(strings.pttab_wf_insufficient_resources)
         #     msg_box.exec()
 
-        split = msg.split(PtTab.NODE_MSG_DIVIDER)
-
-        # For every message starts by "nipype_pt_x.", remove the prefix
-        split.pop(0)
-
-        # Remaining message must be like: workflow_name.node_name.message_type
-        if len(split) < 3:
-            return
-
-        if split[2] == MonitoredMultiProcPlugin.NODE_STARTED:
+        if wf_report.signal_type == WorkflowSignals.NODE_STARTED:
             icon = self.main_window.LOADING_MOVIE_FILE
-        elif split[2] == MonitoredMultiProcPlugin.NODE_COMPLETED:
+        elif wf_report.signal_type == WorkflowSignals.NODE_COMPLETED:
             icon = self.main_window.OK_ICON_FILE
         else:
             icon = self.main_window.ERROR_ICON_FILE
 
-        self.node_list[split[0]].node_list[split[1]].node_holder.set_art(icon)
+        self.node_list[wf_report.workflow_name].node_list[wf_report.node_name].node_holder.set_art(icon)
 
-        self.node_list[split[0]].node_holder.setExpanded(True)
+        if wf_report.info is not None:
+            self.node_list[wf_report.workflow_name].node_list[wf_report.node_name].node_holder.setToolTip(0, wf_report.info)
+
+        self.node_list[wf_report.workflow_name].node_holder.setExpanded(True)
 
         if icon == self.main_window.OK_ICON_FILE:
             completed = True
-            for key in self.node_list[split[0]].node_list.keys():
-                if self.node_list[split[0]].node_list[key].node_holder.art != self.main_window.OK_ICON_FILE:
+            for key in self.node_list[wf_report.workflow_name].node_list.keys():
+                if self.node_list[wf_report.workflow_name].node_list[key].node_holder.art != self.main_window.OK_ICON_FILE:
                     completed = False
                     break
             if completed:
-                self.node_list[split[0]].node_holder.set_art(self.main_window.OK_ICON_FILE)
-                self.node_list[split[0]].node_holder.setExpanded(False)
-                self.node_list[split[0]].node_holder.completed = True
+                self.node_list[wf_report.workflow_name].node_holder.set_art(self.main_window.OK_ICON_FILE)
+                self.node_list[wf_report.workflow_name].node_holder.setExpanded(False)
+                self.node_list[wf_report.workflow_name].node_holder.completed = True
 
     def remove_running_icon(self):
         """
         Remove all the loading icons from the series labels.
 
         Returns
         -------
@@ -185,60 +179,14 @@
         """
         
         for key1 in self.node_list.keys():
             for key2 in self.node_list[key1].node_list.keys():
                 if self.node_list[key1].node_list[key2].node_holder.art == self.main_window.LOADING_MOVIE_FILE:
                     self.node_list[key1].node_list[key2].node_holder.set_art(self.main_window.VOID_SVG_FILE)
 
-    def start_gen_wf_thread(self):
-        """
-        Generates the workflow object in its thread during the patient loading.
-        The first workflow generation can be heavy because SWANe needs to load nypipe modules.
-        If repeated, the operation is faster and therefore executed in the main thread.
-
-        Returns
-        -------
-        None.
-
-        """
-        
-        if not self.main_window.fsl:
-            return
-        
-        workflow_generator_work = WorkflowGeneratorWorker(self.pt_folder)
-        workflow_generator_work.signal.workflow.connect(self.set_wf)
-        QThreadPool.globalInstance().start(workflow_generator_work)
-
-    def set_wf(self, wf: MainWorkflow):
-        """
-        Saves the specified workflow into Main Thread and updates the UI.
-
-        Parameters
-        ----------
-        wf : MainWorkflow
-            The workflow passed to the Main Thread.
-
-        Returns
-        -------
-        None.
-
-        """
-        
-        self.workflow = wf
-
-        try:
-            self.node_button.setEnabled(True)
-            self.wf_type_combo.setEnabled(True)
-            self.pt_config_button.setEnabled(True)
-
-            self.enable_exec_tab()
-
-        except AttributeError:
-            pass
-
     def data_tab_ui(self):
         """
         Generates the Data tab UI.
 
         Returns
         -------
         None.
@@ -253,167 +201,169 @@
         folder_layout = QGridLayout()
         scroll_area.m_scrollAreaWidgetContents.setLayout(folder_layout)
 
         bold_font = QFont()
         bold_font.setBold(True)
         x = 0
 
-        self.input_report = {}
-
-        remove_list = []
-
-        for data_input in self.data_input_list.values():
-
-            if data_input.optional and not self.global_config.is_optional_series_enabled(data_input.name):
-                remove_list.append(data_input.name)
-                continue
-
-            self.input_report[data_input.name] = [QSvgWidget(self),
-                                             QLabel(data_input.label),
+        for data_input in self.subject.input_state_list:
+            self.input_report[data_input] = [QSvgWidget(self),
+                                             QLabel(data_input.value.label),
                                              QLabel(""),
-                                             QPushButton(strings.pttab_import_button),
-                                             QPushButton(strings.pttab_clear_button)]
-            self.input_report[data_input.name][0].load(self.main_window.ERROR_ICON_FILE)
-            self.input_report[data_input.name][0].setFixedSize(25, 25)
-            if data_input.tooltip != "":
+                                             QPushButton(strings.subj_tab_import_button),
+                                             QPushButton(strings.subj_tab_clear_button),
+                                             None]
+            self.set_error(data_input, "")
+            if data_input.value.tooltip != "":
                 # Add tooltips and append ⓘ character to label
-                self.input_report[data_input.name][1].setText(data_input.label+" \u24D8")
-                self.input_report[data_input.name][1].setToolTip(data_input.tooltip)
-            self.input_report[data_input.name][1].setFont(bold_font)
-            self.input_report[data_input.name][1].setAlignment(Qt.AlignLeft | Qt.AlignBottom)
-            self.input_report[data_input.name][2].setAlignment(Qt.AlignLeft | Qt.AlignTop)
-            self.input_report[data_input.name][2].setStyleSheet("margin-bottom: 20px")
-            self.input_report[data_input.name][3].setEnabled(False)
-            self.input_report[data_input.name][3].clicked.connect(
-                lambda checked=None, z=data_input.name: self.dicom_import_to_folder(z))
-            self.input_report[data_input.name][3].setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Fixed)
-            self.input_report[data_input.name][4].setEnabled(False)
-            self.input_report[data_input.name][4].clicked.connect(
-                lambda checked=None, z=data_input.name: self.clear_import_folder(z))
-            self.input_report[data_input.name][4].setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Fixed)
+                self.input_report[data_input][1].setText(data_input.value.label+" "+strings.INFOCHAR)
+                self.input_report[data_input][1].setToolTip(data_input.value.tooltip)
+            self.input_report[data_input][1].setFont(bold_font)
+            self.input_report[data_input][1].setAlignment(Qt.AlignLeft | Qt.AlignBottom)
+            self.input_report[data_input][2].setAlignment(Qt.AlignLeft | Qt.AlignTop)
+            self.input_report[data_input][2].setStyleSheet("margin-bottom: 20px")
+            self.input_report[data_input][3].clicked.connect(
+                lambda checked=None, z=data_input: self.dicom_import_to_folder(z))
+            self.input_report[data_input][3].setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Fixed)
+            self.input_report[data_input][4].clicked.connect(
+                lambda checked=None, z=data_input: self.clear_import_folder(z))
+            self.input_report[data_input][4].setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Fixed)
 
-            folder_layout.addWidget(self.input_report[data_input.name][0], (x * 2), 0, 2, 1)
-            folder_layout.addWidget(self.input_report[data_input.name][1], (x * 2), 1)
+            folder_layout.addWidget(self.input_report[data_input][0], (x * 2), 0, 2, 1)
+            folder_layout.addWidget(self.input_report[data_input][1], (x * 2), 1)
 
-            folder_layout.addWidget(self.input_report[data_input.name][3], (x * 2), 2)
-            folder_layout.addWidget(self.input_report[data_input.name][4], (x * 2), 3)
+            folder_layout.addWidget(self.input_report[data_input][3], (x * 2), 2)
+            folder_layout.addWidget(self.input_report[data_input][4], (x * 2), 3)
 
-            folder_layout.addWidget(self.input_report[data_input.name][2], (x * 2) + 1, 1, 1, 3)
+            folder_layout.addWidget(self.input_report[data_input][2], (x * 2) + 1, 1, 1, 3)
             x += 1
 
-        for to_remove in remove_list:
-            self.data_input_list.pop(to_remove)
-
         # Second Column: Series to be imported
         import_group_box = QGroupBox()
         import_layout = QVBoxLayout()
         import_group_box.setLayout(import_layout)
 
-        scan_dicom_folder_button = QPushButton(strings.pttab_scan_dicom_button)
+        scan_dicom_folder_button = QPushButton(strings.subj_tab_scan_dicom_button)
         scan_dicom_folder_button.clicked.connect(self.scan_dicom_folder)
 
-        self.importable_series_list = QListWidget()
         import_layout.addWidget(scan_dicom_folder_button)
         import_layout.addWidget(self.importable_series_list)
 
         # Adding data_input columns to Main Layout
         layout.addWidget(scroll_area, stretch=1)
         layout.addWidget(import_group_box, stretch=1)
         self.data_tab.setLayout(layout)
 
-    def dicom_import_to_folder(self, input_name: str):
+    def dicom_import_to_folder(self, data_input: DataInputList, force_mod: bool = False):
         """
-        Copies the files inside the selected folder in the input list into the folder specified by input_name var.
+        Copies the files inside the selected folder in the input list into the folder specified by data_input var.
 
         Parameters
         ----------
-        input_name : str
+        data_input: DataInputList
             The name of the series to which couple the selected file.
+        force_mod: bool
+            Skip the modality check. Default is False
 
         Returns
         -------
         None.
 
         """
         
         if self.importable_series_list.currentRow() == -1:
             msg_box = QMessageBox()
-            msg_box.setText(strings.pttab_selected_series_error)
+            msg_box.setText(strings.subj_tab_selected_series_error)
             msg_box.exec()
             return
 
-        import shutil
-        dest_path = os.path.join(self.pt_folder,
-                                 self.global_config.get_default_dicom_folder(), input_name)
-        found_mod = self.final_series_list[self.importable_series_list.currentRow()][0].split("-")[1].upper()
-
-        if not self.data_input_list[input_name].is_image_modality(found_mod):
-            msg_box = QMessageBox()
-            msg_box.setText(strings.pttab_wrong_type_check_msg % (found_mod, self.data_input_list[input_name].image_modality))
-            msg_box.setText(strings.pttab_wrong_type_check)
-            msg_box.setIcon(QMessageBox.Icon.Warning)
-            msg_box.setStandardButtons(QMessageBox.StandardButton.Yes | QMessageBox.StandardButton.No)
-            msg_box.setDefaultButton(QMessageBox.StandardButton.No)
-            ret = msg_box.exec()
-            
-            if ret == QMessageBox.StandardButton.No:
-                return
-
-        copy_list = self.final_series_list[self.importable_series_list.currentRow()][1]
-
-        progress = PersistentProgressDialog(strings.pttab_dicom_copy, 0, len(copy_list) + 1, self)
-        progress.show()
-
-        self.input_report[input_name][0].load(self.main_window.LOADING_MOVIE_FILE)
-
-        for thisFile in copy_list:
-            if not os.path.isfile(thisFile):
-                continue
-            
-            shutil.copy(thisFile, dest_path)
-            progress.increase_value(1)
+        copy_list = self.dicom_scan_series_list[self.importable_series_list.currentRow()][1]
+        vols = self.dicom_scan_series_list[self.importable_series_list.currentRow()][3]
+        found_mod = self.dicom_scan_series_list[self.importable_series_list.currentRow()][2].upper()
+
+        progress = PersistentProgressDialog(strings.subj_tab_dicom_copy, 0, len(copy_list) + 1, self)
+        self.set_loading(data_input)
+
+        # Copy files and check for return
+        import_ret = self.subject.dicom_import_to_folder(data_input=data_input,
+                                                         copy_list=copy_list,
+                                                         vols=vols,
+                                                         mod=found_mod,
+                                                         force_modality=force_mod,
+                                                         progress_callback=progress.increase_value
+                                                         )
+        if import_ret != SubjectRet.DataImportCompleted:
+            if import_ret == SubjectRet.DataImportErrorVolumesMax:
+                msg_box = QMessageBox()
+                msg_box.setText(strings.subj_tab_wrong_max_vols_check_msg % (vols, data_input.value.max_volumes))
+                msg_box.exec()
+            elif import_ret == SubjectRet.DataInputNonEmpty:
+                msg_box = QMessageBox()
+                msg_box.setText(strings.subj_tab_import_folder_not_empy)
+                msg_box.exec()
+            elif import_ret == SubjectRet.DataImportErrorVolumesMin:
+                msg_box = QMessageBox()
+                msg_box.setText(strings.subj_tab_wrong_min_vols_check_msg % (vols, data_input.value.min_volumes))
+                msg_box.exec()
+            elif import_ret == SubjectRet.DataImportErrorCopy:
+                msg_box = QMessageBox()
+                msg_box.setText(strings.subj_tab_import_copy_error_msg)
+                msg_box.exec()
+            elif import_ret == SubjectRet.DataImportErrorModality:
+                msg_box = QMessageBox()
+                msg_box.setText(strings.subj_tab_wrong_type_check_msg % (found_mod, data_input.value.image_modality.value))
+                msg_box.setInformativeText(strings.subj_tab_wrong_type_check)
+                msg_box.setIcon(QMessageBox.Icon.Warning)
+                msg_box.setStandardButtons(QMessageBox.StandardButton.Yes | QMessageBox.StandardButton.No)
+                msg_box.setDefaultButton(QMessageBox.StandardButton.No)
+                ret = msg_box.exec()
+                if ret == QMessageBox.StandardButton.Yes:
+                    self.dicom_import_to_folder(data_input, force_mod=True)
+            self.set_error(data_input, "")
+            progress.deleteLater()
+            return
 
         progress.setRange(0, 0)
-        progress.setLabelText(strings.pttab_dicom_check)
+        progress.setLabelText(strings.subj_tab_dicom_check)
 
-        self.check_input_folder(input_name, progress)
+        self.subject.check_input_folder(data_input, status_callback=self.input_check_update, progress_callback=progress.increase_value)
         self.reset_workflow()
 
     def scan_dicom_folder(self):
         """
         Opens a folder dialog window to select the DICOM files folder to import.
         Scans the folder in a new thread.
 
         Returns
         -------
         None.
 
         """
         
-        folder_path = QFileDialog.getExistingDirectory(self, strings.pttab_select_dicom_folder)
+        folder_path = QFileDialog.getExistingDirectory(self, strings.subj_tab_select_dicom_folder)
         
         if not os.path.exists(folder_path):
             return
 
         dicom_src_work = DicomSearchWorker(folder_path)
         dicom_src_work.load_dir()
 
         if dicom_src_work.get_files_len() > 0:
-            self.importable_series_list.clear()
-            self.final_series_list = []
-            progress = PersistentProgressDialog(strings.pttab_dicom_scan, 0, 0, parent=self.parent())
+            self.clear_scan_result()
+            self.dicom_scan_series_list = []
+            progress = PersistentProgressDialog(strings.subj_tab_dicom_scan, 0, 0, parent=self.parent())
             progress.show()
             progress.setMaximum(dicom_src_work.get_files_len())
             dicom_src_work.signal.sig_loop.connect(lambda i: progress.increase_value(i))
             dicom_src_work.signal.sig_finish.connect(self.show_scan_result)
             QThreadPool.globalInstance().start(dicom_src_work)
 
         else:
             msg_box = QMessageBox()
-            msg_box.setText(strings.pttab_no_dicom_error + folder_path)
+            msg_box.setText(strings.subj_tab_no_dicom_error + folder_path)
             msg_box.exec()
 
     def exec_tab_ui(self):
         """
         Generates the Execute Workflow tab UI.
 
         Returns
@@ -421,27 +371,27 @@
         None.
 
         """
         
         layout = QGridLayout()
 
         # First Column: NODE LIST
-        self.wf_type_combo = QComboBox(self)
+        self.workflow_type_combo = QComboBox(self)
 
-        for index, label in enumerate(ConfigManager.WORKFLOW_TYPES):
-            self.wf_type_combo.insertItem(index, label)
+        for row in WORKFLOW_TYPES:
+            self.workflow_type_combo.addItem(row.value, userData=row.name)
 
-        layout.addWidget(self.wf_type_combo, 0, 0)
+        layout.addWidget(self.workflow_type_combo, 0, 0)
 
-        self.node_button = QPushButton(strings.GENBUTTONTEXT)
-        self.node_button.clicked.connect(self.gen_wf)
-        if self.workflow is None:
-            self.node_button.setEnabled(False)
+        self.generate_workflow_button = QPushButton(strings.GENBUTTONTEXT)
+        self.generate_workflow_button.setFixedHeight(self.main_window.NON_UNICODE_BUTTON_HEIGHT)
+        self.generate_workflow_button.setSizePolicy(QSizePolicy.Minimum, QSizePolicy.Fixed)
+        self.generate_workflow_button.clicked.connect(self.generate_workflow)
 
-        layout.addWidget(self.node_button, 1, 0)
+        layout.addWidget(self.generate_workflow_button, 1, 0)
 
         self.node_list_treeWidget = QTreeWidget()
         self.node_list_treeWidget.setHeaderHidden(True)
         node_list_width = 320
         self.node_list_treeWidget.setFixedWidth(node_list_width)
         self.node_list_treeWidget.header().setMinimumSectionSize(node_list_width)
         self.node_list_treeWidget.header().setSectionResizeMode(QHeaderView.ResizeToContents)
@@ -449,42 +399,49 @@
         self.node_list_treeWidget.setHorizontalScrollBarPolicy(Qt.ScrollBarAsNeeded)
         self.node_list_treeWidget.horizontalScrollBar().setEnabled(True)
 
         layout.addWidget(self.node_list_treeWidget, 2, 0)
         self.node_list_treeWidget.itemClicked.connect(self.tree_item_clicked)
 
         # Second Column: Graphviz Graph Layout
-        self.pt_config_button = QPushButton(strings.PTCONFIGBUTTONTEXT)
-        self.pt_config_button.clicked.connect(self.edit_pt_config)
-        layout.addWidget(self.pt_config_button, 0, 1)
+        self.subject_config_button = QPushButton(strings.SUBJCONFIGBUTTONTEXT)
+        self.subject_config_button.setFixedHeight(self.main_window.NON_UNICODE_BUTTON_HEIGHT)
+        self.subject_config_button.setSizePolicy(QSizePolicy.Minimum, QSizePolicy.Fixed)
+        self.subject_config_button.clicked.connect(self.edit_subject_config)
+        layout.addWidget(self.subject_config_button, 0, 1)
 
         self.exec_button = QPushButton(strings.EXECBUTTONTEXT)
-        self.exec_button.clicked.connect(self.start_workflow_thread)
-        self.exec_button.setEnabled(False)
+        self.exec_button.setFixedHeight(self.main_window.NON_UNICODE_BUTTON_HEIGHT)
+        self.exec_button.setSizePolicy(QSizePolicy.Minimum, QSizePolicy.Fixed)
+        self.exec_button.clicked.connect(self.toggle_workflow_execution)
+        self.exec_button_set_enabled(False)
 
         layout.addWidget(self.exec_button, 1, 1)
         self.exec_graph = QSvgWidget()
         layout.addWidget(self.exec_graph, 2, 1)
 
         self.exec_tab.setLayout(layout)
 
-    def edit_pt_config(self):
+    def edit_subject_config(self):
         """
-        Opens the Patient Preference Window.
+        Opens the subject Preference Window.
 
         Returns
         -------
         None.
 
         """
-        
-        preference_window = PreferencesWindow(self.pt_config, self.data_input_list, self)
+
+        preference_window = PreferencesWindow(self.subject.config, self.subject.dependency_manager, True, self)
         ret = preference_window.exec()
         if ret != 0:
             self.reset_workflow()
+        if ret == -1:
+            self.subject.config.reset_to_defaults()
+            self.edit_subject_config()
 
     def on_wf_type_changed(self, index: int):
         """
         Updates the workflow at workflow type combo change.
 
         Parameters
         ----------
@@ -492,76 +449,56 @@
             The new selected value from the Execution tab workflow type combo.
 
         Returns
         -------
         None.
 
         """
-        
-        self.pt_config.set_wf_option(index)
-        self.pt_config.save()
+
+        new_workflow_type = self.workflow_type_combo.itemData(index)
+        self.subject.config.set_workflow_option(WORKFLOW_TYPES[new_workflow_type])
+        self.subject.config.save()
         self.reset_workflow()
 
-    def gen_wf(self):
+    def generate_workflow(self):
         """
         Generates and populates the Main Workflow.
         Shows the node list into the UI.
         Generates the graphviz analysis graphs on a new thread.
 
         Returns
         -------
         None.
 
         """
         
-        if not self.main_window.fsl:
+        generate_workflow_return = self.subject.generate_workflow()
+        
+        if generate_workflow_return == SubjectRet.GenWfMissingRequisites:
             error_dialog = QErrorMessage(parent=self)
-            error_dialog.showMessage(strings.pttab_missing_fsl_error)
+            error_dialog.showMessage(strings.subj_tab_missing_fsl_error)
             return
-
-        # Main Workflow generation
-        if self.workflow is None:
-            self.workflow = MainWorkflow(name=self.pt_name + WorkflowGeneratorWorker.WF_DIR_SUFFIX, base_dir=self.pt_folder)
-        
-        # Node List population
-        try:
-            self.workflow.add_input_folders(self.global_config, self.pt_config, self.data_input_list)
-        except:
+        elif generate_workflow_return == SubjectRet.GenWfError:
             error_dialog = QErrorMessage(parent=self)
-            error_dialog.showMessage(strings.pttab_wf_gen_error)
-            traceback.print_exc()
-            # TODO: generiamo un file crash nella cartella log?
+            error_dialog.showMessage(strings.subj_tab_wf_gen_error)
             return
         
-        self.node_list = self.workflow.get_node_array()
         self.node_list_treeWidget.clear()
-
-        graph_dir = os.path.join(self.pt_folder, PtTab.GRAPH_DIR_NAME)
-        shutil.rmtree(graph_dir, ignore_errors=True)
-        os.mkdir(graph_dir)
+        self.node_list = self.subject.workflow.get_node_array()
         
         # Graphviz analysis graphs drawing
         for node in self.node_list.keys():
             self.node_list[node].node_holder = CustomTreeWidgetItem(self.node_list_treeWidget, self.node_list_treeWidget, self.node_list[node].long_name)
-            if len(self.node_list[node].node_list.keys()) > 0:
-                if self.main_window.graphviz:
-                    graph_name = self.node_list[node].long_name.lower().replace(" ", "_")
-                    thread = Thread(target=self.workflow.get_node(node).write_graph,
-                                    kwargs={'graph2use': self.GRAPH_TYPE, 'format': PtTab.GRAPH_FILE_EXT,
-                                            'dotfilename': os.path.join(graph_dir,
-                                                                        PtTab.GRAPH_FILE_PREFIX + graph_name + '.dot')})
-                    thread.start()
-                    
+            if len(self.node_list[node].node_list.keys()) > 0:                    
                 for sub_node in self.node_list[node].node_list.keys():
                     self.node_list[node].node_list[sub_node].node_holder = CustomTreeWidgetItem(self.node_list[node].node_holder, self.node_list_treeWidget, self.node_list[node].node_list[sub_node].long_name)
         
         # UI updating
-        self.exec_button.setEnabled(True)
-        self.exec_button.setText(strings.EXECBUTTONTEXT)
-        self.node_button.setEnabled(False)
+        self.exec_button_set_enabled(True)
+        self.generate_workflow_button.setEnabled(False)
 
     def tree_item_clicked(self, item, col: int):
         """
         Listener for the QTreeWidget Items.
         Shows the clicked analysis graphviz graph.
 
         Parameters
@@ -573,19 +510,19 @@
 
         Returns
         -------
         None.
 
         """
         
-        if self.main_window.graphviz and item.parent() is None:
-            file = os.path.join(self.pt_folder, PtTab.GRAPH_DIR_NAME, PtTab.GRAPH_FILE_PREFIX + item.get_text().lower().replace(" ", "_") + '.'
-                                + PtTab.GRAPH_FILE_EXT)
-            self.exec_graph.load(file)
-            self.exec_graph.renderer().setAspectRatioMode(Qt.AspectRatioMode.KeepAspectRatio)
+        if item.parent() is None:
+            graph_file = self.subject.graph_file(item.get_text())
+            if os.path.exists(graph_file):
+                self.exec_graph.load(graph_file)
+                self.exec_graph.renderer().setAspectRatioMode(Qt.AspectRatioMode.KeepAspectRatio)
 
     @staticmethod
     def no_close_event(event):
         """
         Used to prevent the user to close a dialog.
 
         Parameters
@@ -597,171 +534,187 @@
         -------
         None.
 
         """
         
         event.ignore()
 
-    def is_workflow_process_alive(self) -> bool:
-        """
-        Checks if a workflow is in execution.
-
-        Returns
-        -------
-        bool
-            True if the workflow is executing, elsewise False.
-
-        """
-        
-        try:
-            if self.workflow_process is None:
-                return False
-            
-            return self.workflow_process.is_alive()
-        
-        except AttributeError:
-            return False
-
-    def start_workflow_thread(self):
+    def toggle_workflow_execution(self, resume: bool = None, resume_freesurfer: bool = None):
         """
         If the workflow is not started, executes it.
         If the workflow is executing, kills it.
 
         Returns
         -------
         None.
 
         """
         
         # Workflow not started
-        if not self.is_workflow_process_alive():
-            workflow_dir = os.path.join(self.pt_folder, self.pt_name + WorkflowGeneratorWorker.WF_DIR_SUFFIX)
-            # Checks for a previous workflow execution
-            if os.path.exists(workflow_dir):
-                # If yes, asks for workflow resume or reset
+        if not self.subject.is_workflow_process_alive():
+            workflow_start_ret = self.subject.start_workflow(resume=resume, resume_freesurfer=resume_freesurfer, update_node_callback=self.update_node_list)
+            if workflow_start_ret == SubjectRet.ExecWfResume:
                 msg_box = QMessageBox()
-                msg_box.setText(strings.pttab_old_wf_found)
+                msg_box.setText(strings.subj_tab_old_wf_found)
                 msg_box.setIcon(QMessageBox.Icon.Question)
                 msg_box.setStandardButtons(QMessageBox.StandardButton.Yes | QMessageBox.StandardButton.No)
-                msg_box.button(QMessageBox.StandardButton.Yes).setText(strings.pttab_old_wf_resume)
-                msg_box.button(QMessageBox.StandardButton.No).setText(strings.pttab_old_wf_reset)
+                msg_box.button(QMessageBox.StandardButton.Yes).setText(strings.subj_tab_old_wf_resume)
+                msg_box.button(QMessageBox.StandardButton.No).setText(strings.subj_tab_old_wf_reset)
                 msg_box.setDefaultButton(QMessageBox.StandardButton.Yes)
                 msg_box.setWindowFlags(Qt.CustomizeWindowHint | Qt.WindowTitleHint)
                 msg_box.closeEvent = self.no_close_event
                 ret = msg_box.exec()
-                
-                if ret == QMessageBox.StandardButton.No:
-                    shutil.rmtree(workflow_dir, ignore_errors=True)
-
-            fsdir = os.path.join(self.pt_folder, FS_DIR)
-            # Checks for a previous workflow FreeSurfer execution
-            if self.pt_config.get_pt_wf_freesurfer() and os.path.exists(fsdir):
-                # If yes, asks for workflow resume or reset
+                resume = ret == QMessageBox.StandardButton.Yes
+                self.toggle_workflow_execution(resume=resume, resume_freesurfer=resume_freesurfer)
+            elif workflow_start_ret == SubjectRet.ExecWfResumeFreesurfer:
                 msg_box = QMessageBox()
-                msg_box.setText(strings.pttab_old_fs_found)
+                msg_box.setText(strings.subj_tab_old_fs_found)
                 msg_box.setIcon(QMessageBox.Icon.Question)
                 msg_box.setStandardButtons(QMessageBox.StandardButton.Yes | QMessageBox.StandardButton.No)
-                msg_box.button(QMessageBox.StandardButton.Yes).setText(strings.pttab_old_fs_resume)
-                msg_box.button(QMessageBox.StandardButton.No).setText(strings.pttab_old_fs_reset)
+                msg_box.button(QMessageBox.StandardButton.Yes).setText(strings.subj_tab_old_fs_resume)
+                msg_box.button(QMessageBox.StandardButton.No).setText(strings.subj_tab_old_fs_reset)
                 msg_box.setDefaultButton(QMessageBox.StandardButton.Yes)
                 msg_box.setWindowFlags(Qt.CustomizeWindowHint | Qt.WindowTitleHint)
                 msg_box.closeEvent = self.no_close_event
                 ret = msg_box.exec()
-                
-                if ret == QMessageBox.StandardButton.No:
-                    shutil.rmtree(fsdir, ignore_errors=True)
-
-            queue = Queue(maxsize=500)
-            
-            # Generates a Monitor Worker to receive workflows notifications
-            workflow_monitor_work = WorkflowMonitorWorker(queue)
-            workflow_monitor_work.signal.log_msg.connect(self.update_node_list)
-            QThreadPool.globalInstance().start(workflow_monitor_work)
-            
-            # Starts the workflow on a new process
-            self.workflow_process = WorkflowProcess(self.pt_name, self.workflow, queue)
-            self.workflow_process.start()
-            
-            # UI updating
-            self.exec_button.setText(strings.EXECBUTTONTEXT_STOP)
-            self.setTabEnabled(PtTab.DATATAB, False)
-            self.setTabEnabled(PtTab.RESULTTAB, False)
-            self.wf_type_combo.setEnabled(False)
-            self.pt_config_button.setEnabled(False)
+                resume_freesurfer = ret == QMessageBox.StandardButton.Yes
+                self.toggle_workflow_execution(resume=resume, resume_freesurfer=resume_freesurfer)
+            elif workflow_start_ret == SubjectRet.ExecWfStatusError:
+                # Already running, should not be possible
+                pass
+            else:
+                # UI updating
+                self.exec_button.setText(strings.EXECBUTTONTEXT_STOP)
+                self.setTabEnabled(SubjectTab.DATATAB, False)
+                self.setTabEnabled(SubjectTab.RESULTTAB, False)
+                self.workflow_type_combo.setEnabled(False)
+                self.subject_config_button.setEnabled(False)
 
         # Workflow executing
         else:
             # Asks for workflow kill confirmation
             msg_box = QMessageBox()
-            msg_box.setText(strings.pttab_wf_stop)
+            msg_box.setText(strings.subj_tab_wf_stop)
             msg_box.setIcon(QMessageBox.Icon.Question)
             msg_box.setStandardButtons(QMessageBox.StandardButton.Yes | QMessageBox.StandardButton.No)
             msg_box.setDefaultButton(QMessageBox.StandardButton.No)
             msg_box.closeEvent = self.no_close_event
             ret = msg_box.exec()
             
             if ret == QMessageBox.StandardButton.No:
                 return
-            
-            # Workflow killing
-            self.workflow_process.stop_event.set()
-            
-            # UI updating
-            self.remove_running_icon()
-            self.exec_button.setText(strings.EXECBUTTONTEXT)
-            self.setTabEnabled(PtTab.DATATAB, True)
-            self.reset_workflow(force=True)
-            self.enable_tab_if_result_dir()
 
-    def slicer_tab_ui(self):
+            workflow_stop_ret = self.subject.stop_workflow()
+            if workflow_stop_ret == SubjectRet.ExecWfStatusError:
+                # Not running, should not be possible
+                pass
+            else:
+                # UI updating
+                self.remove_running_icon()
+                self.exec_button.setText(strings.EXECBUTTONTEXT)
+                self.setTabEnabled(SubjectTab.DATATAB, True)
+                self.reset_workflow(force=True)
+                self.enable_tab_if_result_dir()
+
+    def export_results_button_update_state(self):
+        """
+        Enable the export results button if Slicer is found on system
+        """
+        try:
+            if not DependencyManager.is_slicer(self.global_config):
+                self.generate_scene_button.setEnabled(False)
+                self.generate_scene_button.setToolTip(strings.subj_tab_generate_scene_button_disabled_tooltip)
+            else:
+                self.generate_scene_button.setEnabled(True)
+                self.generate_scene_button.setToolTip(strings.subj_tab_generate_scene_button_tooltip)
+        except:
+            pass
+
+    def load_scene_button_update_state(self):
+        """
+        Enable the load scene button if a scene file is present, otherwise disable it
+        """
+        try:
+            if not DependencyManager.is_slicer(self.global_config):
+                self.load_scene_button.setEnabled(False)
+                self.load_scene_button.setText(strings.subj_tab_load_scene_button + " " + strings.INFOCHAR)
+                self.load_scene_button.setToolTip(strings.subj_tab_generate_scene_button_disabled_tooltip)
+            elif os.path.exists(self.subject.scene_path()):
+                self.load_scene_button.setEnabled(True)
+                self.load_scene_button.setToolTip("")
+                self.load_scene_button.setText(strings.subj_tab_load_scene_button)
+            else:
+                self.load_scene_button.setEnabled(False)
+                self.load_scene_button.setToolTip(strings.subj_tab_load_scene_button_tooltip)
+                self.load_scene_button.setText(strings.subj_tab_load_scene_button + " " + strings.INFOCHAR)
+        except:
+            pass
+
+    def result_tab_ui(self):
         """
         Generates the Results tab UI.
 
         Returns
         -------
         None.
 
         """
         
-        slicer_tab_layout = QGridLayout()
-        self.slicer_tab.setLayout(slicer_tab_layout)
+        result_tab_layout = QGridLayout()
+        self.result_tab.setLayout(result_tab_layout)
 
-        self.export_results_button = QPushButton(strings.pttab_results_button)
-        self.export_results_button.clicked.connect(self.slicer_thread)
-        self.export_results_button.setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Fixed)
-        
-        if self.global_config.get_slicer_path() == '' or not os.path.exists(self.global_config.get_slicer_path()):
-            self.export_results_button.setEnabled(False)
-        slicer_tab_layout.addWidget(self.export_results_button, 0, 0)
+        self.generate_scene_button = QPushButton(strings.subj_tab_generate_scene_button)
+        self.generate_scene_button.clicked.connect(self.generate_scene)
+        self.generate_scene_button.setFixedHeight(self.main_window.NON_UNICODE_BUTTON_HEIGHT)
+        self.generate_scene_button.setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Fixed)
+        self.export_results_button_update_state()
+        result_tab_layout.addWidget(self.generate_scene_button, 0, 0)
+
+        horizontal_spacer = QSpacerItem(20, 40, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        result_tab_layout.addItem(horizontal_spacer, 0, 1, 1, 1)
+
+        self.load_scene_button = QPushButton(strings.subj_tab_load_scene_button)
+        self.load_scene_button.clicked.connect(self.load_scene)
+        self.load_scene_button.setFixedHeight(self.main_window.NON_UNICODE_BUTTON_HEIGHT)
+        self.load_scene_button.setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Fixed)
+        self.load_scene_button_update_state()
+        result_tab_layout.addWidget(self.load_scene_button, 0, 2)
+
+        self.open_results_directory_button = QPushButton(strings.subj_tab_open_results_directory)
+        self.open_results_directory_button.clicked.connect(
+            lambda pushed=False, results_dir=self.subject.result_dir(): open_results_directory(pushed, results_dir)
+        )
+        self.open_results_directory_button.setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Fixed)
+        self.open_results_directory_button.setFixedHeight(self.main_window.NON_UNICODE_BUTTON_HEIGHT)
+        result_tab_layout.addWidget(self.open_results_directory_button, 0, 3)
 
         self.results_model = QFileSystemModel()
         self.result_tree = QTreeView(parent=self)
+        self.result_tree.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
         self.result_tree.setModel(self.results_model)
 
-        slicer_tab_layout.addWidget(self.result_tree, 1, 0)
+        result_tab_layout.addWidget(self.result_tree, 1, 0, 1, 4)
 
-    def slicer_thread(self):
+    def generate_scene(self) -> PersistentProgressDialog:
         """
         Exports the workflow results into 3D Slicer using a new thread.
 
         Returns
         -------
-        None.
+        The progress dialog shown.
 
         """
         
-        progress = PersistentProgressDialog(strings.pttab_exporting_start, 0, 0, parent=self)
+        progress = PersistentProgressDialog(strings.subj_tab_exporting_start, 0, 0, parent=self)
         progress.show()
+        self.subject.generate_scene(lambda msg: SubjectTab.slicer_thread_signal(msg, progress))
+        return progress
 
-        slicer_thread = SlicerExportWorker(self.global_config.get_slicer_path(), self.pt_folder,
-                                           self.global_config.get_slicer_scene_ext(), parent=self)
-        slicer_thread.signal.export.connect(lambda msg: self.slicer_thread_signal(msg, progress))
-        QThreadPool.globalInstance().start(slicer_thread)
-
-    def slicer_thread_signal(self, msg: str, progress: PersistentProgressDialog):
+    @staticmethod
+    def slicer_thread_signal(msg: str, progress: PersistentProgressDialog):
         """
         Updates the Progress Dialog text to inform the user of the loading status.
 
         Parameters
         ----------
         msg : str
             The loading text.
@@ -773,275 +726,259 @@
         None.
 
         """
         
         if msg == SlicerExportWorker.END_MSG:
             progress.done(1)
         else:
-            progress.setLabelText(strings.pttab_exporting_prefix + msg)
+            progress.setLabelText(strings.subj_tab_exporting_prefix + msg)
+
+    def input_check_update(self, data_input: DataInputList, state: SubjectRet, dicom_src_work: DicomSearchWorker = None):
+        """
+        Function used as callback after subject dicom folder check
+
+        Parameters
+        ----------
+        data_input: DataInputList
+            The data input checked
+        state: SubjectRet
+            The return code of the scan
+        dicom_src_work: DicomSearchWorker, optional
+            The dicom scanner calling the function. Default is None
+        """
+        if data_input not in self.input_report:
+            return
+        if state == SubjectRet.DataInputWarningNoDicom:
+            self.set_error(data_input, strings.subj_tab_no_dicom_error + dicom_src_work.dicom_dir)
+        elif state == SubjectRet.DataInputWarningMultiSubj:
+            self.set_warn(data_input, strings.subj_tab_multi_subj_error + dicom_src_work.dicom_dir)
+        elif state == SubjectRet.DataInputWarningMultiExam:
+            self.set_warn(data_input, strings.subj_tab_multi_exam_error + dicom_src_work.dicom_dir)
+        elif state == SubjectRet.DataInputWarningMultiSeries:
+            self.set_warn(data_input, strings.subj_tab_multi_series_error + dicom_src_work.dicom_dir)
+        elif state == SubjectRet.DataInputLoading:
+            self.set_loading(data_input)
+        elif state == SubjectRet.DataInputValid:
+
+            subject_list = dicom_src_work.get_subject_list()
+            exam_list = dicom_src_work.get_exam_list(subject_list[0])
+            series_list = dicom_src_work.get_series_list(subject_list[0], exam_list[0])
+            image_list, subject_name, mod, series_description, vols = dicom_src_work.get_series_info(subject_list[0], exam_list[0], series_list[0])
+
+            label = SubjectTab.label_from_dicom(image_list, subject_name, mod, series_description, vols)
+
+            self.set_ok(data_input, label)
+            self.enable_exec_tab()
+            self.check_venous_volumes()
 
-    def load_pt(self):
+    def load_subject(self):
         """
-        Loads the Patient configuration and folder.
+        Loads the subject configuration and folder.
 
         Returns
         -------
         None.
 
         """
-        
-        dicom_scanners = {}
-        total_files = 0
 
-        # Config import absed on nipype_pipeline
-        self.pt_config = ConfigManager(self.pt_folder, self.main_window.freesurfer)
-        self.wf_type_combo.setCurrentIndex(self.pt_config.get_pt_wf_type())
-        # Set after patient loading to prevent the onchanged fire on previous line command
-        self.wf_type_combo.currentIndexChanged.connect(self.on_wf_type_changed)
+        index = self.workflow_type_combo.findData(self.subject.config.get_subject_workflow_type().name)
+        self.workflow_type_combo.setCurrentIndex(index)
+        # Set after subject loading to prevent the onchanged fire on previous line command
+        self.workflow_type_combo.currentIndexChanged.connect(self.on_wf_type_changed)
 
-        for data_input in self.data_input_list.values():
-            input_name = data_input.name
-            dicom_scanners[input_name] = self.check_input_folder_step1(input_name)
-            total_files = total_files + dicom_scanners[input_name].get_files_len()
+        # Scan subject dicom folder
+        dicom_scanners, total_files = self.subject.prepare_scan_dicom_folders()
 
         if total_files > 0:
-            progress = PersistentProgressDialog(strings.pttab_pt_loading, 0, 0, parent=self.parent())
+            progress = PersistentProgressDialog(strings.subj_tab_subj_loading, 0, 0, parent=self.parent())
             progress.show()
             progress.setMaximum(total_files)
-        else:
-            progress = None
+            self.subject.execute_scan_dicom_folders(dicom_scanners, status_callback=self.input_check_update,
+                                                    progress_callback=progress.increase_value)
 
-        for data_input in self.data_input_list.values():
-            input_name = data_input.name
-            self.input_report[input_name][0].load(self.main_window.LOADING_MOVIE_FILE)
-            self.check_input_folder_step2(input_name, dicom_scanners[input_name], progress)
-            self.directory_watcher.addPath(
-                os.path.join(self.pt_folder, self.global_config.get_default_dicom_folder(), input_name))
-
-        self.setTabEnabled(PtTab.DATATAB, True)
+        # Update UI after loading dicom
+        self.setTabEnabled(SubjectTab.DATATAB, True)
         self.setCurrentWidget(self.data_tab)
 
-        self.importable_series_list.clear()
+        self.clear_scan_result()
         self.reset_workflow()
 
         self.enable_tab_if_result_dir()
 
-    def enable_tab_if_result_dir(self):
+    def enable_tab_if_result_dir(self, changed_path: str = "", on_workflow_running: bool = False):
         """
         Enables Results tab, if any.
 
+        Parameters
+        _______
+        changed_path: str
+            The changed directory, passed if called by watcher
+        on_workflow_running: bool
+            If True, updte states even if workflow is running. Default is False.
+
         Returns
         -------
         None.
 
         """
-        scene_dir = os.path.join(self.pt_folder, MainWorkflow.SCENE_DIR)
+        scene_dir = self.subject.result_dir()
+
+        if self.subject.is_workflow_process_alive() and not on_workflow_running:
+            return
         
         if os.path.exists(scene_dir):
-            self.setTabEnabled(PtTab.RESULTTAB, True)
+            self.setTabEnabled(SubjectTab.RESULTTAB, True)
             self.results_model.setRootPath(scene_dir)
             index_root = self.results_model.index(self.results_model.rootPath())
             self.result_tree.setRootIndex(index_root)
+            self.result_directory_watcher.addPath(scene_dir)
+            self.load_scene_button_update_state()
         else:
-            self.setTabEnabled(PtTab.RESULTTAB, False)
+            self.setTabEnabled(SubjectTab.RESULTTAB, False)
+            self.result_directory_watcher.removePaths([scene_dir])
 
-    def check_input_folder_step1(self, input_name: str) -> DicomSearchWorker:
+    def clear_import_folder(self, data_input: DataInputList):
         """
-        Generates a Worker that scan the series folder in search for DICOM files.
+        Clears the subject series folder.
 
         Parameters
         ----------
-        input_name : str
-            The series folder name to check.
-
-        Returns
-        -------
-        dicom_src_work : DicomSearchWorker
-            The DICOM Search Worker.
-
-        """
-        
-        src_path = os.path.join(self.pt_folder,
-                                self.global_config.get_default_dicom_folder(), input_name)
-        dicom_src_work = DicomSearchWorker(src_path)
-        dicom_src_work.load_dir()
-        
-        return dicom_src_work
-
-    def check_input_folder_step2(self, input_name: str, dicom_src_work: DicomSearchWorker, progress: PersistentProgressDialog=None):
-        """
-        Starts the DICOM files scan Worker into the series folder on a new thread.
-
-        Parameters
-        ----------
-        input_name : str
-            The series folder name to check.
-        dicom_src_work : DicomSearchWorker
-            The DICOM Search Worker.
-        progress : PersistentProgressDialog, optional
-            The progress dialog. The default is None.
+        data_input : DataInputList
+            The series folder name to clear.
 
         Returns
         -------
         None.
 
         """
-        
-        dicom_src_work.signal.sig_finish.connect(lambda src, name=input_name: self.check_input_folder_step3(name, src))
-        
-        if progress is not None:
-            if progress.maximum() == 0:
-                progress.setMaximum(dicom_src_work.get_files_len())
-            dicom_src_work.signal.sig_loop.connect(lambda i: progress.increase_value(i))
-            
-        QThreadPool.globalInstance().start(dicom_src_work)
 
-    def check_input_folder_step3(self, input_name: str, dicom_src_work: DicomSearchWorker):
-        """
-        Updates SWANe UI at the end of the DICOM files scan Worker execution for a patient.
+        src_path = self.subject.dicom_folder(data_input)
 
-        Parameters
-        ----------
-        input_name : str
-            The series folder name to check.
-        dicom_src_work : DicomSearchWorker
-            The DICOM Search Worker.
-
-        Returns
-        -------
-        None.
+        progress = PersistentProgressDialog(strings.subj_tab_dicom_clearing + src_path, 0, 0, self)
+        progress.show()
 
-        """
-        
-        src_path = dicom_src_work.dicom_dir
-        pt_list = dicom_src_work.get_patient_list()
+        self.subject.clear_import_folder(data_input)
 
-        if len(pt_list) == 0:
-            self.set_error(input_name, strings.pttab_no_dicom_error + src_path)
-            return
+        self.set_error(data_input, strings.subj_tab_no_dicom_error + src_path)
+        self.enable_exec_tab()
 
-        if len(pt_list) > 1:
-            self.set_warn(input_name, strings.pttab_multi_pt_error + src_path)
-            return
-        
-        exam_list = dicom_src_work.get_exam_list(pt_list[0])
-        
-        if len(exam_list) != 1:
-            self.set_warn(input_name, strings.pttab_multi_exam_error + src_path)
-            return
-        
-        series_list = dicom_src_work.get_series_list(pt_list[0], exam_list[0])
-        
-        if len(series_list) != 1:
-            self.set_warn(input_name, strings.pttab_multi_series_error + src_path)
-            return
+        progress.accept()
 
-        image_list = dicom_src_work.get_series_files(pt_list[0], exam_list[0], series_list[0])
-        ds = pydicom.read_file(image_list[0], force=True)
-        mod = ds.Modality
-        
-        if mod in DataInput.IMAGE_MODALITY_RENAME_LIST:
-            mod = DataInput.IMAGE_MODALITY_RENAME_LIST[mod]
-            
-        self.set_ok(input_name, str(ds.PatientName) + "-" + mod + "-" + ds.SeriesDescription + ": " + str(
-            len(image_list)) + " images")
+        self.reset_workflow()
+        self.check_venous_volumes()
 
-        self.data_input_list[input_name].loaded = True
+        if data_input == DataInputList.VENOUS and self.subject.input_state_list[DataInputList.VENOUS2].loaded:
+            self.clear_import_folder(DataInputList.VENOUS2)
 
-        self.enable_exec_tab()
+    def check_venous_volumes(self):
+        """
+        Display informative warnings in venous and venous2 data input rows to help user in data loading
+        """
+        phases = self.subject.input_state_list[DataInputList.VENOUS].volumes + self.subject.input_state_list[DataInputList.VENOUS2].volumes
+        if phases == 0:
+            self.input_report[DataInputList.VENOUS2][3].setEnabled(False)
+        elif phases == 1:
+            if self.subject.input_state_list[DataInputList.VENOUS].loaded:
+                self.set_warn(DataInputList.VENOUS, "Series has only one phase, load the second phase below", False)
+                self.input_report[DataInputList.VENOUS2][3].setEnabled(True)
+            if self.subject.input_state_list[DataInputList.VENOUS2].loaded:
+                # this should not be possible!
+                self.set_warn(DataInputList.VENOUS2, "Series has only one phase, load the second phase above", False)
+        elif phases == 2:
+            if self.subject.input_state_list[DataInputList.VENOUS].loaded:
+                self.set_ok(DataInputList.VENOUS, None)
+                self.input_report[DataInputList.VENOUS2][3].setEnabled(False)
+            if self.subject.input_state_list[DataInputList.VENOUS2].loaded:
+                self.set_ok(DataInputList.VENOUS2, None)
+        else:
+            # something gone wrong, more than 2 phases!
+            if self.subject.input_state_list[DataInputList.VENOUS].loaded:
+                self.set_warn(DataInputList.VENOUS, "Too many venous phases loaded, delete some!", False)
+                self.input_report[DataInputList.VENOUS2][3].setEnabled(True)
+            if self.subject.input_state_list[DataInputList.VENOUS2].loaded:
+                self.set_warn(DataInputList.VENOUS2, "Too many venous phases loaded, delete some!", False)
 
-    def check_input_folder(self, input_name: str, progress: PersistentProgressDialog=None):
+    def exec_button_set_enabled(self, enabled: bool):
         """
-        Checks if the series folder labelled input_name contains DICOM files.
-        If PersistentProgressDialog is not None, it will be used to show the scan progress.
+        Change the status and the tooltip of the exec workflow button.
 
         Parameters
         ----------
-        input_name : str
-            The series folder name to check.
-        progress : PersistentProgressDialog, optional
-            The progress dialog. The default is None.
-
-        Returns
-        -------
-        None.
-
+        enabled : bool
+            The new status of the button
         """
-        
-        dicom_src_work = self.check_input_folder_step1(input_name)
-        self.check_input_folder_step2(input_name, dicom_src_work, progress)
+        if enabled:
+            self.exec_button.setEnabled(True)
+            self.exec_button.setToolTip("")
+            self.exec_button.setText(strings.EXECBUTTONTEXT)
+        else:
+            self.exec_button.setEnabled(False)
+            self.exec_button.setToolTip(strings.EXECBUTTONTEXT_disabled_tooltip)
+            self.exec_button.setText(strings.EXECBUTTONTEXT + "  " + strings.INFOCHAR)
 
-    def clear_import_folder(self, input_name: str):
+    def reset_workflow(self, force: bool = False):
         """
-        Clears the patient series folder.
+        Set the workflow var to None.
+        Resets the UI.
+        Works only if the worklow is not in execution or if force var is True.
 
         Parameters
         ----------
-        input_name : str
-            The series folder name to clear.
+        force : bool, optional
+            Force the usage of this function during workflow execution. The default is False.
 
         Returns
         -------
         None.
 
         """
 
-        src_path = os.path.join(self.pt_folder,
-                                self.global_config.get_default_dicom_folder(), input_name)
-
-        progress = PersistentProgressDialog(strings.pttab_dicom_clearing + src_path, 0, 0, self)
-        progress.show()
+        if self.subject.reset_workflow(force):
+            self.node_list_treeWidget.clear()
+            self.exec_graph.load(self.main_window.VOID_SVG_FILE)
+            self.exec_button_set_enabled(False)
+            self.generate_workflow_button.setEnabled(True)
+            self.workflow_type_combo.setEnabled(True)
+            self.subject_config_button.setEnabled(True)
 
-        import shutil
-        shutil.rmtree(src_path, ignore_errors=True)
-        os.makedirs(src_path, exist_ok=True)
-
-        # Reset the workflows related to the deleted DICOM images
-        src_path = os.path.join(self.pt_folder, self.pt_name + WorkflowGeneratorWorker.WF_DIR_SUFFIX,
-                                self.data_input_list[input_name].wf_name)
-        shutil.rmtree(src_path, ignore_errors=True)
-
-        self.set_error(input_name, strings.pttab_no_dicom_error + src_path)
-        self.data_input_list[input_name].loaded = False
-        self.enable_exec_tab()
-
-        progress.accept()
-        
-        self.reset_workflow()
-
-    def reset_workflow(self, force: bool=False):
+    @staticmethod
+    def label_from_dicom(image_list: list[str], subject_name: str, mod: str, series_description: str, vols: int) -> str:
         """
-        Set the workflow var to None.
-        Resets the UI.
-        Works only if the worklow is not in execution or if force var is True.
+        Compose dicom scan result into a readable label
 
         Parameters
         ----------
-        force : bool, optional
-            Force the usage of this function during workflow execution. The default is False.
+        image_list : list[str]
+            The list of file found
+        subject_name: str
+            The subject name found
+        mod: str
+            The image modality found
+        series_description: str
+            The series description found
+        vols: int
+            The volumes count found in the series
 
         Returns
         -------
-        None.
+        A string containing the label text
 
         """
-        
-        if self.workflow is None:
-            return
-        if not force and self.is_workflow_process_alive():
-            return
-
-        self.workflow = None
-        self.node_list_treeWidget.clear()
-        self.exec_graph.load(self.main_window.VOID_SVG_FILE)
-        self.exec_button.setEnabled(False)
-        self.exec_button.setText(strings.EXECBUTTONTEXT)
-        self.node_button.setEnabled(True)
-        self.wf_type_combo.setEnabled(True)
-        self.pt_config_button.setEnabled(True)
+        if image_list is None:
+            return None
+        try:
+            label = subject_name + "-" + mod + "-" + series_description + ": " + str(
+                len(image_list)) + " images, " + str(vols) + " "
+            if vols > 1:
+                label += "volumes"
+            else:
+                label += "volume"
+            return label
+        except:
+            return ""
 
     def show_scan_result(self, dicom_src_work: DicomSearchWorker):
         """
         Updates importable series list using DICOM Search Worker results.
 
         Parameters
         ----------
@@ -1051,130 +988,237 @@
         Returns
         -------
         None.
 
         """
         
         folder_path = dicom_src_work.dicom_dir
-        pt_list = dicom_src_work.get_patient_list()
+        self.scan_directory_watcher.addPath(folder_path)
+        subject_list = dicom_src_work.get_subject_list()
 
-        if len(pt_list) == 0:
+        if len(subject_list) == 0:
             msg_box = QMessageBox()
-            msg_box.setText(strings.pttab_no_dicom_error + folder_path)
+            msg_box.setText(strings.subj_tab_no_dicom_error + folder_path)
             msg_box.exec()
             return
         
-        if len(pt_list) > 1:
+        if len(subject_list) > 1:
             msg_box = QMessageBox()
-            msg_box.setText(strings.pttab_multi_pt_error + folder_path)
+            msg_box.setText(strings.subj_tab_multi_subj_error + folder_path)
             msg_box.exec()
             return
         
-        exam_list = dicom_src_work.get_exam_list(pt_list[0])
+        exam_list = dicom_src_work.get_exam_list(subject_list[0])
         
         for exam in exam_list:
-            series_list = dicom_src_work.get_series_list(pt_list[0], exam)
+            series_list = dicom_src_work.get_series_list(subject_list[0], exam)
             for series in series_list:
-                image_list = dicom_src_work.get_series_files(pt_list[0], exam, series)
-                ds = pydicom.read_file(image_list[0], force=True)
-                
-                # Excludes series with less than 10 images unless they are siemens mosaics series
-                if len(image_list) < 10 and hasattr(ds, 'ImageType') and "MOSAIC" not in ds.ImageType:
-                    continue
-
-                mod = ds.Modality
-
-                if mod in DataInput.IMAGE_MODALITY_RENAME_LIST:
-                    mod = DataInput.IMAGE_MODALITY_RENAME_LIST[mod]
-
-                self.final_series_list.append(
-                    [str(ds.PatientName) + "-" + mod + "-" + ds.SeriesDescription + ": " + str(
-                        len(image_list)) + " images", image_list])
-                del image_list
 
-        for series in self.final_series_list:
+                image_list, subject_name, mod, series_description, vols = dicom_src_work.get_series_info(subject_list[0], exam, series)
+
+                if image_list is not None:
+                    label = SubjectTab.label_from_dicom(image_list, subject_name, mod, series_description, vols)
+                    self.dicom_scan_series_list.append(
+                        [label, image_list, mod, vols])
+
+        for series in self.dicom_scan_series_list:
             self.importable_series_list.addItem(series[0])
 
-    def set_warn(self, input_name: str, msg: str):
+    def clear_scan_result(self):
+        """
+        Clear the content of the scan result list
+        """
+        self.importable_series_list.clear()
+        self.dicom_scan_series_list = None
+        if len(self.scan_directory_watcher.directories()) > 0:
+            self.scan_directory_watcher.removePaths(self.scan_directory_watcher.directories())
+
+    def is_data_loading(self) -> bool:
+        """
+        Returns
+            True if any data folder is being scanned
+        """
+
+        for row in self.input_report.values():
+            if row[5] == self.main_window.LOADING_MOVIE_FILE:
+                return True
+        return False
+
+    def update_input_report(self, data_input: DataInputList, icon: str, tooltip: str, import_enable: bool, clear_enable: bool, text: str = None):
+        """
+        Generic update function for series labels.
+
+        Parameters
+        ----------
+        data_input: DataInputList
+            The series label.
+        icon: str
+            The icon file to set near the label
+        tooltip: str
+            Mouse over tooltip:
+        import_enable: bool
+            The enable status of the import series button
+        clear_enable: bool
+            The enable status of the clear series button
+        text: str
+            The text to show under the label, if not None. Default is None
+        """
+        self.input_report[data_input][0].load(icon)
+        self.input_report[data_input][0].setFixedSize(25, 25)
+        self.input_report[data_input][0].setToolTip(tooltip)
+        self.input_report[data_input][3].setEnabled(import_enable)
+        self.input_report[data_input][4].setEnabled(clear_enable)
+        self.input_report[data_input][5] = icon
+        if text is not None:
+            self.input_report[data_input][2].setText(text)
+
+    def set_warn(self, data_input: DataInputList, tooltip: str, clear_text: bool = True):
         """
         Set a warning message and icon near a series label.
 
         Parameters
         ----------
-        input_name : str
+        data_input : DataInputList
             The series label.
-        msg : str
+        tooltip : str
             The warning message.
+        clear_text : bool
+            If True delete the label text
 
         Returns
         -------
         None.
 
         """
-        
-        self.input_report[input_name][0].load(self.main_window.WARNING_ICON_FILE)
-        self.input_report[input_name][0].setFixedSize(25, 25)
-        self.input_report[input_name][0].setToolTip(msg)
-        self.input_report[input_name][3].setEnabled(False)
-        self.input_report[input_name][4].setEnabled(True)
-        self.input_report[input_name][2].setText("")
+        text = None
+        if clear_text:
+            text = ""
 
-    def set_error(self, input_name: str, msg: str):
+        self.update_input_report(
+            data_input=data_input,
+            icon=self.main_window.WARNING_ICON_FILE,
+            tooltip=tooltip,
+            import_enable=False,
+            clear_enable=True,
+            text=text
+        )
+
+    def set_error(self, data_input: DataInputList, tooltip: str):
         """
         Set an error message and icon near a series label.
 
         Parameters
         ----------
-        input_name : str
+        data_input : DataInputList
             The series label.
-        msg : str
+        tooltip : str
             The error message.
-
-        Returns
-        -------
-        None.
-
         """
-        
-        self.input_report[input_name][0].load(self.main_window.ERROR_ICON_FILE)
-        self.input_report[input_name][0].setFixedSize(25, 25)
-        self.input_report[input_name][0].setToolTip(msg)
-        self.input_report[input_name][3].setEnabled(True)
-        self.input_report[input_name][4].setEnabled(False)
-        self.input_report[input_name][2].setText("")
 
-    def set_ok(self, input_name: str, msg: str):
+        self.update_input_report(
+            data_input=data_input,
+            icon=self.main_window.ERROR_ICON_FILE,
+            tooltip=tooltip,
+            import_enable=True,
+            clear_enable=False,
+            text=""
+        )
+
+    def set_ok(self, data_input: DataInputList, text: str):
         """
         Set a success message and icon near a series label.
 
         Parameters
         ----------
-        input_name : str
+        data_input : DataInputList
             The series label.
-        msg : str
-            The success message.
+        text : str
+            The success message. If string is None keep the current text
+        """
+        self.update_input_report(
+            data_input=data_input,
+            icon=self.main_window.OK_ICON_FILE,
+            tooltip="",
+            import_enable=False,
+            clear_enable=True,
+            text=text,
+        )
 
-        Returns
-        -------
-        None.
+    def set_loading(self, data_input: DataInputList):
+        """
+        Set a loading message and icon near a series label.
 
+        Parameters
+        ----------
+        data_input : DataInputList
+            The series label.
         """
-        
-        self.input_report[input_name][0].load(self.main_window.OK_ICON_FILE)
-        self.input_report[input_name][0].setFixedSize(25, 25)
-        self.input_report[input_name][0].setToolTip("")
-        self.input_report[input_name][3].setEnabled(False)
-        self.input_report[input_name][4].setEnabled(True)
-        self.input_report[input_name][2].setText(msg)
+        self.update_input_report(
+            data_input=data_input,
+            icon=self.main_window.LOADING_MOVIE_FILE,
+            tooltip="",
+            import_enable=False,
+            clear_enable=False,
+            text=None,
+        )
 
     def enable_exec_tab(self):
         """
         Enables the Execute Workflow tab into the UI.
 
         Returns
         -------
         None.
 
         """
         
-        enable = self.data_input_list.is_ref_loaded() and self.main_window.fsl and self.main_window.dcm2niix
-        self.setTabEnabled(PtTab.EXECTAB, enable)
+        enable = self.subject.can_generate_workflow()
+        self.setTabEnabled(SubjectTab.EXECTAB, enable)
+
+    def load_scene(self):
+        """
+            Visualize the workflow results into 3D Slicer.
+        """
+
+        slicer_open_thread = SlicerViewerWorker(self.global_config.get_slicer_path(), self.subject.scene_path())
+        QThreadPool.globalInstance().start(slicer_open_thread)
+
+    def setTabEnabled(self, index: int, enabled: bool):
+        """
+        Changes the status of a tab and set an informative tooltip
+
+        Parameters
+        -------
+        index: int
+            The tab index
+        enabled: bool
+            The new tab status
+        """
+        if index == SubjectTab.EXECTAB and not enabled:
+            if not self.subject.dependency_manager.is_fsl() or not self.subject.dependency_manager.is_dcm2niix():
+                self.setTabToolTip(index, strings.subj_tab_tabtooltip_exec_disabled_dependency)
+            else:
+                self.setTabToolTip(index, strings.subj_tab_tabtooltip_exec_disabled_series)
+        elif index == SubjectTab.RESULTTAB and not enabled:
+            self.setTabToolTip(index, strings.subj_tab_tabtooltip_result_disabled)
+        elif index == SubjectTab.DATATAB and not enabled:
+            self.setTabToolTip(index, strings.subj_tab_tabtooltip_data_disabled)
+        else:
+            self.setTabToolTip(index, "")
+        super().setTabEnabled(index, enabled)
+
+    def setTabToolTip(self, index: int, tooltip: str):
+        """
+        Changes the tooltip of a tab
+
+        Parameters
+        -------
+        index: int
+            The tab index
+        tooltip: str
+            The tooltip to show
+        """
+        super().setTabToolTip(index, tooltip)
+        if tooltip == "" and self.tabText(index).endswith(strings.INFOCHAR):
+            self.setTabText(index, self.tabText(index).replace(" "+strings.INFOCHAR, ""))
+        elif tooltip != "" and not self.tabText(index).endswith(strings.INFOCHAR):
+            self.setTabText(index, self.tabText(index) + " " + strings.INFOCHAR)
```

### Comparing `swane-0.0.6/swane/ui/VerticalScrollArea.py` & `swane-0.1.0/swane/ui/VerticalScrollArea.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.6/swane/utils/fsl_conflict_handler.py` & `swane-0.1.0/swane/utils/fsl_conflict_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
                  'csh': ['.cshrc'],
                  'tcsh': ['.tcshrc']}
 
 FIX_LINE = "PATH=$(echo \"$PATH\" | sed -e \"s/:$( echo \"$FSL_DIR\" | sed 's/\//\\\\\//g')\/bin//\")"
 APP_EXEC_COMMAND = "python3 -m " + __name__.split(".")[0]
 
 
-def check_config_file(config_file):
+def check_config_file(config_file: str):
     try:
         with open(config_file) as file:
             file_content = file.read()
         return FREESURFER_CONFIG_FILE in file_content
     except:
         return False
 
@@ -46,40 +46,46 @@
 
 
 def runtime_fix():
     cmd = FIX_LINE + ";" + APP_EXEC_COMMAND
     subprocess.run(cmd, shell=True)
 
 
-def config_file_fix(config_file):
+def config_file_fix(config_file: str):
     with open(config_file, "a") as file_object:
-        # Append 'hello' at the end of file
         file_object.write("\n"+FIX_LINE)
 
 
 def copy_fix_to_clipboard():
     # Linux shell copy command
     subprocess.run("xclip -selection c", shell=True, text=True, input=FIX_LINE)
     # MacOS shell copy command
     subprocess.run("pbcopy", shell=True, text=True, input=FIX_LINE)
 
 
-def fsl_conflict_check():
-    # Handle freesurfer<=7.3.2 overwriting system python executable if fsl>=6.0.6 is installed
+def fsl_conflict_check() -> bool:
+    """
+        Handle freesurfer<=7.3.2 overwriting system python executable if fsl>=6.0.6 is installed
+        In that case propose a fix
+
+    Returns
+    -------
+        True if system Python is unaffected, False if it was hidden
+
+    """
+
     if FSL_CONFLICT_PATH not in sys.executable:
         return True
 
-    # This functions uses fsl built-in qt library to show a warning
+    # This function uses fsl built-in qt library to show a warning: ignore IDE import error!
     from PyQt5.QtWidgets import QApplication, QLabel, QMessageBox
-    from PyQt5.QtGui import QIcon, QPixmap
 
     app = QApplication([])
     app.setApplicationDisplayName(strings.APPNAME)
 
-    # todo Add wiki link with example images
     config_file = get_config_file()
     error_string = strings.fsl_python_error % config_file
 
     msg_box = QMessageBox()
     msg_box.setText(error_string)
     msg_box.setInformativeText(FIX_LINE)
     msg_box.setIcon(QMessageBox.Warning)
```

### Comparing `swane-0.0.6/swane/utils/print_error.py` & `swane-0.1.0/swane/utils/print_error.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.6/swane.egg-info/SOURCES.txt` & `swane-0.1.0/swane.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -7,76 +7,88 @@
 swane/strings.py
 swane.egg-info/PKG-INFO
 swane.egg-info/SOURCES.txt
 swane.egg-info/dependency_links.txt
 swane.egg-info/entry_points.txt
 swane.egg-info/requires.txt
 swane.egg-info/top_level.txt
+swane/config/ConfigManager.py
+swane/config/PrefCategory.py
+swane/config/PreferenceEntry.py
+swane/config/__init__.py
+swane/config/config_enums.py
+swane/config/preference_list.py
 swane/nipype_pipeline/MainWorkflow.py
 swane/nipype_pipeline/__init__.py
 swane/nipype_pipeline/engine/CustomWorkflow.py
 swane/nipype_pipeline/engine/MonitoredMultiProcPlugin.py
 swane/nipype_pipeline/engine/NodeListEntry.py
+swane/nipype_pipeline/engine/WorkflowReport.py
 swane/nipype_pipeline/engine/__init__.py
 swane/nipype_pipeline/nodes/AsymmetryIndex.py
+swane/nipype_pipeline/nodes/CropFov.py
 swane/nipype_pipeline/nodes/CustomBEDPOSTX5.py
 swane/nipype_pipeline/nodes/CustomDcm2niix.py
-swane/nipype_pipeline/nodes/CustomDilateImage.py
+swane/nipype_pipeline/nodes/CustomEddy.py
 swane/nipype_pipeline/nodes/CustomLabel2Vol.py
 swane/nipype_pipeline/nodes/CustomProbTrackX2.py
 swane/nipype_pipeline/nodes/CustomSliceTimer.py
 swane/nipype_pipeline/nodes/DeleteVolumes.py
 swane/nipype_pipeline/nodes/FLAT1OutliersMask.py
 swane/nipype_pipeline/nodes/FMRIGenSpec.py
 swane/nipype_pipeline/nodes/ForceOrient.py
-swane/nipype_pipeline/nodes/FslCluster.py
 swane/nipype_pipeline/nodes/FslNVols.py
+swane/nipype_pipeline/nodes/GenEddyFiles.py
 swane/nipype_pipeline/nodes/GetNiftiTR.py
 swane/nipype_pipeline/nodes/MergeTargets.py
 swane/nipype_pipeline/nodes/Orient.py
 swane/nipype_pipeline/nodes/RandomSeedGenerator.py
 swane/nipype_pipeline/nodes/SegmentHA.py
 swane/nipype_pipeline/nodes/SumMultiTracks.py
 swane/nipype_pipeline/nodes/SumMultiVols.py
 swane/nipype_pipeline/nodes/TTest.py
 swane/nipype_pipeline/nodes/ThrROI.py
 swane/nipype_pipeline/nodes/VenousCheck.py
 swane/nipype_pipeline/nodes/Zscore.py
 swane/nipype_pipeline/nodes/__init__.py
 swane/nipype_pipeline/nodes/utils.py
-swane/nipype_pipeline/workflows/FLAT1_workflow.py
 swane/nipype_pipeline/workflows/__init__.py
 swane/nipype_pipeline/workflows/dti_preproc_workflow.py
+swane/nipype_pipeline/workflows/flat1_workflow.py
 swane/nipype_pipeline/workflows/freesurfer_asymmetry_index_workflow.py
 swane/nipype_pipeline/workflows/freesurfer_workflow.py
 swane/nipype_pipeline/workflows/func_map_workflow.py
 swane/nipype_pipeline/workflows/linear_reg_workflow.py
 swane/nipype_pipeline/workflows/nonlinear_reg_workflow.py
 swane/nipype_pipeline/workflows/ref_workflow.py
 swane/nipype_pipeline/workflows/task_fMRI_workflow.py
 swane/nipype_pipeline/workflows/tractography_workflow.py
 swane/nipype_pipeline/workflows/venous_workflow.py
-swane/slicer/SlicerCheckWorker.py
-swane/slicer/SlicerExportWorker.py
-swane/slicer/__init__.py
-swane/slicer/slicer_script_freesurfer_module_check.py
-swane/slicer/slicer_script_result.py
 swane/ui/CustomTreeWidgetItem.py
 swane/ui/MainWindow.py
 swane/ui/PersistentProgressDialog.py
+swane/ui/PreferenceUIEntry.py
 swane/ui/PreferencesWindow.py
-swane/ui/PtTab.py
+swane/ui/SubjectTab.py
 swane/ui/VerticalScrollArea.py
 swane/ui/__init__.py
-swane/ui/workers/DicomSearchWorker.py
-swane/ui/workers/WorkflowGeneratorWorker.py
-swane/ui/workers/WorkflowMonitorWorker.py
-swane/ui/workers/WorkflowProcess.py
-swane/ui/workers/__init__.py
-swane/utils/ConfigManager.py
-swane/utils/DataInput.py
-swane/utils/PreferenceEntry.py
+swane/utils/DataInputList.py
+swane/utils/DependencyManager.py
+swane/utils/Subject.py
+swane/utils/SubjectInputStateList.py
 swane/utils/__init__.py
-swane/utils/check_dependency.py
+swane/utils/decorators.py
 swane/utils/fsl_conflict_handler.py
+swane/utils/last_pid_is_running.py
 swane/utils/print_error.py
-swane/utils/shortcut_manager.py
+swane/workers/DicomSearchWorker.py
+swane/workers/SlicerCheckWorker.py
+swane/workers/SlicerExportWorker.py
+swane/workers/SlicerViewerWorker.py
+swane/workers/UpdateCheckWorker.py
+swane/workers/WorkflowMonitorWorker.py
+swane/workers/WorkflowProcess.py
+swane/workers/__init__.py
+swane/workers/open_results_directory.py
+swane/workers/slicer_script_freesurfer_module_check.py
+swane/workers/slicer_script_freesurfer_module_install.py
+swane/workers/slicer_script_result.py
```

