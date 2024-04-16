# Comparing `tmp/meggie-1.7.0.tar.gz` & `tmp/meggie-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meggie-1.7.0.tar", last modified: Mon Mar 25 07:36:14 2024, max compression
+gzip compressed data, was "meggie-1.8.0.tar", last modified: Tue Apr 16 18:23:02 2024, max compression
```

## Comparing `meggie-1.7.0.tar` & `meggie-1.8.0.tar`

### file list

```diff
@@ -1,415 +1,417 @@
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.881636 meggie-1.7.0/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      170 2024-02-25 09:06:03.000000 meggie-1.7.0/AUTHORS.rst
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1519 2024-02-25 09:06:03.000000 meggie-1.7.0/LICENSE
--rw-r--r--   0 zairex    (1000) zairex    (1000)      129 2024-02-25 09:06:03.000000 meggie-1.7.0/MANIFEST.in
--rw-r--r--   0 zairex    (1000) zairex    (1000)      395 2024-03-25 07:36:14.881636 meggie-1.7.0/PKG-INFO
--rw-r--r--   0 zairex    (1000) zairex    (1000)      508 2024-02-25 09:06:03.000000 meggie-1.7.0/README.md
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/
--rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/__init__.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/
--rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/__init__.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/epochs_create/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1074 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/epochs_create/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      165 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/epochs_create/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/epochs_create/controller/
--rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/epochs_create/controller/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     3539 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/epochs_create/controller/epoching.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/epochs_create/dialogs/
--rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/epochs_create/dialogs/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     6814 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/epochs_create/dialogs/createEpochsFromEventsDialogMain.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)    21556 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/epochs_create/dialogs/createEpochsFromEventsDialogUi.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/epochs_create/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      923 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/epochs_create/tests/test_epochs_create.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/epochs_delete/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      821 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/epochs_delete/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      178 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/epochs_delete/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/epochs_delete/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      426 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/epochs_delete/tests/test_epochs_delete.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/epochs_delete_from_all/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1210 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/epochs_delete_from_all/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      205 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/epochs_delete_from_all/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/epochs_delete_from_all/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      483 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/epochs_delete_from_all/tests/test_epochs_delete_from_all.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/epochs_info/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1613 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/epochs_info/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      155 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/epochs_info/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/epochs_info/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      433 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/epochs_info/tests/test_epochs_info.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/epochs_plot/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      761 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/epochs_plot/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      155 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/epochs_plot/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/epochs_plot/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      412 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/epochs_plot/tests/test_epochs_plot.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/epochs_plot_image/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1049 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/epochs_plot_image/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      172 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/epochs_plot_image/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/epochs_plot_image/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      451 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/epochs_plot_image/tests/test_epochs_plot_image.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/evoked_create/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     2240 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/evoked_create/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      263 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/evoked_create/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/evoked_create/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      577 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/evoked_create/tests/test_evoked_create.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/evoked_delete/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      821 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/evoked_delete/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      184 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/evoked_delete/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/evoked_delete/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      426 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/evoked_delete/tests/test_evoked_delete.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/evoked_delete_from_all/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1208 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/evoked_delete_from_all/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      211 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/evoked_delete_from_all/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/evoked_delete_from_all/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      483 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/evoked_delete_from_all/tests/test_evoked_delete_from_all.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/evoked_group_average/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1626 2024-03-01 18:37:34.000000 meggie-1.7.0/meggie/actions/evoked_group_average/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      252 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/evoked_group_average/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/evoked_group_average/controller/
--rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/evoked_group_average/controller/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     4038 2024-03-01 17:58:36.000000 meggie-1.7.0/meggie/actions/evoked_group_average/controller/evoked.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/evoked_group_average/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      884 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/evoked_group_average/tests/test_evoked_group_average.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/evoked_info/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      891 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/evoked_info/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      154 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/evoked_info/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/evoked_info/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      433 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/evoked_info/tests/test_evoked_info.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/evoked_plot/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1853 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/evoked_plot/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      265 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/evoked_plot/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/evoked_plot/controller/
--rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/evoked_plot/controller/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     3964 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/evoked_plot/controller/evoked.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/evoked_plot/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      641 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/evoked_plot/tests/test_evoked_plot_all_channels.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      648 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/evoked_plot/tests/test_evoked_plot_channel_averages.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/evoked_plot_topomap/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     2787 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/evoked_plot_topomap/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      229 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/evoked_plot_topomap/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/evoked_plot_topomap/dialogs/
--rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/evoked_plot_topomap/dialogs/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1457 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/evoked_plot_topomap/dialogs/evokedTopomapDialogMain.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     6965 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/evoked_plot_topomap/dialogs/evokedTopomapDialogUi.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/evoked_plot_topomap/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      714 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/evoked_plot_topomap/tests/test_evoked_plot_topomap.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/evoked_save/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     2069 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/evoked_save/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      205 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/evoked_save/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/evoked_save/controller/
--rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/evoked_save/controller/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     2821 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/evoked_save/controller/evoked.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/evoked_save/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      641 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/evoked_save/tests/test_evoked_save_all_channels.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      648 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/evoked_save/tests/test_evoked_save_channel_averages.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/raw_event_info/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1121 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/raw_event_info/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      145 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/raw_event_info/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/raw_event_info/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      372 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/raw_event_info/tests/test_raw_event_info.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie/actions/raw_events_from_annotations/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1025 2024-03-02 10:07:31.000000 meggie-1.7.0/meggie/actions/raw_events_from_annotations/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      196 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/raw_events_from_annotations/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/raw_events_from_annotations/dialogs/
--rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/raw_events_from_annotations/dialogs/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     3386 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/raw_events_from_annotations/dialogs/eventsFromAnnotationsDialogMain.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     8107 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/raw_events_from_annotations/dialogs/eventsFromAnnotationsDialogUi.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/raw_events_from_annotations/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1058 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/raw_events_from_annotations/tests/test_raw_events_from_annotations.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/raw_filter/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      805 2024-03-02 10:07:31.000000 meggie-1.7.0/meggie/actions/raw_filter/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      235 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/raw_filter/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/raw_filter/controller/
--rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/raw_filter/controller/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1343 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/raw_filter/controller/filter.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/raw_filter/dialogs/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     4378 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/raw_filter/dialogs/filterDialogMain.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)    16994 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/raw_filter/dialogs/filterDialogUi.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/raw_filter/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      506 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/raw_filter/tests/test_raw_filter.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/raw_ica/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      617 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/raw_ica/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      221 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/raw_ica/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/raw_ica/controller/
--rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/raw_ica/controller/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1762 2024-03-13 19:16:16.000000 meggie-1.7.0/meggie/actions/raw_ica/controller/ica.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/raw_ica/dialogs/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     7113 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/raw_ica/dialogs/icaDialogMain.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     8934 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/raw_ica/dialogs/icaDialogUi.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/raw_ica/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1048 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/raw_ica/tests/test_raw_ica.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/raw_measurement_info/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1603 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/raw_measurement_info/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      163 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/raw_measurement_info/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/raw_measurement_info/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      402 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/raw_measurement_info/tests/test_raw_measurement_info.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/raw_montage/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1322 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/raw_montage/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      200 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/raw_montage/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/raw_montage/dialogs/
--rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/raw_montage/dialogs/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     4202 2024-03-02 10:07:31.000000 meggie-1.7.0/meggie/actions/raw_montage/dialogs/montageDialogMain.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     8450 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/raw_montage/dialogs/montageDialogUi.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/raw_montage/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1022 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/raw_montage/tests/test_raw_montage.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/raw_plot/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     2222 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/raw_plot/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      139 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/raw_plot/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/raw_plot/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      386 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/raw_plot/tests/test_raw_plot.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/raw_plot_projections/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1004 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/raw_plot_projections/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      206 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/raw_plot_projections/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/raw_plot_projections/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      391 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/raw_plot_projections/tests/test_raw_plot_projections.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/raw_rereference/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      990 2024-03-02 10:07:31.000000 meggie-1.7.0/meggie/actions/raw_rereference/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      255 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/raw_rereference/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/raw_rereference/dialogs/
--rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/raw_rereference/dialogs/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     3302 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/raw_rereference/dialogs/rereferencingDialogMain.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     7452 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/raw_rereference/dialogs/rereferencingDialogUi.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/raw_rereference/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      604 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/raw_rereference/tests/test_raw_rereference.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/raw_resample/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      813 2024-03-02 10:07:31.000000 meggie-1.7.0/meggie/actions/raw_resample/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      171 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/raw_resample/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/raw_resample/dialogs/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     2352 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/raw_resample/dialogs/resamplingDialogMain.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     6232 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/raw_resample/dialogs/resamplingDialogUi.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/raw_resample/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      538 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/raw_resample/tests/test_raw_resample.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/spectrum_create/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1311 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/spectrum_create/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      197 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/spectrum_create/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/spectrum_create/controller/
--rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/spectrum_create/controller/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     2738 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/spectrum_create/controller/spectrum.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/spectrum_create/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      676 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/spectrum_create/tests/test_spectrum_create.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/spectrum_delete/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      831 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/spectrum_delete/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      181 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/spectrum_delete/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/spectrum_delete/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      444 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/spectrum_delete/tests/test_spectrum_delete.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/spectrum_delete_from_all/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1222 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/spectrum_delete_from_all/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      208 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/spectrum_delete_from_all/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/spectrum_delete_from_all/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      501 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/spectrum_delete_from_all/tests/test_spectrum_delete_from_all.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/spectrum_group_average/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1626 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/spectrum_group_average/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      247 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/spectrum_group_average/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/spectrum_group_average/controller/
--rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/spectrum_group_average/controller/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     4006 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/spectrum_group_average/controller/spectrum.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/spectrum_group_average/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      898 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/spectrum_group_average/tests/test_spectrum_group_average.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/spectrum_info/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1849 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/spectrum_info/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      158 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/spectrum_info/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/spectrum_info/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      447 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/spectrum_info/tests/test_spectrum_info.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/spectrum_plot/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1757 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/spectrum_plot/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      269 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/spectrum_plot/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/spectrum_plot/controller/
--rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/spectrum_plot/controller/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     4384 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/spectrum_plot/controller/spectrum.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/spectrum_plot/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      659 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/spectrum_plot/tests/test_spectrum_plot_all_channels.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      666 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/spectrum_plot/tests/test_spectrum_plot_channel_averages.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/spectrum_save/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     2029 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/spectrum_save/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      202 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/spectrum_save/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/spectrum_save/controller/
--rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/spectrum_save/controller/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     2664 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/spectrum_save/controller/spectrum.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/spectrum_save/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      659 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/spectrum_save/tests/test_spectrum_save_all_channels.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      666 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/spectrum_save/tests/test_spectrum_save_channels_averages.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/tfr_create/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1474 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/tfr_create/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      239 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/tfr_create/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/tfr_create/controller/
--rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/tfr_create/controller/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1400 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/tfr_create/controller/tfr.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/tfr_create/dialogs/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     5741 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/tfr_create/dialogs/TFRDialogMain.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)    14520 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/tfr_create/dialogs/TFRDialogUi.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/tfr_create/dialogs/__init__.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/tfr_create/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      774 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/tfr_create/tests/test_tfr_create.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/tfr_delete/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      807 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/tfr_delete/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      166 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/tfr_delete/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/tfr_delete/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      399 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/tfr_delete/tests/test_tfr_delete.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/tfr_delete_from_all/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1187 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/tfr_delete_from_all/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      193 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/tfr_delete_from_all/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/tfr_delete_from_all/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      456 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/tfr_delete_from_all/tests/test_tfr_delete_from_all.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/tfr_group_average/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1582 2024-03-01 18:37:20.000000 meggie-1.7.0/meggie/actions/tfr_group_average/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      237 2024-03-01 18:18:16.000000 meggie-1.7.0/meggie/actions/tfr_group_average/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/tfr_group_average/controller/
--rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-03-01 18:18:16.000000 meggie-1.7.0/meggie/actions/tfr_group_average/controller/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     3978 2024-03-01 18:18:16.000000 meggie-1.7.0/meggie/actions/tfr_group_average/controller/tfr.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/tfr_group_average/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      863 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/tfr_group_average/tests/test_tfr_group_average.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/tfr_info/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1983 2024-03-02 10:07:31.000000 meggie-1.7.0/meggie/actions/tfr_info/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      143 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/tfr_info/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/tfr_info/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      412 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/tfr_info/tests/test_tfr_info.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/tfr_plot/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     3263 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/tfr_plot/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      229 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/tfr_plot/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/tfr_plot/controller/
--rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/tfr_plot/controller/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     4539 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/tfr_plot/controller/tfr.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/tfr_plot/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      623 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/tfr_plot/tests/test_tfr_plot_all_channels.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      630 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/tfr_plot/tests/test_tfr_plot_channel_averages.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/tfr_plot_tse/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     2719 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/tfr_plot_tse/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      296 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/tfr_plot_tse/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/tfr_plot_tse/controller/
--rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/tfr_plot_tse/controller/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     6129 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/tfr_plot_tse/controller/tfr.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/tfr_plot_tse/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      642 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/tfr_plot_tse/tests/test_tfr_plot_tse_all_channels.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      649 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/tfr_plot_tse/tests/test_tfr_plot_tse_channel_averages.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/tfr_save/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     2547 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/tfr_save/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      191 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/tfr_save/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/tfr_save/controller/
--rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/tfr_save/controller/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     3700 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/tfr_save/controller/tfr.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/tfr_save/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      623 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/tfr_save/tests/test_tfr_save_all_channels.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      630 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/tfr_save/tests/test_tfr_save_channel_averages.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/tfr_save_tse/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     2535 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/tfr_save_tse/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      252 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/tfr_save_tse/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/tfr_save_tse/controller/
--rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/actions/tfr_save_tse/controller/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     3951 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/tfr_save_tse/controller/tfr.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/actions/tfr_save_tse/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      642 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/tfr_save_tse/tests/test_tfr_save_tse_all_channels.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      649 2024-03-20 09:10:34.000000 meggie-1.7.0/meggie/actions/tfr_save_tse/tests/test_tfr_save_tse_channel_averages.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     2368 2024-03-16 07:32:56.000000 meggie-1.7.0/meggie/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/datatypes/
--rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/datatypes/__init__.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/datatypes/epochs/
--rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/datatypes/epochs/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      122 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/datatypes/epochs/configuration.json
--rw-r--r--   0 zairex    (1000) zairex    (1000)     2207 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/datatypes/epochs/epochs.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/datatypes/epochs/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1171 2024-03-20 09:10:51.000000 meggie-1.7.0/meggie/datatypes/epochs/tests/test_epochs.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/datatypes/evoked/
--rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/datatypes/evoked/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      124 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/datatypes/evoked/configuration.json
--rw-r--r--   0 zairex    (1000) zairex    (1000)     3616 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/datatypes/evoked/evoked.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/datatypes/evoked/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1334 2024-03-20 09:10:51.000000 meggie-1.7.0/meggie/datatypes/evoked/tests/test_evoked.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/datatypes/spectrum/
--rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/datatypes/spectrum/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      136 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/datatypes/spectrum/configuration.json
--rw-r--r--   0 zairex    (1000) zairex    (1000)     7604 2024-03-20 09:10:51.000000 meggie-1.7.0/meggie/datatypes/spectrum/spectrum.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/datatypes/spectrum/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1449 2024-03-20 09:10:51.000000 meggie-1.7.0/meggie/datatypes/spectrum/tests/test_spectrum.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/datatypes/tfr/
--rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/datatypes/tfr/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      106 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/datatypes/tfr/configuration.json
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/datatypes/tfr/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1500 2024-03-20 09:10:51.000000 meggie-1.7.0/meggie/datatypes/tfr/tests/test_tfr.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     5562 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/datatypes/tfr/tfr.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)    15001 2024-03-20 09:10:51.000000 meggie-1.7.0/meggie/experiment.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)    14151 2024-03-25 07:31:42.000000 meggie-1.7.0/meggie/mainWindowMain.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)    12346 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/mainWindowUi.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/mainwindow/
--rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/mainwindow/__init__.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/mainwindow/dialogs/
--rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/mainwindow/dialogs/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      745 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/mainwindow/dialogs/aboutDialogMain.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)    12478 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/mainwindow/dialogs/aboutDialogUi.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     5688 2024-03-20 09:11:10.000000 meggie-1.7.0/meggie/mainwindow/dialogs/actionDialogMain.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     3618 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/mainwindow/dialogs/actionDialogUi.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1545 2024-03-15 09:03:28.000000 meggie-1.7.0/meggie/mainwindow/dialogs/activePluginsDialogMain.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     2669 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/mainwindow/dialogs/activePluginsDialogUi.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     5131 2024-03-25 07:31:42.000000 meggie-1.7.0/meggie/mainwindow/dialogs/addSubjectDialogMain.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     4720 2024-03-25 07:31:42.000000 meggie-1.7.0/meggie/mainwindow/dialogs/addSubjectDialogUi.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     7957 2024-03-14 08:37:56.000000 meggie-1.7.0/meggie/mainwindow/dialogs/channelGroupsDialogMain.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     7676 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/mainwindow/dialogs/channelGroupsDialogUi.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     3205 2024-03-20 09:11:10.000000 meggie-1.7.0/meggie/mainwindow/dialogs/createExperimentDialogMain.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     5186 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/mainwindow/dialogs/createExperimentDialogUi.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     2884 2024-03-20 09:11:10.000000 meggie-1.7.0/meggie/mainwindow/dialogs/pipelineDialogMain.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     3618 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/mainwindow/dialogs/pipelineDialogUi.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     2626 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/mainwindow/dialogs/preferencesDialogMain.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     5645 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/mainwindow/dialogs/preferencesDialogUi.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)    30567 2024-03-20 09:11:10.000000 meggie-1.7.0/meggie/mainwindow/dynamic.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     3363 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/mainwindow/preferences.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      570 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/run.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     5385 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/subject.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.871636 meggie-1.7.0/meggie/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1806 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/tests/test_experiment_and_subject.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.881636 meggie-1.7.0/meggie/utilities/
--rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     9514 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/channels.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1606 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/compare.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     2162 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/datatype.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      650 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/debug.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.881636 meggie-1.7.0/meggie/utilities/dialogs/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     3394 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/dialogs/TFROutputOptionsMain.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)    14493 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/dialogs/TFROutputOptionsUi.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/dialogs/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     2480 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/dialogs/bitSelectionDialogMain.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)    19515 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/dialogs/bitSelectionDialogUi.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     3271 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/dialogs/groupSelectionDialogMain.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     3767 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/dialogs/groupSelectionDialogUi.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      919 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/dialogs/outputOptionsMain.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     3214 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/dialogs/outputOptionsUi.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     2440 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/dialogs/powerSpectrumAddAdvancedDialogMain.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)    14149 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/dialogs/powerSpectrumAddAdvancedDialogUi.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     7443 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/dialogs/powerSpectrumDialogMain.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)    13826 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/dialogs/powerSpectrumDialogUi.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      513 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/dialogs/shortMessageBoxMain.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     3522 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/dialogs/shortMessageBoxUi.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      759 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/dialogs/shortQuestionBoxMain.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     3877 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/dialogs/shortQuestionBoxUi.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     3010 2024-03-20 09:10:51.000000 meggie-1.7.0/meggie/utilities/dialogs/simpleDialogMain.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     4680 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/dialogs/simpleDialogUi.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     2763 2024-03-20 09:10:51.000000 meggie-1.7.0/meggie/utilities/dialogs/singleChannelDialogMain.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     9496 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/dialogs/singleChannelDialogUi.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     7899 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/events.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     6905 2024-03-13 19:16:16.000000 meggie-1.7.0/meggie/utilities/filemanager.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      605 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/formats.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1492 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/measurement_info.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     2227 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/messaging.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      851 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/names.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     2110 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/plotting.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)    12332 2024-03-23 08:45:50.000000 meggie-1.7.0/meggie/utilities/testing.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.881636 meggie-1.7.0/meggie/utilities/tests/
--rw-r--r--   0 zairex    (1000) zairex    (1000)     3108 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/tests/test_channels.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     1476 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/tests/test_events.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     2373 2024-03-20 09:10:51.000000 meggie-1.7.0/meggie/utilities/tests/test_filemanager.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      559 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/tests/test_measurement_info.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      523 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/tests/test_names.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      203 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/tests/test_plotting.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     2311 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/threading.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)      158 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/uid.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     2079 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/units.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     2046 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/validators.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.881636 meggie-1.7.0/meggie/utilities/widgets/
--rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/widgets/__init__.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     3867 2024-03-20 09:10:51.000000 meggie-1.7.0/meggie/utilities/widgets/batchingWidgetMain.py
--rw-r--r--   0 zairex    (1000) zairex    (1000)     6168 2024-02-25 09:06:03.000000 meggie-1.7.0/meggie/utilities/widgets/batchingWidgetUi.py
-drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-03-25 07:36:14.861637 meggie-1.7.0/meggie.egg-info/
--rw-r--r--   0 zairex    (1000) zairex    (1000)      395 2024-03-25 07:36:14.000000 meggie-1.7.0/meggie.egg-info/PKG-INFO
--rw-r--r--   0 zairex    (1000) zairex    (1000)    13654 2024-03-25 07:36:14.000000 meggie-1.7.0/meggie.egg-info/SOURCES.txt
--rw-r--r--   0 zairex    (1000) zairex    (1000)        1 2024-03-25 07:36:14.000000 meggie-1.7.0/meggie.egg-info/dependency_links.txt
--rw-r--r--   0 zairex    (1000) zairex    (1000)       43 2024-03-25 07:36:14.000000 meggie-1.7.0/meggie.egg-info/entry_points.txt
--rw-r--r--   0 zairex    (1000) zairex    (1000)        1 2024-02-25 09:09:15.000000 meggie-1.7.0/meggie.egg-info/not-zip-safe
--rw-r--r--   0 zairex    (1000) zairex    (1000)        7 2024-03-25 07:36:14.000000 meggie-1.7.0/meggie.egg-info/top_level.txt
--rw-r--r--   0 zairex    (1000) zairex    (1000)       38 2024-03-25 07:36:14.881636 meggie-1.7.0/setup.cfg
--rw-r--r--   0 zairex    (1000) zairex    (1000)      603 2024-03-25 07:19:14.000000 meggie-1.7.0/setup.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.072518 meggie-1.8.0/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      170 2024-02-25 09:06:03.000000 meggie-1.8.0/AUTHORS.rst
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1519 2024-02-25 09:06:03.000000 meggie-1.8.0/LICENSE
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      129 2024-02-25 09:06:03.000000 meggie-1.8.0/MANIFEST.in
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      395 2024-04-16 18:23:02.072518 meggie-1.8.0/PKG-INFO
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      508 2024-02-25 09:06:03.000000 meggie-1.8.0/README.md
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.052518 meggie-1.8.0/meggie/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/__init__.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.052518 meggie-1.8.0/meggie/actions/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/__init__.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.052518 meggie-1.8.0/meggie/actions/epochs_create/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1074 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/epochs_create/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      186 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/epochs_create/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.052518 meggie-1.8.0/meggie/actions/epochs_create/controller/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/epochs_create/controller/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     3539 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/epochs_create/controller/epoching.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.052518 meggie-1.8.0/meggie/actions/epochs_create/dialogs/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/epochs_create/dialogs/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     6814 2024-03-28 11:19:06.000000 meggie-1.8.0/meggie/actions/epochs_create/dialogs/createEpochsFromEventsDialogMain.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)    21556 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/epochs_create/dialogs/createEpochsFromEventsDialogUi.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.052518 meggie-1.8.0/meggie/actions/epochs_create/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      923 2024-03-28 11:19:06.000000 meggie-1.8.0/meggie/actions/epochs_create/tests/test_epochs_create.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.052518 meggie-1.8.0/meggie/actions/epochs_delete/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      821 2024-03-28 11:19:06.000000 meggie-1.8.0/meggie/actions/epochs_delete/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      178 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/epochs_delete/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.052518 meggie-1.8.0/meggie/actions/epochs_delete/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      368 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/epochs_delete/tests/test_epochs_delete.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.052518 meggie-1.8.0/meggie/actions/epochs_delete_from_all/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1210 2024-03-28 11:19:06.000000 meggie-1.8.0/meggie/actions/epochs_delete_from_all/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      205 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/epochs_delete_from_all/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.052518 meggie-1.8.0/meggie/actions/epochs_delete_from_all/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      416 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/epochs_delete_from_all/tests/test_epochs_delete_from_all.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.052518 meggie-1.8.0/meggie/actions/epochs_info/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1613 2024-03-28 11:19:06.000000 meggie-1.8.0/meggie/actions/epochs_info/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      155 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/epochs_info/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.052518 meggie-1.8.0/meggie/actions/epochs_info/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      377 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/epochs_info/tests/test_epochs_info.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.052518 meggie-1.8.0/meggie/actions/epochs_plot/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      793 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/epochs_plot/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      155 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/epochs_plot/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.052518 meggie-1.8.0/meggie/actions/epochs_plot/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      309 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/epochs_plot/tests/test_epochs_plot.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.052518 meggie-1.8.0/meggie/actions/epochs_plot_image/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1081 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/epochs_plot_image/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      172 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/epochs_plot_image/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.052518 meggie-1.8.0/meggie/actions/epochs_plot_image/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      389 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/epochs_plot_image/tests/test_epochs_plot_image.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.052518 meggie-1.8.0/meggie/actions/evoked_create/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     2148 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/evoked_create/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      263 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/evoked_create/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.052518 meggie-1.8.0/meggie/actions/evoked_create/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      577 2024-03-28 11:19:06.000000 meggie-1.8.0/meggie/actions/evoked_create/tests/test_evoked_create.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.052518 meggie-1.8.0/meggie/actions/evoked_delete/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      821 2024-03-28 11:19:06.000000 meggie-1.8.0/meggie/actions/evoked_delete/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      184 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/evoked_delete/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.052518 meggie-1.8.0/meggie/actions/evoked_delete/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      368 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/evoked_delete/tests/test_evoked_delete.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.052518 meggie-1.8.0/meggie/actions/evoked_delete_from_all/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1208 2024-03-28 11:19:06.000000 meggie-1.8.0/meggie/actions/evoked_delete_from_all/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      211 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/evoked_delete_from_all/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.052518 meggie-1.8.0/meggie/actions/evoked_delete_from_all/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      416 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/evoked_delete_from_all/tests/test_evoked_delete_from_all.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.052518 meggie-1.8.0/meggie/actions/evoked_group_average/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1626 2024-03-01 18:37:34.000000 meggie-1.8.0/meggie/actions/evoked_group_average/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      252 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/evoked_group_average/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.052518 meggie-1.8.0/meggie/actions/evoked_group_average/controller/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/evoked_group_average/controller/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     4038 2024-03-01 17:58:36.000000 meggie-1.8.0/meggie/actions/evoked_group_average/controller/evoked.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.052518 meggie-1.8.0/meggie/actions/evoked_group_average/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      819 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/evoked_group_average/tests/test_evoked_group_average.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.052518 meggie-1.8.0/meggie/actions/evoked_info/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      891 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/evoked_info/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      154 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/evoked_info/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.052518 meggie-1.8.0/meggie/actions/evoked_info/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      377 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/evoked_info/tests/test_evoked_info.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.052518 meggie-1.8.0/meggie/actions/evoked_plot/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1871 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/evoked_plot/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      265 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/evoked_plot/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.052518 meggie-1.8.0/meggie/actions/evoked_plot/controller/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/evoked_plot/controller/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     4112 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/evoked_plot/controller/evoked.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.052518 meggie-1.8.0/meggie/actions/evoked_plot/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      585 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/evoked_plot/tests/test_evoked_plot_all_channels.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      592 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/evoked_plot/tests/test_evoked_plot_channel_averages.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.052518 meggie-1.8.0/meggie/actions/evoked_plot_topomap/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     2805 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/evoked_plot_topomap/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      229 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/evoked_plot_topomap/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.052518 meggie-1.8.0/meggie/actions/evoked_plot_topomap/dialogs/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/evoked_plot_topomap/dialogs/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1457 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/evoked_plot_topomap/dialogs/evokedTopomapDialogMain.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     6965 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/evoked_plot_topomap/dialogs/evokedTopomapDialogUi.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.052518 meggie-1.8.0/meggie/actions/evoked_plot_topomap/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      714 2024-03-28 11:19:06.000000 meggie-1.8.0/meggie/actions/evoked_plot_topomap/tests/test_evoked_plot_topomap.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.052518 meggie-1.8.0/meggie/actions/evoked_save/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     2069 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/evoked_save/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      205 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/evoked_save/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/evoked_save/controller/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/evoked_save/controller/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     2821 2024-03-28 11:19:06.000000 meggie-1.8.0/meggie/actions/evoked_save/controller/evoked.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/evoked_save/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      585 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/evoked_save/tests/test_evoked_save_all_channels.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      592 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/evoked_save/tests/test_evoked_save_channel_averages.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/raw_event_info/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1121 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/raw_event_info/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      166 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/raw_event_info/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/raw_event_info/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      313 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/raw_event_info/tests/test_raw_event_info.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/raw_events_from_annotations/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1025 2024-03-02 10:07:31.000000 meggie-1.8.0/meggie/actions/raw_events_from_annotations/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      217 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/raw_events_from_annotations/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/raw_events_from_annotations/dialogs/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/raw_events_from_annotations/dialogs/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     3386 2024-03-28 11:19:06.000000 meggie-1.8.0/meggie/actions/raw_events_from_annotations/dialogs/eventsFromAnnotationsDialogMain.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     8107 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/raw_events_from_annotations/dialogs/eventsFromAnnotationsDialogUi.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/raw_events_from_annotations/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1058 2024-03-28 11:19:06.000000 meggie-1.8.0/meggie/actions/raw_events_from_annotations/tests/test_raw_events_from_annotations.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/raw_filter/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      805 2024-03-02 10:07:31.000000 meggie-1.8.0/meggie/actions/raw_filter/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      256 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/raw_filter/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/raw_filter/controller/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/raw_filter/controller/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1343 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/raw_filter/controller/filter.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/raw_filter/dialogs/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     4378 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/raw_filter/dialogs/filterDialogMain.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)    16994 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/raw_filter/dialogs/filterDialogUi.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/raw_filter/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      506 2024-03-28 11:19:06.000000 meggie-1.8.0/meggie/actions/raw_filter/tests/test_raw_filter.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/raw_ica/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      617 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/raw_ica/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      242 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/raw_ica/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/raw_ica/controller/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/raw_ica/controller/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1762 2024-03-13 19:16:16.000000 meggie-1.8.0/meggie/actions/raw_ica/controller/ica.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/raw_ica/dialogs/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     7113 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/raw_ica/dialogs/icaDialogMain.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     8934 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/raw_ica/dialogs/icaDialogUi.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/raw_ica/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1048 2024-03-28 11:19:06.000000 meggie-1.8.0/meggie/actions/raw_ica/tests/test_raw_ica.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/raw_measurement_info/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1608 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/raw_measurement_info/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      184 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/raw_measurement_info/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/raw_measurement_info/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      337 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/raw_measurement_info/tests/test_raw_measurement_info.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/raw_montage/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1404 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/raw_montage/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      200 2024-04-03 15:31:36.000000 meggie-1.8.0/meggie/actions/raw_montage/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/raw_montage/dialogs/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/raw_montage/dialogs/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     4202 2024-03-02 10:07:31.000000 meggie-1.8.0/meggie/actions/raw_montage/dialogs/montageDialogMain.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     8450 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/raw_montage/dialogs/montageDialogUi.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/raw_montage/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1022 2024-03-28 11:19:06.000000 meggie-1.8.0/meggie/actions/raw_montage/tests/test_raw_montage.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/raw_plot/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     2222 2024-03-28 11:19:06.000000 meggie-1.8.0/meggie/actions/raw_plot/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      160 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/raw_plot/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/raw_plot/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      333 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/raw_plot/tests/test_raw_plot.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/raw_plot_projections/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1004 2024-03-28 11:19:06.000000 meggie-1.8.0/meggie/actions/raw_plot_projections/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      227 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/raw_plot_projections/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/raw_plot_projections/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      326 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/raw_plot_projections/tests/test_raw_plot_projections.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/raw_rereference/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      990 2024-03-02 10:07:31.000000 meggie-1.8.0/meggie/actions/raw_rereference/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      262 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/raw_rereference/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/raw_rereference/dialogs/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/raw_rereference/dialogs/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     3302 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/raw_rereference/dialogs/rereferencingDialogMain.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     7452 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/raw_rereference/dialogs/rereferencingDialogUi.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/raw_rereference/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      604 2024-03-28 11:19:06.000000 meggie-1.8.0/meggie/actions/raw_rereference/tests/test_raw_rereference.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/raw_resample/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      835 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/raw_resample/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      192 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/raw_resample/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/raw_resample/dialogs/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     2352 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/raw_resample/dialogs/resamplingDialogMain.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     6232 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/raw_resample/dialogs/resamplingDialogUi.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/raw_resample/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      538 2024-03-28 11:19:06.000000 meggie-1.8.0/meggie/actions/raw_resample/tests/test_raw_resample.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/spectrum_create/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1311 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/spectrum_create/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      218 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/spectrum_create/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/spectrum_create/controller/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/spectrum_create/controller/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     2739 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/spectrum_create/controller/spectrum.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/spectrum_create/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      676 2024-03-28 11:19:06.000000 meggie-1.8.0/meggie/actions/spectrum_create/tests/test_spectrum_create.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/spectrum_delete/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      831 2024-03-28 11:19:06.000000 meggie-1.8.0/meggie/actions/spectrum_delete/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      181 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/spectrum_delete/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/spectrum_delete/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      384 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/spectrum_delete/tests/test_spectrum_delete.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/spectrum_delete_from_all/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1222 2024-03-28 11:19:06.000000 meggie-1.8.0/meggie/actions/spectrum_delete_from_all/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      208 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/spectrum_delete_from_all/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/spectrum_delete_from_all/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      432 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/spectrum_delete_from_all/tests/test_spectrum_delete_from_all.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/spectrum_group_average/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1626 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/spectrum_group_average/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      247 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/spectrum_group_average/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/spectrum_group_average/controller/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/spectrum_group_average/controller/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     4006 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/spectrum_group_average/controller/spectrum.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/spectrum_group_average/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      831 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/spectrum_group_average/tests/test_spectrum_group_average.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/spectrum_info/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1849 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/spectrum_info/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      158 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/spectrum_info/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/spectrum_info/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      389 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/spectrum_info/tests/test_spectrum_info.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/spectrum_plot/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1757 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/spectrum_plot/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      269 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/spectrum_plot/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/spectrum_plot/controller/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/spectrum_plot/controller/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     4481 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/spectrum_plot/controller/spectrum.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/spectrum_plot/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      601 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/spectrum_plot/tests/test_spectrum_plot_all_channels.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      608 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/spectrum_plot/tests/test_spectrum_plot_channel_averages.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/spectrum_save/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     2029 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/spectrum_save/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      202 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/spectrum_save/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/spectrum_save/controller/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/spectrum_save/controller/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     2664 2024-03-28 11:19:06.000000 meggie-1.8.0/meggie/actions/spectrum_save/controller/spectrum.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/spectrum_save/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      601 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/spectrum_save/tests/test_spectrum_save_all_channels.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      608 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/spectrum_save/tests/test_spectrum_save_channels_averages.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/tfr_create/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1382 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/tfr_create/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      239 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/tfr_create/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/tfr_create/controller/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/tfr_create/controller/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1400 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/tfr_create/controller/tfr.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/tfr_create/dialogs/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     5741 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/tfr_create/dialogs/TFRDialogMain.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)    14520 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/tfr_create/dialogs/TFRDialogUi.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/tfr_create/dialogs/__init__.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/tfr_create/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      774 2024-03-28 11:19:06.000000 meggie-1.8.0/meggie/actions/tfr_create/tests/test_tfr_create.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/tfr_delete/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      807 2024-03-28 11:19:06.000000 meggie-1.8.0/meggie/actions/tfr_delete/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      166 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/tfr_delete/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/tfr_delete/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      344 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/tfr_delete/tests/test_tfr_delete.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/tfr_delete_from_all/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1187 2024-03-28 11:19:06.000000 meggie-1.8.0/meggie/actions/tfr_delete_from_all/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      193 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/tfr_delete_from_all/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/tfr_delete_from_all/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      392 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/tfr_delete_from_all/tests/test_tfr_delete_from_all.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/tfr_group_average/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1582 2024-03-01 18:37:20.000000 meggie-1.8.0/meggie/actions/tfr_group_average/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      237 2024-03-01 18:18:16.000000 meggie-1.8.0/meggie/actions/tfr_group_average/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/tfr_group_average/controller/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-03-01 18:18:16.000000 meggie-1.8.0/meggie/actions/tfr_group_average/controller/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     3941 2024-04-03 15:31:36.000000 meggie-1.8.0/meggie/actions/tfr_group_average/controller/tfr.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/tfr_group_average/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      801 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/tfr_group_average/tests/test_tfr_group_average.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/tfr_info/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1983 2024-03-02 10:07:31.000000 meggie-1.8.0/meggie/actions/tfr_info/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      143 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/tfr_info/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/tfr_info/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      359 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/tfr_info/tests/test_tfr_info.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/tfr_plot/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     3263 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/tfr_plot/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      229 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/tfr_plot/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/tfr_plot/controller/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/tfr_plot/controller/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     4635 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/tfr_plot/controller/tfr.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/tfr_plot/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      570 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/tfr_plot/tests/test_tfr_plot_all_channels.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      577 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/tfr_plot/tests/test_tfr_plot_channel_averages.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/tfr_plot_tse/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     2719 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/tfr_plot_tse/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      296 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/tfr_plot_tse/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/tfr_plot_tse/controller/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/tfr_plot_tse/controller/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     6226 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/tfr_plot_tse/controller/tfr.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/tfr_plot_tse/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      585 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/tfr_plot_tse/tests/test_tfr_plot_tse_all_channels.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      592 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/tfr_plot_tse/tests/test_tfr_plot_tse_channel_averages.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/tfr_save/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     2547 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/tfr_save/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      191 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/tfr_save/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/tfr_save/controller/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/tfr_save/controller/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     3700 2024-03-28 11:19:06.000000 meggie-1.8.0/meggie/actions/tfr_save/controller/tfr.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/tfr_save/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      570 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/tfr_save/tests/test_tfr_save_all_channels.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      577 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/tfr_save/tests/test_tfr_save_channel_averages.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/tfr_save_tse/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     2535 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/tfr_save_tse/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      252 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/tfr_save_tse/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/tfr_save_tse/controller/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/actions/tfr_save_tse/controller/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     3951 2024-03-28 11:19:06.000000 meggie-1.8.0/meggie/actions/tfr_save_tse/controller/tfr.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/actions/tfr_save_tse/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      585 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/tfr_save_tse/tests/test_tfr_save_tse_all_channels.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      592 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/actions/tfr_save_tse/tests/test_tfr_save_tse_channel_averages.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     2329 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/datatypes/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/datatypes/__init__.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/datatypes/epochs/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/datatypes/epochs/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      122 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/datatypes/epochs/configuration.json
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     2303 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/datatypes/epochs/epochs.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/datatypes/epochs/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1171 2024-03-28 11:19:10.000000 meggie-1.8.0/meggie/datatypes/epochs/tests/test_epochs.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/datatypes/evoked/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/datatypes/evoked/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      124 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/datatypes/evoked/configuration.json
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     3616 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/datatypes/evoked/evoked.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/datatypes/evoked/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1334 2024-03-28 11:19:10.000000 meggie-1.8.0/meggie/datatypes/evoked/tests/test_evoked.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.062518 meggie-1.8.0/meggie/datatypes/spectrum/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/datatypes/spectrum/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      136 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/datatypes/spectrum/configuration.json
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     7604 2024-03-28 11:19:10.000000 meggie-1.8.0/meggie/datatypes/spectrum/spectrum.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.072518 meggie-1.8.0/meggie/datatypes/spectrum/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1449 2024-03-28 11:19:10.000000 meggie-1.8.0/meggie/datatypes/spectrum/tests/test_spectrum.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.072518 meggie-1.8.0/meggie/datatypes/tfr/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/datatypes/tfr/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      106 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/datatypes/tfr/configuration.json
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.072518 meggie-1.8.0/meggie/datatypes/tfr/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1500 2024-03-28 11:19:10.000000 meggie-1.8.0/meggie/datatypes/tfr/tests/test_tfr.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     5570 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/datatypes/tfr/tfr.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)    15581 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/experiment.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)    14364 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/mainWindowMain.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)    12346 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/mainWindowUi.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.072518 meggie-1.8.0/meggie/mainwindow/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/mainwindow/__init__.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.072518 meggie-1.8.0/meggie/mainwindow/dialogs/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/mainwindow/dialogs/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      745 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/mainwindow/dialogs/aboutDialogMain.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)    12478 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/mainwindow/dialogs/aboutDialogUi.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     5688 2024-03-28 11:19:06.000000 meggie-1.8.0/meggie/mainwindow/dialogs/actionDialogMain.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     3618 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/mainwindow/dialogs/actionDialogUi.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1545 2024-03-15 09:03:28.000000 meggie-1.8.0/meggie/mainwindow/dialogs/activePluginsDialogMain.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     2669 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/mainwindow/dialogs/activePluginsDialogUi.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     5131 2024-03-25 07:31:42.000000 meggie-1.8.0/meggie/mainwindow/dialogs/addSubjectDialogMain.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     4720 2024-03-25 07:31:42.000000 meggie-1.8.0/meggie/mainwindow/dialogs/addSubjectDialogUi.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     8301 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/mainwindow/dialogs/channelGroupsDialogMain.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     7676 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/mainwindow/dialogs/channelGroupsDialogUi.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     4012 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/mainwindow/dialogs/createExperimentDialogMain.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     6271 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/mainwindow/dialogs/createExperimentDialogUi.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     2884 2024-03-28 11:19:06.000000 meggie-1.8.0/meggie/mainwindow/dialogs/pipelineDialogMain.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     3618 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/mainwindow/dialogs/pipelineDialogUi.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     2626 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/mainwindow/dialogs/preferencesDialogMain.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     5645 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/mainwindow/dialogs/preferencesDialogUi.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)    31180 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/mainwindow/dynamic.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     3778 2024-04-16 17:06:38.000000 meggie-1.8.0/meggie/mainwindow/preferences.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      778 2024-04-15 15:25:04.000000 meggie-1.8.0/meggie/run.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     6590 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/subject.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.072518 meggie-1.8.0/meggie/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1789 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/tests/test_experiment_and_subject.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.072518 meggie-1.8.0/meggie/utilities/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/utilities/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)    10528 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/utilities/channels.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1590 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/utilities/compare.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     3681 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/utilities/datasets.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     2162 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/utilities/datatype.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      650 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/utilities/debug.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.072518 meggie-1.8.0/meggie/utilities/dialogs/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     3394 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/utilities/dialogs/TFROutputOptionsMain.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)    14493 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/utilities/dialogs/TFROutputOptionsUi.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/utilities/dialogs/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     2480 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/utilities/dialogs/bitSelectionDialogMain.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)    19515 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/utilities/dialogs/bitSelectionDialogUi.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     3271 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/utilities/dialogs/groupSelectionDialogMain.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     3767 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/utilities/dialogs/groupSelectionDialogUi.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      919 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/utilities/dialogs/outputOptionsMain.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     3214 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/utilities/dialogs/outputOptionsUi.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     2440 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/utilities/dialogs/powerSpectrumAddAdvancedDialogMain.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)    14149 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/utilities/dialogs/powerSpectrumAddAdvancedDialogUi.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     7443 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/utilities/dialogs/powerSpectrumDialogMain.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)    13826 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/utilities/dialogs/powerSpectrumDialogUi.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      513 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/utilities/dialogs/shortMessageBoxMain.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     3522 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/utilities/dialogs/shortMessageBoxUi.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      759 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/utilities/dialogs/shortQuestionBoxMain.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     3877 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/utilities/dialogs/shortQuestionBoxUi.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     3010 2024-03-28 11:19:29.000000 meggie-1.8.0/meggie/utilities/dialogs/simpleDialogMain.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     4680 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/utilities/dialogs/simpleDialogUi.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     2763 2024-03-28 11:19:29.000000 meggie-1.8.0/meggie/utilities/dialogs/singleChannelDialogMain.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     9496 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/utilities/dialogs/singleChannelDialogUi.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     7899 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/utilities/events.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     7275 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/utilities/filemanager.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      605 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/utilities/formats.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1492 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/utilities/measurement_info.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     2227 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/utilities/messaging.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      851 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/utilities/names.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     2110 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/utilities/plotting.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)    12681 2024-04-16 17:55:54.000000 meggie-1.8.0/meggie/utilities/testing.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.072518 meggie-1.8.0/meggie/utilities/tests/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     3123 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/utilities/tests/test_channels.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      491 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/utilities/tests/test_datasets.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     1476 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/utilities/tests/test_events.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     2373 2024-03-28 11:19:22.000000 meggie-1.8.0/meggie/utilities/tests/test_filemanager.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      559 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/utilities/tests/test_measurement_info.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      523 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/utilities/tests/test_names.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      203 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/utilities/tests/test_plotting.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     2178 2024-04-15 15:23:54.000000 meggie-1.8.0/meggie/utilities/threading.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      158 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/utilities/uid.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     2079 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/utilities/units.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     2046 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/utilities/validators.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.072518 meggie-1.8.0/meggie/utilities/widgets/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)        0 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/utilities/widgets/__init__.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     3867 2024-03-28 11:19:37.000000 meggie-1.8.0/meggie/utilities/widgets/batchingWidgetMain.py
+-rw-r--r--   0 zairex    (1000) zairex    (1000)     6168 2024-02-25 09:06:03.000000 meggie-1.8.0/meggie/utilities/widgets/batchingWidgetUi.py
+drwxr-xr-x   0 zairex    (1000) zairex    (1000)        0 2024-04-16 18:23:02.052518 meggie-1.8.0/meggie.egg-info/
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      395 2024-04-16 18:23:02.000000 meggie-1.8.0/meggie.egg-info/PKG-INFO
+-rw-r--r--   0 zairex    (1000) zairex    (1000)    13723 2024-04-16 18:23:02.000000 meggie-1.8.0/meggie.egg-info/SOURCES.txt
+-rw-r--r--   0 zairex    (1000) zairex    (1000)        1 2024-04-16 18:23:02.000000 meggie-1.8.0/meggie.egg-info/dependency_links.txt
+-rw-r--r--   0 zairex    (1000) zairex    (1000)       43 2024-04-16 18:23:02.000000 meggie-1.8.0/meggie.egg-info/entry_points.txt
+-rw-r--r--   0 zairex    (1000) zairex    (1000)        1 2024-02-25 09:09:15.000000 meggie-1.8.0/meggie.egg-info/not-zip-safe
+-rw-r--r--   0 zairex    (1000) zairex    (1000)        7 2024-04-16 18:23:02.000000 meggie-1.8.0/meggie.egg-info/top_level.txt
+-rw-r--r--   0 zairex    (1000) zairex    (1000)       38 2024-04-16 18:23:02.072518 meggie-1.8.0/setup.cfg
+-rw-r--r--   0 zairex    (1000) zairex    (1000)      603 2024-04-16 18:09:01.000000 meggie-1.8.0/setup.py
```

### Comparing `meggie-1.7.0/LICENSE` & `meggie-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/epochs_create/__init__.py` & `meggie-1.8.0/meggie/actions/epochs_create/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/epochs_create/controller/epoching.py` & `meggie-1.8.0/meggie/actions/epochs_create/controller/epoching.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/epochs_create/dialogs/createEpochsFromEventsDialogMain.py` & `meggie-1.8.0/meggie/actions/epochs_create/dialogs/createEpochsFromEventsDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/epochs_create/dialogs/createEpochsFromEventsDialogUi.py` & `meggie-1.8.0/meggie/actions/epochs_create/dialogs/createEpochsFromEventsDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/epochs_create/tests/test_epochs_create.py` & `meggie-1.8.0/meggie/actions/epochs_create/tests/test_epochs_create.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/epochs_delete/__init__.py` & `meggie-1.8.0/meggie/actions/epochs_delete/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/epochs_delete_from_all/__init__.py` & `meggie-1.8.0/meggie/actions/epochs_delete_from_all/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/epochs_info/__init__.py` & `meggie-1.8.0/meggie/actions/epochs_info/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/epochs_plot/__init__.py` & `meggie-1.8.0/meggie/actions/epochs_plot/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,8 +22,9 @@
             self.handler(subject, {"name": selected_name})
         except Exception as exc:
             exc_messagebox(self.window, exc)
 
     @subject_action
     def handler(self, subject, params):
         epochs = subject.epochs.get(params["name"])
-        epochs.content.plot()
+        mne_epochs = epochs.content
+        mne_epochs.plot()
```

### Comparing `meggie-1.7.0/meggie/actions/epochs_plot_image/__init__.py` & `meggie-1.8.0/meggie/actions/raw_plot_projections/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,33 @@
-""" Contains implementation for epochs plot
+""" Contains implementation for raw plot projections
 """
 
+from meggie.utilities.messaging import messagebox
 from meggie.utilities.messaging import exc_messagebox
 from meggie.utilities.plotting import set_figure_title
-from meggie.utilities.plotting import get_figure_title
 
 from meggie.mainwindow.dynamic import Action
 from meggie.mainwindow.dynamic import subject_action
 
 
-class PlotEpochsImage(Action):
-    """Opens MNE's image plot."""
+class PlotProjections(Action):
+    """Shows a plot of existing projection vectors."""
 
     def run(self):
 
-        try:
-            selected_name = self.data["outputs"]["epochs"][0]
-        except IndexError:
-            return
-
         subject = self.experiment.active_subject
         try:
-            self.handler(subject, {"name": selected_name})
+            self.handler(subject, {})
         except Exception as exc:
             exc_messagebox(self.window, exc)
 
     @subject_action
     def handler(self, subject, params):
-        epochs = subject.epochs.get(params["name"])
-        figs = epochs.content.plot_image()
-        for fig in figs:
-            ch_type = get_figure_title(fig)
-            title = "{0}_{1}".format(params["name"], ch_type)
-            set_figure_title(fig, title)
+        raw = subject.get_raw()
+        if not raw.info["projs"]:
+            messagebox(self.window, "Data does not contain any projection vectors")
+            return
+        fig = raw.plot_projs_topomap()
+
+        elems = ["projections", subject.name]
+        set_figure_title(fig, "_".join(elems))
+        fig.suptitle(" ".join(elems))
```

### Comparing `meggie-1.7.0/meggie/actions/evoked_create/__init__.py` & `meggie-1.8.0/meggie/actions/evoked_create/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,18 +19,15 @@
     def run(self):
 
         selected_names = self.data["inputs"]["epochs"]
 
         if not selected_names:
             return
 
-        if len(selected_names) == 1:
-            stem = selected_names[0]
-        else:
-            stem = "Evoked"
+        stem = "Evoked"
 
         default_name = next_available_name(
             self.experiment.active_subject.evoked.keys(), stem
         )
 
         def close_handle(subject, params):
             params["conditions"] = selected_names
```

### Comparing `meggie-1.7.0/meggie/actions/evoked_create/tests/test_evoked_create.py` & `meggie-1.8.0/meggie/actions/evoked_create/tests/test_evoked_create.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/evoked_delete/__init__.py` & `meggie-1.8.0/meggie/actions/evoked_delete/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/evoked_delete_from_all/__init__.py` & `meggie-1.8.0/meggie/actions/evoked_delete_from_all/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/evoked_group_average/__init__.py` & `meggie-1.8.0/meggie/actions/evoked_group_average/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/evoked_group_average/controller/evoked.py` & `meggie-1.8.0/meggie/actions/evoked_group_average/controller/evoked.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/evoked_group_average/tests/test_evoked_group_average.py` & `meggie-1.8.0/meggie/actions/evoked_group_average/tests/test_evoked_group_average.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,17 +12,16 @@
 
         data = {"outputs": {"evoked": ["Evoked"]}}
 
         self.run_action(
             action_name="evoked_group_average",
             handler=GroupAverage,
             data=data,
-            patch_paths=["meggie.actions.evoked_group_average"],
         )
         dialog = self.find_dialog(GroupSelectionDialog)
 
         dialog.ui.checkBoxGroup_0.setCheckState(QtCore.Qt.Checked)
         dialog.ui.spinBoxGroup_0.setValue(1)
         dialog.ui.checkBoxGroup_1.setCheckState(QtCore.Qt.Checked)
-        dialog.ui.spinBoxGroup_1.setValue(2)
+        dialog.ui.spinBoxGroup_1.setValue(1)
 
         dialog.accept()
```

### Comparing `meggie-1.7.0/meggie/actions/evoked_info/__init__.py` & `meggie-1.8.0/meggie/actions/evoked_info/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/evoked_plot/__init__.py` & `meggie-1.8.0/meggie/actions/evoked_plot/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,12 +45,12 @@
 
         try:
             if params["output_option"] == "channel_averages":
                 plot_evoked_averages(evoked, params["channel_groups"])
             else:
                 chs = list(get_channels_by_type(info).keys())
                 if "eeg" in chs:
-                    plot_evoked_topo(evoked, ch_type="eeg")
+                    plot_evoked_topo(subject, evoked, ch_type="eeg")
                 if "grad" in chs or "mag" in chs:
-                    plot_evoked_topo(evoked, ch_type="meg")
+                    plot_evoked_topo(subject, evoked, ch_type="meg")
         except Exception as exc:
             exc_messagebox(self.window, exc)
```

### Comparing `meggie-1.7.0/meggie/actions/evoked_plot/controller/evoked.py` & `meggie-1.8.0/meggie/actions/evoked_plot/controller/evoked.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import matplotlib.pyplot as plt
 
 from matplotlib.lines import Line2D
 
 from meggie.utilities.plotting import color_cycle
 from meggie.utilities.plotting import create_channel_average_plot
 from meggie.utilities.channels import average_to_channel_groups
+from meggie.utilities.channels import ensure_montage
 from meggie.utilities.plotting import set_figure_title
 
 from meggie.utilities.units import get_unit
 
 
 def _create_averages(mne_evoked, channel_groups):
     mne_evoked = mne_evoked.copy().drop_channels(mne_evoked.info["bads"])
@@ -62,48 +63,52 @@
         title = " ".join([evoked.name, ch_type])
         legend = list(zip(conditions, colors))
         create_channel_average_plot(len(ch_groups), plot_fun, title, legend)
 
     plt.show()
 
 
-def plot_evoked_topo(evoked, ch_type):
+def plot_evoked_topo(subject, evoked, ch_type):
     """Plots evoked time courses arranged as a topography"""
     evokeds = []
     labels = []
-    for key, evok in sorted(evoked.content.items()):
+    for key, mne_evoked in sorted(evoked.content.items()):
 
-        info = evok.info
+        info = mne_evoked.info
         if ch_type == "eeg":
             dropped_names = [
                 ch_name
                 for ch_idx, ch_name in enumerate(info["ch_names"])
                 if ch_idx not in mne.pick_types(info, eeg=True, meg=False)
             ]
         else:
             dropped_names = [
                 ch_name
                 for ch_idx, ch_name in enumerate(info["ch_names"])
                 if ch_idx not in mne.pick_types(info, eeg=False, meg=True)
             ]
 
-        evok = evok.copy().drop_channels(dropped_names)
+        mne_evoked = mne_evoked.copy().drop_channels(dropped_names)
+
+        ensure_montage(subject, mne_evoked, ch_type)
+
+        evokeds.append(mne_evoked)
 
-        evokeds.append(evok)
         labels.append(key)
 
     colors = color_cycle(len(evoked.content.keys()))
 
     # setup legend for subplots
     lines = [
         Line2D([0], [0], color=colors[idx], label=labels[idx])
         for idx in range(len(labels))
     ]
 
     fig, axes = plt.subplots()
+
     mne.viz.plot_evoked_topo(evokeds, color=colors, legend=False, show=False, axes=axes)
     axes.legend(handles=lines, loc="upper right")
     title = "{0}_{1}".format(evoked.name, ch_type)
     set_figure_title(fig, title)
 
     def onclick(event):
         try:
```

### Comparing `meggie-1.7.0/meggie/actions/evoked_plot/tests/test_evoked_plot_all_channels.py` & `meggie-1.8.0/meggie/actions/tfr_plot_tse/tests/test_tfr_plot_tse_all_channels.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from meggie.utilities.testing import BaseTestAction
-from meggie.actions.evoked_plot import PlotEvoked
-from meggie.utilities.dialogs.outputOptionsMain import OutputOptions
+from meggie.actions.tfr_plot_tse import PlotTSE
+from meggie.utilities.dialogs.TFROutputOptionsMain import TFROutputOptions
 
 
-class TestEvokedPlotAllChannels(BaseTestAction):
-    def test_evoked_plot_all_channels(self):
+class TestTFRPlotTSEAllChannels(BaseTestAction):
+    def test_tfr_plot_tse_all_channels(self):
 
-        data = {"outputs": {"evoked": ["Evoked"]}}
+        data = {"outputs": {"tfr": ["TFR"]}}
 
         self.run_action(
-            action_name="evoked_plot",
-            handler=PlotEvoked,
+            action_name="tfr_plot_tse",
+            handler=PlotTSE,
             data=data,
-            patch_paths=["meggie.actions.evoked_plot"],
         )
-        dialog = self.find_dialog(OutputOptions)
+        dialog = self.find_dialog(TFROutputOptions)
         dialog.ui.radioButtonChannelAverages.setChecked(False)
         dialog.accept()
```

### Comparing `meggie-1.7.0/meggie/actions/evoked_plot/tests/test_evoked_plot_channel_averages.py` & `meggie-1.8.0/meggie/actions/evoked_plot/tests/test_evoked_plot_all_channels.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from meggie.utilities.testing import BaseTestAction
 from meggie.actions.evoked_plot import PlotEvoked
 from meggie.utilities.dialogs.outputOptionsMain import OutputOptions
 
 
-class TestEvokedPlotChannelAverages(BaseTestAction):
-    def test_evoked_plot_channel_averages(self):
+class TestEvokedPlotAllChannels(BaseTestAction):
+    def test_evoked_plot_all_channels(self):
 
         data = {"outputs": {"evoked": ["Evoked"]}}
 
         self.run_action(
             action_name="evoked_plot",
             handler=PlotEvoked,
             data=data,
-            patch_paths=["meggie.actions.evoked_plot"],
         )
         dialog = self.find_dialog(OutputOptions)
-        dialog.ui.radioButtonChannelAverages.setChecked(True)
+        dialog.ui.radioButtonChannelAverages.setChecked(False)
         dialog.accept()
```

### Comparing `meggie-1.7.0/meggie/actions/evoked_plot_topomap/__init__.py` & `meggie-1.8.0/meggie/actions/evoked_plot_topomap/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,16 +48,16 @@
         name = params["name"]
         tmin = params["tmin"]
         tmax = params["tmax"]
         step = params["step"]
         radius = params["radius"]
         evoked = subject.evoked.get(name)
 
-        for key, evok in sorted(evoked.content.items()):
-            channels = get_channels_by_type(evok.info)
+        for key, mne_evoked in sorted(evoked.content.items()):
+            channels = get_channels_by_type(mne_evoked.info)
             for ch_type in channels.keys():
                 title_elems = [name, key, ch_type]
                 times = np.arange(tmin, tmax, step)
 
                 # Use custom figure so that mne does not remove the mpl toolbar
                 fig = plt.figure()
                 axes = []
@@ -76,11 +76,11 @@
                 axes.append(fig.add_subplot(spec))
 
                 # until there is a good solution to topomap skirts, fix a value
                 sphere = None
                 if ch_type in ["mag", "grad"]:
                     sphere = radius
 
-                fig = evok.plot_topomap(
+                fig = mne_evoked.plot_topomap(
                     times=times, ch_type=ch_type, axes=axes, sphere=sphere
                 )
                 set_figure_title(fig, "_".join(title_elems))
```

### Comparing `meggie-1.7.0/meggie/actions/evoked_plot_topomap/dialogs/evokedTopomapDialogMain.py` & `meggie-1.8.0/meggie/actions/evoked_plot_topomap/dialogs/evokedTopomapDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/evoked_plot_topomap/dialogs/evokedTopomapDialogUi.py` & `meggie-1.8.0/meggie/actions/evoked_plot_topomap/dialogs/evokedTopomapDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/evoked_plot_topomap/tests/test_evoked_plot_topomap.py` & `meggie-1.8.0/meggie/actions/evoked_plot_topomap/tests/test_evoked_plot_topomap.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/evoked_save/__init__.py` & `meggie-1.8.0/meggie/actions/evoked_save/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/evoked_save/controller/evoked.py` & `meggie-1.8.0/meggie/actions/evoked_save/controller/evoked.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/evoked_save/tests/test_evoked_save_all_channels.py` & `meggie-1.8.0/meggie/actions/evoked_save/tests/test_evoked_save_all_channels.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,12 +8,11 @@
 
         data = {"outputs": {"evoked": ["Evoked"]}}
 
         self.run_action(
             action_name="evoked_save",
             handler=SaveEvoked,
             data=data,
-            patch_paths=["meggie.actions.evoked_save"],
         )
         dialog = self.find_dialog(OutputOptions)
         dialog.ui.radioButtonChannelAverages.setChecked(False)
         dialog.accept()
```

### Comparing `meggie-1.7.0/meggie/actions/evoked_save/tests/test_evoked_save_channel_averages.py` & `meggie-1.8.0/meggie/actions/evoked_save/tests/test_evoked_save_channel_averages.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,12 +8,11 @@
 
         data = {"outputs": {"evoked": ["Evoked"]}}
 
         self.run_action(
             action_name="evoked_save",
             handler=SaveEvoked,
             data=data,
-            patch_paths=["meggie.actions.evoked_save"],
         )
         dialog = self.find_dialog(OutputOptions)
         dialog.ui.radioButtonChannelAverages.setChecked(True)
         dialog.accept()
```

### Comparing `meggie-1.7.0/meggie/actions/raw_event_info/__init__.py` & `meggie-1.8.0/meggie/actions/raw_event_info/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/raw_events_from_annotations/__init__.py` & `meggie-1.8.0/meggie/actions/raw_events_from_annotations/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/raw_events_from_annotations/dialogs/eventsFromAnnotationsDialogMain.py` & `meggie-1.8.0/meggie/actions/raw_events_from_annotations/dialogs/eventsFromAnnotationsDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/raw_events_from_annotations/dialogs/eventsFromAnnotationsDialogUi.py` & `meggie-1.8.0/meggie/actions/raw_events_from_annotations/dialogs/eventsFromAnnotationsDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/raw_events_from_annotations/tests/test_raw_events_from_annotations.py` & `meggie-1.8.0/meggie/actions/raw_events_from_annotations/tests/test_raw_events_from_annotations.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/raw_filter/__init__.py` & `meggie-1.8.0/meggie/actions/raw_filter/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/raw_filter/controller/filter.py` & `meggie-1.8.0/meggie/actions/raw_filter/controller/filter.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/raw_filter/dialogs/filterDialogMain.py` & `meggie-1.8.0/meggie/actions/raw_filter/dialogs/filterDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/raw_filter/dialogs/filterDialogUi.py` & `meggie-1.8.0/meggie/actions/raw_filter/dialogs/filterDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/raw_ica/__init__.py` & `meggie-1.8.0/meggie/actions/raw_ica/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/raw_ica/controller/ica.py` & `meggie-1.8.0/meggie/actions/raw_ica/controller/ica.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/raw_ica/dialogs/icaDialogMain.py` & `meggie-1.8.0/meggie/actions/raw_ica/dialogs/icaDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/raw_ica/dialogs/icaDialogUi.py` & `meggie-1.8.0/meggie/actions/raw_ica/dialogs/icaDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/raw_ica/tests/test_raw_ica.py` & `meggie-1.8.0/meggie/actions/raw_ica/tests/test_raw_ica.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/raw_measurement_info/__init__.py` & `meggie-1.8.0/meggie/actions/raw_measurement_info/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             mi = MeasurementInfo(raw)
 
             maxfilter_applied = subject.sss_applied
             ica_applied = subject.ica_applied
             rereferenced = subject.rereferenced
 
             try:
-                eeg_montage_set = is_montage_set(raw, "eeg")
+                eeg_montage_set = is_montage_set(raw.info, "eeg")
             except Exception:
                 eeg_montage_set = False
 
             message += "Subject name: {0}\n".format(mi.subject_name)
             message += "Date: {0}\n".format(mi.date)
             message += "Length: {0:.2f} s\n".format(raw.times[-1])
             message += "Highpass: {0} Hz\n".format(mi.high_pass)
```

### Comparing `meggie-1.7.0/meggie/actions/raw_montage/__init__.py` & `meggie-1.8.0/meggie/actions/raw_montage/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,30 +19,32 @@
     @subject_action
     def handler(self, subject, params):
         """ """
 
         @threaded
         def montage_fun():
             """ """
-            raw = subject.get_raw()
-
             head_size = params["head_size"]
 
             if params["custom"] is True:
                 montage_fname = params["selection"]
                 montage = mne.channels.read_custom_montage(
                     montage_fname, head_size=head_size
                 )
             else:
                 montage_name = params["selection"]
                 montage = mne.channels.make_standard_montage(
                     montage_name, head_size=head_size
                 )
 
-            raw.set_montage(montage)
+            if subject.has_raw:
+                raw = subject.get_raw()
+                raw.set_montage(montage)
+
+            subject.save_montage(montage)
             subject.save()
 
         montage_fun(do_meanwhile=self.window.update_ui)
 
     def run(self):
         montage_dialog = MontageDialog(self.window, self.experiment, self.handler)
         montage_dialog.show()
```

### Comparing `meggie-1.7.0/meggie/actions/raw_montage/dialogs/montageDialogMain.py` & `meggie-1.8.0/meggie/actions/raw_montage/dialogs/montageDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/raw_montage/dialogs/montageDialogUi.py` & `meggie-1.8.0/meggie/actions/raw_montage/dialogs/montageDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/raw_montage/tests/test_raw_montage.py` & `meggie-1.8.0/meggie/actions/raw_montage/tests/test_raw_montage.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/raw_plot/__init__.py` & `meggie-1.8.0/meggie/actions/raw_plot/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/raw_plot_projections/__init__.py` & `meggie-1.8.0/meggie/actions/spectrum_delete_from_all/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,41 @@
-""" Contains implementation for raw plot projections
+""" Contains implementation for delete spectrum from all
 """
 
-from meggie.utilities.messaging import messagebox
+import logging
+
 from meggie.utilities.messaging import exc_messagebox
-from meggie.utilities.plotting import set_figure_title
 
 from meggie.mainwindow.dynamic import Action
 from meggie.mainwindow.dynamic import subject_action
 
 
-class PlotProjections(Action):
-    """Shows a plot of existing projection vectors."""
+class DeleteSpectrumFromAll(Action):
+    """Deletes spectrum of selected name from all subjects"""
 
     def run(self):
 
-        subject = self.experiment.active_subject
         try:
-            self.handler(subject, {})
+            selected_name = self.data["outputs"]["spectrum"][0]
+        except IndexError:
+            return
+
+        for subject in self.experiment.subjects.values():
+            if selected_name in subject.spectrum:
+                try:
+                    self.handler(subject, {"name": selected_name})
+                except Exception:
+                    logging.getLogger("ui_logger").exception("")
+                    logging.getLogger("ui_logger").warning(
+                        "Could not remove spectrum for " + subject.name
+                    )
+
+        try:
+            self.experiment.save_experiment_settings()
         except Exception as exc:
             exc_messagebox(self.window, exc)
 
+        self.window.initialize_ui()
+
     @subject_action
     def handler(self, subject, params):
-        raw = subject.get_raw()
-        if not raw.info["projs"]:
-            messagebox(self.window, "Data does not contain any projection vectors")
-            return
-        fig = raw.plot_projs_topomap()
-
-        elems = ["projections", subject.name]
-        set_figure_title(fig, "_".join(elems))
-        fig.suptitle(" ".join(elems))
+        subject.remove(params["name"], "spectrum")
```

### Comparing `meggie-1.7.0/meggie/actions/raw_rereference/__init__.py` & `meggie-1.8.0/meggie/actions/raw_rereference/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/raw_rereference/dialogs/rereferencingDialogMain.py` & `meggie-1.8.0/meggie/actions/raw_rereference/dialogs/rereferencingDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/raw_rereference/dialogs/rereferencingDialogUi.py` & `meggie-1.8.0/meggie/actions/raw_rereference/dialogs/rereferencingDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/raw_rereference/tests/test_raw_rereference.py` & `meggie-1.8.0/meggie/actions/raw_rereference/tests/test_raw_rereference.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/raw_resample/__init__.py` & `meggie-1.8.0/meggie/actions/raw_resample/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,11 +20,12 @@
 
     @subject_action
     def handler(self, subject, params):
         """ """
 
         @threaded
         def resample_fun():
-            subject.get_raw().resample(params["rate"])
+            raw = subject.get_raw()
+            raw.resample(params["rate"])
 
         resample_fun(do_meanwhile=self.window.update_ui)
         subject.save()
```

### Comparing `meggie-1.7.0/meggie/actions/raw_resample/dialogs/resamplingDialogMain.py` & `meggie-1.8.0/meggie/actions/raw_resample/dialogs/resamplingDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/raw_resample/dialogs/resamplingDialogUi.py` & `meggie-1.8.0/meggie/actions/raw_resample/dialogs/resamplingDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/raw_resample/tests/test_raw_resample.py` & `meggie-1.8.0/meggie/actions/raw_resample/tests/test_raw_resample.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/spectrum_create/__init__.py` & `meggie-1.8.0/meggie/actions/spectrum_create/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/spectrum_create/controller/spectrum.py` & `meggie-1.8.0/meggie/actions/spectrum_create/controller/spectrum.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from meggie.utilities.threading import threaded
 from meggie.utilities.events import get_raw_blocks_from_intervals
 
 
 @threaded
 def create_power_spectrum(subject, spectrum_name, intervals, fmin, fmax, nfft, overlap):
     """Creates a power spectrum item."""
+
     # get raw objects organized with average groups as keys
     ival_times, raw_block_groups = get_raw_blocks_from_intervals(subject, intervals)
 
     raw = subject.get_raw()
     picks = mne.pick_types(raw.info, meg=True, eeg=True, exclude="bads")
 
     # remove zero channels from picks
```

### Comparing `meggie-1.7.0/meggie/actions/spectrum_create/tests/test_spectrum_create.py` & `meggie-1.8.0/meggie/actions/spectrum_create/tests/test_spectrum_create.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/spectrum_delete/__init__.py` & `meggie-1.8.0/meggie/actions/spectrum_delete/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/spectrum_delete_from_all/__init__.py` & `meggie-1.8.0/meggie/actions/tfr_delete_from_all/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-""" Contains implementation for delete spectrum from all
+""" Contains implementation for delete tfr from all
 """
 
 import logging
 
 from meggie.utilities.messaging import exc_messagebox
 
 from meggie.mainwindow.dynamic import Action
 from meggie.mainwindow.dynamic import subject_action
 
 
-class DeleteSpectrumFromAll(Action):
-    """Deletes spectrum of selected name from all subjects"""
+class DeleteTFRFromAll(Action):
+    """Deletes TFR of selected name from all subjects"""
 
     def run(self):
 
         try:
-            selected_name = self.data["outputs"]["spectrum"][0]
+            selected_name = self.data["outputs"]["tfr"][0]
         except IndexError:
             return
 
         for subject in self.experiment.subjects.values():
-            if selected_name in subject.spectrum:
+            if selected_name in subject.tfr:
                 try:
                     self.handler(subject, {"name": selected_name})
                 except Exception:
                     logging.getLogger("ui_logger").exception("")
                     logging.getLogger("ui_logger").warning(
-                        "Could not remove spectrum for " + subject.name
+                        "Could not remove TFR for " + subject.name
                     )
 
         try:
             self.experiment.save_experiment_settings()
         except Exception as exc:
             exc_messagebox(self.window, exc)
 
         self.window.initialize_ui()
 
     @subject_action
     def handler(self, subject, params):
-        subject.remove(params["name"], "spectrum")
+        subject.remove(params["name"], "tfr")
```

### Comparing `meggie-1.7.0/meggie/actions/spectrum_group_average/__init__.py` & `meggie-1.8.0/meggie/actions/spectrum_group_average/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/spectrum_group_average/controller/spectrum.py` & `meggie-1.8.0/meggie/actions/spectrum_group_average/controller/spectrum.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/spectrum_group_average/tests/test_spectrum_group_average.py` & `meggie-1.8.0/meggie/actions/spectrum_group_average/tests/test_spectrum_group_average.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,17 +12,16 @@
 
         data = {"outputs": {"spectrum": ["Spectrum"]}}
 
         self.run_action(
             action_name="spectrum_group_average",
             handler=GroupAverage,
             data=data,
-            patch_paths=["meggie.actions.spectrum_group_average"],
         )
         dialog = self.find_dialog(GroupSelectionDialog)
 
         dialog.ui.checkBoxGroup_0.setCheckState(QtCore.Qt.Checked)
         dialog.ui.spinBoxGroup_0.setValue(1)
         dialog.ui.checkBoxGroup_1.setCheckState(QtCore.Qt.Checked)
-        dialog.ui.spinBoxGroup_1.setValue(2)
+        dialog.ui.spinBoxGroup_1.setValue(1)
 
         dialog.accept()
```

### Comparing `meggie-1.7.0/meggie/actions/spectrum_info/__init__.py` & `meggie-1.8.0/meggie/actions/spectrum_info/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/spectrum_plot/__init__.py` & `meggie-1.8.0/meggie/actions/spectrum_plot/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/spectrum_plot/controller/spectrum.py` & `meggie-1.8.0/meggie/actions/spectrum_plot/controller/spectrum.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import matplotlib.pyplot as plt
 
 from meggie.utilities.plotting import color_cycle
 from meggie.utilities.plotting import create_channel_average_plot
 from meggie.utilities.channels import average_to_channel_groups
 from meggie.utilities.channels import iterate_topography
 from meggie.utilities.channels import filter_info
+from meggie.utilities.channels import ensure_montage
 from meggie.utilities.plotting import set_figure_title
 from meggie.utilities.units import get_power_unit
 
 
 def plot_spectrum_averages(subject, channel_groups, name, log_transformed=True):
     """Plots spectrum averages."""
 
@@ -84,14 +85,16 @@
             ch_name
             for ch_idx, ch_name in enumerate(info["ch_names"])
             if ch_idx in mne.pick_types(info, eeg=True, meg=False)
         ]
 
     info = filter_info(info, picked_channels)
 
+    ensure_montage(subject, info, ch_type)
+
     colors = color_cycle(len(data))
 
     def individual_plot(ax, info_idx, names_idx):
         """ """
         ch_name = ch_names[names_idx]
         for color_idx, (key, psd) in enumerate(sorted(data.items())):
```

### Comparing `meggie-1.7.0/meggie/actions/spectrum_plot/tests/test_spectrum_plot_all_channels.py` & `meggie-1.8.0/meggie/actions/spectrum_plot/tests/test_spectrum_plot_all_channels.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,12 +8,11 @@
 
         data = {"outputs": {"spectrum": ["Spectrum"]}}
 
         self.run_action(
             action_name="spectrum_plot",
             handler=PlotSpectrum,
             data=data,
-            patch_paths=["meggie.actions.spectrum_plot"],
         )
         dialog = self.find_dialog(OutputOptions)
         dialog.ui.radioButtonChannelAverages.setChecked(False)
         dialog.accept()
```

### Comparing `meggie-1.7.0/meggie/actions/spectrum_plot/tests/test_spectrum_plot_channel_averages.py` & `meggie-1.8.0/meggie/actions/spectrum_save/tests/test_spectrum_save_channels_averages.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from meggie.utilities.testing import BaseTestAction
-from meggie.actions.spectrum_plot import PlotSpectrum
+from meggie.actions.spectrum_save import SaveSpectrum
 from meggie.utilities.dialogs.outputOptionsMain import OutputOptions
 
 
-class TestSpectrumPlotChannelAverages(BaseTestAction):
-    def test_spectrum_plot_channel_averages(self):
+class TestSpectrumSaveChannelAverages(BaseTestAction):
+    def test_spectrum_save_channel_averages(self):
 
         data = {"outputs": {"spectrum": ["Spectrum"]}}
 
         self.run_action(
-            action_name="spectrum_plot",
-            handler=PlotSpectrum,
+            action_name="spectrum_save",
+            handler=SaveSpectrum,
             data=data,
-            patch_paths=["meggie.actions.spectrum_plot"],
         )
         dialog = self.find_dialog(OutputOptions)
         dialog.ui.radioButtonChannelAverages.setChecked(True)
         dialog.accept()
```

### Comparing `meggie-1.7.0/meggie/actions/spectrum_save/__init__.py` & `meggie-1.8.0/meggie/actions/spectrum_save/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/spectrum_save/controller/spectrum.py` & `meggie-1.8.0/meggie/actions/spectrum_save/controller/spectrum.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/spectrum_save/tests/test_spectrum_save_all_channels.py` & `meggie-1.8.0/meggie/actions/spectrum_save/tests/test_spectrum_save_all_channels.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,12 +8,11 @@
 
         data = {"outputs": {"spectrum": ["Spectrum"]}}
 
         self.run_action(
             action_name="spectrum_save",
             handler=SaveSpectrum,
             data=data,
-            patch_paths=["meggie.actions.spectrum_save"],
         )
         dialog = self.find_dialog(OutputOptions)
         dialog.ui.radioButtonChannelAverages.setChecked(False)
         dialog.accept()
```

### Comparing `meggie-1.7.0/meggie/actions/spectrum_save/tests/test_spectrum_save_channels_averages.py` & `meggie-1.8.0/meggie/actions/tfr_plot/tests/test_tfr_plot_channel_averages.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from meggie.utilities.testing import BaseTestAction
-from meggie.actions.spectrum_save import SaveSpectrum
-from meggie.utilities.dialogs.outputOptionsMain import OutputOptions
+from meggie.actions.tfr_plot import PlotTFR
+from meggie.utilities.dialogs.TFROutputOptionsMain import TFROutputOptions
 
 
-class TestSpectrumSaveChannelAverages(BaseTestAction):
-    def test_spectrum_save_channel_averages(self):
+class TestTFRPlotChannelAverages(BaseTestAction):
+    def test_tfr_plot_channel_averages(self):
 
-        data = {"outputs": {"spectrum": ["Spectrum"]}}
+        data = {"outputs": {"tfr": ["TFR"]}}
 
         self.run_action(
-            action_name="spectrum_save",
-            handler=SaveSpectrum,
+            action_name="tfr_plot",
+            handler=PlotTFR,
             data=data,
-            patch_paths=["meggie.actions.spectrum_save"],
         )
-        dialog = self.find_dialog(OutputOptions)
+        dialog = self.find_dialog(TFROutputOptions)
         dialog.ui.radioButtonChannelAverages.setChecked(True)
         dialog.accept()
```

### Comparing `meggie-1.7.0/meggie/actions/tfr_create/__init__.py` & `meggie-1.8.0/meggie/actions/tfr_create/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,18 +17,15 @@
     def run(self):
 
         selected_names = self.data["inputs"]["epochs"]
 
         if not selected_names:
             return
 
-        if len(selected_names) == 1:
-            stem = selected_names[0]
-        else:
-            stem = "TFR"
+        stem = "TFR"
 
         default_name = next_available_name(
             self.experiment.active_subject.tfr.keys(), stem
         )
 
         dialog = TFRDialog(
             self.experiment, self.window, selected_names, default_name, self.handler
```

### Comparing `meggie-1.7.0/meggie/actions/tfr_create/controller/tfr.py` & `meggie-1.8.0/meggie/actions/tfr_create/controller/tfr.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/tfr_create/dialogs/TFRDialogMain.py` & `meggie-1.8.0/meggie/actions/tfr_create/dialogs/TFRDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/tfr_create/dialogs/TFRDialogUi.py` & `meggie-1.8.0/meggie/actions/tfr_create/dialogs/TFRDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/tfr_create/tests/test_tfr_create.py` & `meggie-1.8.0/meggie/actions/tfr_create/tests/test_tfr_create.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/tfr_delete/__init__.py` & `meggie-1.8.0/meggie/actions/tfr_delete/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/tfr_group_average/__init__.py` & `meggie-1.8.0/meggie/actions/tfr_group_average/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/tfr_group_average/controller/tfr.py` & `meggie-1.8.0/meggie/actions/tfr_group_average/controller/tfr.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,18 +71,19 @@
                 continue
 
             for tfr_item_key, tfr_item in meggie_tfr.content.items():
                 grand_key = (group_key, tfr_item_key)
 
                 # get common channels in "subject specific space"
                 subject_ch_names = tfr_item.info["ch_names"]
-                for ch_idx, ch_name in enumerate(clean_names(subject_ch_names)):
-                    drop_names = []
-                    if ch_name not in common_ch_names:
-                        drop_names.append(subject_ch_names[ch_idx])
+                drop_names = [
+                    name
+                    for idx, name in enumerate(clean_names(subject_ch_names))
+                    if name not in common_ch_names
+                ]
                 tfr_item = tfr_item.copy().drop_channels(drop_names)
 
                 # sanity check
                 if len(tfr_item.info["ch_names"]) != len(common_ch_names):
                     raise Exception("Something wrong with the channels")
 
                 if grand_key in grand_tfrs:
```

### Comparing `meggie-1.7.0/meggie/actions/tfr_group_average/tests/test_tfr_group_average.py` & `meggie-1.8.0/meggie/actions/tfr_group_average/tests/test_tfr_group_average.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,17 +12,16 @@
 
         data = {"outputs": {"tfr": ["TFR"]}}
 
         self.run_action(
             action_name="tfr_group_average",
             handler=GroupAverage,
             data=data,
-            patch_paths=["meggie.actions.tfr_group_average"],
         )
         dialog = self.find_dialog(GroupSelectionDialog)
 
         dialog.ui.checkBoxGroup_0.setCheckState(QtCore.Qt.Checked)
         dialog.ui.spinBoxGroup_0.setValue(1)
         dialog.ui.checkBoxGroup_1.setCheckState(QtCore.Qt.Checked)
-        dialog.ui.spinBoxGroup_1.setValue(2)
+        dialog.ui.spinBoxGroup_1.setValue(1)
 
         dialog.accept()
```

### Comparing `meggie-1.7.0/meggie/actions/tfr_info/__init__.py` & `meggie-1.8.0/meggie/actions/tfr_info/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/tfr_plot/__init__.py` & `meggie-1.8.0/meggie/actions/tfr_plot/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/tfr_plot/controller/tfr.py` & `meggie-1.8.0/meggie/actions/tfr_plot/controller/tfr.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import numpy as np
 import matplotlib.pyplot as plt
 import mne
 
 from meggie.utilities.plotting import create_channel_average_plot
 from meggie.utilities.channels import average_to_channel_groups
+from meggie.utilities.channels import ensure_montage
 from meggie.utilities.plotting import set_figure_title
 
 
 def plot_tfr_averages(
     subject,
     tfr_name,
     tfr_condition,
@@ -135,14 +136,16 @@
         ]
 
     tfr = tfr.copy().drop_channels(dropped_names)
 
     # apply baseline here to get better vmin and vmax values
     tfr.apply_baseline(baseline=bline, mode=mode)
 
+    ensure_montage(subject, tfr, ch_type)
+
     values = tfr.data.flatten()
     vmax = np.percentile(np.abs(values), 99)
     vmin = -vmax
 
     title = "{0}_{1}_{2}".format(tfr_name, tfr_condition, ch_type)
     fig = tfr.plot_topo(
         show=False,
```

### Comparing `meggie-1.7.0/meggie/actions/tfr_plot/tests/test_tfr_plot_all_channels.py` & `meggie-1.8.0/meggie/actions/tfr_plot/tests/test_tfr_plot_all_channels.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,12 +8,11 @@
 
         data = {"outputs": {"tfr": ["TFR"]}}
 
         self.run_action(
             action_name="tfr_plot",
             handler=PlotTFR,
             data=data,
-            patch_paths=["meggie.actions.tfr_plot"],
         )
         dialog = self.find_dialog(TFROutputOptions)
         dialog.ui.radioButtonChannelAverages.setChecked(False)
         dialog.accept()
```

### Comparing `meggie-1.7.0/meggie/actions/tfr_plot/tests/test_tfr_plot_channel_averages.py` & `meggie-1.8.0/meggie/actions/tfr_plot_tse/tests/test_tfr_plot_tse_channel_averages.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from meggie.utilities.testing import BaseTestAction
-from meggie.actions.tfr_plot import PlotTFR
+from meggie.actions.tfr_plot_tse import PlotTSE
 from meggie.utilities.dialogs.TFROutputOptionsMain import TFROutputOptions
 
 
-class TestTFRPlotChannelAverages(BaseTestAction):
-    def test_tfr_plot_channel_averages(self):
+class TestTFRPlotTSEChannelAverages(BaseTestAction):
+    def test_tfr_plot_tse_channel_averages(self):
 
         data = {"outputs": {"tfr": ["TFR"]}}
 
         self.run_action(
-            action_name="tfr_plot",
-            handler=PlotTFR,
+            action_name="tfr_plot_tse",
+            handler=PlotTSE,
             data=data,
-            patch_paths=["meggie.actions.tfr_plot"],
         )
         dialog = self.find_dialog(TFROutputOptions)
         dialog.ui.radioButtonChannelAverages.setChecked(True)
         dialog.accept()
```

### Comparing `meggie-1.7.0/meggie/actions/tfr_plot_tse/__init__.py` & `meggie-1.8.0/meggie/actions/tfr_plot_tse/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/tfr_plot_tse/controller/tfr.py` & `meggie-1.8.0/meggie/actions/tfr_plot_tse/controller/tfr.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from meggie.utilities.plotting import color_cycle
 from meggie.utilities.plotting import create_channel_average_plot
 from meggie.utilities.plotting import set_figure_title
 from meggie.utilities.channels import average_to_channel_groups
 from meggie.utilities.channels import iterate_topography
 from meggie.utilities.channels import filter_info
+from meggie.utilities.channels import ensure_montage
 from meggie.utilities.units import get_power_unit
 
 
 def _compute_tse(meggie_tfr, fmin, fmax):
     tfrs = meggie_tfr.content
 
     fmin_idx = np.where(meggie_tfr.freqs >= fmin)[0][0]
@@ -71,14 +72,16 @@
             ch_name
             for ch_idx, ch_name in enumerate(info["ch_names"])
             if ch_idx in mne.pick_types(info, meg=False, eeg=True)
         ]
 
     info = filter_info(info, picked_channels)
 
+    ensure_montage(subject, info, ch_type)
+
     ch_names = meggie_tfr.ch_names
     colors = color_cycle(len(tses))
 
     def individual_plot(ax, info_idx, names_idx):
         """ """
         ch_name = ch_names[names_idx]
```

### Comparing `meggie-1.7.0/meggie/actions/tfr_plot_tse/tests/test_tfr_plot_tse_all_channels.py` & `meggie-1.8.0/meggie/actions/tfr_save_tse/tests/test_tfr_save_tse_channel_averages.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from meggie.utilities.testing import BaseTestAction
-from meggie.actions.tfr_plot_tse import PlotTSE
+from meggie.actions.tfr_save_tse import SaveTSE
 from meggie.utilities.dialogs.TFROutputOptionsMain import TFROutputOptions
 
 
-class TestTFRPlotTSEAllChannels(BaseTestAction):
-    def test_tfr_plot_tse_all_channels(self):
+class TestTFRSaveTSEChannelAverages(BaseTestAction):
+    def test_tfr_save_tse_channel_averages(self):
 
         data = {"outputs": {"tfr": ["TFR"]}}
 
         self.run_action(
-            action_name="tfr_plot_tse",
-            handler=PlotTSE,
+            action_name="tfr_save_tse",
+            handler=SaveTSE,
             data=data,
-            patch_paths=["meggie.actions.tfr_plot_tse"],
         )
         dialog = self.find_dialog(TFROutputOptions)
-        dialog.ui.radioButtonChannelAverages.setChecked(False)
+        dialog.ui.radioButtonChannelAverages.setChecked(True)
         dialog.accept()
```

### Comparing `meggie-1.7.0/meggie/actions/tfr_plot_tse/tests/test_tfr_plot_tse_channel_averages.py` & `meggie-1.8.0/meggie/actions/tfr_save/tests/test_tfr_save_channel_averages.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from meggie.utilities.testing import BaseTestAction
-from meggie.actions.tfr_plot_tse import PlotTSE
+from meggie.actions.tfr_save import SaveTFR
 from meggie.utilities.dialogs.TFROutputOptionsMain import TFROutputOptions
 
 
-class TestTFRPlotTSEChannelAverages(BaseTestAction):
-    def test_tfr_plot_tse_channel_averages(self):
+class TestTFRSaveChannelAverages(BaseTestAction):
+    def test_tfr_save_channel_averages(self):
 
         data = {"outputs": {"tfr": ["TFR"]}}
 
         self.run_action(
-            action_name="tfr_plot_tse",
-            handler=PlotTSE,
+            action_name="tfr_save",
+            handler=SaveTFR,
             data=data,
-            patch_paths=["meggie.actions.tfr_plot_tse"],
         )
         dialog = self.find_dialog(TFROutputOptions)
         dialog.ui.radioButtonChannelAverages.setChecked(True)
         dialog.accept()
```

### Comparing `meggie-1.7.0/meggie/actions/tfr_save/__init__.py` & `meggie-1.8.0/meggie/actions/tfr_save/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/tfr_save/controller/tfr.py` & `meggie-1.8.0/meggie/actions/tfr_save/controller/tfr.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/tfr_save/tests/test_tfr_save_all_channels.py` & `meggie-1.8.0/meggie/actions/tfr_save/tests/test_tfr_save_all_channels.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,12 +8,11 @@
 
         data = {"outputs": {"tfr": ["TFR"]}}
 
         self.run_action(
             action_name="tfr_save",
             handler=SaveTFR,
             data=data,
-            patch_paths=["meggie.actions.tfr_save"],
         )
         dialog = self.find_dialog(TFROutputOptions)
         dialog.ui.radioButtonChannelAverages.setChecked(False)
         dialog.accept()
```

### Comparing `meggie-1.7.0/meggie/actions/tfr_save_tse/__init__.py` & `meggie-1.8.0/meggie/actions/tfr_save_tse/__init__.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/tfr_save_tse/controller/tfr.py` & `meggie-1.8.0/meggie/actions/tfr_save_tse/controller/tfr.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/actions/tfr_save_tse/tests/test_tfr_save_tse_all_channels.py` & `meggie-1.8.0/meggie/actions/tfr_save_tse/tests/test_tfr_save_tse_all_channels.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,12 +8,11 @@
 
         data = {"outputs": {"tfr": ["TFR"]}}
 
         self.run_action(
             action_name="tfr_save_tse",
             handler=SaveTSE,
             data=data,
-            patch_paths=["meggie.actions.tfr_save_tse"],
         )
         dialog = self.find_dialog(TFROutputOptions)
         dialog.ui.radioButtonChannelAverages.setChecked(False)
         dialog.accept()
```

### Comparing `meggie-1.7.0/meggie/configuration.json` & `meggie-1.8.0/meggie/configuration.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222223%*

 * *Differences: {"'pipelines'": "{0: {'name': 'Continuous data analysis'}, 1: {'name': 'Evoked response "*

 * *                "analysis'}, 2: {'name': 'Induced response analysis'}}"}*

```diff
@@ -3,33 +3,33 @@
     "pipelines": [
         {
             "id": "spectrum_sensor",
             "include_tabs": [
                 "preprocessing",
                 "spectrum"
             ],
-            "name": "Sensor-level continuous data analysis"
+            "name": "Continuous data analysis"
         },
         {
             "id": "evoked_sensor",
             "include_tabs": [
                 "preprocessing",
                 "epochs",
                 "evoked"
             ],
-            "name": "Sensor-level evoked response analysis"
+            "name": "Evoked response analysis"
         },
         {
             "id": "induced_sensor",
             "include_tabs": [
                 "preprocessing",
                 "epochs",
                 "tfr"
             ],
-            "name": "Sensor-level induced response analysis"
+            "name": "Induced response analysis"
         }
     ],
     "tabs": [
         {
             "id": "preprocessing",
             "info": [
                 "raw_measurement_info",
```

### Comparing `meggie-1.7.0/meggie/datatypes/epochs/epochs.py` & `meggie-1.8.0/meggie/datatypes/epochs/epochs.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,14 +56,19 @@
         return len(self.content.events)
 
     @property
     def params(self):
         """Returns additional information stored."""
         return self._params
 
+    @property
+    def info(self):
+        """Returns info."""
+        return self.content.info
+
     def delete_content(self):
         """Deletes the fif file from the files system"""
         os.remove(self._path)
 
     def save_content(self):
         """Saves the mne.Epochs to a fif file in the epochs
         directory"""
```

### Comparing `meggie-1.7.0/meggie/datatypes/epochs/tests/test_epochs.py` & `meggie-1.8.0/meggie/datatypes/epochs/tests/test_epochs.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/datatypes/evoked/evoked.py` & `meggie-1.8.0/meggie/datatypes/evoked/evoked.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/datatypes/evoked/tests/test_evoked.py` & `meggie-1.8.0/meggie/datatypes/evoked/tests/test_evoked.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/datatypes/spectrum/spectrum.py` & `meggie-1.8.0/meggie/datatypes/spectrum/spectrum.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/datatypes/spectrum/tests/test_spectrum.py` & `meggie-1.8.0/meggie/datatypes/spectrum/tests/test_spectrum.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/datatypes/tfr/tests/test_tfr.py` & `meggie-1.8.0/meggie/datatypes/tfr/tests/test_tfr.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/datatypes/tfr/tfr.py` & `meggie-1.8.0/meggie/datatypes/tfr/tfr.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,17 +45,17 @@
 
         fname = os.path.join(self._directory, name)
         return fname
 
     def save_content(self):
         """Saves the mne.AverageTFR to h5 files in the tfr directory."""
         try:
-            for tfr_name, tfr in self._content.items():
+            for tfr_name, mne_tfr in self._content.items():
                 fname = self._get_fname(tfr_name)
-                tfr.save(fname, overwrite=True)
+                mne_tfr.save(fname, overwrite=True)
         except Exception:
             raise Exception(
                 "Writing TFRs failed. Please ensure that the "
                 "entire experiment folder has write permissions."
             )
 
     def delete_content(self):
```

### Comparing `meggie-1.7.0/meggie/experiment.py` & `meggie-1.8.0/meggie/experiment.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import pkg_resources
 
 from meggie.subject import Subject
 
 from meggie.utilities.filemanager import open_raw
 from meggie.utilities.filemanager import save_raw
 from meggie.utilities.channels import get_default_channel_groups
+from meggie.utilities.channels import find_montage_info
 from meggie.utilities.validators import validate_name
 from meggie.utilities.uid import generate_uid
 
 from meggie.mainwindow.dynamic import find_all_datatype_specs
 
 
 class Experiment:
@@ -77,31 +78,34 @@
         self._author = validate_name(author, minlength=0, fieldname="author")
 
     @property
     def channel_groups(self):
         """Returns channel groups for experiment. If not set,
         uses defaults."""
         channel_groups = self._channel_groups.copy()
+        specs = find_all_datatype_specs()
 
-        # if channel groups not found, use defaults..
+        # if channel groups not found, look for defaults..
         if not channel_groups.get("eeg"):
             if self.active_subject:
-                raw = self.active_subject.get_raw(preload=False)
-                try:
-                    channel_groups["eeg"] = get_default_channel_groups(raw, "eeg")
-                except Exception:
-                    pass
+                info = find_montage_info(self.active_subject, specs.keys(), "eeg")
+                if info:
+                    try:
+                        channel_groups["eeg"] = get_default_channel_groups(info, "eeg")
+                    except Exception:
+                        pass
 
         if not channel_groups.get("meg"):
             if self.active_subject:
-                raw = self.active_subject.get_raw(preload=False)
-                try:
-                    channel_groups["meg"] = get_default_channel_groups(raw, "meg")
-                except Exception:
-                    pass
+                info = find_montage_info(self.active_subject, specs.keys(), "meg")
+                if info:
+                    try:
+                        channel_groups["meg"] = get_default_channel_groups(info, "meg")
+                    except Exception:
+                        pass
 
         return channel_groups
 
     @channel_groups.setter
     def channel_groups(self, channel_groups):
         """Sets the channel groups."""
         self._channel_groups = channel_groups
@@ -180,56 +184,73 @@
         # remove raw files from memory before activating new subject.
         if self.active_subject:
             self.active_subject.release_memory()
 
         self.active_subject = self.subjects[subject_name]
 
         # test validity
-        self.active_subject.get_raw(preload=False)
+        if self.active_subject.has_raw:
+            self.active_subject.get_raw(preload=False)
 
         return self.active_subject
 
     def create_subject(self, subject_name, raw_path):
         """Creates a subject object and copies the raw file
         inside it (by reading and saving).
 
         Parameters
         ----------
         subject_name : str
             Name of the new subject.
-        raw_path : str
+        raw_path : str | None
             Path to the data file.
+
+        Returns
+        -------
+        meggie.subject.Subject
+            The activated subject.
+
         """
-        bname = os.path.basename(raw_path)
-        stem, ext = os.path.splitext(bname)
-        new_fname = stem + ".fif"
 
         uid = generate_uid()
 
-        subject = Subject(self, subject_name, new_fname, uid)
-        subject.ensure_folders()
+        # it is possible to add "placeholder" subjects with only e.g epochs data
+        if raw_path:
+            bname = os.path.basename(raw_path)
+            stem, ext = os.path.splitext(bname)
+            new_fname = stem + ".fif"
+
+            subject = Subject(self, subject_name, new_fname, uid)
+            subject.ensure_folders()
 
-        raw = open_raw(raw_path)
+            raw = open_raw(raw_path)
 
-        new_path = os.path.join(subject.path, new_fname)
-        save_raw(raw, new_path)
+            new_path = os.path.join(subject.path, new_fname)
+            save_raw(raw, new_path)
+
+        else:
+            subject = Subject(self, subject_name, "", uid)
+
+        subject.ensure_folders()
 
         self.add_subject(subject)
 
+        return subject
+
     def save_experiment_settings(self):
         """
         Saves the experiment settings into a file in the root of
         the experiment directory structure.
         """
         subjects = []
 
         for subject in self.subjects.values():
             subject_dict = {
                 "subject_name": subject.name,
-                "raw_fname": subject.raw_fname,
+                "raw_fname": subject.raw_fname if subject.raw_fname else "",
                 "uid": subject.uid,
                 "ica_applied": subject.ica_applied,
                 "rereferenced": subject.rereferenced,
             }
 
             datatype_specs = find_all_datatype_specs()
 
@@ -397,19 +418,18 @@
         return experiment
 
     for subject_data in data["subjects"]:
 
         subject_name = subject_data["subject_name"]
 
         raw_fname = subject_data.get("raw_fname")
+
         # for backwards compatibility
         if not raw_fname:
             raw_fname = subject_data.get("working_file_name")
-        if not raw_fname:
-            raise Exception("raw_fname not set in the exp file")
 
         uid = subject_data.get("uid")
         if not uid:
             uid = generate_uid()
             experiment_updated = True
 
         subject = Subject(
```

### Comparing `meggie-1.7.0/meggie/mainWindowMain.py` & `meggie-1.8.0/meggie/mainWindowMain.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,26 +269,35 @@
     def update_ui(self):
         """Used for keeping the ui responsive when threading."""
         QApplication.processEvents()
 
     def reconstruct_tabs(self):
         """Reconstructs the tabs."""
 
-        if self.experiment and self.experiment.active_subject:
-            include_eeg = self.experiment.active_subject.has_eeg
-        else:
-            include_eeg = True
+        include_eeg = True
+        has_raw = True
+        if self.experiment:
+            active_subject = self.experiment.active_subject
+            if active_subject:
+                has_raw = active_subject.has_raw
+                if has_raw:
+                    include_eeg = active_subject.has_eeg
 
         if self.experiment:
             selected_pipeline = self.experiment.selected_pipeline
         else:
             selected_pipeline = "classic"
+
         try:
             self.tabs = construct_tabs(
-                selected_pipeline, self, self.prefs, include_eeg=include_eeg
+                selected_pipeline,
+                self,
+                self.prefs,
+                include_eeg=include_eeg,
+                has_raw=has_raw,
             )
         except Exception as exc:
             self.tabs = []
             exc_messagebox(self, exc)
 
     def initialize_ui(self):
         """Initializes the main window UI view.
```

### Comparing `meggie-1.7.0/meggie/mainWindowUi.py` & `meggie-1.8.0/meggie/mainWindowUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/mainwindow/dialogs/aboutDialogMain.py` & `meggie-1.8.0/meggie/mainwindow/dialogs/aboutDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/mainwindow/dialogs/aboutDialogUi.py` & `meggie-1.8.0/meggie/mainwindow/dialogs/aboutDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/mainwindow/dialogs/actionDialogMain.py` & `meggie-1.8.0/meggie/mainwindow/dialogs/actionDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/mainwindow/dialogs/actionDialogUi.py` & `meggie-1.8.0/meggie/mainwindow/dialogs/actionDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/mainwindow/dialogs/activePluginsDialogMain.py` & `meggie-1.8.0/meggie/mainwindow/dialogs/activePluginsDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/mainwindow/dialogs/activePluginsDialogUi.py` & `meggie-1.8.0/meggie/mainwindow/dialogs/activePluginsDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/mainwindow/dialogs/addSubjectDialogMain.py` & `meggie-1.8.0/meggie/mainwindow/dialogs/addSubjectDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/mainwindow/dialogs/addSubjectDialogUi.py` & `meggie-1.8.0/meggie/mainwindow/dialogs/addSubjectDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/mainwindow/dialogs/channelGroupsDialogMain.py` & `meggie-1.8.0/meggie/mainwindow/dialogs/channelGroupsDialogMain.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 
 from meggie.utilities.messaging import messagebox
 from meggie.utilities.messaging import exc_messagebox
 from meggie.utilities.channels import get_default_channel_groups
 from meggie.utilities.channels import get_triplet_from_mag
+from meggie.utilities.channels import find_montage_info
+from meggie.mainwindow.dynamic import find_all_datatype_specs
 
 from meggie.mainwindow.dialogs.channelGroupsDialogUi import Ui_channelGroupsDialog
 
 
 class ChannelGroupsDialog(QtWidgets.QDialog):
     """Contains the the logic for channel groups dialog."""
 
@@ -89,25 +91,26 @@
             return
 
         subject = self.parent.experiment.active_subject
         if not subject:
             messagebox(self.parent, "To reset, active subject is needed")
             return
 
-        raw = subject.get_raw()
+        specs = find_all_datatype_specs()
 
         if self.ui.radioButtonEEG.isChecked():
-            self.eeg_channel_groups = get_default_channel_groups(raw, "eeg")
+            info = find_montage_info(subject, specs.keys(), "eeg")
+            self.eeg_channel_groups = get_default_channel_groups(info, "eeg")
             self.ui.listWidgetChannelGroups.clear()
             for ch_name in sorted(self.eeg_channel_groups.keys()):
                 self.ui.listWidgetChannelGroups.addItem(ch_name)
 
         else:
-            meg_defaults = get_default_channel_groups(raw, "meg")
-            self.meg_channel_groups = meg_defaults
+            info = find_montage_info(subject, specs.keys(), "meg")
+            self.meg_channel_groups = get_default_channel_groups(info, "meg")
             self.ui.listWidgetChannelGroups.clear()
             for ch_name in sorted(self.meg_channel_groups.keys()):
                 self.ui.listWidgetChannelGroups.addItem(ch_name)
 
     def on_pushButtonSetChannels_clicked(self, checked=None):
         if checked is None:
             return
@@ -119,65 +122,67 @@
 
         try:
             selected_item = self.ui.listWidgetChannelGroups.selectedItems()[0]
         except IndexError:
             messagebox(self.parent, "Select a channel group first")
             return
 
-        raw = subject.get_raw()
+        specs = find_all_datatype_specs()
 
         if self.ui.radioButtonEEG.isChecked():
-            if mne.pick_types(raw.info, meg=False, eeg=True).size == 0:
+            info = find_montage_info(subject, specs.keys(), "eeg")
+            if mne.pick_types(info, meg=False, eeg=True).size == 0:
                 messagebox(self.parent, "No EEG channels found")
                 return
 
             ch_names = self.eeg_channel_groups[selected_item.text()]
             try:
-                ch_idxs = [raw.info["ch_names"].index(ch_name) for ch_name in ch_names]
+                ch_idxs = [info["ch_names"].index(ch_name) for ch_name in ch_names]
             except ValueError:
                 messagebox(
                     self.parent,
                     "Channel names in the group " "and the current subject don't match",
                 )
                 return
 
             ch_groups = [[], ch_idxs]
 
             try:
                 fig, selection = mne.viz.plot_sensors(
-                    raw.info,
+                    info,
                     kind="select",
                     ch_type="eeg",
                     ch_groups=ch_groups,
                     show=False,
                     title="Group channels",
                 )
             except RuntimeError:
                 messagebox(self.parent, "Could not plot sensors. Is the montage set?")
                 return
 
         else:
-            if mne.pick_types(raw.info, meg=True, eeg=False).size == 0:
+            info = find_montage_info(subject, specs.keys(), "meg")
+            if mne.pick_types(info, meg=True, eeg=False).size == 0:
                 messagebox(self.parent, "No MEG channels found")
                 return
 
             ch_names = self.meg_channel_groups[selected_item.text()]
             try:
-                ch_idxs = [raw.info["ch_names"].index(ch_name) for ch_name in ch_names]
+                ch_idxs = [info["ch_names"].index(ch_name) for ch_name in ch_names]
             except ValueError:
                 messagebox(
                     self.parent,
                     "Channel names in the group " "and the current subject don't match",
                 )
                 return
 
             ch_groups = [[], ch_idxs]
 
             fig, selection = mne.viz.plot_sensors(
-                raw.info,
+                info,
                 kind="select",
                 ch_type="mag",
                 ch_groups=ch_groups,
                 show=False,
                 title="Group channels",
             )
```

### Comparing `meggie-1.7.0/meggie/mainwindow/dialogs/channelGroupsDialogUi.py` & `meggie-1.8.0/meggie/mainwindow/dialogs/channelGroupsDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/mainwindow/dialogs/createExperimentDialogMain.py` & `meggie-1.8.0/meggie/mainwindow/dialogs/pipelineDialogMain.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,97 +1,89 @@
-""" Contains a class for logic of experiment creation dialog.
+""" Contains a class for logic of pipeline dialog.
 """
 
 from PyQt5 import QtWidgets
 
-from meggie.mainwindow.dialogs.createExperimentDialogUi import Ui_CreateExperimentDialog
-
-from meggie.experiment import initialize_new_experiment
-
 from meggie.mainwindow.dynamic import find_all_package_specs
 
+from meggie.mainwindow.dialogs.pipelineDialogUi import Ui_pipelineDialog
+
 from meggie.utilities.messaging import exc_messagebox
-from meggie.utilities.messaging import messagebox
 
 
-class CreateExperimentDialog(QtWidgets.QDialog):
-    """Contains logic for experiment creation dialog."""
+class PipelineDialog(QtWidgets.QDialog):
+    """Contains logic for pipeline dialog."""
 
-    def __init__(self, parent):
+    def __init__(self, parent, prefs):
         QtWidgets.QDialog.__init__(self, parent)
-
-        self.ui = Ui_CreateExperimentDialog()
+        self.ui = Ui_pipelineDialog()
         self.ui.setupUi(self)
 
         self.parent = parent
-        prefs = parent.prefs
+        self.experiment = parent.experiment
+
+        # Read selected pipeline from the experiment
+        selected_pipeline = self.experiment.selected_pipeline
 
         self.active_plugins = prefs.active_plugins
 
         # read all pipeline ids and names to a list
         pipelines = []
         package_specs = find_all_package_specs()
 
         for source, package_spec in package_specs.items():
-
             if source == "meggie" or source in self.active_plugins:
+
                 if "pipelines" in package_spec:
                     for pipeline in package_spec["pipelines"]:
                         try:
                             id_ = pipeline["id"]
                         except Exception:
                             raise Exception("Every pipeline should have id.")
 
                         name = pipeline.get("name", "")
                         pipelines.append((id_, name))
 
-        # Add classic
         pipelines.append(("classic", "Include everything"))
 
         self.pipelines = pipelines
 
-        # Create buttons for pipelines
+        # create buttons for pipelines
         self.pipeline_buttons = []
         for idx, (pipeline_id, pipeline_name) in enumerate(self.pipelines):
             radio_button = QtWidgets.QRadioButton(self.ui.groupBoxPipeline)
             radio_button.setText(pipeline_name)
 
             self.ui.gridLayoutPipeline.addWidget(radio_button, idx + 1, 0, 1, 1)
 
             self.pipeline_buttons.append(radio_button)
 
-            if idx == 0:
+            if selected_pipeline == pipeline_id:
                 radio_button.setChecked(True)
 
         if len(self.pipeline_buttons) == 1:
             self.pipeline_buttons[0].setEnabled(False)
             self.pipeline_buttons[0].setChecked(True)
 
     def accept(self):
-        if self.ui.lineEditExperimentName.text() == "":
-            message = "Give experiment a name."
-            messagebox(self.parent, message)
-            return
 
         selected_pipeline = ""
         for button_idx, radio_button in enumerate(self.pipeline_buttons):
             if radio_button.isChecked():
                 selected_pipeline = self.pipelines[button_idx][0]
                 break
 
-        try:
-            experiment = initialize_new_experiment(
-                self.ui.lineEditExperimentName.text(),
-                self.ui.lineEditAuthor.text(),
-                self.parent.prefs,
-            )
+        # store selected pipeline to the experiment
+        if not selected_pipeline:
+            return
 
-            experiment.selected_pipeline = selected_pipeline
-            experiment.save_experiment_settings()
+        try:
+            self.experiment.selected_pipeline = selected_pipeline
+            self.experiment.save_experiment_settings()
         except Exception as exc:
             exc_messagebox(self, exc)
             return
 
-        self.parent.experiment = experiment
         self.parent.reconstruct_tabs()
         self.parent.initialize_ui()
+
         self.close()
```

### Comparing `meggie-1.7.0/meggie/mainwindow/dialogs/createExperimentDialogUi.py` & `meggie-1.8.0/meggie/mainwindow/dialogs/preferencesDialogUi.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,95 +1,108 @@
 # -*- coding: utf-8 -*-
 
-# Form implementation generated from reading ui file 'createExperimentDialogUi.ui'
+# Form implementation generated from reading ui file 'preferencesDialogUi.ui'
 #
 # Created by: PyQt5 UI code generator 5.12.3
 #
 # WARNING! All changes made in this file will be lost!
 
 
 from PyQt5 import QtCore, QtWidgets
 
 
-class Ui_CreateExperimentDialog(object):
-    def setupUi(self, CreateExperimentDialog):
-        CreateExperimentDialog.setObjectName("CreateExperimentDialog")
-        CreateExperimentDialog.setWindowModality(QtCore.Qt.WindowModal)
-        CreateExperimentDialog.resize(506, 373)
-        self.gridLayout_3 = QtWidgets.QGridLayout(CreateExperimentDialog)
+class Ui_DialogPreferences(object):
+    def setupUi(self, DialogPreferences):
+        DialogPreferences.setObjectName("DialogPreferences")
+        DialogPreferences.resize(507, 482)
+        self.gridLayout_3 = QtWidgets.QGridLayout(DialogPreferences)
         self.gridLayout_3.setObjectName("gridLayout_3")
-        self.scrollArea = QtWidgets.QScrollArea(CreateExperimentDialog)
-        self.scrollArea.setFrameShape(QtWidgets.QFrame.NoFrame)
+        self.horizontalLayout_2 = QtWidgets.QHBoxLayout()
+        self.horizontalLayout_2.setObjectName("horizontalLayout_2")
+        spacerItem = QtWidgets.QSpacerItem(
+            40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum
+        )
+        self.horizontalLayout_2.addItem(spacerItem)
+        self.pushButtonCancel = QtWidgets.QPushButton(DialogPreferences)
+        self.pushButtonCancel.setObjectName("pushButtonCancel")
+        self.horizontalLayout_2.addWidget(self.pushButtonCancel)
+        self.pushButtonAccept = QtWidgets.QPushButton(DialogPreferences)
+        self.pushButtonAccept.setObjectName("pushButtonAccept")
+        self.horizontalLayout_2.addWidget(self.pushButtonAccept)
+        self.gridLayout_3.addLayout(self.horizontalLayout_2, 5, 0, 1, 1)
+        self.scrollArea = QtWidgets.QScrollArea(DialogPreferences)
         self.scrollArea.setWidgetResizable(True)
         self.scrollArea.setObjectName("scrollArea")
         self.scrollAreaWidgetContents = QtWidgets.QWidget()
-        self.scrollAreaWidgetContents.setGeometry(QtCore.QRect(0, 0, 488, 324))
-        self.scrollAreaWidgetContents.setMinimumSize(QtCore.QSize(0, 0))
+        self.scrollAreaWidgetContents.setGeometry(QtCore.QRect(0, 0, 487, 431))
         self.scrollAreaWidgetContents.setObjectName("scrollAreaWidgetContents")
-        self.gridLayout = QtWidgets.QGridLayout(self.scrollAreaWidgetContents)
-        self.gridLayout.setObjectName("gridLayout")
-        spacerItem = QtWidgets.QSpacerItem(
+        self.gridLayout_5 = QtWidgets.QGridLayout(self.scrollAreaWidgetContents)
+        self.gridLayout_5.setObjectName("gridLayout_5")
+        self.groupBoxMisc = QtWidgets.QGroupBox(self.scrollAreaWidgetContents)
+        self.groupBoxMisc.setObjectName("groupBoxMisc")
+        self.gridLayout_4 = QtWidgets.QGridLayout(self.groupBoxMisc)
+        self.gridLayout_4.setObjectName("gridLayout_4")
+        self.checkBoxAutomaticOpenPreviousExperiment = QtWidgets.QCheckBox(
+            self.groupBoxMisc
+        )
+        self.checkBoxAutomaticOpenPreviousExperiment.setObjectName(
+            "checkBoxAutomaticOpenPreviousExperiment"
+        )
+        self.gridLayout_4.addWidget(
+            self.checkBoxAutomaticOpenPreviousExperiment, 0, 0, 1, 1
+        )
+        self.gridLayout_5.addWidget(self.groupBoxMisc, 2, 0, 1, 1)
+        spacerItem1 = QtWidgets.QSpacerItem(
             20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding
         )
-        self.gridLayout.addItem(spacerItem, 2, 1, 1, 1)
-        self.groupBoxInfo = QtWidgets.QGroupBox(self.scrollAreaWidgetContents)
-        self.groupBoxInfo.setObjectName("groupBoxInfo")
-        self.gridLayout_2 = QtWidgets.QGridLayout(self.groupBoxInfo)
+        self.gridLayout_5.addItem(spacerItem1, 3, 0, 1, 1)
+        self.groupBoxWorkspace = QtWidgets.QGroupBox(self.scrollAreaWidgetContents)
+        self.groupBoxWorkspace.setObjectName("groupBoxWorkspace")
+        self.gridLayout_2 = QtWidgets.QGridLayout(self.groupBoxWorkspace)
         self.gridLayout_2.setObjectName("gridLayout_2")
-        self.labelExperimentName = QtWidgets.QLabel(self.groupBoxInfo)
-        self.labelExperimentName.setObjectName("labelExperimentName")
-        self.gridLayout_2.addWidget(self.labelExperimentName, 0, 0, 1, 1)
-        self.lineEditExperimentName = QtWidgets.QLineEdit(self.groupBoxInfo)
-        self.lineEditExperimentName.setObjectName("lineEditExperimentName")
-        self.gridLayout_2.addWidget(self.lineEditExperimentName, 0, 1, 1, 1)
-        self.lineEditAuthor = QtWidgets.QLineEdit(self.groupBoxInfo)
-        self.lineEditAuthor.setObjectName("lineEditAuthor")
-        self.gridLayout_2.addWidget(self.lineEditAuthor, 1, 1, 1, 1)
-        self.labelAuthor = QtWidgets.QLabel(self.groupBoxInfo)
-        self.labelAuthor.setObjectName("labelAuthor")
-        self.gridLayout_2.addWidget(self.labelAuthor, 1, 0, 1, 1)
-        self.gridLayout.addWidget(self.groupBoxInfo, 0, 1, 1, 1)
-        self.groupBoxPipeline = QtWidgets.QGroupBox(self.scrollAreaWidgetContents)
-        self.groupBoxPipeline.setObjectName("groupBoxPipeline")
-        self.gridLayoutPipeline = QtWidgets.QGridLayout(self.groupBoxPipeline)
-        self.gridLayoutPipeline.setObjectName("gridLayoutPipeline")
-        self.gridLayout.addWidget(self.groupBoxPipeline, 1, 1, 1, 1)
+        self.LineEditFilePath = QtWidgets.QLineEdit(self.groupBoxWorkspace)
+        self.LineEditFilePath.setObjectName("LineEditFilePath")
+        self.gridLayout_2.addWidget(self.LineEditFilePath, 0, 0, 1, 1)
+        self.ButtonBrowseWorkingDir = QtWidgets.QPushButton(self.groupBoxWorkspace)
+        self.ButtonBrowseWorkingDir.setObjectName("ButtonBrowseWorkingDir")
+        self.gridLayout_2.addWidget(self.ButtonBrowseWorkingDir, 0, 1, 1, 1)
+        self.gridLayout_5.addWidget(self.groupBoxWorkspace, 0, 0, 1, 1)
+        self.groupBoxPlugins = QtWidgets.QGroupBox(self.scrollAreaWidgetContents)
+        self.groupBoxPlugins.setObjectName("groupBoxPlugins")
+        self.formLayout = QtWidgets.QFormLayout(self.groupBoxPlugins)
+        self.formLayout.setObjectName("formLayout")
+        self.pushButtonPlugins = QtWidgets.QPushButton(self.groupBoxPlugins)
+        self.pushButtonPlugins.setObjectName("pushButtonPlugins")
+        self.formLayout.setWidget(
+            0, QtWidgets.QFormLayout.SpanningRole, self.pushButtonPlugins
+        )
+        self.gridLayout_5.addWidget(self.groupBoxPlugins, 1, 0, 1, 1)
         self.scrollArea.setWidget(self.scrollAreaWidgetContents)
         self.gridLayout_3.addWidget(self.scrollArea, 0, 0, 1, 1)
-        self.horizontalLayoutButtons = QtWidgets.QHBoxLayout()
-        self.horizontalLayoutButtons.setObjectName("horizontalLayoutButtons")
-        spacerItem1 = QtWidgets.QSpacerItem(
-            40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum
-        )
-        self.horizontalLayoutButtons.addItem(spacerItem1)
-        self.pushButtonCancel = QtWidgets.QPushButton(CreateExperimentDialog)
-        self.pushButtonCancel.setObjectName("pushButtonCancel")
-        self.horizontalLayoutButtons.addWidget(self.pushButtonCancel)
-        self.pushButtonAccept = QtWidgets.QPushButton(CreateExperimentDialog)
-        self.pushButtonAccept.setObjectName("pushButtonAccept")
-        self.horizontalLayoutButtons.addWidget(self.pushButtonAccept)
-        self.gridLayout_3.addLayout(self.horizontalLayoutButtons, 2, 0, 1, 1)
 
-        self.retranslateUi(CreateExperimentDialog)
-        self.pushButtonAccept.clicked.connect(CreateExperimentDialog.accept)
-        self.pushButtonCancel.clicked.connect(CreateExperimentDialog.reject)
-        QtCore.QMetaObject.connectSlotsByName(CreateExperimentDialog)
+        self.retranslateUi(DialogPreferences)
+        self.pushButtonCancel.clicked.connect(DialogPreferences.reject)
+        self.pushButtonAccept.clicked.connect(DialogPreferences.accept)
+        QtCore.QMetaObject.connectSlotsByName(DialogPreferences)
 
-    def retranslateUi(self, CreateExperimentDialog):
+    def retranslateUi(self, DialogPreferences):
         _translate = QtCore.QCoreApplication.translate
-        CreateExperimentDialog.setWindowTitle(
-            _translate("CreateExperimentDialog", "Meggie - Create new experiment")
-        )
-        self.groupBoxInfo.setTitle(
-            _translate("CreateExperimentDialog", "Experiment information")
-        )
-        self.labelExperimentName.setText(
-            _translate("CreateExperimentDialog", "Experiment name:")
-        )
-        self.labelAuthor.setText(
-            _translate("CreateExperimentDialog", "Experiment author:")
+        DialogPreferences.setWindowTitle(
+            _translate("DialogPreferences", "Meggie - Preferences")
         )
-        self.groupBoxPipeline.setTitle(
-            _translate("CreateExperimentDialog", "Select a pipeline for the analysis:")
+        self.pushButtonCancel.setText(_translate("DialogPreferences", "Cancel"))
+        self.pushButtonAccept.setText(_translate("DialogPreferences", "Ok"))
+        self.groupBoxMisc.setTitle(_translate("DialogPreferences", "Miscellaneous:"))
+        self.checkBoxAutomaticOpenPreviousExperiment.setText(
+            _translate(
+                "DialogPreferences",
+                "Automatically open previous experiment upon application startup",
+            )
+        )
+        self.groupBoxWorkspace.setTitle(_translate("DialogPreferences", "Workspace:"))
+        self.ButtonBrowseWorkingDir.setText(
+            _translate("DialogPreferences", "Browse...")
+        )
+        self.groupBoxPlugins.setTitle(_translate("DialogPreferences", "Plugins:"))
+        self.pushButtonPlugins.setText(
+            _translate("DialogPreferences", "Select active plugins...")
         )
-        self.pushButtonCancel.setText(_translate("CreateExperimentDialog", "Cancel"))
-        self.pushButtonAccept.setText(_translate("CreateExperimentDialog", "Ok"))
```

### Comparing `meggie-1.7.0/meggie/mainwindow/dialogs/pipelineDialogUi.py` & `meggie-1.8.0/meggie/mainwindow/dialogs/pipelineDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/mainwindow/dialogs/preferencesDialogMain.py` & `meggie-1.8.0/meggie/mainwindow/dialogs/preferencesDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/mainwindow/dialogs/preferencesDialogUi.py` & `meggie-1.8.0/meggie/mainwindow/dialogs/createExperimentDialogUi.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,108 +1,111 @@
 # -*- coding: utf-8 -*-
 
-# Form implementation generated from reading ui file 'preferencesDialogUi.ui'
+# Form implementation generated from reading ui file 'createExperimentDialogUi.ui'
 #
-# Created by: PyQt5 UI code generator 5.12.3
+# Created by: PyQt5 UI code generator 5.15.9
 #
-# WARNING! All changes made in this file will be lost!
+# WARNING: Any manual changes made to this file will be lost when pyuic5 is
+# run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtWidgets
 
 
-class Ui_DialogPreferences(object):
-    def setupUi(self, DialogPreferences):
-        DialogPreferences.setObjectName("DialogPreferences")
-        DialogPreferences.resize(507, 482)
-        self.gridLayout_3 = QtWidgets.QGridLayout(DialogPreferences)
+class Ui_CreateExperimentDialog(object):
+    def setupUi(self, CreateExperimentDialog):
+        CreateExperimentDialog.setObjectName("CreateExperimentDialog")
+        CreateExperimentDialog.setWindowModality(QtCore.Qt.WindowModal)
+        CreateExperimentDialog.resize(506, 373)
+        self.gridLayout_3 = QtWidgets.QGridLayout(CreateExperimentDialog)
         self.gridLayout_3.setObjectName("gridLayout_3")
-        self.horizontalLayout_2 = QtWidgets.QHBoxLayout()
-        self.horizontalLayout_2.setObjectName("horizontalLayout_2")
-        spacerItem = QtWidgets.QSpacerItem(
-            40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum
-        )
-        self.horizontalLayout_2.addItem(spacerItem)
-        self.pushButtonCancel = QtWidgets.QPushButton(DialogPreferences)
-        self.pushButtonCancel.setObjectName("pushButtonCancel")
-        self.horizontalLayout_2.addWidget(self.pushButtonCancel)
-        self.pushButtonAccept = QtWidgets.QPushButton(DialogPreferences)
-        self.pushButtonAccept.setObjectName("pushButtonAccept")
-        self.horizontalLayout_2.addWidget(self.pushButtonAccept)
-        self.gridLayout_3.addLayout(self.horizontalLayout_2, 5, 0, 1, 1)
-        self.scrollArea = QtWidgets.QScrollArea(DialogPreferences)
+        self.scrollArea = QtWidgets.QScrollArea(CreateExperimentDialog)
+        self.scrollArea.setFrameShape(QtWidgets.QFrame.NoFrame)
         self.scrollArea.setWidgetResizable(True)
         self.scrollArea.setObjectName("scrollArea")
         self.scrollAreaWidgetContents = QtWidgets.QWidget()
-        self.scrollAreaWidgetContents.setGeometry(QtCore.QRect(0, 0, 487, 431))
+        self.scrollAreaWidgetContents.setGeometry(QtCore.QRect(0, 0, 488, 324))
+        self.scrollAreaWidgetContents.setMinimumSize(QtCore.QSize(0, 0))
         self.scrollAreaWidgetContents.setObjectName("scrollAreaWidgetContents")
-        self.gridLayout_5 = QtWidgets.QGridLayout(self.scrollAreaWidgetContents)
-        self.gridLayout_5.setObjectName("gridLayout_5")
-        self.groupBoxMisc = QtWidgets.QGroupBox(self.scrollAreaWidgetContents)
-        self.groupBoxMisc.setObjectName("groupBoxMisc")
-        self.gridLayout_4 = QtWidgets.QGridLayout(self.groupBoxMisc)
-        self.gridLayout_4.setObjectName("gridLayout_4")
-        self.checkBoxAutomaticOpenPreviousExperiment = QtWidgets.QCheckBox(
-            self.groupBoxMisc
-        )
-        self.checkBoxAutomaticOpenPreviousExperiment.setObjectName(
-            "checkBoxAutomaticOpenPreviousExperiment"
-        )
-        self.gridLayout_4.addWidget(
-            self.checkBoxAutomaticOpenPreviousExperiment, 0, 0, 1, 1
-        )
-        self.gridLayout_5.addWidget(self.groupBoxMisc, 2, 0, 1, 1)
-        spacerItem1 = QtWidgets.QSpacerItem(
-            20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding
-        )
-        self.gridLayout_5.addItem(spacerItem1, 3, 0, 1, 1)
-        self.groupBoxWorkspace = QtWidgets.QGroupBox(self.scrollAreaWidgetContents)
-        self.groupBoxWorkspace.setObjectName("groupBoxWorkspace")
-        self.gridLayout_2 = QtWidgets.QGridLayout(self.groupBoxWorkspace)
+        self.gridLayout = QtWidgets.QGridLayout(self.scrollAreaWidgetContents)
+        self.gridLayout.setObjectName("gridLayout")
+        self.groupBoxInfo = QtWidgets.QGroupBox(self.scrollAreaWidgetContents)
+        self.groupBoxInfo.setObjectName("groupBoxInfo")
+        self.gridLayout_2 = QtWidgets.QGridLayout(self.groupBoxInfo)
         self.gridLayout_2.setObjectName("gridLayout_2")
-        self.LineEditFilePath = QtWidgets.QLineEdit(self.groupBoxWorkspace)
-        self.LineEditFilePath.setObjectName("LineEditFilePath")
-        self.gridLayout_2.addWidget(self.LineEditFilePath, 0, 0, 1, 1)
-        self.ButtonBrowseWorkingDir = QtWidgets.QPushButton(self.groupBoxWorkspace)
-        self.ButtonBrowseWorkingDir.setObjectName("ButtonBrowseWorkingDir")
-        self.gridLayout_2.addWidget(self.ButtonBrowseWorkingDir, 0, 1, 1, 1)
-        self.gridLayout_5.addWidget(self.groupBoxWorkspace, 0, 0, 1, 1)
-        self.groupBoxPlugins = QtWidgets.QGroupBox(self.scrollAreaWidgetContents)
-        self.groupBoxPlugins.setObjectName("groupBoxPlugins")
-        self.formLayout = QtWidgets.QFormLayout(self.groupBoxPlugins)
-        self.formLayout.setObjectName("formLayout")
-        self.pushButtonPlugins = QtWidgets.QPushButton(self.groupBoxPlugins)
-        self.pushButtonPlugins.setObjectName("pushButtonPlugins")
-        self.formLayout.setWidget(
-            0, QtWidgets.QFormLayout.SpanningRole, self.pushButtonPlugins
+        self.labelExperimentName = QtWidgets.QLabel(self.groupBoxInfo)
+        self.labelExperimentName.setObjectName("labelExperimentName")
+        self.gridLayout_2.addWidget(self.labelExperimentName, 0, 0, 1, 1)
+        self.lineEditExperimentName = QtWidgets.QLineEdit(self.groupBoxInfo)
+        self.lineEditExperimentName.setObjectName("lineEditExperimentName")
+        self.gridLayout_2.addWidget(self.lineEditExperimentName, 0, 1, 1, 1)
+        self.lineEditAuthor = QtWidgets.QLineEdit(self.groupBoxInfo)
+        self.lineEditAuthor.setObjectName("lineEditAuthor")
+        self.gridLayout_2.addWidget(self.lineEditAuthor, 1, 1, 1, 1)
+        self.labelAuthor = QtWidgets.QLabel(self.groupBoxInfo)
+        self.labelAuthor.setObjectName("labelAuthor")
+        self.gridLayout_2.addWidget(self.labelAuthor, 1, 0, 1, 1)
+        self.gridLayout.addWidget(self.groupBoxInfo, 0, 1, 1, 1)
+        self.groupBoxPipeline = QtWidgets.QGroupBox(self.scrollAreaWidgetContents)
+        self.groupBoxPipeline.setObjectName("groupBoxPipeline")
+        self.gridLayoutPipeline = QtWidgets.QGridLayout(self.groupBoxPipeline)
+        self.gridLayoutPipeline.setObjectName("gridLayoutPipeline")
+        self.gridLayout.addWidget(self.groupBoxPipeline, 1, 1, 1, 1)
+        spacerItem = QtWidgets.QSpacerItem(
+            20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding
         )
-        self.gridLayout_5.addWidget(self.groupBoxPlugins, 1, 0, 1, 1)
+        self.gridLayout.addItem(spacerItem, 3, 1, 1, 1)
+        self.groupBoxOpenData = QtWidgets.QGroupBox(self.scrollAreaWidgetContents)
+        self.groupBoxOpenData.setObjectName("groupBoxOpenData")
+        self.gridLayout_4 = QtWidgets.QGridLayout(self.groupBoxOpenData)
+        self.gridLayout_4.setObjectName("gridLayout_4")
+        self.labelOpenData = QtWidgets.QLabel(self.groupBoxOpenData)
+        self.labelOpenData.setObjectName("labelOpenData")
+        self.gridLayout_4.addWidget(self.labelOpenData, 0, 0, 1, 1)
+        self.comboBoxOpenData = QtWidgets.QComboBox(self.groupBoxOpenData)
+        self.comboBoxOpenData.setObjectName("comboBoxOpenData")
+        self.gridLayout_4.addWidget(self.comboBoxOpenData, 0, 1, 1, 1)
+        self.gridLayout.addWidget(self.groupBoxOpenData, 2, 1, 1, 1)
         self.scrollArea.setWidget(self.scrollAreaWidgetContents)
         self.gridLayout_3.addWidget(self.scrollArea, 0, 0, 1, 1)
+        self.horizontalLayoutButtons = QtWidgets.QHBoxLayout()
+        self.horizontalLayoutButtons.setObjectName("horizontalLayoutButtons")
+        spacerItem1 = QtWidgets.QSpacerItem(
+            40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum
+        )
+        self.horizontalLayoutButtons.addItem(spacerItem1)
+        self.pushButtonCancel = QtWidgets.QPushButton(CreateExperimentDialog)
+        self.pushButtonCancel.setObjectName("pushButtonCancel")
+        self.horizontalLayoutButtons.addWidget(self.pushButtonCancel)
+        self.pushButtonAccept = QtWidgets.QPushButton(CreateExperimentDialog)
+        self.pushButtonAccept.setObjectName("pushButtonAccept")
+        self.horizontalLayoutButtons.addWidget(self.pushButtonAccept)
+        self.gridLayout_3.addLayout(self.horizontalLayoutButtons, 2, 0, 1, 1)
 
-        self.retranslateUi(DialogPreferences)
-        self.pushButtonCancel.clicked.connect(DialogPreferences.reject)
-        self.pushButtonAccept.clicked.connect(DialogPreferences.accept)
-        QtCore.QMetaObject.connectSlotsByName(DialogPreferences)
+        self.retranslateUi(CreateExperimentDialog)
+        self.pushButtonAccept.clicked.connect(CreateExperimentDialog.accept)  # type: ignore
+        self.pushButtonCancel.clicked.connect(CreateExperimentDialog.reject)  # type: ignore
+        QtCore.QMetaObject.connectSlotsByName(CreateExperimentDialog)
 
-    def retranslateUi(self, DialogPreferences):
+    def retranslateUi(self, CreateExperimentDialog):
         _translate = QtCore.QCoreApplication.translate
-        DialogPreferences.setWindowTitle(
-            _translate("DialogPreferences", "Meggie - Preferences")
+        CreateExperimentDialog.setWindowTitle(
+            _translate("CreateExperimentDialog", "Meggie - Create new experiment")
+        )
+        self.groupBoxInfo.setTitle(
+            _translate("CreateExperimentDialog", "Experiment information")
+        )
+        self.labelExperimentName.setText(
+            _translate("CreateExperimentDialog", "Experiment name:")
+        )
+        self.labelAuthor.setText(
+            _translate("CreateExperimentDialog", "Experiment author:")
+        )
+        self.groupBoxPipeline.setTitle(
+            _translate("CreateExperimentDialog", "Select a pipeline for the analysis:")
         )
-        self.pushButtonCancel.setText(_translate("DialogPreferences", "Cancel"))
-        self.pushButtonAccept.setText(_translate("DialogPreferences", "Ok"))
-        self.groupBoxMisc.setTitle(_translate("DialogPreferences", "Miscellaneous:"))
-        self.checkBoxAutomaticOpenPreviousExperiment.setText(
-            _translate(
-                "DialogPreferences",
-                "Automatically open previous experiment upon application startup",
-            )
-        )
-        self.groupBoxWorkspace.setTitle(_translate("DialogPreferences", "Workspace:"))
-        self.ButtonBrowseWorkingDir.setText(
-            _translate("DialogPreferences", "Browse...")
-        )
-        self.groupBoxPlugins.setTitle(_translate("DialogPreferences", "Plugins:"))
-        self.pushButtonPlugins.setText(
-            _translate("DialogPreferences", "Select active plugins...")
+        self.groupBoxOpenData.setTitle(
+            _translate("CreateExperimentDialog", "Create from open data:")
         )
+        self.labelOpenData.setText(_translate("CreateExperimentDialog", "Dataset:"))
+        self.pushButtonCancel.setText(_translate("CreateExperimentDialog", "Cancel"))
+        self.pushButtonAccept.setText(_translate("CreateExperimentDialog", "Ok"))
```

### Comparing `meggie-1.7.0/meggie/mainwindow/dynamic.py` & `meggie-1.8.0/meggie/mainwindow/dynamic.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 
         if "name" not in action_spec:
             action_spec["name"] = action_spec["id"]
 
     return action_specs
 
 
-def construct_tab(tab_spec, action_specs, datatype_specs, parent):
+def construct_tab(tab_spec, action_specs, datatype_specs, has_raw, parent):
     """Constructs analysis tab dynamically. Returns a QDialog
     that can be used within a QTabDialog of the main window.
 
     Parameters
     ----------
     tab_spec : dict
         The specification of the tab read to a dict
@@ -286,14 +286,18 @@
                 action_spec = self.action_specs[action_name][2]
                 title = action_spec["name"]
                 description = action_spec.get("description", "")
 
                 pushButtonInputActionElement = QtWidgets.QPushButton(
                     self.groupBoxInputActions
                 )
+
+                if "raw" in action_spec.get("tags", []) and not has_raw:
+                    pushButtonInputActionElement.setEnabled(False)
+
                 pushButtonInputActionElement.setText(title)
                 pushButtonInputActionElement.setToolTip(description)
                 self.gridLayoutInputActions.addWidget(
                     pushButtonInputActionElement, idx, 0, 1, 1
                 )
                 setattr(
                     self,
@@ -306,24 +310,28 @@
                     20,
                     10,
                     QtWidgets.QSizePolicy.Minimum,
                     QtWidgets.QSizePolicy.Expanding,
                 )
                 self.gridLayoutInputActions.addItem(spacer, idx + 1, 0, 1, 1)
 
-            # add action buttons
+            # add output action buttons
             for idx, action_name in enumerate(self.tab_spec["output_actions"]):
 
                 action_spec = self.action_specs[action_name][2]
                 title = action_spec["name"]
                 description = action_spec.get("description", "")
 
                 pushButtonOutputActionElement = QtWidgets.QPushButton(
                     self.groupBoxOutputActions
                 )
+
+                if "raw" in action_spec.get("tags", []) and not has_raw:
+                    pushButtonOutputActionElement.setEnabled(False)
+
                 pushButtonOutputActionElement.setText(title)
                 pushButtonOutputActionElement.setToolTip(description)
                 self.gridLayoutOutputActions.addWidget(
                     pushButtonOutputActionElement, idx, 0, 1, 1
                 )
                 setattr(
                     self,
@@ -416,14 +424,17 @@
                     experiment = self.parent.experiment
                     if not experiment:
                         return
                     subject = experiment.active_subject
                     if not subject:
                         return
 
+                    if "raw" in action_spec.get("tags", []) and not has_raw:
+                        return
+
                     data = self._get_data()
 
                     try:
                         info_content = handler(
                             experiment,
                             data,
                             parent,
@@ -571,14 +582,20 @@
 
                 ui_element = getattr(self, "plainTextEditInfoElement_" + str(idx + 1))
 
                 source, package, action_spec = self.action_specs[info_name]
                 module = importlib.import_module(".".join([source, "actions", package]))
                 entry = action_spec["entry"]
 
+                if not subject:
+                    continue
+
+                if "raw" in action_spec.get("tags", []) and not has_raw:
+                    return
+
                 @threaded
                 def handler(*args):
                     return getattr(module, entry)(*args).run()
 
                 try:
                     info_content = handler(
                         experiment,
@@ -599,15 +616,15 @@
     DynamicTab.__name__ = "MainWindowTab" + tab_spec["id"].capitalize()
 
     tab = DynamicTab(parent)
 
     return tab
 
 
-def construct_tabs(selected_pipeline, window, prefs, include_eeg):
+def construct_tabs(selected_pipeline, window, prefs, include_eeg, has_raw):
     """Constructs as set of tabs based on specifications and the
     selected pipeline.
 
     Parameters
     ----------
     selected_pipeline : str
         ID of the selected pipeline
@@ -753,15 +770,17 @@
 
             if info_spec not in combined_tabs[idx]["info"]:
                 combined_tabs[idx]["info"].append(info_spec)
 
     # If everything is fine, construct each of the tabs
     tabs = []
     for tab_spec in combined_tabs:
-        tabs.append(construct_tab(tab_spec, action_specs, datatype_specs, window))
+        tabs.append(
+            construct_tab(tab_spec, action_specs, datatype_specs, has_raw, window)
+        )
 
     return tabs
 
 
 def subject_action(inner_function):
     """Decorator for automatically logging actions for each subject
     separately. Should be used within Action-instances.
```

### Comparing `meggie-1.7.0/meggie/mainwindow/preferences.py` & `meggie-1.8.0/meggie/mainwindow/preferences.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 """Contains a class for handling reading and storing of
 global preferences such as the previous experiment and
-the tab settings. Normally saved to ~/.meggieprefs.
+the tab settings.
 """
 
 import os
 import configparser
 import logging
 
-from meggie.utilities.filemanager import homepath
+from meggie.utilities.filemanager import configpath
+from meggie.utilities.filemanager import datapath
 
 
 class PreferencesHandler(object):
     """Class for storing and setting preferences."""
 
-    def __init__(self):
-        self.prefs_path = ""
-        self.workspace = ""
+    def __init__(self, prefs_path=""):
+
+        if prefs_path:
+            self.prefs_path = prefs_path
+        else:
+            self.prefs_path = os.path.join(configpath(), "preferences.cfg")
+
+        self.workspace = datapath()
+
         self.previous_experiment_name = ""
         self.auto_load_last_open_experiment = False
         self.active_plugins = []
 
         self.read_preferences_from_disk()
 
     def read_config(self):
         """Reads the config file from file system"""
-        filename = os.path.join(homepath(), ".meggieprefs")
         config = configparser.RawConfigParser()
-        if os.path.isfile(filename):
-            config.read(filename)
+        if os.path.isfile(self.prefs_path):
+            config.read(self.prefs_path)
         return config
 
     def write_preferences_to_disk(self):
         """Writes the preferences to file system, in INI style."""
         # Base the new config on the old one.
         config = self.read_config()
         try:
@@ -62,23 +68,33 @@
         )
 
         config.set("MiscOptions", "activePlugins", ",".join(self.active_plugins))
         logging.getLogger("ui_logger").info(
             "Active plugins: " + str(self.active_plugins)
         )
 
-        path = self.prefs_path
-        if not path:
-            path = os.path.join(homepath(), ".meggieprefs")
+        try:
+            os.makedirs(os.path.dirname(self.prefs_path))
+        except PermissionError:
+            logging.getLogger("ui_logger").exception(
+                "Could not save the configuration file."
+            )
+        except FileExistsError:
+            pass
 
-        with open(path, "w") as configfile:
+        with open(self.prefs_path, "w") as configfile:
             config.write(configfile)
 
     def read_preferences_from_disk(self):
         """Reads the preferences from file system into attributes."""
+
+        logging.getLogger("ui_logger").info(
+            f"Reading preferences from: {self.prefs_path}"
+        )
+
         config = self.read_config()
 
         try:
             self.workspace = config.get("Workspace", "workspaceDir")
         except Exception:
             pass
```

### Comparing `meggie-1.7.0/meggie/subject.py` & `meggie-1.8.0/meggie/subject.py`

 * *Files 16% similar despite different names*

```diff
@@ -122,22 +122,23 @@
             except OSError:
                 raise IOError("Could not find the raw file.")
             self._raw = raw
             return raw
 
     def save(self):
         """Saves the data to the existing path."""
-        try:
-            filemanager.save_raw(self._raw, self.raw_path)
-        except Exception:
-            raise Exception(
-                "Could not save the raw file. Please ensure "
-                "that the entire experiment folder has "
-                "write permissions."
-            )
+        if self.has_raw:
+            try:
+                filemanager.save_raw(self._raw, self.raw_path)
+            except Exception:
+                raise Exception(
+                    "Could not save the raw file. Please ensure "
+                    "that the entire experiment folder has "
+                    "write permissions."
+                )
 
     def release_memory(self):
         """Releases data from the memory."""
         if self._raw is not None:
             self._raw = None
 
     @property
@@ -146,14 +147,22 @@
         raw = self.get_raw(preload=False)
         channels = mne.pick_types(raw.info, eeg=True, meg=False)
         if len(channels) == 0:
             return False
         return True
 
     @property
+    def has_raw(self):
+        """Checks if is a 'placeholder' subject."""
+        if self.raw_fname:
+            return True
+        else:
+            return False
+
+    @property
     def sss_applied(self):
         """Checks if sss applied."""
 
         try:
             raw = self.get_raw()
             for item in raw.info["proc_history"]:
                 if "maxfilter" in item.get("creator", []):
@@ -179,7 +188,35 @@
             filemanager.ensure_folders([self.path] + paths)
         except OSError:
             raise OSError(
                 "Couldn't create all the necessary folders. "
                 "Please ensure that the experiment folder "
                 "has write permissions everywhere."
             )
+
+    def save_montage(self, montage):
+
+        ch_names = montage.ch_names
+        with open(os.path.join(self.path, "montage_channels.txt"), "w") as f:
+            for ch_name in ch_names:
+                f.write(ch_name + "\n")
+
+        montage.save(os.path.join(self.path, "montage.fif"), overwrite=True)
+
+    def read_montage(self):
+        montage_path = os.path.join(self.path, "montage.fif")
+        channels_path = os.path.join(self.path, "montage_channels.txt")
+        if os.path.exists(montage_path) and os.path.exists(channels_path):
+            ch_names = []
+            with open(channels_path, "r") as f:
+                for line in f:
+                    ch_names.append(line.strip())
+
+            montage = mne.channels.read_dig_fif(montage_path)
+
+            mapping = {}
+            for idx, name in enumerate(montage.ch_names):
+                mapping[name] = ch_names[idx]
+
+            montage.rename_channels(mapping)
+
+            return montage
```

### Comparing `meggie-1.7.0/meggie/tests/test_experiment_and_subject.py` & `meggie-1.8.0/meggie/tests/test_experiment_and_subject.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,17 +13,16 @@
         sample_folder = mne.datasets.sample.data_path()
         sample_fname = os.path.join(
             sample_folder, "MEG", "sample", "sample_audvis_raw.fif"
         )
 
         # Create preferences object to store working directory
         # Also set prefs_path inside tempdir
-        prefs = PreferencesHandler()
+        prefs = PreferencesHandler(prefs_path=os.path.join(dirpath, ".meggieprefs"))
         prefs.workspace = dirpath
-        prefs.prefs_path = os.path.join(dirpath, ".meggieprefs")
 
         # create experiment (creates experiment directory inside working directory,
         # also saves prefs (previous_experiment is set) and saves .exp file)
         name = "Test experiment äö€ê*ë"
         author = "Author"
         experiment = initialize_new_experiment(name, author, prefs)
```

### Comparing `meggie-1.7.0/meggie/utilities/channels.py` & `meggie-1.8.0/meggie/utilities/channels.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,98 @@
 """Contains functions that help with channel-related tasks.
 """
 
 import numpy as np
 import mne
 
-from mne.channels import _divide_to_regions
 
-
-def is_montage_set(raw, ch_type):
+def is_montage_set(info, ch_type):
     """Checks whether channel locations are found in the info for given channel type.
 
     Parameters
     ----------
-    raw : mne.io.Raw
-        Raw containing info which contains channel information.
+    info : mne.Info
+        Info containing channel information.
     ch_type : str
         Should be 'meg' or 'eeg'.
 
     Returns
     -------
     bool
         Whether the channel locations were found.
     """
 
     if ch_type == "meg":
-        picks = mne.pick_types(raw.info, meg=True, eeg=False)
+        picks = mne.pick_types(info, meg=True, eeg=False)
     else:
-        picks = mne.pick_types(raw.info, meg=False, eeg=True)
+        picks = mne.pick_types(info, meg=False, eeg=True)
 
-    ch_names = [
-        ch_name for idx, ch_name in enumerate(raw.info["ch_names"]) if idx in picks
-    ]
+    ch_names = [ch_name for idx, ch_name in enumerate(info["ch_names"]) if idx in picks]
 
     if not ch_names:
-        raise Exception("Data does not contain channels of type " + str(ch_type))
+        return False
 
-    info_filt = filter_info(raw.info, ch_names)
+    info_filt = filter_info(info, ch_names)
 
     # check if there is no montage set..
     ch_norms = []
     for ch in info_filt["chs"]:
         ch_norms.append(np.linalg.norm(ch["loc"]))
     if np.all(np.isclose(ch_norms, ch_norms[0])):
         return False
 
     return True
 
 
-def get_default_channel_groups(raw, ch_type):
+def ensure_montage(subject, inst, ch_type):
+    """Checks if the subject contains a montage that could be used for inst."""
+    montage = subject.read_montage()
+    if montage:
+        inst.set_montage(montage)
+
+
+def find_montage_info(subject, datatypes, ch_type):
+    """Try to find channel locations first from raw and then from any dataobject.
+
+    Parameters
+    ----------
+    subject : meggie.subject.Subject
+        The subject to find the montage info in
+    ch_type : str
+        Should be 'meg' or 'eeg'.
+    datatypes : list
+        List of datatypes to look into
+
+    Returns
+    -------
+    info : mne.Info | None
+        Info containing channel locations.
+    """
+
+    if subject.has_raw:
+        raw = subject.get_raw(preload=False)
+        if is_montage_set(raw.info, ch_type):
+            return raw.info
+
+    for datatype in datatypes:
+        objects = getattr(subject, datatype, {})
+        for key, item in objects.items():
+            try:
+                info = item.info
+            except NotImplementedError:
+                continue
+
+            if is_montage_set(info, ch_type):
+                return info
+
+    # Did not find anything..
+    return None
+
+
+def get_default_channel_groups(info, ch_type):
     """Returns channels grouped by standard locations
     (Left-frontal, Right-occipital, etc.). Grouping is done via
     geometric division from mne, to have a generic ability
     to divide different eeg caps into groups.
 
     Parameters
     ----------
@@ -65,31 +106,29 @@
     dict
         A dictionary with groups (Left-temporal, etc.) as keys and
         lists of channels as values.
 
     """
 
     if ch_type == "meg":
-        picks = mne.pick_types(raw.info, meg=True, eeg=False)
+        picks = mne.pick_types(info, meg=True, eeg=False)
     else:
-        picks = mne.pick_types(raw.info, meg=False, eeg=True)
+        picks = mne.pick_types(info, meg=False, eeg=True)
 
-    ch_names = [
-        ch_name for idx, ch_name in enumerate(raw.info["ch_names"]) if idx in picks
-    ]
+    ch_names = [ch_name for idx, ch_name in enumerate(info["ch_names"]) if idx in picks]
     if not ch_names:
         return {}
 
     # check if there is no montage set..
-    if not is_montage_set(raw, ch_type):
+    if not is_montage_set(info, ch_type):
         return {}
 
-    info_filt = filter_info(raw.info, ch_names)
+    info_filt = filter_info(info, ch_names)
 
-    regions = _divide_to_regions(info_filt, add_stim=False)
+    regions = mne.channels._divide_to_regions(info_filt, add_stim=False)
 
     ch_groups = {}
     for region_key, region in regions.items():
         region_ch_names = [info_filt["ch_names"][ch_idx] for ch_idx in region]
         ch_groups[region_key] = region_ch_names
 
     return ch_groups
```

### Comparing `meggie-1.7.0/meggie/utilities/compare.py` & `meggie-1.8.0/meggie/utilities/compare.py`

 * *Files 18% similar despite different names*

```diff
@@ -45,9 +45,9 @@
     ----------
     raw_from : mne.io.Raw
         The original raw.
     raw_to : mne.io.Raw
         The changed raw.
 
     """
-    changes_raw = _prepare_raw_for_changes(raw_from, raw_to)
-    changes_raw.plot(color="red", bad_color="blue", title="Comparison plot")
+    raw = _prepare_raw_for_changes(raw_from, raw_to)
+    raw.plot(color="red", bad_color="blue", title="Comparison plot")
```

### Comparing `meggie-1.7.0/meggie/utilities/datatype.py` & `meggie-1.8.0/meggie/utilities/datatype.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/utilities/debug.py` & `meggie-1.8.0/meggie/utilities/debug.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/utilities/dialogs/TFROutputOptionsMain.py` & `meggie-1.8.0/meggie/utilities/dialogs/TFROutputOptionsMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/utilities/dialogs/TFROutputOptionsUi.py` & `meggie-1.8.0/meggie/utilities/dialogs/TFROutputOptionsUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/utilities/dialogs/bitSelectionDialogMain.py` & `meggie-1.8.0/meggie/utilities/dialogs/bitSelectionDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/utilities/dialogs/bitSelectionDialogUi.py` & `meggie-1.8.0/meggie/utilities/dialogs/bitSelectionDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/utilities/dialogs/groupSelectionDialogMain.py` & `meggie-1.8.0/meggie/utilities/dialogs/groupSelectionDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/utilities/dialogs/groupSelectionDialogUi.py` & `meggie-1.8.0/meggie/utilities/dialogs/groupSelectionDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/utilities/dialogs/outputOptionsMain.py` & `meggie-1.8.0/meggie/utilities/dialogs/outputOptionsMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/utilities/dialogs/outputOptionsUi.py` & `meggie-1.8.0/meggie/utilities/dialogs/outputOptionsUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/utilities/dialogs/powerSpectrumAddAdvancedDialogMain.py` & `meggie-1.8.0/meggie/utilities/dialogs/powerSpectrumAddAdvancedDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/utilities/dialogs/powerSpectrumAddAdvancedDialogUi.py` & `meggie-1.8.0/meggie/utilities/dialogs/powerSpectrumAddAdvancedDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/utilities/dialogs/powerSpectrumDialogMain.py` & `meggie-1.8.0/meggie/utilities/dialogs/powerSpectrumDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/utilities/dialogs/powerSpectrumDialogUi.py` & `meggie-1.8.0/meggie/utilities/dialogs/powerSpectrumDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/utilities/dialogs/shortMessageBoxMain.py` & `meggie-1.8.0/meggie/utilities/dialogs/shortMessageBoxMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/utilities/dialogs/shortMessageBoxUi.py` & `meggie-1.8.0/meggie/utilities/dialogs/shortMessageBoxUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/utilities/dialogs/shortQuestionBoxMain.py` & `meggie-1.8.0/meggie/utilities/dialogs/shortQuestionBoxMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/utilities/dialogs/shortQuestionBoxUi.py` & `meggie-1.8.0/meggie/utilities/dialogs/shortQuestionBoxUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/utilities/dialogs/simpleDialogMain.py` & `meggie-1.8.0/meggie/utilities/dialogs/simpleDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/utilities/dialogs/simpleDialogUi.py` & `meggie-1.8.0/meggie/utilities/dialogs/simpleDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/utilities/dialogs/singleChannelDialogMain.py` & `meggie-1.8.0/meggie/utilities/dialogs/singleChannelDialogMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/utilities/dialogs/singleChannelDialogUi.py` & `meggie-1.8.0/meggie/utilities/dialogs/singleChannelDialogUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/utilities/events.py` & `meggie-1.8.0/meggie/utilities/events.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/utilities/filemanager.py` & `meggie-1.8.0/meggie/utilities/filemanager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Contains functions for tasks related to file system.
 """
 
+import appdirs
 import os
 import shutil
 import re
 import datetime
 import logging
 import errno
 
@@ -256,24 +257,47 @@
 
     Returns
     -------
     str
         Path to home directory.
 
     """
-    from os.path import expanduser
 
-    home = expanduser("~")
+    home = os.path.expanduser("~")
 
     if not home:
         return "."
 
     return home
 
 
+def configpath():
+    """Find a path for configuration files.
+
+    Returns
+    -------
+    str
+        Path to config directory
+
+    """
+    return appdirs.user_config_dir("meggie")
+
+
+def datapath():
+    """Find a path for data files.
+
+    Returns
+    -------
+    str
+        Path to data directory
+
+    """
+    return os.path.join(appdirs.user_data_dir("meggie"), "experiments")
+
+
 def get_supported_formats():
     mne_supported = mne_get_supported()
 
     items = []
     for ext_item in mne_supported.items():
         ext = ext_item[0]
         names = [val[0] for val in ext_item[1].items()]
```

### Comparing `meggie-1.7.0/meggie/utilities/formats.py` & `meggie-1.8.0/meggie/utilities/formats.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/utilities/measurement_info.py` & `meggie-1.8.0/meggie/utilities/measurement_info.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/utilities/messaging.py` & `meggie-1.8.0/meggie/utilities/messaging.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/utilities/names.py` & `meggie-1.8.0/meggie/utilities/names.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/utilities/plotting.py` & `meggie-1.8.0/meggie/utilities/plotting.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/utilities/testing.py` & `meggie-1.8.0/meggie/utilities/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from meggie.datatypes.tfr.tfr import TFR
 
 os.environ["QT_QPA_PLATFORM"] = "offscreen"
 mne.viz.set_browser_backend("matplotlib")
 matplotlib.use("Agg")
 
 
-def create_experiment(
+def create_multi_sample_experiment(
     experiment_folder, experiment_name, subjects_raw, overwrite=False
 ):
     """Creates experiment from list of raw objects.
 
     Parameters
     ----------
     experiment_folder : str
@@ -138,15 +138,15 @@
 
         subject_raw = mne.io.RawArray(
             np.concatenate(data, axis=1), raw.info, first_samp=0
         )
 
         subjects_raw.append(subject_raw)
 
-    return create_experiment(
+    return create_multi_sample_experiment(
         experiment_folder, experiment_name, subjects_raw, overwrite=overwrite
     )
 
 
 def create_test_experiment(experiment_folder, experiment_name, n_subjects=2):
     """Generate experiment with data for testing."""
 
@@ -336,36 +336,44 @@
         # before each test
         os.environ["QT_QPA_PLATFORM"] = "offscreen"
         self.qtbot = qtbot
         self.monkeypatch = monkeypatch
         self.mock_main_window = MockMainWindow()
         self.temp_dir = tempfile.TemporaryDirectory()
         self.dirpath = self.temp_dir.name
+        self.package = "meggie.actions"
         self.setup_experiment()
         yield
         # after each test
         self.temp_dir.cleanup()
         for widget in QApplication.topLevelWidgets():
             if widget.isWindow():
                 widget.close()
                 widget.deleteLater()
 
     def setup_experiment(self):
         self.experiment = create_test_experiment(self.dirpath, "test_experiment")
         self.experiment.activate_subject("sample_01-raw")
 
     def run_action(self, action_name, handler, data={}, patch_paths=[]):
-
         # patch logger to raise exceptions
         logger = logging.getLogger("ui_logger")
         self.monkeypatch.setattr(logger, "exception", patched_logger_exception)
 
+        basepath = f"{self.package}.{action_name}"
+        if basepath not in patch_paths:
+            patch_paths.append(basepath)
+
         # patch messageboxes to raise exceptions
         for patch_path in patch_paths:
-            module = importlib.import_module(patch_path)
+            try:
+                module = importlib.import_module(patch_path)
+            except ModuleNotFoundError:
+                # the action is probably not within self.package
+                continue
 
             if getattr(module, "exc_messagebox", None):
                 self.monkeypatch.setattr(
                     ".".join([patch_path, "exc_messagebox"]),
                     patched_exc_messagebox,
                 )
```

### Comparing `meggie-1.7.0/meggie/utilities/tests/test_channels.py` & `meggie-1.8.0/meggie/utilities/tests/test_channels.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 def test_default_channel_groups():
     sample_folder = mne.datasets.sample.data_path()
     sample_fname = os.path.join(sample_folder, "MEG", "sample", "sample_audvis_raw.fif")
 
     raw = mne.io.read_raw_fif(sample_fname)
 
-    assert get_default_channel_groups(raw, "eeg")["Left-frontal"] == [
+    assert get_default_channel_groups(raw.info, "eeg")["Left-frontal"] == [
         "EEG 001",
         "EEG 004",
         "EEG 005",
         "EEG 009",
         "EEG 010",
         "EEG 011",
         "EEG 012",
@@ -73,16 +73,16 @@
     sample_fname = os.path.join(sample_folder, "MEG", "sample", "sample_audvis_raw.fif")
 
     raw = mne.io.read_raw_fif(sample_fname, preload=True)
     info = raw.info
 
     ch_names = info["ch_names"][:20]
 
-    meg_channel_groups = get_default_channel_groups(raw, "meg")
-    eeg_channel_groups = get_default_channel_groups(raw, "eeg")
+    meg_channel_groups = get_default_channel_groups(raw.info, "meg")
+    eeg_channel_groups = get_default_channel_groups(raw.info, "eeg")
 
     # find out to which channel group each of the channels belongs to
     results = []
     for ch_name in ch_names:
         for ch_group_name, ch_group in meg_channel_groups.items():
             if ch_name in ch_group:
                 results.append((ch_name, ch_group_name))
```

### Comparing `meggie-1.7.0/meggie/utilities/tests/test_events.py` & `meggie-1.8.0/meggie/utilities/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/utilities/tests/test_filemanager.py` & `meggie-1.8.0/meggie/utilities/tests/test_filemanager.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/utilities/tests/test_measurement_info.py` & `meggie-1.8.0/meggie/utilities/tests/test_measurement_info.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/utilities/tests/test_names.py` & `meggie-1.8.0/meggie/utilities/tests/test_names.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/utilities/threading.py` & `meggie-1.8.0/meggie/utilities/threading.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,18 +30,14 @@
     function
         The wrapped function.
     """
 
     def decorated(*args, **kwargs):
         """Inner function for threaded-decoration"""
 
-        # allow bypassing threads for testing
-        if kwargs.pop("no_threading", None):
-            return func(*args, **kwargs)
-
         # worker threads should be used on time consuming
         # tasks so add a indicator for user
         QtWidgets.QApplication.setOverrideCursor(QtGui.QCursor(QtCore.Qt.WaitCursor))
 
         pool = ThreadPool(processes=1)
         do_meanwhile = kwargs.pop("do_meanwhile", None)
         bucket = Queue()
```

### Comparing `meggie-1.7.0/meggie/utilities/units.py` & `meggie-1.8.0/meggie/utilities/units.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/utilities/validators.py` & `meggie-1.8.0/meggie/utilities/validators.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/utilities/widgets/batchingWidgetMain.py` & `meggie-1.8.0/meggie/utilities/widgets/batchingWidgetMain.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie/utilities/widgets/batchingWidgetUi.py` & `meggie-1.8.0/meggie/utilities/widgets/batchingWidgetUi.py`

 * *Files identical despite different names*

### Comparing `meggie-1.7.0/meggie.egg-info/SOURCES.txt` & `meggie-1.8.0/meggie.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -238,14 +238,15 @@
 meggie/mainwindow/dialogs/pipelineDialogUi.py
 meggie/mainwindow/dialogs/preferencesDialogMain.py
 meggie/mainwindow/dialogs/preferencesDialogUi.py
 meggie/tests/test_experiment_and_subject.py
 meggie/utilities/__init__.py
 meggie/utilities/channels.py
 meggie/utilities/compare.py
+meggie/utilities/datasets.py
 meggie/utilities/datatype.py
 meggie/utilities/debug.py
 meggie/utilities/events.py
 meggie/utilities/filemanager.py
 meggie/utilities/formats.py
 meggie/utilities/measurement_info.py
 meggie/utilities/messaging.py
@@ -274,14 +275,15 @@
 meggie/utilities/dialogs/shortQuestionBoxMain.py
 meggie/utilities/dialogs/shortQuestionBoxUi.py
 meggie/utilities/dialogs/simpleDialogMain.py
 meggie/utilities/dialogs/simpleDialogUi.py
 meggie/utilities/dialogs/singleChannelDialogMain.py
 meggie/utilities/dialogs/singleChannelDialogUi.py
 meggie/utilities/tests/test_channels.py
+meggie/utilities/tests/test_datasets.py
 meggie/utilities/tests/test_events.py
 meggie/utilities/tests/test_filemanager.py
 meggie/utilities/tests/test_measurement_info.py
 meggie/utilities/tests/test_names.py
 meggie/utilities/tests/test_plotting.py
 meggie/utilities/widgets/__init__.py
 meggie/utilities/widgets/batchingWidgetMain.py
```

### Comparing `meggie-1.7.0/setup.py` & `meggie-1.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 description = "User-friendly graphical user interface to do M/EEG analysis"
 
 setup(
     name='meggie',
-    version='1.7.0',
+    version='1.8.0',
     description=description,
     long_description=description,
     long_description_content_type="text/plain",
     author='CIBR',
     author_email='erkka.heinila@jyu.fi',
     url='https://github.com/cibr-jyu/meggie',
     license='BSD',
```

