# Comparing `tmp/grav-toolbox-0.2.7.tar.gz` & `tmp/grav_toolbox-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grav-toolbox-0.2.7.tar", last modified: Wed Feb 21 13:44:55 2024, max compression
+gzip compressed data, was "grav_toolbox-0.2.8.tar", last modified: Tue Apr 16 17:54:45 2024, max compression
```

## Comparing `grav-toolbox-0.2.7.tar` & `grav_toolbox-0.2.8.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2024-02-21 13:44:55.902725 grav-toolbox-0.2.7/
--rw-rw-r--   0 heller    (1000) heller    (1000)    35148 2023-10-08 16:08:47.000000 grav-toolbox-0.2.7/LICENSE
--rw-r--r--   0 heller    (1000) heller    (1000)     6840 2024-02-21 13:44:55.902725 grav-toolbox-0.2.7/PKG-INFO
--rw-rw-r--   0 heller    (1000) heller    (1000)     6060 2023-10-08 16:08:47.000000 grav-toolbox-0.2.7/README.md
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2024-02-21 13:44:55.894725 grav-toolbox-0.2.7/bev_legacy/
--rw-rw-r--   0 heller    (1000) heller    (1000)        0 2023-10-08 16:08:47.000000 grav-toolbox-0.2.7/bev_legacy/__init__.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)    20574 2024-01-26 10:29:01.000000 grav-toolbox-0.2.7/bev_legacy/adjust.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     7276 2024-01-26 10:29:01.000000 grav-toolbox-0.2.7/bev_legacy/adjust_reilly1970.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     2736 2023-10-08 16:08:47.000000 grav-toolbox-0.2.7/bev_legacy/command_line.py
--rw-rw-r--   0 heller    (1000) heller    (1000)      139 2023-10-08 16:08:47.000000 grav-toolbox-0.2.7/bev_legacy/const.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     3935 2023-10-08 16:08:47.000000 grav-toolbox-0.2.7/bev_legacy/drift_mlr.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)    11170 2023-10-08 16:08:47.000000 grav-toolbox-0.2.7/bev_legacy/init.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     7718 2024-01-26 10:29:01.000000 grav-toolbox-0.2.7/bev_legacy/output.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     2408 2023-10-08 16:08:47.000000 grav-toolbox-0.2.7/bev_legacy/plots.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     9365 2023-10-08 16:08:47.000000 grav-toolbox-0.2.7/bev_legacy/schwaus.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     4485 2024-02-21 11:50:37.000000 grav-toolbox-0.2.7/bev_legacy/settings.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     1933 2023-10-08 16:08:47.000000 grav-toolbox-0.2.7/bev_legacy/utils.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2024-02-21 13:44:55.902725 grav-toolbox-0.2.7/grav_toolbox.egg-info/
--rw-r--r--   0 heller    (1000) heller    (1000)     6840 2024-02-21 13:44:55.000000 grav-toolbox-0.2.7/grav_toolbox.egg-info/PKG-INFO
--rw-rw-r--   0 heller    (1000) heller    (1000)     2614 2024-02-21 13:44:55.000000 grav-toolbox-0.2.7/grav_toolbox.egg-info/SOURCES.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)        1 2024-02-21 13:44:55.000000 grav-toolbox-0.2.7/grav_toolbox.egg-info/dependency_links.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)       57 2024-02-21 13:44:55.000000 grav-toolbox-0.2.7/grav_toolbox.egg-info/entry_points.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)       59 2024-02-21 13:44:55.000000 grav-toolbox-0.2.7/grav_toolbox.egg-info/requires.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)       21 2024-02-21 13:44:55.000000 grav-toolbox-0.2.7/grav_toolbox.egg-info/top_level.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)        1 2024-01-26 08:15:16.000000 grav-toolbox-0.2.7/grav_toolbox.egg-info/zip-safe
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2024-02-21 13:44:55.894725 grav-toolbox-0.2.7/gravtools/
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2024-02-21 13:44:55.894725 grav-toolbox-0.2.7/gravtools/CG5_utils/
--rw-rw-r--   0 heller    (1000) heller    (1000)     1122 2023-10-08 16:08:47.000000 grav-toolbox-0.2.7/gravtools/CG5_utils/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    35358 2023-10-08 16:08:47.000000 grav-toolbox-0.2.7/gravtools/CG5_utils/cg5_survey.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1299 2024-02-20 10:25:14.000000 grav-toolbox-0.2.7/gravtools/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)      757 2023-10-08 16:08:47.000000 grav-toolbox-0.2.7/gravtools/const.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2024-02-21 13:44:55.898725 grav-toolbox-0.2.7/gravtools/gui/
--rw-rw-r--   0 heller    (1000) heller    (1000)    88637 2024-02-21 11:32:12.000000 grav-toolbox-0.2.7/gravtools/gui/MainWindow.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1322 2023-10-08 16:08:47.000000 grav-toolbox-0.2.7/gravtools/gui/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1473 2023-10-08 16:08:47.000000 grav-toolbox-0.2.7/gravtools/gui/cumstom_widgets.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    42685 2024-02-21 11:32:12.000000 grav-toolbox-0.2.7/gravtools/gui/dialog_about.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    12317 2024-02-21 11:32:12.000000 grav-toolbox-0.2.7/gravtools/gui/dialog_autoselection_settings.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    18526 2024-02-21 11:32:12.000000 grav-toolbox-0.2.7/gravtools/gui/dialog_correction_time_series.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    17303 2024-02-21 11:32:12.000000 grav-toolbox-0.2.7/gravtools/gui/dialog_corrections.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    42384 2024-02-21 11:32:12.000000 grav-toolbox-0.2.7/gravtools/gui/dialog_estimation_settings.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    18945 2024-02-21 11:32:12.000000 grav-toolbox-0.2.7/gravtools/gui/dialog_export_results.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    10236 2024-02-21 11:32:12.000000 grav-toolbox-0.2.7/gravtools/gui/dialog_gis_export_settings.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     2946 2024-02-21 11:32:12.000000 grav-toolbox-0.2.7/gravtools/gui/dialog_load_stations.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    12699 2024-02-21 11:32:12.000000 grav-toolbox-0.2.7/gravtools/gui/dialog_load_tsf_file.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     4384 2024-02-21 11:32:12.000000 grav-toolbox-0.2.7/gravtools/gui/dialog_new_campaign.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     3979 2024-02-21 11:32:12.000000 grav-toolbox-0.2.7/gravtools/gui/dialog_options.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     9036 2024-02-21 11:32:12.000000 grav-toolbox-0.2.7/gravtools/gui/dialog_setup_data.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    15615 2024-02-20 10:24:49.000000 grav-toolbox-0.2.7/gravtools/gui/dlg_correction_time_series.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1890 2023-10-08 16:08:47.000000 grav-toolbox-0.2.7/gravtools/gui/dlg_corrections.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     2371 2023-10-08 16:08:47.000000 grav-toolbox-0.2.7/gravtools/gui/dlg_load_tsf_file.py
--rw-rw-r--   0 heller    (1000) heller    (1000)   223200 2024-02-21 12:06:34.000000 grav-toolbox-0.2.7/gravtools/gui/gui_main.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     3246 2023-10-08 16:08:47.000000 grav-toolbox-0.2.7/gravtools/gui/gui_misc.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    16070 2024-02-20 10:24:49.000000 grav-toolbox-0.2.7/gravtools/gui/gui_model_observation_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     6396 2024-01-15 16:13:37.000000 grav-toolbox-0.2.7/gravtools/gui/gui_model_results_correlation_matrix_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     6311 2023-10-08 16:08:47.000000 grav-toolbox-0.2.7/gravtools/gui/gui_model_results_drift_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    14416 2024-01-15 16:13:37.000000 grav-toolbox-0.2.7/gravtools/gui/gui_model_results_obs_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    11739 2023-10-08 16:08:47.000000 grav-toolbox-0.2.7/gravtools/gui/gui_model_results_stat_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     5454 2023-10-08 16:08:47.000000 grav-toolbox-0.2.7/gravtools/gui/gui_model_results_vg_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    10717 2024-02-20 10:24:49.000000 grav-toolbox-0.2.7/gravtools/gui/gui_model_setup_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     9716 2024-01-22 17:59:38.000000 grav-toolbox-0.2.7/gravtools/gui/gui_model_station_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    10556 2024-01-26 10:29:01.000000 grav-toolbox-0.2.7/gravtools/gui/gui_model_survey_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     5771 2024-02-21 10:08:41.000000 grav-toolbox-0.2.7/gravtools/gui/gui_models_gravimeters_scale_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1806 2023-10-08 16:10:22.000000 grav-toolbox-0.2.7/gravtools/gui/survey_table_handler.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2024-02-21 13:44:55.898725 grav-toolbox-0.2.7/gravtools/models/
--rw-rw-r--   0 heller    (1000) heller    (1000)     1166 2023-10-08 16:08:47.000000 grav-toolbox-0.2.7/gravtools/models/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     3978 2023-10-08 16:08:47.000000 grav-toolbox-0.2.7/gravtools/models/atmosphere_correction.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    54458 2024-02-21 11:46:43.000000 grav-toolbox-0.2.7/gravtools/models/campaign.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1695 2023-10-08 16:08:47.000000 grav-toolbox-0.2.7/gravtools/models/exceptions.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    20441 2024-02-21 11:53:38.000000 grav-toolbox-0.2.7/gravtools/models/gravimeter.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    42262 2024-02-21 13:13:33.000000 grav-toolbox-0.2.7/gravtools/models/lsm.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    38962 2024-02-21 11:54:24.000000 grav-toolbox-0.2.7/gravtools/models/lsm_diff.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    35415 2024-02-21 11:49:38.000000 grav-toolbox-0.2.7/gravtools/models/lsm_nondiff.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     3602 2023-10-08 16:08:47.000000 grav-toolbox-0.2.7/gravtools/models/misc.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    19052 2024-01-26 10:29:01.000000 grav-toolbox-0.2.7/gravtools/models/mlr_bev_legacy.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    22830 2024-02-20 10:24:49.000000 grav-toolbox-0.2.7/gravtools/models/station.py
--rw-rw-r--   0 heller    (1000) heller    (1000)   121311 2024-02-21 12:09:39.000000 grav-toolbox-0.2.7/gravtools/models/survey.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    32559 2024-02-21 11:49:38.000000 grav-toolbox-0.2.7/gravtools/models/vg_lsm.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2024-02-21 13:44:55.898725 grav-toolbox-0.2.7/gravtools/scripts/
--rw-rw-r--   0 heller    (1000) heller    (1000)     1064 2023-10-08 16:08:47.000000 grav-toolbox-0.2.7/gravtools/scripts/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1893 2023-10-08 16:08:47.000000 grav-toolbox-0.2.7/gravtools/scripts/create_correction_time_seriens_from_tsf.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1481 2023-10-08 16:08:47.000000 grav-toolbox-0.2.7/gravtools/scripts/load_tfs_file.py
--rw-rw-r--   0 heller    (1000) heller    (1000)      884 2023-10-08 16:08:47.000000 grav-toolbox-0.2.7/gravtools/scripts/run_gui.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)    14324 2024-02-21 11:52:41.000000 grav-toolbox-0.2.7/gravtools/settings.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2024-02-21 13:44:55.898725 grav-toolbox-0.2.7/gravtools/tides/
--rw-rw-r--   0 heller    (1000) heller    (1000)     1090 2023-10-08 16:08:47.000000 grav-toolbox-0.2.7/gravtools/tides/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    16241 2024-01-15 16:13:37.000000 grav-toolbox-0.2.7/gravtools/tides/correction_time_series.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    16019 2023-10-08 16:08:47.000000 grav-toolbox-0.2.7/gravtools/tides/longman1959.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     3413 2023-10-08 16:08:47.000000 grav-toolbox-0.2.7/gravtools/tides/tide_data.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    18006 2024-01-15 16:13:37.000000 grav-toolbox-0.2.7/gravtools/tides/tide_data_tfs.py
--rw-rw-r--   0 heller    (1000) heller    (1000)       89 2023-10-08 16:08:47.000000 grav-toolbox-0.2.7/pyproject.toml
--rw-rw-r--   0 heller    (1000) heller    (1000)      917 2024-02-21 13:44:55.902725 grav-toolbox-0.2.7/setup.cfg
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2024-04-16 17:54:45.622567 grav_toolbox-0.2.8/
+-rw-rw-r--   0 heller    (1000) heller    (1000)    35148 2023-10-08 16:08:47.000000 grav_toolbox-0.2.8/LICENSE
+-rw-r--r--   0 heller    (1000) heller    (1000)     6840 2024-04-16 17:54:45.622567 grav_toolbox-0.2.8/PKG-INFO
+-rw-rw-r--   0 heller    (1000) heller    (1000)     6060 2023-10-08 16:08:47.000000 grav_toolbox-0.2.8/README.md
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2024-04-16 17:54:45.614567 grav_toolbox-0.2.8/bev_legacy/
+-rw-rw-r--   0 heller    (1000) heller    (1000)        0 2023-10-08 16:08:47.000000 grav_toolbox-0.2.8/bev_legacy/__init__.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)    20574 2024-01-26 10:29:01.000000 grav_toolbox-0.2.8/bev_legacy/adjust.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     7276 2024-01-26 10:29:01.000000 grav_toolbox-0.2.8/bev_legacy/adjust_reilly1970.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     2736 2023-10-08 16:08:47.000000 grav_toolbox-0.2.8/bev_legacy/command_line.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)      139 2023-10-08 16:08:47.000000 grav_toolbox-0.2.8/bev_legacy/const.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     3935 2023-10-08 16:08:47.000000 grav_toolbox-0.2.8/bev_legacy/drift_mlr.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)    11170 2023-10-08 16:08:47.000000 grav_toolbox-0.2.8/bev_legacy/init.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     7718 2024-01-26 10:29:01.000000 grav_toolbox-0.2.8/bev_legacy/output.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     2408 2023-10-08 16:08:47.000000 grav_toolbox-0.2.8/bev_legacy/plots.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     9365 2023-10-08 16:08:47.000000 grav_toolbox-0.2.8/bev_legacy/schwaus.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     4485 2024-02-21 11:50:37.000000 grav_toolbox-0.2.8/bev_legacy/settings.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     1933 2023-10-08 16:08:47.000000 grav_toolbox-0.2.8/bev_legacy/utils.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2024-04-16 17:54:45.622567 grav_toolbox-0.2.8/grav_toolbox.egg-info/
+-rw-r--r--   0 heller    (1000) heller    (1000)     6840 2024-04-16 17:54:45.000000 grav_toolbox-0.2.8/grav_toolbox.egg-info/PKG-INFO
+-rw-rw-r--   0 heller    (1000) heller    (1000)     2614 2024-04-16 17:54:45.000000 grav_toolbox-0.2.8/grav_toolbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)        1 2024-04-16 17:54:45.000000 grav_toolbox-0.2.8/grav_toolbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)       57 2024-04-16 17:54:45.000000 grav_toolbox-0.2.8/grav_toolbox.egg-info/entry_points.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)       59 2024-04-16 17:54:45.000000 grav_toolbox-0.2.8/grav_toolbox.egg-info/requires.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)       21 2024-04-16 17:54:45.000000 grav_toolbox-0.2.8/grav_toolbox.egg-info/top_level.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)        1 2024-01-26 08:15:16.000000 grav_toolbox-0.2.8/grav_toolbox.egg-info/zip-safe
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2024-04-16 17:54:45.618567 grav_toolbox-0.2.8/gravtools/
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2024-04-16 17:54:45.618567 grav_toolbox-0.2.8/gravtools/CG5_utils/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1122 2023-10-08 16:08:47.000000 grav_toolbox-0.2.8/gravtools/CG5_utils/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    35358 2023-10-08 16:08:47.000000 grav_toolbox-0.2.8/gravtools/CG5_utils/cg5_survey.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1299 2024-03-06 09:12:07.000000 grav_toolbox-0.2.8/gravtools/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)      757 2023-10-08 16:08:47.000000 grav_toolbox-0.2.8/gravtools/const.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2024-04-16 17:54:45.622567 grav_toolbox-0.2.8/gravtools/gui/
+-rw-rw-r--   0 heller    (1000) heller    (1000)    90754 2024-03-06 15:01:11.000000 grav_toolbox-0.2.8/gravtools/gui/MainWindow.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1322 2023-10-08 16:08:47.000000 grav_toolbox-0.2.8/gravtools/gui/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1473 2023-10-08 16:08:47.000000 grav_toolbox-0.2.8/gravtools/gui/cumstom_widgets.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    42685 2024-03-06 15:01:11.000000 grav_toolbox-0.2.8/gravtools/gui/dialog_about.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    12317 2024-03-06 15:01:11.000000 grav_toolbox-0.2.8/gravtools/gui/dialog_autoselection_settings.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    18526 2024-03-06 15:01:11.000000 grav_toolbox-0.2.8/gravtools/gui/dialog_correction_time_series.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    17303 2024-03-06 15:01:11.000000 grav_toolbox-0.2.8/gravtools/gui/dialog_corrections.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    42384 2024-03-06 15:01:11.000000 grav_toolbox-0.2.8/gravtools/gui/dialog_estimation_settings.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    18945 2024-03-06 15:01:11.000000 grav_toolbox-0.2.8/gravtools/gui/dialog_export_results.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    10236 2024-03-06 15:01:11.000000 grav_toolbox-0.2.8/gravtools/gui/dialog_gis_export_settings.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     2946 2024-03-06 15:01:11.000000 grav_toolbox-0.2.8/gravtools/gui/dialog_load_stations.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    12699 2024-03-06 15:01:11.000000 grav_toolbox-0.2.8/gravtools/gui/dialog_load_tsf_file.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     4384 2024-03-06 15:01:11.000000 grav_toolbox-0.2.8/gravtools/gui/dialog_new_campaign.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     3979 2024-03-06 15:01:11.000000 grav_toolbox-0.2.8/gravtools/gui/dialog_options.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     9036 2024-03-06 15:01:11.000000 grav_toolbox-0.2.8/gravtools/gui/dialog_setup_data.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    15615 2024-02-20 10:24:49.000000 grav_toolbox-0.2.8/gravtools/gui/dlg_correction_time_series.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1890 2023-10-08 16:08:47.000000 grav_toolbox-0.2.8/gravtools/gui/dlg_corrections.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     2371 2023-10-08 16:08:47.000000 grav_toolbox-0.2.8/gravtools/gui/dlg_load_tsf_file.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)   226349 2024-03-06 14:15:24.000000 grav_toolbox-0.2.8/gravtools/gui/gui_main.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     3246 2023-10-08 16:08:47.000000 grav_toolbox-0.2.8/gravtools/gui/gui_misc.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    16070 2024-02-20 10:24:49.000000 grav_toolbox-0.2.8/gravtools/gui/gui_model_observation_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     6396 2024-01-15 16:13:37.000000 grav_toolbox-0.2.8/gravtools/gui/gui_model_results_correlation_matrix_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     6311 2023-10-08 16:08:47.000000 grav_toolbox-0.2.8/gravtools/gui/gui_model_results_drift_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    14740 2024-04-16 17:51:39.000000 grav_toolbox-0.2.8/gravtools/gui/gui_model_results_obs_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    11739 2023-10-08 16:08:47.000000 grav_toolbox-0.2.8/gravtools/gui/gui_model_results_stat_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     5454 2023-10-08 16:08:47.000000 grav_toolbox-0.2.8/gravtools/gui/gui_model_results_vg_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    10784 2024-04-16 17:51:39.000000 grav_toolbox-0.2.8/gravtools/gui/gui_model_setup_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     9716 2024-01-22 17:59:38.000000 grav_toolbox-0.2.8/gravtools/gui/gui_model_station_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    10556 2024-01-26 10:29:01.000000 grav_toolbox-0.2.8/gravtools/gui/gui_model_survey_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     5771 2024-02-21 10:08:41.000000 grav_toolbox-0.2.8/gravtools/gui/gui_models_gravimeters_scale_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1806 2023-10-08 16:10:22.000000 grav_toolbox-0.2.8/gravtools/gui/survey_table_handler.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2024-04-16 17:54:45.622567 grav_toolbox-0.2.8/gravtools/models/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1166 2023-10-08 16:08:47.000000 grav_toolbox-0.2.8/gravtools/models/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     3978 2023-10-08 16:08:47.000000 grav_toolbox-0.2.8/gravtools/models/atmosphere_correction.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    55890 2024-03-06 14:26:12.000000 grav_toolbox-0.2.8/gravtools/models/campaign.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1695 2023-10-08 16:08:47.000000 grav_toolbox-0.2.8/gravtools/models/exceptions.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    20441 2024-02-21 11:53:38.000000 grav_toolbox-0.2.8/gravtools/models/gravimeter.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    42262 2024-02-21 13:13:33.000000 grav_toolbox-0.2.8/gravtools/models/lsm.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    40159 2024-03-06 09:10:44.000000 grav_toolbox-0.2.8/gravtools/models/lsm_diff.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    36774 2024-03-06 09:10:44.000000 grav_toolbox-0.2.8/gravtools/models/lsm_nondiff.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     4117 2024-03-06 09:10:44.000000 grav_toolbox-0.2.8/gravtools/models/misc.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    19052 2024-01-26 10:29:01.000000 grav_toolbox-0.2.8/gravtools/models/mlr_bev_legacy.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    22830 2024-02-20 10:24:49.000000 grav_toolbox-0.2.8/gravtools/models/station.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)   122167 2024-04-16 17:51:39.000000 grav_toolbox-0.2.8/gravtools/models/survey.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    33704 2024-03-06 09:10:44.000000 grav_toolbox-0.2.8/gravtools/models/vg_lsm.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2024-04-16 17:54:45.622567 grav_toolbox-0.2.8/gravtools/scripts/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1064 2023-10-08 16:08:47.000000 grav_toolbox-0.2.8/gravtools/scripts/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1893 2023-10-08 16:08:47.000000 grav_toolbox-0.2.8/gravtools/scripts/create_correction_time_seriens_from_tsf.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1481 2023-10-08 16:08:47.000000 grav_toolbox-0.2.8/gravtools/scripts/load_tfs_file.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)      884 2023-10-08 16:08:47.000000 grav_toolbox-0.2.8/gravtools/scripts/run_gui.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)    14627 2024-03-06 09:10:44.000000 grav_toolbox-0.2.8/gravtools/settings.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2024-04-16 17:54:45.622567 grav_toolbox-0.2.8/gravtools/tides/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1090 2023-10-08 16:08:47.000000 grav_toolbox-0.2.8/gravtools/tides/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    16241 2024-01-15 16:13:37.000000 grav_toolbox-0.2.8/gravtools/tides/correction_time_series.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    16019 2023-10-08 16:08:47.000000 grav_toolbox-0.2.8/gravtools/tides/longman1959.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     3413 2023-10-08 16:08:47.000000 grav_toolbox-0.2.8/gravtools/tides/tide_data.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    18006 2024-01-15 16:13:37.000000 grav_toolbox-0.2.8/gravtools/tides/tide_data_tfs.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)       89 2023-10-08 16:08:47.000000 grav_toolbox-0.2.8/pyproject.toml
+-rw-rw-r--   0 heller    (1000) heller    (1000)      917 2024-04-16 17:54:45.622567 grav_toolbox-0.2.8/setup.cfg
```

### Comparing `grav-toolbox-0.2.7/LICENSE` & `grav_toolbox-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/PKG-INFO` & `grav_toolbox-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grav-toolbox
-Version: 0.2.7
+Version: 0.2.8
 Summary: Gravity survey utility tools
 Home-page: https://github.com/ahellers/GravTools
 Author: Andreas Hellerschmied
 Author-email: andreas.hellerschmied@bev.gv.at
 License: GNU GPLv3
 Keywords: gravity,gravimeter,least squares adjustment,geodesy,geophysics
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `grav-toolbox-0.2.7/README.md` & `grav_toolbox-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/bev_legacy/adjust.py` & `grav_toolbox-0.2.8/bev_legacy/adjust.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/bev_legacy/adjust_reilly1970.py` & `grav_toolbox-0.2.8/bev_legacy/adjust_reilly1970.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/bev_legacy/command_line.py` & `grav_toolbox-0.2.8/bev_legacy/command_line.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/bev_legacy/drift_mlr.py` & `grav_toolbox-0.2.8/bev_legacy/drift_mlr.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/bev_legacy/init.py` & `grav_toolbox-0.2.8/bev_legacy/init.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/bev_legacy/output.py` & `grav_toolbox-0.2.8/bev_legacy/output.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/bev_legacy/plots.py` & `grav_toolbox-0.2.8/bev_legacy/plots.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/bev_legacy/schwaus.py` & `grav_toolbox-0.2.8/bev_legacy/schwaus.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/bev_legacy/settings.py` & `grav_toolbox-0.2.8/bev_legacy/settings.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/bev_legacy/utils.py` & `grav_toolbox-0.2.8/bev_legacy/utils.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/grav_toolbox.egg-info/PKG-INFO` & `grav_toolbox-0.2.8/grav_toolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grav-toolbox
-Version: 0.2.7
+Version: 0.2.8
 Summary: Gravity survey utility tools
 Home-page: https://github.com/ahellers/GravTools
 Author: Andreas Hellerschmied
 Author-email: andreas.hellerschmied@bev.gv.at
 License: GNU GPLv3
 Keywords: gravity,gravimeter,least squares adjustment,geodesy,geophysics
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `grav-toolbox-0.2.7/grav_toolbox.egg-info/SOURCES.txt` & `grav_toolbox-0.2.8/grav_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/CG5_utils/__init__.py` & `grav_toolbox-0.2.8/gravtools/CG5_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/CG5_utils/cg5_survey.py` & `grav_toolbox-0.2.8/gravtools/CG5_utils/cg5_survey.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/__init__.py` & `grav_toolbox-0.2.8/gravtools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,13 +22,13 @@
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 :Authors:
     Andreas Hellerschmied (andreas.hellerschmied@bev.gv.at)
 """
 
-__version__ = '0.2.7'
+__version__ = '0.2.8'
 __author__ = 'Andreas Hellerschmied'
 __git_repo__ = 'https://github.com/ahellers/GravTools'
 __pypi_repo__ = 'https://pypi.org/project/grav-toolbox/'
 __email__ = 'andreas.hellerschmied@bev.gv.at'
 __copyright__ = '(c) 2022 Andreas Hellerschmied'
```

### Comparing `grav-toolbox-0.2.7/gravtools/const.py` & `grav_toolbox-0.2.8/gravtools/const.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/gui/MainWindow.py` & `grav_toolbox-0.2.8/gravtools/gui/MainWindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,5506 +35,5639 @@
 00000220: 7365 6c66 2e63 656e 7472 616c 7769 6467  self.centralwidg
 00000230: 6574 203d 2051 7457 6964 6765 7473 2e51  et = QtWidgets.Q
 00000240: 5769 6467 6574 284d 6169 6e57 696e 646f  Widget(MainWindo
 00000250: 7729 0a20 2020 2020 2020 2073 656c 662e  w).        self.
 00000260: 6365 6e74 7261 6c77 6964 6765 742e 7365  centralwidget.se
 00000270: 744f 626a 6563 744e 616d 6528 2263 656e  tObjectName("cen
 00000280: 7472 616c 7769 6467 6574 2229 0a20 2020  tralwidget").   
-00000290: 2020 2020 2073 656c 662e 686f 7269 7a6f       self.horizo
-000002a0: 6e74 616c 4c61 796f 7574 5f35 203d 2051  ntalLayout_5 = Q
-000002b0: 7457 6964 6765 7473 2e51 4842 6f78 4c61  tWidgets.QHBoxLa
-000002c0: 796f 7574 2873 656c 662e 6365 6e74 7261  yout(self.centra
-000002d0: 6c77 6964 6765 7429 0a20 2020 2020 2020  lwidget).       
-000002e0: 2073 656c 662e 686f 7269 7a6f 6e74 616c   self.horizontal
-000002f0: 4c61 796f 7574 5f35 2e73 6574 4f62 6a65  Layout_5.setObje
-00000300: 6374 4e61 6d65 2822 686f 7269 7a6f 6e74  ctName("horizont
-00000310: 616c 4c61 796f 7574 5f35 2229 0a20 2020  alLayout_5").   
-00000320: 2020 2020 2073 656c 662e 7461 6257 6964       self.tabWid
-00000330: 6765 745f 4d61 696e 203d 2051 7457 6964  get_Main = QtWid
-00000340: 6765 7473 2e51 5461 6257 6964 6765 7428  gets.QTabWidget(
-00000350: 7365 6c66 2e63 656e 7472 616c 7769 6467  self.centralwidg
-00000360: 6574 290a 2020 2020 2020 2020 7365 6c66  et).        self
-00000370: 2e74 6162 5769 6467 6574 5f4d 6169 6e2e  .tabWidget_Main.
-00000380: 7365 7454 6162 506f 7369 7469 6f6e 2851  setTabPosition(Q
-00000390: 7457 6964 6765 7473 2e51 5461 6257 6964  tWidgets.QTabWid
-000003a0: 6765 742e 4561 7374 290a 2020 2020 2020  get.East).      
-000003b0: 2020 7365 6c66 2e74 6162 5769 6467 6574    self.tabWidget
-000003c0: 5f4d 6169 6e2e 7365 744d 6f76 6162 6c65  _Main.setMovable
-000003d0: 2854 7275 6529 0a20 2020 2020 2020 2073  (True).        s
-000003e0: 656c 662e 7461 6257 6964 6765 745f 4d61  elf.tabWidget_Ma
-000003f0: 696e 2e73 6574 4f62 6a65 6374 4e61 6d65  in.setObjectName
-00000400: 2822 7461 6257 6964 6765 745f 4d61 696e  ("tabWidget_Main
-00000410: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00000420: 7461 625f 6d61 696e 5f73 7461 7469 6f6e  tab_main_station
-00000430: 7320 3d20 5174 5769 6467 6574 732e 5157  s = QtWidgets.QW
-00000440: 6964 6765 7428 290a 2020 2020 2020 2020  idget().        
-00000450: 7365 6c66 2e74 6162 5f6d 6169 6e5f 7374  self.tab_main_st
-00000460: 6174 696f 6e73 2e73 6574 4f62 6a65 6374  ations.setObject
-00000470: 4e61 6d65 2822 7461 625f 6d61 696e 5f73  Name("tab_main_s
-00000480: 7461 7469 6f6e 7322 290a 2020 2020 2020  tations").      
-00000490: 2020 7365 6c66 2e76 6572 7469 6361 6c4c    self.verticalL
-000004a0: 6179 6f75 745f 3420 3d20 5174 5769 6467  ayout_4 = QtWidg
-000004b0: 6574 732e 5156 426f 784c 6179 6f75 7428  ets.QVBoxLayout(
-000004c0: 7365 6c66 2e74 6162 5f6d 6169 6e5f 7374  self.tab_main_st
-000004d0: 6174 696f 6e73 290a 2020 2020 2020 2020  ations).        
-000004e0: 7365 6c66 2e76 6572 7469 6361 6c4c 6179  self.verticalLay
-000004f0: 6f75 745f 342e 7365 744f 626a 6563 744e  out_4.setObjectN
-00000500: 616d 6528 2276 6572 7469 6361 6c4c 6179  ame("verticalLay
-00000510: 6f75 745f 3422 290a 2020 2020 2020 2020  out_4").        
-00000520: 7365 6c66 2e68 6f72 697a 6f6e 7461 6c4c  self.horizontalL
-00000530: 6179 6f75 745f 3220 3d20 5174 5769 6467  ayout_2 = QtWidg
-00000540: 6574 732e 5148 426f 784c 6179 6f75 7428  ets.QHBoxLayout(
-00000550: 290a 2020 2020 2020 2020 7365 6c66 2e68  ).        self.h
-00000560: 6f72 697a 6f6e 7461 6c4c 6179 6f75 745f  orizontalLayout_
-00000570: 322e 7365 744f 626a 6563 744e 616d 6528  2.setObjectName(
-00000580: 2268 6f72 697a 6f6e 7461 6c4c 6179 6f75  "horizontalLayou
-00000590: 745f 3222 290a 2020 2020 2020 2020 7365  t_2").        se
-000005a0: 6c66 2e76 6572 7469 6361 6c4c 6179 6f75  lf.verticalLayou
-000005b0: 745f 3320 3d20 5174 5769 6467 6574 732e  t_3 = QtWidgets.
-000005c0: 5156 426f 784c 6179 6f75 7428 290a 2020  QVBoxLayout().  
-000005d0: 2020 2020 2020 7365 6c66 2e76 6572 7469        self.verti
-000005e0: 6361 6c4c 6179 6f75 745f 332e 7365 744f  calLayout_3.setO
-000005f0: 626a 6563 744e 616d 6528 2276 6572 7469  bjectName("verti
-00000600: 6361 6c4c 6179 6f75 745f 3322 290a 2020  calLayout_3").  
-00000610: 2020 2020 2020 7365 6c66 2e67 726f 7570        self.group
-00000620: 426f 785f 6669 6c74 6572 5f6f 7074 696f  Box_filter_optio
-00000630: 6e73 203d 2051 7457 6964 6765 7473 2e51  ns = QtWidgets.Q
-00000640: 4772 6f75 7042 6f78 2873 656c 662e 7461  GroupBox(self.ta
-00000650: 625f 6d61 696e 5f73 7461 7469 6f6e 7329  b_main_stations)
-00000660: 0a20 2020 2020 2020 2073 656c 662e 6772  .        self.gr
-00000670: 6f75 7042 6f78 5f66 696c 7465 725f 6f70  oupBox_filter_op
-00000680: 7469 6f6e 732e 7365 7445 6e61 626c 6564  tions.setEnabled
-00000690: 2846 616c 7365 290a 2020 2020 2020 2020  (False).        
-000006a0: 7365 6c66 2e67 726f 7570 426f 785f 6669  self.groupBox_fi
-000006b0: 6c74 6572 5f6f 7074 696f 6e73 2e73 6574  lter_options.set
-000006c0: 466c 6174 2846 616c 7365 290a 2020 2020  Flat(False).    
-000006d0: 2020 2020 7365 6c66 2e67 726f 7570 426f      self.groupBo
-000006e0: 785f 6669 6c74 6572 5f6f 7074 696f 6e73  x_filter_options
-000006f0: 2e73 6574 4368 6563 6b61 626c 6528 4661  .setCheckable(Fa
-00000700: 6c73 6529 0a20 2020 2020 2020 2073 656c  lse).        sel
-00000710: 662e 6772 6f75 7042 6f78 5f66 696c 7465  f.groupBox_filte
-00000720: 725f 6f70 7469 6f6e 732e 7365 744f 626a  r_options.setObj
-00000730: 6563 744e 616d 6528 2267 726f 7570 426f  ectName("groupBo
-00000740: 785f 6669 6c74 6572 5f6f 7074 696f 6e73  x_filter_options
-00000750: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00000760: 7665 7274 6963 616c 4c61 796f 7574 5f32  verticalLayout_2
-00000770: 203d 2051 7457 6964 6765 7473 2e51 5642   = QtWidgets.QVB
-00000780: 6f78 4c61 796f 7574 2873 656c 662e 6772  oxLayout(self.gr
-00000790: 6f75 7042 6f78 5f66 696c 7465 725f 6f70  oupBox_filter_op
-000007a0: 7469 6f6e 7329 0a20 2020 2020 2020 2073  tions).        s
-000007b0: 656c 662e 7665 7274 6963 616c 4c61 796f  elf.verticalLayo
-000007c0: 7574 5f32 2e73 6574 4f62 6a65 6374 4e61  ut_2.setObjectNa
-000007d0: 6d65 2822 7665 7274 6963 616c 4c61 796f  me("verticalLayo
-000007e0: 7574 5f32 2229 0a20 2020 2020 2020 2073  ut_2").        s
-000007f0: 656c 662e 6368 6563 6b42 6f78 5f66 696c  elf.checkBox_fil
-00000800: 7465 725f 6f62 7365 7276 6564 5f73 7461  ter_observed_sta
-00000810: 745f 6f6e 6c79 203d 2051 7457 6964 6765  t_only = QtWidge
-00000820: 7473 2e51 4368 6563 6b42 6f78 2873 656c  ts.QCheckBox(sel
-00000830: 662e 6772 6f75 7042 6f78 5f66 696c 7465  f.groupBox_filte
-00000840: 725f 6f70 7469 6f6e 7329 0a20 2020 2020  r_options).     
-00000850: 2020 2073 656c 662e 6368 6563 6b42 6f78     self.checkBox
-00000860: 5f66 696c 7465 725f 6f62 7365 7276 6564  _filter_observed
-00000870: 5f73 7461 745f 6f6e 6c79 2e73 6574 4368  _stat_only.setCh
-00000880: 6563 6b65 6428 5472 7565 290a 2020 2020  ecked(True).    
-00000890: 2020 2020 7365 6c66 2e63 6865 636b 426f      self.checkBo
-000008a0: 785f 6669 6c74 6572 5f6f 6273 6572 7665  x_filter_observe
-000008b0: 645f 7374 6174 5f6f 6e6c 792e 7365 744f  d_stat_only.setO
-000008c0: 626a 6563 744e 616d 6528 2263 6865 636b  bjectName("check
-000008d0: 426f 785f 6669 6c74 6572 5f6f 6273 6572  Box_filter_obser
-000008e0: 7665 645f 7374 6174 5f6f 6e6c 7922 290a  ved_stat_only").
-000008f0: 2020 2020 2020 2020 7365 6c66 2e76 6572          self.ver
-00000900: 7469 6361 6c4c 6179 6f75 745f 322e 6164  ticalLayout_2.ad
-00000910: 6457 6964 6765 7428 7365 6c66 2e63 6865  dWidget(self.che
-00000920: 636b 426f 785f 6669 6c74 6572 5f6f 6273  ckBox_filter_obs
-00000930: 6572 7665 645f 7374 6174 5f6f 6e6c 7929  erved_stat_only)
-00000940: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
-00000950: 6265 6c20 3d20 5174 5769 6467 6574 732e  bel = QtWidgets.
-00000960: 514c 6162 656c 2873 656c 662e 6772 6f75  QLabel(self.grou
-00000970: 7042 6f78 5f66 696c 7465 725f 6f70 7469  pBox_filter_opti
-00000980: 6f6e 7329 0a20 2020 2020 2020 2073 656c  ons).        sel
-00000990: 662e 6c61 6265 6c2e 7365 744f 626a 6563  f.label.setObjec
-000009a0: 744e 616d 6528 226c 6162 656c 2229 0a20  tName("label"). 
-000009b0: 2020 2020 2020 2073 656c 662e 7665 7274         self.vert
-000009c0: 6963 616c 4c61 796f 7574 5f32 2e61 6464  icalLayout_2.add
-000009d0: 5769 6467 6574 2873 656c 662e 6c61 6265  Widget(self.labe
-000009e0: 6c29 0a20 2020 2020 2020 2073 656c 662e  l).        self.
-000009f0: 6c69 6e65 4564 6974 5f66 696c 7465 725f  lineEdit_filter_
-00000a00: 7374 6174 5f6e 616d 6520 3d20 5174 5769  stat_name = QtWi
-00000a10: 6467 6574 732e 514c 696e 6545 6469 7428  dgets.QLineEdit(
-00000a20: 7365 6c66 2e67 726f 7570 426f 785f 6669  self.groupBox_fi
-00000a30: 6c74 6572 5f6f 7074 696f 6e73 290a 2020  lter_options).  
-00000a40: 2020 2020 2020 7365 6c66 2e6c 696e 6545        self.lineE
-00000a50: 6469 745f 6669 6c74 6572 5f73 7461 745f  dit_filter_stat_
-00000a60: 6e61 6d65 2e73 6574 5465 7874 2822 2229  name.setText("")
-00000a70: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00000a80: 6e65 4564 6974 5f66 696c 7465 725f 7374  neEdit_filter_st
-00000a90: 6174 5f6e 616d 652e 7365 744f 626a 6563  at_name.setObjec
-00000aa0: 744e 616d 6528 226c 696e 6545 6469 745f  tName("lineEdit_
-00000ab0: 6669 6c74 6572 5f73 7461 745f 6e61 6d65  filter_stat_name
-00000ac0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00000ad0: 7665 7274 6963 616c 4c61 796f 7574 5f32  verticalLayout_2
-00000ae0: 2e61 6464 5769 6467 6574 2873 656c 662e  .addWidget(self.
-00000af0: 6c69 6e65 4564 6974 5f66 696c 7465 725f  lineEdit_filter_
-00000b00: 7374 6174 5f6e 616d 6529 0a20 2020 2020  stat_name).     
-00000b10: 2020 2073 656c 662e 7665 7274 6963 616c     self.vertical
-00000b20: 4c61 796f 7574 5f33 2e61 6464 5769 6467  Layout_3.addWidg
-00000b30: 6574 2873 656c 662e 6772 6f75 7042 6f78  et(self.groupBox
-00000b40: 5f66 696c 7465 725f 6f70 7469 6f6e 7329  _filter_options)
-00000b50: 0a20 2020 2020 2020 2073 656c 662e 6772  .        self.gr
-00000b60: 6f75 7042 6f78 5f73 7461 7469 6f6e 735f  oupBox_stations_
-00000b70: 6d61 705f 7669 6577 5f6f 7074 696f 6e73  map_view_options
-00000b80: 203d 2051 7457 6964 6765 7473 2e51 4772   = QtWidgets.QGr
-00000b90: 6f75 7042 6f78 2873 656c 662e 7461 625f  oupBox(self.tab_
-00000ba0: 6d61 696e 5f73 7461 7469 6f6e 7329 0a20  main_stations). 
-00000bb0: 2020 2020 2020 2073 656c 662e 6772 6f75         self.grou
-00000bc0: 7042 6f78 5f73 7461 7469 6f6e 735f 6d61  pBox_stations_ma
-00000bd0: 705f 7669 6577 5f6f 7074 696f 6e73 2e73  p_view_options.s
-00000be0: 6574 456e 6162 6c65 6428 4661 6c73 6529  etEnabled(False)
-00000bf0: 0a20 2020 2020 2020 2073 656c 662e 6772  .        self.gr
-00000c00: 6f75 7042 6f78 5f73 7461 7469 6f6e 735f  oupBox_stations_
-00000c10: 6d61 705f 7669 6577 5f6f 7074 696f 6e73  map_view_options
-00000c20: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
-00000c30: 6772 6f75 7042 6f78 5f73 7461 7469 6f6e  groupBox_station
-00000c40: 735f 6d61 705f 7669 6577 5f6f 7074 696f  s_map_view_optio
-00000c50: 6e73 2229 0a20 2020 2020 2020 2073 656c  ns").        sel
-00000c60: 662e 7665 7274 6963 616c 4c61 796f 7574  f.verticalLayout
-00000c70: 5f33 3120 3d20 5174 5769 6467 6574 732e  _31 = QtWidgets.
-00000c80: 5156 426f 784c 6179 6f75 7428 7365 6c66  QVBoxLayout(self
-00000c90: 2e67 726f 7570 426f 785f 7374 6174 696f  .groupBox_statio
-00000ca0: 6e73 5f6d 6170 5f76 6965 775f 6f70 7469  ns_map_view_opti
-00000cb0: 6f6e 7329 0a20 2020 2020 2020 2073 656c  ons).        sel
-00000cc0: 662e 7665 7274 6963 616c 4c61 796f 7574  f.verticalLayout
-00000cd0: 5f33 312e 7365 744f 626a 6563 744e 616d  _31.setObjectNam
-00000ce0: 6528 2276 6572 7469 6361 6c4c 6179 6f75  e("verticalLayou
-00000cf0: 745f 3331 2229 0a20 2020 2020 2020 2073  t_31").        s
-00000d00: 656c 662e 6368 6563 6b42 6f78 5f73 7461  elf.checkBox_sta
-00000d10: 7469 6f6e 735f 6d61 705f 7368 6f77 5f73  tions_map_show_s
-00000d20: 7461 745f 6e61 6d65 5f6c 6162 656c 7320  tat_name_labels 
-00000d30: 3d20 5174 5769 6467 6574 732e 5143 6865  = QtWidgets.QChe
-00000d40: 636b 426f 7828 7365 6c66 2e67 726f 7570  ckBox(self.group
-00000d50: 426f 785f 7374 6174 696f 6e73 5f6d 6170  Box_stations_map
-00000d60: 5f76 6965 775f 6f70 7469 6f6e 7329 0a20  _view_options). 
-00000d70: 2020 2020 2020 2073 656c 662e 6368 6563         self.chec
-00000d80: 6b42 6f78 5f73 7461 7469 6f6e 735f 6d61  kBox_stations_ma
-00000d90: 705f 7368 6f77 5f73 7461 745f 6e61 6d65  p_show_stat_name
-00000da0: 5f6c 6162 656c 732e 7365 7443 6865 636b  _labels.setCheck
-00000db0: 6564 2854 7275 6529 0a20 2020 2020 2020  ed(True).       
-00000dc0: 2073 656c 662e 6368 6563 6b42 6f78 5f73   self.checkBox_s
-00000dd0: 7461 7469 6f6e 735f 6d61 705f 7368 6f77  tations_map_show
-00000de0: 5f73 7461 745f 6e61 6d65 5f6c 6162 656c  _stat_name_label
-00000df0: 732e 7365 744f 626a 6563 744e 616d 6528  s.setObjectName(
-00000e00: 2263 6865 636b 426f 785f 7374 6174 696f  "checkBox_statio
-00000e10: 6e73 5f6d 6170 5f73 686f 775f 7374 6174  ns_map_show_stat
-00000e20: 5f6e 616d 655f 6c61 6265 6c73 2229 0a20  _name_labels"). 
-00000e30: 2020 2020 2020 2073 656c 662e 7665 7274         self.vert
-00000e40: 6963 616c 4c61 796f 7574 5f33 312e 6164  icalLayout_31.ad
-00000e50: 6457 6964 6765 7428 7365 6c66 2e63 6865  dWidget(self.che
-00000e60: 636b 426f 785f 7374 6174 696f 6e73 5f6d  ckBox_stations_m
-00000e70: 6170 5f73 686f 775f 7374 6174 5f6e 616d  ap_show_stat_nam
-00000e80: 655f 6c61 6265 6c73 290a 2020 2020 2020  e_labels).      
-00000e90: 2020 7365 6c66 2e63 6865 636b 426f 785f    self.checkBox_
-00000ea0: 7374 6174 696f 6e73 5f70 6c6f 745f 6f62  stations_plot_ob
-00000eb0: 735f 6d61 7020 3d20 5174 5769 6467 6574  s_map = QtWidget
-00000ec0: 732e 5143 6865 636b 426f 7828 7365 6c66  s.QCheckBox(self
-00000ed0: 2e67 726f 7570 426f 785f 7374 6174 696f  .groupBox_statio
-00000ee0: 6e73 5f6d 6170 5f76 6965 775f 6f70 7469  ns_map_view_opti
-00000ef0: 6f6e 7329 0a20 2020 2020 2020 2073 656c  ons).        sel
-00000f00: 662e 6368 6563 6b42 6f78 5f73 7461 7469  f.checkBox_stati
-00000f10: 6f6e 735f 706c 6f74 5f6f 6273 5f6d 6170  ons_plot_obs_map
-00000f20: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
-00000f30: 6368 6563 6b42 6f78 5f73 7461 7469 6f6e  checkBox_station
-00000f40: 735f 706c 6f74 5f6f 6273 5f6d 6170 2229  s_plot_obs_map")
-00000f50: 0a20 2020 2020 2020 2073 656c 662e 7665  .        self.ve
-00000f60: 7274 6963 616c 4c61 796f 7574 5f33 312e  rticalLayout_31.
-00000f70: 6164 6457 6964 6765 7428 7365 6c66 2e63  addWidget(self.c
-00000f80: 6865 636b 426f 785f 7374 6174 696f 6e73  heckBox_stations
-00000f90: 5f70 6c6f 745f 6f62 735f 6d61 7029 0a20  _plot_obs_map). 
-00000fa0: 2020 2020 2020 2073 656c 662e 636f 6d62         self.comb
-00000fb0: 6f42 6f78 5f73 7461 7469 6f6e 735f 706c  oBox_stations_pl
-00000fc0: 6f74 5f6f 6273 5f6d 6170 5f73 7572 7665  ot_obs_map_surve
-00000fd0: 7973 203d 2051 7457 6964 6765 7473 2e51  ys = QtWidgets.Q
-00000fe0: 436f 6d62 6f42 6f78 2873 656c 662e 6772  ComboBox(self.gr
-00000ff0: 6f75 7042 6f78 5f73 7461 7469 6f6e 735f  oupBox_stations_
-00001000: 6d61 705f 7669 6577 5f6f 7074 696f 6e73  map_view_options
-00001010: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
-00001020: 6f6d 626f 426f 785f 7374 6174 696f 6e73  omboBox_stations
-00001030: 5f70 6c6f 745f 6f62 735f 6d61 705f 7375  _plot_obs_map_su
-00001040: 7276 6579 732e 7365 7445 6e61 626c 6564  rveys.setEnabled
-00001050: 2846 616c 7365 290a 2020 2020 2020 2020  (False).        
-00001060: 7365 6c66 2e63 6f6d 626f 426f 785f 7374  self.comboBox_st
-00001070: 6174 696f 6e73 5f70 6c6f 745f 6f62 735f  ations_plot_obs_
-00001080: 6d61 705f 7375 7276 6579 732e 7365 744f  map_surveys.setO
-00001090: 626a 6563 744e 616d 6528 2263 6f6d 626f  bjectName("combo
-000010a0: 426f 785f 7374 6174 696f 6e73 5f70 6c6f  Box_stations_plo
-000010b0: 745f 6f62 735f 6d61 705f 7375 7276 6579  t_obs_map_survey
-000010c0: 7322 290a 2020 2020 2020 2020 7365 6c66  s").        self
-000010d0: 2e76 6572 7469 6361 6c4c 6179 6f75 745f  .verticalLayout_
-000010e0: 3331 2e61 6464 5769 6467 6574 2873 656c  31.addWidget(sel
-000010f0: 662e 636f 6d62 6f42 6f78 5f73 7461 7469  f.comboBox_stati
-00001100: 6f6e 735f 706c 6f74 5f6f 6273 5f6d 6170  ons_plot_obs_map
-00001110: 5f73 7572 7665 7973 290a 2020 2020 2020  _surveys).      
-00001120: 2020 7365 6c66 2e76 6572 7469 6361 6c4c    self.verticalL
-00001130: 6179 6f75 745f 332e 6164 6457 6964 6765  ayout_3.addWidge
-00001140: 7428 7365 6c66 2e67 726f 7570 426f 785f  t(self.groupBox_
-00001150: 7374 6174 696f 6e73 5f6d 6170 5f76 6965  stations_map_vie
-00001160: 775f 6f70 7469 6f6e 7329 0a20 2020 2020  w_options).     
-00001170: 2020 2073 7061 6365 7249 7465 6d20 3d20     spacerItem = 
-00001180: 5174 5769 6467 6574 732e 5153 7061 6365  QtWidgets.QSpace
-00001190: 7249 7465 6d28 3230 2c20 3430 2c20 5174  rItem(20, 40, Qt
-000011a0: 5769 6467 6574 732e 5153 697a 6550 6f6c  Widgets.QSizePol
-000011b0: 6963 792e 4d69 6e69 6d75 6d2c 2051 7457  icy.Minimum, QtW
-000011c0: 6964 6765 7473 2e51 5369 7a65 506f 6c69  idgets.QSizePoli
-000011d0: 6379 2e45 7870 616e 6469 6e67 290a 2020  cy.Expanding).  
-000011e0: 2020 2020 2020 7365 6c66 2e76 6572 7469        self.verti
-000011f0: 6361 6c4c 6179 6f75 745f 332e 6164 6449  calLayout_3.addI
-00001200: 7465 6d28 7370 6163 6572 4974 656d 290a  tem(spacerItem).
-00001210: 2020 2020 2020 2020 7365 6c66 2e68 6f72          self.hor
-00001220: 697a 6f6e 7461 6c4c 6179 6f75 745f 322e  izontalLayout_2.
-00001230: 6164 644c 6179 6f75 7428 7365 6c66 2e76  addLayout(self.v
-00001240: 6572 7469 6361 6c4c 6179 6f75 745f 3329  erticalLayout_3)
-00001250: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
-00001260: 625f 5769 6467 6574 5f53 7461 7469 6f6e  b_Widget_Station
-00001270: 7320 3d20 5174 5769 6467 6574 732e 5154  s = QtWidgets.QT
-00001280: 6162 5769 6467 6574 2873 656c 662e 7461  abWidget(self.ta
-00001290: 625f 6d61 696e 5f73 7461 7469 6f6e 7329  b_main_stations)
-000012a0: 0a20 2020 2020 2020 2073 697a 6550 6f6c  .        sizePol
-000012b0: 6963 7920 3d20 5174 5769 6467 6574 732e  icy = QtWidgets.
-000012c0: 5153 697a 6550 6f6c 6963 7928 5174 5769  QSizePolicy(QtWi
-000012d0: 6467 6574 732e 5153 697a 6550 6f6c 6963  dgets.QSizePolic
-000012e0: 792e 4578 7061 6e64 696e 672c 2051 7457  y.Expanding, QtW
-000012f0: 6964 6765 7473 2e51 5369 7a65 506f 6c69  idgets.QSizePoli
-00001300: 6379 2e45 7870 616e 6469 6e67 290a 2020  cy.Expanding).  
-00001310: 2020 2020 2020 7369 7a65 506f 6c69 6379        sizePolicy
-00001320: 2e73 6574 486f 7269 7a6f 6e74 616c 5374  .setHorizontalSt
-00001330: 7265 7463 6828 3029 0a20 2020 2020 2020  retch(0).       
-00001340: 2073 697a 6550 6f6c 6963 792e 7365 7456   sizePolicy.setV
-00001350: 6572 7469 6361 6c53 7472 6574 6368 2830  erticalStretch(0
-00001360: 290a 2020 2020 2020 2020 7369 7a65 506f  ).        sizePo
-00001370: 6c69 6379 2e73 6574 4865 6967 6874 466f  licy.setHeightFo
-00001380: 7257 6964 7468 2873 656c 662e 7461 625f  rWidth(self.tab_
-00001390: 5769 6467 6574 5f53 7461 7469 6f6e 732e  Widget_Stations.
-000013a0: 7369 7a65 506f 6c69 6379 2829 2e68 6173  sizePolicy().has
-000013b0: 4865 6967 6874 466f 7257 6964 7468 2829  HeightForWidth()
-000013c0: 290a 2020 2020 2020 2020 7365 6c66 2e74  ).        self.t
-000013d0: 6162 5f57 6964 6765 745f 5374 6174 696f  ab_Widget_Statio
-000013e0: 6e73 2e73 6574 5369 7a65 506f 6c69 6379  ns.setSizePolicy
-000013f0: 2873 697a 6550 6f6c 6963 7929 0a20 2020  (sizePolicy).   
-00001400: 2020 2020 2073 656c 662e 7461 625f 5769       self.tab_Wi
-00001410: 6467 6574 5f53 7461 7469 6f6e 732e 7365  dget_Stations.se
-00001420: 744f 626a 6563 744e 616d 6528 2274 6162  tObjectName("tab
-00001430: 5f57 6964 6765 745f 5374 6174 696f 6e73  _Widget_Stations
-00001440: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00001450: 7461 625f 5374 6174 696f 6e73 5f54 6162  tab_Stations_Tab
-00001460: 6c65 203d 2051 7457 6964 6765 7473 2e51  le = QtWidgets.Q
-00001470: 5769 6467 6574 2829 0a20 2020 2020 2020  Widget().       
-00001480: 2073 656c 662e 7461 625f 5374 6174 696f   self.tab_Statio
-00001490: 6e73 5f54 6162 6c65 2e73 6574 4f62 6a65  ns_Table.setObje
-000014a0: 6374 4e61 6d65 2822 7461 625f 5374 6174  ctName("tab_Stat
-000014b0: 696f 6e73 5f54 6162 6c65 2229 0a20 2020  ions_Table").   
-000014c0: 2020 2020 2073 656c 662e 7665 7274 6963       self.vertic
-000014d0: 616c 4c61 796f 7574 203d 2051 7457 6964  alLayout = QtWid
-000014e0: 6765 7473 2e51 5642 6f78 4c61 796f 7574  gets.QVBoxLayout
-000014f0: 2873 656c 662e 7461 625f 5374 6174 696f  (self.tab_Statio
-00001500: 6e73 5f54 6162 6c65 290a 2020 2020 2020  ns_Table).      
-00001510: 2020 7365 6c66 2e76 6572 7469 6361 6c4c    self.verticalL
-00001520: 6179 6f75 742e 7365 744f 626a 6563 744e  ayout.setObjectN
-00001530: 616d 6528 2276 6572 7469 6361 6c4c 6179  ame("verticalLay
-00001540: 6f75 7422 290a 2020 2020 2020 2020 7365  out").        se
-00001550: 6c66 2e74 6162 6c65 5669 6577 5f53 7461  lf.tableView_Sta
-00001560: 7469 6f6e 7320 3d20 5174 5769 6467 6574  tions = QtWidget
-00001570: 732e 5154 6162 6c65 5669 6577 2873 656c  s.QTableView(sel
-00001580: 662e 7461 625f 5374 6174 696f 6e73 5f54  f.tab_Stations_T
-00001590: 6162 6c65 290a 2020 2020 2020 2020 7365  able).        se
-000015a0: 6c66 2e74 6162 6c65 5669 6577 5f53 7461  lf.tableView_Sta
-000015b0: 7469 6f6e 732e 7365 7453 697a 6541 646a  tions.setSizeAdj
-000015c0: 7573 7450 6f6c 6963 7928 5174 5769 6467  ustPolicy(QtWidg
-000015d0: 6574 732e 5141 6273 7472 6163 7453 6372  ets.QAbstractScr
-000015e0: 6f6c 6c41 7265 612e 4164 6a75 7374 546f  ollArea.AdjustTo
-000015f0: 436f 6e74 656e 7473 290a 2020 2020 2020  Contents).      
-00001600: 2020 7365 6c66 2e74 6162 6c65 5669 6577    self.tableView
-00001610: 5f53 7461 7469 6f6e 732e 7365 744f 626a  _Stations.setObj
-00001620: 6563 744e 616d 6528 2274 6162 6c65 5669  ectName("tableVi
-00001630: 6577 5f53 7461 7469 6f6e 7322 290a 2020  ew_Stations").  
-00001640: 2020 2020 2020 7365 6c66 2e74 6162 6c65        self.table
-00001650: 5669 6577 5f53 7461 7469 6f6e 732e 686f  View_Stations.ho
-00001660: 7269 7a6f 6e74 616c 4865 6164 6572 2829  rizontalHeader()
-00001670: 2e73 6574 4361 7363 6164 696e 6753 6563  .setCascadingSec
-00001680: 7469 6f6e 5265 7369 7a65 7328 5472 7565  tionResizes(True
-00001690: 290a 2020 2020 2020 2020 7365 6c66 2e76  ).        self.v
-000016a0: 6572 7469 6361 6c4c 6179 6f75 742e 6164  erticalLayout.ad
-000016b0: 6457 6964 6765 7428 7365 6c66 2e74 6162  dWidget(self.tab
-000016c0: 6c65 5669 6577 5f53 7461 7469 6f6e 7329  leView_Stations)
-000016d0: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
-000016e0: 625f 5769 6467 6574 5f53 7461 7469 6f6e  b_Widget_Station
-000016f0: 732e 6164 6454 6162 2873 656c 662e 7461  s.addTab(self.ta
-00001700: 625f 5374 6174 696f 6e73 5f54 6162 6c65  b_Stations_Table
-00001710: 2c20 2222 290a 2020 2020 2020 2020 7365  , "").        se
-00001720: 6c66 2e74 6162 5f73 7461 7469 6f6e 735f  lf.tab_stations_
-00001730: 6d61 7020 3d20 5174 5769 6467 6574 732e  map = QtWidgets.
-00001740: 5157 6964 6765 7428 290a 2020 2020 2020  QWidget().      
-00001750: 2020 7365 6c66 2e74 6162 5f73 7461 7469    self.tab_stati
-00001760: 6f6e 735f 6d61 702e 7365 744f 626a 6563  ons_map.setObjec
-00001770: 744e 616d 6528 2274 6162 5f73 7461 7469  tName("tab_stati
-00001780: 6f6e 735f 6d61 7022 290a 2020 2020 2020  ons_map").      
-00001790: 2020 7365 6c66 2e76 6572 7469 6361 6c4c    self.verticalL
-000017a0: 6179 6f75 745f 3330 203d 2051 7457 6964  ayout_30 = QtWid
-000017b0: 6765 7473 2e51 5642 6f78 4c61 796f 7574  gets.QVBoxLayout
-000017c0: 2873 656c 662e 7461 625f 7374 6174 696f  (self.tab_statio
-000017d0: 6e73 5f6d 6170 290a 2020 2020 2020 2020  ns_map).        
-000017e0: 7365 6c66 2e76 6572 7469 6361 6c4c 6179  self.verticalLay
-000017f0: 6f75 745f 3330 2e73 6574 4f62 6a65 6374  out_30.setObject
-00001800: 4e61 6d65 2822 7665 7274 6963 616c 4c61  Name("verticalLa
-00001810: 796f 7574 5f33 3022 290a 2020 2020 2020  yout_30").      
-00001820: 2020 7365 6c66 2e47 7261 7068 6963 734c    self.GraphicsL
-00001830: 6179 6f75 7457 6964 6765 745f 7374 6174  ayoutWidget_stat
-00001840: 696f 6e73 5f6d 6170 203d 2047 7261 7068  ions_map = Graph
-00001850: 6963 734c 6179 6f75 7457 6964 6765 7428  icsLayoutWidget(
-00001860: 7365 6c66 2e74 6162 5f73 7461 7469 6f6e  self.tab_station
-00001870: 735f 6d61 7029 0a20 2020 2020 2020 2073  s_map).        s
-00001880: 656c 662e 4772 6170 6869 6373 4c61 796f  elf.GraphicsLayo
-00001890: 7574 5769 6467 6574 5f73 7461 7469 6f6e  utWidget_station
-000018a0: 735f 6d61 702e 7365 744f 626a 6563 744e  s_map.setObjectN
-000018b0: 616d 6528 2247 7261 7068 6963 734c 6179  ame("GraphicsLay
-000018c0: 6f75 7457 6964 6765 745f 7374 6174 696f  outWidget_statio
-000018d0: 6e73 5f6d 6170 2229 0a20 2020 2020 2020  ns_map").       
-000018e0: 2073 656c 662e 7665 7274 6963 616c 4c61   self.verticalLa
-000018f0: 796f 7574 5f33 302e 6164 6457 6964 6765  yout_30.addWidge
-00001900: 7428 7365 6c66 2e47 7261 7068 6963 734c  t(self.GraphicsL
-00001910: 6179 6f75 7457 6964 6765 745f 7374 6174  ayoutWidget_stat
-00001920: 696f 6e73 5f6d 6170 290a 2020 2020 2020  ions_map).      
-00001930: 2020 7365 6c66 2e74 6162 5f57 6964 6765    self.tab_Widge
-00001940: 745f 5374 6174 696f 6e73 2e61 6464 5461  t_Stations.addTa
-00001950: 6228 7365 6c66 2e74 6162 5f73 7461 7469  b(self.tab_stati
-00001960: 6f6e 735f 6d61 702c 2022 2229 0a20 2020  ons_map, "").   
-00001970: 2020 2020 2073 656c 662e 686f 7269 7a6f       self.horizo
-00001980: 6e74 616c 4c61 796f 7574 5f32 2e61 6464  ntalLayout_2.add
-00001990: 5769 6467 6574 2873 656c 662e 7461 625f  Widget(self.tab_
-000019a0: 5769 6467 6574 5f53 7461 7469 6f6e 7329  Widget_Stations)
-000019b0: 0a20 2020 2020 2020 2073 656c 662e 686f  .        self.ho
-000019c0: 7269 7a6f 6e74 616c 4c61 796f 7574 5f32  rizontalLayout_2
-000019d0: 2e73 6574 5374 7265 7463 6828 302c 2031  .setStretch(0, 1
-000019e0: 290a 2020 2020 2020 2020 7365 6c66 2e68  ).        self.h
-000019f0: 6f72 697a 6f6e 7461 6c4c 6179 6f75 745f  orizontalLayout_
-00001a00: 322e 7365 7453 7472 6574 6368 2831 2c20  2.setStretch(1, 
-00001a10: 3429 0a20 2020 2020 2020 2073 656c 662e  4).        self.
-00001a20: 7665 7274 6963 616c 4c61 796f 7574 5f34  verticalLayout_4
-00001a30: 2e61 6464 4c61 796f 7574 2873 656c 662e  .addLayout(self.
-00001a40: 686f 7269 7a6f 6e74 616c 4c61 796f 7574  horizontalLayout
-00001a50: 5f32 290a 2020 2020 2020 2020 7365 6c66  _2).        self
-00001a60: 2e74 6162 5769 6467 6574 5f4d 6169 6e2e  .tabWidget_Main.
-00001a70: 6164 6454 6162 2873 656c 662e 7461 625f  addTab(self.tab_
-00001a80: 6d61 696e 5f73 7461 7469 6f6e 732c 2022  main_stations, "
-00001a90: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00001aa0: 7461 625f 6d61 696e 5f67 7261 7669 6d65  tab_main_gravime
-00001ab0: 7465 7273 203d 2051 7457 6964 6765 7473  ters = QtWidgets
-00001ac0: 2e51 5769 6467 6574 2829 0a20 2020 2020  .QWidget().     
-00001ad0: 2020 2073 656c 662e 7461 625f 6d61 696e     self.tab_main
-00001ae0: 5f67 7261 7669 6d65 7465 7273 2e73 6574  _gravimeters.set
-00001af0: 4f62 6a65 6374 4e61 6d65 2822 7461 625f  ObjectName("tab_
-00001b00: 6d61 696e 5f67 7261 7669 6d65 7465 7273  main_gravimeters
-00001b10: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00001b20: 7665 7274 6963 616c 4c61 796f 7574 5f32  verticalLayout_2
-00001b30: 3820 3d20 5174 5769 6467 6574 732e 5156  8 = QtWidgets.QV
-00001b40: 426f 784c 6179 6f75 7428 7365 6c66 2e74  BoxLayout(self.t
-00001b50: 6162 5f6d 6169 6e5f 6772 6176 696d 6574  ab_main_gravimet
-00001b60: 6572 7329 0a20 2020 2020 2020 2073 656c  ers).        sel
-00001b70: 662e 7665 7274 6963 616c 4c61 796f 7574  f.verticalLayout
-00001b80: 5f32 382e 7365 744f 626a 6563 744e 616d  _28.setObjectNam
-00001b90: 6528 2276 6572 7469 6361 6c4c 6179 6f75  e("verticalLayou
-00001ba0: 745f 3238 2229 0a20 2020 2020 2020 2073  t_28").        s
-00001bb0: 656c 662e 7370 6c69 7474 6572 5f67 7261  elf.splitter_gra
-00001bc0: 7669 6d65 7465 7273 203d 2051 7457 6964  vimeters = QtWid
-00001bd0: 6765 7473 2e51 5370 6c69 7474 6572 2873  gets.QSplitter(s
-00001be0: 656c 662e 7461 625f 6d61 696e 5f67 7261  elf.tab_main_gra
-00001bf0: 7669 6d65 7465 7273 290a 2020 2020 2020  vimeters).      
-00001c00: 2020 7365 6c66 2e73 706c 6974 7465 725f    self.splitter_
-00001c10: 6772 6176 696d 6574 6572 732e 7365 744f  gravimeters.setO
-00001c20: 7269 656e 7461 7469 6f6e 2851 7443 6f72  rientation(QtCor
-00001c30: 652e 5174 2e48 6f72 697a 6f6e 7461 6c29  e.Qt.Horizontal)
-00001c40: 0a20 2020 2020 2020 2073 656c 662e 7370  .        self.sp
-00001c50: 6c69 7474 6572 5f67 7261 7669 6d65 7465  litter_gravimete
-00001c60: 7273 2e73 6574 4f62 6a65 6374 4e61 6d65  rs.setObjectName
-00001c70: 2822 7370 6c69 7474 6572 5f67 7261 7669  ("splitter_gravi
-00001c80: 6d65 7465 7273 2229 0a20 2020 2020 2020  meters").       
-00001c90: 2073 656c 662e 6c61 796f 7574 5769 6467   self.layoutWidg
-00001ca0: 6574 203d 2051 7457 6964 6765 7473 2e51  et = QtWidgets.Q
-00001cb0: 5769 6467 6574 2873 656c 662e 7370 6c69  Widget(self.spli
-00001cc0: 7474 6572 5f67 7261 7669 6d65 7465 7273  tter_gravimeters
-00001cd0: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
-00001ce0: 6179 6f75 7457 6964 6765 742e 7365 744f  ayoutWidget.setO
-00001cf0: 626a 6563 744e 616d 6528 226c 6179 6f75  bjectName("layou
-00001d00: 7457 6964 6765 7422 290a 2020 2020 2020  tWidget").      
-00001d10: 2020 7365 6c66 2e76 6572 7469 6361 6c4c    self.verticalL
-00001d20: 6179 6f75 745f 3430 203d 2051 7457 6964  ayout_40 = QtWid
-00001d30: 6765 7473 2e51 5642 6f78 4c61 796f 7574  gets.QVBoxLayout
-00001d40: 2873 656c 662e 6c61 796f 7574 5769 6467  (self.layoutWidg
-00001d50: 6574 290a 2020 2020 2020 2020 7365 6c66  et).        self
-00001d60: 2e76 6572 7469 6361 6c4c 6179 6f75 745f  .verticalLayout_
-00001d70: 3430 2e73 6574 436f 6e74 656e 7473 4d61  40.setContentsMa
-00001d80: 7267 696e 7328 302c 2030 2c20 302c 2030  rgins(0, 0, 0, 0
-00001d90: 290a 2020 2020 2020 2020 7365 6c66 2e76  ).        self.v
-00001da0: 6572 7469 6361 6c4c 6179 6f75 745f 3430  erticalLayout_40
-00001db0: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
-00001dc0: 7665 7274 6963 616c 4c61 796f 7574 5f34  verticalLayout_4
-00001dd0: 3022 290a 2020 2020 2020 2020 7365 6c66  0").        self
-00001de0: 2e74 7265 6557 6964 6765 745f 6772 6176  .treeWidget_grav
-00001df0: 696d 6574 6572 7320 3d20 5174 5769 6467  imeters = QtWidg
-00001e00: 6574 732e 5154 7265 6557 6964 6765 7428  ets.QTreeWidget(
-00001e10: 7365 6c66 2e6c 6179 6f75 7457 6964 6765  self.layoutWidge
-00001e20: 7429 0a20 2020 2020 2020 2073 656c 662e  t).        self.
-00001e30: 7472 6565 5769 6467 6574 5f67 7261 7669  treeWidget_gravi
-00001e40: 6d65 7465 7273 2e73 6574 4865 6164 6572  meters.setHeader
-00001e50: 4869 6464 656e 2846 616c 7365 290a 2020  Hidden(False).  
-00001e60: 2020 2020 2020 7365 6c66 2e74 7265 6557        self.treeW
-00001e70: 6964 6765 745f 6772 6176 696d 6574 6572  idget_gravimeter
-00001e80: 732e 7365 7443 6f6c 756d 6e43 6f75 6e74  s.setColumnCount
-00001e90: 2832 290a 2020 2020 2020 2020 7365 6c66  (2).        self
-00001ea0: 2e74 7265 6557 6964 6765 745f 6772 6176  .treeWidget_grav
-00001eb0: 696d 6574 6572 732e 7365 744f 626a 6563  imeters.setObjec
-00001ec0: 744e 616d 6528 2274 7265 6557 6964 6765  tName("treeWidge
-00001ed0: 745f 6772 6176 696d 6574 6572 7322 290a  t_gravimeters").
-00001ee0: 2020 2020 2020 2020 7365 6c66 2e76 6572          self.ver
-00001ef0: 7469 6361 6c4c 6179 6f75 745f 3430 2e61  ticalLayout_40.a
-00001f00: 6464 5769 6467 6574 2873 656c 662e 7472  ddWidget(self.tr
-00001f10: 6565 5769 6467 6574 5f67 7261 7669 6d65  eeWidget_gravime
-00001f20: 7465 7273 290a 2020 2020 2020 2020 7365  ters).        se
-00001f30: 6c66 2e70 7573 6842 7574 746f 6e5f 6465  lf.pushButton_de
-00001f40: 6c65 7465 5f67 7261 7669 6d65 7465 7220  lete_gravimeter 
-00001f50: 3d20 5174 5769 6467 6574 732e 5150 7573  = QtWidgets.QPus
-00001f60: 6842 7574 746f 6e28 7365 6c66 2e6c 6179  hButton(self.lay
-00001f70: 6f75 7457 6964 6765 7429 0a20 2020 2020  outWidget).     
-00001f80: 2020 2073 656c 662e 7075 7368 4275 7474     self.pushButt
-00001f90: 6f6e 5f64 656c 6574 655f 6772 6176 696d  on_delete_gravim
-00001fa0: 6574 6572 2e73 6574 456e 6162 6c65 6428  eter.setEnabled(
-00001fb0: 4661 6c73 6529 0a20 2020 2020 2020 2073  False).        s
-00001fc0: 656c 662e 7075 7368 4275 7474 6f6e 5f64  elf.pushButton_d
-00001fd0: 656c 6574 655f 6772 6176 696d 6574 6572  elete_gravimeter
-00001fe0: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
-00001ff0: 7075 7368 4275 7474 6f6e 5f64 656c 6574  pushButton_delet
-00002000: 655f 6772 6176 696d 6574 6572 2229 0a20  e_gravimeter"). 
-00002010: 2020 2020 2020 2073 656c 662e 7665 7274         self.vert
-00002020: 6963 616c 4c61 796f 7574 5f34 302e 6164  icalLayout_40.ad
-00002030: 6457 6964 6765 7428 7365 6c66 2e70 7573  dWidget(self.pus
-00002040: 6842 7574 746f 6e5f 6465 6c65 7465 5f67  hButton_delete_g
-00002050: 7261 7669 6d65 7465 7229 0a20 2020 2020  ravimeter).     
-00002060: 2020 2073 656c 662e 7461 6257 6964 6765     self.tabWidge
-00002070: 745f 6772 6176 696d 6574 6572 7320 3d20  t_gravimeters = 
-00002080: 5174 5769 6467 6574 732e 5154 6162 5769  QtWidgets.QTabWi
-00002090: 6467 6574 2873 656c 662e 7370 6c69 7474  dget(self.splitt
-000020a0: 6572 5f67 7261 7669 6d65 7465 7273 290a  er_gravimeters).
-000020b0: 2020 2020 2020 2020 7369 7a65 506f 6c69          sizePoli
-000020c0: 6379 203d 2051 7457 6964 6765 7473 2e51  cy = QtWidgets.Q
-000020d0: 5369 7a65 506f 6c69 6379 2851 7457 6964  SizePolicy(QtWid
-000020e0: 6765 7473 2e51 5369 7a65 506f 6c69 6379  gets.QSizePolicy
-000020f0: 2e45 7870 616e 6469 6e67 2c20 5174 5769  .Expanding, QtWi
-00002100: 6467 6574 732e 5153 697a 6550 6f6c 6963  dgets.QSizePolic
-00002110: 792e 4578 7061 6e64 696e 6729 0a20 2020  y.Expanding).   
-00002120: 2020 2020 2073 697a 6550 6f6c 6963 792e       sizePolicy.
-00002130: 7365 7448 6f72 697a 6f6e 7461 6c53 7472  setHorizontalStr
-00002140: 6574 6368 2831 290a 2020 2020 2020 2020  etch(1).        
-00002150: 7369 7a65 506f 6c69 6379 2e73 6574 5665  sizePolicy.setVe
-00002160: 7274 6963 616c 5374 7265 7463 6828 3029  rticalStretch(0)
-00002170: 0a20 2020 2020 2020 2073 697a 6550 6f6c  .        sizePol
-00002180: 6963 792e 7365 7448 6569 6768 7446 6f72  icy.setHeightFor
-00002190: 5769 6474 6828 7365 6c66 2e74 6162 5769  Width(self.tabWi
-000021a0: 6467 6574 5f67 7261 7669 6d65 7465 7273  dget_gravimeters
-000021b0: 2e73 697a 6550 6f6c 6963 7928 292e 6861  .sizePolicy().ha
-000021c0: 7348 6569 6768 7446 6f72 5769 6474 6828  sHeightForWidth(
-000021d0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-000021e0: 7461 6257 6964 6765 745f 6772 6176 696d  tabWidget_gravim
-000021f0: 6574 6572 732e 7365 7453 697a 6550 6f6c  eters.setSizePol
-00002200: 6963 7928 7369 7a65 506f 6c69 6379 290a  icy(sizePolicy).
-00002210: 2020 2020 2020 2020 7365 6c66 2e74 6162          self.tab
-00002220: 5769 6467 6574 5f67 7261 7669 6d65 7465  Widget_gravimete
-00002230: 7273 2e73 6574 4f62 6a65 6374 4e61 6d65  rs.setObjectName
-00002240: 2822 7461 6257 6964 6765 745f 6772 6176  ("tabWidget_grav
-00002250: 696d 6574 6572 7322 290a 2020 2020 2020  imeters").      
-00002260: 2020 7365 6c66 2e74 6162 5f67 7261 7669    self.tab_gravi
-00002270: 6d65 7465 725f 696e 666f 203d 2051 7457  meter_info = QtW
-00002280: 6964 6765 7473 2e51 5769 6467 6574 2829  idgets.QWidget()
-00002290: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
-000022a0: 625f 6772 6176 696d 6574 6572 5f69 6e66  b_gravimeter_inf
-000022b0: 6f2e 7365 744f 626a 6563 744e 616d 6528  o.setObjectName(
-000022c0: 2274 6162 5f67 7261 7669 6d65 7465 725f  "tab_gravimeter_
-000022d0: 696e 666f 2229 0a20 2020 2020 2020 2073  info").        s
-000022e0: 656c 662e 7665 7274 6963 616c 4c61 796f  elf.verticalLayo
-000022f0: 7574 5f34 3220 3d20 5174 5769 6467 6574  ut_42 = QtWidget
-00002300: 732e 5156 426f 784c 6179 6f75 7428 7365  s.QVBoxLayout(se
-00002310: 6c66 2e74 6162 5f67 7261 7669 6d65 7465  lf.tab_gravimete
-00002320: 725f 696e 666f 290a 2020 2020 2020 2020  r_info).        
-00002330: 7365 6c66 2e76 6572 7469 6361 6c4c 6179  self.verticalLay
-00002340: 6f75 745f 3432 2e73 6574 4f62 6a65 6374  out_42.setObject
-00002350: 4e61 6d65 2822 7665 7274 6963 616c 4c61  Name("verticalLa
-00002360: 796f 7574 5f34 3222 290a 2020 2020 2020  yout_42").      
-00002370: 2020 7365 6c66 2e66 6f72 6d4c 6179 6f75    self.formLayou
-00002380: 745f 3132 203d 2051 7457 6964 6765 7473  t_12 = QtWidgets
-00002390: 2e51 466f 726d 4c61 796f 7574 2829 0a20  .QFormLayout(). 
-000023a0: 2020 2020 2020 2073 656c 662e 666f 726d         self.form
-000023b0: 4c61 796f 7574 5f31 322e 7365 744f 626a  Layout_12.setObj
-000023c0: 6563 744e 616d 6528 2266 6f72 6d4c 6179  ectName("formLay
-000023d0: 6f75 745f 3132 2229 0a20 2020 2020 2020  out_12").       
-000023e0: 2073 656c 662e 6c61 6265 6c5f 3139 203d   self.label_19 =
-000023f0: 2051 7457 6964 6765 7473 2e51 4c61 6265   QtWidgets.QLabe
-00002400: 6c28 7365 6c66 2e74 6162 5f67 7261 7669  l(self.tab_gravi
-00002410: 6d65 7465 725f 696e 666f 290a 2020 2020  meter_info).    
-00002420: 2020 2020 7365 6c66 2e6c 6162 656c 5f31      self.label_1
-00002430: 392e 7365 744f 626a 6563 744e 616d 6528  9.setObjectName(
-00002440: 226c 6162 656c 5f31 3922 290a 2020 2020  "label_19").    
-00002450: 2020 2020 7365 6c66 2e66 6f72 6d4c 6179      self.formLay
-00002460: 6f75 745f 3132 2e73 6574 5769 6467 6574  out_12.setWidget
-00002470: 2830 2c20 5174 5769 6467 6574 732e 5146  (0, QtWidgets.QF
-00002480: 6f72 6d4c 6179 6f75 742e 4c61 6265 6c52  ormLayout.LabelR
-00002490: 6f6c 652c 2073 656c 662e 6c61 6265 6c5f  ole, self.label_
-000024a0: 3139 290a 2020 2020 2020 2020 7365 6c66  19).        self
-000024b0: 2e6c 6162 656c 5f67 7261 7669 5f6d 616e  .label_gravi_man
-000024c0: 7566 6163 7475 7265 7220 3d20 5174 5769  ufacturer = QtWi
-000024d0: 6467 6574 732e 514c 6162 656c 2873 656c  dgets.QLabel(sel
-000024e0: 662e 7461 625f 6772 6176 696d 6574 6572  f.tab_gravimeter
-000024f0: 5f69 6e66 6f29 0a20 2020 2020 2020 2073  _info).        s
-00002500: 656c 662e 6c61 6265 6c5f 6772 6176 695f  elf.label_gravi_
-00002510: 6d61 6e75 6661 6374 7572 6572 2e73 6574  manufacturer.set
-00002520: 5465 7874 2822 2229 0a20 2020 2020 2020  Text("").       
-00002530: 2073 656c 662e 6c61 6265 6c5f 6772 6176   self.label_grav
-00002540: 695f 6d61 6e75 6661 6374 7572 6572 2e73  i_manufacturer.s
-00002550: 6574 4f62 6a65 6374 4e61 6d65 2822 6c61  etObjectName("la
-00002560: 6265 6c5f 6772 6176 695f 6d61 6e75 6661  bel_gravi_manufa
-00002570: 6374 7572 6572 2229 0a20 2020 2020 2020  cturer").       
-00002580: 2073 656c 662e 666f 726d 4c61 796f 7574   self.formLayout
-00002590: 5f31 322e 7365 7457 6964 6765 7428 302c  _12.setWidget(0,
-000025a0: 2051 7457 6964 6765 7473 2e51 466f 726d   QtWidgets.QForm
-000025b0: 4c61 796f 7574 2e46 6965 6c64 526f 6c65  Layout.FieldRole
-000025c0: 2c20 7365 6c66 2e6c 6162 656c 5f67 7261  , self.label_gra
-000025d0: 7669 5f6d 616e 7566 6163 7475 7265 7229  vi_manufacturer)
-000025e0: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
-000025f0: 6265 6c5f 3230 203d 2051 7457 6964 6765  bel_20 = QtWidge
-00002600: 7473 2e51 4c61 6265 6c28 7365 6c66 2e74  ts.QLabel(self.t
-00002610: 6162 5f67 7261 7669 6d65 7465 725f 696e  ab_gravimeter_in
-00002620: 666f 290a 2020 2020 2020 2020 7365 6c66  fo).        self
-00002630: 2e6c 6162 656c 5f32 302e 7365 744f 626a  .label_20.setObj
-00002640: 6563 744e 616d 6528 226c 6162 656c 5f32  ectName("label_2
-00002650: 3022 290a 2020 2020 2020 2020 7365 6c66  0").        self
-00002660: 2e66 6f72 6d4c 6179 6f75 745f 3132 2e73  .formLayout_12.s
-00002670: 6574 5769 6467 6574 2831 2c20 5174 5769  etWidget(1, QtWi
-00002680: 6467 6574 732e 5146 6f72 6d4c 6179 6f75  dgets.QFormLayou
-00002690: 742e 4c61 6265 6c52 6f6c 652c 2073 656c  t.LabelRole, sel
-000026a0: 662e 6c61 6265 6c5f 3230 290a 2020 2020  f.label_20).    
-000026b0: 2020 2020 7365 6c66 2e6c 6162 656c 5f67      self.label_g
-000026c0: 7261 7669 5f74 7970 6520 3d20 5174 5769  ravi_type = QtWi
-000026d0: 6467 6574 732e 514c 6162 656c 2873 656c  dgets.QLabel(sel
-000026e0: 662e 7461 625f 6772 6176 696d 6574 6572  f.tab_gravimeter
-000026f0: 5f69 6e66 6f29 0a20 2020 2020 2020 2073  _info).        s
-00002700: 656c 662e 6c61 6265 6c5f 6772 6176 695f  elf.label_gravi_
-00002710: 7479 7065 2e73 6574 5465 7874 2822 2229  type.setText("")
-00002720: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
-00002730: 6265 6c5f 6772 6176 695f 7479 7065 2e73  bel_gravi_type.s
-00002740: 6574 4f62 6a65 6374 4e61 6d65 2822 6c61  etObjectName("la
-00002750: 6265 6c5f 6772 6176 695f 7479 7065 2229  bel_gravi_type")
-00002760: 0a20 2020 2020 2020 2073 656c 662e 666f  .        self.fo
-00002770: 726d 4c61 796f 7574 5f31 322e 7365 7457  rmLayout_12.setW
-00002780: 6964 6765 7428 312c 2051 7457 6964 6765  idget(1, QtWidge
-00002790: 7473 2e51 466f 726d 4c61 796f 7574 2e46  ts.QFormLayout.F
-000027a0: 6965 6c64 526f 6c65 2c20 7365 6c66 2e6c  ieldRole, self.l
-000027b0: 6162 656c 5f67 7261 7669 5f74 7970 6529  abel_gravi_type)
-000027c0: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
-000027d0: 6265 6c5f 3231 203d 2051 7457 6964 6765  bel_21 = QtWidge
-000027e0: 7473 2e51 4c61 6265 6c28 7365 6c66 2e74  ts.QLabel(self.t
-000027f0: 6162 5f67 7261 7669 6d65 7465 725f 696e  ab_gravimeter_in
-00002800: 666f 290a 2020 2020 2020 2020 7365 6c66  fo).        self
-00002810: 2e6c 6162 656c 5f32 312e 7365 744f 626a  .label_21.setObj
-00002820: 6563 744e 616d 6528 226c 6162 656c 5f32  ectName("label_2
-00002830: 3122 290a 2020 2020 2020 2020 7365 6c66  1").        self
-00002840: 2e66 6f72 6d4c 6179 6f75 745f 3132 2e73  .formLayout_12.s
-00002850: 6574 5769 6467 6574 2832 2c20 5174 5769  etWidget(2, QtWi
-00002860: 6467 6574 732e 5146 6f72 6d4c 6179 6f75  dgets.QFormLayou
-00002870: 742e 4c61 6265 6c52 6f6c 652c 2073 656c  t.LabelRole, sel
-00002880: 662e 6c61 6265 6c5f 3231 290a 2020 2020  f.label_21).    
-00002890: 2020 2020 7365 6c66 2e6c 6162 656c 5f67      self.label_g
-000028a0: 7261 7669 5f73 6572 6961 6c5f 6e75 6d62  ravi_serial_numb
-000028b0: 6572 203d 2051 7457 6964 6765 7473 2e51  er = QtWidgets.Q
-000028c0: 4c61 6265 6c28 7365 6c66 2e74 6162 5f67  Label(self.tab_g
-000028d0: 7261 7669 6d65 7465 725f 696e 666f 290a  ravimeter_info).
-000028e0: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
-000028f0: 656c 5f67 7261 7669 5f73 6572 6961 6c5f  el_gravi_serial_
-00002900: 6e75 6d62 6572 2e73 6574 5465 7874 2822  number.setText("
-00002910: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00002920: 6c61 6265 6c5f 6772 6176 695f 7365 7269  label_gravi_seri
-00002930: 616c 5f6e 756d 6265 722e 7365 744f 626a  al_number.setObj
-00002940: 6563 744e 616d 6528 226c 6162 656c 5f67  ectName("label_g
-00002950: 7261 7669 5f73 6572 6961 6c5f 6e75 6d62  ravi_serial_numb
-00002960: 6572 2229 0a20 2020 2020 2020 2073 656c  er").        sel
-00002970: 662e 666f 726d 4c61 796f 7574 5f31 322e  f.formLayout_12.
-00002980: 7365 7457 6964 6765 7428 322c 2051 7457  setWidget(2, QtW
-00002990: 6964 6765 7473 2e51 466f 726d 4c61 796f  idgets.QFormLayo
-000029a0: 7574 2e46 6965 6c64 526f 6c65 2c20 7365  ut.FieldRole, se
-000029b0: 6c66 2e6c 6162 656c 5f67 7261 7669 5f73  lf.label_gravi_s
-000029c0: 6572 6961 6c5f 6e75 6d62 6572 290a 2020  erial_number).  
-000029d0: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
-000029e0: 5f32 3520 3d20 5174 5769 6467 6574 732e  _25 = QtWidgets.
-000029f0: 514c 6162 656c 2873 656c 662e 7461 625f  QLabel(self.tab_
-00002a00: 6772 6176 696d 6574 6572 5f69 6e66 6f29  gravimeter_info)
-00002a10: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
-00002a20: 6265 6c5f 3235 2e73 6574 4f62 6a65 6374  bel_25.setObject
-00002a30: 4e61 6d65 2822 6c61 6265 6c5f 3235 2229  Name("label_25")
-00002a40: 0a20 2020 2020 2020 2073 656c 662e 666f  .        self.fo
-00002a50: 726d 4c61 796f 7574 5f31 322e 7365 7457  rmLayout_12.setW
-00002a60: 6964 6765 7428 332c 2051 7457 6964 6765  idget(3, QtWidge
-00002a70: 7473 2e51 466f 726d 4c61 796f 7574 2e4c  ts.QFormLayout.L
-00002a80: 6162 656c 526f 6c65 2c20 7365 6c66 2e6c  abelRole, self.l
-00002a90: 6162 656c 5f32 3529 0a20 2020 2020 2020  abel_25).       
-00002aa0: 2073 656c 662e 6c61 6265 6c5f 6772 6176   self.label_grav
-00002ab0: 695f 636f 6465 203d 2051 7457 6964 6765  i_code = QtWidge
-00002ac0: 7473 2e51 4c61 6265 6c28 7365 6c66 2e74  ts.QLabel(self.t
-00002ad0: 6162 5f67 7261 7669 6d65 7465 725f 696e  ab_gravimeter_in
-00002ae0: 666f 290a 2020 2020 2020 2020 7365 6c66  fo).        self
-00002af0: 2e6c 6162 656c 5f67 7261 7669 5f63 6f64  .label_gravi_cod
-00002b00: 652e 7365 7454 6578 7428 2222 290a 2020  e.setText("").  
-00002b10: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
-00002b20: 5f67 7261 7669 5f63 6f64 652e 7365 744f  _gravi_code.setO
-00002b30: 626a 6563 744e 616d 6528 226c 6162 656c  bjectName("label
-00002b40: 5f67 7261 7669 5f63 6f64 6522 290a 2020  _gravi_code").  
-00002b50: 2020 2020 2020 7365 6c66 2e66 6f72 6d4c        self.formL
-00002b60: 6179 6f75 745f 3132 2e73 6574 5769 6467  ayout_12.setWidg
-00002b70: 6574 2833 2c20 5174 5769 6467 6574 732e  et(3, QtWidgets.
-00002b80: 5146 6f72 6d4c 6179 6f75 742e 4669 656c  QFormLayout.Fiel
-00002b90: 6452 6f6c 652c 2073 656c 662e 6c61 6265  dRole, self.labe
-00002ba0: 6c5f 6772 6176 695f 636f 6465 290a 2020  l_gravi_code).  
-00002bb0: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
-00002bc0: 5f32 3220 3d20 5174 5769 6467 6574 732e  _22 = QtWidgets.
-00002bd0: 514c 6162 656c 2873 656c 662e 7461 625f  QLabel(self.tab_
-00002be0: 6772 6176 696d 6574 6572 5f69 6e66 6f29  gravimeter_info)
-00002bf0: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
-00002c00: 6265 6c5f 3232 2e73 6574 4f62 6a65 6374  bel_22.setObject
-00002c10: 4e61 6d65 2822 6c61 6265 6c5f 3232 2229  Name("label_22")
-00002c20: 0a20 2020 2020 2020 2073 656c 662e 666f  .        self.fo
-00002c30: 726d 4c61 796f 7574 5f31 322e 7365 7457  rmLayout_12.setW
-00002c40: 6964 6765 7428 342c 2051 7457 6964 6765  idget(4, QtWidge
-00002c50: 7473 2e51 466f 726d 4c61 796f 7574 2e4c  ts.QFormLayout.L
-00002c60: 6162 656c 526f 6c65 2c20 7365 6c66 2e6c  abelRole, self.l
-00002c70: 6162 656c 5f32 3229 0a20 2020 2020 2020  abel_22).       
-00002c80: 2073 656c 662e 6c61 6265 6c5f 6772 6176   self.label_grav
-00002c90: 695f 6865 6967 6874 5f6f 6666 7365 7420  i_height_offset 
-00002ca0: 3d20 5174 5769 6467 6574 732e 514c 6162  = QtWidgets.QLab
-00002cb0: 656c 2873 656c 662e 7461 625f 6772 6176  el(self.tab_grav
-00002cc0: 696d 6574 6572 5f69 6e66 6f29 0a20 2020  imeter_info).   
-00002cd0: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
-00002ce0: 6772 6176 695f 6865 6967 6874 5f6f 6666  gravi_height_off
-00002cf0: 7365 742e 7365 7454 6578 7428 2222 290a  set.setText("").
-00002d00: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
-00002d10: 656c 5f67 7261 7669 5f68 6569 6768 745f  el_gravi_height_
-00002d20: 6f66 6673 6574 2e73 6574 4f62 6a65 6374  offset.setObject
-00002d30: 4e61 6d65 2822 6c61 6265 6c5f 6772 6176  Name("label_grav
-00002d40: 695f 6865 6967 6874 5f6f 6666 7365 7422  i_height_offset"
-00002d50: 290a 2020 2020 2020 2020 7365 6c66 2e66  ).        self.f
-00002d60: 6f72 6d4c 6179 6f75 745f 3132 2e73 6574  ormLayout_12.set
-00002d70: 5769 6467 6574 2834 2c20 5174 5769 6467  Widget(4, QtWidg
-00002d80: 6574 732e 5146 6f72 6d4c 6179 6f75 742e  ets.QFormLayout.
-00002d90: 4669 656c 6452 6f6c 652c 2073 656c 662e  FieldRole, self.
-00002da0: 6c61 6265 6c5f 6772 6176 695f 6865 6967  label_gravi_heig
-00002db0: 6874 5f6f 6666 7365 7429 0a20 2020 2020  ht_offset).     
-00002dc0: 2020 2073 656c 662e 6c61 6265 6c5f 3233     self.label_23
-00002dd0: 203d 2051 7457 6964 6765 7473 2e51 4c61   = QtWidgets.QLa
-00002de0: 6265 6c28 7365 6c66 2e74 6162 5f67 7261  bel(self.tab_gra
-00002df0: 7669 6d65 7465 725f 696e 666f 290a 2020  vimeter_info).  
-00002e00: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
-00002e10: 5f32 332e 7365 744f 626a 6563 744e 616d  _23.setObjectNam
-00002e20: 6528 226c 6162 656c 5f32 3322 290a 2020  e("label_23").  
-00002e30: 2020 2020 2020 7365 6c66 2e66 6f72 6d4c        self.formL
-00002e40: 6179 6f75 745f 3132 2e73 6574 5769 6467  ayout_12.setWidg
-00002e50: 6574 2835 2c20 5174 5769 6467 6574 732e  et(5, QtWidgets.
-00002e60: 5146 6f72 6d4c 6179 6f75 742e 4c61 6265  QFormLayout.Labe
-00002e70: 6c52 6f6c 652c 2073 656c 662e 6c61 6265  lRole, self.labe
-00002e80: 6c5f 3233 290a 2020 2020 2020 2020 7365  l_23).        se
-00002e90: 6c66 2e6c 6162 656c 5f67 7261 7669 5f64  lf.label_gravi_d
-00002ea0: 6174 615f 736f 7572 6365 203d 2051 7457  ata_source = QtW
-00002eb0: 6964 6765 7473 2e51 4c61 6265 6c28 7365  idgets.QLabel(se
-00002ec0: 6c66 2e74 6162 5f67 7261 7669 6d65 7465  lf.tab_gravimete
-00002ed0: 725f 696e 666f 290a 2020 2020 2020 2020  r_info).        
-00002ee0: 7365 6c66 2e6c 6162 656c 5f67 7261 7669  self.label_gravi
-00002ef0: 5f64 6174 615f 736f 7572 6365 2e73 6574  _data_source.set
-00002f00: 5465 7874 2822 2229 0a20 2020 2020 2020  Text("").       
-00002f10: 2073 656c 662e 6c61 6265 6c5f 6772 6176   self.label_grav
-00002f20: 695f 6461 7461 5f73 6f75 7263 652e 7365  i_data_source.se
-00002f30: 744f 626a 6563 744e 616d 6528 226c 6162  tObjectName("lab
-00002f40: 656c 5f67 7261 7669 5f64 6174 615f 736f  el_gravi_data_so
-00002f50: 7572 6365 2229 0a20 2020 2020 2020 2073  urce").        s
-00002f60: 656c 662e 666f 726d 4c61 796f 7574 5f31  elf.formLayout_1
-00002f70: 322e 7365 7457 6964 6765 7428 352c 2051  2.setWidget(5, Q
-00002f80: 7457 6964 6765 7473 2e51 466f 726d 4c61  tWidgets.QFormLa
-00002f90: 796f 7574 2e46 6965 6c64 526f 6c65 2c20  yout.FieldRole, 
-00002fa0: 7365 6c66 2e6c 6162 656c 5f67 7261 7669  self.label_gravi
-00002fb0: 5f64 6174 615f 736f 7572 6365 290a 2020  _data_source).  
-00002fc0: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
-00002fd0: 5f32 3420 3d20 5174 5769 6467 6574 732e  _24 = QtWidgets.
-00002fe0: 514c 6162 656c 2873 656c 662e 7461 625f  QLabel(self.tab_
-00002ff0: 6772 6176 696d 6574 6572 5f69 6e66 6f29  gravimeter_info)
-00003000: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
-00003010: 6265 6c5f 3234 2e73 6574 4f62 6a65 6374  bel_24.setObject
-00003020: 4e61 6d65 2822 6c61 6265 6c5f 3234 2229  Name("label_24")
-00003030: 0a20 2020 2020 2020 2073 656c 662e 666f  .        self.fo
-00003040: 726d 4c61 796f 7574 5f31 322e 7365 7457  rmLayout_12.setW
-00003050: 6964 6765 7428 362c 2051 7457 6964 6765  idget(6, QtWidge
-00003060: 7473 2e51 466f 726d 4c61 796f 7574 2e4c  ts.QFormLayout.L
-00003070: 6162 656c 526f 6c65 2c20 7365 6c66 2e6c  abelRole, self.l
-00003080: 6162 656c 5f32 3429 0a20 2020 2020 2020  abel_24).       
-00003090: 2073 656c 662e 6c61 6265 6c5f 6772 6176   self.label_grav
-000030a0: 695f 6461 7461 5f73 6f75 7263 655f 7479  i_data_source_ty
-000030b0: 7065 203d 2051 7457 6964 6765 7473 2e51  pe = QtWidgets.Q
-000030c0: 4c61 6265 6c28 7365 6c66 2e74 6162 5f67  Label(self.tab_g
-000030d0: 7261 7669 6d65 7465 725f 696e 666f 290a  ravimeter_info).
-000030e0: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
-000030f0: 656c 5f67 7261 7669 5f64 6174 615f 736f  el_gravi_data_so
-00003100: 7572 6365 5f74 7970 652e 7365 7454 6578  urce_type.setTex
-00003110: 7428 2222 290a 2020 2020 2020 2020 7365  t("").        se
-00003120: 6c66 2e6c 6162 656c 5f67 7261 7669 5f64  lf.label_gravi_d
-00003130: 6174 615f 736f 7572 6365 5f74 7970 652e  ata_source_type.
-00003140: 7365 744f 626a 6563 744e 616d 6528 226c  setObjectName("l
-00003150: 6162 656c 5f67 7261 7669 5f64 6174 615f  abel_gravi_data_
-00003160: 736f 7572 6365 5f74 7970 6522 290a 2020  source_type").  
-00003170: 2020 2020 2020 7365 6c66 2e66 6f72 6d4c        self.formL
-00003180: 6179 6f75 745f 3132 2e73 6574 5769 6467  ayout_12.setWidg
-00003190: 6574 2836 2c20 5174 5769 6467 6574 732e  et(6, QtWidgets.
-000031a0: 5146 6f72 6d4c 6179 6f75 742e 4669 656c  QFormLayout.Fiel
-000031b0: 6452 6f6c 652c 2073 656c 662e 6c61 6265  dRole, self.labe
-000031c0: 6c5f 6772 6176 695f 6461 7461 5f73 6f75  l_gravi_data_sou
-000031d0: 7263 655f 7479 7065 290a 2020 2020 2020  rce_type).      
-000031e0: 2020 7365 6c66 2e6c 6162 656c 5f32 3620    self.label_26 
-000031f0: 3d20 5174 5769 6467 6574 732e 514c 6162  = QtWidgets.QLab
-00003200: 656c 2873 656c 662e 7461 625f 6772 6176  el(self.tab_grav
-00003210: 696d 6574 6572 5f69 6e66 6f29 0a20 2020  imeter_info).   
-00003220: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
-00003230: 3236 2e73 6574 4f62 6a65 6374 4e61 6d65  26.setObjectName
-00003240: 2822 6c61 6265 6c5f 3236 2229 0a20 2020  ("label_26").   
-00003250: 2020 2020 2073 656c 662e 666f 726d 4c61       self.formLa
-00003260: 796f 7574 5f31 322e 7365 7457 6964 6765  yout_12.setWidge
-00003270: 7428 372c 2051 7457 6964 6765 7473 2e51  t(7, QtWidgets.Q
-00003280: 466f 726d 4c61 796f 7574 2e4c 6162 656c  FormLayout.Label
-00003290: 526f 6c65 2c20 7365 6c66 2e6c 6162 656c  Role, self.label
-000032a0: 5f32 3629 0a20 2020 2020 2020 2073 656c  _26).        sel
-000032b0: 662e 6c61 6265 6c5f 6772 6176 695f 6e75  f.label_gravi_nu
-000032c0: 6d5f 7363 616c 655f 6661 6374 6f72 7320  m_scale_factors 
-000032d0: 3d20 5174 5769 6467 6574 732e 514c 6162  = QtWidgets.QLab
-000032e0: 656c 2873 656c 662e 7461 625f 6772 6176  el(self.tab_grav
-000032f0: 696d 6574 6572 5f69 6e66 6f29 0a20 2020  imeter_info).   
-00003300: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
-00003310: 6772 6176 695f 6e75 6d5f 7363 616c 655f  gravi_num_scale_
-00003320: 6661 6374 6f72 732e 7365 7454 6578 7428  factors.setText(
-00003330: 2222 290a 2020 2020 2020 2020 7365 6c66  "").        self
-00003340: 2e6c 6162 656c 5f67 7261 7669 5f6e 756d  .label_gravi_num
-00003350: 5f73 6361 6c65 5f66 6163 746f 7273 2e73  _scale_factors.s
-00003360: 6574 4f62 6a65 6374 4e61 6d65 2822 6c61  etObjectName("la
-00003370: 6265 6c5f 6772 6176 695f 6e75 6d5f 7363  bel_gravi_num_sc
-00003380: 616c 655f 6661 6374 6f72 7322 290a 2020  ale_factors").  
-00003390: 2020 2020 2020 7365 6c66 2e66 6f72 6d4c        self.formL
-000033a0: 6179 6f75 745f 3132 2e73 6574 5769 6467  ayout_12.setWidg
-000033b0: 6574 2837 2c20 5174 5769 6467 6574 732e  et(7, QtWidgets.
-000033c0: 5146 6f72 6d4c 6179 6f75 742e 4669 656c  QFormLayout.Fiel
-000033d0: 6452 6f6c 652c 2073 656c 662e 6c61 6265  dRole, self.labe
-000033e0: 6c5f 6772 6176 695f 6e75 6d5f 7363 616c  l_gravi_num_scal
-000033f0: 655f 6661 6374 6f72 7329 0a20 2020 2020  e_factors).     
-00003400: 2020 2073 656c 662e 6c61 6265 6c5f 3238     self.label_28
-00003410: 203d 2051 7457 6964 6765 7473 2e51 4c61   = QtWidgets.QLa
-00003420: 6265 6c28 7365 6c66 2e74 6162 5f67 7261  bel(self.tab_gra
-00003430: 7669 6d65 7465 725f 696e 666f 290a 2020  vimeter_info).  
-00003440: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
-00003450: 5f32 382e 7365 744f 626a 6563 744e 616d  _28.setObjectNam
-00003460: 6528 226c 6162 656c 5f32 3822 290a 2020  e("label_28").  
-00003470: 2020 2020 2020 7365 6c66 2e66 6f72 6d4c        self.formL
-00003480: 6179 6f75 745f 3132 2e73 6574 5769 6467  ayout_12.setWidg
-00003490: 6574 2838 2c20 5174 5769 6467 6574 732e  et(8, QtWidgets.
-000034a0: 5146 6f72 6d4c 6179 6f75 742e 4c61 6265  QFormLayout.Labe
-000034b0: 6c52 6f6c 652c 2073 656c 662e 6c61 6265  lRole, self.labe
-000034c0: 6c5f 3238 290a 2020 2020 2020 2020 7365  l_28).        se
-000034d0: 6c66 2e6c 6162 656c 5f67 7261 7669 5f64  lf.label_gravi_d
-000034e0: 6573 6372 6970 7469 6f6e 203d 2051 7457  escription = QtW
-000034f0: 6964 6765 7473 2e51 4c61 6265 6c28 7365  idgets.QLabel(se
-00003500: 6c66 2e74 6162 5f67 7261 7669 6d65 7465  lf.tab_gravimete
-00003510: 725f 696e 666f 290a 2020 2020 2020 2020  r_info).        
-00003520: 7365 6c66 2e6c 6162 656c 5f67 7261 7669  self.label_gravi
-00003530: 5f64 6573 6372 6970 7469 6f6e 2e73 6574  _description.set
-00003540: 5465 7874 2822 2229 0a20 2020 2020 2020  Text("").       
-00003550: 2073 656c 662e 6c61 6265 6c5f 6772 6176   self.label_grav
-00003560: 695f 6465 7363 7269 7074 696f 6e2e 7365  i_description.se
-00003570: 7457 6f72 6457 7261 7028 5472 7565 290a  tWordWrap(True).
-00003580: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
-00003590: 656c 5f67 7261 7669 5f64 6573 6372 6970  el_gravi_descrip
-000035a0: 7469 6f6e 2e73 6574 4f62 6a65 6374 4e61  tion.setObjectNa
-000035b0: 6d65 2822 6c61 6265 6c5f 6772 6176 695f  me("label_gravi_
-000035c0: 6465 7363 7269 7074 696f 6e22 290a 2020  description").  
-000035d0: 2020 2020 2020 7365 6c66 2e66 6f72 6d4c        self.formL
-000035e0: 6179 6f75 745f 3132 2e73 6574 5769 6467  ayout_12.setWidg
-000035f0: 6574 2838 2c20 5174 5769 6467 6574 732e  et(8, QtWidgets.
-00003600: 5146 6f72 6d4c 6179 6f75 742e 4669 656c  QFormLayout.Fiel
-00003610: 6452 6f6c 652c 2073 656c 662e 6c61 6265  dRole, self.labe
-00003620: 6c5f 6772 6176 695f 6465 7363 7269 7074  l_gravi_descript
-00003630: 696f 6e29 0a20 2020 2020 2020 2073 656c  ion).        sel
-00003640: 662e 7665 7274 6963 616c 4c61 796f 7574  f.verticalLayout
-00003650: 5f34 322e 6164 644c 6179 6f75 7428 7365  _42.addLayout(se
-00003660: 6c66 2e66 6f72 6d4c 6179 6f75 745f 3132  lf.formLayout_12
-00003670: 290a 2020 2020 2020 2020 7365 6c66 2e74  ).        self.t
-00003680: 6162 5769 6467 6574 5f67 7261 7669 6d65  abWidget_gravime
-00003690: 7465 7273 2e61 6464 5461 6228 7365 6c66  ters.addTab(self
-000036a0: 2e74 6162 5f67 7261 7669 6d65 7465 725f  .tab_gravimeter_
-000036b0: 696e 666f 2c20 2222 290a 2020 2020 2020  info, "").      
-000036c0: 2020 7365 6c66 2e74 6162 5f67 7261 7669    self.tab_gravi
-000036d0: 6d65 7465 725f 7363 616c 6520 3d20 5174  meter_scale = Qt
-000036e0: 5769 6467 6574 732e 5157 6964 6765 7428  Widgets.QWidget(
-000036f0: 290a 2020 2020 2020 2020 7365 6c66 2e74  ).        self.t
-00003700: 6162 5f67 7261 7669 6d65 7465 725f 7363  ab_gravimeter_sc
-00003710: 616c 652e 7365 744f 626a 6563 744e 616d  ale.setObjectNam
-00003720: 6528 2274 6162 5f67 7261 7669 6d65 7465  e("tab_gravimete
-00003730: 725f 7363 616c 6522 290a 2020 2020 2020  r_scale").      
-00003740: 2020 7365 6c66 2e76 6572 7469 6361 6c4c    self.verticalL
-00003750: 6179 6f75 745f 3431 203d 2051 7457 6964  ayout_41 = QtWid
-00003760: 6765 7473 2e51 5642 6f78 4c61 796f 7574  gets.QVBoxLayout
-00003770: 2873 656c 662e 7461 625f 6772 6176 696d  (self.tab_gravim
-00003780: 6574 6572 5f73 6361 6c65 290a 2020 2020  eter_scale).    
-00003790: 2020 2020 7365 6c66 2e76 6572 7469 6361      self.vertica
-000037a0: 6c4c 6179 6f75 745f 3431 2e73 6574 4f62  lLayout_41.setOb
-000037b0: 6a65 6374 4e61 6d65 2822 7665 7274 6963  jectName("vertic
-000037c0: 616c 4c61 796f 7574 5f34 3122 290a 2020  alLayout_41").  
-000037d0: 2020 2020 2020 7365 6c66 2e74 6162 6c65        self.table
-000037e0: 5669 6577 5f67 7261 7669 6d65 7465 7273  View_gravimeters
-000037f0: 5f73 6361 6c65 203d 2051 7457 6964 6765  _scale = QtWidge
-00003800: 7473 2e51 5461 626c 6556 6965 7728 7365  ts.QTableView(se
-00003810: 6c66 2e74 6162 5f67 7261 7669 6d65 7465  lf.tab_gravimete
-00003820: 725f 7363 616c 6529 0a20 2020 2020 2020  r_scale).       
-00003830: 2073 656c 662e 7461 626c 6556 6965 775f   self.tableView_
-00003840: 6772 6176 696d 6574 6572 735f 7363 616c  gravimeters_scal
-00003850: 652e 7365 744f 626a 6563 744e 616d 6528  e.setObjectName(
-00003860: 2274 6162 6c65 5669 6577 5f67 7261 7669  "tableView_gravi
-00003870: 6d65 7465 7273 5f73 6361 6c65 2229 0a20  meters_scale"). 
-00003880: 2020 2020 2020 2073 656c 662e 7665 7274         self.vert
-00003890: 6963 616c 4c61 796f 7574 5f34 312e 6164  icalLayout_41.ad
-000038a0: 6457 6964 6765 7428 7365 6c66 2e74 6162  dWidget(self.tab
-000038b0: 6c65 5669 6577 5f67 7261 7669 6d65 7465  leView_gravimete
-000038c0: 7273 5f73 6361 6c65 290a 2020 2020 2020  rs_scale).      
-000038d0: 2020 7365 6c66 2e74 6162 5769 6467 6574    self.tabWidget
-000038e0: 5f67 7261 7669 6d65 7465 7273 2e61 6464  _gravimeters.add
-000038f0: 5461 6228 7365 6c66 2e74 6162 5f67 7261  Tab(self.tab_gra
-00003900: 7669 6d65 7465 725f 7363 616c 652c 2022  vimeter_scale, "
-00003910: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00003920: 7665 7274 6963 616c 4c61 796f 7574 5f32  verticalLayout_2
-00003930: 382e 6164 6457 6964 6765 7428 7365 6c66  8.addWidget(self
-00003940: 2e73 706c 6974 7465 725f 6772 6176 696d  .splitter_gravim
-00003950: 6574 6572 7329 0a20 2020 2020 2020 2073  eters).        s
-00003960: 656c 662e 7461 6257 6964 6765 745f 4d61  elf.tabWidget_Ma
-00003970: 696e 2e61 6464 5461 6228 7365 6c66 2e74  in.addTab(self.t
-00003980: 6162 5f6d 6169 6e5f 6772 6176 696d 6574  ab_main_gravimet
-00003990: 6572 732c 2022 2229 0a20 2020 2020 2020  ers, "").       
-000039a0: 2073 656c 662e 7461 625f 6d61 696e 5f6f   self.tab_main_o
-000039b0: 6273 6572 7661 7469 6f6e 7320 3d20 5174  bservations = Qt
-000039c0: 5769 6467 6574 732e 5157 6964 6765 7428  Widgets.QWidget(
-000039d0: 290a 2020 2020 2020 2020 7365 6c66 2e74  ).        self.t
-000039e0: 6162 5f6d 6169 6e5f 6f62 7365 7276 6174  ab_main_observat
-000039f0: 696f 6e73 2e73 6574 4f62 6a65 6374 4e61  ions.setObjectNa
-00003a00: 6d65 2822 7461 625f 6d61 696e 5f6f 6273  me("tab_main_obs
-00003a10: 6572 7661 7469 6f6e 7322 290a 2020 2020  ervations").    
-00003a20: 2020 2020 7365 6c66 2e76 6572 7469 6361      self.vertica
-00003a30: 6c4c 6179 6f75 745f 3720 3d20 5174 5769  lLayout_7 = QtWi
-00003a40: 6467 6574 732e 5156 426f 784c 6179 6f75  dgets.QVBoxLayou
-00003a50: 7428 7365 6c66 2e74 6162 5f6d 6169 6e5f  t(self.tab_main_
-00003a60: 6f62 7365 7276 6174 696f 6e73 290a 2020  observations).  
-00003a70: 2020 2020 2020 7365 6c66 2e76 6572 7469        self.verti
-00003a80: 6361 6c4c 6179 6f75 745f 372e 7365 744f  calLayout_7.setO
-00003a90: 626a 6563 744e 616d 6528 2276 6572 7469  bjectName("verti
-00003aa0: 6361 6c4c 6179 6f75 745f 3722 290a 2020  calLayout_7").  
-00003ab0: 2020 2020 2020 7365 6c66 2e73 706c 6974        self.split
-00003ac0: 7465 725f 6f62 7320 3d20 5174 5769 6467  ter_obs = QtWidg
-00003ad0: 6574 732e 5153 706c 6974 7465 7228 7365  ets.QSplitter(se
-00003ae0: 6c66 2e74 6162 5f6d 6169 6e5f 6f62 7365  lf.tab_main_obse
-00003af0: 7276 6174 696f 6e73 290a 2020 2020 2020  rvations).      
-00003b00: 2020 7365 6c66 2e73 706c 6974 7465 725f    self.splitter_
-00003b10: 6f62 732e 7365 7454 6f6f 6c54 6970 4475  obs.setToolTipDu
-00003b20: 7261 7469 6f6e 2831 290a 2020 2020 2020  ration(1).      
-00003b30: 2020 7365 6c66 2e73 706c 6974 7465 725f    self.splitter_
-00003b40: 6f62 732e 7365 744f 7269 656e 7461 7469  obs.setOrientati
-00003b50: 6f6e 2851 7443 6f72 652e 5174 2e48 6f72  on(QtCore.Qt.Hor
-00003b60: 697a 6f6e 7461 6c29 0a20 2020 2020 2020  izontal).       
-00003b70: 2073 656c 662e 7370 6c69 7474 6572 5f6f   self.splitter_o
-00003b80: 6273 2e73 6574 4f62 6a65 6374 4e61 6d65  bs.setObjectName
-00003b90: 2822 7370 6c69 7474 6572 5f6f 6273 2229  ("splitter_obs")
-00003ba0: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
-00003bb0: 796f 7574 5769 6467 6574 3120 3d20 5174  youtWidget1 = Qt
-00003bc0: 5769 6467 6574 732e 5157 6964 6765 7428  Widgets.QWidget(
-00003bd0: 7365 6c66 2e73 706c 6974 7465 725f 6f62  self.splitter_ob
-00003be0: 7329 0a20 2020 2020 2020 2073 656c 662e  s).        self.
-00003bf0: 6c61 796f 7574 5769 6467 6574 312e 7365  layoutWidget1.se
-00003c00: 744f 626a 6563 744e 616d 6528 226c 6179  tObjectName("lay
-00003c10: 6f75 7457 6964 6765 7431 2229 0a20 2020  outWidget1").   
-00003c20: 2020 2020 2073 656c 662e 7665 7274 6963       self.vertic
-00003c30: 616c 4c61 796f 7574 5f35 203d 2051 7457  alLayout_5 = QtW
-00003c40: 6964 6765 7473 2e51 5642 6f78 4c61 796f  idgets.QVBoxLayo
-00003c50: 7574 2873 656c 662e 6c61 796f 7574 5769  ut(self.layoutWi
-00003c60: 6467 6574 3129 0a20 2020 2020 2020 2073  dget1).        s
-00003c70: 656c 662e 7665 7274 6963 616c 4c61 796f  elf.verticalLayo
-00003c80: 7574 5f35 2e73 6574 436f 6e74 656e 7473  ut_5.setContents
-00003c90: 4d61 7267 696e 7328 302c 2030 2c20 302c  Margins(0, 0, 0,
-00003ca0: 2030 290a 2020 2020 2020 2020 7365 6c66   0).        self
-00003cb0: 2e76 6572 7469 6361 6c4c 6179 6f75 745f  .verticalLayout_
-00003cc0: 352e 7365 744f 626a 6563 744e 616d 6528  5.setObjectName(
-00003cd0: 2276 6572 7469 6361 6c4c 6179 6f75 745f  "verticalLayout_
-00003ce0: 3522 290a 2020 2020 2020 2020 7365 6c66  5").        self
-00003cf0: 2e74 7265 6557 6964 6765 745f 6f62 7365  .treeWidget_obse
-00003d00: 7276 6174 696f 6e73 203d 2051 7457 6964  rvations = QtWid
-00003d10: 6765 7473 2e51 5472 6565 5769 6467 6574  gets.QTreeWidget
-00003d20: 2873 656c 662e 6c61 796f 7574 5769 6467  (self.layoutWidg
-00003d30: 6574 3129 0a20 2020 2020 2020 2073 697a  et1).        siz
-00003d40: 6550 6f6c 6963 7920 3d20 5174 5769 6467  ePolicy = QtWidg
-00003d50: 6574 732e 5153 697a 6550 6f6c 6963 7928  ets.QSizePolicy(
-00003d60: 5174 5769 6467 6574 732e 5153 697a 6550  QtWidgets.QSizeP
-00003d70: 6f6c 6963 792e 4578 7061 6e64 696e 672c  olicy.Expanding,
-00003d80: 2051 7457 6964 6765 7473 2e51 5369 7a65   QtWidgets.QSize
-00003d90: 506f 6c69 6379 2e45 7870 616e 6469 6e67  Policy.Expanding
-00003da0: 290a 2020 2020 2020 2020 7369 7a65 506f  ).        sizePo
-00003db0: 6c69 6379 2e73 6574 486f 7269 7a6f 6e74  licy.setHorizont
-00003dc0: 616c 5374 7265 7463 6828 3029 0a20 2020  alStretch(0).   
-00003dd0: 2020 2020 2073 697a 6550 6f6c 6963 792e       sizePolicy.
-00003de0: 7365 7456 6572 7469 6361 6c53 7472 6574  setVerticalStret
-00003df0: 6368 2830 290a 2020 2020 2020 2020 7369  ch(0).        si
-00003e00: 7a65 506f 6c69 6379 2e73 6574 4865 6967  zePolicy.setHeig
-00003e10: 6874 466f 7257 6964 7468 2873 656c 662e  htForWidth(self.
-00003e20: 7472 6565 5769 6467 6574 5f6f 6273 6572  treeWidget_obser
-00003e30: 7661 7469 6f6e 732e 7369 7a65 506f 6c69  vations.sizePoli
-00003e40: 6379 2829 2e68 6173 4865 6967 6874 466f  cy().hasHeightFo
-00003e50: 7257 6964 7468 2829 290a 2020 2020 2020  rWidth()).      
-00003e60: 2020 7365 6c66 2e74 7265 6557 6964 6765    self.treeWidge
-00003e70: 745f 6f62 7365 7276 6174 696f 6e73 2e73  t_observations.s
-00003e80: 6574 5369 7a65 506f 6c69 6379 2873 697a  etSizePolicy(siz
-00003e90: 6550 6f6c 6963 7929 0a20 2020 2020 2020  ePolicy).       
-00003ea0: 2073 656c 662e 7472 6565 5769 6467 6574   self.treeWidget
-00003eb0: 5f6f 6273 6572 7661 7469 6f6e 732e 7365  _observations.se
-00003ec0: 744d 696e 696d 756d 5369 7a65 2851 7443  tMinimumSize(QtC
-00003ed0: 6f72 652e 5153 697a 6528 3238 302c 2030  ore.QSize(280, 0
-00003ee0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-00003ef0: 7472 6565 5769 6467 6574 5f6f 6273 6572  treeWidget_obser
-00003f00: 7661 7469 6f6e 732e 7365 7448 6561 6465  vations.setHeade
-00003f10: 7248 6964 6465 6e28 5472 7565 290a 2020  rHidden(True).  
-00003f20: 2020 2020 2020 7365 6c66 2e74 7265 6557        self.treeW
-00003f30: 6964 6765 745f 6f62 7365 7276 6174 696f  idget_observatio
-00003f40: 6e73 2e73 6574 4f62 6a65 6374 4e61 6d65  ns.setObjectName
-00003f50: 2822 7472 6565 5769 6467 6574 5f6f 6273  ("treeWidget_obs
-00003f60: 6572 7661 7469 6f6e 7322 290a 2020 2020  ervations").    
-00003f70: 2020 2020 7365 6c66 2e74 7265 6557 6964      self.treeWid
-00003f80: 6765 745f 6f62 7365 7276 6174 696f 6e73  get_observations
-00003f90: 2e68 6561 6465 7228 292e 7365 7456 6973  .header().setVis
-00003fa0: 6962 6c65 2846 616c 7365 290a 2020 2020  ible(False).    
-00003fb0: 2020 2020 7365 6c66 2e74 7265 6557 6964      self.treeWid
-00003fc0: 6765 745f 6f62 7365 7276 6174 696f 6e73  get_observations
-00003fd0: 2e68 6561 6465 7228 292e 7365 7453 7472  .header().setStr
-00003fe0: 6574 6368 4c61 7374 5365 6374 696f 6e28  etchLastSection(
-00003ff0: 5472 7565 290a 2020 2020 2020 2020 7365  True).        se
-00004000: 6c66 2e76 6572 7469 6361 6c4c 6179 6f75  lf.verticalLayou
-00004010: 745f 352e 6164 6457 6964 6765 7428 7365  t_5.addWidget(se
-00004020: 6c66 2e74 7265 6557 6964 6765 745f 6f62  lf.treeWidget_ob
-00004030: 7365 7276 6174 696f 6e73 290a 2020 2020  servations).    
-00004040: 2020 2020 7365 6c66 2e68 6f72 697a 6f6e      self.horizon
-00004050: 7461 6c4c 6179 6f75 745f 3320 3d20 5174  talLayout_3 = Qt
-00004060: 5769 6467 6574 732e 5148 426f 784c 6179  Widgets.QHBoxLay
-00004070: 6f75 7428 290a 2020 2020 2020 2020 7365  out().        se
-00004080: 6c66 2e68 6f72 697a 6f6e 7461 6c4c 6179  lf.horizontalLay
-00004090: 6f75 745f 332e 7365 744f 626a 6563 744e  out_3.setObjectN
-000040a0: 616d 6528 2268 6f72 697a 6f6e 7461 6c4c  ame("horizontalL
-000040b0: 6179 6f75 745f 3322 290a 2020 2020 2020  ayout_3").      
-000040c0: 2020 7365 6c66 2e70 7573 6842 7574 746f    self.pushButto
-000040d0: 6e5f 6f62 735f 636f 6c6c 6170 735f 616c  n_obs_collaps_al
-000040e0: 6c20 3d20 5174 5769 6467 6574 732e 5150  l = QtWidgets.QP
-000040f0: 7573 6842 7574 746f 6e28 7365 6c66 2e6c  ushButton(self.l
-00004100: 6179 6f75 7457 6964 6765 7431 290a 2020  ayoutWidget1).  
-00004110: 2020 2020 2020 7365 6c66 2e70 7573 6842        self.pushB
-00004120: 7574 746f 6e5f 6f62 735f 636f 6c6c 6170  utton_obs_collap
-00004130: 735f 616c 6c2e 7365 744f 626a 6563 744e  s_all.setObjectN
-00004140: 616d 6528 2270 7573 6842 7574 746f 6e5f  ame("pushButton_
-00004150: 6f62 735f 636f 6c6c 6170 735f 616c 6c22  obs_collaps_all"
-00004160: 290a 2020 2020 2020 2020 7365 6c66 2e68  ).        self.h
-00004170: 6f72 697a 6f6e 7461 6c4c 6179 6f75 745f  orizontalLayout_
-00004180: 332e 6164 6457 6964 6765 7428 7365 6c66  3.addWidget(self
-00004190: 2e70 7573 6842 7574 746f 6e5f 6f62 735f  .pushButton_obs_
-000041a0: 636f 6c6c 6170 735f 616c 6c29 0a20 2020  collaps_all).   
-000041b0: 2020 2020 2073 656c 662e 7075 7368 4275       self.pushBu
-000041c0: 7474 6f6e 5f6f 6273 5f65 7870 616e 645f  tton_obs_expand_
-000041d0: 616c 6c20 3d20 5174 5769 6467 6574 732e  all = QtWidgets.
-000041e0: 5150 7573 6842 7574 746f 6e28 7365 6c66  QPushButton(self
-000041f0: 2e6c 6179 6f75 7457 6964 6765 7431 290a  .layoutWidget1).
-00004200: 2020 2020 2020 2020 7365 6c66 2e70 7573          self.pus
-00004210: 6842 7574 746f 6e5f 6f62 735f 6578 7061  hButton_obs_expa
-00004220: 6e64 5f61 6c6c 2e73 6574 4f62 6a65 6374  nd_all.setObject
-00004230: 4e61 6d65 2822 7075 7368 4275 7474 6f6e  Name("pushButton
-00004240: 5f6f 6273 5f65 7870 616e 645f 616c 6c22  _obs_expand_all"
-00004250: 290a 2020 2020 2020 2020 7365 6c66 2e68  ).        self.h
-00004260: 6f72 697a 6f6e 7461 6c4c 6179 6f75 745f  orizontalLayout_
-00004270: 332e 6164 6457 6964 6765 7428 7365 6c66  3.addWidget(self
-00004280: 2e70 7573 6842 7574 746f 6e5f 6f62 735f  .pushButton_obs_
-00004290: 6578 7061 6e64 5f61 6c6c 290a 2020 2020  expand_all).    
-000042a0: 2020 2020 7365 6c66 2e76 6572 7469 6361      self.vertica
-000042b0: 6c4c 6179 6f75 745f 352e 6164 644c 6179  lLayout_5.addLay
-000042c0: 6f75 7428 7365 6c66 2e68 6f72 697a 6f6e  out(self.horizon
-000042d0: 7461 6c4c 6179 6f75 745f 3329 0a20 2020  talLayout_3).   
-000042e0: 2020 2020 2073 656c 662e 6772 6f75 7042       self.groupB
-000042f0: 6f78 5f6f 6273 5f64 6174 615f 6d61 6e69  ox_obs_data_mani
-00004300: 7075 6c61 7469 6f6e 203d 2051 7457 6964  pulation = QtWid
-00004310: 6765 7473 2e51 4772 6f75 7042 6f78 2873  gets.QGroupBox(s
-00004320: 656c 662e 6c61 796f 7574 5769 6467 6574  elf.layoutWidget
-00004330: 3129 0a20 2020 2020 2020 2073 656c 662e  1).        self.
-00004340: 6772 6f75 7042 6f78 5f6f 6273 5f64 6174  groupBox_obs_dat
-00004350: 615f 6d61 6e69 7075 6c61 7469 6f6e 2e73  a_manipulation.s
-00004360: 6574 456e 6162 6c65 6428 4661 6c73 6529  etEnabled(False)
-00004370: 0a20 2020 2020 2020 2073 656c 662e 6772  .        self.gr
-00004380: 6f75 7042 6f78 5f6f 6273 5f64 6174 615f  oupBox_obs_data_
-00004390: 6d61 6e69 7075 6c61 7469 6f6e 2e73 6574  manipulation.set
-000043a0: 4f62 6a65 6374 4e61 6d65 2822 6772 6f75  ObjectName("grou
-000043b0: 7042 6f78 5f6f 6273 5f64 6174 615f 6d61  pBox_obs_data_ma
-000043c0: 6e69 7075 6c61 7469 6f6e 2229 0a20 2020  nipulation").   
-000043d0: 2020 2020 2073 656c 662e 7665 7274 6963       self.vertic
-000043e0: 616c 4c61 796f 7574 5f31 3020 3d20 5174  alLayout_10 = Qt
-000043f0: 5769 6467 6574 732e 5156 426f 784c 6179  Widgets.QVBoxLay
-00004400: 6f75 7428 7365 6c66 2e67 726f 7570 426f  out(self.groupBo
-00004410: 785f 6f62 735f 6461 7461 5f6d 616e 6970  x_obs_data_manip
-00004420: 756c 6174 696f 6e29 0a20 2020 2020 2020  ulation).       
-00004430: 2073 656c 662e 7665 7274 6963 616c 4c61   self.verticalLa
-00004440: 796f 7574 5f31 302e 7365 744f 626a 6563  yout_10.setObjec
-00004450: 744e 616d 6528 2276 6572 7469 6361 6c4c  tName("verticalL
-00004460: 6179 6f75 745f 3130 2229 0a20 2020 2020  ayout_10").     
-00004470: 2020 2073 656c 662e 7075 7368 4275 7474     self.pushButt
-00004480: 6f6e 5f6f 6273 5f61 7070 6c79 5f61 7574  on_obs_apply_aut
-00004490: 6f73 656c 6563 745f 6375 7272 656e 745f  oselect_current_
-000044a0: 6461 7461 203d 2051 7457 6964 6765 7473  data = QtWidgets
-000044b0: 2e51 5075 7368 4275 7474 6f6e 2873 656c  .QPushButton(sel
-000044c0: 662e 6772 6f75 7042 6f78 5f6f 6273 5f64  f.groupBox_obs_d
-000044d0: 6174 615f 6d61 6e69 7075 6c61 7469 6f6e  ata_manipulation
-000044e0: 290a 2020 2020 2020 2020 7365 6c66 2e70  ).        self.p
-000044f0: 7573 6842 7574 746f 6e5f 6f62 735f 6170  ushButton_obs_ap
-00004500: 706c 795f 6175 746f 7365 6c65 6374 5f63  ply_autoselect_c
-00004510: 7572 7265 6e74 5f64 6174 612e 7365 744f  urrent_data.setO
-00004520: 626a 6563 744e 616d 6528 2270 7573 6842  bjectName("pushB
-00004530: 7574 746f 6e5f 6f62 735f 6170 706c 795f  utton_obs_apply_
-00004540: 6175 746f 7365 6c65 6374 5f63 7572 7265  autoselect_curre
-00004550: 6e74 5f64 6174 6122 290a 2020 2020 2020  nt_data").      
-00004560: 2020 7365 6c66 2e76 6572 7469 6361 6c4c    self.verticalL
-00004570: 6179 6f75 745f 3130 2e61 6464 5769 6467  ayout_10.addWidg
-00004580: 6574 2873 656c 662e 7075 7368 4275 7474  et(self.pushButt
-00004590: 6f6e 5f6f 6273 5f61 7070 6c79 5f61 7574  on_obs_apply_aut
-000045a0: 6f73 656c 6563 745f 6375 7272 656e 745f  oselect_current_
-000045b0: 6461 7461 290a 2020 2020 2020 2020 7365  data).        se
-000045c0: 6c66 2e70 7573 6842 7574 746f 6e5f 6f62  lf.pushButton_ob
-000045d0: 735f 636f 6d70 5f73 6574 7570 5f64 6174  s_comp_setup_dat
-000045e0: 6120 3d20 5174 5769 6467 6574 732e 5150  a = QtWidgets.QP
-000045f0: 7573 6842 7574 746f 6e28 7365 6c66 2e67  ushButton(self.g
-00004600: 726f 7570 426f 785f 6f62 735f 6461 7461  roupBox_obs_data
-00004610: 5f6d 616e 6970 756c 6174 696f 6e29 0a20  _manipulation). 
-00004620: 2020 2020 2020 2073 656c 662e 7075 7368         self.push
-00004630: 4275 7474 6f6e 5f6f 6273 5f63 6f6d 705f  Button_obs_comp_
-00004640: 7365 7475 705f 6461 7461 2e73 6574 4f62  setup_data.setOb
-00004650: 6a65 6374 4e61 6d65 2822 7075 7368 4275  jectName("pushBu
-00004660: 7474 6f6e 5f6f 6273 5f63 6f6d 705f 7365  tton_obs_comp_se
-00004670: 7475 705f 6461 7461 2229 0a20 2020 2020  tup_data").     
-00004680: 2020 2073 656c 662e 7665 7274 6963 616c     self.vertical
-00004690: 4c61 796f 7574 5f31 302e 6164 6457 6964  Layout_10.addWid
-000046a0: 6765 7428 7365 6c66 2e70 7573 6842 7574  get(self.pushBut
-000046b0: 746f 6e5f 6f62 735f 636f 6d70 5f73 6574  ton_obs_comp_set
-000046c0: 7570 5f64 6174 6129 0a20 2020 2020 2020  up_data).       
-000046d0: 2073 656c 662e 7075 7368 4275 7474 6f6e   self.pushButton
-000046e0: 5f6f 6273 5f72 756e 5f65 7374 696d 6174  _obs_run_estimat
-000046f0: 696f 6e20 3d20 5174 5769 6467 6574 732e  ion = QtWidgets.
-00004700: 5150 7573 6842 7574 746f 6e28 7365 6c66  QPushButton(self
-00004710: 2e67 726f 7570 426f 785f 6f62 735f 6461  .groupBox_obs_da
-00004720: 7461 5f6d 616e 6970 756c 6174 696f 6e29  ta_manipulation)
-00004730: 0a20 2020 2020 2020 2073 656c 662e 7075  .        self.pu
-00004740: 7368 4275 7474 6f6e 5f6f 6273 5f72 756e  shButton_obs_run
-00004750: 5f65 7374 696d 6174 696f 6e2e 7365 744f  _estimation.setO
-00004760: 626a 6563 744e 616d 6528 2270 7573 6842  bjectName("pushB
-00004770: 7574 746f 6e5f 6f62 735f 7275 6e5f 6573  utton_obs_run_es
-00004780: 7469 6d61 7469 6f6e 2229 0a20 2020 2020  timation").     
-00004790: 2020 2073 656c 662e 7665 7274 6963 616c     self.vertical
-000047a0: 4c61 796f 7574 5f31 302e 6164 6457 6964  Layout_10.addWid
-000047b0: 6765 7428 7365 6c66 2e70 7573 6842 7574  get(self.pushBut
-000047c0: 746f 6e5f 6f62 735f 7275 6e5f 6573 7469  ton_obs_run_esti
-000047d0: 6d61 7469 6f6e 290a 2020 2020 2020 2020  mation).        
-000047e0: 7365 6c66 2e76 6572 7469 6361 6c4c 6179  self.verticalLay
-000047f0: 6f75 745f 352e 6164 6457 6964 6765 7428  out_5.addWidget(
-00004800: 7365 6c66 2e67 726f 7570 426f 785f 6f62  self.groupBox_ob
-00004810: 735f 6461 7461 5f6d 616e 6970 756c 6174  s_data_manipulat
-00004820: 696f 6e29 0a20 2020 2020 2020 2073 656c  ion).        sel
-00004830: 662e 6772 6f75 7042 6f78 5f6f 6273 5f76  f.groupBox_obs_v
-00004840: 6965 775f 6f70 7469 6f6e 7320 3d20 5174  iew_options = Qt
-00004850: 5769 6467 6574 732e 5147 726f 7570 426f  Widgets.QGroupBo
-00004860: 7828 7365 6c66 2e6c 6179 6f75 7457 6964  x(self.layoutWid
-00004870: 6765 7431 290a 2020 2020 2020 2020 7365  get1).        se
-00004880: 6c66 2e67 726f 7570 426f 785f 6f62 735f  lf.groupBox_obs_
-00004890: 7669 6577 5f6f 7074 696f 6e73 2e73 6574  view_options.set
-000048a0: 456e 6162 6c65 6428 4661 6c73 6529 0a20  Enabled(False). 
-000048b0: 2020 2020 2020 2073 656c 662e 6772 6f75         self.grou
-000048c0: 7042 6f78 5f6f 6273 5f76 6965 775f 6f70  pBox_obs_view_op
-000048d0: 7469 6f6e 732e 7365 744f 626a 6563 744e  tions.setObjectN
-000048e0: 616d 6528 2267 726f 7570 426f 785f 6f62  ame("groupBox_ob
-000048f0: 735f 7669 6577 5f6f 7074 696f 6e73 2229  s_view_options")
-00004900: 0a20 2020 2020 2020 2073 656c 662e 7665  .        self.ve
-00004910: 7274 6963 616c 4c61 796f 7574 5f39 203d  rticalLayout_9 =
-00004920: 2051 7457 6964 6765 7473 2e51 5642 6f78   QtWidgets.QVBox
-00004930: 4c61 796f 7574 2873 656c 662e 6772 6f75  Layout(self.grou
-00004940: 7042 6f78 5f6f 6273 5f76 6965 775f 6f70  pBox_obs_view_op
-00004950: 7469 6f6e 7329 0a20 2020 2020 2020 2073  tions).        s
-00004960: 656c 662e 7665 7274 6963 616c 4c61 796f  elf.verticalLayo
-00004970: 7574 5f39 2e73 6574 4f62 6a65 6374 4e61  ut_9.setObjectNa
-00004980: 6d65 2822 7665 7274 6963 616c 4c61 796f  me("verticalLayo
-00004990: 7574 5f39 2229 0a20 2020 2020 2020 2073  ut_9").        s
-000049a0: 656c 662e 6368 6563 6b42 6f78 5f6f 6273  elf.checkBox_obs
-000049b0: 5f70 6c6f 745f 7265 6475 6365 645f 6f62  _plot_reduced_ob
-000049c0: 7365 7276 6174 696f 6e73 203d 2051 7457  servations = QtW
-000049d0: 6964 6765 7473 2e51 4368 6563 6b42 6f78  idgets.QCheckBox
-000049e0: 2873 656c 662e 6772 6f75 7042 6f78 5f6f  (self.groupBox_o
-000049f0: 6273 5f76 6965 775f 6f70 7469 6f6e 7329  bs_view_options)
-00004a00: 0a20 2020 2020 2020 2073 656c 662e 6368  .        self.ch
-00004a10: 6563 6b42 6f78 5f6f 6273 5f70 6c6f 745f  eckBox_obs_plot_
-00004a20: 7265 6475 6365 645f 6f62 7365 7276 6174  reduced_observat
-00004a30: 696f 6e73 2e73 6574 4368 6563 6b65 6428  ions.setChecked(
-00004a40: 5472 7565 290a 2020 2020 2020 2020 7365  True).        se
-00004a50: 6c66 2e63 6865 636b 426f 785f 6f62 735f  lf.checkBox_obs_
-00004a60: 706c 6f74 5f72 6564 7563 6564 5f6f 6273  plot_reduced_obs
-00004a70: 6572 7661 7469 6f6e 732e 7365 744f 626a  ervations.setObj
-00004a80: 6563 744e 616d 6528 2263 6865 636b 426f  ectName("checkBo
-00004a90: 785f 6f62 735f 706c 6f74 5f72 6564 7563  x_obs_plot_reduc
-00004aa0: 6564 5f6f 6273 6572 7661 7469 6f6e 7322  ed_observations"
-00004ab0: 290a 2020 2020 2020 2020 7365 6c66 2e76  ).        self.v
-00004ac0: 6572 7469 6361 6c4c 6179 6f75 745f 392e  erticalLayout_9.
-00004ad0: 6164 6457 6964 6765 7428 7365 6c66 2e63  addWidget(self.c
-00004ae0: 6865 636b 426f 785f 6f62 735f 706c 6f74  heckBox_obs_plot
-00004af0: 5f72 6564 7563 6564 5f6f 6273 6572 7661  _reduced_observa
-00004b00: 7469 6f6e 7329 0a20 2020 2020 2020 2073  tions).        s
-00004b10: 656c 662e 6368 6563 6b42 6f78 5f6f 6273  elf.checkBox_obs
-00004b20: 5f70 6c6f 745f 7365 7475 705f 6461 7461  _plot_setup_data
-00004b30: 203d 2051 7457 6964 6765 7473 2e51 4368   = QtWidgets.QCh
-00004b40: 6563 6b42 6f78 2873 656c 662e 6772 6f75  eckBox(self.grou
-00004b50: 7042 6f78 5f6f 6273 5f76 6965 775f 6f70  pBox_obs_view_op
-00004b60: 7469 6f6e 7329 0a20 2020 2020 2020 2073  tions).        s
-00004b70: 656c 662e 6368 6563 6b42 6f78 5f6f 6273  elf.checkBox_obs
-00004b80: 5f70 6c6f 745f 7365 7475 705f 6461 7461  _plot_setup_data
-00004b90: 2e73 6574 4368 6563 6b65 6428 5472 7565  .setChecked(True
-00004ba0: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
-00004bb0: 6865 636b 426f 785f 6f62 735f 706c 6f74  heckBox_obs_plot
-00004bc0: 5f73 6574 7570 5f64 6174 612e 7365 744f  _setup_data.setO
-00004bd0: 626a 6563 744e 616d 6528 2263 6865 636b  bjectName("check
-00004be0: 426f 785f 6f62 735f 706c 6f74 5f73 6574  Box_obs_plot_set
-00004bf0: 7570 5f64 6174 6122 290a 2020 2020 2020  up_data").      
-00004c00: 2020 7365 6c66 2e76 6572 7469 6361 6c4c    self.verticalL
-00004c10: 6179 6f75 745f 392e 6164 6457 6964 6765  ayout_9.addWidge
-00004c20: 7428 7365 6c66 2e63 6865 636b 426f 785f  t(self.checkBox_
-00004c30: 6f62 735f 706c 6f74 5f73 6574 7570 5f64  obs_plot_setup_d
-00004c40: 6174 6129 0a20 2020 2020 2020 2073 656c  ata).        sel
-00004c50: 662e 7665 7274 6963 616c 4c61 796f 7574  f.verticalLayout
-00004c60: 5f35 2e61 6464 5769 6467 6574 2873 656c  _5.addWidget(sel
-00004c70: 662e 6772 6f75 7042 6f78 5f6f 6273 5f76  f.groupBox_obs_v
-00004c80: 6965 775f 6f70 7469 6f6e 7329 0a20 2020  iew_options).   
-00004c90: 2020 2020 2073 656c 662e 7461 6257 6964       self.tabWid
-00004ca0: 6765 745f 6f62 7365 7276 6174 696f 6e73  get_observations
-00004cb0: 203d 2051 7457 6964 6765 7473 2e51 5461   = QtWidgets.QTa
-00004cc0: 6257 6964 6765 7428 7365 6c66 2e73 706c  bWidget(self.spl
-00004cd0: 6974 7465 725f 6f62 7329 0a20 2020 2020  itter_obs).     
-00004ce0: 2020 2073 697a 6550 6f6c 6963 7920 3d20     sizePolicy = 
-00004cf0: 5174 5769 6467 6574 732e 5153 697a 6550  QtWidgets.QSizeP
-00004d00: 6f6c 6963 7928 5174 5769 6467 6574 732e  olicy(QtWidgets.
-00004d10: 5153 697a 6550 6f6c 6963 792e 4578 7061  QSizePolicy.Expa
-00004d20: 6e64 696e 672c 2051 7457 6964 6765 7473  nding, QtWidgets
-00004d30: 2e51 5369 7a65 506f 6c69 6379 2e45 7870  .QSizePolicy.Exp
-00004d40: 616e 6469 6e67 290a 2020 2020 2020 2020  anding).        
-00004d50: 7369 7a65 506f 6c69 6379 2e73 6574 486f  sizePolicy.setHo
-00004d60: 7269 7a6f 6e74 616c 5374 7265 7463 6828  rizontalStretch(
-00004d70: 3129 0a20 2020 2020 2020 2073 697a 6550  1).        sizeP
-00004d80: 6f6c 6963 792e 7365 7456 6572 7469 6361  olicy.setVertica
-00004d90: 6c53 7472 6574 6368 2830 290a 2020 2020  lStretch(0).    
-00004da0: 2020 2020 7369 7a65 506f 6c69 6379 2e73      sizePolicy.s
-00004db0: 6574 4865 6967 6874 466f 7257 6964 7468  etHeightForWidth
-00004dc0: 2873 656c 662e 7461 6257 6964 6765 745f  (self.tabWidget_
-00004dd0: 6f62 7365 7276 6174 696f 6e73 2e73 697a  observations.siz
-00004de0: 6550 6f6c 6963 7928 292e 6861 7348 6569  ePolicy().hasHei
-00004df0: 6768 7446 6f72 5769 6474 6828 2929 0a20  ghtForWidth()). 
-00004e00: 2020 2020 2020 2073 656c 662e 7461 6257         self.tabW
-00004e10: 6964 6765 745f 6f62 7365 7276 6174 696f  idget_observatio
-00004e20: 6e73 2e73 6574 5369 7a65 506f 6c69 6379  ns.setSizePolicy
-00004e30: 2873 697a 6550 6f6c 6963 7929 0a20 2020  (sizePolicy).   
-00004e40: 2020 2020 2073 656c 662e 7461 6257 6964       self.tabWid
-00004e50: 6765 745f 6f62 7365 7276 6174 696f 6e73  get_observations
-00004e60: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
-00004e70: 7461 6257 6964 6765 745f 6f62 7365 7276  tabWidget_observ
-00004e80: 6174 696f 6e73 2229 0a20 2020 2020 2020  ations").       
-00004e90: 2073 656c 662e 7461 625f 6f62 7365 7276   self.tab_observ
-00004ea0: 6174 696f 6e73 5f70 6c6f 7473 203d 2051  ations_plots = Q
-00004eb0: 7457 6964 6765 7473 2e51 5769 6467 6574  tWidgets.QWidget
-00004ec0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-00004ed0: 7461 625f 6f62 7365 7276 6174 696f 6e73  tab_observations
-00004ee0: 5f70 6c6f 7473 2e73 6574 4f62 6a65 6374  _plots.setObject
-00004ef0: 4e61 6d65 2822 7461 625f 6f62 7365 7276  Name("tab_observ
-00004f00: 6174 696f 6e73 5f70 6c6f 7473 2229 0a20  ations_plots"). 
-00004f10: 2020 2020 2020 2073 656c 662e 7665 7274         self.vert
-00004f20: 6963 616c 4c61 796f 7574 5f38 203d 2051  icalLayout_8 = Q
-00004f30: 7457 6964 6765 7473 2e51 5642 6f78 4c61  tWidgets.QVBoxLa
-00004f40: 796f 7574 2873 656c 662e 7461 625f 6f62  yout(self.tab_ob
-00004f50: 7365 7276 6174 696f 6e73 5f70 6c6f 7473  servations_plots
-00004f60: 290a 2020 2020 2020 2020 7365 6c66 2e76  ).        self.v
-00004f70: 6572 7469 6361 6c4c 6179 6f75 745f 382e  erticalLayout_8.
-00004f80: 7365 744f 626a 6563 744e 616d 6528 2276  setObjectName("v
-00004f90: 6572 7469 6361 6c4c 6179 6f75 745f 3822  erticalLayout_8"
-00004fa0: 290a 2020 2020 2020 2020 7365 6c66 2e47  ).        self.G
-00004fb0: 7261 7068 6963 734c 6179 6f75 7457 6964  raphicsLayoutWid
-00004fc0: 6765 745f 6f62 7365 7276 6174 696f 6e73  get_observations
-00004fd0: 203d 2047 7261 7068 6963 734c 6179 6f75   = GraphicsLayou
-00004fe0: 7457 6964 6765 7428 7365 6c66 2e74 6162  tWidget(self.tab
-00004ff0: 5f6f 6273 6572 7661 7469 6f6e 735f 706c  _observations_pl
-00005000: 6f74 7329 0a20 2020 2020 2020 2073 656c  ots).        sel
-00005010: 662e 4772 6170 6869 6373 4c61 796f 7574  f.GraphicsLayout
-00005020: 5769 6467 6574 5f6f 6273 6572 7661 7469  Widget_observati
-00005030: 6f6e 732e 7365 744f 626a 6563 744e 616d  ons.setObjectNam
-00005040: 6528 2247 7261 7068 6963 734c 6179 6f75  e("GraphicsLayou
-00005050: 7457 6964 6765 745f 6f62 7365 7276 6174  tWidget_observat
-00005060: 696f 6e73 2229 0a20 2020 2020 2020 2073  ions").        s
-00005070: 656c 662e 7665 7274 6963 616c 4c61 796f  elf.verticalLayo
-00005080: 7574 5f38 2e61 6464 5769 6467 6574 2873  ut_8.addWidget(s
-00005090: 656c 662e 4772 6170 6869 6373 4c61 796f  elf.GraphicsLayo
-000050a0: 7574 5769 6467 6574 5f6f 6273 6572 7661  utWidget_observa
-000050b0: 7469 6f6e 7329 0a20 2020 2020 2020 2073  tions).        s
-000050c0: 656c 662e 7461 6257 6964 6765 745f 6f62  elf.tabWidget_ob
-000050d0: 7365 7276 6174 696f 6e73 2e61 6464 5461  servations.addTa
-000050e0: 6228 7365 6c66 2e74 6162 5f6f 6273 6572  b(self.tab_obser
-000050f0: 7661 7469 6f6e 735f 706c 6f74 732c 2022  vations_plots, "
-00005100: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00005110: 7461 625f 6f62 7365 7276 6174 696f 6e73  tab_observations
-00005120: 5f74 6162 6c65 203d 2051 7457 6964 6765  _table = QtWidge
-00005130: 7473 2e51 5769 6467 6574 2829 0a20 2020  ts.QWidget().   
-00005140: 2020 2020 2073 656c 662e 7461 625f 6f62       self.tab_ob
-00005150: 7365 7276 6174 696f 6e73 5f74 6162 6c65  servations_table
-00005160: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
-00005170: 7461 625f 6f62 7365 7276 6174 696f 6e73  tab_observations
-00005180: 5f74 6162 6c65 2229 0a20 2020 2020 2020  _table").       
-00005190: 2073 656c 662e 7665 7274 6963 616c 4c61   self.verticalLa
-000051a0: 796f 7574 5f36 203d 2051 7457 6964 6765  yout_6 = QtWidge
-000051b0: 7473 2e51 5642 6f78 4c61 796f 7574 2873  ts.QVBoxLayout(s
-000051c0: 656c 662e 7461 625f 6f62 7365 7276 6174  elf.tab_observat
-000051d0: 696f 6e73 5f74 6162 6c65 290a 2020 2020  ions_table).    
-000051e0: 2020 2020 7365 6c66 2e76 6572 7469 6361      self.vertica
-000051f0: 6c4c 6179 6f75 745f 362e 7365 744f 626a  lLayout_6.setObj
-00005200: 6563 744e 616d 6528 2276 6572 7469 6361  ectName("vertica
-00005210: 6c4c 6179 6f75 745f 3622 290a 2020 2020  lLayout_6").    
-00005220: 2020 2020 7365 6c66 2e74 6162 6c65 5669      self.tableVi
-00005230: 6577 5f6f 6273 6572 7661 7469 6f6e 7320  ew_observations 
-00005240: 3d20 5174 5769 6467 6574 732e 5154 6162  = QtWidgets.QTab
-00005250: 6c65 5669 6577 2873 656c 662e 7461 625f  leView(self.tab_
-00005260: 6f62 7365 7276 6174 696f 6e73 5f74 6162  observations_tab
-00005270: 6c65 290a 2020 2020 2020 2020 7365 6c66  le).        self
-00005280: 2e74 6162 6c65 5669 6577 5f6f 6273 6572  .tableView_obser
-00005290: 7661 7469 6f6e 732e 7365 744f 626a 6563  vations.setObjec
-000052a0: 744e 616d 6528 2274 6162 6c65 5669 6577  tName("tableView
-000052b0: 5f6f 6273 6572 7661 7469 6f6e 7322 290a  _observations").
-000052c0: 2020 2020 2020 2020 7365 6c66 2e76 6572          self.ver
-000052d0: 7469 6361 6c4c 6179 6f75 745f 362e 6164  ticalLayout_6.ad
-000052e0: 6457 6964 6765 7428 7365 6c66 2e74 6162  dWidget(self.tab
-000052f0: 6c65 5669 6577 5f6f 6273 6572 7661 7469  leView_observati
-00005300: 6f6e 7329 0a20 2020 2020 2020 2073 656c  ons).        sel
-00005310: 662e 7461 6257 6964 6765 745f 6f62 7365  f.tabWidget_obse
-00005320: 7276 6174 696f 6e73 2e61 6464 5461 6228  rvations.addTab(
-00005330: 7365 6c66 2e74 6162 5f6f 6273 6572 7661  self.tab_observa
-00005340: 7469 6f6e 735f 7461 626c 652c 2022 2229  tions_table, "")
-00005350: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
-00005360: 625f 7375 7276 6579 7320 3d20 5174 5769  b_surveys = QtWi
-00005370: 6467 6574 732e 5157 6964 6765 7428 290a  dgets.QWidget().
-00005380: 2020 2020 2020 2020 7365 6c66 2e74 6162          self.tab
-00005390: 5f73 7572 7665 7973 2e73 6574 4f62 6a65  _surveys.setObje
-000053a0: 6374 4e61 6d65 2822 7461 625f 7375 7276  ctName("tab_surv
-000053b0: 6579 7322 290a 2020 2020 2020 2020 7365  eys").        se
-000053c0: 6c66 2e76 6572 7469 6361 6c4c 6179 6f75  lf.verticalLayou
-000053d0: 745f 3337 203d 2051 7457 6964 6765 7473  t_37 = QtWidgets
-000053e0: 2e51 5642 6f78 4c61 796f 7574 2873 656c  .QVBoxLayout(sel
-000053f0: 662e 7461 625f 7375 7276 6579 7329 0a20  f.tab_surveys). 
-00005400: 2020 2020 2020 2073 656c 662e 7665 7274         self.vert
-00005410: 6963 616c 4c61 796f 7574 5f33 372e 7365  icalLayout_37.se
-00005420: 744f 626a 6563 744e 616d 6528 2276 6572  tObjectName("ver
-00005430: 7469 6361 6c4c 6179 6f75 745f 3337 2229  ticalLayout_37")
-00005440: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
-00005450: 626c 6556 6965 775f 7375 7276 6579 7320  bleView_surveys 
-00005460: 3d20 5174 5769 6467 6574 732e 5154 6162  = QtWidgets.QTab
-00005470: 6c65 5669 6577 2873 656c 662e 7461 625f  leView(self.tab_
-00005480: 7375 7276 6579 7329 0a20 2020 2020 2020  surveys).       
-00005490: 2073 656c 662e 7461 626c 6556 6965 775f   self.tableView_
-000054a0: 7375 7276 6579 732e 7365 7443 6f6e 7465  surveys.setConte
-000054b0: 7874 4d65 6e75 506f 6c69 6379 2851 7443  xtMenuPolicy(QtC
-000054c0: 6f72 652e 5174 2e43 7573 746f 6d43 6f6e  ore.Qt.CustomCon
-000054d0: 7465 7874 4d65 6e75 290a 2020 2020 2020  textMenu).      
-000054e0: 2020 7365 6c66 2e74 6162 6c65 5669 6577    self.tableView
-000054f0: 5f73 7572 7665 7973 2e73 6574 4f62 6a65  _surveys.setObje
-00005500: 6374 4e61 6d65 2822 7461 626c 6556 6965  ctName("tableVie
-00005510: 775f 7375 7276 6579 7322 290a 2020 2020  w_surveys").    
-00005520: 2020 2020 7365 6c66 2e76 6572 7469 6361      self.vertica
-00005530: 6c4c 6179 6f75 745f 3337 2e61 6464 5769  lLayout_37.addWi
-00005540: 6467 6574 2873 656c 662e 7461 626c 6556  dget(self.tableV
-00005550: 6965 775f 7375 7276 6579 7329 0a20 2020  iew_surveys).   
-00005560: 2020 2020 2073 656c 662e 7461 6257 6964       self.tabWid
-00005570: 6765 745f 6f62 7365 7276 6174 696f 6e73  get_observations
-00005580: 2e61 6464 5461 6228 7365 6c66 2e74 6162  .addTab(self.tab
-00005590: 5f73 7572 7665 7973 2c20 2222 290a 2020  _surveys, "").  
-000055a0: 2020 2020 2020 7365 6c66 2e74 6162 5f6f        self.tab_o
-000055b0: 6273 6572 7661 7469 6f6e 735f 7365 7475  bservations_setu
-000055c0: 7073 203d 2051 7457 6964 6765 7473 2e51  ps = QtWidgets.Q
-000055d0: 5769 6467 6574 2829 0a20 2020 2020 2020  Widget().       
-000055e0: 2073 656c 662e 7461 625f 6f62 7365 7276   self.tab_observ
-000055f0: 6174 696f 6e73 5f73 6574 7570 732e 7365  ations_setups.se
-00005600: 744f 626a 6563 744e 616d 6528 2274 6162  tObjectName("tab
-00005610: 5f6f 6273 6572 7661 7469 6f6e 735f 7365  _observations_se
-00005620: 7475 7073 2229 0a20 2020 2020 2020 2073  tups").        s
-00005630: 656c 662e 7665 7274 6963 616c 4c61 796f  elf.verticalLayo
-00005640: 7574 5f31 3120 3d20 5174 5769 6467 6574  ut_11 = QtWidget
-00005650: 732e 5156 426f 784c 6179 6f75 7428 7365  s.QVBoxLayout(se
-00005660: 6c66 2e74 6162 5f6f 6273 6572 7661 7469  lf.tab_observati
-00005670: 6f6e 735f 7365 7475 7073 290a 2020 2020  ons_setups).    
-00005680: 2020 2020 7365 6c66 2e76 6572 7469 6361      self.vertica
-00005690: 6c4c 6179 6f75 745f 3131 2e73 6574 4f62  lLayout_11.setOb
-000056a0: 6a65 6374 4e61 6d65 2822 7665 7274 6963  jectName("vertic
-000056b0: 616c 4c61 796f 7574 5f31 3122 290a 2020  alLayout_11").  
-000056c0: 2020 2020 2020 7365 6c66 2e74 6162 6c65        self.table
-000056d0: 5669 6577 5f6f 6273 6572 7661 7469 6f6e  View_observation
-000056e0: 735f 7365 7475 7073 203d 2051 7457 6964  s_setups = QtWid
-000056f0: 6765 7473 2e51 5461 626c 6556 6965 7728  gets.QTableView(
-00005700: 7365 6c66 2e74 6162 5f6f 6273 6572 7661  self.tab_observa
-00005710: 7469 6f6e 735f 7365 7475 7073 290a 2020  tions_setups).  
-00005720: 2020 2020 2020 7365 6c66 2e74 6162 6c65        self.table
-00005730: 5669 6577 5f6f 6273 6572 7661 7469 6f6e  View_observation
-00005740: 735f 7365 7475 7073 2e73 6574 4f62 6a65  s_setups.setObje
-00005750: 6374 4e61 6d65 2822 7461 626c 6556 6965  ctName("tableVie
-00005760: 775f 6f62 7365 7276 6174 696f 6e73 5f73  w_observations_s
-00005770: 6574 7570 7322 290a 2020 2020 2020 2020  etups").        
-00005780: 7365 6c66 2e76 6572 7469 6361 6c4c 6179  self.verticalLay
-00005790: 6f75 745f 3131 2e61 6464 5769 6467 6574  out_11.addWidget
-000057a0: 2873 656c 662e 7461 626c 6556 6965 775f  (self.tableView_
-000057b0: 6f62 7365 7276 6174 696f 6e73 5f73 6574  observations_set
-000057c0: 7570 7329 0a20 2020 2020 2020 2073 656c  ups).        sel
-000057d0: 662e 6772 6f75 7042 6f78 5f6f 6273 5f73  f.groupBox_obs_s
-000057e0: 6574 7570 735f 6170 706c 6965 645f 636f  etups_applied_co
-000057f0: 7272 6563 7469 6f6e 7320 3d20 5174 5769  rrections = QtWi
-00005800: 6467 6574 732e 5147 726f 7570 426f 7828  dgets.QGroupBox(
-00005810: 7365 6c66 2e74 6162 5f6f 6273 6572 7661  self.tab_observa
-00005820: 7469 6f6e 735f 7365 7475 7073 290a 2020  tions_setups).  
-00005830: 2020 2020 2020 7365 6c66 2e67 726f 7570        self.group
-00005840: 426f 785f 6f62 735f 7365 7475 7073 5f61  Box_obs_setups_a
-00005850: 7070 6c69 6564 5f63 6f72 7265 6374 696f  pplied_correctio
-00005860: 6e73 2e73 6574 4f62 6a65 6374 4e61 6d65  ns.setObjectName
-00005870: 2822 6772 6f75 7042 6f78 5f6f 6273 5f73  ("groupBox_obs_s
-00005880: 6574 7570 735f 6170 706c 6965 645f 636f  etups_applied_co
-00005890: 7272 6563 7469 6f6e 7322 290a 2020 2020  rrections").    
-000058a0: 2020 2020 7365 6c66 2e66 6f72 6d4c 6179      self.formLay
-000058b0: 6f75 745f 3620 3d20 5174 5769 6467 6574  out_6 = QtWidget
-000058c0: 732e 5146 6f72 6d4c 6179 6f75 7428 7365  s.QFormLayout(se
-000058d0: 6c66 2e67 726f 7570 426f 785f 6f62 735f  lf.groupBox_obs_
-000058e0: 7365 7475 7073 5f61 7070 6c69 6564 5f63  setups_applied_c
-000058f0: 6f72 7265 6374 696f 6e73 290a 2020 2020  orrections).    
-00005900: 2020 2020 7365 6c66 2e66 6f72 6d4c 6179      self.formLay
-00005910: 6f75 745f 362e 7365 744f 626a 6563 744e  out_6.setObjectN
-00005920: 616d 6528 2266 6f72 6d4c 6179 6f75 745f  ame("formLayout_
-00005930: 3622 290a 2020 2020 2020 2020 7365 6c66  6").        self
-00005940: 2e6c 6162 656c 5f6f 6273 5f73 6574 7570  .label_obs_setup
-00005950: 735f 3120 3d20 5174 5769 6467 6574 732e  s_1 = QtWidgets.
-00005960: 514c 6162 656c 2873 656c 662e 6772 6f75  QLabel(self.grou
-00005970: 7042 6f78 5f6f 6273 5f73 6574 7570 735f  pBox_obs_setups_
-00005980: 6170 706c 6965 645f 636f 7272 6563 7469  applied_correcti
-00005990: 6f6e 7329 0a20 2020 2020 2020 2073 656c  ons).        sel
-000059a0: 662e 6c61 6265 6c5f 6f62 735f 7365 7475  f.label_obs_setu
-000059b0: 7073 5f31 2e73 6574 4f62 6a65 6374 4e61  ps_1.setObjectNa
-000059c0: 6d65 2822 6c61 6265 6c5f 6f62 735f 7365  me("label_obs_se
-000059d0: 7475 7073 5f31 2229 0a20 2020 2020 2020  tups_1").       
-000059e0: 2073 656c 662e 666f 726d 4c61 796f 7574   self.formLayout
-000059f0: 5f36 2e73 6574 5769 6467 6574 2830 2c20  _6.setWidget(0, 
-00005a00: 5174 5769 6467 6574 732e 5146 6f72 6d4c  QtWidgets.QFormL
-00005a10: 6179 6f75 742e 4c61 6265 6c52 6f6c 652c  ayout.LabelRole,
-00005a20: 2073 656c 662e 6c61 6265 6c5f 6f62 735f   self.label_obs_
-00005a30: 7365 7475 7073 5f31 290a 2020 2020 2020  setups_1).      
-00005a40: 2020 7365 6c66 2e6c 6162 656c 5f6f 6273    self.label_obs
-00005a50: 5f73 6574 7570 735f 7469 6461 6c5f 636f  _setups_tidal_co
-00005a60: 7272 203d 2051 7457 6964 6765 7473 2e51  rr = QtWidgets.Q
-00005a70: 4c61 6265 6c28 7365 6c66 2e67 726f 7570  Label(self.group
-00005a80: 426f 785f 6f62 735f 7365 7475 7073 5f61  Box_obs_setups_a
-00005a90: 7070 6c69 6564 5f63 6f72 7265 6374 696f  pplied_correctio
-00005aa0: 6e73 290a 2020 2020 2020 2020 7365 6c66  ns).        self
-00005ab0: 2e6c 6162 656c 5f6f 6273 5f73 6574 7570  .label_obs_setup
-00005ac0: 735f 7469 6461 6c5f 636f 7272 2e73 6574  s_tidal_corr.set
-00005ad0: 5465 7874 2822 2229 0a20 2020 2020 2020  Text("").       
-00005ae0: 2073 656c 662e 6c61 6265 6c5f 6f62 735f   self.label_obs_
-00005af0: 7365 7475 7073 5f74 6964 616c 5f63 6f72  setups_tidal_cor
-00005b00: 722e 7365 744f 626a 6563 744e 616d 6528  r.setObjectName(
-00005b10: 226c 6162 656c 5f6f 6273 5f73 6574 7570  "label_obs_setup
-00005b20: 735f 7469 6461 6c5f 636f 7272 2229 0a20  s_tidal_corr"). 
-00005b30: 2020 2020 2020 2073 656c 662e 666f 726d         self.form
-00005b40: 4c61 796f 7574 5f36 2e73 6574 5769 6467  Layout_6.setWidg
-00005b50: 6574 2830 2c20 5174 5769 6467 6574 732e  et(0, QtWidgets.
-00005b60: 5146 6f72 6d4c 6179 6f75 742e 4669 656c  QFormLayout.Fiel
-00005b70: 6452 6f6c 652c 2073 656c 662e 6c61 6265  dRole, self.labe
-00005b80: 6c5f 6f62 735f 7365 7475 7073 5f74 6964  l_obs_setups_tid
-00005b90: 616c 5f63 6f72 7229 0a20 2020 2020 2020  al_corr).       
-00005ba0: 2073 656c 662e 6c61 6265 6c5f 6f62 735f   self.label_obs_
-00005bb0: 7365 7475 7073 5f32 203d 2051 7457 6964  setups_2 = QtWid
-00005bc0: 6765 7473 2e51 4c61 6265 6c28 7365 6c66  gets.QLabel(self
-00005bd0: 2e67 726f 7570 426f 785f 6f62 735f 7365  .groupBox_obs_se
-00005be0: 7475 7073 5f61 7070 6c69 6564 5f63 6f72  tups_applied_cor
-00005bf0: 7265 6374 696f 6e73 290a 2020 2020 2020  rections).      
-00005c00: 2020 7365 6c66 2e6c 6162 656c 5f6f 6273    self.label_obs
-00005c10: 5f73 6574 7570 735f 322e 7365 744f 626a  _setups_2.setObj
-00005c20: 6563 744e 616d 6528 226c 6162 656c 5f6f  ectName("label_o
-00005c30: 6273 5f73 6574 7570 735f 3222 290a 2020  bs_setups_2").  
-00005c40: 2020 2020 2020 7365 6c66 2e66 6f72 6d4c        self.formL
-00005c50: 6179 6f75 745f 362e 7365 7457 6964 6765  ayout_6.setWidge
-00005c60: 7428 312c 2051 7457 6964 6765 7473 2e51  t(1, QtWidgets.Q
-00005c70: 466f 726d 4c61 796f 7574 2e4c 6162 656c  FormLayout.Label
-00005c80: 526f 6c65 2c20 7365 6c66 2e6c 6162 656c  Role, self.label
-00005c90: 5f6f 6273 5f73 6574 7570 735f 3229 0a20  _obs_setups_2). 
-00005ca0: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
-00005cb0: 6c5f 6f62 735f 7365 7475 7073 5f72 6566  l_obs_setups_ref
-00005cc0: 5f68 6569 6768 7420 3d20 5174 5769 6467  _height = QtWidg
-00005cd0: 6574 732e 514c 6162 656c 2873 656c 662e  ets.QLabel(self.
-00005ce0: 6772 6f75 7042 6f78 5f6f 6273 5f73 6574  groupBox_obs_set
-00005cf0: 7570 735f 6170 706c 6965 645f 636f 7272  ups_applied_corr
-00005d00: 6563 7469 6f6e 7329 0a20 2020 2020 2020  ections).       
-00005d10: 2073 656c 662e 6c61 6265 6c5f 6f62 735f   self.label_obs_
-00005d20: 7365 7475 7073 5f72 6566 5f68 6569 6768  setups_ref_heigh
-00005d30: 742e 7365 7454 6578 7428 2222 290a 2020  t.setText("").  
-00005d40: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
-00005d50: 5f6f 6273 5f73 6574 7570 735f 7265 665f  _obs_setups_ref_
-00005d60: 6865 6967 6874 2e73 6574 4f62 6a65 6374  height.setObject
-00005d70: 4e61 6d65 2822 6c61 6265 6c5f 6f62 735f  Name("label_obs_
-00005d80: 7365 7475 7073 5f72 6566 5f68 6569 6768  setups_ref_heigh
-00005d90: 7422 290a 2020 2020 2020 2020 7365 6c66  t").        self
-00005da0: 2e66 6f72 6d4c 6179 6f75 745f 362e 7365  .formLayout_6.se
-00005db0: 7457 6964 6765 7428 312c 2051 7457 6964  tWidget(1, QtWid
-00005dc0: 6765 7473 2e51 466f 726d 4c61 796f 7574  gets.QFormLayout
-00005dd0: 2e46 6965 6c64 526f 6c65 2c20 7365 6c66  .FieldRole, self
-00005de0: 2e6c 6162 656c 5f6f 6273 5f73 6574 7570  .label_obs_setup
-00005df0: 735f 7265 665f 6865 6967 6874 290a 2020  s_ref_height).  
-00005e00: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
-00005e10: 5f32 3720 3d20 5174 5769 6467 6574 732e  _27 = QtWidgets.
-00005e20: 514c 6162 656c 2873 656c 662e 6772 6f75  QLabel(self.grou
-00005e30: 7042 6f78 5f6f 6273 5f73 6574 7570 735f  pBox_obs_setups_
-00005e40: 6170 706c 6965 645f 636f 7272 6563 7469  applied_correcti
-00005e50: 6f6e 7329 0a20 2020 2020 2020 2073 656c  ons).        sel
-00005e60: 662e 6c61 6265 6c5f 3237 2e73 6574 4f62  f.label_27.setOb
-00005e70: 6a65 6374 4e61 6d65 2822 6c61 6265 6c5f  jectName("label_
-00005e80: 3237 2229 0a20 2020 2020 2020 2073 656c  27").        sel
-00005e90: 662e 666f 726d 4c61 796f 7574 5f36 2e73  f.formLayout_6.s
-00005ea0: 6574 5769 6467 6574 2832 2c20 5174 5769  etWidget(2, QtWi
-00005eb0: 6467 6574 732e 5146 6f72 6d4c 6179 6f75  dgets.QFormLayou
-00005ec0: 742e 4c61 6265 6c52 6f6c 652c 2073 656c  t.LabelRole, sel
-00005ed0: 662e 6c61 6265 6c5f 3237 290a 2020 2020  f.label_27).    
-00005ee0: 2020 2020 7365 6c66 2e6c 6162 656c 5f6f      self.label_o
-00005ef0: 6273 5f73 6574 7570 735f 3320 3d20 5174  bs_setups_3 = Qt
-00005f00: 5769 6467 6574 732e 514c 6162 656c 2873  Widgets.QLabel(s
-00005f10: 656c 662e 6772 6f75 7042 6f78 5f6f 6273  elf.groupBox_obs
-00005f20: 5f73 6574 7570 735f 6170 706c 6965 645f  _setups_applied_
-00005f30: 636f 7272 6563 7469 6f6e 7329 0a20 2020  corrections).   
-00005f40: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
-00005f50: 6f62 735f 7365 7475 7073 5f33 2e73 6574  obs_setups_3.set
-00005f60: 4f62 6a65 6374 4e61 6d65 2822 6c61 6265  ObjectName("labe
-00005f70: 6c5f 6f62 735f 7365 7475 7073 5f33 2229  l_obs_setups_3")
-00005f80: 0a20 2020 2020 2020 2073 656c 662e 666f  .        self.fo
-00005f90: 726d 4c61 796f 7574 5f36 2e73 6574 5769  rmLayout_6.setWi
-00005fa0: 6467 6574 2833 2c20 5174 5769 6467 6574  dget(3, QtWidget
-00005fb0: 732e 5146 6f72 6d4c 6179 6f75 742e 4c61  s.QFormLayout.La
-00005fc0: 6265 6c52 6f6c 652c 2073 656c 662e 6c61  belRole, self.la
-00005fd0: 6265 6c5f 6f62 735f 7365 7475 7073 5f33  bel_obs_setups_3
-00005fe0: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
+00000290: 2020 2020 2073 656c 662e 7665 7274 6963       self.vertic
+000002a0: 616c 4c61 796f 7574 5f33 3720 3d20 5174  alLayout_37 = Qt
+000002b0: 5769 6467 6574 732e 5156 426f 784c 6179  Widgets.QVBoxLay
+000002c0: 6f75 7428 7365 6c66 2e63 656e 7472 616c  out(self.central
+000002d0: 7769 6467 6574 290a 2020 2020 2020 2020  widget).        
+000002e0: 7365 6c66 2e76 6572 7469 6361 6c4c 6179  self.verticalLay
+000002f0: 6f75 745f 3337 2e73 6574 4f62 6a65 6374  out_37.setObject
+00000300: 4e61 6d65 2822 7665 7274 6963 616c 4c61  Name("verticalLa
+00000310: 796f 7574 5f33 3722 290a 2020 2020 2020  yout_37").      
+00000320: 2020 7365 6c66 2e74 6162 5769 6467 6574    self.tabWidget
+00000330: 5f4d 6169 6e20 3d20 5174 5769 6467 6574  _Main = QtWidget
+00000340: 732e 5154 6162 5769 6467 6574 2873 656c  s.QTabWidget(sel
+00000350: 662e 6365 6e74 7261 6c77 6964 6765 7429  f.centralwidget)
+00000360: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
+00000370: 6257 6964 6765 745f 4d61 696e 2e73 6574  bWidget_Main.set
+00000380: 5461 6250 6f73 6974 696f 6e28 5174 5769  TabPosition(QtWi
+00000390: 6467 6574 732e 5154 6162 5769 6467 6574  dgets.QTabWidget
+000003a0: 2e45 6173 7429 0a20 2020 2020 2020 2073  .East).        s
+000003b0: 656c 662e 7461 6257 6964 6765 745f 4d61  elf.tabWidget_Ma
+000003c0: 696e 2e73 6574 4d6f 7661 626c 6528 5472  in.setMovable(Tr
+000003d0: 7565 290a 2020 2020 2020 2020 7365 6c66  ue).        self
+000003e0: 2e74 6162 5769 6467 6574 5f4d 6169 6e2e  .tabWidget_Main.
+000003f0: 7365 744f 626a 6563 744e 616d 6528 2274  setObjectName("t
+00000400: 6162 5769 6467 6574 5f4d 6169 6e22 290a  abWidget_Main").
+00000410: 2020 2020 2020 2020 7365 6c66 2e74 6162          self.tab
+00000420: 5f6d 6169 6e5f 7374 6174 696f 6e73 203d  _main_stations =
+00000430: 2051 7457 6964 6765 7473 2e51 5769 6467   QtWidgets.QWidg
+00000440: 6574 2829 0a20 2020 2020 2020 2073 656c  et().        sel
+00000450: 662e 7461 625f 6d61 696e 5f73 7461 7469  f.tab_main_stati
+00000460: 6f6e 732e 7365 744f 626a 6563 744e 616d  ons.setObjectNam
+00000470: 6528 2274 6162 5f6d 6169 6e5f 7374 6174  e("tab_main_stat
+00000480: 696f 6e73 2229 0a20 2020 2020 2020 2073  ions").        s
+00000490: 656c 662e 7665 7274 6963 616c 4c61 796f  elf.verticalLayo
+000004a0: 7574 5f34 203d 2051 7457 6964 6765 7473  ut_4 = QtWidgets
+000004b0: 2e51 5642 6f78 4c61 796f 7574 2873 656c  .QVBoxLayout(sel
+000004c0: 662e 7461 625f 6d61 696e 5f73 7461 7469  f.tab_main_stati
+000004d0: 6f6e 7329 0a20 2020 2020 2020 2073 656c  ons).        sel
+000004e0: 662e 7665 7274 6963 616c 4c61 796f 7574  f.verticalLayout
+000004f0: 5f34 2e73 6574 4f62 6a65 6374 4e61 6d65  _4.setObjectName
+00000500: 2822 7665 7274 6963 616c 4c61 796f 7574  ("verticalLayout
+00000510: 5f34 2229 0a20 2020 2020 2020 2073 656c  _4").        sel
+00000520: 662e 686f 7269 7a6f 6e74 616c 4c61 796f  f.horizontalLayo
+00000530: 7574 5f32 203d 2051 7457 6964 6765 7473  ut_2 = QtWidgets
+00000540: 2e51 4842 6f78 4c61 796f 7574 2829 0a20  .QHBoxLayout(). 
+00000550: 2020 2020 2020 2073 656c 662e 686f 7269         self.hori
+00000560: 7a6f 6e74 616c 4c61 796f 7574 5f32 2e73  zontalLayout_2.s
+00000570: 6574 4f62 6a65 6374 4e61 6d65 2822 686f  etObjectName("ho
+00000580: 7269 7a6f 6e74 616c 4c61 796f 7574 5f32  rizontalLayout_2
+00000590: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+000005a0: 7665 7274 6963 616c 4c61 796f 7574 5f33  verticalLayout_3
+000005b0: 203d 2051 7457 6964 6765 7473 2e51 5642   = QtWidgets.QVB
+000005c0: 6f78 4c61 796f 7574 2829 0a20 2020 2020  oxLayout().     
+000005d0: 2020 2073 656c 662e 7665 7274 6963 616c     self.vertical
+000005e0: 4c61 796f 7574 5f33 2e73 6574 4f62 6a65  Layout_3.setObje
+000005f0: 6374 4e61 6d65 2822 7665 7274 6963 616c  ctName("vertical
+00000600: 4c61 796f 7574 5f33 2229 0a20 2020 2020  Layout_3").     
+00000610: 2020 2073 656c 662e 6772 6f75 7042 6f78     self.groupBox
+00000620: 5f66 696c 7465 725f 6f70 7469 6f6e 7320  _filter_options 
+00000630: 3d20 5174 5769 6467 6574 732e 5147 726f  = QtWidgets.QGro
+00000640: 7570 426f 7828 7365 6c66 2e74 6162 5f6d  upBox(self.tab_m
+00000650: 6169 6e5f 7374 6174 696f 6e73 290a 2020  ain_stations).  
+00000660: 2020 2020 2020 7365 6c66 2e67 726f 7570        self.group
+00000670: 426f 785f 6669 6c74 6572 5f6f 7074 696f  Box_filter_optio
+00000680: 6e73 2e73 6574 456e 6162 6c65 6428 4661  ns.setEnabled(Fa
+00000690: 6c73 6529 0a20 2020 2020 2020 2073 656c  lse).        sel
+000006a0: 662e 6772 6f75 7042 6f78 5f66 696c 7465  f.groupBox_filte
+000006b0: 725f 6f70 7469 6f6e 732e 7365 7446 6c61  r_options.setFla
+000006c0: 7428 4661 6c73 6529 0a20 2020 2020 2020  t(False).       
+000006d0: 2073 656c 662e 6772 6f75 7042 6f78 5f66   self.groupBox_f
+000006e0: 696c 7465 725f 6f70 7469 6f6e 732e 7365  ilter_options.se
+000006f0: 7443 6865 636b 6162 6c65 2846 616c 7365  tCheckable(False
+00000700: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
+00000710: 726f 7570 426f 785f 6669 6c74 6572 5f6f  roupBox_filter_o
+00000720: 7074 696f 6e73 2e73 6574 4f62 6a65 6374  ptions.setObject
+00000730: 4e61 6d65 2822 6772 6f75 7042 6f78 5f66  Name("groupBox_f
+00000740: 696c 7465 725f 6f70 7469 6f6e 7322 290a  ilter_options").
+00000750: 2020 2020 2020 2020 7365 6c66 2e76 6572          self.ver
+00000760: 7469 6361 6c4c 6179 6f75 745f 3220 3d20  ticalLayout_2 = 
+00000770: 5174 5769 6467 6574 732e 5156 426f 784c  QtWidgets.QVBoxL
+00000780: 6179 6f75 7428 7365 6c66 2e67 726f 7570  ayout(self.group
+00000790: 426f 785f 6669 6c74 6572 5f6f 7074 696f  Box_filter_optio
+000007a0: 6e73 290a 2020 2020 2020 2020 7365 6c66  ns).        self
+000007b0: 2e76 6572 7469 6361 6c4c 6179 6f75 745f  .verticalLayout_
+000007c0: 322e 7365 744f 626a 6563 744e 616d 6528  2.setObjectName(
+000007d0: 2276 6572 7469 6361 6c4c 6179 6f75 745f  "verticalLayout_
+000007e0: 3222 290a 2020 2020 2020 2020 7365 6c66  2").        self
+000007f0: 2e63 6865 636b 426f 785f 6669 6c74 6572  .checkBox_filter
+00000800: 5f6f 6273 6572 7665 645f 7374 6174 5f6f  _observed_stat_o
+00000810: 6e6c 7920 3d20 5174 5769 6467 6574 732e  nly = QtWidgets.
+00000820: 5143 6865 636b 426f 7828 7365 6c66 2e67  QCheckBox(self.g
+00000830: 726f 7570 426f 785f 6669 6c74 6572 5f6f  roupBox_filter_o
+00000840: 7074 696f 6e73 290a 2020 2020 2020 2020  ptions).        
+00000850: 7365 6c66 2e63 6865 636b 426f 785f 6669  self.checkBox_fi
+00000860: 6c74 6572 5f6f 6273 6572 7665 645f 7374  lter_observed_st
+00000870: 6174 5f6f 6e6c 792e 7365 7443 6865 636b  at_only.setCheck
+00000880: 6564 2854 7275 6529 0a20 2020 2020 2020  ed(True).       
+00000890: 2073 656c 662e 6368 6563 6b42 6f78 5f66   self.checkBox_f
+000008a0: 696c 7465 725f 6f62 7365 7276 6564 5f73  ilter_observed_s
+000008b0: 7461 745f 6f6e 6c79 2e73 6574 4f62 6a65  tat_only.setObje
+000008c0: 6374 4e61 6d65 2822 6368 6563 6b42 6f78  ctName("checkBox
+000008d0: 5f66 696c 7465 725f 6f62 7365 7276 6564  _filter_observed
+000008e0: 5f73 7461 745f 6f6e 6c79 2229 0a20 2020  _stat_only").   
+000008f0: 2020 2020 2073 656c 662e 7665 7274 6963       self.vertic
+00000900: 616c 4c61 796f 7574 5f32 2e61 6464 5769  alLayout_2.addWi
+00000910: 6467 6574 2873 656c 662e 6368 6563 6b42  dget(self.checkB
+00000920: 6f78 5f66 696c 7465 725f 6f62 7365 7276  ox_filter_observ
+00000930: 6564 5f73 7461 745f 6f6e 6c79 290a 2020  ed_stat_only).  
+00000940: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
+00000950: 203d 2051 7457 6964 6765 7473 2e51 4c61   = QtWidgets.QLa
+00000960: 6265 6c28 7365 6c66 2e67 726f 7570 426f  bel(self.groupBo
+00000970: 785f 6669 6c74 6572 5f6f 7074 696f 6e73  x_filter_options
+00000980: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
+00000990: 6162 656c 2e73 6574 4f62 6a65 6374 4e61  abel.setObjectNa
+000009a0: 6d65 2822 6c61 6265 6c22 290a 2020 2020  me("label").    
+000009b0: 2020 2020 7365 6c66 2e76 6572 7469 6361      self.vertica
+000009c0: 6c4c 6179 6f75 745f 322e 6164 6457 6964  lLayout_2.addWid
+000009d0: 6765 7428 7365 6c66 2e6c 6162 656c 290a  get(self.label).
+000009e0: 2020 2020 2020 2020 7365 6c66 2e6c 696e          self.lin
+000009f0: 6545 6469 745f 6669 6c74 6572 5f73 7461  eEdit_filter_sta
+00000a00: 745f 6e61 6d65 203d 2051 7457 6964 6765  t_name = QtWidge
+00000a10: 7473 2e51 4c69 6e65 4564 6974 2873 656c  ts.QLineEdit(sel
+00000a20: 662e 6772 6f75 7042 6f78 5f66 696c 7465  f.groupBox_filte
+00000a30: 725f 6f70 7469 6f6e 7329 0a20 2020 2020  r_options).     
+00000a40: 2020 2073 656c 662e 6c69 6e65 4564 6974     self.lineEdit
+00000a50: 5f66 696c 7465 725f 7374 6174 5f6e 616d  _filter_stat_nam
+00000a60: 652e 7365 7454 6578 7428 2222 290a 2020  e.setText("").  
+00000a70: 2020 2020 2020 7365 6c66 2e6c 696e 6545        self.lineE
+00000a80: 6469 745f 6669 6c74 6572 5f73 7461 745f  dit_filter_stat_
+00000a90: 6e61 6d65 2e73 6574 4f62 6a65 6374 4e61  name.setObjectNa
+00000aa0: 6d65 2822 6c69 6e65 4564 6974 5f66 696c  me("lineEdit_fil
+00000ab0: 7465 725f 7374 6174 5f6e 616d 6522 290a  ter_stat_name").
+00000ac0: 2020 2020 2020 2020 7365 6c66 2e76 6572          self.ver
+00000ad0: 7469 6361 6c4c 6179 6f75 745f 322e 6164  ticalLayout_2.ad
+00000ae0: 6457 6964 6765 7428 7365 6c66 2e6c 696e  dWidget(self.lin
+00000af0: 6545 6469 745f 6669 6c74 6572 5f73 7461  eEdit_filter_sta
+00000b00: 745f 6e61 6d65 290a 2020 2020 2020 2020  t_name).        
+00000b10: 7365 6c66 2e76 6572 7469 6361 6c4c 6179  self.verticalLay
+00000b20: 6f75 745f 332e 6164 6457 6964 6765 7428  out_3.addWidget(
+00000b30: 7365 6c66 2e67 726f 7570 426f 785f 6669  self.groupBox_fi
+00000b40: 6c74 6572 5f6f 7074 696f 6e73 290a 2020  lter_options).  
+00000b50: 2020 2020 2020 7365 6c66 2e67 726f 7570        self.group
+00000b60: 426f 785f 7374 6174 696f 6e73 5f6d 6170  Box_stations_map
+00000b70: 5f76 6965 775f 6f70 7469 6f6e 7320 3d20  _view_options = 
+00000b80: 5174 5769 6467 6574 732e 5147 726f 7570  QtWidgets.QGroup
+00000b90: 426f 7828 7365 6c66 2e74 6162 5f6d 6169  Box(self.tab_mai
+00000ba0: 6e5f 7374 6174 696f 6e73 290a 2020 2020  n_stations).    
+00000bb0: 2020 2020 7365 6c66 2e67 726f 7570 426f      self.groupBo
+00000bc0: 785f 7374 6174 696f 6e73 5f6d 6170 5f76  x_stations_map_v
+00000bd0: 6965 775f 6f70 7469 6f6e 732e 7365 7445  iew_options.setE
+00000be0: 6e61 626c 6564 2846 616c 7365 290a 2020  nabled(False).  
+00000bf0: 2020 2020 2020 7365 6c66 2e67 726f 7570        self.group
+00000c00: 426f 785f 7374 6174 696f 6e73 5f6d 6170  Box_stations_map
+00000c10: 5f76 6965 775f 6f70 7469 6f6e 732e 7365  _view_options.se
+00000c20: 744f 626a 6563 744e 616d 6528 2267 726f  tObjectName("gro
+00000c30: 7570 426f 785f 7374 6174 696f 6e73 5f6d  upBox_stations_m
+00000c40: 6170 5f76 6965 775f 6f70 7469 6f6e 7322  ap_view_options"
+00000c50: 290a 2020 2020 2020 2020 7365 6c66 2e76  ).        self.v
+00000c60: 6572 7469 6361 6c4c 6179 6f75 745f 3331  erticalLayout_31
+00000c70: 203d 2051 7457 6964 6765 7473 2e51 5642   = QtWidgets.QVB
+00000c80: 6f78 4c61 796f 7574 2873 656c 662e 6772  oxLayout(self.gr
+00000c90: 6f75 7042 6f78 5f73 7461 7469 6f6e 735f  oupBox_stations_
+00000ca0: 6d61 705f 7669 6577 5f6f 7074 696f 6e73  map_view_options
+00000cb0: 290a 2020 2020 2020 2020 7365 6c66 2e76  ).        self.v
+00000cc0: 6572 7469 6361 6c4c 6179 6f75 745f 3331  erticalLayout_31
+00000cd0: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
+00000ce0: 7665 7274 6963 616c 4c61 796f 7574 5f33  verticalLayout_3
+00000cf0: 3122 290a 2020 2020 2020 2020 7365 6c66  1").        self
+00000d00: 2e63 6865 636b 426f 785f 7374 6174 696f  .checkBox_statio
+00000d10: 6e73 5f6d 6170 5f73 686f 775f 7374 6174  ns_map_show_stat
+00000d20: 5f6e 616d 655f 6c61 6265 6c73 203d 2051  _name_labels = Q
+00000d30: 7457 6964 6765 7473 2e51 4368 6563 6b42  tWidgets.QCheckB
+00000d40: 6f78 2873 656c 662e 6772 6f75 7042 6f78  ox(self.groupBox
+00000d50: 5f73 7461 7469 6f6e 735f 6d61 705f 7669  _stations_map_vi
+00000d60: 6577 5f6f 7074 696f 6e73 290a 2020 2020  ew_options).    
+00000d70: 2020 2020 7365 6c66 2e63 6865 636b 426f      self.checkBo
+00000d80: 785f 7374 6174 696f 6e73 5f6d 6170 5f73  x_stations_map_s
+00000d90: 686f 775f 7374 6174 5f6e 616d 655f 6c61  how_stat_name_la
+00000da0: 6265 6c73 2e73 6574 4368 6563 6b65 6428  bels.setChecked(
+00000db0: 5472 7565 290a 2020 2020 2020 2020 7365  True).        se
+00000dc0: 6c66 2e63 6865 636b 426f 785f 7374 6174  lf.checkBox_stat
+00000dd0: 696f 6e73 5f6d 6170 5f73 686f 775f 7374  ions_map_show_st
+00000de0: 6174 5f6e 616d 655f 6c61 6265 6c73 2e73  at_name_labels.s
+00000df0: 6574 4f62 6a65 6374 4e61 6d65 2822 6368  etObjectName("ch
+00000e00: 6563 6b42 6f78 5f73 7461 7469 6f6e 735f  eckBox_stations_
+00000e10: 6d61 705f 7368 6f77 5f73 7461 745f 6e61  map_show_stat_na
+00000e20: 6d65 5f6c 6162 656c 7322 290a 2020 2020  me_labels").    
+00000e30: 2020 2020 7365 6c66 2e76 6572 7469 6361      self.vertica
+00000e40: 6c4c 6179 6f75 745f 3331 2e61 6464 5769  lLayout_31.addWi
+00000e50: 6467 6574 2873 656c 662e 6368 6563 6b42  dget(self.checkB
+00000e60: 6f78 5f73 7461 7469 6f6e 735f 6d61 705f  ox_stations_map_
+00000e70: 7368 6f77 5f73 7461 745f 6e61 6d65 5f6c  show_stat_name_l
+00000e80: 6162 656c 7329 0a20 2020 2020 2020 2073  abels).        s
+00000e90: 656c 662e 6368 6563 6b42 6f78 5f73 7461  elf.checkBox_sta
+00000ea0: 7469 6f6e 735f 706c 6f74 5f6f 6273 5f6d  tions_plot_obs_m
+00000eb0: 6170 203d 2051 7457 6964 6765 7473 2e51  ap = QtWidgets.Q
+00000ec0: 4368 6563 6b42 6f78 2873 656c 662e 6772  CheckBox(self.gr
+00000ed0: 6f75 7042 6f78 5f73 7461 7469 6f6e 735f  oupBox_stations_
+00000ee0: 6d61 705f 7669 6577 5f6f 7074 696f 6e73  map_view_options
+00000ef0: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+00000f00: 6865 636b 426f 785f 7374 6174 696f 6e73  heckBox_stations
+00000f10: 5f70 6c6f 745f 6f62 735f 6d61 702e 7365  _plot_obs_map.se
+00000f20: 744f 626a 6563 744e 616d 6528 2263 6865  tObjectName("che
+00000f30: 636b 426f 785f 7374 6174 696f 6e73 5f70  ckBox_stations_p
+00000f40: 6c6f 745f 6f62 735f 6d61 7022 290a 2020  lot_obs_map").  
+00000f50: 2020 2020 2020 7365 6c66 2e76 6572 7469        self.verti
+00000f60: 6361 6c4c 6179 6f75 745f 3331 2e61 6464  calLayout_31.add
+00000f70: 5769 6467 6574 2873 656c 662e 6368 6563  Widget(self.chec
+00000f80: 6b42 6f78 5f73 7461 7469 6f6e 735f 706c  kBox_stations_pl
+00000f90: 6f74 5f6f 6273 5f6d 6170 290a 2020 2020  ot_obs_map).    
+00000fa0: 2020 2020 7365 6c66 2e63 6f6d 626f 426f      self.comboBo
+00000fb0: 785f 7374 6174 696f 6e73 5f70 6c6f 745f  x_stations_plot_
+00000fc0: 6f62 735f 6d61 705f 7375 7276 6579 7320  obs_map_surveys 
+00000fd0: 3d20 5174 5769 6467 6574 732e 5143 6f6d  = QtWidgets.QCom
+00000fe0: 626f 426f 7828 7365 6c66 2e67 726f 7570  boBox(self.group
+00000ff0: 426f 785f 7374 6174 696f 6e73 5f6d 6170  Box_stations_map
+00001000: 5f76 6965 775f 6f70 7469 6f6e 7329 0a20  _view_options). 
+00001010: 2020 2020 2020 2073 656c 662e 636f 6d62         self.comb
+00001020: 6f42 6f78 5f73 7461 7469 6f6e 735f 706c  oBox_stations_pl
+00001030: 6f74 5f6f 6273 5f6d 6170 5f73 7572 7665  ot_obs_map_surve
+00001040: 7973 2e73 6574 456e 6162 6c65 6428 4661  ys.setEnabled(Fa
+00001050: 6c73 6529 0a20 2020 2020 2020 2073 656c  lse).        sel
+00001060: 662e 636f 6d62 6f42 6f78 5f73 7461 7469  f.comboBox_stati
+00001070: 6f6e 735f 706c 6f74 5f6f 6273 5f6d 6170  ons_plot_obs_map
+00001080: 5f73 7572 7665 7973 2e73 6574 4f62 6a65  _surveys.setObje
+00001090: 6374 4e61 6d65 2822 636f 6d62 6f42 6f78  ctName("comboBox
+000010a0: 5f73 7461 7469 6f6e 735f 706c 6f74 5f6f  _stations_plot_o
+000010b0: 6273 5f6d 6170 5f73 7572 7665 7973 2229  bs_map_surveys")
+000010c0: 0a20 2020 2020 2020 2073 656c 662e 7665  .        self.ve
+000010d0: 7274 6963 616c 4c61 796f 7574 5f33 312e  rticalLayout_31.
+000010e0: 6164 6457 6964 6765 7428 7365 6c66 2e63  addWidget(self.c
+000010f0: 6f6d 626f 426f 785f 7374 6174 696f 6e73  omboBox_stations
+00001100: 5f70 6c6f 745f 6f62 735f 6d61 705f 7375  _plot_obs_map_su
+00001110: 7276 6579 7329 0a20 2020 2020 2020 2073  rveys).        s
+00001120: 656c 662e 7665 7274 6963 616c 4c61 796f  elf.verticalLayo
+00001130: 7574 5f33 2e61 6464 5769 6467 6574 2873  ut_3.addWidget(s
+00001140: 656c 662e 6772 6f75 7042 6f78 5f73 7461  elf.groupBox_sta
+00001150: 7469 6f6e 735f 6d61 705f 7669 6577 5f6f  tions_map_view_o
+00001160: 7074 696f 6e73 290a 2020 2020 2020 2020  ptions).        
+00001170: 7370 6163 6572 4974 656d 203d 2051 7457  spacerItem = QtW
+00001180: 6964 6765 7473 2e51 5370 6163 6572 4974  idgets.QSpacerIt
+00001190: 656d 2832 302c 2034 302c 2051 7457 6964  em(20, 40, QtWid
+000011a0: 6765 7473 2e51 5369 7a65 506f 6c69 6379  gets.QSizePolicy
+000011b0: 2e4d 696e 696d 756d 2c20 5174 5769 6467  .Minimum, QtWidg
+000011c0: 6574 732e 5153 697a 6550 6f6c 6963 792e  ets.QSizePolicy.
+000011d0: 4578 7061 6e64 696e 6729 0a20 2020 2020  Expanding).     
+000011e0: 2020 2073 656c 662e 7665 7274 6963 616c     self.vertical
+000011f0: 4c61 796f 7574 5f33 2e61 6464 4974 656d  Layout_3.addItem
+00001200: 2873 7061 6365 7249 7465 6d29 0a20 2020  (spacerItem).   
+00001210: 2020 2020 2073 656c 662e 686f 7269 7a6f       self.horizo
+00001220: 6e74 616c 4c61 796f 7574 5f32 2e61 6464  ntalLayout_2.add
+00001230: 4c61 796f 7574 2873 656c 662e 7665 7274  Layout(self.vert
+00001240: 6963 616c 4c61 796f 7574 5f33 290a 2020  icalLayout_3).  
+00001250: 2020 2020 2020 7365 6c66 2e74 6162 5f57        self.tab_W
+00001260: 6964 6765 745f 5374 6174 696f 6e73 203d  idget_Stations =
+00001270: 2051 7457 6964 6765 7473 2e51 5461 6257   QtWidgets.QTabW
+00001280: 6964 6765 7428 7365 6c66 2e74 6162 5f6d  idget(self.tab_m
+00001290: 6169 6e5f 7374 6174 696f 6e73 290a 2020  ain_stations).  
+000012a0: 2020 2020 2020 7369 7a65 506f 6c69 6379        sizePolicy
+000012b0: 203d 2051 7457 6964 6765 7473 2e51 5369   = QtWidgets.QSi
+000012c0: 7a65 506f 6c69 6379 2851 7457 6964 6765  zePolicy(QtWidge
+000012d0: 7473 2e51 5369 7a65 506f 6c69 6379 2e45  ts.QSizePolicy.E
+000012e0: 7870 616e 6469 6e67 2c20 5174 5769 6467  xpanding, QtWidg
+000012f0: 6574 732e 5153 697a 6550 6f6c 6963 792e  ets.QSizePolicy.
+00001300: 4578 7061 6e64 696e 6729 0a20 2020 2020  Expanding).     
+00001310: 2020 2073 697a 6550 6f6c 6963 792e 7365     sizePolicy.se
+00001320: 7448 6f72 697a 6f6e 7461 6c53 7472 6574  tHorizontalStret
+00001330: 6368 2830 290a 2020 2020 2020 2020 7369  ch(0).        si
+00001340: 7a65 506f 6c69 6379 2e73 6574 5665 7274  zePolicy.setVert
+00001350: 6963 616c 5374 7265 7463 6828 3029 0a20  icalStretch(0). 
+00001360: 2020 2020 2020 2073 697a 6550 6f6c 6963         sizePolic
+00001370: 792e 7365 7448 6569 6768 7446 6f72 5769  y.setHeightForWi
+00001380: 6474 6828 7365 6c66 2e74 6162 5f57 6964  dth(self.tab_Wid
+00001390: 6765 745f 5374 6174 696f 6e73 2e73 697a  get_Stations.siz
+000013a0: 6550 6f6c 6963 7928 292e 6861 7348 6569  ePolicy().hasHei
+000013b0: 6768 7446 6f72 5769 6474 6828 2929 0a20  ghtForWidth()). 
+000013c0: 2020 2020 2020 2073 656c 662e 7461 625f         self.tab_
+000013d0: 5769 6467 6574 5f53 7461 7469 6f6e 732e  Widget_Stations.
+000013e0: 7365 7453 697a 6550 6f6c 6963 7928 7369  setSizePolicy(si
+000013f0: 7a65 506f 6c69 6379 290a 2020 2020 2020  zePolicy).      
+00001400: 2020 7365 6c66 2e74 6162 5f57 6964 6765    self.tab_Widge
+00001410: 745f 5374 6174 696f 6e73 2e73 6574 4f62  t_Stations.setOb
+00001420: 6a65 6374 4e61 6d65 2822 7461 625f 5769  jectName("tab_Wi
+00001430: 6467 6574 5f53 7461 7469 6f6e 7322 290a  dget_Stations").
+00001440: 2020 2020 2020 2020 7365 6c66 2e74 6162          self.tab
+00001450: 5f53 7461 7469 6f6e 735f 5461 626c 6520  _Stations_Table 
+00001460: 3d20 5174 5769 6467 6574 732e 5157 6964  = QtWidgets.QWid
+00001470: 6765 7428 290a 2020 2020 2020 2020 7365  get().        se
+00001480: 6c66 2e74 6162 5f53 7461 7469 6f6e 735f  lf.tab_Stations_
+00001490: 5461 626c 652e 7365 744f 626a 6563 744e  Table.setObjectN
+000014a0: 616d 6528 2274 6162 5f53 7461 7469 6f6e  ame("tab_Station
+000014b0: 735f 5461 626c 6522 290a 2020 2020 2020  s_Table").      
+000014c0: 2020 7365 6c66 2e76 6572 7469 6361 6c4c    self.verticalL
+000014d0: 6179 6f75 7420 3d20 5174 5769 6467 6574  ayout = QtWidget
+000014e0: 732e 5156 426f 784c 6179 6f75 7428 7365  s.QVBoxLayout(se
+000014f0: 6c66 2e74 6162 5f53 7461 7469 6f6e 735f  lf.tab_Stations_
+00001500: 5461 626c 6529 0a20 2020 2020 2020 2073  Table).        s
+00001510: 656c 662e 7665 7274 6963 616c 4c61 796f  elf.verticalLayo
+00001520: 7574 2e73 6574 4f62 6a65 6374 4e61 6d65  ut.setObjectName
+00001530: 2822 7665 7274 6963 616c 4c61 796f 7574  ("verticalLayout
+00001540: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00001550: 7461 626c 6556 6965 775f 5374 6174 696f  tableView_Statio
+00001560: 6e73 203d 2051 7457 6964 6765 7473 2e51  ns = QtWidgets.Q
+00001570: 5461 626c 6556 6965 7728 7365 6c66 2e74  TableView(self.t
+00001580: 6162 5f53 7461 7469 6f6e 735f 5461 626c  ab_Stations_Tabl
+00001590: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
+000015a0: 7461 626c 6556 6965 775f 5374 6174 696f  tableView_Statio
+000015b0: 6e73 2e73 6574 5369 7a65 4164 6a75 7374  ns.setSizeAdjust
+000015c0: 506f 6c69 6379 2851 7457 6964 6765 7473  Policy(QtWidgets
+000015d0: 2e51 4162 7374 7261 6374 5363 726f 6c6c  .QAbstractScroll
+000015e0: 4172 6561 2e41 646a 7573 7454 6f43 6f6e  Area.AdjustToCon
+000015f0: 7465 6e74 7329 0a20 2020 2020 2020 2073  tents).        s
+00001600: 656c 662e 7461 626c 6556 6965 775f 5374  elf.tableView_St
+00001610: 6174 696f 6e73 2e73 6574 4f62 6a65 6374  ations.setObject
+00001620: 4e61 6d65 2822 7461 626c 6556 6965 775f  Name("tableView_
+00001630: 5374 6174 696f 6e73 2229 0a20 2020 2020  Stations").     
+00001640: 2020 2073 656c 662e 7461 626c 6556 6965     self.tableVie
+00001650: 775f 5374 6174 696f 6e73 2e68 6f72 697a  w_Stations.horiz
+00001660: 6f6e 7461 6c48 6561 6465 7228 292e 7365  ontalHeader().se
+00001670: 7443 6173 6361 6469 6e67 5365 6374 696f  tCascadingSectio
+00001680: 6e52 6573 697a 6573 2854 7275 6529 0a20  nResizes(True). 
+00001690: 2020 2020 2020 2073 656c 662e 7665 7274         self.vert
+000016a0: 6963 616c 4c61 796f 7574 2e61 6464 5769  icalLayout.addWi
+000016b0: 6467 6574 2873 656c 662e 7461 626c 6556  dget(self.tableV
+000016c0: 6965 775f 5374 6174 696f 6e73 290a 2020  iew_Stations).  
+000016d0: 2020 2020 2020 7365 6c66 2e74 6162 5f57        self.tab_W
+000016e0: 6964 6765 745f 5374 6174 696f 6e73 2e61  idget_Stations.a
+000016f0: 6464 5461 6228 7365 6c66 2e74 6162 5f53  ddTab(self.tab_S
+00001700: 7461 7469 6f6e 735f 5461 626c 652c 2022  tations_Table, "
+00001710: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00001720: 7461 625f 7374 6174 696f 6e73 5f6d 6170  tab_stations_map
+00001730: 203d 2051 7457 6964 6765 7473 2e51 5769   = QtWidgets.QWi
+00001740: 6467 6574 2829 0a20 2020 2020 2020 2073  dget().        s
+00001750: 656c 662e 7461 625f 7374 6174 696f 6e73  elf.tab_stations
+00001760: 5f6d 6170 2e73 6574 4f62 6a65 6374 4e61  _map.setObjectNa
+00001770: 6d65 2822 7461 625f 7374 6174 696f 6e73  me("tab_stations
+00001780: 5f6d 6170 2229 0a20 2020 2020 2020 2073  _map").        s
+00001790: 656c 662e 7665 7274 6963 616c 4c61 796f  elf.verticalLayo
+000017a0: 7574 5f33 3020 3d20 5174 5769 6467 6574  ut_30 = QtWidget
+000017b0: 732e 5156 426f 784c 6179 6f75 7428 7365  s.QVBoxLayout(se
+000017c0: 6c66 2e74 6162 5f73 7461 7469 6f6e 735f  lf.tab_stations_
+000017d0: 6d61 7029 0a20 2020 2020 2020 2073 656c  map).        sel
+000017e0: 662e 7665 7274 6963 616c 4c61 796f 7574  f.verticalLayout
+000017f0: 5f33 302e 7365 744f 626a 6563 744e 616d  _30.setObjectNam
+00001800: 6528 2276 6572 7469 6361 6c4c 6179 6f75  e("verticalLayou
+00001810: 745f 3330 2229 0a20 2020 2020 2020 2073  t_30").        s
+00001820: 656c 662e 4772 6170 6869 6373 4c61 796f  elf.GraphicsLayo
+00001830: 7574 5769 6467 6574 5f73 7461 7469 6f6e  utWidget_station
+00001840: 735f 6d61 7020 3d20 4772 6170 6869 6373  s_map = Graphics
+00001850: 4c61 796f 7574 5769 6467 6574 2873 656c  LayoutWidget(sel
+00001860: 662e 7461 625f 7374 6174 696f 6e73 5f6d  f.tab_stations_m
+00001870: 6170 290a 2020 2020 2020 2020 7365 6c66  ap).        self
+00001880: 2e47 7261 7068 6963 734c 6179 6f75 7457  .GraphicsLayoutW
+00001890: 6964 6765 745f 7374 6174 696f 6e73 5f6d  idget_stations_m
+000018a0: 6170 2e73 6574 4f62 6a65 6374 4e61 6d65  ap.setObjectName
+000018b0: 2822 4772 6170 6869 6373 4c61 796f 7574  ("GraphicsLayout
+000018c0: 5769 6467 6574 5f73 7461 7469 6f6e 735f  Widget_stations_
+000018d0: 6d61 7022 290a 2020 2020 2020 2020 7365  map").        se
+000018e0: 6c66 2e76 6572 7469 6361 6c4c 6179 6f75  lf.verticalLayou
+000018f0: 745f 3330 2e61 6464 5769 6467 6574 2873  t_30.addWidget(s
+00001900: 656c 662e 4772 6170 6869 6373 4c61 796f  elf.GraphicsLayo
+00001910: 7574 5769 6467 6574 5f73 7461 7469 6f6e  utWidget_station
+00001920: 735f 6d61 7029 0a20 2020 2020 2020 2073  s_map).        s
+00001930: 656c 662e 7461 625f 5769 6467 6574 5f53  elf.tab_Widget_S
+00001940: 7461 7469 6f6e 732e 6164 6454 6162 2873  tations.addTab(s
+00001950: 656c 662e 7461 625f 7374 6174 696f 6e73  elf.tab_stations
+00001960: 5f6d 6170 2c20 2222 290a 2020 2020 2020  _map, "").      
+00001970: 2020 7365 6c66 2e68 6f72 697a 6f6e 7461    self.horizonta
+00001980: 6c4c 6179 6f75 745f 322e 6164 6457 6964  lLayout_2.addWid
+00001990: 6765 7428 7365 6c66 2e74 6162 5f57 6964  get(self.tab_Wid
+000019a0: 6765 745f 5374 6174 696f 6e73 290a 2020  get_Stations).  
+000019b0: 2020 2020 2020 7365 6c66 2e68 6f72 697a        self.horiz
+000019c0: 6f6e 7461 6c4c 6179 6f75 745f 322e 7365  ontalLayout_2.se
+000019d0: 7453 7472 6574 6368 2830 2c20 3129 0a20  tStretch(0, 1). 
+000019e0: 2020 2020 2020 2073 656c 662e 686f 7269         self.hori
+000019f0: 7a6f 6e74 616c 4c61 796f 7574 5f32 2e73  zontalLayout_2.s
+00001a00: 6574 5374 7265 7463 6828 312c 2034 290a  etStretch(1, 4).
+00001a10: 2020 2020 2020 2020 7365 6c66 2e76 6572          self.ver
+00001a20: 7469 6361 6c4c 6179 6f75 745f 342e 6164  ticalLayout_4.ad
+00001a30: 644c 6179 6f75 7428 7365 6c66 2e68 6f72  dLayout(self.hor
+00001a40: 697a 6f6e 7461 6c4c 6179 6f75 745f 3229  izontalLayout_2)
+00001a50: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
+00001a60: 6257 6964 6765 745f 4d61 696e 2e61 6464  bWidget_Main.add
+00001a70: 5461 6228 7365 6c66 2e74 6162 5f6d 6169  Tab(self.tab_mai
+00001a80: 6e5f 7374 6174 696f 6e73 2c20 2222 290a  n_stations, "").
+00001a90: 2020 2020 2020 2020 7365 6c66 2e74 6162          self.tab
+00001aa0: 5f6d 6169 6e5f 6772 6176 696d 6574 6572  _main_gravimeter
+00001ab0: 7320 3d20 5174 5769 6467 6574 732e 5157  s = QtWidgets.QW
+00001ac0: 6964 6765 7428 290a 2020 2020 2020 2020  idget().        
+00001ad0: 7365 6c66 2e74 6162 5f6d 6169 6e5f 6772  self.tab_main_gr
+00001ae0: 6176 696d 6574 6572 732e 7365 744f 626a  avimeters.setObj
+00001af0: 6563 744e 616d 6528 2274 6162 5f6d 6169  ectName("tab_mai
+00001b00: 6e5f 6772 6176 696d 6574 6572 7322 290a  n_gravimeters").
+00001b10: 2020 2020 2020 2020 7365 6c66 2e76 6572          self.ver
+00001b20: 7469 6361 6c4c 6179 6f75 745f 3238 203d  ticalLayout_28 =
+00001b30: 2051 7457 6964 6765 7473 2e51 5642 6f78   QtWidgets.QVBox
+00001b40: 4c61 796f 7574 2873 656c 662e 7461 625f  Layout(self.tab_
+00001b50: 6d61 696e 5f67 7261 7669 6d65 7465 7273  main_gravimeters
+00001b60: 290a 2020 2020 2020 2020 7365 6c66 2e76  ).        self.v
+00001b70: 6572 7469 6361 6c4c 6179 6f75 745f 3238  erticalLayout_28
+00001b80: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
+00001b90: 7665 7274 6963 616c 4c61 796f 7574 5f32  verticalLayout_2
+00001ba0: 3822 290a 2020 2020 2020 2020 7365 6c66  8").        self
+00001bb0: 2e73 706c 6974 7465 725f 6772 6176 696d  .splitter_gravim
+00001bc0: 6574 6572 7320 3d20 5174 5769 6467 6574  eters = QtWidget
+00001bd0: 732e 5153 706c 6974 7465 7228 7365 6c66  s.QSplitter(self
+00001be0: 2e74 6162 5f6d 6169 6e5f 6772 6176 696d  .tab_main_gravim
+00001bf0: 6574 6572 7329 0a20 2020 2020 2020 2073  eters).        s
+00001c00: 656c 662e 7370 6c69 7474 6572 5f67 7261  elf.splitter_gra
+00001c10: 7669 6d65 7465 7273 2e73 6574 4f72 6965  vimeters.setOrie
+00001c20: 6e74 6174 696f 6e28 5174 436f 7265 2e51  ntation(QtCore.Q
+00001c30: 742e 486f 7269 7a6f 6e74 616c 290a 2020  t.Horizontal).  
+00001c40: 2020 2020 2020 7365 6c66 2e73 706c 6974        self.split
+00001c50: 7465 725f 6772 6176 696d 6574 6572 732e  ter_gravimeters.
+00001c60: 7365 744f 626a 6563 744e 616d 6528 2273  setObjectName("s
+00001c70: 706c 6974 7465 725f 6772 6176 696d 6574  plitter_gravimet
+00001c80: 6572 7322 290a 2020 2020 2020 2020 7365  ers").        se
+00001c90: 6c66 2e6c 6179 6f75 7457 6964 6765 7420  lf.layoutWidget 
+00001ca0: 3d20 5174 5769 6467 6574 732e 5157 6964  = QtWidgets.QWid
+00001cb0: 6765 7428 7365 6c66 2e73 706c 6974 7465  get(self.splitte
+00001cc0: 725f 6772 6176 696d 6574 6572 7329 0a20  r_gravimeters). 
+00001cd0: 2020 2020 2020 2073 656c 662e 6c61 796f         self.layo
+00001ce0: 7574 5769 6467 6574 2e73 6574 4f62 6a65  utWidget.setObje
+00001cf0: 6374 4e61 6d65 2822 6c61 796f 7574 5769  ctName("layoutWi
+00001d00: 6467 6574 2229 0a20 2020 2020 2020 2073  dget").        s
+00001d10: 656c 662e 7665 7274 6963 616c 4c61 796f  elf.verticalLayo
+00001d20: 7574 5f34 3020 3d20 5174 5769 6467 6574  ut_40 = QtWidget
+00001d30: 732e 5156 426f 784c 6179 6f75 7428 7365  s.QVBoxLayout(se
+00001d40: 6c66 2e6c 6179 6f75 7457 6964 6765 7429  lf.layoutWidget)
+00001d50: 0a20 2020 2020 2020 2073 656c 662e 7665  .        self.ve
+00001d60: 7274 6963 616c 4c61 796f 7574 5f34 302e  rticalLayout_40.
+00001d70: 7365 7443 6f6e 7465 6e74 734d 6172 6769  setContentsMargi
+00001d80: 6e73 2830 2c20 302c 2030 2c20 3029 0a20  ns(0, 0, 0, 0). 
+00001d90: 2020 2020 2020 2073 656c 662e 7665 7274         self.vert
+00001da0: 6963 616c 4c61 796f 7574 5f34 302e 7365  icalLayout_40.se
+00001db0: 744f 626a 6563 744e 616d 6528 2276 6572  tObjectName("ver
+00001dc0: 7469 6361 6c4c 6179 6f75 745f 3430 2229  ticalLayout_40")
+00001dd0: 0a20 2020 2020 2020 2073 656c 662e 7472  .        self.tr
+00001de0: 6565 5769 6467 6574 5f67 7261 7669 6d65  eeWidget_gravime
+00001df0: 7465 7273 203d 2051 7457 6964 6765 7473  ters = QtWidgets
+00001e00: 2e51 5472 6565 5769 6467 6574 2873 656c  .QTreeWidget(sel
+00001e10: 662e 6c61 796f 7574 5769 6467 6574 290a  f.layoutWidget).
+00001e20: 2020 2020 2020 2020 7365 6c66 2e74 7265          self.tre
+00001e30: 6557 6964 6765 745f 6772 6176 696d 6574  eWidget_gravimet
+00001e40: 6572 732e 7365 7448 6561 6465 7248 6964  ers.setHeaderHid
+00001e50: 6465 6e28 4661 6c73 6529 0a20 2020 2020  den(False).     
+00001e60: 2020 2073 656c 662e 7472 6565 5769 6467     self.treeWidg
+00001e70: 6574 5f67 7261 7669 6d65 7465 7273 2e73  et_gravimeters.s
+00001e80: 6574 436f 6c75 6d6e 436f 756e 7428 3229  etColumnCount(2)
+00001e90: 0a20 2020 2020 2020 2073 656c 662e 7472  .        self.tr
+00001ea0: 6565 5769 6467 6574 5f67 7261 7669 6d65  eeWidget_gravime
+00001eb0: 7465 7273 2e73 6574 4f62 6a65 6374 4e61  ters.setObjectNa
+00001ec0: 6d65 2822 7472 6565 5769 6467 6574 5f67  me("treeWidget_g
+00001ed0: 7261 7669 6d65 7465 7273 2229 0a20 2020  ravimeters").   
+00001ee0: 2020 2020 2073 656c 662e 7665 7274 6963       self.vertic
+00001ef0: 616c 4c61 796f 7574 5f34 302e 6164 6457  alLayout_40.addW
+00001f00: 6964 6765 7428 7365 6c66 2e74 7265 6557  idget(self.treeW
+00001f10: 6964 6765 745f 6772 6176 696d 6574 6572  idget_gravimeter
+00001f20: 7329 0a20 2020 2020 2020 2073 656c 662e  s).        self.
+00001f30: 7075 7368 4275 7474 6f6e 5f64 656c 6574  pushButton_delet
+00001f40: 655f 6772 6176 696d 6574 6572 203d 2051  e_gravimeter = Q
+00001f50: 7457 6964 6765 7473 2e51 5075 7368 4275  tWidgets.QPushBu
+00001f60: 7474 6f6e 2873 656c 662e 6c61 796f 7574  tton(self.layout
+00001f70: 5769 6467 6574 290a 2020 2020 2020 2020  Widget).        
+00001f80: 7365 6c66 2e70 7573 6842 7574 746f 6e5f  self.pushButton_
+00001f90: 6465 6c65 7465 5f67 7261 7669 6d65 7465  delete_gravimete
+00001fa0: 722e 7365 7445 6e61 626c 6564 2846 616c  r.setEnabled(Fal
+00001fb0: 7365 290a 2020 2020 2020 2020 7365 6c66  se).        self
+00001fc0: 2e70 7573 6842 7574 746f 6e5f 6465 6c65  .pushButton_dele
+00001fd0: 7465 5f67 7261 7669 6d65 7465 722e 7365  te_gravimeter.se
+00001fe0: 744f 626a 6563 744e 616d 6528 2270 7573  tObjectName("pus
+00001ff0: 6842 7574 746f 6e5f 6465 6c65 7465 5f67  hButton_delete_g
+00002000: 7261 7669 6d65 7465 7222 290a 2020 2020  ravimeter").    
+00002010: 2020 2020 7365 6c66 2e76 6572 7469 6361      self.vertica
+00002020: 6c4c 6179 6f75 745f 3430 2e61 6464 5769  lLayout_40.addWi
+00002030: 6467 6574 2873 656c 662e 7075 7368 4275  dget(self.pushBu
+00002040: 7474 6f6e 5f64 656c 6574 655f 6772 6176  tton_delete_grav
+00002050: 696d 6574 6572 290a 2020 2020 2020 2020  imeter).        
+00002060: 7365 6c66 2e74 6162 5769 6467 6574 5f67  self.tabWidget_g
+00002070: 7261 7669 6d65 7465 7273 203d 2051 7457  ravimeters = QtW
+00002080: 6964 6765 7473 2e51 5461 6257 6964 6765  idgets.QTabWidge
+00002090: 7428 7365 6c66 2e73 706c 6974 7465 725f  t(self.splitter_
+000020a0: 6772 6176 696d 6574 6572 7329 0a20 2020  gravimeters).   
+000020b0: 2020 2020 2073 697a 6550 6f6c 6963 7920       sizePolicy 
+000020c0: 3d20 5174 5769 6467 6574 732e 5153 697a  = QtWidgets.QSiz
+000020d0: 6550 6f6c 6963 7928 5174 5769 6467 6574  ePolicy(QtWidget
+000020e0: 732e 5153 697a 6550 6f6c 6963 792e 4578  s.QSizePolicy.Ex
+000020f0: 7061 6e64 696e 672c 2051 7457 6964 6765  panding, QtWidge
+00002100: 7473 2e51 5369 7a65 506f 6c69 6379 2e45  ts.QSizePolicy.E
+00002110: 7870 616e 6469 6e67 290a 2020 2020 2020  xpanding).      
+00002120: 2020 7369 7a65 506f 6c69 6379 2e73 6574    sizePolicy.set
+00002130: 486f 7269 7a6f 6e74 616c 5374 7265 7463  HorizontalStretc
+00002140: 6828 3129 0a20 2020 2020 2020 2073 697a  h(1).        siz
+00002150: 6550 6f6c 6963 792e 7365 7456 6572 7469  ePolicy.setVerti
+00002160: 6361 6c53 7472 6574 6368 2830 290a 2020  calStretch(0).  
+00002170: 2020 2020 2020 7369 7a65 506f 6c69 6379        sizePolicy
+00002180: 2e73 6574 4865 6967 6874 466f 7257 6964  .setHeightForWid
+00002190: 7468 2873 656c 662e 7461 6257 6964 6765  th(self.tabWidge
+000021a0: 745f 6772 6176 696d 6574 6572 732e 7369  t_gravimeters.si
+000021b0: 7a65 506f 6c69 6379 2829 2e68 6173 4865  zePolicy().hasHe
+000021c0: 6967 6874 466f 7257 6964 7468 2829 290a  ightForWidth()).
+000021d0: 2020 2020 2020 2020 7365 6c66 2e74 6162          self.tab
+000021e0: 5769 6467 6574 5f67 7261 7669 6d65 7465  Widget_gravimete
+000021f0: 7273 2e73 6574 5369 7a65 506f 6c69 6379  rs.setSizePolicy
+00002200: 2873 697a 6550 6f6c 6963 7929 0a20 2020  (sizePolicy).   
+00002210: 2020 2020 2073 656c 662e 7461 6257 6964       self.tabWid
+00002220: 6765 745f 6772 6176 696d 6574 6572 732e  get_gravimeters.
+00002230: 7365 744f 626a 6563 744e 616d 6528 2274  setObjectName("t
+00002240: 6162 5769 6467 6574 5f67 7261 7669 6d65  abWidget_gravime
+00002250: 7465 7273 2229 0a20 2020 2020 2020 2073  ters").        s
+00002260: 656c 662e 7461 625f 6772 6176 696d 6574  elf.tab_gravimet
+00002270: 6572 5f69 6e66 6f20 3d20 5174 5769 6467  er_info = QtWidg
+00002280: 6574 732e 5157 6964 6765 7428 290a 2020  ets.QWidget().  
+00002290: 2020 2020 2020 7365 6c66 2e74 6162 5f67        self.tab_g
+000022a0: 7261 7669 6d65 7465 725f 696e 666f 2e73  ravimeter_info.s
+000022b0: 6574 4f62 6a65 6374 4e61 6d65 2822 7461  etObjectName("ta
+000022c0: 625f 6772 6176 696d 6574 6572 5f69 6e66  b_gravimeter_inf
+000022d0: 6f22 290a 2020 2020 2020 2020 7365 6c66  o").        self
+000022e0: 2e76 6572 7469 6361 6c4c 6179 6f75 745f  .verticalLayout_
+000022f0: 3432 203d 2051 7457 6964 6765 7473 2e51  42 = QtWidgets.Q
+00002300: 5642 6f78 4c61 796f 7574 2873 656c 662e  VBoxLayout(self.
+00002310: 7461 625f 6772 6176 696d 6574 6572 5f69  tab_gravimeter_i
+00002320: 6e66 6f29 0a20 2020 2020 2020 2073 656c  nfo).        sel
+00002330: 662e 7665 7274 6963 616c 4c61 796f 7574  f.verticalLayout
+00002340: 5f34 322e 7365 744f 626a 6563 744e 616d  _42.setObjectNam
+00002350: 6528 2276 6572 7469 6361 6c4c 6179 6f75  e("verticalLayou
+00002360: 745f 3432 2229 0a20 2020 2020 2020 2073  t_42").        s
+00002370: 656c 662e 666f 726d 4c61 796f 7574 5f31  elf.formLayout_1
+00002380: 3220 3d20 5174 5769 6467 6574 732e 5146  2 = QtWidgets.QF
+00002390: 6f72 6d4c 6179 6f75 7428 290a 2020 2020  ormLayout().    
+000023a0: 2020 2020 7365 6c66 2e66 6f72 6d4c 6179      self.formLay
+000023b0: 6f75 745f 3132 2e73 6574 4f62 6a65 6374  out_12.setObject
+000023c0: 4e61 6d65 2822 666f 726d 4c61 796f 7574  Name("formLayout
+000023d0: 5f31 3222 290a 2020 2020 2020 2020 7365  _12").        se
+000023e0: 6c66 2e6c 6162 656c 5f31 3920 3d20 5174  lf.label_19 = Qt
+000023f0: 5769 6467 6574 732e 514c 6162 656c 2873  Widgets.QLabel(s
+00002400: 656c 662e 7461 625f 6772 6176 696d 6574  elf.tab_gravimet
+00002410: 6572 5f69 6e66 6f29 0a20 2020 2020 2020  er_info).       
+00002420: 2073 656c 662e 6c61 6265 6c5f 3139 2e73   self.label_19.s
+00002430: 6574 4f62 6a65 6374 4e61 6d65 2822 6c61  etObjectName("la
+00002440: 6265 6c5f 3139 2229 0a20 2020 2020 2020  bel_19").       
+00002450: 2073 656c 662e 666f 726d 4c61 796f 7574   self.formLayout
+00002460: 5f31 322e 7365 7457 6964 6765 7428 302c  _12.setWidget(0,
+00002470: 2051 7457 6964 6765 7473 2e51 466f 726d   QtWidgets.QForm
+00002480: 4c61 796f 7574 2e4c 6162 656c 526f 6c65  Layout.LabelRole
+00002490: 2c20 7365 6c66 2e6c 6162 656c 5f31 3929  , self.label_19)
+000024a0: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
+000024b0: 6265 6c5f 6772 6176 695f 6d61 6e75 6661  bel_gravi_manufa
+000024c0: 6374 7572 6572 203d 2051 7457 6964 6765  cturer = QtWidge
+000024d0: 7473 2e51 4c61 6265 6c28 7365 6c66 2e74  ts.QLabel(self.t
+000024e0: 6162 5f67 7261 7669 6d65 7465 725f 696e  ab_gravimeter_in
+000024f0: 666f 290a 2020 2020 2020 2020 7365 6c66  fo).        self
+00002500: 2e6c 6162 656c 5f67 7261 7669 5f6d 616e  .label_gravi_man
+00002510: 7566 6163 7475 7265 722e 7365 7454 6578  ufacturer.setTex
+00002520: 7428 2222 290a 2020 2020 2020 2020 7365  t("").        se
+00002530: 6c66 2e6c 6162 656c 5f67 7261 7669 5f6d  lf.label_gravi_m
+00002540: 616e 7566 6163 7475 7265 722e 7365 744f  anufacturer.setO
+00002550: 626a 6563 744e 616d 6528 226c 6162 656c  bjectName("label
+00002560: 5f67 7261 7669 5f6d 616e 7566 6163 7475  _gravi_manufactu
+00002570: 7265 7222 290a 2020 2020 2020 2020 7365  rer").        se
+00002580: 6c66 2e66 6f72 6d4c 6179 6f75 745f 3132  lf.formLayout_12
+00002590: 2e73 6574 5769 6467 6574 2830 2c20 5174  .setWidget(0, Qt
+000025a0: 5769 6467 6574 732e 5146 6f72 6d4c 6179  Widgets.QFormLay
+000025b0: 6f75 742e 4669 656c 6452 6f6c 652c 2073  out.FieldRole, s
+000025c0: 656c 662e 6c61 6265 6c5f 6772 6176 695f  elf.label_gravi_
+000025d0: 6d61 6e75 6661 6374 7572 6572 290a 2020  manufacturer).  
+000025e0: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
+000025f0: 5f32 3020 3d20 5174 5769 6467 6574 732e  _20 = QtWidgets.
+00002600: 514c 6162 656c 2873 656c 662e 7461 625f  QLabel(self.tab_
+00002610: 6772 6176 696d 6574 6572 5f69 6e66 6f29  gravimeter_info)
+00002620: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
+00002630: 6265 6c5f 3230 2e73 6574 4f62 6a65 6374  bel_20.setObject
+00002640: 4e61 6d65 2822 6c61 6265 6c5f 3230 2229  Name("label_20")
+00002650: 0a20 2020 2020 2020 2073 656c 662e 666f  .        self.fo
+00002660: 726d 4c61 796f 7574 5f31 322e 7365 7457  rmLayout_12.setW
+00002670: 6964 6765 7428 312c 2051 7457 6964 6765  idget(1, QtWidge
+00002680: 7473 2e51 466f 726d 4c61 796f 7574 2e4c  ts.QFormLayout.L
+00002690: 6162 656c 526f 6c65 2c20 7365 6c66 2e6c  abelRole, self.l
+000026a0: 6162 656c 5f32 3029 0a20 2020 2020 2020  abel_20).       
+000026b0: 2073 656c 662e 6c61 6265 6c5f 6772 6176   self.label_grav
+000026c0: 695f 7479 7065 203d 2051 7457 6964 6765  i_type = QtWidge
+000026d0: 7473 2e51 4c61 6265 6c28 7365 6c66 2e74  ts.QLabel(self.t
+000026e0: 6162 5f67 7261 7669 6d65 7465 725f 696e  ab_gravimeter_in
+000026f0: 666f 290a 2020 2020 2020 2020 7365 6c66  fo).        self
+00002700: 2e6c 6162 656c 5f67 7261 7669 5f74 7970  .label_gravi_typ
+00002710: 652e 7365 7454 6578 7428 2222 290a 2020  e.setText("").  
+00002720: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
+00002730: 5f67 7261 7669 5f74 7970 652e 7365 744f  _gravi_type.setO
+00002740: 626a 6563 744e 616d 6528 226c 6162 656c  bjectName("label
+00002750: 5f67 7261 7669 5f74 7970 6522 290a 2020  _gravi_type").  
+00002760: 2020 2020 2020 7365 6c66 2e66 6f72 6d4c        self.formL
+00002770: 6179 6f75 745f 3132 2e73 6574 5769 6467  ayout_12.setWidg
+00002780: 6574 2831 2c20 5174 5769 6467 6574 732e  et(1, QtWidgets.
+00002790: 5146 6f72 6d4c 6179 6f75 742e 4669 656c  QFormLayout.Fiel
+000027a0: 6452 6f6c 652c 2073 656c 662e 6c61 6265  dRole, self.labe
+000027b0: 6c5f 6772 6176 695f 7479 7065 290a 2020  l_gravi_type).  
+000027c0: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
+000027d0: 5f32 3120 3d20 5174 5769 6467 6574 732e  _21 = QtWidgets.
+000027e0: 514c 6162 656c 2873 656c 662e 7461 625f  QLabel(self.tab_
+000027f0: 6772 6176 696d 6574 6572 5f69 6e66 6f29  gravimeter_info)
+00002800: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
+00002810: 6265 6c5f 3231 2e73 6574 4f62 6a65 6374  bel_21.setObject
+00002820: 4e61 6d65 2822 6c61 6265 6c5f 3231 2229  Name("label_21")
+00002830: 0a20 2020 2020 2020 2073 656c 662e 666f  .        self.fo
+00002840: 726d 4c61 796f 7574 5f31 322e 7365 7457  rmLayout_12.setW
+00002850: 6964 6765 7428 322c 2051 7457 6964 6765  idget(2, QtWidge
+00002860: 7473 2e51 466f 726d 4c61 796f 7574 2e4c  ts.QFormLayout.L
+00002870: 6162 656c 526f 6c65 2c20 7365 6c66 2e6c  abelRole, self.l
+00002880: 6162 656c 5f32 3129 0a20 2020 2020 2020  abel_21).       
+00002890: 2073 656c 662e 6c61 6265 6c5f 6772 6176   self.label_grav
+000028a0: 695f 7365 7269 616c 5f6e 756d 6265 7220  i_serial_number 
+000028b0: 3d20 5174 5769 6467 6574 732e 514c 6162  = QtWidgets.QLab
+000028c0: 656c 2873 656c 662e 7461 625f 6772 6176  el(self.tab_grav
+000028d0: 696d 6574 6572 5f69 6e66 6f29 0a20 2020  imeter_info).   
+000028e0: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
+000028f0: 6772 6176 695f 7365 7269 616c 5f6e 756d  gravi_serial_num
+00002900: 6265 722e 7365 7454 6578 7428 2222 290a  ber.setText("").
+00002910: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
+00002920: 656c 5f67 7261 7669 5f73 6572 6961 6c5f  el_gravi_serial_
+00002930: 6e75 6d62 6572 2e73 6574 4f62 6a65 6374  number.setObject
+00002940: 4e61 6d65 2822 6c61 6265 6c5f 6772 6176  Name("label_grav
+00002950: 695f 7365 7269 616c 5f6e 756d 6265 7222  i_serial_number"
+00002960: 290a 2020 2020 2020 2020 7365 6c66 2e66  ).        self.f
+00002970: 6f72 6d4c 6179 6f75 745f 3132 2e73 6574  ormLayout_12.set
+00002980: 5769 6467 6574 2832 2c20 5174 5769 6467  Widget(2, QtWidg
+00002990: 6574 732e 5146 6f72 6d4c 6179 6f75 742e  ets.QFormLayout.
+000029a0: 4669 656c 6452 6f6c 652c 2073 656c 662e  FieldRole, self.
+000029b0: 6c61 6265 6c5f 6772 6176 695f 7365 7269  label_gravi_seri
+000029c0: 616c 5f6e 756d 6265 7229 0a20 2020 2020  al_number).     
+000029d0: 2020 2073 656c 662e 6c61 6265 6c5f 3235     self.label_25
+000029e0: 203d 2051 7457 6964 6765 7473 2e51 4c61   = QtWidgets.QLa
+000029f0: 6265 6c28 7365 6c66 2e74 6162 5f67 7261  bel(self.tab_gra
+00002a00: 7669 6d65 7465 725f 696e 666f 290a 2020  vimeter_info).  
+00002a10: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
+00002a20: 5f32 352e 7365 744f 626a 6563 744e 616d  _25.setObjectNam
+00002a30: 6528 226c 6162 656c 5f32 3522 290a 2020  e("label_25").  
+00002a40: 2020 2020 2020 7365 6c66 2e66 6f72 6d4c        self.formL
+00002a50: 6179 6f75 745f 3132 2e73 6574 5769 6467  ayout_12.setWidg
+00002a60: 6574 2833 2c20 5174 5769 6467 6574 732e  et(3, QtWidgets.
+00002a70: 5146 6f72 6d4c 6179 6f75 742e 4c61 6265  QFormLayout.Labe
+00002a80: 6c52 6f6c 652c 2073 656c 662e 6c61 6265  lRole, self.labe
+00002a90: 6c5f 3235 290a 2020 2020 2020 2020 7365  l_25).        se
+00002aa0: 6c66 2e6c 6162 656c 5f67 7261 7669 5f63  lf.label_gravi_c
+00002ab0: 6f64 6520 3d20 5174 5769 6467 6574 732e  ode = QtWidgets.
+00002ac0: 514c 6162 656c 2873 656c 662e 7461 625f  QLabel(self.tab_
+00002ad0: 6772 6176 696d 6574 6572 5f69 6e66 6f29  gravimeter_info)
+00002ae0: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
+00002af0: 6265 6c5f 6772 6176 695f 636f 6465 2e73  bel_gravi_code.s
+00002b00: 6574 5465 7874 2822 2229 0a20 2020 2020  etText("").     
+00002b10: 2020 2073 656c 662e 6c61 6265 6c5f 6772     self.label_gr
+00002b20: 6176 695f 636f 6465 2e73 6574 4f62 6a65  avi_code.setObje
+00002b30: 6374 4e61 6d65 2822 6c61 6265 6c5f 6772  ctName("label_gr
+00002b40: 6176 695f 636f 6465 2229 0a20 2020 2020  avi_code").     
+00002b50: 2020 2073 656c 662e 666f 726d 4c61 796f     self.formLayo
+00002b60: 7574 5f31 322e 7365 7457 6964 6765 7428  ut_12.setWidget(
+00002b70: 332c 2051 7457 6964 6765 7473 2e51 466f  3, QtWidgets.QFo
+00002b80: 726d 4c61 796f 7574 2e46 6965 6c64 526f  rmLayout.FieldRo
+00002b90: 6c65 2c20 7365 6c66 2e6c 6162 656c 5f67  le, self.label_g
+00002ba0: 7261 7669 5f63 6f64 6529 0a20 2020 2020  ravi_code).     
+00002bb0: 2020 2073 656c 662e 6c61 6265 6c5f 3232     self.label_22
+00002bc0: 203d 2051 7457 6964 6765 7473 2e51 4c61   = QtWidgets.QLa
+00002bd0: 6265 6c28 7365 6c66 2e74 6162 5f67 7261  bel(self.tab_gra
+00002be0: 7669 6d65 7465 725f 696e 666f 290a 2020  vimeter_info).  
+00002bf0: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
+00002c00: 5f32 322e 7365 744f 626a 6563 744e 616d  _22.setObjectNam
+00002c10: 6528 226c 6162 656c 5f32 3222 290a 2020  e("label_22").  
+00002c20: 2020 2020 2020 7365 6c66 2e66 6f72 6d4c        self.formL
+00002c30: 6179 6f75 745f 3132 2e73 6574 5769 6467  ayout_12.setWidg
+00002c40: 6574 2834 2c20 5174 5769 6467 6574 732e  et(4, QtWidgets.
+00002c50: 5146 6f72 6d4c 6179 6f75 742e 4c61 6265  QFormLayout.Labe
+00002c60: 6c52 6f6c 652c 2073 656c 662e 6c61 6265  lRole, self.labe
+00002c70: 6c5f 3232 290a 2020 2020 2020 2020 7365  l_22).        se
+00002c80: 6c66 2e6c 6162 656c 5f67 7261 7669 5f68  lf.label_gravi_h
+00002c90: 6569 6768 745f 6f66 6673 6574 203d 2051  eight_offset = Q
+00002ca0: 7457 6964 6765 7473 2e51 4c61 6265 6c28  tWidgets.QLabel(
+00002cb0: 7365 6c66 2e74 6162 5f67 7261 7669 6d65  self.tab_gravime
+00002cc0: 7465 725f 696e 666f 290a 2020 2020 2020  ter_info).      
+00002cd0: 2020 7365 6c66 2e6c 6162 656c 5f67 7261    self.label_gra
+00002ce0: 7669 5f68 6569 6768 745f 6f66 6673 6574  vi_height_offset
+00002cf0: 2e73 6574 5465 7874 2822 2229 0a20 2020  .setText("").   
+00002d00: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
+00002d10: 6772 6176 695f 6865 6967 6874 5f6f 6666  gravi_height_off
+00002d20: 7365 742e 7365 744f 626a 6563 744e 616d  set.setObjectNam
+00002d30: 6528 226c 6162 656c 5f67 7261 7669 5f68  e("label_gravi_h
+00002d40: 6569 6768 745f 6f66 6673 6574 2229 0a20  eight_offset"). 
+00002d50: 2020 2020 2020 2073 656c 662e 666f 726d         self.form
+00002d60: 4c61 796f 7574 5f31 322e 7365 7457 6964  Layout_12.setWid
+00002d70: 6765 7428 342c 2051 7457 6964 6765 7473  get(4, QtWidgets
+00002d80: 2e51 466f 726d 4c61 796f 7574 2e46 6965  .QFormLayout.Fie
+00002d90: 6c64 526f 6c65 2c20 7365 6c66 2e6c 6162  ldRole, self.lab
+00002da0: 656c 5f67 7261 7669 5f68 6569 6768 745f  el_gravi_height_
+00002db0: 6f66 6673 6574 290a 2020 2020 2020 2020  offset).        
+00002dc0: 7365 6c66 2e6c 6162 656c 5f32 3320 3d20  self.label_23 = 
+00002dd0: 5174 5769 6467 6574 732e 514c 6162 656c  QtWidgets.QLabel
+00002de0: 2873 656c 662e 7461 625f 6772 6176 696d  (self.tab_gravim
+00002df0: 6574 6572 5f69 6e66 6f29 0a20 2020 2020  eter_info).     
+00002e00: 2020 2073 656c 662e 6c61 6265 6c5f 3233     self.label_23
+00002e10: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
+00002e20: 6c61 6265 6c5f 3233 2229 0a20 2020 2020  label_23").     
+00002e30: 2020 2073 656c 662e 666f 726d 4c61 796f     self.formLayo
+00002e40: 7574 5f31 322e 7365 7457 6964 6765 7428  ut_12.setWidget(
+00002e50: 352c 2051 7457 6964 6765 7473 2e51 466f  5, QtWidgets.QFo
+00002e60: 726d 4c61 796f 7574 2e4c 6162 656c 526f  rmLayout.LabelRo
+00002e70: 6c65 2c20 7365 6c66 2e6c 6162 656c 5f32  le, self.label_2
+00002e80: 3329 0a20 2020 2020 2020 2073 656c 662e  3).        self.
+00002e90: 6c61 6265 6c5f 6772 6176 695f 6461 7461  label_gravi_data
+00002ea0: 5f73 6f75 7263 6520 3d20 5174 5769 6467  _source = QtWidg
+00002eb0: 6574 732e 514c 6162 656c 2873 656c 662e  ets.QLabel(self.
+00002ec0: 7461 625f 6772 6176 696d 6574 6572 5f69  tab_gravimeter_i
+00002ed0: 6e66 6f29 0a20 2020 2020 2020 2073 656c  nfo).        sel
+00002ee0: 662e 6c61 6265 6c5f 6772 6176 695f 6461  f.label_gravi_da
+00002ef0: 7461 5f73 6f75 7263 652e 7365 7454 6578  ta_source.setTex
+00002f00: 7428 2222 290a 2020 2020 2020 2020 7365  t("").        se
+00002f10: 6c66 2e6c 6162 656c 5f67 7261 7669 5f64  lf.label_gravi_d
+00002f20: 6174 615f 736f 7572 6365 2e73 6574 4f62  ata_source.setOb
+00002f30: 6a65 6374 4e61 6d65 2822 6c61 6265 6c5f  jectName("label_
+00002f40: 6772 6176 695f 6461 7461 5f73 6f75 7263  gravi_data_sourc
+00002f50: 6522 290a 2020 2020 2020 2020 7365 6c66  e").        self
+00002f60: 2e66 6f72 6d4c 6179 6f75 745f 3132 2e73  .formLayout_12.s
+00002f70: 6574 5769 6467 6574 2835 2c20 5174 5769  etWidget(5, QtWi
+00002f80: 6467 6574 732e 5146 6f72 6d4c 6179 6f75  dgets.QFormLayou
+00002f90: 742e 4669 656c 6452 6f6c 652c 2073 656c  t.FieldRole, sel
+00002fa0: 662e 6c61 6265 6c5f 6772 6176 695f 6461  f.label_gravi_da
+00002fb0: 7461 5f73 6f75 7263 6529 0a20 2020 2020  ta_source).     
+00002fc0: 2020 2073 656c 662e 6c61 6265 6c5f 3234     self.label_24
+00002fd0: 203d 2051 7457 6964 6765 7473 2e51 4c61   = QtWidgets.QLa
+00002fe0: 6265 6c28 7365 6c66 2e74 6162 5f67 7261  bel(self.tab_gra
+00002ff0: 7669 6d65 7465 725f 696e 666f 290a 2020  vimeter_info).  
+00003000: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
+00003010: 5f32 342e 7365 744f 626a 6563 744e 616d  _24.setObjectNam
+00003020: 6528 226c 6162 656c 5f32 3422 290a 2020  e("label_24").  
+00003030: 2020 2020 2020 7365 6c66 2e66 6f72 6d4c        self.formL
+00003040: 6179 6f75 745f 3132 2e73 6574 5769 6467  ayout_12.setWidg
+00003050: 6574 2836 2c20 5174 5769 6467 6574 732e  et(6, QtWidgets.
+00003060: 5146 6f72 6d4c 6179 6f75 742e 4c61 6265  QFormLayout.Labe
+00003070: 6c52 6f6c 652c 2073 656c 662e 6c61 6265  lRole, self.labe
+00003080: 6c5f 3234 290a 2020 2020 2020 2020 7365  l_24).        se
+00003090: 6c66 2e6c 6162 656c 5f67 7261 7669 5f64  lf.label_gravi_d
+000030a0: 6174 615f 736f 7572 6365 5f74 7970 6520  ata_source_type 
+000030b0: 3d20 5174 5769 6467 6574 732e 514c 6162  = QtWidgets.QLab
+000030c0: 656c 2873 656c 662e 7461 625f 6772 6176  el(self.tab_grav
+000030d0: 696d 6574 6572 5f69 6e66 6f29 0a20 2020  imeter_info).   
+000030e0: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
+000030f0: 6772 6176 695f 6461 7461 5f73 6f75 7263  gravi_data_sourc
+00003100: 655f 7479 7065 2e73 6574 5465 7874 2822  e_type.setText("
+00003110: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00003120: 6c61 6265 6c5f 6772 6176 695f 6461 7461  label_gravi_data
+00003130: 5f73 6f75 7263 655f 7479 7065 2e73 6574  _source_type.set
+00003140: 4f62 6a65 6374 4e61 6d65 2822 6c61 6265  ObjectName("labe
+00003150: 6c5f 6772 6176 695f 6461 7461 5f73 6f75  l_gravi_data_sou
+00003160: 7263 655f 7479 7065 2229 0a20 2020 2020  rce_type").     
+00003170: 2020 2073 656c 662e 666f 726d 4c61 796f     self.formLayo
+00003180: 7574 5f31 322e 7365 7457 6964 6765 7428  ut_12.setWidget(
+00003190: 362c 2051 7457 6964 6765 7473 2e51 466f  6, QtWidgets.QFo
+000031a0: 726d 4c61 796f 7574 2e46 6965 6c64 526f  rmLayout.FieldRo
+000031b0: 6c65 2c20 7365 6c66 2e6c 6162 656c 5f67  le, self.label_g
+000031c0: 7261 7669 5f64 6174 615f 736f 7572 6365  ravi_data_source
+000031d0: 5f74 7970 6529 0a20 2020 2020 2020 2073  _type).        s
+000031e0: 656c 662e 6c61 6265 6c5f 3236 203d 2051  elf.label_26 = Q
+000031f0: 7457 6964 6765 7473 2e51 4c61 6265 6c28  tWidgets.QLabel(
+00003200: 7365 6c66 2e74 6162 5f67 7261 7669 6d65  self.tab_gravime
+00003210: 7465 725f 696e 666f 290a 2020 2020 2020  ter_info).      
+00003220: 2020 7365 6c66 2e6c 6162 656c 5f32 362e    self.label_26.
+00003230: 7365 744f 626a 6563 744e 616d 6528 226c  setObjectName("l
+00003240: 6162 656c 5f32 3622 290a 2020 2020 2020  abel_26").      
+00003250: 2020 7365 6c66 2e66 6f72 6d4c 6179 6f75    self.formLayou
+00003260: 745f 3132 2e73 6574 5769 6467 6574 2837  t_12.setWidget(7
+00003270: 2c20 5174 5769 6467 6574 732e 5146 6f72  , QtWidgets.QFor
+00003280: 6d4c 6179 6f75 742e 4c61 6265 6c52 6f6c  mLayout.LabelRol
+00003290: 652c 2073 656c 662e 6c61 6265 6c5f 3236  e, self.label_26
+000032a0: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
+000032b0: 6162 656c 5f67 7261 7669 5f6e 756d 5f73  abel_gravi_num_s
+000032c0: 6361 6c65 5f66 6163 746f 7273 203d 2051  cale_factors = Q
+000032d0: 7457 6964 6765 7473 2e51 4c61 6265 6c28  tWidgets.QLabel(
+000032e0: 7365 6c66 2e74 6162 5f67 7261 7669 6d65  self.tab_gravime
+000032f0: 7465 725f 696e 666f 290a 2020 2020 2020  ter_info).      
+00003300: 2020 7365 6c66 2e6c 6162 656c 5f67 7261    self.label_gra
+00003310: 7669 5f6e 756d 5f73 6361 6c65 5f66 6163  vi_num_scale_fac
+00003320: 746f 7273 2e73 6574 5465 7874 2822 2229  tors.setText("")
+00003330: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
+00003340: 6265 6c5f 6772 6176 695f 6e75 6d5f 7363  bel_gravi_num_sc
+00003350: 616c 655f 6661 6374 6f72 732e 7365 744f  ale_factors.setO
+00003360: 626a 6563 744e 616d 6528 226c 6162 656c  bjectName("label
+00003370: 5f67 7261 7669 5f6e 756d 5f73 6361 6c65  _gravi_num_scale
+00003380: 5f66 6163 746f 7273 2229 0a20 2020 2020  _factors").     
+00003390: 2020 2073 656c 662e 666f 726d 4c61 796f     self.formLayo
+000033a0: 7574 5f31 322e 7365 7457 6964 6765 7428  ut_12.setWidget(
+000033b0: 372c 2051 7457 6964 6765 7473 2e51 466f  7, QtWidgets.QFo
+000033c0: 726d 4c61 796f 7574 2e46 6965 6c64 526f  rmLayout.FieldRo
+000033d0: 6c65 2c20 7365 6c66 2e6c 6162 656c 5f67  le, self.label_g
+000033e0: 7261 7669 5f6e 756d 5f73 6361 6c65 5f66  ravi_num_scale_f
+000033f0: 6163 746f 7273 290a 2020 2020 2020 2020  actors).        
+00003400: 7365 6c66 2e6c 6162 656c 5f32 3820 3d20  self.label_28 = 
+00003410: 5174 5769 6467 6574 732e 514c 6162 656c  QtWidgets.QLabel
+00003420: 2873 656c 662e 7461 625f 6772 6176 696d  (self.tab_gravim
+00003430: 6574 6572 5f69 6e66 6f29 0a20 2020 2020  eter_info).     
+00003440: 2020 2073 656c 662e 6c61 6265 6c5f 3238     self.label_28
+00003450: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
+00003460: 6c61 6265 6c5f 3238 2229 0a20 2020 2020  label_28").     
+00003470: 2020 2073 656c 662e 666f 726d 4c61 796f     self.formLayo
+00003480: 7574 5f31 322e 7365 7457 6964 6765 7428  ut_12.setWidget(
+00003490: 382c 2051 7457 6964 6765 7473 2e51 466f  8, QtWidgets.QFo
+000034a0: 726d 4c61 796f 7574 2e4c 6162 656c 526f  rmLayout.LabelRo
+000034b0: 6c65 2c20 7365 6c66 2e6c 6162 656c 5f32  le, self.label_2
+000034c0: 3829 0a20 2020 2020 2020 2073 656c 662e  8).        self.
+000034d0: 6c61 6265 6c5f 6772 6176 695f 6465 7363  label_gravi_desc
+000034e0: 7269 7074 696f 6e20 3d20 5174 5769 6467  ription = QtWidg
+000034f0: 6574 732e 514c 6162 656c 2873 656c 662e  ets.QLabel(self.
+00003500: 7461 625f 6772 6176 696d 6574 6572 5f69  tab_gravimeter_i
+00003510: 6e66 6f29 0a20 2020 2020 2020 2073 656c  nfo).        sel
+00003520: 662e 6c61 6265 6c5f 6772 6176 695f 6465  f.label_gravi_de
+00003530: 7363 7269 7074 696f 6e2e 7365 7454 6578  scription.setTex
+00003540: 7428 2222 290a 2020 2020 2020 2020 7365  t("").        se
+00003550: 6c66 2e6c 6162 656c 5f67 7261 7669 5f64  lf.label_gravi_d
+00003560: 6573 6372 6970 7469 6f6e 2e73 6574 576f  escription.setWo
+00003570: 7264 5772 6170 2854 7275 6529 0a20 2020  rdWrap(True).   
+00003580: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
+00003590: 6772 6176 695f 6465 7363 7269 7074 696f  gravi_descriptio
+000035a0: 6e2e 7365 744f 626a 6563 744e 616d 6528  n.setObjectName(
+000035b0: 226c 6162 656c 5f67 7261 7669 5f64 6573  "label_gravi_des
+000035c0: 6372 6970 7469 6f6e 2229 0a20 2020 2020  cription").     
+000035d0: 2020 2073 656c 662e 666f 726d 4c61 796f     self.formLayo
+000035e0: 7574 5f31 322e 7365 7457 6964 6765 7428  ut_12.setWidget(
+000035f0: 382c 2051 7457 6964 6765 7473 2e51 466f  8, QtWidgets.QFo
+00003600: 726d 4c61 796f 7574 2e46 6965 6c64 526f  rmLayout.FieldRo
+00003610: 6c65 2c20 7365 6c66 2e6c 6162 656c 5f67  le, self.label_g
+00003620: 7261 7669 5f64 6573 6372 6970 7469 6f6e  ravi_description
+00003630: 290a 2020 2020 2020 2020 7365 6c66 2e76  ).        self.v
+00003640: 6572 7469 6361 6c4c 6179 6f75 745f 3432  erticalLayout_42
+00003650: 2e61 6464 4c61 796f 7574 2873 656c 662e  .addLayout(self.
+00003660: 666f 726d 4c61 796f 7574 5f31 3229 0a20  formLayout_12). 
+00003670: 2020 2020 2020 2073 656c 662e 7461 6257         self.tabW
+00003680: 6964 6765 745f 6772 6176 696d 6574 6572  idget_gravimeter
+00003690: 732e 6164 6454 6162 2873 656c 662e 7461  s.addTab(self.ta
+000036a0: 625f 6772 6176 696d 6574 6572 5f69 6e66  b_gravimeter_inf
+000036b0: 6f2c 2022 2229 0a20 2020 2020 2020 2073  o, "").        s
+000036c0: 656c 662e 7461 625f 6772 6176 696d 6574  elf.tab_gravimet
+000036d0: 6572 5f73 6361 6c65 203d 2051 7457 6964  er_scale = QtWid
+000036e0: 6765 7473 2e51 5769 6467 6574 2829 0a20  gets.QWidget(). 
+000036f0: 2020 2020 2020 2073 656c 662e 7461 625f         self.tab_
+00003700: 6772 6176 696d 6574 6572 5f73 6361 6c65  gravimeter_scale
+00003710: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
+00003720: 7461 625f 6772 6176 696d 6574 6572 5f73  tab_gravimeter_s
+00003730: 6361 6c65 2229 0a20 2020 2020 2020 2073  cale").        s
+00003740: 656c 662e 7665 7274 6963 616c 4c61 796f  elf.verticalLayo
+00003750: 7574 5f34 3120 3d20 5174 5769 6467 6574  ut_41 = QtWidget
+00003760: 732e 5156 426f 784c 6179 6f75 7428 7365  s.QVBoxLayout(se
+00003770: 6c66 2e74 6162 5f67 7261 7669 6d65 7465  lf.tab_gravimete
+00003780: 725f 7363 616c 6529 0a20 2020 2020 2020  r_scale).       
+00003790: 2073 656c 662e 7665 7274 6963 616c 4c61   self.verticalLa
+000037a0: 796f 7574 5f34 312e 7365 744f 626a 6563  yout_41.setObjec
+000037b0: 744e 616d 6528 2276 6572 7469 6361 6c4c  tName("verticalL
+000037c0: 6179 6f75 745f 3431 2229 0a20 2020 2020  ayout_41").     
+000037d0: 2020 2073 656c 662e 7461 626c 6556 6965     self.tableVie
+000037e0: 775f 6772 6176 696d 6574 6572 735f 7363  w_gravimeters_sc
+000037f0: 616c 6520 3d20 5174 5769 6467 6574 732e  ale = QtWidgets.
+00003800: 5154 6162 6c65 5669 6577 2873 656c 662e  QTableView(self.
+00003810: 7461 625f 6772 6176 696d 6574 6572 5f73  tab_gravimeter_s
+00003820: 6361 6c65 290a 2020 2020 2020 2020 7365  cale).        se
+00003830: 6c66 2e74 6162 6c65 5669 6577 5f67 7261  lf.tableView_gra
+00003840: 7669 6d65 7465 7273 5f73 6361 6c65 2e73  vimeters_scale.s
+00003850: 6574 4f62 6a65 6374 4e61 6d65 2822 7461  etObjectName("ta
+00003860: 626c 6556 6965 775f 6772 6176 696d 6574  bleView_gravimet
+00003870: 6572 735f 7363 616c 6522 290a 2020 2020  ers_scale").    
+00003880: 2020 2020 7365 6c66 2e76 6572 7469 6361      self.vertica
+00003890: 6c4c 6179 6f75 745f 3431 2e61 6464 5769  lLayout_41.addWi
+000038a0: 6467 6574 2873 656c 662e 7461 626c 6556  dget(self.tableV
+000038b0: 6965 775f 6772 6176 696d 6574 6572 735f  iew_gravimeters_
+000038c0: 7363 616c 6529 0a20 2020 2020 2020 2073  scale).        s
+000038d0: 656c 662e 7461 6257 6964 6765 745f 6772  elf.tabWidget_gr
+000038e0: 6176 696d 6574 6572 732e 6164 6454 6162  avimeters.addTab
+000038f0: 2873 656c 662e 7461 625f 6772 6176 696d  (self.tab_gravim
+00003900: 6574 6572 5f73 6361 6c65 2c20 2222 290a  eter_scale, "").
+00003910: 2020 2020 2020 2020 7365 6c66 2e76 6572          self.ver
+00003920: 7469 6361 6c4c 6179 6f75 745f 3238 2e61  ticalLayout_28.a
+00003930: 6464 5769 6467 6574 2873 656c 662e 7370  ddWidget(self.sp
+00003940: 6c69 7474 6572 5f67 7261 7669 6d65 7465  litter_gravimete
+00003950: 7273 290a 2020 2020 2020 2020 7365 6c66  rs).        self
+00003960: 2e74 6162 5769 6467 6574 5f4d 6169 6e2e  .tabWidget_Main.
+00003970: 6164 6454 6162 2873 656c 662e 7461 625f  addTab(self.tab_
+00003980: 6d61 696e 5f67 7261 7669 6d65 7465 7273  main_gravimeters
+00003990: 2c20 2222 290a 2020 2020 2020 2020 7365  , "").        se
+000039a0: 6c66 2e74 6162 5f6d 6169 6e5f 6f62 7365  lf.tab_main_obse
+000039b0: 7276 6174 696f 6e73 203d 2051 7457 6964  rvations = QtWid
+000039c0: 6765 7473 2e51 5769 6467 6574 2829 0a20  gets.QWidget(). 
+000039d0: 2020 2020 2020 2073 656c 662e 7461 625f         self.tab_
+000039e0: 6d61 696e 5f6f 6273 6572 7661 7469 6f6e  main_observation
+000039f0: 732e 7365 744f 626a 6563 744e 616d 6528  s.setObjectName(
+00003a00: 2274 6162 5f6d 6169 6e5f 6f62 7365 7276  "tab_main_observ
+00003a10: 6174 696f 6e73 2229 0a20 2020 2020 2020  ations").       
+00003a20: 2073 656c 662e 7665 7274 6963 616c 4c61   self.verticalLa
+00003a30: 796f 7574 5f37 203d 2051 7457 6964 6765  yout_7 = QtWidge
+00003a40: 7473 2e51 5642 6f78 4c61 796f 7574 2873  ts.QVBoxLayout(s
+00003a50: 656c 662e 7461 625f 6d61 696e 5f6f 6273  elf.tab_main_obs
+00003a60: 6572 7661 7469 6f6e 7329 0a20 2020 2020  ervations).     
+00003a70: 2020 2073 656c 662e 7665 7274 6963 616c     self.vertical
+00003a80: 4c61 796f 7574 5f37 2e73 6574 4f62 6a65  Layout_7.setObje
+00003a90: 6374 4e61 6d65 2822 7665 7274 6963 616c  ctName("vertical
+00003aa0: 4c61 796f 7574 5f37 2229 0a20 2020 2020  Layout_7").     
+00003ab0: 2020 2073 656c 662e 7370 6c69 7474 6572     self.splitter
+00003ac0: 5f6f 6273 203d 2051 7457 6964 6765 7473  _obs = QtWidgets
+00003ad0: 2e51 5370 6c69 7474 6572 2873 656c 662e  .QSplitter(self.
+00003ae0: 7461 625f 6d61 696e 5f6f 6273 6572 7661  tab_main_observa
+00003af0: 7469 6f6e 7329 0a20 2020 2020 2020 2073  tions).        s
+00003b00: 656c 662e 7370 6c69 7474 6572 5f6f 6273  elf.splitter_obs
+00003b10: 2e73 6574 546f 6f6c 5469 7044 7572 6174  .setToolTipDurat
+00003b20: 696f 6e28 3129 0a20 2020 2020 2020 2073  ion(1).        s
+00003b30: 656c 662e 7370 6c69 7474 6572 5f6f 6273  elf.splitter_obs
+00003b40: 2e73 6574 4f72 6965 6e74 6174 696f 6e28  .setOrientation(
+00003b50: 5174 436f 7265 2e51 742e 486f 7269 7a6f  QtCore.Qt.Horizo
+00003b60: 6e74 616c 290a 2020 2020 2020 2020 7365  ntal).        se
+00003b70: 6c66 2e73 706c 6974 7465 725f 6f62 732e  lf.splitter_obs.
+00003b80: 7365 744f 626a 6563 744e 616d 6528 2273  setObjectName("s
+00003b90: 706c 6974 7465 725f 6f62 7322 290a 2020  plitter_obs").  
+00003ba0: 2020 2020 2020 7365 6c66 2e6c 6179 6f75        self.layou
+00003bb0: 7457 6964 6765 7431 203d 2051 7457 6964  tWidget1 = QtWid
+00003bc0: 6765 7473 2e51 5769 6467 6574 2873 656c  gets.QWidget(sel
+00003bd0: 662e 7370 6c69 7474 6572 5f6f 6273 290a  f.splitter_obs).
+00003be0: 2020 2020 2020 2020 7365 6c66 2e6c 6179          self.lay
+00003bf0: 6f75 7457 6964 6765 7431 2e73 6574 4f62  outWidget1.setOb
+00003c00: 6a65 6374 4e61 6d65 2822 6c61 796f 7574  jectName("layout
+00003c10: 5769 6467 6574 3122 290a 2020 2020 2020  Widget1").      
+00003c20: 2020 7365 6c66 2e76 6572 7469 6361 6c4c    self.verticalL
+00003c30: 6179 6f75 745f 3520 3d20 5174 5769 6467  ayout_5 = QtWidg
+00003c40: 6574 732e 5156 426f 784c 6179 6f75 7428  ets.QVBoxLayout(
+00003c50: 7365 6c66 2e6c 6179 6f75 7457 6964 6765  self.layoutWidge
+00003c60: 7431 290a 2020 2020 2020 2020 7365 6c66  t1).        self
+00003c70: 2e76 6572 7469 6361 6c4c 6179 6f75 745f  .verticalLayout_
+00003c80: 352e 7365 7443 6f6e 7465 6e74 734d 6172  5.setContentsMar
+00003c90: 6769 6e73 2830 2c20 302c 2030 2c20 3029  gins(0, 0, 0, 0)
+00003ca0: 0a20 2020 2020 2020 2073 656c 662e 7665  .        self.ve
+00003cb0: 7274 6963 616c 4c61 796f 7574 5f35 2e73  rticalLayout_5.s
+00003cc0: 6574 4f62 6a65 6374 4e61 6d65 2822 7665  etObjectName("ve
+00003cd0: 7274 6963 616c 4c61 796f 7574 5f35 2229  rticalLayout_5")
+00003ce0: 0a20 2020 2020 2020 2073 656c 662e 7472  .        self.tr
+00003cf0: 6565 5769 6467 6574 5f6f 6273 6572 7661  eeWidget_observa
+00003d00: 7469 6f6e 7320 3d20 5174 5769 6467 6574  tions = QtWidget
+00003d10: 732e 5154 7265 6557 6964 6765 7428 7365  s.QTreeWidget(se
+00003d20: 6c66 2e6c 6179 6f75 7457 6964 6765 7431  lf.layoutWidget1
+00003d30: 290a 2020 2020 2020 2020 7369 7a65 506f  ).        sizePo
+00003d40: 6c69 6379 203d 2051 7457 6964 6765 7473  licy = QtWidgets
+00003d50: 2e51 5369 7a65 506f 6c69 6379 2851 7457  .QSizePolicy(QtW
+00003d60: 6964 6765 7473 2e51 5369 7a65 506f 6c69  idgets.QSizePoli
+00003d70: 6379 2e45 7870 616e 6469 6e67 2c20 5174  cy.Expanding, Qt
+00003d80: 5769 6467 6574 732e 5153 697a 6550 6f6c  Widgets.QSizePol
+00003d90: 6963 792e 4578 7061 6e64 696e 6729 0a20  icy.Expanding). 
+00003da0: 2020 2020 2020 2073 697a 6550 6f6c 6963         sizePolic
+00003db0: 792e 7365 7448 6f72 697a 6f6e 7461 6c53  y.setHorizontalS
+00003dc0: 7472 6574 6368 2830 290a 2020 2020 2020  tretch(0).      
+00003dd0: 2020 7369 7a65 506f 6c69 6379 2e73 6574    sizePolicy.set
+00003de0: 5665 7274 6963 616c 5374 7265 7463 6828  VerticalStretch(
+00003df0: 3029 0a20 2020 2020 2020 2073 697a 6550  0).        sizeP
+00003e00: 6f6c 6963 792e 7365 7448 6569 6768 7446  olicy.setHeightF
+00003e10: 6f72 5769 6474 6828 7365 6c66 2e74 7265  orWidth(self.tre
+00003e20: 6557 6964 6765 745f 6f62 7365 7276 6174  eWidget_observat
+00003e30: 696f 6e73 2e73 697a 6550 6f6c 6963 7928  ions.sizePolicy(
+00003e40: 292e 6861 7348 6569 6768 7446 6f72 5769  ).hasHeightForWi
+00003e50: 6474 6828 2929 0a20 2020 2020 2020 2073  dth()).        s
+00003e60: 656c 662e 7472 6565 5769 6467 6574 5f6f  elf.treeWidget_o
+00003e70: 6273 6572 7661 7469 6f6e 732e 7365 7453  bservations.setS
+00003e80: 697a 6550 6f6c 6963 7928 7369 7a65 506f  izePolicy(sizePo
+00003e90: 6c69 6379 290a 2020 2020 2020 2020 7365  licy).        se
+00003ea0: 6c66 2e74 7265 6557 6964 6765 745f 6f62  lf.treeWidget_ob
+00003eb0: 7365 7276 6174 696f 6e73 2e73 6574 4d69  servations.setMi
+00003ec0: 6e69 6d75 6d53 697a 6528 5174 436f 7265  nimumSize(QtCore
+00003ed0: 2e51 5369 7a65 2832 3830 2c20 3029 290a  .QSize(280, 0)).
+00003ee0: 2020 2020 2020 2020 7365 6c66 2e74 7265          self.tre
+00003ef0: 6557 6964 6765 745f 6f62 7365 7276 6174  eWidget_observat
+00003f00: 696f 6e73 2e73 6574 4865 6164 6572 4869  ions.setHeaderHi
+00003f10: 6464 656e 2854 7275 6529 0a20 2020 2020  dden(True).     
+00003f20: 2020 2073 656c 662e 7472 6565 5769 6467     self.treeWidg
+00003f30: 6574 5f6f 6273 6572 7661 7469 6f6e 732e  et_observations.
+00003f40: 7365 744f 626a 6563 744e 616d 6528 2274  setObjectName("t
+00003f50: 7265 6557 6964 6765 745f 6f62 7365 7276  reeWidget_observ
+00003f60: 6174 696f 6e73 2229 0a20 2020 2020 2020  ations").       
+00003f70: 2073 656c 662e 7472 6565 5769 6467 6574   self.treeWidget
+00003f80: 5f6f 6273 6572 7661 7469 6f6e 732e 6865  _observations.he
+00003f90: 6164 6572 2829 2e73 6574 5669 7369 626c  ader().setVisibl
+00003fa0: 6528 4661 6c73 6529 0a20 2020 2020 2020  e(False).       
+00003fb0: 2073 656c 662e 7472 6565 5769 6467 6574   self.treeWidget
+00003fc0: 5f6f 6273 6572 7661 7469 6f6e 732e 6865  _observations.he
+00003fd0: 6164 6572 2829 2e73 6574 5374 7265 7463  ader().setStretc
+00003fe0: 684c 6173 7453 6563 7469 6f6e 2854 7275  hLastSection(Tru
+00003ff0: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
+00004000: 7665 7274 6963 616c 4c61 796f 7574 5f35  verticalLayout_5
+00004010: 2e61 6464 5769 6467 6574 2873 656c 662e  .addWidget(self.
+00004020: 7472 6565 5769 6467 6574 5f6f 6273 6572  treeWidget_obser
+00004030: 7661 7469 6f6e 7329 0a20 2020 2020 2020  vations).       
+00004040: 2073 656c 662e 686f 7269 7a6f 6e74 616c   self.horizontal
+00004050: 4c61 796f 7574 5f33 203d 2051 7457 6964  Layout_3 = QtWid
+00004060: 6765 7473 2e51 4842 6f78 4c61 796f 7574  gets.QHBoxLayout
+00004070: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+00004080: 686f 7269 7a6f 6e74 616c 4c61 796f 7574  horizontalLayout
+00004090: 5f33 2e73 6574 4f62 6a65 6374 4e61 6d65  _3.setObjectName
+000040a0: 2822 686f 7269 7a6f 6e74 616c 4c61 796f  ("horizontalLayo
+000040b0: 7574 5f33 2229 0a20 2020 2020 2020 2073  ut_3").        s
+000040c0: 656c 662e 7075 7368 4275 7474 6f6e 5f6f  elf.pushButton_o
+000040d0: 6273 5f63 6f6c 6c61 7073 5f61 6c6c 203d  bs_collaps_all =
+000040e0: 2051 7457 6964 6765 7473 2e51 5075 7368   QtWidgets.QPush
+000040f0: 4275 7474 6f6e 2873 656c 662e 6c61 796f  Button(self.layo
+00004100: 7574 5769 6467 6574 3129 0a20 2020 2020  utWidget1).     
+00004110: 2020 2073 656c 662e 7075 7368 4275 7474     self.pushButt
+00004120: 6f6e 5f6f 6273 5f63 6f6c 6c61 7073 5f61  on_obs_collaps_a
+00004130: 6c6c 2e73 6574 4f62 6a65 6374 4e61 6d65  ll.setObjectName
+00004140: 2822 7075 7368 4275 7474 6f6e 5f6f 6273  ("pushButton_obs
+00004150: 5f63 6f6c 6c61 7073 5f61 6c6c 2229 0a20  _collaps_all"). 
+00004160: 2020 2020 2020 2073 656c 662e 686f 7269         self.hori
+00004170: 7a6f 6e74 616c 4c61 796f 7574 5f33 2e61  zontalLayout_3.a
+00004180: 6464 5769 6467 6574 2873 656c 662e 7075  ddWidget(self.pu
+00004190: 7368 4275 7474 6f6e 5f6f 6273 5f63 6f6c  shButton_obs_col
+000041a0: 6c61 7073 5f61 6c6c 290a 2020 2020 2020  laps_all).      
+000041b0: 2020 7365 6c66 2e70 7573 6842 7574 746f    self.pushButto
+000041c0: 6e5f 6f62 735f 6578 7061 6e64 5f61 6c6c  n_obs_expand_all
+000041d0: 203d 2051 7457 6964 6765 7473 2e51 5075   = QtWidgets.QPu
+000041e0: 7368 4275 7474 6f6e 2873 656c 662e 6c61  shButton(self.la
+000041f0: 796f 7574 5769 6467 6574 3129 0a20 2020  youtWidget1).   
+00004200: 2020 2020 2073 656c 662e 7075 7368 4275       self.pushBu
+00004210: 7474 6f6e 5f6f 6273 5f65 7870 616e 645f  tton_obs_expand_
+00004220: 616c 6c2e 7365 744f 626a 6563 744e 616d  all.setObjectNam
+00004230: 6528 2270 7573 6842 7574 746f 6e5f 6f62  e("pushButton_ob
+00004240: 735f 6578 7061 6e64 5f61 6c6c 2229 0a20  s_expand_all"). 
+00004250: 2020 2020 2020 2073 656c 662e 686f 7269         self.hori
+00004260: 7a6f 6e74 616c 4c61 796f 7574 5f33 2e61  zontalLayout_3.a
+00004270: 6464 5769 6467 6574 2873 656c 662e 7075  ddWidget(self.pu
+00004280: 7368 4275 7474 6f6e 5f6f 6273 5f65 7870  shButton_obs_exp
+00004290: 616e 645f 616c 6c29 0a20 2020 2020 2020  and_all).       
+000042a0: 2073 656c 662e 7665 7274 6963 616c 4c61   self.verticalLa
+000042b0: 796f 7574 5f35 2e61 6464 4c61 796f 7574  yout_5.addLayout
+000042c0: 2873 656c 662e 686f 7269 7a6f 6e74 616c  (self.horizontal
+000042d0: 4c61 796f 7574 5f33 290a 2020 2020 2020  Layout_3).      
+000042e0: 2020 7365 6c66 2e67 726f 7570 426f 785f    self.groupBox_
+000042f0: 6f62 735f 6461 7461 5f6d 616e 6970 756c  obs_data_manipul
+00004300: 6174 696f 6e20 3d20 5174 5769 6467 6574  ation = QtWidget
+00004310: 732e 5147 726f 7570 426f 7828 7365 6c66  s.QGroupBox(self
+00004320: 2e6c 6179 6f75 7457 6964 6765 7431 290a  .layoutWidget1).
+00004330: 2020 2020 2020 2020 7365 6c66 2e67 726f          self.gro
+00004340: 7570 426f 785f 6f62 735f 6461 7461 5f6d  upBox_obs_data_m
+00004350: 616e 6970 756c 6174 696f 6e2e 7365 7445  anipulation.setE
+00004360: 6e61 626c 6564 2846 616c 7365 290a 2020  nabled(False).  
+00004370: 2020 2020 2020 7365 6c66 2e67 726f 7570        self.group
+00004380: 426f 785f 6f62 735f 6461 7461 5f6d 616e  Box_obs_data_man
+00004390: 6970 756c 6174 696f 6e2e 7365 744f 626a  ipulation.setObj
+000043a0: 6563 744e 616d 6528 2267 726f 7570 426f  ectName("groupBo
+000043b0: 785f 6f62 735f 6461 7461 5f6d 616e 6970  x_obs_data_manip
+000043c0: 756c 6174 696f 6e22 290a 2020 2020 2020  ulation").      
+000043d0: 2020 7365 6c66 2e76 6572 7469 6361 6c4c    self.verticalL
+000043e0: 6179 6f75 745f 3130 203d 2051 7457 6964  ayout_10 = QtWid
+000043f0: 6765 7473 2e51 5642 6f78 4c61 796f 7574  gets.QVBoxLayout
+00004400: 2873 656c 662e 6772 6f75 7042 6f78 5f6f  (self.groupBox_o
+00004410: 6273 5f64 6174 615f 6d61 6e69 7075 6c61  bs_data_manipula
+00004420: 7469 6f6e 290a 2020 2020 2020 2020 7365  tion).        se
+00004430: 6c66 2e76 6572 7469 6361 6c4c 6179 6f75  lf.verticalLayou
+00004440: 745f 3130 2e73 6574 4f62 6a65 6374 4e61  t_10.setObjectNa
+00004450: 6d65 2822 7665 7274 6963 616c 4c61 796f  me("verticalLayo
+00004460: 7574 5f31 3022 290a 2020 2020 2020 2020  ut_10").        
+00004470: 7365 6c66 2e70 7573 6842 7574 746f 6e5f  self.pushButton_
+00004480: 6f62 735f 6170 706c 795f 6175 746f 7365  obs_apply_autose
+00004490: 6c65 6374 5f63 7572 7265 6e74 5f64 6174  lect_current_dat
+000044a0: 6120 3d20 5174 5769 6467 6574 732e 5150  a = QtWidgets.QP
+000044b0: 7573 6842 7574 746f 6e28 7365 6c66 2e67  ushButton(self.g
+000044c0: 726f 7570 426f 785f 6f62 735f 6461 7461  roupBox_obs_data
+000044d0: 5f6d 616e 6970 756c 6174 696f 6e29 0a20  _manipulation). 
+000044e0: 2020 2020 2020 2073 656c 662e 7075 7368         self.push
+000044f0: 4275 7474 6f6e 5f6f 6273 5f61 7070 6c79  Button_obs_apply
+00004500: 5f61 7574 6f73 656c 6563 745f 6375 7272  _autoselect_curr
+00004510: 656e 745f 6461 7461 2e73 6574 4f62 6a65  ent_data.setObje
+00004520: 6374 4e61 6d65 2822 7075 7368 4275 7474  ctName("pushButt
+00004530: 6f6e 5f6f 6273 5f61 7070 6c79 5f61 7574  on_obs_apply_aut
+00004540: 6f73 656c 6563 745f 6375 7272 656e 745f  oselect_current_
+00004550: 6461 7461 2229 0a20 2020 2020 2020 2073  data").        s
+00004560: 656c 662e 7665 7274 6963 616c 4c61 796f  elf.verticalLayo
+00004570: 7574 5f31 302e 6164 6457 6964 6765 7428  ut_10.addWidget(
+00004580: 7365 6c66 2e70 7573 6842 7574 746f 6e5f  self.pushButton_
+00004590: 6f62 735f 6170 706c 795f 6175 746f 7365  obs_apply_autose
+000045a0: 6c65 6374 5f63 7572 7265 6e74 5f64 6174  lect_current_dat
+000045b0: 6129 0a20 2020 2020 2020 2073 656c 662e  a).        self.
+000045c0: 7075 7368 4275 7474 6f6e 5f6f 6273 5f63  pushButton_obs_c
+000045d0: 6f6d 705f 7365 7475 705f 6461 7461 203d  omp_setup_data =
+000045e0: 2051 7457 6964 6765 7473 2e51 5075 7368   QtWidgets.QPush
+000045f0: 4275 7474 6f6e 2873 656c 662e 6772 6f75  Button(self.grou
+00004600: 7042 6f78 5f6f 6273 5f64 6174 615f 6d61  pBox_obs_data_ma
+00004610: 6e69 7075 6c61 7469 6f6e 290a 2020 2020  nipulation).    
+00004620: 2020 2020 7365 6c66 2e70 7573 6842 7574      self.pushBut
+00004630: 746f 6e5f 6f62 735f 636f 6d70 5f73 6574  ton_obs_comp_set
+00004640: 7570 5f64 6174 612e 7365 744f 626a 6563  up_data.setObjec
+00004650: 744e 616d 6528 2270 7573 6842 7574 746f  tName("pushButto
+00004660: 6e5f 6f62 735f 636f 6d70 5f73 6574 7570  n_obs_comp_setup
+00004670: 5f64 6174 6122 290a 2020 2020 2020 2020  _data").        
+00004680: 7365 6c66 2e76 6572 7469 6361 6c4c 6179  self.verticalLay
+00004690: 6f75 745f 3130 2e61 6464 5769 6467 6574  out_10.addWidget
+000046a0: 2873 656c 662e 7075 7368 4275 7474 6f6e  (self.pushButton
+000046b0: 5f6f 6273 5f63 6f6d 705f 7365 7475 705f  _obs_comp_setup_
+000046c0: 6461 7461 290a 2020 2020 2020 2020 7365  data).        se
+000046d0: 6c66 2e70 7573 6842 7574 746f 6e5f 6f62  lf.pushButton_ob
+000046e0: 735f 7275 6e5f 6573 7469 6d61 7469 6f6e  s_run_estimation
+000046f0: 203d 2051 7457 6964 6765 7473 2e51 5075   = QtWidgets.QPu
+00004700: 7368 4275 7474 6f6e 2873 656c 662e 6772  shButton(self.gr
+00004710: 6f75 7042 6f78 5f6f 6273 5f64 6174 615f  oupBox_obs_data_
+00004720: 6d61 6e69 7075 6c61 7469 6f6e 290a 2020  manipulation).  
+00004730: 2020 2020 2020 7365 6c66 2e70 7573 6842        self.pushB
+00004740: 7574 746f 6e5f 6f62 735f 7275 6e5f 6573  utton_obs_run_es
+00004750: 7469 6d61 7469 6f6e 2e73 6574 4f62 6a65  timation.setObje
+00004760: 6374 4e61 6d65 2822 7075 7368 4275 7474  ctName("pushButt
+00004770: 6f6e 5f6f 6273 5f72 756e 5f65 7374 696d  on_obs_run_estim
+00004780: 6174 696f 6e22 290a 2020 2020 2020 2020  ation").        
+00004790: 7365 6c66 2e76 6572 7469 6361 6c4c 6179  self.verticalLay
+000047a0: 6f75 745f 3130 2e61 6464 5769 6467 6574  out_10.addWidget
+000047b0: 2873 656c 662e 7075 7368 4275 7474 6f6e  (self.pushButton
+000047c0: 5f6f 6273 5f72 756e 5f65 7374 696d 6174  _obs_run_estimat
+000047d0: 696f 6e29 0a20 2020 2020 2020 2073 656c  ion).        sel
+000047e0: 662e 7665 7274 6963 616c 4c61 796f 7574  f.verticalLayout
+000047f0: 5f35 2e61 6464 5769 6467 6574 2873 656c  _5.addWidget(sel
+00004800: 662e 6772 6f75 7042 6f78 5f6f 6273 5f64  f.groupBox_obs_d
+00004810: 6174 615f 6d61 6e69 7075 6c61 7469 6f6e  ata_manipulation
+00004820: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
+00004830: 726f 7570 426f 785f 6f62 735f 7669 6577  roupBox_obs_view
+00004840: 5f6f 7074 696f 6e73 203d 2051 7457 6964  _options = QtWid
+00004850: 6765 7473 2e51 4772 6f75 7042 6f78 2873  gets.QGroupBox(s
+00004860: 656c 662e 6c61 796f 7574 5769 6467 6574  elf.layoutWidget
+00004870: 3129 0a20 2020 2020 2020 2073 656c 662e  1).        self.
+00004880: 6772 6f75 7042 6f78 5f6f 6273 5f76 6965  groupBox_obs_vie
+00004890: 775f 6f70 7469 6f6e 732e 7365 7445 6e61  w_options.setEna
+000048a0: 626c 6564 2846 616c 7365 290a 2020 2020  bled(False).    
+000048b0: 2020 2020 7365 6c66 2e67 726f 7570 426f      self.groupBo
+000048c0: 785f 6f62 735f 7669 6577 5f6f 7074 696f  x_obs_view_optio
+000048d0: 6e73 2e73 6574 4f62 6a65 6374 4e61 6d65  ns.setObjectName
+000048e0: 2822 6772 6f75 7042 6f78 5f6f 6273 5f76  ("groupBox_obs_v
+000048f0: 6965 775f 6f70 7469 6f6e 7322 290a 2020  iew_options").  
+00004900: 2020 2020 2020 7365 6c66 2e76 6572 7469        self.verti
+00004910: 6361 6c4c 6179 6f75 745f 3920 3d20 5174  calLayout_9 = Qt
+00004920: 5769 6467 6574 732e 5156 426f 784c 6179  Widgets.QVBoxLay
+00004930: 6f75 7428 7365 6c66 2e67 726f 7570 426f  out(self.groupBo
+00004940: 785f 6f62 735f 7669 6577 5f6f 7074 696f  x_obs_view_optio
+00004950: 6e73 290a 2020 2020 2020 2020 7365 6c66  ns).        self
+00004960: 2e76 6572 7469 6361 6c4c 6179 6f75 745f  .verticalLayout_
+00004970: 392e 7365 744f 626a 6563 744e 616d 6528  9.setObjectName(
+00004980: 2276 6572 7469 6361 6c4c 6179 6f75 745f  "verticalLayout_
+00004990: 3922 290a 2020 2020 2020 2020 7365 6c66  9").        self
+000049a0: 2e63 6865 636b 426f 785f 6f62 735f 706c  .checkBox_obs_pl
+000049b0: 6f74 5f72 6564 7563 6564 5f6f 6273 6572  ot_reduced_obser
+000049c0: 7661 7469 6f6e 7320 3d20 5174 5769 6467  vations = QtWidg
+000049d0: 6574 732e 5143 6865 636b 426f 7828 7365  ets.QCheckBox(se
+000049e0: 6c66 2e67 726f 7570 426f 785f 6f62 735f  lf.groupBox_obs_
+000049f0: 7669 6577 5f6f 7074 696f 6e73 290a 2020  view_options).  
+00004a00: 2020 2020 2020 7365 6c66 2e63 6865 636b        self.check
+00004a10: 426f 785f 6f62 735f 706c 6f74 5f72 6564  Box_obs_plot_red
+00004a20: 7563 6564 5f6f 6273 6572 7661 7469 6f6e  uced_observation
+00004a30: 732e 7365 7443 6865 636b 6564 2854 7275  s.setChecked(Tru
+00004a40: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
+00004a50: 6368 6563 6b42 6f78 5f6f 6273 5f70 6c6f  checkBox_obs_plo
+00004a60: 745f 7265 6475 6365 645f 6f62 7365 7276  t_reduced_observ
+00004a70: 6174 696f 6e73 2e73 6574 4f62 6a65 6374  ations.setObject
+00004a80: 4e61 6d65 2822 6368 6563 6b42 6f78 5f6f  Name("checkBox_o
+00004a90: 6273 5f70 6c6f 745f 7265 6475 6365 645f  bs_plot_reduced_
+00004aa0: 6f62 7365 7276 6174 696f 6e73 2229 0a20  observations"). 
+00004ab0: 2020 2020 2020 2073 656c 662e 7665 7274         self.vert
+00004ac0: 6963 616c 4c61 796f 7574 5f39 2e61 6464  icalLayout_9.add
+00004ad0: 5769 6467 6574 2873 656c 662e 6368 6563  Widget(self.chec
+00004ae0: 6b42 6f78 5f6f 6273 5f70 6c6f 745f 7265  kBox_obs_plot_re
+00004af0: 6475 6365 645f 6f62 7365 7276 6174 696f  duced_observatio
+00004b00: 6e73 290a 2020 2020 2020 2020 7365 6c66  ns).        self
+00004b10: 2e63 6865 636b 426f 785f 6f62 735f 706c  .checkBox_obs_pl
+00004b20: 6f74 5f73 6574 7570 5f64 6174 6120 3d20  ot_setup_data = 
+00004b30: 5174 5769 6467 6574 732e 5143 6865 636b  QtWidgets.QCheck
+00004b40: 426f 7828 7365 6c66 2e67 726f 7570 426f  Box(self.groupBo
+00004b50: 785f 6f62 735f 7669 6577 5f6f 7074 696f  x_obs_view_optio
+00004b60: 6e73 290a 2020 2020 2020 2020 7365 6c66  ns).        self
+00004b70: 2e63 6865 636b 426f 785f 6f62 735f 706c  .checkBox_obs_pl
+00004b80: 6f74 5f73 6574 7570 5f64 6174 612e 7365  ot_setup_data.se
+00004b90: 7443 6865 636b 6564 2854 7275 6529 0a20  tChecked(True). 
+00004ba0: 2020 2020 2020 2073 656c 662e 6368 6563         self.chec
+00004bb0: 6b42 6f78 5f6f 6273 5f70 6c6f 745f 7365  kBox_obs_plot_se
+00004bc0: 7475 705f 6461 7461 2e73 6574 4f62 6a65  tup_data.setObje
+00004bd0: 6374 4e61 6d65 2822 6368 6563 6b42 6f78  ctName("checkBox
+00004be0: 5f6f 6273 5f70 6c6f 745f 7365 7475 705f  _obs_plot_setup_
+00004bf0: 6461 7461 2229 0a20 2020 2020 2020 2073  data").        s
+00004c00: 656c 662e 7665 7274 6963 616c 4c61 796f  elf.verticalLayo
+00004c10: 7574 5f39 2e61 6464 5769 6467 6574 2873  ut_9.addWidget(s
+00004c20: 656c 662e 6368 6563 6b42 6f78 5f6f 6273  elf.checkBox_obs
+00004c30: 5f70 6c6f 745f 7365 7475 705f 6461 7461  _plot_setup_data
+00004c40: 290a 2020 2020 2020 2020 7365 6c66 2e76  ).        self.v
+00004c50: 6572 7469 6361 6c4c 6179 6f75 745f 352e  erticalLayout_5.
+00004c60: 6164 6457 6964 6765 7428 7365 6c66 2e67  addWidget(self.g
+00004c70: 726f 7570 426f 785f 6f62 735f 7669 6577  roupBox_obs_view
+00004c80: 5f6f 7074 696f 6e73 290a 2020 2020 2020  _options).      
+00004c90: 2020 7365 6c66 2e74 6162 5769 6467 6574    self.tabWidget
+00004ca0: 5f6f 6273 6572 7661 7469 6f6e 7320 3d20  _observations = 
+00004cb0: 5174 5769 6467 6574 732e 5154 6162 5769  QtWidgets.QTabWi
+00004cc0: 6467 6574 2873 656c 662e 7370 6c69 7474  dget(self.splitt
+00004cd0: 6572 5f6f 6273 290a 2020 2020 2020 2020  er_obs).        
+00004ce0: 7369 7a65 506f 6c69 6379 203d 2051 7457  sizePolicy = QtW
+00004cf0: 6964 6765 7473 2e51 5369 7a65 506f 6c69  idgets.QSizePoli
+00004d00: 6379 2851 7457 6964 6765 7473 2e51 5369  cy(QtWidgets.QSi
+00004d10: 7a65 506f 6c69 6379 2e45 7870 616e 6469  zePolicy.Expandi
+00004d20: 6e67 2c20 5174 5769 6467 6574 732e 5153  ng, QtWidgets.QS
+00004d30: 697a 6550 6f6c 6963 792e 4578 7061 6e64  izePolicy.Expand
+00004d40: 696e 6729 0a20 2020 2020 2020 2073 697a  ing).        siz
+00004d50: 6550 6f6c 6963 792e 7365 7448 6f72 697a  ePolicy.setHoriz
+00004d60: 6f6e 7461 6c53 7472 6574 6368 2831 290a  ontalStretch(1).
+00004d70: 2020 2020 2020 2020 7369 7a65 506f 6c69          sizePoli
+00004d80: 6379 2e73 6574 5665 7274 6963 616c 5374  cy.setVerticalSt
+00004d90: 7265 7463 6828 3029 0a20 2020 2020 2020  retch(0).       
+00004da0: 2073 697a 6550 6f6c 6963 792e 7365 7448   sizePolicy.setH
+00004db0: 6569 6768 7446 6f72 5769 6474 6828 7365  eightForWidth(se
+00004dc0: 6c66 2e74 6162 5769 6467 6574 5f6f 6273  lf.tabWidget_obs
+00004dd0: 6572 7661 7469 6f6e 732e 7369 7a65 506f  ervations.sizePo
+00004de0: 6c69 6379 2829 2e68 6173 4865 6967 6874  licy().hasHeight
+00004df0: 466f 7257 6964 7468 2829 290a 2020 2020  ForWidth()).    
+00004e00: 2020 2020 7365 6c66 2e74 6162 5769 6467      self.tabWidg
+00004e10: 6574 5f6f 6273 6572 7661 7469 6f6e 732e  et_observations.
+00004e20: 7365 7453 697a 6550 6f6c 6963 7928 7369  setSizePolicy(si
+00004e30: 7a65 506f 6c69 6379 290a 2020 2020 2020  zePolicy).      
+00004e40: 2020 7365 6c66 2e74 6162 5769 6467 6574    self.tabWidget
+00004e50: 5f6f 6273 6572 7661 7469 6f6e 732e 7365  _observations.se
+00004e60: 744f 626a 6563 744e 616d 6528 2274 6162  tObjectName("tab
+00004e70: 5769 6467 6574 5f6f 6273 6572 7661 7469  Widget_observati
+00004e80: 6f6e 7322 290a 2020 2020 2020 2020 7365  ons").        se
+00004e90: 6c66 2e74 6162 5f6f 6273 6572 7661 7469  lf.tab_observati
+00004ea0: 6f6e 735f 706c 6f74 7320 3d20 5174 5769  ons_plots = QtWi
+00004eb0: 6467 6574 732e 5157 6964 6765 7428 290a  dgets.QWidget().
+00004ec0: 2020 2020 2020 2020 7365 6c66 2e74 6162          self.tab
+00004ed0: 5f6f 6273 6572 7661 7469 6f6e 735f 706c  _observations_pl
+00004ee0: 6f74 732e 7365 744f 626a 6563 744e 616d  ots.setObjectNam
+00004ef0: 6528 2274 6162 5f6f 6273 6572 7661 7469  e("tab_observati
+00004f00: 6f6e 735f 706c 6f74 7322 290a 2020 2020  ons_plots").    
+00004f10: 2020 2020 7365 6c66 2e76 6572 7469 6361      self.vertica
+00004f20: 6c4c 6179 6f75 745f 3820 3d20 5174 5769  lLayout_8 = QtWi
+00004f30: 6467 6574 732e 5156 426f 784c 6179 6f75  dgets.QVBoxLayou
+00004f40: 7428 7365 6c66 2e74 6162 5f6f 6273 6572  t(self.tab_obser
+00004f50: 7661 7469 6f6e 735f 706c 6f74 7329 0a20  vations_plots). 
+00004f60: 2020 2020 2020 2073 656c 662e 7665 7274         self.vert
+00004f70: 6963 616c 4c61 796f 7574 5f38 2e73 6574  icalLayout_8.set
+00004f80: 4f62 6a65 6374 4e61 6d65 2822 7665 7274  ObjectName("vert
+00004f90: 6963 616c 4c61 796f 7574 5f38 2229 0a20  icalLayout_8"). 
+00004fa0: 2020 2020 2020 2073 656c 662e 4772 6170         self.Grap
+00004fb0: 6869 6373 4c61 796f 7574 5769 6467 6574  hicsLayoutWidget
+00004fc0: 5f6f 6273 6572 7661 7469 6f6e 7320 3d20  _observations = 
+00004fd0: 4772 6170 6869 6373 4c61 796f 7574 5769  GraphicsLayoutWi
+00004fe0: 6467 6574 2873 656c 662e 7461 625f 6f62  dget(self.tab_ob
+00004ff0: 7365 7276 6174 696f 6e73 5f70 6c6f 7473  servations_plots
+00005000: 290a 2020 2020 2020 2020 7365 6c66 2e47  ).        self.G
+00005010: 7261 7068 6963 734c 6179 6f75 7457 6964  raphicsLayoutWid
+00005020: 6765 745f 6f62 7365 7276 6174 696f 6e73  get_observations
+00005030: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
+00005040: 4772 6170 6869 6373 4c61 796f 7574 5769  GraphicsLayoutWi
+00005050: 6467 6574 5f6f 6273 6572 7661 7469 6f6e  dget_observation
+00005060: 7322 290a 2020 2020 2020 2020 7365 6c66  s").        self
+00005070: 2e76 6572 7469 6361 6c4c 6179 6f75 745f  .verticalLayout_
+00005080: 382e 6164 6457 6964 6765 7428 7365 6c66  8.addWidget(self
+00005090: 2e47 7261 7068 6963 734c 6179 6f75 7457  .GraphicsLayoutW
+000050a0: 6964 6765 745f 6f62 7365 7276 6174 696f  idget_observatio
+000050b0: 6e73 290a 2020 2020 2020 2020 7365 6c66  ns).        self
+000050c0: 2e74 6162 5769 6467 6574 5f6f 6273 6572  .tabWidget_obser
+000050d0: 7661 7469 6f6e 732e 6164 6454 6162 2873  vations.addTab(s
+000050e0: 656c 662e 7461 625f 6f62 7365 7276 6174  elf.tab_observat
+000050f0: 696f 6e73 5f70 6c6f 7473 2c20 2222 290a  ions_plots, "").
+00005100: 2020 2020 2020 2020 7365 6c66 2e74 6162          self.tab
+00005110: 5f6f 6273 6572 7661 7469 6f6e 735f 7461  _observations_ta
+00005120: 626c 6520 3d20 5174 5769 6467 6574 732e  ble = QtWidgets.
+00005130: 5157 6964 6765 7428 290a 2020 2020 2020  QWidget().      
+00005140: 2020 7365 6c66 2e74 6162 5f6f 6273 6572    self.tab_obser
+00005150: 7661 7469 6f6e 735f 7461 626c 652e 7365  vations_table.se
+00005160: 744f 626a 6563 744e 616d 6528 2274 6162  tObjectName("tab
+00005170: 5f6f 6273 6572 7661 7469 6f6e 735f 7461  _observations_ta
+00005180: 626c 6522 290a 2020 2020 2020 2020 7365  ble").        se
+00005190: 6c66 2e76 6572 7469 6361 6c4c 6179 6f75  lf.verticalLayou
+000051a0: 745f 3620 3d20 5174 5769 6467 6574 732e  t_6 = QtWidgets.
+000051b0: 5156 426f 784c 6179 6f75 7428 7365 6c66  QVBoxLayout(self
+000051c0: 2e74 6162 5f6f 6273 6572 7661 7469 6f6e  .tab_observation
+000051d0: 735f 7461 626c 6529 0a20 2020 2020 2020  s_table).       
+000051e0: 2073 656c 662e 7665 7274 6963 616c 4c61   self.verticalLa
+000051f0: 796f 7574 5f36 2e73 6574 4f62 6a65 6374  yout_6.setObject
+00005200: 4e61 6d65 2822 7665 7274 6963 616c 4c61  Name("verticalLa
+00005210: 796f 7574 5f36 2229 0a20 2020 2020 2020  yout_6").       
+00005220: 2073 656c 662e 7461 626c 6556 6965 775f   self.tableView_
+00005230: 6f62 7365 7276 6174 696f 6e73 203d 2051  observations = Q
+00005240: 7457 6964 6765 7473 2e51 5461 626c 6556  tWidgets.QTableV
+00005250: 6965 7728 7365 6c66 2e74 6162 5f6f 6273  iew(self.tab_obs
+00005260: 6572 7661 7469 6f6e 735f 7461 626c 6529  ervations_table)
+00005270: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
+00005280: 626c 6556 6965 775f 6f62 7365 7276 6174  bleView_observat
+00005290: 696f 6e73 2e73 6574 4f62 6a65 6374 4e61  ions.setObjectNa
+000052a0: 6d65 2822 7461 626c 6556 6965 775f 6f62  me("tableView_ob
+000052b0: 7365 7276 6174 696f 6e73 2229 0a20 2020  servations").   
+000052c0: 2020 2020 2073 656c 662e 7665 7274 6963       self.vertic
+000052d0: 616c 4c61 796f 7574 5f36 2e61 6464 5769  alLayout_6.addWi
+000052e0: 6467 6574 2873 656c 662e 7461 626c 6556  dget(self.tableV
+000052f0: 6965 775f 6f62 7365 7276 6174 696f 6e73  iew_observations
+00005300: 290a 2020 2020 2020 2020 7365 6c66 2e74  ).        self.t
+00005310: 6162 5769 6467 6574 5f6f 6273 6572 7661  abWidget_observa
+00005320: 7469 6f6e 732e 6164 6454 6162 2873 656c  tions.addTab(sel
+00005330: 662e 7461 625f 6f62 7365 7276 6174 696f  f.tab_observatio
+00005340: 6e73 5f74 6162 6c65 2c20 2222 290a 2020  ns_table, "").  
+00005350: 2020 2020 2020 7365 6c66 2e74 6162 5f73        self.tab_s
+00005360: 7572 7665 7973 203d 2051 7457 6964 6765  urveys = QtWidge
+00005370: 7473 2e51 5769 6467 6574 2829 0a20 2020  ts.QWidget().   
+00005380: 2020 2020 2073 656c 662e 7461 625f 7375       self.tab_su
+00005390: 7276 6579 732e 7365 744f 626a 6563 744e  rveys.setObjectN
+000053a0: 616d 6528 2274 6162 5f73 7572 7665 7973  ame("tab_surveys
+000053b0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+000053c0: 7665 7274 6963 616c 4c61 796f 7574 5f34  verticalLayout_4
+000053d0: 3320 3d20 5174 5769 6467 6574 732e 5156  3 = QtWidgets.QV
+000053e0: 426f 784c 6179 6f75 7428 7365 6c66 2e74  BoxLayout(self.t
+000053f0: 6162 5f73 7572 7665 7973 290a 2020 2020  ab_surveys).    
+00005400: 2020 2020 7365 6c66 2e76 6572 7469 6361      self.vertica
+00005410: 6c4c 6179 6f75 745f 3433 2e73 6574 4f62  lLayout_43.setOb
+00005420: 6a65 6374 4e61 6d65 2822 7665 7274 6963  jectName("vertic
+00005430: 616c 4c61 796f 7574 5f34 3322 290a 2020  alLayout_43").  
+00005440: 2020 2020 2020 7365 6c66 2e74 6162 6c65        self.table
+00005450: 5669 6577 5f73 7572 7665 7973 203d 2051  View_surveys = Q
+00005460: 7457 6964 6765 7473 2e51 5461 626c 6556  tWidgets.QTableV
+00005470: 6965 7728 7365 6c66 2e74 6162 5f73 7572  iew(self.tab_sur
+00005480: 7665 7973 290a 2020 2020 2020 2020 7365  veys).        se
+00005490: 6c66 2e74 6162 6c65 5669 6577 5f73 7572  lf.tableView_sur
+000054a0: 7665 7973 2e73 6574 436f 6e74 6578 744d  veys.setContextM
+000054b0: 656e 7550 6f6c 6963 7928 5174 436f 7265  enuPolicy(QtCore
+000054c0: 2e51 742e 4375 7374 6f6d 436f 6e74 6578  .Qt.CustomContex
+000054d0: 744d 656e 7529 0a20 2020 2020 2020 2073  tMenu).        s
+000054e0: 656c 662e 7461 626c 6556 6965 775f 7375  elf.tableView_su
+000054f0: 7276 6579 732e 7365 744f 626a 6563 744e  rveys.setObjectN
+00005500: 616d 6528 2274 6162 6c65 5669 6577 5f73  ame("tableView_s
+00005510: 7572 7665 7973 2229 0a20 2020 2020 2020  urveys").       
+00005520: 2073 656c 662e 7665 7274 6963 616c 4c61   self.verticalLa
+00005530: 796f 7574 5f34 332e 6164 6457 6964 6765  yout_43.addWidge
+00005540: 7428 7365 6c66 2e74 6162 6c65 5669 6577  t(self.tableView
+00005550: 5f73 7572 7665 7973 290a 2020 2020 2020  _surveys).      
+00005560: 2020 7365 6c66 2e68 6f72 697a 6f6e 7461    self.horizonta
+00005570: 6c4c 6179 6f75 745f 3620 3d20 5174 5769  lLayout_6 = QtWi
+00005580: 6467 6574 732e 5148 426f 784c 6179 6f75  dgets.QHBoxLayou
+00005590: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
+000055a0: 2e68 6f72 697a 6f6e 7461 6c4c 6179 6f75  .horizontalLayou
+000055b0: 745f 362e 7365 744f 626a 6563 744e 616d  t_6.setObjectNam
+000055c0: 6528 2268 6f72 697a 6f6e 7461 6c4c 6179  e("horizontalLay
+000055d0: 6f75 745f 3622 290a 2020 2020 2020 2020  out_6").        
+000055e0: 7365 6c66 2e70 7573 6842 7574 746f 6e5f  self.pushButton_
+000055f0: 7375 7276 6579 735f 656e 6162 6c65 5f61  surveys_enable_a
+00005600: 6c6c 203d 2051 7457 6964 6765 7473 2e51  ll = QtWidgets.Q
+00005610: 5075 7368 4275 7474 6f6e 2873 656c 662e  PushButton(self.
+00005620: 7461 625f 7375 7276 6579 7329 0a20 2020  tab_surveys).   
+00005630: 2020 2020 2073 656c 662e 7075 7368 4275       self.pushBu
+00005640: 7474 6f6e 5f73 7572 7665 7973 5f65 6e61  tton_surveys_ena
+00005650: 626c 655f 616c 6c2e 7365 744f 626a 6563  ble_all.setObjec
+00005660: 744e 616d 6528 2270 7573 6842 7574 746f  tName("pushButto
+00005670: 6e5f 7375 7276 6579 735f 656e 6162 6c65  n_surveys_enable
+00005680: 5f61 6c6c 2229 0a20 2020 2020 2020 2073  _all").        s
+00005690: 656c 662e 686f 7269 7a6f 6e74 616c 4c61  elf.horizontalLa
+000056a0: 796f 7574 5f36 2e61 6464 5769 6467 6574  yout_6.addWidget
+000056b0: 2873 656c 662e 7075 7368 4275 7474 6f6e  (self.pushButton
+000056c0: 5f73 7572 7665 7973 5f65 6e61 626c 655f  _surveys_enable_
+000056d0: 616c 6c29 0a20 2020 2020 2020 2073 656c  all).        sel
+000056e0: 662e 7075 7368 4275 7474 6f6e 5f73 7572  f.pushButton_sur
+000056f0: 7665 7973 5f64 6973 6162 6c65 5f61 6c6c  veys_disable_all
+00005700: 203d 2051 7457 6964 6765 7473 2e51 5075   = QtWidgets.QPu
+00005710: 7368 4275 7474 6f6e 2873 656c 662e 7461  shButton(self.ta
+00005720: 625f 7375 7276 6579 7329 0a20 2020 2020  b_surveys).     
+00005730: 2020 2073 656c 662e 7075 7368 4275 7474     self.pushButt
+00005740: 6f6e 5f73 7572 7665 7973 5f64 6973 6162  on_surveys_disab
+00005750: 6c65 5f61 6c6c 2e73 6574 4f62 6a65 6374  le_all.setObject
+00005760: 4e61 6d65 2822 7075 7368 4275 7474 6f6e  Name("pushButton
+00005770: 5f73 7572 7665 7973 5f64 6973 6162 6c65  _surveys_disable
+00005780: 5f61 6c6c 2229 0a20 2020 2020 2020 2073  _all").        s
+00005790: 656c 662e 686f 7269 7a6f 6e74 616c 4c61  elf.horizontalLa
+000057a0: 796f 7574 5f36 2e61 6464 5769 6467 6574  yout_6.addWidget
+000057b0: 2873 656c 662e 7075 7368 4275 7474 6f6e  (self.pushButton
+000057c0: 5f73 7572 7665 7973 5f64 6973 6162 6c65  _surveys_disable
+000057d0: 5f61 6c6c 290a 2020 2020 2020 2020 7370  _all).        sp
+000057e0: 6163 6572 4974 656d 3120 3d20 5174 5769  acerItem1 = QtWi
+000057f0: 6467 6574 732e 5153 7061 6365 7249 7465  dgets.QSpacerIte
+00005800: 6d28 3430 2c20 3230 2c20 5174 5769 6467  m(40, 20, QtWidg
+00005810: 6574 732e 5153 697a 6550 6f6c 6963 792e  ets.QSizePolicy.
+00005820: 4578 7061 6e64 696e 672c 2051 7457 6964  Expanding, QtWid
+00005830: 6765 7473 2e51 5369 7a65 506f 6c69 6379  gets.QSizePolicy
+00005840: 2e4d 696e 696d 756d 290a 2020 2020 2020  .Minimum).      
+00005850: 2020 7365 6c66 2e68 6f72 697a 6f6e 7461    self.horizonta
+00005860: 6c4c 6179 6f75 745f 362e 6164 6449 7465  lLayout_6.addIte
+00005870: 6d28 7370 6163 6572 4974 656d 3129 0a20  m(spacerItem1). 
+00005880: 2020 2020 2020 2073 656c 662e 7665 7274         self.vert
+00005890: 6963 616c 4c61 796f 7574 5f34 332e 6164  icalLayout_43.ad
+000058a0: 644c 6179 6f75 7428 7365 6c66 2e68 6f72  dLayout(self.hor
+000058b0: 697a 6f6e 7461 6c4c 6179 6f75 745f 3629  izontalLayout_6)
+000058c0: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
+000058d0: 6257 6964 6765 745f 6f62 7365 7276 6174  bWidget_observat
+000058e0: 696f 6e73 2e61 6464 5461 6228 7365 6c66  ions.addTab(self
+000058f0: 2e74 6162 5f73 7572 7665 7973 2c20 2222  .tab_surveys, ""
+00005900: 290a 2020 2020 2020 2020 7365 6c66 2e74  ).        self.t
+00005910: 6162 5f6f 6273 6572 7661 7469 6f6e 735f  ab_observations_
+00005920: 7365 7475 7073 203d 2051 7457 6964 6765  setups = QtWidge
+00005930: 7473 2e51 5769 6467 6574 2829 0a20 2020  ts.QWidget().   
+00005940: 2020 2020 2073 656c 662e 7461 625f 6f62       self.tab_ob
+00005950: 7365 7276 6174 696f 6e73 5f73 6574 7570  servations_setup
+00005960: 732e 7365 744f 626a 6563 744e 616d 6528  s.setObjectName(
+00005970: 2274 6162 5f6f 6273 6572 7661 7469 6f6e  "tab_observation
+00005980: 735f 7365 7475 7073 2229 0a20 2020 2020  s_setups").     
+00005990: 2020 2073 656c 662e 7665 7274 6963 616c     self.vertical
+000059a0: 4c61 796f 7574 5f31 3120 3d20 5174 5769  Layout_11 = QtWi
+000059b0: 6467 6574 732e 5156 426f 784c 6179 6f75  dgets.QVBoxLayou
+000059c0: 7428 7365 6c66 2e74 6162 5f6f 6273 6572  t(self.tab_obser
+000059d0: 7661 7469 6f6e 735f 7365 7475 7073 290a  vations_setups).
+000059e0: 2020 2020 2020 2020 7365 6c66 2e76 6572          self.ver
+000059f0: 7469 6361 6c4c 6179 6f75 745f 3131 2e73  ticalLayout_11.s
+00005a00: 6574 4f62 6a65 6374 4e61 6d65 2822 7665  etObjectName("ve
+00005a10: 7274 6963 616c 4c61 796f 7574 5f31 3122  rticalLayout_11"
+00005a20: 290a 2020 2020 2020 2020 7365 6c66 2e74  ).        self.t
+00005a30: 6162 6c65 5669 6577 5f6f 6273 6572 7661  ableView_observa
+00005a40: 7469 6f6e 735f 7365 7475 7073 203d 2051  tions_setups = Q
+00005a50: 7457 6964 6765 7473 2e51 5461 626c 6556  tWidgets.QTableV
+00005a60: 6965 7728 7365 6c66 2e74 6162 5f6f 6273  iew(self.tab_obs
+00005a70: 6572 7661 7469 6f6e 735f 7365 7475 7073  ervations_setups
+00005a80: 290a 2020 2020 2020 2020 7365 6c66 2e74  ).        self.t
+00005a90: 6162 6c65 5669 6577 5f6f 6273 6572 7661  ableView_observa
+00005aa0: 7469 6f6e 735f 7365 7475 7073 2e73 6574  tions_setups.set
+00005ab0: 4f62 6a65 6374 4e61 6d65 2822 7461 626c  ObjectName("tabl
+00005ac0: 6556 6965 775f 6f62 7365 7276 6174 696f  eView_observatio
+00005ad0: 6e73 5f73 6574 7570 7322 290a 2020 2020  ns_setups").    
+00005ae0: 2020 2020 7365 6c66 2e76 6572 7469 6361      self.vertica
+00005af0: 6c4c 6179 6f75 745f 3131 2e61 6464 5769  lLayout_11.addWi
+00005b00: 6467 6574 2873 656c 662e 7461 626c 6556  dget(self.tableV
+00005b10: 6965 775f 6f62 7365 7276 6174 696f 6e73  iew_observations
+00005b20: 5f73 6574 7570 7329 0a20 2020 2020 2020  _setups).       
+00005b30: 2073 656c 662e 6772 6f75 7042 6f78 5f6f   self.groupBox_o
+00005b40: 6273 5f73 6574 7570 735f 6170 706c 6965  bs_setups_applie
+00005b50: 645f 636f 7272 6563 7469 6f6e 7320 3d20  d_corrections = 
+00005b60: 5174 5769 6467 6574 732e 5147 726f 7570  QtWidgets.QGroup
+00005b70: 426f 7828 7365 6c66 2e74 6162 5f6f 6273  Box(self.tab_obs
+00005b80: 6572 7661 7469 6f6e 735f 7365 7475 7073  ervations_setups
+00005b90: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
+00005ba0: 726f 7570 426f 785f 6f62 735f 7365 7475  roupBox_obs_setu
+00005bb0: 7073 5f61 7070 6c69 6564 5f63 6f72 7265  ps_applied_corre
+00005bc0: 6374 696f 6e73 2e73 6574 4f62 6a65 6374  ctions.setObject
+00005bd0: 4e61 6d65 2822 6772 6f75 7042 6f78 5f6f  Name("groupBox_o
+00005be0: 6273 5f73 6574 7570 735f 6170 706c 6965  bs_setups_applie
+00005bf0: 645f 636f 7272 6563 7469 6f6e 7322 290a  d_corrections").
+00005c00: 2020 2020 2020 2020 7365 6c66 2e66 6f72          self.for
+00005c10: 6d4c 6179 6f75 745f 3620 3d20 5174 5769  mLayout_6 = QtWi
+00005c20: 6467 6574 732e 5146 6f72 6d4c 6179 6f75  dgets.QFormLayou
+00005c30: 7428 7365 6c66 2e67 726f 7570 426f 785f  t(self.groupBox_
+00005c40: 6f62 735f 7365 7475 7073 5f61 7070 6c69  obs_setups_appli
+00005c50: 6564 5f63 6f72 7265 6374 696f 6e73 290a  ed_corrections).
+00005c60: 2020 2020 2020 2020 7365 6c66 2e66 6f72          self.for
+00005c70: 6d4c 6179 6f75 745f 362e 7365 744f 626a  mLayout_6.setObj
+00005c80: 6563 744e 616d 6528 2266 6f72 6d4c 6179  ectName("formLay
+00005c90: 6f75 745f 3622 290a 2020 2020 2020 2020  out_6").        
+00005ca0: 7365 6c66 2e6c 6162 656c 5f6f 6273 5f73  self.label_obs_s
+00005cb0: 6574 7570 735f 3120 3d20 5174 5769 6467  etups_1 = QtWidg
+00005cc0: 6574 732e 514c 6162 656c 2873 656c 662e  ets.QLabel(self.
+00005cd0: 6772 6f75 7042 6f78 5f6f 6273 5f73 6574  groupBox_obs_set
+00005ce0: 7570 735f 6170 706c 6965 645f 636f 7272  ups_applied_corr
+00005cf0: 6563 7469 6f6e 7329 0a20 2020 2020 2020  ections).       
+00005d00: 2073 656c 662e 6c61 6265 6c5f 6f62 735f   self.label_obs_
+00005d10: 7365 7475 7073 5f31 2e73 6574 4f62 6a65  setups_1.setObje
+00005d20: 6374 4e61 6d65 2822 6c61 6265 6c5f 6f62  ctName("label_ob
+00005d30: 735f 7365 7475 7073 5f31 2229 0a20 2020  s_setups_1").   
+00005d40: 2020 2020 2073 656c 662e 666f 726d 4c61       self.formLa
+00005d50: 796f 7574 5f36 2e73 6574 5769 6467 6574  yout_6.setWidget
+00005d60: 2830 2c20 5174 5769 6467 6574 732e 5146  (0, QtWidgets.QF
+00005d70: 6f72 6d4c 6179 6f75 742e 4c61 6265 6c52  ormLayout.LabelR
+00005d80: 6f6c 652c 2073 656c 662e 6c61 6265 6c5f  ole, self.label_
+00005d90: 6f62 735f 7365 7475 7073 5f31 290a 2020  obs_setups_1).  
+00005da0: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
+00005db0: 5f6f 6273 5f73 6574 7570 735f 7469 6461  _obs_setups_tida
+00005dc0: 6c5f 636f 7272 203d 2051 7457 6964 6765  l_corr = QtWidge
+00005dd0: 7473 2e51 4c61 6265 6c28 7365 6c66 2e67  ts.QLabel(self.g
+00005de0: 726f 7570 426f 785f 6f62 735f 7365 7475  roupBox_obs_setu
+00005df0: 7073 5f61 7070 6c69 6564 5f63 6f72 7265  ps_applied_corre
+00005e00: 6374 696f 6e73 290a 2020 2020 2020 2020  ctions).        
+00005e10: 7365 6c66 2e6c 6162 656c 5f6f 6273 5f73  self.label_obs_s
+00005e20: 6574 7570 735f 7469 6461 6c5f 636f 7272  etups_tidal_corr
+00005e30: 2e73 6574 5465 7874 2822 2229 0a20 2020  .setText("").   
+00005e40: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
+00005e50: 6f62 735f 7365 7475 7073 5f74 6964 616c  obs_setups_tidal
+00005e60: 5f63 6f72 722e 7365 744f 626a 6563 744e  _corr.setObjectN
+00005e70: 616d 6528 226c 6162 656c 5f6f 6273 5f73  ame("label_obs_s
+00005e80: 6574 7570 735f 7469 6461 6c5f 636f 7272  etups_tidal_corr
+00005e90: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00005ea0: 666f 726d 4c61 796f 7574 5f36 2e73 6574  formLayout_6.set
+00005eb0: 5769 6467 6574 2830 2c20 5174 5769 6467  Widget(0, QtWidg
+00005ec0: 6574 732e 5146 6f72 6d4c 6179 6f75 742e  ets.QFormLayout.
+00005ed0: 4669 656c 6452 6f6c 652c 2073 656c 662e  FieldRole, self.
+00005ee0: 6c61 6265 6c5f 6f62 735f 7365 7475 7073  label_obs_setups
+00005ef0: 5f74 6964 616c 5f63 6f72 7229 0a20 2020  _tidal_corr).   
+00005f00: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
+00005f10: 6f62 735f 7365 7475 7073 5f32 203d 2051  obs_setups_2 = Q
+00005f20: 7457 6964 6765 7473 2e51 4c61 6265 6c28  tWidgets.QLabel(
+00005f30: 7365 6c66 2e67 726f 7570 426f 785f 6f62  self.groupBox_ob
+00005f40: 735f 7365 7475 7073 5f61 7070 6c69 6564  s_setups_applied
+00005f50: 5f63 6f72 7265 6374 696f 6e73 290a 2020  _corrections).  
+00005f60: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
+00005f70: 5f6f 6273 5f73 6574 7570 735f 322e 7365  _obs_setups_2.se
+00005f80: 744f 626a 6563 744e 616d 6528 226c 6162  tObjectName("lab
+00005f90: 656c 5f6f 6273 5f73 6574 7570 735f 3222  el_obs_setups_2"
+00005fa0: 290a 2020 2020 2020 2020 7365 6c66 2e66  ).        self.f
+00005fb0: 6f72 6d4c 6179 6f75 745f 362e 7365 7457  ormLayout_6.setW
+00005fc0: 6964 6765 7428 312c 2051 7457 6964 6765  idget(1, QtWidge
+00005fd0: 7473 2e51 466f 726d 4c61 796f 7574 2e4c  ts.QFormLayout.L
+00005fe0: 6162 656c 526f 6c65 2c20 7365 6c66 2e6c  abelRole, self.l
 00005ff0: 6162 656c 5f6f 6273 5f73 6574 7570 735f  abel_obs_setups_
-00006000: 6174 6d5f 7072 6573 5f63 6f72 7220 3d20  atm_pres_corr = 
-00006010: 5174 5769 6467 6574 732e 514c 6162 656c  QtWidgets.QLabel
-00006020: 2873 656c 662e 6772 6f75 7042 6f78 5f6f  (self.groupBox_o
-00006030: 6273 5f73 6574 7570 735f 6170 706c 6965  bs_setups_applie
-00006040: 645f 636f 7272 6563 7469 6f6e 7329 0a20  d_corrections). 
-00006050: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
-00006060: 6c5f 6f62 735f 7365 7475 7073 5f61 746d  l_obs_setups_atm
-00006070: 5f70 7265 735f 636f 7272 2e73 6574 5465  _pres_corr.setTe
-00006080: 7874 2822 2229 0a20 2020 2020 2020 2073  xt("").        s
-00006090: 656c 662e 6c61 6265 6c5f 6f62 735f 7365  elf.label_obs_se
-000060a0: 7475 7073 5f61 746d 5f70 7265 735f 636f  tups_atm_pres_co
-000060b0: 7272 2e73 6574 4f62 6a65 6374 4e61 6d65  rr.setObjectName
-000060c0: 2822 6c61 6265 6c5f 6f62 735f 7365 7475  ("label_obs_setu
-000060d0: 7073 5f61 746d 5f70 7265 735f 636f 7272  ps_atm_pres_corr
-000060e0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-000060f0: 666f 726d 4c61 796f 7574 5f36 2e73 6574  formLayout_6.set
-00006100: 5769 6467 6574 2833 2c20 5174 5769 6467  Widget(3, QtWidg
-00006110: 6574 732e 5146 6f72 6d4c 6179 6f75 742e  ets.QFormLayout.
-00006120: 4669 656c 6452 6f6c 652c 2073 656c 662e  FieldRole, self.
-00006130: 6c61 6265 6c5f 6f62 735f 7365 7475 7073  label_obs_setups
-00006140: 5f61 746d 5f70 7265 735f 636f 7272 290a  _atm_pres_corr).
-00006150: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
-00006160: 656c 5f6f 6273 5f73 6574 7570 735f 7363  el_obs_setups_sc
-00006170: 616c 655f 636f 7272 203d 2051 7457 6964  ale_corr = QtWid
-00006180: 6765 7473 2e51 4c61 6265 6c28 7365 6c66  gets.QLabel(self
-00006190: 2e67 726f 7570 426f 785f 6f62 735f 7365  .groupBox_obs_se
-000061a0: 7475 7073 5f61 7070 6c69 6564 5f63 6f72  tups_applied_cor
-000061b0: 7265 6374 696f 6e73 290a 2020 2020 2020  rections).      
-000061c0: 2020 7365 6c66 2e6c 6162 656c 5f6f 6273    self.label_obs
-000061d0: 5f73 6574 7570 735f 7363 616c 655f 636f  _setups_scale_co
-000061e0: 7272 2e73 6574 5465 7874 2822 2229 0a20  rr.setText(""). 
-000061f0: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
-00006200: 6c5f 6f62 735f 7365 7475 7073 5f73 6361  l_obs_setups_sca
-00006210: 6c65 5f63 6f72 722e 7365 744f 626a 6563  le_corr.setObjec
-00006220: 744e 616d 6528 226c 6162 656c 5f6f 6273  tName("label_obs
-00006230: 5f73 6574 7570 735f 7363 616c 655f 636f  _setups_scale_co
-00006240: 7272 2229 0a20 2020 2020 2020 2073 656c  rr").        sel
-00006250: 662e 666f 726d 4c61 796f 7574 5f36 2e73  f.formLayout_6.s
-00006260: 6574 5769 6467 6574 2832 2c20 5174 5769  etWidget(2, QtWi
-00006270: 6467 6574 732e 5146 6f72 6d4c 6179 6f75  dgets.QFormLayou
-00006280: 742e 4669 656c 6452 6f6c 652c 2073 656c  t.FieldRole, sel
-00006290: 662e 6c61 6265 6c5f 6f62 735f 7365 7475  f.label_obs_setu
-000062a0: 7073 5f73 6361 6c65 5f63 6f72 7229 0a20  ps_scale_corr). 
-000062b0: 2020 2020 2020 2073 656c 662e 7665 7274         self.vert
-000062c0: 6963 616c 4c61 796f 7574 5f31 312e 6164  icalLayout_11.ad
-000062d0: 6457 6964 6765 7428 7365 6c66 2e67 726f  dWidget(self.gro
-000062e0: 7570 426f 785f 6f62 735f 7365 7475 7073  upBox_obs_setups
-000062f0: 5f61 7070 6c69 6564 5f63 6f72 7265 6374  _applied_correct
-00006300: 696f 6e73 290a 2020 2020 2020 2020 7365  ions).        se
-00006310: 6c66 2e74 6162 5769 6467 6574 5f6f 6273  lf.tabWidget_obs
-00006320: 6572 7661 7469 6f6e 732e 6164 6454 6162  ervations.addTab
-00006330: 2873 656c 662e 7461 625f 6f62 7365 7276  (self.tab_observ
-00006340: 6174 696f 6e73 5f73 6574 7570 732c 2022  ations_setups, "
-00006350: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00006360: 7665 7274 6963 616c 4c61 796f 7574 5f37  verticalLayout_7
-00006370: 2e61 6464 5769 6467 6574 2873 656c 662e  .addWidget(self.
-00006380: 7370 6c69 7474 6572 5f6f 6273 290a 2020  splitter_obs).  
-00006390: 2020 2020 2020 7365 6c66 2e74 6162 5769        self.tabWi
-000063a0: 6467 6574 5f4d 6169 6e2e 6164 6454 6162  dget_Main.addTab
-000063b0: 2873 656c 662e 7461 625f 6d61 696e 5f6f  (self.tab_main_o
-000063c0: 6273 6572 7661 7469 6f6e 732c 2022 2229  bservations, "")
-000063d0: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
-000063e0: 625f 6d61 696e 5f72 6573 756c 7473 203d  b_main_results =
-000063f0: 2051 7457 6964 6765 7473 2e51 5769 6467   QtWidgets.QWidg
-00006400: 6574 2829 0a20 2020 2020 2020 2073 656c  et().        sel
-00006410: 662e 7461 625f 6d61 696e 5f72 6573 756c  f.tab_main_resul
-00006420: 7473 2e73 6574 546f 6f6c 5469 7044 7572  ts.setToolTipDur
-00006430: 6174 696f 6e28 3229 0a20 2020 2020 2020  ation(2).       
-00006440: 2073 656c 662e 7461 625f 6d61 696e 5f72   self.tab_main_r
-00006450: 6573 756c 7473 2e73 6574 4f62 6a65 6374  esults.setObject
-00006460: 4e61 6d65 2822 7461 625f 6d61 696e 5f72  Name("tab_main_r
-00006470: 6573 756c 7473 2229 0a20 2020 2020 2020  esults").       
-00006480: 2073 656c 662e 7665 7274 6963 616c 4c61   self.verticalLa
-00006490: 796f 7574 5f31 3420 3d20 5174 5769 6467  yout_14 = QtWidg
-000064a0: 6574 732e 5156 426f 784c 6179 6f75 7428  ets.QVBoxLayout(
-000064b0: 7365 6c66 2e74 6162 5f6d 6169 6e5f 7265  self.tab_main_re
-000064c0: 7375 6c74 7329 0a20 2020 2020 2020 2073  sults).        s
-000064d0: 656c 662e 7665 7274 6963 616c 4c61 796f  elf.verticalLayo
-000064e0: 7574 5f31 342e 7365 744f 626a 6563 744e  ut_14.setObjectN
-000064f0: 616d 6528 2276 6572 7469 6361 6c4c 6179  ame("verticalLay
-00006500: 6f75 745f 3134 2229 0a20 2020 2020 2020  out_14").       
-00006510: 2073 656c 662e 7370 6c69 7474 6572 5f72   self.splitter_r
-00006520: 6573 756c 7473 203d 2051 7457 6964 6765  esults = QtWidge
-00006530: 7473 2e51 5370 6c69 7474 6572 2873 656c  ts.QSplitter(sel
-00006540: 662e 7461 625f 6d61 696e 5f72 6573 756c  f.tab_main_resul
-00006550: 7473 290a 2020 2020 2020 2020 7365 6c66  ts).        self
-00006560: 2e73 706c 6974 7465 725f 7265 7375 6c74  .splitter_result
-00006570: 732e 7365 744f 7269 656e 7461 7469 6f6e  s.setOrientation
-00006580: 2851 7443 6f72 652e 5174 2e48 6f72 697a  (QtCore.Qt.Horiz
-00006590: 6f6e 7461 6c29 0a20 2020 2020 2020 2073  ontal).        s
-000065a0: 656c 662e 7370 6c69 7474 6572 5f72 6573  elf.splitter_res
-000065b0: 756c 7473 2e73 6574 4f62 6a65 6374 4e61  ults.setObjectNa
-000065c0: 6d65 2822 7370 6c69 7474 6572 5f72 6573  me("splitter_res
-000065d0: 756c 7473 2229 0a20 2020 2020 2020 2073  ults").        s
-000065e0: 656c 662e 7665 7274 6963 616c 4c61 796f  elf.verticalLayo
-000065f0: 7574 5769 6467 6574 203d 2051 7457 6964  utWidget = QtWid
-00006600: 6765 7473 2e51 5769 6467 6574 2873 656c  gets.QWidget(sel
-00006610: 662e 7370 6c69 7474 6572 5f72 6573 756c  f.splitter_resul
-00006620: 7473 290a 2020 2020 2020 2020 7365 6c66  ts).        self
-00006630: 2e76 6572 7469 6361 6c4c 6179 6f75 7457  .verticalLayoutW
-00006640: 6964 6765 742e 7365 744f 626a 6563 744e  idget.setObjectN
-00006650: 616d 6528 2276 6572 7469 6361 6c4c 6179  ame("verticalLay
-00006660: 6f75 7457 6964 6765 7422 290a 2020 2020  outWidget").    
-00006670: 2020 2020 7365 6c66 2e76 6572 7469 6361      self.vertica
-00006680: 6c4c 6179 6f75 745f 3132 203d 2051 7457  lLayout_12 = QtW
-00006690: 6964 6765 7473 2e51 5642 6f78 4c61 796f  idgets.QVBoxLayo
-000066a0: 7574 2873 656c 662e 7665 7274 6963 616c  ut(self.vertical
-000066b0: 4c61 796f 7574 5769 6467 6574 290a 2020  LayoutWidget).  
-000066c0: 2020 2020 2020 7365 6c66 2e76 6572 7469        self.verti
-000066d0: 6361 6c4c 6179 6f75 745f 3132 2e73 6574  calLayout_12.set
-000066e0: 436f 6e74 656e 7473 4d61 7267 696e 7328  ContentsMargins(
-000066f0: 302c 2030 2c20 302c 2030 290a 2020 2020  0, 0, 0, 0).    
-00006700: 2020 2020 7365 6c66 2e76 6572 7469 6361      self.vertica
-00006710: 6c4c 6179 6f75 745f 3132 2e73 6574 4f62  lLayout_12.setOb
-00006720: 6a65 6374 4e61 6d65 2822 7665 7274 6963  jectName("vertic
-00006730: 616c 4c61 796f 7574 5f31 3222 290a 2020  alLayout_12").  
-00006740: 2020 2020 2020 7365 6c66 2e67 726f 7570        self.group
-00006750: 426f 785f 7265 7375 6c74 735f 6c73 6d5f  Box_results_lsm_
-00006760: 7275 6e73 203d 2051 7457 6964 6765 7473  runs = QtWidgets
-00006770: 2e51 4772 6f75 7042 6f78 2873 656c 662e  .QGroupBox(self.
-00006780: 7665 7274 6963 616c 4c61 796f 7574 5769  verticalLayoutWi
-00006790: 6467 6574 290a 2020 2020 2020 2020 7365  dget).        se
-000067a0: 6c66 2e67 726f 7570 426f 785f 7265 7375  lf.groupBox_resu
-000067b0: 6c74 735f 6c73 6d5f 7275 6e73 2e73 6574  lts_lsm_runs.set
-000067c0: 4f62 6a65 6374 4e61 6d65 2822 6772 6f75  ObjectName("grou
-000067d0: 7042 6f78 5f72 6573 756c 7473 5f6c 736d  pBox_results_lsm
-000067e0: 5f72 756e 7322 290a 2020 2020 2020 2020  _runs").        
-000067f0: 7365 6c66 2e76 6572 7469 6361 6c4c 6179  self.verticalLay
-00006800: 6f75 745f 3136 203d 2051 7457 6964 6765  out_16 = QtWidge
-00006810: 7473 2e51 5642 6f78 4c61 796f 7574 2873  ts.QVBoxLayout(s
-00006820: 656c 662e 6772 6f75 7042 6f78 5f72 6573  elf.groupBox_res
-00006830: 756c 7473 5f6c 736d 5f72 756e 7329 0a20  ults_lsm_runs). 
-00006840: 2020 2020 2020 2073 656c 662e 7665 7274         self.vert
-00006850: 6963 616c 4c61 796f 7574 5f31 362e 7365  icalLayout_16.se
-00006860: 744f 626a 6563 744e 616d 6528 2276 6572  tObjectName("ver
-00006870: 7469 6361 6c4c 6179 6f75 745f 3136 2229  ticalLayout_16")
-00006880: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-00006890: 6d62 6f42 6f78 5f72 6573 756c 7473 5f6c  mboBox_results_l
-000068a0: 736d 5f72 756e 5f73 656c 6563 7469 6f6e  sm_run_selection
-000068b0: 203d 2051 7457 6964 6765 7473 2e51 436f   = QtWidgets.QCo
-000068c0: 6d62 6f42 6f78 2873 656c 662e 6772 6f75  mboBox(self.grou
-000068d0: 7042 6f78 5f72 6573 756c 7473 5f6c 736d  pBox_results_lsm
-000068e0: 5f72 756e 7329 0a20 2020 2020 2020 2073  _runs).        s
-000068f0: 656c 662e 636f 6d62 6f42 6f78 5f72 6573  elf.comboBox_res
-00006900: 756c 7473 5f6c 736d 5f72 756e 5f73 656c  ults_lsm_run_sel
-00006910: 6563 7469 6f6e 2e73 6574 4f62 6a65 6374  ection.setObject
-00006920: 4e61 6d65 2822 636f 6d62 6f42 6f78 5f72  Name("comboBox_r
-00006930: 6573 756c 7473 5f6c 736d 5f72 756e 5f73  esults_lsm_run_s
-00006940: 656c 6563 7469 6f6e 2229 0a20 2020 2020  election").     
-00006950: 2020 2073 656c 662e 7665 7274 6963 616c     self.vertical
-00006960: 4c61 796f 7574 5f31 362e 6164 6457 6964  Layout_16.addWid
-00006970: 6765 7428 7365 6c66 2e63 6f6d 626f 426f  get(self.comboBo
-00006980: 785f 7265 7375 6c74 735f 6c73 6d5f 7275  x_results_lsm_ru
-00006990: 6e5f 7365 6c65 6374 696f 6e29 0a20 2020  n_selection).   
-000069a0: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
-000069b0: 7265 7375 6c74 735f 6c73 6d5f 7275 6e5f  results_lsm_run_
-000069c0: 636f 6d6d 656e 745f 6469 7370 6c61 7920  comment_display 
-000069d0: 3d20 5174 5769 6467 6574 732e 514c 6162  = QtWidgets.QLab
-000069e0: 656c 2873 656c 662e 6772 6f75 7042 6f78  el(self.groupBox
-000069f0: 5f72 6573 756c 7473 5f6c 736d 5f72 756e  _results_lsm_run
-00006a00: 7329 0a20 2020 2020 2020 2073 656c 662e  s).        self.
-00006a10: 6c61 6265 6c5f 7265 7375 6c74 735f 6c73  label_results_ls
-00006a20: 6d5f 7275 6e5f 636f 6d6d 656e 745f 6469  m_run_comment_di
-00006a30: 7370 6c61 792e 7365 7454 6578 7428 2222  splay.setText(""
-00006a40: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
-00006a50: 6162 656c 5f72 6573 756c 7473 5f6c 736d  abel_results_lsm
-00006a60: 5f72 756e 5f63 6f6d 6d65 6e74 5f64 6973  _run_comment_dis
-00006a70: 706c 6179 2e73 6574 4f62 6a65 6374 4e61  play.setObjectNa
-00006a80: 6d65 2822 6c61 6265 6c5f 7265 7375 6c74  me("label_result
-00006a90: 735f 6c73 6d5f 7275 6e5f 636f 6d6d 656e  s_lsm_run_commen
-00006aa0: 745f 6469 7370 6c61 7922 290a 2020 2020  t_display").    
-00006ab0: 2020 2020 7365 6c66 2e76 6572 7469 6361      self.vertica
-00006ac0: 6c4c 6179 6f75 745f 3136 2e61 6464 5769  lLayout_16.addWi
-00006ad0: 6467 6574 2873 656c 662e 6c61 6265 6c5f  dget(self.label_
-00006ae0: 7265 7375 6c74 735f 6c73 6d5f 7275 6e5f  results_lsm_run_
-00006af0: 636f 6d6d 656e 745f 6469 7370 6c61 7929  comment_display)
-00006b00: 0a20 2020 2020 2020 2073 656c 662e 7075  .        self.pu
-00006b10: 7368 4275 7474 6f6e 5f72 6573 756c 7473  shButton_results
-00006b20: 5f64 656c 6574 655f 6c73 6d5f 7275 6e20  _delete_lsm_run 
-00006b30: 3d20 5174 5769 6467 6574 732e 5150 7573  = QtWidgets.QPus
-00006b40: 6842 7574 746f 6e28 7365 6c66 2e67 726f  hButton(self.gro
-00006b50: 7570 426f 785f 7265 7375 6c74 735f 6c73  upBox_results_ls
-00006b60: 6d5f 7275 6e73 290a 2020 2020 2020 2020  m_runs).        
-00006b70: 7365 6c66 2e70 7573 6842 7574 746f 6e5f  self.pushButton_
-00006b80: 7265 7375 6c74 735f 6465 6c65 7465 5f6c  results_delete_l
-00006b90: 736d 5f72 756e 2e73 6574 4f62 6a65 6374  sm_run.setObject
-00006ba0: 4e61 6d65 2822 7075 7368 4275 7474 6f6e  Name("pushButton
-00006bb0: 5f72 6573 756c 7473 5f64 656c 6574 655f  _results_delete_
-00006bc0: 6c73 6d5f 7275 6e22 290a 2020 2020 2020  lsm_run").      
-00006bd0: 2020 7365 6c66 2e76 6572 7469 6361 6c4c    self.verticalL
-00006be0: 6179 6f75 745f 3136 2e61 6464 5769 6467  ayout_16.addWidg
-00006bf0: 6574 2873 656c 662e 7075 7368 4275 7474  et(self.pushButt
-00006c00: 6f6e 5f72 6573 756c 7473 5f64 656c 6574  on_results_delet
-00006c10: 655f 6c73 6d5f 7275 6e29 0a20 2020 2020  e_lsm_run).     
-00006c20: 2020 2073 656c 662e 7665 7274 6963 616c     self.vertical
-00006c30: 4c61 796f 7574 5f31 322e 6164 6457 6964  Layout_12.addWid
-00006c40: 6765 7428 7365 6c66 2e67 726f 7570 426f  get(self.groupBo
-00006c50: 785f 7265 7375 6c74 735f 6c73 6d5f 7275  x_results_lsm_ru
-00006c60: 6e73 290a 2020 2020 2020 2020 7365 6c66  ns).        self
-00006c70: 2e67 726f 7570 426f 785f 7265 7375 6c74  .groupBox_result
-00006c80: 735f 6461 7461 5f73 656c 6563 7469 6f6e  s_data_selection
-00006c90: 203d 2051 7457 6964 6765 7473 2e51 4772   = QtWidgets.QGr
-00006ca0: 6f75 7042 6f78 2873 656c 662e 7665 7274  oupBox(self.vert
-00006cb0: 6963 616c 4c61 796f 7574 5769 6467 6574  icalLayoutWidget
-00006cc0: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
-00006cd0: 726f 7570 426f 785f 7265 7375 6c74 735f  roupBox_results_
-00006ce0: 6461 7461 5f73 656c 6563 7469 6f6e 2e73  data_selection.s
-00006cf0: 6574 4f62 6a65 6374 4e61 6d65 2822 6772  etObjectName("gr
-00006d00: 6f75 7042 6f78 5f72 6573 756c 7473 5f64  oupBox_results_d
-00006d10: 6174 615f 7365 6c65 6374 696f 6e22 290a  ata_selection").
-00006d20: 2020 2020 2020 2020 7365 6c66 2e76 6572          self.ver
-00006d30: 7469 6361 6c4c 6179 6f75 745f 3137 203d  ticalLayout_17 =
-00006d40: 2051 7457 6964 6765 7473 2e51 5642 6f78   QtWidgets.QVBox
-00006d50: 4c61 796f 7574 2873 656c 662e 6772 6f75  Layout(self.grou
-00006d60: 7042 6f78 5f72 6573 756c 7473 5f64 6174  pBox_results_dat
-00006d70: 615f 7365 6c65 6374 696f 6e29 0a20 2020  a_selection).   
-00006d80: 2020 2020 2073 656c 662e 7665 7274 6963       self.vertic
-00006d90: 616c 4c61 796f 7574 5f31 372e 7365 744f  alLayout_17.setO
-00006da0: 626a 6563 744e 616d 6528 2276 6572 7469  bjectName("verti
-00006db0: 6361 6c4c 6179 6f75 745f 3137 2229 0a20  calLayout_17"). 
-00006dc0: 2020 2020 2020 2073 656c 662e 666f 726d         self.form
-00006dd0: 4c61 796f 7574 203d 2051 7457 6964 6765  Layout = QtWidge
-00006de0: 7473 2e51 466f 726d 4c61 796f 7574 2829  ts.QFormLayout()
-00006df0: 0a20 2020 2020 2020 2073 656c 662e 666f  .        self.fo
-00006e00: 726d 4c61 796f 7574 2e73 6574 4f62 6a65  rmLayout.setObje
-00006e10: 6374 4e61 6d65 2822 666f 726d 4c61 796f  ctName("formLayo
-00006e20: 7574 2229 0a20 2020 2020 2020 2073 656c  ut").        sel
-00006e30: 662e 6c61 6265 6c5f 3220 3d20 5174 5769  f.label_2 = QtWi
-00006e40: 6467 6574 732e 514c 6162 656c 2873 656c  dgets.QLabel(sel
-00006e50: 662e 6772 6f75 7042 6f78 5f72 6573 756c  f.groupBox_resul
-00006e60: 7473 5f64 6174 615f 7365 6c65 6374 696f  ts_data_selectio
-00006e70: 6e29 0a20 2020 2020 2020 2073 656c 662e  n).        self.
-00006e80: 6c61 6265 6c5f 322e 7365 744f 626a 6563  label_2.setObjec
-00006e90: 744e 616d 6528 226c 6162 656c 5f32 2229  tName("label_2")
-00006ea0: 0a20 2020 2020 2020 2073 656c 662e 666f  .        self.fo
-00006eb0: 726d 4c61 796f 7574 2e73 6574 5769 6467  rmLayout.setWidg
-00006ec0: 6574 2830 2c20 5174 5769 6467 6574 732e  et(0, QtWidgets.
-00006ed0: 5146 6f72 6d4c 6179 6f75 742e 4c61 6265  QFormLayout.Labe
-00006ee0: 6c52 6f6c 652c 2073 656c 662e 6c61 6265  lRole, self.labe
-00006ef0: 6c5f 3229 0a20 2020 2020 2020 2073 656c  l_2).        sel
-00006f00: 662e 636f 6d62 6f42 6f78 5f72 6573 756c  f.comboBox_resul
-00006f10: 7473 5f73 656c 6563 7469 6f6e 5f73 7461  ts_selection_sta
-00006f20: 7469 6f6e 203d 2051 7457 6964 6765 7473  tion = QtWidgets
-00006f30: 2e51 436f 6d62 6f42 6f78 2873 656c 662e  .QComboBox(self.
-00006f40: 6772 6f75 7042 6f78 5f72 6573 756c 7473  groupBox_results
-00006f50: 5f64 6174 615f 7365 6c65 6374 696f 6e29  _data_selection)
-00006f60: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-00006f70: 6d62 6f42 6f78 5f72 6573 756c 7473 5f73  mboBox_results_s
-00006f80: 656c 6563 7469 6f6e 5f73 7461 7469 6f6e  election_station
-00006f90: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
-00006fa0: 636f 6d62 6f42 6f78 5f72 6573 756c 7473  comboBox_results
-00006fb0: 5f73 656c 6563 7469 6f6e 5f73 7461 7469  _selection_stati
-00006fc0: 6f6e 2229 0a20 2020 2020 2020 2073 656c  on").        sel
-00006fd0: 662e 636f 6d62 6f42 6f78 5f72 6573 756c  f.comboBox_resul
-00006fe0: 7473 5f73 656c 6563 7469 6f6e 5f73 7461  ts_selection_sta
-00006ff0: 7469 6f6e 2e61 6464 4974 656d 2822 2229  tion.addItem("")
-00007000: 0a20 2020 2020 2020 2073 656c 662e 666f  .        self.fo
-00007010: 726d 4c61 796f 7574 2e73 6574 5769 6467  rmLayout.setWidg
-00007020: 6574 2830 2c20 5174 5769 6467 6574 732e  et(0, QtWidgets.
-00007030: 5146 6f72 6d4c 6179 6f75 742e 4669 656c  QFormLayout.Fiel
-00007040: 6452 6f6c 652c 2073 656c 662e 636f 6d62  dRole, self.comb
-00007050: 6f42 6f78 5f72 6573 756c 7473 5f73 656c  oBox_results_sel
-00007060: 6563 7469 6f6e 5f73 7461 7469 6f6e 290a  ection_station).
-00007070: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
-00007080: 656c 5f35 203d 2051 7457 6964 6765 7473  el_5 = QtWidgets
-00007090: 2e51 4c61 6265 6c28 7365 6c66 2e67 726f  .QLabel(self.gro
-000070a0: 7570 426f 785f 7265 7375 6c74 735f 6461  upBox_results_da
-000070b0: 7461 5f73 656c 6563 7469 6f6e 290a 2020  ta_selection).  
-000070c0: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
-000070d0: 5f35 2e73 6574 4f62 6a65 6374 4e61 6d65  _5.setObjectName
-000070e0: 2822 6c61 6265 6c5f 3522 290a 2020 2020  ("label_5").    
-000070f0: 2020 2020 7365 6c66 2e66 6f72 6d4c 6179      self.formLay
-00007100: 6f75 742e 7365 7457 6964 6765 7428 312c  out.setWidget(1,
-00007110: 2051 7457 6964 6765 7473 2e51 466f 726d   QtWidgets.QForm
-00007120: 4c61 796f 7574 2e4c 6162 656c 526f 6c65  Layout.LabelRole
-00007130: 2c20 7365 6c66 2e6c 6162 656c 5f35 290a  , self.label_5).
-00007140: 2020 2020 2020 2020 7365 6c66 2e63 6f6d          self.com
-00007150: 626f 426f 785f 7265 7375 6c74 735f 7365  boBox_results_se
-00007160: 6c65 6374 696f 6e5f 7375 7276 6579 203d  lection_survey =
-00007170: 2051 7457 6964 6765 7473 2e51 436f 6d62   QtWidgets.QComb
-00007180: 6f42 6f78 2873 656c 662e 6772 6f75 7042  oBox(self.groupB
-00007190: 6f78 5f72 6573 756c 7473 5f64 6174 615f  ox_results_data_
-000071a0: 7365 6c65 6374 696f 6e29 0a20 2020 2020  selection).     
-000071b0: 2020 2073 656c 662e 636f 6d62 6f42 6f78     self.comboBox
-000071c0: 5f72 6573 756c 7473 5f73 656c 6563 7469  _results_selecti
-000071d0: 6f6e 5f73 7572 7665 792e 7365 744f 626a  on_survey.setObj
-000071e0: 6563 744e 616d 6528 2263 6f6d 626f 426f  ectName("comboBo
-000071f0: 785f 7265 7375 6c74 735f 7365 6c65 6374  x_results_select
-00007200: 696f 6e5f 7375 7276 6579 2229 0a20 2020  ion_survey").   
-00007210: 2020 2020 2073 656c 662e 636f 6d62 6f42       self.comboB
-00007220: 6f78 5f72 6573 756c 7473 5f73 656c 6563  ox_results_selec
-00007230: 7469 6f6e 5f73 7572 7665 792e 6164 6449  tion_survey.addI
-00007240: 7465 6d28 2222 290a 2020 2020 2020 2020  tem("").        
-00007250: 7365 6c66 2e66 6f72 6d4c 6179 6f75 742e  self.formLayout.
-00007260: 7365 7457 6964 6765 7428 312c 2051 7457  setWidget(1, QtW
-00007270: 6964 6765 7473 2e51 466f 726d 4c61 796f  idgets.QFormLayo
-00007280: 7574 2e46 6965 6c64 526f 6c65 2c20 7365  ut.FieldRole, se
-00007290: 6c66 2e63 6f6d 626f 426f 785f 7265 7375  lf.comboBox_resu
-000072a0: 6c74 735f 7365 6c65 6374 696f 6e5f 7375  lts_selection_su
-000072b0: 7276 6579 290a 2020 2020 2020 2020 7365  rvey).        se
-000072c0: 6c66 2e76 6572 7469 6361 6c4c 6179 6f75  lf.verticalLayou
-000072d0: 745f 3137 2e61 6464 4c61 796f 7574 2873  t_17.addLayout(s
-000072e0: 656c 662e 666f 726d 4c61 796f 7574 290a  elf.formLayout).
-000072f0: 2020 2020 2020 2020 7365 6c66 2e76 6572          self.ver
-00007300: 7469 6361 6c4c 6179 6f75 745f 3132 2e61  ticalLayout_12.a
-00007310: 6464 5769 6467 6574 2873 656c 662e 6772  ddWidget(self.gr
-00007320: 6f75 7042 6f78 5f72 6573 756c 7473 5f64  oupBox_results_d
-00007330: 6174 615f 7365 6c65 6374 696f 6e29 0a20  ata_selection). 
-00007340: 2020 2020 2020 2073 656c 662e 6772 6f75         self.grou
-00007350: 7042 6f78 5f67 6973 5f64 6174 6120 3d20  pBox_gis_data = 
-00007360: 5174 5769 6467 6574 732e 5147 726f 7570  QtWidgets.QGroup
-00007370: 426f 7828 7365 6c66 2e76 6572 7469 6361  Box(self.vertica
-00007380: 6c4c 6179 6f75 7457 6964 6765 7429 0a20  lLayoutWidget). 
-00007390: 2020 2020 2020 2073 656c 662e 6772 6f75         self.grou
-000073a0: 7042 6f78 5f67 6973 5f64 6174 612e 7365  pBox_gis_data.se
-000073b0: 744f 626a 6563 744e 616d 6528 2267 726f  tObjectName("gro
-000073c0: 7570 426f 785f 6769 735f 6461 7461 2229  upBox_gis_data")
-000073d0: 0a20 2020 2020 2020 2073 656c 662e 7665  .        self.ve
-000073e0: 7274 6963 616c 4c61 796f 7574 5f33 3620  rticalLayout_36 
-000073f0: 3d20 5174 5769 6467 6574 732e 5156 426f  = QtWidgets.QVBo
-00007400: 784c 6179 6f75 7428 7365 6c66 2e67 726f  xLayout(self.gro
-00007410: 7570 426f 785f 6769 735f 6461 7461 290a  upBox_gis_data).
-00007420: 2020 2020 2020 2020 7365 6c66 2e76 6572          self.ver
-00007430: 7469 6361 6c4c 6179 6f75 745f 3336 2e73  ticalLayout_36.s
-00007440: 6574 4f62 6a65 6374 4e61 6d65 2822 7665  etObjectName("ve
-00007450: 7274 6963 616c 4c61 796f 7574 5f33 3622  rticalLayout_36"
-00007460: 290a 2020 2020 2020 2020 7365 6c66 2e70  ).        self.p
-00007470: 7573 6842 7574 746f 6e5f 7265 7375 6c74  ushButton_result
-00007480: 735f 6578 706f 7274 5f73 6861 7065 6669  s_export_shapefi
-00007490: 6c65 203d 2051 7457 6964 6765 7473 2e51  le = QtWidgets.Q
-000074a0: 5075 7368 4275 7474 6f6e 2873 656c 662e  PushButton(self.
-000074b0: 6772 6f75 7042 6f78 5f67 6973 5f64 6174  groupBox_gis_dat
-000074c0: 6129 0a20 2020 2020 2020 2073 656c 662e  a).        self.
-000074d0: 7075 7368 4275 7474 6f6e 5f72 6573 756c  pushButton_resul
-000074e0: 7473 5f65 7870 6f72 745f 7368 6170 6566  ts_export_shapef
-000074f0: 696c 652e 7365 744f 626a 6563 744e 616d  ile.setObjectNam
-00007500: 6528 2270 7573 6842 7574 746f 6e5f 7265  e("pushButton_re
-00007510: 7375 6c74 735f 6578 706f 7274 5f73 6861  sults_export_sha
-00007520: 7065 6669 6c65 2229 0a20 2020 2020 2020  pefile").       
-00007530: 2073 656c 662e 7665 7274 6963 616c 4c61   self.verticalLa
-00007540: 796f 7574 5f33 362e 6164 6457 6964 6765  yout_36.addWidge
-00007550: 7428 7365 6c66 2e70 7573 6842 7574 746f  t(self.pushButto
-00007560: 6e5f 7265 7375 6c74 735f 6578 706f 7274  n_results_export
-00007570: 5f73 6861 7065 6669 6c65 290a 2020 2020  _shapefile).    
-00007580: 2020 2020 7365 6c66 2e66 6f72 6d4c 6179      self.formLay
-00007590: 6f75 745f 3720 3d20 5174 5769 6467 6574  out_7 = QtWidget
-000075a0: 732e 5146 6f72 6d4c 6179 6f75 7428 290a  s.QFormLayout().
-000075b0: 2020 2020 2020 2020 7365 6c66 2e66 6f72          self.for
-000075c0: 6d4c 6179 6f75 745f 372e 7365 744f 626a  mLayout_7.setObj
-000075d0: 6563 744e 616d 6528 2266 6f72 6d4c 6179  ectName("formLay
-000075e0: 6f75 745f 3722 290a 2020 2020 2020 2020  out_7").        
-000075f0: 7365 6c66 2e76 6572 7469 6361 6c4c 6179  self.verticalLay
-00007600: 6f75 745f 3336 2e61 6464 4c61 796f 7574  out_36.addLayout
-00007610: 2873 656c 662e 666f 726d 4c61 796f 7574  (self.formLayout
-00007620: 5f37 290a 2020 2020 2020 2020 7365 6c66  _7).        self
-00007630: 2e76 6572 7469 6361 6c4c 6179 6f75 745f  .verticalLayout_
-00007640: 3132 2e61 6464 5769 6467 6574 2873 656c  12.addWidget(sel
-00007650: 662e 6772 6f75 7042 6f78 5f67 6973 5f64  f.groupBox_gis_d
-00007660: 6174 6129 0a20 2020 2020 2020 2073 7061  ata).        spa
-00007670: 6365 7249 7465 6d31 203d 2051 7457 6964  cerItem1 = QtWid
-00007680: 6765 7473 2e51 5370 6163 6572 4974 656d  gets.QSpacerItem
-00007690: 2832 302c 2034 302c 2051 7457 6964 6765  (20, 40, QtWidge
-000076a0: 7473 2e51 5369 7a65 506f 6c69 6379 2e4d  ts.QSizePolicy.M
-000076b0: 696e 696d 756d 2c20 5174 5769 6467 6574  inimum, QtWidget
-000076c0: 732e 5153 697a 6550 6f6c 6963 792e 4578  s.QSizePolicy.Ex
-000076d0: 7061 6e64 696e 6729 0a20 2020 2020 2020  panding).       
-000076e0: 2073 656c 662e 7665 7274 6963 616c 4c61   self.verticalLa
-000076f0: 796f 7574 5f31 322e 6164 6449 7465 6d28  yout_12.addItem(
-00007700: 7370 6163 6572 4974 656d 3129 0a20 2020  spacerItem1).   
-00007710: 2020 2020 2073 656c 662e 7461 6257 6964       self.tabWid
-00007720: 6765 745f 7265 7375 6c74 7320 3d20 5174  get_results = Qt
-00007730: 5769 6467 6574 732e 5154 6162 5769 6467  Widgets.QTabWidg
-00007740: 6574 2873 656c 662e 7370 6c69 7474 6572  et(self.splitter
-00007750: 5f72 6573 756c 7473 290a 2020 2020 2020  _results).      
-00007760: 2020 7369 7a65 506f 6c69 6379 203d 2051    sizePolicy = Q
-00007770: 7457 6964 6765 7473 2e51 5369 7a65 506f  tWidgets.QSizePo
-00007780: 6c69 6379 2851 7457 6964 6765 7473 2e51  licy(QtWidgets.Q
-00007790: 5369 7a65 506f 6c69 6379 2e45 7870 616e  SizePolicy.Expan
-000077a0: 6469 6e67 2c20 5174 5769 6467 6574 732e  ding, QtWidgets.
-000077b0: 5153 697a 6550 6f6c 6963 792e 4578 7061  QSizePolicy.Expa
-000077c0: 6e64 696e 6729 0a20 2020 2020 2020 2073  nding).        s
-000077d0: 697a 6550 6f6c 6963 792e 7365 7448 6f72  izePolicy.setHor
-000077e0: 697a 6f6e 7461 6c53 7472 6574 6368 2831  izontalStretch(1
-000077f0: 290a 2020 2020 2020 2020 7369 7a65 506f  ).        sizePo
-00007800: 6c69 6379 2e73 6574 5665 7274 6963 616c  licy.setVertical
-00007810: 5374 7265 7463 6828 3029 0a20 2020 2020  Stretch(0).     
-00007820: 2020 2073 697a 6550 6f6c 6963 792e 7365     sizePolicy.se
-00007830: 7448 6569 6768 7446 6f72 5769 6474 6828  tHeightForWidth(
-00007840: 7365 6c66 2e74 6162 5769 6467 6574 5f72  self.tabWidget_r
-00007850: 6573 756c 7473 2e73 697a 6550 6f6c 6963  esults.sizePolic
-00007860: 7928 292e 6861 7348 6569 6768 7446 6f72  y().hasHeightFor
-00007870: 5769 6474 6828 2929 0a20 2020 2020 2020  Width()).       
-00007880: 2073 656c 662e 7461 6257 6964 6765 745f   self.tabWidget_
-00007890: 7265 7375 6c74 732e 7365 7453 697a 6550  results.setSizeP
-000078a0: 6f6c 6963 7928 7369 7a65 506f 6c69 6379  olicy(sizePolicy
-000078b0: 290a 2020 2020 2020 2020 7365 6c66 2e74  ).        self.t
-000078c0: 6162 5769 6467 6574 5f72 6573 756c 7473  abWidget_results
+00006000: 3229 0a20 2020 2020 2020 2073 656c 662e  2).        self.
+00006010: 6c61 6265 6c5f 6f62 735f 7365 7475 7073  label_obs_setups
+00006020: 5f72 6566 5f68 6569 6768 7420 3d20 5174  _ref_height = Qt
+00006030: 5769 6467 6574 732e 514c 6162 656c 2873  Widgets.QLabel(s
+00006040: 656c 662e 6772 6f75 7042 6f78 5f6f 6273  elf.groupBox_obs
+00006050: 5f73 6574 7570 735f 6170 706c 6965 645f  _setups_applied_
+00006060: 636f 7272 6563 7469 6f6e 7329 0a20 2020  corrections).   
+00006070: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
+00006080: 6f62 735f 7365 7475 7073 5f72 6566 5f68  obs_setups_ref_h
+00006090: 6569 6768 742e 7365 7454 6578 7428 2222  eight.setText(""
+000060a0: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
+000060b0: 6162 656c 5f6f 6273 5f73 6574 7570 735f  abel_obs_setups_
+000060c0: 7265 665f 6865 6967 6874 2e73 6574 4f62  ref_height.setOb
+000060d0: 6a65 6374 4e61 6d65 2822 6c61 6265 6c5f  jectName("label_
+000060e0: 6f62 735f 7365 7475 7073 5f72 6566 5f68  obs_setups_ref_h
+000060f0: 6569 6768 7422 290a 2020 2020 2020 2020  eight").        
+00006100: 7365 6c66 2e66 6f72 6d4c 6179 6f75 745f  self.formLayout_
+00006110: 362e 7365 7457 6964 6765 7428 312c 2051  6.setWidget(1, Q
+00006120: 7457 6964 6765 7473 2e51 466f 726d 4c61  tWidgets.QFormLa
+00006130: 796f 7574 2e46 6965 6c64 526f 6c65 2c20  yout.FieldRole, 
+00006140: 7365 6c66 2e6c 6162 656c 5f6f 6273 5f73  self.label_obs_s
+00006150: 6574 7570 735f 7265 665f 6865 6967 6874  etups_ref_height
+00006160: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
+00006170: 6162 656c 5f32 3720 3d20 5174 5769 6467  abel_27 = QtWidg
+00006180: 6574 732e 514c 6162 656c 2873 656c 662e  ets.QLabel(self.
+00006190: 6772 6f75 7042 6f78 5f6f 6273 5f73 6574  groupBox_obs_set
+000061a0: 7570 735f 6170 706c 6965 645f 636f 7272  ups_applied_corr
+000061b0: 6563 7469 6f6e 7329 0a20 2020 2020 2020  ections).       
+000061c0: 2073 656c 662e 6c61 6265 6c5f 3237 2e73   self.label_27.s
+000061d0: 6574 4f62 6a65 6374 4e61 6d65 2822 6c61  etObjectName("la
+000061e0: 6265 6c5f 3237 2229 0a20 2020 2020 2020  bel_27").       
+000061f0: 2073 656c 662e 666f 726d 4c61 796f 7574   self.formLayout
+00006200: 5f36 2e73 6574 5769 6467 6574 2832 2c20  _6.setWidget(2, 
+00006210: 5174 5769 6467 6574 732e 5146 6f72 6d4c  QtWidgets.QFormL
+00006220: 6179 6f75 742e 4c61 6265 6c52 6f6c 652c  ayout.LabelRole,
+00006230: 2073 656c 662e 6c61 6265 6c5f 3237 290a   self.label_27).
+00006240: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
+00006250: 656c 5f6f 6273 5f73 6574 7570 735f 3320  el_obs_setups_3 
+00006260: 3d20 5174 5769 6467 6574 732e 514c 6162  = QtWidgets.QLab
+00006270: 656c 2873 656c 662e 6772 6f75 7042 6f78  el(self.groupBox
+00006280: 5f6f 6273 5f73 6574 7570 735f 6170 706c  _obs_setups_appl
+00006290: 6965 645f 636f 7272 6563 7469 6f6e 7329  ied_corrections)
+000062a0: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
+000062b0: 6265 6c5f 6f62 735f 7365 7475 7073 5f33  bel_obs_setups_3
+000062c0: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
+000062d0: 6c61 6265 6c5f 6f62 735f 7365 7475 7073  label_obs_setups
+000062e0: 5f33 2229 0a20 2020 2020 2020 2073 656c  _3").        sel
+000062f0: 662e 666f 726d 4c61 796f 7574 5f36 2e73  f.formLayout_6.s
+00006300: 6574 5769 6467 6574 2833 2c20 5174 5769  etWidget(3, QtWi
+00006310: 6467 6574 732e 5146 6f72 6d4c 6179 6f75  dgets.QFormLayou
+00006320: 742e 4c61 6265 6c52 6f6c 652c 2073 656c  t.LabelRole, sel
+00006330: 662e 6c61 6265 6c5f 6f62 735f 7365 7475  f.label_obs_setu
+00006340: 7073 5f33 290a 2020 2020 2020 2020 7365  ps_3).        se
+00006350: 6c66 2e6c 6162 656c 5f6f 6273 5f73 6574  lf.label_obs_set
+00006360: 7570 735f 6174 6d5f 7072 6573 5f63 6f72  ups_atm_pres_cor
+00006370: 7220 3d20 5174 5769 6467 6574 732e 514c  r = QtWidgets.QL
+00006380: 6162 656c 2873 656c 662e 6772 6f75 7042  abel(self.groupB
+00006390: 6f78 5f6f 6273 5f73 6574 7570 735f 6170  ox_obs_setups_ap
+000063a0: 706c 6965 645f 636f 7272 6563 7469 6f6e  plied_correction
+000063b0: 7329 0a20 2020 2020 2020 2073 656c 662e  s).        self.
+000063c0: 6c61 6265 6c5f 6f62 735f 7365 7475 7073  label_obs_setups
+000063d0: 5f61 746d 5f70 7265 735f 636f 7272 2e73  _atm_pres_corr.s
+000063e0: 6574 5465 7874 2822 2229 0a20 2020 2020  etText("").     
+000063f0: 2020 2073 656c 662e 6c61 6265 6c5f 6f62     self.label_ob
+00006400: 735f 7365 7475 7073 5f61 746d 5f70 7265  s_setups_atm_pre
+00006410: 735f 636f 7272 2e73 6574 4f62 6a65 6374  s_corr.setObject
+00006420: 4e61 6d65 2822 6c61 6265 6c5f 6f62 735f  Name("label_obs_
+00006430: 7365 7475 7073 5f61 746d 5f70 7265 735f  setups_atm_pres_
+00006440: 636f 7272 2229 0a20 2020 2020 2020 2073  corr").        s
+00006450: 656c 662e 666f 726d 4c61 796f 7574 5f36  elf.formLayout_6
+00006460: 2e73 6574 5769 6467 6574 2833 2c20 5174  .setWidget(3, Qt
+00006470: 5769 6467 6574 732e 5146 6f72 6d4c 6179  Widgets.QFormLay
+00006480: 6f75 742e 4669 656c 6452 6f6c 652c 2073  out.FieldRole, s
+00006490: 656c 662e 6c61 6265 6c5f 6f62 735f 7365  elf.label_obs_se
+000064a0: 7475 7073 5f61 746d 5f70 7265 735f 636f  tups_atm_pres_co
+000064b0: 7272 290a 2020 2020 2020 2020 7365 6c66  rr).        self
+000064c0: 2e6c 6162 656c 5f6f 6273 5f73 6574 7570  .label_obs_setup
+000064d0: 735f 7363 616c 655f 636f 7272 203d 2051  s_scale_corr = Q
+000064e0: 7457 6964 6765 7473 2e51 4c61 6265 6c28  tWidgets.QLabel(
+000064f0: 7365 6c66 2e67 726f 7570 426f 785f 6f62  self.groupBox_ob
+00006500: 735f 7365 7475 7073 5f61 7070 6c69 6564  s_setups_applied
+00006510: 5f63 6f72 7265 6374 696f 6e73 290a 2020  _corrections).  
+00006520: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
+00006530: 5f6f 6273 5f73 6574 7570 735f 7363 616c  _obs_setups_scal
+00006540: 655f 636f 7272 2e73 6574 5465 7874 2822  e_corr.setText("
+00006550: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00006560: 6c61 6265 6c5f 6f62 735f 7365 7475 7073  label_obs_setups
+00006570: 5f73 6361 6c65 5f63 6f72 722e 7365 744f  _scale_corr.setO
+00006580: 626a 6563 744e 616d 6528 226c 6162 656c  bjectName("label
+00006590: 5f6f 6273 5f73 6574 7570 735f 7363 616c  _obs_setups_scal
+000065a0: 655f 636f 7272 2229 0a20 2020 2020 2020  e_corr").       
+000065b0: 2073 656c 662e 666f 726d 4c61 796f 7574   self.formLayout
+000065c0: 5f36 2e73 6574 5769 6467 6574 2832 2c20  _6.setWidget(2, 
+000065d0: 5174 5769 6467 6574 732e 5146 6f72 6d4c  QtWidgets.QFormL
+000065e0: 6179 6f75 742e 4669 656c 6452 6f6c 652c  ayout.FieldRole,
+000065f0: 2073 656c 662e 6c61 6265 6c5f 6f62 735f   self.label_obs_
+00006600: 7365 7475 7073 5f73 6361 6c65 5f63 6f72  setups_scale_cor
+00006610: 7229 0a20 2020 2020 2020 2073 656c 662e  r).        self.
+00006620: 7665 7274 6963 616c 4c61 796f 7574 5f31  verticalLayout_1
+00006630: 312e 6164 6457 6964 6765 7428 7365 6c66  1.addWidget(self
+00006640: 2e67 726f 7570 426f 785f 6f62 735f 7365  .groupBox_obs_se
+00006650: 7475 7073 5f61 7070 6c69 6564 5f63 6f72  tups_applied_cor
+00006660: 7265 6374 696f 6e73 290a 2020 2020 2020  rections).      
+00006670: 2020 7365 6c66 2e74 6162 5769 6467 6574    self.tabWidget
+00006680: 5f6f 6273 6572 7661 7469 6f6e 732e 6164  _observations.ad
+00006690: 6454 6162 2873 656c 662e 7461 625f 6f62  dTab(self.tab_ob
+000066a0: 7365 7276 6174 696f 6e73 5f73 6574 7570  servations_setup
+000066b0: 732c 2022 2229 0a20 2020 2020 2020 2073  s, "").        s
+000066c0: 656c 662e 7665 7274 6963 616c 4c61 796f  elf.verticalLayo
+000066d0: 7574 5f37 2e61 6464 5769 6467 6574 2873  ut_7.addWidget(s
+000066e0: 656c 662e 7370 6c69 7474 6572 5f6f 6273  elf.splitter_obs
+000066f0: 290a 2020 2020 2020 2020 7365 6c66 2e74  ).        self.t
+00006700: 6162 5769 6467 6574 5f4d 6169 6e2e 6164  abWidget_Main.ad
+00006710: 6454 6162 2873 656c 662e 7461 625f 6d61  dTab(self.tab_ma
+00006720: 696e 5f6f 6273 6572 7661 7469 6f6e 732c  in_observations,
+00006730: 2022 2229 0a20 2020 2020 2020 2073 656c   "").        sel
+00006740: 662e 7461 625f 6d61 696e 5f72 6573 756c  f.tab_main_resul
+00006750: 7473 203d 2051 7457 6964 6765 7473 2e51  ts = QtWidgets.Q
+00006760: 5769 6467 6574 2829 0a20 2020 2020 2020  Widget().       
+00006770: 2073 656c 662e 7461 625f 6d61 696e 5f72   self.tab_main_r
+00006780: 6573 756c 7473 2e73 6574 546f 6f6c 5469  esults.setToolTi
+00006790: 7044 7572 6174 696f 6e28 3229 0a20 2020  pDuration(2).   
+000067a0: 2020 2020 2073 656c 662e 7461 625f 6d61       self.tab_ma
+000067b0: 696e 5f72 6573 756c 7473 2e73 6574 4f62  in_results.setOb
+000067c0: 6a65 6374 4e61 6d65 2822 7461 625f 6d61  jectName("tab_ma
+000067d0: 696e 5f72 6573 756c 7473 2229 0a20 2020  in_results").   
+000067e0: 2020 2020 2073 656c 662e 7665 7274 6963       self.vertic
+000067f0: 616c 4c61 796f 7574 5f31 3420 3d20 5174  alLayout_14 = Qt
+00006800: 5769 6467 6574 732e 5156 426f 784c 6179  Widgets.QVBoxLay
+00006810: 6f75 7428 7365 6c66 2e74 6162 5f6d 6169  out(self.tab_mai
+00006820: 6e5f 7265 7375 6c74 7329 0a20 2020 2020  n_results).     
+00006830: 2020 2073 656c 662e 7665 7274 6963 616c     self.vertical
+00006840: 4c61 796f 7574 5f31 342e 7365 744f 626a  Layout_14.setObj
+00006850: 6563 744e 616d 6528 2276 6572 7469 6361  ectName("vertica
+00006860: 6c4c 6179 6f75 745f 3134 2229 0a20 2020  lLayout_14").   
+00006870: 2020 2020 2073 656c 662e 7370 6c69 7474       self.splitt
+00006880: 6572 5f72 6573 756c 7473 203d 2051 7457  er_results = QtW
+00006890: 6964 6765 7473 2e51 5370 6c69 7474 6572  idgets.QSplitter
+000068a0: 2873 656c 662e 7461 625f 6d61 696e 5f72  (self.tab_main_r
+000068b0: 6573 756c 7473 290a 2020 2020 2020 2020  esults).        
+000068c0: 7365 6c66 2e73 706c 6974 7465 725f 7265  self.splitter_re
+000068d0: 7375 6c74 732e 7365 744f 7269 656e 7461  sults.setOrienta
+000068e0: 7469 6f6e 2851 7443 6f72 652e 5174 2e48  tion(QtCore.Qt.H
+000068f0: 6f72 697a 6f6e 7461 6c29 0a20 2020 2020  orizontal).     
+00006900: 2020 2073 656c 662e 7370 6c69 7474 6572     self.splitter
+00006910: 5f72 6573 756c 7473 2e73 6574 4f62 6a65  _results.setObje
+00006920: 6374 4e61 6d65 2822 7370 6c69 7474 6572  ctName("splitter
+00006930: 5f72 6573 756c 7473 2229 0a20 2020 2020  _results").     
+00006940: 2020 2073 656c 662e 7665 7274 6963 616c     self.vertical
+00006950: 4c61 796f 7574 5769 6467 6574 203d 2051  LayoutWidget = Q
+00006960: 7457 6964 6765 7473 2e51 5769 6467 6574  tWidgets.QWidget
+00006970: 2873 656c 662e 7370 6c69 7474 6572 5f72  (self.splitter_r
+00006980: 6573 756c 7473 290a 2020 2020 2020 2020  esults).        
+00006990: 7365 6c66 2e76 6572 7469 6361 6c4c 6179  self.verticalLay
+000069a0: 6f75 7457 6964 6765 742e 7365 744f 626a  outWidget.setObj
+000069b0: 6563 744e 616d 6528 2276 6572 7469 6361  ectName("vertica
+000069c0: 6c4c 6179 6f75 7457 6964 6765 7422 290a  lLayoutWidget").
+000069d0: 2020 2020 2020 2020 7365 6c66 2e76 6572          self.ver
+000069e0: 7469 6361 6c4c 6179 6f75 745f 3132 203d  ticalLayout_12 =
+000069f0: 2051 7457 6964 6765 7473 2e51 5642 6f78   QtWidgets.QVBox
+00006a00: 4c61 796f 7574 2873 656c 662e 7665 7274  Layout(self.vert
+00006a10: 6963 616c 4c61 796f 7574 5769 6467 6574  icalLayoutWidget
+00006a20: 290a 2020 2020 2020 2020 7365 6c66 2e76  ).        self.v
+00006a30: 6572 7469 6361 6c4c 6179 6f75 745f 3132  erticalLayout_12
+00006a40: 2e73 6574 436f 6e74 656e 7473 4d61 7267  .setContentsMarg
+00006a50: 696e 7328 302c 2030 2c20 302c 2030 290a  ins(0, 0, 0, 0).
+00006a60: 2020 2020 2020 2020 7365 6c66 2e76 6572          self.ver
+00006a70: 7469 6361 6c4c 6179 6f75 745f 3132 2e73  ticalLayout_12.s
+00006a80: 6574 4f62 6a65 6374 4e61 6d65 2822 7665  etObjectName("ve
+00006a90: 7274 6963 616c 4c61 796f 7574 5f31 3222  rticalLayout_12"
+00006aa0: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
+00006ab0: 726f 7570 426f 785f 7265 7375 6c74 735f  roupBox_results_
+00006ac0: 6c73 6d5f 7275 6e73 203d 2051 7457 6964  lsm_runs = QtWid
+00006ad0: 6765 7473 2e51 4772 6f75 7042 6f78 2873  gets.QGroupBox(s
+00006ae0: 656c 662e 7665 7274 6963 616c 4c61 796f  elf.verticalLayo
+00006af0: 7574 5769 6467 6574 290a 2020 2020 2020  utWidget).      
+00006b00: 2020 7365 6c66 2e67 726f 7570 426f 785f    self.groupBox_
+00006b10: 7265 7375 6c74 735f 6c73 6d5f 7275 6e73  results_lsm_runs
+00006b20: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
+00006b30: 6772 6f75 7042 6f78 5f72 6573 756c 7473  groupBox_results
+00006b40: 5f6c 736d 5f72 756e 7322 290a 2020 2020  _lsm_runs").    
+00006b50: 2020 2020 7365 6c66 2e76 6572 7469 6361      self.vertica
+00006b60: 6c4c 6179 6f75 745f 3136 203d 2051 7457  lLayout_16 = QtW
+00006b70: 6964 6765 7473 2e51 5642 6f78 4c61 796f  idgets.QVBoxLayo
+00006b80: 7574 2873 656c 662e 6772 6f75 7042 6f78  ut(self.groupBox
+00006b90: 5f72 6573 756c 7473 5f6c 736d 5f72 756e  _results_lsm_run
+00006ba0: 7329 0a20 2020 2020 2020 2073 656c 662e  s).        self.
+00006bb0: 7665 7274 6963 616c 4c61 796f 7574 5f31  verticalLayout_1
+00006bc0: 362e 7365 744f 626a 6563 744e 616d 6528  6.setObjectName(
+00006bd0: 2276 6572 7469 6361 6c4c 6179 6f75 745f  "verticalLayout_
+00006be0: 3136 2229 0a20 2020 2020 2020 2073 656c  16").        sel
+00006bf0: 662e 636f 6d62 6f42 6f78 5f72 6573 756c  f.comboBox_resul
+00006c00: 7473 5f6c 736d 5f72 756e 5f73 656c 6563  ts_lsm_run_selec
+00006c10: 7469 6f6e 203d 2051 7457 6964 6765 7473  tion = QtWidgets
+00006c20: 2e51 436f 6d62 6f42 6f78 2873 656c 662e  .QComboBox(self.
+00006c30: 6772 6f75 7042 6f78 5f72 6573 756c 7473  groupBox_results
+00006c40: 5f6c 736d 5f72 756e 7329 0a20 2020 2020  _lsm_runs).     
+00006c50: 2020 2073 656c 662e 636f 6d62 6f42 6f78     self.comboBox
+00006c60: 5f72 6573 756c 7473 5f6c 736d 5f72 756e  _results_lsm_run
+00006c70: 5f73 656c 6563 7469 6f6e 2e73 6574 4f62  _selection.setOb
+00006c80: 6a65 6374 4e61 6d65 2822 636f 6d62 6f42  jectName("comboB
+00006c90: 6f78 5f72 6573 756c 7473 5f6c 736d 5f72  ox_results_lsm_r
+00006ca0: 756e 5f73 656c 6563 7469 6f6e 2229 0a20  un_selection"). 
+00006cb0: 2020 2020 2020 2073 656c 662e 7665 7274         self.vert
+00006cc0: 6963 616c 4c61 796f 7574 5f31 362e 6164  icalLayout_16.ad
+00006cd0: 6457 6964 6765 7428 7365 6c66 2e63 6f6d  dWidget(self.com
+00006ce0: 626f 426f 785f 7265 7375 6c74 735f 6c73  boBox_results_ls
+00006cf0: 6d5f 7275 6e5f 7365 6c65 6374 696f 6e29  m_run_selection)
+00006d00: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
+00006d10: 6265 6c5f 7265 7375 6c74 735f 6c73 6d5f  bel_results_lsm_
+00006d20: 7275 6e5f 636f 6d6d 656e 745f 6469 7370  run_comment_disp
+00006d30: 6c61 7920 3d20 5174 5769 6467 6574 732e  lay = QtWidgets.
+00006d40: 514c 6162 656c 2873 656c 662e 6772 6f75  QLabel(self.grou
+00006d50: 7042 6f78 5f72 6573 756c 7473 5f6c 736d  pBox_results_lsm
+00006d60: 5f72 756e 7329 0a20 2020 2020 2020 2073  _runs).        s
+00006d70: 656c 662e 6c61 6265 6c5f 7265 7375 6c74  elf.label_result
+00006d80: 735f 6c73 6d5f 7275 6e5f 636f 6d6d 656e  s_lsm_run_commen
+00006d90: 745f 6469 7370 6c61 792e 7365 7454 6578  t_display.setTex
+00006da0: 7428 2222 290a 2020 2020 2020 2020 7365  t("").        se
+00006db0: 6c66 2e6c 6162 656c 5f72 6573 756c 7473  lf.label_results
+00006dc0: 5f6c 736d 5f72 756e 5f63 6f6d 6d65 6e74  _lsm_run_comment
+00006dd0: 5f64 6973 706c 6179 2e73 6574 4f62 6a65  _display.setObje
+00006de0: 6374 4e61 6d65 2822 6c61 6265 6c5f 7265  ctName("label_re
+00006df0: 7375 6c74 735f 6c73 6d5f 7275 6e5f 636f  sults_lsm_run_co
+00006e00: 6d6d 656e 745f 6469 7370 6c61 7922 290a  mment_display").
+00006e10: 2020 2020 2020 2020 7365 6c66 2e76 6572          self.ver
+00006e20: 7469 6361 6c4c 6179 6f75 745f 3136 2e61  ticalLayout_16.a
+00006e30: 6464 5769 6467 6574 2873 656c 662e 6c61  ddWidget(self.la
+00006e40: 6265 6c5f 7265 7375 6c74 735f 6c73 6d5f  bel_results_lsm_
+00006e50: 7275 6e5f 636f 6d6d 656e 745f 6469 7370  run_comment_disp
+00006e60: 6c61 7929 0a20 2020 2020 2020 2073 656c  lay).        sel
+00006e70: 662e 7075 7368 4275 7474 6f6e 5f72 6573  f.pushButton_res
+00006e80: 756c 7473 5f64 656c 6574 655f 6c73 6d5f  ults_delete_lsm_
+00006e90: 7275 6e20 3d20 5174 5769 6467 6574 732e  run = QtWidgets.
+00006ea0: 5150 7573 6842 7574 746f 6e28 7365 6c66  QPushButton(self
+00006eb0: 2e67 726f 7570 426f 785f 7265 7375 6c74  .groupBox_result
+00006ec0: 735f 6c73 6d5f 7275 6e73 290a 2020 2020  s_lsm_runs).    
+00006ed0: 2020 2020 7365 6c66 2e70 7573 6842 7574      self.pushBut
+00006ee0: 746f 6e5f 7265 7375 6c74 735f 6465 6c65  ton_results_dele
+00006ef0: 7465 5f6c 736d 5f72 756e 2e73 6574 4f62  te_lsm_run.setOb
+00006f00: 6a65 6374 4e61 6d65 2822 7075 7368 4275  jectName("pushBu
+00006f10: 7474 6f6e 5f72 6573 756c 7473 5f64 656c  tton_results_del
+00006f20: 6574 655f 6c73 6d5f 7275 6e22 290a 2020  ete_lsm_run").  
+00006f30: 2020 2020 2020 7365 6c66 2e76 6572 7469        self.verti
+00006f40: 6361 6c4c 6179 6f75 745f 3136 2e61 6464  calLayout_16.add
+00006f50: 5769 6467 6574 2873 656c 662e 7075 7368  Widget(self.push
+00006f60: 4275 7474 6f6e 5f72 6573 756c 7473 5f64  Button_results_d
+00006f70: 656c 6574 655f 6c73 6d5f 7275 6e29 0a20  elete_lsm_run). 
+00006f80: 2020 2020 2020 2073 656c 662e 7075 7368         self.push
+00006f90: 4275 7474 6f6e 5f72 6573 756c 7473 5f64  Button_results_d
+00006fa0: 656c 6574 655f 616c 6c5f 6c73 6d5f 7275  elete_all_lsm_ru
+00006fb0: 6e73 203d 2051 7457 6964 6765 7473 2e51  ns = QtWidgets.Q
+00006fc0: 5075 7368 4275 7474 6f6e 2873 656c 662e  PushButton(self.
+00006fd0: 6772 6f75 7042 6f78 5f72 6573 756c 7473  groupBox_results
+00006fe0: 5f6c 736d 5f72 756e 7329 0a20 2020 2020  _lsm_runs).     
+00006ff0: 2020 2073 656c 662e 7075 7368 4275 7474     self.pushButt
+00007000: 6f6e 5f72 6573 756c 7473 5f64 656c 6574  on_results_delet
+00007010: 655f 616c 6c5f 6c73 6d5f 7275 6e73 2e73  e_all_lsm_runs.s
+00007020: 6574 4f62 6a65 6374 4e61 6d65 2822 7075  etObjectName("pu
+00007030: 7368 4275 7474 6f6e 5f72 6573 756c 7473  shButton_results
+00007040: 5f64 656c 6574 655f 616c 6c5f 6c73 6d5f  _delete_all_lsm_
+00007050: 7275 6e73 2229 0a20 2020 2020 2020 2073  runs").        s
+00007060: 656c 662e 7665 7274 6963 616c 4c61 796f  elf.verticalLayo
+00007070: 7574 5f31 362e 6164 6457 6964 6765 7428  ut_16.addWidget(
+00007080: 7365 6c66 2e70 7573 6842 7574 746f 6e5f  self.pushButton_
+00007090: 7265 7375 6c74 735f 6465 6c65 7465 5f61  results_delete_a
+000070a0: 6c6c 5f6c 736d 5f72 756e 7329 0a20 2020  ll_lsm_runs).   
+000070b0: 2020 2020 2073 656c 662e 7665 7274 6963       self.vertic
+000070c0: 616c 4c61 796f 7574 5f31 322e 6164 6457  alLayout_12.addW
+000070d0: 6964 6765 7428 7365 6c66 2e67 726f 7570  idget(self.group
+000070e0: 426f 785f 7265 7375 6c74 735f 6c73 6d5f  Box_results_lsm_
+000070f0: 7275 6e73 290a 2020 2020 2020 2020 7365  runs).        se
+00007100: 6c66 2e67 726f 7570 426f 785f 7265 7375  lf.groupBox_resu
+00007110: 6c74 735f 6461 7461 5f73 656c 6563 7469  lts_data_selecti
+00007120: 6f6e 203d 2051 7457 6964 6765 7473 2e51  on = QtWidgets.Q
+00007130: 4772 6f75 7042 6f78 2873 656c 662e 7665  GroupBox(self.ve
+00007140: 7274 6963 616c 4c61 796f 7574 5769 6467  rticalLayoutWidg
+00007150: 6574 290a 2020 2020 2020 2020 7365 6c66  et).        self
+00007160: 2e67 726f 7570 426f 785f 7265 7375 6c74  .groupBox_result
+00007170: 735f 6461 7461 5f73 656c 6563 7469 6f6e  s_data_selection
+00007180: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
+00007190: 6772 6f75 7042 6f78 5f72 6573 756c 7473  groupBox_results
+000071a0: 5f64 6174 615f 7365 6c65 6374 696f 6e22  _data_selection"
+000071b0: 290a 2020 2020 2020 2020 7365 6c66 2e76  ).        self.v
+000071c0: 6572 7469 6361 6c4c 6179 6f75 745f 3137  erticalLayout_17
+000071d0: 203d 2051 7457 6964 6765 7473 2e51 5642   = QtWidgets.QVB
+000071e0: 6f78 4c61 796f 7574 2873 656c 662e 6772  oxLayout(self.gr
+000071f0: 6f75 7042 6f78 5f72 6573 756c 7473 5f64  oupBox_results_d
+00007200: 6174 615f 7365 6c65 6374 696f 6e29 0a20  ata_selection). 
+00007210: 2020 2020 2020 2073 656c 662e 7665 7274         self.vert
+00007220: 6963 616c 4c61 796f 7574 5f31 372e 7365  icalLayout_17.se
+00007230: 744f 626a 6563 744e 616d 6528 2276 6572  tObjectName("ver
+00007240: 7469 6361 6c4c 6179 6f75 745f 3137 2229  ticalLayout_17")
+00007250: 0a20 2020 2020 2020 2073 656c 662e 666f  .        self.fo
+00007260: 726d 4c61 796f 7574 203d 2051 7457 6964  rmLayout = QtWid
+00007270: 6765 7473 2e51 466f 726d 4c61 796f 7574  gets.QFormLayout
+00007280: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+00007290: 666f 726d 4c61 796f 7574 2e73 6574 4f62  formLayout.setOb
+000072a0: 6a65 6374 4e61 6d65 2822 666f 726d 4c61  jectName("formLa
+000072b0: 796f 7574 2229 0a20 2020 2020 2020 2073  yout").        s
+000072c0: 656c 662e 6c61 6265 6c5f 3220 3d20 5174  elf.label_2 = Qt
+000072d0: 5769 6467 6574 732e 514c 6162 656c 2873  Widgets.QLabel(s
+000072e0: 656c 662e 6772 6f75 7042 6f78 5f72 6573  elf.groupBox_res
+000072f0: 756c 7473 5f64 6174 615f 7365 6c65 6374  ults_data_select
+00007300: 696f 6e29 0a20 2020 2020 2020 2073 656c  ion).        sel
+00007310: 662e 6c61 6265 6c5f 322e 7365 744f 626a  f.label_2.setObj
+00007320: 6563 744e 616d 6528 226c 6162 656c 5f32  ectName("label_2
+00007330: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00007340: 666f 726d 4c61 796f 7574 2e73 6574 5769  formLayout.setWi
+00007350: 6467 6574 2830 2c20 5174 5769 6467 6574  dget(0, QtWidget
+00007360: 732e 5146 6f72 6d4c 6179 6f75 742e 4c61  s.QFormLayout.La
+00007370: 6265 6c52 6f6c 652c 2073 656c 662e 6c61  belRole, self.la
+00007380: 6265 6c5f 3229 0a20 2020 2020 2020 2073  bel_2).        s
+00007390: 656c 662e 636f 6d62 6f42 6f78 5f72 6573  elf.comboBox_res
+000073a0: 756c 7473 5f73 656c 6563 7469 6f6e 5f73  ults_selection_s
+000073b0: 7461 7469 6f6e 203d 2051 7457 6964 6765  tation = QtWidge
+000073c0: 7473 2e51 436f 6d62 6f42 6f78 2873 656c  ts.QComboBox(sel
+000073d0: 662e 6772 6f75 7042 6f78 5f72 6573 756c  f.groupBox_resul
+000073e0: 7473 5f64 6174 615f 7365 6c65 6374 696f  ts_data_selectio
+000073f0: 6e29 0a20 2020 2020 2020 2073 656c 662e  n).        self.
+00007400: 636f 6d62 6f42 6f78 5f72 6573 756c 7473  comboBox_results
+00007410: 5f73 656c 6563 7469 6f6e 5f73 7461 7469  _selection_stati
+00007420: 6f6e 2e73 6574 4f62 6a65 6374 4e61 6d65  on.setObjectName
+00007430: 2822 636f 6d62 6f42 6f78 5f72 6573 756c  ("comboBox_resul
+00007440: 7473 5f73 656c 6563 7469 6f6e 5f73 7461  ts_selection_sta
+00007450: 7469 6f6e 2229 0a20 2020 2020 2020 2073  tion").        s
+00007460: 656c 662e 636f 6d62 6f42 6f78 5f72 6573  elf.comboBox_res
+00007470: 756c 7473 5f73 656c 6563 7469 6f6e 5f73  ults_selection_s
+00007480: 7461 7469 6f6e 2e61 6464 4974 656d 2822  tation.addItem("
+00007490: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+000074a0: 666f 726d 4c61 796f 7574 2e73 6574 5769  formLayout.setWi
+000074b0: 6467 6574 2830 2c20 5174 5769 6467 6574  dget(0, QtWidget
+000074c0: 732e 5146 6f72 6d4c 6179 6f75 742e 4669  s.QFormLayout.Fi
+000074d0: 656c 6452 6f6c 652c 2073 656c 662e 636f  eldRole, self.co
+000074e0: 6d62 6f42 6f78 5f72 6573 756c 7473 5f73  mboBox_results_s
+000074f0: 656c 6563 7469 6f6e 5f73 7461 7469 6f6e  election_station
+00007500: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
+00007510: 6162 656c 5f35 203d 2051 7457 6964 6765  abel_5 = QtWidge
+00007520: 7473 2e51 4c61 6265 6c28 7365 6c66 2e67  ts.QLabel(self.g
+00007530: 726f 7570 426f 785f 7265 7375 6c74 735f  roupBox_results_
+00007540: 6461 7461 5f73 656c 6563 7469 6f6e 290a  data_selection).
+00007550: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
+00007560: 656c 5f35 2e73 6574 4f62 6a65 6374 4e61  el_5.setObjectNa
+00007570: 6d65 2822 6c61 6265 6c5f 3522 290a 2020  me("label_5").  
+00007580: 2020 2020 2020 7365 6c66 2e66 6f72 6d4c        self.formL
+00007590: 6179 6f75 742e 7365 7457 6964 6765 7428  ayout.setWidget(
+000075a0: 312c 2051 7457 6964 6765 7473 2e51 466f  1, QtWidgets.QFo
+000075b0: 726d 4c61 796f 7574 2e4c 6162 656c 526f  rmLayout.LabelRo
+000075c0: 6c65 2c20 7365 6c66 2e6c 6162 656c 5f35  le, self.label_5
+000075d0: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+000075e0: 6f6d 626f 426f 785f 7265 7375 6c74 735f  omboBox_results_
+000075f0: 7365 6c65 6374 696f 6e5f 7375 7276 6579  selection_survey
+00007600: 203d 2051 7457 6964 6765 7473 2e51 436f   = QtWidgets.QCo
+00007610: 6d62 6f42 6f78 2873 656c 662e 6772 6f75  mboBox(self.grou
+00007620: 7042 6f78 5f72 6573 756c 7473 5f64 6174  pBox_results_dat
+00007630: 615f 7365 6c65 6374 696f 6e29 0a20 2020  a_selection).   
+00007640: 2020 2020 2073 656c 662e 636f 6d62 6f42       self.comboB
+00007650: 6f78 5f72 6573 756c 7473 5f73 656c 6563  ox_results_selec
+00007660: 7469 6f6e 5f73 7572 7665 792e 7365 744f  tion_survey.setO
+00007670: 626a 6563 744e 616d 6528 2263 6f6d 626f  bjectName("combo
+00007680: 426f 785f 7265 7375 6c74 735f 7365 6c65  Box_results_sele
+00007690: 6374 696f 6e5f 7375 7276 6579 2229 0a20  ction_survey"). 
+000076a0: 2020 2020 2020 2073 656c 662e 636f 6d62         self.comb
+000076b0: 6f42 6f78 5f72 6573 756c 7473 5f73 656c  oBox_results_sel
+000076c0: 6563 7469 6f6e 5f73 7572 7665 792e 6164  ection_survey.ad
+000076d0: 6449 7465 6d28 2222 290a 2020 2020 2020  dItem("").      
+000076e0: 2020 7365 6c66 2e66 6f72 6d4c 6179 6f75    self.formLayou
+000076f0: 742e 7365 7457 6964 6765 7428 312c 2051  t.setWidget(1, Q
+00007700: 7457 6964 6765 7473 2e51 466f 726d 4c61  tWidgets.QFormLa
+00007710: 796f 7574 2e46 6965 6c64 526f 6c65 2c20  yout.FieldRole, 
+00007720: 7365 6c66 2e63 6f6d 626f 426f 785f 7265  self.comboBox_re
+00007730: 7375 6c74 735f 7365 6c65 6374 696f 6e5f  sults_selection_
+00007740: 7375 7276 6579 290a 2020 2020 2020 2020  survey).        
+00007750: 7365 6c66 2e76 6572 7469 6361 6c4c 6179  self.verticalLay
+00007760: 6f75 745f 3137 2e61 6464 4c61 796f 7574  out_17.addLayout
+00007770: 2873 656c 662e 666f 726d 4c61 796f 7574  (self.formLayout
+00007780: 290a 2020 2020 2020 2020 7365 6c66 2e76  ).        self.v
+00007790: 6572 7469 6361 6c4c 6179 6f75 745f 3132  erticalLayout_12
+000077a0: 2e61 6464 5769 6467 6574 2873 656c 662e  .addWidget(self.
+000077b0: 6772 6f75 7042 6f78 5f72 6573 756c 7473  groupBox_results
+000077c0: 5f64 6174 615f 7365 6c65 6374 696f 6e29  _data_selection)
+000077d0: 0a20 2020 2020 2020 2073 656c 662e 6772  .        self.gr
+000077e0: 6f75 7042 6f78 5f67 6973 5f64 6174 6120  oupBox_gis_data 
+000077f0: 3d20 5174 5769 6467 6574 732e 5147 726f  = QtWidgets.QGro
+00007800: 7570 426f 7828 7365 6c66 2e76 6572 7469  upBox(self.verti
+00007810: 6361 6c4c 6179 6f75 7457 6964 6765 7429  calLayoutWidget)
+00007820: 0a20 2020 2020 2020 2073 656c 662e 6772  .        self.gr
+00007830: 6f75 7042 6f78 5f67 6973 5f64 6174 612e  oupBox_gis_data.
+00007840: 7365 744f 626a 6563 744e 616d 6528 2267  setObjectName("g
+00007850: 726f 7570 426f 785f 6769 735f 6461 7461  roupBox_gis_data
+00007860: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00007870: 7665 7274 6963 616c 4c61 796f 7574 5f33  verticalLayout_3
+00007880: 3620 3d20 5174 5769 6467 6574 732e 5156  6 = QtWidgets.QV
+00007890: 426f 784c 6179 6f75 7428 7365 6c66 2e67  BoxLayout(self.g
+000078a0: 726f 7570 426f 785f 6769 735f 6461 7461  roupBox_gis_data
+000078b0: 290a 2020 2020 2020 2020 7365 6c66 2e76  ).        self.v
+000078c0: 6572 7469 6361 6c4c 6179 6f75 745f 3336  erticalLayout_36
 000078d0: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
-000078e0: 7461 6257 6964 6765 745f 7265 7375 6c74  tabWidget_result
-000078f0: 7322 290a 2020 2020 2020 2020 7365 6c66  s").        self
-00007900: 2e74 6162 5f72 6573 756c 7473 5f69 6e66  .tab_results_inf
-00007910: 6f20 3d20 5174 5769 6467 6574 732e 5157  o = QtWidgets.QW
-00007920: 6964 6765 7428 290a 2020 2020 2020 2020  idget().        
-00007930: 7365 6c66 2e74 6162 5f72 6573 756c 7473  self.tab_results
-00007940: 5f69 6e66 6f2e 7365 744f 626a 6563 744e  _info.setObjectN
-00007950: 616d 6528 2274 6162 5f72 6573 756c 7473  ame("tab_results
-00007960: 5f69 6e66 6f22 290a 2020 2020 2020 2020  _info").        
-00007970: 7365 6c66 2e76 6572 7469 6361 6c4c 6179  self.verticalLay
-00007980: 6f75 745f 3233 203d 2051 7457 6964 6765  out_23 = QtWidge
-00007990: 7473 2e51 5642 6f78 4c61 796f 7574 2873  ts.QVBoxLayout(s
-000079a0: 656c 662e 7461 625f 7265 7375 6c74 735f  elf.tab_results_
-000079b0: 696e 666f 290a 2020 2020 2020 2020 7365  info).        se
-000079c0: 6c66 2e76 6572 7469 6361 6c4c 6179 6f75  lf.verticalLayou
-000079d0: 745f 3233 2e73 6574 4f62 6a65 6374 4e61  t_23.setObjectNa
-000079e0: 6d65 2822 7665 7274 6963 616c 4c61 796f  me("verticalLayo
-000079f0: 7574 5f32 3322 290a 2020 2020 2020 2020  ut_23").        
-00007a00: 7365 6c66 2e76 6572 7469 6361 6c4c 6179  self.verticalLay
-00007a10: 6f75 745f 3232 203d 2051 7457 6964 6765  out_22 = QtWidge
-00007a20: 7473 2e51 5642 6f78 4c61 796f 7574 2829  ts.QVBoxLayout()
-00007a30: 0a20 2020 2020 2020 2073 656c 662e 7665  .        self.ve
-00007a40: 7274 6963 616c 4c61 796f 7574 5f32 322e  rticalLayout_22.
-00007a50: 7365 744f 626a 6563 744e 616d 6528 2276  setObjectName("v
-00007a60: 6572 7469 6361 6c4c 6179 6f75 745f 3232  erticalLayout_22
-00007a70: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00007a80: 6772 6f75 7042 6f78 5f72 6573 756c 7473  groupBox_results
-00007a90: 5f69 6e66 6f20 3d20 5174 5769 6467 6574  _info = QtWidget
-00007aa0: 732e 5147 726f 7570 426f 7828 7365 6c66  s.QGroupBox(self
-00007ab0: 2e74 6162 5f72 6573 756c 7473 5f69 6e66  .tab_results_inf
-00007ac0: 6f29 0a20 2020 2020 2020 2073 656c 662e  o).        self.
-00007ad0: 6772 6f75 7042 6f78 5f72 6573 756c 7473  groupBox_results
-00007ae0: 5f69 6e66 6f2e 7365 744f 626a 6563 744e  _info.setObjectN
-00007af0: 616d 6528 2267 726f 7570 426f 785f 7265  ame("groupBox_re
-00007b00: 7375 6c74 735f 696e 666f 2229 0a20 2020  sults_info").   
-00007b10: 2020 2020 2073 656c 662e 7665 7274 6963       self.vertic
-00007b20: 616c 4c61 796f 7574 5f32 3120 3d20 5174  alLayout_21 = Qt
-00007b30: 5769 6467 6574 732e 5156 426f 784c 6179  Widgets.QVBoxLay
-00007b40: 6f75 7428 7365 6c66 2e67 726f 7570 426f  out(self.groupBo
-00007b50: 785f 7265 7375 6c74 735f 696e 666f 290a  x_results_info).
-00007b60: 2020 2020 2020 2020 7365 6c66 2e76 6572          self.ver
-00007b70: 7469 6361 6c4c 6179 6f75 745f 3231 2e73  ticalLayout_21.s
-00007b80: 6574 4f62 6a65 6374 4e61 6d65 2822 7665  etObjectName("ve
-00007b90: 7274 6963 616c 4c61 796f 7574 5f32 3122  rticalLayout_21"
-00007ba0: 290a 2020 2020 2020 2020 7365 6c66 2e66  ).        self.f
-00007bb0: 6f72 6d4c 6179 6f75 745f 3220 3d20 5174  ormLayout_2 = Qt
-00007bc0: 5769 6467 6574 732e 5146 6f72 6d4c 6179  Widgets.QFormLay
-00007bd0: 6f75 7428 290a 2020 2020 2020 2020 7365  out().        se
-00007be0: 6c66 2e66 6f72 6d4c 6179 6f75 745f 322e  lf.formLayout_2.
-00007bf0: 7365 744f 626a 6563 744e 616d 6528 2266  setObjectName("f
-00007c00: 6f72 6d4c 6179 6f75 745f 3222 290a 2020  ormLayout_2").  
-00007c10: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
-00007c20: 5f33 203d 2051 7457 6964 6765 7473 2e51  _3 = QtWidgets.Q
-00007c30: 4c61 6265 6c28 7365 6c66 2e67 726f 7570  Label(self.group
-00007c40: 426f 785f 7265 7375 6c74 735f 696e 666f  Box_results_info
-00007c50: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
-00007c60: 6162 656c 5f33 2e73 6574 4f62 6a65 6374  abel_3.setObject
-00007c70: 4e61 6d65 2822 6c61 6265 6c5f 3322 290a  Name("label_3").
-00007c80: 2020 2020 2020 2020 7365 6c66 2e66 6f72          self.for
-00007c90: 6d4c 6179 6f75 745f 322e 7365 7457 6964  mLayout_2.setWid
-00007ca0: 6765 7428 302c 2051 7457 6964 6765 7473  get(0, QtWidgets
-00007cb0: 2e51 466f 726d 4c61 796f 7574 2e4c 6162  .QFormLayout.Lab
-00007cc0: 656c 526f 6c65 2c20 7365 6c66 2e6c 6162  elRole, self.lab
-00007cd0: 656c 5f33 290a 2020 2020 2020 2020 7365  el_3).        se
-00007ce0: 6c66 2e6c 6162 656c 5f72 6573 756c 7473  lf.label_results
-00007cf0: 5f61 646a 7573 746d 656e 745f 6d65 7468  _adjustment_meth
-00007d00: 6f64 203d 2051 7457 6964 6765 7473 2e51  od = QtWidgets.Q
-00007d10: 4c61 6265 6c28 7365 6c66 2e67 726f 7570  Label(self.group
-00007d20: 426f 785f 7265 7375 6c74 735f 696e 666f  Box_results_info
-00007d30: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
-00007d40: 6162 656c 5f72 6573 756c 7473 5f61 646a  abel_results_adj
-00007d50: 7573 746d 656e 745f 6d65 7468 6f64 2e73  ustment_method.s
-00007d60: 6574 4d69 6e69 6d75 6d53 697a 6528 5174  etMinimumSize(Qt
-00007d70: 436f 7265 2e51 5369 7a65 2831 3030 2c20  Core.QSize(100, 
-00007d80: 3029 290a 2020 2020 2020 2020 7365 6c66  0)).        self
-00007d90: 2e6c 6162 656c 5f72 6573 756c 7473 5f61  .label_results_a
-00007da0: 646a 7573 746d 656e 745f 6d65 7468 6f64  djustment_method
-00007db0: 2e73 6574 5465 7874 2822 2229 0a20 2020  .setText("").   
-00007dc0: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
-00007dd0: 7265 7375 6c74 735f 6164 6a75 7374 6d65  results_adjustme
-00007de0: 6e74 5f6d 6574 686f 642e 7365 744f 626a  nt_method.setObj
-00007df0: 6563 744e 616d 6528 226c 6162 656c 5f72  ectName("label_r
-00007e00: 6573 756c 7473 5f61 646a 7573 746d 656e  esults_adjustmen
-00007e10: 745f 6d65 7468 6f64 2229 0a20 2020 2020  t_method").     
-00007e20: 2020 2073 656c 662e 666f 726d 4c61 796f     self.formLayo
-00007e30: 7574 5f32 2e73 6574 5769 6467 6574 2830  ut_2.setWidget(0
-00007e40: 2c20 5174 5769 6467 6574 732e 5146 6f72  , QtWidgets.QFor
-00007e50: 6d4c 6179 6f75 742e 4669 656c 6452 6f6c  mLayout.FieldRol
-00007e60: 652c 2073 656c 662e 6c61 6265 6c5f 7265  e, self.label_re
-00007e70: 7375 6c74 735f 6164 6a75 7374 6d65 6e74  sults_adjustment
-00007e80: 5f6d 6574 686f 6429 0a20 2020 2020 2020  _method).       
-00007e90: 2073 656c 662e 6c61 6265 6c5f 7265 7375   self.label_resu
-00007ea0: 6c74 735f 7469 6d65 5f61 6e64 5f64 6174  lts_time_and_dat
-00007eb0: 6520 3d20 5174 5769 6467 6574 732e 514c  e = QtWidgets.QL
-00007ec0: 6162 656c 2873 656c 662e 6772 6f75 7042  abel(self.groupB
-00007ed0: 6f78 5f72 6573 756c 7473 5f69 6e66 6f29  ox_results_info)
-00007ee0: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
-00007ef0: 6265 6c5f 7265 7375 6c74 735f 7469 6d65  bel_results_time
-00007f00: 5f61 6e64 5f64 6174 652e 7365 744d 696e  _and_date.setMin
-00007f10: 696d 756d 5369 7a65 2851 7443 6f72 652e  imumSize(QtCore.
-00007f20: 5153 697a 6528 3130 302c 2030 2929 0a20  QSize(100, 0)). 
-00007f30: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
-00007f40: 6c5f 7265 7375 6c74 735f 7469 6d65 5f61  l_results_time_a
-00007f50: 6e64 5f64 6174 652e 7365 7454 6578 7428  nd_date.setText(
-00007f60: 2222 290a 2020 2020 2020 2020 7365 6c66  "").        self
-00007f70: 2e6c 6162 656c 5f72 6573 756c 7473 5f74  .label_results_t
-00007f80: 696d 655f 616e 645f 6461 7465 2e73 6574  ime_and_date.set
-00007f90: 4f62 6a65 6374 4e61 6d65 2822 6c61 6265  ObjectName("labe
-00007fa0: 6c5f 7265 7375 6c74 735f 7469 6d65 5f61  l_results_time_a
-00007fb0: 6e64 5f64 6174 6522 290a 2020 2020 2020  nd_date").      
-00007fc0: 2020 7365 6c66 2e66 6f72 6d4c 6179 6f75    self.formLayou
-00007fd0: 745f 322e 7365 7457 6964 6765 7428 312c  t_2.setWidget(1,
-00007fe0: 2051 7457 6964 6765 7473 2e51 466f 726d   QtWidgets.QForm
-00007ff0: 4c61 796f 7574 2e46 6965 6c64 526f 6c65  Layout.FieldRole
-00008000: 2c20 7365 6c66 2e6c 6162 656c 5f72 6573  , self.label_res
-00008010: 756c 7473 5f74 696d 655f 616e 645f 6461  ults_time_and_da
-00008020: 7465 290a 2020 2020 2020 2020 7365 6c66  te).        self
-00008030: 2e6c 6162 656c 5f38 203d 2051 7457 6964  .label_8 = QtWid
-00008040: 6765 7473 2e51 4c61 6265 6c28 7365 6c66  gets.QLabel(self
-00008050: 2e67 726f 7570 426f 785f 7265 7375 6c74  .groupBox_result
-00008060: 735f 696e 666f 290a 2020 2020 2020 2020  s_info).        
-00008070: 7365 6c66 2e6c 6162 656c 5f38 2e73 6574  self.label_8.set
-00008080: 4f62 6a65 6374 4e61 6d65 2822 6c61 6265  ObjectName("labe
-00008090: 6c5f 3822 290a 2020 2020 2020 2020 7365  l_8").        se
-000080a0: 6c66 2e66 6f72 6d4c 6179 6f75 745f 322e  lf.formLayout_2.
-000080b0: 7365 7457 6964 6765 7428 322c 2051 7457  setWidget(2, QtW
-000080c0: 6964 6765 7473 2e51 466f 726d 4c61 796f  idgets.QFormLayo
-000080d0: 7574 2e4c 6162 656c 526f 6c65 2c20 7365  ut.LabelRole, se
-000080e0: 6c66 2e6c 6162 656c 5f38 290a 2020 2020  lf.label_8).    
-000080f0: 2020 2020 7365 6c66 2e6c 6162 656c 5f72      self.label_r
-00008100: 6573 756c 7473 5f6e 756d 6265 725f 6f66  esults_number_of
-00008110: 5f69 7465 7261 7469 6f6e 7320 3d20 5174  _iterations = Qt
-00008120: 5769 6467 6574 732e 514c 6162 656c 2873  Widgets.QLabel(s
-00008130: 656c 662e 6772 6f75 7042 6f78 5f72 6573  elf.groupBox_res
-00008140: 756c 7473 5f69 6e66 6f29 0a20 2020 2020  ults_info).     
-00008150: 2020 2073 656c 662e 6c61 6265 6c5f 7265     self.label_re
-00008160: 7375 6c74 735f 6e75 6d62 6572 5f6f 665f  sults_number_of_
-00008170: 6974 6572 6174 696f 6e73 2e73 6574 5465  iterations.setTe
-00008180: 7874 2822 2229 0a20 2020 2020 2020 2073  xt("").        s
-00008190: 656c 662e 6c61 6265 6c5f 7265 7375 6c74  elf.label_result
-000081a0: 735f 6e75 6d62 6572 5f6f 665f 6974 6572  s_number_of_iter
-000081b0: 6174 696f 6e73 2e73 6574 4f62 6a65 6374  ations.setObject
-000081c0: 4e61 6d65 2822 6c61 6265 6c5f 7265 7375  Name("label_resu
-000081d0: 6c74 735f 6e75 6d62 6572 5f6f 665f 6974  lts_number_of_it
-000081e0: 6572 6174 696f 6e73 2229 0a20 2020 2020  erations").     
-000081f0: 2020 2073 656c 662e 666f 726d 4c61 796f     self.formLayo
-00008200: 7574 5f32 2e73 6574 5769 6467 6574 2832  ut_2.setWidget(2
-00008210: 2c20 5174 5769 6467 6574 732e 5146 6f72  , QtWidgets.QFor
-00008220: 6d4c 6179 6f75 742e 4669 656c 6452 6f6c  mLayout.FieldRol
-00008230: 652c 2073 656c 662e 6c61 6265 6c5f 7265  e, self.label_re
-00008240: 7375 6c74 735f 6e75 6d62 6572 5f6f 665f  sults_number_of_
-00008250: 6974 6572 6174 696f 6e73 290a 2020 2020  iterations).    
-00008260: 2020 2020 7365 6c66 2e6c 6162 656c 5f31      self.label_1
-00008270: 3020 3d20 5174 5769 6467 6574 732e 514c  0 = QtWidgets.QL
-00008280: 6162 656c 2873 656c 662e 6772 6f75 7042  abel(self.groupB
-00008290: 6f78 5f72 6573 756c 7473 5f69 6e66 6f29  ox_results_info)
-000082a0: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
-000082b0: 6265 6c5f 3130 2e73 6574 4f62 6a65 6374  bel_10.setObject
-000082c0: 4e61 6d65 2822 6c61 6265 6c5f 3130 2229  Name("label_10")
-000082d0: 0a20 2020 2020 2020 2073 656c 662e 666f  .        self.fo
-000082e0: 726d 4c61 796f 7574 5f32 2e73 6574 5769  rmLayout_2.setWi
-000082f0: 6467 6574 2833 2c20 5174 5769 6467 6574  dget(3, QtWidget
-00008300: 732e 5146 6f72 6d4c 6179 6f75 742e 4c61  s.QFormLayout.La
-00008310: 6265 6c52 6f6c 652c 2073 656c 662e 6c61  belRole, self.la
-00008320: 6265 6c5f 3130 290a 2020 2020 2020 2020  bel_10).        
-00008330: 7365 6c66 2e6c 6162 656c 5f72 6573 756c  self.label_resul
-00008340: 7473 5f63 6f6d 6d65 6e74 203d 2051 7457  ts_comment = QtW
-00008350: 6964 6765 7473 2e51 4c61 6265 6c28 7365  idgets.QLabel(se
-00008360: 6c66 2e67 726f 7570 426f 785f 7265 7375  lf.groupBox_resu
-00008370: 6c74 735f 696e 666f 290a 2020 2020 2020  lts_info).      
-00008380: 2020 7365 6c66 2e6c 6162 656c 5f72 6573    self.label_res
-00008390: 756c 7473 5f63 6f6d 6d65 6e74 2e73 6574  ults_comment.set
-000083a0: 4d69 6e69 6d75 6d53 697a 6528 5174 436f  MinimumSize(QtCo
-000083b0: 7265 2e51 5369 7a65 2831 3030 2c20 3029  re.QSize(100, 0)
-000083c0: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
-000083d0: 6162 656c 5f72 6573 756c 7473 5f63 6f6d  abel_results_com
-000083e0: 6d65 6e74 2e73 6574 5465 7874 2822 2229  ment.setText("")
-000083f0: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
-00008400: 6265 6c5f 7265 7375 6c74 735f 636f 6d6d  bel_results_comm
-00008410: 656e 742e 7365 744f 626a 6563 744e 616d  ent.setObjectNam
-00008420: 6528 226c 6162 656c 5f72 6573 756c 7473  e("label_results
-00008430: 5f63 6f6d 6d65 6e74 2229 0a20 2020 2020  _comment").     
-00008440: 2020 2073 656c 662e 666f 726d 4c61 796f     self.formLayo
-00008450: 7574 5f32 2e73 6574 5769 6467 6574 2833  ut_2.setWidget(3
-00008460: 2c20 5174 5769 6467 6574 732e 5146 6f72  , QtWidgets.QFor
-00008470: 6d4c 6179 6f75 742e 4669 656c 6452 6f6c  mLayout.FieldRol
-00008480: 652c 2073 656c 662e 6c61 6265 6c5f 7265  e, self.label_re
-00008490: 7375 6c74 735f 636f 6d6d 656e 7429 0a20  sults_comment). 
-000084a0: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
-000084b0: 6c5f 3420 3d20 5174 5769 6467 6574 732e  l_4 = QtWidgets.
-000084c0: 514c 6162 656c 2873 656c 662e 6772 6f75  QLabel(self.grou
-000084d0: 7042 6f78 5f72 6573 756c 7473 5f69 6e66  pBox_results_inf
-000084e0: 6f29 0a20 2020 2020 2020 2073 656c 662e  o).        self.
-000084f0: 6c61 6265 6c5f 342e 7365 744f 626a 6563  label_4.setObjec
-00008500: 744e 616d 6528 226c 6162 656c 5f34 2229  tName("label_4")
-00008510: 0a20 2020 2020 2020 2073 656c 662e 666f  .        self.fo
-00008520: 726d 4c61 796f 7574 5f32 2e73 6574 5769  rmLayout_2.setWi
-00008530: 6467 6574 2831 2c20 5174 5769 6467 6574  dget(1, QtWidget
-00008540: 732e 5146 6f72 6d4c 6179 6f75 742e 4c61  s.QFormLayout.La
-00008550: 6265 6c52 6f6c 652c 2073 656c 662e 6c61  belRole, self.la
-00008560: 6265 6c5f 3429 0a20 2020 2020 2020 2073  bel_4).        s
-00008570: 656c 662e 7665 7274 6963 616c 4c61 796f  elf.verticalLayo
-00008580: 7574 5f32 312e 6164 644c 6179 6f75 7428  ut_21.addLayout(
-00008590: 7365 6c66 2e66 6f72 6d4c 6179 6f75 745f  self.formLayout_
-000085a0: 3229 0a20 2020 2020 2020 2073 656c 662e  2).        self.
-000085b0: 7665 7274 6963 616c 4c61 796f 7574 5f32  verticalLayout_2
-000085c0: 322e 6164 6457 6964 6765 7428 7365 6c66  2.addWidget(self
-000085d0: 2e67 726f 7570 426f 785f 7265 7375 6c74  .groupBox_result
-000085e0: 735f 696e 666f 290a 2020 2020 2020 2020  s_info).        
-000085f0: 7365 6c66 2e67 726f 7570 426f 785f 7265  self.groupBox_re
-00008600: 7375 6c74 735f 7374 6174 6973 7469 6373  sults_statistics
-00008610: 203d 2051 7457 6964 6765 7473 2e51 4772   = QtWidgets.QGr
-00008620: 6f75 7042 6f78 2873 656c 662e 7461 625f  oupBox(self.tab_
-00008630: 7265 7375 6c74 735f 696e 666f 290a 2020  results_info).  
-00008640: 2020 2020 2020 7365 6c66 2e67 726f 7570        self.group
-00008650: 426f 785f 7265 7375 6c74 735f 7374 6174  Box_results_stat
-00008660: 6973 7469 6373 2e73 6574 4f62 6a65 6374  istics.setObject
-00008670: 4e61 6d65 2822 6772 6f75 7042 6f78 5f72  Name("groupBox_r
-00008680: 6573 756c 7473 5f73 7461 7469 7374 6963  esults_statistic
-00008690: 7322 290a 2020 2020 2020 2020 7365 6c66  s").        self
-000086a0: 2e76 6572 7469 6361 6c4c 6179 6f75 745f  .verticalLayout_
-000086b0: 3234 203d 2051 7457 6964 6765 7473 2e51  24 = QtWidgets.Q
-000086c0: 5642 6f78 4c61 796f 7574 2873 656c 662e  VBoxLayout(self.
-000086d0: 6772 6f75 7042 6f78 5f72 6573 756c 7473  groupBox_results
-000086e0: 5f73 7461 7469 7374 6963 7329 0a20 2020  _statistics).   
-000086f0: 2020 2020 2073 656c 662e 7665 7274 6963       self.vertic
-00008700: 616c 4c61 796f 7574 5f32 342e 7365 744f  alLayout_24.setO
-00008710: 626a 6563 744e 616d 6528 2276 6572 7469  bjectName("verti
-00008720: 6361 6c4c 6179 6f75 745f 3234 2229 0a20  calLayout_24"). 
-00008730: 2020 2020 2020 2073 656c 662e 666f 726d         self.form
-00008740: 4c61 796f 7574 5f33 203d 2051 7457 6964  Layout_3 = QtWid
-00008750: 6765 7473 2e51 466f 726d 4c61 796f 7574  gets.QFormLayout
-00008760: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-00008770: 666f 726d 4c61 796f 7574 5f33 2e73 6574  formLayout_3.set
-00008780: 4f62 6a65 6374 4e61 6d65 2822 666f 726d  ObjectName("form
-00008790: 4c61 796f 7574 5f33 2229 0a20 2020 2020  Layout_3").     
-000087a0: 2020 2073 656c 662e 6c61 6265 6c5f 3920     self.label_9 
-000087b0: 3d20 5174 5769 6467 6574 732e 514c 6162  = QtWidgets.QLab
-000087c0: 656c 2873 656c 662e 6772 6f75 7042 6f78  el(self.groupBox
-000087d0: 5f72 6573 756c 7473 5f73 7461 7469 7374  _results_statist
-000087e0: 6963 7329 0a20 2020 2020 2020 2073 656c  ics).        sel
-000087f0: 662e 6c61 6265 6c5f 392e 7365 744f 626a  f.label_9.setObj
-00008800: 6563 744e 616d 6528 226c 6162 656c 5f39  ectName("label_9
-00008810: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00008820: 666f 726d 4c61 796f 7574 5f33 2e73 6574  formLayout_3.set
-00008830: 5769 6467 6574 2830 2c20 5174 5769 6467  Widget(0, QtWidg
-00008840: 6574 732e 5146 6f72 6d4c 6179 6f75 742e  ets.QFormLayout.
-00008850: 4c61 6265 6c52 6f6c 652c 2073 656c 662e  LabelRole, self.
-00008860: 6c61 6265 6c5f 3929 0a20 2020 2020 2020  label_9).       
-00008870: 2073 656c 662e 6c61 6265 6c5f 7265 7375   self.label_resu
-00008880: 6c74 735f 7369 6730 203d 2051 7457 6964  lts_sig0 = QtWid
-00008890: 6765 7473 2e51 4c61 6265 6c28 7365 6c66  gets.QLabel(self
-000088a0: 2e67 726f 7570 426f 785f 7265 7375 6c74  .groupBox_result
-000088b0: 735f 7374 6174 6973 7469 6373 290a 2020  s_statistics).  
-000088c0: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
-000088d0: 5f72 6573 756c 7473 5f73 6967 302e 7365  _results_sig0.se
-000088e0: 744d 696e 696d 756d 5369 7a65 2851 7443  tMinimumSize(QtC
-000088f0: 6f72 652e 5153 697a 6528 3130 302c 2030  ore.QSize(100, 0
-00008900: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-00008910: 6c61 6265 6c5f 7265 7375 6c74 735f 7369  label_results_si
-00008920: 6730 2e73 6574 5465 7874 2822 2229 0a20  g0.setText(""). 
-00008930: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
-00008940: 6c5f 7265 7375 6c74 735f 7369 6730 2e73  l_results_sig0.s
-00008950: 6574 4f62 6a65 6374 4e61 6d65 2822 6c61  etObjectName("la
-00008960: 6265 6c5f 7265 7375 6c74 735f 7369 6730  bel_results_sig0
-00008970: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00008980: 666f 726d 4c61 796f 7574 5f33 2e73 6574  formLayout_3.set
-00008990: 5769 6467 6574 2830 2c20 5174 5769 6467  Widget(0, QtWidg
-000089a0: 6574 732e 5146 6f72 6d4c 6179 6f75 742e  ets.QFormLayout.
-000089b0: 4669 656c 6452 6f6c 652c 2073 656c 662e  FieldRole, self.
-000089c0: 6c61 6265 6c5f 7265 7375 6c74 735f 7369  label_results_si
-000089d0: 6730 290a 2020 2020 2020 2020 7365 6c66  g0).        self
-000089e0: 2e6c 6162 656c 5f36 203d 2051 7457 6964  .label_6 = QtWid
-000089f0: 6765 7473 2e51 4c61 6265 6c28 7365 6c66  gets.QLabel(self
-00008a00: 2e67 726f 7570 426f 785f 7265 7375 6c74  .groupBox_result
-00008a10: 735f 7374 6174 6973 7469 6373 290a 2020  s_statistics).  
-00008a20: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
-00008a30: 5f36 2e73 6574 4f62 6a65 6374 4e61 6d65  _6.setObjectName
-00008a40: 2822 6c61 6265 6c5f 3622 290a 2020 2020  ("label_6").    
-00008a50: 2020 2020 7365 6c66 2e66 6f72 6d4c 6179      self.formLay
-00008a60: 6f75 745f 332e 7365 7457 6964 6765 7428  out_3.setWidget(
-00008a70: 312c 2051 7457 6964 6765 7473 2e51 466f  1, QtWidgets.QFo
-00008a80: 726d 4c61 796f 7574 2e4c 6162 656c 526f  rmLayout.LabelRo
-00008a90: 6c65 2c20 7365 6c66 2e6c 6162 656c 5f36  le, self.label_6
-00008aa0: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
-00008ab0: 6162 656c 5f72 6573 756c 7473 5f67 6f6f  abel_results_goo
-00008ac0: 646e 6573 735f 6f66 5f66 6974 5f74 6573  dness_of_fit_tes
-00008ad0: 745f 7374 6174 7573 203d 2051 7457 6964  t_status = QtWid
-00008ae0: 6765 7473 2e51 4c61 6265 6c28 7365 6c66  gets.QLabel(self
-00008af0: 2e67 726f 7570 426f 785f 7265 7375 6c74  .groupBox_result
-00008b00: 735f 7374 6174 6973 7469 6373 290a 2020  s_statistics).  
-00008b10: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
-00008b20: 5f72 6573 756c 7473 5f67 6f6f 646e 6573  _results_goodnes
-00008b30: 735f 6f66 5f66 6974 5f74 6573 745f 7374  s_of_fit_test_st
-00008b40: 6174 7573 2e73 6574 5465 7874 2822 2229  atus.setText("")
-00008b50: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
-00008b60: 6265 6c5f 7265 7375 6c74 735f 676f 6f64  bel_results_good
-00008b70: 6e65 7373 5f6f 665f 6669 745f 7465 7374  ness_of_fit_test
-00008b80: 5f73 7461 7475 732e 7365 744f 626a 6563  _status.setObjec
-00008b90: 744e 616d 6528 226c 6162 656c 5f72 6573  tName("label_res
-00008ba0: 756c 7473 5f67 6f6f 646e 6573 735f 6f66  ults_goodness_of
-00008bb0: 5f66 6974 5f74 6573 745f 7374 6174 7573  _fit_test_status
-00008bc0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00008bd0: 666f 726d 4c61 796f 7574 5f33 2e73 6574  formLayout_3.set
-00008be0: 5769 6467 6574 2831 2c20 5174 5769 6467  Widget(1, QtWidg
-00008bf0: 6574 732e 5146 6f72 6d4c 6179 6f75 742e  ets.QFormLayout.
-00008c00: 4669 656c 6452 6f6c 652c 2073 656c 662e  FieldRole, self.
-00008c10: 6c61 6265 6c5f 7265 7375 6c74 735f 676f  label_results_go
-00008c20: 6f64 6e65 7373 5f6f 665f 6669 745f 7465  odness_of_fit_te
-00008c30: 7374 5f73 7461 7475 7329 0a20 2020 2020  st_status).     
-00008c40: 2020 2073 656c 662e 6c61 6265 6c5f 3720     self.label_7 
-00008c50: 3d20 5174 5769 6467 6574 732e 514c 6162  = QtWidgets.QLab
-00008c60: 656c 2873 656c 662e 6772 6f75 7042 6f78  el(self.groupBox
-00008c70: 5f72 6573 756c 7473 5f73 7461 7469 7374  _results_statist
-00008c80: 6963 7329 0a20 2020 2020 2020 2073 656c  ics).        sel
-00008c90: 662e 6c61 6265 6c5f 372e 7365 744f 626a  f.label_7.setObj
-00008ca0: 6563 744e 616d 6528 226c 6162 656c 5f37  ectName("label_7
-00008cb0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00008cc0: 666f 726d 4c61 796f 7574 5f33 2e73 6574  formLayout_3.set
-00008cd0: 5769 6467 6574 2832 2c20 5174 5769 6467  Widget(2, QtWidg
-00008ce0: 6574 732e 5146 6f72 6d4c 6179 6f75 742e  ets.QFormLayout.
-00008cf0: 4c61 6265 6c52 6f6c 652c 2073 656c 662e  LabelRole, self.
-00008d00: 6c61 6265 6c5f 3729 0a20 2020 2020 2020  label_7).       
-00008d10: 2073 656c 662e 6c61 6265 6c5f 7265 7375   self.label_resu
-00008d20: 6c74 735f 6e75 6d62 6572 5f6f 665f 6f75  lts_number_of_ou
-00008d30: 746c 6965 7273 203d 2051 7457 6964 6765  tliers = QtWidge
-00008d40: 7473 2e51 4c61 6265 6c28 7365 6c66 2e67  ts.QLabel(self.g
-00008d50: 726f 7570 426f 785f 7265 7375 6c74 735f  roupBox_results_
-00008d60: 7374 6174 6973 7469 6373 290a 2020 2020  statistics).    
-00008d70: 2020 2020 7365 6c66 2e6c 6162 656c 5f72      self.label_r
-00008d80: 6573 756c 7473 5f6e 756d 6265 725f 6f66  esults_number_of
-00008d90: 5f6f 7574 6c69 6572 732e 7365 7454 6578  _outliers.setTex
-00008da0: 7428 2222 290a 2020 2020 2020 2020 7365  t("").        se
-00008db0: 6c66 2e6c 6162 656c 5f72 6573 756c 7473  lf.label_results
-00008dc0: 5f6e 756d 6265 725f 6f66 5f6f 7574 6c69  _number_of_outli
-00008dd0: 6572 732e 7365 744f 626a 6563 744e 616d  ers.setObjectNam
-00008de0: 6528 226c 6162 656c 5f72 6573 756c 7473  e("label_results
-00008df0: 5f6e 756d 6265 725f 6f66 5f6f 7574 6c69  _number_of_outli
-00008e00: 6572 7322 290a 2020 2020 2020 2020 7365  ers").        se
-00008e10: 6c66 2e66 6f72 6d4c 6179 6f75 745f 332e  lf.formLayout_3.
-00008e20: 7365 7457 6964 6765 7428 322c 2051 7457  setWidget(2, QtW
-00008e30: 6964 6765 7473 2e51 466f 726d 4c61 796f  idgets.QFormLayo
-00008e40: 7574 2e46 6965 6c64 526f 6c65 2c20 7365  ut.FieldRole, se
-00008e50: 6c66 2e6c 6162 656c 5f72 6573 756c 7473  lf.label_results
-00008e60: 5f6e 756d 6265 725f 6f66 5f6f 7574 6c69  _number_of_outli
-00008e70: 6572 7329 0a20 2020 2020 2020 2073 656c  ers).        sel
-00008e80: 662e 7665 7274 6963 616c 4c61 796f 7574  f.verticalLayout
-00008e90: 5f32 342e 6164 644c 6179 6f75 7428 7365  _24.addLayout(se
-00008ea0: 6c66 2e66 6f72 6d4c 6179 6f75 745f 3329  lf.formLayout_3)
-00008eb0: 0a20 2020 2020 2020 2073 656c 662e 7665  .        self.ve
-00008ec0: 7274 6963 616c 4c61 796f 7574 5f32 322e  rticalLayout_22.
-00008ed0: 6164 6457 6964 6765 7428 7365 6c66 2e67  addWidget(self.g
-00008ee0: 726f 7570 426f 785f 7265 7375 6c74 735f  roupBox_results_
-00008ef0: 7374 6174 6973 7469 6373 290a 2020 2020  statistics).    
-00008f00: 2020 2020 7365 6c66 2e67 726f 7570 426f      self.groupBo
-00008f10: 785f 7265 7375 6c74 735f 6c73 6d5f 7275  x_results_lsm_ru
-00008f20: 6e5f 6c6f 6720 3d20 5174 5769 6467 6574  n_log = QtWidget
-00008f30: 732e 5147 726f 7570 426f 7828 7365 6c66  s.QGroupBox(self
-00008f40: 2e74 6162 5f72 6573 756c 7473 5f69 6e66  .tab_results_inf
-00008f50: 6f29 0a20 2020 2020 2020 2073 656c 662e  o).        self.
-00008f60: 6772 6f75 7042 6f78 5f72 6573 756c 7473  groupBox_results
-00008f70: 5f6c 736d 5f72 756e 5f6c 6f67 2e73 6574  _lsm_run_log.set
-00008f80: 4f62 6a65 6374 4e61 6d65 2822 6772 6f75  ObjectName("grou
-00008f90: 7042 6f78 5f72 6573 756c 7473 5f6c 736d  pBox_results_lsm
-00008fa0: 5f72 756e 5f6c 6f67 2229 0a20 2020 2020  _run_log").     
-00008fb0: 2020 2073 656c 662e 7665 7274 6963 616c     self.vertical
-00008fc0: 4c61 796f 7574 5f32 3020 3d20 5174 5769  Layout_20 = QtWi
-00008fd0: 6467 6574 732e 5156 426f 784c 6179 6f75  dgets.QVBoxLayou
-00008fe0: 7428 7365 6c66 2e67 726f 7570 426f 785f  t(self.groupBox_
-00008ff0: 7265 7375 6c74 735f 6c73 6d5f 7275 6e5f  results_lsm_run_
-00009000: 6c6f 6729 0a20 2020 2020 2020 2073 656c  log).        sel
-00009010: 662e 7665 7274 6963 616c 4c61 796f 7574  f.verticalLayout
-00009020: 5f32 302e 7365 744f 626a 6563 744e 616d  _20.setObjectNam
-00009030: 6528 2276 6572 7469 6361 6c4c 6179 6f75  e("verticalLayou
-00009040: 745f 3230 2229 0a20 2020 2020 2020 2073  t_20").        s
-00009050: 656c 662e 706c 6169 6e54 6578 7445 6469  elf.plainTextEdi
-00009060: 745f 7265 7375 6c74 735f 6c6f 6720 3d20  t_results_log = 
-00009070: 5174 5769 6467 6574 732e 5150 6c61 696e  QtWidgets.QPlain
-00009080: 5465 7874 4564 6974 2873 656c 662e 6772  TextEdit(self.gr
-00009090: 6f75 7042 6f78 5f72 6573 756c 7473 5f6c  oupBox_results_l
-000090a0: 736d 5f72 756e 5f6c 6f67 290a 2020 2020  sm_run_log).    
-000090b0: 2020 2020 7365 6c66 2e70 6c61 696e 5465      self.plainTe
-000090c0: 7874 4564 6974 5f72 6573 756c 7473 5f6c  xtEdit_results_l
-000090d0: 6f67 2e73 6574 5265 6164 4f6e 6c79 2854  og.setReadOnly(T
-000090e0: 7275 6529 0a20 2020 2020 2020 2073 656c  rue).        sel
-000090f0: 662e 706c 6169 6e54 6578 7445 6469 745f  f.plainTextEdit_
-00009100: 7265 7375 6c74 735f 6c6f 672e 7365 744f  results_log.setO
-00009110: 626a 6563 744e 616d 6528 2270 6c61 696e  bjectName("plain
-00009120: 5465 7874 4564 6974 5f72 6573 756c 7473  TextEdit_results
-00009130: 5f6c 6f67 2229 0a20 2020 2020 2020 2073  _log").        s
-00009140: 656c 662e 7665 7274 6963 616c 4c61 796f  elf.verticalLayo
-00009150: 7574 5f32 302e 6164 6457 6964 6765 7428  ut_20.addWidget(
-00009160: 7365 6c66 2e70 6c61 696e 5465 7874 4564  self.plainTextEd
-00009170: 6974 5f72 6573 756c 7473 5f6c 6f67 290a  it_results_log).
-00009180: 2020 2020 2020 2020 7365 6c66 2e76 6572          self.ver
-00009190: 7469 6361 6c4c 6179 6f75 745f 3232 2e61  ticalLayout_22.a
-000091a0: 6464 5769 6467 6574 2873 656c 662e 6772  ddWidget(self.gr
-000091b0: 6f75 7042 6f78 5f72 6573 756c 7473 5f6c  oupBox_results_l
-000091c0: 736d 5f72 756e 5f6c 6f67 290a 2020 2020  sm_run_log).    
-000091d0: 2020 2020 7365 6c66 2e76 6572 7469 6361      self.vertica
-000091e0: 6c4c 6179 6f75 745f 3233 2e61 6464 4c61  lLayout_23.addLa
-000091f0: 796f 7574 2873 656c 662e 7665 7274 6963  yout(self.vertic
-00009200: 616c 4c61 796f 7574 5f32 3229 0a20 2020  alLayout_22).   
-00009210: 2020 2020 2073 656c 662e 7461 6257 6964       self.tabWid
-00009220: 6765 745f 7265 7375 6c74 732e 6164 6454  get_results.addT
-00009230: 6162 2873 656c 662e 7461 625f 7265 7375  ab(self.tab_resu
-00009240: 6c74 735f 696e 666f 2c20 2222 290a 2020  lts_info, "").  
-00009250: 2020 2020 2020 7365 6c66 2e74 6162 5f72        self.tab_r
-00009260: 6573 756c 7473 5f6f 6273 5f74 6162 6c65  esults_obs_table
-00009270: 203d 2051 7457 6964 6765 7473 2e51 5769   = QtWidgets.QWi
-00009280: 6467 6574 2829 0a20 2020 2020 2020 2073  dget().        s
-00009290: 656c 662e 7461 625f 7265 7375 6c74 735f  elf.tab_results_
-000092a0: 6f62 735f 7461 626c 652e 7365 744f 626a  obs_table.setObj
-000092b0: 6563 744e 616d 6528 2274 6162 5f72 6573  ectName("tab_res
-000092c0: 756c 7473 5f6f 6273 5f74 6162 6c65 2229  ults_obs_table")
-000092d0: 0a20 2020 2020 2020 2073 656c 662e 7665  .        self.ve
-000092e0: 7274 6963 616c 4c61 796f 7574 5f31 3520  rticalLayout_15 
-000092f0: 3d20 5174 5769 6467 6574 732e 5156 426f  = QtWidgets.QVBo
-00009300: 784c 6179 6f75 7428 7365 6c66 2e74 6162  xLayout(self.tab
-00009310: 5f72 6573 756c 7473 5f6f 6273 5f74 6162  _results_obs_tab
-00009320: 6c65 290a 2020 2020 2020 2020 7365 6c66  le).        self
-00009330: 2e76 6572 7469 6361 6c4c 6179 6f75 745f  .verticalLayout_
-00009340: 3135 2e73 6574 4f62 6a65 6374 4e61 6d65  15.setObjectName
-00009350: 2822 7665 7274 6963 616c 4c61 796f 7574  ("verticalLayout
-00009360: 5f31 3522 290a 2020 2020 2020 2020 7365  _15").        se
-00009370: 6c66 2e74 6162 6c65 5669 6577 5f72 6573  lf.tableView_res
-00009380: 756c 7473 5f6f 6273 6572 7661 7469 6f6e  ults_observation
-00009390: 7320 3d20 5174 5769 6467 6574 732e 5154  s = QtWidgets.QT
-000093a0: 6162 6c65 5669 6577 2873 656c 662e 7461  ableView(self.ta
-000093b0: 625f 7265 7375 6c74 735f 6f62 735f 7461  b_results_obs_ta
-000093c0: 626c 6529 0a20 2020 2020 2020 2073 656c  ble).        sel
-000093d0: 662e 7461 626c 6556 6965 775f 7265 7375  f.tableView_resu
-000093e0: 6c74 735f 6f62 7365 7276 6174 696f 6e73  lts_observations
-000093f0: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
-00009400: 7461 626c 6556 6965 775f 7265 7375 6c74  tableView_result
-00009410: 735f 6f62 7365 7276 6174 696f 6e73 2229  s_observations")
-00009420: 0a20 2020 2020 2020 2073 656c 662e 7665  .        self.ve
-00009430: 7274 6963 616c 4c61 796f 7574 5f31 352e  rticalLayout_15.
-00009440: 6164 6457 6964 6765 7428 7365 6c66 2e74  addWidget(self.t
-00009450: 6162 6c65 5669 6577 5f72 6573 756c 7473  ableView_results
-00009460: 5f6f 6273 6572 7661 7469 6f6e 7329 0a20  _observations). 
-00009470: 2020 2020 2020 2073 656c 662e 7461 6257         self.tabW
-00009480: 6964 6765 745f 7265 7375 6c74 732e 6164  idget_results.ad
-00009490: 6454 6162 2873 656c 662e 7461 625f 7265  dTab(self.tab_re
-000094a0: 7375 6c74 735f 6f62 735f 7461 626c 652c  sults_obs_table,
-000094b0: 2022 2229 0a20 2020 2020 2020 2073 656c   "").        sel
-000094c0: 662e 7461 625f 7265 7375 6c74 735f 6f62  f.tab_results_ob
-000094d0: 735f 706c 6f74 7320 3d20 5174 5769 6467  s_plots = QtWidg
-000094e0: 6574 732e 5157 6964 6765 7428 290a 2020  ets.QWidget().  
-000094f0: 2020 2020 2020 7365 6c66 2e74 6162 5f72        self.tab_r
-00009500: 6573 756c 7473 5f6f 6273 5f70 6c6f 7473  esults_obs_plots
-00009510: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
-00009520: 7461 625f 7265 7375 6c74 735f 6f62 735f  tab_results_obs_
-00009530: 706c 6f74 7322 290a 2020 2020 2020 2020  plots").        
-00009540: 7365 6c66 2e76 6572 7469 6361 6c4c 6179  self.verticalLay
-00009550: 6f75 745f 3338 203d 2051 7457 6964 6765  out_38 = QtWidge
-00009560: 7473 2e51 5642 6f78 4c61 796f 7574 2873  ts.QVBoxLayout(s
-00009570: 656c 662e 7461 625f 7265 7375 6c74 735f  elf.tab_results_
-00009580: 6f62 735f 706c 6f74 7329 0a20 2020 2020  obs_plots).     
-00009590: 2020 2073 656c 662e 7665 7274 6963 616c     self.vertical
-000095a0: 4c61 796f 7574 5f33 382e 7365 744f 626a  Layout_38.setObj
-000095b0: 6563 744e 616d 6528 2276 6572 7469 6361  ectName("vertica
-000095c0: 6c4c 6179 6f75 745f 3338 2229 0a20 2020  lLayout_38").   
-000095d0: 2020 2020 2073 656c 662e 6772 6170 6869       self.graphi
-000095e0: 6373 4c61 796f 7574 5769 6467 6574 5f72  csLayoutWidget_r
-000095f0: 6573 756c 7473 5f6f 6273 6572 7661 7469  esults_observati
-00009600: 6f6e 735f 706c 6f74 7320 3d20 4772 6170  ons_plots = Grap
-00009610: 6869 6373 4c61 796f 7574 5769 6467 6574  hicsLayoutWidget
-00009620: 2873 656c 662e 7461 625f 7265 7375 6c74  (self.tab_result
-00009630: 735f 6f62 735f 706c 6f74 7329 0a20 2020  s_obs_plots).   
-00009640: 2020 2020 2073 656c 662e 6772 6170 6869       self.graphi
-00009650: 6373 4c61 796f 7574 5769 6467 6574 5f72  csLayoutWidget_r
-00009660: 6573 756c 7473 5f6f 6273 6572 7661 7469  esults_observati
-00009670: 6f6e 735f 706c 6f74 732e 7365 744f 626a  ons_plots.setObj
-00009680: 6563 744e 616d 6528 2267 7261 7068 6963  ectName("graphic
-00009690: 734c 6179 6f75 7457 6964 6765 745f 7265  sLayoutWidget_re
-000096a0: 7375 6c74 735f 6f62 7365 7276 6174 696f  sults_observatio
-000096b0: 6e73 5f70 6c6f 7473 2229 0a20 2020 2020  ns_plots").     
-000096c0: 2020 2073 656c 662e 7665 7274 6963 616c     self.vertical
-000096d0: 4c61 796f 7574 5f33 382e 6164 6457 6964  Layout_38.addWid
-000096e0: 6765 7428 7365 6c66 2e67 7261 7068 6963  get(self.graphic
-000096f0: 734c 6179 6f75 7457 6964 6765 745f 7265  sLayoutWidget_re
-00009700: 7375 6c74 735f 6f62 7365 7276 6174 696f  sults_observatio
-00009710: 6e73 5f70 6c6f 7473 290a 2020 2020 2020  ns_plots).      
-00009720: 2020 7365 6c66 2e68 6f72 697a 6f6e 7461    self.horizonta
-00009730: 6c4c 6179 6f75 7420 3d20 5174 5769 6467  lLayout = QtWidg
-00009740: 6574 732e 5148 426f 784c 6179 6f75 7428  ets.QHBoxLayout(
-00009750: 290a 2020 2020 2020 2020 7365 6c66 2e68  ).        self.h
-00009760: 6f72 697a 6f6e 7461 6c4c 6179 6f75 742e  orizontalLayout.
-00009770: 7365 744f 626a 6563 744e 616d 6528 2268  setObjectName("h
-00009780: 6f72 697a 6f6e 7461 6c4c 6179 6f75 7422  orizontalLayout"
-00009790: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
-000097a0: 726f 7570 426f 785f 706c 6f74 5f73 6574  roupBox_plot_set
-000097b0: 7469 6e67 7320 3d20 5174 5769 6467 6574  tings = QtWidget
-000097c0: 732e 5147 726f 7570 426f 7828 7365 6c66  s.QGroupBox(self
-000097d0: 2e74 6162 5f72 6573 756c 7473 5f6f 6273  .tab_results_obs
-000097e0: 5f70 6c6f 7473 290a 2020 2020 2020 2020  _plots).        
-000097f0: 7365 6c66 2e67 726f 7570 426f 785f 706c  self.groupBox_pl
-00009800: 6f74 5f73 6574 7469 6e67 732e 7365 744f  ot_settings.setO
-00009810: 626a 6563 744e 616d 6528 2267 726f 7570  bjectName("group
-00009820: 426f 785f 706c 6f74 5f73 6574 7469 6e67  Box_plot_setting
-00009830: 7322 290a 2020 2020 2020 2020 7365 6c66  s").        self
-00009840: 2e76 6572 7469 6361 6c4c 6179 6f75 745f  .verticalLayout_
-00009850: 3235 203d 2051 7457 6964 6765 7473 2e51  25 = QtWidgets.Q
-00009860: 5642 6f78 4c61 796f 7574 2873 656c 662e  VBoxLayout(self.
-00009870: 6772 6f75 7042 6f78 5f70 6c6f 745f 7365  groupBox_plot_se
-00009880: 7474 696e 6773 290a 2020 2020 2020 2020  ttings).        
-00009890: 7365 6c66 2e76 6572 7469 6361 6c4c 6179  self.verticalLay
-000098a0: 6f75 745f 3235 2e73 6574 4f62 6a65 6374  out_25.setObject
-000098b0: 4e61 6d65 2822 7665 7274 6963 616c 4c61  Name("verticalLa
-000098c0: 796f 7574 5f32 3522 290a 2020 2020 2020  yout_25").      
-000098d0: 2020 7365 6c66 2e66 6f72 6d4c 6179 6f75    self.formLayou
-000098e0: 745f 3420 3d20 5174 5769 6467 6574 732e  t_4 = QtWidgets.
-000098f0: 5146 6f72 6d4c 6179 6f75 7428 290a 2020  QFormLayout().  
-00009900: 2020 2020 2020 7365 6c66 2e66 6f72 6d4c        self.formL
-00009910: 6179 6f75 745f 342e 7365 744f 626a 6563  ayout_4.setObjec
-00009920: 744e 616d 6528 2266 6f72 6d4c 6179 6f75  tName("formLayou
-00009930: 745f 3422 290a 2020 2020 2020 2020 7365  t_4").        se
-00009940: 6c66 2e6c 6162 656c 5f72 6573 756c 7473  lf.label_results
-00009950: 5f6f 6273 5f70 6c6f 745f 7365 6c65 635f  _obs_plot_selec_
-00009960: 6461 7461 5f63 6f6c 756d 6e20 3d20 5174  data_column = Qt
-00009970: 5769 6467 6574 732e 514c 6162 656c 2873  Widgets.QLabel(s
-00009980: 656c 662e 6772 6f75 7042 6f78 5f70 6c6f  elf.groupBox_plo
-00009990: 745f 7365 7474 696e 6773 290a 2020 2020  t_settings).    
-000099a0: 2020 2020 7365 6c66 2e6c 6162 656c 5f72      self.label_r
-000099b0: 6573 756c 7473 5f6f 6273 5f70 6c6f 745f  esults_obs_plot_
-000099c0: 7365 6c65 635f 6461 7461 5f63 6f6c 756d  selec_data_colum
-000099d0: 6e2e 7365 744f 626a 6563 744e 616d 6528  n.setObjectName(
-000099e0: 226c 6162 656c 5f72 6573 756c 7473 5f6f  "label_results_o
-000099f0: 6273 5f70 6c6f 745f 7365 6c65 635f 6461  bs_plot_selec_da
-00009a00: 7461 5f63 6f6c 756d 6e22 290a 2020 2020  ta_column").    
-00009a10: 2020 2020 7365 6c66 2e66 6f72 6d4c 6179      self.formLay
-00009a20: 6f75 745f 342e 7365 7457 6964 6765 7428  out_4.setWidget(
-00009a30: 302c 2051 7457 6964 6765 7473 2e51 466f  0, QtWidgets.QFo
-00009a40: 726d 4c61 796f 7574 2e4c 6162 656c 526f  rmLayout.LabelRo
-00009a50: 6c65 2c20 7365 6c66 2e6c 6162 656c 5f72  le, self.label_r
-00009a60: 6573 756c 7473 5f6f 6273 5f70 6c6f 745f  esults_obs_plot_
-00009a70: 7365 6c65 635f 6461 7461 5f63 6f6c 756d  selec_data_colum
-00009a80: 6e29 0a20 2020 2020 2020 2073 656c 662e  n).        self.
-00009a90: 636f 6d62 6f42 6f78 5f72 6573 756c 7473  comboBox_results
-00009aa0: 5f6f 6273 5f70 6c6f 745f 7365 6c65 6374  _obs_plot_select
-00009ab0: 5f64 6174 615f 636f 6c75 6d6e 203d 2051  _data_column = Q
-00009ac0: 7457 6964 6765 7473 2e51 436f 6d62 6f42  tWidgets.QComboB
-00009ad0: 6f78 2873 656c 662e 6772 6f75 7042 6f78  ox(self.groupBox
-00009ae0: 5f70 6c6f 745f 7365 7474 696e 6773 290a  _plot_settings).
-00009af0: 2020 2020 2020 2020 7365 6c66 2e63 6f6d          self.com
-00009b00: 626f 426f 785f 7265 7375 6c74 735f 6f62  boBox_results_ob
-00009b10: 735f 706c 6f74 5f73 656c 6563 745f 6461  s_plot_select_da
-00009b20: 7461 5f63 6f6c 756d 6e2e 7365 744f 626a  ta_column.setObj
-00009b30: 6563 744e 616d 6528 2263 6f6d 626f 426f  ectName("comboBo
-00009b40: 785f 7265 7375 6c74 735f 6f62 735f 706c  x_results_obs_pl
-00009b50: 6f74 5f73 656c 6563 745f 6461 7461 5f63  ot_select_data_c
-00009b60: 6f6c 756d 6e22 290a 2020 2020 2020 2020  olumn").        
-00009b70: 7365 6c66 2e66 6f72 6d4c 6179 6f75 745f  self.formLayout_
-00009b80: 342e 7365 7457 6964 6765 7428 302c 2051  4.setWidget(0, Q
-00009b90: 7457 6964 6765 7473 2e51 466f 726d 4c61  tWidgets.QFormLa
-00009ba0: 796f 7574 2e46 6965 6c64 526f 6c65 2c20  yout.FieldRole, 
-00009bb0: 7365 6c66 2e63 6f6d 626f 426f 785f 7265  self.comboBox_re
-00009bc0: 7375 6c74 735f 6f62 735f 706c 6f74 5f73  sults_obs_plot_s
-00009bd0: 656c 6563 745f 6461 7461 5f63 6f6c 756d  elect_data_colum
-00009be0: 6e29 0a20 2020 2020 2020 2073 656c 662e  n).        self.
-00009bf0: 7665 7274 6963 616c 4c61 796f 7574 5f32  verticalLayout_2
-00009c00: 352e 6164 644c 6179 6f75 7428 7365 6c66  5.addLayout(self
-00009c10: 2e66 6f72 6d4c 6179 6f75 745f 3429 0a20  .formLayout_4). 
-00009c20: 2020 2020 2020 2073 656c 662e 7261 6469         self.radi
-00009c30: 6f42 7574 746f 6e5f 7265 7375 6c74 735f  oButton_results_
-00009c40: 6f62 735f 706c 6f74 5f74 696d 6573 6572  obs_plot_timeser
-00009c50: 6965 7320 3d20 5174 5769 6467 6574 732e  ies = QtWidgets.
-00009c60: 5152 6164 696f 4275 7474 6f6e 2873 656c  QRadioButton(sel
-00009c70: 662e 6772 6f75 7042 6f78 5f70 6c6f 745f  f.groupBox_plot_
-00009c80: 7365 7474 696e 6773 290a 2020 2020 2020  settings).      
-00009c90: 2020 7365 6c66 2e72 6164 696f 4275 7474    self.radioButt
-00009ca0: 6f6e 5f72 6573 756c 7473 5f6f 6273 5f70  on_results_obs_p
-00009cb0: 6c6f 745f 7469 6d65 7365 7269 6573 2e73  lot_timeseries.s
-00009cc0: 6574 4368 6563 6b65 6428 5472 7565 290a  etChecked(True).
-00009cd0: 2020 2020 2020 2020 7365 6c66 2e72 6164          self.rad
-00009ce0: 696f 4275 7474 6f6e 5f72 6573 756c 7473  ioButton_results
-00009cf0: 5f6f 6273 5f70 6c6f 745f 7469 6d65 7365  _obs_plot_timese
-00009d00: 7269 6573 2e73 6574 4f62 6a65 6374 4e61  ries.setObjectNa
-00009d10: 6d65 2822 7261 6469 6f42 7574 746f 6e5f  me("radioButton_
-00009d20: 7265 7375 6c74 735f 6f62 735f 706c 6f74  results_obs_plot
-00009d30: 5f74 696d 6573 6572 6965 7322 290a 2020  _timeseries").  
-00009d40: 2020 2020 2020 7365 6c66 2e76 6572 7469        self.verti
-00009d50: 6361 6c4c 6179 6f75 745f 3235 2e61 6464  calLayout_25.add
-00009d60: 5769 6467 6574 2873 656c 662e 7261 6469  Widget(self.radi
-00009d70: 6f42 7574 746f 6e5f 7265 7375 6c74 735f  oButton_results_
-00009d80: 6f62 735f 706c 6f74 5f74 696d 6573 6572  obs_plot_timeser
-00009d90: 6965 7329 0a20 2020 2020 2020 2073 656c  ies).        sel
-00009da0: 662e 7261 6469 6f42 7574 746f 6e5f 7265  f.radioButton_re
-00009db0: 7375 6c74 735f 6f62 735f 706c 6f74 5f68  sults_obs_plot_h
-00009dc0: 6973 746f 6772 616d 203d 2051 7457 6964  istogram = QtWid
-00009dd0: 6765 7473 2e51 5261 6469 6f42 7574 746f  gets.QRadioButto
-00009de0: 6e28 7365 6c66 2e67 726f 7570 426f 785f  n(self.groupBox_
-00009df0: 706c 6f74 5f73 6574 7469 6e67 7329 0a20  plot_settings). 
-00009e00: 2020 2020 2020 2073 656c 662e 7261 6469         self.radi
-00009e10: 6f42 7574 746f 6e5f 7265 7375 6c74 735f  oButton_results_
-00009e20: 6f62 735f 706c 6f74 5f68 6973 746f 6772  obs_plot_histogr
-00009e30: 616d 2e73 6574 4f62 6a65 6374 4e61 6d65  am.setObjectName
-00009e40: 2822 7261 6469 6f42 7574 746f 6e5f 7265  ("radioButton_re
-00009e50: 7375 6c74 735f 6f62 735f 706c 6f74 5f68  sults_obs_plot_h
-00009e60: 6973 746f 6772 616d 2229 0a20 2020 2020  istogram").     
-00009e70: 2020 2073 656c 662e 7665 7274 6963 616c     self.vertical
-00009e80: 4c61 796f 7574 5f32 352e 6164 6457 6964  Layout_25.addWid
-00009e90: 6765 7428 7365 6c66 2e72 6164 696f 4275  get(self.radioBu
-00009ea0: 7474 6f6e 5f72 6573 756c 7473 5f6f 6273  tton_results_obs
-00009eb0: 5f70 6c6f 745f 6869 7374 6f67 7261 6d29  _plot_histogram)
-00009ec0: 0a20 2020 2020 2020 2073 656c 662e 686f  .        self.ho
-00009ed0: 7269 7a6f 6e74 616c 4c61 796f 7574 2e61  rizontalLayout.a
-00009ee0: 6464 5769 6467 6574 2873 656c 662e 6772  ddWidget(self.gr
-00009ef0: 6f75 7042 6f78 5f70 6c6f 745f 7365 7474  oupBox_plot_sett
-00009f00: 696e 6773 290a 2020 2020 2020 2020 7365  ings).        se
-00009f10: 6c66 2e67 726f 7570 426f 785f 6869 7374  lf.groupBox_hist
-00009f20: 6f67 7261 6d5f 7365 7474 696e 6773 203d  ogram_settings =
-00009f30: 2051 7457 6964 6765 7473 2e51 4772 6f75   QtWidgets.QGrou
-00009f40: 7042 6f78 2873 656c 662e 7461 625f 7265  pBox(self.tab_re
-00009f50: 7375 6c74 735f 6f62 735f 706c 6f74 7329  sults_obs_plots)
-00009f60: 0a20 2020 2020 2020 2073 656c 662e 6772  .        self.gr
-00009f70: 6f75 7042 6f78 5f68 6973 746f 6772 616d  oupBox_histogram
-00009f80: 5f73 6574 7469 6e67 732e 7365 7445 6e61  _settings.setEna
-00009f90: 626c 6564 2846 616c 7365 290a 2020 2020  bled(False).    
-00009fa0: 2020 2020 7365 6c66 2e67 726f 7570 426f      self.groupBo
-00009fb0: 785f 6869 7374 6f67 7261 6d5f 7365 7474  x_histogram_sett
-00009fc0: 696e 6773 2e73 6574 4f62 6a65 6374 4e61  ings.setObjectNa
-00009fd0: 6d65 2822 6772 6f75 7042 6f78 5f68 6973  me("groupBox_his
-00009fe0: 746f 6772 616d 5f73 6574 7469 6e67 7322  togram_settings"
-00009ff0: 290a 2020 2020 2020 2020 7365 6c66 2e76  ).        self.v
-0000a000: 6572 7469 6361 6c4c 6179 6f75 745f 3133  erticalLayout_13
-0000a010: 203d 2051 7457 6964 6765 7473 2e51 5642   = QtWidgets.QVB
-0000a020: 6f78 4c61 796f 7574 2873 656c 662e 6772  oxLayout(self.gr
-0000a030: 6f75 7042 6f78 5f68 6973 746f 6772 616d  oupBox_histogram
-0000a040: 5f73 6574 7469 6e67 7329 0a20 2020 2020  _settings).     
-0000a050: 2020 2073 656c 662e 7665 7274 6963 616c     self.vertical
-0000a060: 4c61 796f 7574 5f31 332e 7365 744f 626a  Layout_13.setObj
-0000a070: 6563 744e 616d 6528 2276 6572 7469 6361  ectName("vertica
-0000a080: 6c4c 6179 6f75 745f 3133 2229 0a20 2020  lLayout_13").   
-0000a090: 2020 2020 2073 656c 662e 666f 726d 4c61       self.formLa
-0000a0a0: 796f 7574 5f38 203d 2051 7457 6964 6765  yout_8 = QtWidge
-0000a0b0: 7473 2e51 466f 726d 4c61 796f 7574 2829  ts.QFormLayout()
-0000a0c0: 0a20 2020 2020 2020 2073 656c 662e 666f  .        self.fo
-0000a0d0: 726d 4c61 796f 7574 5f38 2e73 6574 4f62  rmLayout_8.setOb
-0000a0e0: 6a65 6374 4e61 6d65 2822 666f 726d 4c61  jectName("formLa
-0000a0f0: 796f 7574 5f38 2229 0a20 2020 2020 2020  yout_8").       
-0000a100: 2073 656c 662e 6c61 6265 6c5f 3131 203d   self.label_11 =
-0000a110: 2051 7457 6964 6765 7473 2e51 4c61 6265   QtWidgets.QLabe
-0000a120: 6c28 7365 6c66 2e67 726f 7570 426f 785f  l(self.groupBox_
-0000a130: 6869 7374 6f67 7261 6d5f 7365 7474 696e  histogram_settin
-0000a140: 6773 290a 2020 2020 2020 2020 7365 6c66  gs).        self
-0000a150: 2e6c 6162 656c 5f31 312e 7365 744f 626a  .label_11.setObj
-0000a160: 6563 744e 616d 6528 226c 6162 656c 5f31  ectName("label_1
-0000a170: 3122 290a 2020 2020 2020 2020 7365 6c66  1").        self
-0000a180: 2e66 6f72 6d4c 6179 6f75 745f 382e 7365  .formLayout_8.se
-0000a190: 7457 6964 6765 7428 302c 2051 7457 6964  tWidget(0, QtWid
-0000a1a0: 6765 7473 2e51 466f 726d 4c61 796f 7574  gets.QFormLayout
-0000a1b0: 2e4c 6162 656c 526f 6c65 2c20 7365 6c66  .LabelRole, self
-0000a1c0: 2e6c 6162 656c 5f31 3129 0a20 2020 2020  .label_11).     
-0000a1d0: 2020 2073 656c 662e 636f 6d62 6f42 6f78     self.comboBox
-0000a1e0: 5f72 6573 756c 7473 5f6f 6273 5f70 6c6f  _results_obs_plo
-0000a1f0: 745f 6869 7374 5f6d 6574 686f 6420 3d20  t_hist_method = 
-0000a200: 5174 5769 6467 6574 732e 5143 6f6d 626f  QtWidgets.QCombo
-0000a210: 426f 7828 7365 6c66 2e67 726f 7570 426f  Box(self.groupBo
-0000a220: 785f 6869 7374 6f67 7261 6d5f 7365 7474  x_histogram_sett
-0000a230: 696e 6773 290a 2020 2020 2020 2020 7365  ings).        se
-0000a240: 6c66 2e63 6f6d 626f 426f 785f 7265 7375  lf.comboBox_resu
-0000a250: 6c74 735f 6f62 735f 706c 6f74 5f68 6973  lts_obs_plot_his
-0000a260: 745f 6d65 7468 6f64 2e73 6574 4f62 6a65  t_method.setObje
-0000a270: 6374 4e61 6d65 2822 636f 6d62 6f42 6f78  ctName("comboBox
-0000a280: 5f72 6573 756c 7473 5f6f 6273 5f70 6c6f  _results_obs_plo
-0000a290: 745f 6869 7374 5f6d 6574 686f 6422 290a  t_hist_method").
-0000a2a0: 2020 2020 2020 2020 7365 6c66 2e66 6f72          self.for
-0000a2b0: 6d4c 6179 6f75 745f 382e 7365 7457 6964  mLayout_8.setWid
-0000a2c0: 6765 7428 302c 2051 7457 6964 6765 7473  get(0, QtWidgets
-0000a2d0: 2e51 466f 726d 4c61 796f 7574 2e46 6965  .QFormLayout.Fie
-0000a2e0: 6c64 526f 6c65 2c20 7365 6c66 2e63 6f6d  ldRole, self.com
-0000a2f0: 626f 426f 785f 7265 7375 6c74 735f 6f62  boBox_results_ob
-0000a300: 735f 706c 6f74 5f68 6973 745f 6d65 7468  s_plot_hist_meth
-0000a310: 6f64 290a 2020 2020 2020 2020 7365 6c66  od).        self
-0000a320: 2e6c 6162 656c 5f72 6573 756c 7473 5f6f  .label_results_o
-0000a330: 6273 5f70 6c6f 745f 6e75 6d62 6572 5f62  bs_plot_number_b
-0000a340: 696e 7320 3d20 5174 5769 6467 6574 732e  ins = QtWidgets.
-0000a350: 514c 6162 656c 2873 656c 662e 6772 6f75  QLabel(self.grou
-0000a360: 7042 6f78 5f68 6973 746f 6772 616d 5f73  pBox_histogram_s
-0000a370: 6574 7469 6e67 7329 0a20 2020 2020 2020  ettings).       
-0000a380: 2073 656c 662e 6c61 6265 6c5f 7265 7375   self.label_resu
-0000a390: 6c74 735f 6f62 735f 706c 6f74 5f6e 756d  lts_obs_plot_num
-0000a3a0: 6265 725f 6269 6e73 2e73 6574 4f62 6a65  ber_bins.setObje
-0000a3b0: 6374 4e61 6d65 2822 6c61 6265 6c5f 7265  ctName("label_re
-0000a3c0: 7375 6c74 735f 6f62 735f 706c 6f74 5f6e  sults_obs_plot_n
-0000a3d0: 756d 6265 725f 6269 6e73 2229 0a20 2020  umber_bins").   
-0000a3e0: 2020 2020 2073 656c 662e 666f 726d 4c61       self.formLa
-0000a3f0: 796f 7574 5f38 2e73 6574 5769 6467 6574  yout_8.setWidget
-0000a400: 2831 2c20 5174 5769 6467 6574 732e 5146  (1, QtWidgets.QF
-0000a410: 6f72 6d4c 6179 6f75 742e 4c61 6265 6c52  ormLayout.LabelR
-0000a420: 6f6c 652c 2073 656c 662e 6c61 6265 6c5f  ole, self.label_
-0000a430: 7265 7375 6c74 735f 6f62 735f 706c 6f74  results_obs_plot
-0000a440: 5f6e 756d 6265 725f 6269 6e73 290a 2020  _number_bins).  
-0000a450: 2020 2020 2020 7365 6c66 2e73 7069 6e42        self.spinB
-0000a460: 6f78 5f72 6573 756c 7473 5f6f 6273 5f70  ox_results_obs_p
-0000a470: 6c6f 745f 6e75 6d62 6572 5f62 696e 7320  lot_number_bins 
-0000a480: 3d20 5174 5769 6467 6574 732e 5153 7069  = QtWidgets.QSpi
-0000a490: 6e42 6f78 2873 656c 662e 6772 6f75 7042  nBox(self.groupB
-0000a4a0: 6f78 5f68 6973 746f 6772 616d 5f73 6574  ox_histogram_set
-0000a4b0: 7469 6e67 7329 0a20 2020 2020 2020 2073  tings).        s
-0000a4c0: 656c 662e 7370 696e 426f 785f 7265 7375  elf.spinBox_resu
-0000a4d0: 6c74 735f 6f62 735f 706c 6f74 5f6e 756d  lts_obs_plot_num
-0000a4e0: 6265 725f 6269 6e73 2e73 6574 4d69 6e69  ber_bins.setMini
-0000a4f0: 6d75 6d28 3229 0a20 2020 2020 2020 2073  mum(2).        s
-0000a500: 656c 662e 7370 696e 426f 785f 7265 7375  elf.spinBox_resu
-0000a510: 6c74 735f 6f62 735f 706c 6f74 5f6e 756d  lts_obs_plot_num
-0000a520: 6265 725f 6269 6e73 2e73 6574 4d61 7869  ber_bins.setMaxi
-0000a530: 6d75 6d28 3130 3030 290a 2020 2020 2020  mum(1000).      
-0000a540: 2020 7365 6c66 2e73 7069 6e42 6f78 5f72    self.spinBox_r
-0000a550: 6573 756c 7473 5f6f 6273 5f70 6c6f 745f  esults_obs_plot_
-0000a560: 6e75 6d62 6572 5f62 696e 732e 7365 7450  number_bins.setP
-0000a570: 726f 7065 7274 7928 2276 616c 7565 222c  roperty("value",
-0000a580: 2031 3029 0a20 2020 2020 2020 2073 656c   10).        sel
-0000a590: 662e 7370 696e 426f 785f 7265 7375 6c74  f.spinBox_result
-0000a5a0: 735f 6f62 735f 706c 6f74 5f6e 756d 6265  s_obs_plot_numbe
-0000a5b0: 725f 6269 6e73 2e73 6574 4f62 6a65 6374  r_bins.setObject
-0000a5c0: 4e61 6d65 2822 7370 696e 426f 785f 7265  Name("spinBox_re
-0000a5d0: 7375 6c74 735f 6f62 735f 706c 6f74 5f6e  sults_obs_plot_n
-0000a5e0: 756d 6265 725f 6269 6e73 2229 0a20 2020  umber_bins").   
-0000a5f0: 2020 2020 2073 656c 662e 666f 726d 4c61       self.formLa
-0000a600: 796f 7574 5f38 2e73 6574 5769 6467 6574  yout_8.setWidget
-0000a610: 2831 2c20 5174 5769 6467 6574 732e 5146  (1, QtWidgets.QF
-0000a620: 6f72 6d4c 6179 6f75 742e 4669 656c 6452  ormLayout.FieldR
-0000a630: 6f6c 652c 2073 656c 662e 7370 696e 426f  ole, self.spinBo
-0000a640: 785f 7265 7375 6c74 735f 6f62 735f 706c  x_results_obs_pl
-0000a650: 6f74 5f6e 756d 6265 725f 6269 6e73 290a  ot_number_bins).
-0000a660: 2020 2020 2020 2020 7365 6c66 2e76 6572          self.ver
-0000a670: 7469 6361 6c4c 6179 6f75 745f 3133 2e61  ticalLayout_13.a
-0000a680: 6464 4c61 796f 7574 2873 656c 662e 666f  ddLayout(self.fo
-0000a690: 726d 4c61 796f 7574 5f38 290a 2020 2020  rmLayout_8).    
-0000a6a0: 2020 2020 7365 6c66 2e63 6865 636b 426f      self.checkBo
-0000a6b0: 785f 7265 7375 6c74 735f 6f62 735f 706c  x_results_obs_pl
-0000a6c0: 6f74 5f73 686f 775f 6f75 746c 6965 7273  ot_show_outliers
-0000a6d0: 203d 2051 7457 6964 6765 7473 2e51 4368   = QtWidgets.QCh
-0000a6e0: 6563 6b42 6f78 2873 656c 662e 6772 6f75  eckBox(self.grou
-0000a6f0: 7042 6f78 5f68 6973 746f 6772 616d 5f73  pBox_histogram_s
-0000a700: 6574 7469 6e67 7329 0a20 2020 2020 2020  ettings).       
-0000a710: 2073 656c 662e 6368 6563 6b42 6f78 5f72   self.checkBox_r
-0000a720: 6573 756c 7473 5f6f 6273 5f70 6c6f 745f  esults_obs_plot_
-0000a730: 7368 6f77 5f6f 7574 6c69 6572 732e 7365  show_outliers.se
-0000a740: 7445 6e61 626c 6564 2846 616c 7365 290a  tEnabled(False).
-0000a750: 2020 2020 2020 2020 7365 6c66 2e63 6865          self.che
-0000a760: 636b 426f 785f 7265 7375 6c74 735f 6f62  ckBox_results_ob
-0000a770: 735f 706c 6f74 5f73 686f 775f 6f75 746c  s_plot_show_outl
-0000a780: 6965 7273 2e73 6574 4f62 6a65 6374 4e61  iers.setObjectNa
-0000a790: 6d65 2822 6368 6563 6b42 6f78 5f72 6573  me("checkBox_res
-0000a7a0: 756c 7473 5f6f 6273 5f70 6c6f 745f 7368  ults_obs_plot_sh
-0000a7b0: 6f77 5f6f 7574 6c69 6572 7322 290a 2020  ow_outliers").  
-0000a7c0: 2020 2020 2020 7365 6c66 2e76 6572 7469        self.verti
-0000a7d0: 6361 6c4c 6179 6f75 745f 3133 2e61 6464  calLayout_13.add
-0000a7e0: 5769 6467 6574 2873 656c 662e 6368 6563  Widget(self.chec
-0000a7f0: 6b42 6f78 5f72 6573 756c 7473 5f6f 6273  kBox_results_obs
-0000a800: 5f70 6c6f 745f 7368 6f77 5f6f 7574 6c69  _plot_show_outli
-0000a810: 6572 7329 0a20 2020 2020 2020 2073 656c  ers).        sel
-0000a820: 662e 686f 7269 7a6f 6e74 616c 4c61 796f  f.horizontalLayo
-0000a830: 7574 2e61 6464 5769 6467 6574 2873 656c  ut.addWidget(sel
-0000a840: 662e 6772 6f75 7042 6f78 5f68 6973 746f  f.groupBox_histo
-0000a850: 6772 616d 5f73 6574 7469 6e67 7329 0a20  gram_settings). 
-0000a860: 2020 2020 2020 2073 656c 662e 7665 7274         self.vert
-0000a870: 6963 616c 4c61 796f 7574 5f33 382e 6164  icalLayout_38.ad
-0000a880: 644c 6179 6f75 7428 7365 6c66 2e68 6f72  dLayout(self.hor
-0000a890: 697a 6f6e 7461 6c4c 6179 6f75 7429 0a20  izontalLayout). 
-0000a8a0: 2020 2020 2020 2073 656c 662e 7461 6257         self.tabW
-0000a8b0: 6964 6765 745f 7265 7375 6c74 732e 6164  idget_results.ad
-0000a8c0: 6454 6162 2873 656c 662e 7461 625f 7265  dTab(self.tab_re
-0000a8d0: 7375 6c74 735f 6f62 735f 706c 6f74 732c  sults_obs_plots,
-0000a8e0: 2022 2229 0a20 2020 2020 2020 2073 656c   "").        sel
-0000a8f0: 662e 7461 625f 7265 7375 6c74 735f 6472  f.tab_results_dr
-0000a900: 6966 7420 3d20 5174 5769 6467 6574 732e  ift = QtWidgets.
-0000a910: 5157 6964 6765 7428 290a 2020 2020 2020  QWidget().      
-0000a920: 2020 7365 6c66 2e74 6162 5f72 6573 756c    self.tab_resul
-0000a930: 7473 5f64 7269 6674 2e73 6574 4f62 6a65  ts_drift.setObje
-0000a940: 6374 4e61 6d65 2822 7461 625f 7265 7375  ctName("tab_resu
-0000a950: 6c74 735f 6472 6966 7422 290a 2020 2020  lts_drift").    
-0000a960: 2020 2020 7365 6c66 2e76 6572 7469 6361      self.vertica
-0000a970: 6c4c 6179 6f75 745f 3138 203d 2051 7457  lLayout_18 = QtW
-0000a980: 6964 6765 7473 2e51 5642 6f78 4c61 796f  idgets.QVBoxLayo
-0000a990: 7574 2873 656c 662e 7461 625f 7265 7375  ut(self.tab_resu
-0000a9a0: 6c74 735f 6472 6966 7429 0a20 2020 2020  lts_drift).     
-0000a9b0: 2020 2073 656c 662e 7665 7274 6963 616c     self.vertical
-0000a9c0: 4c61 796f 7574 5f31 382e 7365 744f 626a  Layout_18.setObj
-0000a9d0: 6563 744e 616d 6528 2276 6572 7469 6361  ectName("vertica
-0000a9e0: 6c4c 6179 6f75 745f 3138 2229 0a20 2020  lLayout_18").   
-0000a9f0: 2020 2020 2073 656c 662e 7461 626c 6556       self.tableV
-0000aa00: 6965 775f 7265 7375 6c74 735f 6472 6966  iew_results_drif
-0000aa10: 7420 3d20 5174 5769 6467 6574 732e 5154  t = QtWidgets.QT
-0000aa20: 6162 6c65 5669 6577 2873 656c 662e 7461  ableView(self.ta
-0000aa30: 625f 7265 7375 6c74 735f 6472 6966 7429  b_results_drift)
-0000aa40: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
-0000aa50: 626c 6556 6965 775f 7265 7375 6c74 735f  bleView_results_
-0000aa60: 6472 6966 742e 7365 744f 626a 6563 744e  drift.setObjectN
-0000aa70: 616d 6528 2274 6162 6c65 5669 6577 5f72  ame("tableView_r
-0000aa80: 6573 756c 7473 5f64 7269 6674 2229 0a20  esults_drift"). 
-0000aa90: 2020 2020 2020 2073 656c 662e 7665 7274         self.vert
-0000aaa0: 6963 616c 4c61 796f 7574 5f31 382e 6164  icalLayout_18.ad
-0000aab0: 6457 6964 6765 7428 7365 6c66 2e74 6162  dWidget(self.tab
-0000aac0: 6c65 5669 6577 5f72 6573 756c 7473 5f64  leView_results_d
-0000aad0: 7269 6674 290a 2020 2020 2020 2020 7365  rift).        se
-0000aae0: 6c66 2e74 6162 5769 6467 6574 5f72 6573  lf.tabWidget_res
-0000aaf0: 756c 7473 2e61 6464 5461 6228 7365 6c66  ults.addTab(self
-0000ab00: 2e74 6162 5f72 6573 756c 7473 5f64 7269  .tab_results_dri
-0000ab10: 6674 2c20 2222 290a 2020 2020 2020 2020  ft, "").        
-0000ab20: 7365 6c66 2e74 6162 5f72 6573 756c 7473  self.tab_results
-0000ab30: 5f64 7269 6674 706c 6f74 203d 2051 7457  _driftplot = QtW
-0000ab40: 6964 6765 7473 2e51 5769 6467 6574 2829  idgets.QWidget()
-0000ab50: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
-0000ab60: 625f 7265 7375 6c74 735f 6472 6966 7470  b_results_driftp
-0000ab70: 6c6f 742e 7365 744f 626a 6563 744e 616d  lot.setObjectNam
-0000ab80: 6528 2274 6162 5f72 6573 756c 7473 5f64  e("tab_results_d
-0000ab90: 7269 6674 706c 6f74 2229 0a20 2020 2020  riftplot").     
-0000aba0: 2020 2073 656c 662e 7665 7274 6963 616c     self.vertical
-0000abb0: 4c61 796f 7574 5f32 3920 3d20 5174 5769  Layout_29 = QtWi
-0000abc0: 6467 6574 732e 5156 426f 784c 6179 6f75  dgets.QVBoxLayou
-0000abd0: 7428 7365 6c66 2e74 6162 5f72 6573 756c  t(self.tab_resul
-0000abe0: 7473 5f64 7269 6674 706c 6f74 290a 2020  ts_driftplot).  
-0000abf0: 2020 2020 2020 7365 6c66 2e76 6572 7469        self.verti
-0000ac00: 6361 6c4c 6179 6f75 745f 3239 2e73 6574  calLayout_29.set
-0000ac10: 4f62 6a65 6374 4e61 6d65 2822 7665 7274  ObjectName("vert
-0000ac20: 6963 616c 4c61 796f 7574 5f32 3922 290a  icalLayout_29").
-0000ac30: 2020 2020 2020 2020 7365 6c66 2e76 6572          self.ver
-0000ac40: 7469 6361 6c4c 6179 6f75 745f 3237 203d  ticalLayout_27 =
-0000ac50: 2051 7457 6964 6765 7473 2e51 5642 6f78   QtWidgets.QVBox
-0000ac60: 4c61 796f 7574 2829 0a20 2020 2020 2020  Layout().       
-0000ac70: 2073 656c 662e 7665 7274 6963 616c 4c61   self.verticalLa
-0000ac80: 796f 7574 5f32 372e 7365 744f 626a 6563  yout_27.setObjec
-0000ac90: 744e 616d 6528 2276 6572 7469 6361 6c4c  tName("verticalL
-0000aca0: 6179 6f75 745f 3237 2229 0a20 2020 2020  ayout_27").     
-0000acb0: 2020 2073 656c 662e 6772 6170 6869 6373     self.graphics
-0000acc0: 4c61 796f 7574 5769 6467 6574 5f72 6573  LayoutWidget_res
-0000acd0: 756c 7473 5f64 7269 6674 5f70 6c6f 7420  ults_drift_plot 
-0000ace0: 3d20 4772 6170 6869 6373 4c61 796f 7574  = GraphicsLayout
-0000acf0: 5769 6467 6574 2873 656c 662e 7461 625f  Widget(self.tab_
-0000ad00: 7265 7375 6c74 735f 6472 6966 7470 6c6f  results_driftplo
-0000ad10: 7429 0a20 2020 2020 2020 2073 656c 662e  t).        self.
-0000ad20: 6772 6170 6869 6373 4c61 796f 7574 5769  graphicsLayoutWi
-0000ad30: 6467 6574 5f72 6573 756c 7473 5f64 7269  dget_results_dri
-0000ad40: 6674 5f70 6c6f 742e 7365 744f 626a 6563  ft_plot.setObjec
-0000ad50: 744e 616d 6528 2267 7261 7068 6963 734c  tName("graphicsL
-0000ad60: 6179 6f75 7457 6964 6765 745f 7265 7375  ayoutWidget_resu
-0000ad70: 6c74 735f 6472 6966 745f 706c 6f74 2229  lts_drift_plot")
-0000ad80: 0a20 2020 2020 2020 2073 656c 662e 7665  .        self.ve
-0000ad90: 7274 6963 616c 4c61 796f 7574 5f32 372e  rticalLayout_27.
-0000ada0: 6164 6457 6964 6765 7428 7365 6c66 2e67  addWidget(self.g
-0000adb0: 7261 7068 6963 734c 6179 6f75 7457 6964  raphicsLayoutWid
-0000adc0: 6765 745f 7265 7375 6c74 735f 6472 6966  get_results_drif
-0000add0: 745f 706c 6f74 290a 2020 2020 2020 2020  t_plot).        
-0000ade0: 7365 6c66 2e67 726f 7570 426f 785f 7265  self.groupBox_re
-0000adf0: 7375 6c74 735f 6472 6966 745f 706c 6f74  sults_drift_plot
-0000ae00: 203d 2051 7457 6964 6765 7473 2e51 4772   = QtWidgets.QGr
-0000ae10: 6f75 7042 6f78 2873 656c 662e 7461 625f  oupBox(self.tab_
-0000ae20: 7265 7375 6c74 735f 6472 6966 7470 6c6f  results_driftplo
-0000ae30: 7429 0a20 2020 2020 2020 2073 656c 662e  t).        self.
-0000ae40: 6772 6f75 7042 6f78 5f72 6573 756c 7473  groupBox_results
-0000ae50: 5f64 7269 6674 5f70 6c6f 742e 7365 7445  _drift_plot.setE
-0000ae60: 6e61 626c 6564 2854 7275 6529 0a20 2020  nabled(True).   
-0000ae70: 2020 2020 2073 656c 662e 6772 6f75 7042       self.groupB
-0000ae80: 6f78 5f72 6573 756c 7473 5f64 7269 6674  ox_results_drift
-0000ae90: 5f70 6c6f 742e 7365 744f 626a 6563 744e  _plot.setObjectN
-0000aea0: 616d 6528 2267 726f 7570 426f 785f 7265  ame("groupBox_re
-0000aeb0: 7375 6c74 735f 6472 6966 745f 706c 6f74  sults_drift_plot
-0000aec0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-0000aed0: 7665 7274 6963 616c 4c61 796f 7574 5f32  verticalLayout_2
-0000aee0: 3620 3d20 5174 5769 6467 6574 732e 5156  6 = QtWidgets.QV
-0000aef0: 426f 784c 6179 6f75 7428 7365 6c66 2e67  BoxLayout(self.g
-0000af00: 726f 7570 426f 785f 7265 7375 6c74 735f  roupBox_results_
-0000af10: 6472 6966 745f 706c 6f74 290a 2020 2020  drift_plot).    
-0000af20: 2020 2020 7365 6c66 2e76 6572 7469 6361      self.vertica
-0000af30: 6c4c 6179 6f75 745f 3236 2e73 6574 4f62  lLayout_26.setOb
-0000af40: 6a65 6374 4e61 6d65 2822 7665 7274 6963  jectName("vertic
-0000af50: 616c 4c61 796f 7574 5f32 3622 290a 2020  alLayout_26").  
-0000af60: 2020 2020 2020 7365 6c66 2e66 6f72 6d4c        self.formL
-0000af70: 6179 6f75 745f 3520 3d20 5174 5769 6467  ayout_5 = QtWidg
-0000af80: 6574 732e 5146 6f72 6d4c 6179 6f75 7428  ets.QFormLayout(
-0000af90: 290a 2020 2020 2020 2020 7365 6c66 2e66  ).        self.f
-0000afa0: 6f72 6d4c 6179 6f75 745f 352e 7365 744f  ormLayout_5.setO
-0000afb0: 626a 6563 744e 616d 6528 2266 6f72 6d4c  bjectName("formL
-0000afc0: 6179 6f75 745f 3522 290a 2020 2020 2020  ayout_5").      
-0000afd0: 2020 7365 6c66 2e6c 6162 656c 5f72 6573    self.label_res
-0000afe0: 756c 7473 5f64 7269 6674 5f70 6c6f 745f  ults_drift_plot_
-0000aff0: 765f 6f66 6673 6574 203d 2051 7457 6964  v_offset = QtWid
-0000b000: 6765 7473 2e51 4c61 6265 6c28 7365 6c66  gets.QLabel(self
-0000b010: 2e67 726f 7570 426f 785f 7265 7375 6c74  .groupBox_result
-0000b020: 735f 6472 6966 745f 706c 6f74 290a 2020  s_drift_plot).  
-0000b030: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
-0000b040: 5f72 6573 756c 7473 5f64 7269 6674 5f70  _results_drift_p
-0000b050: 6c6f 745f 765f 6f66 6673 6574 2e73 6574  lot_v_offset.set
-0000b060: 456e 6162 6c65 6428 4661 6c73 6529 0a20  Enabled(False). 
-0000b070: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
-0000b080: 6c5f 7265 7375 6c74 735f 6472 6966 745f  l_results_drift_
-0000b090: 706c 6f74 5f76 5f6f 6666 7365 742e 7365  plot_v_offset.se
-0000b0a0: 744f 626a 6563 744e 616d 6528 226c 6162  tObjectName("lab
-0000b0b0: 656c 5f72 6573 756c 7473 5f64 7269 6674  el_results_drift
-0000b0c0: 5f70 6c6f 745f 765f 6f66 6673 6574 2229  _plot_v_offset")
-0000b0d0: 0a20 2020 2020 2020 2073 656c 662e 666f  .        self.fo
-0000b0e0: 726d 4c61 796f 7574 5f35 2e73 6574 5769  rmLayout_5.setWi
-0000b0f0: 6467 6574 2830 2c20 5174 5769 6467 6574  dget(0, QtWidget
-0000b100: 732e 5146 6f72 6d4c 6179 6f75 742e 4c61  s.QFormLayout.La
-0000b110: 6265 6c52 6f6c 652c 2073 656c 662e 6c61  belRole, self.la
-0000b120: 6265 6c5f 7265 7375 6c74 735f 6472 6966  bel_results_drif
-0000b130: 745f 706c 6f74 5f76 5f6f 6666 7365 7429  t_plot_v_offset)
-0000b140: 0a20 2020 2020 2020 2073 656c 662e 7370  .        self.sp
-0000b150: 696e 426f 785f 7265 7375 6c74 735f 6472  inBox_results_dr
-0000b160: 6966 745f 706c 6f74 5f76 5f6f 6666 7365  ift_plot_v_offse
-0000b170: 7420 3d20 5174 5769 6467 6574 732e 5153  t = QtWidgets.QS
-0000b180: 7069 6e42 6f78 2873 656c 662e 6772 6f75  pinBox(self.grou
-0000b190: 7042 6f78 5f72 6573 756c 7473 5f64 7269  pBox_results_dri
-0000b1a0: 6674 5f70 6c6f 7429 0a20 2020 2020 2020  ft_plot).       
-0000b1b0: 2073 656c 662e 7370 696e 426f 785f 7265   self.spinBox_re
-0000b1c0: 7375 6c74 735f 6472 6966 745f 706c 6f74  sults_drift_plot
-0000b1d0: 5f76 5f6f 6666 7365 742e 7365 7445 6e61  _v_offset.setEna
-0000b1e0: 626c 6564 2846 616c 7365 290a 2020 2020  bled(False).    
-0000b1f0: 2020 2020 7365 6c66 2e73 7069 6e42 6f78      self.spinBox
-0000b200: 5f72 6573 756c 7473 5f64 7269 6674 5f70  _results_drift_p
-0000b210: 6c6f 745f 765f 6f66 6673 6574 2e73 6574  lot_v_offset.set
-0000b220: 4d69 6e69 6d75 6d28 2d31 3030 3029 0a20  Minimum(-1000). 
-0000b230: 2020 2020 2020 2073 656c 662e 7370 696e         self.spin
-0000b240: 426f 785f 7265 7375 6c74 735f 6472 6966  Box_results_drif
-0000b250: 745f 706c 6f74 5f76 5f6f 6666 7365 742e  t_plot_v_offset.
-0000b260: 7365 744d 6178 696d 756d 2831 3030 3029  setMaximum(1000)
-0000b270: 0a20 2020 2020 2020 2073 656c 662e 7370  .        self.sp
-0000b280: 696e 426f 785f 7265 7375 6c74 735f 6472  inBox_results_dr
-0000b290: 6966 745f 706c 6f74 5f76 5f6f 6666 7365  ift_plot_v_offse
-0000b2a0: 742e 7365 744f 626a 6563 744e 616d 6528  t.setObjectName(
-0000b2b0: 2273 7069 6e42 6f78 5f72 6573 756c 7473  "spinBox_results
-0000b2c0: 5f64 7269 6674 5f70 6c6f 745f 765f 6f66  _drift_plot_v_of
-0000b2d0: 6673 6574 2229 0a20 2020 2020 2020 2073  fset").        s
-0000b2e0: 656c 662e 666f 726d 4c61 796f 7574 5f35  elf.formLayout_5
-0000b2f0: 2e73 6574 5769 6467 6574 2830 2c20 5174  .setWidget(0, Qt
-0000b300: 5769 6467 6574 732e 5146 6f72 6d4c 6179  Widgets.QFormLay
-0000b310: 6f75 742e 4669 656c 6452 6f6c 652c 2073  out.FieldRole, s
-0000b320: 656c 662e 7370 696e 426f 785f 7265 7375  elf.spinBox_resu
-0000b330: 6c74 735f 6472 6966 745f 706c 6f74 5f76  lts_drift_plot_v
-0000b340: 5f6f 6666 7365 7429 0a20 2020 2020 2020  _offset).       
-0000b350: 2073 656c 662e 7665 7274 6963 616c 4c61   self.verticalLa
-0000b360: 796f 7574 5f32 362e 6164 644c 6179 6f75  yout_26.addLayou
-0000b370: 7428 7365 6c66 2e66 6f72 6d4c 6179 6f75  t(self.formLayou
-0000b380: 745f 3529 0a20 2020 2020 2020 2073 656c  t_5).        sel
-0000b390: 662e 7665 7274 6963 616c 4c61 796f 7574  f.verticalLayout
-0000b3a0: 5f32 372e 6164 6457 6964 6765 7428 7365  _27.addWidget(se
-0000b3b0: 6c66 2e67 726f 7570 426f 785f 7265 7375  lf.groupBox_resu
-0000b3c0: 6c74 735f 6472 6966 745f 706c 6f74 290a  lts_drift_plot).
-0000b3d0: 2020 2020 2020 2020 7365 6c66 2e76 6572          self.ver
-0000b3e0: 7469 6361 6c4c 6179 6f75 745f 3239 2e61  ticalLayout_29.a
-0000b3f0: 6464 4c61 796f 7574 2873 656c 662e 7665  ddLayout(self.ve
-0000b400: 7274 6963 616c 4c61 796f 7574 5f32 3729  rticalLayout_27)
-0000b410: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
-0000b420: 6257 6964 6765 745f 7265 7375 6c74 732e  bWidget_results.
-0000b430: 6164 6454 6162 2873 656c 662e 7461 625f  addTab(self.tab_
-0000b440: 7265 7375 6c74 735f 6472 6966 7470 6c6f  results_driftplo
-0000b450: 742c 2022 2229 0a20 2020 2020 2020 2073  t, "").        s
-0000b460: 656c 662e 7461 625f 7265 7375 6c74 735f  elf.tab_results_
-0000b470: 7374 6174 5f74 6162 6c65 203d 2051 7457  stat_table = QtW
-0000b480: 6964 6765 7473 2e51 5769 6467 6574 2829  idgets.QWidget()
-0000b490: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
-0000b4a0: 625f 7265 7375 6c74 735f 7374 6174 5f74  b_results_stat_t
-0000b4b0: 6162 6c65 2e73 6574 4f62 6a65 6374 4e61  able.setObjectNa
-0000b4c0: 6d65 2822 7461 625f 7265 7375 6c74 735f  me("tab_results_
-0000b4d0: 7374 6174 5f74 6162 6c65 2229 0a20 2020  stat_table").   
-0000b4e0: 2020 2020 2073 656c 662e 7665 7274 6963       self.vertic
-0000b4f0: 616c 4c61 796f 7574 5f33 3920 3d20 5174  alLayout_39 = Qt
-0000b500: 5769 6467 6574 732e 5156 426f 784c 6179  Widgets.QVBoxLay
-0000b510: 6f75 7428 7365 6c66 2e74 6162 5f72 6573  out(self.tab_res
-0000b520: 756c 7473 5f73 7461 745f 7461 626c 6529  ults_stat_table)
-0000b530: 0a20 2020 2020 2020 2073 656c 662e 7665  .        self.ve
-0000b540: 7274 6963 616c 4c61 796f 7574 5f33 392e  rticalLayout_39.
-0000b550: 7365 744f 626a 6563 744e 616d 6528 2276  setObjectName("v
-0000b560: 6572 7469 6361 6c4c 6179 6f75 745f 3339  erticalLayout_39
-0000b570: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-0000b580: 7461 626c 6556 6965 775f 7265 7375 6c74  tableView_result
-0000b590: 735f 7374 6174 696f 6e73 203d 2051 7457  s_stations = QtW
-0000b5a0: 6964 6765 7473 2e51 5461 626c 6556 6965  idgets.QTableVie
-0000b5b0: 7728 7365 6c66 2e74 6162 5f72 6573 756c  w(self.tab_resul
-0000b5c0: 7473 5f73 7461 745f 7461 626c 6529 0a20  ts_stat_table). 
-0000b5d0: 2020 2020 2020 2073 656c 662e 7461 626c         self.tabl
-0000b5e0: 6556 6965 775f 7265 7375 6c74 735f 7374  eView_results_st
-0000b5f0: 6174 696f 6e73 2e73 6574 4f62 6a65 6374  ations.setObject
-0000b600: 4e61 6d65 2822 7461 626c 6556 6965 775f  Name("tableView_
-0000b610: 7265 7375 6c74 735f 7374 6174 696f 6e73  results_stations
-0000b620: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-0000b630: 7665 7274 6963 616c 4c61 796f 7574 5f33  verticalLayout_3
-0000b640: 392e 6164 6457 6964 6765 7428 7365 6c66  9.addWidget(self
-0000b650: 2e74 6162 6c65 5669 6577 5f72 6573 756c  .tableView_resul
-0000b660: 7473 5f73 7461 7469 6f6e 7329 0a20 2020  ts_stations).   
-0000b670: 2020 2020 2073 656c 662e 6772 6f75 7042       self.groupB
-0000b680: 6f78 5f72 6573 756c 7473 5f73 7461 7469  ox_results_stati
-0000b690: 6f6e 735f 7374 6174 6973 7469 6373 203d  ons_statistics =
-0000b6a0: 2051 7457 6964 6765 7473 2e51 4772 6f75   QtWidgets.QGrou
-0000b6b0: 7042 6f78 2873 656c 662e 7461 625f 7265  pBox(self.tab_re
-0000b6c0: 7375 6c74 735f 7374 6174 5f74 6162 6c65  sults_stat_table
-0000b6d0: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
-0000b6e0: 726f 7570 426f 785f 7265 7375 6c74 735f  roupBox_results_
-0000b6f0: 7374 6174 696f 6e73 5f73 7461 7469 7374  stations_statist
-0000b700: 6963 732e 7365 744f 626a 6563 744e 616d  ics.setObjectNam
-0000b710: 6528 2267 726f 7570 426f 785f 7265 7375  e("groupBox_resu
-0000b720: 6c74 735f 7374 6174 696f 6e73 5f73 7461  lts_stations_sta
-0000b730: 7469 7374 6963 7322 290a 2020 2020 2020  tistics").      
-0000b740: 2020 7365 6c66 2e68 6f72 697a 6f6e 7461    self.horizonta
-0000b750: 6c4c 6179 6f75 745f 3420 3d20 5174 5769  lLayout_4 = QtWi
-0000b760: 6467 6574 732e 5148 426f 784c 6179 6f75  dgets.QHBoxLayou
-0000b770: 7428 7365 6c66 2e67 726f 7570 426f 785f  t(self.groupBox_
-0000b780: 7265 7375 6c74 735f 7374 6174 696f 6e73  results_stations
-0000b790: 5f73 7461 7469 7374 6963 7329 0a20 2020  _statistics).   
-0000b7a0: 2020 2020 2073 656c 662e 686f 7269 7a6f       self.horizo
-0000b7b0: 6e74 616c 4c61 796f 7574 5f34 2e73 6574  ntalLayout_4.set
-0000b7c0: 4f62 6a65 6374 4e61 6d65 2822 686f 7269  ObjectName("hori
-0000b7d0: 7a6f 6e74 616c 4c61 796f 7574 5f34 2229  zontalLayout_4")
-0000b7e0: 0a20 2020 2020 2020 2073 656c 662e 7665  .        self.ve
-0000b7f0: 7274 6963 616c 4c61 796f 7574 5f31 3920  rticalLayout_19 
-0000b800: 3d20 5174 5769 6467 6574 732e 5156 426f  = QtWidgets.QVBo
-0000b810: 784c 6179 6f75 7428 290a 2020 2020 2020  xLayout().      
-0000b820: 2020 7365 6c66 2e76 6572 7469 6361 6c4c    self.verticalL
-0000b830: 6179 6f75 745f 3139 2e73 6574 4f62 6a65  ayout_19.setObje
-0000b840: 6374 4e61 6d65 2822 7665 7274 6963 616c  ctName("vertical
-0000b850: 4c61 796f 7574 5f31 3922 290a 2020 2020  Layout_19").    
-0000b860: 2020 2020 7365 6c66 2e6c 6162 656c 5f31      self.label_1
-0000b870: 3220 3d20 5174 5769 6467 6574 732e 514c  2 = QtWidgets.QL
-0000b880: 6162 656c 2873 656c 662e 6772 6f75 7042  abel(self.groupB
-0000b890: 6f78 5f72 6573 756c 7473 5f73 7461 7469  ox_results_stati
-0000b8a0: 6f6e 735f 7374 6174 6973 7469 6373 290a  ons_statistics).
-0000b8b0: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
-0000b8c0: 656c 5f31 322e 7365 744f 626a 6563 744e  el_12.setObjectN
-0000b8d0: 616d 6528 226c 6162 656c 5f31 3222 290a  ame("label_12").
-0000b8e0: 2020 2020 2020 2020 7365 6c66 2e76 6572          self.ver
-0000b8f0: 7469 6361 6c4c 6179 6f75 745f 3139 2e61  ticalLayout_19.a
-0000b900: 6464 5769 6467 6574 2873 656c 662e 6c61  ddWidget(self.la
-0000b910: 6265 6c5f 3132 290a 2020 2020 2020 2020  bel_12).        
-0000b920: 7365 6c66 2e63 6f6d 626f 426f 785f 7265  self.comboBox_re
-0000b930: 7375 6c74 735f 7374 6174 696f 6e73 5f73  sults_stations_s
-0000b940: 7461 7469 7374 6963 735f 7365 6c65 6374  tatistics_select
-0000b950: 5f63 6f6c 203d 2051 7457 6964 6765 7473  _col = QtWidgets
-0000b960: 2e51 436f 6d62 6f42 6f78 2873 656c 662e  .QComboBox(self.
-0000b970: 6772 6f75 7042 6f78 5f72 6573 756c 7473  groupBox_results
-0000b980: 5f73 7461 7469 6f6e 735f 7374 6174 6973  _stations_statis
-0000b990: 7469 6373 290a 2020 2020 2020 2020 7365  tics).        se
-0000b9a0: 6c66 2e63 6f6d 626f 426f 785f 7265 7375  lf.comboBox_resu
-0000b9b0: 6c74 735f 7374 6174 696f 6e73 5f73 7461  lts_stations_sta
-0000b9c0: 7469 7374 6963 735f 7365 6c65 6374 5f63  tistics_select_c
-0000b9d0: 6f6c 2e73 6574 4f62 6a65 6374 4e61 6d65  ol.setObjectName
-0000b9e0: 2822 636f 6d62 6f42 6f78 5f72 6573 756c  ("comboBox_resul
-0000b9f0: 7473 5f73 7461 7469 6f6e 735f 7374 6174  ts_stations_stat
-0000ba00: 6973 7469 6373 5f73 656c 6563 745f 636f  istics_select_co
-0000ba10: 6c22 290a 2020 2020 2020 2020 7365 6c66  l").        self
-0000ba20: 2e76 6572 7469 6361 6c4c 6179 6f75 745f  .verticalLayout_
-0000ba30: 3139 2e61 6464 5769 6467 6574 2873 656c  19.addWidget(sel
-0000ba40: 662e 636f 6d62 6f42 6f78 5f72 6573 756c  f.comboBox_resul
-0000ba50: 7473 5f73 7461 7469 6f6e 735f 7374 6174  ts_stations_stat
-0000ba60: 6973 7469 6373 5f73 656c 6563 745f 636f  istics_select_co
-0000ba70: 6c29 0a20 2020 2020 2020 2073 656c 662e  l).        self.
-0000ba80: 686f 7269 7a6f 6e74 616c 4c61 796f 7574  horizontalLayout
-0000ba90: 5f34 2e61 6464 4c61 796f 7574 2873 656c  _4.addLayout(sel
-0000baa0: 662e 7665 7274 6963 616c 4c61 796f 7574  f.verticalLayout
-0000bab0: 5f31 3929 0a20 2020 2020 2020 2073 656c  _19).        sel
-0000bac0: 662e 666f 726d 4c61 796f 7574 5f39 203d  f.formLayout_9 =
-0000bad0: 2051 7457 6964 6765 7473 2e51 466f 726d   QtWidgets.QForm
-0000bae0: 4c61 796f 7574 2829 0a20 2020 2020 2020  Layout().       
-0000baf0: 2073 656c 662e 666f 726d 4c61 796f 7574   self.formLayout
-0000bb00: 5f39 2e73 6574 4f62 6a65 6374 4e61 6d65  _9.setObjectName
-0000bb10: 2822 666f 726d 4c61 796f 7574 5f39 2229  ("formLayout_9")
-0000bb20: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
-0000bb30: 6265 6c5f 3133 203d 2051 7457 6964 6765  bel_13 = QtWidge
-0000bb40: 7473 2e51 4c61 6265 6c28 7365 6c66 2e67  ts.QLabel(self.g
-0000bb50: 726f 7570 426f 785f 7265 7375 6c74 735f  roupBox_results_
-0000bb60: 7374 6174 696f 6e73 5f73 7461 7469 7374  stations_statist
-0000bb70: 6963 7329 0a20 2020 2020 2020 2073 656c  ics).        sel
-0000bb80: 662e 6c61 6265 6c5f 3133 2e73 6574 4f62  f.label_13.setOb
-0000bb90: 6a65 6374 4e61 6d65 2822 6c61 6265 6c5f  jectName("label_
-0000bba0: 3133 2229 0a20 2020 2020 2020 2073 656c  13").        sel
-0000bbb0: 662e 666f 726d 4c61 796f 7574 5f39 2e73  f.formLayout_9.s
-0000bbc0: 6574 5769 6467 6574 2830 2c20 5174 5769  etWidget(0, QtWi
-0000bbd0: 6467 6574 732e 5146 6f72 6d4c 6179 6f75  dgets.QFormLayou
-0000bbe0: 742e 4c61 6265 6c52 6f6c 652c 2073 656c  t.LabelRole, sel
-0000bbf0: 662e 6c61 6265 6c5f 3133 290a 2020 2020  f.label_13).    
-0000bc00: 2020 2020 7365 6c66 2e6c 6162 656c 5f72      self.label_r
-0000bc10: 6573 756c 7473 5f73 7461 7469 6f6e 735f  esults_stations_
-0000bc20: 7374 6174 6973 7469 6373 5f6d 6561 6e20  statistics_mean 
-0000bc30: 3d20 5174 5769 6467 6574 732e 514c 6162  = QtWidgets.QLab
-0000bc40: 656c 2873 656c 662e 6772 6f75 7042 6f78  el(self.groupBox
-0000bc50: 5f72 6573 756c 7473 5f73 7461 7469 6f6e  _results_station
-0000bc60: 735f 7374 6174 6973 7469 6373 290a 2020  s_statistics).  
-0000bc70: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
-0000bc80: 5f72 6573 756c 7473 5f73 7461 7469 6f6e  _results_station
-0000bc90: 735f 7374 6174 6973 7469 6373 5f6d 6561  s_statistics_mea
-0000bca0: 6e2e 7365 7454 6578 7428 2222 290a 2020  n.setText("").  
-0000bcb0: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
-0000bcc0: 5f72 6573 756c 7473 5f73 7461 7469 6f6e  _results_station
-0000bcd0: 735f 7374 6174 6973 7469 6373 5f6d 6561  s_statistics_mea
-0000bce0: 6e2e 7365 744f 626a 6563 744e 616d 6528  n.setObjectName(
-0000bcf0: 226c 6162 656c 5f72 6573 756c 7473 5f73  "label_results_s
-0000bd00: 7461 7469 6f6e 735f 7374 6174 6973 7469  tations_statisti
-0000bd10: 6373 5f6d 6561 6e22 290a 2020 2020 2020  cs_mean").      
-0000bd20: 2020 7365 6c66 2e66 6f72 6d4c 6179 6f75    self.formLayou
-0000bd30: 745f 392e 7365 7457 6964 6765 7428 302c  t_9.setWidget(0,
-0000bd40: 2051 7457 6964 6765 7473 2e51 466f 726d   QtWidgets.QForm
-0000bd50: 4c61 796f 7574 2e46 6965 6c64 526f 6c65  Layout.FieldRole
-0000bd60: 2c20 7365 6c66 2e6c 6162 656c 5f72 6573  , self.label_res
-0000bd70: 756c 7473 5f73 7461 7469 6f6e 735f 7374  ults_stations_st
-0000bd80: 6174 6973 7469 6373 5f6d 6561 6e29 0a20  atistics_mean). 
-0000bd90: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
-0000bda0: 6c5f 3134 203d 2051 7457 6964 6765 7473  l_14 = QtWidgets
-0000bdb0: 2e51 4c61 6265 6c28 7365 6c66 2e67 726f  .QLabel(self.gro
-0000bdc0: 7570 426f 785f 7265 7375 6c74 735f 7374  upBox_results_st
-0000bdd0: 6174 696f 6e73 5f73 7461 7469 7374 6963  ations_statistic
-0000bde0: 7329 0a20 2020 2020 2020 2073 656c 662e  s).        self.
-0000bdf0: 6c61 6265 6c5f 3134 2e73 6574 4f62 6a65  label_14.setObje
-0000be00: 6374 4e61 6d65 2822 6c61 6265 6c5f 3134  ctName("label_14
-0000be10: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-0000be20: 666f 726d 4c61 796f 7574 5f39 2e73 6574  formLayout_9.set
-0000be30: 5769 6467 6574 2831 2c20 5174 5769 6467  Widget(1, QtWidg
-0000be40: 6574 732e 5146 6f72 6d4c 6179 6f75 742e  ets.QFormLayout.
-0000be50: 4c61 6265 6c52 6f6c 652c 2073 656c 662e  LabelRole, self.
-0000be60: 6c61 6265 6c5f 3134 290a 2020 2020 2020  label_14).      
-0000be70: 2020 7365 6c66 2e6c 6162 656c 5f72 6573    self.label_res
+000078e0: 7665 7274 6963 616c 4c61 796f 7574 5f33  verticalLayout_3
+000078f0: 3622 290a 2020 2020 2020 2020 7365 6c66  6").        self
+00007900: 2e70 7573 6842 7574 746f 6e5f 7265 7375  .pushButton_resu
+00007910: 6c74 735f 6578 706f 7274 5f73 6861 7065  lts_export_shape
+00007920: 6669 6c65 203d 2051 7457 6964 6765 7473  file = QtWidgets
+00007930: 2e51 5075 7368 4275 7474 6f6e 2873 656c  .QPushButton(sel
+00007940: 662e 6772 6f75 7042 6f78 5f67 6973 5f64  f.groupBox_gis_d
+00007950: 6174 6129 0a20 2020 2020 2020 2073 656c  ata).        sel
+00007960: 662e 7075 7368 4275 7474 6f6e 5f72 6573  f.pushButton_res
+00007970: 756c 7473 5f65 7870 6f72 745f 7368 6170  ults_export_shap
+00007980: 6566 696c 652e 7365 744f 626a 6563 744e  efile.setObjectN
+00007990: 616d 6528 2270 7573 6842 7574 746f 6e5f  ame("pushButton_
+000079a0: 7265 7375 6c74 735f 6578 706f 7274 5f73  results_export_s
+000079b0: 6861 7065 6669 6c65 2229 0a20 2020 2020  hapefile").     
+000079c0: 2020 2073 656c 662e 7665 7274 6963 616c     self.vertical
+000079d0: 4c61 796f 7574 5f33 362e 6164 6457 6964  Layout_36.addWid
+000079e0: 6765 7428 7365 6c66 2e70 7573 6842 7574  get(self.pushBut
+000079f0: 746f 6e5f 7265 7375 6c74 735f 6578 706f  ton_results_expo
+00007a00: 7274 5f73 6861 7065 6669 6c65 290a 2020  rt_shapefile).  
+00007a10: 2020 2020 2020 7365 6c66 2e66 6f72 6d4c        self.formL
+00007a20: 6179 6f75 745f 3720 3d20 5174 5769 6467  ayout_7 = QtWidg
+00007a30: 6574 732e 5146 6f72 6d4c 6179 6f75 7428  ets.QFormLayout(
+00007a40: 290a 2020 2020 2020 2020 7365 6c66 2e66  ).        self.f
+00007a50: 6f72 6d4c 6179 6f75 745f 372e 7365 744f  ormLayout_7.setO
+00007a60: 626a 6563 744e 616d 6528 2266 6f72 6d4c  bjectName("formL
+00007a70: 6179 6f75 745f 3722 290a 2020 2020 2020  ayout_7").      
+00007a80: 2020 7365 6c66 2e76 6572 7469 6361 6c4c    self.verticalL
+00007a90: 6179 6f75 745f 3336 2e61 6464 4c61 796f  ayout_36.addLayo
+00007aa0: 7574 2873 656c 662e 666f 726d 4c61 796f  ut(self.formLayo
+00007ab0: 7574 5f37 290a 2020 2020 2020 2020 7365  ut_7).        se
+00007ac0: 6c66 2e76 6572 7469 6361 6c4c 6179 6f75  lf.verticalLayou
+00007ad0: 745f 3132 2e61 6464 5769 6467 6574 2873  t_12.addWidget(s
+00007ae0: 656c 662e 6772 6f75 7042 6f78 5f67 6973  elf.groupBox_gis
+00007af0: 5f64 6174 6129 0a20 2020 2020 2020 2073  _data).        s
+00007b00: 7061 6365 7249 7465 6d32 203d 2051 7457  pacerItem2 = QtW
+00007b10: 6964 6765 7473 2e51 5370 6163 6572 4974  idgets.QSpacerIt
+00007b20: 656d 2832 302c 2034 302c 2051 7457 6964  em(20, 40, QtWid
+00007b30: 6765 7473 2e51 5369 7a65 506f 6c69 6379  gets.QSizePolicy
+00007b40: 2e4d 696e 696d 756d 2c20 5174 5769 6467  .Minimum, QtWidg
+00007b50: 6574 732e 5153 697a 6550 6f6c 6963 792e  ets.QSizePolicy.
+00007b60: 4578 7061 6e64 696e 6729 0a20 2020 2020  Expanding).     
+00007b70: 2020 2073 656c 662e 7665 7274 6963 616c     self.vertical
+00007b80: 4c61 796f 7574 5f31 322e 6164 6449 7465  Layout_12.addIte
+00007b90: 6d28 7370 6163 6572 4974 656d 3229 0a20  m(spacerItem2). 
+00007ba0: 2020 2020 2020 2073 656c 662e 7461 6257         self.tabW
+00007bb0: 6964 6765 745f 7265 7375 6c74 7320 3d20  idget_results = 
+00007bc0: 5174 5769 6467 6574 732e 5154 6162 5769  QtWidgets.QTabWi
+00007bd0: 6467 6574 2873 656c 662e 7370 6c69 7474  dget(self.splitt
+00007be0: 6572 5f72 6573 756c 7473 290a 2020 2020  er_results).    
+00007bf0: 2020 2020 7369 7a65 506f 6c69 6379 203d      sizePolicy =
+00007c00: 2051 7457 6964 6765 7473 2e51 5369 7a65   QtWidgets.QSize
+00007c10: 506f 6c69 6379 2851 7457 6964 6765 7473  Policy(QtWidgets
+00007c20: 2e51 5369 7a65 506f 6c69 6379 2e45 7870  .QSizePolicy.Exp
+00007c30: 616e 6469 6e67 2c20 5174 5769 6467 6574  anding, QtWidget
+00007c40: 732e 5153 697a 6550 6f6c 6963 792e 4578  s.QSizePolicy.Ex
+00007c50: 7061 6e64 696e 6729 0a20 2020 2020 2020  panding).       
+00007c60: 2073 697a 6550 6f6c 6963 792e 7365 7448   sizePolicy.setH
+00007c70: 6f72 697a 6f6e 7461 6c53 7472 6574 6368  orizontalStretch
+00007c80: 2831 290a 2020 2020 2020 2020 7369 7a65  (1).        size
+00007c90: 506f 6c69 6379 2e73 6574 5665 7274 6963  Policy.setVertic
+00007ca0: 616c 5374 7265 7463 6828 3029 0a20 2020  alStretch(0).   
+00007cb0: 2020 2020 2073 697a 6550 6f6c 6963 792e       sizePolicy.
+00007cc0: 7365 7448 6569 6768 7446 6f72 5769 6474  setHeightForWidt
+00007cd0: 6828 7365 6c66 2e74 6162 5769 6467 6574  h(self.tabWidget
+00007ce0: 5f72 6573 756c 7473 2e73 697a 6550 6f6c  _results.sizePol
+00007cf0: 6963 7928 292e 6861 7348 6569 6768 7446  icy().hasHeightF
+00007d00: 6f72 5769 6474 6828 2929 0a20 2020 2020  orWidth()).     
+00007d10: 2020 2073 656c 662e 7461 6257 6964 6765     self.tabWidge
+00007d20: 745f 7265 7375 6c74 732e 7365 7453 697a  t_results.setSiz
+00007d30: 6550 6f6c 6963 7928 7369 7a65 506f 6c69  ePolicy(sizePoli
+00007d40: 6379 290a 2020 2020 2020 2020 7365 6c66  cy).        self
+00007d50: 2e74 6162 5769 6467 6574 5f72 6573 756c  .tabWidget_resul
+00007d60: 7473 2e73 6574 4f62 6a65 6374 4e61 6d65  ts.setObjectName
+00007d70: 2822 7461 6257 6964 6765 745f 7265 7375  ("tabWidget_resu
+00007d80: 6c74 7322 290a 2020 2020 2020 2020 7365  lts").        se
+00007d90: 6c66 2e74 6162 5f72 6573 756c 7473 5f69  lf.tab_results_i
+00007da0: 6e66 6f20 3d20 5174 5769 6467 6574 732e  nfo = QtWidgets.
+00007db0: 5157 6964 6765 7428 290a 2020 2020 2020  QWidget().      
+00007dc0: 2020 7365 6c66 2e74 6162 5f72 6573 756c    self.tab_resul
+00007dd0: 7473 5f69 6e66 6f2e 7365 744f 626a 6563  ts_info.setObjec
+00007de0: 744e 616d 6528 2274 6162 5f72 6573 756c  tName("tab_resul
+00007df0: 7473 5f69 6e66 6f22 290a 2020 2020 2020  ts_info").      
+00007e00: 2020 7365 6c66 2e76 6572 7469 6361 6c4c    self.verticalL
+00007e10: 6179 6f75 745f 3233 203d 2051 7457 6964  ayout_23 = QtWid
+00007e20: 6765 7473 2e51 5642 6f78 4c61 796f 7574  gets.QVBoxLayout
+00007e30: 2873 656c 662e 7461 625f 7265 7375 6c74  (self.tab_result
+00007e40: 735f 696e 666f 290a 2020 2020 2020 2020  s_info).        
+00007e50: 7365 6c66 2e76 6572 7469 6361 6c4c 6179  self.verticalLay
+00007e60: 6f75 745f 3233 2e73 6574 4f62 6a65 6374  out_23.setObject
+00007e70: 4e61 6d65 2822 7665 7274 6963 616c 4c61  Name("verticalLa
+00007e80: 796f 7574 5f32 3322 290a 2020 2020 2020  yout_23").      
+00007e90: 2020 7365 6c66 2e76 6572 7469 6361 6c4c    self.verticalL
+00007ea0: 6179 6f75 745f 3232 203d 2051 7457 6964  ayout_22 = QtWid
+00007eb0: 6765 7473 2e51 5642 6f78 4c61 796f 7574  gets.QVBoxLayout
+00007ec0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+00007ed0: 7665 7274 6963 616c 4c61 796f 7574 5f32  verticalLayout_2
+00007ee0: 322e 7365 744f 626a 6563 744e 616d 6528  2.setObjectName(
+00007ef0: 2276 6572 7469 6361 6c4c 6179 6f75 745f  "verticalLayout_
+00007f00: 3232 2229 0a20 2020 2020 2020 2073 656c  22").        sel
+00007f10: 662e 6772 6f75 7042 6f78 5f72 6573 756c  f.groupBox_resul
+00007f20: 7473 5f69 6e66 6f20 3d20 5174 5769 6467  ts_info = QtWidg
+00007f30: 6574 732e 5147 726f 7570 426f 7828 7365  ets.QGroupBox(se
+00007f40: 6c66 2e74 6162 5f72 6573 756c 7473 5f69  lf.tab_results_i
+00007f50: 6e66 6f29 0a20 2020 2020 2020 2073 656c  nfo).        sel
+00007f60: 662e 6772 6f75 7042 6f78 5f72 6573 756c  f.groupBox_resul
+00007f70: 7473 5f69 6e66 6f2e 7365 744f 626a 6563  ts_info.setObjec
+00007f80: 744e 616d 6528 2267 726f 7570 426f 785f  tName("groupBox_
+00007f90: 7265 7375 6c74 735f 696e 666f 2229 0a20  results_info"). 
+00007fa0: 2020 2020 2020 2073 656c 662e 7665 7274         self.vert
+00007fb0: 6963 616c 4c61 796f 7574 5f32 3120 3d20  icalLayout_21 = 
+00007fc0: 5174 5769 6467 6574 732e 5156 426f 784c  QtWidgets.QVBoxL
+00007fd0: 6179 6f75 7428 7365 6c66 2e67 726f 7570  ayout(self.group
+00007fe0: 426f 785f 7265 7375 6c74 735f 696e 666f  Box_results_info
+00007ff0: 290a 2020 2020 2020 2020 7365 6c66 2e76  ).        self.v
+00008000: 6572 7469 6361 6c4c 6179 6f75 745f 3231  erticalLayout_21
+00008010: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
+00008020: 7665 7274 6963 616c 4c61 796f 7574 5f32  verticalLayout_2
+00008030: 3122 290a 2020 2020 2020 2020 7365 6c66  1").        self
+00008040: 2e66 6f72 6d4c 6179 6f75 745f 3220 3d20  .formLayout_2 = 
+00008050: 5174 5769 6467 6574 732e 5146 6f72 6d4c  QtWidgets.QFormL
+00008060: 6179 6f75 7428 290a 2020 2020 2020 2020  ayout().        
+00008070: 7365 6c66 2e66 6f72 6d4c 6179 6f75 745f  self.formLayout_
+00008080: 322e 7365 744f 626a 6563 744e 616d 6528  2.setObjectName(
+00008090: 2266 6f72 6d4c 6179 6f75 745f 3222 290a  "formLayout_2").
+000080a0: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
+000080b0: 656c 5f33 203d 2051 7457 6964 6765 7473  el_3 = QtWidgets
+000080c0: 2e51 4c61 6265 6c28 7365 6c66 2e67 726f  .QLabel(self.gro
+000080d0: 7570 426f 785f 7265 7375 6c74 735f 696e  upBox_results_in
+000080e0: 666f 290a 2020 2020 2020 2020 7365 6c66  fo).        self
+000080f0: 2e6c 6162 656c 5f33 2e73 6574 4f62 6a65  .label_3.setObje
+00008100: 6374 4e61 6d65 2822 6c61 6265 6c5f 3322  ctName("label_3"
+00008110: 290a 2020 2020 2020 2020 7365 6c66 2e66  ).        self.f
+00008120: 6f72 6d4c 6179 6f75 745f 322e 7365 7457  ormLayout_2.setW
+00008130: 6964 6765 7428 302c 2051 7457 6964 6765  idget(0, QtWidge
+00008140: 7473 2e51 466f 726d 4c61 796f 7574 2e4c  ts.QFormLayout.L
+00008150: 6162 656c 526f 6c65 2c20 7365 6c66 2e6c  abelRole, self.l
+00008160: 6162 656c 5f33 290a 2020 2020 2020 2020  abel_3).        
+00008170: 7365 6c66 2e6c 6162 656c 5f72 6573 756c  self.label_resul
+00008180: 7473 5f61 646a 7573 746d 656e 745f 6d65  ts_adjustment_me
+00008190: 7468 6f64 203d 2051 7457 6964 6765 7473  thod = QtWidgets
+000081a0: 2e51 4c61 6265 6c28 7365 6c66 2e67 726f  .QLabel(self.gro
+000081b0: 7570 426f 785f 7265 7375 6c74 735f 696e  upBox_results_in
+000081c0: 666f 290a 2020 2020 2020 2020 7365 6c66  fo).        self
+000081d0: 2e6c 6162 656c 5f72 6573 756c 7473 5f61  .label_results_a
+000081e0: 646a 7573 746d 656e 745f 6d65 7468 6f64  djustment_method
+000081f0: 2e73 6574 4d69 6e69 6d75 6d53 697a 6528  .setMinimumSize(
+00008200: 5174 436f 7265 2e51 5369 7a65 2831 3030  QtCore.QSize(100
+00008210: 2c20 3029 290a 2020 2020 2020 2020 7365  , 0)).        se
+00008220: 6c66 2e6c 6162 656c 5f72 6573 756c 7473  lf.label_results
+00008230: 5f61 646a 7573 746d 656e 745f 6d65 7468  _adjustment_meth
+00008240: 6f64 2e73 6574 5465 7874 2822 2229 0a20  od.setText(""). 
+00008250: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
+00008260: 6c5f 7265 7375 6c74 735f 6164 6a75 7374  l_results_adjust
+00008270: 6d65 6e74 5f6d 6574 686f 642e 7365 744f  ment_method.setO
+00008280: 626a 6563 744e 616d 6528 226c 6162 656c  bjectName("label
+00008290: 5f72 6573 756c 7473 5f61 646a 7573 746d  _results_adjustm
+000082a0: 656e 745f 6d65 7468 6f64 2229 0a20 2020  ent_method").   
+000082b0: 2020 2020 2073 656c 662e 666f 726d 4c61       self.formLa
+000082c0: 796f 7574 5f32 2e73 6574 5769 6467 6574  yout_2.setWidget
+000082d0: 2830 2c20 5174 5769 6467 6574 732e 5146  (0, QtWidgets.QF
+000082e0: 6f72 6d4c 6179 6f75 742e 4669 656c 6452  ormLayout.FieldR
+000082f0: 6f6c 652c 2073 656c 662e 6c61 6265 6c5f  ole, self.label_
+00008300: 7265 7375 6c74 735f 6164 6a75 7374 6d65  results_adjustme
+00008310: 6e74 5f6d 6574 686f 6429 0a20 2020 2020  nt_method).     
+00008320: 2020 2073 656c 662e 6c61 6265 6c5f 7265     self.label_re
+00008330: 7375 6c74 735f 7469 6d65 5f61 6e64 5f64  sults_time_and_d
+00008340: 6174 6520 3d20 5174 5769 6467 6574 732e  ate = QtWidgets.
+00008350: 514c 6162 656c 2873 656c 662e 6772 6f75  QLabel(self.grou
+00008360: 7042 6f78 5f72 6573 756c 7473 5f69 6e66  pBox_results_inf
+00008370: 6f29 0a20 2020 2020 2020 2073 656c 662e  o).        self.
+00008380: 6c61 6265 6c5f 7265 7375 6c74 735f 7469  label_results_ti
+00008390: 6d65 5f61 6e64 5f64 6174 652e 7365 744d  me_and_date.setM
+000083a0: 696e 696d 756d 5369 7a65 2851 7443 6f72  inimumSize(QtCor
+000083b0: 652e 5153 697a 6528 3130 302c 2030 2929  e.QSize(100, 0))
+000083c0: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
+000083d0: 6265 6c5f 7265 7375 6c74 735f 7469 6d65  bel_results_time
+000083e0: 5f61 6e64 5f64 6174 652e 7365 7454 6578  _and_date.setTex
+000083f0: 7428 2222 290a 2020 2020 2020 2020 7365  t("").        se
+00008400: 6c66 2e6c 6162 656c 5f72 6573 756c 7473  lf.label_results
+00008410: 5f74 696d 655f 616e 645f 6461 7465 2e73  _time_and_date.s
+00008420: 6574 4f62 6a65 6374 4e61 6d65 2822 6c61  etObjectName("la
+00008430: 6265 6c5f 7265 7375 6c74 735f 7469 6d65  bel_results_time
+00008440: 5f61 6e64 5f64 6174 6522 290a 2020 2020  _and_date").    
+00008450: 2020 2020 7365 6c66 2e66 6f72 6d4c 6179      self.formLay
+00008460: 6f75 745f 322e 7365 7457 6964 6765 7428  out_2.setWidget(
+00008470: 312c 2051 7457 6964 6765 7473 2e51 466f  1, QtWidgets.QFo
+00008480: 726d 4c61 796f 7574 2e46 6965 6c64 526f  rmLayout.FieldRo
+00008490: 6c65 2c20 7365 6c66 2e6c 6162 656c 5f72  le, self.label_r
+000084a0: 6573 756c 7473 5f74 696d 655f 616e 645f  esults_time_and_
+000084b0: 6461 7465 290a 2020 2020 2020 2020 7365  date).        se
+000084c0: 6c66 2e6c 6162 656c 5f38 203d 2051 7457  lf.label_8 = QtW
+000084d0: 6964 6765 7473 2e51 4c61 6265 6c28 7365  idgets.QLabel(se
+000084e0: 6c66 2e67 726f 7570 426f 785f 7265 7375  lf.groupBox_resu
+000084f0: 6c74 735f 696e 666f 290a 2020 2020 2020  lts_info).      
+00008500: 2020 7365 6c66 2e6c 6162 656c 5f38 2e73    self.label_8.s
+00008510: 6574 4f62 6a65 6374 4e61 6d65 2822 6c61  etObjectName("la
+00008520: 6265 6c5f 3822 290a 2020 2020 2020 2020  bel_8").        
+00008530: 7365 6c66 2e66 6f72 6d4c 6179 6f75 745f  self.formLayout_
+00008540: 322e 7365 7457 6964 6765 7428 322c 2051  2.setWidget(2, Q
+00008550: 7457 6964 6765 7473 2e51 466f 726d 4c61  tWidgets.QFormLa
+00008560: 796f 7574 2e4c 6162 656c 526f 6c65 2c20  yout.LabelRole, 
+00008570: 7365 6c66 2e6c 6162 656c 5f38 290a 2020  self.label_8).  
+00008580: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
+00008590: 5f72 6573 756c 7473 5f6e 756d 6265 725f  _results_number_
+000085a0: 6f66 5f69 7465 7261 7469 6f6e 7320 3d20  of_iterations = 
+000085b0: 5174 5769 6467 6574 732e 514c 6162 656c  QtWidgets.QLabel
+000085c0: 2873 656c 662e 6772 6f75 7042 6f78 5f72  (self.groupBox_r
+000085d0: 6573 756c 7473 5f69 6e66 6f29 0a20 2020  esults_info).   
+000085e0: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
+000085f0: 7265 7375 6c74 735f 6e75 6d62 6572 5f6f  results_number_o
+00008600: 665f 6974 6572 6174 696f 6e73 2e73 6574  f_iterations.set
+00008610: 5465 7874 2822 2229 0a20 2020 2020 2020  Text("").       
+00008620: 2073 656c 662e 6c61 6265 6c5f 7265 7375   self.label_resu
+00008630: 6c74 735f 6e75 6d62 6572 5f6f 665f 6974  lts_number_of_it
+00008640: 6572 6174 696f 6e73 2e73 6574 4f62 6a65  erations.setObje
+00008650: 6374 4e61 6d65 2822 6c61 6265 6c5f 7265  ctName("label_re
+00008660: 7375 6c74 735f 6e75 6d62 6572 5f6f 665f  sults_number_of_
+00008670: 6974 6572 6174 696f 6e73 2229 0a20 2020  iterations").   
+00008680: 2020 2020 2073 656c 662e 666f 726d 4c61       self.formLa
+00008690: 796f 7574 5f32 2e73 6574 5769 6467 6574  yout_2.setWidget
+000086a0: 2832 2c20 5174 5769 6467 6574 732e 5146  (2, QtWidgets.QF
+000086b0: 6f72 6d4c 6179 6f75 742e 4669 656c 6452  ormLayout.FieldR
+000086c0: 6f6c 652c 2073 656c 662e 6c61 6265 6c5f  ole, self.label_
+000086d0: 7265 7375 6c74 735f 6e75 6d62 6572 5f6f  results_number_o
+000086e0: 665f 6974 6572 6174 696f 6e73 290a 2020  f_iterations).  
+000086f0: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
+00008700: 5f31 3020 3d20 5174 5769 6467 6574 732e  _10 = QtWidgets.
+00008710: 514c 6162 656c 2873 656c 662e 6772 6f75  QLabel(self.grou
+00008720: 7042 6f78 5f72 6573 756c 7473 5f69 6e66  pBox_results_inf
+00008730: 6f29 0a20 2020 2020 2020 2073 656c 662e  o).        self.
+00008740: 6c61 6265 6c5f 3130 2e73 6574 4f62 6a65  label_10.setObje
+00008750: 6374 4e61 6d65 2822 6c61 6265 6c5f 3130  ctName("label_10
+00008760: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00008770: 666f 726d 4c61 796f 7574 5f32 2e73 6574  formLayout_2.set
+00008780: 5769 6467 6574 2833 2c20 5174 5769 6467  Widget(3, QtWidg
+00008790: 6574 732e 5146 6f72 6d4c 6179 6f75 742e  ets.QFormLayout.
+000087a0: 4c61 6265 6c52 6f6c 652c 2073 656c 662e  LabelRole, self.
+000087b0: 6c61 6265 6c5f 3130 290a 2020 2020 2020  label_10).      
+000087c0: 2020 7365 6c66 2e6c 6162 656c 5f72 6573    self.label_res
+000087d0: 756c 7473 5f63 6f6d 6d65 6e74 203d 2051  ults_comment = Q
+000087e0: 7457 6964 6765 7473 2e51 4c61 6265 6c28  tWidgets.QLabel(
+000087f0: 7365 6c66 2e67 726f 7570 426f 785f 7265  self.groupBox_re
+00008800: 7375 6c74 735f 696e 666f 290a 2020 2020  sults_info).    
+00008810: 2020 2020 7365 6c66 2e6c 6162 656c 5f72      self.label_r
+00008820: 6573 756c 7473 5f63 6f6d 6d65 6e74 2e73  esults_comment.s
+00008830: 6574 4d69 6e69 6d75 6d53 697a 6528 5174  etMinimumSize(Qt
+00008840: 436f 7265 2e51 5369 7a65 2831 3030 2c20  Core.QSize(100, 
+00008850: 3029 290a 2020 2020 2020 2020 7365 6c66  0)).        self
+00008860: 2e6c 6162 656c 5f72 6573 756c 7473 5f63  .label_results_c
+00008870: 6f6d 6d65 6e74 2e73 6574 5465 7874 2822  omment.setText("
+00008880: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00008890: 6c61 6265 6c5f 7265 7375 6c74 735f 636f  label_results_co
+000088a0: 6d6d 656e 742e 7365 744f 626a 6563 744e  mment.setObjectN
+000088b0: 616d 6528 226c 6162 656c 5f72 6573 756c  ame("label_resul
+000088c0: 7473 5f63 6f6d 6d65 6e74 2229 0a20 2020  ts_comment").   
+000088d0: 2020 2020 2073 656c 662e 666f 726d 4c61       self.formLa
+000088e0: 796f 7574 5f32 2e73 6574 5769 6467 6574  yout_2.setWidget
+000088f0: 2833 2c20 5174 5769 6467 6574 732e 5146  (3, QtWidgets.QF
+00008900: 6f72 6d4c 6179 6f75 742e 4669 656c 6452  ormLayout.FieldR
+00008910: 6f6c 652c 2073 656c 662e 6c61 6265 6c5f  ole, self.label_
+00008920: 7265 7375 6c74 735f 636f 6d6d 656e 7429  results_comment)
+00008930: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
+00008940: 6265 6c5f 3420 3d20 5174 5769 6467 6574  bel_4 = QtWidget
+00008950: 732e 514c 6162 656c 2873 656c 662e 6772  s.QLabel(self.gr
+00008960: 6f75 7042 6f78 5f72 6573 756c 7473 5f69  oupBox_results_i
+00008970: 6e66 6f29 0a20 2020 2020 2020 2073 656c  nfo).        sel
+00008980: 662e 6c61 6265 6c5f 342e 7365 744f 626a  f.label_4.setObj
+00008990: 6563 744e 616d 6528 226c 6162 656c 5f34  ectName("label_4
+000089a0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+000089b0: 666f 726d 4c61 796f 7574 5f32 2e73 6574  formLayout_2.set
+000089c0: 5769 6467 6574 2831 2c20 5174 5769 6467  Widget(1, QtWidg
+000089d0: 6574 732e 5146 6f72 6d4c 6179 6f75 742e  ets.QFormLayout.
+000089e0: 4c61 6265 6c52 6f6c 652c 2073 656c 662e  LabelRole, self.
+000089f0: 6c61 6265 6c5f 3429 0a20 2020 2020 2020  label_4).       
+00008a00: 2073 656c 662e 7665 7274 6963 616c 4c61   self.verticalLa
+00008a10: 796f 7574 5f32 312e 6164 644c 6179 6f75  yout_21.addLayou
+00008a20: 7428 7365 6c66 2e66 6f72 6d4c 6179 6f75  t(self.formLayou
+00008a30: 745f 3229 0a20 2020 2020 2020 2073 656c  t_2).        sel
+00008a40: 662e 7665 7274 6963 616c 4c61 796f 7574  f.verticalLayout
+00008a50: 5f32 322e 6164 6457 6964 6765 7428 7365  _22.addWidget(se
+00008a60: 6c66 2e67 726f 7570 426f 785f 7265 7375  lf.groupBox_resu
+00008a70: 6c74 735f 696e 666f 290a 2020 2020 2020  lts_info).      
+00008a80: 2020 7365 6c66 2e67 726f 7570 426f 785f    self.groupBox_
+00008a90: 7265 7375 6c74 735f 7374 6174 6973 7469  results_statisti
+00008aa0: 6373 203d 2051 7457 6964 6765 7473 2e51  cs = QtWidgets.Q
+00008ab0: 4772 6f75 7042 6f78 2873 656c 662e 7461  GroupBox(self.ta
+00008ac0: 625f 7265 7375 6c74 735f 696e 666f 290a  b_results_info).
+00008ad0: 2020 2020 2020 2020 7365 6c66 2e67 726f          self.gro
+00008ae0: 7570 426f 785f 7265 7375 6c74 735f 7374  upBox_results_st
+00008af0: 6174 6973 7469 6373 2e73 6574 4f62 6a65  atistics.setObje
+00008b00: 6374 4e61 6d65 2822 6772 6f75 7042 6f78  ctName("groupBox
+00008b10: 5f72 6573 756c 7473 5f73 7461 7469 7374  _results_statist
+00008b20: 6963 7322 290a 2020 2020 2020 2020 7365  ics").        se
+00008b30: 6c66 2e76 6572 7469 6361 6c4c 6179 6f75  lf.verticalLayou
+00008b40: 745f 3234 203d 2051 7457 6964 6765 7473  t_24 = QtWidgets
+00008b50: 2e51 5642 6f78 4c61 796f 7574 2873 656c  .QVBoxLayout(sel
+00008b60: 662e 6772 6f75 7042 6f78 5f72 6573 756c  f.groupBox_resul
+00008b70: 7473 5f73 7461 7469 7374 6963 7329 0a20  ts_statistics). 
+00008b80: 2020 2020 2020 2073 656c 662e 7665 7274         self.vert
+00008b90: 6963 616c 4c61 796f 7574 5f32 342e 7365  icalLayout_24.se
+00008ba0: 744f 626a 6563 744e 616d 6528 2276 6572  tObjectName("ver
+00008bb0: 7469 6361 6c4c 6179 6f75 745f 3234 2229  ticalLayout_24")
+00008bc0: 0a20 2020 2020 2020 2073 656c 662e 666f  .        self.fo
+00008bd0: 726d 4c61 796f 7574 5f33 203d 2051 7457  rmLayout_3 = QtW
+00008be0: 6964 6765 7473 2e51 466f 726d 4c61 796f  idgets.QFormLayo
+00008bf0: 7574 2829 0a20 2020 2020 2020 2073 656c  ut().        sel
+00008c00: 662e 666f 726d 4c61 796f 7574 5f33 2e73  f.formLayout_3.s
+00008c10: 6574 4f62 6a65 6374 4e61 6d65 2822 666f  etObjectName("fo
+00008c20: 726d 4c61 796f 7574 5f33 2229 0a20 2020  rmLayout_3").   
+00008c30: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
+00008c40: 3920 3d20 5174 5769 6467 6574 732e 514c  9 = QtWidgets.QL
+00008c50: 6162 656c 2873 656c 662e 6772 6f75 7042  abel(self.groupB
+00008c60: 6f78 5f72 6573 756c 7473 5f73 7461 7469  ox_results_stati
+00008c70: 7374 6963 7329 0a20 2020 2020 2020 2073  stics).        s
+00008c80: 656c 662e 6c61 6265 6c5f 392e 7365 744f  elf.label_9.setO
+00008c90: 626a 6563 744e 616d 6528 226c 6162 656c  bjectName("label
+00008ca0: 5f39 2229 0a20 2020 2020 2020 2073 656c  _9").        sel
+00008cb0: 662e 666f 726d 4c61 796f 7574 5f33 2e73  f.formLayout_3.s
+00008cc0: 6574 5769 6467 6574 2830 2c20 5174 5769  etWidget(0, QtWi
+00008cd0: 6467 6574 732e 5146 6f72 6d4c 6179 6f75  dgets.QFormLayou
+00008ce0: 742e 4c61 6265 6c52 6f6c 652c 2073 656c  t.LabelRole, sel
+00008cf0: 662e 6c61 6265 6c5f 3929 0a20 2020 2020  f.label_9).     
+00008d00: 2020 2073 656c 662e 6c61 6265 6c5f 7265     self.label_re
+00008d10: 7375 6c74 735f 7369 6730 203d 2051 7457  sults_sig0 = QtW
+00008d20: 6964 6765 7473 2e51 4c61 6265 6c28 7365  idgets.QLabel(se
+00008d30: 6c66 2e67 726f 7570 426f 785f 7265 7375  lf.groupBox_resu
+00008d40: 6c74 735f 7374 6174 6973 7469 6373 290a  lts_statistics).
+00008d50: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
+00008d60: 656c 5f72 6573 756c 7473 5f73 6967 302e  el_results_sig0.
+00008d70: 7365 744d 696e 696d 756d 5369 7a65 2851  setMinimumSize(Q
+00008d80: 7443 6f72 652e 5153 697a 6528 3130 302c  tCore.QSize(100,
+00008d90: 2030 2929 0a20 2020 2020 2020 2073 656c   0)).        sel
+00008da0: 662e 6c61 6265 6c5f 7265 7375 6c74 735f  f.label_results_
+00008db0: 7369 6730 2e73 6574 5465 7874 2822 2229  sig0.setText("")
+00008dc0: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
+00008dd0: 6265 6c5f 7265 7375 6c74 735f 7369 6730  bel_results_sig0
+00008de0: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
+00008df0: 6c61 6265 6c5f 7265 7375 6c74 735f 7369  label_results_si
+00008e00: 6730 2229 0a20 2020 2020 2020 2073 656c  g0").        sel
+00008e10: 662e 666f 726d 4c61 796f 7574 5f33 2e73  f.formLayout_3.s
+00008e20: 6574 5769 6467 6574 2830 2c20 5174 5769  etWidget(0, QtWi
+00008e30: 6467 6574 732e 5146 6f72 6d4c 6179 6f75  dgets.QFormLayou
+00008e40: 742e 4669 656c 6452 6f6c 652c 2073 656c  t.FieldRole, sel
+00008e50: 662e 6c61 6265 6c5f 7265 7375 6c74 735f  f.label_results_
+00008e60: 7369 6730 290a 2020 2020 2020 2020 7365  sig0).        se
+00008e70: 6c66 2e6c 6162 656c 5f36 203d 2051 7457  lf.label_6 = QtW
+00008e80: 6964 6765 7473 2e51 4c61 6265 6c28 7365  idgets.QLabel(se
+00008e90: 6c66 2e67 726f 7570 426f 785f 7265 7375  lf.groupBox_resu
+00008ea0: 6c74 735f 7374 6174 6973 7469 6373 290a  lts_statistics).
+00008eb0: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
+00008ec0: 656c 5f36 2e73 6574 4f62 6a65 6374 4e61  el_6.setObjectNa
+00008ed0: 6d65 2822 6c61 6265 6c5f 3622 290a 2020  me("label_6").  
+00008ee0: 2020 2020 2020 7365 6c66 2e66 6f72 6d4c        self.formL
+00008ef0: 6179 6f75 745f 332e 7365 7457 6964 6765  ayout_3.setWidge
+00008f00: 7428 312c 2051 7457 6964 6765 7473 2e51  t(1, QtWidgets.Q
+00008f10: 466f 726d 4c61 796f 7574 2e4c 6162 656c  FormLayout.Label
+00008f20: 526f 6c65 2c20 7365 6c66 2e6c 6162 656c  Role, self.label
+00008f30: 5f36 290a 2020 2020 2020 2020 7365 6c66  _6).        self
+00008f40: 2e6c 6162 656c 5f72 6573 756c 7473 5f67  .label_results_g
+00008f50: 6f6f 646e 6573 735f 6f66 5f66 6974 5f74  oodness_of_fit_t
+00008f60: 6573 745f 7374 6174 7573 203d 2051 7457  est_status = QtW
+00008f70: 6964 6765 7473 2e51 4c61 6265 6c28 7365  idgets.QLabel(se
+00008f80: 6c66 2e67 726f 7570 426f 785f 7265 7375  lf.groupBox_resu
+00008f90: 6c74 735f 7374 6174 6973 7469 6373 290a  lts_statistics).
+00008fa0: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
+00008fb0: 656c 5f72 6573 756c 7473 5f67 6f6f 646e  el_results_goodn
+00008fc0: 6573 735f 6f66 5f66 6974 5f74 6573 745f  ess_of_fit_test_
+00008fd0: 7374 6174 7573 2e73 6574 5465 7874 2822  status.setText("
+00008fe0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00008ff0: 6c61 6265 6c5f 7265 7375 6c74 735f 676f  label_results_go
+00009000: 6f64 6e65 7373 5f6f 665f 6669 745f 7465  odness_of_fit_te
+00009010: 7374 5f73 7461 7475 732e 7365 744f 626a  st_status.setObj
+00009020: 6563 744e 616d 6528 226c 6162 656c 5f72  ectName("label_r
+00009030: 6573 756c 7473 5f67 6f6f 646e 6573 735f  esults_goodness_
+00009040: 6f66 5f66 6974 5f74 6573 745f 7374 6174  of_fit_test_stat
+00009050: 7573 2229 0a20 2020 2020 2020 2073 656c  us").        sel
+00009060: 662e 666f 726d 4c61 796f 7574 5f33 2e73  f.formLayout_3.s
+00009070: 6574 5769 6467 6574 2831 2c20 5174 5769  etWidget(1, QtWi
+00009080: 6467 6574 732e 5146 6f72 6d4c 6179 6f75  dgets.QFormLayou
+00009090: 742e 4669 656c 6452 6f6c 652c 2073 656c  t.FieldRole, sel
+000090a0: 662e 6c61 6265 6c5f 7265 7375 6c74 735f  f.label_results_
+000090b0: 676f 6f64 6e65 7373 5f6f 665f 6669 745f  goodness_of_fit_
+000090c0: 7465 7374 5f73 7461 7475 7329 0a20 2020  test_status).   
+000090d0: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
+000090e0: 3720 3d20 5174 5769 6467 6574 732e 514c  7 = QtWidgets.QL
+000090f0: 6162 656c 2873 656c 662e 6772 6f75 7042  abel(self.groupB
+00009100: 6f78 5f72 6573 756c 7473 5f73 7461 7469  ox_results_stati
+00009110: 7374 6963 7329 0a20 2020 2020 2020 2073  stics).        s
+00009120: 656c 662e 6c61 6265 6c5f 372e 7365 744f  elf.label_7.setO
+00009130: 626a 6563 744e 616d 6528 226c 6162 656c  bjectName("label
+00009140: 5f37 2229 0a20 2020 2020 2020 2073 656c  _7").        sel
+00009150: 662e 666f 726d 4c61 796f 7574 5f33 2e73  f.formLayout_3.s
+00009160: 6574 5769 6467 6574 2832 2c20 5174 5769  etWidget(2, QtWi
+00009170: 6467 6574 732e 5146 6f72 6d4c 6179 6f75  dgets.QFormLayou
+00009180: 742e 4c61 6265 6c52 6f6c 652c 2073 656c  t.LabelRole, sel
+00009190: 662e 6c61 6265 6c5f 3729 0a20 2020 2020  f.label_7).     
+000091a0: 2020 2073 656c 662e 6c61 6265 6c5f 7265     self.label_re
+000091b0: 7375 6c74 735f 6e75 6d62 6572 5f6f 665f  sults_number_of_
+000091c0: 6f75 746c 6965 7273 203d 2051 7457 6964  outliers = QtWid
+000091d0: 6765 7473 2e51 4c61 6265 6c28 7365 6c66  gets.QLabel(self
+000091e0: 2e67 726f 7570 426f 785f 7265 7375 6c74  .groupBox_result
+000091f0: 735f 7374 6174 6973 7469 6373 290a 2020  s_statistics).  
+00009200: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
+00009210: 5f72 6573 756c 7473 5f6e 756d 6265 725f  _results_number_
+00009220: 6f66 5f6f 7574 6c69 6572 732e 7365 7454  of_outliers.setT
+00009230: 6578 7428 2222 290a 2020 2020 2020 2020  ext("").        
+00009240: 7365 6c66 2e6c 6162 656c 5f72 6573 756c  self.label_resul
+00009250: 7473 5f6e 756d 6265 725f 6f66 5f6f 7574  ts_number_of_out
+00009260: 6c69 6572 732e 7365 744f 626a 6563 744e  liers.setObjectN
+00009270: 616d 6528 226c 6162 656c 5f72 6573 756c  ame("label_resul
+00009280: 7473 5f6e 756d 6265 725f 6f66 5f6f 7574  ts_number_of_out
+00009290: 6c69 6572 7322 290a 2020 2020 2020 2020  liers").        
+000092a0: 7365 6c66 2e66 6f72 6d4c 6179 6f75 745f  self.formLayout_
+000092b0: 332e 7365 7457 6964 6765 7428 322c 2051  3.setWidget(2, Q
+000092c0: 7457 6964 6765 7473 2e51 466f 726d 4c61  tWidgets.QFormLa
+000092d0: 796f 7574 2e46 6965 6c64 526f 6c65 2c20  yout.FieldRole, 
+000092e0: 7365 6c66 2e6c 6162 656c 5f72 6573 756c  self.label_resul
+000092f0: 7473 5f6e 756d 6265 725f 6f66 5f6f 7574  ts_number_of_out
+00009300: 6c69 6572 7329 0a20 2020 2020 2020 2073  liers).        s
+00009310: 656c 662e 7665 7274 6963 616c 4c61 796f  elf.verticalLayo
+00009320: 7574 5f32 342e 6164 644c 6179 6f75 7428  ut_24.addLayout(
+00009330: 7365 6c66 2e66 6f72 6d4c 6179 6f75 745f  self.formLayout_
+00009340: 3329 0a20 2020 2020 2020 2073 656c 662e  3).        self.
+00009350: 7665 7274 6963 616c 4c61 796f 7574 5f32  verticalLayout_2
+00009360: 322e 6164 6457 6964 6765 7428 7365 6c66  2.addWidget(self
+00009370: 2e67 726f 7570 426f 785f 7265 7375 6c74  .groupBox_result
+00009380: 735f 7374 6174 6973 7469 6373 290a 2020  s_statistics).  
+00009390: 2020 2020 2020 7365 6c66 2e67 726f 7570        self.group
+000093a0: 426f 785f 7265 7375 6c74 735f 6c73 6d5f  Box_results_lsm_
+000093b0: 7275 6e5f 6c6f 6720 3d20 5174 5769 6467  run_log = QtWidg
+000093c0: 6574 732e 5147 726f 7570 426f 7828 7365  ets.QGroupBox(se
+000093d0: 6c66 2e74 6162 5f72 6573 756c 7473 5f69  lf.tab_results_i
+000093e0: 6e66 6f29 0a20 2020 2020 2020 2073 656c  nfo).        sel
+000093f0: 662e 6772 6f75 7042 6f78 5f72 6573 756c  f.groupBox_resul
+00009400: 7473 5f6c 736d 5f72 756e 5f6c 6f67 2e73  ts_lsm_run_log.s
+00009410: 6574 4f62 6a65 6374 4e61 6d65 2822 6772  etObjectName("gr
+00009420: 6f75 7042 6f78 5f72 6573 756c 7473 5f6c  oupBox_results_l
+00009430: 736d 5f72 756e 5f6c 6f67 2229 0a20 2020  sm_run_log").   
+00009440: 2020 2020 2073 656c 662e 7665 7274 6963       self.vertic
+00009450: 616c 4c61 796f 7574 5f32 3020 3d20 5174  alLayout_20 = Qt
+00009460: 5769 6467 6574 732e 5156 426f 784c 6179  Widgets.QVBoxLay
+00009470: 6f75 7428 7365 6c66 2e67 726f 7570 426f  out(self.groupBo
+00009480: 785f 7265 7375 6c74 735f 6c73 6d5f 7275  x_results_lsm_ru
+00009490: 6e5f 6c6f 6729 0a20 2020 2020 2020 2073  n_log).        s
+000094a0: 656c 662e 7665 7274 6963 616c 4c61 796f  elf.verticalLayo
+000094b0: 7574 5f32 302e 7365 744f 626a 6563 744e  ut_20.setObjectN
+000094c0: 616d 6528 2276 6572 7469 6361 6c4c 6179  ame("verticalLay
+000094d0: 6f75 745f 3230 2229 0a20 2020 2020 2020  out_20").       
+000094e0: 2073 656c 662e 706c 6169 6e54 6578 7445   self.plainTextE
+000094f0: 6469 745f 7265 7375 6c74 735f 6c6f 6720  dit_results_log 
+00009500: 3d20 5174 5769 6467 6574 732e 5150 6c61  = QtWidgets.QPla
+00009510: 696e 5465 7874 4564 6974 2873 656c 662e  inTextEdit(self.
+00009520: 6772 6f75 7042 6f78 5f72 6573 756c 7473  groupBox_results
+00009530: 5f6c 736d 5f72 756e 5f6c 6f67 290a 2020  _lsm_run_log).  
+00009540: 2020 2020 2020 7365 6c66 2e70 6c61 696e        self.plain
+00009550: 5465 7874 4564 6974 5f72 6573 756c 7473  TextEdit_results
+00009560: 5f6c 6f67 2e73 6574 5265 6164 4f6e 6c79  _log.setReadOnly
+00009570: 2854 7275 6529 0a20 2020 2020 2020 2073  (True).        s
+00009580: 656c 662e 706c 6169 6e54 6578 7445 6469  elf.plainTextEdi
+00009590: 745f 7265 7375 6c74 735f 6c6f 672e 7365  t_results_log.se
+000095a0: 744f 626a 6563 744e 616d 6528 2270 6c61  tObjectName("pla
+000095b0: 696e 5465 7874 4564 6974 5f72 6573 756c  inTextEdit_resul
+000095c0: 7473 5f6c 6f67 2229 0a20 2020 2020 2020  ts_log").       
+000095d0: 2073 656c 662e 7665 7274 6963 616c 4c61   self.verticalLa
+000095e0: 796f 7574 5f32 302e 6164 6457 6964 6765  yout_20.addWidge
+000095f0: 7428 7365 6c66 2e70 6c61 696e 5465 7874  t(self.plainText
+00009600: 4564 6974 5f72 6573 756c 7473 5f6c 6f67  Edit_results_log
+00009610: 290a 2020 2020 2020 2020 7365 6c66 2e76  ).        self.v
+00009620: 6572 7469 6361 6c4c 6179 6f75 745f 3232  erticalLayout_22
+00009630: 2e61 6464 5769 6467 6574 2873 656c 662e  .addWidget(self.
+00009640: 6772 6f75 7042 6f78 5f72 6573 756c 7473  groupBox_results
+00009650: 5f6c 736d 5f72 756e 5f6c 6f67 290a 2020  _lsm_run_log).  
+00009660: 2020 2020 2020 7365 6c66 2e76 6572 7469        self.verti
+00009670: 6361 6c4c 6179 6f75 745f 3233 2e61 6464  calLayout_23.add
+00009680: 4c61 796f 7574 2873 656c 662e 7665 7274  Layout(self.vert
+00009690: 6963 616c 4c61 796f 7574 5f32 3229 0a20  icalLayout_22). 
+000096a0: 2020 2020 2020 2073 656c 662e 7461 6257         self.tabW
+000096b0: 6964 6765 745f 7265 7375 6c74 732e 6164  idget_results.ad
+000096c0: 6454 6162 2873 656c 662e 7461 625f 7265  dTab(self.tab_re
+000096d0: 7375 6c74 735f 696e 666f 2c20 2222 290a  sults_info, "").
+000096e0: 2020 2020 2020 2020 7365 6c66 2e74 6162          self.tab
+000096f0: 5f72 6573 756c 7473 5f6f 6273 5f74 6162  _results_obs_tab
+00009700: 6c65 203d 2051 7457 6964 6765 7473 2e51  le = QtWidgets.Q
+00009710: 5769 6467 6574 2829 0a20 2020 2020 2020  Widget().       
+00009720: 2073 656c 662e 7461 625f 7265 7375 6c74   self.tab_result
+00009730: 735f 6f62 735f 7461 626c 652e 7365 744f  s_obs_table.setO
+00009740: 626a 6563 744e 616d 6528 2274 6162 5f72  bjectName("tab_r
+00009750: 6573 756c 7473 5f6f 6273 5f74 6162 6c65  esults_obs_table
+00009760: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00009770: 7665 7274 6963 616c 4c61 796f 7574 5f31  verticalLayout_1
+00009780: 3520 3d20 5174 5769 6467 6574 732e 5156  5 = QtWidgets.QV
+00009790: 426f 784c 6179 6f75 7428 7365 6c66 2e74  BoxLayout(self.t
+000097a0: 6162 5f72 6573 756c 7473 5f6f 6273 5f74  ab_results_obs_t
+000097b0: 6162 6c65 290a 2020 2020 2020 2020 7365  able).        se
+000097c0: 6c66 2e76 6572 7469 6361 6c4c 6179 6f75  lf.verticalLayou
+000097d0: 745f 3135 2e73 6574 4f62 6a65 6374 4e61  t_15.setObjectNa
+000097e0: 6d65 2822 7665 7274 6963 616c 4c61 796f  me("verticalLayo
+000097f0: 7574 5f31 3522 290a 2020 2020 2020 2020  ut_15").        
+00009800: 7365 6c66 2e74 6162 6c65 5669 6577 5f72  self.tableView_r
+00009810: 6573 756c 7473 5f6f 6273 6572 7661 7469  esults_observati
+00009820: 6f6e 7320 3d20 5174 5769 6467 6574 732e  ons = QtWidgets.
+00009830: 5154 6162 6c65 5669 6577 2873 656c 662e  QTableView(self.
+00009840: 7461 625f 7265 7375 6c74 735f 6f62 735f  tab_results_obs_
+00009850: 7461 626c 6529 0a20 2020 2020 2020 2073  table).        s
+00009860: 656c 662e 7461 626c 6556 6965 775f 7265  elf.tableView_re
+00009870: 7375 6c74 735f 6f62 7365 7276 6174 696f  sults_observatio
+00009880: 6e73 2e73 6574 4f62 6a65 6374 4e61 6d65  ns.setObjectName
+00009890: 2822 7461 626c 6556 6965 775f 7265 7375  ("tableView_resu
+000098a0: 6c74 735f 6f62 7365 7276 6174 696f 6e73  lts_observations
+000098b0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+000098c0: 7665 7274 6963 616c 4c61 796f 7574 5f31  verticalLayout_1
+000098d0: 352e 6164 6457 6964 6765 7428 7365 6c66  5.addWidget(self
+000098e0: 2e74 6162 6c65 5669 6577 5f72 6573 756c  .tableView_resul
+000098f0: 7473 5f6f 6273 6572 7661 7469 6f6e 7329  ts_observations)
+00009900: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
+00009910: 6257 6964 6765 745f 7265 7375 6c74 732e  bWidget_results.
+00009920: 6164 6454 6162 2873 656c 662e 7461 625f  addTab(self.tab_
+00009930: 7265 7375 6c74 735f 6f62 735f 7461 626c  results_obs_tabl
+00009940: 652c 2022 2229 0a20 2020 2020 2020 2073  e, "").        s
+00009950: 656c 662e 7461 625f 7265 7375 6c74 735f  elf.tab_results_
+00009960: 6f62 735f 706c 6f74 7320 3d20 5174 5769  obs_plots = QtWi
+00009970: 6467 6574 732e 5157 6964 6765 7428 290a  dgets.QWidget().
+00009980: 2020 2020 2020 2020 7365 6c66 2e74 6162          self.tab
+00009990: 5f72 6573 756c 7473 5f6f 6273 5f70 6c6f  _results_obs_plo
+000099a0: 7473 2e73 6574 4f62 6a65 6374 4e61 6d65  ts.setObjectName
+000099b0: 2822 7461 625f 7265 7375 6c74 735f 6f62  ("tab_results_ob
+000099c0: 735f 706c 6f74 7322 290a 2020 2020 2020  s_plots").      
+000099d0: 2020 7365 6c66 2e76 6572 7469 6361 6c4c    self.verticalL
+000099e0: 6179 6f75 745f 3338 203d 2051 7457 6964  ayout_38 = QtWid
+000099f0: 6765 7473 2e51 5642 6f78 4c61 796f 7574  gets.QVBoxLayout
+00009a00: 2873 656c 662e 7461 625f 7265 7375 6c74  (self.tab_result
+00009a10: 735f 6f62 735f 706c 6f74 7329 0a20 2020  s_obs_plots).   
+00009a20: 2020 2020 2073 656c 662e 7665 7274 6963       self.vertic
+00009a30: 616c 4c61 796f 7574 5f33 382e 7365 744f  alLayout_38.setO
+00009a40: 626a 6563 744e 616d 6528 2276 6572 7469  bjectName("verti
+00009a50: 6361 6c4c 6179 6f75 745f 3338 2229 0a20  calLayout_38"). 
+00009a60: 2020 2020 2020 2073 656c 662e 6772 6170         self.grap
+00009a70: 6869 6373 4c61 796f 7574 5769 6467 6574  hicsLayoutWidget
+00009a80: 5f72 6573 756c 7473 5f6f 6273 6572 7661  _results_observa
+00009a90: 7469 6f6e 735f 706c 6f74 7320 3d20 4772  tions_plots = Gr
+00009aa0: 6170 6869 6373 4c61 796f 7574 5769 6467  aphicsLayoutWidg
+00009ab0: 6574 2873 656c 662e 7461 625f 7265 7375  et(self.tab_resu
+00009ac0: 6c74 735f 6f62 735f 706c 6f74 7329 0a20  lts_obs_plots). 
+00009ad0: 2020 2020 2020 2073 656c 662e 6772 6170         self.grap
+00009ae0: 6869 6373 4c61 796f 7574 5769 6467 6574  hicsLayoutWidget
+00009af0: 5f72 6573 756c 7473 5f6f 6273 6572 7661  _results_observa
+00009b00: 7469 6f6e 735f 706c 6f74 732e 7365 744f  tions_plots.setO
+00009b10: 626a 6563 744e 616d 6528 2267 7261 7068  bjectName("graph
+00009b20: 6963 734c 6179 6f75 7457 6964 6765 745f  icsLayoutWidget_
+00009b30: 7265 7375 6c74 735f 6f62 7365 7276 6174  results_observat
+00009b40: 696f 6e73 5f70 6c6f 7473 2229 0a20 2020  ions_plots").   
+00009b50: 2020 2020 2073 656c 662e 7665 7274 6963       self.vertic
+00009b60: 616c 4c61 796f 7574 5f33 382e 6164 6457  alLayout_38.addW
+00009b70: 6964 6765 7428 7365 6c66 2e67 7261 7068  idget(self.graph
+00009b80: 6963 734c 6179 6f75 7457 6964 6765 745f  icsLayoutWidget_
+00009b90: 7265 7375 6c74 735f 6f62 7365 7276 6174  results_observat
+00009ba0: 696f 6e73 5f70 6c6f 7473 290a 2020 2020  ions_plots).    
+00009bb0: 2020 2020 7365 6c66 2e68 6f72 697a 6f6e      self.horizon
+00009bc0: 7461 6c4c 6179 6f75 7420 3d20 5174 5769  talLayout = QtWi
+00009bd0: 6467 6574 732e 5148 426f 784c 6179 6f75  dgets.QHBoxLayou
+00009be0: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
+00009bf0: 2e68 6f72 697a 6f6e 7461 6c4c 6179 6f75  .horizontalLayou
+00009c00: 742e 7365 744f 626a 6563 744e 616d 6528  t.setObjectName(
+00009c10: 2268 6f72 697a 6f6e 7461 6c4c 6179 6f75  "horizontalLayou
+00009c20: 7422 290a 2020 2020 2020 2020 7365 6c66  t").        self
+00009c30: 2e67 726f 7570 426f 785f 706c 6f74 5f73  .groupBox_plot_s
+00009c40: 6574 7469 6e67 7320 3d20 5174 5769 6467  ettings = QtWidg
+00009c50: 6574 732e 5147 726f 7570 426f 7828 7365  ets.QGroupBox(se
+00009c60: 6c66 2e74 6162 5f72 6573 756c 7473 5f6f  lf.tab_results_o
+00009c70: 6273 5f70 6c6f 7473 290a 2020 2020 2020  bs_plots).      
+00009c80: 2020 7365 6c66 2e67 726f 7570 426f 785f    self.groupBox_
+00009c90: 706c 6f74 5f73 6574 7469 6e67 732e 7365  plot_settings.se
+00009ca0: 744f 626a 6563 744e 616d 6528 2267 726f  tObjectName("gro
+00009cb0: 7570 426f 785f 706c 6f74 5f73 6574 7469  upBox_plot_setti
+00009cc0: 6e67 7322 290a 2020 2020 2020 2020 7365  ngs").        se
+00009cd0: 6c66 2e76 6572 7469 6361 6c4c 6179 6f75  lf.verticalLayou
+00009ce0: 745f 3235 203d 2051 7457 6964 6765 7473  t_25 = QtWidgets
+00009cf0: 2e51 5642 6f78 4c61 796f 7574 2873 656c  .QVBoxLayout(sel
+00009d00: 662e 6772 6f75 7042 6f78 5f70 6c6f 745f  f.groupBox_plot_
+00009d10: 7365 7474 696e 6773 290a 2020 2020 2020  settings).      
+00009d20: 2020 7365 6c66 2e76 6572 7469 6361 6c4c    self.verticalL
+00009d30: 6179 6f75 745f 3235 2e73 6574 4f62 6a65  ayout_25.setObje
+00009d40: 6374 4e61 6d65 2822 7665 7274 6963 616c  ctName("vertical
+00009d50: 4c61 796f 7574 5f32 3522 290a 2020 2020  Layout_25").    
+00009d60: 2020 2020 7365 6c66 2e66 6f72 6d4c 6179      self.formLay
+00009d70: 6f75 745f 3420 3d20 5174 5769 6467 6574  out_4 = QtWidget
+00009d80: 732e 5146 6f72 6d4c 6179 6f75 7428 290a  s.QFormLayout().
+00009d90: 2020 2020 2020 2020 7365 6c66 2e66 6f72          self.for
+00009da0: 6d4c 6179 6f75 745f 342e 7365 744f 626a  mLayout_4.setObj
+00009db0: 6563 744e 616d 6528 2266 6f72 6d4c 6179  ectName("formLay
+00009dc0: 6f75 745f 3422 290a 2020 2020 2020 2020  out_4").        
+00009dd0: 7365 6c66 2e6c 6162 656c 5f72 6573 756c  self.label_resul
+00009de0: 7473 5f6f 6273 5f70 6c6f 745f 7365 6c65  ts_obs_plot_sele
+00009df0: 635f 6461 7461 5f63 6f6c 756d 6e20 3d20  c_data_column = 
+00009e00: 5174 5769 6467 6574 732e 514c 6162 656c  QtWidgets.QLabel
+00009e10: 2873 656c 662e 6772 6f75 7042 6f78 5f70  (self.groupBox_p
+00009e20: 6c6f 745f 7365 7474 696e 6773 290a 2020  lot_settings).  
+00009e30: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
+00009e40: 5f72 6573 756c 7473 5f6f 6273 5f70 6c6f  _results_obs_plo
+00009e50: 745f 7365 6c65 635f 6461 7461 5f63 6f6c  t_selec_data_col
+00009e60: 756d 6e2e 7365 744f 626a 6563 744e 616d  umn.setObjectNam
+00009e70: 6528 226c 6162 656c 5f72 6573 756c 7473  e("label_results
+00009e80: 5f6f 6273 5f70 6c6f 745f 7365 6c65 635f  _obs_plot_selec_
+00009e90: 6461 7461 5f63 6f6c 756d 6e22 290a 2020  data_column").  
+00009ea0: 2020 2020 2020 7365 6c66 2e66 6f72 6d4c        self.formL
+00009eb0: 6179 6f75 745f 342e 7365 7457 6964 6765  ayout_4.setWidge
+00009ec0: 7428 302c 2051 7457 6964 6765 7473 2e51  t(0, QtWidgets.Q
+00009ed0: 466f 726d 4c61 796f 7574 2e4c 6162 656c  FormLayout.Label
+00009ee0: 526f 6c65 2c20 7365 6c66 2e6c 6162 656c  Role, self.label
+00009ef0: 5f72 6573 756c 7473 5f6f 6273 5f70 6c6f  _results_obs_plo
+00009f00: 745f 7365 6c65 635f 6461 7461 5f63 6f6c  t_selec_data_col
+00009f10: 756d 6e29 0a20 2020 2020 2020 2073 656c  umn).        sel
+00009f20: 662e 636f 6d62 6f42 6f78 5f72 6573 756c  f.comboBox_resul
+00009f30: 7473 5f6f 6273 5f70 6c6f 745f 7365 6c65  ts_obs_plot_sele
+00009f40: 6374 5f64 6174 615f 636f 6c75 6d6e 203d  ct_data_column =
+00009f50: 2051 7457 6964 6765 7473 2e51 436f 6d62   QtWidgets.QComb
+00009f60: 6f42 6f78 2873 656c 662e 6772 6f75 7042  oBox(self.groupB
+00009f70: 6f78 5f70 6c6f 745f 7365 7474 696e 6773  ox_plot_settings
+00009f80: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+00009f90: 6f6d 626f 426f 785f 7265 7375 6c74 735f  omboBox_results_
+00009fa0: 6f62 735f 706c 6f74 5f73 656c 6563 745f  obs_plot_select_
+00009fb0: 6461 7461 5f63 6f6c 756d 6e2e 7365 744f  data_column.setO
+00009fc0: 626a 6563 744e 616d 6528 2263 6f6d 626f  bjectName("combo
+00009fd0: 426f 785f 7265 7375 6c74 735f 6f62 735f  Box_results_obs_
+00009fe0: 706c 6f74 5f73 656c 6563 745f 6461 7461  plot_select_data
+00009ff0: 5f63 6f6c 756d 6e22 290a 2020 2020 2020  _column").      
+0000a000: 2020 7365 6c66 2e66 6f72 6d4c 6179 6f75    self.formLayou
+0000a010: 745f 342e 7365 7457 6964 6765 7428 302c  t_4.setWidget(0,
+0000a020: 2051 7457 6964 6765 7473 2e51 466f 726d   QtWidgets.QForm
+0000a030: 4c61 796f 7574 2e46 6965 6c64 526f 6c65  Layout.FieldRole
+0000a040: 2c20 7365 6c66 2e63 6f6d 626f 426f 785f  , self.comboBox_
+0000a050: 7265 7375 6c74 735f 6f62 735f 706c 6f74  results_obs_plot
+0000a060: 5f73 656c 6563 745f 6461 7461 5f63 6f6c  _select_data_col
+0000a070: 756d 6e29 0a20 2020 2020 2020 2073 656c  umn).        sel
+0000a080: 662e 7665 7274 6963 616c 4c61 796f 7574  f.verticalLayout
+0000a090: 5f32 352e 6164 644c 6179 6f75 7428 7365  _25.addLayout(se
+0000a0a0: 6c66 2e66 6f72 6d4c 6179 6f75 745f 3429  lf.formLayout_4)
+0000a0b0: 0a20 2020 2020 2020 2073 656c 662e 7261  .        self.ra
+0000a0c0: 6469 6f42 7574 746f 6e5f 7265 7375 6c74  dioButton_result
+0000a0d0: 735f 6f62 735f 706c 6f74 5f74 696d 6573  s_obs_plot_times
+0000a0e0: 6572 6965 7320 3d20 5174 5769 6467 6574  eries = QtWidget
+0000a0f0: 732e 5152 6164 696f 4275 7474 6f6e 2873  s.QRadioButton(s
+0000a100: 656c 662e 6772 6f75 7042 6f78 5f70 6c6f  elf.groupBox_plo
+0000a110: 745f 7365 7474 696e 6773 290a 2020 2020  t_settings).    
+0000a120: 2020 2020 7365 6c66 2e72 6164 696f 4275      self.radioBu
+0000a130: 7474 6f6e 5f72 6573 756c 7473 5f6f 6273  tton_results_obs
+0000a140: 5f70 6c6f 745f 7469 6d65 7365 7269 6573  _plot_timeseries
+0000a150: 2e73 6574 4368 6563 6b65 6428 5472 7565  .setChecked(True
+0000a160: 290a 2020 2020 2020 2020 7365 6c66 2e72  ).        self.r
+0000a170: 6164 696f 4275 7474 6f6e 5f72 6573 756c  adioButton_resul
+0000a180: 7473 5f6f 6273 5f70 6c6f 745f 7469 6d65  ts_obs_plot_time
+0000a190: 7365 7269 6573 2e73 6574 4f62 6a65 6374  series.setObject
+0000a1a0: 4e61 6d65 2822 7261 6469 6f42 7574 746f  Name("radioButto
+0000a1b0: 6e5f 7265 7375 6c74 735f 6f62 735f 706c  n_results_obs_pl
+0000a1c0: 6f74 5f74 696d 6573 6572 6965 7322 290a  ot_timeseries").
+0000a1d0: 2020 2020 2020 2020 7365 6c66 2e76 6572          self.ver
+0000a1e0: 7469 6361 6c4c 6179 6f75 745f 3235 2e61  ticalLayout_25.a
+0000a1f0: 6464 5769 6467 6574 2873 656c 662e 7261  ddWidget(self.ra
+0000a200: 6469 6f42 7574 746f 6e5f 7265 7375 6c74  dioButton_result
+0000a210: 735f 6f62 735f 706c 6f74 5f74 696d 6573  s_obs_plot_times
+0000a220: 6572 6965 7329 0a20 2020 2020 2020 2073  eries).        s
+0000a230: 656c 662e 7261 6469 6f42 7574 746f 6e5f  elf.radioButton_
+0000a240: 7265 7375 6c74 735f 6f62 735f 706c 6f74  results_obs_plot
+0000a250: 5f68 6973 746f 6772 616d 203d 2051 7457  _histogram = QtW
+0000a260: 6964 6765 7473 2e51 5261 6469 6f42 7574  idgets.QRadioBut
+0000a270: 746f 6e28 7365 6c66 2e67 726f 7570 426f  ton(self.groupBo
+0000a280: 785f 706c 6f74 5f73 6574 7469 6e67 7329  x_plot_settings)
+0000a290: 0a20 2020 2020 2020 2073 656c 662e 7261  .        self.ra
+0000a2a0: 6469 6f42 7574 746f 6e5f 7265 7375 6c74  dioButton_result
+0000a2b0: 735f 6f62 735f 706c 6f74 5f68 6973 746f  s_obs_plot_histo
+0000a2c0: 6772 616d 2e73 6574 4f62 6a65 6374 4e61  gram.setObjectNa
+0000a2d0: 6d65 2822 7261 6469 6f42 7574 746f 6e5f  me("radioButton_
+0000a2e0: 7265 7375 6c74 735f 6f62 735f 706c 6f74  results_obs_plot
+0000a2f0: 5f68 6973 746f 6772 616d 2229 0a20 2020  _histogram").   
+0000a300: 2020 2020 2073 656c 662e 7665 7274 6963       self.vertic
+0000a310: 616c 4c61 796f 7574 5f32 352e 6164 6457  alLayout_25.addW
+0000a320: 6964 6765 7428 7365 6c66 2e72 6164 696f  idget(self.radio
+0000a330: 4275 7474 6f6e 5f72 6573 756c 7473 5f6f  Button_results_o
+0000a340: 6273 5f70 6c6f 745f 6869 7374 6f67 7261  bs_plot_histogra
+0000a350: 6d29 0a20 2020 2020 2020 2073 656c 662e  m).        self.
+0000a360: 686f 7269 7a6f 6e74 616c 4c61 796f 7574  horizontalLayout
+0000a370: 2e61 6464 5769 6467 6574 2873 656c 662e  .addWidget(self.
+0000a380: 6772 6f75 7042 6f78 5f70 6c6f 745f 7365  groupBox_plot_se
+0000a390: 7474 696e 6773 290a 2020 2020 2020 2020  ttings).        
+0000a3a0: 7365 6c66 2e67 726f 7570 426f 785f 6869  self.groupBox_hi
+0000a3b0: 7374 6f67 7261 6d5f 7365 7474 696e 6773  stogram_settings
+0000a3c0: 203d 2051 7457 6964 6765 7473 2e51 4772   = QtWidgets.QGr
+0000a3d0: 6f75 7042 6f78 2873 656c 662e 7461 625f  oupBox(self.tab_
+0000a3e0: 7265 7375 6c74 735f 6f62 735f 706c 6f74  results_obs_plot
+0000a3f0: 7329 0a20 2020 2020 2020 2073 656c 662e  s).        self.
+0000a400: 6772 6f75 7042 6f78 5f68 6973 746f 6772  groupBox_histogr
+0000a410: 616d 5f73 6574 7469 6e67 732e 7365 7445  am_settings.setE
+0000a420: 6e61 626c 6564 2846 616c 7365 290a 2020  nabled(False).  
+0000a430: 2020 2020 2020 7365 6c66 2e67 726f 7570        self.group
+0000a440: 426f 785f 6869 7374 6f67 7261 6d5f 7365  Box_histogram_se
+0000a450: 7474 696e 6773 2e73 6574 4f62 6a65 6374  ttings.setObject
+0000a460: 4e61 6d65 2822 6772 6f75 7042 6f78 5f68  Name("groupBox_h
+0000a470: 6973 746f 6772 616d 5f73 6574 7469 6e67  istogram_setting
+0000a480: 7322 290a 2020 2020 2020 2020 7365 6c66  s").        self
+0000a490: 2e76 6572 7469 6361 6c4c 6179 6f75 745f  .verticalLayout_
+0000a4a0: 3133 203d 2051 7457 6964 6765 7473 2e51  13 = QtWidgets.Q
+0000a4b0: 5642 6f78 4c61 796f 7574 2873 656c 662e  VBoxLayout(self.
+0000a4c0: 6772 6f75 7042 6f78 5f68 6973 746f 6772  groupBox_histogr
+0000a4d0: 616d 5f73 6574 7469 6e67 7329 0a20 2020  am_settings).   
+0000a4e0: 2020 2020 2073 656c 662e 7665 7274 6963       self.vertic
+0000a4f0: 616c 4c61 796f 7574 5f31 332e 7365 744f  alLayout_13.setO
+0000a500: 626a 6563 744e 616d 6528 2276 6572 7469  bjectName("verti
+0000a510: 6361 6c4c 6179 6f75 745f 3133 2229 0a20  calLayout_13"). 
+0000a520: 2020 2020 2020 2073 656c 662e 666f 726d         self.form
+0000a530: 4c61 796f 7574 5f38 203d 2051 7457 6964  Layout_8 = QtWid
+0000a540: 6765 7473 2e51 466f 726d 4c61 796f 7574  gets.QFormLayout
+0000a550: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+0000a560: 666f 726d 4c61 796f 7574 5f38 2e73 6574  formLayout_8.set
+0000a570: 4f62 6a65 6374 4e61 6d65 2822 666f 726d  ObjectName("form
+0000a580: 4c61 796f 7574 5f38 2229 0a20 2020 2020  Layout_8").     
+0000a590: 2020 2073 656c 662e 6c61 6265 6c5f 3131     self.label_11
+0000a5a0: 203d 2051 7457 6964 6765 7473 2e51 4c61   = QtWidgets.QLa
+0000a5b0: 6265 6c28 7365 6c66 2e67 726f 7570 426f  bel(self.groupBo
+0000a5c0: 785f 6869 7374 6f67 7261 6d5f 7365 7474  x_histogram_sett
+0000a5d0: 696e 6773 290a 2020 2020 2020 2020 7365  ings).        se
+0000a5e0: 6c66 2e6c 6162 656c 5f31 312e 7365 744f  lf.label_11.setO
+0000a5f0: 626a 6563 744e 616d 6528 226c 6162 656c  bjectName("label
+0000a600: 5f31 3122 290a 2020 2020 2020 2020 7365  _11").        se
+0000a610: 6c66 2e66 6f72 6d4c 6179 6f75 745f 382e  lf.formLayout_8.
+0000a620: 7365 7457 6964 6765 7428 302c 2051 7457  setWidget(0, QtW
+0000a630: 6964 6765 7473 2e51 466f 726d 4c61 796f  idgets.QFormLayo
+0000a640: 7574 2e4c 6162 656c 526f 6c65 2c20 7365  ut.LabelRole, se
+0000a650: 6c66 2e6c 6162 656c 5f31 3129 0a20 2020  lf.label_11).   
+0000a660: 2020 2020 2073 656c 662e 636f 6d62 6f42       self.comboB
+0000a670: 6f78 5f72 6573 756c 7473 5f6f 6273 5f70  ox_results_obs_p
+0000a680: 6c6f 745f 6869 7374 5f6d 6574 686f 6420  lot_hist_method 
+0000a690: 3d20 5174 5769 6467 6574 732e 5143 6f6d  = QtWidgets.QCom
+0000a6a0: 626f 426f 7828 7365 6c66 2e67 726f 7570  boBox(self.group
+0000a6b0: 426f 785f 6869 7374 6f67 7261 6d5f 7365  Box_histogram_se
+0000a6c0: 7474 696e 6773 290a 2020 2020 2020 2020  ttings).        
+0000a6d0: 7365 6c66 2e63 6f6d 626f 426f 785f 7265  self.comboBox_re
+0000a6e0: 7375 6c74 735f 6f62 735f 706c 6f74 5f68  sults_obs_plot_h
+0000a6f0: 6973 745f 6d65 7468 6f64 2e73 6574 4f62  ist_method.setOb
+0000a700: 6a65 6374 4e61 6d65 2822 636f 6d62 6f42  jectName("comboB
+0000a710: 6f78 5f72 6573 756c 7473 5f6f 6273 5f70  ox_results_obs_p
+0000a720: 6c6f 745f 6869 7374 5f6d 6574 686f 6422  lot_hist_method"
+0000a730: 290a 2020 2020 2020 2020 7365 6c66 2e66  ).        self.f
+0000a740: 6f72 6d4c 6179 6f75 745f 382e 7365 7457  ormLayout_8.setW
+0000a750: 6964 6765 7428 302c 2051 7457 6964 6765  idget(0, QtWidge
+0000a760: 7473 2e51 466f 726d 4c61 796f 7574 2e46  ts.QFormLayout.F
+0000a770: 6965 6c64 526f 6c65 2c20 7365 6c66 2e63  ieldRole, self.c
+0000a780: 6f6d 626f 426f 785f 7265 7375 6c74 735f  omboBox_results_
+0000a790: 6f62 735f 706c 6f74 5f68 6973 745f 6d65  obs_plot_hist_me
+0000a7a0: 7468 6f64 290a 2020 2020 2020 2020 7365  thod).        se
+0000a7b0: 6c66 2e6c 6162 656c 5f72 6573 756c 7473  lf.label_results
+0000a7c0: 5f6f 6273 5f70 6c6f 745f 6e75 6d62 6572  _obs_plot_number
+0000a7d0: 5f62 696e 7320 3d20 5174 5769 6467 6574  _bins = QtWidget
+0000a7e0: 732e 514c 6162 656c 2873 656c 662e 6772  s.QLabel(self.gr
+0000a7f0: 6f75 7042 6f78 5f68 6973 746f 6772 616d  oupBox_histogram
+0000a800: 5f73 6574 7469 6e67 7329 0a20 2020 2020  _settings).     
+0000a810: 2020 2073 656c 662e 6c61 6265 6c5f 7265     self.label_re
+0000a820: 7375 6c74 735f 6f62 735f 706c 6f74 5f6e  sults_obs_plot_n
+0000a830: 756d 6265 725f 6269 6e73 2e73 6574 4f62  umber_bins.setOb
+0000a840: 6a65 6374 4e61 6d65 2822 6c61 6265 6c5f  jectName("label_
+0000a850: 7265 7375 6c74 735f 6f62 735f 706c 6f74  results_obs_plot
+0000a860: 5f6e 756d 6265 725f 6269 6e73 2229 0a20  _number_bins"). 
+0000a870: 2020 2020 2020 2073 656c 662e 666f 726d         self.form
+0000a880: 4c61 796f 7574 5f38 2e73 6574 5769 6467  Layout_8.setWidg
+0000a890: 6574 2831 2c20 5174 5769 6467 6574 732e  et(1, QtWidgets.
+0000a8a0: 5146 6f72 6d4c 6179 6f75 742e 4c61 6265  QFormLayout.Labe
+0000a8b0: 6c52 6f6c 652c 2073 656c 662e 6c61 6265  lRole, self.labe
+0000a8c0: 6c5f 7265 7375 6c74 735f 6f62 735f 706c  l_results_obs_pl
+0000a8d0: 6f74 5f6e 756d 6265 725f 6269 6e73 290a  ot_number_bins).
+0000a8e0: 2020 2020 2020 2020 7365 6c66 2e73 7069          self.spi
+0000a8f0: 6e42 6f78 5f72 6573 756c 7473 5f6f 6273  nBox_results_obs
+0000a900: 5f70 6c6f 745f 6e75 6d62 6572 5f62 696e  _plot_number_bin
+0000a910: 7320 3d20 5174 5769 6467 6574 732e 5153  s = QtWidgets.QS
+0000a920: 7069 6e42 6f78 2873 656c 662e 6772 6f75  pinBox(self.grou
+0000a930: 7042 6f78 5f68 6973 746f 6772 616d 5f73  pBox_histogram_s
+0000a940: 6574 7469 6e67 7329 0a20 2020 2020 2020  ettings).       
+0000a950: 2073 656c 662e 7370 696e 426f 785f 7265   self.spinBox_re
+0000a960: 7375 6c74 735f 6f62 735f 706c 6f74 5f6e  sults_obs_plot_n
+0000a970: 756d 6265 725f 6269 6e73 2e73 6574 4d69  umber_bins.setMi
+0000a980: 6e69 6d75 6d28 3229 0a20 2020 2020 2020  nimum(2).       
+0000a990: 2073 656c 662e 7370 696e 426f 785f 7265   self.spinBox_re
+0000a9a0: 7375 6c74 735f 6f62 735f 706c 6f74 5f6e  sults_obs_plot_n
+0000a9b0: 756d 6265 725f 6269 6e73 2e73 6574 4d61  umber_bins.setMa
+0000a9c0: 7869 6d75 6d28 3130 3030 290a 2020 2020  ximum(1000).    
+0000a9d0: 2020 2020 7365 6c66 2e73 7069 6e42 6f78      self.spinBox
+0000a9e0: 5f72 6573 756c 7473 5f6f 6273 5f70 6c6f  _results_obs_plo
+0000a9f0: 745f 6e75 6d62 6572 5f62 696e 732e 7365  t_number_bins.se
+0000aa00: 7450 726f 7065 7274 7928 2276 616c 7565  tProperty("value
+0000aa10: 222c 2031 3029 0a20 2020 2020 2020 2073  ", 10).        s
+0000aa20: 656c 662e 7370 696e 426f 785f 7265 7375  elf.spinBox_resu
+0000aa30: 6c74 735f 6f62 735f 706c 6f74 5f6e 756d  lts_obs_plot_num
+0000aa40: 6265 725f 6269 6e73 2e73 6574 4f62 6a65  ber_bins.setObje
+0000aa50: 6374 4e61 6d65 2822 7370 696e 426f 785f  ctName("spinBox_
+0000aa60: 7265 7375 6c74 735f 6f62 735f 706c 6f74  results_obs_plot
+0000aa70: 5f6e 756d 6265 725f 6269 6e73 2229 0a20  _number_bins"). 
+0000aa80: 2020 2020 2020 2073 656c 662e 666f 726d         self.form
+0000aa90: 4c61 796f 7574 5f38 2e73 6574 5769 6467  Layout_8.setWidg
+0000aaa0: 6574 2831 2c20 5174 5769 6467 6574 732e  et(1, QtWidgets.
+0000aab0: 5146 6f72 6d4c 6179 6f75 742e 4669 656c  QFormLayout.Fiel
+0000aac0: 6452 6f6c 652c 2073 656c 662e 7370 696e  dRole, self.spin
+0000aad0: 426f 785f 7265 7375 6c74 735f 6f62 735f  Box_results_obs_
+0000aae0: 706c 6f74 5f6e 756d 6265 725f 6269 6e73  plot_number_bins
+0000aaf0: 290a 2020 2020 2020 2020 7365 6c66 2e76  ).        self.v
+0000ab00: 6572 7469 6361 6c4c 6179 6f75 745f 3133  erticalLayout_13
+0000ab10: 2e61 6464 4c61 796f 7574 2873 656c 662e  .addLayout(self.
+0000ab20: 666f 726d 4c61 796f 7574 5f38 290a 2020  formLayout_8).  
+0000ab30: 2020 2020 2020 7365 6c66 2e63 6865 636b        self.check
+0000ab40: 426f 785f 7265 7375 6c74 735f 6f62 735f  Box_results_obs_
+0000ab50: 706c 6f74 5f73 686f 775f 6f75 746c 6965  plot_show_outlie
+0000ab60: 7273 203d 2051 7457 6964 6765 7473 2e51  rs = QtWidgets.Q
+0000ab70: 4368 6563 6b42 6f78 2873 656c 662e 6772  CheckBox(self.gr
+0000ab80: 6f75 7042 6f78 5f68 6973 746f 6772 616d  oupBox_histogram
+0000ab90: 5f73 6574 7469 6e67 7329 0a20 2020 2020  _settings).     
+0000aba0: 2020 2073 656c 662e 6368 6563 6b42 6f78     self.checkBox
+0000abb0: 5f72 6573 756c 7473 5f6f 6273 5f70 6c6f  _results_obs_plo
+0000abc0: 745f 7368 6f77 5f6f 7574 6c69 6572 732e  t_show_outliers.
+0000abd0: 7365 7445 6e61 626c 6564 2846 616c 7365  setEnabled(False
+0000abe0: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+0000abf0: 6865 636b 426f 785f 7265 7375 6c74 735f  heckBox_results_
+0000ac00: 6f62 735f 706c 6f74 5f73 686f 775f 6f75  obs_plot_show_ou
+0000ac10: 746c 6965 7273 2e73 6574 4f62 6a65 6374  tliers.setObject
+0000ac20: 4e61 6d65 2822 6368 6563 6b42 6f78 5f72  Name("checkBox_r
+0000ac30: 6573 756c 7473 5f6f 6273 5f70 6c6f 745f  esults_obs_plot_
+0000ac40: 7368 6f77 5f6f 7574 6c69 6572 7322 290a  show_outliers").
+0000ac50: 2020 2020 2020 2020 7365 6c66 2e76 6572          self.ver
+0000ac60: 7469 6361 6c4c 6179 6f75 745f 3133 2e61  ticalLayout_13.a
+0000ac70: 6464 5769 6467 6574 2873 656c 662e 6368  ddWidget(self.ch
+0000ac80: 6563 6b42 6f78 5f72 6573 756c 7473 5f6f  eckBox_results_o
+0000ac90: 6273 5f70 6c6f 745f 7368 6f77 5f6f 7574  bs_plot_show_out
+0000aca0: 6c69 6572 7329 0a20 2020 2020 2020 2073  liers).        s
+0000acb0: 656c 662e 686f 7269 7a6f 6e74 616c 4c61  elf.horizontalLa
+0000acc0: 796f 7574 2e61 6464 5769 6467 6574 2873  yout.addWidget(s
+0000acd0: 656c 662e 6772 6f75 7042 6f78 5f68 6973  elf.groupBox_his
+0000ace0: 746f 6772 616d 5f73 6574 7469 6e67 7329  togram_settings)
+0000acf0: 0a20 2020 2020 2020 2073 656c 662e 7665  .        self.ve
+0000ad00: 7274 6963 616c 4c61 796f 7574 5f33 382e  rticalLayout_38.
+0000ad10: 6164 644c 6179 6f75 7428 7365 6c66 2e68  addLayout(self.h
+0000ad20: 6f72 697a 6f6e 7461 6c4c 6179 6f75 7429  orizontalLayout)
+0000ad30: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
+0000ad40: 6257 6964 6765 745f 7265 7375 6c74 732e  bWidget_results.
+0000ad50: 6164 6454 6162 2873 656c 662e 7461 625f  addTab(self.tab_
+0000ad60: 7265 7375 6c74 735f 6f62 735f 706c 6f74  results_obs_plot
+0000ad70: 732c 2022 2229 0a20 2020 2020 2020 2073  s, "").        s
+0000ad80: 656c 662e 7461 625f 7265 7375 6c74 735f  elf.tab_results_
+0000ad90: 6472 6966 7420 3d20 5174 5769 6467 6574  drift = QtWidget
+0000ada0: 732e 5157 6964 6765 7428 290a 2020 2020  s.QWidget().    
+0000adb0: 2020 2020 7365 6c66 2e74 6162 5f72 6573      self.tab_res
+0000adc0: 756c 7473 5f64 7269 6674 2e73 6574 4f62  ults_drift.setOb
+0000add0: 6a65 6374 4e61 6d65 2822 7461 625f 7265  jectName("tab_re
+0000ade0: 7375 6c74 735f 6472 6966 7422 290a 2020  sults_drift").  
+0000adf0: 2020 2020 2020 7365 6c66 2e76 6572 7469        self.verti
+0000ae00: 6361 6c4c 6179 6f75 745f 3138 203d 2051  calLayout_18 = Q
+0000ae10: 7457 6964 6765 7473 2e51 5642 6f78 4c61  tWidgets.QVBoxLa
+0000ae20: 796f 7574 2873 656c 662e 7461 625f 7265  yout(self.tab_re
+0000ae30: 7375 6c74 735f 6472 6966 7429 0a20 2020  sults_drift).   
+0000ae40: 2020 2020 2073 656c 662e 7665 7274 6963       self.vertic
+0000ae50: 616c 4c61 796f 7574 5f31 382e 7365 744f  alLayout_18.setO
+0000ae60: 626a 6563 744e 616d 6528 2276 6572 7469  bjectName("verti
+0000ae70: 6361 6c4c 6179 6f75 745f 3138 2229 0a20  calLayout_18"). 
+0000ae80: 2020 2020 2020 2073 656c 662e 7461 626c         self.tabl
+0000ae90: 6556 6965 775f 7265 7375 6c74 735f 6472  eView_results_dr
+0000aea0: 6966 7420 3d20 5174 5769 6467 6574 732e  ift = QtWidgets.
+0000aeb0: 5154 6162 6c65 5669 6577 2873 656c 662e  QTableView(self.
+0000aec0: 7461 625f 7265 7375 6c74 735f 6472 6966  tab_results_drif
+0000aed0: 7429 0a20 2020 2020 2020 2073 656c 662e  t).        self.
+0000aee0: 7461 626c 6556 6965 775f 7265 7375 6c74  tableView_result
+0000aef0: 735f 6472 6966 742e 7365 744f 626a 6563  s_drift.setObjec
+0000af00: 744e 616d 6528 2274 6162 6c65 5669 6577  tName("tableView
+0000af10: 5f72 6573 756c 7473 5f64 7269 6674 2229  _results_drift")
+0000af20: 0a20 2020 2020 2020 2073 656c 662e 7665  .        self.ve
+0000af30: 7274 6963 616c 4c61 796f 7574 5f31 382e  rticalLayout_18.
+0000af40: 6164 6457 6964 6765 7428 7365 6c66 2e74  addWidget(self.t
+0000af50: 6162 6c65 5669 6577 5f72 6573 756c 7473  ableView_results
+0000af60: 5f64 7269 6674 290a 2020 2020 2020 2020  _drift).        
+0000af70: 7365 6c66 2e74 6162 5769 6467 6574 5f72  self.tabWidget_r
+0000af80: 6573 756c 7473 2e61 6464 5461 6228 7365  esults.addTab(se
+0000af90: 6c66 2e74 6162 5f72 6573 756c 7473 5f64  lf.tab_results_d
+0000afa0: 7269 6674 2c20 2222 290a 2020 2020 2020  rift, "").      
+0000afb0: 2020 7365 6c66 2e74 6162 5f72 6573 756c    self.tab_resul
+0000afc0: 7473 5f64 7269 6674 706c 6f74 203d 2051  ts_driftplot = Q
+0000afd0: 7457 6964 6765 7473 2e51 5769 6467 6574  tWidgets.QWidget
+0000afe0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+0000aff0: 7461 625f 7265 7375 6c74 735f 6472 6966  tab_results_drif
+0000b000: 7470 6c6f 742e 7365 744f 626a 6563 744e  tplot.setObjectN
+0000b010: 616d 6528 2274 6162 5f72 6573 756c 7473  ame("tab_results
+0000b020: 5f64 7269 6674 706c 6f74 2229 0a20 2020  _driftplot").   
+0000b030: 2020 2020 2073 656c 662e 7665 7274 6963       self.vertic
+0000b040: 616c 4c61 796f 7574 5f32 3920 3d20 5174  alLayout_29 = Qt
+0000b050: 5769 6467 6574 732e 5156 426f 784c 6179  Widgets.QVBoxLay
+0000b060: 6f75 7428 7365 6c66 2e74 6162 5f72 6573  out(self.tab_res
+0000b070: 756c 7473 5f64 7269 6674 706c 6f74 290a  ults_driftplot).
+0000b080: 2020 2020 2020 2020 7365 6c66 2e76 6572          self.ver
+0000b090: 7469 6361 6c4c 6179 6f75 745f 3239 2e73  ticalLayout_29.s
+0000b0a0: 6574 4f62 6a65 6374 4e61 6d65 2822 7665  etObjectName("ve
+0000b0b0: 7274 6963 616c 4c61 796f 7574 5f32 3922  rticalLayout_29"
+0000b0c0: 290a 2020 2020 2020 2020 7365 6c66 2e76  ).        self.v
+0000b0d0: 6572 7469 6361 6c4c 6179 6f75 745f 3237  erticalLayout_27
+0000b0e0: 203d 2051 7457 6964 6765 7473 2e51 5642   = QtWidgets.QVB
+0000b0f0: 6f78 4c61 796f 7574 2829 0a20 2020 2020  oxLayout().     
+0000b100: 2020 2073 656c 662e 7665 7274 6963 616c     self.vertical
+0000b110: 4c61 796f 7574 5f32 372e 7365 744f 626a  Layout_27.setObj
+0000b120: 6563 744e 616d 6528 2276 6572 7469 6361  ectName("vertica
+0000b130: 6c4c 6179 6f75 745f 3237 2229 0a20 2020  lLayout_27").   
+0000b140: 2020 2020 2073 656c 662e 6772 6170 6869       self.graphi
+0000b150: 6373 4c61 796f 7574 5769 6467 6574 5f72  csLayoutWidget_r
+0000b160: 6573 756c 7473 5f64 7269 6674 5f70 6c6f  esults_drift_plo
+0000b170: 7420 3d20 4772 6170 6869 6373 4c61 796f  t = GraphicsLayo
+0000b180: 7574 5769 6467 6574 2873 656c 662e 7461  utWidget(self.ta
+0000b190: 625f 7265 7375 6c74 735f 6472 6966 7470  b_results_driftp
+0000b1a0: 6c6f 7429 0a20 2020 2020 2020 2073 656c  lot).        sel
+0000b1b0: 662e 6772 6170 6869 6373 4c61 796f 7574  f.graphicsLayout
+0000b1c0: 5769 6467 6574 5f72 6573 756c 7473 5f64  Widget_results_d
+0000b1d0: 7269 6674 5f70 6c6f 742e 7365 744f 626a  rift_plot.setObj
+0000b1e0: 6563 744e 616d 6528 2267 7261 7068 6963  ectName("graphic
+0000b1f0: 734c 6179 6f75 7457 6964 6765 745f 7265  sLayoutWidget_re
+0000b200: 7375 6c74 735f 6472 6966 745f 706c 6f74  sults_drift_plot
+0000b210: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+0000b220: 7665 7274 6963 616c 4c61 796f 7574 5f32  verticalLayout_2
+0000b230: 372e 6164 6457 6964 6765 7428 7365 6c66  7.addWidget(self
+0000b240: 2e67 7261 7068 6963 734c 6179 6f75 7457  .graphicsLayoutW
+0000b250: 6964 6765 745f 7265 7375 6c74 735f 6472  idget_results_dr
+0000b260: 6966 745f 706c 6f74 290a 2020 2020 2020  ift_plot).      
+0000b270: 2020 7365 6c66 2e67 726f 7570 426f 785f    self.groupBox_
+0000b280: 7265 7375 6c74 735f 6472 6966 745f 706c  results_drift_pl
+0000b290: 6f74 203d 2051 7457 6964 6765 7473 2e51  ot = QtWidgets.Q
+0000b2a0: 4772 6f75 7042 6f78 2873 656c 662e 7461  GroupBox(self.ta
+0000b2b0: 625f 7265 7375 6c74 735f 6472 6966 7470  b_results_driftp
+0000b2c0: 6c6f 7429 0a20 2020 2020 2020 2073 656c  lot).        sel
+0000b2d0: 662e 6772 6f75 7042 6f78 5f72 6573 756c  f.groupBox_resul
+0000b2e0: 7473 5f64 7269 6674 5f70 6c6f 742e 7365  ts_drift_plot.se
+0000b2f0: 7445 6e61 626c 6564 2854 7275 6529 0a20  tEnabled(True). 
+0000b300: 2020 2020 2020 2073 656c 662e 6772 6f75         self.grou
+0000b310: 7042 6f78 5f72 6573 756c 7473 5f64 7269  pBox_results_dri
+0000b320: 6674 5f70 6c6f 742e 7365 744f 626a 6563  ft_plot.setObjec
+0000b330: 744e 616d 6528 2267 726f 7570 426f 785f  tName("groupBox_
+0000b340: 7265 7375 6c74 735f 6472 6966 745f 706c  results_drift_pl
+0000b350: 6f74 2229 0a20 2020 2020 2020 2073 656c  ot").        sel
+0000b360: 662e 7665 7274 6963 616c 4c61 796f 7574  f.verticalLayout
+0000b370: 5f32 3620 3d20 5174 5769 6467 6574 732e  _26 = QtWidgets.
+0000b380: 5156 426f 784c 6179 6f75 7428 7365 6c66  QVBoxLayout(self
+0000b390: 2e67 726f 7570 426f 785f 7265 7375 6c74  .groupBox_result
+0000b3a0: 735f 6472 6966 745f 706c 6f74 290a 2020  s_drift_plot).  
+0000b3b0: 2020 2020 2020 7365 6c66 2e76 6572 7469        self.verti
+0000b3c0: 6361 6c4c 6179 6f75 745f 3236 2e73 6574  calLayout_26.set
+0000b3d0: 4f62 6a65 6374 4e61 6d65 2822 7665 7274  ObjectName("vert
+0000b3e0: 6963 616c 4c61 796f 7574 5f32 3622 290a  icalLayout_26").
+0000b3f0: 2020 2020 2020 2020 7365 6c66 2e66 6f72          self.for
+0000b400: 6d4c 6179 6f75 745f 3520 3d20 5174 5769  mLayout_5 = QtWi
+0000b410: 6467 6574 732e 5146 6f72 6d4c 6179 6f75  dgets.QFormLayou
+0000b420: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
+0000b430: 2e66 6f72 6d4c 6179 6f75 745f 352e 7365  .formLayout_5.se
+0000b440: 744f 626a 6563 744e 616d 6528 2266 6f72  tObjectName("for
+0000b450: 6d4c 6179 6f75 745f 3522 290a 2020 2020  mLayout_5").    
+0000b460: 2020 2020 7365 6c66 2e6c 6162 656c 5f72      self.label_r
+0000b470: 6573 756c 7473 5f64 7269 6674 5f70 6c6f  esults_drift_plo
+0000b480: 745f 765f 6f66 6673 6574 203d 2051 7457  t_v_offset = QtW
+0000b490: 6964 6765 7473 2e51 4c61 6265 6c28 7365  idgets.QLabel(se
+0000b4a0: 6c66 2e67 726f 7570 426f 785f 7265 7375  lf.groupBox_resu
+0000b4b0: 6c74 735f 6472 6966 745f 706c 6f74 290a  lts_drift_plot).
+0000b4c0: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
+0000b4d0: 656c 5f72 6573 756c 7473 5f64 7269 6674  el_results_drift
+0000b4e0: 5f70 6c6f 745f 765f 6f66 6673 6574 2e73  _plot_v_offset.s
+0000b4f0: 6574 456e 6162 6c65 6428 4661 6c73 6529  etEnabled(False)
+0000b500: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
+0000b510: 6265 6c5f 7265 7375 6c74 735f 6472 6966  bel_results_drif
+0000b520: 745f 706c 6f74 5f76 5f6f 6666 7365 742e  t_plot_v_offset.
+0000b530: 7365 744f 626a 6563 744e 616d 6528 226c  setObjectName("l
+0000b540: 6162 656c 5f72 6573 756c 7473 5f64 7269  abel_results_dri
+0000b550: 6674 5f70 6c6f 745f 765f 6f66 6673 6574  ft_plot_v_offset
+0000b560: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+0000b570: 666f 726d 4c61 796f 7574 5f35 2e73 6574  formLayout_5.set
+0000b580: 5769 6467 6574 2830 2c20 5174 5769 6467  Widget(0, QtWidg
+0000b590: 6574 732e 5146 6f72 6d4c 6179 6f75 742e  ets.QFormLayout.
+0000b5a0: 4c61 6265 6c52 6f6c 652c 2073 656c 662e  LabelRole, self.
+0000b5b0: 6c61 6265 6c5f 7265 7375 6c74 735f 6472  label_results_dr
+0000b5c0: 6966 745f 706c 6f74 5f76 5f6f 6666 7365  ift_plot_v_offse
+0000b5d0: 7429 0a20 2020 2020 2020 2073 656c 662e  t).        self.
+0000b5e0: 7370 696e 426f 785f 7265 7375 6c74 735f  spinBox_results_
+0000b5f0: 6472 6966 745f 706c 6f74 5f76 5f6f 6666  drift_plot_v_off
+0000b600: 7365 7420 3d20 5174 5769 6467 6574 732e  set = QtWidgets.
+0000b610: 5153 7069 6e42 6f78 2873 656c 662e 6772  QSpinBox(self.gr
+0000b620: 6f75 7042 6f78 5f72 6573 756c 7473 5f64  oupBox_results_d
+0000b630: 7269 6674 5f70 6c6f 7429 0a20 2020 2020  rift_plot).     
+0000b640: 2020 2073 656c 662e 7370 696e 426f 785f     self.spinBox_
+0000b650: 7265 7375 6c74 735f 6472 6966 745f 706c  results_drift_pl
+0000b660: 6f74 5f76 5f6f 6666 7365 742e 7365 7445  ot_v_offset.setE
+0000b670: 6e61 626c 6564 2846 616c 7365 290a 2020  nabled(False).  
+0000b680: 2020 2020 2020 7365 6c66 2e73 7069 6e42        self.spinB
+0000b690: 6f78 5f72 6573 756c 7473 5f64 7269 6674  ox_results_drift
+0000b6a0: 5f70 6c6f 745f 765f 6f66 6673 6574 2e73  _plot_v_offset.s
+0000b6b0: 6574 4d69 6e69 6d75 6d28 2d31 3030 3029  etMinimum(-1000)
+0000b6c0: 0a20 2020 2020 2020 2073 656c 662e 7370  .        self.sp
+0000b6d0: 696e 426f 785f 7265 7375 6c74 735f 6472  inBox_results_dr
+0000b6e0: 6966 745f 706c 6f74 5f76 5f6f 6666 7365  ift_plot_v_offse
+0000b6f0: 742e 7365 744d 6178 696d 756d 2831 3030  t.setMaximum(100
+0000b700: 3029 0a20 2020 2020 2020 2073 656c 662e  0).        self.
+0000b710: 7370 696e 426f 785f 7265 7375 6c74 735f  spinBox_results_
+0000b720: 6472 6966 745f 706c 6f74 5f76 5f6f 6666  drift_plot_v_off
+0000b730: 7365 742e 7365 744f 626a 6563 744e 616d  set.setObjectNam
+0000b740: 6528 2273 7069 6e42 6f78 5f72 6573 756c  e("spinBox_resul
+0000b750: 7473 5f64 7269 6674 5f70 6c6f 745f 765f  ts_drift_plot_v_
+0000b760: 6f66 6673 6574 2229 0a20 2020 2020 2020  offset").       
+0000b770: 2073 656c 662e 666f 726d 4c61 796f 7574   self.formLayout
+0000b780: 5f35 2e73 6574 5769 6467 6574 2830 2c20  _5.setWidget(0, 
+0000b790: 5174 5769 6467 6574 732e 5146 6f72 6d4c  QtWidgets.QFormL
+0000b7a0: 6179 6f75 742e 4669 656c 6452 6f6c 652c  ayout.FieldRole,
+0000b7b0: 2073 656c 662e 7370 696e 426f 785f 7265   self.spinBox_re
+0000b7c0: 7375 6c74 735f 6472 6966 745f 706c 6f74  sults_drift_plot
+0000b7d0: 5f76 5f6f 6666 7365 7429 0a20 2020 2020  _v_offset).     
+0000b7e0: 2020 2073 656c 662e 7665 7274 6963 616c     self.vertical
+0000b7f0: 4c61 796f 7574 5f32 362e 6164 644c 6179  Layout_26.addLay
+0000b800: 6f75 7428 7365 6c66 2e66 6f72 6d4c 6179  out(self.formLay
+0000b810: 6f75 745f 3529 0a20 2020 2020 2020 2073  out_5).        s
+0000b820: 656c 662e 7665 7274 6963 616c 4c61 796f  elf.verticalLayo
+0000b830: 7574 5f32 372e 6164 6457 6964 6765 7428  ut_27.addWidget(
+0000b840: 7365 6c66 2e67 726f 7570 426f 785f 7265  self.groupBox_re
+0000b850: 7375 6c74 735f 6472 6966 745f 706c 6f74  sults_drift_plot
+0000b860: 290a 2020 2020 2020 2020 7365 6c66 2e76  ).        self.v
+0000b870: 6572 7469 6361 6c4c 6179 6f75 745f 3239  erticalLayout_29
+0000b880: 2e61 6464 4c61 796f 7574 2873 656c 662e  .addLayout(self.
+0000b890: 7665 7274 6963 616c 4c61 796f 7574 5f32  verticalLayout_2
+0000b8a0: 3729 0a20 2020 2020 2020 2073 656c 662e  7).        self.
+0000b8b0: 7461 6257 6964 6765 745f 7265 7375 6c74  tabWidget_result
+0000b8c0: 732e 6164 6454 6162 2873 656c 662e 7461  s.addTab(self.ta
+0000b8d0: 625f 7265 7375 6c74 735f 6472 6966 7470  b_results_driftp
+0000b8e0: 6c6f 742c 2022 2229 0a20 2020 2020 2020  lot, "").       
+0000b8f0: 2073 656c 662e 7461 625f 7265 7375 6c74   self.tab_result
+0000b900: 735f 7374 6174 5f74 6162 6c65 203d 2051  s_stat_table = Q
+0000b910: 7457 6964 6765 7473 2e51 5769 6467 6574  tWidgets.QWidget
+0000b920: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+0000b930: 7461 625f 7265 7375 6c74 735f 7374 6174  tab_results_stat
+0000b940: 5f74 6162 6c65 2e73 6574 4f62 6a65 6374  _table.setObject
+0000b950: 4e61 6d65 2822 7461 625f 7265 7375 6c74  Name("tab_result
+0000b960: 735f 7374 6174 5f74 6162 6c65 2229 0a20  s_stat_table"). 
+0000b970: 2020 2020 2020 2073 656c 662e 7665 7274         self.vert
+0000b980: 6963 616c 4c61 796f 7574 5f33 3920 3d20  icalLayout_39 = 
+0000b990: 5174 5769 6467 6574 732e 5156 426f 784c  QtWidgets.QVBoxL
+0000b9a0: 6179 6f75 7428 7365 6c66 2e74 6162 5f72  ayout(self.tab_r
+0000b9b0: 6573 756c 7473 5f73 7461 745f 7461 626c  esults_stat_tabl
+0000b9c0: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
+0000b9d0: 7665 7274 6963 616c 4c61 796f 7574 5f33  verticalLayout_3
+0000b9e0: 392e 7365 744f 626a 6563 744e 616d 6528  9.setObjectName(
+0000b9f0: 2276 6572 7469 6361 6c4c 6179 6f75 745f  "verticalLayout_
+0000ba00: 3339 2229 0a20 2020 2020 2020 2073 656c  39").        sel
+0000ba10: 662e 7461 626c 6556 6965 775f 7265 7375  f.tableView_resu
+0000ba20: 6c74 735f 7374 6174 696f 6e73 203d 2051  lts_stations = Q
+0000ba30: 7457 6964 6765 7473 2e51 5461 626c 6556  tWidgets.QTableV
+0000ba40: 6965 7728 7365 6c66 2e74 6162 5f72 6573  iew(self.tab_res
+0000ba50: 756c 7473 5f73 7461 745f 7461 626c 6529  ults_stat_table)
+0000ba60: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
+0000ba70: 626c 6556 6965 775f 7265 7375 6c74 735f  bleView_results_
+0000ba80: 7374 6174 696f 6e73 2e73 6574 4f62 6a65  stations.setObje
+0000ba90: 6374 4e61 6d65 2822 7461 626c 6556 6965  ctName("tableVie
+0000baa0: 775f 7265 7375 6c74 735f 7374 6174 696f  w_results_statio
+0000bab0: 6e73 2229 0a20 2020 2020 2020 2073 656c  ns").        sel
+0000bac0: 662e 7665 7274 6963 616c 4c61 796f 7574  f.verticalLayout
+0000bad0: 5f33 392e 6164 6457 6964 6765 7428 7365  _39.addWidget(se
+0000bae0: 6c66 2e74 6162 6c65 5669 6577 5f72 6573  lf.tableView_res
+0000baf0: 756c 7473 5f73 7461 7469 6f6e 7329 0a20  ults_stations). 
+0000bb00: 2020 2020 2020 2073 656c 662e 6772 6f75         self.grou
+0000bb10: 7042 6f78 5f72 6573 756c 7473 5f73 7461  pBox_results_sta
+0000bb20: 7469 6f6e 735f 7374 6174 6973 7469 6373  tions_statistics
+0000bb30: 203d 2051 7457 6964 6765 7473 2e51 4772   = QtWidgets.QGr
+0000bb40: 6f75 7042 6f78 2873 656c 662e 7461 625f  oupBox(self.tab_
+0000bb50: 7265 7375 6c74 735f 7374 6174 5f74 6162  results_stat_tab
+0000bb60: 6c65 290a 2020 2020 2020 2020 7365 6c66  le).        self
+0000bb70: 2e67 726f 7570 426f 785f 7265 7375 6c74  .groupBox_result
+0000bb80: 735f 7374 6174 696f 6e73 5f73 7461 7469  s_stations_stati
+0000bb90: 7374 6963 732e 7365 744f 626a 6563 744e  stics.setObjectN
+0000bba0: 616d 6528 2267 726f 7570 426f 785f 7265  ame("groupBox_re
+0000bbb0: 7375 6c74 735f 7374 6174 696f 6e73 5f73  sults_stations_s
+0000bbc0: 7461 7469 7374 6963 7322 290a 2020 2020  tatistics").    
+0000bbd0: 2020 2020 7365 6c66 2e68 6f72 697a 6f6e      self.horizon
+0000bbe0: 7461 6c4c 6179 6f75 745f 3420 3d20 5174  talLayout_4 = Qt
+0000bbf0: 5769 6467 6574 732e 5148 426f 784c 6179  Widgets.QHBoxLay
+0000bc00: 6f75 7428 7365 6c66 2e67 726f 7570 426f  out(self.groupBo
+0000bc10: 785f 7265 7375 6c74 735f 7374 6174 696f  x_results_statio
+0000bc20: 6e73 5f73 7461 7469 7374 6963 7329 0a20  ns_statistics). 
+0000bc30: 2020 2020 2020 2073 656c 662e 686f 7269         self.hori
+0000bc40: 7a6f 6e74 616c 4c61 796f 7574 5f34 2e73  zontalLayout_4.s
+0000bc50: 6574 4f62 6a65 6374 4e61 6d65 2822 686f  etObjectName("ho
+0000bc60: 7269 7a6f 6e74 616c 4c61 796f 7574 5f34  rizontalLayout_4
+0000bc70: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+0000bc80: 7665 7274 6963 616c 4c61 796f 7574 5f31  verticalLayout_1
+0000bc90: 3920 3d20 5174 5769 6467 6574 732e 5156  9 = QtWidgets.QV
+0000bca0: 426f 784c 6179 6f75 7428 290a 2020 2020  BoxLayout().    
+0000bcb0: 2020 2020 7365 6c66 2e76 6572 7469 6361      self.vertica
+0000bcc0: 6c4c 6179 6f75 745f 3139 2e73 6574 4f62  lLayout_19.setOb
+0000bcd0: 6a65 6374 4e61 6d65 2822 7665 7274 6963  jectName("vertic
+0000bce0: 616c 4c61 796f 7574 5f31 3922 290a 2020  alLayout_19").  
+0000bcf0: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
+0000bd00: 5f31 3220 3d20 5174 5769 6467 6574 732e  _12 = QtWidgets.
+0000bd10: 514c 6162 656c 2873 656c 662e 6772 6f75  QLabel(self.grou
+0000bd20: 7042 6f78 5f72 6573 756c 7473 5f73 7461  pBox_results_sta
+0000bd30: 7469 6f6e 735f 7374 6174 6973 7469 6373  tions_statistics
+0000bd40: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
+0000bd50: 6162 656c 5f31 322e 7365 744f 626a 6563  abel_12.setObjec
+0000bd60: 744e 616d 6528 226c 6162 656c 5f31 3222  tName("label_12"
+0000bd70: 290a 2020 2020 2020 2020 7365 6c66 2e76  ).        self.v
+0000bd80: 6572 7469 6361 6c4c 6179 6f75 745f 3139  erticalLayout_19
+0000bd90: 2e61 6464 5769 6467 6574 2873 656c 662e  .addWidget(self.
+0000bda0: 6c61 6265 6c5f 3132 290a 2020 2020 2020  label_12).      
+0000bdb0: 2020 7365 6c66 2e63 6f6d 626f 426f 785f    self.comboBox_
+0000bdc0: 7265 7375 6c74 735f 7374 6174 696f 6e73  results_stations
+0000bdd0: 5f73 7461 7469 7374 6963 735f 7365 6c65  _statistics_sele
+0000bde0: 6374 5f63 6f6c 203d 2051 7457 6964 6765  ct_col = QtWidge
+0000bdf0: 7473 2e51 436f 6d62 6f42 6f78 2873 656c  ts.QComboBox(sel
+0000be00: 662e 6772 6f75 7042 6f78 5f72 6573 756c  f.groupBox_resul
+0000be10: 7473 5f73 7461 7469 6f6e 735f 7374 6174  ts_stations_stat
+0000be20: 6973 7469 6373 290a 2020 2020 2020 2020  istics).        
+0000be30: 7365 6c66 2e63 6f6d 626f 426f 785f 7265  self.comboBox_re
+0000be40: 7375 6c74 735f 7374 6174 696f 6e73 5f73  sults_stations_s
+0000be50: 7461 7469 7374 6963 735f 7365 6c65 6374  tatistics_select
+0000be60: 5f63 6f6c 2e73 6574 4f62 6a65 6374 4e61  _col.setObjectNa
+0000be70: 6d65 2822 636f 6d62 6f42 6f78 5f72 6573  me("comboBox_res
 0000be80: 756c 7473 5f73 7461 7469 6f6e 735f 7374  ults_stations_st
-0000be90: 6174 6973 7469 6373 5f73 7464 203d 2051  atistics_std = Q
-0000bea0: 7457 6964 6765 7473 2e51 4c61 6265 6c28  tWidgets.QLabel(
-0000beb0: 7365 6c66 2e67 726f 7570 426f 785f 7265  self.groupBox_re
-0000bec0: 7375 6c74 735f 7374 6174 696f 6e73 5f73  sults_stations_s
-0000bed0: 7461 7469 7374 6963 7329 0a20 2020 2020  tatistics).     
-0000bee0: 2020 2073 656c 662e 6c61 6265 6c5f 7265     self.label_re
-0000bef0: 7375 6c74 735f 7374 6174 696f 6e73 5f73  sults_stations_s
-0000bf00: 7461 7469 7374 6963 735f 7374 642e 7365  tatistics_std.se
-0000bf10: 7454 6578 7428 2222 290a 2020 2020 2020  tText("").      
-0000bf20: 2020 7365 6c66 2e6c 6162 656c 5f72 6573    self.label_res
-0000bf30: 756c 7473 5f73 7461 7469 6f6e 735f 7374  ults_stations_st
-0000bf40: 6174 6973 7469 6373 5f73 7464 2e73 6574  atistics_std.set
-0000bf50: 4f62 6a65 6374 4e61 6d65 2822 6c61 6265  ObjectName("labe
-0000bf60: 6c5f 7265 7375 6c74 735f 7374 6174 696f  l_results_statio
-0000bf70: 6e73 5f73 7461 7469 7374 6963 735f 7374  ns_statistics_st
-0000bf80: 6422 290a 2020 2020 2020 2020 7365 6c66  d").        self
-0000bf90: 2e66 6f72 6d4c 6179 6f75 745f 392e 7365  .formLayout_9.se
-0000bfa0: 7457 6964 6765 7428 312c 2051 7457 6964  tWidget(1, QtWid
-0000bfb0: 6765 7473 2e51 466f 726d 4c61 796f 7574  gets.QFormLayout
-0000bfc0: 2e46 6965 6c64 526f 6c65 2c20 7365 6c66  .FieldRole, self
-0000bfd0: 2e6c 6162 656c 5f72 6573 756c 7473 5f73  .label_results_s
-0000bfe0: 7461 7469 6f6e 735f 7374 6174 6973 7469  tations_statisti
-0000bff0: 6373 5f73 7464 290a 2020 2020 2020 2020  cs_std).        
-0000c000: 7365 6c66 2e68 6f72 697a 6f6e 7461 6c4c  self.horizontalL
-0000c010: 6179 6f75 745f 342e 6164 644c 6179 6f75  ayout_4.addLayou
-0000c020: 7428 7365 6c66 2e66 6f72 6d4c 6179 6f75  t(self.formLayou
-0000c030: 745f 3929 0a20 2020 2020 2020 2073 656c  t_9).        sel
-0000c040: 662e 666f 726d 4c61 796f 7574 5f31 3020  f.formLayout_10 
-0000c050: 3d20 5174 5769 6467 6574 732e 5146 6f72  = QtWidgets.QFor
-0000c060: 6d4c 6179 6f75 7428 290a 2020 2020 2020  mLayout().      
-0000c070: 2020 7365 6c66 2e66 6f72 6d4c 6179 6f75    self.formLayou
-0000c080: 745f 3130 2e73 6574 4f62 6a65 6374 4e61  t_10.setObjectNa
-0000c090: 6d65 2822 666f 726d 4c61 796f 7574 5f31  me("formLayout_1
-0000c0a0: 3022 290a 2020 2020 2020 2020 7365 6c66  0").        self
-0000c0b0: 2e6c 6162 656c 5f31 3520 3d20 5174 5769  .label_15 = QtWi
-0000c0c0: 6467 6574 732e 514c 6162 656c 2873 656c  dgets.QLabel(sel
-0000c0d0: 662e 6772 6f75 7042 6f78 5f72 6573 756c  f.groupBox_resul
-0000c0e0: 7473 5f73 7461 7469 6f6e 735f 7374 6174  ts_stations_stat
-0000c0f0: 6973 7469 6373 290a 2020 2020 2020 2020  istics).        
-0000c100: 7365 6c66 2e6c 6162 656c 5f31 352e 7365  self.label_15.se
-0000c110: 744f 626a 6563 744e 616d 6528 226c 6162  tObjectName("lab
-0000c120: 656c 5f31 3522 290a 2020 2020 2020 2020  el_15").        
-0000c130: 7365 6c66 2e66 6f72 6d4c 6179 6f75 745f  self.formLayout_
-0000c140: 3130 2e73 6574 5769 6467 6574 2830 2c20  10.setWidget(0, 
-0000c150: 5174 5769 6467 6574 732e 5146 6f72 6d4c  QtWidgets.QFormL
-0000c160: 6179 6f75 742e 4c61 6265 6c52 6f6c 652c  ayout.LabelRole,
-0000c170: 2073 656c 662e 6c61 6265 6c5f 3135 290a   self.label_15).
-0000c180: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
-0000c190: 656c 5f72 6573 756c 7473 5f73 7461 7469  el_results_stati
-0000c1a0: 6f6e 735f 7374 6174 6973 7469 6373 5f6d  ons_statistics_m
-0000c1b0: 696e 203d 2051 7457 6964 6765 7473 2e51  in = QtWidgets.Q
-0000c1c0: 4c61 6265 6c28 7365 6c66 2e67 726f 7570  Label(self.group
-0000c1d0: 426f 785f 7265 7375 6c74 735f 7374 6174  Box_results_stat
-0000c1e0: 696f 6e73 5f73 7461 7469 7374 6963 7329  ions_statistics)
-0000c1f0: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
-0000c200: 6265 6c5f 7265 7375 6c74 735f 7374 6174  bel_results_stat
-0000c210: 696f 6e73 5f73 7461 7469 7374 6963 735f  ions_statistics_
-0000c220: 6d69 6e2e 7365 7454 6578 7428 2222 290a  min.setText("").
-0000c230: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
-0000c240: 656c 5f72 6573 756c 7473 5f73 7461 7469  el_results_stati
-0000c250: 6f6e 735f 7374 6174 6973 7469 6373 5f6d  ons_statistics_m
-0000c260: 696e 2e73 6574 4f62 6a65 6374 4e61 6d65  in.setObjectName
-0000c270: 2822 6c61 6265 6c5f 7265 7375 6c74 735f  ("label_results_
-0000c280: 7374 6174 696f 6e73 5f73 7461 7469 7374  stations_statist
-0000c290: 6963 735f 6d69 6e22 290a 2020 2020 2020  ics_min").      
-0000c2a0: 2020 7365 6c66 2e66 6f72 6d4c 6179 6f75    self.formLayou
-0000c2b0: 745f 3130 2e73 6574 5769 6467 6574 2830  t_10.setWidget(0
-0000c2c0: 2c20 5174 5769 6467 6574 732e 5146 6f72  , QtWidgets.QFor
-0000c2d0: 6d4c 6179 6f75 742e 4669 656c 6452 6f6c  mLayout.FieldRol
-0000c2e0: 652c 2073 656c 662e 6c61 6265 6c5f 7265  e, self.label_re
-0000c2f0: 7375 6c74 735f 7374 6174 696f 6e73 5f73  sults_stations_s
-0000c300: 7461 7469 7374 6963 735f 6d69 6e29 0a20  tatistics_min). 
-0000c310: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
-0000c320: 6c5f 3136 203d 2051 7457 6964 6765 7473  l_16 = QtWidgets
-0000c330: 2e51 4c61 6265 6c28 7365 6c66 2e67 726f  .QLabel(self.gro
-0000c340: 7570 426f 785f 7265 7375 6c74 735f 7374  upBox_results_st
-0000c350: 6174 696f 6e73 5f73 7461 7469 7374 6963  ations_statistic
-0000c360: 7329 0a20 2020 2020 2020 2073 656c 662e  s).        self.
-0000c370: 6c61 6265 6c5f 3136 2e73 6574 4f62 6a65  label_16.setObje
-0000c380: 6374 4e61 6d65 2822 6c61 6265 6c5f 3136  ctName("label_16
-0000c390: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-0000c3a0: 666f 726d 4c61 796f 7574 5f31 302e 7365  formLayout_10.se
-0000c3b0: 7457 6964 6765 7428 312c 2051 7457 6964  tWidget(1, QtWid
-0000c3c0: 6765 7473 2e51 466f 726d 4c61 796f 7574  gets.QFormLayout
-0000c3d0: 2e4c 6162 656c 526f 6c65 2c20 7365 6c66  .LabelRole, self
-0000c3e0: 2e6c 6162 656c 5f31 3629 0a20 2020 2020  .label_16).     
-0000c3f0: 2020 2073 656c 662e 6c61 6265 6c5f 7265     self.label_re
-0000c400: 7375 6c74 735f 7374 6174 696f 6e73 5f73  sults_stations_s
-0000c410: 7461 7469 7374 6963 735f 6d61 7820 3d20  tatistics_max = 
-0000c420: 5174 5769 6467 6574 732e 514c 6162 656c  QtWidgets.QLabel
-0000c430: 2873 656c 662e 6772 6f75 7042 6f78 5f72  (self.groupBox_r
-0000c440: 6573 756c 7473 5f73 7461 7469 6f6e 735f  esults_stations_
-0000c450: 7374 6174 6973 7469 6373 290a 2020 2020  statistics).    
-0000c460: 2020 2020 7365 6c66 2e6c 6162 656c 5f72      self.label_r
-0000c470: 6573 756c 7473 5f73 7461 7469 6f6e 735f  esults_stations_
-0000c480: 7374 6174 6973 7469 6373 5f6d 6178 2e73  statistics_max.s
-0000c490: 6574 5465 7874 2822 2229 0a20 2020 2020  etText("").     
-0000c4a0: 2020 2073 656c 662e 6c61 6265 6c5f 7265     self.label_re
-0000c4b0: 7375 6c74 735f 7374 6174 696f 6e73 5f73  sults_stations_s
-0000c4c0: 7461 7469 7374 6963 735f 6d61 782e 7365  tatistics_max.se
-0000c4d0: 744f 626a 6563 744e 616d 6528 226c 6162  tObjectName("lab
-0000c4e0: 656c 5f72 6573 756c 7473 5f73 7461 7469  el_results_stati
-0000c4f0: 6f6e 735f 7374 6174 6973 7469 6373 5f6d  ons_statistics_m
-0000c500: 6178 2229 0a20 2020 2020 2020 2073 656c  ax").        sel
-0000c510: 662e 666f 726d 4c61 796f 7574 5f31 302e  f.formLayout_10.
-0000c520: 7365 7457 6964 6765 7428 312c 2051 7457  setWidget(1, QtW
-0000c530: 6964 6765 7473 2e51 466f 726d 4c61 796f  idgets.QFormLayo
-0000c540: 7574 2e46 6965 6c64 526f 6c65 2c20 7365  ut.FieldRole, se
-0000c550: 6c66 2e6c 6162 656c 5f72 6573 756c 7473  lf.label_results
-0000c560: 5f73 7461 7469 6f6e 735f 7374 6174 6973  _stations_statis
-0000c570: 7469 6373 5f6d 6178 290a 2020 2020 2020  tics_max).      
-0000c580: 2020 7365 6c66 2e68 6f72 697a 6f6e 7461    self.horizonta
-0000c590: 6c4c 6179 6f75 745f 342e 6164 644c 6179  lLayout_4.addLay
-0000c5a0: 6f75 7428 7365 6c66 2e66 6f72 6d4c 6179  out(self.formLay
-0000c5b0: 6f75 745f 3130 290a 2020 2020 2020 2020  out_10).        
-0000c5c0: 7365 6c66 2e66 6f72 6d4c 6179 6f75 745f  self.formLayout_
-0000c5d0: 3131 203d 2051 7457 6964 6765 7473 2e51  11 = QtWidgets.Q
-0000c5e0: 466f 726d 4c61 796f 7574 2829 0a20 2020  FormLayout().   
-0000c5f0: 2020 2020 2073 656c 662e 666f 726d 4c61       self.formLa
-0000c600: 796f 7574 5f31 312e 7365 744f 626a 6563  yout_11.setObjec
-0000c610: 744e 616d 6528 2266 6f72 6d4c 6179 6f75  tName("formLayou
-0000c620: 745f 3131 2229 0a20 2020 2020 2020 2073  t_11").        s
-0000c630: 656c 662e 6c61 6265 6c5f 3137 203d 2051  elf.label_17 = Q
-0000c640: 7457 6964 6765 7473 2e51 4c61 6265 6c28  tWidgets.QLabel(
-0000c650: 7365 6c66 2e67 726f 7570 426f 785f 7265  self.groupBox_re
-0000c660: 7375 6c74 735f 7374 6174 696f 6e73 5f73  sults_stations_s
-0000c670: 7461 7469 7374 6963 7329 0a20 2020 2020  tatistics).     
-0000c680: 2020 2073 656c 662e 6c61 6265 6c5f 3137     self.label_17
-0000c690: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
-0000c6a0: 6c61 6265 6c5f 3137 2229 0a20 2020 2020  label_17").     
-0000c6b0: 2020 2073 656c 662e 666f 726d 4c61 796f     self.formLayo
-0000c6c0: 7574 5f31 312e 7365 7457 6964 6765 7428  ut_11.setWidget(
-0000c6d0: 302c 2051 7457 6964 6765 7473 2e51 466f  0, QtWidgets.QFo
-0000c6e0: 726d 4c61 796f 7574 2e4c 6162 656c 526f  rmLayout.LabelRo
-0000c6f0: 6c65 2c20 7365 6c66 2e6c 6162 656c 5f31  le, self.label_1
-0000c700: 3729 0a20 2020 2020 2020 2073 656c 662e  7).        self.
-0000c710: 6c61 6265 6c5f 5f72 6573 756c 7473 5f73  label__results_s
-0000c720: 7461 7469 6f6e 735f 7374 6174 6973 7469  tations_statisti
-0000c730: 6373 5f6d 6564 6961 6e20 3d20 5174 5769  cs_median = QtWi
-0000c740: 6467 6574 732e 514c 6162 656c 2873 656c  dgets.QLabel(sel
-0000c750: 662e 6772 6f75 7042 6f78 5f72 6573 756c  f.groupBox_resul
-0000c760: 7473 5f73 7461 7469 6f6e 735f 7374 6174  ts_stations_stat
-0000c770: 6973 7469 6373 290a 2020 2020 2020 2020  istics).        
-0000c780: 7365 6c66 2e6c 6162 656c 5f5f 7265 7375  self.label__resu
-0000c790: 6c74 735f 7374 6174 696f 6e73 5f73 7461  lts_stations_sta
-0000c7a0: 7469 7374 6963 735f 6d65 6469 616e 2e73  tistics_median.s
-0000c7b0: 6574 5465 7874 2822 2229 0a20 2020 2020  etText("").     
-0000c7c0: 2020 2073 656c 662e 6c61 6265 6c5f 5f72     self.label__r
-0000c7d0: 6573 756c 7473 5f73 7461 7469 6f6e 735f  esults_stations_
-0000c7e0: 7374 6174 6973 7469 6373 5f6d 6564 6961  statistics_media
-0000c7f0: 6e2e 7365 744f 626a 6563 744e 616d 6528  n.setObjectName(
-0000c800: 226c 6162 656c 5f5f 7265 7375 6c74 735f  "label__results_
-0000c810: 7374 6174 696f 6e73 5f73 7461 7469 7374  stations_statist
-0000c820: 6963 735f 6d65 6469 616e 2229 0a20 2020  ics_median").   
-0000c830: 2020 2020 2073 656c 662e 666f 726d 4c61       self.formLa
-0000c840: 796f 7574 5f31 312e 7365 7457 6964 6765  yout_11.setWidge
-0000c850: 7428 302c 2051 7457 6964 6765 7473 2e51  t(0, QtWidgets.Q
-0000c860: 466f 726d 4c61 796f 7574 2e46 6965 6c64  FormLayout.Field
-0000c870: 526f 6c65 2c20 7365 6c66 2e6c 6162 656c  Role, self.label
-0000c880: 5f5f 7265 7375 6c74 735f 7374 6174 696f  __results_statio
-0000c890: 6e73 5f73 7461 7469 7374 6963 735f 6d65  ns_statistics_me
-0000c8a0: 6469 616e 290a 2020 2020 2020 2020 7365  dian).        se
-0000c8b0: 6c66 2e6c 6162 656c 5f31 3820 3d20 5174  lf.label_18 = Qt
-0000c8c0: 5769 6467 6574 732e 514c 6162 656c 2873  Widgets.QLabel(s
-0000c8d0: 656c 662e 6772 6f75 7042 6f78 5f72 6573  elf.groupBox_res
-0000c8e0: 756c 7473 5f73 7461 7469 6f6e 735f 7374  ults_stations_st
-0000c8f0: 6174 6973 7469 6373 290a 2020 2020 2020  atistics).      
-0000c900: 2020 7365 6c66 2e6c 6162 656c 5f31 382e    self.label_18.
-0000c910: 7365 744f 626a 6563 744e 616d 6528 226c  setObjectName("l
-0000c920: 6162 656c 5f31 3822 290a 2020 2020 2020  abel_18").      
-0000c930: 2020 7365 6c66 2e66 6f72 6d4c 6179 6f75    self.formLayou
-0000c940: 745f 3131 2e73 6574 5769 6467 6574 2831  t_11.setWidget(1
-0000c950: 2c20 5174 5769 6467 6574 732e 5146 6f72  , QtWidgets.QFor
-0000c960: 6d4c 6179 6f75 742e 4c61 6265 6c52 6f6c  mLayout.LabelRol
-0000c970: 652c 2073 656c 662e 6c61 6265 6c5f 3138  e, self.label_18
-0000c980: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
-0000c990: 6162 656c 5f5f 7265 7375 6c74 735f 7374  abel__results_st
-0000c9a0: 6174 696f 6e73 5f73 7461 7469 7374 6963  ations_statistic
-0000c9b0: 735f 6971 7220 3d20 5174 5769 6467 6574  s_iqr = QtWidget
-0000c9c0: 732e 514c 6162 656c 2873 656c 662e 6772  s.QLabel(self.gr
-0000c9d0: 6f75 7042 6f78 5f72 6573 756c 7473 5f73  oupBox_results_s
-0000c9e0: 7461 7469 6f6e 735f 7374 6174 6973 7469  tations_statisti
-0000c9f0: 6373 290a 2020 2020 2020 2020 7365 6c66  cs).        self
-0000ca00: 2e6c 6162 656c 5f5f 7265 7375 6c74 735f  .label__results_
-0000ca10: 7374 6174 696f 6e73 5f73 7461 7469 7374  stations_statist
-0000ca20: 6963 735f 6971 722e 7365 7454 6578 7428  ics_iqr.setText(
-0000ca30: 2222 290a 2020 2020 2020 2020 7365 6c66  "").        self
-0000ca40: 2e6c 6162 656c 5f5f 7265 7375 6c74 735f  .label__results_
-0000ca50: 7374 6174 696f 6e73 5f73 7461 7469 7374  stations_statist
-0000ca60: 6963 735f 6971 722e 7365 744f 626a 6563  ics_iqr.setObjec
-0000ca70: 744e 616d 6528 226c 6162 656c 5f5f 7265  tName("label__re
-0000ca80: 7375 6c74 735f 7374 6174 696f 6e73 5f73  sults_stations_s
-0000ca90: 7461 7469 7374 6963 735f 6971 7222 290a  tatistics_iqr").
-0000caa0: 2020 2020 2020 2020 7365 6c66 2e66 6f72          self.for
-0000cab0: 6d4c 6179 6f75 745f 3131 2e73 6574 5769  mLayout_11.setWi
-0000cac0: 6467 6574 2831 2c20 5174 5769 6467 6574  dget(1, QtWidget
-0000cad0: 732e 5146 6f72 6d4c 6179 6f75 742e 4669  s.QFormLayout.Fi
-0000cae0: 656c 6452 6f6c 652c 2073 656c 662e 6c61  eldRole, self.la
-0000caf0: 6265 6c5f 5f72 6573 756c 7473 5f73 7461  bel__results_sta
-0000cb00: 7469 6f6e 735f 7374 6174 6973 7469 6373  tions_statistics
-0000cb10: 5f69 7172 290a 2020 2020 2020 2020 7365  _iqr).        se
-0000cb20: 6c66 2e68 6f72 697a 6f6e 7461 6c4c 6179  lf.horizontalLay
-0000cb30: 6f75 745f 342e 6164 644c 6179 6f75 7428  out_4.addLayout(
-0000cb40: 7365 6c66 2e66 6f72 6d4c 6179 6f75 745f  self.formLayout_
-0000cb50: 3131 290a 2020 2020 2020 2020 7365 6c66  11).        self
-0000cb60: 2e76 6572 7469 6361 6c4c 6179 6f75 745f  .verticalLayout_
-0000cb70: 3339 2e61 6464 5769 6467 6574 2873 656c  39.addWidget(sel
-0000cb80: 662e 6772 6f75 7042 6f78 5f72 6573 756c  f.groupBox_resul
-0000cb90: 7473 5f73 7461 7469 6f6e 735f 7374 6174  ts_stations_stat
-0000cba0: 6973 7469 6373 290a 2020 2020 2020 2020  istics).        
-0000cbb0: 7365 6c66 2e74 6162 5769 6467 6574 5f72  self.tabWidget_r
-0000cbc0: 6573 756c 7473 2e61 6464 5461 6228 7365  esults.addTab(se
-0000cbd0: 6c66 2e74 6162 5f72 6573 756c 7473 5f73  lf.tab_results_s
-0000cbe0: 7461 745f 7461 626c 652c 2022 2229 0a20  tat_table, ""). 
-0000cbf0: 2020 2020 2020 2073 656c 662e 7461 625f         self.tab_
-0000cc00: 7265 7375 6c74 735f 636f 7272 656c 6174  results_correlat
-0000cc10: 696f 6e5f 6d61 7472 6978 203d 2051 7457  ion_matrix = QtW
-0000cc20: 6964 6765 7473 2e51 5769 6467 6574 2829  idgets.QWidget()
-0000cc30: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
-0000cc40: 625f 7265 7375 6c74 735f 636f 7272 656c  b_results_correl
-0000cc50: 6174 696f 6e5f 6d61 7472 6978 2e73 6574  ation_matrix.set
-0000cc60: 4f62 6a65 6374 4e61 6d65 2822 7461 625f  ObjectName("tab_
-0000cc70: 7265 7375 6c74 735f 636f 7272 656c 6174  results_correlat
-0000cc80: 696f 6e5f 6d61 7472 6978 2229 0a20 2020  ion_matrix").   
-0000cc90: 2020 2020 2073 656c 662e 7665 7274 6963       self.vertic
-0000cca0: 616c 4c61 796f 7574 5f33 3220 3d20 5174  alLayout_32 = Qt
-0000ccb0: 5769 6467 6574 732e 5156 426f 784c 6179  Widgets.QVBoxLay
-0000ccc0: 6f75 7428 7365 6c66 2e74 6162 5f72 6573  out(self.tab_res
-0000ccd0: 756c 7473 5f63 6f72 7265 6c61 7469 6f6e  ults_correlation
-0000cce0: 5f6d 6174 7269 7829 0a20 2020 2020 2020  _matrix).       
-0000ccf0: 2073 656c 662e 7665 7274 6963 616c 4c61   self.verticalLa
-0000cd00: 796f 7574 5f33 322e 7365 744f 626a 6563  yout_32.setObjec
-0000cd10: 744e 616d 6528 2276 6572 7469 6361 6c4c  tName("verticalL
-0000cd20: 6179 6f75 745f 3332 2229 0a20 2020 2020  ayout_32").     
-0000cd30: 2020 2073 656c 662e 7461 626c 6556 6965     self.tableVie
-0000cd40: 775f 7265 7375 6c74 735f 636f 7272 656c  w_results_correl
-0000cd50: 6174 696f 6e5f 6d61 7472 6978 203d 2051  ation_matrix = Q
-0000cd60: 7457 6964 6765 7473 2e51 5461 626c 6556  tWidgets.QTableV
-0000cd70: 6965 7728 7365 6c66 2e74 6162 5f72 6573  iew(self.tab_res
-0000cd80: 756c 7473 5f63 6f72 7265 6c61 7469 6f6e  ults_correlation
-0000cd90: 5f6d 6174 7269 7829 0a20 2020 2020 2020  _matrix).       
-0000cda0: 2073 656c 662e 7461 626c 6556 6965 775f   self.tableView_
-0000cdb0: 7265 7375 6c74 735f 636f 7272 656c 6174  results_correlat
-0000cdc0: 696f 6e5f 6d61 7472 6978 2e73 6574 4f62  ion_matrix.setOb
-0000cdd0: 6a65 6374 4e61 6d65 2822 7461 626c 6556  jectName("tableV
-0000cde0: 6965 775f 7265 7375 6c74 735f 636f 7272  iew_results_corr
-0000cdf0: 656c 6174 696f 6e5f 6d61 7472 6978 2229  elation_matrix")
-0000ce00: 0a20 2020 2020 2020 2073 656c 662e 7665  .        self.ve
-0000ce10: 7274 6963 616c 4c61 796f 7574 5f33 322e  rticalLayout_32.
-0000ce20: 6164 6457 6964 6765 7428 7365 6c66 2e74  addWidget(self.t
-0000ce30: 6162 6c65 5669 6577 5f72 6573 756c 7473  ableView_results
-0000ce40: 5f63 6f72 7265 6c61 7469 6f6e 5f6d 6174  _correlation_mat
-0000ce50: 7269 7829 0a20 2020 2020 2020 2073 656c  rix).        sel
-0000ce60: 662e 7461 6257 6964 6765 745f 7265 7375  f.tabWidget_resu
-0000ce70: 6c74 732e 6164 6454 6162 2873 656c 662e  lts.addTab(self.
-0000ce80: 7461 625f 7265 7375 6c74 735f 636f 7272  tab_results_corr
-0000ce90: 656c 6174 696f 6e5f 6d61 7472 6978 2c20  elation_matrix, 
-0000cea0: 2222 290a 2020 2020 2020 2020 7365 6c66  "").        self
-0000ceb0: 2e74 6162 5f76 675f 7461 626c 6520 3d20  .tab_vg_table = 
-0000cec0: 5174 5769 6467 6574 732e 5157 6964 6765  QtWidgets.QWidge
-0000ced0: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
-0000cee0: 2e74 6162 5f76 675f 7461 626c 652e 7365  .tab_vg_table.se
-0000cef0: 744f 626a 6563 744e 616d 6528 2274 6162  tObjectName("tab
-0000cf00: 5f76 675f 7461 626c 6522 290a 2020 2020  _vg_table").    
-0000cf10: 2020 2020 7365 6c66 2e76 6572 7469 6361      self.vertica
-0000cf20: 6c4c 6179 6f75 745f 3333 203d 2051 7457  lLayout_33 = QtW
-0000cf30: 6964 6765 7473 2e51 5642 6f78 4c61 796f  idgets.QVBoxLayo
-0000cf40: 7574 2873 656c 662e 7461 625f 7667 5f74  ut(self.tab_vg_t
-0000cf50: 6162 6c65 290a 2020 2020 2020 2020 7365  able).        se
-0000cf60: 6c66 2e76 6572 7469 6361 6c4c 6179 6f75  lf.verticalLayou
-0000cf70: 745f 3333 2e73 6574 4f62 6a65 6374 4e61  t_33.setObjectNa
-0000cf80: 6d65 2822 7665 7274 6963 616c 4c61 796f  me("verticalLayo
-0000cf90: 7574 5f33 3322 290a 2020 2020 2020 2020  ut_33").        
-0000cfa0: 7365 6c66 2e74 6162 6c65 5669 6577 5f72  self.tableView_r
-0000cfb0: 6573 756c 7473 5f76 675f 7461 626c 6520  esults_vg_table 
-0000cfc0: 3d20 5174 5769 6467 6574 732e 5154 6162  = QtWidgets.QTab
-0000cfd0: 6c65 5669 6577 2873 656c 662e 7461 625f  leView(self.tab_
-0000cfe0: 7667 5f74 6162 6c65 290a 2020 2020 2020  vg_table).      
-0000cff0: 2020 7365 6c66 2e74 6162 6c65 5669 6577    self.tableView
-0000d000: 5f72 6573 756c 7473 5f76 675f 7461 626c  _results_vg_tabl
-0000d010: 652e 7365 744f 626a 6563 744e 616d 6528  e.setObjectName(
-0000d020: 2274 6162 6c65 5669 6577 5f72 6573 756c  "tableView_resul
-0000d030: 7473 5f76 675f 7461 626c 6522 290a 2020  ts_vg_table").  
-0000d040: 2020 2020 2020 7365 6c66 2e76 6572 7469        self.verti
-0000d050: 6361 6c4c 6179 6f75 745f 3333 2e61 6464  calLayout_33.add
-0000d060: 5769 6467 6574 2873 656c 662e 7461 626c  Widget(self.tabl
-0000d070: 6556 6965 775f 7265 7375 6c74 735f 7667  eView_results_vg
-0000d080: 5f74 6162 6c65 290a 2020 2020 2020 2020  _table).        
-0000d090: 7365 6c66 2e74 6162 5769 6467 6574 5f72  self.tabWidget_r
-0000d0a0: 6573 756c 7473 2e61 6464 5461 6228 7365  esults.addTab(se
-0000d0b0: 6c66 2e74 6162 5f76 675f 7461 626c 652c  lf.tab_vg_table,
-0000d0c0: 2022 2229 0a20 2020 2020 2020 2073 656c   "").        sel
-0000d0d0: 662e 7461 625f 7667 5f70 6c6f 7420 3d20  f.tab_vg_plot = 
-0000d0e0: 5174 5769 6467 6574 732e 5157 6964 6765  QtWidgets.QWidge
-0000d0f0: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
-0000d100: 2e74 6162 5f76 675f 706c 6f74 2e73 6574  .tab_vg_plot.set
-0000d110: 4f62 6a65 6374 4e61 6d65 2822 7461 625f  ObjectName("tab_
-0000d120: 7667 5f70 6c6f 7422 290a 2020 2020 2020  vg_plot").      
-0000d130: 2020 7365 6c66 2e76 6572 7469 6361 6c4c    self.verticalL
-0000d140: 6179 6f75 745f 3335 203d 2051 7457 6964  ayout_35 = QtWid
-0000d150: 6765 7473 2e51 5642 6f78 4c61 796f 7574  gets.QVBoxLayout
-0000d160: 2873 656c 662e 7461 625f 7667 5f70 6c6f  (self.tab_vg_plo
-0000d170: 7429 0a20 2020 2020 2020 2073 656c 662e  t).        self.
-0000d180: 7665 7274 6963 616c 4c61 796f 7574 5f33  verticalLayout_3
-0000d190: 352e 7365 744f 626a 6563 744e 616d 6528  5.setObjectName(
-0000d1a0: 2276 6572 7469 6361 6c4c 6179 6f75 745f  "verticalLayout_
-0000d1b0: 3335 2229 0a20 2020 2020 2020 2073 656c  35").        sel
-0000d1c0: 662e 6772 6170 6869 6373 4c61 796f 7574  f.graphicsLayout
-0000d1d0: 5769 6467 6574 5f72 6573 756c 7473 5f76  Widget_results_v
-0000d1e0: 675f 706c 6f74 203d 2047 7261 7068 6963  g_plot = Graphic
-0000d1f0: 734c 6179 6f75 7457 6964 6765 7428 7365  sLayoutWidget(se
-0000d200: 6c66 2e74 6162 5f76 675f 706c 6f74 290a  lf.tab_vg_plot).
-0000d210: 2020 2020 2020 2020 7365 6c66 2e67 7261          self.gra
-0000d220: 7068 6963 734c 6179 6f75 7457 6964 6765  phicsLayoutWidge
-0000d230: 745f 7265 7375 6c74 735f 7667 5f70 6c6f  t_results_vg_plo
-0000d240: 742e 7365 744f 626a 6563 744e 616d 6528  t.setObjectName(
-0000d250: 2267 7261 7068 6963 734c 6179 6f75 7457  "graphicsLayoutW
-0000d260: 6964 6765 745f 7265 7375 6c74 735f 7667  idget_results_vg
-0000d270: 5f70 6c6f 7422 290a 2020 2020 2020 2020  _plot").        
-0000d280: 7365 6c66 2e76 6572 7469 6361 6c4c 6179  self.verticalLay
-0000d290: 6f75 745f 3335 2e61 6464 5769 6467 6574  out_35.addWidget
-0000d2a0: 2873 656c 662e 6772 6170 6869 6373 4c61  (self.graphicsLa
-0000d2b0: 796f 7574 5769 6467 6574 5f72 6573 756c  youtWidget_resul
-0000d2c0: 7473 5f76 675f 706c 6f74 290a 2020 2020  ts_vg_plot).    
-0000d2d0: 2020 2020 7365 6c66 2e67 726f 7570 426f      self.groupBo
-0000d2e0: 785f 7265 7375 6c74 735f 7667 5f70 6c6f  x_results_vg_plo
-0000d2f0: 745f 7365 7474 696e 6773 203d 2051 7457  t_settings = QtW
-0000d300: 6964 6765 7473 2e51 4772 6f75 7042 6f78  idgets.QGroupBox
-0000d310: 2873 656c 662e 7461 625f 7667 5f70 6c6f  (self.tab_vg_plo
-0000d320: 7429 0a20 2020 2020 2020 2073 656c 662e  t).        self.
-0000d330: 6772 6f75 7042 6f78 5f72 6573 756c 7473  groupBox_results
-0000d340: 5f76 675f 706c 6f74 5f73 6574 7469 6e67  _vg_plot_setting
-0000d350: 732e 7365 744f 626a 6563 744e 616d 6528  s.setObjectName(
-0000d360: 2267 726f 7570 426f 785f 7265 7375 6c74  "groupBox_result
-0000d370: 735f 7667 5f70 6c6f 745f 7365 7474 696e  s_vg_plot_settin
-0000d380: 6773 2229 0a20 2020 2020 2020 2073 656c  gs").        sel
-0000d390: 662e 7665 7274 6963 616c 4c61 796f 7574  f.verticalLayout
-0000d3a0: 5f33 3420 3d20 5174 5769 6467 6574 732e  _34 = QtWidgets.
-0000d3b0: 5156 426f 784c 6179 6f75 7428 7365 6c66  QVBoxLayout(self
-0000d3c0: 2e67 726f 7570 426f 785f 7265 7375 6c74  .groupBox_result
-0000d3d0: 735f 7667 5f70 6c6f 745f 7365 7474 696e  s_vg_plot_settin
-0000d3e0: 6773 290a 2020 2020 2020 2020 7365 6c66  gs).        self
-0000d3f0: 2e76 6572 7469 6361 6c4c 6179 6f75 745f  .verticalLayout_
-0000d400: 3334 2e73 6574 4f62 6a65 6374 4e61 6d65  34.setObjectName
-0000d410: 2822 7665 7274 6963 616c 4c61 796f 7574  ("verticalLayout
-0000d420: 5f33 3422 290a 2020 2020 2020 2020 7365  _34").        se
-0000d430: 6c66 2e63 6865 636b 426f 785f 7265 7375  lf.checkBox_resu
-0000d440: 6c74 735f 7667 5f70 6c6f 745f 7368 6f77  lts_vg_plot_show
-0000d450: 5f72 6573 6964 7561 6c73 203d 2051 7457  _residuals = QtW
-0000d460: 6964 6765 7473 2e51 4368 6563 6b42 6f78  idgets.QCheckBox
-0000d470: 2873 656c 662e 6772 6f75 7042 6f78 5f72  (self.groupBox_r
-0000d480: 6573 756c 7473 5f76 675f 706c 6f74 5f73  esults_vg_plot_s
-0000d490: 6574 7469 6e67 7329 0a20 2020 2020 2020  ettings).       
-0000d4a0: 2073 656c 662e 6368 6563 6b42 6f78 5f72   self.checkBox_r
-0000d4b0: 6573 756c 7473 5f76 675f 706c 6f74 5f73  esults_vg_plot_s
-0000d4c0: 686f 775f 7265 7369 6475 616c 732e 7365  how_residuals.se
-0000d4d0: 7443 6865 636b 6564 2854 7275 6529 0a20  tChecked(True). 
-0000d4e0: 2020 2020 2020 2073 656c 662e 6368 6563         self.chec
-0000d4f0: 6b42 6f78 5f72 6573 756c 7473 5f76 675f  kBox_results_vg_
-0000d500: 706c 6f74 5f73 686f 775f 7265 7369 6475  plot_show_residu
-0000d510: 616c 732e 7365 744f 626a 6563 744e 616d  als.setObjectNam
-0000d520: 6528 2263 6865 636b 426f 785f 7265 7375  e("checkBox_resu
-0000d530: 6c74 735f 7667 5f70 6c6f 745f 7368 6f77  lts_vg_plot_show
-0000d540: 5f72 6573 6964 7561 6c73 2229 0a20 2020  _residuals").   
-0000d550: 2020 2020 2073 656c 662e 7665 7274 6963       self.vertic
-0000d560: 616c 4c61 796f 7574 5f33 342e 6164 6457  alLayout_34.addW
-0000d570: 6964 6765 7428 7365 6c66 2e63 6865 636b  idget(self.check
-0000d580: 426f 785f 7265 7375 6c74 735f 7667 5f70  Box_results_vg_p
-0000d590: 6c6f 745f 7368 6f77 5f72 6573 6964 7561  lot_show_residua
-0000d5a0: 6c73 290a 2020 2020 2020 2020 7365 6c66  ls).        self
-0000d5b0: 2e72 6164 696f 4275 7474 6f6e 5f72 6573  .radioButton_res
-0000d5c0: 756c 7473 5f76 675f 706c 6f74 5f64 6574  ults_vg_plot_det
-0000d5d0: 6169 6c73 203d 2051 7457 6964 6765 7473  ails = QtWidgets
-0000d5e0: 2e51 5261 6469 6f42 7574 746f 6e28 7365  .QRadioButton(se
-0000d5f0: 6c66 2e67 726f 7570 426f 785f 7265 7375  lf.groupBox_resu
-0000d600: 6c74 735f 7667 5f70 6c6f 745f 7365 7474  lts_vg_plot_sett
-0000d610: 696e 6773 290a 2020 2020 2020 2020 7365  ings).        se
-0000d620: 6c66 2e72 6164 696f 4275 7474 6f6e 5f72  lf.radioButton_r
-0000d630: 6573 756c 7473 5f76 675f 706c 6f74 5f64  esults_vg_plot_d
-0000d640: 6574 6169 6c73 2e73 6574 4368 6563 6b65  etails.setChecke
-0000d650: 6428 5472 7565 290a 2020 2020 2020 2020  d(True).        
-0000d660: 7365 6c66 2e72 6164 696f 4275 7474 6f6e  self.radioButton
-0000d670: 5f72 6573 756c 7473 5f76 675f 706c 6f74  _results_vg_plot
-0000d680: 5f64 6574 6169 6c73 2e73 6574 4f62 6a65  _details.setObje
-0000d690: 6374 4e61 6d65 2822 7261 6469 6f42 7574  ctName("radioBut
-0000d6a0: 746f 6e5f 7265 7375 6c74 735f 7667 5f70  ton_results_vg_p
-0000d6b0: 6c6f 745f 6465 7461 696c 7322 290a 2020  lot_details").  
-0000d6c0: 2020 2020 2020 7365 6c66 2e62 7574 746f        self.butto
-0000d6d0: 6e47 726f 7570 5f72 6573 756c 7473 5f76  nGroup_results_v
-0000d6e0: 675f 706c 6f74 5f74 7970 655f 7365 6c65  g_plot_type_sele
-0000d6f0: 6374 696f 6e20 3d20 5174 5769 6467 6574  ction = QtWidget
-0000d700: 732e 5142 7574 746f 6e47 726f 7570 284d  s.QButtonGroup(M
-0000d710: 6169 6e57 696e 646f 7729 0a20 2020 2020  ainWindow).     
-0000d720: 2020 2073 656c 662e 6275 7474 6f6e 4772     self.buttonGr
-0000d730: 6f75 705f 7265 7375 6c74 735f 7667 5f70  oup_results_vg_p
-0000d740: 6c6f 745f 7479 7065 5f73 656c 6563 7469  lot_type_selecti
-0000d750: 6f6e 2e73 6574 4f62 6a65 6374 4e61 6d65  on.setObjectName
-0000d760: 2822 6275 7474 6f6e 4772 6f75 705f 7265  ("buttonGroup_re
-0000d770: 7375 6c74 735f 7667 5f70 6c6f 745f 7479  sults_vg_plot_ty
-0000d780: 7065 5f73 656c 6563 7469 6f6e 2229 0a20  pe_selection"). 
-0000d790: 2020 2020 2020 2073 656c 662e 6275 7474         self.butt
-0000d7a0: 6f6e 4772 6f75 705f 7265 7375 6c74 735f  onGroup_results_
-0000d7b0: 7667 5f70 6c6f 745f 7479 7065 5f73 656c  vg_plot_type_sel
-0000d7c0: 6563 7469 6f6e 2e61 6464 4275 7474 6f6e  ection.addButton
-0000d7d0: 2873 656c 662e 7261 6469 6f42 7574 746f  (self.radioButto
-0000d7e0: 6e5f 7265 7375 6c74 735f 7667 5f70 6c6f  n_results_vg_plo
-0000d7f0: 745f 6465 7461 696c 7329 0a20 2020 2020  t_details).     
-0000d800: 2020 2073 656c 662e 7665 7274 6963 616c     self.vertical
-0000d810: 4c61 796f 7574 5f33 342e 6164 6457 6964  Layout_34.addWid
-0000d820: 6765 7428 7365 6c66 2e72 6164 696f 4275  get(self.radioBu
-0000d830: 7474 6f6e 5f72 6573 756c 7473 5f76 675f  tton_results_vg_
-0000d840: 706c 6f74 5f64 6574 6169 6c73 290a 2020  plot_details).  
-0000d850: 2020 2020 2020 7365 6c66 2e72 6164 696f        self.radio
-0000d860: 4275 7474 6f6e 5f72 6573 756c 7473 5f76  Button_results_v
-0000d870: 675f 706c 6f74 5f66 756c 6c5f 706f 6c79  g_plot_full_poly
-0000d880: 6e6f 6d69 616c 203d 2051 7457 6964 6765  nomial = QtWidge
-0000d890: 7473 2e51 5261 6469 6f42 7574 746f 6e28  ts.QRadioButton(
-0000d8a0: 7365 6c66 2e67 726f 7570 426f 785f 7265  self.groupBox_re
-0000d8b0: 7375 6c74 735f 7667 5f70 6c6f 745f 7365  sults_vg_plot_se
-0000d8c0: 7474 696e 6773 290a 2020 2020 2020 2020  ttings).        
-0000d8d0: 7365 6c66 2e72 6164 696f 4275 7474 6f6e  self.radioButton
-0000d8e0: 5f72 6573 756c 7473 5f76 675f 706c 6f74  _results_vg_plot
-0000d8f0: 5f66 756c 6c5f 706f 6c79 6e6f 6d69 616c  _full_polynomial
-0000d900: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
-0000d910: 7261 6469 6f42 7574 746f 6e5f 7265 7375  radioButton_resu
-0000d920: 6c74 735f 7667 5f70 6c6f 745f 6675 6c6c  lts_vg_plot_full
-0000d930: 5f70 6f6c 796e 6f6d 6961 6c22 290a 2020  _polynomial").  
-0000d940: 2020 2020 2020 7365 6c66 2e62 7574 746f        self.butto
-0000d950: 6e47 726f 7570 5f72 6573 756c 7473 5f76  nGroup_results_v
-0000d960: 675f 706c 6f74 5f74 7970 655f 7365 6c65  g_plot_type_sele
-0000d970: 6374 696f 6e2e 6164 6442 7574 746f 6e28  ction.addButton(
-0000d980: 7365 6c66 2e72 6164 696f 4275 7474 6f6e  self.radioButton
-0000d990: 5f72 6573 756c 7473 5f76 675f 706c 6f74  _results_vg_plot
-0000d9a0: 5f66 756c 6c5f 706f 6c79 6e6f 6d69 616c  _full_polynomial
-0000d9b0: 290a 2020 2020 2020 2020 7365 6c66 2e76  ).        self.v
-0000d9c0: 6572 7469 6361 6c4c 6179 6f75 745f 3334  erticalLayout_34
-0000d9d0: 2e61 6464 5769 6467 6574 2873 656c 662e  .addWidget(self.
-0000d9e0: 7261 6469 6f42 7574 746f 6e5f 7265 7375  radioButton_resu
-0000d9f0: 6c74 735f 7667 5f70 6c6f 745f 6675 6c6c  lts_vg_plot_full
-0000da00: 5f70 6f6c 796e 6f6d 6961 6c29 0a20 2020  _polynomial).   
-0000da10: 2020 2020 2073 656c 662e 7665 7274 6963       self.vertic
-0000da20: 616c 4c61 796f 7574 5f33 352e 6164 6457  alLayout_35.addW
-0000da30: 6964 6765 7428 7365 6c66 2e67 726f 7570  idget(self.group
-0000da40: 426f 785f 7265 7375 6c74 735f 7667 5f70  Box_results_vg_p
-0000da50: 6c6f 745f 7365 7474 696e 6773 290a 2020  lot_settings).  
-0000da60: 2020 2020 2020 7365 6c66 2e74 6162 5769        self.tabWi
-0000da70: 6467 6574 5f72 6573 756c 7473 2e61 6464  dget_results.add
-0000da80: 5461 6228 7365 6c66 2e74 6162 5f76 675f  Tab(self.tab_vg_
-0000da90: 706c 6f74 2c20 2222 290a 2020 2020 2020  plot, "").      
-0000daa0: 2020 7365 6c66 2e76 6572 7469 6361 6c4c    self.verticalL
-0000dab0: 6179 6f75 745f 3134 2e61 6464 5769 6467  ayout_14.addWidg
-0000dac0: 6574 2873 656c 662e 7370 6c69 7474 6572  et(self.splitter
-0000dad0: 5f72 6573 756c 7473 290a 2020 2020 2020  _results).      
-0000dae0: 2020 7365 6c66 2e74 6162 5769 6467 6574    self.tabWidget
-0000daf0: 5f4d 6169 6e2e 6164 6454 6162 2873 656c  _Main.addTab(sel
-0000db00: 662e 7461 625f 6d61 696e 5f72 6573 756c  f.tab_main_resul
-0000db10: 7473 2c20 2222 290a 2020 2020 2020 2020  ts, "").        
-0000db20: 7365 6c66 2e68 6f72 697a 6f6e 7461 6c4c  self.horizontalL
-0000db30: 6179 6f75 745f 352e 6164 6457 6964 6765  ayout_5.addWidge
-0000db40: 7428 7365 6c66 2e74 6162 5769 6467 6574  t(self.tabWidget
-0000db50: 5f4d 6169 6e29 0a20 2020 2020 2020 204d  _Main).        M
-0000db60: 6169 6e57 696e 646f 772e 7365 7443 656e  ainWindow.setCen
-0000db70: 7472 616c 5769 6467 6574 2873 656c 662e  tralWidget(self.
-0000db80: 6365 6e74 7261 6c77 6964 6765 7429 0a20  centralwidget). 
-0000db90: 2020 2020 2020 2073 656c 662e 6d65 6e75         self.menu
-0000dba0: 6261 7220 3d20 5174 5769 6467 6574 732e  bar = QtWidgets.
-0000dbb0: 514d 656e 7542 6172 284d 6169 6e57 696e  QMenuBar(MainWin
-0000dbc0: 646f 7729 0a20 2020 2020 2020 2073 656c  dow).        sel
-0000dbd0: 662e 6d65 6e75 6261 722e 7365 7447 656f  f.menubar.setGeo
-0000dbe0: 6d65 7472 7928 5174 436f 7265 2e51 5265  metry(QtCore.QRe
-0000dbf0: 6374 2830 2c20 302c 2031 3333 372c 2032  ct(0, 0, 1337, 2
-0000dc00: 3229 290a 2020 2020 2020 2020 7365 6c66  2)).        self
-0000dc10: 2e6d 656e 7562 6172 2e73 6574 4f62 6a65  .menubar.setObje
-0000dc20: 6374 4e61 6d65 2822 6d65 6e75 6261 7222  ctName("menubar"
-0000dc30: 290a 2020 2020 2020 2020 7365 6c66 2e6d  ).        self.m
-0000dc40: 656e 755f 4669 6c65 203d 2051 7457 6964  enu_File = QtWid
-0000dc50: 6765 7473 2e51 4d65 6e75 2873 656c 662e  gets.QMenu(self.
-0000dc60: 6d65 6e75 6261 7229 0a20 2020 2020 2020  menubar).       
-0000dc70: 2073 656c 662e 6d65 6e75 5f46 696c 652e   self.menu_File.
-0000dc80: 7365 744f 626a 6563 744e 616d 6528 226d  setObjectName("m
-0000dc90: 656e 755f 4669 6c65 2229 0a20 2020 2020  enu_File").     
-0000dca0: 2020 2073 656c 662e 6d65 6e75 4164 645f     self.menuAdd_
-0000dcb0: 5375 7276 6579 203d 2051 7457 6964 6765  Survey = QtWidge
-0000dcc0: 7473 2e51 4d65 6e75 2873 656c 662e 6d65  ts.QMenu(self.me
-0000dcd0: 6e75 5f46 696c 6529 0a20 2020 2020 2020  nu_File).       
-0000dce0: 2073 656c 662e 6d65 6e75 4164 645f 5375   self.menuAdd_Su
-0000dcf0: 7276 6579 2e73 6574 456e 6162 6c65 6428  rvey.setEnabled(
-0000dd00: 4661 6c73 6529 0a20 2020 2020 2020 2073  False).        s
-0000dd10: 656c 662e 6d65 6e75 4164 645f 5375 7276  elf.menuAdd_Surv
-0000dd20: 6579 2e73 6574 4f62 6a65 6374 4e61 6d65  ey.setObjectName
-0000dd30: 2822 6d65 6e75 4164 645f 5375 7276 6579  ("menuAdd_Survey
-0000dd40: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-0000dd50: 6d65 6e75 5f41 6464 5f53 7461 7469 6f6e  menu_Add_Station
-0000dd60: 7320 3d20 5174 5769 6467 6574 732e 514d  s = QtWidgets.QM
-0000dd70: 656e 7528 7365 6c66 2e6d 656e 755f 4669  enu(self.menu_Fi
-0000dd80: 6c65 290a 2020 2020 2020 2020 7365 6c66  le).        self
-0000dd90: 2e6d 656e 755f 4164 645f 5374 6174 696f  .menu_Add_Statio
-0000dda0: 6e73 2e73 6574 456e 6162 6c65 6428 4661  ns.setEnabled(Fa
-0000ddb0: 6c73 6529 0a20 2020 2020 2020 2073 656c  lse).        sel
-0000ddc0: 662e 6d65 6e75 5f41 6464 5f53 7461 7469  f.menu_Add_Stati
-0000ddd0: 6f6e 732e 7365 744f 626a 6563 744e 616d  ons.setObjectNam
-0000dde0: 6528 226d 656e 755f 4164 645f 5374 6174  e("menu_Add_Stat
-0000ddf0: 696f 6e73 2229 0a20 2020 2020 2020 2073  ions").        s
-0000de00: 656c 662e 6d65 6e75 5f41 6464 5f47 7261  elf.menu_Add_Gra
-0000de10: 7669 6d65 7465 7273 203d 2051 7457 6964  vimeters = QtWid
-0000de20: 6765 7473 2e51 4d65 6e75 2873 656c 662e  gets.QMenu(self.
-0000de30: 6d65 6e75 5f46 696c 6529 0a20 2020 2020  menu_File).     
-0000de40: 2020 2073 656c 662e 6d65 6e75 5f41 6464     self.menu_Add
-0000de50: 5f47 7261 7669 6d65 7465 7273 2e73 6574  _Gravimeters.set
-0000de60: 456e 6162 6c65 6428 4661 6c73 6529 0a20  Enabled(False). 
-0000de70: 2020 2020 2020 2073 656c 662e 6d65 6e75         self.menu
-0000de80: 5f41 6464 5f47 7261 7669 6d65 7465 7273  _Add_Gravimeters
-0000de90: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
-0000dea0: 6d65 6e75 5f41 6464 5f47 7261 7669 6d65  menu_Add_Gravime
-0000deb0: 7465 7273 2229 0a20 2020 2020 2020 2073  ters").        s
-0000dec0: 656c 662e 6d65 6e75 5f4f 6273 6572 7661  elf.menu_Observa
-0000ded0: 7469 6f6e 7320 3d20 5174 5769 6467 6574  tions = QtWidget
-0000dee0: 732e 514d 656e 7528 7365 6c66 2e6d 656e  s.QMenu(self.men
-0000def0: 7562 6172 290a 2020 2020 2020 2020 7365  ubar).        se
-0000df00: 6c66 2e6d 656e 755f 4f62 7365 7276 6174  lf.menu_Observat
-0000df10: 696f 6e73 2e73 6574 456e 6162 6c65 6428  ions.setEnabled(
-0000df20: 4661 6c73 6529 0a20 2020 2020 2020 2073  False).        s
-0000df30: 656c 662e 6d65 6e75 5f4f 6273 6572 7661  elf.menu_Observa
-0000df40: 7469 6f6e 732e 7365 7454 6561 724f 6666  tions.setTearOff
-0000df50: 456e 6162 6c65 6428 4661 6c73 6529 0a20  Enabled(False). 
-0000df60: 2020 2020 2020 2073 656c 662e 6d65 6e75         self.menu
-0000df70: 5f4f 6273 6572 7661 7469 6f6e 732e 7365  _Observations.se
-0000df80: 744f 626a 6563 744e 616d 6528 226d 656e  tObjectName("men
-0000df90: 755f 4f62 7365 7276 6174 696f 6e73 2229  u_Observations")
-0000dfa0: 0a20 2020 2020 2020 2073 656c 662e 6d65  .        self.me
-0000dfb0: 6e75 4573 7469 6d61 7469 6f6e 5f73 6574  nuEstimation_set
-0000dfc0: 7469 6e67 7320 3d20 5174 5769 6467 6574  tings = QtWidget
-0000dfd0: 732e 514d 656e 7528 7365 6c66 2e6d 656e  s.QMenu(self.men
-0000dfe0: 7562 6172 290a 2020 2020 2020 2020 7365  ubar).        se
-0000dff0: 6c66 2e6d 656e 7545 7374 696d 6174 696f  lf.menuEstimatio
-0000e000: 6e5f 7365 7474 696e 6773 2e73 6574 456e  n_settings.setEn
-0000e010: 6162 6c65 6428 5472 7565 290a 2020 2020  abled(True).    
-0000e020: 2020 2020 7365 6c66 2e6d 656e 7545 7374      self.menuEst
-0000e030: 696d 6174 696f 6e5f 7365 7474 696e 6773  imation_settings
-0000e040: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
-0000e050: 6d65 6e75 4573 7469 6d61 7469 6f6e 5f73  menuEstimation_s
-0000e060: 6574 7469 6e67 7322 290a 2020 2020 2020  ettings").      
-0000e070: 2020 7365 6c66 2e6d 656e 7548 656c 7020    self.menuHelp 
-0000e080: 3d20 5174 5769 6467 6574 732e 514d 656e  = QtWidgets.QMen
-0000e090: 7528 7365 6c66 2e6d 656e 7562 6172 290a  u(self.menubar).
-0000e0a0: 2020 2020 2020 2020 7365 6c66 2e6d 656e          self.men
-0000e0b0: 7548 656c 702e 7365 744f 626a 6563 744e  uHelp.setObjectN
-0000e0c0: 616d 6528 226d 656e 7548 656c 7022 290a  ame("menuHelp").
-0000e0d0: 2020 2020 2020 2020 7365 6c66 2e6d 656e          self.men
-0000e0e0: 7543 6f72 7265 6374 696f 6e73 203d 2051  uCorrections = Q
-0000e0f0: 7457 6964 6765 7473 2e51 4d65 6e75 2873  tWidgets.QMenu(s
-0000e100: 656c 662e 6d65 6e75 6261 7229 0a20 2020  elf.menubar).   
-0000e110: 2020 2020 2073 656c 662e 6d65 6e75 436f       self.menuCo
-0000e120: 7272 6563 7469 6f6e 732e 7365 744f 626a  rrections.setObj
-0000e130: 6563 744e 616d 6528 226d 656e 7543 6f72  ectName("menuCor
-0000e140: 7265 6374 696f 6e73 2229 0a20 2020 2020  rections").     
-0000e150: 2020 204d 6169 6e57 696e 646f 772e 7365     MainWindow.se
-0000e160: 744d 656e 7542 6172 2873 656c 662e 6d65  tMenuBar(self.me
-0000e170: 6e75 6261 7229 0a20 2020 2020 2020 2073  nubar).        s
-0000e180: 656c 662e 7374 6174 7573 6261 7220 3d20  elf.statusbar = 
-0000e190: 5174 5769 6467 6574 732e 5153 7461 7475  QtWidgets.QStatu
-0000e1a0: 7342 6172 284d 6169 6e57 696e 646f 7729  sBar(MainWindow)
-0000e1b0: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
-0000e1c0: 6174 7573 6261 722e 7365 7449 6e70 7574  atusbar.setInput
-0000e1d0: 4d65 7468 6f64 4869 6e74 7328 5174 436f  MethodHints(QtCo
-0000e1e0: 7265 2e51 742e 496d 684e 6f6e 6529 0a20  re.Qt.ImhNone). 
-0000e1f0: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-0000e200: 7573 6261 722e 7365 744f 626a 6563 744e  usbar.setObjectN
-0000e210: 616d 6528 2273 7461 7475 7362 6172 2229  ame("statusbar")
-0000e220: 0a20 2020 2020 2020 204d 6169 6e57 696e  .        MainWin
-0000e230: 646f 772e 7365 7453 7461 7475 7342 6172  dow.setStatusBar
-0000e240: 2873 656c 662e 7374 6174 7573 6261 7229  (self.statusbar)
-0000e250: 0a20 2020 2020 2020 2073 656c 662e 6163  .        self.ac
-0000e260: 7469 6f6e 5f4e 6577 5f43 616d 7061 6967  tion_New_Campaig
-0000e270: 6e20 3d20 5174 5769 6467 6574 732e 5141  n = QtWidgets.QA
-0000e280: 6374 696f 6e28 4d61 696e 5769 6e64 6f77  ction(MainWindow
-0000e290: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-0000e2a0: 6374 696f 6e5f 4e65 775f 4361 6d70 6169  ction_New_Campai
-0000e2b0: 676e 2e73 6574 4f62 6a65 6374 4e61 6d65  gn.setObjectName
-0000e2c0: 2822 6163 7469 6f6e 5f4e 6577 5f43 616d  ("action_New_Cam
-0000e2d0: 7061 6967 6e22 290a 2020 2020 2020 2020  paign").        
-0000e2e0: 7365 6c66 2e61 6374 696f 6e5f 5361 7665  self.action_Save
-0000e2f0: 5f43 616d 7061 6967 6e20 3d20 5174 5769  _Campaign = QtWi
-0000e300: 6467 6574 732e 5141 6374 696f 6e28 4d61  dgets.QAction(Ma
-0000e310: 696e 5769 6e64 6f77 290a 2020 2020 2020  inWindow).      
-0000e320: 2020 7365 6c66 2e61 6374 696f 6e5f 5361    self.action_Sa
-0000e330: 7665 5f43 616d 7061 6967 6e2e 7365 7445  ve_Campaign.setE
-0000e340: 6e61 626c 6564 2846 616c 7365 290a 2020  nabled(False).  
-0000e350: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
-0000e360: 6e5f 5361 7665 5f43 616d 7061 6967 6e2e  n_Save_Campaign.
-0000e370: 7365 744f 626a 6563 744e 616d 6528 2261  setObjectName("a
-0000e380: 6374 696f 6e5f 5361 7665 5f43 616d 7061  ction_Save_Campa
-0000e390: 6967 6e22 290a 2020 2020 2020 2020 7365  ign").        se
-0000e3a0: 6c66 2e61 6374 696f 6e5f 4c6f 6164 5f43  lf.action_Load_C
-0000e3b0: 616d 7061 6967 6e20 3d20 5174 5769 6467  ampaign = QtWidg
-0000e3c0: 6574 732e 5141 6374 696f 6e28 4d61 696e  ets.QAction(Main
-0000e3d0: 5769 6e64 6f77 290a 2020 2020 2020 2020  Window).        
-0000e3e0: 7365 6c66 2e61 6374 696f 6e5f 4c6f 6164  self.action_Load
-0000e3f0: 5f43 616d 7061 6967 6e2e 7365 7445 6e61  _Campaign.setEna
-0000e400: 626c 6564 2854 7275 6529 0a20 2020 2020  bled(True).     
-0000e410: 2020 2073 656c 662e 6163 7469 6f6e 5f4c     self.action_L
-0000e420: 6f61 645f 4361 6d70 6169 676e 2e73 6574  oad_Campaign.set
-0000e430: 4f62 6a65 6374 4e61 6d65 2822 6163 7469  ObjectName("acti
-0000e440: 6f6e 5f4c 6f61 645f 4361 6d70 6169 676e  on_Load_Campaign
-0000e450: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-0000e460: 6163 7469 6f6e 5f41 6464 5f53 7461 7469  action_Add_Stati
-0000e470: 6f6e 7320 3d20 5174 5769 6467 6574 732e  ons = QtWidgets.
-0000e480: 5141 6374 696f 6e28 4d61 696e 5769 6e64  QAction(MainWind
-0000e490: 6f77 290a 2020 2020 2020 2020 7365 6c66  ow).        self
-0000e4a0: 2e61 6374 696f 6e5f 4164 645f 5374 6174  .action_Add_Stat
-0000e4b0: 696f 6e73 2e73 6574 456e 6162 6c65 6428  ions.setEnabled(
-0000e4c0: 4661 6c73 6529 0a20 2020 2020 2020 2073  False).        s
-0000e4d0: 656c 662e 6163 7469 6f6e 5f41 6464 5f53  elf.action_Add_S
-0000e4e0: 7461 7469 6f6e 732e 7365 744f 626a 6563  tations.setObjec
-0000e4f0: 744e 616d 6528 2261 6374 696f 6e5f 4164  tName("action_Ad
-0000e500: 645f 5374 6174 696f 6e73 2229 0a20 2020  d_Stations").   
-0000e510: 2020 2020 2073 656c 662e 6163 7469 6f6e       self.action
-0000e520: 5f45 7869 7420 3d20 5174 5769 6467 6574  _Exit = QtWidget
-0000e530: 732e 5141 6374 696f 6e28 4d61 696e 5769  s.QAction(MainWi
-0000e540: 6e64 6f77 290a 2020 2020 2020 2020 7365  ndow).        se
-0000e550: 6c66 2e61 6374 696f 6e5f 4578 6974 2e73  lf.action_Exit.s
-0000e560: 6574 4f62 6a65 6374 4e61 6d65 2822 6163  etObjectName("ac
-0000e570: 7469 6f6e 5f45 7869 7422 290a 2020 2020  tion_Exit").    
-0000e580: 2020 2020 7365 6c66 2e61 6374 696f 6e5f      self.action_
-0000e590: 4564 6974 5f4f 6273 6572 7661 7469 6f6e  Edit_Observation
-0000e5a0: 7320 3d20 5174 5769 6467 6574 732e 5141  s = QtWidgets.QA
-0000e5b0: 6374 696f 6e28 4d61 696e 5769 6e64 6f77  ction(MainWindow
-0000e5c0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-0000e5d0: 6374 696f 6e5f 4564 6974 5f4f 6273 6572  ction_Edit_Obser
-0000e5e0: 7661 7469 6f6e 732e 7365 7445 6e61 626c  vations.setEnabl
-0000e5f0: 6564 2854 7275 6529 0a20 2020 2020 2020  ed(True).       
-0000e600: 2073 656c 662e 6163 7469 6f6e 5f45 6469   self.action_Edi
-0000e610: 745f 4f62 7365 7276 6174 696f 6e73 2e73  t_Observations.s
-0000e620: 6574 4f62 6a65 6374 4e61 6d65 2822 6163  etObjectName("ac
-0000e630: 7469 6f6e 5f45 6469 745f 4f62 7365 7276  tion_Edit_Observ
-0000e640: 6174 696f 6e73 2229 0a20 2020 2020 2020  ations").       
-0000e650: 2073 656c 662e 6163 7469 6f6e 5265 7369   self.actionResi
-0000e660: 6475 616c 7320 3d20 5174 5769 6467 6574  duals = QtWidget
-0000e670: 732e 5141 6374 696f 6e28 4d61 696e 5769  s.QAction(MainWi
-0000e680: 6e64 6f77 290a 2020 2020 2020 2020 7365  ndow).        se
-0000e690: 6c66 2e61 6374 696f 6e52 6573 6964 7561  lf.actionResidua
-0000e6a0: 6c73 2e73 6574 4f62 6a65 6374 4e61 6d65  ls.setObjectName
-0000e6b0: 2822 6163 7469 6f6e 5265 7369 6475 616c  ("actionResidual
-0000e6c0: 7322 290a 2020 2020 2020 2020 7365 6c66  s").        self
-0000e6d0: 2e61 6374 696f 6e45 7374 696d 6174 6573  .actionEstimates
-0000e6e0: 203d 2051 7457 6964 6765 7473 2e51 4163   = QtWidgets.QAc
-0000e6f0: 7469 6f6e 284d 6169 6e57 696e 646f 7729  tion(MainWindow)
-0000e700: 0a20 2020 2020 2020 2073 656c 662e 6163  .        self.ac
-0000e710: 7469 6f6e 4573 7469 6d61 7465 732e 7365  tionEstimates.se
-0000e720: 744f 626a 6563 744e 616d 6528 2261 6374  tObjectName("act
-0000e730: 696f 6e45 7374 696d 6174 6573 2229 0a20  ionEstimates"). 
-0000e740: 2020 2020 2020 2073 656c 662e 6163 7469         self.acti
-0000e750: 6f6e 5f43 6f72 7265 6374 696f 6e73 203d  on_Corrections =
-0000e760: 2051 7457 6964 6765 7473 2e51 4163 7469   QtWidgets.QActi
-0000e770: 6f6e 284d 6169 6e57 696e 646f 7729 0a20  on(MainWindow). 
-0000e780: 2020 2020 2020 2073 656c 662e 6163 7469         self.acti
-0000e790: 6f6e 5f43 6f72 7265 6374 696f 6e73 2e73  on_Corrections.s
-0000e7a0: 6574 456e 6162 6c65 6428 5472 7565 290a  etEnabled(True).
-0000e7b0: 2020 2020 2020 2020 7365 6c66 2e61 6374          self.act
-0000e7c0: 696f 6e5f 436f 7272 6563 7469 6f6e 732e  ion_Corrections.
-0000e7d0: 7365 744f 626a 6563 744e 616d 6528 2261  setObjectName("a
-0000e7e0: 6374 696f 6e5f 436f 7272 6563 7469 6f6e  ction_Correction
-0000e7f0: 7322 290a 2020 2020 2020 2020 7365 6c66  s").        self
-0000e800: 2e61 6374 696f 6e53 686f 775f 5374 6174  .actionShow_Stat
-0000e810: 696f 6e73 203d 2051 7457 6964 6765 7473  ions = QtWidgets
-0000e820: 2e51 4163 7469 6f6e 284d 6169 6e57 696e  .QAction(MainWin
-0000e830: 646f 7729 0a20 2020 2020 2020 2073 656c  dow).        sel
-0000e840: 662e 6163 7469 6f6e 5368 6f77 5f53 7461  f.actionShow_Sta
-0000e850: 7469 6f6e 732e 7365 744f 626a 6563 744e  tions.setObjectN
-0000e860: 616d 6528 2261 6374 696f 6e53 686f 775f  ame("actionShow_
-0000e870: 5374 6174 696f 6e73 2229 0a20 2020 2020  Stations").     
-0000e880: 2020 2073 656c 662e 6163 7469 6f6e 5f66     self.action_f
-0000e890: 726f 6d5f 4347 355f 6f62 7365 7276 6174  rom_CG5_observat
-0000e8a0: 696f 6e5f 6669 6c65 203d 2051 7457 6964  ion_file = QtWid
-0000e8b0: 6765 7473 2e51 4163 7469 6f6e 284d 6169  gets.QAction(Mai
-0000e8c0: 6e57 696e 646f 7729 0a20 2020 2020 2020  nWindow).       
-0000e8d0: 2073 656c 662e 6163 7469 6f6e 5f66 726f   self.action_fro
-0000e8e0: 6d5f 4347 355f 6f62 7365 7276 6174 696f  m_CG5_observatio
-0000e8f0: 6e5f 6669 6c65 2e73 6574 4f62 6a65 6374  n_file.setObject
-0000e900: 4e61 6d65 2822 6163 7469 6f6e 5f66 726f  Name("action_fro
-0000e910: 6d5f 4347 355f 6f62 7365 7276 6174 696f  m_CG5_observatio
-0000e920: 6e5f 6669 6c65 2229 0a20 2020 2020 2020  n_file").       
-0000e930: 2073 656c 662e 6163 7469 6f6e 5f66 726f   self.action_fro
-0000e940: 6d5f 4245 565f 6f62 7365 7276 6174 696f  m_BEV_observatio
-0000e950: 6e5f 6669 6c65 203d 2051 7457 6964 6765  n_file = QtWidge
-0000e960: 7473 2e51 4163 7469 6f6e 284d 6169 6e57  ts.QAction(MainW
-0000e970: 696e 646f 7729 0a20 2020 2020 2020 2073  indow).        s
-0000e980: 656c 662e 6163 7469 6f6e 5f66 726f 6d5f  elf.action_from_
-0000e990: 4245 565f 6f62 7365 7276 6174 696f 6e5f  BEV_observation_
-0000e9a0: 6669 6c65 2e73 6574 456e 6162 6c65 6428  file.setEnabled(
-0000e9b0: 4661 6c73 6529 0a20 2020 2020 2020 2073  False).        s
-0000e9c0: 656c 662e 6163 7469 6f6e 5f66 726f 6d5f  elf.action_from_
-0000e9d0: 4245 565f 6f62 7365 7276 6174 696f 6e5f  BEV_observation_
-0000e9e0: 6669 6c65 2e73 6574 4f62 6a65 6374 4e61  file.setObjectNa
-0000e9f0: 6d65 2822 6163 7469 6f6e 5f66 726f 6d5f  me("action_from_
-0000ea00: 4245 565f 6f62 7365 7276 6174 696f 6e5f  BEV_observation_
-0000ea10: 6669 6c65 2229 0a20 2020 2020 2020 2073  file").        s
-0000ea20: 656c 662e 6163 7469 6f6e 5f41 7574 6f73  elf.action_Autos
-0000ea30: 656c 6563 7469 6f6e 5f73 6574 7469 6e67  election_setting
-0000ea40: 7320 3d20 5174 5769 6467 6574 732e 5141  s = QtWidgets.QA
-0000ea50: 6374 696f 6e28 4d61 696e 5769 6e64 6f77  ction(MainWindow
-0000ea60: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-0000ea70: 6374 696f 6e5f 4175 746f 7365 6c65 6374  ction_Autoselect
-0000ea80: 696f 6e5f 7365 7474 696e 6773 2e73 6574  ion_settings.set
-0000ea90: 4f62 6a65 6374 4e61 6d65 2822 6163 7469  ObjectName("acti
-0000eaa0: 6f6e 5f41 7574 6f73 656c 6563 7469 6f6e  on_Autoselection
-0000eab0: 5f73 6574 7469 6e67 7322 290a 2020 2020  _settings").    
-0000eac0: 2020 2020 7365 6c66 2e61 6374 696f 6e5f      self.action_
-0000ead0: 4573 7469 6d61 7469 6f6e 5f73 6574 7469  Estimation_setti
-0000eae0: 6e67 7320 3d20 5174 5769 6467 6574 732e  ngs = QtWidgets.
-0000eaf0: 5141 6374 696f 6e28 4d61 696e 5769 6e64  QAction(MainWind
-0000eb00: 6f77 290a 2020 2020 2020 2020 7365 6c66  ow).        self
-0000eb10: 2e61 6374 696f 6e5f 4573 7469 6d61 7469  .action_Estimati
-0000eb20: 6f6e 5f73 6574 7469 6e67 732e 7365 7445  on_settings.setE
-0000eb30: 6e61 626c 6564 2854 7275 6529 0a20 2020  nabled(True).   
-0000eb40: 2020 2020 2073 656c 662e 6163 7469 6f6e       self.action
-0000eb50: 5f45 7374 696d 6174 696f 6e5f 7365 7474  _Estimation_sett
-0000eb60: 696e 6773 2e73 6574 4f62 6a65 6374 4e61  ings.setObjectNa
-0000eb70: 6d65 2822 6163 7469 6f6e 5f45 7374 696d  me("action_Estim
-0000eb80: 6174 696f 6e5f 7365 7474 696e 6773 2229  ation_settings")
-0000eb90: 0a20 2020 2020 2020 2073 656c 662e 6163  .        self.ac
-0000eba0: 7469 6f6e 4573 7469 6d61 7465 5f6c 6f6e  tionEstimate_lon
-0000ebb0: 675f 7465 726d 5f64 7269 6674 203d 2051  g_term_drift = Q
-0000ebc0: 7457 6964 6765 7473 2e51 4163 7469 6f6e  tWidgets.QAction
-0000ebd0: 284d 6169 6e57 696e 646f 7729 0a20 2020  (MainWindow).   
-0000ebe0: 2020 2020 2073 656c 662e 6163 7469 6f6e       self.action
-0000ebf0: 4573 7469 6d61 7465 5f6c 6f6e 675f 7465  Estimate_long_te
-0000ec00: 726d 5f64 7269 6674 2e73 6574 456e 6162  rm_drift.setEnab
-0000ec10: 6c65 6428 5472 7565 290a 2020 2020 2020  led(True).      
-0000ec20: 2020 7365 6c66 2e61 6374 696f 6e45 7374    self.actionEst
-0000ec30: 696d 6174 655f 6c6f 6e67 5f74 6572 6d5f  imate_long_term_
-0000ec40: 6472 6966 742e 7365 744f 626a 6563 744e  drift.setObjectN
-0000ec50: 616d 6528 2261 6374 696f 6e45 7374 696d  ame("actionEstim
-0000ec60: 6174 655f 6c6f 6e67 5f74 6572 6d5f 6472  ate_long_term_dr
-0000ec70: 6966 7422 290a 2020 2020 2020 2020 7365  ift").        se
-0000ec80: 6c66 2e61 6374 696f 6e5f 4578 706f 7274  lf.action_Export
-0000ec90: 5f52 6573 756c 7473 203d 2051 7457 6964  _Results = QtWid
-0000eca0: 6765 7473 2e51 4163 7469 6f6e 284d 6169  gets.QAction(Mai
-0000ecb0: 6e57 696e 646f 7729 0a20 2020 2020 2020  nWindow).       
-0000ecc0: 2073 656c 662e 6163 7469 6f6e 5f45 7870   self.action_Exp
-0000ecd0: 6f72 745f 5265 7375 6c74 732e 7365 7445  ort_Results.setE
-0000ece0: 6e61 626c 6564 2846 616c 7365 290a 2020  nabled(False).  
-0000ecf0: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
-0000ed00: 6e5f 4578 706f 7274 5f52 6573 756c 7473  n_Export_Results
-0000ed10: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
-0000ed20: 6163 7469 6f6e 5f45 7870 6f72 745f 5265  action_Export_Re
-0000ed30: 7375 6c74 7322 290a 2020 2020 2020 2020  sults").        
-0000ed40: 7365 6c66 2e61 6374 696f 6e5f 4368 616e  self.action_Chan
-0000ed50: 6765 5f6f 7574 7075 745f 6469 7265 6374  ge_output_direct
-0000ed60: 6f72 7920 3d20 5174 5769 6467 6574 732e  ory = QtWidgets.
-0000ed70: 5141 6374 696f 6e28 4d61 696e 5769 6e64  QAction(MainWind
-0000ed80: 6f77 290a 2020 2020 2020 2020 7365 6c66  ow).        self
-0000ed90: 2e61 6374 696f 6e5f 4368 616e 6765 5f6f  .action_Change_o
-0000eda0: 7574 7075 745f 6469 7265 6374 6f72 792e  utput_directory.
-0000edb0: 7365 7445 6e61 626c 6564 2846 616c 7365  setEnabled(False
-0000edc0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-0000edd0: 6374 696f 6e5f 4368 616e 6765 5f6f 7574  ction_Change_out
-0000ede0: 7075 745f 6469 7265 6374 6f72 792e 7365  put_directory.se
-0000edf0: 744f 626a 6563 744e 616d 6528 2261 6374  tObjectName("act
-0000ee00: 696f 6e5f 4368 616e 6765 5f6f 7574 7075  ion_Change_outpu
-0000ee10: 745f 6469 7265 6374 6f72 7922 290a 2020  t_directory").  
-0000ee20: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
-0000ee30: 6e5f 4f70 7469 6f6e 7320 3d20 5174 5769  n_Options = QtWi
-0000ee40: 6467 6574 732e 5141 6374 696f 6e28 4d61  dgets.QAction(Ma
-0000ee50: 696e 5769 6e64 6f77 290a 2020 2020 2020  inWindow).      
-0000ee60: 2020 7365 6c66 2e61 6374 696f 6e5f 4f70    self.action_Op
-0000ee70: 7469 6f6e 732e 7365 744f 626a 6563 744e  tions.setObjectN
-0000ee80: 616d 6528 2261 6374 696f 6e5f 4f70 7469  ame("action_Opti
-0000ee90: 6f6e 7322 290a 2020 2020 2020 2020 7365  ons").        se
-0000eea0: 6c66 2e61 6374 696f 6e5f 5365 7475 705f  lf.action_Setup_
-0000eeb0: 6461 7461 5f6f 7074 696f 6e73 203d 2051  data_options = Q
-0000eec0: 7457 6964 6765 7473 2e51 4163 7469 6f6e  tWidgets.QAction
-0000eed0: 284d 6169 6e57 696e 646f 7729 0a20 2020  (MainWindow).   
-0000eee0: 2020 2020 2073 656c 662e 6163 7469 6f6e       self.action
-0000eef0: 5f53 6574 7570 5f64 6174 615f 6f70 7469  _Setup_data_opti
-0000ef00: 6f6e 732e 7365 7445 6e61 626c 6564 2854  ons.setEnabled(T
-0000ef10: 7275 6529 0a20 2020 2020 2020 2073 656c  rue).        sel
-0000ef20: 662e 6163 7469 6f6e 5f53 6574 7570 5f64  f.action_Setup_d
-0000ef30: 6174 615f 6f70 7469 6f6e 732e 7365 744f  ata_options.setO
-0000ef40: 626a 6563 744e 616d 6528 2261 6374 696f  bjectName("actio
-0000ef50: 6e5f 5365 7475 705f 6461 7461 5f6f 7074  n_Setup_data_opt
-0000ef60: 696f 6e73 2229 0a20 2020 2020 2020 2073  ions").        s
-0000ef70: 656c 662e 6163 7469 6f6e 5f46 6c61 675f  elf.action_Flag_
-0000ef80: 6f62 7365 7276 6174 696f 6e73 203d 2051  observations = Q
-0000ef90: 7457 6964 6765 7473 2e51 4163 7469 6f6e  tWidgets.QAction
-0000efa0: 284d 6169 6e57 696e 646f 7729 0a20 2020  (MainWindow).   
-0000efb0: 2020 2020 2073 656c 662e 6163 7469 6f6e       self.action
-0000efc0: 5f46 6c61 675f 6f62 7365 7276 6174 696f  _Flag_observatio
-0000efd0: 6e73 2e73 6574 4f62 6a65 6374 4e61 6d65  ns.setObjectName
-0000efe0: 2822 6163 7469 6f6e 5f46 6c61 675f 6f62  ("action_Flag_ob
-0000eff0: 7365 7276 6174 696f 6e73 2229 0a20 2020  servations").   
-0000f000: 2020 2020 2073 656c 662e 6163 7469 6f6e       self.action
-0000f010: 5f43 6861 6e67 655f 4361 6d70 6169 676e  _Change_Campaign
-0000f020: 5f6e 616d 6520 3d20 5174 5769 6467 6574  _name = QtWidget
-0000f030: 732e 5141 6374 696f 6e28 4d61 696e 5769  s.QAction(MainWi
-0000f040: 6e64 6f77 290a 2020 2020 2020 2020 7365  ndow).        se
-0000f050: 6c66 2e61 6374 696f 6e5f 4368 616e 6765  lf.action_Change
-0000f060: 5f43 616d 7061 6967 6e5f 6e61 6d65 2e73  _Campaign_name.s
-0000f070: 6574 456e 6162 6c65 6428 4661 6c73 6529  etEnabled(False)
-0000f080: 0a20 2020 2020 2020 2073 656c 662e 6163  .        self.ac
-0000f090: 7469 6f6e 5f43 6861 6e67 655f 4361 6d70  tion_Change_Camp
-0000f0a0: 6169 676e 5f6e 616d 652e 7365 744f 626a  aign_name.setObj
-0000f0b0: 6563 744e 616d 6528 2261 6374 696f 6e5f  ectName("action_
-0000f0c0: 4368 616e 6765 5f43 616d 7061 6967 6e5f  Change_Campaign_
-0000f0d0: 6e61 6d65 2229 0a20 2020 2020 2020 2073  name").        s
-0000f0e0: 656c 662e 6163 7469 6f6e 5f41 626f 7574  elf.action_About
-0000f0f0: 203d 2051 7457 6964 6765 7473 2e51 4163   = QtWidgets.QAc
-0000f100: 7469 6f6e 284d 6169 6e57 696e 646f 7729  tion(MainWindow)
-0000f110: 0a20 2020 2020 2020 2073 656c 662e 6163  .        self.ac
-0000f120: 7469 6f6e 5f41 626f 7574 2e73 6574 4f62  tion_About.setOb
-0000f130: 6a65 6374 4e61 6d65 2822 6163 7469 6f6e  jectName("action
-0000f140: 5f41 626f 7574 2229 0a20 2020 2020 2020  _About").       
-0000f150: 2073 656c 662e 6163 7469 6f6e 5f4c 6963   self.action_Lic
-0000f160: 656e 7365 203d 2051 7457 6964 6765 7473  ense = QtWidgets
-0000f170: 2e51 4163 7469 6f6e 284d 6169 6e57 696e  .QAction(MainWin
-0000f180: 646f 7729 0a20 2020 2020 2020 2073 656c  dow).        sel
-0000f190: 662e 6163 7469 6f6e 5f4c 6963 656e 7365  f.action_License
-0000f1a0: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
-0000f1b0: 6163 7469 6f6e 5f4c 6963 656e 7365 2229  action_License")
-0000f1c0: 0a20 2020 2020 2020 2073 656c 662e 6163  .        self.ac
-0000f1d0: 7469 6f6e 5f47 6973 5f45 7870 6f72 745f  tion_Gis_Export_
-0000f1e0: 7365 7474 696e 6773 203d 2051 7457 6964  settings = QtWid
-0000f1f0: 6765 7473 2e51 4163 7469 6f6e 284d 6169  gets.QAction(Mai
-0000f200: 6e57 696e 646f 7729 0a20 2020 2020 2020  nWindow).       
-0000f210: 2073 656c 662e 6163 7469 6f6e 5f47 6973   self.action_Gis
-0000f220: 5f45 7870 6f72 745f 7365 7474 696e 6773  _Export_settings
-0000f230: 2e73 6574 456e 6162 6c65 6428 4661 6c73  .setEnabled(Fals
-0000f240: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
-0000f250: 6163 7469 6f6e 5f47 6973 5f45 7870 6f72  action_Gis_Expor
-0000f260: 745f 7365 7474 696e 6773 2e73 6574 4f62  t_settings.setOb
-0000f270: 6a65 6374 4e61 6d65 2822 6163 7469 6f6e  jectName("action
-0000f280: 5f47 6973 5f45 7870 6f72 745f 7365 7474  _Gis_Export_sett
-0000f290: 696e 6773 2229 0a20 2020 2020 2020 2073  ings").        s
-0000f2a0: 656c 662e 6163 7469 6f6e 5f66 726f 6d5f  elf.action_from_
-0000f2b0: 6f65 7367 6e5f 7461 626c 6520 3d20 5174  oesgn_table = Qt
-0000f2c0: 5769 6467 6574 732e 5141 6374 696f 6e28  Widgets.QAction(
-0000f2d0: 4d61 696e 5769 6e64 6f77 290a 2020 2020  MainWindow).    
-0000f2e0: 2020 2020 7365 6c66 2e61 6374 696f 6e5f      self.action_
-0000f2f0: 6672 6f6d 5f6f 6573 676e 5f74 6162 6c65  from_oesgn_table
-0000f300: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
-0000f310: 6163 7469 6f6e 5f66 726f 6d5f 6f65 7367  action_from_oesg
-0000f320: 6e5f 7461 626c 6522 290a 2020 2020 2020  n_table").      
-0000f330: 2020 7365 6c66 2e61 6374 696f 6e5f 6672    self.action_fr
-0000f340: 6f6d 5f63 7376 5f66 696c 6520 3d20 5174  om_csv_file = Qt
-0000f350: 5769 6467 6574 732e 5141 6374 696f 6e28  Widgets.QAction(
-0000f360: 4d61 696e 5769 6e64 6f77 290a 2020 2020  MainWindow).    
-0000f370: 2020 2020 7365 6c66 2e61 6374 696f 6e5f      self.action_
-0000f380: 6672 6f6d 5f63 7376 5f66 696c 652e 7365  from_csv_file.se
-0000f390: 744f 626a 6563 744e 616d 6528 2261 6374  tObjectName("act
-0000f3a0: 696f 6e5f 6672 6f6d 5f63 7376 5f66 696c  ion_from_csv_fil
-0000f3b0: 6522 290a 2020 2020 2020 2020 7365 6c66  e").        self
-0000f3c0: 2e61 6374 696f 6e5f 436f 7272 6563 7469  .action_Correcti
-0000f3d0: 6f6e 5f74 696d 655f 7365 7269 6573 203d  on_time_series =
-0000f3e0: 2051 7457 6964 6765 7473 2e51 4163 7469   QtWidgets.QActi
-0000f3f0: 6f6e 284d 6169 6e57 696e 646f 7729 0a20  on(MainWindow). 
-0000f400: 2020 2020 2020 2073 656c 662e 6163 7469         self.acti
-0000f410: 6f6e 5f43 6f72 7265 6374 696f 6e5f 7469  on_Correction_ti
-0000f420: 6d65 5f73 6572 6965 732e 7365 744f 626a  me_series.setObj
-0000f430: 6563 744e 616d 6528 2261 6374 696f 6e5f  ectName("action_
-0000f440: 436f 7272 6563 7469 6f6e 5f74 696d 655f  Correction_time_
-0000f450: 7365 7269 6573 2229 0a20 2020 2020 2020  series").       
-0000f460: 2073 656c 662e 6163 7469 6f6e 5f67 7261   self.action_gra
-0000f470: 7669 6d65 7465 7273 5f66 726f 6d5f 6a73  vimeters_from_js
-0000f480: 6f6e 5f66 696c 6520 3d20 5174 5769 6467  on_file = QtWidg
-0000f490: 6574 732e 5141 6374 696f 6e28 4d61 696e  ets.QAction(Main
-0000f4a0: 5769 6e64 6f77 290a 2020 2020 2020 2020  Window).        
-0000f4b0: 7365 6c66 2e61 6374 696f 6e5f 6772 6176  self.action_grav
-0000f4c0: 696d 6574 6572 735f 6672 6f6d 5f6a 736f  imeters_from_jso
-0000f4d0: 6e5f 6669 6c65 2e73 6574 4f62 6a65 6374  n_file.setObject
-0000f4e0: 4e61 6d65 2822 6163 7469 6f6e 5f67 7261  Name("action_gra
-0000f4f0: 7669 6d65 7465 7273 5f66 726f 6d5f 6a73  vimeters_from_js
-0000f500: 6f6e 5f66 696c 6522 290a 2020 2020 2020  on_file").      
-0000f510: 2020 7365 6c66 2e6d 656e 7541 6464 5f53    self.menuAdd_S
-0000f520: 7572 7665 792e 6164 6441 6374 696f 6e28  urvey.addAction(
-0000f530: 7365 6c66 2e61 6374 696f 6e5f 6672 6f6d  self.action_from
-0000f540: 5f43 4735 5f6f 6273 6572 7661 7469 6f6e  _CG5_observation
-0000f550: 5f66 696c 6529 0a20 2020 2020 2020 2073  _file).        s
-0000f560: 656c 662e 6d65 6e75 4164 645f 5375 7276  elf.menuAdd_Surv
-0000f570: 6579 2e61 6464 4163 7469 6f6e 2873 656c  ey.addAction(sel
-0000f580: 662e 6163 7469 6f6e 5f66 726f 6d5f 4245  f.action_from_BE
-0000f590: 565f 6f62 7365 7276 6174 696f 6e5f 6669  V_observation_fi
-0000f5a0: 6c65 290a 2020 2020 2020 2020 7365 6c66  le).        self
-0000f5b0: 2e6d 656e 755f 4164 645f 5374 6174 696f  .menu_Add_Statio
-0000f5c0: 6e73 2e61 6464 4163 7469 6f6e 2873 656c  ns.addAction(sel
-0000f5d0: 662e 6163 7469 6f6e 5f66 726f 6d5f 6f65  f.action_from_oe
-0000f5e0: 7367 6e5f 7461 626c 6529 0a20 2020 2020  sgn_table).     
-0000f5f0: 2020 2073 656c 662e 6d65 6e75 5f41 6464     self.menu_Add
-0000f600: 5f53 7461 7469 6f6e 732e 6164 6441 6374  _Stations.addAct
-0000f610: 696f 6e28 7365 6c66 2e61 6374 696f 6e5f  ion(self.action_
-0000f620: 6672 6f6d 5f63 7376 5f66 696c 6529 0a20  from_csv_file). 
-0000f630: 2020 2020 2020 2073 656c 662e 6d65 6e75         self.menu
-0000f640: 5f41 6464 5f47 7261 7669 6d65 7465 7273  _Add_Gravimeters
-0000f650: 2e61 6464 4163 7469 6f6e 2873 656c 662e  .addAction(self.
-0000f660: 6163 7469 6f6e 5f67 7261 7669 6d65 7465  action_gravimete
-0000f670: 7273 5f66 726f 6d5f 6a73 6f6e 5f66 696c  rs_from_json_fil
-0000f680: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
-0000f690: 6d65 6e75 5f46 696c 652e 6164 6441 6374  menu_File.addAct
-0000f6a0: 696f 6e28 7365 6c66 2e61 6374 696f 6e5f  ion(self.action_
-0000f6b0: 4e65 775f 4361 6d70 6169 676e 290a 2020  New_Campaign).  
-0000f6c0: 2020 2020 2020 7365 6c66 2e6d 656e 755f        self.menu_
-0000f6d0: 4669 6c65 2e61 6464 4163 7469 6f6e 2873  File.addAction(s
-0000f6e0: 656c 662e 6163 7469 6f6e 5f43 6861 6e67  elf.action_Chang
-0000f6f0: 655f 6f75 7470 7574 5f64 6972 6563 746f  e_output_directo
-0000f700: 7279 290a 2020 2020 2020 2020 7365 6c66  ry).        self
-0000f710: 2e6d 656e 755f 4669 6c65 2e61 6464 4163  .menu_File.addAc
-0000f720: 7469 6f6e 2873 656c 662e 6163 7469 6f6e  tion(self.action
-0000f730: 5f43 6861 6e67 655f 4361 6d70 6169 676e  _Change_Campaign
-0000f740: 5f6e 616d 6529 0a20 2020 2020 2020 2073  _name).        s
-0000f750: 656c 662e 6d65 6e75 5f46 696c 652e 6164  elf.menu_File.ad
-0000f760: 6441 6374 696f 6e28 7365 6c66 2e61 6374  dAction(self.act
-0000f770: 696f 6e5f 5361 7665 5f43 616d 7061 6967  ion_Save_Campaig
-0000f780: 6e29 0a20 2020 2020 2020 2073 656c 662e  n).        self.
-0000f790: 6d65 6e75 5f46 696c 652e 6164 6441 6374  menu_File.addAct
-0000f7a0: 696f 6e28 7365 6c66 2e61 6374 696f 6e5f  ion(self.action_
-0000f7b0: 4c6f 6164 5f43 616d 7061 6967 6e29 0a20  Load_Campaign). 
-0000f7c0: 2020 2020 2020 2073 656c 662e 6d65 6e75         self.menu
-0000f7d0: 5f46 696c 652e 6164 6453 6570 6172 6174  _File.addSeparat
-0000f7e0: 6f72 2829 0a20 2020 2020 2020 2073 656c  or().        sel
-0000f7f0: 662e 6d65 6e75 5f46 696c 652e 6164 6441  f.menu_File.addA
-0000f800: 6374 696f 6e28 7365 6c66 2e6d 656e 7541  ction(self.menuA
-0000f810: 6464 5f53 7572 7665 792e 6d65 6e75 4163  dd_Survey.menuAc
-0000f820: 7469 6f6e 2829 290a 2020 2020 2020 2020  tion()).        
-0000f830: 7365 6c66 2e6d 656e 755f 4669 6c65 2e61  self.menu_File.a
-0000f840: 6464 4163 7469 6f6e 2873 656c 662e 6d65  ddAction(self.me
-0000f850: 6e75 5f41 6464 5f53 7461 7469 6f6e 732e  nu_Add_Stations.
-0000f860: 6d65 6e75 4163 7469 6f6e 2829 290a 2020  menuAction()).  
-0000f870: 2020 2020 2020 7365 6c66 2e6d 656e 755f        self.menu_
-0000f880: 4669 6c65 2e61 6464 4163 7469 6f6e 2873  File.addAction(s
-0000f890: 656c 662e 6d65 6e75 5f41 6464 5f47 7261  elf.menu_Add_Gra
-0000f8a0: 7669 6d65 7465 7273 2e6d 656e 7541 6374  vimeters.menuAct
-0000f8b0: 696f 6e28 2929 0a20 2020 2020 2020 2073  ion()).        s
-0000f8c0: 656c 662e 6d65 6e75 5f46 696c 652e 6164  elf.menu_File.ad
-0000f8d0: 6453 6570 6172 6174 6f72 2829 0a20 2020  dSeparator().   
-0000f8e0: 2020 2020 2073 656c 662e 6d65 6e75 5f46       self.menu_F
-0000f8f0: 696c 652e 6164 6441 6374 696f 6e28 7365  ile.addAction(se
-0000f900: 6c66 2e61 6374 696f 6e5f 4578 706f 7274  lf.action_Export
-0000f910: 5f52 6573 756c 7473 290a 2020 2020 2020  _Results).      
-0000f920: 2020 7365 6c66 2e6d 656e 755f 4669 6c65    self.menu_File
-0000f930: 2e61 6464 5365 7061 7261 746f 7228 290a  .addSeparator().
-0000f940: 2020 2020 2020 2020 7365 6c66 2e6d 656e          self.men
-0000f950: 755f 4669 6c65 2e61 6464 4163 7469 6f6e  u_File.addAction
-0000f960: 2873 656c 662e 6163 7469 6f6e 5f4f 7074  (self.action_Opt
-0000f970: 696f 6e73 290a 2020 2020 2020 2020 7365  ions).        se
-0000f980: 6c66 2e6d 656e 755f 4669 6c65 2e61 6464  lf.menu_File.add
-0000f990: 5365 7061 7261 746f 7228 290a 2020 2020  Separator().    
-0000f9a0: 2020 2020 7365 6c66 2e6d 656e 755f 4669      self.menu_Fi
-0000f9b0: 6c65 2e61 6464 4163 7469 6f6e 2873 656c  le.addAction(sel
-0000f9c0: 662e 6163 7469 6f6e 5f45 7869 7429 0a20  f.action_Exit). 
-0000f9d0: 2020 2020 2020 2073 656c 662e 6d65 6e75         self.menu
-0000f9e0: 5f4f 6273 6572 7661 7469 6f6e 732e 6164  _Observations.ad
-0000f9f0: 6453 6570 6172 6174 6f72 2829 0a20 2020  dSeparator().   
-0000fa00: 2020 2020 2073 656c 662e 6d65 6e75 5f4f       self.menu_O
-0000fa10: 6273 6572 7661 7469 6f6e 732e 6164 6441  bservations.addA
-0000fa20: 6374 696f 6e28 7365 6c66 2e61 6374 696f  ction(self.actio
-0000fa30: 6e5f 4175 746f 7365 6c65 6374 696f 6e5f  n_Autoselection_
-0000fa40: 7365 7474 696e 6773 290a 2020 2020 2020  settings).      
-0000fa50: 2020 7365 6c66 2e6d 656e 755f 4f62 7365    self.menu_Obse
-0000fa60: 7276 6174 696f 6e73 2e61 6464 4163 7469  rvations.addActi
-0000fa70: 6f6e 2873 656c 662e 6163 7469 6f6e 5f53  on(self.action_S
-0000fa80: 6574 7570 5f64 6174 615f 6f70 7469 6f6e  etup_data_option
-0000fa90: 7329 0a20 2020 2020 2020 2073 656c 662e  s).        self.
-0000faa0: 6d65 6e75 5f4f 6273 6572 7661 7469 6f6e  menu_Observation
-0000fab0: 732e 6164 6441 6374 696f 6e28 7365 6c66  s.addAction(self
-0000fac0: 2e61 6374 696f 6e5f 466c 6167 5f6f 6273  .action_Flag_obs
-0000fad0: 6572 7661 7469 6f6e 7329 0a20 2020 2020  ervations).     
-0000fae0: 2020 2073 656c 662e 6d65 6e75 4573 7469     self.menuEsti
-0000faf0: 6d61 7469 6f6e 5f73 6574 7469 6e67 732e  mation_settings.
-0000fb00: 6164 6441 6374 696f 6e28 7365 6c66 2e61  addAction(self.a
-0000fb10: 6374 696f 6e5f 4573 7469 6d61 7469 6f6e  ction_Estimation
-0000fb20: 5f73 6574 7469 6e67 7329 0a20 2020 2020  _settings).     
-0000fb30: 2020 2073 656c 662e 6d65 6e75 4573 7469     self.menuEsti
-0000fb40: 6d61 7469 6f6e 5f73 6574 7469 6e67 732e  mation_settings.
-0000fb50: 6164 6441 6374 696f 6e28 7365 6c66 2e61  addAction(self.a
-0000fb60: 6374 696f 6e5f 4769 735f 4578 706f 7274  ction_Gis_Export
-0000fb70: 5f73 6574 7469 6e67 7329 0a20 2020 2020  _settings).     
-0000fb80: 2020 2073 656c 662e 6d65 6e75 4865 6c70     self.menuHelp
-0000fb90: 2e61 6464 4163 7469 6f6e 2873 656c 662e  .addAction(self.
-0000fba0: 6163 7469 6f6e 5f41 626f 7574 290a 2020  action_About).  
-0000fbb0: 2020 2020 2020 7365 6c66 2e6d 656e 7543        self.menuC
-0000fbc0: 6f72 7265 6374 696f 6e73 2e61 6464 4163  orrections.addAc
-0000fbd0: 7469 6f6e 2873 656c 662e 6163 7469 6f6e  tion(self.action
-0000fbe0: 5f43 6f72 7265 6374 696f 6e73 290a 2020  _Corrections).  
-0000fbf0: 2020 2020 2020 7365 6c66 2e6d 656e 7543        self.menuC
-0000fc00: 6f72 7265 6374 696f 6e73 2e61 6464 4163  orrections.addAc
-0000fc10: 7469 6f6e 2873 656c 662e 6163 7469 6f6e  tion(self.action
-0000fc20: 5f43 6f72 7265 6374 696f 6e5f 7469 6d65  _Correction_time
-0000fc30: 5f73 6572 6965 7329 0a20 2020 2020 2020  _series).       
-0000fc40: 2073 656c 662e 6d65 6e75 6261 722e 6164   self.menubar.ad
-0000fc50: 6441 6374 696f 6e28 7365 6c66 2e6d 656e  dAction(self.men
-0000fc60: 755f 4669 6c65 2e6d 656e 7541 6374 696f  u_File.menuActio
-0000fc70: 6e28 2929 0a20 2020 2020 2020 2073 656c  n()).        sel
-0000fc80: 662e 6d65 6e75 6261 722e 6164 6441 6374  f.menubar.addAct
-0000fc90: 696f 6e28 7365 6c66 2e6d 656e 755f 4f62  ion(self.menu_Ob
-0000fca0: 7365 7276 6174 696f 6e73 2e6d 656e 7541  servations.menuA
+0000be90: 6174 6973 7469 6373 5f73 656c 6563 745f  atistics_select_
+0000bea0: 636f 6c22 290a 2020 2020 2020 2020 7365  col").        se
+0000beb0: 6c66 2e76 6572 7469 6361 6c4c 6179 6f75  lf.verticalLayou
+0000bec0: 745f 3139 2e61 6464 5769 6467 6574 2873  t_19.addWidget(s
+0000bed0: 656c 662e 636f 6d62 6f42 6f78 5f72 6573  elf.comboBox_res
+0000bee0: 756c 7473 5f73 7461 7469 6f6e 735f 7374  ults_stations_st
+0000bef0: 6174 6973 7469 6373 5f73 656c 6563 745f  atistics_select_
+0000bf00: 636f 6c29 0a20 2020 2020 2020 2073 656c  col).        sel
+0000bf10: 662e 686f 7269 7a6f 6e74 616c 4c61 796f  f.horizontalLayo
+0000bf20: 7574 5f34 2e61 6464 4c61 796f 7574 2873  ut_4.addLayout(s
+0000bf30: 656c 662e 7665 7274 6963 616c 4c61 796f  elf.verticalLayo
+0000bf40: 7574 5f31 3929 0a20 2020 2020 2020 2073  ut_19).        s
+0000bf50: 656c 662e 666f 726d 4c61 796f 7574 5f39  elf.formLayout_9
+0000bf60: 203d 2051 7457 6964 6765 7473 2e51 466f   = QtWidgets.QFo
+0000bf70: 726d 4c61 796f 7574 2829 0a20 2020 2020  rmLayout().     
+0000bf80: 2020 2073 656c 662e 666f 726d 4c61 796f     self.formLayo
+0000bf90: 7574 5f39 2e73 6574 4f62 6a65 6374 4e61  ut_9.setObjectNa
+0000bfa0: 6d65 2822 666f 726d 4c61 796f 7574 5f39  me("formLayout_9
+0000bfb0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+0000bfc0: 6c61 6265 6c5f 3133 203d 2051 7457 6964  label_13 = QtWid
+0000bfd0: 6765 7473 2e51 4c61 6265 6c28 7365 6c66  gets.QLabel(self
+0000bfe0: 2e67 726f 7570 426f 785f 7265 7375 6c74  .groupBox_result
+0000bff0: 735f 7374 6174 696f 6e73 5f73 7461 7469  s_stations_stati
+0000c000: 7374 6963 7329 0a20 2020 2020 2020 2073  stics).        s
+0000c010: 656c 662e 6c61 6265 6c5f 3133 2e73 6574  elf.label_13.set
+0000c020: 4f62 6a65 6374 4e61 6d65 2822 6c61 6265  ObjectName("labe
+0000c030: 6c5f 3133 2229 0a20 2020 2020 2020 2073  l_13").        s
+0000c040: 656c 662e 666f 726d 4c61 796f 7574 5f39  elf.formLayout_9
+0000c050: 2e73 6574 5769 6467 6574 2830 2c20 5174  .setWidget(0, Qt
+0000c060: 5769 6467 6574 732e 5146 6f72 6d4c 6179  Widgets.QFormLay
+0000c070: 6f75 742e 4c61 6265 6c52 6f6c 652c 2073  out.LabelRole, s
+0000c080: 656c 662e 6c61 6265 6c5f 3133 290a 2020  elf.label_13).  
+0000c090: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
+0000c0a0: 5f72 6573 756c 7473 5f73 7461 7469 6f6e  _results_station
+0000c0b0: 735f 7374 6174 6973 7469 6373 5f6d 6561  s_statistics_mea
+0000c0c0: 6e20 3d20 5174 5769 6467 6574 732e 514c  n = QtWidgets.QL
+0000c0d0: 6162 656c 2873 656c 662e 6772 6f75 7042  abel(self.groupB
+0000c0e0: 6f78 5f72 6573 756c 7473 5f73 7461 7469  ox_results_stati
+0000c0f0: 6f6e 735f 7374 6174 6973 7469 6373 290a  ons_statistics).
+0000c100: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
+0000c110: 656c 5f72 6573 756c 7473 5f73 7461 7469  el_results_stati
+0000c120: 6f6e 735f 7374 6174 6973 7469 6373 5f6d  ons_statistics_m
+0000c130: 6561 6e2e 7365 7454 6578 7428 2222 290a  ean.setText("").
+0000c140: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
+0000c150: 656c 5f72 6573 756c 7473 5f73 7461 7469  el_results_stati
+0000c160: 6f6e 735f 7374 6174 6973 7469 6373 5f6d  ons_statistics_m
+0000c170: 6561 6e2e 7365 744f 626a 6563 744e 616d  ean.setObjectNam
+0000c180: 6528 226c 6162 656c 5f72 6573 756c 7473  e("label_results
+0000c190: 5f73 7461 7469 6f6e 735f 7374 6174 6973  _stations_statis
+0000c1a0: 7469 6373 5f6d 6561 6e22 290a 2020 2020  tics_mean").    
+0000c1b0: 2020 2020 7365 6c66 2e66 6f72 6d4c 6179      self.formLay
+0000c1c0: 6f75 745f 392e 7365 7457 6964 6765 7428  out_9.setWidget(
+0000c1d0: 302c 2051 7457 6964 6765 7473 2e51 466f  0, QtWidgets.QFo
+0000c1e0: 726d 4c61 796f 7574 2e46 6965 6c64 526f  rmLayout.FieldRo
+0000c1f0: 6c65 2c20 7365 6c66 2e6c 6162 656c 5f72  le, self.label_r
+0000c200: 6573 756c 7473 5f73 7461 7469 6f6e 735f  esults_stations_
+0000c210: 7374 6174 6973 7469 6373 5f6d 6561 6e29  statistics_mean)
+0000c220: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
+0000c230: 6265 6c5f 3134 203d 2051 7457 6964 6765  bel_14 = QtWidge
+0000c240: 7473 2e51 4c61 6265 6c28 7365 6c66 2e67  ts.QLabel(self.g
+0000c250: 726f 7570 426f 785f 7265 7375 6c74 735f  roupBox_results_
+0000c260: 7374 6174 696f 6e73 5f73 7461 7469 7374  stations_statist
+0000c270: 6963 7329 0a20 2020 2020 2020 2073 656c  ics).        sel
+0000c280: 662e 6c61 6265 6c5f 3134 2e73 6574 4f62  f.label_14.setOb
+0000c290: 6a65 6374 4e61 6d65 2822 6c61 6265 6c5f  jectName("label_
+0000c2a0: 3134 2229 0a20 2020 2020 2020 2073 656c  14").        sel
+0000c2b0: 662e 666f 726d 4c61 796f 7574 5f39 2e73  f.formLayout_9.s
+0000c2c0: 6574 5769 6467 6574 2831 2c20 5174 5769  etWidget(1, QtWi
+0000c2d0: 6467 6574 732e 5146 6f72 6d4c 6179 6f75  dgets.QFormLayou
+0000c2e0: 742e 4c61 6265 6c52 6f6c 652c 2073 656c  t.LabelRole, sel
+0000c2f0: 662e 6c61 6265 6c5f 3134 290a 2020 2020  f.label_14).    
+0000c300: 2020 2020 7365 6c66 2e6c 6162 656c 5f72      self.label_r
+0000c310: 6573 756c 7473 5f73 7461 7469 6f6e 735f  esults_stations_
+0000c320: 7374 6174 6973 7469 6373 5f73 7464 203d  statistics_std =
+0000c330: 2051 7457 6964 6765 7473 2e51 4c61 6265   QtWidgets.QLabe
+0000c340: 6c28 7365 6c66 2e67 726f 7570 426f 785f  l(self.groupBox_
+0000c350: 7265 7375 6c74 735f 7374 6174 696f 6e73  results_stations
+0000c360: 5f73 7461 7469 7374 6963 7329 0a20 2020  _statistics).   
+0000c370: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
+0000c380: 7265 7375 6c74 735f 7374 6174 696f 6e73  results_stations
+0000c390: 5f73 7461 7469 7374 6963 735f 7374 642e  _statistics_std.
+0000c3a0: 7365 7454 6578 7428 2222 290a 2020 2020  setText("").    
+0000c3b0: 2020 2020 7365 6c66 2e6c 6162 656c 5f72      self.label_r
+0000c3c0: 6573 756c 7473 5f73 7461 7469 6f6e 735f  esults_stations_
+0000c3d0: 7374 6174 6973 7469 6373 5f73 7464 2e73  statistics_std.s
+0000c3e0: 6574 4f62 6a65 6374 4e61 6d65 2822 6c61  etObjectName("la
+0000c3f0: 6265 6c5f 7265 7375 6c74 735f 7374 6174  bel_results_stat
+0000c400: 696f 6e73 5f73 7461 7469 7374 6963 735f  ions_statistics_
+0000c410: 7374 6422 290a 2020 2020 2020 2020 7365  std").        se
+0000c420: 6c66 2e66 6f72 6d4c 6179 6f75 745f 392e  lf.formLayout_9.
+0000c430: 7365 7457 6964 6765 7428 312c 2051 7457  setWidget(1, QtW
+0000c440: 6964 6765 7473 2e51 466f 726d 4c61 796f  idgets.QFormLayo
+0000c450: 7574 2e46 6965 6c64 526f 6c65 2c20 7365  ut.FieldRole, se
+0000c460: 6c66 2e6c 6162 656c 5f72 6573 756c 7473  lf.label_results
+0000c470: 5f73 7461 7469 6f6e 735f 7374 6174 6973  _stations_statis
+0000c480: 7469 6373 5f73 7464 290a 2020 2020 2020  tics_std).      
+0000c490: 2020 7365 6c66 2e68 6f72 697a 6f6e 7461    self.horizonta
+0000c4a0: 6c4c 6179 6f75 745f 342e 6164 644c 6179  lLayout_4.addLay
+0000c4b0: 6f75 7428 7365 6c66 2e66 6f72 6d4c 6179  out(self.formLay
+0000c4c0: 6f75 745f 3929 0a20 2020 2020 2020 2073  out_9).        s
+0000c4d0: 656c 662e 666f 726d 4c61 796f 7574 5f31  elf.formLayout_1
+0000c4e0: 3020 3d20 5174 5769 6467 6574 732e 5146  0 = QtWidgets.QF
+0000c4f0: 6f72 6d4c 6179 6f75 7428 290a 2020 2020  ormLayout().    
+0000c500: 2020 2020 7365 6c66 2e66 6f72 6d4c 6179      self.formLay
+0000c510: 6f75 745f 3130 2e73 6574 4f62 6a65 6374  out_10.setObject
+0000c520: 4e61 6d65 2822 666f 726d 4c61 796f 7574  Name("formLayout
+0000c530: 5f31 3022 290a 2020 2020 2020 2020 7365  _10").        se
+0000c540: 6c66 2e6c 6162 656c 5f31 3520 3d20 5174  lf.label_15 = Qt
+0000c550: 5769 6467 6574 732e 514c 6162 656c 2873  Widgets.QLabel(s
+0000c560: 656c 662e 6772 6f75 7042 6f78 5f72 6573  elf.groupBox_res
+0000c570: 756c 7473 5f73 7461 7469 6f6e 735f 7374  ults_stations_st
+0000c580: 6174 6973 7469 6373 290a 2020 2020 2020  atistics).      
+0000c590: 2020 7365 6c66 2e6c 6162 656c 5f31 352e    self.label_15.
+0000c5a0: 7365 744f 626a 6563 744e 616d 6528 226c  setObjectName("l
+0000c5b0: 6162 656c 5f31 3522 290a 2020 2020 2020  abel_15").      
+0000c5c0: 2020 7365 6c66 2e66 6f72 6d4c 6179 6f75    self.formLayou
+0000c5d0: 745f 3130 2e73 6574 5769 6467 6574 2830  t_10.setWidget(0
+0000c5e0: 2c20 5174 5769 6467 6574 732e 5146 6f72  , QtWidgets.QFor
+0000c5f0: 6d4c 6179 6f75 742e 4c61 6265 6c52 6f6c  mLayout.LabelRol
+0000c600: 652c 2073 656c 662e 6c61 6265 6c5f 3135  e, self.label_15
+0000c610: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
+0000c620: 6162 656c 5f72 6573 756c 7473 5f73 7461  abel_results_sta
+0000c630: 7469 6f6e 735f 7374 6174 6973 7469 6373  tions_statistics
+0000c640: 5f6d 696e 203d 2051 7457 6964 6765 7473  _min = QtWidgets
+0000c650: 2e51 4c61 6265 6c28 7365 6c66 2e67 726f  .QLabel(self.gro
+0000c660: 7570 426f 785f 7265 7375 6c74 735f 7374  upBox_results_st
+0000c670: 6174 696f 6e73 5f73 7461 7469 7374 6963  ations_statistic
+0000c680: 7329 0a20 2020 2020 2020 2073 656c 662e  s).        self.
+0000c690: 6c61 6265 6c5f 7265 7375 6c74 735f 7374  label_results_st
+0000c6a0: 6174 696f 6e73 5f73 7461 7469 7374 6963  ations_statistic
+0000c6b0: 735f 6d69 6e2e 7365 7454 6578 7428 2222  s_min.setText(""
+0000c6c0: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
+0000c6d0: 6162 656c 5f72 6573 756c 7473 5f73 7461  abel_results_sta
+0000c6e0: 7469 6f6e 735f 7374 6174 6973 7469 6373  tions_statistics
+0000c6f0: 5f6d 696e 2e73 6574 4f62 6a65 6374 4e61  _min.setObjectNa
+0000c700: 6d65 2822 6c61 6265 6c5f 7265 7375 6c74  me("label_result
+0000c710: 735f 7374 6174 696f 6e73 5f73 7461 7469  s_stations_stati
+0000c720: 7374 6963 735f 6d69 6e22 290a 2020 2020  stics_min").    
+0000c730: 2020 2020 7365 6c66 2e66 6f72 6d4c 6179      self.formLay
+0000c740: 6f75 745f 3130 2e73 6574 5769 6467 6574  out_10.setWidget
+0000c750: 2830 2c20 5174 5769 6467 6574 732e 5146  (0, QtWidgets.QF
+0000c760: 6f72 6d4c 6179 6f75 742e 4669 656c 6452  ormLayout.FieldR
+0000c770: 6f6c 652c 2073 656c 662e 6c61 6265 6c5f  ole, self.label_
+0000c780: 7265 7375 6c74 735f 7374 6174 696f 6e73  results_stations
+0000c790: 5f73 7461 7469 7374 6963 735f 6d69 6e29  _statistics_min)
+0000c7a0: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
+0000c7b0: 6265 6c5f 3136 203d 2051 7457 6964 6765  bel_16 = QtWidge
+0000c7c0: 7473 2e51 4c61 6265 6c28 7365 6c66 2e67  ts.QLabel(self.g
+0000c7d0: 726f 7570 426f 785f 7265 7375 6c74 735f  roupBox_results_
+0000c7e0: 7374 6174 696f 6e73 5f73 7461 7469 7374  stations_statist
+0000c7f0: 6963 7329 0a20 2020 2020 2020 2073 656c  ics).        sel
+0000c800: 662e 6c61 6265 6c5f 3136 2e73 6574 4f62  f.label_16.setOb
+0000c810: 6a65 6374 4e61 6d65 2822 6c61 6265 6c5f  jectName("label_
+0000c820: 3136 2229 0a20 2020 2020 2020 2073 656c  16").        sel
+0000c830: 662e 666f 726d 4c61 796f 7574 5f31 302e  f.formLayout_10.
+0000c840: 7365 7457 6964 6765 7428 312c 2051 7457  setWidget(1, QtW
+0000c850: 6964 6765 7473 2e51 466f 726d 4c61 796f  idgets.QFormLayo
+0000c860: 7574 2e4c 6162 656c 526f 6c65 2c20 7365  ut.LabelRole, se
+0000c870: 6c66 2e6c 6162 656c 5f31 3629 0a20 2020  lf.label_16).   
+0000c880: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
+0000c890: 7265 7375 6c74 735f 7374 6174 696f 6e73  results_stations
+0000c8a0: 5f73 7461 7469 7374 6963 735f 6d61 7820  _statistics_max 
+0000c8b0: 3d20 5174 5769 6467 6574 732e 514c 6162  = QtWidgets.QLab
+0000c8c0: 656c 2873 656c 662e 6772 6f75 7042 6f78  el(self.groupBox
+0000c8d0: 5f72 6573 756c 7473 5f73 7461 7469 6f6e  _results_station
+0000c8e0: 735f 7374 6174 6973 7469 6373 290a 2020  s_statistics).  
+0000c8f0: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
+0000c900: 5f72 6573 756c 7473 5f73 7461 7469 6f6e  _results_station
+0000c910: 735f 7374 6174 6973 7469 6373 5f6d 6178  s_statistics_max
+0000c920: 2e73 6574 5465 7874 2822 2229 0a20 2020  .setText("").   
+0000c930: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
+0000c940: 7265 7375 6c74 735f 7374 6174 696f 6e73  results_stations
+0000c950: 5f73 7461 7469 7374 6963 735f 6d61 782e  _statistics_max.
+0000c960: 7365 744f 626a 6563 744e 616d 6528 226c  setObjectName("l
+0000c970: 6162 656c 5f72 6573 756c 7473 5f73 7461  abel_results_sta
+0000c980: 7469 6f6e 735f 7374 6174 6973 7469 6373  tions_statistics
+0000c990: 5f6d 6178 2229 0a20 2020 2020 2020 2073  _max").        s
+0000c9a0: 656c 662e 666f 726d 4c61 796f 7574 5f31  elf.formLayout_1
+0000c9b0: 302e 7365 7457 6964 6765 7428 312c 2051  0.setWidget(1, Q
+0000c9c0: 7457 6964 6765 7473 2e51 466f 726d 4c61  tWidgets.QFormLa
+0000c9d0: 796f 7574 2e46 6965 6c64 526f 6c65 2c20  yout.FieldRole, 
+0000c9e0: 7365 6c66 2e6c 6162 656c 5f72 6573 756c  self.label_resul
+0000c9f0: 7473 5f73 7461 7469 6f6e 735f 7374 6174  ts_stations_stat
+0000ca00: 6973 7469 6373 5f6d 6178 290a 2020 2020  istics_max).    
+0000ca10: 2020 2020 7365 6c66 2e68 6f72 697a 6f6e      self.horizon
+0000ca20: 7461 6c4c 6179 6f75 745f 342e 6164 644c  talLayout_4.addL
+0000ca30: 6179 6f75 7428 7365 6c66 2e66 6f72 6d4c  ayout(self.formL
+0000ca40: 6179 6f75 745f 3130 290a 2020 2020 2020  ayout_10).      
+0000ca50: 2020 7365 6c66 2e66 6f72 6d4c 6179 6f75    self.formLayou
+0000ca60: 745f 3131 203d 2051 7457 6964 6765 7473  t_11 = QtWidgets
+0000ca70: 2e51 466f 726d 4c61 796f 7574 2829 0a20  .QFormLayout(). 
+0000ca80: 2020 2020 2020 2073 656c 662e 666f 726d         self.form
+0000ca90: 4c61 796f 7574 5f31 312e 7365 744f 626a  Layout_11.setObj
+0000caa0: 6563 744e 616d 6528 2266 6f72 6d4c 6179  ectName("formLay
+0000cab0: 6f75 745f 3131 2229 0a20 2020 2020 2020  out_11").       
+0000cac0: 2073 656c 662e 6c61 6265 6c5f 3137 203d   self.label_17 =
+0000cad0: 2051 7457 6964 6765 7473 2e51 4c61 6265   QtWidgets.QLabe
+0000cae0: 6c28 7365 6c66 2e67 726f 7570 426f 785f  l(self.groupBox_
+0000caf0: 7265 7375 6c74 735f 7374 6174 696f 6e73  results_stations
+0000cb00: 5f73 7461 7469 7374 6963 7329 0a20 2020  _statistics).   
+0000cb10: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
+0000cb20: 3137 2e73 6574 4f62 6a65 6374 4e61 6d65  17.setObjectName
+0000cb30: 2822 6c61 6265 6c5f 3137 2229 0a20 2020  ("label_17").   
+0000cb40: 2020 2020 2073 656c 662e 666f 726d 4c61       self.formLa
+0000cb50: 796f 7574 5f31 312e 7365 7457 6964 6765  yout_11.setWidge
+0000cb60: 7428 302c 2051 7457 6964 6765 7473 2e51  t(0, QtWidgets.Q
+0000cb70: 466f 726d 4c61 796f 7574 2e4c 6162 656c  FormLayout.Label
+0000cb80: 526f 6c65 2c20 7365 6c66 2e6c 6162 656c  Role, self.label
+0000cb90: 5f31 3729 0a20 2020 2020 2020 2073 656c  _17).        sel
+0000cba0: 662e 6c61 6265 6c5f 5f72 6573 756c 7473  f.label__results
+0000cbb0: 5f73 7461 7469 6f6e 735f 7374 6174 6973  _stations_statis
+0000cbc0: 7469 6373 5f6d 6564 6961 6e20 3d20 5174  tics_median = Qt
+0000cbd0: 5769 6467 6574 732e 514c 6162 656c 2873  Widgets.QLabel(s
+0000cbe0: 656c 662e 6772 6f75 7042 6f78 5f72 6573  elf.groupBox_res
+0000cbf0: 756c 7473 5f73 7461 7469 6f6e 735f 7374  ults_stations_st
+0000cc00: 6174 6973 7469 6373 290a 2020 2020 2020  atistics).      
+0000cc10: 2020 7365 6c66 2e6c 6162 656c 5f5f 7265    self.label__re
+0000cc20: 7375 6c74 735f 7374 6174 696f 6e73 5f73  sults_stations_s
+0000cc30: 7461 7469 7374 6963 735f 6d65 6469 616e  tatistics_median
+0000cc40: 2e73 6574 5465 7874 2822 2229 0a20 2020  .setText("").   
+0000cc50: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
+0000cc60: 5f72 6573 756c 7473 5f73 7461 7469 6f6e  _results_station
+0000cc70: 735f 7374 6174 6973 7469 6373 5f6d 6564  s_statistics_med
+0000cc80: 6961 6e2e 7365 744f 626a 6563 744e 616d  ian.setObjectNam
+0000cc90: 6528 226c 6162 656c 5f5f 7265 7375 6c74  e("label__result
+0000cca0: 735f 7374 6174 696f 6e73 5f73 7461 7469  s_stations_stati
+0000ccb0: 7374 6963 735f 6d65 6469 616e 2229 0a20  stics_median"). 
+0000ccc0: 2020 2020 2020 2073 656c 662e 666f 726d         self.form
+0000ccd0: 4c61 796f 7574 5f31 312e 7365 7457 6964  Layout_11.setWid
+0000cce0: 6765 7428 302c 2051 7457 6964 6765 7473  get(0, QtWidgets
+0000ccf0: 2e51 466f 726d 4c61 796f 7574 2e46 6965  .QFormLayout.Fie
+0000cd00: 6c64 526f 6c65 2c20 7365 6c66 2e6c 6162  ldRole, self.lab
+0000cd10: 656c 5f5f 7265 7375 6c74 735f 7374 6174  el__results_stat
+0000cd20: 696f 6e73 5f73 7461 7469 7374 6963 735f  ions_statistics_
+0000cd30: 6d65 6469 616e 290a 2020 2020 2020 2020  median).        
+0000cd40: 7365 6c66 2e6c 6162 656c 5f31 3820 3d20  self.label_18 = 
+0000cd50: 5174 5769 6467 6574 732e 514c 6162 656c  QtWidgets.QLabel
+0000cd60: 2873 656c 662e 6772 6f75 7042 6f78 5f72  (self.groupBox_r
+0000cd70: 6573 756c 7473 5f73 7461 7469 6f6e 735f  esults_stations_
+0000cd80: 7374 6174 6973 7469 6373 290a 2020 2020  statistics).    
+0000cd90: 2020 2020 7365 6c66 2e6c 6162 656c 5f31      self.label_1
+0000cda0: 382e 7365 744f 626a 6563 744e 616d 6528  8.setObjectName(
+0000cdb0: 226c 6162 656c 5f31 3822 290a 2020 2020  "label_18").    
+0000cdc0: 2020 2020 7365 6c66 2e66 6f72 6d4c 6179      self.formLay
+0000cdd0: 6f75 745f 3131 2e73 6574 5769 6467 6574  out_11.setWidget
+0000cde0: 2831 2c20 5174 5769 6467 6574 732e 5146  (1, QtWidgets.QF
+0000cdf0: 6f72 6d4c 6179 6f75 742e 4c61 6265 6c52  ormLayout.LabelR
+0000ce00: 6f6c 652c 2073 656c 662e 6c61 6265 6c5f  ole, self.label_
+0000ce10: 3138 290a 2020 2020 2020 2020 7365 6c66  18).        self
+0000ce20: 2e6c 6162 656c 5f5f 7265 7375 6c74 735f  .label__results_
+0000ce30: 7374 6174 696f 6e73 5f73 7461 7469 7374  stations_statist
+0000ce40: 6963 735f 6971 7220 3d20 5174 5769 6467  ics_iqr = QtWidg
+0000ce50: 6574 732e 514c 6162 656c 2873 656c 662e  ets.QLabel(self.
+0000ce60: 6772 6f75 7042 6f78 5f72 6573 756c 7473  groupBox_results
+0000ce70: 5f73 7461 7469 6f6e 735f 7374 6174 6973  _stations_statis
+0000ce80: 7469 6373 290a 2020 2020 2020 2020 7365  tics).        se
+0000ce90: 6c66 2e6c 6162 656c 5f5f 7265 7375 6c74  lf.label__result
+0000cea0: 735f 7374 6174 696f 6e73 5f73 7461 7469  s_stations_stati
+0000ceb0: 7374 6963 735f 6971 722e 7365 7454 6578  stics_iqr.setTex
+0000cec0: 7428 2222 290a 2020 2020 2020 2020 7365  t("").        se
+0000ced0: 6c66 2e6c 6162 656c 5f5f 7265 7375 6c74  lf.label__result
+0000cee0: 735f 7374 6174 696f 6e73 5f73 7461 7469  s_stations_stati
+0000cef0: 7374 6963 735f 6971 722e 7365 744f 626a  stics_iqr.setObj
+0000cf00: 6563 744e 616d 6528 226c 6162 656c 5f5f  ectName("label__
+0000cf10: 7265 7375 6c74 735f 7374 6174 696f 6e73  results_stations
+0000cf20: 5f73 7461 7469 7374 6963 735f 6971 7222  _statistics_iqr"
+0000cf30: 290a 2020 2020 2020 2020 7365 6c66 2e66  ).        self.f
+0000cf40: 6f72 6d4c 6179 6f75 745f 3131 2e73 6574  ormLayout_11.set
+0000cf50: 5769 6467 6574 2831 2c20 5174 5769 6467  Widget(1, QtWidg
+0000cf60: 6574 732e 5146 6f72 6d4c 6179 6f75 742e  ets.QFormLayout.
+0000cf70: 4669 656c 6452 6f6c 652c 2073 656c 662e  FieldRole, self.
+0000cf80: 6c61 6265 6c5f 5f72 6573 756c 7473 5f73  label__results_s
+0000cf90: 7461 7469 6f6e 735f 7374 6174 6973 7469  tations_statisti
+0000cfa0: 6373 5f69 7172 290a 2020 2020 2020 2020  cs_iqr).        
+0000cfb0: 7365 6c66 2e68 6f72 697a 6f6e 7461 6c4c  self.horizontalL
+0000cfc0: 6179 6f75 745f 342e 6164 644c 6179 6f75  ayout_4.addLayou
+0000cfd0: 7428 7365 6c66 2e66 6f72 6d4c 6179 6f75  t(self.formLayou
+0000cfe0: 745f 3131 290a 2020 2020 2020 2020 7365  t_11).        se
+0000cff0: 6c66 2e76 6572 7469 6361 6c4c 6179 6f75  lf.verticalLayou
+0000d000: 745f 3339 2e61 6464 5769 6467 6574 2873  t_39.addWidget(s
+0000d010: 656c 662e 6772 6f75 7042 6f78 5f72 6573  elf.groupBox_res
+0000d020: 756c 7473 5f73 7461 7469 6f6e 735f 7374  ults_stations_st
+0000d030: 6174 6973 7469 6373 290a 2020 2020 2020  atistics).      
+0000d040: 2020 7365 6c66 2e74 6162 5769 6467 6574    self.tabWidget
+0000d050: 5f72 6573 756c 7473 2e61 6464 5461 6228  _results.addTab(
+0000d060: 7365 6c66 2e74 6162 5f72 6573 756c 7473  self.tab_results
+0000d070: 5f73 7461 745f 7461 626c 652c 2022 2229  _stat_table, "")
+0000d080: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
+0000d090: 625f 7265 7375 6c74 735f 636f 7272 656c  b_results_correl
+0000d0a0: 6174 696f 6e5f 6d61 7472 6978 203d 2051  ation_matrix = Q
+0000d0b0: 7457 6964 6765 7473 2e51 5769 6467 6574  tWidgets.QWidget
+0000d0c0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+0000d0d0: 7461 625f 7265 7375 6c74 735f 636f 7272  tab_results_corr
+0000d0e0: 656c 6174 696f 6e5f 6d61 7472 6978 2e73  elation_matrix.s
+0000d0f0: 6574 4f62 6a65 6374 4e61 6d65 2822 7461  etObjectName("ta
+0000d100: 625f 7265 7375 6c74 735f 636f 7272 656c  b_results_correl
+0000d110: 6174 696f 6e5f 6d61 7472 6978 2229 0a20  ation_matrix"). 
+0000d120: 2020 2020 2020 2073 656c 662e 7665 7274         self.vert
+0000d130: 6963 616c 4c61 796f 7574 5f33 3220 3d20  icalLayout_32 = 
+0000d140: 5174 5769 6467 6574 732e 5156 426f 784c  QtWidgets.QVBoxL
+0000d150: 6179 6f75 7428 7365 6c66 2e74 6162 5f72  ayout(self.tab_r
+0000d160: 6573 756c 7473 5f63 6f72 7265 6c61 7469  esults_correlati
+0000d170: 6f6e 5f6d 6174 7269 7829 0a20 2020 2020  on_matrix).     
+0000d180: 2020 2073 656c 662e 7665 7274 6963 616c     self.vertical
+0000d190: 4c61 796f 7574 5f33 322e 7365 744f 626a  Layout_32.setObj
+0000d1a0: 6563 744e 616d 6528 2276 6572 7469 6361  ectName("vertica
+0000d1b0: 6c4c 6179 6f75 745f 3332 2229 0a20 2020  lLayout_32").   
+0000d1c0: 2020 2020 2073 656c 662e 7461 626c 6556       self.tableV
+0000d1d0: 6965 775f 7265 7375 6c74 735f 636f 7272  iew_results_corr
+0000d1e0: 656c 6174 696f 6e5f 6d61 7472 6978 203d  elation_matrix =
+0000d1f0: 2051 7457 6964 6765 7473 2e51 5461 626c   QtWidgets.QTabl
+0000d200: 6556 6965 7728 7365 6c66 2e74 6162 5f72  eView(self.tab_r
+0000d210: 6573 756c 7473 5f63 6f72 7265 6c61 7469  esults_correlati
+0000d220: 6f6e 5f6d 6174 7269 7829 0a20 2020 2020  on_matrix).     
+0000d230: 2020 2073 656c 662e 7461 626c 6556 6965     self.tableVie
+0000d240: 775f 7265 7375 6c74 735f 636f 7272 656c  w_results_correl
+0000d250: 6174 696f 6e5f 6d61 7472 6978 2e73 6574  ation_matrix.set
+0000d260: 4f62 6a65 6374 4e61 6d65 2822 7461 626c  ObjectName("tabl
+0000d270: 6556 6965 775f 7265 7375 6c74 735f 636f  eView_results_co
+0000d280: 7272 656c 6174 696f 6e5f 6d61 7472 6978  rrelation_matrix
+0000d290: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+0000d2a0: 7665 7274 6963 616c 4c61 796f 7574 5f33  verticalLayout_3
+0000d2b0: 322e 6164 6457 6964 6765 7428 7365 6c66  2.addWidget(self
+0000d2c0: 2e74 6162 6c65 5669 6577 5f72 6573 756c  .tableView_resul
+0000d2d0: 7473 5f63 6f72 7265 6c61 7469 6f6e 5f6d  ts_correlation_m
+0000d2e0: 6174 7269 7829 0a20 2020 2020 2020 2073  atrix).        s
+0000d2f0: 656c 662e 7461 6257 6964 6765 745f 7265  elf.tabWidget_re
+0000d300: 7375 6c74 732e 6164 6454 6162 2873 656c  sults.addTab(sel
+0000d310: 662e 7461 625f 7265 7375 6c74 735f 636f  f.tab_results_co
+0000d320: 7272 656c 6174 696f 6e5f 6d61 7472 6978  rrelation_matrix
+0000d330: 2c20 2222 290a 2020 2020 2020 2020 7365  , "").        se
+0000d340: 6c66 2e74 6162 5f76 675f 7461 626c 6520  lf.tab_vg_table 
+0000d350: 3d20 5174 5769 6467 6574 732e 5157 6964  = QtWidgets.QWid
+0000d360: 6765 7428 290a 2020 2020 2020 2020 7365  get().        se
+0000d370: 6c66 2e74 6162 5f76 675f 7461 626c 652e  lf.tab_vg_table.
+0000d380: 7365 744f 626a 6563 744e 616d 6528 2274  setObjectName("t
+0000d390: 6162 5f76 675f 7461 626c 6522 290a 2020  ab_vg_table").  
+0000d3a0: 2020 2020 2020 7365 6c66 2e76 6572 7469        self.verti
+0000d3b0: 6361 6c4c 6179 6f75 745f 3333 203d 2051  calLayout_33 = Q
+0000d3c0: 7457 6964 6765 7473 2e51 5642 6f78 4c61  tWidgets.QVBoxLa
+0000d3d0: 796f 7574 2873 656c 662e 7461 625f 7667  yout(self.tab_vg
+0000d3e0: 5f74 6162 6c65 290a 2020 2020 2020 2020  _table).        
+0000d3f0: 7365 6c66 2e76 6572 7469 6361 6c4c 6179  self.verticalLay
+0000d400: 6f75 745f 3333 2e73 6574 4f62 6a65 6374  out_33.setObject
+0000d410: 4e61 6d65 2822 7665 7274 6963 616c 4c61  Name("verticalLa
+0000d420: 796f 7574 5f33 3322 290a 2020 2020 2020  yout_33").      
+0000d430: 2020 7365 6c66 2e74 6162 6c65 5669 6577    self.tableView
+0000d440: 5f72 6573 756c 7473 5f76 675f 7461 626c  _results_vg_tabl
+0000d450: 6520 3d20 5174 5769 6467 6574 732e 5154  e = QtWidgets.QT
+0000d460: 6162 6c65 5669 6577 2873 656c 662e 7461  ableView(self.ta
+0000d470: 625f 7667 5f74 6162 6c65 290a 2020 2020  b_vg_table).    
+0000d480: 2020 2020 7365 6c66 2e74 6162 6c65 5669      self.tableVi
+0000d490: 6577 5f72 6573 756c 7473 5f76 675f 7461  ew_results_vg_ta
+0000d4a0: 626c 652e 7365 744f 626a 6563 744e 616d  ble.setObjectNam
+0000d4b0: 6528 2274 6162 6c65 5669 6577 5f72 6573  e("tableView_res
+0000d4c0: 756c 7473 5f76 675f 7461 626c 6522 290a  ults_vg_table").
+0000d4d0: 2020 2020 2020 2020 7365 6c66 2e76 6572          self.ver
+0000d4e0: 7469 6361 6c4c 6179 6f75 745f 3333 2e61  ticalLayout_33.a
+0000d4f0: 6464 5769 6467 6574 2873 656c 662e 7461  ddWidget(self.ta
+0000d500: 626c 6556 6965 775f 7265 7375 6c74 735f  bleView_results_
+0000d510: 7667 5f74 6162 6c65 290a 2020 2020 2020  vg_table).      
+0000d520: 2020 7365 6c66 2e74 6162 5769 6467 6574    self.tabWidget
+0000d530: 5f72 6573 756c 7473 2e61 6464 5461 6228  _results.addTab(
+0000d540: 7365 6c66 2e74 6162 5f76 675f 7461 626c  self.tab_vg_tabl
+0000d550: 652c 2022 2229 0a20 2020 2020 2020 2073  e, "").        s
+0000d560: 656c 662e 7461 625f 7667 5f70 6c6f 7420  elf.tab_vg_plot 
+0000d570: 3d20 5174 5769 6467 6574 732e 5157 6964  = QtWidgets.QWid
+0000d580: 6765 7428 290a 2020 2020 2020 2020 7365  get().        se
+0000d590: 6c66 2e74 6162 5f76 675f 706c 6f74 2e73  lf.tab_vg_plot.s
+0000d5a0: 6574 4f62 6a65 6374 4e61 6d65 2822 7461  etObjectName("ta
+0000d5b0: 625f 7667 5f70 6c6f 7422 290a 2020 2020  b_vg_plot").    
+0000d5c0: 2020 2020 7365 6c66 2e76 6572 7469 6361      self.vertica
+0000d5d0: 6c4c 6179 6f75 745f 3335 203d 2051 7457  lLayout_35 = QtW
+0000d5e0: 6964 6765 7473 2e51 5642 6f78 4c61 796f  idgets.QVBoxLayo
+0000d5f0: 7574 2873 656c 662e 7461 625f 7667 5f70  ut(self.tab_vg_p
+0000d600: 6c6f 7429 0a20 2020 2020 2020 2073 656c  lot).        sel
+0000d610: 662e 7665 7274 6963 616c 4c61 796f 7574  f.verticalLayout
+0000d620: 5f33 352e 7365 744f 626a 6563 744e 616d  _35.setObjectNam
+0000d630: 6528 2276 6572 7469 6361 6c4c 6179 6f75  e("verticalLayou
+0000d640: 745f 3335 2229 0a20 2020 2020 2020 2073  t_35").        s
+0000d650: 656c 662e 6772 6170 6869 6373 4c61 796f  elf.graphicsLayo
+0000d660: 7574 5769 6467 6574 5f72 6573 756c 7473  utWidget_results
+0000d670: 5f76 675f 706c 6f74 203d 2047 7261 7068  _vg_plot = Graph
+0000d680: 6963 734c 6179 6f75 7457 6964 6765 7428  icsLayoutWidget(
+0000d690: 7365 6c66 2e74 6162 5f76 675f 706c 6f74  self.tab_vg_plot
+0000d6a0: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
+0000d6b0: 7261 7068 6963 734c 6179 6f75 7457 6964  raphicsLayoutWid
+0000d6c0: 6765 745f 7265 7375 6c74 735f 7667 5f70  get_results_vg_p
+0000d6d0: 6c6f 742e 7365 744f 626a 6563 744e 616d  lot.setObjectNam
+0000d6e0: 6528 2267 7261 7068 6963 734c 6179 6f75  e("graphicsLayou
+0000d6f0: 7457 6964 6765 745f 7265 7375 6c74 735f  tWidget_results_
+0000d700: 7667 5f70 6c6f 7422 290a 2020 2020 2020  vg_plot").      
+0000d710: 2020 7365 6c66 2e76 6572 7469 6361 6c4c    self.verticalL
+0000d720: 6179 6f75 745f 3335 2e61 6464 5769 6467  ayout_35.addWidg
+0000d730: 6574 2873 656c 662e 6772 6170 6869 6373  et(self.graphics
+0000d740: 4c61 796f 7574 5769 6467 6574 5f72 6573  LayoutWidget_res
+0000d750: 756c 7473 5f76 675f 706c 6f74 290a 2020  ults_vg_plot).  
+0000d760: 2020 2020 2020 7365 6c66 2e67 726f 7570        self.group
+0000d770: 426f 785f 7265 7375 6c74 735f 7667 5f70  Box_results_vg_p
+0000d780: 6c6f 745f 7365 7474 696e 6773 203d 2051  lot_settings = Q
+0000d790: 7457 6964 6765 7473 2e51 4772 6f75 7042  tWidgets.QGroupB
+0000d7a0: 6f78 2873 656c 662e 7461 625f 7667 5f70  ox(self.tab_vg_p
+0000d7b0: 6c6f 7429 0a20 2020 2020 2020 2073 656c  lot).        sel
+0000d7c0: 662e 6772 6f75 7042 6f78 5f72 6573 756c  f.groupBox_resul
+0000d7d0: 7473 5f76 675f 706c 6f74 5f73 6574 7469  ts_vg_plot_setti
+0000d7e0: 6e67 732e 7365 744f 626a 6563 744e 616d  ngs.setObjectNam
+0000d7f0: 6528 2267 726f 7570 426f 785f 7265 7375  e("groupBox_resu
+0000d800: 6c74 735f 7667 5f70 6c6f 745f 7365 7474  lts_vg_plot_sett
+0000d810: 696e 6773 2229 0a20 2020 2020 2020 2073  ings").        s
+0000d820: 656c 662e 7665 7274 6963 616c 4c61 796f  elf.verticalLayo
+0000d830: 7574 5f33 3420 3d20 5174 5769 6467 6574  ut_34 = QtWidget
+0000d840: 732e 5156 426f 784c 6179 6f75 7428 7365  s.QVBoxLayout(se
+0000d850: 6c66 2e67 726f 7570 426f 785f 7265 7375  lf.groupBox_resu
+0000d860: 6c74 735f 7667 5f70 6c6f 745f 7365 7474  lts_vg_plot_sett
+0000d870: 696e 6773 290a 2020 2020 2020 2020 7365  ings).        se
+0000d880: 6c66 2e76 6572 7469 6361 6c4c 6179 6f75  lf.verticalLayou
+0000d890: 745f 3334 2e73 6574 4f62 6a65 6374 4e61  t_34.setObjectNa
+0000d8a0: 6d65 2822 7665 7274 6963 616c 4c61 796f  me("verticalLayo
+0000d8b0: 7574 5f33 3422 290a 2020 2020 2020 2020  ut_34").        
+0000d8c0: 7365 6c66 2e63 6865 636b 426f 785f 7265  self.checkBox_re
+0000d8d0: 7375 6c74 735f 7667 5f70 6c6f 745f 7368  sults_vg_plot_sh
+0000d8e0: 6f77 5f72 6573 6964 7561 6c73 203d 2051  ow_residuals = Q
+0000d8f0: 7457 6964 6765 7473 2e51 4368 6563 6b42  tWidgets.QCheckB
+0000d900: 6f78 2873 656c 662e 6772 6f75 7042 6f78  ox(self.groupBox
+0000d910: 5f72 6573 756c 7473 5f76 675f 706c 6f74  _results_vg_plot
+0000d920: 5f73 6574 7469 6e67 7329 0a20 2020 2020  _settings).     
+0000d930: 2020 2073 656c 662e 6368 6563 6b42 6f78     self.checkBox
+0000d940: 5f72 6573 756c 7473 5f76 675f 706c 6f74  _results_vg_plot
+0000d950: 5f73 686f 775f 7265 7369 6475 616c 732e  _show_residuals.
+0000d960: 7365 7443 6865 636b 6564 2854 7275 6529  setChecked(True)
+0000d970: 0a20 2020 2020 2020 2073 656c 662e 6368  .        self.ch
+0000d980: 6563 6b42 6f78 5f72 6573 756c 7473 5f76  eckBox_results_v
+0000d990: 675f 706c 6f74 5f73 686f 775f 7265 7369  g_plot_show_resi
+0000d9a0: 6475 616c 732e 7365 744f 626a 6563 744e  duals.setObjectN
+0000d9b0: 616d 6528 2263 6865 636b 426f 785f 7265  ame("checkBox_re
+0000d9c0: 7375 6c74 735f 7667 5f70 6c6f 745f 7368  sults_vg_plot_sh
+0000d9d0: 6f77 5f72 6573 6964 7561 6c73 2229 0a20  ow_residuals"). 
+0000d9e0: 2020 2020 2020 2073 656c 662e 7665 7274         self.vert
+0000d9f0: 6963 616c 4c61 796f 7574 5f33 342e 6164  icalLayout_34.ad
+0000da00: 6457 6964 6765 7428 7365 6c66 2e63 6865  dWidget(self.che
+0000da10: 636b 426f 785f 7265 7375 6c74 735f 7667  ckBox_results_vg
+0000da20: 5f70 6c6f 745f 7368 6f77 5f72 6573 6964  _plot_show_resid
+0000da30: 7561 6c73 290a 2020 2020 2020 2020 7365  uals).        se
+0000da40: 6c66 2e72 6164 696f 4275 7474 6f6e 5f72  lf.radioButton_r
+0000da50: 6573 756c 7473 5f76 675f 706c 6f74 5f64  esults_vg_plot_d
+0000da60: 6574 6169 6c73 203d 2051 7457 6964 6765  etails = QtWidge
+0000da70: 7473 2e51 5261 6469 6f42 7574 746f 6e28  ts.QRadioButton(
+0000da80: 7365 6c66 2e67 726f 7570 426f 785f 7265  self.groupBox_re
+0000da90: 7375 6c74 735f 7667 5f70 6c6f 745f 7365  sults_vg_plot_se
+0000daa0: 7474 696e 6773 290a 2020 2020 2020 2020  ttings).        
+0000dab0: 7365 6c66 2e72 6164 696f 4275 7474 6f6e  self.radioButton
+0000dac0: 5f72 6573 756c 7473 5f76 675f 706c 6f74  _results_vg_plot
+0000dad0: 5f64 6574 6169 6c73 2e73 6574 4368 6563  _details.setChec
+0000dae0: 6b65 6428 5472 7565 290a 2020 2020 2020  ked(True).      
+0000daf0: 2020 7365 6c66 2e72 6164 696f 4275 7474    self.radioButt
+0000db00: 6f6e 5f72 6573 756c 7473 5f76 675f 706c  on_results_vg_pl
+0000db10: 6f74 5f64 6574 6169 6c73 2e73 6574 4f62  ot_details.setOb
+0000db20: 6a65 6374 4e61 6d65 2822 7261 6469 6f42  jectName("radioB
+0000db30: 7574 746f 6e5f 7265 7375 6c74 735f 7667  utton_results_vg
+0000db40: 5f70 6c6f 745f 6465 7461 696c 7322 290a  _plot_details").
+0000db50: 2020 2020 2020 2020 7365 6c66 2e62 7574          self.but
+0000db60: 746f 6e47 726f 7570 5f72 6573 756c 7473  tonGroup_results
+0000db70: 5f76 675f 706c 6f74 5f74 7970 655f 7365  _vg_plot_type_se
+0000db80: 6c65 6374 696f 6e20 3d20 5174 5769 6467  lection = QtWidg
+0000db90: 6574 732e 5142 7574 746f 6e47 726f 7570  ets.QButtonGroup
+0000dba0: 284d 6169 6e57 696e 646f 7729 0a20 2020  (MainWindow).   
+0000dbb0: 2020 2020 2073 656c 662e 6275 7474 6f6e       self.button
+0000dbc0: 4772 6f75 705f 7265 7375 6c74 735f 7667  Group_results_vg
+0000dbd0: 5f70 6c6f 745f 7479 7065 5f73 656c 6563  _plot_type_selec
+0000dbe0: 7469 6f6e 2e73 6574 4f62 6a65 6374 4e61  tion.setObjectNa
+0000dbf0: 6d65 2822 6275 7474 6f6e 4772 6f75 705f  me("buttonGroup_
+0000dc00: 7265 7375 6c74 735f 7667 5f70 6c6f 745f  results_vg_plot_
+0000dc10: 7479 7065 5f73 656c 6563 7469 6f6e 2229  type_selection")
+0000dc20: 0a20 2020 2020 2020 2073 656c 662e 6275  .        self.bu
+0000dc30: 7474 6f6e 4772 6f75 705f 7265 7375 6c74  ttonGroup_result
+0000dc40: 735f 7667 5f70 6c6f 745f 7479 7065 5f73  s_vg_plot_type_s
+0000dc50: 656c 6563 7469 6f6e 2e61 6464 4275 7474  election.addButt
+0000dc60: 6f6e 2873 656c 662e 7261 6469 6f42 7574  on(self.radioBut
+0000dc70: 746f 6e5f 7265 7375 6c74 735f 7667 5f70  ton_results_vg_p
+0000dc80: 6c6f 745f 6465 7461 696c 7329 0a20 2020  lot_details).   
+0000dc90: 2020 2020 2073 656c 662e 7665 7274 6963       self.vertic
+0000dca0: 616c 4c61 796f 7574 5f33 342e 6164 6457  alLayout_34.addW
+0000dcb0: 6964 6765 7428 7365 6c66 2e72 6164 696f  idget(self.radio
+0000dcc0: 4275 7474 6f6e 5f72 6573 756c 7473 5f76  Button_results_v
+0000dcd0: 675f 706c 6f74 5f64 6574 6169 6c73 290a  g_plot_details).
+0000dce0: 2020 2020 2020 2020 7365 6c66 2e72 6164          self.rad
+0000dcf0: 696f 4275 7474 6f6e 5f72 6573 756c 7473  ioButton_results
+0000dd00: 5f76 675f 706c 6f74 5f66 756c 6c5f 706f  _vg_plot_full_po
+0000dd10: 6c79 6e6f 6d69 616c 203d 2051 7457 6964  lynomial = QtWid
+0000dd20: 6765 7473 2e51 5261 6469 6f42 7574 746f  gets.QRadioButto
+0000dd30: 6e28 7365 6c66 2e67 726f 7570 426f 785f  n(self.groupBox_
+0000dd40: 7265 7375 6c74 735f 7667 5f70 6c6f 745f  results_vg_plot_
+0000dd50: 7365 7474 696e 6773 290a 2020 2020 2020  settings).      
+0000dd60: 2020 7365 6c66 2e72 6164 696f 4275 7474    self.radioButt
+0000dd70: 6f6e 5f72 6573 756c 7473 5f76 675f 706c  on_results_vg_pl
+0000dd80: 6f74 5f66 756c 6c5f 706f 6c79 6e6f 6d69  ot_full_polynomi
+0000dd90: 616c 2e73 6574 4f62 6a65 6374 4e61 6d65  al.setObjectName
+0000dda0: 2822 7261 6469 6f42 7574 746f 6e5f 7265  ("radioButton_re
+0000ddb0: 7375 6c74 735f 7667 5f70 6c6f 745f 6675  sults_vg_plot_fu
+0000ddc0: 6c6c 5f70 6f6c 796e 6f6d 6961 6c22 290a  ll_polynomial").
+0000ddd0: 2020 2020 2020 2020 7365 6c66 2e62 7574          self.but
+0000dde0: 746f 6e47 726f 7570 5f72 6573 756c 7473  tonGroup_results
+0000ddf0: 5f76 675f 706c 6f74 5f74 7970 655f 7365  _vg_plot_type_se
+0000de00: 6c65 6374 696f 6e2e 6164 6442 7574 746f  lection.addButto
+0000de10: 6e28 7365 6c66 2e72 6164 696f 4275 7474  n(self.radioButt
+0000de20: 6f6e 5f72 6573 756c 7473 5f76 675f 706c  on_results_vg_pl
+0000de30: 6f74 5f66 756c 6c5f 706f 6c79 6e6f 6d69  ot_full_polynomi
+0000de40: 616c 290a 2020 2020 2020 2020 7365 6c66  al).        self
+0000de50: 2e76 6572 7469 6361 6c4c 6179 6f75 745f  .verticalLayout_
+0000de60: 3334 2e61 6464 5769 6467 6574 2873 656c  34.addWidget(sel
+0000de70: 662e 7261 6469 6f42 7574 746f 6e5f 7265  f.radioButton_re
+0000de80: 7375 6c74 735f 7667 5f70 6c6f 745f 6675  sults_vg_plot_fu
+0000de90: 6c6c 5f70 6f6c 796e 6f6d 6961 6c29 0a20  ll_polynomial). 
+0000dea0: 2020 2020 2020 2073 656c 662e 7665 7274         self.vert
+0000deb0: 6963 616c 4c61 796f 7574 5f33 352e 6164  icalLayout_35.ad
+0000dec0: 6457 6964 6765 7428 7365 6c66 2e67 726f  dWidget(self.gro
+0000ded0: 7570 426f 785f 7265 7375 6c74 735f 7667  upBox_results_vg
+0000dee0: 5f70 6c6f 745f 7365 7474 696e 6773 290a  _plot_settings).
+0000def0: 2020 2020 2020 2020 7365 6c66 2e74 6162          self.tab
+0000df00: 5769 6467 6574 5f72 6573 756c 7473 2e61  Widget_results.a
+0000df10: 6464 5461 6228 7365 6c66 2e74 6162 5f76  ddTab(self.tab_v
+0000df20: 675f 706c 6f74 2c20 2222 290a 2020 2020  g_plot, "").    
+0000df30: 2020 2020 7365 6c66 2e76 6572 7469 6361      self.vertica
+0000df40: 6c4c 6179 6f75 745f 3134 2e61 6464 5769  lLayout_14.addWi
+0000df50: 6467 6574 2873 656c 662e 7370 6c69 7474  dget(self.splitt
+0000df60: 6572 5f72 6573 756c 7473 290a 2020 2020  er_results).    
+0000df70: 2020 2020 7365 6c66 2e74 6162 5769 6467      self.tabWidg
+0000df80: 6574 5f4d 6169 6e2e 6164 6454 6162 2873  et_Main.addTab(s
+0000df90: 656c 662e 7461 625f 6d61 696e 5f72 6573  elf.tab_main_res
+0000dfa0: 756c 7473 2c20 2222 290a 2020 2020 2020  ults, "").      
+0000dfb0: 2020 7365 6c66 2e76 6572 7469 6361 6c4c    self.verticalL
+0000dfc0: 6179 6f75 745f 3337 2e61 6464 5769 6467  ayout_37.addWidg
+0000dfd0: 6574 2873 656c 662e 7461 6257 6964 6765  et(self.tabWidge
+0000dfe0: 745f 4d61 696e 290a 2020 2020 2020 2020  t_Main).        
+0000dff0: 4d61 696e 5769 6e64 6f77 2e73 6574 4365  MainWindow.setCe
+0000e000: 6e74 7261 6c57 6964 6765 7428 7365 6c66  ntralWidget(self
+0000e010: 2e63 656e 7472 616c 7769 6467 6574 290a  .centralwidget).
+0000e020: 2020 2020 2020 2020 7365 6c66 2e6d 656e          self.men
+0000e030: 7562 6172 203d 2051 7457 6964 6765 7473  ubar = QtWidgets
+0000e040: 2e51 4d65 6e75 4261 7228 4d61 696e 5769  .QMenuBar(MainWi
+0000e050: 6e64 6f77 290a 2020 2020 2020 2020 7365  ndow).        se
+0000e060: 6c66 2e6d 656e 7562 6172 2e73 6574 4765  lf.menubar.setGe
+0000e070: 6f6d 6574 7279 2851 7443 6f72 652e 5152  ometry(QtCore.QR
+0000e080: 6563 7428 302c 2030 2c20 3133 3337 2c20  ect(0, 0, 1337, 
+0000e090: 3232 2929 0a20 2020 2020 2020 2073 656c  22)).        sel
+0000e0a0: 662e 6d65 6e75 6261 722e 7365 744f 626a  f.menubar.setObj
+0000e0b0: 6563 744e 616d 6528 226d 656e 7562 6172  ectName("menubar
+0000e0c0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+0000e0d0: 6d65 6e75 5f46 696c 6520 3d20 5174 5769  menu_File = QtWi
+0000e0e0: 6467 6574 732e 514d 656e 7528 7365 6c66  dgets.QMenu(self
+0000e0f0: 2e6d 656e 7562 6172 290a 2020 2020 2020  .menubar).      
+0000e100: 2020 7365 6c66 2e6d 656e 755f 4669 6c65    self.menu_File
+0000e110: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
+0000e120: 6d65 6e75 5f46 696c 6522 290a 2020 2020  menu_File").    
+0000e130: 2020 2020 7365 6c66 2e6d 656e 7541 6464      self.menuAdd
+0000e140: 5f53 7572 7665 7920 3d20 5174 5769 6467  _Survey = QtWidg
+0000e150: 6574 732e 514d 656e 7528 7365 6c66 2e6d  ets.QMenu(self.m
+0000e160: 656e 755f 4669 6c65 290a 2020 2020 2020  enu_File).      
+0000e170: 2020 7365 6c66 2e6d 656e 7541 6464 5f53    self.menuAdd_S
+0000e180: 7572 7665 792e 7365 7445 6e61 626c 6564  urvey.setEnabled
+0000e190: 2846 616c 7365 290a 2020 2020 2020 2020  (False).        
+0000e1a0: 7365 6c66 2e6d 656e 7541 6464 5f53 7572  self.menuAdd_Sur
+0000e1b0: 7665 792e 7365 744f 626a 6563 744e 616d  vey.setObjectNam
+0000e1c0: 6528 226d 656e 7541 6464 5f53 7572 7665  e("menuAdd_Surve
+0000e1d0: 7922 290a 2020 2020 2020 2020 7365 6c66  y").        self
+0000e1e0: 2e6d 656e 755f 4164 645f 5374 6174 696f  .menu_Add_Statio
+0000e1f0: 6e73 203d 2051 7457 6964 6765 7473 2e51  ns = QtWidgets.Q
+0000e200: 4d65 6e75 2873 656c 662e 6d65 6e75 5f46  Menu(self.menu_F
+0000e210: 696c 6529 0a20 2020 2020 2020 2073 656c  ile).        sel
+0000e220: 662e 6d65 6e75 5f41 6464 5f53 7461 7469  f.menu_Add_Stati
+0000e230: 6f6e 732e 7365 7445 6e61 626c 6564 2846  ons.setEnabled(F
+0000e240: 616c 7365 290a 2020 2020 2020 2020 7365  alse).        se
+0000e250: 6c66 2e6d 656e 755f 4164 645f 5374 6174  lf.menu_Add_Stat
+0000e260: 696f 6e73 2e73 6574 4f62 6a65 6374 4e61  ions.setObjectNa
+0000e270: 6d65 2822 6d65 6e75 5f41 6464 5f53 7461  me("menu_Add_Sta
+0000e280: 7469 6f6e 7322 290a 2020 2020 2020 2020  tions").        
+0000e290: 7365 6c66 2e6d 656e 755f 4164 645f 4772  self.menu_Add_Gr
+0000e2a0: 6176 696d 6574 6572 7320 3d20 5174 5769  avimeters = QtWi
+0000e2b0: 6467 6574 732e 514d 656e 7528 7365 6c66  dgets.QMenu(self
+0000e2c0: 2e6d 656e 755f 4669 6c65 290a 2020 2020  .menu_File).    
+0000e2d0: 2020 2020 7365 6c66 2e6d 656e 755f 4164      self.menu_Ad
+0000e2e0: 645f 4772 6176 696d 6574 6572 732e 7365  d_Gravimeters.se
+0000e2f0: 7445 6e61 626c 6564 2846 616c 7365 290a  tEnabled(False).
+0000e300: 2020 2020 2020 2020 7365 6c66 2e6d 656e          self.men
+0000e310: 755f 4164 645f 4772 6176 696d 6574 6572  u_Add_Gravimeter
+0000e320: 732e 7365 744f 626a 6563 744e 616d 6528  s.setObjectName(
+0000e330: 226d 656e 755f 4164 645f 4772 6176 696d  "menu_Add_Gravim
+0000e340: 6574 6572 7322 290a 2020 2020 2020 2020  eters").        
+0000e350: 7365 6c66 2e6d 656e 755f 4f62 7365 7276  self.menu_Observ
+0000e360: 6174 696f 6e73 203d 2051 7457 6964 6765  ations = QtWidge
+0000e370: 7473 2e51 4d65 6e75 2873 656c 662e 6d65  ts.QMenu(self.me
+0000e380: 6e75 6261 7229 0a20 2020 2020 2020 2073  nubar).        s
+0000e390: 656c 662e 6d65 6e75 5f4f 6273 6572 7661  elf.menu_Observa
+0000e3a0: 7469 6f6e 732e 7365 7445 6e61 626c 6564  tions.setEnabled
+0000e3b0: 2846 616c 7365 290a 2020 2020 2020 2020  (False).        
+0000e3c0: 7365 6c66 2e6d 656e 755f 4f62 7365 7276  self.menu_Observ
+0000e3d0: 6174 696f 6e73 2e73 6574 5465 6172 4f66  ations.setTearOf
+0000e3e0: 6645 6e61 626c 6564 2846 616c 7365 290a  fEnabled(False).
+0000e3f0: 2020 2020 2020 2020 7365 6c66 2e6d 656e          self.men
+0000e400: 755f 4f62 7365 7276 6174 696f 6e73 2e73  u_Observations.s
+0000e410: 6574 4f62 6a65 6374 4e61 6d65 2822 6d65  etObjectName("me
+0000e420: 6e75 5f4f 6273 6572 7661 7469 6f6e 7322  nu_Observations"
+0000e430: 290a 2020 2020 2020 2020 7365 6c66 2e6d  ).        self.m
+0000e440: 656e 7545 7374 696d 6174 696f 6e5f 7365  enuEstimation_se
+0000e450: 7474 696e 6773 203d 2051 7457 6964 6765  ttings = QtWidge
+0000e460: 7473 2e51 4d65 6e75 2873 656c 662e 6d65  ts.QMenu(self.me
+0000e470: 6e75 6261 7229 0a20 2020 2020 2020 2073  nubar).        s
+0000e480: 656c 662e 6d65 6e75 4573 7469 6d61 7469  elf.menuEstimati
+0000e490: 6f6e 5f73 6574 7469 6e67 732e 7365 7445  on_settings.setE
+0000e4a0: 6e61 626c 6564 2854 7275 6529 0a20 2020  nabled(True).   
+0000e4b0: 2020 2020 2073 656c 662e 6d65 6e75 4573       self.menuEs
+0000e4c0: 7469 6d61 7469 6f6e 5f73 6574 7469 6e67  timation_setting
+0000e4d0: 732e 7365 744f 626a 6563 744e 616d 6528  s.setObjectName(
+0000e4e0: 226d 656e 7545 7374 696d 6174 696f 6e5f  "menuEstimation_
+0000e4f0: 7365 7474 696e 6773 2229 0a20 2020 2020  settings").     
+0000e500: 2020 2073 656c 662e 6d65 6e75 4865 6c70     self.menuHelp
+0000e510: 203d 2051 7457 6964 6765 7473 2e51 4d65   = QtWidgets.QMe
+0000e520: 6e75 2873 656c 662e 6d65 6e75 6261 7229  nu(self.menubar)
+0000e530: 0a20 2020 2020 2020 2073 656c 662e 6d65  .        self.me
+0000e540: 6e75 4865 6c70 2e73 6574 4f62 6a65 6374  nuHelp.setObject
+0000e550: 4e61 6d65 2822 6d65 6e75 4865 6c70 2229  Name("menuHelp")
+0000e560: 0a20 2020 2020 2020 2073 656c 662e 6d65  .        self.me
+0000e570: 6e75 436f 7272 6563 7469 6f6e 7320 3d20  nuCorrections = 
+0000e580: 5174 5769 6467 6574 732e 514d 656e 7528  QtWidgets.QMenu(
+0000e590: 7365 6c66 2e6d 656e 7562 6172 290a 2020  self.menubar).  
+0000e5a0: 2020 2020 2020 7365 6c66 2e6d 656e 7543        self.menuC
+0000e5b0: 6f72 7265 6374 696f 6e73 2e73 6574 4f62  orrections.setOb
+0000e5c0: 6a65 6374 4e61 6d65 2822 6d65 6e75 436f  jectName("menuCo
+0000e5d0: 7272 6563 7469 6f6e 7322 290a 2020 2020  rrections").    
+0000e5e0: 2020 2020 4d61 696e 5769 6e64 6f77 2e73      MainWindow.s
+0000e5f0: 6574 4d65 6e75 4261 7228 7365 6c66 2e6d  etMenuBar(self.m
+0000e600: 656e 7562 6172 290a 2020 2020 2020 2020  enubar).        
+0000e610: 7365 6c66 2e73 7461 7475 7362 6172 203d  self.statusbar =
+0000e620: 2051 7457 6964 6765 7473 2e51 5374 6174   QtWidgets.QStat
+0000e630: 7573 4261 7228 4d61 696e 5769 6e64 6f77  usBar(MainWindow
+0000e640: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000e650: 7461 7475 7362 6172 2e73 6574 496e 7075  tatusbar.setInpu
+0000e660: 744d 6574 686f 6448 696e 7473 2851 7443  tMethodHints(QtC
+0000e670: 6f72 652e 5174 2e49 6d68 4e6f 6e65 290a  ore.Qt.ImhNone).
+0000e680: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+0000e690: 7475 7362 6172 2e73 6574 4f62 6a65 6374  tusbar.setObject
+0000e6a0: 4e61 6d65 2822 7374 6174 7573 6261 7222  Name("statusbar"
+0000e6b0: 290a 2020 2020 2020 2020 4d61 696e 5769  ).        MainWi
+0000e6c0: 6e64 6f77 2e73 6574 5374 6174 7573 4261  ndow.setStatusBa
+0000e6d0: 7228 7365 6c66 2e73 7461 7475 7362 6172  r(self.statusbar
+0000e6e0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+0000e6f0: 6374 696f 6e5f 4e65 775f 4361 6d70 6169  ction_New_Campai
+0000e700: 676e 203d 2051 7457 6964 6765 7473 2e51  gn = QtWidgets.Q
+0000e710: 4163 7469 6f6e 284d 6169 6e57 696e 646f  Action(MainWindo
+0000e720: 7729 0a20 2020 2020 2020 2073 656c 662e  w).        self.
+0000e730: 6163 7469 6f6e 5f4e 6577 5f43 616d 7061  action_New_Campa
+0000e740: 6967 6e2e 7365 744f 626a 6563 744e 616d  ign.setObjectNam
+0000e750: 6528 2261 6374 696f 6e5f 4e65 775f 4361  e("action_New_Ca
+0000e760: 6d70 6169 676e 2229 0a20 2020 2020 2020  mpaign").       
+0000e770: 2073 656c 662e 6163 7469 6f6e 5f53 6176   self.action_Sav
+0000e780: 655f 4361 6d70 6169 676e 203d 2051 7457  e_Campaign = QtW
+0000e790: 6964 6765 7473 2e51 4163 7469 6f6e 284d  idgets.QAction(M
+0000e7a0: 6169 6e57 696e 646f 7729 0a20 2020 2020  ainWindow).     
+0000e7b0: 2020 2073 656c 662e 6163 7469 6f6e 5f53     self.action_S
+0000e7c0: 6176 655f 4361 6d70 6169 676e 2e73 6574  ave_Campaign.set
+0000e7d0: 456e 6162 6c65 6428 4661 6c73 6529 0a20  Enabled(False). 
+0000e7e0: 2020 2020 2020 2073 656c 662e 6163 7469         self.acti
+0000e7f0: 6f6e 5f53 6176 655f 4361 6d70 6169 676e  on_Save_Campaign
+0000e800: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
+0000e810: 6163 7469 6f6e 5f53 6176 655f 4361 6d70  action_Save_Camp
+0000e820: 6169 676e 2229 0a20 2020 2020 2020 2073  aign").        s
+0000e830: 656c 662e 6163 7469 6f6e 5f4c 6f61 645f  elf.action_Load_
+0000e840: 4361 6d70 6169 676e 203d 2051 7457 6964  Campaign = QtWid
+0000e850: 6765 7473 2e51 4163 7469 6f6e 284d 6169  gets.QAction(Mai
+0000e860: 6e57 696e 646f 7729 0a20 2020 2020 2020  nWindow).       
+0000e870: 2073 656c 662e 6163 7469 6f6e 5f4c 6f61   self.action_Loa
+0000e880: 645f 4361 6d70 6169 676e 2e73 6574 456e  d_Campaign.setEn
+0000e890: 6162 6c65 6428 5472 7565 290a 2020 2020  abled(True).    
+0000e8a0: 2020 2020 7365 6c66 2e61 6374 696f 6e5f      self.action_
+0000e8b0: 4c6f 6164 5f43 616d 7061 6967 6e2e 7365  Load_Campaign.se
+0000e8c0: 744f 626a 6563 744e 616d 6528 2261 6374  tObjectName("act
+0000e8d0: 696f 6e5f 4c6f 6164 5f43 616d 7061 6967  ion_Load_Campaig
+0000e8e0: 6e22 290a 2020 2020 2020 2020 7365 6c66  n").        self
+0000e8f0: 2e61 6374 696f 6e5f 4164 645f 5374 6174  .action_Add_Stat
+0000e900: 696f 6e73 203d 2051 7457 6964 6765 7473  ions = QtWidgets
+0000e910: 2e51 4163 7469 6f6e 284d 6169 6e57 696e  .QAction(MainWin
+0000e920: 646f 7729 0a20 2020 2020 2020 2073 656c  dow).        sel
+0000e930: 662e 6163 7469 6f6e 5f41 6464 5f53 7461  f.action_Add_Sta
+0000e940: 7469 6f6e 732e 7365 7445 6e61 626c 6564  tions.setEnabled
+0000e950: 2846 616c 7365 290a 2020 2020 2020 2020  (False).        
+0000e960: 7365 6c66 2e61 6374 696f 6e5f 4164 645f  self.action_Add_
+0000e970: 5374 6174 696f 6e73 2e73 6574 4f62 6a65  Stations.setObje
+0000e980: 6374 4e61 6d65 2822 6163 7469 6f6e 5f41  ctName("action_A
+0000e990: 6464 5f53 7461 7469 6f6e 7322 290a 2020  dd_Stations").  
+0000e9a0: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
+0000e9b0: 6e5f 4578 6974 203d 2051 7457 6964 6765  n_Exit = QtWidge
+0000e9c0: 7473 2e51 4163 7469 6f6e 284d 6169 6e57  ts.QAction(MainW
+0000e9d0: 696e 646f 7729 0a20 2020 2020 2020 2073  indow).        s
+0000e9e0: 656c 662e 6163 7469 6f6e 5f45 7869 742e  elf.action_Exit.
+0000e9f0: 7365 744f 626a 6563 744e 616d 6528 2261  setObjectName("a
+0000ea00: 6374 696f 6e5f 4578 6974 2229 0a20 2020  ction_Exit").   
+0000ea10: 2020 2020 2073 656c 662e 6163 7469 6f6e       self.action
+0000ea20: 5f45 6469 745f 4f62 7365 7276 6174 696f  _Edit_Observatio
+0000ea30: 6e73 203d 2051 7457 6964 6765 7473 2e51  ns = QtWidgets.Q
+0000ea40: 4163 7469 6f6e 284d 6169 6e57 696e 646f  Action(MainWindo
+0000ea50: 7729 0a20 2020 2020 2020 2073 656c 662e  w).        self.
+0000ea60: 6163 7469 6f6e 5f45 6469 745f 4f62 7365  action_Edit_Obse
+0000ea70: 7276 6174 696f 6e73 2e73 6574 456e 6162  rvations.setEnab
+0000ea80: 6c65 6428 5472 7565 290a 2020 2020 2020  led(True).      
+0000ea90: 2020 7365 6c66 2e61 6374 696f 6e5f 4564    self.action_Ed
+0000eaa0: 6974 5f4f 6273 6572 7661 7469 6f6e 732e  it_Observations.
+0000eab0: 7365 744f 626a 6563 744e 616d 6528 2261  setObjectName("a
+0000eac0: 6374 696f 6e5f 4564 6974 5f4f 6273 6572  ction_Edit_Obser
+0000ead0: 7661 7469 6f6e 7322 290a 2020 2020 2020  vations").      
+0000eae0: 2020 7365 6c66 2e61 6374 696f 6e52 6573    self.actionRes
+0000eaf0: 6964 7561 6c73 203d 2051 7457 6964 6765  iduals = QtWidge
+0000eb00: 7473 2e51 4163 7469 6f6e 284d 6169 6e57  ts.QAction(MainW
+0000eb10: 696e 646f 7729 0a20 2020 2020 2020 2073  indow).        s
+0000eb20: 656c 662e 6163 7469 6f6e 5265 7369 6475  elf.actionResidu
+0000eb30: 616c 732e 7365 744f 626a 6563 744e 616d  als.setObjectNam
+0000eb40: 6528 2261 6374 696f 6e52 6573 6964 7561  e("actionResidua
+0000eb50: 6c73 2229 0a20 2020 2020 2020 2073 656c  ls").        sel
+0000eb60: 662e 6163 7469 6f6e 4573 7469 6d61 7465  f.actionEstimate
+0000eb70: 7320 3d20 5174 5769 6467 6574 732e 5141  s = QtWidgets.QA
+0000eb80: 6374 696f 6e28 4d61 696e 5769 6e64 6f77  ction(MainWindow
+0000eb90: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+0000eba0: 6374 696f 6e45 7374 696d 6174 6573 2e73  ctionEstimates.s
+0000ebb0: 6574 4f62 6a65 6374 4e61 6d65 2822 6163  etObjectName("ac
+0000ebc0: 7469 6f6e 4573 7469 6d61 7465 7322 290a  tionEstimates").
+0000ebd0: 2020 2020 2020 2020 7365 6c66 2e61 6374          self.act
+0000ebe0: 696f 6e5f 436f 7272 6563 7469 6f6e 7320  ion_Corrections 
+0000ebf0: 3d20 5174 5769 6467 6574 732e 5141 6374  = QtWidgets.QAct
+0000ec00: 696f 6e28 4d61 696e 5769 6e64 6f77 290a  ion(MainWindow).
+0000ec10: 2020 2020 2020 2020 7365 6c66 2e61 6374          self.act
+0000ec20: 696f 6e5f 436f 7272 6563 7469 6f6e 732e  ion_Corrections.
+0000ec30: 7365 7445 6e61 626c 6564 2854 7275 6529  setEnabled(True)
+0000ec40: 0a20 2020 2020 2020 2073 656c 662e 6163  .        self.ac
+0000ec50: 7469 6f6e 5f43 6f72 7265 6374 696f 6e73  tion_Corrections
+0000ec60: 2e73 6574 4f62 6a65 6374 4e61 6d65 2822  .setObjectName("
+0000ec70: 6163 7469 6f6e 5f43 6f72 7265 6374 696f  action_Correctio
+0000ec80: 6e73 2229 0a20 2020 2020 2020 2073 656c  ns").        sel
+0000ec90: 662e 6163 7469 6f6e 5368 6f77 5f53 7461  f.actionShow_Sta
+0000eca0: 7469 6f6e 7320 3d20 5174 5769 6467 6574  tions = QtWidget
+0000ecb0: 732e 5141 6374 696f 6e28 4d61 696e 5769  s.QAction(MainWi
+0000ecc0: 6e64 6f77 290a 2020 2020 2020 2020 7365  ndow).        se
+0000ecd0: 6c66 2e61 6374 696f 6e53 686f 775f 5374  lf.actionShow_St
+0000ece0: 6174 696f 6e73 2e73 6574 4f62 6a65 6374  ations.setObject
+0000ecf0: 4e61 6d65 2822 6163 7469 6f6e 5368 6f77  Name("actionShow
+0000ed00: 5f53 7461 7469 6f6e 7322 290a 2020 2020  _Stations").    
+0000ed10: 2020 2020 7365 6c66 2e61 6374 696f 6e5f      self.action_
+0000ed20: 6672 6f6d 5f43 4735 5f6f 6273 6572 7661  from_CG5_observa
+0000ed30: 7469 6f6e 5f66 696c 6520 3d20 5174 5769  tion_file = QtWi
+0000ed40: 6467 6574 732e 5141 6374 696f 6e28 4d61  dgets.QAction(Ma
+0000ed50: 696e 5769 6e64 6f77 290a 2020 2020 2020  inWindow).      
+0000ed60: 2020 7365 6c66 2e61 6374 696f 6e5f 6672    self.action_fr
+0000ed70: 6f6d 5f43 4735 5f6f 6273 6572 7661 7469  om_CG5_observati
+0000ed80: 6f6e 5f66 696c 652e 7365 744f 626a 6563  on_file.setObjec
+0000ed90: 744e 616d 6528 2261 6374 696f 6e5f 6672  tName("action_fr
+0000eda0: 6f6d 5f43 4735 5f6f 6273 6572 7661 7469  om_CG5_observati
+0000edb0: 6f6e 5f66 696c 6522 290a 2020 2020 2020  on_file").      
+0000edc0: 2020 7365 6c66 2e61 6374 696f 6e5f 6672    self.action_fr
+0000edd0: 6f6d 5f42 4556 5f6f 6273 6572 7661 7469  om_BEV_observati
+0000ede0: 6f6e 5f66 696c 6520 3d20 5174 5769 6467  on_file = QtWidg
+0000edf0: 6574 732e 5141 6374 696f 6e28 4d61 696e  ets.QAction(Main
+0000ee00: 5769 6e64 6f77 290a 2020 2020 2020 2020  Window).        
+0000ee10: 7365 6c66 2e61 6374 696f 6e5f 6672 6f6d  self.action_from
+0000ee20: 5f42 4556 5f6f 6273 6572 7661 7469 6f6e  _BEV_observation
+0000ee30: 5f66 696c 652e 7365 7445 6e61 626c 6564  _file.setEnabled
+0000ee40: 2846 616c 7365 290a 2020 2020 2020 2020  (False).        
+0000ee50: 7365 6c66 2e61 6374 696f 6e5f 6672 6f6d  self.action_from
+0000ee60: 5f42 4556 5f6f 6273 6572 7661 7469 6f6e  _BEV_observation
+0000ee70: 5f66 696c 652e 7365 744f 626a 6563 744e  _file.setObjectN
+0000ee80: 616d 6528 2261 6374 696f 6e5f 6672 6f6d  ame("action_from
+0000ee90: 5f42 4556 5f6f 6273 6572 7661 7469 6f6e  _BEV_observation
+0000eea0: 5f66 696c 6522 290a 2020 2020 2020 2020  _file").        
+0000eeb0: 7365 6c66 2e61 6374 696f 6e5f 4175 746f  self.action_Auto
+0000eec0: 7365 6c65 6374 696f 6e5f 7365 7474 696e  selection_settin
+0000eed0: 6773 203d 2051 7457 6964 6765 7473 2e51  gs = QtWidgets.Q
+0000eee0: 4163 7469 6f6e 284d 6169 6e57 696e 646f  Action(MainWindo
+0000eef0: 7729 0a20 2020 2020 2020 2073 656c 662e  w).        self.
+0000ef00: 6163 7469 6f6e 5f41 7574 6f73 656c 6563  action_Autoselec
+0000ef10: 7469 6f6e 5f73 6574 7469 6e67 732e 7365  tion_settings.se
+0000ef20: 744f 626a 6563 744e 616d 6528 2261 6374  tObjectName("act
+0000ef30: 696f 6e5f 4175 746f 7365 6c65 6374 696f  ion_Autoselectio
+0000ef40: 6e5f 7365 7474 696e 6773 2229 0a20 2020  n_settings").   
+0000ef50: 2020 2020 2073 656c 662e 6163 7469 6f6e       self.action
+0000ef60: 5f45 7374 696d 6174 696f 6e5f 7365 7474  _Estimation_sett
+0000ef70: 696e 6773 203d 2051 7457 6964 6765 7473  ings = QtWidgets
+0000ef80: 2e51 4163 7469 6f6e 284d 6169 6e57 696e  .QAction(MainWin
+0000ef90: 646f 7729 0a20 2020 2020 2020 2073 656c  dow).        sel
+0000efa0: 662e 6163 7469 6f6e 5f45 7374 696d 6174  f.action_Estimat
+0000efb0: 696f 6e5f 7365 7474 696e 6773 2e73 6574  ion_settings.set
+0000efc0: 456e 6162 6c65 6428 5472 7565 290a 2020  Enabled(True).  
+0000efd0: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
+0000efe0: 6e5f 4573 7469 6d61 7469 6f6e 5f73 6574  n_Estimation_set
+0000eff0: 7469 6e67 732e 7365 744f 626a 6563 744e  tings.setObjectN
+0000f000: 616d 6528 2261 6374 696f 6e5f 4573 7469  ame("action_Esti
+0000f010: 6d61 7469 6f6e 5f73 6574 7469 6e67 7322  mation_settings"
+0000f020: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+0000f030: 6374 696f 6e45 7374 696d 6174 655f 6c6f  ctionEstimate_lo
+0000f040: 6e67 5f74 6572 6d5f 6472 6966 7420 3d20  ng_term_drift = 
+0000f050: 5174 5769 6467 6574 732e 5141 6374 696f  QtWidgets.QActio
+0000f060: 6e28 4d61 696e 5769 6e64 6f77 290a 2020  n(MainWindow).  
+0000f070: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
+0000f080: 6e45 7374 696d 6174 655f 6c6f 6e67 5f74  nEstimate_long_t
+0000f090: 6572 6d5f 6472 6966 742e 7365 7445 6e61  erm_drift.setEna
+0000f0a0: 626c 6564 2854 7275 6529 0a20 2020 2020  bled(True).     
+0000f0b0: 2020 2073 656c 662e 6163 7469 6f6e 4573     self.actionEs
+0000f0c0: 7469 6d61 7465 5f6c 6f6e 675f 7465 726d  timate_long_term
+0000f0d0: 5f64 7269 6674 2e73 6574 4f62 6a65 6374  _drift.setObject
+0000f0e0: 4e61 6d65 2822 6163 7469 6f6e 4573 7469  Name("actionEsti
+0000f0f0: 6d61 7465 5f6c 6f6e 675f 7465 726d 5f64  mate_long_term_d
+0000f100: 7269 6674 2229 0a20 2020 2020 2020 2073  rift").        s
+0000f110: 656c 662e 6163 7469 6f6e 5f45 7870 6f72  elf.action_Expor
+0000f120: 745f 5265 7375 6c74 7320 3d20 5174 5769  t_Results = QtWi
+0000f130: 6467 6574 732e 5141 6374 696f 6e28 4d61  dgets.QAction(Ma
+0000f140: 696e 5769 6e64 6f77 290a 2020 2020 2020  inWindow).      
+0000f150: 2020 7365 6c66 2e61 6374 696f 6e5f 4578    self.action_Ex
+0000f160: 706f 7274 5f52 6573 756c 7473 2e73 6574  port_Results.set
+0000f170: 456e 6162 6c65 6428 4661 6c73 6529 0a20  Enabled(False). 
+0000f180: 2020 2020 2020 2073 656c 662e 6163 7469         self.acti
+0000f190: 6f6e 5f45 7870 6f72 745f 5265 7375 6c74  on_Export_Result
+0000f1a0: 732e 7365 744f 626a 6563 744e 616d 6528  s.setObjectName(
+0000f1b0: 2261 6374 696f 6e5f 4578 706f 7274 5f52  "action_Export_R
+0000f1c0: 6573 756c 7473 2229 0a20 2020 2020 2020  esults").       
+0000f1d0: 2073 656c 662e 6163 7469 6f6e 5f43 6861   self.action_Cha
+0000f1e0: 6e67 655f 6f75 7470 7574 5f64 6972 6563  nge_output_direc
+0000f1f0: 746f 7279 203d 2051 7457 6964 6765 7473  tory = QtWidgets
+0000f200: 2e51 4163 7469 6f6e 284d 6169 6e57 696e  .QAction(MainWin
+0000f210: 646f 7729 0a20 2020 2020 2020 2073 656c  dow).        sel
+0000f220: 662e 6163 7469 6f6e 5f43 6861 6e67 655f  f.action_Change_
+0000f230: 6f75 7470 7574 5f64 6972 6563 746f 7279  output_directory
+0000f240: 2e73 6574 456e 6162 6c65 6428 4661 6c73  .setEnabled(Fals
+0000f250: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
+0000f260: 6163 7469 6f6e 5f43 6861 6e67 655f 6f75  action_Change_ou
+0000f270: 7470 7574 5f64 6972 6563 746f 7279 2e73  tput_directory.s
+0000f280: 6574 4f62 6a65 6374 4e61 6d65 2822 6163  etObjectName("ac
+0000f290: 7469 6f6e 5f43 6861 6e67 655f 6f75 7470  tion_Change_outp
+0000f2a0: 7574 5f64 6972 6563 746f 7279 2229 0a20  ut_directory"). 
+0000f2b0: 2020 2020 2020 2073 656c 662e 6163 7469         self.acti
+0000f2c0: 6f6e 5f4f 7074 696f 6e73 203d 2051 7457  on_Options = QtW
+0000f2d0: 6964 6765 7473 2e51 4163 7469 6f6e 284d  idgets.QAction(M
+0000f2e0: 6169 6e57 696e 646f 7729 0a20 2020 2020  ainWindow).     
+0000f2f0: 2020 2073 656c 662e 6163 7469 6f6e 5f4f     self.action_O
+0000f300: 7074 696f 6e73 2e73 6574 4f62 6a65 6374  ptions.setObject
+0000f310: 4e61 6d65 2822 6163 7469 6f6e 5f4f 7074  Name("action_Opt
+0000f320: 696f 6e73 2229 0a20 2020 2020 2020 2073  ions").        s
+0000f330: 656c 662e 6163 7469 6f6e 5f53 6574 7570  elf.action_Setup
+0000f340: 5f64 6174 615f 6f70 7469 6f6e 7320 3d20  _data_options = 
+0000f350: 5174 5769 6467 6574 732e 5141 6374 696f  QtWidgets.QActio
+0000f360: 6e28 4d61 696e 5769 6e64 6f77 290a 2020  n(MainWindow).  
+0000f370: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
+0000f380: 6e5f 5365 7475 705f 6461 7461 5f6f 7074  n_Setup_data_opt
+0000f390: 696f 6e73 2e73 6574 456e 6162 6c65 6428  ions.setEnabled(
+0000f3a0: 5472 7565 290a 2020 2020 2020 2020 7365  True).        se
+0000f3b0: 6c66 2e61 6374 696f 6e5f 5365 7475 705f  lf.action_Setup_
+0000f3c0: 6461 7461 5f6f 7074 696f 6e73 2e73 6574  data_options.set
+0000f3d0: 4f62 6a65 6374 4e61 6d65 2822 6163 7469  ObjectName("acti
+0000f3e0: 6f6e 5f53 6574 7570 5f64 6174 615f 6f70  on_Setup_data_op
+0000f3f0: 7469 6f6e 7322 290a 2020 2020 2020 2020  tions").        
+0000f400: 7365 6c66 2e61 6374 696f 6e5f 466c 6167  self.action_Flag
+0000f410: 5f6f 6273 6572 7661 7469 6f6e 7320 3d20  _observations = 
+0000f420: 5174 5769 6467 6574 732e 5141 6374 696f  QtWidgets.QActio
+0000f430: 6e28 4d61 696e 5769 6e64 6f77 290a 2020  n(MainWindow).  
+0000f440: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
+0000f450: 6e5f 466c 6167 5f6f 6273 6572 7661 7469  n_Flag_observati
+0000f460: 6f6e 732e 7365 744f 626a 6563 744e 616d  ons.setObjectNam
+0000f470: 6528 2261 6374 696f 6e5f 466c 6167 5f6f  e("action_Flag_o
+0000f480: 6273 6572 7661 7469 6f6e 7322 290a 2020  bservations").  
+0000f490: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
+0000f4a0: 6e5f 4368 616e 6765 5f43 616d 7061 6967  n_Change_Campaig
+0000f4b0: 6e5f 6e61 6d65 203d 2051 7457 6964 6765  n_name = QtWidge
+0000f4c0: 7473 2e51 4163 7469 6f6e 284d 6169 6e57  ts.QAction(MainW
+0000f4d0: 696e 646f 7729 0a20 2020 2020 2020 2073  indow).        s
+0000f4e0: 656c 662e 6163 7469 6f6e 5f43 6861 6e67  elf.action_Chang
+0000f4f0: 655f 4361 6d70 6169 676e 5f6e 616d 652e  e_Campaign_name.
+0000f500: 7365 7445 6e61 626c 6564 2846 616c 7365  setEnabled(False
+0000f510: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+0000f520: 6374 696f 6e5f 4368 616e 6765 5f43 616d  ction_Change_Cam
+0000f530: 7061 6967 6e5f 6e61 6d65 2e73 6574 4f62  paign_name.setOb
+0000f540: 6a65 6374 4e61 6d65 2822 6163 7469 6f6e  jectName("action
+0000f550: 5f43 6861 6e67 655f 4361 6d70 6169 676e  _Change_Campaign
+0000f560: 5f6e 616d 6522 290a 2020 2020 2020 2020  _name").        
+0000f570: 7365 6c66 2e61 6374 696f 6e5f 4162 6f75  self.action_Abou
+0000f580: 7420 3d20 5174 5769 6467 6574 732e 5141  t = QtWidgets.QA
+0000f590: 6374 696f 6e28 4d61 696e 5769 6e64 6f77  ction(MainWindow
+0000f5a0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+0000f5b0: 6374 696f 6e5f 4162 6f75 742e 7365 744f  ction_About.setO
+0000f5c0: 626a 6563 744e 616d 6528 2261 6374 696f  bjectName("actio
+0000f5d0: 6e5f 4162 6f75 7422 290a 2020 2020 2020  n_About").      
+0000f5e0: 2020 7365 6c66 2e61 6374 696f 6e5f 4c69    self.action_Li
+0000f5f0: 6365 6e73 6520 3d20 5174 5769 6467 6574  cense = QtWidget
+0000f600: 732e 5141 6374 696f 6e28 4d61 696e 5769  s.QAction(MainWi
+0000f610: 6e64 6f77 290a 2020 2020 2020 2020 7365  ndow).        se
+0000f620: 6c66 2e61 6374 696f 6e5f 4c69 6365 6e73  lf.action_Licens
+0000f630: 652e 7365 744f 626a 6563 744e 616d 6528  e.setObjectName(
+0000f640: 2261 6374 696f 6e5f 4c69 6365 6e73 6522  "action_License"
+0000f650: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+0000f660: 6374 696f 6e5f 4769 735f 4578 706f 7274  ction_Gis_Export
+0000f670: 5f73 6574 7469 6e67 7320 3d20 5174 5769  _settings = QtWi
+0000f680: 6467 6574 732e 5141 6374 696f 6e28 4d61  dgets.QAction(Ma
+0000f690: 696e 5769 6e64 6f77 290a 2020 2020 2020  inWindow).      
+0000f6a0: 2020 7365 6c66 2e61 6374 696f 6e5f 4769    self.action_Gi
+0000f6b0: 735f 4578 706f 7274 5f73 6574 7469 6e67  s_Export_setting
+0000f6c0: 732e 7365 7445 6e61 626c 6564 2846 616c  s.setEnabled(Fal
+0000f6d0: 7365 290a 2020 2020 2020 2020 7365 6c66  se).        self
+0000f6e0: 2e61 6374 696f 6e5f 4769 735f 4578 706f  .action_Gis_Expo
+0000f6f0: 7274 5f73 6574 7469 6e67 732e 7365 744f  rt_settings.setO
+0000f700: 626a 6563 744e 616d 6528 2261 6374 696f  bjectName("actio
+0000f710: 6e5f 4769 735f 4578 706f 7274 5f73 6574  n_Gis_Export_set
+0000f720: 7469 6e67 7322 290a 2020 2020 2020 2020  tings").        
+0000f730: 7365 6c66 2e61 6374 696f 6e5f 6672 6f6d  self.action_from
+0000f740: 5f6f 6573 676e 5f74 6162 6c65 203d 2051  _oesgn_table = Q
+0000f750: 7457 6964 6765 7473 2e51 4163 7469 6f6e  tWidgets.QAction
+0000f760: 284d 6169 6e57 696e 646f 7729 0a20 2020  (MainWindow).   
+0000f770: 2020 2020 2073 656c 662e 6163 7469 6f6e       self.action
+0000f780: 5f66 726f 6d5f 6f65 7367 6e5f 7461 626c  _from_oesgn_tabl
+0000f790: 652e 7365 744f 626a 6563 744e 616d 6528  e.setObjectName(
+0000f7a0: 2261 6374 696f 6e5f 6672 6f6d 5f6f 6573  "action_from_oes
+0000f7b0: 676e 5f74 6162 6c65 2229 0a20 2020 2020  gn_table").     
+0000f7c0: 2020 2073 656c 662e 6163 7469 6f6e 5f66     self.action_f
+0000f7d0: 726f 6d5f 6373 765f 6669 6c65 203d 2051  rom_csv_file = Q
+0000f7e0: 7457 6964 6765 7473 2e51 4163 7469 6f6e  tWidgets.QAction
+0000f7f0: 284d 6169 6e57 696e 646f 7729 0a20 2020  (MainWindow).   
+0000f800: 2020 2020 2073 656c 662e 6163 7469 6f6e       self.action
+0000f810: 5f66 726f 6d5f 6373 765f 6669 6c65 2e73  _from_csv_file.s
+0000f820: 6574 4f62 6a65 6374 4e61 6d65 2822 6163  etObjectName("ac
+0000f830: 7469 6f6e 5f66 726f 6d5f 6373 765f 6669  tion_from_csv_fi
+0000f840: 6c65 2229 0a20 2020 2020 2020 2073 656c  le").        sel
+0000f850: 662e 6163 7469 6f6e 5f43 6f72 7265 6374  f.action_Correct
+0000f860: 696f 6e5f 7469 6d65 5f73 6572 6965 7320  ion_time_series 
+0000f870: 3d20 5174 5769 6467 6574 732e 5141 6374  = QtWidgets.QAct
+0000f880: 696f 6e28 4d61 696e 5769 6e64 6f77 290a  ion(MainWindow).
+0000f890: 2020 2020 2020 2020 7365 6c66 2e61 6374          self.act
+0000f8a0: 696f 6e5f 436f 7272 6563 7469 6f6e 5f74  ion_Correction_t
+0000f8b0: 696d 655f 7365 7269 6573 2e73 6574 4f62  ime_series.setOb
+0000f8c0: 6a65 6374 4e61 6d65 2822 6163 7469 6f6e  jectName("action
+0000f8d0: 5f43 6f72 7265 6374 696f 6e5f 7469 6d65  _Correction_time
+0000f8e0: 5f73 6572 6965 7322 290a 2020 2020 2020  _series").      
+0000f8f0: 2020 7365 6c66 2e61 6374 696f 6e5f 6772    self.action_gr
+0000f900: 6176 696d 6574 6572 735f 6672 6f6d 5f6a  avimeters_from_j
+0000f910: 736f 6e5f 6669 6c65 203d 2051 7457 6964  son_file = QtWid
+0000f920: 6765 7473 2e51 4163 7469 6f6e 284d 6169  gets.QAction(Mai
+0000f930: 6e57 696e 646f 7729 0a20 2020 2020 2020  nWindow).       
+0000f940: 2073 656c 662e 6163 7469 6f6e 5f67 7261   self.action_gra
+0000f950: 7669 6d65 7465 7273 5f66 726f 6d5f 6a73  vimeters_from_js
+0000f960: 6f6e 5f66 696c 652e 7365 744f 626a 6563  on_file.setObjec
+0000f970: 744e 616d 6528 2261 6374 696f 6e5f 6772  tName("action_gr
+0000f980: 6176 696d 6574 6572 735f 6672 6f6d 5f6a  avimeters_from_j
+0000f990: 736f 6e5f 6669 6c65 2229 0a20 2020 2020  son_file").     
+0000f9a0: 2020 2073 656c 662e 6d65 6e75 4164 645f     self.menuAdd_
+0000f9b0: 5375 7276 6579 2e61 6464 4163 7469 6f6e  Survey.addAction
+0000f9c0: 2873 656c 662e 6163 7469 6f6e 5f66 726f  (self.action_fro
+0000f9d0: 6d5f 4347 355f 6f62 7365 7276 6174 696f  m_CG5_observatio
+0000f9e0: 6e5f 6669 6c65 290a 2020 2020 2020 2020  n_file).        
+0000f9f0: 7365 6c66 2e6d 656e 7541 6464 5f53 7572  self.menuAdd_Sur
+0000fa00: 7665 792e 6164 6441 6374 696f 6e28 7365  vey.addAction(se
+0000fa10: 6c66 2e61 6374 696f 6e5f 6672 6f6d 5f42  lf.action_from_B
+0000fa20: 4556 5f6f 6273 6572 7661 7469 6f6e 5f66  EV_observation_f
+0000fa30: 696c 6529 0a20 2020 2020 2020 2073 656c  ile).        sel
+0000fa40: 662e 6d65 6e75 5f41 6464 5f53 7461 7469  f.menu_Add_Stati
+0000fa50: 6f6e 732e 6164 6441 6374 696f 6e28 7365  ons.addAction(se
+0000fa60: 6c66 2e61 6374 696f 6e5f 6672 6f6d 5f6f  lf.action_from_o
+0000fa70: 6573 676e 5f74 6162 6c65 290a 2020 2020  esgn_table).    
+0000fa80: 2020 2020 7365 6c66 2e6d 656e 755f 4164      self.menu_Ad
+0000fa90: 645f 5374 6174 696f 6e73 2e61 6464 4163  d_Stations.addAc
+0000faa0: 7469 6f6e 2873 656c 662e 6163 7469 6f6e  tion(self.action
+0000fab0: 5f66 726f 6d5f 6373 765f 6669 6c65 290a  _from_csv_file).
+0000fac0: 2020 2020 2020 2020 7365 6c66 2e6d 656e          self.men
+0000fad0: 755f 4164 645f 4772 6176 696d 6574 6572  u_Add_Gravimeter
+0000fae0: 732e 6164 6441 6374 696f 6e28 7365 6c66  s.addAction(self
+0000faf0: 2e61 6374 696f 6e5f 6772 6176 696d 6574  .action_gravimet
+0000fb00: 6572 735f 6672 6f6d 5f6a 736f 6e5f 6669  ers_from_json_fi
+0000fb10: 6c65 290a 2020 2020 2020 2020 7365 6c66  le).        self
+0000fb20: 2e6d 656e 755f 4669 6c65 2e61 6464 4163  .menu_File.addAc
+0000fb30: 7469 6f6e 2873 656c 662e 6163 7469 6f6e  tion(self.action
+0000fb40: 5f4e 6577 5f43 616d 7061 6967 6e29 0a20  _New_Campaign). 
+0000fb50: 2020 2020 2020 2073 656c 662e 6d65 6e75         self.menu
+0000fb60: 5f46 696c 652e 6164 6441 6374 696f 6e28  _File.addAction(
+0000fb70: 7365 6c66 2e61 6374 696f 6e5f 4368 616e  self.action_Chan
+0000fb80: 6765 5f6f 7574 7075 745f 6469 7265 6374  ge_output_direct
+0000fb90: 6f72 7929 0a20 2020 2020 2020 2073 656c  ory).        sel
+0000fba0: 662e 6d65 6e75 5f46 696c 652e 6164 6441  f.menu_File.addA
+0000fbb0: 6374 696f 6e28 7365 6c66 2e61 6374 696f  ction(self.actio
+0000fbc0: 6e5f 4368 616e 6765 5f43 616d 7061 6967  n_Change_Campaig
+0000fbd0: 6e5f 6e61 6d65 290a 2020 2020 2020 2020  n_name).        
+0000fbe0: 7365 6c66 2e6d 656e 755f 4669 6c65 2e61  self.menu_File.a
+0000fbf0: 6464 4163 7469 6f6e 2873 656c 662e 6163  ddAction(self.ac
+0000fc00: 7469 6f6e 5f53 6176 655f 4361 6d70 6169  tion_Save_Campai
+0000fc10: 676e 290a 2020 2020 2020 2020 7365 6c66  gn).        self
+0000fc20: 2e6d 656e 755f 4669 6c65 2e61 6464 4163  .menu_File.addAc
+0000fc30: 7469 6f6e 2873 656c 662e 6163 7469 6f6e  tion(self.action
+0000fc40: 5f4c 6f61 645f 4361 6d70 6169 676e 290a  _Load_Campaign).
+0000fc50: 2020 2020 2020 2020 7365 6c66 2e6d 656e          self.men
+0000fc60: 755f 4669 6c65 2e61 6464 5365 7061 7261  u_File.addSepara
+0000fc70: 746f 7228 290a 2020 2020 2020 2020 7365  tor().        se
+0000fc80: 6c66 2e6d 656e 755f 4669 6c65 2e61 6464  lf.menu_File.add
+0000fc90: 4163 7469 6f6e 2873 656c 662e 6d65 6e75  Action(self.menu
+0000fca0: 4164 645f 5375 7276 6579 2e6d 656e 7541  Add_Survey.menuA
 0000fcb0: 6374 696f 6e28 2929 0a20 2020 2020 2020  ction()).       
-0000fcc0: 2073 656c 662e 6d65 6e75 6261 722e 6164   self.menubar.ad
-0000fcd0: 6441 6374 696f 6e28 7365 6c66 2e6d 656e  dAction(self.men
-0000fce0: 7545 7374 696d 6174 696f 6e5f 7365 7474  uEstimation_sett
-0000fcf0: 696e 6773 2e6d 656e 7541 6374 696f 6e28  ings.menuAction(
-0000fd00: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-0000fd10: 6d65 6e75 6261 722e 6164 6441 6374 696f  menubar.addActio
-0000fd20: 6e28 7365 6c66 2e6d 656e 7543 6f72 7265  n(self.menuCorre
-0000fd30: 6374 696f 6e73 2e6d 656e 7541 6374 696f  ctions.menuActio
-0000fd40: 6e28 2929 0a20 2020 2020 2020 2073 656c  n()).        sel
-0000fd50: 662e 6d65 6e75 6261 722e 6164 6441 6374  f.menubar.addAct
-0000fd60: 696f 6e28 7365 6c66 2e6d 656e 7548 656c  ion(self.menuHel
-0000fd70: 702e 6d65 6e75 4163 7469 6f6e 2829 290a  p.menuAction()).
-0000fd80: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-0000fd90: 7472 616e 736c 6174 6555 6928 4d61 696e  translateUi(Main
-0000fda0: 5769 6e64 6f77 290a 2020 2020 2020 2020  Window).        
-0000fdb0: 7365 6c66 2e74 6162 5769 6467 6574 5f4d  self.tabWidget_M
-0000fdc0: 6169 6e2e 7365 7443 7572 7265 6e74 496e  ain.setCurrentIn
-0000fdd0: 6465 7828 3229 0a20 2020 2020 2020 2073  dex(2).        s
-0000fde0: 656c 662e 7461 625f 5769 6467 6574 5f53  elf.tab_Widget_S
-0000fdf0: 7461 7469 6f6e 732e 7365 7443 7572 7265  tations.setCurre
-0000fe00: 6e74 496e 6465 7828 3029 0a20 2020 2020  ntIndex(0).     
-0000fe10: 2020 2073 656c 662e 7461 6257 6964 6765     self.tabWidge
-0000fe20: 745f 6772 6176 696d 6574 6572 732e 7365  t_gravimeters.se
-0000fe30: 7443 7572 7265 6e74 496e 6465 7828 3029  tCurrentIndex(0)
-0000fe40: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
-0000fe50: 6257 6964 6765 745f 6f62 7365 7276 6174  bWidget_observat
-0000fe60: 696f 6e73 2e73 6574 4375 7272 656e 7449  ions.setCurrentI
-0000fe70: 6e64 6578 2830 290a 2020 2020 2020 2020  ndex(0).        
-0000fe80: 7365 6c66 2e74 6162 5769 6467 6574 5f72  self.tabWidget_r
-0000fe90: 6573 756c 7473 2e73 6574 4375 7272 656e  esults.setCurren
-0000fea0: 7449 6e64 6578 2830 290a 2020 2020 2020  tIndex(0).      
-0000feb0: 2020 7365 6c66 2e72 6164 696f 4275 7474    self.radioButt
-0000fec0: 6f6e 5f72 6573 756c 7473 5f6f 6273 5f70  on_results_obs_p
-0000fed0: 6c6f 745f 6869 7374 6f67 7261 6d2e 746f  lot_histogram.to
-0000fee0: 6767 6c65 645b 2762 6f6f 6c27 5d2e 636f  ggled['bool'].co
-0000fef0: 6e6e 6563 7428 7365 6c66 2e67 726f 7570  nnect(self.group
-0000ff00: 426f 785f 6869 7374 6f67 7261 6d5f 7365  Box_histogram_se
-0000ff10: 7474 696e 6773 2e73 6574 456e 6162 6c65  ttings.setEnable
-0000ff20: 6429 2023 2074 7970 653a 2069 676e 6f72  d) # type: ignor
-0000ff30: 650a 2020 2020 2020 2020 7365 6c66 2e63  e.        self.c
-0000ff40: 6865 636b 426f 785f 7374 6174 696f 6e73  heckBox_stations
-0000ff50: 5f70 6c6f 745f 6f62 735f 6d61 702e 746f  _plot_obs_map.to
-0000ff60: 6767 6c65 645b 2762 6f6f 6c27 5d2e 636f  ggled['bool'].co
-0000ff70: 6e6e 6563 7428 7365 6c66 2e63 6f6d 626f  nnect(self.combo
-0000ff80: 426f 785f 7374 6174 696f 6e73 5f70 6c6f  Box_stations_plo
-0000ff90: 745f 6f62 735f 6d61 705f 7375 7276 6579  t_obs_map_survey
-0000ffa0: 732e 7365 7445 6e61 626c 6564 2920 2320  s.setEnabled) # 
-0000ffb0: 7479 7065 3a20 6967 6e6f 7265 0a20 2020  type: ignore.   
-0000ffc0: 2020 2020 2051 7443 6f72 652e 514d 6574       QtCore.QMet
-0000ffd0: 614f 626a 6563 742e 636f 6e6e 6563 7453  aObject.connectS
-0000ffe0: 6c6f 7473 4279 4e61 6d65 284d 6169 6e57  lotsByName(MainW
-0000fff0: 696e 646f 7729 0a0a 2020 2020 6465 6620  indow)..    def 
-00010000: 7265 7472 616e 736c 6174 6555 6928 7365  retranslateUi(se
-00010010: 6c66 2c20 4d61 696e 5769 6e64 6f77 293a  lf, MainWindow):
-00010020: 0a20 2020 2020 2020 205f 7472 616e 736c  .        _transl
-00010030: 6174 6520 3d20 5174 436f 7265 2e51 436f  ate = QtCore.QCo
-00010040: 7265 4170 706c 6963 6174 696f 6e2e 7472  reApplication.tr
-00010050: 616e 736c 6174 650a 2020 2020 2020 2020  anslate.        
-00010060: 4d61 696e 5769 6e64 6f77 2e73 6574 5769  MainWindow.setWi
-00010070: 6e64 6f77 5469 746c 6528 5f74 7261 6e73  ndowTitle(_trans
-00010080: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
-00010090: 222c 2022 4772 6176 546f 6f6c 7322 2929  ", "GravTools"))
-000100a0: 0a20 2020 2020 2020 2073 656c 662e 6772  .        self.gr
-000100b0: 6f75 7042 6f78 5f66 696c 7465 725f 6f70  oupBox_filter_op
-000100c0: 7469 6f6e 732e 7365 7454 6f6f 6c54 6970  tions.setToolTip
-000100d0: 285f 7472 616e 736c 6174 6528 224d 6169  (_translate("Mai
-000100e0: 6e57 696e 646f 7722 2c20 2244 6973 706c  nWindow", "Displ
-000100f0: 6179 206f 7074 696f 6e73 2066 6f72 2073  ay options for s
-00010100: 7461 7469 6f6e 7322 2929 0a20 2020 2020  tations")).     
-00010110: 2020 2073 656c 662e 6772 6f75 7042 6f78     self.groupBox
-00010120: 5f66 696c 7465 725f 6f70 7469 6f6e 732e  _filter_options.
-00010130: 7365 7454 6974 6c65 285f 7472 616e 736c  setTitle(_transl
-00010140: 6174 6528 224d 6169 6e57 696e 646f 7722  ate("MainWindow"
-00010150: 2c20 2246 696c 7465 7220 4f70 7469 6f6e  , "Filter Option
-00010160: 7322 2929 0a20 2020 2020 2020 2073 656c  s")).        sel
-00010170: 662e 6368 6563 6b42 6f78 5f66 696c 7465  f.checkBox_filte
-00010180: 725f 6f62 7365 7276 6564 5f73 7461 745f  r_observed_stat_
-00010190: 6f6e 6c79 2e73 6574 546f 6f6c 5469 7028  only.setToolTip(
-000101a0: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
-000101b0: 5769 6e64 6f77 222c 2022 4469 7370 6c61  Window", "Displa
-000101c0: 7920 6f6e 6c79 2073 7461 7469 6f6e 7320  y only stations 
-000101d0: 7468 6174 2077 6572 6520 6f62 7365 7276  that were observ
-000101e0: 6564 2069 6e20 7468 6973 2063 616d 7061  ed in this campa
-000101f0: 6967 6e2e 2022 2929 0a20 2020 2020 2020  ign. ")).       
-00010200: 2073 656c 662e 6368 6563 6b42 6f78 5f66   self.checkBox_f
-00010210: 696c 7465 725f 6f62 7365 7276 6564 5f73  ilter_observed_s
-00010220: 7461 745f 6f6e 6c79 2e73 6574 5465 7874  tat_only.setText
-00010230: 285f 7472 616e 736c 6174 6528 224d 6169  (_translate("Mai
-00010240: 6e57 696e 646f 7722 2c20 224f 6273 6572  nWindow", "Obser
-00010250: 7665 6420 6f6e 6c79 2229 290a 2020 2020  ved only")).    
-00010260: 2020 2020 7365 6c66 2e6c 6162 656c 2e73      self.label.s
-00010270: 6574 5465 7874 285f 7472 616e 736c 6174  etText(_translat
-00010280: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
-00010290: 2253 7461 7469 6f6e 206e 616d 6520 6669  "Station name fi
-000102a0: 6c74 6572 2028 7265 6765 7829 2229 290a  lter (regex)")).
-000102b0: 2020 2020 2020 2020 7365 6c66 2e67 726f          self.gro
-000102c0: 7570 426f 785f 7374 6174 696f 6e73 5f6d  upBox_stations_m
-000102d0: 6170 5f76 6965 775f 6f70 7469 6f6e 732e  ap_view_options.
-000102e0: 7365 7454 6974 6c65 285f 7472 616e 736c  setTitle(_transl
-000102f0: 6174 6528 224d 6169 6e57 696e 646f 7722  ate("MainWindow"
-00010300: 2c20 224d 6170 2076 6965 7720 6f70 7469  , "Map view opti
-00010310: 6f6e 7322 2929 0a20 2020 2020 2020 2073  ons")).        s
-00010320: 656c 662e 6368 6563 6b42 6f78 5f73 7461  elf.checkBox_sta
-00010330: 7469 6f6e 735f 6d61 705f 7368 6f77 5f73  tions_map_show_s
-00010340: 7461 745f 6e61 6d65 5f6c 6162 656c 732e  tat_name_labels.
-00010350: 7365 7454 6578 7428 5f74 7261 6e73 6c61  setText(_transla
-00010360: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
-00010370: 2022 5368 6f77 2073 7461 7469 6f6e 206e   "Show station n
-00010380: 616d 6520 6c61 6265 6c73 2229 290a 2020  ame labels")).  
-00010390: 2020 2020 2020 7365 6c66 2e63 6865 636b        self.check
-000103a0: 426f 785f 7374 6174 696f 6e73 5f70 6c6f  Box_stations_plo
-000103b0: 745f 6f62 735f 6d61 702e 7365 7454 6f6f  t_obs_map.setToo
-000103c0: 6c54 6970 285f 7472 616e 736c 6174 6528  lTip(_translate(
-000103d0: 224d 6169 6e57 696e 646f 7722 2c20 223c  "MainWindow", "<
-000103e0: 6874 6d6c 3e3c 6865 6164 2f3e 3c62 6f64  html><head/><bod
-000103f0: 793e 3c70 3e50 6c6f 7420 6f62 7365 7276  y><p>Plot observ
-00010400: 6174 696f 6e73 2069 6e20 7465 726d 7320  ations in terms 
-00010410: 6f66 206c 696e 6573 2069 6e20 7468 6520  of lines in the 
-00010420: 7374 6174 696f 6e20 706c 6f74 2061 6363  station plot acc
-00010430: 6f72 6469 6e67 2074 6f20 7468 6520 7365  ording to the se
-00010440: 6c65 6374 696f 6e20 6265 6c6f 772e 3c2f  lection below.</
-00010450: 703e 3c2f 626f 6479 3e3c 2f68 746d 6c3e  p></body></html>
-00010460: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
-00010470: 2e63 6865 636b 426f 785f 7374 6174 696f  .checkBox_statio
-00010480: 6e73 5f70 6c6f 745f 6f62 735f 6d61 702e  ns_plot_obs_map.
-00010490: 7365 7454 6578 7428 5f74 7261 6e73 6c61  setText(_transla
-000104a0: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
-000104b0: 2022 506c 6f74 206f 6273 6572 7661 7469   "Plot observati
-000104c0: 6f6e 7322 2929 0a20 2020 2020 2020 2073  ons")).        s
-000104d0: 656c 662e 636f 6d62 6f42 6f78 5f73 7461  elf.comboBox_sta
-000104e0: 7469 6f6e 735f 706c 6f74 5f6f 6273 5f6d  tions_plot_obs_m
-000104f0: 6170 5f73 7572 7665 7973 2e73 6574 546f  ap_surveys.setTo
-00010500: 6f6c 5469 7028 5f74 7261 6e73 6c61 7465  olTip(_translate
-00010510: 2822 4d61 696e 5769 6e64 6f77 222c 2022  ("MainWindow", "
-00010520: 3c68 746d 6c3e 3c68 6561 642f 3e3c 626f  <html><head/><bo
-00010530: 6479 3e3c 703e 5365 6c65 6374 2077 6865  dy><p>Select whe
-00010540: 7468 6572 206f 6273 6572 7661 7469 6f6e  ther observation
-00010550: 7320 6f66 2061 6c6c 2073 7572 7665 7973  s of all surveys
-00010560: 2c20 6f72 206f 6620 6120 7365 6c65 6374  , or of a select
-00010570: 6564 2073 7572 7665 7920 7368 6f75 6c64  ed survey should
-00010580: 2062 6520 706c 6f74 7465 6420 696e 2074   be plotted in t
-00010590: 6865 2073 7461 7469 6f6e 206d 6170 2e3c  he station map.<
-000105a0: 2f70 3e3c 2f62 6f64 793e 3c2f 6874 6d6c  /p></body></html
-000105b0: 3e22 2929 0a20 2020 2020 2020 2073 656c  >")).        sel
-000105c0: 662e 7461 625f 5769 6467 6574 5f53 7461  f.tab_Widget_Sta
-000105d0: 7469 6f6e 732e 7365 7454 6162 5465 7874  tions.setTabText
-000105e0: 2873 656c 662e 7461 625f 5769 6467 6574  (self.tab_Widget
-000105f0: 5f53 7461 7469 6f6e 732e 696e 6465 784f  _Stations.indexO
-00010600: 6628 7365 6c66 2e74 6162 5f53 7461 7469  f(self.tab_Stati
-00010610: 6f6e 735f 5461 626c 6529 2c20 5f74 7261  ons_Table), _tra
-00010620: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
-00010630: 6f77 222c 2022 5461 626c 6522 2929 0a20  ow", "Table")). 
-00010640: 2020 2020 2020 2073 656c 662e 7461 625f         self.tab_
-00010650: 5769 6467 6574 5f53 7461 7469 6f6e 732e  Widget_Stations.
-00010660: 7365 7454 6162 5465 7874 2873 656c 662e  setTabText(self.
-00010670: 7461 625f 5769 6467 6574 5f53 7461 7469  tab_Widget_Stati
-00010680: 6f6e 732e 696e 6465 784f 6628 7365 6c66  ons.indexOf(self
-00010690: 2e74 6162 5f73 7461 7469 6f6e 735f 6d61  .tab_stations_ma
-000106a0: 7029 2c20 5f74 7261 6e73 6c61 7465 2822  p), _translate("
-000106b0: 4d61 696e 5769 6e64 6f77 222c 2022 4d61  MainWindow", "Ma
-000106c0: 7022 2929 0a20 2020 2020 2020 2073 656c  p")).        sel
-000106d0: 662e 7461 6257 6964 6765 745f 4d61 696e  f.tabWidget_Main
-000106e0: 2e73 6574 5461 6254 6578 7428 7365 6c66  .setTabText(self
-000106f0: 2e74 6162 5769 6467 6574 5f4d 6169 6e2e  .tabWidget_Main.
-00010700: 696e 6465 784f 6628 7365 6c66 2e74 6162  indexOf(self.tab
-00010710: 5f6d 6169 6e5f 7374 6174 696f 6e73 292c  _main_stations),
-00010720: 205f 7472 616e 736c 6174 6528 224d 6169   _translate("Mai
-00010730: 6e57 696e 646f 7722 2c20 2253 7461 7469  nWindow", "Stati
-00010740: 6f6e 7322 2929 0a20 2020 2020 2020 2073  ons")).        s
-00010750: 656c 662e 7472 6565 5769 6467 6574 5f67  elf.treeWidget_g
-00010760: 7261 7669 6d65 7465 7273 2e68 6561 6465  ravimeters.heade
-00010770: 7249 7465 6d28 292e 7365 7454 6578 7428  rItem().setText(
-00010780: 302c 205f 7472 616e 736c 6174 6528 224d  0, _translate("M
-00010790: 6169 6e57 696e 646f 7722 2c20 2254 7970  ainWindow", "Typ
-000107a0: 6522 2929 0a20 2020 2020 2020 2073 656c  e")).        sel
-000107b0: 662e 7472 6565 5769 6467 6574 5f67 7261  f.treeWidget_gra
-000107c0: 7669 6d65 7465 7273 2e68 6561 6465 7249  vimeters.headerI
-000107d0: 7465 6d28 292e 7365 7454 6578 7428 312c  tem().setText(1,
-000107e0: 205f 7472 616e 736c 6174 6528 224d 6169   _translate("Mai
-000107f0: 6e57 696e 646f 7722 2c20 2253 2f4e 2229  nWindow", "S/N")
-00010800: 290a 2020 2020 2020 2020 7365 6c66 2e70  ).        self.p
-00010810: 7573 6842 7574 746f 6e5f 6465 6c65 7465  ushButton_delete
-00010820: 5f67 7261 7669 6d65 7465 722e 7365 7454  _gravimeter.setT
-00010830: 6578 7428 5f74 7261 6e73 6c61 7465 2822  ext(_translate("
-00010840: 4d61 696e 5769 6e64 6f77 222c 2022 4465  MainWindow", "De
-00010850: 6c65 7465 2229 290a 2020 2020 2020 2020  lete")).        
-00010860: 7365 6c66 2e6c 6162 656c 5f31 392e 7365  self.label_19.se
-00010870: 7454 6f6f 6c54 6970 285f 7472 616e 736c  tToolTip(_transl
-00010880: 6174 6528 224d 6169 6e57 696e 646f 7722  ate("MainWindow"
-00010890: 2c20 224d 616e 7566 6163 7475 7265 7220  , "Manufacturer 
-000108a0: 6f66 2069 6e73 7472 756d 656e 742e 2229  of instrument.")
-000108b0: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
-000108c0: 6162 656c 5f31 392e 7365 7454 6578 7428  abel_19.setText(
-000108d0: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
-000108e0: 5769 6e64 6f77 222c 2022 4d61 6e75 6661  Window", "Manufa
-000108f0: 6374 7572 6572 3a22 2929 0a20 2020 2020  cturer:")).     
-00010900: 2020 2073 656c 662e 6c61 6265 6c5f 6772     self.label_gr
-00010910: 6176 695f 6d61 6e75 6661 6374 7572 6572  avi_manufacturer
-00010920: 2e73 6574 546f 6f6c 5469 7028 5f74 7261  .setToolTip(_tra
-00010930: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
-00010940: 6f77 222c 2022 4d61 6e75 6661 6374 7572  ow", "Manufactur
-00010950: 6572 206f 6620 696e 7374 7275 6d65 6e74  er of instrument
-00010960: 2e22 2929 0a20 2020 2020 2020 2073 656c  .")).        sel
-00010970: 662e 6c61 6265 6c5f 3230 2e73 6574 546f  f.label_20.setTo
-00010980: 6f6c 5469 7028 5f74 7261 6e73 6c61 7465  olTip(_translate
-00010990: 2822 4d61 696e 5769 6e64 6f77 222c 2022  ("MainWindow", "
-000109a0: 4772 6176 696d 6574 6572 2074 7970 652e  Gravimeter type.
-000109b0: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
-000109c0: 2e6c 6162 656c 5f32 302e 7365 7454 6578  .label_20.setTex
-000109d0: 7428 5f74 7261 6e73 6c61 7465 2822 4d61  t(_translate("Ma
-000109e0: 696e 5769 6e64 6f77 222c 2022 5479 7065  inWindow", "Type
-000109f0: 3a22 2929 0a20 2020 2020 2020 2073 656c  :")).        sel
-00010a00: 662e 6c61 6265 6c5f 6772 6176 695f 7479  f.label_gravi_ty
-00010a10: 7065 2e73 6574 546f 6f6c 5469 7028 5f74  pe.setToolTip(_t
-00010a20: 7261 6e73 6c61 7465 2822 4d61 696e 5769  ranslate("MainWi
-00010a30: 6e64 6f77 222c 2022 4772 6176 696d 6574  ndow", "Gravimet
-00010a40: 6572 2074 7970 652e 2229 290a 2020 2020  er type.")).    
-00010a50: 2020 2020 7365 6c66 2e6c 6162 656c 5f32      self.label_2
-00010a60: 312e 7365 7454 6f6f 6c54 6970 285f 7472  1.setToolTip(_tr
-00010a70: 616e 736c 6174 6528 224d 6169 6e57 696e  anslate("MainWin
-00010a80: 646f 7722 2c20 2253 6572 6961 6c20 6e75  dow", "Serial nu
-00010a90: 6d62 6572 2e22 2929 0a20 2020 2020 2020  mber.")).       
-00010aa0: 2073 656c 662e 6c61 6265 6c5f 3231 2e73   self.label_21.s
-00010ab0: 6574 5465 7874 285f 7472 616e 736c 6174  etText(_translat
-00010ac0: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
-00010ad0: 2253 6572 6961 6c20 6e75 6d62 6572 3a22  "Serial number:"
-00010ae0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-00010af0: 6c61 6265 6c5f 6772 6176 695f 7365 7269  label_gravi_seri
-00010b00: 616c 5f6e 756d 6265 722e 7365 7454 6f6f  al_number.setToo
-00010b10: 6c54 6970 285f 7472 616e 736c 6174 6528  lTip(_translate(
-00010b20: 224d 6169 6e57 696e 646f 7722 2c20 2253  "MainWindow", "S
-00010b30: 6572 6961 6c20 6e75 6d62 6572 2e22 2929  erial number."))
-00010b40: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
-00010b50: 6265 6c5f 3235 2e73 6574 546f 6f6c 5469  bel_25.setToolTi
-00010b60: 7028 5f74 7261 6e73 6c61 7465 2822 4d61  p(_translate("Ma
-00010b70: 696e 5769 6e64 6f77 222c 2022 5368 6f72  inWindow", "Shor
-00010b80: 7420 696e 7374 7275 6d65 6e74 2063 6f64  t instrument cod
-00010b90: 652e 2229 290a 2020 2020 2020 2020 7365  e.")).        se
-00010ba0: 6c66 2e6c 6162 656c 5f32 352e 7365 7454  lf.label_25.setT
-00010bb0: 6578 7428 5f74 7261 6e73 6c61 7465 2822  ext(_translate("
-00010bc0: 4d61 696e 5769 6e64 6f77 222c 2022 436f  MainWindow", "Co
-00010bd0: 6465 3a22 2929 0a20 2020 2020 2020 2073  de:")).        s
-00010be0: 656c 662e 6c61 6265 6c5f 6772 6176 695f  elf.label_gravi_
-00010bf0: 636f 6465 2e73 6574 546f 6f6c 5469 7028  code.setToolTip(
-00010c00: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
-00010c10: 5769 6e64 6f77 222c 2022 5368 6f72 7420  Window", "Short 
-00010c20: 696e 7374 7275 6d65 6e74 2063 6f64 652e  instrument code.
-00010c30: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
-00010c40: 2e6c 6162 656c 5f32 322e 7365 7454 6f6f  .label_22.setToo
-00010c50: 6c54 6970 285f 7472 616e 736c 6174 6528  lTip(_translate(
-00010c60: 224d 6169 6e57 696e 646f 7722 2c20 223c  "MainWindow", "<
-00010c70: 6874 6d6c 3e3c 6865 6164 2f3e 3c62 6f64  html><head/><bod
-00010c80: 793e 3c70 3e48 6569 6768 206f 6666 7365  y><p>Heigh offse
-00010c90: 7420 696e 206d 6574 6572 7320 6265 7477  t in meters betw
-00010ca0: 6565 6e20 696e 7374 7275 6d65 6e74 2074  een instrument t
-00010cb0: 6f70 2061 6e64 2073 656e 736f 7220 6c65  op and sensor le
-00010cc0: 7665 6c20 286e 6567 6174 6976 652c 2069  vel (negative, i
-00010cd0: 6620 7468 6520 7365 6e73 6f72 2069 7320  f the sensor is 
-00010ce0: 6265 6c6f 7720 7468 6520 746f 7029 2e3c  below the top).<
-00010cf0: 2f70 3e3c 2f62 6f64 793e 3c2f 6874 6d6c  /p></body></html
-00010d00: 3e22 2929 0a20 2020 2020 2020 2073 656c  >")).        sel
-00010d10: 662e 6c61 6265 6c5f 3232 2e73 6574 5465  f.label_22.setTe
-00010d20: 7874 285f 7472 616e 736c 6174 6528 224d  xt(_translate("M
-00010d30: 6169 6e57 696e 646f 7722 2c20 2248 6569  ainWindow", "Hei
-00010d40: 6768 7420 6f66 6673 6574 205b 6d5d 3a22  ght offset [m]:"
-00010d50: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-00010d60: 6c61 6265 6c5f 6772 6176 695f 6865 6967  label_gravi_heig
-00010d70: 6874 5f6f 6666 7365 742e 7365 7454 6f6f  ht_offset.setToo
-00010d80: 6c54 6970 285f 7472 616e 736c 6174 6528  lTip(_translate(
-00010d90: 224d 6169 6e57 696e 646f 7722 2c20 223c  "MainWindow", "<
-00010da0: 6874 6d6c 3e3c 6865 6164 2f3e 3c62 6f64  html><head/><bod
-00010db0: 793e 3c70 3e48 6569 6768 206f 6666 7365  y><p>Heigh offse
-00010dc0: 7420 696e 206d 6574 6572 7320 6265 7477  t in meters betw
-00010dd0: 6565 6e20 696e 7374 7275 6d65 6e74 2074  een instrument t
-00010de0: 6f70 2061 6e64 2073 656e 736f 7220 6c65  op and sensor le
-00010df0: 7665 6c20 286e 6567 6174 6976 652c 2069  vel (negative, i
-00010e00: 6620 7468 6520 7365 6e73 6f72 2069 7320  f the sensor is 
-00010e10: 6265 6c6f 7720 7468 6520 746f 7029 2e3c  below the top).<
-00010e20: 2f70 3e3c 2f62 6f64 793e 3c2f 6874 6d6c  /p></body></html
-00010e30: 3e22 2929 0a20 2020 2020 2020 2073 656c  >")).        sel
-00010e40: 662e 6c61 6265 6c5f 3233 2e73 6574 546f  f.label_23.setTo
-00010e50: 6f6c 5469 7028 5f74 7261 6e73 6c61 7465  olTip(_translate
-00010e60: 2822 4d61 696e 5769 6e64 6f77 222c 2022  ("MainWindow", "
-00010e70: 536f 7572 6365 206f 6620 7468 6520 6772  Source of the gr
-00010e80: 6176 696d 6574 6572 2064 6174 612e 2045  avimeter data. E
-00010e90: 6974 6865 7220 7468 6520 6e61 6d65 206f  ither the name o
-00010ea0: 6620 7468 6520 7375 7276 6579 2074 6865  f the survey the
-00010eb0: 2064 6174 6120 7761 7320 7461 6b65 6e20   data was taken 
-00010ec0: 6672 6f6d 2028 6f62 2e20 6669 6c65 292c  from (ob. file),
-00010ed0: 206f 7220 7468 6520 6e61 6d65 206f 6620   or the name of 
-00010ee0: 7468 6520 6772 6176 696d 6574 6572 2066  the gravimeter f
-00010ef0: 696c 652e 2229 290a 2020 2020 2020 2020  ile.")).        
-00010f00: 7365 6c66 2e6c 6162 656c 5f32 332e 7365  self.label_23.se
-00010f10: 7454 6578 7428 5f74 7261 6e73 6c61 7465  tText(_translate
-00010f20: 2822 4d61 696e 5769 6e64 6f77 222c 2022  ("MainWindow", "
-00010f30: 4461 7461 2073 6f75 7263 653a 2229 290a  Data source:")).
-00010f40: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
-00010f50: 656c 5f67 7261 7669 5f64 6174 615f 736f  el_gravi_data_so
-00010f60: 7572 6365 2e73 6574 546f 6f6c 5469 7028  urce.setToolTip(
-00010f70: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
-00010f80: 5769 6e64 6f77 222c 2022 536f 7572 6365  Window", "Source
-00010f90: 206f 6620 7468 6520 6772 6176 696d 6574   of the gravimet
-00010fa0: 6572 2064 6174 612e 2045 6974 6865 7220  er data. Either 
-00010fb0: 7468 6520 6e61 6d65 206f 6620 7468 6520  the name of the 
-00010fc0: 7375 7276 6579 2074 6865 2064 6174 6120  survey the data 
-00010fd0: 7761 7320 7461 6b65 6e20 6672 6f6d 2028  was taken from (
-00010fe0: 6f62 2e20 6669 6c65 292c 206f 7220 7468  ob. file), or th
-00010ff0: 6520 6e61 6d65 206f 6620 7468 6520 6772  e name of the gr
-00011000: 6176 696d 6574 6572 2066 696c 652e 2229  avimeter file.")
-00011010: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
-00011020: 6162 656c 5f32 342e 7365 7454 6f6f 6c54  abel_24.setToolT
-00011030: 6970 285f 7472 616e 736c 6174 6528 224d  ip(_translate("M
-00011040: 6169 6e57 696e 646f 7722 2c20 2254 7970  ainWindow", "Typ
-00011050: 6520 6f66 2074 6865 2067 7261 7669 6d65  e of the gravime
-00011060: 7465 7220 6461 7461 2073 6f75 7263 652e  ter data source.
-00011070: 2022 2929 0a20 2020 2020 2020 2073 656c   ")).        sel
-00011080: 662e 6c61 6265 6c5f 3234 2e73 6574 5465  f.label_24.setTe
-00011090: 7874 285f 7472 616e 736c 6174 6528 224d  xt(_translate("M
-000110a0: 6169 6e57 696e 646f 7722 2c20 2244 6174  ainWindow", "Dat
-000110b0: 6120 736f 7572 6365 2074 7970 653a 2229  a source type:")
-000110c0: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
-000110d0: 6162 656c 5f67 7261 7669 5f64 6174 615f  abel_gravi_data_
-000110e0: 736f 7572 6365 5f74 7970 652e 7365 7454  source_type.setT
-000110f0: 6f6f 6c54 6970 285f 7472 616e 736c 6174  oolTip(_translat
-00011100: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
-00011110: 2254 7970 6520 6f66 2074 6865 2067 7261  "Type of the gra
-00011120: 7669 6d65 7465 7220 6461 7461 2073 6f75  vimeter data sou
-00011130: 7263 652e 2022 2929 0a20 2020 2020 2020  rce. ")).       
-00011140: 2073 656c 662e 6c61 6265 6c5f 3236 2e73   self.label_26.s
-00011150: 6574 546f 6f6c 5469 7028 5f74 7261 6e73  etToolTip(_trans
-00011160: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
-00011170: 222c 2022 4e75 6d62 6572 206f 6620 7363  ", "Number of sc
-00011180: 616c 6520 6661 6374 6f72 2069 7465 6d73  ale factor items
-00011190: 2e22 2929 0a20 2020 2020 2020 2073 656c  .")).        sel
-000111a0: 662e 6c61 6265 6c5f 3236 2e73 6574 5465  f.label_26.setTe
-000111b0: 7874 285f 7472 616e 736c 6174 6528 224d  xt(_translate("M
-000111c0: 6169 6e57 696e 646f 7722 2c20 224e 756d  ainWindow", "Num
-000111d0: 6265 7220 6f66 2073 6361 6c65 2066 6163  ber of scale fac
-000111e0: 746f 7273 3a22 2929 0a20 2020 2020 2020  tors:")).       
-000111f0: 2073 656c 662e 6c61 6265 6c5f 6772 6176   self.label_grav
-00011200: 695f 6e75 6d5f 7363 616c 655f 6661 6374  i_num_scale_fact
-00011210: 6f72 732e 7365 7454 6f6f 6c54 6970 285f  ors.setToolTip(_
-00011220: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
-00011230: 696e 646f 7722 2c20 224e 756d 6265 7220  indow", "Number 
-00011240: 6f66 2073 6361 6c65 2066 6163 746f 7220  of scale factor 
-00011250: 6974 656d 732e 2229 290a 2020 2020 2020  items.")).      
-00011260: 2020 7365 6c66 2e6c 6162 656c 5f32 382e    self.label_28.
-00011270: 7365 7454 6578 7428 5f74 7261 6e73 6c61  setText(_transla
-00011280: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
-00011290: 2022 4465 7363 7269 7074 696f 6e3a 2229   "Description:")
-000112a0: 290a 2020 2020 2020 2020 7365 6c66 2e74  ).        self.t
-000112b0: 6162 5769 6467 6574 5f67 7261 7669 6d65  abWidget_gravime
-000112c0: 7465 7273 2e73 6574 5461 6254 6578 7428  ters.setTabText(
-000112d0: 7365 6c66 2e74 6162 5769 6467 6574 5f67  self.tabWidget_g
-000112e0: 7261 7669 6d65 7465 7273 2e69 6e64 6578  ravimeters.index
-000112f0: 4f66 2873 656c 662e 7461 625f 6772 6176  Of(self.tab_grav
-00011300: 696d 6574 6572 5f69 6e66 6f29 2c20 5f74  imeter_info), _t
-00011310: 7261 6e73 6c61 7465 2822 4d61 696e 5769  ranslate("MainWi
-00011320: 6e64 6f77 222c 2022 496e 666f 2229 290a  ndow", "Info")).
-00011330: 2020 2020 2020 2020 7365 6c66 2e74 6162          self.tab
-00011340: 5769 6467 6574 5f67 7261 7669 6d65 7465  Widget_gravimete
-00011350: 7273 2e73 6574 5461 6254 6578 7428 7365  rs.setTabText(se
-00011360: 6c66 2e74 6162 5769 6467 6574 5f67 7261  lf.tabWidget_gra
-00011370: 7669 6d65 7465 7273 2e69 6e64 6578 4f66  vimeters.indexOf
-00011380: 2873 656c 662e 7461 625f 6772 6176 696d  (self.tab_gravim
-00011390: 6574 6572 5f73 6361 6c65 292c 205f 7472  eter_scale), _tr
-000113a0: 616e 736c 6174 6528 224d 6169 6e57 696e  anslate("MainWin
-000113b0: 646f 7722 2c20 2253 6361 6c65 2054 6162  dow", "Scale Tab
-000113c0: 6c65 2229 290a 2020 2020 2020 2020 7365  le")).        se
-000113d0: 6c66 2e74 6162 5769 6467 6574 5f4d 6169  lf.tabWidget_Mai
-000113e0: 6e2e 7365 7454 6162 5465 7874 2873 656c  n.setTabText(sel
-000113f0: 662e 7461 6257 6964 6765 745f 4d61 696e  f.tabWidget_Main
-00011400: 2e69 6e64 6578 4f66 2873 656c 662e 7461  .indexOf(self.ta
-00011410: 625f 6d61 696e 5f67 7261 7669 6d65 7465  b_main_gravimete
-00011420: 7273 292c 205f 7472 616e 736c 6174 6528  rs), _translate(
-00011430: 224d 6169 6e57 696e 646f 7722 2c20 2247  "MainWindow", "G
-00011440: 7261 7669 6d65 7465 7273 2229 290a 2020  ravimeters")).  
-00011450: 2020 2020 2020 7365 6c66 2e74 7265 6557        self.treeW
-00011460: 6964 6765 745f 6f62 7365 7276 6174 696f  idget_observatio
-00011470: 6e73 2e73 6574 536f 7274 696e 6745 6e61  ns.setSortingEna
-00011480: 626c 6564 2846 616c 7365 290a 2020 2020  bled(False).    
-00011490: 2020 2020 7365 6c66 2e74 7265 6557 6964      self.treeWid
-000114a0: 6765 745f 6f62 7365 7276 6174 696f 6e73  get_observations
-000114b0: 2e68 6561 6465 7249 7465 6d28 292e 7365  .headerItem().se
-000114c0: 7454 6578 7428 302c 205f 7472 616e 736c  tText(0, _transl
-000114d0: 6174 6528 224d 6169 6e57 696e 646f 7722  ate("MainWindow"
-000114e0: 2c20 2253 7572 7665 7922 2929 0a20 2020  , "Survey")).   
-000114f0: 2020 2020 2073 656c 662e 7472 6565 5769       self.treeWi
-00011500: 6467 6574 5f6f 6273 6572 7661 7469 6f6e  dget_observation
-00011510: 732e 6865 6164 6572 4974 656d 2829 2e73  s.headerItem().s
-00011520: 6574 5465 7874 2831 2c20 5f74 7261 6e73  etText(1, _trans
-00011530: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
-00011540: 222c 2022 5374 6174 696f 6e22 2929 0a20  ", "Station")). 
-00011550: 2020 2020 2020 2073 656c 662e 7472 6565         self.tree
-00011560: 5769 6467 6574 5f6f 6273 6572 7661 7469  Widget_observati
-00011570: 6f6e 732e 6865 6164 6572 4974 656d 2829  ons.headerItem()
-00011580: 2e73 6574 5465 7874 2832 2c20 5f74 7261  .setText(2, _tra
-00011590: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
-000115a0: 6f77 222c 2022 234f 6273 2229 290a 2020  ow", "#Obs")).  
-000115b0: 2020 2020 2020 7365 6c66 2e70 7573 6842        self.pushB
-000115c0: 7574 746f 6e5f 6f62 735f 636f 6c6c 6170  utton_obs_collap
-000115d0: 735f 616c 6c2e 7365 7454 6578 7428 5f74  s_all.setText(_t
-000115e0: 7261 6e73 6c61 7465 2822 4d61 696e 5769  ranslate("MainWi
-000115f0: 6e64 6f77 222c 2022 436f 6c6c 6170 6520  ndow", "Collape 
-00011600: 616c 6c22 2929 0a20 2020 2020 2020 2073  all")).        s
-00011610: 656c 662e 7075 7368 4275 7474 6f6e 5f6f  elf.pushButton_o
-00011620: 6273 5f65 7870 616e 645f 616c 6c2e 7365  bs_expand_all.se
-00011630: 7454 6578 7428 5f74 7261 6e73 6c61 7465  tText(_translate
-00011640: 2822 4d61 696e 5769 6e64 6f77 222c 2022  ("MainWindow", "
-00011650: 4578 7061 6e64 2061 6c6c 2229 290a 2020  Expand all")).  
-00011660: 2020 2020 2020 7365 6c66 2e67 726f 7570        self.group
-00011670: 426f 785f 6f62 735f 6461 7461 5f6d 616e  Box_obs_data_man
-00011680: 6970 756c 6174 696f 6e2e 7365 7454 6974  ipulation.setTit
-00011690: 6c65 285f 7472 616e 736c 6174 6528 224d  le(_translate("M
-000116a0: 6169 6e57 696e 646f 7722 2c20 2244 6174  ainWindow", "Dat
-000116b0: 6120 6d61 6e69 7075 6c61 7469 6f6e 2229  a manipulation")
-000116c0: 290a 2020 2020 2020 2020 7365 6c66 2e70  ).        self.p
-000116d0: 7573 6842 7574 746f 6e5f 6f62 735f 6170  ushButton_obs_ap
-000116e0: 706c 795f 6175 746f 7365 6c65 6374 5f63  ply_autoselect_c
-000116f0: 7572 7265 6e74 5f64 6174 612e 7365 7454  urrent_data.setT
-00011700: 6f6f 6c54 6970 285f 7472 616e 736c 6174  oolTip(_translat
-00011710: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
-00011720: 2241 6374 6976 6174 652f 6465 6163 7469  "Activate/deacti
-00011730: 7661 7465 206f 6273 6572 7661 7469 6f6e  vate observation
-00011740: 7320 6f66 2074 6865 2063 7572 7265 6e74  s of the current
-00011750: 2073 656c 6563 7465 6420 7375 7276 6579   selected survey
-00011760: 206f 7220 7365 7475 7020 6163 636f 7264   or setup accord
-00011770: 696e 6720 746f 2074 6865 2061 7574 6f2d  ing to the auto-
-00011780: 7365 6c65 6374 696f 6e20 6f70 7469 6f6e  selection option
-00011790: 732e 2229 290a 2020 2020 2020 2020 7365  s.")).        se
-000117a0: 6c66 2e70 7573 6842 7574 746f 6e5f 6f62  lf.pushButton_ob
-000117b0: 735f 6170 706c 795f 6175 746f 7365 6c65  s_apply_autosele
-000117c0: 6374 5f63 7572 7265 6e74 5f64 6174 612e  ct_current_data.
-000117d0: 7365 7454 6578 7428 5f74 7261 6e73 6c61  setText(_transla
-000117e0: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
-000117f0: 2022 4170 706c 7920 4175 746f 7365 6c65   "Apply Autosele
-00011800: 6374 696f 6e22 2929 0a20 2020 2020 2020  ction")).       
-00011810: 2073 656c 662e 7075 7368 4275 7474 6f6e   self.pushButton
-00011820: 5f6f 6273 5f63 6f6d 705f 7365 7475 705f  _obs_comp_setup_
-00011830: 6461 7461 2e73 6574 546f 6f6c 5469 7028  data.setToolTip(
-00011840: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
-00011850: 5769 6e64 6f77 222c 2022 436f 6d70 7574  Window", "Comput
-00011860: 6520 7661 7269 616e 6365 2d77 6569 6768  e variance-weigh
-00011870: 7465 6420 6d65 616e 206f 6620 6163 7469  ted mean of acti
-00011880: 7665 206f 6273 6572 7661 7469 6f6e 7320  ve observations 
-00011890: 666f 7220 616c 6c20 7365 7475 7073 2069  for all setups i
-000118a0: 6e20 6361 6d70 6169 676e 2e22 2929 0a20  n campaign.")). 
-000118b0: 2020 2020 2020 2073 656c 662e 7075 7368         self.push
-000118c0: 4275 7474 6f6e 5f6f 6273 5f63 6f6d 705f  Button_obs_comp_
-000118d0: 7365 7475 705f 6461 7461 2e73 6574 5465  setup_data.setTe
-000118e0: 7874 285f 7472 616e 736c 6174 6528 224d  xt(_translate("M
-000118f0: 6169 6e57 696e 646f 7722 2c20 2243 6f6d  ainWindow", "Com
-00011900: 7075 7465 2073 6574 7570 2064 6174 6120  pute setup data 
-00011910: 666f 7220 6361 6d70 6169 676e 2229 290a  for campaign")).
-00011920: 2020 2020 2020 2020 7365 6c66 2e70 7573          self.pus
-00011930: 6842 7574 746f 6e5f 6f62 735f 7275 6e5f  hButton_obs_run_
-00011940: 6573 7469 6d61 7469 6f6e 2e73 6574 546f  estimation.setTo
-00011950: 6f6c 5469 7028 5f74 7261 6e73 6c61 7465  olTip(_translate
-00011960: 2822 4d61 696e 5769 6e64 6f77 222c 2022  ("MainWindow", "
-00011970: 5275 6e20 7061 7261 6d65 7465 7220 6573  Run parameter es
-00011980: 7469 6d61 7469 6f6e 2061 6363 6f72 6469  timation accordi
-00011990: 6e67 2074 6f20 7468 6520 6573 7469 6d61  ng to the estima
-000119a0: 7469 6f6e 2073 6574 7469 6e67 732e 2229  tion settings.")
-000119b0: 290a 2020 2020 2020 2020 7365 6c66 2e70  ).        self.p
-000119c0: 7573 6842 7574 746f 6e5f 6f62 735f 7275  ushButton_obs_ru
-000119d0: 6e5f 6573 7469 6d61 7469 6f6e 2e73 6574  n_estimation.set
-000119e0: 5465 7874 285f 7472 616e 736c 6174 6528  Text(_translate(
-000119f0: 224d 6169 6e57 696e 646f 7722 2c20 2252  "MainWindow", "R
-00011a00: 756e 2065 7374 696d 6174 696f 6e22 2929  un estimation"))
-00011a10: 0a20 2020 2020 2020 2073 656c 662e 6772  .        self.gr
-00011a20: 6f75 7042 6f78 5f6f 6273 5f76 6965 775f  oupBox_obs_view_
-00011a30: 6f70 7469 6f6e 732e 7365 7454 6974 6c65  options.setTitle
-00011a40: 285f 7472 616e 736c 6174 6528 224d 6169  (_translate("Mai
-00011a50: 6e57 696e 646f 7722 2c20 2256 6965 7720  nWindow", "View 
-00011a60: 4f70 7469 6f6e 7322 2929 0a20 2020 2020  Options")).     
-00011a70: 2020 2073 656c 662e 6368 6563 6b42 6f78     self.checkBox
-00011a80: 5f6f 6273 5f70 6c6f 745f 7265 6475 6365  _obs_plot_reduce
-00011a90: 645f 6f62 7365 7276 6174 696f 6e73 2e73  d_observations.s
-00011aa0: 6574 546f 6f6c 5469 7028 5f74 7261 6e73  etToolTip(_trans
-00011ab0: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
-00011ac0: 222c 2022 506c 6f74 2072 6564 7563 6564  ", "Plot reduced
-00011ad0: 206f 6273 6572 7661 7469 6f20 6461 7461   observatio data
-00011ae0: 2c20 6966 2061 7661 696c 626c 652e 2229  , if availble.")
-00011af0: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
-00011b00: 6865 636b 426f 785f 6f62 735f 706c 6f74  heckBox_obs_plot
-00011b10: 5f72 6564 7563 6564 5f6f 6273 6572 7661  _reduced_observa
-00011b20: 7469 6f6e 732e 7365 7454 6578 7428 5f74  tions.setText(_t
-00011b30: 7261 6e73 6c61 7465 2822 4d61 696e 5769  ranslate("MainWi
-00011b40: 6e64 6f77 222c 2022 506c 6f74 2072 6564  ndow", "Plot red
-00011b50: 7563 6564 206f 6273 6572 7661 7469 6f6e  uced observation
-00011b60: 7322 2929 0a20 2020 2020 2020 2073 656c  s")).        sel
-00011b70: 662e 6368 6563 6b42 6f78 5f6f 6273 5f70  f.checkBox_obs_p
-00011b80: 6c6f 745f 7365 7475 705f 6461 7461 2e73  lot_setup_data.s
-00011b90: 6574 546f 6f6c 5469 7028 5f74 7261 6e73  etToolTip(_trans
-00011ba0: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
-00011bb0: 222c 2022 506c 6f74 2076 6172 6961 6e63  ", "Plot varianc
-00011bc0: 652d 7765 6967 6874 6564 206d 6561 6e20  e-weighted mean 
-00011bd0: 6f66 206f 6273 6572 7661 7469 6f6e 2064  of observation d
-00011be0: 6174 6120 666f 7220 616c 6c20 7365 7475  ata for all setu
-00011bf0: 7073 2e22 2929 0a20 2020 2020 2020 2073  ps.")).        s
-00011c00: 656c 662e 6368 6563 6b42 6f78 5f6f 6273  elf.checkBox_obs
-00011c10: 5f70 6c6f 745f 7365 7475 705f 6461 7461  _plot_setup_data
-00011c20: 2e73 6574 5465 7874 285f 7472 616e 736c  .setText(_transl
-00011c30: 6174 6528 224d 6169 6e57 696e 646f 7722  ate("MainWindow"
-00011c40: 2c20 2250 6c6f 7420 7365 7475 7020 6461  , "Plot setup da
-00011c50: 7461 2229 290a 2020 2020 2020 2020 7365  ta")).        se
-00011c60: 6c66 2e74 6162 5769 6467 6574 5f6f 6273  lf.tabWidget_obs
-00011c70: 6572 7661 7469 6f6e 732e 7365 7454 6162  ervations.setTab
-00011c80: 5465 7874 2873 656c 662e 7461 6257 6964  Text(self.tabWid
-00011c90: 6765 745f 6f62 7365 7276 6174 696f 6e73  get_observations
-00011ca0: 2e69 6e64 6578 4f66 2873 656c 662e 7461  .indexOf(self.ta
-00011cb0: 625f 6f62 7365 7276 6174 696f 6e73 5f70  b_observations_p
-00011cc0: 6c6f 7473 292c 205f 7472 616e 736c 6174  lots), _translat
-00011cd0: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
-00011ce0: 224f 6273 6572 7661 7469 6f6e 2070 6c6f  "Observation plo
-00011cf0: 7473 2229 290a 2020 2020 2020 2020 7365  ts")).        se
-00011d00: 6c66 2e74 6162 5769 6467 6574 5f6f 6273  lf.tabWidget_obs
-00011d10: 6572 7661 7469 6f6e 732e 7365 7454 6162  ervations.setTab
-00011d20: 5465 7874 2873 656c 662e 7461 6257 6964  Text(self.tabWid
-00011d30: 6765 745f 6f62 7365 7276 6174 696f 6e73  get_observations
-00011d40: 2e69 6e64 6578 4f66 2873 656c 662e 7461  .indexOf(self.ta
-00011d50: 625f 6f62 7365 7276 6174 696f 6e73 5f74  b_observations_t
-00011d60: 6162 6c65 292c 205f 7472 616e 736c 6174  able), _translat
-00011d70: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
-00011d80: 224f 6273 6572 7661 7469 6f6e 7320 7461  "Observations ta
-00011d90: 626c 6522 2929 0a20 2020 2020 2020 2073  ble")).        s
-00011da0: 656c 662e 7461 6257 6964 6765 745f 6f62  elf.tabWidget_ob
-00011db0: 7365 7276 6174 696f 6e73 2e73 6574 5461  servations.setTa
-00011dc0: 6254 6578 7428 7365 6c66 2e74 6162 5769  bText(self.tabWi
-00011dd0: 6467 6574 5f6f 6273 6572 7661 7469 6f6e  dget_observation
-00011de0: 732e 696e 6465 784f 6628 7365 6c66 2e74  s.indexOf(self.t
-00011df0: 6162 5f73 7572 7665 7973 292c 205f 7472  ab_surveys), _tr
-00011e00: 616e 736c 6174 6528 224d 6169 6e57 696e  anslate("MainWin
-00011e10: 646f 7722 2c20 2253 7572 7665 7973 2229  dow", "Surveys")
-00011e20: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
-00011e30: 726f 7570 426f 785f 6f62 735f 7365 7475  roupBox_obs_setu
-00011e40: 7073 5f61 7070 6c69 6564 5f63 6f72 7265  ps_applied_corre
-00011e50: 6374 696f 6e73 2e73 6574 546f 6f6c 5469  ctions.setToolTi
-00011e60: 7028 5f74 7261 6e73 6c61 7465 2822 4d61  p(_translate("Ma
-00011e70: 696e 5769 6e64 6f77 222c 2022 496e 666f  inWindow", "Info
-00011e80: 726d 6174 696f 6e20 6f6e 2074 6865 2063  rmation on the c
-00011e90: 6f72 7265 6374 696f 6e73 2074 6861 7420  orrections that 
-00011ea0: 6861 7665 2062 6565 6e20 6170 706c 6965  have been applie
-00011eb0: 6420 6f6e 2074 6865 206f 6273 6572 7661  d on the observa
-00011ec0: 7469 6f6e 7320 6f6e 2077 6869 6368 2074  tions on which t
-00011ed0: 6865 2073 6574 7570 2064 6174 6120 6973  he setup data is
-00011ee0: 2062 6173 6564 206f 6e2e 2229 290a 2020   based on.")).  
-00011ef0: 2020 2020 2020 7365 6c66 2e67 726f 7570        self.group
-00011f00: 426f 785f 6f62 735f 7365 7475 7073 5f61  Box_obs_setups_a
-00011f10: 7070 6c69 6564 5f63 6f72 7265 6374 696f  pplied_correctio
-00011f20: 6e73 2e73 6574 5469 746c 6528 5f74 7261  ns.setTitle(_tra
-00011f30: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
-00011f40: 6f77 222c 2022 4170 706c 6965 6420 636f  ow", "Applied co
-00011f50: 7272 6563 7469 6f6e 733a 2229 290a 2020  rrections:")).  
-00011f60: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
-00011f70: 5f6f 6273 5f73 6574 7570 735f 312e 7365  _obs_setups_1.se
-00011f80: 7454 6f6f 6c54 6970 285f 7472 616e 736c  tToolTip(_transl
-00011f90: 6174 6528 224d 6169 6e57 696e 646f 7722  ate("MainWindow"
-00011fa0: 2c20 2254 7970 6520 6f66 2061 7070 6c69  , "Type of appli
-00011fb0: 6564 2074 6964 616c 2063 6f72 7265 6374  ed tidal correct
-00011fc0: 696f 6e73 2e22 2929 0a20 2020 2020 2020  ions.")).       
-00011fd0: 2073 656c 662e 6c61 6265 6c5f 6f62 735f   self.label_obs_
-00011fe0: 7365 7475 7073 5f31 2e73 6574 5465 7874  setups_1.setText
-00011ff0: 285f 7472 616e 736c 6174 6528 224d 6169  (_translate("Mai
-00012000: 6e57 696e 646f 7722 2c20 2254 6964 616c  nWindow", "Tidal
-00012010: 2063 6f72 7265 6374 696f 6e3a 2229 290a   correction:")).
-00012020: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
-00012030: 656c 5f6f 6273 5f73 6574 7570 735f 7469  el_obs_setups_ti
-00012040: 6461 6c5f 636f 7272 2e73 6574 546f 6f6c  dal_corr.setTool
-00012050: 5469 7028 5f74 7261 6e73 6c61 7465 2822  Tip(_translate("
-00012060: 4d61 696e 5769 6e64 6f77 222c 2022 5479  MainWindow", "Ty
-00012070: 7065 206f 6620 6170 706c 6965 6420 7469  pe of applied ti
-00012080: 6461 6c20 636f 7272 6563 7469 6f6e 732e  dal corrections.
-00012090: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
-000120a0: 2e6c 6162 656c 5f6f 6273 5f73 6574 7570  .label_obs_setup
-000120b0: 735f 322e 7365 7454 6f6f 6c54 6970 285f  s_2.setToolTip(_
-000120c0: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
-000120d0: 696e 646f 7722 2c20 2254 7970 6520 6f66  indow", "Type of
-000120e0: 2074 6865 2061 7070 6c69 6564 2072 6566   the applied ref
-000120f0: 6572 656e 6365 2068 6569 6768 7420 7265  erence height re
-00012100: 6475 6374 696f 6e2e 2229 290a 2020 2020  duction.")).    
-00012110: 2020 2020 7365 6c66 2e6c 6162 656c 5f6f      self.label_o
-00012120: 6273 5f73 6574 7570 735f 322e 7365 7454  bs_setups_2.setT
-00012130: 6578 7428 5f74 7261 6e73 6c61 7465 2822  ext(_translate("
-00012140: 4d61 696e 5769 6e64 6f77 222c 2022 4f62  MainWindow", "Ob
-00012150: 732e 2072 6566 6572 656e 6365 2068 6569  s. reference hei
-00012160: 6768 743a 2229 290a 2020 2020 2020 2020  ght:")).        
-00012170: 7365 6c66 2e6c 6162 656c 5f6f 6273 5f73  self.label_obs_s
-00012180: 6574 7570 735f 7265 665f 6865 6967 6874  etups_ref_height
-00012190: 2e73 6574 546f 6f6c 5469 7028 5f74 7261  .setToolTip(_tra
-000121a0: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
-000121b0: 6f77 222c 2022 5479 7065 206f 6620 7468  ow", "Type of th
-000121c0: 6520 6170 706c 6965 6420 7265 6665 7265  e applied refere
-000121d0: 6e63 6520 6865 6967 6874 2072 6564 7563  nce height reduc
-000121e0: 7469 6f6e 2e22 2929 0a20 2020 2020 2020  tion.")).       
-000121f0: 2073 656c 662e 6c61 6265 6c5f 3237 2e73   self.label_27.s
-00012200: 6574 5465 7874 285f 7472 616e 736c 6174  etText(_translat
-00012210: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
-00012220: 2253 6361 6c65 2043 6f72 7265 6374 696f  "Scale Correctio
-00012230: 6e3a 2229 290a 2020 2020 2020 2020 7365  n:")).        se
-00012240: 6c66 2e6c 6162 656c 5f6f 6273 5f73 6574  lf.label_obs_set
-00012250: 7570 735f 332e 7365 7454 6578 7428 5f74  ups_3.setText(_t
+0000fcc0: 2073 656c 662e 6d65 6e75 5f46 696c 652e   self.menu_File.
+0000fcd0: 6164 6441 6374 696f 6e28 7365 6c66 2e6d  addAction(self.m
+0000fce0: 656e 755f 4164 645f 5374 6174 696f 6e73  enu_Add_Stations
+0000fcf0: 2e6d 656e 7541 6374 696f 6e28 2929 0a20  .menuAction()). 
+0000fd00: 2020 2020 2020 2073 656c 662e 6d65 6e75         self.menu
+0000fd10: 5f46 696c 652e 6164 6441 6374 696f 6e28  _File.addAction(
+0000fd20: 7365 6c66 2e6d 656e 755f 4164 645f 4772  self.menu_Add_Gr
+0000fd30: 6176 696d 6574 6572 732e 6d65 6e75 4163  avimeters.menuAc
+0000fd40: 7469 6f6e 2829 290a 2020 2020 2020 2020  tion()).        
+0000fd50: 7365 6c66 2e6d 656e 755f 4669 6c65 2e61  self.menu_File.a
+0000fd60: 6464 5365 7061 7261 746f 7228 290a 2020  ddSeparator().  
+0000fd70: 2020 2020 2020 7365 6c66 2e6d 656e 755f        self.menu_
+0000fd80: 4669 6c65 2e61 6464 4163 7469 6f6e 2873  File.addAction(s
+0000fd90: 656c 662e 6163 7469 6f6e 5f45 7870 6f72  elf.action_Expor
+0000fda0: 745f 5265 7375 6c74 7329 0a20 2020 2020  t_Results).     
+0000fdb0: 2020 2073 656c 662e 6d65 6e75 5f46 696c     self.menu_Fil
+0000fdc0: 652e 6164 6453 6570 6172 6174 6f72 2829  e.addSeparator()
+0000fdd0: 0a20 2020 2020 2020 2073 656c 662e 6d65  .        self.me
+0000fde0: 6e75 5f46 696c 652e 6164 6441 6374 696f  nu_File.addActio
+0000fdf0: 6e28 7365 6c66 2e61 6374 696f 6e5f 4f70  n(self.action_Op
+0000fe00: 7469 6f6e 7329 0a20 2020 2020 2020 2073  tions).        s
+0000fe10: 656c 662e 6d65 6e75 5f46 696c 652e 6164  elf.menu_File.ad
+0000fe20: 6453 6570 6172 6174 6f72 2829 0a20 2020  dSeparator().   
+0000fe30: 2020 2020 2073 656c 662e 6d65 6e75 5f46       self.menu_F
+0000fe40: 696c 652e 6164 6441 6374 696f 6e28 7365  ile.addAction(se
+0000fe50: 6c66 2e61 6374 696f 6e5f 4578 6974 290a  lf.action_Exit).
+0000fe60: 2020 2020 2020 2020 7365 6c66 2e6d 656e          self.men
+0000fe70: 755f 4f62 7365 7276 6174 696f 6e73 2e61  u_Observations.a
+0000fe80: 6464 5365 7061 7261 746f 7228 290a 2020  ddSeparator().  
+0000fe90: 2020 2020 2020 7365 6c66 2e6d 656e 755f        self.menu_
+0000fea0: 4f62 7365 7276 6174 696f 6e73 2e61 6464  Observations.add
+0000feb0: 4163 7469 6f6e 2873 656c 662e 6163 7469  Action(self.acti
+0000fec0: 6f6e 5f41 7574 6f73 656c 6563 7469 6f6e  on_Autoselection
+0000fed0: 5f73 6574 7469 6e67 7329 0a20 2020 2020  _settings).     
+0000fee0: 2020 2073 656c 662e 6d65 6e75 5f4f 6273     self.menu_Obs
+0000fef0: 6572 7661 7469 6f6e 732e 6164 6441 6374  ervations.addAct
+0000ff00: 696f 6e28 7365 6c66 2e61 6374 696f 6e5f  ion(self.action_
+0000ff10: 5365 7475 705f 6461 7461 5f6f 7074 696f  Setup_data_optio
+0000ff20: 6e73 290a 2020 2020 2020 2020 7365 6c66  ns).        self
+0000ff30: 2e6d 656e 755f 4f62 7365 7276 6174 696f  .menu_Observatio
+0000ff40: 6e73 2e61 6464 4163 7469 6f6e 2873 656c  ns.addAction(sel
+0000ff50: 662e 6163 7469 6f6e 5f46 6c61 675f 6f62  f.action_Flag_ob
+0000ff60: 7365 7276 6174 696f 6e73 290a 2020 2020  servations).    
+0000ff70: 2020 2020 7365 6c66 2e6d 656e 7545 7374      self.menuEst
+0000ff80: 696d 6174 696f 6e5f 7365 7474 696e 6773  imation_settings
+0000ff90: 2e61 6464 4163 7469 6f6e 2873 656c 662e  .addAction(self.
+0000ffa0: 6163 7469 6f6e 5f45 7374 696d 6174 696f  action_Estimatio
+0000ffb0: 6e5f 7365 7474 696e 6773 290a 2020 2020  n_settings).    
+0000ffc0: 2020 2020 7365 6c66 2e6d 656e 7545 7374      self.menuEst
+0000ffd0: 696d 6174 696f 6e5f 7365 7474 696e 6773  imation_settings
+0000ffe0: 2e61 6464 4163 7469 6f6e 2873 656c 662e  .addAction(self.
+0000fff0: 6163 7469 6f6e 5f47 6973 5f45 7870 6f72  action_Gis_Expor
+00010000: 745f 7365 7474 696e 6773 290a 2020 2020  t_settings).    
+00010010: 2020 2020 7365 6c66 2e6d 656e 7548 656c      self.menuHel
+00010020: 702e 6164 6441 6374 696f 6e28 7365 6c66  p.addAction(self
+00010030: 2e61 6374 696f 6e5f 4162 6f75 7429 0a20  .action_About). 
+00010040: 2020 2020 2020 2073 656c 662e 6d65 6e75         self.menu
+00010050: 436f 7272 6563 7469 6f6e 732e 6164 6441  Corrections.addA
+00010060: 6374 696f 6e28 7365 6c66 2e61 6374 696f  ction(self.actio
+00010070: 6e5f 436f 7272 6563 7469 6f6e 7329 0a20  n_Corrections). 
+00010080: 2020 2020 2020 2073 656c 662e 6d65 6e75         self.menu
+00010090: 436f 7272 6563 7469 6f6e 732e 6164 6441  Corrections.addA
+000100a0: 6374 696f 6e28 7365 6c66 2e61 6374 696f  ction(self.actio
+000100b0: 6e5f 436f 7272 6563 7469 6f6e 5f74 696d  n_Correction_tim
+000100c0: 655f 7365 7269 6573 290a 2020 2020 2020  e_series).      
+000100d0: 2020 7365 6c66 2e6d 656e 7562 6172 2e61    self.menubar.a
+000100e0: 6464 4163 7469 6f6e 2873 656c 662e 6d65  ddAction(self.me
+000100f0: 6e75 5f46 696c 652e 6d65 6e75 4163 7469  nu_File.menuActi
+00010100: 6f6e 2829 290a 2020 2020 2020 2020 7365  on()).        se
+00010110: 6c66 2e6d 656e 7562 6172 2e61 6464 4163  lf.menubar.addAc
+00010120: 7469 6f6e 2873 656c 662e 6d65 6e75 5f4f  tion(self.menu_O
+00010130: 6273 6572 7661 7469 6f6e 732e 6d65 6e75  bservations.menu
+00010140: 4163 7469 6f6e 2829 290a 2020 2020 2020  Action()).      
+00010150: 2020 7365 6c66 2e6d 656e 7562 6172 2e61    self.menubar.a
+00010160: 6464 4163 7469 6f6e 2873 656c 662e 6d65  ddAction(self.me
+00010170: 6e75 4573 7469 6d61 7469 6f6e 5f73 6574  nuEstimation_set
+00010180: 7469 6e67 732e 6d65 6e75 4163 7469 6f6e  tings.menuAction
+00010190: 2829 290a 2020 2020 2020 2020 7365 6c66  ()).        self
+000101a0: 2e6d 656e 7562 6172 2e61 6464 4163 7469  .menubar.addActi
+000101b0: 6f6e 2873 656c 662e 6d65 6e75 436f 7272  on(self.menuCorr
+000101c0: 6563 7469 6f6e 732e 6d65 6e75 4163 7469  ections.menuActi
+000101d0: 6f6e 2829 290a 2020 2020 2020 2020 7365  on()).        se
+000101e0: 6c66 2e6d 656e 7562 6172 2e61 6464 4163  lf.menubar.addAc
+000101f0: 7469 6f6e 2873 656c 662e 6d65 6e75 4865  tion(self.menuHe
+00010200: 6c70 2e6d 656e 7541 6374 696f 6e28 2929  lp.menuAction())
+00010210: 0a0a 2020 2020 2020 2020 7365 6c66 2e72  ..        self.r
+00010220: 6574 7261 6e73 6c61 7465 5569 284d 6169  etranslateUi(Mai
+00010230: 6e57 696e 646f 7729 0a20 2020 2020 2020  nWindow).       
+00010240: 2073 656c 662e 7461 6257 6964 6765 745f   self.tabWidget_
+00010250: 4d61 696e 2e73 6574 4375 7272 656e 7449  Main.setCurrentI
+00010260: 6e64 6578 2832 290a 2020 2020 2020 2020  ndex(2).        
+00010270: 7365 6c66 2e74 6162 5f57 6964 6765 745f  self.tab_Widget_
+00010280: 5374 6174 696f 6e73 2e73 6574 4375 7272  Stations.setCurr
+00010290: 656e 7449 6e64 6578 2830 290a 2020 2020  entIndex(0).    
+000102a0: 2020 2020 7365 6c66 2e74 6162 5769 6467      self.tabWidg
+000102b0: 6574 5f67 7261 7669 6d65 7465 7273 2e73  et_gravimeters.s
+000102c0: 6574 4375 7272 656e 7449 6e64 6578 2830  etCurrentIndex(0
+000102d0: 290a 2020 2020 2020 2020 7365 6c66 2e74  ).        self.t
+000102e0: 6162 5769 6467 6574 5f6f 6273 6572 7661  abWidget_observa
+000102f0: 7469 6f6e 732e 7365 7443 7572 7265 6e74  tions.setCurrent
+00010300: 496e 6465 7828 3029 0a20 2020 2020 2020  Index(0).       
+00010310: 2073 656c 662e 7461 6257 6964 6765 745f   self.tabWidget_
+00010320: 7265 7375 6c74 732e 7365 7443 7572 7265  results.setCurre
+00010330: 6e74 496e 6465 7828 3029 0a20 2020 2020  ntIndex(0).     
+00010340: 2020 2073 656c 662e 7261 6469 6f42 7574     self.radioBut
+00010350: 746f 6e5f 7265 7375 6c74 735f 6f62 735f  ton_results_obs_
+00010360: 706c 6f74 5f68 6973 746f 6772 616d 2e74  plot_histogram.t
+00010370: 6f67 676c 6564 5b27 626f 6f6c 275d 2e63  oggled['bool'].c
+00010380: 6f6e 6e65 6374 2873 656c 662e 6772 6f75  onnect(self.grou
+00010390: 7042 6f78 5f68 6973 746f 6772 616d 5f73  pBox_histogram_s
+000103a0: 6574 7469 6e67 732e 7365 7445 6e61 626c  ettings.setEnabl
+000103b0: 6564 2920 2320 7479 7065 3a20 6967 6e6f  ed) # type: igno
+000103c0: 7265 0a20 2020 2020 2020 2073 656c 662e  re.        self.
+000103d0: 6368 6563 6b42 6f78 5f73 7461 7469 6f6e  checkBox_station
+000103e0: 735f 706c 6f74 5f6f 6273 5f6d 6170 2e74  s_plot_obs_map.t
+000103f0: 6f67 676c 6564 5b27 626f 6f6c 275d 2e63  oggled['bool'].c
+00010400: 6f6e 6e65 6374 2873 656c 662e 636f 6d62  onnect(self.comb
+00010410: 6f42 6f78 5f73 7461 7469 6f6e 735f 706c  oBox_stations_pl
+00010420: 6f74 5f6f 6273 5f6d 6170 5f73 7572 7665  ot_obs_map_surve
+00010430: 7973 2e73 6574 456e 6162 6c65 6429 2023  ys.setEnabled) #
+00010440: 2074 7970 653a 2069 676e 6f72 650a 2020   type: ignore.  
+00010450: 2020 2020 2020 5174 436f 7265 2e51 4d65        QtCore.QMe
+00010460: 7461 4f62 6a65 6374 2e63 6f6e 6e65 6374  taObject.connect
+00010470: 536c 6f74 7342 794e 616d 6528 4d61 696e  SlotsByName(Main
+00010480: 5769 6e64 6f77 290a 0a20 2020 2064 6566  Window)..    def
+00010490: 2072 6574 7261 6e73 6c61 7465 5569 2873   retranslateUi(s
+000104a0: 656c 662c 204d 6169 6e57 696e 646f 7729  elf, MainWindow)
+000104b0: 3a0a 2020 2020 2020 2020 5f74 7261 6e73  :.        _trans
+000104c0: 6c61 7465 203d 2051 7443 6f72 652e 5143  late = QtCore.QC
+000104d0: 6f72 6541 7070 6c69 6361 7469 6f6e 2e74  oreApplication.t
+000104e0: 7261 6e73 6c61 7465 0a20 2020 2020 2020  ranslate.       
+000104f0: 204d 6169 6e57 696e 646f 772e 7365 7457   MainWindow.setW
+00010500: 696e 646f 7754 6974 6c65 285f 7472 616e  indowTitle(_tran
+00010510: 736c 6174 6528 224d 6169 6e57 696e 646f  slate("MainWindo
+00010520: 7722 2c20 2247 7261 7654 6f6f 6c73 2229  w", "GravTools")
+00010530: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
+00010540: 726f 7570 426f 785f 6669 6c74 6572 5f6f  roupBox_filter_o
+00010550: 7074 696f 6e73 2e73 6574 546f 6f6c 5469  ptions.setToolTi
+00010560: 7028 5f74 7261 6e73 6c61 7465 2822 4d61  p(_translate("Ma
+00010570: 696e 5769 6e64 6f77 222c 2022 4469 7370  inWindow", "Disp
+00010580: 6c61 7920 6f70 7469 6f6e 7320 666f 7220  lay options for 
+00010590: 7374 6174 696f 6e73 2229 290a 2020 2020  stations")).    
+000105a0: 2020 2020 7365 6c66 2e67 726f 7570 426f      self.groupBo
+000105b0: 785f 6669 6c74 6572 5f6f 7074 696f 6e73  x_filter_options
+000105c0: 2e73 6574 5469 746c 6528 5f74 7261 6e73  .setTitle(_trans
+000105d0: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
+000105e0: 222c 2022 4669 6c74 6572 204f 7074 696f  ", "Filter Optio
+000105f0: 6e73 2229 290a 2020 2020 2020 2020 7365  ns")).        se
+00010600: 6c66 2e63 6865 636b 426f 785f 6669 6c74  lf.checkBox_filt
+00010610: 6572 5f6f 6273 6572 7665 645f 7374 6174  er_observed_stat
+00010620: 5f6f 6e6c 792e 7365 7454 6f6f 6c54 6970  _only.setToolTip
+00010630: 285f 7472 616e 736c 6174 6528 224d 6169  (_translate("Mai
+00010640: 6e57 696e 646f 7722 2c20 2244 6973 706c  nWindow", "Displ
+00010650: 6179 206f 6e6c 7920 7374 6174 696f 6e73  ay only stations
+00010660: 2074 6861 7420 7765 7265 206f 6273 6572   that were obser
+00010670: 7665 6420 696e 2074 6869 7320 6361 6d70  ved in this camp
+00010680: 6169 676e 2e20 2229 290a 2020 2020 2020  aign. ")).      
+00010690: 2020 7365 6c66 2e63 6865 636b 426f 785f    self.checkBox_
+000106a0: 6669 6c74 6572 5f6f 6273 6572 7665 645f  filter_observed_
+000106b0: 7374 6174 5f6f 6e6c 792e 7365 7454 6578  stat_only.setTex
+000106c0: 7428 5f74 7261 6e73 6c61 7465 2822 4d61  t(_translate("Ma
+000106d0: 696e 5769 6e64 6f77 222c 2022 4f62 7365  inWindow", "Obse
+000106e0: 7276 6564 206f 6e6c 7922 2929 0a20 2020  rved only")).   
+000106f0: 2020 2020 2073 656c 662e 6c61 6265 6c2e       self.label.
+00010700: 7365 7454 6578 7428 5f74 7261 6e73 6c61  setText(_transla
+00010710: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
+00010720: 2022 5374 6174 696f 6e20 6e61 6d65 2066   "Station name f
+00010730: 696c 7465 7220 2872 6567 6578 2922 2929  ilter (regex)"))
+00010740: 0a20 2020 2020 2020 2073 656c 662e 6772  .        self.gr
+00010750: 6f75 7042 6f78 5f73 7461 7469 6f6e 735f  oupBox_stations_
+00010760: 6d61 705f 7669 6577 5f6f 7074 696f 6e73  map_view_options
+00010770: 2e73 6574 5469 746c 6528 5f74 7261 6e73  .setTitle(_trans
+00010780: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
+00010790: 222c 2022 4d61 7020 7669 6577 206f 7074  ", "Map view opt
+000107a0: 696f 6e73 2229 290a 2020 2020 2020 2020  ions")).        
+000107b0: 7365 6c66 2e63 6865 636b 426f 785f 7374  self.checkBox_st
+000107c0: 6174 696f 6e73 5f6d 6170 5f73 686f 775f  ations_map_show_
+000107d0: 7374 6174 5f6e 616d 655f 6c61 6265 6c73  stat_name_labels
+000107e0: 2e73 6574 5465 7874 285f 7472 616e 736c  .setText(_transl
+000107f0: 6174 6528 224d 6169 6e57 696e 646f 7722  ate("MainWindow"
+00010800: 2c20 2253 686f 7720 7374 6174 696f 6e20  , "Show station 
+00010810: 6e61 6d65 206c 6162 656c 7322 2929 0a20  name labels")). 
+00010820: 2020 2020 2020 2073 656c 662e 6368 6563         self.chec
+00010830: 6b42 6f78 5f73 7461 7469 6f6e 735f 706c  kBox_stations_pl
+00010840: 6f74 5f6f 6273 5f6d 6170 2e73 6574 546f  ot_obs_map.setTo
+00010850: 6f6c 5469 7028 5f74 7261 6e73 6c61 7465  olTip(_translate
+00010860: 2822 4d61 696e 5769 6e64 6f77 222c 2022  ("MainWindow", "
+00010870: 3c68 746d 6c3e 3c68 6561 642f 3e3c 626f  <html><head/><bo
+00010880: 6479 3e3c 703e 506c 6f74 206f 6273 6572  dy><p>Plot obser
+00010890: 7661 7469 6f6e 7320 696e 2074 6572 6d73  vations in terms
+000108a0: 206f 6620 6c69 6e65 7320 696e 2074 6865   of lines in the
+000108b0: 2073 7461 7469 6f6e 2070 6c6f 7420 6163   station plot ac
+000108c0: 636f 7264 696e 6720 746f 2074 6865 2073  cording to the s
+000108d0: 656c 6563 7469 6f6e 2062 656c 6f77 2e3c  election below.<
+000108e0: 2f70 3e3c 2f62 6f64 793e 3c2f 6874 6d6c  /p></body></html
+000108f0: 3e22 2929 0a20 2020 2020 2020 2073 656c  >")).        sel
+00010900: 662e 6368 6563 6b42 6f78 5f73 7461 7469  f.checkBox_stati
+00010910: 6f6e 735f 706c 6f74 5f6f 6273 5f6d 6170  ons_plot_obs_map
+00010920: 2e73 6574 5465 7874 285f 7472 616e 736c  .setText(_transl
+00010930: 6174 6528 224d 6169 6e57 696e 646f 7722  ate("MainWindow"
+00010940: 2c20 2250 6c6f 7420 6f62 7365 7276 6174  , "Plot observat
+00010950: 696f 6e73 2229 290a 2020 2020 2020 2020  ions")).        
+00010960: 7365 6c66 2e63 6f6d 626f 426f 785f 7374  self.comboBox_st
+00010970: 6174 696f 6e73 5f70 6c6f 745f 6f62 735f  ations_plot_obs_
+00010980: 6d61 705f 7375 7276 6579 732e 7365 7454  map_surveys.setT
+00010990: 6f6f 6c54 6970 285f 7472 616e 736c 6174  oolTip(_translat
+000109a0: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
+000109b0: 223c 6874 6d6c 3e3c 6865 6164 2f3e 3c62  "<html><head/><b
+000109c0: 6f64 793e 3c70 3e53 656c 6563 7420 7768  ody><p>Select wh
+000109d0: 6574 6865 7220 6f62 7365 7276 6174 696f  ether observatio
+000109e0: 6e73 206f 6620 616c 6c20 7375 7276 6579  ns of all survey
+000109f0: 732c 206f 7220 6f66 2061 2073 656c 6563  s, or of a selec
+00010a00: 7465 6420 7375 7276 6579 2073 686f 756c  ted survey shoul
+00010a10: 6420 6265 2070 6c6f 7474 6564 2069 6e20  d be plotted in 
+00010a20: 7468 6520 7374 6174 696f 6e20 6d61 702e  the station map.
+00010a30: 3c2f 703e 3c2f 626f 6479 3e3c 2f68 746d  </p></body></htm
+00010a40: 6c3e 2229 290a 2020 2020 2020 2020 7365  l>")).        se
+00010a50: 6c66 2e74 6162 5f57 6964 6765 745f 5374  lf.tab_Widget_St
+00010a60: 6174 696f 6e73 2e73 6574 5461 6254 6578  ations.setTabTex
+00010a70: 7428 7365 6c66 2e74 6162 5f57 6964 6765  t(self.tab_Widge
+00010a80: 745f 5374 6174 696f 6e73 2e69 6e64 6578  t_Stations.index
+00010a90: 4f66 2873 656c 662e 7461 625f 5374 6174  Of(self.tab_Stat
+00010aa0: 696f 6e73 5f54 6162 6c65 292c 205f 7472  ions_Table), _tr
+00010ab0: 616e 736c 6174 6528 224d 6169 6e57 696e  anslate("MainWin
+00010ac0: 646f 7722 2c20 2254 6162 6c65 2229 290a  dow", "Table")).
+00010ad0: 2020 2020 2020 2020 7365 6c66 2e74 6162          self.tab
+00010ae0: 5f57 6964 6765 745f 5374 6174 696f 6e73  _Widget_Stations
+00010af0: 2e73 6574 5461 6254 6578 7428 7365 6c66  .setTabText(self
+00010b00: 2e74 6162 5f57 6964 6765 745f 5374 6174  .tab_Widget_Stat
+00010b10: 696f 6e73 2e69 6e64 6578 4f66 2873 656c  ions.indexOf(sel
+00010b20: 662e 7461 625f 7374 6174 696f 6e73 5f6d  f.tab_stations_m
+00010b30: 6170 292c 205f 7472 616e 736c 6174 6528  ap), _translate(
+00010b40: 224d 6169 6e57 696e 646f 7722 2c20 224d  "MainWindow", "M
+00010b50: 6170 2229 290a 2020 2020 2020 2020 7365  ap")).        se
+00010b60: 6c66 2e74 6162 5769 6467 6574 5f4d 6169  lf.tabWidget_Mai
+00010b70: 6e2e 7365 7454 6162 5465 7874 2873 656c  n.setTabText(sel
+00010b80: 662e 7461 6257 6964 6765 745f 4d61 696e  f.tabWidget_Main
+00010b90: 2e69 6e64 6578 4f66 2873 656c 662e 7461  .indexOf(self.ta
+00010ba0: 625f 6d61 696e 5f73 7461 7469 6f6e 7329  b_main_stations)
+00010bb0: 2c20 5f74 7261 6e73 6c61 7465 2822 4d61  , _translate("Ma
+00010bc0: 696e 5769 6e64 6f77 222c 2022 5374 6174  inWindow", "Stat
+00010bd0: 696f 6e73 2229 290a 2020 2020 2020 2020  ions")).        
+00010be0: 7365 6c66 2e74 7265 6557 6964 6765 745f  self.treeWidget_
+00010bf0: 6772 6176 696d 6574 6572 732e 6865 6164  gravimeters.head
+00010c00: 6572 4974 656d 2829 2e73 6574 5465 7874  erItem().setText
+00010c10: 2830 2c20 5f74 7261 6e73 6c61 7465 2822  (0, _translate("
+00010c20: 4d61 696e 5769 6e64 6f77 222c 2022 5479  MainWindow", "Ty
+00010c30: 7065 2229 290a 2020 2020 2020 2020 7365  pe")).        se
+00010c40: 6c66 2e74 7265 6557 6964 6765 745f 6772  lf.treeWidget_gr
+00010c50: 6176 696d 6574 6572 732e 6865 6164 6572  avimeters.header
+00010c60: 4974 656d 2829 2e73 6574 5465 7874 2831  Item().setText(1
+00010c70: 2c20 5f74 7261 6e73 6c61 7465 2822 4d61  , _translate("Ma
+00010c80: 696e 5769 6e64 6f77 222c 2022 532f 4e22  inWindow", "S/N"
+00010c90: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+00010ca0: 7075 7368 4275 7474 6f6e 5f64 656c 6574  pushButton_delet
+00010cb0: 655f 6772 6176 696d 6574 6572 2e73 6574  e_gravimeter.set
+00010cc0: 5465 7874 285f 7472 616e 736c 6174 6528  Text(_translate(
+00010cd0: 224d 6169 6e57 696e 646f 7722 2c20 2244  "MainWindow", "D
+00010ce0: 656c 6574 6522 2929 0a20 2020 2020 2020  elete")).       
+00010cf0: 2073 656c 662e 6c61 6265 6c5f 3139 2e73   self.label_19.s
+00010d00: 6574 546f 6f6c 5469 7028 5f74 7261 6e73  etToolTip(_trans
+00010d10: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
+00010d20: 222c 2022 4d61 6e75 6661 6374 7572 6572  ", "Manufacturer
+00010d30: 206f 6620 696e 7374 7275 6d65 6e74 2e22   of instrument."
+00010d40: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+00010d50: 6c61 6265 6c5f 3139 2e73 6574 5465 7874  label_19.setText
+00010d60: 285f 7472 616e 736c 6174 6528 224d 6169  (_translate("Mai
+00010d70: 6e57 696e 646f 7722 2c20 224d 616e 7566  nWindow", "Manuf
+00010d80: 6163 7475 7265 723a 2229 290a 2020 2020  acturer:")).    
+00010d90: 2020 2020 7365 6c66 2e6c 6162 656c 5f67      self.label_g
+00010da0: 7261 7669 5f6d 616e 7566 6163 7475 7265  ravi_manufacture
+00010db0: 722e 7365 7454 6f6f 6c54 6970 285f 7472  r.setToolTip(_tr
+00010dc0: 616e 736c 6174 6528 224d 6169 6e57 696e  anslate("MainWin
+00010dd0: 646f 7722 2c20 224d 616e 7566 6163 7475  dow", "Manufactu
+00010de0: 7265 7220 6f66 2069 6e73 7472 756d 656e  rer of instrumen
+00010df0: 742e 2229 290a 2020 2020 2020 2020 7365  t.")).        se
+00010e00: 6c66 2e6c 6162 656c 5f32 302e 7365 7454  lf.label_20.setT
+00010e10: 6f6f 6c54 6970 285f 7472 616e 736c 6174  oolTip(_translat
+00010e20: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
+00010e30: 2247 7261 7669 6d65 7465 7220 7479 7065  "Gravimeter type
+00010e40: 2e22 2929 0a20 2020 2020 2020 2073 656c  .")).        sel
+00010e50: 662e 6c61 6265 6c5f 3230 2e73 6574 5465  f.label_20.setTe
+00010e60: 7874 285f 7472 616e 736c 6174 6528 224d  xt(_translate("M
+00010e70: 6169 6e57 696e 646f 7722 2c20 2254 7970  ainWindow", "Typ
+00010e80: 653a 2229 290a 2020 2020 2020 2020 7365  e:")).        se
+00010e90: 6c66 2e6c 6162 656c 5f67 7261 7669 5f74  lf.label_gravi_t
+00010ea0: 7970 652e 7365 7454 6f6f 6c54 6970 285f  ype.setToolTip(_
+00010eb0: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
+00010ec0: 696e 646f 7722 2c20 2247 7261 7669 6d65  indow", "Gravime
+00010ed0: 7465 7220 7479 7065 2e22 2929 0a20 2020  ter type.")).   
+00010ee0: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
+00010ef0: 3231 2e73 6574 546f 6f6c 5469 7028 5f74  21.setToolTip(_t
+00010f00: 7261 6e73 6c61 7465 2822 4d61 696e 5769  ranslate("MainWi
+00010f10: 6e64 6f77 222c 2022 5365 7269 616c 206e  ndow", "Serial n
+00010f20: 756d 6265 722e 2229 290a 2020 2020 2020  umber.")).      
+00010f30: 2020 7365 6c66 2e6c 6162 656c 5f32 312e    self.label_21.
+00010f40: 7365 7454 6578 7428 5f74 7261 6e73 6c61  setText(_transla
+00010f50: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
+00010f60: 2022 5365 7269 616c 206e 756d 6265 723a   "Serial number:
+00010f70: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+00010f80: 2e6c 6162 656c 5f67 7261 7669 5f73 6572  .label_gravi_ser
+00010f90: 6961 6c5f 6e75 6d62 6572 2e73 6574 546f  ial_number.setTo
+00010fa0: 6f6c 5469 7028 5f74 7261 6e73 6c61 7465  olTip(_translate
+00010fb0: 2822 4d61 696e 5769 6e64 6f77 222c 2022  ("MainWindow", "
+00010fc0: 5365 7269 616c 206e 756d 6265 722e 2229  Serial number.")
+00010fd0: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
+00010fe0: 6162 656c 5f32 352e 7365 7454 6f6f 6c54  abel_25.setToolT
+00010ff0: 6970 285f 7472 616e 736c 6174 6528 224d  ip(_translate("M
+00011000: 6169 6e57 696e 646f 7722 2c20 2253 686f  ainWindow", "Sho
+00011010: 7274 2069 6e73 7472 756d 656e 7420 636f  rt instrument co
+00011020: 6465 2e22 2929 0a20 2020 2020 2020 2073  de.")).        s
+00011030: 656c 662e 6c61 6265 6c5f 3235 2e73 6574  elf.label_25.set
+00011040: 5465 7874 285f 7472 616e 736c 6174 6528  Text(_translate(
+00011050: 224d 6169 6e57 696e 646f 7722 2c20 2243  "MainWindow", "C
+00011060: 6f64 653a 2229 290a 2020 2020 2020 2020  ode:")).        
+00011070: 7365 6c66 2e6c 6162 656c 5f67 7261 7669  self.label_gravi
+00011080: 5f63 6f64 652e 7365 7454 6f6f 6c54 6970  _code.setToolTip
+00011090: 285f 7472 616e 736c 6174 6528 224d 6169  (_translate("Mai
+000110a0: 6e57 696e 646f 7722 2c20 2253 686f 7274  nWindow", "Short
+000110b0: 2069 6e73 7472 756d 656e 7420 636f 6465   instrument code
+000110c0: 2e22 2929 0a20 2020 2020 2020 2073 656c  .")).        sel
+000110d0: 662e 6c61 6265 6c5f 3232 2e73 6574 546f  f.label_22.setTo
+000110e0: 6f6c 5469 7028 5f74 7261 6e73 6c61 7465  olTip(_translate
+000110f0: 2822 4d61 696e 5769 6e64 6f77 222c 2022  ("MainWindow", "
+00011100: 3c68 746d 6c3e 3c68 6561 642f 3e3c 626f  <html><head/><bo
+00011110: 6479 3e3c 703e 4865 6967 6820 6f66 6673  dy><p>Heigh offs
+00011120: 6574 2069 6e20 6d65 7465 7273 2062 6574  et in meters bet
+00011130: 7765 656e 2069 6e73 7472 756d 656e 7420  ween instrument 
+00011140: 746f 7020 616e 6420 7365 6e73 6f72 206c  top and sensor l
+00011150: 6576 656c 2028 6e65 6761 7469 7665 2c20  evel (negative, 
+00011160: 6966 2074 6865 2073 656e 736f 7220 6973  if the sensor is
+00011170: 2062 656c 6f77 2074 6865 2074 6f70 292e   below the top).
+00011180: 3c2f 703e 3c2f 626f 6479 3e3c 2f68 746d  </p></body></htm
+00011190: 6c3e 2229 290a 2020 2020 2020 2020 7365  l>")).        se
+000111a0: 6c66 2e6c 6162 656c 5f32 322e 7365 7454  lf.label_22.setT
+000111b0: 6578 7428 5f74 7261 6e73 6c61 7465 2822  ext(_translate("
+000111c0: 4d61 696e 5769 6e64 6f77 222c 2022 4865  MainWindow", "He
+000111d0: 6967 6874 206f 6666 7365 7420 5b6d 5d3a  ight offset [m]:
+000111e0: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+000111f0: 2e6c 6162 656c 5f67 7261 7669 5f68 6569  .label_gravi_hei
+00011200: 6768 745f 6f66 6673 6574 2e73 6574 546f  ght_offset.setTo
+00011210: 6f6c 5469 7028 5f74 7261 6e73 6c61 7465  olTip(_translate
+00011220: 2822 4d61 696e 5769 6e64 6f77 222c 2022  ("MainWindow", "
+00011230: 3c68 746d 6c3e 3c68 6561 642f 3e3c 626f  <html><head/><bo
+00011240: 6479 3e3c 703e 4865 6967 6820 6f66 6673  dy><p>Heigh offs
+00011250: 6574 2069 6e20 6d65 7465 7273 2062 6574  et in meters bet
+00011260: 7765 656e 2069 6e73 7472 756d 656e 7420  ween instrument 
+00011270: 746f 7020 616e 6420 7365 6e73 6f72 206c  top and sensor l
+00011280: 6576 656c 2028 6e65 6761 7469 7665 2c20  evel (negative, 
+00011290: 6966 2074 6865 2073 656e 736f 7220 6973  if the sensor is
+000112a0: 2062 656c 6f77 2074 6865 2074 6f70 292e   below the top).
+000112b0: 3c2f 703e 3c2f 626f 6479 3e3c 2f68 746d  </p></body></htm
+000112c0: 6c3e 2229 290a 2020 2020 2020 2020 7365  l>")).        se
+000112d0: 6c66 2e6c 6162 656c 5f32 332e 7365 7454  lf.label_23.setT
+000112e0: 6f6f 6c54 6970 285f 7472 616e 736c 6174  oolTip(_translat
+000112f0: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
+00011300: 2253 6f75 7263 6520 6f66 2074 6865 2067  "Source of the g
+00011310: 7261 7669 6d65 7465 7220 6461 7461 2e20  ravimeter data. 
+00011320: 4569 7468 6572 2074 6865 206e 616d 6520  Either the name 
+00011330: 6f66 2074 6865 2073 7572 7665 7920 7468  of the survey th
+00011340: 6520 6461 7461 2077 6173 2074 616b 656e  e data was taken
+00011350: 2066 726f 6d20 286f 622e 2066 696c 6529   from (ob. file)
+00011360: 2c20 6f72 2074 6865 206e 616d 6520 6f66  , or the name of
+00011370: 2074 6865 2067 7261 7669 6d65 7465 7220   the gravimeter 
+00011380: 6669 6c65 2e22 2929 0a20 2020 2020 2020  file.")).       
+00011390: 2073 656c 662e 6c61 6265 6c5f 3233 2e73   self.label_23.s
+000113a0: 6574 5465 7874 285f 7472 616e 736c 6174  etText(_translat
+000113b0: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
+000113c0: 2244 6174 6120 736f 7572 6365 3a22 2929  "Data source:"))
+000113d0: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
+000113e0: 6265 6c5f 6772 6176 695f 6461 7461 5f73  bel_gravi_data_s
+000113f0: 6f75 7263 652e 7365 7454 6f6f 6c54 6970  ource.setToolTip
+00011400: 285f 7472 616e 736c 6174 6528 224d 6169  (_translate("Mai
+00011410: 6e57 696e 646f 7722 2c20 2253 6f75 7263  nWindow", "Sourc
+00011420: 6520 6f66 2074 6865 2067 7261 7669 6d65  e of the gravime
+00011430: 7465 7220 6461 7461 2e20 4569 7468 6572  ter data. Either
+00011440: 2074 6865 206e 616d 6520 6f66 2074 6865   the name of the
+00011450: 2073 7572 7665 7920 7468 6520 6461 7461   survey the data
+00011460: 2077 6173 2074 616b 656e 2066 726f 6d20   was taken from 
+00011470: 286f 622e 2066 696c 6529 2c20 6f72 2074  (ob. file), or t
+00011480: 6865 206e 616d 6520 6f66 2074 6865 2067  he name of the g
+00011490: 7261 7669 6d65 7465 7220 6669 6c65 2e22  ravimeter file."
+000114a0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+000114b0: 6c61 6265 6c5f 3234 2e73 6574 546f 6f6c  label_24.setTool
+000114c0: 5469 7028 5f74 7261 6e73 6c61 7465 2822  Tip(_translate("
+000114d0: 4d61 696e 5769 6e64 6f77 222c 2022 5479  MainWindow", "Ty
+000114e0: 7065 206f 6620 7468 6520 6772 6176 696d  pe of the gravim
+000114f0: 6574 6572 2064 6174 6120 736f 7572 6365  eter data source
+00011500: 2e20 2229 290a 2020 2020 2020 2020 7365  . ")).        se
+00011510: 6c66 2e6c 6162 656c 5f32 342e 7365 7454  lf.label_24.setT
+00011520: 6578 7428 5f74 7261 6e73 6c61 7465 2822  ext(_translate("
+00011530: 4d61 696e 5769 6e64 6f77 222c 2022 4461  MainWindow", "Da
+00011540: 7461 2073 6f75 7263 6520 7479 7065 3a22  ta source type:"
+00011550: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+00011560: 6c61 6265 6c5f 6772 6176 695f 6461 7461  label_gravi_data
+00011570: 5f73 6f75 7263 655f 7479 7065 2e73 6574  _source_type.set
+00011580: 546f 6f6c 5469 7028 5f74 7261 6e73 6c61  ToolTip(_transla
+00011590: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
+000115a0: 2022 5479 7065 206f 6620 7468 6520 6772   "Type of the gr
+000115b0: 6176 696d 6574 6572 2064 6174 6120 736f  avimeter data so
+000115c0: 7572 6365 2e20 2229 290a 2020 2020 2020  urce. ")).      
+000115d0: 2020 7365 6c66 2e6c 6162 656c 5f32 362e    self.label_26.
+000115e0: 7365 7454 6f6f 6c54 6970 285f 7472 616e  setToolTip(_tran
+000115f0: 736c 6174 6528 224d 6169 6e57 696e 646f  slate("MainWindo
+00011600: 7722 2c20 224e 756d 6265 7220 6f66 2073  w", "Number of s
+00011610: 6361 6c65 2066 6163 746f 7220 6974 656d  cale factor item
+00011620: 732e 2229 290a 2020 2020 2020 2020 7365  s.")).        se
+00011630: 6c66 2e6c 6162 656c 5f32 362e 7365 7454  lf.label_26.setT
+00011640: 6578 7428 5f74 7261 6e73 6c61 7465 2822  ext(_translate("
+00011650: 4d61 696e 5769 6e64 6f77 222c 2022 4e75  MainWindow", "Nu
+00011660: 6d62 6572 206f 6620 7363 616c 6520 6661  mber of scale fa
+00011670: 6374 6f72 733a 2229 290a 2020 2020 2020  ctors:")).      
+00011680: 2020 7365 6c66 2e6c 6162 656c 5f67 7261    self.label_gra
+00011690: 7669 5f6e 756d 5f73 6361 6c65 5f66 6163  vi_num_scale_fac
+000116a0: 746f 7273 2e73 6574 546f 6f6c 5469 7028  tors.setToolTip(
+000116b0: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
+000116c0: 5769 6e64 6f77 222c 2022 4e75 6d62 6572  Window", "Number
+000116d0: 206f 6620 7363 616c 6520 6661 6374 6f72   of scale factor
+000116e0: 2069 7465 6d73 2e22 2929 0a20 2020 2020   items.")).     
+000116f0: 2020 2073 656c 662e 6c61 6265 6c5f 3238     self.label_28
+00011700: 2e73 6574 5465 7874 285f 7472 616e 736c  .setText(_transl
+00011710: 6174 6528 224d 6169 6e57 696e 646f 7722  ate("MainWindow"
+00011720: 2c20 2244 6573 6372 6970 7469 6f6e 3a22  , "Description:"
+00011730: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+00011740: 7461 6257 6964 6765 745f 6772 6176 696d  tabWidget_gravim
+00011750: 6574 6572 732e 7365 7454 6162 5465 7874  eters.setTabText
+00011760: 2873 656c 662e 7461 6257 6964 6765 745f  (self.tabWidget_
+00011770: 6772 6176 696d 6574 6572 732e 696e 6465  gravimeters.inde
+00011780: 784f 6628 7365 6c66 2e74 6162 5f67 7261  xOf(self.tab_gra
+00011790: 7669 6d65 7465 725f 696e 666f 292c 205f  vimeter_info), _
+000117a0: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
+000117b0: 696e 646f 7722 2c20 2249 6e66 6f22 2929  indow", "Info"))
+000117c0: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
+000117d0: 6257 6964 6765 745f 6772 6176 696d 6574  bWidget_gravimet
+000117e0: 6572 732e 7365 7454 6162 5465 7874 2873  ers.setTabText(s
+000117f0: 656c 662e 7461 6257 6964 6765 745f 6772  elf.tabWidget_gr
+00011800: 6176 696d 6574 6572 732e 696e 6465 784f  avimeters.indexO
+00011810: 6628 7365 6c66 2e74 6162 5f67 7261 7669  f(self.tab_gravi
+00011820: 6d65 7465 725f 7363 616c 6529 2c20 5f74  meter_scale), _t
+00011830: 7261 6e73 6c61 7465 2822 4d61 696e 5769  ranslate("MainWi
+00011840: 6e64 6f77 222c 2022 5363 616c 6520 5461  ndow", "Scale Ta
+00011850: 626c 6522 2929 0a20 2020 2020 2020 2073  ble")).        s
+00011860: 656c 662e 7461 6257 6964 6765 745f 4d61  elf.tabWidget_Ma
+00011870: 696e 2e73 6574 5461 6254 6578 7428 7365  in.setTabText(se
+00011880: 6c66 2e74 6162 5769 6467 6574 5f4d 6169  lf.tabWidget_Mai
+00011890: 6e2e 696e 6465 784f 6628 7365 6c66 2e74  n.indexOf(self.t
+000118a0: 6162 5f6d 6169 6e5f 6772 6176 696d 6574  ab_main_gravimet
+000118b0: 6572 7329 2c20 5f74 7261 6e73 6c61 7465  ers), _translate
+000118c0: 2822 4d61 696e 5769 6e64 6f77 222c 2022  ("MainWindow", "
+000118d0: 4772 6176 696d 6574 6572 7322 2929 0a20  Gravimeters")). 
+000118e0: 2020 2020 2020 2073 656c 662e 7472 6565         self.tree
+000118f0: 5769 6467 6574 5f6f 6273 6572 7661 7469  Widget_observati
+00011900: 6f6e 732e 7365 7453 6f72 7469 6e67 456e  ons.setSortingEn
+00011910: 6162 6c65 6428 4661 6c73 6529 0a20 2020  abled(False).   
+00011920: 2020 2020 2073 656c 662e 7472 6565 5769       self.treeWi
+00011930: 6467 6574 5f6f 6273 6572 7661 7469 6f6e  dget_observation
+00011940: 732e 6865 6164 6572 4974 656d 2829 2e73  s.headerItem().s
+00011950: 6574 5465 7874 2830 2c20 5f74 7261 6e73  etText(0, _trans
+00011960: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
+00011970: 222c 2022 5375 7276 6579 2229 290a 2020  ", "Survey")).  
+00011980: 2020 2020 2020 7365 6c66 2e74 7265 6557        self.treeW
+00011990: 6964 6765 745f 6f62 7365 7276 6174 696f  idget_observatio
+000119a0: 6e73 2e68 6561 6465 7249 7465 6d28 292e  ns.headerItem().
+000119b0: 7365 7454 6578 7428 312c 205f 7472 616e  setText(1, _tran
+000119c0: 736c 6174 6528 224d 6169 6e57 696e 646f  slate("MainWindo
+000119d0: 7722 2c20 2253 7461 7469 6f6e 2229 290a  w", "Station")).
+000119e0: 2020 2020 2020 2020 7365 6c66 2e74 7265          self.tre
+000119f0: 6557 6964 6765 745f 6f62 7365 7276 6174  eWidget_observat
+00011a00: 696f 6e73 2e68 6561 6465 7249 7465 6d28  ions.headerItem(
+00011a10: 292e 7365 7454 6578 7428 322c 205f 7472  ).setText(2, _tr
+00011a20: 616e 736c 6174 6528 224d 6169 6e57 696e  anslate("MainWin
+00011a30: 646f 7722 2c20 2223 4f62 7322 2929 0a20  dow", "#Obs")). 
+00011a40: 2020 2020 2020 2073 656c 662e 7075 7368         self.push
+00011a50: 4275 7474 6f6e 5f6f 6273 5f63 6f6c 6c61  Button_obs_colla
+00011a60: 7073 5f61 6c6c 2e73 6574 5465 7874 285f  ps_all.setText(_
+00011a70: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
+00011a80: 696e 646f 7722 2c20 2243 6f6c 6c61 7065  indow", "Collape
+00011a90: 2061 6c6c 2229 290a 2020 2020 2020 2020   all")).        
+00011aa0: 7365 6c66 2e70 7573 6842 7574 746f 6e5f  self.pushButton_
+00011ab0: 6f62 735f 6578 7061 6e64 5f61 6c6c 2e73  obs_expand_all.s
+00011ac0: 6574 5465 7874 285f 7472 616e 736c 6174  etText(_translat
+00011ad0: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
+00011ae0: 2245 7870 616e 6420 616c 6c22 2929 0a20  "Expand all")). 
+00011af0: 2020 2020 2020 2073 656c 662e 6772 6f75         self.grou
+00011b00: 7042 6f78 5f6f 6273 5f64 6174 615f 6d61  pBox_obs_data_ma
+00011b10: 6e69 7075 6c61 7469 6f6e 2e73 6574 5469  nipulation.setTi
+00011b20: 746c 6528 5f74 7261 6e73 6c61 7465 2822  tle(_translate("
+00011b30: 4d61 696e 5769 6e64 6f77 222c 2022 4461  MainWindow", "Da
+00011b40: 7461 206d 616e 6970 756c 6174 696f 6e22  ta manipulation"
+00011b50: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+00011b60: 7075 7368 4275 7474 6f6e 5f6f 6273 5f61  pushButton_obs_a
+00011b70: 7070 6c79 5f61 7574 6f73 656c 6563 745f  pply_autoselect_
+00011b80: 6375 7272 656e 745f 6461 7461 2e73 6574  current_data.set
+00011b90: 546f 6f6c 5469 7028 5f74 7261 6e73 6c61  ToolTip(_transla
+00011ba0: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
+00011bb0: 2022 4163 7469 7661 7465 2f64 6561 6374   "Activate/deact
+00011bc0: 6976 6174 6520 6f62 7365 7276 6174 696f  ivate observatio
+00011bd0: 6e73 206f 6620 7468 6520 6375 7272 656e  ns of the curren
+00011be0: 7420 7365 6c65 6374 6564 2073 7572 7665  t selected surve
+00011bf0: 7920 6f72 2073 6574 7570 2061 6363 6f72  y or setup accor
+00011c00: 6469 6e67 2074 6f20 7468 6520 6175 746f  ding to the auto
+00011c10: 2d73 656c 6563 7469 6f6e 206f 7074 696f  -selection optio
+00011c20: 6e73 2e22 2929 0a20 2020 2020 2020 2073  ns.")).        s
+00011c30: 656c 662e 7075 7368 4275 7474 6f6e 5f6f  elf.pushButton_o
+00011c40: 6273 5f61 7070 6c79 5f61 7574 6f73 656c  bs_apply_autosel
+00011c50: 6563 745f 6375 7272 656e 745f 6461 7461  ect_current_data
+00011c60: 2e73 6574 5465 7874 285f 7472 616e 736c  .setText(_transl
+00011c70: 6174 6528 224d 6169 6e57 696e 646f 7722  ate("MainWindow"
+00011c80: 2c20 2241 7070 6c79 2041 7574 6f73 656c  , "Apply Autosel
+00011c90: 6563 7469 6f6e 2229 290a 2020 2020 2020  ection")).      
+00011ca0: 2020 7365 6c66 2e70 7573 6842 7574 746f    self.pushButto
+00011cb0: 6e5f 6f62 735f 636f 6d70 5f73 6574 7570  n_obs_comp_setup
+00011cc0: 5f64 6174 612e 7365 7454 6f6f 6c54 6970  _data.setToolTip
+00011cd0: 285f 7472 616e 736c 6174 6528 224d 6169  (_translate("Mai
+00011ce0: 6e57 696e 646f 7722 2c20 2243 6f6d 7075  nWindow", "Compu
+00011cf0: 7465 2076 6172 6961 6e63 652d 7765 6967  te variance-weig
+00011d00: 6874 6564 206d 6561 6e20 6f66 2061 6374  hted mean of act
+00011d10: 6976 6520 6f62 7365 7276 6174 696f 6e73  ive observations
+00011d20: 2066 6f72 2061 6c6c 2073 6574 7570 7320   for all setups 
+00011d30: 696e 2063 616d 7061 6967 6e2e 2229 290a  in campaign.")).
+00011d40: 2020 2020 2020 2020 7365 6c66 2e70 7573          self.pus
+00011d50: 6842 7574 746f 6e5f 6f62 735f 636f 6d70  hButton_obs_comp
+00011d60: 5f73 6574 7570 5f64 6174 612e 7365 7454  _setup_data.setT
+00011d70: 6578 7428 5f74 7261 6e73 6c61 7465 2822  ext(_translate("
+00011d80: 4d61 696e 5769 6e64 6f77 222c 2022 436f  MainWindow", "Co
+00011d90: 6d70 7574 6520 7365 7475 7020 6461 7461  mpute setup data
+00011da0: 2066 6f72 2063 616d 7061 6967 6e22 2929   for campaign"))
+00011db0: 0a20 2020 2020 2020 2073 656c 662e 7075  .        self.pu
+00011dc0: 7368 4275 7474 6f6e 5f6f 6273 5f72 756e  shButton_obs_run
+00011dd0: 5f65 7374 696d 6174 696f 6e2e 7365 7454  _estimation.setT
+00011de0: 6f6f 6c54 6970 285f 7472 616e 736c 6174  oolTip(_translat
+00011df0: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
+00011e00: 2252 756e 2070 6172 616d 6574 6572 2065  "Run parameter e
+00011e10: 7374 696d 6174 696f 6e20 6163 636f 7264  stimation accord
+00011e20: 696e 6720 746f 2074 6865 2065 7374 696d  ing to the estim
+00011e30: 6174 696f 6e20 7365 7474 696e 6773 2e22  ation settings."
+00011e40: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+00011e50: 7075 7368 4275 7474 6f6e 5f6f 6273 5f72  pushButton_obs_r
+00011e60: 756e 5f65 7374 696d 6174 696f 6e2e 7365  un_estimation.se
+00011e70: 7454 6578 7428 5f74 7261 6e73 6c61 7465  tText(_translate
+00011e80: 2822 4d61 696e 5769 6e64 6f77 222c 2022  ("MainWindow", "
+00011e90: 5275 6e20 6573 7469 6d61 7469 6f6e 2229  Run estimation")
+00011ea0: 290a 2020 2020 2020 2020 7365 6c66 2e67  ).        self.g
+00011eb0: 726f 7570 426f 785f 6f62 735f 7669 6577  roupBox_obs_view
+00011ec0: 5f6f 7074 696f 6e73 2e73 6574 5469 746c  _options.setTitl
+00011ed0: 6528 5f74 7261 6e73 6c61 7465 2822 4d61  e(_translate("Ma
+00011ee0: 696e 5769 6e64 6f77 222c 2022 5669 6577  inWindow", "View
+00011ef0: 204f 7074 696f 6e73 2229 290a 2020 2020   Options")).    
+00011f00: 2020 2020 7365 6c66 2e63 6865 636b 426f      self.checkBo
+00011f10: 785f 6f62 735f 706c 6f74 5f72 6564 7563  x_obs_plot_reduc
+00011f20: 6564 5f6f 6273 6572 7661 7469 6f6e 732e  ed_observations.
+00011f30: 7365 7454 6f6f 6c54 6970 285f 7472 616e  setToolTip(_tran
+00011f40: 736c 6174 6528 224d 6169 6e57 696e 646f  slate("MainWindo
+00011f50: 7722 2c20 2250 6c6f 7420 7265 6475 6365  w", "Plot reduce
+00011f60: 6420 6f62 7365 7276 6174 696f 2064 6174  d observatio dat
+00011f70: 612c 2069 6620 6176 6169 6c62 6c65 2e22  a, if availble."
+00011f80: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+00011f90: 6368 6563 6b42 6f78 5f6f 6273 5f70 6c6f  checkBox_obs_plo
+00011fa0: 745f 7265 6475 6365 645f 6f62 7365 7276  t_reduced_observ
+00011fb0: 6174 696f 6e73 2e73 6574 5465 7874 285f  ations.setText(_
+00011fc0: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
+00011fd0: 696e 646f 7722 2c20 2250 6c6f 7420 7265  indow", "Plot re
+00011fe0: 6475 6365 6420 6f62 7365 7276 6174 696f  duced observatio
+00011ff0: 6e73 2229 290a 2020 2020 2020 2020 7365  ns")).        se
+00012000: 6c66 2e63 6865 636b 426f 785f 6f62 735f  lf.checkBox_obs_
+00012010: 706c 6f74 5f73 6574 7570 5f64 6174 612e  plot_setup_data.
+00012020: 7365 7454 6f6f 6c54 6970 285f 7472 616e  setToolTip(_tran
+00012030: 736c 6174 6528 224d 6169 6e57 696e 646f  slate("MainWindo
+00012040: 7722 2c20 2250 6c6f 7420 7661 7269 616e  w", "Plot varian
+00012050: 6365 2d77 6569 6768 7465 6420 6d65 616e  ce-weighted mean
+00012060: 206f 6620 6f62 7365 7276 6174 696f 6e20   of observation 
+00012070: 6461 7461 2066 6f72 2061 6c6c 2073 6574  data for all set
+00012080: 7570 732e 2229 290a 2020 2020 2020 2020  ups.")).        
+00012090: 7365 6c66 2e63 6865 636b 426f 785f 6f62  self.checkBox_ob
+000120a0: 735f 706c 6f74 5f73 6574 7570 5f64 6174  s_plot_setup_dat
+000120b0: 612e 7365 7454 6578 7428 5f74 7261 6e73  a.setText(_trans
+000120c0: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
+000120d0: 222c 2022 506c 6f74 2073 6574 7570 2064  ", "Plot setup d
+000120e0: 6174 6122 2929 0a20 2020 2020 2020 2073  ata")).        s
+000120f0: 656c 662e 7461 6257 6964 6765 745f 6f62  elf.tabWidget_ob
+00012100: 7365 7276 6174 696f 6e73 2e73 6574 5461  servations.setTa
+00012110: 6254 6578 7428 7365 6c66 2e74 6162 5769  bText(self.tabWi
+00012120: 6467 6574 5f6f 6273 6572 7661 7469 6f6e  dget_observation
+00012130: 732e 696e 6465 784f 6628 7365 6c66 2e74  s.indexOf(self.t
+00012140: 6162 5f6f 6273 6572 7661 7469 6f6e 735f  ab_observations_
+00012150: 706c 6f74 7329 2c20 5f74 7261 6e73 6c61  plots), _transla
+00012160: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
+00012170: 2022 4f62 7365 7276 6174 696f 6e20 706c   "Observation pl
+00012180: 6f74 7322 2929 0a20 2020 2020 2020 2073  ots")).        s
+00012190: 656c 662e 7461 6257 6964 6765 745f 6f62  elf.tabWidget_ob
+000121a0: 7365 7276 6174 696f 6e73 2e73 6574 5461  servations.setTa
+000121b0: 6254 6578 7428 7365 6c66 2e74 6162 5769  bText(self.tabWi
+000121c0: 6467 6574 5f6f 6273 6572 7661 7469 6f6e  dget_observation
+000121d0: 732e 696e 6465 784f 6628 7365 6c66 2e74  s.indexOf(self.t
+000121e0: 6162 5f6f 6273 6572 7661 7469 6f6e 735f  ab_observations_
+000121f0: 7461 626c 6529 2c20 5f74 7261 6e73 6c61  table), _transla
+00012200: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
+00012210: 2022 4f62 7365 7276 6174 696f 6e73 2074   "Observations t
+00012220: 6162 6c65 2229 290a 2020 2020 2020 2020  able")).        
+00012230: 7365 6c66 2e70 7573 6842 7574 746f 6e5f  self.pushButton_
+00012240: 7375 7276 6579 735f 656e 6162 6c65 5f61  surveys_enable_a
+00012250: 6c6c 2e73 6574 546f 6f6c 5469 7028 5f74  ll.setToolTip(_t
 00012260: 7261 6e73 6c61 7465 2822 4d61 696e 5769  ranslate("MainWi
-00012270: 6e64 6f77 222c 2022 4174 6d2e 2070 7265  ndow", "Atm. pre
-00012280: 7373 7572 6520 636f 7272 6563 7469 6f6e  ssure correction
-00012290: 3a20 2229 290a 2020 2020 2020 2020 7365  : ")).        se
-000122a0: 6c66 2e74 6162 5769 6467 6574 5f6f 6273  lf.tabWidget_obs
-000122b0: 6572 7661 7469 6f6e 732e 7365 7454 6162  ervations.setTab
-000122c0: 5465 7874 2873 656c 662e 7461 6257 6964  Text(self.tabWid
-000122d0: 6765 745f 6f62 7365 7276 6174 696f 6e73  get_observations
-000122e0: 2e69 6e64 6578 4f66 2873 656c 662e 7461  .indexOf(self.ta
-000122f0: 625f 6f62 7365 7276 6174 696f 6e73 5f73  b_observations_s
-00012300: 6574 7570 7329 2c20 5f74 7261 6e73 6c61  etups), _transla
-00012310: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
-00012320: 2022 5365 7475 7073 2074 6162 6c65 2229   "Setups table")
-00012330: 290a 2020 2020 2020 2020 7365 6c66 2e74  ).        self.t
-00012340: 6162 5769 6467 6574 5f4d 6169 6e2e 7365  abWidget_Main.se
-00012350: 7454 6162 5465 7874 2873 656c 662e 7461  tTabText(self.ta
-00012360: 6257 6964 6765 745f 4d61 696e 2e69 6e64  bWidget_Main.ind
-00012370: 6578 4f66 2873 656c 662e 7461 625f 6d61  exOf(self.tab_ma
-00012380: 696e 5f6f 6273 6572 7661 7469 6f6e 7329  in_observations)
-00012390: 2c20 5f74 7261 6e73 6c61 7465 2822 4d61  , _translate("Ma
-000123a0: 696e 5769 6e64 6f77 222c 2022 4f62 7365  inWindow", "Obse
-000123b0: 7276 6174 696f 6e73 2229 290a 2020 2020  rvations")).    
-000123c0: 2020 2020 7365 6c66 2e67 726f 7570 426f      self.groupBo
-000123d0: 785f 7265 7375 6c74 735f 6c73 6d5f 7275  x_results_lsm_ru
-000123e0: 6e73 2e73 6574 5469 746c 6528 5f74 7261  ns.setTitle(_tra
-000123f0: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
-00012400: 6f77 222c 2022 4c53 4d20 7275 6e73 2229  ow", "LSM runs")
-00012410: 290a 2020 2020 2020 2020 7365 6c66 2e70  ).        self.p
-00012420: 7573 6842 7574 746f 6e5f 7265 7375 6c74  ushButton_result
-00012430: 735f 6465 6c65 7465 5f6c 736d 5f72 756e  s_delete_lsm_run
-00012440: 2e73 6574 5465 7874 285f 7472 616e 736c  .setText(_transl
-00012450: 6174 6528 224d 6169 6e57 696e 646f 7722  ate("MainWindow"
-00012460: 2c20 2244 656c 6574 6520 7365 6c65 6374  , "Delete select
-00012470: 6564 206c 736d 2072 756e 2229 290a 2020  ed lsm run")).  
-00012480: 2020 2020 2020 7365 6c66 2e67 726f 7570        self.group
-00012490: 426f 785f 7265 7375 6c74 735f 6461 7461  Box_results_data
-000124a0: 5f73 656c 6563 7469 6f6e 2e73 6574 5469  _selection.setTi
-000124b0: 746c 6528 5f74 7261 6e73 6c61 7465 2822  tle(_translate("
-000124c0: 4d61 696e 5769 6e64 6f77 222c 2022 4461  MainWindow", "Da
-000124d0: 7461 2073 656c 6563 7469 6f6e 2229 290a  ta selection")).
-000124e0: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
-000124f0: 656c 5f32 2e73 6574 5465 7874 285f 7472  el_2.setText(_tr
-00012500: 616e 736c 6174 6528 224d 6169 6e57 696e  anslate("MainWin
-00012510: 646f 7722 2c20 2253 7461 7469 6f6e 2229  dow", "Station")
-00012520: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
-00012530: 6f6d 626f 426f 785f 7265 7375 6c74 735f  omboBox_results_
-00012540: 7365 6c65 6374 696f 6e5f 7374 6174 696f  selection_statio
-00012550: 6e2e 7365 7449 7465 6d54 6578 7428 302c  n.setItemText(0,
-00012560: 205f 7472 616e 736c 6174 6528 224d 6169   _translate("Mai
-00012570: 6e57 696e 646f 7722 2c20 2241 6c6c 2073  nWindow", "All s
-00012580: 7461 7469 6f6e 7322 2929 0a20 2020 2020  tations")).     
-00012590: 2020 2073 656c 662e 6c61 6265 6c5f 352e     self.label_5.
-000125a0: 7365 7454 6578 7428 5f74 7261 6e73 6c61  setText(_transla
-000125b0: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
-000125c0: 2022 5375 7276 6579 2229 290a 2020 2020   "Survey")).    
-000125d0: 2020 2020 7365 6c66 2e63 6f6d 626f 426f      self.comboBo
-000125e0: 785f 7265 7375 6c74 735f 7365 6c65 6374  x_results_select
-000125f0: 696f 6e5f 7375 7276 6579 2e73 6574 4974  ion_survey.setIt
-00012600: 656d 5465 7874 2830 2c20 5f74 7261 6e73  emText(0, _trans
-00012610: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
-00012620: 222c 2022 416c 6c20 7375 7276 6579 7322  ", "All surveys"
-00012630: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-00012640: 6772 6f75 7042 6f78 5f67 6973 5f64 6174  groupBox_gis_dat
-00012650: 612e 7365 7454 6f6f 6c54 6970 285f 7472  a.setToolTip(_tr
-00012660: 616e 736c 6174 6528 224d 6169 6e57 696e  anslate("MainWin
-00012670: 646f 7722 2c20 223c 6874 6d6c 3e3c 6865  dow", "<html><he
-00012680: 6164 2f3e 3c62 6f64 793e 3c70 3e45 7870  ad/><body><p>Exp
-00012690: 6f72 7420 7468 6520 6375 7272 656e 7420  ort the current 
-000126a0: 636f 6e74 656e 7420 6f66 2074 6865 206f  content of the o
-000126b0: 6273 6572 7661 7469 6f6e 7320 616e 6420  bservations and 
-000126c0: 7468 6520 7374 6174 696f 6e73 2074 6162  the stations tab
-000126d0: 6c65 2074 6f20 616e 2045 5352 4920 7368  le to an ESRI sh
-000126e0: 6170 6566 696c 6520 286f 6273 5f72 6573  apefile (obs_res
-000126f0: 756c 7473 2e73 6870 2061 6e64 2073 7461  ults.shp and sta
-00012700: 745f 7265 7375 6c74 732e 7368 7029 2e20  t_results.shp). 
-00012710: 506c 6561 7365 2064 6563 6c61 7265 2074  Please declare t
-00012720: 6865 2043 5253 206f 6620 7468 6520 7374  he CRS of the st
-00012730: 6174 696f 6e20 636f 6f72 6469 6e61 7465  ation coordinate
-00012740: 7320 6279 2061 2076 616c 6964 2045 5053  s by a valid EPS
-00012750: 4720 636f 6465 2e20 5468 6520 6669 6c65  G code. The file
-00012760: 7320 6172 6520 7772 6974 7465 6e20 746f  s are written to
-00012770: 2074 6865 2063 616d 7061 6967 6e5c 2773   the campaign\'s
-00012780: 206f 7574 7075 7420 6469 7265 6374 6f72   output director
-00012790: 792e 203c 2f70 3e3c 2f62 6f64 793e 3c2f  y. </p></body></
-000127a0: 6874 6d6c 3e22 2929 0a20 2020 2020 2020  html>")).       
-000127b0: 2073 656c 662e 6772 6f75 7042 6f78 5f67   self.groupBox_g
-000127c0: 6973 5f64 6174 612e 7365 7454 6974 6c65  is_data.setTitle
-000127d0: 285f 7472 616e 736c 6174 6528 224d 6169  (_translate("Mai
-000127e0: 6e57 696e 646f 7722 2c20 2247 4953 2064  nWindow", "GIS d
-000127f0: 6174 6122 2929 0a20 2020 2020 2020 2073  ata")).        s
-00012800: 656c 662e 7075 7368 4275 7474 6f6e 5f72  elf.pushButton_r
-00012810: 6573 756c 7473 5f65 7870 6f72 745f 7368  esults_export_sh
-00012820: 6170 6566 696c 652e 7365 7454 6f6f 6c54  apefile.setToolT
-00012830: 6970 285f 7472 616e 736c 6174 6528 224d  ip(_translate("M
-00012840: 6169 6e57 696e 646f 7722 2c20 223c 6874  ainWindow", "<ht
-00012850: 6d6c 3e3c 6865 6164 2f3e 3c62 6f64 793e  ml><head/><body>
-00012860: 3c70 3e45 7870 6f72 7420 2074 6865 2063  <p>Export  the c
-00012870: 7572 7265 6e74 2063 6f6e 7465 6e74 206f  urrent content o
-00012880: 6620 7468 6520 6f62 7365 7276 6174 696f  f the observatio
-00012890: 6e73 2061 6e64 2074 6865 2073 7461 7469  ns and the stati
-000128a0: 6f6e 7320 7461 626c 6520 746f 2061 6e20  ons table to an 
-000128b0: 4553 5249 2073 6861 7065 6669 6c65 2028  ESRI shapefile (
-000128c0: 266c 743b 6361 6d70 6169 676e 206e 616d  &lt;campaign nam
-000128d0: 6526 6774 3b5f 6f62 732e 7368 7020 616e  e&gt;_obs.shp an
-000128e0: 6420 266c 743b 6361 6d70 6169 676e 206e  d &lt;campaign n
-000128f0: 616d 6526 6774 3b5f 7374 6174 2e73 6870  ame&gt;_stat.shp
-00012900: 292e 3c2f 703e 3c2f 626f 6479 3e3c 2f68  ).</p></body></h
-00012910: 746d 6c3e 2229 290a 2020 2020 2020 2020  tml>")).        
-00012920: 7365 6c66 2e70 7573 6842 7574 746f 6e5f  self.pushButton_
-00012930: 7265 7375 6c74 735f 6578 706f 7274 5f73  results_export_s
-00012940: 6861 7065 6669 6c65 2e73 6574 5465 7874  hapefile.setText
-00012950: 285f 7472 616e 736c 6174 6528 224d 6169  (_translate("Mai
-00012960: 6e57 696e 646f 7722 2c20 2245 7870 6f72  nWindow", "Expor
-00012970: 7420 7368 6170 6566 696c 6522 2929 0a20  t shapefile")). 
-00012980: 2020 2020 2020 2073 656c 662e 6772 6f75         self.grou
-00012990: 7042 6f78 5f72 6573 756c 7473 5f69 6e66  pBox_results_inf
-000129a0: 6f2e 7365 7454 6974 6c65 285f 7472 616e  o.setTitle(_tran
-000129b0: 736c 6174 6528 224d 6169 6e57 696e 646f  slate("MainWindo
-000129c0: 7722 2c20 2249 6e66 6f22 2929 0a20 2020  w", "Info")).   
-000129d0: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
-000129e0: 332e 7365 7454 6f6f 6c54 6970 285f 7472  3.setToolTip(_tr
-000129f0: 616e 736c 6174 6528 224d 6169 6e57 696e  anslate("MainWin
-00012a00: 646f 7722 2c20 2241 646a 7573 746d 656e  dow", "Adjustmen
-00012a10: 7420 6d65 7468 6f64 2e22 2929 0a20 2020  t method.")).   
-00012a20: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
-00012a30: 332e 7365 7454 6578 7428 5f74 7261 6e73  3.setText(_trans
-00012a40: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
-00012a50: 222c 2022 4164 6a75 7374 6d65 6e74 206d  ", "Adjustment m
-00012a60: 6574 686f 643a 2229 290a 2020 2020 2020  ethod:")).      
-00012a70: 2020 7365 6c66 2e6c 6162 656c 5f38 2e73    self.label_8.s
-00012a80: 6574 546f 6f6c 5469 7028 5f74 7261 6e73  etToolTip(_trans
-00012a90: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
-00012aa0: 222c 2022 4e75 6d62 6572 206f 6620 6974  ", "Number of it
-00012ab0: 6572 6174 696f 6e73 2069 6e20 6361 7365  erations in case
-00012ac0: 2074 6865 2069 7465 7261 7469 7665 2061   the iterative a
-00012ad0: 646a 7573 7465 6d6e 7420 6f66 2073 30c2  djustemnt of s0.
-00012ae0: b220 7761 7320 7365 6c65 6374 6564 2e22  . was selected."
-00012af0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-00012b00: 6c61 6265 6c5f 382e 7365 7454 6578 7428  label_8.setText(
-00012b10: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
-00012b20: 5769 6e64 6f77 222c 2022 4e75 6d62 6572  Window", "Number
-00012b30: 206f 6620 6974 6572 6174 696f 6e73 3a22   of iterations:"
-00012b40: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-00012b50: 6c61 6265 6c5f 3130 2e73 6574 546f 6f6c  label_10.setTool
-00012b60: 5469 7028 5f74 7261 6e73 6c61 7465 2822  Tip(_translate("
-00012b70: 4d61 696e 5769 6e64 6f77 222c 2022 4f70  MainWindow", "Op
-00012b80: 7469 6f6e 616c 2063 6f6d 6d65 6e74 206f  tional comment o
-00012b90: 6e20 7468 6520 6c73 6d20 7275 6e2e 2229  n the lsm run.")
-00012ba0: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
-00012bb0: 6162 656c 5f31 302e 7365 7454 6578 7428  abel_10.setText(
-00012bc0: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
-00012bd0: 5769 6e64 6f77 222c 2022 436f 6d6d 656e  Window", "Commen
-00012be0: 743a 2022 2929 0a20 2020 2020 2020 2073  t: ")).        s
-00012bf0: 656c 662e 6c61 6265 6c5f 342e 7365 7454  elf.label_4.setT
-00012c00: 6f6f 6c54 6970 285f 7472 616e 736c 6174  oolTip(_translat
-00012c10: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
-00012c20: 2254 696d 6520 616e 6420 6461 7465 2074  "Time and date t
-00012c30: 6865 2061 646a 7573 746d 656e 7420 7761  he adjustment wa
-00012c40: 7320 6361 7272 6965 6420 6f75 742e 2229  s carried out.")
-00012c50: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
-00012c60: 6162 656c 5f34 2e73 6574 5465 7874 285f  abel_4.setText(_
-00012c70: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
-00012c80: 696e 646f 7722 2c20 2254 696d 6520 616e  indow", "Time an
-00012c90: 6420 4461 7465 3a22 2929 0a20 2020 2020  d Date:")).     
-00012ca0: 2020 2073 656c 662e 6772 6f75 7042 6f78     self.groupBox
-00012cb0: 5f72 6573 756c 7473 5f73 7461 7469 7374  _results_statist
-00012cc0: 6963 732e 7365 7454 6974 6c65 285f 7472  ics.setTitle(_tr
-00012cd0: 616e 736c 6174 6528 224d 6169 6e57 696e  anslate("MainWin
-00012ce0: 646f 7722 2c20 2253 7461 7469 7374 6963  dow", "Statistic
-00012cf0: 7320 616e 6420 7465 7374 7322 2929 0a20  s and tests")). 
-00012d00: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
-00012d10: 6c5f 392e 7365 7454 6f6f 6c54 6970 285f  l_9.setToolTip(_
-00012d20: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
-00012d30: 696e 646f 7722 2c20 2241 2070 6f73 7465  indow", "A poste
-00012d40: 7269 6f72 6920 7661 7269 616e 6365 206f  riori variance o
-00012d50: 6620 756e 6974 2077 6569 6768 742e 2229  f unit weight.")
-00012d60: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
-00012d70: 6162 656c 5f39 2e73 6574 5465 7874 285f  abel_9.setText(_
-00012d80: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
-00012d90: 696e 646f 7722 2c20 2273 30c2 b23a 2229  indow", "s0..:")
-00012da0: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
-00012db0: 6162 656c 5f36 2e73 6574 546f 6f6c 5469  abel_6.setToolTi
-00012dc0: 7028 5f74 7261 6e73 6c61 7465 2822 4d61  p(_translate("Ma
-00012dd0: 696e 5769 6e64 6f77 222c 2022 4f75 7463  inWindow", "Outc
-00012de0: 6f6d 6520 6f66 2074 6865 2067 6c6f 6261  ome of the globa
-00012df0: 6c20 6d6f 6465 6c20 7465 7374 2e22 2929  l model test."))
-00012e00: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
-00012e10: 6265 6c5f 362e 7365 7454 6578 7428 5f74  bel_6.setText(_t
-00012e20: 7261 6e73 6c61 7465 2822 4d61 696e 5769  ranslate("MainWi
-00012e30: 6e64 6f77 222c 2022 476f 6f64 6e65 7373  ndow", "Goodness
-00012e40: 2d6f 662d 6669 7420 7465 7374 3a22 2929  -of-fit test:"))
-00012e50: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
-00012e60: 6265 6c5f 372e 7365 7454 6f6f 6c54 6970  bel_7.setToolTip
-00012e70: 285f 7472 616e 736c 6174 6528 224d 6169  (_translate("Mai
-00012e80: 6e57 696e 646f 7722 2c20 224e 756d 6265  nWindow", "Numbe
-00012e90: 7220 6f66 2064 6574 6563 7465 6420 6f75  r of detected ou
-00012ea0: 746c 6965 7273 2e22 2929 0a20 2020 2020  tliers.")).     
-00012eb0: 2020 2073 656c 662e 6c61 6265 6c5f 372e     self.label_7.
-00012ec0: 7365 7454 6578 7428 5f74 7261 6e73 6c61  setText(_transla
-00012ed0: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
-00012ee0: 2022 4e75 6d62 6572 206f 6620 6f75 746c   "Number of outl
-00012ef0: 6965 7273 3a22 2929 0a20 2020 2020 2020  iers:")).       
-00012f00: 2073 656c 662e 6772 6f75 7042 6f78 5f72   self.groupBox_r
-00012f10: 6573 756c 7473 5f6c 736d 5f72 756e 5f6c  esults_lsm_run_l
-00012f20: 6f67 2e73 6574 5469 746c 6528 5f74 7261  og.setTitle(_tra
-00012f30: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
-00012f40: 6f77 222c 2022 4c53 4d20 7275 6e20 6c6f  ow", "LSM run lo
-00012f50: 6722 2929 0a20 2020 2020 2020 2073 656c  g")).        sel
-00012f60: 662e 7461 6257 6964 6765 745f 7265 7375  f.tabWidget_resu
-00012f70: 6c74 732e 7365 7454 6162 5465 7874 2873  lts.setTabText(s
-00012f80: 656c 662e 7461 6257 6964 6765 745f 7265  elf.tabWidget_re
-00012f90: 7375 6c74 732e 696e 6465 784f 6628 7365  sults.indexOf(se
-00012fa0: 6c66 2e74 6162 5f72 6573 756c 7473 5f69  lf.tab_results_i
-00012fb0: 6e66 6f29 2c20 5f74 7261 6e73 6c61 7465  nfo), _translate
-00012fc0: 2822 4d61 696e 5769 6e64 6f77 222c 2022  ("MainWindow", "
-00012fd0: 496e 666f 2229 290a 2020 2020 2020 2020  Info")).        
-00012fe0: 7365 6c66 2e74 6162 5769 6467 6574 5f72  self.tabWidget_r
-00012ff0: 6573 756c 7473 2e73 6574 5461 6254 6578  esults.setTabTex
-00013000: 7428 7365 6c66 2e74 6162 5769 6467 6574  t(self.tabWidget
-00013010: 5f72 6573 756c 7473 2e69 6e64 6578 4f66  _results.indexOf
-00013020: 2873 656c 662e 7461 625f 7265 7375 6c74  (self.tab_result
-00013030: 735f 6f62 735f 7461 626c 6529 2c20 5f74  s_obs_table), _t
-00013040: 7261 6e73 6c61 7465 2822 4d61 696e 5769  ranslate("MainWi
-00013050: 6e64 6f77 222c 2022 4f62 7365 7276 6174  ndow", "Observat
-00013060: 696f 6e73 2054 6162 6c65 2229 290a 2020  ions Table")).  
-00013070: 2020 2020 2020 7365 6c66 2e67 726f 7570        self.group
-00013080: 426f 785f 706c 6f74 5f73 6574 7469 6e67  Box_plot_setting
-00013090: 732e 7365 7454 6974 6c65 285f 7472 616e  s.setTitle(_tran
-000130a0: 736c 6174 6528 224d 6169 6e57 696e 646f  slate("MainWindo
-000130b0: 7722 2c20 2250 6c6f 7420 7365 7474 696e  w", "Plot settin
-000130c0: 6773 2229 290a 2020 2020 2020 2020 7365  gs")).        se
-000130d0: 6c66 2e6c 6162 656c 5f72 6573 756c 7473  lf.label_results
-000130e0: 5f6f 6273 5f70 6c6f 745f 7365 6c65 635f  _obs_plot_selec_
-000130f0: 6461 7461 5f63 6f6c 756d 6e2e 7365 7454  data_column.setT
-00013100: 6578 7428 5f74 7261 6e73 6c61 7465 2822  ext(_translate("
-00013110: 4d61 696e 5769 6e64 6f77 222c 2022 5365  MainWindow", "Se
-00013120: 6c65 6374 2064 6174 6120 636f 6c75 6d6e  lect data column
-00013130: 3a22 2929 0a20 2020 2020 2020 2073 656c  :")).        sel
-00013140: 662e 7261 6469 6f42 7574 746f 6e5f 7265  f.radioButton_re
-00013150: 7375 6c74 735f 6f62 735f 706c 6f74 5f74  sults_obs_plot_t
-00013160: 696d 6573 6572 6965 732e 7365 7454 6578  imeseries.setTex
-00013170: 7428 5f74 7261 6e73 6c61 7465 2822 4d61  t(_translate("Ma
-00013180: 696e 5769 6e64 6f77 222c 2022 5469 6d65  inWindow", "Time
-00013190: 2073 6572 6965 7322 2929 0a20 2020 2020   series")).     
-000131a0: 2020 2073 656c 662e 7261 6469 6f42 7574     self.radioBut
-000131b0: 746f 6e5f 7265 7375 6c74 735f 6f62 735f  ton_results_obs_
-000131c0: 706c 6f74 5f68 6973 746f 6772 616d 2e73  plot_histogram.s
-000131d0: 6574 5465 7874 285f 7472 616e 736c 6174  etText(_translat
-000131e0: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
-000131f0: 2248 6973 746f 6772 616d 2229 290a 2020  "Histogram")).  
-00013200: 2020 2020 2020 7365 6c66 2e67 726f 7570        self.group
-00013210: 426f 785f 6869 7374 6f67 7261 6d5f 7365  Box_histogram_se
-00013220: 7474 696e 6773 2e73 6574 5469 746c 6528  ttings.setTitle(
-00013230: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
-00013240: 5769 6e64 6f77 222c 2022 4869 7374 6f67  Window", "Histog
-00013250: 7261 6d20 7365 7474 696e 6773 2229 290a  ram settings")).
-00013260: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
-00013270: 656c 5f31 312e 7365 7454 6578 7428 5f74  el_11.setText(_t
-00013280: 7261 6e73 6c61 7465 2822 4d61 696e 5769  ranslate("MainWi
-00013290: 6e64 6f77 222c 2022 4d65 7468 6f64 2229  ndow", "Method")
-000132a0: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
-000132b0: 6162 656c 5f72 6573 756c 7473 5f6f 6273  abel_results_obs
-000132c0: 5f70 6c6f 745f 6e75 6d62 6572 5f62 696e  _plot_number_bin
-000132d0: 732e 7365 7454 6578 7428 5f74 7261 6e73  s.setText(_trans
-000132e0: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
-000132f0: 222c 2022 4e75 6d62 6572 206f 6620 6269  ", "Number of bi
-00013300: 6e73 2229 290a 2020 2020 2020 2020 7365  ns")).        se
-00013310: 6c66 2e63 6865 636b 426f 785f 7265 7375  lf.checkBox_resu
-00013320: 6c74 735f 6f62 735f 706c 6f74 5f73 686f  lts_obs_plot_sho
-00013330: 775f 6f75 746c 6965 7273 2e73 6574 5465  w_outliers.setTe
-00013340: 7874 285f 7472 616e 736c 6174 6528 224d  xt(_translate("M
-00013350: 6169 6e57 696e 646f 7722 2c20 2253 686f  ainWindow", "Sho
-00013360: 7720 6f75 746c 6965 7273 2229 290a 2020  w outliers")).  
-00013370: 2020 2020 2020 7365 6c66 2e74 6162 5769        self.tabWi
-00013380: 6467 6574 5f72 6573 756c 7473 2e73 6574  dget_results.set
-00013390: 5461 6254 6578 7428 7365 6c66 2e74 6162  TabText(self.tab
-000133a0: 5769 6467 6574 5f72 6573 756c 7473 2e69  Widget_results.i
-000133b0: 6e64 6578 4f66 2873 656c 662e 7461 625f  ndexOf(self.tab_
-000133c0: 7265 7375 6c74 735f 6f62 735f 706c 6f74  results_obs_plot
-000133d0: 7329 2c20 5f74 7261 6e73 6c61 7465 2822  s), _translate("
-000133e0: 4d61 696e 5769 6e64 6f77 222c 2022 4f62  MainWindow", "Ob
-000133f0: 7365 7276 6174 696f 6e73 2050 6c6f 7473  servations Plots
-00013400: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
-00013410: 2e74 6162 5769 6467 6574 5f72 6573 756c  .tabWidget_resul
-00013420: 7473 2e73 6574 5461 6254 6578 7428 7365  ts.setTabText(se
-00013430: 6c66 2e74 6162 5769 6467 6574 5f72 6573  lf.tabWidget_res
-00013440: 756c 7473 2e69 6e64 6578 4f66 2873 656c  ults.indexOf(sel
-00013450: 662e 7461 625f 7265 7375 6c74 735f 6472  f.tab_results_dr
-00013460: 6966 7429 2c20 5f74 7261 6e73 6c61 7465  ift), _translate
-00013470: 2822 4d61 696e 5769 6e64 6f77 222c 2022  ("MainWindow", "
-00013480: 4472 6966 7420 5461 626c 6522 2929 0a20  Drift Table")). 
-00013490: 2020 2020 2020 2073 656c 662e 6772 6170         self.grap
-000134a0: 6869 6373 4c61 796f 7574 5769 6467 6574  hicsLayoutWidget
-000134b0: 5f72 6573 756c 7473 5f64 7269 6674 5f70  _results_drift_p
-000134c0: 6c6f 742e 7365 7454 6f6f 6c54 6970 285f  lot.setToolTip(_
-000134d0: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
-000134e0: 696e 646f 7722 2c20 223c 6874 6d6c 3e3c  indow", "<html><
-000134f0: 6865 6164 2f3e 3c62 6f64 793e 3c70 3e54  head/><body><p>T
-00013500: 6869 7320 706c 6f74 2064 6570 6963 7473  his plot depicts
-00013510: 2073 6574 7570 206f 6273 6572 7661 7469   setup observati
-00013520: 6f6e 7320 616e 6420 7468 6520 7468 6520  ons and the the 
-00013530: 6472 6966 7420 6675 6e63 7469 6f6e 2028  drift function (
-00013540: 706f 6c79 6e6f 6d69 616c 206f 6620 6465  polynomial of de
-00013550: 6772 6565 206e 2920 6669 7474 6564 2074  gree n) fitted t
-00013560: 6f20 7468 6573 6520 6f62 7365 7276 6174  o these observat
-00013570: 696f 6e73 2e3c 2f70 3e3c 2f62 6f64 793e  ions.</p></body>
-00013580: 3c2f 6874 6d6c 3e22 2929 0a20 2020 2020  </html>")).     
-00013590: 2020 2073 656c 662e 6772 6f75 7042 6f78     self.groupBox
-000135a0: 5f72 6573 756c 7473 5f64 7269 6674 5f70  _results_drift_p
-000135b0: 6c6f 742e 7365 7454 6974 6c65 285f 7472  lot.setTitle(_tr
-000135c0: 616e 736c 6174 6528 224d 6169 6e57 696e  anslate("MainWin
-000135d0: 646f 7722 2c20 2244 7269 6674 2070 6c6f  dow", "Drift plo
-000135e0: 7420 7365 7474 696e 6773 2229 290a 2020  t settings")).  
-000135f0: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
-00013600: 5f72 6573 756c 7473 5f64 7269 6674 5f70  _results_drift_p
-00013610: 6c6f 745f 765f 6f66 6673 6574 2e73 6574  lot_v_offset.set
-00013620: 546f 6f6c 5469 7028 5f74 7261 6e73 6c61  ToolTip(_transla
-00013630: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
-00013640: 2022 3c68 746d 6c3e 3c68 6561 642f 3e3c   "<html><head/><
-00013650: 626f 6479 3e3c 703e 4164 6420 7665 7274  body><p>Add vert
-00013660: 6963 616c 206f 6666 7365 7420 746f 2074  ical offset to t
-00013670: 6865 2064 7269 6674 2066 756e 6374 696f  he drift functio
-00013680: 6e20 2870 6f6c 796e 6f6d 6961 6c29 2077  n (polynomial) w
-00013690: 2e72 2e74 2e20 7468 6520 7365 7475 7020  .r.t. the setup 
-000136a0: 6f62 7365 7276 6174 696f 6e73 2e20 5468  observations. Th
-000136b0: 6973 2069 7320 6e65 6564 6564 2074 6f20  is is needed to 
-000136c0: 7768 656e 2064 6966 6665 7265 6e74 6961  when differentia
-000136d0: 6c20 6f62 7365 7276 6174 696f 6e73 2061  l observations a
-000136e0: 7265 2075 7365 6420 666f 7220 7072 616d  re used for pram
-000136f0: 6574 6572 2065 7374 696d 6174 696f 6e2e  eter estimation.
-00013700: 2049 6e20 7468 6973 2063 6173 6520 7468   In this case th
-00013710: 6520 636f 6e73 7461 6e74 2062 6961 7320  e constant bias 
-00013720: 6f66 2074 6865 2067 7261 7669 6d65 7465  of the gravimete
-00013730: 7220 7265 6164 696e 6720 6361 6e6e 6f74  r reading cannot
-00013740: 2062 6520 6573 7469 6d61 7465 6420 616e   be estimated an
-00013750: 6420 6973 206f 6e6c 7920 6465 7465 726d  d is only determ
-00013760: 696e 6564 2061 7070 726f 7869 6d61 7465  ined approximate
-00013770: 6c79 2e3c 2f70 3e3c 2f62 6f64 793e 3c2f  ly.</p></body></
-00013780: 6874 6d6c 3e22 2929 0a20 2020 2020 2020  html>")).       
-00013790: 2073 656c 662e 6c61 6265 6c5f 7265 7375   self.label_resu
-000137a0: 6c74 735f 6472 6966 745f 706c 6f74 5f76  lts_drift_plot_v
-000137b0: 5f6f 6666 7365 742e 7365 7454 6578 7428  _offset.setText(
-000137c0: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
-000137d0: 5769 6e64 6f77 222c 2022 5665 7274 6963  Window", "Vertic
-000137e0: 616c 206f 6666 7365 7420 6f66 2064 7269  al offset of dri
-000137f0: 6674 2070 6f6c 796e 6f6d 6961 6c20 772e  ft polynomial w.
-00013800: 722e 742e 2073 6574 7570 206f 6273 6572  r.t. setup obser
-00013810: 7661 7469 6f6e 7320 5bc2 b547 616c 5d22  vations [..Gal]"
-00013820: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-00013830: 7370 696e 426f 785f 7265 7375 6c74 735f  spinBox_results_
-00013840: 6472 6966 745f 706c 6f74 5f76 5f6f 6666  drift_plot_v_off
-00013850: 7365 742e 7365 7454 6f6f 6c54 6970 285f  set.setToolTip(_
-00013860: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
-00013870: 696e 646f 7722 2c20 223c 6874 6d6c 3e3c  indow", "<html><
-00013880: 6865 6164 2f3e 3c62 6f64 793e 3c70 3e41  head/><body><p>A
-00013890: 6464 2076 6572 7469 6361 6c20 6f66 6673  dd vertical offs
-000138a0: 6574 2074 6f20 7468 6520 6472 6966 7420  et to the drift 
-000138b0: 6675 6e63 7469 6f6e 2028 706f 6c79 6e6f  function (polyno
-000138c0: 6d69 616c 2920 772e 722e 742e 2074 6865  mial) w.r.t. the
-000138d0: 2073 6574 7570 206f 6273 6572 7661 7469   setup observati
-000138e0: 6f6e 732e 2054 6869 7320 6973 206e 6565  ons. This is nee
-000138f0: 6465 6420 746f 2077 6865 6e20 6469 6666  ded to when diff
-00013900: 6572 656e 7469 616c 206f 6273 6572 7661  erential observa
-00013910: 7469 6f6e 7320 6172 6520 7573 6564 2066  tions are used f
-00013920: 6f72 2070 7261 6d65 7465 7220 6573 7469  or prameter esti
-00013930: 6d61 7469 6f6e 2e20 496e 2074 6869 7320  mation. In this 
-00013940: 6361 7365 2074 6865 2063 6f6e 7374 616e  case the constan
-00013950: 7420 6269 6173 206f 6620 7468 6520 6772  t bias of the gr
-00013960: 6176 696d 6574 6572 2072 6561 6469 6e67  avimeter reading
-00013970: 2063 616e 6e6f 7420 6265 2065 7374 696d   cannot be estim
-00013980: 6174 6564 2061 6e64 2069 7320 6f6e 6c79  ated and is only
-00013990: 2064 6574 6572 6d69 6e65 6420 6170 7072   determined appr
-000139a0: 6f78 696d 6174 656c 792e 3c2f 703e 3c2f  oximately.</p></
-000139b0: 626f 6479 3e3c 2f68 746d 6c3e 2229 290a  body></html>")).
-000139c0: 2020 2020 2020 2020 7365 6c66 2e74 6162          self.tab
-000139d0: 5769 6467 6574 5f72 6573 756c 7473 2e73  Widget_results.s
-000139e0: 6574 5461 6254 6578 7428 7365 6c66 2e74  etTabText(self.t
-000139f0: 6162 5769 6467 6574 5f72 6573 756c 7473  abWidget_results
-00013a00: 2e69 6e64 6578 4f66 2873 656c 662e 7461  .indexOf(self.ta
-00013a10: 625f 7265 7375 6c74 735f 6472 6966 7470  b_results_driftp
-00013a20: 6c6f 7429 2c20 5f74 7261 6e73 6c61 7465  lot), _translate
-00013a30: 2822 4d61 696e 5769 6e64 6f77 222c 2022  ("MainWindow", "
-00013a40: 4472 6966 7420 506c 6f74 2229 290a 2020  Drift Plot")).  
-00013a50: 2020 2020 2020 7365 6c66 2e67 726f 7570        self.group
-00013a60: 426f 785f 7265 7375 6c74 735f 7374 6174  Box_results_stat
-00013a70: 696f 6e73 5f73 7461 7469 7374 6963 732e  ions_statistics.
-00013a80: 7365 7454 6f6f 6c54 6970 285f 7472 616e  setToolTip(_tran
-00013a90: 736c 6174 6528 224d 6169 6e57 696e 646f  slate("MainWindo
-00013aa0: 7722 2c20 223c 6874 6d6c 3e3c 6865 6164  w", "<html><head
-00013ab0: 2f3e 3c62 6f64 793e 3c70 3e43 616c 6375  /><body><p>Calcu
-00013ac0: 6c61 7465 2061 6e64 2064 6973 706c 6179  late and display
-00013ad0: 2064 6573 6372 6970 7469 7665 2073 7461   descriptive sta
-00013ae0: 7469 7374 6963 7320 666f 7220 7468 6520  tistics for the 
-00013af0: 7365 6c65 6374 6564 2064 6174 6120 636f  selected data co
-00013b00: 6c75 6d6e 2e3c 2f70 3e3c 2f62 6f64 793e  lumn.</p></body>
-00013b10: 3c2f 6874 6d6c 3e22 2929 0a20 2020 2020  </html>")).     
-00013b20: 2020 2073 656c 662e 6772 6f75 7042 6f78     self.groupBox
-00013b30: 5f72 6573 756c 7473 5f73 7461 7469 6f6e  _results_station
-00013b40: 735f 7374 6174 6973 7469 6373 2e73 6574  s_statistics.set
-00013b50: 5469 746c 6528 5f74 7261 6e73 6c61 7465  Title(_translate
-00013b60: 2822 4d61 696e 5769 6e64 6f77 222c 2022  ("MainWindow", "
-00013b70: 5374 6174 6973 7469 6373 2229 290a 2020  Statistics")).  
-00013b80: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
-00013b90: 5f31 322e 7365 7454 6f6f 6c54 6970 285f  _12.setToolTip(_
-00013ba0: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
-00013bb0: 696e 646f 7722 2c20 223c 6874 6d6c 3e3c  indow", "<html><
-00013bc0: 6865 6164 2f3e 3c62 6f64 793e 3c70 3e53  head/><body><p>S
-00013bd0: 656c 6563 7420 6461 7461 2063 6f6c 756d  elect data colum
-00013be0: 6e20 666f 7220 6469 7370 6c61 7969 6e67  n for displaying
-00013bf0: 2073 7461 7469 7374 6963 732e 3c2f 703e   statistics.</p>
-00013c00: 3c2f 626f 6479 3e3c 2f68 746d 6c3e 2229  </body></html>")
-00013c10: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
-00013c20: 6162 656c 5f31 322e 7365 7454 6578 7428  abel_12.setText(
-00013c30: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
-00013c40: 5769 6e64 6f77 222c 2022 5365 6c65 6374  Window", "Select
-00013c50: 2063 6f6c 756d 6e22 2929 0a20 2020 2020   column")).     
-00013c60: 2020 2073 656c 662e 636f 6d62 6f42 6f78     self.comboBox
-00013c70: 5f72 6573 756c 7473 5f73 7461 7469 6f6e  _results_station
-00013c80: 735f 7374 6174 6973 7469 6373 5f73 656c  s_statistics_sel
-00013c90: 6563 745f 636f 6c2e 7365 7454 6f6f 6c54  ect_col.setToolT
-00013ca0: 6970 285f 7472 616e 736c 6174 6528 224d  ip(_translate("M
-00013cb0: 6169 6e57 696e 646f 7722 2c20 223c 6874  ainWindow", "<ht
-00013cc0: 6d6c 3e3c 6865 6164 2f3e 3c62 6f64 793e  ml><head/><body>
-00013cd0: 3c70 3e53 656c 6563 7420 6461 7461 2063  <p>Select data c
-00013ce0: 6f6c 756d 6e20 666f 7220 6469 7370 6c61  olumn for displa
-00013cf0: 7969 6e67 2073 7461 7469 7374 6963 732e  ying statistics.
-00013d00: 3c2f 703e 3c2f 626f 6479 3e3c 2f68 746d  </p></body></htm
-00013d10: 6c3e 2229 290a 2020 2020 2020 2020 7365  l>")).        se
-00013d20: 6c66 2e6c 6162 656c 5f31 332e 7365 7454  lf.label_13.setT
-00013d30: 6f6f 6c54 6970 285f 7472 616e 736c 6174  oolTip(_translat
-00013d40: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
-00013d50: 224d 6561 6e22 2929 0a20 2020 2020 2020  "Mean")).       
-00013d60: 2073 656c 662e 6c61 6265 6c5f 3133 2e73   self.label_13.s
-00013d70: 6574 5465 7874 285f 7472 616e 736c 6174  etText(_translat
-00013d80: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
-00013d90: 224d 6561 6e3a 2229 290a 2020 2020 2020  "Mean:")).      
-00013da0: 2020 7365 6c66 2e6c 6162 656c 5f72 6573    self.label_res
-00013db0: 756c 7473 5f73 7461 7469 6f6e 735f 7374  ults_stations_st
-00013dc0: 6174 6973 7469 6373 5f6d 6561 6e2e 7365  atistics_mean.se
-00013dd0: 7454 6f6f 6c54 6970 285f 7472 616e 736c  tToolTip(_transl
-00013de0: 6174 6528 224d 6169 6e57 696e 646f 7722  ate("MainWindow"
-00013df0: 2c20 224d 6561 6e22 2929 0a20 2020 2020  , "Mean")).     
-00013e00: 2020 2073 656c 662e 6c61 6265 6c5f 3134     self.label_14
-00013e10: 2e73 6574 546f 6f6c 5469 7028 5f74 7261  .setToolTip(_tra
-00013e20: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
-00013e30: 6f77 222c 2022 5374 616e 6461 7264 2064  ow", "Standard d
-00013e40: 6576 6961 7469 6f6e 2229 290a 2020 2020  eviation")).    
-00013e50: 2020 2020 7365 6c66 2e6c 6162 656c 5f31      self.label_1
-00013e60: 342e 7365 7454 6578 7428 5f74 7261 6e73  4.setText(_trans
-00013e70: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
-00013e80: 222c 2022 5374 642e 3a22 2929 0a20 2020  ", "Std.:")).   
-00013e90: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
-00013ea0: 7265 7375 6c74 735f 7374 6174 696f 6e73  results_stations
-00013eb0: 5f73 7461 7469 7374 6963 735f 7374 642e  _statistics_std.
-00013ec0: 7365 7454 6f6f 6c54 6970 285f 7472 616e  setToolTip(_tran
-00013ed0: 736c 6174 6528 224d 6169 6e57 696e 646f  slate("MainWindo
-00013ee0: 7722 2c20 2253 7461 6e64 6172 6420 6465  w", "Standard de
-00013ef0: 7669 6174 696f 6e22 2929 0a20 2020 2020  viation")).     
-00013f00: 2020 2073 656c 662e 6c61 6265 6c5f 3135     self.label_15
-00013f10: 2e73 6574 546f 6f6c 5469 7028 5f74 7261  .setToolTip(_tra
-00013f20: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
-00013f30: 6f77 222c 2022 4d69 6e69 6d75 6d22 2929  ow", "Minimum"))
-00013f40: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
-00013f50: 6265 6c5f 3135 2e73 6574 5465 7874 285f  bel_15.setText(_
-00013f60: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
-00013f70: 696e 646f 7722 2c20 224d 696e 2e3a 2229  indow", "Min.:")
-00013f80: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
-00013f90: 6162 656c 5f72 6573 756c 7473 5f73 7461  abel_results_sta
-00013fa0: 7469 6f6e 735f 7374 6174 6973 7469 6373  tions_statistics
-00013fb0: 5f6d 696e 2e73 6574 546f 6f6c 5469 7028  _min.setToolTip(
-00013fc0: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
-00013fd0: 5769 6e64 6f77 222c 2022 4d69 6e69 6d75  Window", "Minimu
-00013fe0: 6d22 2929 0a20 2020 2020 2020 2073 656c  m")).        sel
-00013ff0: 662e 6c61 6265 6c5f 3136 2e73 6574 546f  f.label_16.setTo
-00014000: 6f6c 5469 7028 5f74 7261 6e73 6c61 7465  olTip(_translate
-00014010: 2822 4d61 696e 5769 6e64 6f77 222c 2022  ("MainWindow", "
-00014020: 4d61 7869 6d75 6d22 2929 0a20 2020 2020  Maximum")).     
-00014030: 2020 2073 656c 662e 6c61 6265 6c5f 3136     self.label_16
-00014040: 2e73 6574 5465 7874 285f 7472 616e 736c  .setText(_transl
-00014050: 6174 6528 224d 6169 6e57 696e 646f 7722  ate("MainWindow"
-00014060: 2c20 224d 6178 2e3a 2229 290a 2020 2020  , "Max.:")).    
-00014070: 2020 2020 7365 6c66 2e6c 6162 656c 5f72      self.label_r
-00014080: 6573 756c 7473 5f73 7461 7469 6f6e 735f  esults_stations_
-00014090: 7374 6174 6973 7469 6373 5f6d 6178 2e73  statistics_max.s
-000140a0: 6574 546f 6f6c 5469 7028 5f74 7261 6e73  etToolTip(_trans
-000140b0: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
-000140c0: 222c 2022 4d61 7869 6d75 6d22 2929 0a20  ", "Maximum")). 
-000140d0: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
-000140e0: 6c5f 3137 2e73 6574 546f 6f6c 5469 7028  l_17.setToolTip(
-000140f0: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
-00014100: 5769 6e64 6f77 222c 2022 4d65 6469 616e  Window", "Median
-00014110: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
-00014120: 2e6c 6162 656c 5f31 372e 7365 7454 6578  .label_17.setTex
-00014130: 7428 5f74 7261 6e73 6c61 7465 2822 4d61  t(_translate("Ma
-00014140: 696e 5769 6e64 6f77 222c 2022 4d65 6469  inWindow", "Medi
-00014150: 616e 3a22 2929 0a20 2020 2020 2020 2073  an:")).        s
-00014160: 656c 662e 6c61 6265 6c5f 5f72 6573 756c  elf.label__resul
-00014170: 7473 5f73 7461 7469 6f6e 735f 7374 6174  ts_stations_stat
-00014180: 6973 7469 6373 5f6d 6564 6961 6e2e 7365  istics_median.se
-00014190: 7454 6f6f 6c54 6970 285f 7472 616e 736c  tToolTip(_transl
-000141a0: 6174 6528 224d 6169 6e57 696e 646f 7722  ate("MainWindow"
-000141b0: 2c20 224d 6564 6961 6e22 2929 0a20 2020  , "Median")).   
-000141c0: 2020 2020 2073 656c 662e 6c61 6265 6c5f       self.label_
-000141d0: 3138 2e73 6574 546f 6f6c 5469 7028 5f74  18.setToolTip(_t
-000141e0: 7261 6e73 6c61 7465 2822 4d61 696e 5769  ranslate("MainWi
-000141f0: 6e64 6f77 222c 2022 496e 7465 7271 7561  ndow", "Interqua
-00014200: 7274 696c 6520 7261 6e67 6522 2929 0a20  rtile range")). 
-00014210: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
-00014220: 6c5f 3138 2e73 6574 5465 7874 285f 7472  l_18.setText(_tr
-00014230: 616e 736c 6174 6528 224d 6169 6e57 696e  anslate("MainWin
-00014240: 646f 7722 2c20 2249 5152 3a22 2929 0a20  dow", "IQR:")). 
-00014250: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
-00014260: 6c5f 5f72 6573 756c 7473 5f73 7461 7469  l__results_stati
-00014270: 6f6e 735f 7374 6174 6973 7469 6373 5f69  ons_statistics_i
-00014280: 7172 2e73 6574 546f 6f6c 5469 7028 5f74  qr.setToolTip(_t
-00014290: 7261 6e73 6c61 7465 2822 4d61 696e 5769  ranslate("MainWi
-000142a0: 6e64 6f77 222c 2022 496e 7465 7271 7561  ndow", "Interqua
-000142b0: 7274 696c 6520 7261 6e67 6522 2929 0a20  rtile range")). 
-000142c0: 2020 2020 2020 2073 656c 662e 7461 6257         self.tabW
-000142d0: 6964 6765 745f 7265 7375 6c74 732e 7365  idget_results.se
-000142e0: 7454 6162 5465 7874 2873 656c 662e 7461  tTabText(self.ta
-000142f0: 6257 6964 6765 745f 7265 7375 6c74 732e  bWidget_results.
-00014300: 696e 6465 784f 6628 7365 6c66 2e74 6162  indexOf(self.tab
-00014310: 5f72 6573 756c 7473 5f73 7461 745f 7461  _results_stat_ta
-00014320: 626c 6529 2c20 5f74 7261 6e73 6c61 7465  ble), _translate
-00014330: 2822 4d61 696e 5769 6e64 6f77 222c 2022  ("MainWindow", "
-00014340: 2053 7461 7469 6f6e 7320 5461 626c 6522   Stations Table"
-00014350: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-00014360: 7461 6257 6964 6765 745f 7265 7375 6c74  tabWidget_result
-00014370: 732e 7365 7454 6162 5465 7874 2873 656c  s.setTabText(sel
-00014380: 662e 7461 6257 6964 6765 745f 7265 7375  f.tabWidget_resu
-00014390: 6c74 732e 696e 6465 784f 6628 7365 6c66  lts.indexOf(self
-000143a0: 2e74 6162 5f72 6573 756c 7473 5f63 6f72  .tab_results_cor
-000143b0: 7265 6c61 7469 6f6e 5f6d 6174 7269 7829  relation_matrix)
-000143c0: 2c20 5f74 7261 6e73 6c61 7465 2822 4d61  , _translate("Ma
-000143d0: 696e 5769 6e64 6f77 222c 2022 436f 7272  inWindow", "Corr
-000143e0: 656c 6174 696f 6e20 4d61 7472 6978 2229  elation Matrix")
-000143f0: 290a 2020 2020 2020 2020 7365 6c66 2e74  ).        self.t
-00014400: 6162 5769 6467 6574 5f72 6573 756c 7473  abWidget_results
-00014410: 2e73 6574 5461 6254 6578 7428 7365 6c66  .setTabText(self
-00014420: 2e74 6162 5769 6467 6574 5f72 6573 756c  .tabWidget_resul
-00014430: 7473 2e69 6e64 6578 4f66 2873 656c 662e  ts.indexOf(self.
-00014440: 7461 625f 7667 5f74 6162 6c65 292c 205f  tab_vg_table), _
-00014450: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
-00014460: 696e 646f 7722 2c20 2256 4720 5461 626c  indow", "VG Tabl
-00014470: 6522 2929 0a20 2020 2020 2020 2073 656c  e")).        sel
-00014480: 662e 6772 6170 6869 6373 4c61 796f 7574  f.graphicsLayout
-00014490: 5769 6467 6574 5f72 6573 756c 7473 5f76  Widget_results_v
-000144a0: 675f 706c 6f74 2e73 6574 546f 6f6c 5469  g_plot.setToolTi
-000144b0: 7028 5f74 7261 6e73 6c61 7465 2822 4d61  p(_translate("Ma
-000144c0: 696e 5769 6e64 6f77 222c 2022 5468 6520  inWindow", "The 
-000144d0: 5647 2070 6c6f 7420 696c 6c75 7374 6172  VG plot illustar
-000144e0: 7465 7320 7468 6520 6573 7469 6d61 7469  tes the estimati
-000144f0: 6f6e 2072 6573 756c 7473 206f 6620 7468  on results of th
-00014500: 6520 5647 2070 6f6c 796e 6f6d 6961 6c2e  e VG polynomial.
-00014510: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
-00014520: 2e67 726f 7570 426f 785f 7265 7375 6c74  .groupBox_result
-00014530: 735f 7667 5f70 6c6f 745f 7365 7474 696e  s_vg_plot_settin
-00014540: 6773 2e73 6574 546f 6f6c 5469 7028 5f74  gs.setToolTip(_t
-00014550: 7261 6e73 6c61 7465 2822 4d61 696e 5769  ranslate("MainWi
-00014560: 6e64 6f77 222c 2022 5365 7474 696e 6773  ndow", "Settings
-00014570: 2066 6f72 2074 6865 2056 4720 706c 6f74   for the VG plot
-00014580: 2e22 2929 0a20 2020 2020 2020 2073 656c  .")).        sel
-00014590: 662e 6772 6f75 7042 6f78 5f72 6573 756c  f.groupBox_resul
-000145a0: 7473 5f76 675f 706c 6f74 5f73 6574 7469  ts_vg_plot_setti
-000145b0: 6e67 732e 7365 7454 6974 6c65 285f 7472  ngs.setTitle(_tr
-000145c0: 616e 736c 6174 6528 224d 6169 6e57 696e  anslate("MainWin
-000145d0: 646f 7722 2c20 2256 4720 706c 6f74 2073  dow", "VG plot s
-000145e0: 6574 7469 6e67 7322 2929 0a20 2020 2020  ettings")).     
-000145f0: 2020 2073 656c 662e 6368 6563 6b42 6f78     self.checkBox
-00014600: 5f72 6573 756c 7473 5f76 675f 706c 6f74  _results_vg_plot
-00014610: 5f73 686f 775f 7265 7369 6475 616c 732e  _show_residuals.
-00014620: 7365 7454 6f6f 6c54 6970 285f 7472 616e  setToolTip(_tran
-00014630: 736c 6174 6528 224d 6169 6e57 696e 646f  slate("MainWindo
-00014640: 7722 2c20 2250 6c6f 7420 7468 6520 706f  w", "Plot the po
-00014650: 7374 2066 6974 2072 6573 6964 7561 6c73  st fit residuals
-00014660: 2067 726f 7570 6564 2062 7920 7468 6520   grouped by the 
-00014670: 7365 7475 7020 6865 6967 6874 2028 7374  setup height (st
-00014680: 6174 696f 6e20 6e61 6d65 292e 2049 6620  ation name). If 
-00014690: 6c69 6e65 6172 2061 6e64 206e 6f2d 6c69  linear and no-li
-000146a0: 6e65 6172 2063 6f6d 706f 6e65 6e74 7320  near components 
-000146b0: 6f66 2074 6865 2056 4720 706f 6c79 6e6f  of the VG polyno
-000146c0: 6d69 616c 2028 6465 6772 6565 203e 2031  mial (degree > 1
-000146d0: 2920 6172 6520 706c 6f74 7465 6420 7365  ) are plotted se
-000146e0: 7061 7261 7465 6c79 2c20 7468 6520 7265  parately, the re
-000146f0: 7369 6475 616c 7320 772e 722e 742e 2074  siduals w.r.t. t
-00014700: 6865 206c 696e 6561 7220 636f 6d70 6f6e  he linear compon
-00014710: 656e 7420 6573 7469 6d61 7465 6420 696e  ent estimated in
-00014720: 2074 6865 204c 534d 2061 646a 7573 746d   the LSM adjustm
-00014730: 656e 7420 6172 6520 7368 6f77 6e2e 2229  ent are shown.")
-00014740: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
-00014750: 6865 636b 426f 785f 7265 7375 6c74 735f  heckBox_results_
-00014760: 7667 5f70 6c6f 745f 7368 6f77 5f72 6573  vg_plot_show_res
-00014770: 6964 7561 6c73 2e73 6574 5465 7874 285f  iduals.setText(_
-00014780: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
-00014790: 696e 646f 7722 2c20 2253 686f 7720 7265  indow", "Show re
-000147a0: 7369 6475 616c 7322 2929 0a20 2020 2020  siduals")).     
-000147b0: 2020 2073 656c 662e 7261 6469 6f42 7574     self.radioBut
-000147c0: 746f 6e5f 7265 7375 6c74 735f 7667 5f70  ton_results_vg_p
-000147d0: 6c6f 745f 6465 7461 696c 732e 7365 7454  lot_details.setT
-000147e0: 6f6f 6c54 6970 285f 7472 616e 736c 6174  oolTip(_translat
-000147f0: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
-00014800: 2250 6c6f 7420 7468 6520 6c69 6e65 6172  "Plot the linear
-00014810: 2061 6e64 206e 6f6e 2d6c 696e 6561 7220   and non-linear 
-00014820: 636f 6d70 6f6e 656e 7473 206f 6620 7468  components of th
-00014830: 6520 6573 7469 6d61 7465 7320 5647 2070  e estimates VG p
-00014840: 6f6c 796e 6f6d 6961 6c20 7365 7061 7261  olynomial separa
-00014850: 7465 6c79 2e20 2229 290a 2020 2020 2020  tely. ")).      
-00014860: 2020 7365 6c66 2e72 6164 696f 4275 7474    self.radioButt
-00014870: 6f6e 5f72 6573 756c 7473 5f76 675f 706c  on_results_vg_pl
-00014880: 6f74 5f64 6574 6169 6c73 2e73 6574 5465  ot_details.setTe
-00014890: 7874 285f 7472 616e 736c 6174 6528 224d  xt(_translate("M
-000148a0: 6169 6e57 696e 646f 7722 2c20 2250 6c6f  ainWindow", "Plo
-000148b0: 7420 6c69 6e65 6172 2061 6e64 206e 6f6e  t linear and non
-000148c0: 2d6c 696e 6561 7220 636f 6d70 6f6e 656e  -linear componen
-000148d0: 7473 2073 6570 6172 6174 656c 7922 2929  ts separately"))
-000148e0: 0a20 2020 2020 2020 2073 656c 662e 7261  .        self.ra
-000148f0: 6469 6f42 7574 746f 6e5f 7265 7375 6c74  dioButton_result
-00014900: 735f 7667 5f70 6c6f 745f 6675 6c6c 5f70  s_vg_plot_full_p
-00014910: 6f6c 796e 6f6d 6961 6c2e 7365 7454 6f6f  olynomial.setToo
-00014920: 6c54 6970 285f 7472 616e 736c 6174 6528  lTip(_translate(
-00014930: 224d 6169 6e57 696e 646f 7722 2c20 2250  "MainWindow", "P
-00014940: 6c6f 7420 7468 6520 6675 6c6c 2065 7374  lot the full est
-00014950: 696d 6174 6564 2056 4720 706f 6c79 6e6f  imated VG polyno
-00014960: 6d69 616c 2076 6572 7375 7320 6865 6967  mial versus heig
-00014970: 6874 2061 626f 7665 2074 6865 2072 6566  ht above the ref
-00014980: 6572 656e 6365 2e22 2929 0a20 2020 2020  erence.")).     
-00014990: 2020 2073 656c 662e 7261 6469 6f42 7574     self.radioBut
-000149a0: 746f 6e5f 7265 7375 6c74 735f 7667 5f70  ton_results_vg_p
-000149b0: 6c6f 745f 6675 6c6c 5f70 6f6c 796e 6f6d  lot_full_polynom
-000149c0: 6961 6c2e 7365 7454 6578 7428 5f74 7261  ial.setText(_tra
-000149d0: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
-000149e0: 6f77 222c 2022 506c 6f74 2066 756c 6c20  ow", "Plot full 
-000149f0: 706f 6c79 6e6f 6d69 616c 2229 290a 2020  polynomial")).  
-00014a00: 2020 2020 2020 7365 6c66 2e74 6162 5769        self.tabWi
-00014a10: 6467 6574 5f72 6573 756c 7473 2e73 6574  dget_results.set
-00014a20: 5461 6254 6578 7428 7365 6c66 2e74 6162  TabText(self.tab
-00014a30: 5769 6467 6574 5f72 6573 756c 7473 2e69  Widget_results.i
-00014a40: 6e64 6578 4f66 2873 656c 662e 7461 625f  ndexOf(self.tab_
-00014a50: 7667 5f70 6c6f 7429 2c20 5f74 7261 6e73  vg_plot), _trans
-00014a60: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
-00014a70: 222c 2022 5647 2050 6c6f 7422 2929 0a20  ", "VG Plot")). 
-00014a80: 2020 2020 2020 2073 656c 662e 7461 6257         self.tabW
-00014a90: 6964 6765 745f 4d61 696e 2e73 6574 5461  idget_Main.setTa
-00014aa0: 6254 6578 7428 7365 6c66 2e74 6162 5769  bText(self.tabWi
-00014ab0: 6467 6574 5f4d 6169 6e2e 696e 6465 784f  dget_Main.indexO
-00014ac0: 6628 7365 6c66 2e74 6162 5f6d 6169 6e5f  f(self.tab_main_
-00014ad0: 7265 7375 6c74 7329 2c20 5f74 7261 6e73  results), _trans
-00014ae0: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
-00014af0: 222c 2022 5265 7375 6c74 7322 2929 0a20  ", "Results")). 
-00014b00: 2020 2020 2020 2073 656c 662e 7461 6257         self.tabW
-00014b10: 6964 6765 745f 4d61 696e 2e73 6574 5461  idget_Main.setTa
-00014b20: 6254 6f6f 6c54 6970 2873 656c 662e 7461  bToolTip(self.ta
-00014b30: 6257 6964 6765 745f 4d61 696e 2e69 6e64  bWidget_Main.ind
-00014b40: 6578 4f66 2873 656c 662e 7461 625f 6d61  exOf(self.tab_ma
-00014b50: 696e 5f72 6573 756c 7473 292c 205f 7472  in_results), _tr
-00014b60: 616e 736c 6174 6528 224d 6169 6e57 696e  anslate("MainWin
-00014b70: 646f 7722 2c20 2253 6574 7570 2064 6174  dow", "Setup dat
-00014b80: 613a 2043 6f72 7265 6374 6564 2061 6e64  a: Corrected and
-00014b90: 2072 6564 7563 6573 206f 6273 6572 7661   reduces observa
-00014ba0: 7469 6f6e 2064 6174 6120 6163 6375 6d75  tion data accumu
-00014bb0: 6c61 7465 6420 666f 7220 6561 6368 2069  lated for each i
-00014bc0: 6e73 7472 756d 656e 7420 7365 7475 702e  nstrument setup.
-00014bd0: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
-00014be0: 2e6d 656e 755f 4669 6c65 2e73 6574 5469  .menu_File.setTi
-00014bf0: 746c 6528 5f74 7261 6e73 6c61 7465 2822  tle(_translate("
-00014c00: 4d61 696e 5769 6e64 6f77 222c 2022 4669  MainWindow", "Fi
-00014c10: 6c65 2229 290a 2020 2020 2020 2020 7365  le")).        se
-00014c20: 6c66 2e6d 656e 7541 6464 5f53 7572 7665  lf.menuAdd_Surve
-00014c30: 792e 7365 7454 6974 6c65 285f 7472 616e  y.setTitle(_tran
-00014c40: 736c 6174 6528 224d 6169 6e57 696e 646f  slate("MainWindo
-00014c50: 7722 2c20 2241 6464 2053 7572 7665 7922  w", "Add Survey"
-00014c60: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-00014c70: 6d65 6e75 5f41 6464 5f53 7461 7469 6f6e  menu_Add_Station
-00014c80: 732e 7365 7454 6974 6c65 285f 7472 616e  s.setTitle(_tran
-00014c90: 736c 6174 6528 224d 6169 6e57 696e 646f  slate("MainWindo
-00014ca0: 7722 2c20 2241 6464 2053 7461 7469 6f6e  w", "Add Station
-00014cb0: 7322 2929 0a20 2020 2020 2020 2073 656c  s")).        sel
-00014cc0: 662e 6d65 6e75 5f41 6464 5f47 7261 7669  f.menu_Add_Gravi
-00014cd0: 6d65 7465 7273 2e73 6574 5469 746c 6528  meters.setTitle(
-00014ce0: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
-00014cf0: 5769 6e64 6f77 222c 2022 4164 6420 4772  Window", "Add Gr
-00014d00: 6176 696d 6574 6572 7322 2929 0a20 2020  avimeters")).   
-00014d10: 2020 2020 2073 656c 662e 6d65 6e75 5f4f       self.menu_O
-00014d20: 6273 6572 7661 7469 6f6e 732e 7365 7454  bservations.setT
-00014d30: 6974 6c65 285f 7472 616e 736c 6174 6528  itle(_translate(
-00014d40: 224d 6169 6e57 696e 646f 7722 2c20 224f  "MainWindow", "O
-00014d50: 6273 6572 7661 7469 6f6e 7322 2929 0a20  bservations")). 
-00014d60: 2020 2020 2020 2073 656c 662e 6d65 6e75         self.menu
-00014d70: 4573 7469 6d61 7469 6f6e 5f73 6574 7469  Estimation_setti
-00014d80: 6e67 732e 7365 7454 6974 6c65 285f 7472  ngs.setTitle(_tr
-00014d90: 616e 736c 6174 6528 224d 6169 6e57 696e  anslate("MainWin
-00014da0: 646f 7722 2c20 2253 6574 7469 6e67 7322  dow", "Settings"
-00014db0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-00014dc0: 6d65 6e75 4865 6c70 2e73 6574 5469 746c  menuHelp.setTitl
-00014dd0: 6528 5f74 7261 6e73 6c61 7465 2822 4d61  e(_translate("Ma
-00014de0: 696e 5769 6e64 6f77 222c 2022 4865 6c70  inWindow", "Help
-00014df0: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
-00014e00: 2e6d 656e 7543 6f72 7265 6374 696f 6e73  .menuCorrections
-00014e10: 2e73 6574 5469 746c 6528 5f74 7261 6e73  .setTitle(_trans
-00014e20: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
-00014e30: 222c 2022 436f 7272 6563 7469 6f6e 7322  ", "Corrections"
-00014e40: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-00014e50: 6163 7469 6f6e 5f4e 6577 5f43 616d 7061  action_New_Campa
-00014e60: 6967 6e2e 7365 7454 6578 7428 5f74 7261  ign.setText(_tra
-00014e70: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
-00014e80: 6f77 222c 2022 264e 6577 2043 616d 7061  ow", "&New Campa
-00014e90: 6967 6e22 2929 0a20 2020 2020 2020 2073  ign")).        s
-00014ea0: 656c 662e 6163 7469 6f6e 5f53 6176 655f  elf.action_Save_
-00014eb0: 4361 6d70 6169 676e 2e73 6574 5465 7874  Campaign.setText
-00014ec0: 285f 7472 616e 736c 6174 6528 224d 6169  (_translate("Mai
-00014ed0: 6e57 696e 646f 7722 2c20 2226 5361 7665  nWindow", "&Save
-00014ee0: 2043 616d 7061 6967 6e22 2929 0a20 2020   Campaign")).   
-00014ef0: 2020 2020 2073 656c 662e 6163 7469 6f6e       self.action
-00014f00: 5f4c 6f61 645f 4361 6d70 6169 676e 2e73  _Load_Campaign.s
-00014f10: 6574 5465 7874 285f 7472 616e 736c 6174  etText(_translat
-00014f20: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
-00014f30: 2226 4c6f 6164 2043 616d 7061 6967 6e22  "&Load Campaign"
-00014f40: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-00014f50: 6163 7469 6f6e 5f4c 6f61 645f 4361 6d70  action_Load_Camp
-00014f60: 6169 676e 2e73 6574 546f 6f6c 5469 7028  aign.setToolTip(
-00014f70: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
-00014f80: 5769 6e64 6f77 222c 2022 4c6f 6164 2063  Window", "Load c
-00014f90: 616d 7061 6967 6e22 2929 0a20 2020 2020  ampaign")).     
-00014fa0: 2020 2073 656c 662e 6163 7469 6f6e 5f41     self.action_A
-00014fb0: 6464 5f53 7461 7469 6f6e 732e 7365 7454  dd_Stations.setT
+00012270: 6e64 6f77 222c 2022 3c68 746d 6c3e 3c68  ndow", "<html><h
+00012280: 6561 642f 3e3c 626f 6479 3e3c 703e 4163  ead/><body><p>Ac
+00012290: 7469 7661 7465 2061 6c6c 2073 7572 7665  tivate all surve
+000122a0: 7973 2069 6e20 7468 6520 6361 6d70 6169  ys in the campai
+000122b0: 676e 2e3c 2f70 3e3c 2f62 6f64 793e 3c2f  gn.</p></body></
+000122c0: 6874 6d6c 3e22 2929 0a20 2020 2020 2020  html>")).       
+000122d0: 2073 656c 662e 7075 7368 4275 7474 6f6e   self.pushButton
+000122e0: 5f73 7572 7665 7973 5f65 6e61 626c 655f  _surveys_enable_
+000122f0: 616c 6c2e 7365 7454 6578 7428 5f74 7261  all.setText(_tra
+00012300: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
+00012310: 6f77 222c 2022 4163 7469 7661 7465 2061  ow", "Activate a
+00012320: 6c6c 2229 290a 2020 2020 2020 2020 7365  ll")).        se
+00012330: 6c66 2e70 7573 6842 7574 746f 6e5f 7375  lf.pushButton_su
+00012340: 7276 6579 735f 6469 7361 626c 655f 616c  rveys_disable_al
+00012350: 6c2e 7365 7454 6f6f 6c54 6970 285f 7472  l.setToolTip(_tr
+00012360: 616e 736c 6174 6528 224d 6169 6e57 696e  anslate("MainWin
+00012370: 646f 7722 2c20 223c 6874 6d6c 3e3c 6865  dow", "<html><he
+00012380: 6164 2f3e 3c62 6f64 793e 3c70 3e44 6561  ad/><body><p>Dea
+00012390: 6374 6976 6174 6520 616c 6c20 7375 7276  ctivate all surv
+000123a0: 6579 7320 696e 2074 6865 2063 616d 7061  eys in the campa
+000123b0: 6967 6e2e 3c2f 703e 3c2f 626f 6479 3e3c  ign.</p></body><
+000123c0: 2f68 746d 6c3e 2229 290a 2020 2020 2020  /html>")).      
+000123d0: 2020 7365 6c66 2e70 7573 6842 7574 746f    self.pushButto
+000123e0: 6e5f 7375 7276 6579 735f 6469 7361 626c  n_surveys_disabl
+000123f0: 655f 616c 6c2e 7365 7454 6578 7428 5f74  e_all.setText(_t
+00012400: 7261 6e73 6c61 7465 2822 4d61 696e 5769  ranslate("MainWi
+00012410: 6e64 6f77 222c 2022 4465 6163 7469 7661  ndow", "Deactiva
+00012420: 7465 2061 6c6c 2229 290a 2020 2020 2020  te all")).      
+00012430: 2020 7365 6c66 2e74 6162 5769 6467 6574    self.tabWidget
+00012440: 5f6f 6273 6572 7661 7469 6f6e 732e 7365  _observations.se
+00012450: 7454 6162 5465 7874 2873 656c 662e 7461  tTabText(self.ta
+00012460: 6257 6964 6765 745f 6f62 7365 7276 6174  bWidget_observat
+00012470: 696f 6e73 2e69 6e64 6578 4f66 2873 656c  ions.indexOf(sel
+00012480: 662e 7461 625f 7375 7276 6579 7329 2c20  f.tab_surveys), 
+00012490: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
+000124a0: 5769 6e64 6f77 222c 2022 5375 7276 6579  Window", "Survey
+000124b0: 7322 2929 0a20 2020 2020 2020 2073 656c  s")).        sel
+000124c0: 662e 6772 6f75 7042 6f78 5f6f 6273 5f73  f.groupBox_obs_s
+000124d0: 6574 7570 735f 6170 706c 6965 645f 636f  etups_applied_co
+000124e0: 7272 6563 7469 6f6e 732e 7365 7454 6f6f  rrections.setToo
+000124f0: 6c54 6970 285f 7472 616e 736c 6174 6528  lTip(_translate(
+00012500: 224d 6169 6e57 696e 646f 7722 2c20 2249  "MainWindow", "I
+00012510: 6e66 6f72 6d61 7469 6f6e 206f 6e20 7468  nformation on th
+00012520: 6520 636f 7272 6563 7469 6f6e 7320 7468  e corrections th
+00012530: 6174 2068 6176 6520 6265 656e 2061 7070  at have been app
+00012540: 6c69 6564 206f 6e20 7468 6520 6f62 7365  lied on the obse
+00012550: 7276 6174 696f 6e73 206f 6e20 7768 6963  rvations on whic
+00012560: 6820 7468 6520 7365 7475 7020 6461 7461  h the setup data
+00012570: 2069 7320 6261 7365 6420 6f6e 2e22 2929   is based on."))
+00012580: 0a20 2020 2020 2020 2073 656c 662e 6772  .        self.gr
+00012590: 6f75 7042 6f78 5f6f 6273 5f73 6574 7570  oupBox_obs_setup
+000125a0: 735f 6170 706c 6965 645f 636f 7272 6563  s_applied_correc
+000125b0: 7469 6f6e 732e 7365 7454 6974 6c65 285f  tions.setTitle(_
+000125c0: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
+000125d0: 696e 646f 7722 2c20 2241 7070 6c69 6564  indow", "Applied
+000125e0: 2063 6f72 7265 6374 696f 6e73 3a22 2929   corrections:"))
+000125f0: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
+00012600: 6265 6c5f 6f62 735f 7365 7475 7073 5f31  bel_obs_setups_1
+00012610: 2e73 6574 546f 6f6c 5469 7028 5f74 7261  .setToolTip(_tra
+00012620: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
+00012630: 6f77 222c 2022 5479 7065 206f 6620 6170  ow", "Type of ap
+00012640: 706c 6965 6420 7469 6461 6c20 636f 7272  plied tidal corr
+00012650: 6563 7469 6f6e 732e 2229 290a 2020 2020  ections.")).    
+00012660: 2020 2020 7365 6c66 2e6c 6162 656c 5f6f      self.label_o
+00012670: 6273 5f73 6574 7570 735f 312e 7365 7454  bs_setups_1.setT
+00012680: 6578 7428 5f74 7261 6e73 6c61 7465 2822  ext(_translate("
+00012690: 4d61 696e 5769 6e64 6f77 222c 2022 5469  MainWindow", "Ti
+000126a0: 6461 6c20 636f 7272 6563 7469 6f6e 3a22  dal correction:"
+000126b0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+000126c0: 6c61 6265 6c5f 6f62 735f 7365 7475 7073  label_obs_setups
+000126d0: 5f74 6964 616c 5f63 6f72 722e 7365 7454  _tidal_corr.setT
+000126e0: 6f6f 6c54 6970 285f 7472 616e 736c 6174  oolTip(_translat
+000126f0: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
+00012700: 2254 7970 6520 6f66 2061 7070 6c69 6564  "Type of applied
+00012710: 2074 6964 616c 2063 6f72 7265 6374 696f   tidal correctio
+00012720: 6e73 2e22 2929 0a20 2020 2020 2020 2073  ns.")).        s
+00012730: 656c 662e 6c61 6265 6c5f 6f62 735f 7365  elf.label_obs_se
+00012740: 7475 7073 5f32 2e73 6574 546f 6f6c 5469  tups_2.setToolTi
+00012750: 7028 5f74 7261 6e73 6c61 7465 2822 4d61  p(_translate("Ma
+00012760: 696e 5769 6e64 6f77 222c 2022 5479 7065  inWindow", "Type
+00012770: 206f 6620 7468 6520 6170 706c 6965 6420   of the applied 
+00012780: 7265 6665 7265 6e63 6520 6865 6967 6874  reference height
+00012790: 2072 6564 7563 7469 6f6e 2e22 2929 0a20   reduction.")). 
+000127a0: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
+000127b0: 6c5f 6f62 735f 7365 7475 7073 5f32 2e73  l_obs_setups_2.s
+000127c0: 6574 5465 7874 285f 7472 616e 736c 6174  etText(_translat
+000127d0: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
+000127e0: 224f 6273 2e20 7265 6665 7265 6e63 6520  "Obs. reference 
+000127f0: 6865 6967 6874 3a22 2929 0a20 2020 2020  height:")).     
+00012800: 2020 2073 656c 662e 6c61 6265 6c5f 6f62     self.label_ob
+00012810: 735f 7365 7475 7073 5f72 6566 5f68 6569  s_setups_ref_hei
+00012820: 6768 742e 7365 7454 6f6f 6c54 6970 285f  ght.setToolTip(_
+00012830: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
+00012840: 696e 646f 7722 2c20 2254 7970 6520 6f66  indow", "Type of
+00012850: 2074 6865 2061 7070 6c69 6564 2072 6566   the applied ref
+00012860: 6572 656e 6365 2068 6569 6768 7420 7265  erence height re
+00012870: 6475 6374 696f 6e2e 2229 290a 2020 2020  duction.")).    
+00012880: 2020 2020 7365 6c66 2e6c 6162 656c 5f32      self.label_2
+00012890: 372e 7365 7454 6578 7428 5f74 7261 6e73  7.setText(_trans
+000128a0: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
+000128b0: 222c 2022 5363 616c 6520 436f 7272 6563  ", "Scale Correc
+000128c0: 7469 6f6e 3a22 2929 0a20 2020 2020 2020  tion:")).       
+000128d0: 2073 656c 662e 6c61 6265 6c5f 6f62 735f   self.label_obs_
+000128e0: 7365 7475 7073 5f33 2e73 6574 5465 7874  setups_3.setText
+000128f0: 285f 7472 616e 736c 6174 6528 224d 6169  (_translate("Mai
+00012900: 6e57 696e 646f 7722 2c20 2241 746d 2e20  nWindow", "Atm. 
+00012910: 7072 6573 7375 7265 2063 6f72 7265 6374  pressure correct
+00012920: 696f 6e3a 2022 2929 0a20 2020 2020 2020  ion: ")).       
+00012930: 2073 656c 662e 7461 6257 6964 6765 745f   self.tabWidget_
+00012940: 6f62 7365 7276 6174 696f 6e73 2e73 6574  observations.set
+00012950: 5461 6254 6578 7428 7365 6c66 2e74 6162  TabText(self.tab
+00012960: 5769 6467 6574 5f6f 6273 6572 7661 7469  Widget_observati
+00012970: 6f6e 732e 696e 6465 784f 6628 7365 6c66  ons.indexOf(self
+00012980: 2e74 6162 5f6f 6273 6572 7661 7469 6f6e  .tab_observation
+00012990: 735f 7365 7475 7073 292c 205f 7472 616e  s_setups), _tran
+000129a0: 736c 6174 6528 224d 6169 6e57 696e 646f  slate("MainWindo
+000129b0: 7722 2c20 2253 6574 7570 7320 7461 626c  w", "Setups tabl
+000129c0: 6522 2929 0a20 2020 2020 2020 2073 656c  e")).        sel
+000129d0: 662e 7461 6257 6964 6765 745f 4d61 696e  f.tabWidget_Main
+000129e0: 2e73 6574 5461 6254 6578 7428 7365 6c66  .setTabText(self
+000129f0: 2e74 6162 5769 6467 6574 5f4d 6169 6e2e  .tabWidget_Main.
+00012a00: 696e 6465 784f 6628 7365 6c66 2e74 6162  indexOf(self.tab
+00012a10: 5f6d 6169 6e5f 6f62 7365 7276 6174 696f  _main_observatio
+00012a20: 6e73 292c 205f 7472 616e 736c 6174 6528  ns), _translate(
+00012a30: 224d 6169 6e57 696e 646f 7722 2c20 224f  "MainWindow", "O
+00012a40: 6273 6572 7661 7469 6f6e 7322 2929 0a20  bservations")). 
+00012a50: 2020 2020 2020 2073 656c 662e 6772 6f75         self.grou
+00012a60: 7042 6f78 5f72 6573 756c 7473 5f6c 736d  pBox_results_lsm
+00012a70: 5f72 756e 732e 7365 7454 6974 6c65 285f  _runs.setTitle(_
+00012a80: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
+00012a90: 696e 646f 7722 2c20 224c 534d 2072 756e  indow", "LSM run
+00012aa0: 7322 2929 0a20 2020 2020 2020 2073 656c  s")).        sel
+00012ab0: 662e 7075 7368 4275 7474 6f6e 5f72 6573  f.pushButton_res
+00012ac0: 756c 7473 5f64 656c 6574 655f 6c73 6d5f  ults_delete_lsm_
+00012ad0: 7275 6e2e 7365 7454 6f6f 6c54 6970 285f  run.setToolTip(_
+00012ae0: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
+00012af0: 696e 646f 7722 2c20 223c 6874 6d6c 3e3c  indow", "<html><
+00012b00: 6865 6164 2f3e 3c62 6f64 793e 3c70 3e44  head/><body><p>D
+00012b10: 656c 6574 6520 7468 6520 7365 6c65 6374  elete the select
+00012b20: 6564 204c 534d 2072 756e 2e3c 2f70 3e3c  ed LSM run.</p><
+00012b30: 2f62 6f64 793e 3c2f 6874 6d6c 3e22 2929  /body></html>"))
+00012b40: 0a20 2020 2020 2020 2073 656c 662e 7075  .        self.pu
+00012b50: 7368 4275 7474 6f6e 5f72 6573 756c 7473  shButton_results
+00012b60: 5f64 656c 6574 655f 6c73 6d5f 7275 6e2e  _delete_lsm_run.
+00012b70: 7365 7454 6578 7428 5f74 7261 6e73 6c61  setText(_transla
+00012b80: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
+00012b90: 2022 4465 6c65 7465 2073 656c 6563 7465   "Delete selecte
+00012ba0: 6420 6c73 6d20 7275 6e22 2929 0a20 2020  d lsm run")).   
+00012bb0: 2020 2020 2073 656c 662e 7075 7368 4275       self.pushBu
+00012bc0: 7474 6f6e 5f72 6573 756c 7473 5f64 656c  tton_results_del
+00012bd0: 6574 655f 616c 6c5f 6c73 6d5f 7275 6e73  ete_all_lsm_runs
+00012be0: 2e73 6574 546f 6f6c 5469 7028 5f74 7261  .setToolTip(_tra
+00012bf0: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
+00012c00: 6f77 222c 2022 3c68 746d 6c3e 3c68 6561  ow", "<html><hea
+00012c10: 642f 3e3c 626f 6479 3e3c 703e 4465 6c65  d/><body><p>Dele
+00012c20: 7465 2041 4c4c 206c 736d 2072 756e 7320  te ALL lsm runs 
+00012c30: 696e 2074 6865 2063 616d 7061 6967 6e2e  in the campaign.
+00012c40: 3c2f 703e 3c2f 626f 6479 3e3c 2f68 746d  </p></body></htm
+00012c50: 6c3e 2229 290a 2020 2020 2020 2020 7365  l>")).        se
+00012c60: 6c66 2e70 7573 6842 7574 746f 6e5f 7265  lf.pushButton_re
+00012c70: 7375 6c74 735f 6465 6c65 7465 5f61 6c6c  sults_delete_all
+00012c80: 5f6c 736d 5f72 756e 732e 7365 7454 6578  _lsm_runs.setTex
+00012c90: 7428 5f74 7261 6e73 6c61 7465 2822 4d61  t(_translate("Ma
+00012ca0: 696e 5769 6e64 6f77 222c 2022 4465 6c65  inWindow", "Dele
+00012cb0: 7465 2061 6c6c 206c 736d 2072 756e 7322  te all lsm runs"
+00012cc0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+00012cd0: 6772 6f75 7042 6f78 5f72 6573 756c 7473  groupBox_results
+00012ce0: 5f64 6174 615f 7365 6c65 6374 696f 6e2e  _data_selection.
+00012cf0: 7365 7454 6974 6c65 285f 7472 616e 736c  setTitle(_transl
+00012d00: 6174 6528 224d 6169 6e57 696e 646f 7722  ate("MainWindow"
+00012d10: 2c20 2244 6174 6120 7365 6c65 6374 696f  , "Data selectio
+00012d20: 6e22 2929 0a20 2020 2020 2020 2073 656c  n")).        sel
+00012d30: 662e 6c61 6265 6c5f 322e 7365 7454 6578  f.label_2.setTex
+00012d40: 7428 5f74 7261 6e73 6c61 7465 2822 4d61  t(_translate("Ma
+00012d50: 696e 5769 6e64 6f77 222c 2022 5374 6174  inWindow", "Stat
+00012d60: 696f 6e22 2929 0a20 2020 2020 2020 2073  ion")).        s
+00012d70: 656c 662e 636f 6d62 6f42 6f78 5f72 6573  elf.comboBox_res
+00012d80: 756c 7473 5f73 656c 6563 7469 6f6e 5f73  ults_selection_s
+00012d90: 7461 7469 6f6e 2e73 6574 4974 656d 5465  tation.setItemTe
+00012da0: 7874 2830 2c20 5f74 7261 6e73 6c61 7465  xt(0, _translate
+00012db0: 2822 4d61 696e 5769 6e64 6f77 222c 2022  ("MainWindow", "
+00012dc0: 416c 6c20 7374 6174 696f 6e73 2229 290a  All stations")).
+00012dd0: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
+00012de0: 656c 5f35 2e73 6574 5465 7874 285f 7472  el_5.setText(_tr
+00012df0: 616e 736c 6174 6528 224d 6169 6e57 696e  anslate("MainWin
+00012e00: 646f 7722 2c20 2253 7572 7665 7922 2929  dow", "Survey"))
+00012e10: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
+00012e20: 6d62 6f42 6f78 5f72 6573 756c 7473 5f73  mboBox_results_s
+00012e30: 656c 6563 7469 6f6e 5f73 7572 7665 792e  election_survey.
+00012e40: 7365 7449 7465 6d54 6578 7428 302c 205f  setItemText(0, _
+00012e50: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
+00012e60: 696e 646f 7722 2c20 2241 6c6c 2073 7572  indow", "All sur
+00012e70: 7665 7973 2229 290a 2020 2020 2020 2020  veys")).        
+00012e80: 7365 6c66 2e67 726f 7570 426f 785f 6769  self.groupBox_gi
+00012e90: 735f 6461 7461 2e73 6574 546f 6f6c 5469  s_data.setToolTi
+00012ea0: 7028 5f74 7261 6e73 6c61 7465 2822 4d61  p(_translate("Ma
+00012eb0: 696e 5769 6e64 6f77 222c 2022 3c68 746d  inWindow", "<htm
+00012ec0: 6c3e 3c68 6561 642f 3e3c 626f 6479 3e3c  l><head/><body><
+00012ed0: 703e 4578 706f 7274 2074 6865 2063 7572  p>Export the cur
+00012ee0: 7265 6e74 2063 6f6e 7465 6e74 206f 6620  rent content of 
+00012ef0: 7468 6520 6f62 7365 7276 6174 696f 6e73  the observations
+00012f00: 2061 6e64 2074 6865 2073 7461 7469 6f6e   and the station
+00012f10: 7320 7461 626c 6520 746f 2061 6e20 4553  s table to an ES
+00012f20: 5249 2073 6861 7065 6669 6c65 2028 6f62  RI shapefile (ob
+00012f30: 735f 7265 7375 6c74 732e 7368 7020 616e  s_results.shp an
+00012f40: 6420 7374 6174 5f72 6573 756c 7473 2e73  d stat_results.s
+00012f50: 6870 292e 2050 6c65 6173 6520 6465 636c  hp). Please decl
+00012f60: 6172 6520 7468 6520 4352 5320 6f66 2074  are the CRS of t
+00012f70: 6865 2073 7461 7469 6f6e 2063 6f6f 7264  he station coord
+00012f80: 696e 6174 6573 2062 7920 6120 7661 6c69  inates by a vali
+00012f90: 6420 4550 5347 2063 6f64 652e 2054 6865  d EPSG code. The
+00012fa0: 2066 696c 6573 2061 7265 2077 7269 7474   files are writt
+00012fb0: 656e 2074 6f20 7468 6520 6361 6d70 6169  en to the campai
+00012fc0: 676e 5c27 7320 6f75 7470 7574 2064 6972  gn\'s output dir
+00012fd0: 6563 746f 7279 2e20 3c2f 703e 3c2f 626f  ectory. </p></bo
+00012fe0: 6479 3e3c 2f68 746d 6c3e 2229 290a 2020  dy></html>")).  
+00012ff0: 2020 2020 2020 7365 6c66 2e67 726f 7570        self.group
+00013000: 426f 785f 6769 735f 6461 7461 2e73 6574  Box_gis_data.set
+00013010: 5469 746c 6528 5f74 7261 6e73 6c61 7465  Title(_translate
+00013020: 2822 4d61 696e 5769 6e64 6f77 222c 2022  ("MainWindow", "
+00013030: 4749 5320 6461 7461 2229 290a 2020 2020  GIS data")).    
+00013040: 2020 2020 7365 6c66 2e70 7573 6842 7574      self.pushBut
+00013050: 746f 6e5f 7265 7375 6c74 735f 6578 706f  ton_results_expo
+00013060: 7274 5f73 6861 7065 6669 6c65 2e73 6574  rt_shapefile.set
+00013070: 546f 6f6c 5469 7028 5f74 7261 6e73 6c61  ToolTip(_transla
+00013080: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
+00013090: 2022 3c68 746d 6c3e 3c68 6561 642f 3e3c   "<html><head/><
+000130a0: 626f 6479 3e3c 703e 4578 706f 7274 2020  body><p>Export  
+000130b0: 7468 6520 6375 7272 656e 7420 636f 6e74  the current cont
+000130c0: 656e 7420 6f66 2074 6865 206f 6273 6572  ent of the obser
+000130d0: 7661 7469 6f6e 7320 616e 6420 7468 6520  vations and the 
+000130e0: 7374 6174 696f 6e73 2074 6162 6c65 2074  stations table t
+000130f0: 6f20 616e 2045 5352 4920 7368 6170 6566  o an ESRI shapef
+00013100: 696c 6520 2826 6c74 3b63 616d 7061 6967  ile (&lt;campaig
+00013110: 6e20 6e61 6d65 2667 743b 5f6f 6273 2e73  n name&gt;_obs.s
+00013120: 6870 2061 6e64 2026 6c74 3b63 616d 7061  hp and &lt;campa
+00013130: 6967 6e20 6e61 6d65 2667 743b 5f73 7461  ign name&gt;_sta
+00013140: 742e 7368 7029 2e3c 2f70 3e3c 2f62 6f64  t.shp).</p></bod
+00013150: 793e 3c2f 6874 6d6c 3e22 2929 0a20 2020  y></html>")).   
+00013160: 2020 2020 2073 656c 662e 7075 7368 4275       self.pushBu
+00013170: 7474 6f6e 5f72 6573 756c 7473 5f65 7870  tton_results_exp
+00013180: 6f72 745f 7368 6170 6566 696c 652e 7365  ort_shapefile.se
+00013190: 7454 6578 7428 5f74 7261 6e73 6c61 7465  tText(_translate
+000131a0: 2822 4d61 696e 5769 6e64 6f77 222c 2022  ("MainWindow", "
+000131b0: 4578 706f 7274 2073 6861 7065 6669 6c65  Export shapefile
+000131c0: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+000131d0: 2e67 726f 7570 426f 785f 7265 7375 6c74  .groupBox_result
+000131e0: 735f 696e 666f 2e73 6574 5469 746c 6528  s_info.setTitle(
+000131f0: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
+00013200: 5769 6e64 6f77 222c 2022 496e 666f 2229  Window", "Info")
+00013210: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
+00013220: 6162 656c 5f33 2e73 6574 546f 6f6c 5469  abel_3.setToolTi
+00013230: 7028 5f74 7261 6e73 6c61 7465 2822 4d61  p(_translate("Ma
+00013240: 696e 5769 6e64 6f77 222c 2022 4164 6a75  inWindow", "Adju
+00013250: 7374 6d65 6e74 206d 6574 686f 642e 2229  stment method.")
+00013260: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
+00013270: 6162 656c 5f33 2e73 6574 5465 7874 285f  abel_3.setText(_
+00013280: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
+00013290: 696e 646f 7722 2c20 2241 646a 7573 746d  indow", "Adjustm
+000132a0: 656e 7420 6d65 7468 6f64 3a22 2929 0a20  ent method:")). 
+000132b0: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
+000132c0: 6c5f 382e 7365 7454 6f6f 6c54 6970 285f  l_8.setToolTip(_
+000132d0: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
+000132e0: 696e 646f 7722 2c20 224e 756d 6265 7220  indow", "Number 
+000132f0: 6f66 2069 7465 7261 7469 6f6e 7320 696e  of iterations in
+00013300: 2063 6173 6520 7468 6520 6974 6572 6174   case the iterat
+00013310: 6976 6520 6164 6a75 7374 656d 6e74 206f  ive adjustemnt o
+00013320: 6620 7330 c2b2 2077 6173 2073 656c 6563  f s0.. was selec
+00013330: 7465 642e 2229 290a 2020 2020 2020 2020  ted.")).        
+00013340: 7365 6c66 2e6c 6162 656c 5f38 2e73 6574  self.label_8.set
+00013350: 5465 7874 285f 7472 616e 736c 6174 6528  Text(_translate(
+00013360: 224d 6169 6e57 696e 646f 7722 2c20 224e  "MainWindow", "N
+00013370: 756d 6265 7220 6f66 2069 7465 7261 7469  umber of iterati
+00013380: 6f6e 733a 2229 290a 2020 2020 2020 2020  ons:")).        
+00013390: 7365 6c66 2e6c 6162 656c 5f31 302e 7365  self.label_10.se
+000133a0: 7454 6f6f 6c54 6970 285f 7472 616e 736c  tToolTip(_transl
+000133b0: 6174 6528 224d 6169 6e57 696e 646f 7722  ate("MainWindow"
+000133c0: 2c20 224f 7074 696f 6e61 6c20 636f 6d6d  , "Optional comm
+000133d0: 656e 7420 6f6e 2074 6865 206c 736d 2072  ent on the lsm r
+000133e0: 756e 2e22 2929 0a20 2020 2020 2020 2073  un.")).        s
+000133f0: 656c 662e 6c61 6265 6c5f 3130 2e73 6574  elf.label_10.set
+00013400: 5465 7874 285f 7472 616e 736c 6174 6528  Text(_translate(
+00013410: 224d 6169 6e57 696e 646f 7722 2c20 2243  "MainWindow", "C
+00013420: 6f6d 6d65 6e74 3a20 2229 290a 2020 2020  omment: ")).    
+00013430: 2020 2020 7365 6c66 2e6c 6162 656c 5f34      self.label_4
+00013440: 2e73 6574 546f 6f6c 5469 7028 5f74 7261  .setToolTip(_tra
+00013450: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
+00013460: 6f77 222c 2022 5469 6d65 2061 6e64 2064  ow", "Time and d
+00013470: 6174 6520 7468 6520 6164 6a75 7374 6d65  ate the adjustme
+00013480: 6e74 2077 6173 2063 6172 7269 6564 206f  nt was carried o
+00013490: 7574 2e22 2929 0a20 2020 2020 2020 2073  ut.")).        s
+000134a0: 656c 662e 6c61 6265 6c5f 342e 7365 7454  elf.label_4.setT
+000134b0: 6578 7428 5f74 7261 6e73 6c61 7465 2822  ext(_translate("
+000134c0: 4d61 696e 5769 6e64 6f77 222c 2022 5469  MainWindow", "Ti
+000134d0: 6d65 2061 6e64 2044 6174 653a 2229 290a  me and Date:")).
+000134e0: 2020 2020 2020 2020 7365 6c66 2e67 726f          self.gro
+000134f0: 7570 426f 785f 7265 7375 6c74 735f 7374  upBox_results_st
+00013500: 6174 6973 7469 6373 2e73 6574 5469 746c  atistics.setTitl
+00013510: 6528 5f74 7261 6e73 6c61 7465 2822 4d61  e(_translate("Ma
+00013520: 696e 5769 6e64 6f77 222c 2022 5374 6174  inWindow", "Stat
+00013530: 6973 7469 6373 2061 6e64 2074 6573 7473  istics and tests
+00013540: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+00013550: 2e6c 6162 656c 5f39 2e73 6574 546f 6f6c  .label_9.setTool
+00013560: 5469 7028 5f74 7261 6e73 6c61 7465 2822  Tip(_translate("
+00013570: 4d61 696e 5769 6e64 6f77 222c 2022 4120  MainWindow", "A 
+00013580: 706f 7374 6572 696f 7269 2076 6172 6961  posteriori varia
+00013590: 6e63 6520 6f66 2075 6e69 7420 7765 6967  nce of unit weig
+000135a0: 6874 2e22 2929 0a20 2020 2020 2020 2073  ht.")).        s
+000135b0: 656c 662e 6c61 6265 6c5f 392e 7365 7454  elf.label_9.setT
+000135c0: 6578 7428 5f74 7261 6e73 6c61 7465 2822  ext(_translate("
+000135d0: 4d61 696e 5769 6e64 6f77 222c 2022 7330  MainWindow", "s0
+000135e0: c2b2 3a22 2929 0a20 2020 2020 2020 2073  ..:")).        s
+000135f0: 656c 662e 6c61 6265 6c5f 362e 7365 7454  elf.label_6.setT
+00013600: 6f6f 6c54 6970 285f 7472 616e 736c 6174  oolTip(_translat
+00013610: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
+00013620: 224f 7574 636f 6d65 206f 6620 7468 6520  "Outcome of the 
+00013630: 676c 6f62 616c 206d 6f64 656c 2074 6573  global model tes
+00013640: 742e 2229 290a 2020 2020 2020 2020 7365  t.")).        se
+00013650: 6c66 2e6c 6162 656c 5f36 2e73 6574 5465  lf.label_6.setTe
+00013660: 7874 285f 7472 616e 736c 6174 6528 224d  xt(_translate("M
+00013670: 6169 6e57 696e 646f 7722 2c20 2247 6f6f  ainWindow", "Goo
+00013680: 646e 6573 732d 6f66 2d66 6974 2074 6573  dness-of-fit tes
+00013690: 743a 2229 290a 2020 2020 2020 2020 7365  t:")).        se
+000136a0: 6c66 2e6c 6162 656c 5f37 2e73 6574 546f  lf.label_7.setTo
+000136b0: 6f6c 5469 7028 5f74 7261 6e73 6c61 7465  olTip(_translate
+000136c0: 2822 4d61 696e 5769 6e64 6f77 222c 2022  ("MainWindow", "
+000136d0: 4e75 6d62 6572 206f 6620 6465 7465 6374  Number of detect
+000136e0: 6564 206f 7574 6c69 6572 732e 2229 290a  ed outliers.")).
+000136f0: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
+00013700: 656c 5f37 2e73 6574 5465 7874 285f 7472  el_7.setText(_tr
+00013710: 616e 736c 6174 6528 224d 6169 6e57 696e  anslate("MainWin
+00013720: 646f 7722 2c20 224e 756d 6265 7220 6f66  dow", "Number of
+00013730: 206f 7574 6c69 6572 733a 2229 290a 2020   outliers:")).  
+00013740: 2020 2020 2020 7365 6c66 2e67 726f 7570        self.group
+00013750: 426f 785f 7265 7375 6c74 735f 6c73 6d5f  Box_results_lsm_
+00013760: 7275 6e5f 6c6f 672e 7365 7454 6974 6c65  run_log.setTitle
+00013770: 285f 7472 616e 736c 6174 6528 224d 6169  (_translate("Mai
+00013780: 6e57 696e 646f 7722 2c20 224c 534d 2072  nWindow", "LSM r
+00013790: 756e 206c 6f67 2229 290a 2020 2020 2020  un log")).      
+000137a0: 2020 7365 6c66 2e74 6162 5769 6467 6574    self.tabWidget
+000137b0: 5f72 6573 756c 7473 2e73 6574 5461 6254  _results.setTabT
+000137c0: 6578 7428 7365 6c66 2e74 6162 5769 6467  ext(self.tabWidg
+000137d0: 6574 5f72 6573 756c 7473 2e69 6e64 6578  et_results.index
+000137e0: 4f66 2873 656c 662e 7461 625f 7265 7375  Of(self.tab_resu
+000137f0: 6c74 735f 696e 666f 292c 205f 7472 616e  lts_info), _tran
+00013800: 736c 6174 6528 224d 6169 6e57 696e 646f  slate("MainWindo
+00013810: 7722 2c20 2249 6e66 6f22 2929 0a20 2020  w", "Info")).   
+00013820: 2020 2020 2073 656c 662e 7461 6257 6964       self.tabWid
+00013830: 6765 745f 7265 7375 6c74 732e 7365 7454  get_results.setT
+00013840: 6162 5465 7874 2873 656c 662e 7461 6257  abText(self.tabW
+00013850: 6964 6765 745f 7265 7375 6c74 732e 696e  idget_results.in
+00013860: 6465 784f 6628 7365 6c66 2e74 6162 5f72  dexOf(self.tab_r
+00013870: 6573 756c 7473 5f6f 6273 5f74 6162 6c65  esults_obs_table
+00013880: 292c 205f 7472 616e 736c 6174 6528 224d  ), _translate("M
+00013890: 6169 6e57 696e 646f 7722 2c20 224f 6273  ainWindow", "Obs
+000138a0: 6572 7661 7469 6f6e 7320 5461 626c 6522  ervations Table"
+000138b0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+000138c0: 6772 6f75 7042 6f78 5f70 6c6f 745f 7365  groupBox_plot_se
+000138d0: 7474 696e 6773 2e73 6574 5469 746c 6528  ttings.setTitle(
+000138e0: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
+000138f0: 5769 6e64 6f77 222c 2022 506c 6f74 2073  Window", "Plot s
+00013900: 6574 7469 6e67 7322 2929 0a20 2020 2020  ettings")).     
+00013910: 2020 2073 656c 662e 6c61 6265 6c5f 7265     self.label_re
+00013920: 7375 6c74 735f 6f62 735f 706c 6f74 5f73  sults_obs_plot_s
+00013930: 656c 6563 5f64 6174 615f 636f 6c75 6d6e  elec_data_column
+00013940: 2e73 6574 5465 7874 285f 7472 616e 736c  .setText(_transl
+00013950: 6174 6528 224d 6169 6e57 696e 646f 7722  ate("MainWindow"
+00013960: 2c20 2253 656c 6563 7420 6461 7461 2063  , "Select data c
+00013970: 6f6c 756d 6e3a 2229 290a 2020 2020 2020  olumn:")).      
+00013980: 2020 7365 6c66 2e72 6164 696f 4275 7474    self.radioButt
+00013990: 6f6e 5f72 6573 756c 7473 5f6f 6273 5f70  on_results_obs_p
+000139a0: 6c6f 745f 7469 6d65 7365 7269 6573 2e73  lot_timeseries.s
+000139b0: 6574 5465 7874 285f 7472 616e 736c 6174  etText(_translat
+000139c0: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
+000139d0: 2254 696d 6520 7365 7269 6573 2229 290a  "Time series")).
+000139e0: 2020 2020 2020 2020 7365 6c66 2e72 6164          self.rad
+000139f0: 696f 4275 7474 6f6e 5f72 6573 756c 7473  ioButton_results
+00013a00: 5f6f 6273 5f70 6c6f 745f 6869 7374 6f67  _obs_plot_histog
+00013a10: 7261 6d2e 7365 7454 6578 7428 5f74 7261  ram.setText(_tra
+00013a20: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
+00013a30: 6f77 222c 2022 4869 7374 6f67 7261 6d22  ow", "Histogram"
+00013a40: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+00013a50: 6772 6f75 7042 6f78 5f68 6973 746f 6772  groupBox_histogr
+00013a60: 616d 5f73 6574 7469 6e67 732e 7365 7454  am_settings.setT
+00013a70: 6974 6c65 285f 7472 616e 736c 6174 6528  itle(_translate(
+00013a80: 224d 6169 6e57 696e 646f 7722 2c20 2248  "MainWindow", "H
+00013a90: 6973 746f 6772 616d 2073 6574 7469 6e67  istogram setting
+00013aa0: 7322 2929 0a20 2020 2020 2020 2073 656c  s")).        sel
+00013ab0: 662e 6c61 6265 6c5f 3131 2e73 6574 5465  f.label_11.setTe
+00013ac0: 7874 285f 7472 616e 736c 6174 6528 224d  xt(_translate("M
+00013ad0: 6169 6e57 696e 646f 7722 2c20 224d 6574  ainWindow", "Met
+00013ae0: 686f 6422 2929 0a20 2020 2020 2020 2073  hod")).        s
+00013af0: 656c 662e 6c61 6265 6c5f 7265 7375 6c74  elf.label_result
+00013b00: 735f 6f62 735f 706c 6f74 5f6e 756d 6265  s_obs_plot_numbe
+00013b10: 725f 6269 6e73 2e73 6574 5465 7874 285f  r_bins.setText(_
+00013b20: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
+00013b30: 696e 646f 7722 2c20 224e 756d 6265 7220  indow", "Number 
+00013b40: 6f66 2062 696e 7322 2929 0a20 2020 2020  of bins")).     
+00013b50: 2020 2073 656c 662e 6368 6563 6b42 6f78     self.checkBox
+00013b60: 5f72 6573 756c 7473 5f6f 6273 5f70 6c6f  _results_obs_plo
+00013b70: 745f 7368 6f77 5f6f 7574 6c69 6572 732e  t_show_outliers.
+00013b80: 7365 7454 6578 7428 5f74 7261 6e73 6c61  setText(_transla
+00013b90: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
+00013ba0: 2022 5368 6f77 206f 7574 6c69 6572 7322   "Show outliers"
+00013bb0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+00013bc0: 7461 6257 6964 6765 745f 7265 7375 6c74  tabWidget_result
+00013bd0: 732e 7365 7454 6162 5465 7874 2873 656c  s.setTabText(sel
+00013be0: 662e 7461 6257 6964 6765 745f 7265 7375  f.tabWidget_resu
+00013bf0: 6c74 732e 696e 6465 784f 6628 7365 6c66  lts.indexOf(self
+00013c00: 2e74 6162 5f72 6573 756c 7473 5f6f 6273  .tab_results_obs
+00013c10: 5f70 6c6f 7473 292c 205f 7472 616e 736c  _plots), _transl
+00013c20: 6174 6528 224d 6169 6e57 696e 646f 7722  ate("MainWindow"
+00013c30: 2c20 224f 6273 6572 7661 7469 6f6e 7320  , "Observations 
+00013c40: 506c 6f74 7322 2929 0a20 2020 2020 2020  Plots")).       
+00013c50: 2073 656c 662e 7461 6257 6964 6765 745f   self.tabWidget_
+00013c60: 7265 7375 6c74 732e 7365 7454 6162 5465  results.setTabTe
+00013c70: 7874 2873 656c 662e 7461 6257 6964 6765  xt(self.tabWidge
+00013c80: 745f 7265 7375 6c74 732e 696e 6465 784f  t_results.indexO
+00013c90: 6628 7365 6c66 2e74 6162 5f72 6573 756c  f(self.tab_resul
+00013ca0: 7473 5f64 7269 6674 292c 205f 7472 616e  ts_drift), _tran
+00013cb0: 736c 6174 6528 224d 6169 6e57 696e 646f  slate("MainWindo
+00013cc0: 7722 2c20 2244 7269 6674 2054 6162 6c65  w", "Drift Table
+00013cd0: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+00013ce0: 2e67 7261 7068 6963 734c 6179 6f75 7457  .graphicsLayoutW
+00013cf0: 6964 6765 745f 7265 7375 6c74 735f 6472  idget_results_dr
+00013d00: 6966 745f 706c 6f74 2e73 6574 546f 6f6c  ift_plot.setTool
+00013d10: 5469 7028 5f74 7261 6e73 6c61 7465 2822  Tip(_translate("
+00013d20: 4d61 696e 5769 6e64 6f77 222c 2022 3c68  MainWindow", "<h
+00013d30: 746d 6c3e 3c68 6561 642f 3e3c 626f 6479  tml><head/><body
+00013d40: 3e3c 703e 5468 6973 2070 6c6f 7420 6465  ><p>This plot de
+00013d50: 7069 6374 7320 7365 7475 7020 6f62 7365  picts setup obse
+00013d60: 7276 6174 696f 6e73 2061 6e64 2074 6865  rvations and the
+00013d70: 2074 6865 2064 7269 6674 2066 756e 6374   the drift funct
+00013d80: 696f 6e20 2870 6f6c 796e 6f6d 6961 6c20  ion (polynomial 
+00013d90: 6f66 2064 6567 7265 6520 6e29 2066 6974  of degree n) fit
+00013da0: 7465 6420 746f 2074 6865 7365 206f 6273  ted to these obs
+00013db0: 6572 7661 7469 6f6e 732e 3c2f 703e 3c2f  ervations.</p></
+00013dc0: 626f 6479 3e3c 2f68 746d 6c3e 2229 290a  body></html>")).
+00013dd0: 2020 2020 2020 2020 7365 6c66 2e67 726f          self.gro
+00013de0: 7570 426f 785f 7265 7375 6c74 735f 6472  upBox_results_dr
+00013df0: 6966 745f 706c 6f74 2e73 6574 5469 746c  ift_plot.setTitl
+00013e00: 6528 5f74 7261 6e73 6c61 7465 2822 4d61  e(_translate("Ma
+00013e10: 696e 5769 6e64 6f77 222c 2022 4472 6966  inWindow", "Drif
+00013e20: 7420 706c 6f74 2073 6574 7469 6e67 7322  t plot settings"
+00013e30: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+00013e40: 6c61 6265 6c5f 7265 7375 6c74 735f 6472  label_results_dr
+00013e50: 6966 745f 706c 6f74 5f76 5f6f 6666 7365  ift_plot_v_offse
+00013e60: 742e 7365 7454 6f6f 6c54 6970 285f 7472  t.setToolTip(_tr
+00013e70: 616e 736c 6174 6528 224d 6169 6e57 696e  anslate("MainWin
+00013e80: 646f 7722 2c20 223c 6874 6d6c 3e3c 6865  dow", "<html><he
+00013e90: 6164 2f3e 3c62 6f64 793e 3c70 3e41 6464  ad/><body><p>Add
+00013ea0: 2076 6572 7469 6361 6c20 6f66 6673 6574   vertical offset
+00013eb0: 2074 6f20 7468 6520 6472 6966 7420 6675   to the drift fu
+00013ec0: 6e63 7469 6f6e 2028 706f 6c79 6e6f 6d69  nction (polynomi
+00013ed0: 616c 2920 772e 722e 742e 2074 6865 2073  al) w.r.t. the s
+00013ee0: 6574 7570 206f 6273 6572 7661 7469 6f6e  etup observation
+00013ef0: 732e 2054 6869 7320 6973 206e 6565 6465  s. This is neede
+00013f00: 6420 746f 2077 6865 6e20 6469 6666 6572  d to when differ
+00013f10: 656e 7469 616c 206f 6273 6572 7661 7469  ential observati
+00013f20: 6f6e 7320 6172 6520 7573 6564 2066 6f72  ons are used for
+00013f30: 2070 7261 6d65 7465 7220 6573 7469 6d61   prameter estima
+00013f40: 7469 6f6e 2e20 496e 2074 6869 7320 6361  tion. In this ca
+00013f50: 7365 2074 6865 2063 6f6e 7374 616e 7420  se the constant 
+00013f60: 6269 6173 206f 6620 7468 6520 6772 6176  bias of the grav
+00013f70: 696d 6574 6572 2072 6561 6469 6e67 2063  imeter reading c
+00013f80: 616e 6e6f 7420 6265 2065 7374 696d 6174  annot be estimat
+00013f90: 6564 2061 6e64 2069 7320 6f6e 6c79 2064  ed and is only d
+00013fa0: 6574 6572 6d69 6e65 6420 6170 7072 6f78  etermined approx
+00013fb0: 696d 6174 656c 792e 3c2f 703e 3c2f 626f  imately.</p></bo
+00013fc0: 6479 3e3c 2f68 746d 6c3e 2229 290a 2020  dy></html>")).  
+00013fd0: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
+00013fe0: 5f72 6573 756c 7473 5f64 7269 6674 5f70  _results_drift_p
+00013ff0: 6c6f 745f 765f 6f66 6673 6574 2e73 6574  lot_v_offset.set
+00014000: 5465 7874 285f 7472 616e 736c 6174 6528  Text(_translate(
+00014010: 224d 6169 6e57 696e 646f 7722 2c20 2256  "MainWindow", "V
+00014020: 6572 7469 6361 6c20 6f66 6673 6574 206f  ertical offset o
+00014030: 6620 6472 6966 7420 706f 6c79 6e6f 6d69  f drift polynomi
+00014040: 616c 2077 2e72 2e74 2e20 7365 7475 7020  al w.r.t. setup 
+00014050: 6f62 7365 7276 6174 696f 6e73 205b c2b5  observations [..
+00014060: 4761 6c5d 2229 290a 2020 2020 2020 2020  Gal]")).        
+00014070: 7365 6c66 2e73 7069 6e42 6f78 5f72 6573  self.spinBox_res
+00014080: 756c 7473 5f64 7269 6674 5f70 6c6f 745f  ults_drift_plot_
+00014090: 765f 6f66 6673 6574 2e73 6574 546f 6f6c  v_offset.setTool
+000140a0: 5469 7028 5f74 7261 6e73 6c61 7465 2822  Tip(_translate("
+000140b0: 4d61 696e 5769 6e64 6f77 222c 2022 3c68  MainWindow", "<h
+000140c0: 746d 6c3e 3c68 6561 642f 3e3c 626f 6479  tml><head/><body
+000140d0: 3e3c 703e 4164 6420 7665 7274 6963 616c  ><p>Add vertical
+000140e0: 206f 6666 7365 7420 746f 2074 6865 2064   offset to the d
+000140f0: 7269 6674 2066 756e 6374 696f 6e20 2870  rift function (p
+00014100: 6f6c 796e 6f6d 6961 6c29 2077 2e72 2e74  olynomial) w.r.t
+00014110: 2e20 7468 6520 7365 7475 7020 6f62 7365  . the setup obse
+00014120: 7276 6174 696f 6e73 2e20 5468 6973 2069  rvations. This i
+00014130: 7320 6e65 6564 6564 2074 6f20 7768 656e  s needed to when
+00014140: 2064 6966 6665 7265 6e74 6961 6c20 6f62   differential ob
+00014150: 7365 7276 6174 696f 6e73 2061 7265 2075  servations are u
+00014160: 7365 6420 666f 7220 7072 616d 6574 6572  sed for prameter
+00014170: 2065 7374 696d 6174 696f 6e2e 2049 6e20   estimation. In 
+00014180: 7468 6973 2063 6173 6520 7468 6520 636f  this case the co
+00014190: 6e73 7461 6e74 2062 6961 7320 6f66 2074  nstant bias of t
+000141a0: 6865 2067 7261 7669 6d65 7465 7220 7265  he gravimeter re
+000141b0: 6164 696e 6720 6361 6e6e 6f74 2062 6520  ading cannot be 
+000141c0: 6573 7469 6d61 7465 6420 616e 6420 6973  estimated and is
+000141d0: 206f 6e6c 7920 6465 7465 726d 696e 6564   only determined
+000141e0: 2061 7070 726f 7869 6d61 7465 6c79 2e3c   approximately.<
+000141f0: 2f70 3e3c 2f62 6f64 793e 3c2f 6874 6d6c  /p></body></html
+00014200: 3e22 2929 0a20 2020 2020 2020 2073 656c  >")).        sel
+00014210: 662e 7461 6257 6964 6765 745f 7265 7375  f.tabWidget_resu
+00014220: 6c74 732e 7365 7454 6162 5465 7874 2873  lts.setTabText(s
+00014230: 656c 662e 7461 6257 6964 6765 745f 7265  elf.tabWidget_re
+00014240: 7375 6c74 732e 696e 6465 784f 6628 7365  sults.indexOf(se
+00014250: 6c66 2e74 6162 5f72 6573 756c 7473 5f64  lf.tab_results_d
+00014260: 7269 6674 706c 6f74 292c 205f 7472 616e  riftplot), _tran
+00014270: 736c 6174 6528 224d 6169 6e57 696e 646f  slate("MainWindo
+00014280: 7722 2c20 2244 7269 6674 2050 6c6f 7422  w", "Drift Plot"
+00014290: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+000142a0: 6772 6f75 7042 6f78 5f72 6573 756c 7473  groupBox_results
+000142b0: 5f73 7461 7469 6f6e 735f 7374 6174 6973  _stations_statis
+000142c0: 7469 6373 2e73 6574 546f 6f6c 5469 7028  tics.setToolTip(
+000142d0: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
+000142e0: 5769 6e64 6f77 222c 2022 3c68 746d 6c3e  Window", "<html>
+000142f0: 3c68 6561 642f 3e3c 626f 6479 3e3c 703e  <head/><body><p>
+00014300: 4361 6c63 756c 6174 6520 616e 6420 6469  Calculate and di
+00014310: 7370 6c61 7920 6465 7363 7269 7074 6976  splay descriptiv
+00014320: 6520 7374 6174 6973 7469 6373 2066 6f72  e statistics for
+00014330: 2074 6865 2073 656c 6563 7465 6420 6461   the selected da
+00014340: 7461 2063 6f6c 756d 6e2e 3c2f 703e 3c2f  ta column.</p></
+00014350: 626f 6479 3e3c 2f68 746d 6c3e 2229 290a  body></html>")).
+00014360: 2020 2020 2020 2020 7365 6c66 2e67 726f          self.gro
+00014370: 7570 426f 785f 7265 7375 6c74 735f 7374  upBox_results_st
+00014380: 6174 696f 6e73 5f73 7461 7469 7374 6963  ations_statistic
+00014390: 732e 7365 7454 6974 6c65 285f 7472 616e  s.setTitle(_tran
+000143a0: 736c 6174 6528 224d 6169 6e57 696e 646f  slate("MainWindo
+000143b0: 7722 2c20 2253 7461 7469 7374 6963 7322  w", "Statistics"
+000143c0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+000143d0: 6c61 6265 6c5f 3132 2e73 6574 546f 6f6c  label_12.setTool
+000143e0: 5469 7028 5f74 7261 6e73 6c61 7465 2822  Tip(_translate("
+000143f0: 4d61 696e 5769 6e64 6f77 222c 2022 3c68  MainWindow", "<h
+00014400: 746d 6c3e 3c68 6561 642f 3e3c 626f 6479  tml><head/><body
+00014410: 3e3c 703e 5365 6c65 6374 2064 6174 6120  ><p>Select data 
+00014420: 636f 6c75 6d6e 2066 6f72 2064 6973 706c  column for displ
+00014430: 6179 696e 6720 7374 6174 6973 7469 6373  aying statistics
+00014440: 2e3c 2f70 3e3c 2f62 6f64 793e 3c2f 6874  .</p></body></ht
+00014450: 6d6c 3e22 2929 0a20 2020 2020 2020 2073  ml>")).        s
+00014460: 656c 662e 6c61 6265 6c5f 3132 2e73 6574  elf.label_12.set
+00014470: 5465 7874 285f 7472 616e 736c 6174 6528  Text(_translate(
+00014480: 224d 6169 6e57 696e 646f 7722 2c20 2253  "MainWindow", "S
+00014490: 656c 6563 7420 636f 6c75 6d6e 2229 290a  elect column")).
+000144a0: 2020 2020 2020 2020 7365 6c66 2e63 6f6d          self.com
+000144b0: 626f 426f 785f 7265 7375 6c74 735f 7374  boBox_results_st
+000144c0: 6174 696f 6e73 5f73 7461 7469 7374 6963  ations_statistic
+000144d0: 735f 7365 6c65 6374 5f63 6f6c 2e73 6574  s_select_col.set
+000144e0: 546f 6f6c 5469 7028 5f74 7261 6e73 6c61  ToolTip(_transla
+000144f0: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
+00014500: 2022 3c68 746d 6c3e 3c68 6561 642f 3e3c   "<html><head/><
+00014510: 626f 6479 3e3c 703e 5365 6c65 6374 2064  body><p>Select d
+00014520: 6174 6120 636f 6c75 6d6e 2066 6f72 2064  ata column for d
+00014530: 6973 706c 6179 696e 6720 7374 6174 6973  isplaying statis
+00014540: 7469 6373 2e3c 2f70 3e3c 2f62 6f64 793e  tics.</p></body>
+00014550: 3c2f 6874 6d6c 3e22 2929 0a20 2020 2020  </html>")).     
+00014560: 2020 2073 656c 662e 6c61 6265 6c5f 3133     self.label_13
+00014570: 2e73 6574 546f 6f6c 5469 7028 5f74 7261  .setToolTip(_tra
+00014580: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
+00014590: 6f77 222c 2022 4d65 616e 2229 290a 2020  ow", "Mean")).  
+000145a0: 2020 2020 2020 7365 6c66 2e6c 6162 656c        self.label
+000145b0: 5f31 332e 7365 7454 6578 7428 5f74 7261  _13.setText(_tra
+000145c0: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
+000145d0: 6f77 222c 2022 4d65 616e 3a22 2929 0a20  ow", "Mean:")). 
+000145e0: 2020 2020 2020 2073 656c 662e 6c61 6265         self.labe
+000145f0: 6c5f 7265 7375 6c74 735f 7374 6174 696f  l_results_statio
+00014600: 6e73 5f73 7461 7469 7374 6963 735f 6d65  ns_statistics_me
+00014610: 616e 2e73 6574 546f 6f6c 5469 7028 5f74  an.setToolTip(_t
+00014620: 7261 6e73 6c61 7465 2822 4d61 696e 5769  ranslate("MainWi
+00014630: 6e64 6f77 222c 2022 4d65 616e 2229 290a  ndow", "Mean")).
+00014640: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
+00014650: 656c 5f31 342e 7365 7454 6f6f 6c54 6970  el_14.setToolTip
+00014660: 285f 7472 616e 736c 6174 6528 224d 6169  (_translate("Mai
+00014670: 6e57 696e 646f 7722 2c20 2253 7461 6e64  nWindow", "Stand
+00014680: 6172 6420 6465 7669 6174 696f 6e22 2929  ard deviation"))
+00014690: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
+000146a0: 6265 6c5f 3134 2e73 6574 5465 7874 285f  bel_14.setText(_
+000146b0: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
+000146c0: 696e 646f 7722 2c20 2253 7464 2e3a 2229  indow", "Std.:")
+000146d0: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
+000146e0: 6162 656c 5f72 6573 756c 7473 5f73 7461  abel_results_sta
+000146f0: 7469 6f6e 735f 7374 6174 6973 7469 6373  tions_statistics
+00014700: 5f73 7464 2e73 6574 546f 6f6c 5469 7028  _std.setToolTip(
+00014710: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
+00014720: 5769 6e64 6f77 222c 2022 5374 616e 6461  Window", "Standa
+00014730: 7264 2064 6576 6961 7469 6f6e 2229 290a  rd deviation")).
+00014740: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
+00014750: 656c 5f31 352e 7365 7454 6f6f 6c54 6970  el_15.setToolTip
+00014760: 285f 7472 616e 736c 6174 6528 224d 6169  (_translate("Mai
+00014770: 6e57 696e 646f 7722 2c20 224d 696e 696d  nWindow", "Minim
+00014780: 756d 2229 290a 2020 2020 2020 2020 7365  um")).        se
+00014790: 6c66 2e6c 6162 656c 5f31 352e 7365 7454  lf.label_15.setT
+000147a0: 6578 7428 5f74 7261 6e73 6c61 7465 2822  ext(_translate("
+000147b0: 4d61 696e 5769 6e64 6f77 222c 2022 4d69  MainWindow", "Mi
+000147c0: 6e2e 3a22 2929 0a20 2020 2020 2020 2073  n.:")).        s
+000147d0: 656c 662e 6c61 6265 6c5f 7265 7375 6c74  elf.label_result
+000147e0: 735f 7374 6174 696f 6e73 5f73 7461 7469  s_stations_stati
+000147f0: 7374 6963 735f 6d69 6e2e 7365 7454 6f6f  stics_min.setToo
+00014800: 6c54 6970 285f 7472 616e 736c 6174 6528  lTip(_translate(
+00014810: 224d 6169 6e57 696e 646f 7722 2c20 224d  "MainWindow", "M
+00014820: 696e 696d 756d 2229 290a 2020 2020 2020  inimum")).      
+00014830: 2020 7365 6c66 2e6c 6162 656c 5f31 362e    self.label_16.
+00014840: 7365 7454 6f6f 6c54 6970 285f 7472 616e  setToolTip(_tran
+00014850: 736c 6174 6528 224d 6169 6e57 696e 646f  slate("MainWindo
+00014860: 7722 2c20 224d 6178 696d 756d 2229 290a  w", "Maximum")).
+00014870: 2020 2020 2020 2020 7365 6c66 2e6c 6162          self.lab
+00014880: 656c 5f31 362e 7365 7454 6578 7428 5f74  el_16.setText(_t
+00014890: 7261 6e73 6c61 7465 2822 4d61 696e 5769  ranslate("MainWi
+000148a0: 6e64 6f77 222c 2022 4d61 782e 3a22 2929  ndow", "Max.:"))
+000148b0: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
+000148c0: 6265 6c5f 7265 7375 6c74 735f 7374 6174  bel_results_stat
+000148d0: 696f 6e73 5f73 7461 7469 7374 6963 735f  ions_statistics_
+000148e0: 6d61 782e 7365 7454 6f6f 6c54 6970 285f  max.setToolTip(_
+000148f0: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
+00014900: 696e 646f 7722 2c20 224d 6178 696d 756d  indow", "Maximum
+00014910: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+00014920: 2e6c 6162 656c 5f31 372e 7365 7454 6f6f  .label_17.setToo
+00014930: 6c54 6970 285f 7472 616e 736c 6174 6528  lTip(_translate(
+00014940: 224d 6169 6e57 696e 646f 7722 2c20 224d  "MainWindow", "M
+00014950: 6564 6961 6e22 2929 0a20 2020 2020 2020  edian")).       
+00014960: 2073 656c 662e 6c61 6265 6c5f 3137 2e73   self.label_17.s
+00014970: 6574 5465 7874 285f 7472 616e 736c 6174  etText(_translat
+00014980: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
+00014990: 224d 6564 6961 6e3a 2229 290a 2020 2020  "Median:")).    
+000149a0: 2020 2020 7365 6c66 2e6c 6162 656c 5f5f      self.label__
+000149b0: 7265 7375 6c74 735f 7374 6174 696f 6e73  results_stations
+000149c0: 5f73 7461 7469 7374 6963 735f 6d65 6469  _statistics_medi
+000149d0: 616e 2e73 6574 546f 6f6c 5469 7028 5f74  an.setToolTip(_t
+000149e0: 7261 6e73 6c61 7465 2822 4d61 696e 5769  ranslate("MainWi
+000149f0: 6e64 6f77 222c 2022 4d65 6469 616e 2229  ndow", "Median")
+00014a00: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
+00014a10: 6162 656c 5f31 382e 7365 7454 6f6f 6c54  abel_18.setToolT
+00014a20: 6970 285f 7472 616e 736c 6174 6528 224d  ip(_translate("M
+00014a30: 6169 6e57 696e 646f 7722 2c20 2249 6e74  ainWindow", "Int
+00014a40: 6572 7175 6172 7469 6c65 2072 616e 6765  erquartile range
+00014a50: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+00014a60: 2e6c 6162 656c 5f31 382e 7365 7454 6578  .label_18.setTex
+00014a70: 7428 5f74 7261 6e73 6c61 7465 2822 4d61  t(_translate("Ma
+00014a80: 696e 5769 6e64 6f77 222c 2022 4951 523a  inWindow", "IQR:
+00014a90: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+00014aa0: 2e6c 6162 656c 5f5f 7265 7375 6c74 735f  .label__results_
+00014ab0: 7374 6174 696f 6e73 5f73 7461 7469 7374  stations_statist
+00014ac0: 6963 735f 6971 722e 7365 7454 6f6f 6c54  ics_iqr.setToolT
+00014ad0: 6970 285f 7472 616e 736c 6174 6528 224d  ip(_translate("M
+00014ae0: 6169 6e57 696e 646f 7722 2c20 2249 6e74  ainWindow", "Int
+00014af0: 6572 7175 6172 7469 6c65 2072 616e 6765  erquartile range
+00014b00: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+00014b10: 2e74 6162 5769 6467 6574 5f72 6573 756c  .tabWidget_resul
+00014b20: 7473 2e73 6574 5461 6254 6578 7428 7365  ts.setTabText(se
+00014b30: 6c66 2e74 6162 5769 6467 6574 5f72 6573  lf.tabWidget_res
+00014b40: 756c 7473 2e69 6e64 6578 4f66 2873 656c  ults.indexOf(sel
+00014b50: 662e 7461 625f 7265 7375 6c74 735f 7374  f.tab_results_st
+00014b60: 6174 5f74 6162 6c65 292c 205f 7472 616e  at_table), _tran
+00014b70: 736c 6174 6528 224d 6169 6e57 696e 646f  slate("MainWindo
+00014b80: 7722 2c20 2220 5374 6174 696f 6e73 2054  w", " Stations T
+00014b90: 6162 6c65 2229 290a 2020 2020 2020 2020  able")).        
+00014ba0: 7365 6c66 2e74 6162 5769 6467 6574 5f72  self.tabWidget_r
+00014bb0: 6573 756c 7473 2e73 6574 5461 6254 6578  esults.setTabTex
+00014bc0: 7428 7365 6c66 2e74 6162 5769 6467 6574  t(self.tabWidget
+00014bd0: 5f72 6573 756c 7473 2e69 6e64 6578 4f66  _results.indexOf
+00014be0: 2873 656c 662e 7461 625f 7265 7375 6c74  (self.tab_result
+00014bf0: 735f 636f 7272 656c 6174 696f 6e5f 6d61  s_correlation_ma
+00014c00: 7472 6978 292c 205f 7472 616e 736c 6174  trix), _translat
+00014c10: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
+00014c20: 2243 6f72 7265 6c61 7469 6f6e 204d 6174  "Correlation Mat
+00014c30: 7269 7822 2929 0a20 2020 2020 2020 2073  rix")).        s
+00014c40: 656c 662e 7461 6257 6964 6765 745f 7265  elf.tabWidget_re
+00014c50: 7375 6c74 732e 7365 7454 6162 5465 7874  sults.setTabText
+00014c60: 2873 656c 662e 7461 6257 6964 6765 745f  (self.tabWidget_
+00014c70: 7265 7375 6c74 732e 696e 6465 784f 6628  results.indexOf(
+00014c80: 7365 6c66 2e74 6162 5f76 675f 7461 626c  self.tab_vg_tabl
+00014c90: 6529 2c20 5f74 7261 6e73 6c61 7465 2822  e), _translate("
+00014ca0: 4d61 696e 5769 6e64 6f77 222c 2022 5647  MainWindow", "VG
+00014cb0: 2054 6162 6c65 2229 290a 2020 2020 2020   Table")).      
+00014cc0: 2020 7365 6c66 2e67 7261 7068 6963 734c    self.graphicsL
+00014cd0: 6179 6f75 7457 6964 6765 745f 7265 7375  ayoutWidget_resu
+00014ce0: 6c74 735f 7667 5f70 6c6f 742e 7365 7454  lts_vg_plot.setT
+00014cf0: 6f6f 6c54 6970 285f 7472 616e 736c 6174  oolTip(_translat
+00014d00: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
+00014d10: 2254 6865 2056 4720 706c 6f74 2069 6c6c  "The VG plot ill
+00014d20: 7573 7461 7274 6573 2074 6865 2065 7374  ustartes the est
+00014d30: 696d 6174 696f 6e20 7265 7375 6c74 7320  imation results 
+00014d40: 6f66 2074 6865 2056 4720 706f 6c79 6e6f  of the VG polyno
+00014d50: 6d69 616c 2e22 2929 0a20 2020 2020 2020  mial.")).       
+00014d60: 2073 656c 662e 6772 6f75 7042 6f78 5f72   self.groupBox_r
+00014d70: 6573 756c 7473 5f76 675f 706c 6f74 5f73  esults_vg_plot_s
+00014d80: 6574 7469 6e67 732e 7365 7454 6f6f 6c54  ettings.setToolT
+00014d90: 6970 285f 7472 616e 736c 6174 6528 224d  ip(_translate("M
+00014da0: 6169 6e57 696e 646f 7722 2c20 2253 6574  ainWindow", "Set
+00014db0: 7469 6e67 7320 666f 7220 7468 6520 5647  tings for the VG
+00014dc0: 2070 6c6f 742e 2229 290a 2020 2020 2020   plot.")).      
+00014dd0: 2020 7365 6c66 2e67 726f 7570 426f 785f    self.groupBox_
+00014de0: 7265 7375 6c74 735f 7667 5f70 6c6f 745f  results_vg_plot_
+00014df0: 7365 7474 696e 6773 2e73 6574 5469 746c  settings.setTitl
+00014e00: 6528 5f74 7261 6e73 6c61 7465 2822 4d61  e(_translate("Ma
+00014e10: 696e 5769 6e64 6f77 222c 2022 5647 2070  inWindow", "VG p
+00014e20: 6c6f 7420 7365 7474 696e 6773 2229 290a  lot settings")).
+00014e30: 2020 2020 2020 2020 7365 6c66 2e63 6865          self.che
+00014e40: 636b 426f 785f 7265 7375 6c74 735f 7667  ckBox_results_vg
+00014e50: 5f70 6c6f 745f 7368 6f77 5f72 6573 6964  _plot_show_resid
+00014e60: 7561 6c73 2e73 6574 546f 6f6c 5469 7028  uals.setToolTip(
+00014e70: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
+00014e80: 5769 6e64 6f77 222c 2022 506c 6f74 2074  Window", "Plot t
+00014e90: 6865 2070 6f73 7420 6669 7420 7265 7369  he post fit resi
+00014ea0: 6475 616c 7320 6772 6f75 7065 6420 6279  duals grouped by
+00014eb0: 2074 6865 2073 6574 7570 2068 6569 6768   the setup heigh
+00014ec0: 7420 2873 7461 7469 6f6e 206e 616d 6529  t (station name)
+00014ed0: 2e20 4966 206c 696e 6561 7220 616e 6420  . If linear and 
+00014ee0: 6e6f 2d6c 696e 6561 7220 636f 6d70 6f6e  no-linear compon
+00014ef0: 656e 7473 206f 6620 7468 6520 5647 2070  ents of the VG p
+00014f00: 6f6c 796e 6f6d 6961 6c20 2864 6567 7265  olynomial (degre
+00014f10: 6520 3e20 3129 2061 7265 2070 6c6f 7474  e > 1) are plott
+00014f20: 6564 2073 6570 6172 6174 656c 792c 2074  ed separately, t
+00014f30: 6865 2072 6573 6964 7561 6c73 2077 2e72  he residuals w.r
+00014f40: 2e74 2e20 7468 6520 6c69 6e65 6172 2063  .t. the linear c
+00014f50: 6f6d 706f 6e65 6e74 2065 7374 696d 6174  omponent estimat
+00014f60: 6564 2069 6e20 7468 6520 4c53 4d20 6164  ed in the LSM ad
+00014f70: 6a75 7374 6d65 6e74 2061 7265 2073 686f  justment are sho
+00014f80: 776e 2e22 2929 0a20 2020 2020 2020 2073  wn.")).        s
+00014f90: 656c 662e 6368 6563 6b42 6f78 5f72 6573  elf.checkBox_res
+00014fa0: 756c 7473 5f76 675f 706c 6f74 5f73 686f  ults_vg_plot_sho
+00014fb0: 775f 7265 7369 6475 616c 732e 7365 7454  w_residuals.setT
 00014fc0: 6578 7428 5f74 7261 6e73 6c61 7465 2822  ext(_translate("
-00014fd0: 4d61 696e 5769 6e64 6f77 222c 2022 4164  MainWindow", "Ad
-00014fe0: 6420 5374 6174 696f 6e73 2229 290a 2020  d Stations")).  
-00014ff0: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
-00015000: 6e5f 4578 6974 2e73 6574 5465 7874 285f  n_Exit.setText(_
-00015010: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
-00015020: 696e 646f 7722 2c20 2245 2678 6974 2229  indow", "E&xit")
-00015030: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00015040: 6374 696f 6e5f 4578 6974 2e73 6574 546f  ction_Exit.setTo
-00015050: 6f6c 5469 7028 5f74 7261 6e73 6c61 7465  olTip(_translate
-00015060: 2822 4d61 696e 5769 6e64 6f77 222c 2022  ("MainWindow", "
-00015070: 4578 6974 2047 7261 7654 6f6f 6c73 2229  Exit GravTools")
-00015080: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00015090: 6374 696f 6e5f 4564 6974 5f4f 6273 6572  ction_Edit_Obser
-000150a0: 7661 7469 6f6e 732e 7365 7454 6578 7428  vations.setText(
-000150b0: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
-000150c0: 5769 6e64 6f77 222c 2022 4564 6974 204f  Window", "Edit O
-000150d0: 6273 6572 7661 7469 6f6e 7322 2929 0a20  bservations")). 
-000150e0: 2020 2020 2020 2073 656c 662e 6163 7469         self.acti
-000150f0: 6f6e 5265 7369 6475 616c 732e 7365 7454  onResiduals.setT
-00015100: 6578 7428 5f74 7261 6e73 6c61 7465 2822  ext(_translate("
-00015110: 4d61 696e 5769 6e64 6f77 222c 2022 5265  MainWindow", "Re
-00015120: 7369 6475 616c 7322 2929 0a20 2020 2020  siduals")).     
-00015130: 2020 2073 656c 662e 6163 7469 6f6e 4573     self.actionEs
-00015140: 7469 6d61 7465 732e 7365 7454 6578 7428  timates.setText(
-00015150: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
-00015160: 5769 6e64 6f77 222c 2022 4573 7469 6d61  Window", "Estima
-00015170: 7465 7322 2929 0a20 2020 2020 2020 2073  tes")).        s
-00015180: 656c 662e 6163 7469 6f6e 5f43 6f72 7265  elf.action_Corre
-00015190: 6374 696f 6e73 2e73 6574 5465 7874 285f  ctions.setText(_
-000151a0: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
-000151b0: 696e 646f 7722 2c20 2243 6f72 7265 6374  indow", "Correct
-000151c0: 696f 6e20 7365 7474 696e 6773 2229 290a  ion settings")).
-000151d0: 2020 2020 2020 2020 7365 6c66 2e61 6374          self.act
-000151e0: 696f 6e53 686f 775f 5374 6174 696f 6e73  ionShow_Stations
-000151f0: 2e73 6574 5465 7874 285f 7472 616e 736c  .setText(_transl
-00015200: 6174 6528 224d 6169 6e57 696e 646f 7722  ate("MainWindow"
-00015210: 2c20 2253 686f 7720 5374 6174 696f 6e73  , "Show Stations
-00015220: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
-00015230: 2e61 6374 696f 6e5f 6672 6f6d 5f43 4735  .action_from_CG5
-00015240: 5f6f 6273 6572 7661 7469 6f6e 5f66 696c  _observation_fil
-00015250: 652e 7365 7454 6578 7428 5f74 7261 6e73  e.setText(_trans
-00015260: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
-00015270: 222c 2022 6672 6f6d 2043 4735 206f 6273  ", "from CG5 obs
-00015280: 6572 7661 7469 6f6e 2066 696c 6522 2929  ervation file"))
-00015290: 0a20 2020 2020 2020 2073 656c 662e 6163  .        self.ac
-000152a0: 7469 6f6e 5f66 726f 6d5f 4245 565f 6f62  tion_from_BEV_ob
-000152b0: 7365 7276 6174 696f 6e5f 6669 6c65 2e73  servation_file.s
-000152c0: 6574 5465 7874 285f 7472 616e 736c 6174  etText(_translat
-000152d0: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
-000152e0: 2266 726f 6d20 4245 5620 6f62 7365 7276  "from BEV observ
-000152f0: 6174 696f 6e20 6669 6c65 2229 290a 2020  ation file")).  
-00015300: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
-00015310: 6e5f 4175 746f 7365 6c65 6374 696f 6e5f  n_Autoselection_
-00015320: 7365 7474 696e 6773 2e73 6574 5465 7874  settings.setText
-00015330: 285f 7472 616e 736c 6174 6528 224d 6169  (_translate("Mai
-00015340: 6e57 696e 646f 7722 2c20 2241 7574 6f73  nWindow", "Autos
-00015350: 656c 6563 7469 6f6e 2073 6574 7469 6e67  election setting
-00015360: 7322 2929 0a20 2020 2020 2020 2073 656c  s")).        sel
-00015370: 662e 6163 7469 6f6e 5f45 7374 696d 6174  f.action_Estimat
-00015380: 696f 6e5f 7365 7474 696e 6773 2e73 6574  ion_settings.set
-00015390: 5465 7874 285f 7472 616e 736c 6174 6528  Text(_translate(
-000153a0: 224d 6169 6e57 696e 646f 7722 2c20 2245  "MainWindow", "E
-000153b0: 7374 696d 6174 696f 6e20 7365 7474 696e  stimation settin
-000153c0: 6773 2229 290a 2020 2020 2020 2020 7365  gs")).        se
-000153d0: 6c66 2e61 6374 696f 6e45 7374 696d 6174  lf.actionEstimat
-000153e0: 655f 6c6f 6e67 5f74 6572 6d5f 6472 6966  e_long_term_drif
-000153f0: 742e 7365 7454 6578 7428 5f74 7261 6e73  t.setText(_trans
-00015400: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
-00015410: 222c 2022 4573 7469 6d61 7465 206c 6f6e  ", "Estimate lon
-00015420: 672d 7465 726d 2064 7269 6674 2229 290a  g-term drift")).
-00015430: 2020 2020 2020 2020 7365 6c66 2e61 6374          self.act
-00015440: 696f 6e5f 4578 706f 7274 5f52 6573 756c  ion_Export_Resul
-00015450: 7473 2e73 6574 5465 7874 285f 7472 616e  ts.setText(_tran
-00015460: 736c 6174 6528 224d 6169 6e57 696e 646f  slate("MainWindo
-00015470: 7722 2c20 2245 7870 6f72 7420 4461 7461  w", "Export Data
-00015480: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
-00015490: 2e61 6374 696f 6e5f 4578 706f 7274 5f52  .action_Export_R
-000154a0: 6573 756c 7473 2e73 6574 546f 6f6c 5469  esults.setToolTi
-000154b0: 7028 5f74 7261 6e73 6c61 7465 2822 4d61  p(_translate("Ma
-000154c0: 696e 5769 6e64 6f77 222c 2022 4578 706f  inWindow", "Expo
-000154d0: 7274 2064 6174 6122 2929 0a20 2020 2020  rt data")).     
-000154e0: 2020 2073 656c 662e 6163 7469 6f6e 5f43     self.action_C
-000154f0: 6861 6e67 655f 6f75 7470 7574 5f64 6972  hange_output_dir
-00015500: 6563 746f 7279 2e73 6574 5465 7874 285f  ectory.setText(_
-00015510: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
-00015520: 696e 646f 7722 2c20 2243 6861 6e67 6520  indow", "Change 
-00015530: 6f75 7470 7574 2064 6972 6563 746f 7279  output directory
-00015540: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
-00015550: 2e61 6374 696f 6e5f 4f70 7469 6f6e 732e  .action_Options.
-00015560: 7365 7454 6578 7428 5f74 7261 6e73 6c61  setText(_transla
-00015570: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
-00015580: 2022 4f70 7469 6f6e 7322 2929 0a20 2020   "Options")).   
-00015590: 2020 2020 2073 656c 662e 6163 7469 6f6e       self.action
-000155a0: 5f53 6574 7570 5f64 6174 615f 6f70 7469  _Setup_data_opti
-000155b0: 6f6e 732e 7365 7454 6578 7428 5f74 7261  ons.setText(_tra
-000155c0: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
-000155d0: 6f77 222c 2022 5365 7475 7020 6461 7461  ow", "Setup data
-000155e0: 206f 7074 696f 6e73 2229 290a 2020 2020   options")).    
-000155f0: 2020 2020 7365 6c66 2e61 6374 696f 6e5f      self.action_
-00015600: 466c 6167 5f6f 6273 6572 7661 7469 6f6e  Flag_observation
-00015610: 732e 7365 7454 6578 7428 5f74 7261 6e73  s.setText(_trans
-00015620: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
-00015630: 222c 2022 4c6f 6164 2066 6c61 6773 2066  ", "Load flags f
-00015640: 726f 6d20 6f62 732e 206c 6973 7420 6669  rom obs. list fi
-00015650: 6c65 2229 290a 2020 2020 2020 2020 7365  le")).        se
-00015660: 6c66 2e61 6374 696f 6e5f 466c 6167 5f6f  lf.action_Flag_o
-00015670: 6273 6572 7661 7469 6f6e 732e 7365 7454  bservations.setT
-00015680: 6f6f 6c54 6970 285f 7472 616e 736c 6174  oolTip(_translat
-00015690: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
-000156a0: 2246 6c61 6720 6f62 7365 7276 6174 696f  "Flag observatio
-000156b0: 6e73 2062 6173 6564 206f 6220 6f62 7365  ns based ob obse
-000156c0: 7276 6174 696f 6e73 2066 696c 6522 2929  rvations file"))
-000156d0: 0a20 2020 2020 2020 2073 656c 662e 6163  .        self.ac
-000156e0: 7469 6f6e 5f43 6861 6e67 655f 4361 6d70  tion_Change_Camp
-000156f0: 6169 676e 5f6e 616d 652e 7365 7454 6578  aign_name.setTex
-00015700: 7428 5f74 7261 6e73 6c61 7465 2822 4d61  t(_translate("Ma
-00015710: 696e 5769 6e64 6f77 222c 2022 4368 616e  inWindow", "Chan
-00015720: 6765 2043 616d 7061 6967 6e20 6e61 6d65  ge Campaign name
-00015730: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
-00015740: 2e61 6374 696f 6e5f 4162 6f75 742e 7365  .action_About.se
-00015750: 7454 6578 7428 5f74 7261 6e73 6c61 7465  tText(_translate
-00015760: 2822 4d61 696e 5769 6e64 6f77 222c 2022  ("MainWindow", "
-00015770: 4162 6f75 7422 2929 0a20 2020 2020 2020  About")).       
-00015780: 2073 656c 662e 6163 7469 6f6e 5f4c 6963   self.action_Lic
-00015790: 656e 7365 2e73 6574 5465 7874 285f 7472  ense.setText(_tr
-000157a0: 616e 736c 6174 6528 224d 6169 6e57 696e  anslate("MainWin
-000157b0: 646f 7722 2c20 224c 6963 656e 7365 2229  dow", "License")
-000157c0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-000157d0: 6374 696f 6e5f 4769 735f 4578 706f 7274  ction_Gis_Export
-000157e0: 5f73 6574 7469 6e67 732e 7365 7454 6578  _settings.setTex
-000157f0: 7428 5f74 7261 6e73 6c61 7465 2822 4d61  t(_translate("Ma
-00015800: 696e 5769 6e64 6f77 222c 2022 4749 5320  inWindow", "GIS 
-00015810: 6578 706f 7274 2073 6574 7469 6e67 7322  export settings"
-00015820: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-00015830: 6163 7469 6f6e 5f66 726f 6d5f 6f65 7367  action_from_oesg
-00015840: 6e5f 7461 626c 652e 7365 7454 6578 7428  n_table.setText(
-00015850: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
-00015860: 5769 6e64 6f77 222c 2022 4672 6f6d 204f  Window", "From O
-00015870: 4553 474e 2066 696c 6522 2929 0a20 2020  ESGN file")).   
-00015880: 2020 2020 2073 656c 662e 6163 7469 6f6e       self.action
-00015890: 5f66 726f 6d5f 6373 765f 6669 6c65 2e73  _from_csv_file.s
-000158a0: 6574 5465 7874 285f 7472 616e 736c 6174  etText(_translat
-000158b0: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
-000158c0: 2246 726f 6d20 4353 5620 6669 6c65 2229  "From CSV file")
-000158d0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-000158e0: 6374 696f 6e5f 436f 7272 6563 7469 6f6e  ction_Correction
-000158f0: 5f74 696d 655f 7365 7269 6573 2e73 6574  _time_series.set
-00015900: 5465 7874 285f 7472 616e 736c 6174 6528  Text(_translate(
-00015910: 224d 6169 6e57 696e 646f 7722 2c20 2243  "MainWindow", "C
-00015920: 6f72 7265 6374 696f 6e20 7469 6d65 2073  orrection time s
-00015930: 6572 6965 7322 2929 0a20 2020 2020 2020  eries")).       
-00015940: 2073 656c 662e 6163 7469 6f6e 5f43 6f72   self.action_Cor
-00015950: 7265 6374 696f 6e5f 7469 6d65 5f73 6572  rection_time_ser
-00015960: 6965 732e 7365 7454 6f6f 6c54 6970 285f  ies.setToolTip(_
-00015970: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
-00015980: 696e 646f 7722 2c20 224d 616e 6167 6520  indow", "Manage 
-00015990: 636f 7272 6563 7469 6f6e 2074 696d 6520  correction time 
-000159a0: 7365 7269 6573 2064 6174 6122 2929 0a20  series data")). 
-000159b0: 2020 2020 2020 2073 656c 662e 6163 7469         self.acti
-000159c0: 6f6e 5f67 7261 7669 6d65 7465 7273 5f66  on_gravimeters_f
-000159d0: 726f 6d5f 6a73 6f6e 5f66 696c 652e 7365  rom_json_file.se
-000159e0: 7454 6578 7428 5f74 7261 6e73 6c61 7465  tText(_translate
-000159f0: 2822 4d61 696e 5769 6e64 6f77 222c 2022  ("MainWindow", "
-00015a00: 4672 6f6d 206a 736f 6e20 6669 6c65 2229  From json file")
-00015a10: 290a 6672 6f6d 2070 7971 7467 7261 7068  ).from pyqtgraph
-00015a20: 2069 6d70 6f72 7420 4772 6170 6869 6373   import Graphics
-00015a30: 4c61 796f 7574 5769 6467 6574 0a         LayoutWidget.
+00014fd0: 4d61 696e 5769 6e64 6f77 222c 2022 5368  MainWindow", "Sh
+00014fe0: 6f77 2072 6573 6964 7561 6c73 2229 290a  ow residuals")).
+00014ff0: 2020 2020 2020 2020 7365 6c66 2e72 6164          self.rad
+00015000: 696f 4275 7474 6f6e 5f72 6573 756c 7473  ioButton_results
+00015010: 5f76 675f 706c 6f74 5f64 6574 6169 6c73  _vg_plot_details
+00015020: 2e73 6574 546f 6f6c 5469 7028 5f74 7261  .setToolTip(_tra
+00015030: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
+00015040: 6f77 222c 2022 506c 6f74 2074 6865 206c  ow", "Plot the l
+00015050: 696e 6561 7220 616e 6420 6e6f 6e2d 6c69  inear and non-li
+00015060: 6e65 6172 2063 6f6d 706f 6e65 6e74 7320  near components 
+00015070: 6f66 2074 6865 2065 7374 696d 6174 6573  of the estimates
+00015080: 2056 4720 706f 6c79 6e6f 6d69 616c 2073   VG polynomial s
+00015090: 6570 6172 6174 656c 792e 2022 2929 0a20  eparately. ")). 
+000150a0: 2020 2020 2020 2073 656c 662e 7261 6469         self.radi
+000150b0: 6f42 7574 746f 6e5f 7265 7375 6c74 735f  oButton_results_
+000150c0: 7667 5f70 6c6f 745f 6465 7461 696c 732e  vg_plot_details.
+000150d0: 7365 7454 6578 7428 5f74 7261 6e73 6c61  setText(_transla
+000150e0: 7465 2822 4d61 696e 5769 6e64 6f77 222c  te("MainWindow",
+000150f0: 2022 506c 6f74 206c 696e 6561 7220 616e   "Plot linear an
+00015100: 6420 6e6f 6e2d 6c69 6e65 6172 2063 6f6d  d non-linear com
+00015110: 706f 6e65 6e74 7320 7365 7061 7261 7465  ponents separate
+00015120: 6c79 2229 290a 2020 2020 2020 2020 7365  ly")).        se
+00015130: 6c66 2e72 6164 696f 4275 7474 6f6e 5f72  lf.radioButton_r
+00015140: 6573 756c 7473 5f76 675f 706c 6f74 5f66  esults_vg_plot_f
+00015150: 756c 6c5f 706f 6c79 6e6f 6d69 616c 2e73  ull_polynomial.s
+00015160: 6574 546f 6f6c 5469 7028 5f74 7261 6e73  etToolTip(_trans
+00015170: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
+00015180: 222c 2022 506c 6f74 2074 6865 2066 756c  ", "Plot the ful
+00015190: 6c20 6573 7469 6d61 7465 6420 5647 2070  l estimated VG p
+000151a0: 6f6c 796e 6f6d 6961 6c20 7665 7273 7573  olynomial versus
+000151b0: 2068 6569 6768 7420 6162 6f76 6520 7468   height above th
+000151c0: 6520 7265 6665 7265 6e63 652e 2229 290a  e reference.")).
+000151d0: 2020 2020 2020 2020 7365 6c66 2e72 6164          self.rad
+000151e0: 696f 4275 7474 6f6e 5f72 6573 756c 7473  ioButton_results
+000151f0: 5f76 675f 706c 6f74 5f66 756c 6c5f 706f  _vg_plot_full_po
+00015200: 6c79 6e6f 6d69 616c 2e73 6574 5465 7874  lynomial.setText
+00015210: 285f 7472 616e 736c 6174 6528 224d 6169  (_translate("Mai
+00015220: 6e57 696e 646f 7722 2c20 2250 6c6f 7420  nWindow", "Plot 
+00015230: 6675 6c6c 2070 6f6c 796e 6f6d 6961 6c22  full polynomial"
+00015240: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+00015250: 7461 6257 6964 6765 745f 7265 7375 6c74  tabWidget_result
+00015260: 732e 7365 7454 6162 5465 7874 2873 656c  s.setTabText(sel
+00015270: 662e 7461 6257 6964 6765 745f 7265 7375  f.tabWidget_resu
+00015280: 6c74 732e 696e 6465 784f 6628 7365 6c66  lts.indexOf(self
+00015290: 2e74 6162 5f76 675f 706c 6f74 292c 205f  .tab_vg_plot), _
+000152a0: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
+000152b0: 696e 646f 7722 2c20 2256 4720 506c 6f74  indow", "VG Plot
+000152c0: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+000152d0: 2e74 6162 5769 6467 6574 5f4d 6169 6e2e  .tabWidget_Main.
+000152e0: 7365 7454 6162 5465 7874 2873 656c 662e  setTabText(self.
+000152f0: 7461 6257 6964 6765 745f 4d61 696e 2e69  tabWidget_Main.i
+00015300: 6e64 6578 4f66 2873 656c 662e 7461 625f  ndexOf(self.tab_
+00015310: 6d61 696e 5f72 6573 756c 7473 292c 205f  main_results), _
+00015320: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
+00015330: 696e 646f 7722 2c20 2252 6573 756c 7473  indow", "Results
+00015340: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+00015350: 2e74 6162 5769 6467 6574 5f4d 6169 6e2e  .tabWidget_Main.
+00015360: 7365 7454 6162 546f 6f6c 5469 7028 7365  setTabToolTip(se
+00015370: 6c66 2e74 6162 5769 6467 6574 5f4d 6169  lf.tabWidget_Mai
+00015380: 6e2e 696e 6465 784f 6628 7365 6c66 2e74  n.indexOf(self.t
+00015390: 6162 5f6d 6169 6e5f 7265 7375 6c74 7329  ab_main_results)
+000153a0: 2c20 5f74 7261 6e73 6c61 7465 2822 4d61  , _translate("Ma
+000153b0: 696e 5769 6e64 6f77 222c 2022 5365 7475  inWindow", "Setu
+000153c0: 7020 6461 7461 3a20 436f 7272 6563 7465  p data: Correcte
+000153d0: 6420 616e 6420 7265 6475 6365 7320 6f62  d and reduces ob
+000153e0: 7365 7276 6174 696f 6e20 6461 7461 2061  servation data a
+000153f0: 6363 756d 756c 6174 6564 2066 6f72 2065  ccumulated for e
+00015400: 6163 6820 696e 7374 7275 6d65 6e74 2073  ach instrument s
+00015410: 6574 7570 2e22 2929 0a20 2020 2020 2020  etup.")).       
+00015420: 2073 656c 662e 6d65 6e75 5f46 696c 652e   self.menu_File.
+00015430: 7365 7454 6974 6c65 285f 7472 616e 736c  setTitle(_transl
+00015440: 6174 6528 224d 6169 6e57 696e 646f 7722  ate("MainWindow"
+00015450: 2c20 2246 696c 6522 2929 0a20 2020 2020  , "File")).     
+00015460: 2020 2073 656c 662e 6d65 6e75 4164 645f     self.menuAdd_
+00015470: 5375 7276 6579 2e73 6574 5469 746c 6528  Survey.setTitle(
+00015480: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
+00015490: 5769 6e64 6f77 222c 2022 4164 6420 5375  Window", "Add Su
+000154a0: 7276 6579 2229 290a 2020 2020 2020 2020  rvey")).        
+000154b0: 7365 6c66 2e6d 656e 755f 4164 645f 5374  self.menu_Add_St
+000154c0: 6174 696f 6e73 2e73 6574 5469 746c 6528  ations.setTitle(
+000154d0: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
+000154e0: 5769 6e64 6f77 222c 2022 4164 6420 5374  Window", "Add St
+000154f0: 6174 696f 6e73 2229 290a 2020 2020 2020  ations")).      
+00015500: 2020 7365 6c66 2e6d 656e 755f 4164 645f    self.menu_Add_
+00015510: 4772 6176 696d 6574 6572 732e 7365 7454  Gravimeters.setT
+00015520: 6974 6c65 285f 7472 616e 736c 6174 6528  itle(_translate(
+00015530: 224d 6169 6e57 696e 646f 7722 2c20 2241  "MainWindow", "A
+00015540: 6464 2047 7261 7669 6d65 7465 7273 2229  dd Gravimeters")
+00015550: 290a 2020 2020 2020 2020 7365 6c66 2e6d  ).        self.m
+00015560: 656e 755f 4f62 7365 7276 6174 696f 6e73  enu_Observations
+00015570: 2e73 6574 5469 746c 6528 5f74 7261 6e73  .setTitle(_trans
+00015580: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
+00015590: 222c 2022 4f62 7365 7276 6174 696f 6e73  ", "Observations
+000155a0: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+000155b0: 2e6d 656e 7545 7374 696d 6174 696f 6e5f  .menuEstimation_
+000155c0: 7365 7474 696e 6773 2e73 6574 5469 746c  settings.setTitl
+000155d0: 6528 5f74 7261 6e73 6c61 7465 2822 4d61  e(_translate("Ma
+000155e0: 696e 5769 6e64 6f77 222c 2022 5365 7474  inWindow", "Sett
+000155f0: 696e 6773 2229 290a 2020 2020 2020 2020  ings")).        
+00015600: 7365 6c66 2e6d 656e 7548 656c 702e 7365  self.menuHelp.se
+00015610: 7454 6974 6c65 285f 7472 616e 736c 6174  tTitle(_translat
+00015620: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
+00015630: 2248 656c 7022 2929 0a20 2020 2020 2020  "Help")).       
+00015640: 2073 656c 662e 6d65 6e75 436f 7272 6563   self.menuCorrec
+00015650: 7469 6f6e 732e 7365 7454 6974 6c65 285f  tions.setTitle(_
+00015660: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
+00015670: 696e 646f 7722 2c20 2243 6f72 7265 6374  indow", "Correct
+00015680: 696f 6e73 2229 290a 2020 2020 2020 2020  ions")).        
+00015690: 7365 6c66 2e61 6374 696f 6e5f 4e65 775f  self.action_New_
+000156a0: 4361 6d70 6169 676e 2e73 6574 5465 7874  Campaign.setText
+000156b0: 285f 7472 616e 736c 6174 6528 224d 6169  (_translate("Mai
+000156c0: 6e57 696e 646f 7722 2c20 2226 4e65 7720  nWindow", "&New 
+000156d0: 4361 6d70 6169 676e 2229 290a 2020 2020  Campaign")).    
+000156e0: 2020 2020 7365 6c66 2e61 6374 696f 6e5f      self.action_
+000156f0: 5361 7665 5f43 616d 7061 6967 6e2e 7365  Save_Campaign.se
+00015700: 7454 6578 7428 5f74 7261 6e73 6c61 7465  tText(_translate
+00015710: 2822 4d61 696e 5769 6e64 6f77 222c 2022  ("MainWindow", "
+00015720: 2653 6176 6520 4361 6d70 6169 676e 2229  &Save Campaign")
+00015730: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+00015740: 6374 696f 6e5f 4c6f 6164 5f43 616d 7061  ction_Load_Campa
+00015750: 6967 6e2e 7365 7454 6578 7428 5f74 7261  ign.setText(_tra
+00015760: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
+00015770: 6f77 222c 2022 264c 6f61 6420 4361 6d70  ow", "&Load Camp
+00015780: 6169 676e 2229 290a 2020 2020 2020 2020  aign")).        
+00015790: 7365 6c66 2e61 6374 696f 6e5f 4c6f 6164  self.action_Load
+000157a0: 5f43 616d 7061 6967 6e2e 7365 7454 6f6f  _Campaign.setToo
+000157b0: 6c54 6970 285f 7472 616e 736c 6174 6528  lTip(_translate(
+000157c0: 224d 6169 6e57 696e 646f 7722 2c20 224c  "MainWindow", "L
+000157d0: 6f61 6420 6361 6d70 6169 676e 2229 290a  oad campaign")).
+000157e0: 2020 2020 2020 2020 7365 6c66 2e61 6374          self.act
+000157f0: 696f 6e5f 4164 645f 5374 6174 696f 6e73  ion_Add_Stations
+00015800: 2e73 6574 5465 7874 285f 7472 616e 736c  .setText(_transl
+00015810: 6174 6528 224d 6169 6e57 696e 646f 7722  ate("MainWindow"
+00015820: 2c20 2241 6464 2053 7461 7469 6f6e 7322  , "Add Stations"
+00015830: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+00015840: 6163 7469 6f6e 5f45 7869 742e 7365 7454  action_Exit.setT
+00015850: 6578 7428 5f74 7261 6e73 6c61 7465 2822  ext(_translate("
+00015860: 4d61 696e 5769 6e64 6f77 222c 2022 4526  MainWindow", "E&
+00015870: 7869 7422 2929 0a20 2020 2020 2020 2073  xit")).        s
+00015880: 656c 662e 6163 7469 6f6e 5f45 7869 742e  elf.action_Exit.
+00015890: 7365 7454 6f6f 6c54 6970 285f 7472 616e  setToolTip(_tran
+000158a0: 736c 6174 6528 224d 6169 6e57 696e 646f  slate("MainWindo
+000158b0: 7722 2c20 2245 7869 7420 4772 6176 546f  w", "Exit GravTo
+000158c0: 6f6c 7322 2929 0a20 2020 2020 2020 2073  ols")).        s
+000158d0: 656c 662e 6163 7469 6f6e 5f45 6469 745f  elf.action_Edit_
+000158e0: 4f62 7365 7276 6174 696f 6e73 2e73 6574  Observations.set
+000158f0: 5465 7874 285f 7472 616e 736c 6174 6528  Text(_translate(
+00015900: 224d 6169 6e57 696e 646f 7722 2c20 2245  "MainWindow", "E
+00015910: 6469 7420 4f62 7365 7276 6174 696f 6e73  dit Observations
+00015920: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+00015930: 2e61 6374 696f 6e52 6573 6964 7561 6c73  .actionResiduals
+00015940: 2e73 6574 5465 7874 285f 7472 616e 736c  .setText(_transl
+00015950: 6174 6528 224d 6169 6e57 696e 646f 7722  ate("MainWindow"
+00015960: 2c20 2252 6573 6964 7561 6c73 2229 290a  , "Residuals")).
+00015970: 2020 2020 2020 2020 7365 6c66 2e61 6374          self.act
+00015980: 696f 6e45 7374 696d 6174 6573 2e73 6574  ionEstimates.set
+00015990: 5465 7874 285f 7472 616e 736c 6174 6528  Text(_translate(
+000159a0: 224d 6169 6e57 696e 646f 7722 2c20 2245  "MainWindow", "E
+000159b0: 7374 696d 6174 6573 2229 290a 2020 2020  stimates")).    
+000159c0: 2020 2020 7365 6c66 2e61 6374 696f 6e5f      self.action_
+000159d0: 436f 7272 6563 7469 6f6e 732e 7365 7454  Corrections.setT
+000159e0: 6578 7428 5f74 7261 6e73 6c61 7465 2822  ext(_translate("
+000159f0: 4d61 696e 5769 6e64 6f77 222c 2022 436f  MainWindow", "Co
+00015a00: 7272 6563 7469 6f6e 2073 6574 7469 6e67  rrection setting
+00015a10: 7322 2929 0a20 2020 2020 2020 2073 656c  s")).        sel
+00015a20: 662e 6163 7469 6f6e 5368 6f77 5f53 7461  f.actionShow_Sta
+00015a30: 7469 6f6e 732e 7365 7454 6578 7428 5f74  tions.setText(_t
+00015a40: 7261 6e73 6c61 7465 2822 4d61 696e 5769  ranslate("MainWi
+00015a50: 6e64 6f77 222c 2022 5368 6f77 2053 7461  ndow", "Show Sta
+00015a60: 7469 6f6e 7322 2929 0a20 2020 2020 2020  tions")).       
+00015a70: 2073 656c 662e 6163 7469 6f6e 5f66 726f   self.action_fro
+00015a80: 6d5f 4347 355f 6f62 7365 7276 6174 696f  m_CG5_observatio
+00015a90: 6e5f 6669 6c65 2e73 6574 5465 7874 285f  n_file.setText(_
+00015aa0: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
+00015ab0: 696e 646f 7722 2c20 2266 726f 6d20 4347  indow", "from CG
+00015ac0: 3520 6f62 7365 7276 6174 696f 6e20 6669  5 observation fi
+00015ad0: 6c65 2229 290a 2020 2020 2020 2020 7365  le")).        se
+00015ae0: 6c66 2e61 6374 696f 6e5f 6672 6f6d 5f42  lf.action_from_B
+00015af0: 4556 5f6f 6273 6572 7661 7469 6f6e 5f66  EV_observation_f
+00015b00: 696c 652e 7365 7454 6578 7428 5f74 7261  ile.setText(_tra
+00015b10: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
+00015b20: 6f77 222c 2022 6672 6f6d 2042 4556 206f  ow", "from BEV o
+00015b30: 6273 6572 7661 7469 6f6e 2066 696c 6522  bservation file"
+00015b40: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+00015b50: 6163 7469 6f6e 5f41 7574 6f73 656c 6563  action_Autoselec
+00015b60: 7469 6f6e 5f73 6574 7469 6e67 732e 7365  tion_settings.se
+00015b70: 7454 6578 7428 5f74 7261 6e73 6c61 7465  tText(_translate
+00015b80: 2822 4d61 696e 5769 6e64 6f77 222c 2022  ("MainWindow", "
+00015b90: 4175 746f 7365 6c65 6374 696f 6e20 7365  Autoselection se
+00015ba0: 7474 696e 6773 2229 290a 2020 2020 2020  ttings")).      
+00015bb0: 2020 7365 6c66 2e61 6374 696f 6e5f 4573    self.action_Es
+00015bc0: 7469 6d61 7469 6f6e 5f73 6574 7469 6e67  timation_setting
+00015bd0: 732e 7365 7454 6578 7428 5f74 7261 6e73  s.setText(_trans
+00015be0: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
+00015bf0: 222c 2022 4573 7469 6d61 7469 6f6e 2073  ", "Estimation s
+00015c00: 6574 7469 6e67 7322 2929 0a20 2020 2020  ettings")).     
+00015c10: 2020 2073 656c 662e 6163 7469 6f6e 4573     self.actionEs
+00015c20: 7469 6d61 7465 5f6c 6f6e 675f 7465 726d  timate_long_term
+00015c30: 5f64 7269 6674 2e73 6574 5465 7874 285f  _drift.setText(_
+00015c40: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
+00015c50: 696e 646f 7722 2c20 2245 7374 696d 6174  indow", "Estimat
+00015c60: 6520 6c6f 6e67 2d74 6572 6d20 6472 6966  e long-term drif
+00015c70: 7422 2929 0a20 2020 2020 2020 2073 656c  t")).        sel
+00015c80: 662e 6163 7469 6f6e 5f45 7870 6f72 745f  f.action_Export_
+00015c90: 5265 7375 6c74 732e 7365 7454 6578 7428  Results.setText(
+00015ca0: 5f74 7261 6e73 6c61 7465 2822 4d61 696e  _translate("Main
+00015cb0: 5769 6e64 6f77 222c 2022 4578 706f 7274  Window", "Export
+00015cc0: 2044 6174 6122 2929 0a20 2020 2020 2020   Data")).       
+00015cd0: 2073 656c 662e 6163 7469 6f6e 5f45 7870   self.action_Exp
+00015ce0: 6f72 745f 5265 7375 6c74 732e 7365 7454  ort_Results.setT
+00015cf0: 6f6f 6c54 6970 285f 7472 616e 736c 6174  oolTip(_translat
+00015d00: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
+00015d10: 2245 7870 6f72 7420 6461 7461 2229 290a  "Export data")).
+00015d20: 2020 2020 2020 2020 7365 6c66 2e61 6374          self.act
+00015d30: 696f 6e5f 4368 616e 6765 5f6f 7574 7075  ion_Change_outpu
+00015d40: 745f 6469 7265 6374 6f72 792e 7365 7454  t_directory.setT
+00015d50: 6578 7428 5f74 7261 6e73 6c61 7465 2822  ext(_translate("
+00015d60: 4d61 696e 5769 6e64 6f77 222c 2022 4368  MainWindow", "Ch
+00015d70: 616e 6765 206f 7574 7075 7420 6469 7265  ange output dire
+00015d80: 6374 6f72 7922 2929 0a20 2020 2020 2020  ctory")).       
+00015d90: 2073 656c 662e 6163 7469 6f6e 5f4f 7074   self.action_Opt
+00015da0: 696f 6e73 2e73 6574 5465 7874 285f 7472  ions.setText(_tr
+00015db0: 616e 736c 6174 6528 224d 6169 6e57 696e  anslate("MainWin
+00015dc0: 646f 7722 2c20 224f 7074 696f 6e73 2229  dow", "Options")
+00015dd0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+00015de0: 6374 696f 6e5f 5365 7475 705f 6461 7461  ction_Setup_data
+00015df0: 5f6f 7074 696f 6e73 2e73 6574 5465 7874  _options.setText
+00015e00: 285f 7472 616e 736c 6174 6528 224d 6169  (_translate("Mai
+00015e10: 6e57 696e 646f 7722 2c20 2253 6574 7570  nWindow", "Setup
+00015e20: 2064 6174 6120 6f70 7469 6f6e 7322 2929   data options"))
+00015e30: 0a20 2020 2020 2020 2073 656c 662e 6163  .        self.ac
+00015e40: 7469 6f6e 5f46 6c61 675f 6f62 7365 7276  tion_Flag_observ
+00015e50: 6174 696f 6e73 2e73 6574 5465 7874 285f  ations.setText(_
+00015e60: 7472 616e 736c 6174 6528 224d 6169 6e57  translate("MainW
+00015e70: 696e 646f 7722 2c20 224c 6f61 6420 666c  indow", "Load fl
+00015e80: 6167 7320 6672 6f6d 206f 6273 2e20 6c69  ags from obs. li
+00015e90: 7374 2066 696c 6522 2929 0a20 2020 2020  st file")).     
+00015ea0: 2020 2073 656c 662e 6163 7469 6f6e 5f46     self.action_F
+00015eb0: 6c61 675f 6f62 7365 7276 6174 696f 6e73  lag_observations
+00015ec0: 2e73 6574 546f 6f6c 5469 7028 5f74 7261  .setToolTip(_tra
+00015ed0: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
+00015ee0: 6f77 222c 2022 466c 6167 206f 6273 6572  ow", "Flag obser
+00015ef0: 7661 7469 6f6e 7320 6261 7365 6420 6f62  vations based ob
+00015f00: 206f 6273 6572 7661 7469 6f6e 7320 6669   observations fi
+00015f10: 6c65 2229 290a 2020 2020 2020 2020 7365  le")).        se
+00015f20: 6c66 2e61 6374 696f 6e5f 4368 616e 6765  lf.action_Change
+00015f30: 5f43 616d 7061 6967 6e5f 6e61 6d65 2e73  _Campaign_name.s
+00015f40: 6574 5465 7874 285f 7472 616e 736c 6174  etText(_translat
+00015f50: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
+00015f60: 2243 6861 6e67 6520 4361 6d70 6169 676e  "Change Campaign
+00015f70: 206e 616d 6522 2929 0a20 2020 2020 2020   name")).       
+00015f80: 2073 656c 662e 6163 7469 6f6e 5f41 626f   self.action_Abo
+00015f90: 7574 2e73 6574 5465 7874 285f 7472 616e  ut.setText(_tran
+00015fa0: 736c 6174 6528 224d 6169 6e57 696e 646f  slate("MainWindo
+00015fb0: 7722 2c20 2241 626f 7574 2229 290a 2020  w", "About")).  
+00015fc0: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
+00015fd0: 6e5f 4c69 6365 6e73 652e 7365 7454 6578  n_License.setTex
+00015fe0: 7428 5f74 7261 6e73 6c61 7465 2822 4d61  t(_translate("Ma
+00015ff0: 696e 5769 6e64 6f77 222c 2022 4c69 6365  inWindow", "Lice
+00016000: 6e73 6522 2929 0a20 2020 2020 2020 2073  nse")).        s
+00016010: 656c 662e 6163 7469 6f6e 5f47 6973 5f45  elf.action_Gis_E
+00016020: 7870 6f72 745f 7365 7474 696e 6773 2e73  xport_settings.s
+00016030: 6574 5465 7874 285f 7472 616e 736c 6174  etText(_translat
+00016040: 6528 224d 6169 6e57 696e 646f 7722 2c20  e("MainWindow", 
+00016050: 2247 4953 2065 7870 6f72 7420 7365 7474  "GIS export sett
+00016060: 696e 6773 2229 290a 2020 2020 2020 2020  ings")).        
+00016070: 7365 6c66 2e61 6374 696f 6e5f 6672 6f6d  self.action_from
+00016080: 5f6f 6573 676e 5f74 6162 6c65 2e73 6574  _oesgn_table.set
+00016090: 5465 7874 285f 7472 616e 736c 6174 6528  Text(_translate(
+000160a0: 224d 6169 6e57 696e 646f 7722 2c20 2246  "MainWindow", "F
+000160b0: 726f 6d20 4f45 5347 4e20 6669 6c65 2229  rom OESGN file")
+000160c0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+000160d0: 6374 696f 6e5f 6672 6f6d 5f63 7376 5f66  ction_from_csv_f
+000160e0: 696c 652e 7365 7454 6578 7428 5f74 7261  ile.setText(_tra
+000160f0: 6e73 6c61 7465 2822 4d61 696e 5769 6e64  nslate("MainWind
+00016100: 6f77 222c 2022 4672 6f6d 2043 5356 2066  ow", "From CSV f
+00016110: 696c 6522 2929 0a20 2020 2020 2020 2073  ile")).        s
+00016120: 656c 662e 6163 7469 6f6e 5f43 6f72 7265  elf.action_Corre
+00016130: 6374 696f 6e5f 7469 6d65 5f73 6572 6965  ction_time_serie
+00016140: 732e 7365 7454 6578 7428 5f74 7261 6e73  s.setText(_trans
+00016150: 6c61 7465 2822 4d61 696e 5769 6e64 6f77  late("MainWindow
+00016160: 222c 2022 436f 7272 6563 7469 6f6e 2074  ", "Correction t
+00016170: 696d 6520 7365 7269 6573 2229 290a 2020  ime series")).  
+00016180: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
+00016190: 6e5f 436f 7272 6563 7469 6f6e 5f74 696d  n_Correction_tim
+000161a0: 655f 7365 7269 6573 2e73 6574 546f 6f6c  e_series.setTool
+000161b0: 5469 7028 5f74 7261 6e73 6c61 7465 2822  Tip(_translate("
+000161c0: 4d61 696e 5769 6e64 6f77 222c 2022 4d61  MainWindow", "Ma
+000161d0: 6e61 6765 2063 6f72 7265 6374 696f 6e20  nage correction 
+000161e0: 7469 6d65 2073 6572 6965 7320 6461 7461  time series data
+000161f0: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+00016200: 2e61 6374 696f 6e5f 6772 6176 696d 6574  .action_gravimet
+00016210: 6572 735f 6672 6f6d 5f6a 736f 6e5f 6669  ers_from_json_fi
+00016220: 6c65 2e73 6574 5465 7874 285f 7472 616e  le.setText(_tran
+00016230: 736c 6174 6528 224d 6169 6e57 696e 646f  slate("MainWindo
+00016240: 7722 2c20 2246 726f 6d20 6a73 6f6e 2066  w", "From json f
+00016250: 696c 6522 2929 0a66 726f 6d20 7079 7174  ile")).from pyqt
+00016260: 6772 6170 6820 696d 706f 7274 2047 7261  graph import Gra
+00016270: 7068 6963 734c 6179 6f75 7457 6964 6765  phicsLayoutWidge
+00016280: 740a                                     t.
```

### Comparing `grav-toolbox-0.2.7/gravtools/gui/__init__.py` & `grav_toolbox-0.2.8/gravtools/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/gui/cumstom_widgets.py` & `grav_toolbox-0.2.8/gravtools/gui/cumstom_widgets.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/gui/dialog_about.py` & `grav_toolbox-0.2.8/gravtools/gui/dialog_about.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/gui/dialog_autoselection_settings.py` & `grav_toolbox-0.2.8/gravtools/gui/dialog_autoselection_settings.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/gui/dialog_correction_time_series.py` & `grav_toolbox-0.2.8/gravtools/gui/dialog_correction_time_series.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/gui/dialog_corrections.py` & `grav_toolbox-0.2.8/gravtools/gui/dialog_corrections.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/gui/dialog_estimation_settings.py` & `grav_toolbox-0.2.8/gravtools/gui/dialog_estimation_settings.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/gui/dialog_export_results.py` & `grav_toolbox-0.2.8/gravtools/gui/dialog_export_results.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/gui/dialog_gis_export_settings.py` & `grav_toolbox-0.2.8/gravtools/gui/dialog_gis_export_settings.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/gui/dialog_load_stations.py` & `grav_toolbox-0.2.8/gravtools/gui/dialog_load_stations.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/gui/dialog_load_tsf_file.py` & `grav_toolbox-0.2.8/gravtools/gui/dialog_load_tsf_file.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/gui/dialog_new_campaign.py` & `grav_toolbox-0.2.8/gravtools/gui/dialog_new_campaign.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/gui/dialog_options.py` & `grav_toolbox-0.2.8/gravtools/gui/dialog_options.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/gui/dialog_setup_data.py` & `grav_toolbox-0.2.8/gravtools/gui/dialog_setup_data.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/gui/dlg_correction_time_series.py` & `grav_toolbox-0.2.8/gravtools/gui/dlg_correction_time_series.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/gui/dlg_corrections.py` & `grav_toolbox-0.2.8/gravtools/gui/dlg_corrections.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/gui/dlg_load_tsf_file.py` & `grav_toolbox-0.2.8/gravtools/gui/dlg_load_tsf_file.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/gui/gui_main.py` & `grav_toolbox-0.2.8/gravtools/gui/gui_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,14 +128,15 @@
         self.action_Export_Results.triggered.connect(self.on_menu_file_export_results)
         self.action_Options.triggered.connect(self.on_menu_file_options)
         self.action_About.triggered.connect(self.on_menu_help_about)
         self.pushButton_obs_apply_autoselect_current_data.pressed.connect(self.on_apply_autoselection)
         self.pushButton_obs_comp_setup_data.pressed.connect(self.on_pushbutton_obs_comp_setup_data)
         self.pushButton_obs_run_estimation.pressed.connect(self.on_pushbutton_obs_run_estimation)
         self.pushButton_results_delete_lsm_run.pressed.connect(self.on_pushbutton_results_delete_lsm_run)
+        self.pushButton_results_delete_all_lsm_runs.pressed.connect(self.on_pushbutton_results_delete_all_lsm_runs)
         self.pushButton_results_export_shapefile.pressed.connect(self.on_pushButton_results_export_shapefile)
         self.action_from_CG5_observation_file.triggered.connect(self.on_menu_file_load_survey_from_cg5_observation_file)
         self.action_from_oesgn_table.triggered.connect(self.on_menu_file_load_stations_from_oesgn_table)
         self.action_from_csv_file.triggered.connect(self.on_menu_file_load_stations_from_csv_file)
         self.action_gravimeters_from_json_file.triggered.connect(self.on_menu_file_load_gravimeters_from_json_file)
         self.action_Correction_time_series.triggered.connect(self.action_correction_time_series_triggered)
         self.lineEdit_filter_stat_name.textChanged.connect(self.on_lineEdit_filter_stat_name_textChanged)
@@ -171,14 +172,16 @@
         self.comboBox_results_obs_plot_hist_method.currentIndexChanged.connect(
             self.on_histogram_bin_method_currentIndexChanged)
         self.spinBox_results_obs_plot_number_bins.valueChanged.connect(self.update_results_obs_plots)
         self.comboBox_results_stations_statistics_select_col.currentIndexChanged.connect(
             self.display_station_results_statistics)
         self.tableView_surveys.customContextMenuRequested.connect(self.tableView_surveys_right_click)
         self.treeWidget_gravimeters.itemSelectionChanged.connect(self.gravimeters_tree_widget_item_selection_changed)
+        self.pushButton_surveys_disable_all.pressed.connect(self.pushbutton_surveys_disable_all_pressed)
+        self.pushButton_surveys_enable_all.pressed.connect(self.pushbutton_surveys_enable_all_pressed)
 
         # Set up GUI items and widgets:
         self.set_up_survey_tree_widget()
         self.set_up_observation_plots_widget()
         self.set_up_observation_results_plots_widget()
         self.set_up_observation_results_plots_hist_method_comboBox()
         self.set_up_drift_plot_widget()
@@ -239,14 +242,28 @@
 
         # Set fonts:
         self.plainTextEdit_results_log.setFont(self.system_default_fixed_width_font)  # Monospace font
 
         # Inits misc:
         self.station_colors_dict_results = {}  # set in self.update_results_tab()
 
+    def pushbutton_surveys_enable_all_pressed(self):
+        """Invoked when pressing the button"""
+        if self.campaign is not None:
+            changed_surveys = self.campaign.activate_all_surveys(verbose=IS_VERBOSE)
+            for survey_name in changed_surveys:
+                self.survey_model.emit_data_changed_survey(survey_name=survey_name)
+
+    def pushbutton_surveys_disable_all_pressed(self):
+        """Invoked when pressing the button"""
+        if self.campaign is not None:
+            changed_surveys = self.campaign.deactivate_all_surveys(verbose=IS_VERBOSE)
+            for survey_name in changed_surveys:
+                self.survey_model.emit_data_changed_survey(survey_name=survey_name)
+
     def populate_gravimeters_tree_widget(self):
         """Populate the gravimeters tree widget."""
         # Delete existing items:
         self.treeWidget_gravimeters.blockSignals(True)
         self.delete_all_items_from_gravimeters_tree_widget()
 
         # Add new items:
@@ -387,21 +404,14 @@
                                     self.treeWidget_observations.topLevelItem(tree_item_idx).childCount()):
                                 if self.treeWidget_observations.topLevelItem(tree_item_idx).child(child_item_idx).text(
                                         0) == selected_setup_id:
                                     self.treeWidget_observations.topLevelItem(tree_item_idx).child(
                                         child_item_idx).setSelected()
             self.enable_menu_observations_based_on_campaign_data()
             self.set_up_survey_view_model()
-
-            # TODO: Handle results!
-            # Problem: Wenn man einen Survey entfernt, so kommt es zu Fehlermeldungen, wenn man bestehende Ergebnisse
-            # dieses Surveys im Results tab anzeigen möchte! Offenbar wird hierbei auf campaing.surveys zugegriffen.
-            # Das muss geändert werden, so dass sämtliche Daten, die zur Visualisierung der Ergebnisse nötig sind,
-            # im LSM object gespeichert werden und dort zur Verfügung stehen.
-
             self.statusBar().showMessage(
                 f'Survey "{survey_name}" removed from campaign.')
 
     def action_correction_time_series_triggered(self):
         """Launch dialog for managing correction time series data."""
         _ = self.dlg_correction_time_series.exec()
 
@@ -1627,15 +1637,15 @@
             self.spinBox_results_obs_plot_number_bins.setEnabled(False)
 
     def plot_observation_results(self, results_obs_df=None, column_name='', type='timeseries'):
         """Plots observation data to the GraphicsLayoutWidget.
 
         Notes
         -----
-        If input parameters `` or/and `` is/are `None` or '', the plot content is deleted and the plot is reseted.
+        If input parameters `` or/and `` is/are `None` or '', the plot content is deleted and the plot is reset.
         """
         # Clear plot in any case:
         self.plot_obs_results.clear()
         # Plot time series:
         if self.radioButton_results_obs_plot_timeseries.isChecked():
             self.init_observation_results_plots_timeseries()
             if results_obs_df is not None:  # Data available for plotting
@@ -1660,14 +1670,29 @@
                 # Get bin method:
                 bins = self.get_hist_bin_method()
                 # Get data:
                 data = results_obs_df[column_name].values
                 if isinstance(data, object):
                     data = data.astype(float)
                 y, x = np.histogram(data, bins=bins)
+                if bins in ['fd', 'auto']:
+                    # This check is required, because the fd binning method creates too many bins in some cases. This
+                    # happens whenever the data contains many values that are nearly identical, e.g. when adjusting
+                    # surveys with low redundancy and many residuals that are (close to) zero. This issue is
+                    # documented here: https://github.com/numpy/numpy/issues/11879
+                    if len(x) > settings.HIST_MAX_BIN_NUM:
+                        QMessageBox.warning(self, 'Warning!', f'More the binning method ({bins}) is '
+                                                              f'creating {len(x)} bins. Whenever more than '
+                                                              f'{settings.HIST_MAX_BIN_NUM:} bins are created the '
+                                                              f'backup binning method '
+                                                              f'({settings.HIST_BACKUP_BIN_METHOD}) is used instead.')
+                        bins = settings.HIST_BACKUP_BIN_METHOD
+                        y, x = np.histogram(data, bins=bins)
+                        self.comboBox_results_obs_plot_hist_method.setCurrentText(settings.HIST_BACKUP_BIN_METHOD)
+
                 self.plot_obs_results.plot(x, y, stepMode=True, fillLevel=0, brush=(0, 0, 255, 80))
                 self.plot_obs_results.showGrid(x=True, y=True)
 
                 # Add legend with statistics:
                 mean = np.mean(data)
                 median = np.median(data)
                 std = np.std(data)
@@ -2091,14 +2116,16 @@
                     self.comboBox_results_lsm_run_selection.setCurrentText(current_time_str)
                 except:
                     self.comboBox_results_lsm_run_selection.setCurrentIndex(0)  # 'All stations'
         self.comboBox_results_lsm_run_selection.blockSignals(False)
 
     def on_pushbutton_results_delete_lsm_run(self):
         """Delete the lsm object with index `idx` in the campaign."""
+        if self.campaign is None:
+            return
         idx, time_str = self.get_selected_lsm_run()
         if idx == -1:  # combo box is empty => No lsm run available!
             QMessageBox.warning(self, 'Warning!', 'No LSM adjustment run to be deleted!')
         else:
             time_str = self.campaign.lsm_runs[idx].init_time.strftime("%Y-%m-%d, %H:%M:%S")
             comment_str = self.campaign.lsm_runs[idx].comment
             msg_text = f'Date and time: {time_str}\nComment: {comment_str}'
@@ -2114,14 +2141,39 @@
                     self.statusBar().showMessage(f'LSM run "{time_str}" not deleted.')
                 else:
                     self.statusBar().showMessage(f'LSM run "{time_str}" deleted.')
                     self.update_results_tab()
             else:
                 pass
 
+    def on_pushbutton_results_delete_all_lsm_runs(self):
+        """Delete all LSM runs in the campaign."""
+        if self.campaign is None:
+            return
+        number_of_lsm_runs = self.campaign.number_of_lsm_runs
+        if number_of_lsm_runs == 0:
+            self.statusBar().showMessage(f'No LSM runs available to delete.')
+            return
+        msg_text = f'Do you really want to delete all {number_of_lsm_runs} LSM runs?'
+        reply = QMessageBox.question(self,
+                                     'Delete all LSM runs?',
+                                     msg_text,
+                                     QMessageBox.Yes | QMessageBox.No, QMessageBox.No)
+        if reply == QMessageBox.Yes:
+            try:
+                self.campaign.delete_all_lsm_runs()
+            except Exception as e:
+                QMessageBox.critical(self, 'Error!', str(e))
+                self.statusBar().showMessage(f'No LSM runs deleted.')
+            else:
+                self.statusBar().showMessage(f'{number_of_lsm_runs} LSM runs deleted.')
+                self.update_results_tab()
+        else:
+            self.statusBar().showMessage(f'No LSM runs deleted.')
+
     def get_selected_lsm_run(self):
         """Get the selected lsm run in the results tab."""
         time_str = self.comboBox_results_lsm_run_selection.currentText()
         idx = self.comboBox_results_lsm_run_selection.currentIndex()
         return idx, time_str
 
     def get_selected_station(self):
@@ -2619,15 +2671,15 @@
                             QMessageBox.critical(self, 'Error!', str(e))
                             flag_export_successful = False
 
                     # Write log file:
                     try:
                         if dlg.checkBox_write_log_file.checkState() == Qt.Checked:
                             filename_log = filename + '.log'
-                            self.campaign.write_log_file(filename=os.path.join(output_path, filename_log),
+                            self.campaign.write_log_file(filename_log=os.path.join(output_path, filename_log),
                                                          lsm_run_index=lsm_run_idx,
                                                          verbose=IS_VERBOSE)
                     except Exception as e:
                         QMessageBox.critical(self, 'Error!', str(e))
                         flag_export_successful = False
 
                     # Save drift plot to PNG file:
@@ -3991,14 +4043,15 @@
 def main():
     """Main program to start the GUI."""
     # Check out debug mode:
     if debugger_is_active():
         print('==> Debugger is active! <==')
         pd.set_option('display.max_columns', 150)
         pd.set_option('display.width', 1000)
+        np.set_printoptions(linewidth=300)
         # pd.set_option('display.max_rows', 20)
 
     # Create the application
     app = QApplication(sys.argv)
 
     # Create and show the application's main window
     main_window = MainWindow()
```

### Comparing `grav-toolbox-0.2.7/gravtools/gui/gui_misc.py` & `grav_toolbox-0.2.8/gravtools/gui/gui_misc.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/gui/gui_model_observation_table.py` & `grav_toolbox-0.2.8/gravtools/gui/gui_model_observation_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/gui/gui_model_results_correlation_matrix_table.py` & `grav_toolbox-0.2.8/gravtools/gui/gui_model_results_correlation_matrix_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/gui/gui_model_results_drift_table.py` & `grav_toolbox-0.2.8/gravtools/gui/gui_model_results_drift_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/gui/gui_model_results_obs_table.py` & `grav_toolbox-0.2.8/gravtools/gui/gui_model_results_obs_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,25 +31,27 @@
 
     # Number of decimal pla
     _DECIMAL_PLACES_PER_FLOAT_COLUMN = {
         'g_diff_mugal': 1,
         'sd_g_diff_mugal': 1,
         'sd_g_diff_est_mugal': 1,
         'v_diff_mugal': 1,
+        'sd_v_diff_mugal': 1,
         'sd_g_mugal': 1,
         'g_mugal': 1,
         'abw_mugal': 1,
         'delta_t_h': 3,
         'corr_drift_mugal': 1,
         'w_diff_mugal': 3,
         'r_diff_obs': 3,
         'ref_epoch_dt': 3,
         'w_obs_est_mugal': 3,  # LSM_non_diff
         'r_obs_est': 3,  # LSM_non_diff
         'v_obs_est_mugal': 1,  # LSM_non_diff
+        'sd_v_obs_est_mugal': 1,  # LSM_non_diff
         'sd_g_obs_est_mugal': 1,  # LSM_non_diff
         'g_obs_mugal': 1,  # LSM_non_diff
         'sd_g_obs_mugal': 1,  # LSM_non_diff
     }
 
     # Columns that will be shown in the table view, if available in the data (Also defines the order of columns):
     # - This is also e pre-selection for data columns that can be plotted in the observation plots in the results tab
@@ -68,14 +70,16 @@
         'sd_g_mugal': 'SD [µGal]',  # MLR
         'sd_g_diff_mugal': 'SD [µGal]',  # LSM_diff
         'sd_g_obs_mugal': 'SD [µGal]',  # LSM_non_diff
         'sd_g_diff_est_mugal': 'SD_est [µGal]',  # LSM_diff
         'sd_g_obs_est_mugal': 'SD_est [µGal]',  # LSM_non_diff
         'v_diff_mugal': 'v [µGal]',  # LSM_diff
         'v_obs_est_mugal': 'v [µGal]',  # LSM_non_diff
+        'sd_v_obs_est_mugal': 'SD_v [µGal]',  # LSM_non_diff
+        'sd_v_diff_mugal': 'SD_v [µGal]',  # LSM_non_diff
         'w_diff_mugal': 'w',  # LSM_diff
         'w_obs_est_mugal': 'w',  # LSM_non_diff
         'r_diff_obs': 'r',  # LSM_diff
         'r_obs_est': 'r',  # LSM_non_diff
         'tau_test_result': 'Outlier test',  # LSM_non_diff, LSM_diff
         'corr_drift_mugal': 'Drift corr. [µGal]',  # MLR: Estimated drift correction
         'abw_mugal': 'abw [µGal]',  # MLR: Difference between drift-corrected instrument reading and the estimated station gravity
@@ -104,28 +108,30 @@
     ]
 
     # Columns that can be plotted. Column names (keys) and description (values):
     # - numerical data only!
     _PLOTABLE_DATA_COLUMNS = {
         # LSM_diff:
         'v_diff_mugal': 'Post-fit residuals [µGal]',  # LSM_diff
+        'w_diff_mugal': 'w',  # LSM_diff
+        'r_diff_obs': 'Redundancy components []',  # LSM_diff
+        'sd_v_diff_mugal': 'SD of post-fit residuals [µGal]',  # LSM_diff
         'sd_g_diff_est_mugal': 'A posteriori SD of diff. obs. [µGal]',  # LSM_diff
         'g_diff_mugal': 'Differential observation [µGal]',  # LSM_diff
         'sd_g_diff_mugal': 'SD of differential observation [µGal]',  # LSM_diff
         # MLR:
         'g_mugal': 'Instrument reading [µGal]',  # MLR
         'sd_g_mugal': 'Standard deviation of the instrument reading [µGal]',  # MLR
         'corr_drift_mugal': 'Estimated drift correction [µGal]',  # MLR
         'abw_mugal': 'Drift-corrected reading minus estimated station gravity (not absolute) [µGal]',  # MLR
-        'r_diff_obs': 'Redundancy components []',  # LSM_diff
-        'w_diff_mugal': 'Standardized post-fit residuals []',  # LSM_diff
         # LSM_non_diff:
+        'v_obs_est_mugal': 'Post-fit residuals [µGal]',  # LSM_non_diff
         'w_obs_est_mugal': 'Standardized post-fit residuals []',  # LSM_non_diff
         'r_obs_est': 'Redundancy components []',  # LSM_non_diff
-        'v_obs_est_mugal': 'Post-fit residuals [µGal]',  # LSM_non_diff
+        'sd_v_obs_est_mugal': 'SD of post-fit residuals [µGal]',  # LSM_non_diff
         'sd_g_obs_est_mugal': 'A posteriori SD of observation [µGal]',  # LSM_non_diff
         'g_obs_mugal': 'Non-differential observation [µGal]',  # LSM_non_diff
         'sd_g_obs_mugal': 'SD of non-differential observation [µGal]',  # LSM_non_diff
     }
 
     def __init__(self, lsm_runs):
         """Initialize the observation-results table view model.
```

### Comparing `grav-toolbox-0.2.7/gravtools/gui/gui_model_results_stat_table.py` & `grav_toolbox-0.2.8/gravtools/gui/gui_model_results_stat_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/gui/gui_model_results_vg_table.py` & `grav_toolbox-0.2.8/gravtools/gui/gui_model_results_vg_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/gui/gui_model_setup_table.py` & `grav_toolbox-0.2.8/gravtools/gui/gui_model_setup_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
         'sd_g_mugal': 'SD [µGal]',
         'epoch_unix': 'Epoch Unix',
         'delta_t_h': 'd_t [h]',
         'delta_t_campaign_h': 'd_t camp [h]',
         'sd_setup_mugal': 'SD of obs [µGal]',
         'number_obs': 'Number of obs.',
         'dhf_sensor_m': 'dhf_sensor [m]',
+        'linear_scale': 'linear scale',
     }
     _SHOW_COLUMNS_IN_TABLE = list(_SHOW_COLUMNS_IN_TABLE_DICT.keys())  # Actual list of columns to be shown
 
     # List of columns that are shown in the simple mode of the GUI
     _SHOW_COLUMNS_IN_TABLE_SIMPLE_GUI = [
         'station_name',
         'setup_id',
@@ -69,14 +70,15 @@
         'g_mugal': 1,
         'sd_g_mugal': 1,
         'epoch_unix': 1,
         'delta_t_h': 3,
         'delta_t_campaign_h': 3,
         'sd_setup_mugal': 1,
         'dhf_sensor_m': 3,
+        'linear_scale': 5,
     }
 
     def __init__(self, surveys):
         """Initialize the observation table view model.
 
         Parameters
         ----------
```

### Comparing `grav-toolbox-0.2.7/gravtools/gui/gui_model_station_table.py` & `grav_toolbox-0.2.8/gravtools/gui/gui_model_station_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/gui/gui_model_survey_table.py` & `grav_toolbox-0.2.8/gravtools/gui/gui_model_survey_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/gui/gui_models_gravimeters_scale_table.py` & `grav_toolbox-0.2.8/gravtools/gui/gui_models_gravimeters_scale_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/gui/survey_table_handler.py` & `grav_toolbox-0.2.8/gravtools/gui/survey_table_handler.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/models/__init__.py` & `grav_toolbox-0.2.8/gravtools/models/__init__.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/models/atmosphere_correction.py` & `grav_toolbox-0.2.8/gravtools/models/atmosphere_correction.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/models/campaign.py` & `grav_toolbox-0.2.8/gravtools/models/campaign.py`

 * *Files 3% similar despite different names*

```diff
@@ -318,14 +318,42 @@
         except:
             if verbose:
                 print(f'Failed to deactivate survey "{survey_name}"')
             return False
         else:
             return True
 
+    def deactivate_all_surveys(self, verbose=False):
+        """Deactivates all surveys in the campaign.
+
+        Parameters
+        ----------
+        verbose : bool, optional (default=False)
+                If True, status messages are printed to the command line.
+        """
+        changed_surveys = []
+        for survey_name, survey in self.surveys.items():
+            if self.deactivate_survey(survey_name=survey_name, verbose=verbose):
+                changed_surveys.append(survey_name)
+        return changed_surveys
+
+    def activate_all_surveys(self, verbose=False):
+        """Activates all surveys in the campaign.
+
+        Parameters
+        ----------
+        verbose : bool, optional (default=False)
+                If True, status messages are printed to the command line.
+        """
+        changed_surveys = []
+        for survey_name, survey in self.surveys.items():
+            if self.activate_survey(survey_name=survey_name, verbose=verbose):
+                changed_surveys.append(survey_name)
+        return changed_surveys
+
     def get_survey_names_and_status(self, verbose: bool = False) -> dict:
         """Return list with all survey names and information whether the survey is set active.
 
         Parameters
         ----------
         verbose : bool, optional (default=False)
             If True, survey names and status are printed to the command line.
@@ -629,27 +657,40 @@
         list : List of string stating the epochs of lsm adjustment runs that can be used to identify individual runs.
         """
         lsm_run_times = []
         for lsm_run in self.lsm_runs:
             lsm_run_times.append(lsm_run.time_str)
         return lsm_run_times
 
+    @property
+    def number_of_lsm_runs(self):
+        """Returns the number of LSM runs in the campaign."""
+        if self.lsm_runs is None:
+            return 0
+        else:
+            return len(self.lsm_runs)
+
     def delete_lsm_run(self, idx):
         """Delete the LSM run with the specified index in the list.
 
         Parameters
         ----------
         idx : int
             Index of the LSM object in the list.
         """
         if idx != -1:
             del self.lsm_runs[idx]
 
+    def delete_all_lsm_runs(self):
+        """Delete all LSM runs in the campaign."""
+        if self.lsm_runs is not None:
+            self.lsm_runs.clear()
+
     def set_reference_time(self, ref_delta_t_dt):
-        """Set refernce time for the determination of relative time spans, e.g. for the drift polynomial.
+        """Set reference time for the determination of relative time spans, e.g. for the drift polynomial.
 
         Parameters
         ----------
         ref_delta_t_dt : datetime object
             Reference time epoch w.r.t. UTC.
         """
         if isinstance(ref_delta_t_dt, dt.datetime):
```

### Comparing `grav-toolbox-0.2.7/gravtools/models/exceptions.py` & `grav_toolbox-0.2.8/gravtools/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/models/gravimeter.py` & `grav_toolbox-0.2.8/gravtools/models/gravimeter.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/models/lsm.py` & `grav_toolbox-0.2.8/gravtools/models/lsm.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/models/lsm_diff.py` & `grav_toolbox-0.2.8/gravtools/models/lsm_diff.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 import pandas as pd
 import datetime as dt
 import pytz
+
 # from matplotlib import pyplot as plt
 
 # optional imports:
 try:
     import geopandas
 except ImportError:
     _has_geopandas = False
@@ -58,14 +59,15 @@
         'station_name_to': 'str',
         'setup_id_from': 'int',
         'setup_id_to': 'int',
         'g_diff_mugal': 'float',
         'sd_g_diff_mugal': 'float',
         'sd_g_diff_est_mugal': 'float',
         'v_diff_mugal': 'float',  # Post fit residuals
+        'sd_v_diff_mugal': 'float',  # SD of post-fit residuals
         'w_diff_mugal': 'float',
         'r_diff_obs': 'float',
         'tau_test_result': 'str',
     }
     _SETUP_DIFF_COLUMNS = list(_SETUP_DIFF_COLUMNS_DTYPES.keys())
 
     # Short colum names with max. 10 char suitable for shapefiles
@@ -77,14 +79,15 @@
         'station_name_to': 'stat_to',
         'setup_id_from': 'setup_from',
         'setup_id_to': 'setup_to',
         'g_diff_mugal': 'dg',
         'sd_g_diff_mugal': 'sd_dg',
         'sd_g_diff_est_mugal': 'sd_dg_est',
         'v_diff_mugal': 'v',  # Post fit residuals
+        'sd_v_diff_mugal': 'sd_v',  # Post fit residuals
         'w_diff_mugal': 'w',
         'r_diff_obs': 'r',
         'tau_test_result': 'tau_test',
     }
 
     # Column names of self.drift_pol_df:
     # - keys: Column names of the pandas dataframe
@@ -387,14 +390,15 @@
                                                   g_diff_obs_mugal_list,
                                                   sd_g_diff_obs_mugal_list,
                                                   None_list_placeholder,
                                                   None_list_placeholder,
                                                   None_list_placeholder,
                                                   None_list_placeholder,
                                                   None_list_placeholder,
+                                                  None_list_placeholder,
                                                   )),
                                          columns=self._SETUP_DIFF_COLUMNS)
         self.setup_obs_df = self.setup_obs_df.astype(self._SETUP_DIFF_COLUMNS_DTYPES)
 
         # - constraints:
         datum_station_id = -1
         for index, row in stat_df_obs_datum.iterrows():
@@ -422,17 +426,20 @@
                 self.log_str += tmp_str
 
         # Solve equation system:
         mat_N = mat_A.T @ mat_P @ mat_A  # Normal equation matrix
         mat_Qxx = np.linalg.inv(mat_N)  # Co-factor matrix of estimates
         mat_x = mat_Qxx @ (mat_A.T @ mat_P @ mat_L)  # Estimates
         mat_v = (mat_A @ mat_x) - mat_L  # Post-fit residuals
+        mat_v = misc.numpy_array_set_zero(mat_v)
         mat_Qldld = mat_A @ mat_Qxx @ mat_A.T  # A posteriori Co-factor matrix of adjusted observations
+        mat_Qldld = misc.numpy_array_set_zero(mat_Qldld)
         # mat_Qll = np.linalg.inv(mat_P)
         mat_Qvv = mat_Qll - mat_Qldld  # Co-factor matrix of post-fit residuals
+        mat_Qvv = misc.numpy_array_set_zero(mat_Qvv)
 
         # Test: "Gewichtsreziprokenprobe nach Ansermet" (see Skriptum AG1, p. 136, Eq. (6.86))
         u = np.sum(np.diag((mat_P @ mat_Qldld)))  # number of unknown parameters (estimates)
         tmp_diff = np.abs(number_of_parameters - u)
         if np.abs(number_of_parameters - u) > settings.ANSERMET_DIFF_THRESHOLD:
             raise AssertionError(f'"Gewichtsreziprokenprobe nach Ansermet" failed! Difference = {tmp_diff}')
         else:
@@ -471,24 +478,34 @@
             if self.write_log:
                 self.log_str += tmp_str
 
         # ### Statistics and tests ###
 
         # Convert co-factor matrices to covariance matrices (variances in diagonal vector)
         mat_Cvv = s02_a_posteriori_mugal2 * mat_Qvv  # A posteriori Covariance matrix of post-fit residuals
-        mat_Cxx = s02_a_posteriori_mugal2 * mat_Qxx  # A posteriori Covariance matrix of estimated paramaters
+        mat_Cxx = s02_a_posteriori_mugal2 * mat_Qxx  # A posteriori Covariance matrix of estimated parameters
         mat_Cldld = s02_a_posteriori_mugal2 * mat_Qldld  # A posteriori Covariance matrix of adjusted observations
         # diag_Qxx = np.diag(mat_Qxx)
 
         # Calculate standard deviations:
         mat_sd_xx = np.sqrt(np.diag(mat_Cxx))  # A posteriori SD of estimates
         mat_sd_ldld = np.sqrt(np.diag(mat_Cldld))  # A posteriori SD of adjusted observations
-        # mat_sd_vv = np.sqrt(np.diag(mat_Cvv))  # A posteriori SD of residuals
-        mat_sd_vv = np.sqrt(
-            np.diag(abs(mat_Cvv)))  # !!!! without "abs()" the sqrt operation fails because neg. values may occure!
+
+        # A posteriori SD of residuals:
+        # - Check just in case, whether all diagonal elements of the Qvv matrix are positive!
+        if (np.diag(mat_Qvv) < 0).any():
+            mat_sd_vv = np.sqrt(np.diag(abs(mat_Cvv)))
+            if verbose or self.write_log:
+                tmp_str = f' - Warning: At least one diagonal element of the Qvv matrix is negative!\n'
+                if verbose:
+                    print(tmp_str)
+                if self.write_log:
+                    self.log_str += tmp_str
+        else:
+            mat_sd_vv = np.sqrt(np.diag(mat_Cvv))
 
         # creating histogram from residuals
         residual_hist, bin_edges = create_hist(mat_v)  # Calculate histogram
 
         # goodness-of-fit test
         chi_crit, chi_val, chi_test = global_model_test(confidence_level_chi_test, dof,
                                                         s02_a_posteriori_mugal2, sig0_mugal ** 2)
@@ -504,26 +521,28 @@
                 tmp_str += f'  {bin_edges[loop_1]:16.4f}  {bin_edges[loop_1 + 1]:16.4f}  {residual_hist[loop_1]:9.0f}\n'
             if verbose:
                 print(tmp_str)
             if self.write_log:
                 self.log_str += tmp_str
 
         # outlier detection effectiveness (redundancy components)
-        diag_Qvv = np.diag(mat_Qvv)  # TODO: Still needed?
+        # diag_Qvv = np.diag(mat_Qvv)
         # mat_R = np.diag(mat_P) * diag_Qvv
         # mat_R is exactly the same as "mat_r"
 
         # Redundanzanteile (redundancy components):
         # - AG II, pp. 66-71
         mat_r = np.diag(mat_Qvv @ mat_P)
 
-        # Standardisierte Versesserungen (AG II, p. 66)
-        # - Normalverteilt mit Erwartwarungswert = 0 (wie Verbesserungen)
-        # - Standardabweichung = 1 (standardisiert)
-        mat_w = mat_v[:, 0] / mat_sd_vv
+        # Standardized residuals used as test statistics for outlier detection:
+        # - AG II, p. 66
+        # - Taking care of zero-elements in the mat_sd_vv vector to prevent division by zero errors!
+        mat_w = np.zeros(len(mat_v))
+        tmp_filter = ~np.isclose(mat_v[:, 0], 0.0)
+        mat_w[tmp_filter] = mat_v[tmp_filter, 0] / mat_sd_vv[tmp_filter]
 
         # Tau test for outlier detection:
         alpha_tau = 1 - confidence_level_tau_test
         tau_test_result, tau_critical_value = tau_test(mat_w=mat_w, dof=dof, alpha=alpha_tau, mat_r=mat_r)
         number_of_outliers = tau_test_result.count("failed")
 
         tau_test_result_diff_obs = tau_test_result[:number_of_diff_obs]
@@ -552,25 +571,28 @@
         sd_g_est_mugal = mat_sd_xx[0:number_of_stations]
         drift_pol_coeff = mat_x[number_of_stations:, 0]
         drift_pol_coeff_sd = mat_sd_xx[number_of_stations:]
         sd_diff_obs_mugal = mat_sd_ldld[:number_of_diff_obs]
         sd_pseudo_obs_mugal = mat_sd_ldld[number_of_diff_obs:]
         v_diff_obs_mugal = mat_v[:number_of_diff_obs, 0]
         v_pseudo_obs_mugal = mat_v[number_of_diff_obs:, 0]
+        sd_v_diff_obs_mugal = mat_sd_vv[:number_of_diff_obs]
+        # sd_v_pseudo_obs_mugal = mat_sd_vv[number_of_diff_obs:]  # Not used
         w_diff_mugal = mat_w[:number_of_diff_obs]
         w_pseudo_obs_mugal = mat_w[number_of_diff_obs:]
         r_diff_obs = mat_r[:number_of_diff_obs]
         r_pseudo_obs = mat_r[number_of_diff_obs:]
 
         # Station related results:
         for idx, stat_name in enumerate(self.observed_stations):
             filter_tmp = self.stat_obs_df['station_name'] == stat_name
             self.stat_obs_df.loc[filter_tmp, 'g_est_mugal'] = g_est_mugal[idx]
             self.stat_obs_df.loc[filter_tmp, 'sd_g_est_mugal'] = sd_g_est_mugal[idx]
-            self.stat_obs_df.loc[filter_tmp, 'se_g_est_mugal'] = np.sqrt(sd_g_est_mugal[idx]**2 + noise_floor_mugal**2)
+            self.stat_obs_df.loc[filter_tmp, 'se_g_est_mugal'] = np.sqrt(
+                sd_g_est_mugal[idx] ** 2 + noise_floor_mugal ** 2)
         # Calculate differences to estimates:
         self.stat_obs_df['diff_g_est_mugal'] = self.stat_obs_df['g_est_mugal'] - self.stat_obs_df['g_mugal']
         self.stat_obs_df['diff_se_g_est_mugal'] = self.stat_obs_df['se_g_est_mugal'] - self.stat_obs_df['sd_g_mugal']
 
         # Drift parameters:
         survey_name_list = []
         degree_list = []
@@ -602,28 +624,30 @@
                                                   coeff_unit_list,
                                                   ref_epoch_t0_dt_list)),
                                          columns=self._DRIFT_POL_DF_COLUMNS)
 
         for idx, v_diff_mugal in enumerate(v_diff_obs_mugal):
             filter_tmp = self.setup_obs_df['diff_obs_id'] == idx
             self.setup_obs_df.loc[filter_tmp, 'v_diff_mugal'] = v_diff_mugal
+            self.setup_obs_df.loc[filter_tmp, 'sd_v_diff_mugal'] = sd_v_diff_obs_mugal[idx]
             self.setup_obs_df.loc[filter_tmp, 'sd_g_diff_est_mugal'] = sd_diff_obs_mugal[idx]
             self.setup_obs_df.loc[filter_tmp, 'w_diff_mugal'] = w_diff_mugal[idx]  # standardized residuals
             self.setup_obs_df.loc[filter_tmp, 'r_diff_obs'] = r_diff_obs[
                 idx]  # redundancy components
             self.setup_obs_df.loc[filter_tmp, 'tau_test_result'] = tau_test_result_diff_obs[idx]  # str
 
         # Print results to terminal:
         if verbose or self.write_log:
             tmp_str = f'\n'
             tmp_str += f' - Station data:\n'
             tmp_str += self.stat_obs_df[['station_name', 'is_datum', 'g_mugal', 'g_est_mugal',
                                          'diff_g_est_mugal', 'sd_g_mugal',
                                          'sd_g_est_mugal', 'se_g_est_mugal']].to_string(index=False,
-                                                                      float_format=lambda x: '{:.1f}'.format(x))
+                                                                                        float_format=lambda
+                                                                                            x: '{:.1f}'.format(x))
             tmp_str += f'\n\n'
             tmp_str += f' - Drift polynomial coefficients:\n'
             tmp_str += self.drift_pol_df.to_string(index=False, float_format=lambda x: '{:.6f}'.format(x))
             tmp_str += f'\n\n'
             tmp_str += f' - Differential observations:\n'
             for survey_name in survey_names:
                 filter_tmp = self.setup_obs_df['survey_name'] == survey_name
```

### Comparing `grav-toolbox-0.2.7/gravtools/models/lsm_nondiff.py` & `grav_toolbox-0.2.8/gravtools/models/lsm_nondiff.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,16 @@
         'ref_epoch_dt': 'datetime64[ns, UTC]',
         'obs_id': 'int',
         'station_name': 'str',
         'setup_id': 'int',
         'g_obs_mugal': 'float',
         'sd_g_obs_mugal': 'float',
         'sd_g_obs_est_mugal': 'float',
-        'v_obs_est_mugal': 'float',  # Post fit residuals
+        'v_obs_est_mugal': 'float',  # Post-fit residuals
+        'sd_v_obs_est_mugal': 'float',  # SD of post-fit residuals
         'w_obs_est_mugal': 'float',
         'r_obs_est': 'float',
         'tau_test_result': 'str',
     }
     _SETUP_OBS_COLUMNS = list(_SETUP_OBS_COLUMNS_DTYPES.keys())
 
     # Short colum names with max. 10 char suitable for shapefiles:
@@ -70,15 +71,16 @@
         'ref_epoch_dt': 'epoch_dt',
         'obs_id': 'obs_id',
         'station_name': 'station',
         'setup_id': 'setup',
         'g_obs_mugal': 'g',
         'sd_g_obs_mugal': 'sd_g',
         'sd_g_obs_est_mugal': 'sd_g_est',
-        'v_obs_est_mugal': 'v',  # Post fit residuals
+        'v_obs_est_mugal': 'v',  # Post-fit residuals
+        'sd_v_obs_est_mugal': 'sd_v',  # SD of post-fit residuals
         'w_obs_est_mugal': 'w',
         'r_obs_est': 'r',
         'tau_test_result': 'tau_test',
     }
 
     # Column names of self.drift_pol_df:
     # - keys: Column names of the pandas dataframe
@@ -104,15 +106,16 @@
             are the survey names (str). The items are again keys with the following items:
 
             - ref_epoch_delta_t_h : datetime object
                 Reference epoch for the relative reference times in the column `delta_t_h` in the `setup_df` dataframe.
                 The reference epoch is determined as the epoch of the first (active) observation in this survey.
             -  ref_epoch_delta_t_campaign_h : datetime object
                 Reference epoch for the relative reference times in the column `delta_t_campaign_h` in the `setup_df`
-                dataframe. The reference epoch is determined as the epoch of the first (active) observation in the campaign.
+                dataframe. The reference epoch is determined as the epoch of the first (active) observation in the
+                campaign.
             - setup_df : Pandas DataFrame
                 Pandas dataframes containing the observation data (see :py:obj:`gravtools.Survey.setup_df`).
 
         comment : str, optional (default = '')
             Arbitrary comment on the LSM run.
         write_log : bool, optional (default=True)
             Flag that indicates whether log string should be written or not.
@@ -329,15 +332,15 @@
                 # Populate matrices and vectors:
                 mat_L0[(obs_id, 0)] = g_obs_mugal
                 mat_sig_ll0[obs_id] = sd_g_obs_mugal ** 2
                 # Partial derivative for g at stations:
                 mat_A0[obs_id, self.observed_stations.index(station_name)] = 1
                 # Partial derivative for drift polynomial including constant instrumental bias (pol. degree = 0):
                 for pd_drift_id in range(drift_pol_degree + 1):
-                    mat_A0[obs_id, pd_drift_col_offset + pd_drift_id + 1 + survey_count*(drift_pol_degree + 1)] = \
+                    mat_A0[obs_id, pd_drift_col_offset + pd_drift_id + 1 + survey_count * (drift_pol_degree + 1)] = \
                         delta_t_h ** pd_drift_id
 
                 # Log data in DataFrame:
                 g_obs_mugal_list.append(g_obs_mugal)
                 sd_g_obs_mugal_list.append(sd_g_obs_mugal)
                 station_name_list.append(station_name)
                 obs_id_list.append(obs_id)
@@ -354,14 +357,15 @@
                                                   g_obs_mugal_list,
                                                   sd_g_obs_mugal_list,
                                                   None_list_placeholder,
                                                   None_list_placeholder,
                                                   None_list_placeholder,
                                                   None_list_placeholder,
                                                   None_list_placeholder,
+                                                  None_list_placeholder,
                                                   )),
                                          columns=self._SETUP_OBS_COLUMNS)
         self.setup_obs_df = self.setup_obs_df.astype(self._SETUP_OBS_COLUMNS_DTYPES)
 
         # - constraints:
         datum_station_id = -1
         for index, row in stat_df_obs_datum.iterrows():
@@ -373,15 +377,15 @@
             sd_mugal_for_weighting = row['sd_g_mugal'] / scaling_factor_datum_observations
             mat_sig_llc[datum_station_id] = sd_mugal_for_weighting ** 2
 
         # Set up all required matrices:
         mat_A = np.vstack((mat_A0, mat_Ac))  # Eq. (16)
         mat_L = np.vstack((mat_L0, mat_Lc))  # Eq. (16)
         mat_sig_ll = np.diag(np.hstack((mat_sig_ll0, mat_sig_llc)))
-        mat_Qll = mat_sig_ll / (sig0_mugal**2)
+        mat_Qll = mat_sig_ll / (sig0_mugal ** 2)
         mat_P = np.linalg.inv(mat_Qll)
 
         if verbose or self.write_log:
             tmp_str = f'\n'
             tmp_str += f'---- Results and statistics ----\n'
             if verbose:
                 print(tmp_str)
@@ -389,17 +393,20 @@
                 self.log_str += tmp_str
 
         # Solve equation system:
         mat_N = mat_A.T @ mat_P @ mat_A  # Normal equation matrix
         mat_Qxx = np.linalg.inv(mat_N)  # Co-factor matrix of estimates
         mat_x = mat_Qxx @ (mat_A.T @ mat_P @ mat_L)  # Estimates
         mat_v = (mat_A @ mat_x) - mat_L  # Post-fit residuals
+        mat_v = misc.numpy_array_set_zero(mat_v, atol=1e-4)
         mat_Qldld = mat_A @ mat_Qxx @ mat_A.T  # A posteriori Co-factor matrix of adjusted observations
         # mat_Qll = np.linalg.inv(mat_P)
+        mat_Qldld = misc.numpy_array_set_zero(mat_Qldld)
         mat_Qvv = mat_Qll - mat_Qldld  # Co-factor matrix of post-fit residuals
+        mat_Qvv = misc.numpy_array_set_zero(mat_Qvv)
 
         # Test: "Gewichtsreziprokenprobe nach Ansermet" (see Skriptum AG1, p. 136, Eq. (6.86))
         u = np.sum(np.diag((mat_P @ mat_Qldld)))  # number of unknown parameters (estimates)
         tmp_diff = np.abs(number_of_parameters - u)
         if np.abs(number_of_parameters - u) > settings.ANSERMET_DIFF_THRESHOLD:
             raise AssertionError(f'"Gewichtsreziprokenprobe nach Ansermet" failed! Difference = {tmp_diff}')
         else:
@@ -409,15 +416,15 @@
                     print(tmp_str)
                 if self.write_log:
                     self.log_str += tmp_str
 
         # Condition of normal equation matrix:
         if verbose or self.write_log:
             cond = np.linalg.cond(mat_N)
-            tmp_str = f'Condition of normal equation matix N = {cond:1.3f}\n'
+            tmp_str = f'Condition of normal equation matrix N = {cond:1.3f}\n'
             if verbose:
                 print(tmp_str)
             if self.write_log:
                 self.log_str += tmp_str
 
         # A posteriori variance of unit weight s02:
         dof = mat_A.shape[0] - mat_A.shape[1]  # degree of freedom
@@ -438,23 +445,34 @@
             if self.write_log:
                 self.log_str += tmp_str
 
         # ### Statistics and tests ###
 
         # Convert co-factor matrices to covariance matrices (variances in diagonal vector)
         mat_Cvv = s02_a_posteriori_mugal2 * mat_Qvv  # A posteriori Covariance matrix of post-fit residuals
-        mat_Cxx = s02_a_posteriori_mugal2 * mat_Qxx  # A posteriori Covariance matrix of estimated paramaters
+        mat_Cxx = s02_a_posteriori_mugal2 * mat_Qxx  # A posteriori Covariance matrix of estimated parameters
         mat_Cldld = s02_a_posteriori_mugal2 * mat_Qldld  # A posteriori Covariance matrix of adjusted observations
         # diag_Qxx = np.diag(mat_Qxx)
 
         # Calculate standard deviations:
         mat_sd_xx = np.sqrt(np.diag(mat_Cxx))  # A posteriori SD of estimates
         mat_sd_ldld = np.sqrt(np.diag(mat_Cldld))  # A posteriori SD of adjusted observations
-        # mat_sd_vv = np.sqrt(np.diag(mat_Cvv))  # A posteriori SD of residuals
-        mat_sd_vv = np.sqrt(np.diag(abs(mat_Cvv)))  # !!!! without "abs()" the sqrt operation fails because neg. values may occur!
+
+        # A posteriori SD of residuals:
+        # - Check just in case, whether all diagonal elements of the Qvv matrix are positive!
+        if (np.diag(mat_Qvv) < 0).any():
+            mat_sd_vv = np.sqrt(np.diag(abs(mat_Cvv)))
+            if verbose or self.write_log:
+                tmp_str = f' - Warning: At least one diagonal element of the Qvv matrix is negative!\n'
+                if verbose:
+                    print(tmp_str)
+                if self.write_log:
+                    self.log_str += tmp_str
+        else:
+            mat_sd_vv = np.sqrt(np.diag(mat_Cvv))
 
         # creating histogram from residuals
         residual_hist, bin_edges = create_hist(mat_v)  # Calculate histogram
 
         # goodness-of-fit test
         chi_crit, chi_val, chi_test = global_model_test(confidence_level_chi_test, dof,
                                                         s02_a_posteriori_mugal2, sig0_mugal ** 2)
@@ -478,18 +496,20 @@
         # mat_R = np.diag(mat_P) * diag_Qvv
         # mat_R is exactly the same as "mat_r"
 
         # Redundanzanteile (redundancy components):
         # - AG II, pp. 66-71
         mat_r = np.diag(mat_Qvv @ mat_P)
 
-        # Standardisierte Versesserungen (AG II, p. 66)
-        # - Normalverteilt mit Erwartwarungswert = 0 (wie Verbesserungen)
-        # - Standardabweichung = 1 (standardisiert)
-        mat_w = mat_v[:,0] / mat_sd_vv
+        # Standardized residuals used as test statistics for outlier detection:
+        # - AG II, p. 66
+        # - Taking care of zero-elements in the mat_sd_vv vector to prevent division by zero errors!
+        mat_w = np.zeros(len(mat_v))
+        tmp_filter = ~np.isclose(mat_v[:, 0], 0.0)
+        mat_w[tmp_filter] = mat_v[tmp_filter, 0] / mat_sd_vv[tmp_filter]
 
         # Tau test for outlier detection:
         alpha_tau = 1 - confidence_level_tau_test
         tau_test_result, tau_critical_value = tau_test(mat_w=mat_w, dof=dof, alpha=alpha_tau, mat_r=mat_r)
         number_of_outliers = tau_test_result.count("failed")
 
         tau_test_result_obs = tau_test_result[:number_of_observations]
@@ -517,15 +537,17 @@
         g_est_mugal = mat_x[0:number_of_stations, 0]
         sd_g_est_mugal = mat_sd_xx[0:number_of_stations]
         drift_pol_coeff = mat_x[number_of_stations:, 0]
         drift_pol_coeff_sd = mat_sd_xx[number_of_stations:]
         sd_g_obs_est_mugal = mat_sd_ldld[:number_of_observations]
         sd_pseudo_obs_est_mugal = mat_sd_ldld[number_of_observations:]
         v_obs_est_mugal = mat_v[:number_of_observations, 0]
+        sd_v_obs_est_mugal = mat_sd_vv[:number_of_observations]
         v_pseudo_obs_mugal = mat_v[number_of_observations:, 0]
+        # sd_v_pseudo_obs_mugal = mat_sd_vv[number_of_observations:]  # Not used
         w_obs_est_mugal = mat_w[:number_of_observations]
         w_pseudo_obs_mugal = mat_w[number_of_observations:]
         r_obs_est = mat_r[:number_of_observations]
         r_pseudo_obs = mat_r[number_of_observations:]
 
         # Station related results:
         for idx, stat_name in enumerate(self.observed_stations):
@@ -572,40 +594,43 @@
                                                   coeff_unit_list,
                                                   ref_epoch_t0_dt_list)),
                                          columns=self._DRIFT_POL_DF_COLUMNS)
 
         for idx, v_obs_mugal in enumerate(v_obs_est_mugal):
             filter_tmp = self.setup_obs_df['obs_id'] == idx
             self.setup_obs_df.loc[filter_tmp, 'v_obs_est_mugal'] = v_obs_mugal
+            self.setup_obs_df.loc[filter_tmp, 'sd_v_obs_est_mugal'] = sd_v_obs_est_mugal[idx]
             self.setup_obs_df.loc[filter_tmp, 'sd_g_obs_est_mugal'] = sd_g_obs_est_mugal[idx]
             self.setup_obs_df.loc[filter_tmp, 'w_obs_est_mugal'] = w_obs_est_mugal[idx]  # standardized residuals
             self.setup_obs_df.loc[filter_tmp, 'r_obs_est'] = r_obs_est[idx]  # redundancy components
             self.setup_obs_df.loc[filter_tmp, 'tau_test_result'] = tau_test_result_obs[idx]  # str
 
         # Print results to terminal:
         if verbose or self.write_log:
             tmp_str = f'\n'
             tmp_str += f' - Station data:\n'
             tmp_str += self.stat_obs_df[['station_name', 'is_datum', 'g_mugal', 'g_est_mugal',
-                                                'diff_g_est_mugal', 'sd_g_mugal',
-                                                'sd_g_est_mugal', 'se_g_est_mugal']].to_string(index=False,
-                                                                             float_format=lambda x: '{:.1f}'.format(x))
+                                         'diff_g_est_mugal', 'sd_g_mugal',
+                                         'sd_g_est_mugal', 'se_g_est_mugal']].to_string(index=False,
+                                                                                        float_format=lambda
+                                                                                            x: '{:.1f}'.format(x))
             tmp_str += f'\n\n'
             tmp_str += f' - Drift polynomial coefficients:\n'
             tmp_str += self.drift_pol_df.to_string(index=False, float_format=lambda x: '{:.6f}'.format(x))
             tmp_str += f'\n\n'
             tmp_str += f' - Observations:\n'
             for survey_name in survey_names:
                 filter_tmp = self.setup_obs_df['survey_name'] == survey_name
                 tmp_str += f'   - Survey: {survey_name}\n'
-            tmp_str += self.setup_obs_df.loc[filter_tmp, ['station_name', 'g_obs_mugal',
-                                                            'sd_g_obs_mugal', 'sd_g_obs_est_mugal',
-                                                            'v_obs_est_mugal']].to_string(index=False,
-                                                                                       float_format=lambda x: '{:.1f}'.format(x))
-            tmp_str += f'\n\n'
+                tmp_str += self.setup_obs_df.loc[filter_tmp, ['station_name', 'g_obs_mugal',
+                                                              'sd_g_obs_mugal', 'sd_g_obs_est_mugal',
+                                                              'v_obs_est_mugal']].to_string(index=False,
+                                                                                            float_format=lambda
+                                                                                                x: '{:.1f}'.format(x))
+                tmp_str += f'\n\n'
             tmp_str += f' - Pseudo observations at datum stations (constraints):\n'
             tmp_str += f'Station name  sd [µGal]   v [µGal]   w [µGal]   r [0-1]    Tau test result\n'
             for idx, station_name in enumerate(datum_stations):
                 tmp_str += f'{station_name:10}   {sd_pseudo_obs_est_mugal[idx]:8.3}     {v_pseudo_obs_mugal[idx]:+8.3}     {w_pseudo_obs_mugal[idx]:+5.3}     {r_pseudo_obs[idx]:+5.3}  {tau_test_result_pseudo_obs[idx]}\n'
             if verbose:
                 print(tmp_str)
             if self.write_log:
@@ -659,11 +684,11 @@
                                           how='left')
 
         # Rename columns to short names with max 10 chars suitable for shapefiles:
         setup_obs_df.rename(columns=self._SETUP_OBS_COLUMNS_SHORT, inplace=True)
         setup_obs_df.drop(columns=['epoch_dt'], inplace=True)  # datetime fields cannot be converted to shapefiles!
 
         setup_obs_gdf = geopandas.GeoDataFrame(setup_obs_df,
-                                              geometry=geopandas.points_from_xy(setup_obs_df['long_deg'],
-                                                                                setup_obs_df['lat_deg']),
-                                              crs=epsg_code)
+                                               geometry=geopandas.points_from_xy(setup_obs_df['long_deg'],
+                                                                                 setup_obs_df['lat_deg']),
+                                               crs=epsg_code)
         setup_obs_gdf.to_file(filename)
```

### Comparing `grav-toolbox-0.2.7/gravtools/models/misc.py` & `grav_toolbox-0.2.8/gravtools/models/misc.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 
     Returns
     -------
     list : Non-unique items.
     """
     return [item for item, count in Counter(lst).items() if count > 1]
 
+
 def unique_ordered_list(seq: list) -> list:
     """Returns a unique list whilst keeping the order.
 
     Parameters
     ----------
     seq : list
         Input list.
@@ -115,14 +116,15 @@
         try:
             return func(*args, **kwargs)
         finally:
             end_ = int(round(time() * 1000)) - start
             print(f'time_it==> {func.__name__}: execution time: {end_ if end_ > 0 else 0} ms')
     return _time_it
 
+
 def conditional_decorator(dec, condition):
     """Generic conditional decorator.
 
     Parameters
     ----------
     dec : decorator
         Decorator that is executed if `condition` is `True`
@@ -132,7 +134,24 @@
     def decorator(func):
         if not condition:
             # Return the function unchanged, not decorated.
             return func
         return dec(func)
     return decorator
 
+
+def numpy_array_set_zero(input_array, atol=np.nan):
+    """Set all values to 0.0 which are close to zero.
+
+    Parameters
+    ----------
+    input_array : `np.array`
+        Input numpy array.
+    atol : float, optional (default=`np.nan`)
+        The absolute tolerance parameter of numpy.isclose (see numpy documentation).
+    """
+    if np.isnan(atol):
+        input_array[np.isclose(input_array, 0.0)] = 0.0
+    else:
+        input_array[np.isclose(input_array, 0.0, atol=atol)] = 0.0
+    return input_array
+
```

### Comparing `grav-toolbox-0.2.7/gravtools/models/mlr_bev_legacy.py` & `grav_toolbox-0.2.8/gravtools/models/mlr_bev_legacy.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/models/station.py` & `grav_toolbox-0.2.8/gravtools/models/station.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/models/survey.py` & `grav_toolbox-0.2.8/gravtools/models/survey.py`

 * *Files 1% similar despite different names*

```diff
@@ -347,14 +347,15 @@
         'epoch_unix',  # Reference epoch of `g_mugal` (unix time [sec])
         'epoch_dt',  # Reference epoch of `g_mugal` (datetime obj)
         'delta_t_h',  # Time span since reference time [hours]
         'delta_t_campaign_h',  # Time span since reference time [hours]
         'sd_setup_mugal',  # Standard deviation of active observations in this setup [µGal]
         'number_obs',  # Number of observations in a setup
         'dhf_sensor_m',  # Vertical distance between control point and sensor height
+        'linear_scale',  # Linear scale factor used for scaling the observations of the setup
     )
 
     _SETUP_OBS_LIST_DF_COLUMNS = (
         'station_name',  # Name of station (str)
         'obs_epoch',  # Observation epoch (datetime object, TZ=<UTC>), start of instrument reading!
         'keep_obs',  # If False, the observation is not used for calculating setup observations (bool)
     )
@@ -2032,14 +2033,15 @@
                 obs_epoch_list_unix = []
                 obs_epoch_list_dt = []
                 delta_t_h_list = []
                 delta_t_campaign_h_list = []
                 sd_setup_mugal_list = []
                 number_obs_list = []
                 dhf_sensor_m_list = []
+                linear_scale_list = []
 
                 setup_ids = active_obs_df['setup_id'].unique()
                 for setup_id in setup_ids:
                     tmp_filter = active_obs_df['setup_id'] == setup_id
                     if obs_type == 'observed':
                         g_mugal = active_obs_df.loc[tmp_filter, 'g_obs_mugal'].to_numpy()
                         sd_g_mugal = active_obs_df.loc[tmp_filter, 'sd_g_obs_mugal'].to_numpy()
@@ -2063,14 +2065,24 @@
                         sd_setup_mugal_list.append(np.nan)
 
                     number_obs_list.append(len(g_mugal))  # Number of observations
 
                     # Get vertical distance between sensor height and control point:
                     dhf_sensor_m_list.append(active_obs_df.loc[tmp_filter, 'dhf_m'].values[0] + dist_m)
 
+                    # Get linear scale factor
+                    unique_linear_scale_factor_of_setup = active_obs_df.loc[tmp_filter, 'linear_scale'].unique()
+                    # - Check whether a single scale factor was used for the setup:
+                    if unique_linear_scale_factor_of_setup.shape[0] == 1:
+                        linear_scale_list.append(unique_linear_scale_factor_of_setup[0])
+                    else:
+                        linear_scale_list.append(np.nan)
+                        if verbose:
+                            print(f'WARNING: In setup {setup_id} of survey {self.name} the linear scale factor is not unique!')
+
                     # observation epoch (UNIX timestamps in full seconds):
                     obs_epochs_series = active_obs_df.loc[tmp_filter, 'obs_epoch']
                     unix_obs_epochs = obs_epochs_series.values.astype(np.int64) / 10 ** 9
                     unix_setup_epoch = np.sum(unix_obs_epochs * weights) / np.sum(weights)
 
                     # Reference epoch as datetime object (TZ=<UTC>):
                     dt_setup_epoch = dt.datetime.utcfromtimestamp(unix_setup_epoch)
@@ -2136,15 +2148,16 @@
                                                   sd_g_red_mugal_list,
                                                   obs_epoch_list_unix,
                                                   obs_epoch_list_dt,
                                                   delta_t_h_list,
                                                   delta_t_campaign_h_list,
                                                   sd_setup_mugal_list,
                                                   number_obs_list,
-                                                  dhf_sensor_m_list)),
+                                                  dhf_sensor_m_list,
+                                                  linear_scale_list)),
                                          columns=self._SETUP_DF_COLUMNS)
             self.set_reference_time(ref_delta_t_dt)  # Save reference time for `delta_t_h`, i.e. for the survey.
 
     def create_setup_obs_list(self):
         """Create list of all observations that contribute to the calculation of setup data in this Survey object.
 
         The list is created as pandas dataframe. It holds information whether an observation in the `obs_df` is
```

### Comparing `grav-toolbox-0.2.7/gravtools/models/vg_lsm.py` & `grav_toolbox-0.2.8/gravtools/models/vg_lsm.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,18 +57,18 @@
         'station_name': 'Station',
         'setup_id': 'Setup ID',
         'g_obs_mugal': 'g [µGal]',
         'sd_g_obs_mugal': 'SD [µGal]',
         'dhf_sensor_m': 'Sensor height [m]',
         'sd_g_obs_est_mugal': 'SD_est [µGal]',
         'v_obs_est_mugal': 'Residuals [µGal]',  # Post fit residuals
+        'sd_v_obs_est_mugal': 'SD_v [µGal]',  # SD of post-fit residuals
         'w_obs_est_mugal': 'Std. Residual []',
         'r_obs_est': 'Redundancy []',
         'tau_test_result': 'Outlier Test',
-        'tau_test_result': 'Outlier Test',
     }
     _SETUP_OBS_COLUMNS = list(_SETUP_OBS_COLUMNS_DICT.keys())
 
     # Column names of self.drift_pol_df:
     # - keys: Column names of the pandas dataframe
     # - values: Short description for table headers, etc., in the GUI
     _DRIFT_POL_DF_COLUMNS_DICT = {
@@ -376,14 +376,15 @@
                                                   sd_g_obs_mugal_list,
                                                   dhf_sensor_m_list,
                                                   None_list_placeholder,
                                                   None_list_placeholder,
                                                   None_list_placeholder,
                                                   None_list_placeholder,
                                                   None_list_placeholder,
+                                                  None_list_placeholder,
                                                   )),
                                          columns=self._SETUP_OBS_COLUMNS)
 
         # Set up all required matrices:
         mat_sig_ll = np.diag(mat_sig_ll)
         mat_Qll = mat_sig_ll / (sig0_mugal ** 2)
         mat_P = np.linalg.inv(mat_Qll)
@@ -397,17 +398,20 @@
                 self.log_str += tmp_str
 
         # Solve equation system:
         mat_N = mat_A.T @ mat_P @ mat_A  # Normal equation matrix
         mat_Qxx = np.linalg.inv(mat_N)  # Co-factor matrix of estimates
         mat_x = mat_Qxx @ (mat_A.T @ mat_P @ mat_L)  # Estimates
         mat_v = (mat_A @ mat_x) - mat_L  # Post-fit residuals
+        mat_v = misc.numpy_array_set_zero(mat_v, atol=1e-4)  # ToDo: Check atol!
         mat_Qldld = mat_A @ mat_Qxx @ mat_A.T  # A posteriori Co-factor matrix of adjusted observations
+        mat_Qldld = misc.numpy_array_set_zero(mat_Qldld)
         # mat_Qll = np.linalg.inv(mat_P)
         mat_Qvv = mat_Qll - mat_Qldld  # Co-factor matrix of post-fit residuals
+        mat_Qvv = misc.numpy_array_set_zero(mat_Qvv)
 
         # Test: "Gewichtsreziprokenprobe nach Ansermet" (see Skriptum AG1, p. 136, Eq. (6.86))
         u = np.sum(np.diag((mat_P @ mat_Qldld)))  # number of unknown parameters (estimates)
         tmp_diff = np.abs(number_of_parameters - u)
         if np.abs(number_of_parameters - u) > settings.ANSERMET_DIFF_THRESHOLD:
             raise AssertionError(f'"Gewichtsreziprokenprobe nach Ansermet" failed! Difference = {tmp_diff}')
         else:
@@ -454,16 +458,28 @@
         mat_Cldld = s02_a_posteriori_mugal2 * mat_Qldld  # A posteriori Covariance matrix of adjusted observations
         # diag_Qxx = np.diag(mat_Qxx)
 
         # Calculate standard deviations:
         mat_sd_xx = np.sqrt(np.diag(mat_Cxx))  # A posteriori SD of estimates
         mat_sd_ldld = np.sqrt(np.diag(mat_Cldld))  # A posteriori SD of adjusted observations
         # mat_sd_vv = np.sqrt(np.diag(mat_Cvv))  # A posteriori SD of residuals
-        mat_sd_vv = np.sqrt(
-            np.diag(abs(mat_Cvv)))  # !!!! without "abs()" the sqrt operation fails because neg. values may occur!
+        # mat_sd_vv = np.sqrt(np.diag(abs(mat_Cvv)))  # !!!! without "abs()" the sqrt operation fails because neg. values may occur!
+
+        # A posteriori SD of residuals:
+        # - Check just in case, whether all diagonal elements of the Qvv matrix are positive!
+        if (np.diag(mat_Qvv) < 0).any():
+            mat_sd_vv = np.sqrt(np.diag(abs(mat_Cvv)))
+            if verbose or self.write_log:
+                tmp_str = f' - Warning: At least one diagonal element of the Qvv matrix is negative!\n'
+                if verbose:
+                    print(tmp_str)
+                if self.write_log:
+                    self.log_str += tmp_str
+        else:
+            mat_sd_vv = np.sqrt(np.diag(mat_Cvv))
 
         # creating histogram from residuals
         residual_hist, bin_edges = create_hist(mat_v)  # Calculate histogram
 
         # goodness-of-fit test
         chi_crit, chi_val, chi_test = global_model_test(confidence_level_chi_test, dof,
                                                         s02_a_posteriori_mugal2, sig0_mugal ** 2)
@@ -483,18 +499,20 @@
                 self.log_str += tmp_str
 
         # Redundanzanteile (redundancy components):
         # - Measure for the outlier detection effectiveness
         # - AG II, pp. 66-71
         mat_r = np.diag(mat_Qvv @ mat_P)
 
-        # Standardisierte Versesserungen (AG II, p. 66)
-        # - Normalverteilt mit Erwartwarungswert = 0 (wie Verbesserungen)
-        # - Standardabweichung = 1 (standardisiert)
-        mat_w = mat_v[:, 0] / mat_sd_vv
+        # Standardized residuals used as test statistics for outlier detection:
+        # - AG II, p. 66
+        # - Taking care of zero-elements in the mat_sd_vv vector to prevent division by zero errors!
+        mat_w = np.zeros(len(mat_v))
+        tmp_filter = ~np.isclose(mat_v[:, 0], 0.0)
+        mat_w[tmp_filter] = mat_v[tmp_filter, 0] / mat_sd_vv[tmp_filter]
 
         # Tau test for outlier detection:
         alpha_tau = 1 - confidence_level_tau_test
         tau_test_result, tau_critical_value = tau_test(mat_w=mat_w, dof=dof, alpha=alpha_tau, mat_r=mat_r)
         number_of_outliers = tau_test_result.count("failed")
 
         if verbose or self.write_log:
@@ -512,14 +530,15 @@
         # #### Store results ####
         drift_pol_coeff = mat_x[:drift_pol_degree + 1, 0]
         drift_pol_coeff_sd = mat_sd_xx[:drift_pol_degree + 1]
         vg_pol_coeff = mat_x[drift_pol_degree + 1:, 0]
         vg_pol_coeff_sd = mat_sd_xx[drift_pol_degree + 1:]
         sd_g_obs_est_mugal = mat_sd_ldld
         v_obs_est_mugal = mat_v
+        sd_v_obs_est_mugal = mat_sd_vv
         w_obs_est_mugal = mat_w
         r_obs_est = mat_r
         tau_test_result_obs = tau_test_result
 
         # Drift parameters:
         survey_name_list = []
         degree_list = []
@@ -573,14 +592,15 @@
                                                coeff_unit_list)),
                                       columns=self._VG_POL_DF_COLUMNS)
 
         # Observation-related results:
         for idx, v_obs_mugal in enumerate(v_obs_est_mugal):
             filter_tmp = self.setup_obs_df['obs_id'] == idx
             self.setup_obs_df.loc[filter_tmp, 'v_obs_est_mugal'] = v_obs_mugal
+            self.setup_obs_df.loc[filter_tmp, 'sd_v_obs_est_mugal'] = sd_v_obs_est_mugal[idx]
             self.setup_obs_df.loc[filter_tmp, 'sd_g_obs_est_mugal'] = sd_g_obs_est_mugal[idx]
             self.setup_obs_df.loc[filter_tmp, 'w_obs_est_mugal'] = w_obs_est_mugal[idx]  # standardized residuals
             self.setup_obs_df.loc[filter_tmp, 'r_obs_est'] = r_obs_est[idx]  # redundancy components
             self.setup_obs_df.loc[filter_tmp, 'tau_test_result'] = tau_test_result_obs[idx]  # str
 
         # Print results to terminal and to log string:
         if verbose or self.write_log:
```

### Comparing `grav-toolbox-0.2.7/gravtools/scripts/__init__.py` & `grav_toolbox-0.2.8/gravtools/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/scripts/create_correction_time_seriens_from_tsf.py` & `grav_toolbox-0.2.8/gravtools/scripts/create_correction_time_seriens_from_tsf.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/scripts/load_tfs_file.py` & `grav_toolbox-0.2.8/gravtools/scripts/load_tfs_file.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/scripts/run_gui.py` & `grav_toolbox-0.2.8/gravtools/scripts/run_gui.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/settings.py` & `grav_toolbox-0.2.8/gravtools/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,14 +199,17 @@
 
 # Available iteration approaches for scaling the SD of setup observations:
 ITERATION_APPROACHES = {
     'Multiplicative': 'Multiplicative iteration approach',
     'Additive': 'Additive iteration approach'
 }
 
+# Absolute tolerance for testing whether a value is equal to zero:
+IS_ZERO_ABS_TOLERANCE = 1e-6
+
 # Threshold for the "Gewichtsreziprokenprobe nach Ansermet" (see Skriptum AG1, p. 136, Eq. (6.86))
 ANSERMET_DIFF_THRESHOLD = 1e-3
 
 # Threshold for the redundancy component of an observation in order to apply a pope test for outlier detection:
 R_POPE_TEST_THRESHOLD = 1e-6
 
 # GUI and Program options:
@@ -224,14 +227,21 @@
     'scott': 'Estimator based on leave-one-out cross-validation estimate of the integrated squared error. Can be regarded as a generalization of Scott’s rule.',
     'rice': 'Estimator does not take variability into account, only data size. Commonly overestimates number of bins required.',
     'sturges': 'R’s default method, only accounts for data size. Only optimal for gaussian data and underestimates number of bins for large non-gaussian datasets.',
     'sqrt': 'Square root (of data size) estimator, used by Excel and other programs for its speed and simplicity.',
     'Num. of bins': 'User defined number of bins (min. = 2, max. = 1000).'
 }
 
+# Maximum number of bina allowed when using "auto" or "fd" binning method:
+HIST_MAX_BIN_NUM = 100
+
+# Backup binning method if more than HIST_MAX_BIN_NUM bins are created:
+HIST_BACKUP_BIN_METHOD = 'doane'
+
+
 # Time label format for y-ticks in time-series plots:
 # - Format string for datetime.strftime()
 Y_TICK_DATETIME_FORMAT = '%Y-%m-%d %H:%M:%S'
 
 # --- General color settings ---
 DATUM_STATION_COLOR = (255, 204, 204)
```

### Comparing `grav-toolbox-0.2.7/gravtools/tides/__init__.py` & `grav_toolbox-0.2.8/gravtools/tides/__init__.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/tides/correction_time_series.py` & `grav_toolbox-0.2.8/gravtools/tides/correction_time_series.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/tides/longman1959.py` & `grav_toolbox-0.2.8/gravtools/tides/longman1959.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/tides/tide_data.py` & `grav_toolbox-0.2.8/gravtools/tides/tide_data.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/gravtools/tides/tide_data_tfs.py` & `grav_toolbox-0.2.8/gravtools/tides/tide_data_tfs.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.2.7/setup.cfg` & `grav_toolbox-0.2.8/setup.cfg`

 * *Files identical despite different names*

