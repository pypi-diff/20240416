# Comparing `tmp/snudda-2.0.1.tar.gz` & `tmp/snudda-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snudda-2.0.1.tar", last modified: Wed Mar 20 06:53:12 2024, max compression
+gzip compressed data, was "snudda-2.0.2.tar", last modified: Tue Apr 16 09:29:00 2024, max compression
```

## Comparing `snudda-2.0.1.tar` & `snudda-2.0.2.tar`

### file list

```diff
@@ -1,514 +1,514 @@
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.623719 snudda-2.0.1/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    35149 2022-09-19 09:45:08.000000 snudda-2.0.1/LICENSE
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4233 2024-03-20 06:53:12.623719 snudda-2.0.1/PKG-INFO
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3756 2023-06-27 13:26:59.000000 snudda-2.0.1/README.md
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)       38 2024-03-20 06:53:12.623719 snudda-2.0.1/setup.cfg
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2696 2023-06-27 13:26:59.000000 snudda-2.0.1/setup.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.519711 snudda-2.0.1/snudda/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      506 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/__init__.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.519711 snudda-2.0.1/snudda/analyse/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      199 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/analyse/__init__.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    98425 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/analyse/analyse.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7932 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/analyse/analyse_gap_junction_coupling.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3250 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/analyse/analyse_input.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5575 2022-11-03 09:16:18.000000 snudda-2.0.1/snudda/analyse/analyse_neuroinformatics2020.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8656 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/analyse/analyse_spike_trains.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19907 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/analyse/analyse_striatum.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5992 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/analyse/analyse_synapse_location.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7575 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/analyse/analyse_topology.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    12380 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/analyse/analyse_topology_activity.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     6277 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/analyse/spike_time_tiling_coefficient.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    12884 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/cli.py
--rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)    38049 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/core.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.515711 snudda-2.0.1/snudda/data/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.515711 snudda-2.0.1/snudda/data/InputAxons/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.519711 snudda-2.0.1/snudda/data/InputAxons/Cortex/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   432939 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/InputAxons/Cortex/AA0059.swc
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.519711 snudda-2.0.1/snudda/data/InputAxons/Cortex/Reg10/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   900524 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/InputAxons/Cortex/Reg10/AA0059-reg10.swc
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.523712 snudda-2.0.1/snudda/data/InputAxons/Cortex/Reg15/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   597398 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/InputAxons/Cortex/Reg15/AA0059-reg15.swc
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.523712 snudda-2.0.1/snudda/data/InputAxons/Cortex/Reg5/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1809577 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/InputAxons/Cortex/Reg5/AA0059-reg5.swc
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.527712 snudda-2.0.1/snudda/data/InputAxons/GPe2Striatum/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1269 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/InputAxons/GPe2Striatum/example-projection-config.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   444324 2023-02-15 16:15:38.000000 snudda-2.0.1/snudda/data/InputAxons/GPe2Striatum/prototypical-axon.swc
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.527712 snudda-2.0.1/snudda/data/InputAxons/Thalamus/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   464916 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/InputAxons/Thalamus/AA0054.swc
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.531712 snudda-2.0.1/snudda/data/InputAxons/Thalamus/Reg10/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   513478 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/InputAxons/Thalamus/Reg10/AA0054-reg10.swc
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.531712 snudda-2.0.1/snudda/data/InputAxons/Thalamus/Reg15/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   346069 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/InputAxons/Thalamus/Reg15/AA0054-reg15.swc
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.531712 snudda-2.0.1/snudda/data/InputAxons/Thalamus/Reg5/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1022637 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/InputAxons/Thalamus/Reg5/AA0054-reg5.swc
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.535713 snudda-2.0.1/snudda/data/density/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    87096 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/density/1001_STRd_Sst_dens.csv
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    89256 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/density/1001_STRd_Sst_dens_smooth.csv
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    74510 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/density/252_STRd_Chat_dens.csv
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    77158 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/density/252_STRd_Chat_dens_smooth.csv
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    94468 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/density/352_STRd_Drd1_dens.csv
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    95346 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/density/352_STRd_Drd1_dens_smooth.csv
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    95932 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/density/72109410_STRd_Adora2a_dens.csv
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    96454 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/density/72109410_STRd_Adora2a_dens_smooth.csv
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    77578 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/density/79556738_STRd_Pvalb_dens.csv
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    79756 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/density/79556738_STRd_Pvalb_dens_smooth.csv
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1132 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/density/combine_densities.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  2256264 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/density/dorsal_striatum_density.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.515711 snudda-2.0.1/snudda/data/experiment_config/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.539713 snudda-2.0.1/snudda/data/experiment_config/pair_recording/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      477 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/data/experiment_config/pair_recording/experiment-config-1.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      591 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/data/experiment_config/pair_recording/experiment-config-2.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      645 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/data/experiment_config/pair_recording/experiment-config-3.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      646 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/data/experiment_config/pair_recording/experiment-config-4.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      461 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/data/experiment_config/pair_recording/experiment-config-5.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      605 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/data/experiment_config/pair_recording/experiment-config-6.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      695 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/data/experiment_config/pair_recording/experiment-config-7.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.539713 snudda-2.0.1/snudda/data/images/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    52659 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/images/snudda-video-qr-code.png
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.543713 snudda-2.0.1/snudda/data/input_config/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.543713 snudda-2.0.1/snudda/data/input_config/Kim2019/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3035 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/data/input_config/Kim2019/Kim et al., 2019 - Henry Yin - Extended2a.csv
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    25975 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/data/input_config/Kim2019/Kim et al., 2019 - Henry Yin - Extended2a.xlsx
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1433 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/data/input_config/Kim2019/get_experimental_firing_freq.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5834 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/input_config/external-input-dSTR-scaled-v2.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5827 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/input_config/external-input-dSTR-scaled-v3.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5827 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/input_config/external-input-dSTR-scaled-v3b.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5834 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/input_config/external-input-dSTR-scaled-v4-cluster-test.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5811 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/input_config/external-input-dSTR-scaled-v4.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5843 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/input_config/external-input-dSTR-scaled.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      768 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/input_config/input-tinytest-ChIN.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1831 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/input_config/input-tinytest-Channel-Activation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1803 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/input_config/input-tinytest-channel-1.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1803 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/input_config/input-tinytest-channel-2.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5395 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/input_config/input-tinytest-v7.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5409 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/input_config/input-tinytest-v8.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5547 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/input_config/input-tinytest-v9-freq-vectors.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5709 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/data/input_config/input-v10-scaled.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      506 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/input_config/input_output_dspn_template_IC.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.555714 snudda-2.0.1/snudda/data/mesh/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    88391 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/data/mesh/GPe-left.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    92643 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/data/mesh/GPe-right.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   192511 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/mesh/GPe.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    28420 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/data/mesh/GPi-left.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    30275 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/data/mesh/GPi-right.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    60912 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/mesh/GPi.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    32645 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/data/mesh/SNc-left.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    33562 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/data/mesh/SNc-right.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    68536 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/mesh/SNc.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    77916 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/data/mesh/SNr-left.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    78090 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/data/mesh/SNr-right.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   164445 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/mesh/SNr.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    20912 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/data/mesh/STN-left.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    21156 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/data/mesh/STN-right.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    44005 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/mesh/STN.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   507113 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/data/mesh/Striatum-d-left.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   531971 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/data/mesh/Striatum-d-right.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1069021 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/mesh/Striatum-d.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1733004 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/mesh/Striatum-dorsal-left-hemisphere.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1813629 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/mesh/Striatum-dorsal-right-hemisphere.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   363232 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/data/mesh/Striatum-v-left.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   374672 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/data/mesh/Striatum-v-right.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   763087 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/mesh/Striatum-v.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      828 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/data/mesh/cut_mesh.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2358 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/mesh/get_mesh.ipynb
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.515711 snudda-2.0.1/snudda/data/nest/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.555714 snudda-2.0.1/snudda/data/nest/models/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      272 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/nest/models/FS.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      278 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/nest/models/dSPN.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      276 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/nest/models/iSPN.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.555714 snudda-2.0.1/snudda/data/nest/synapses/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)       25 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/nest/synapses/excitatory.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)       25 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/nest/synapses/excitatory_distal.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)       25 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/nest/synapses/excitatory_proximal.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)       25 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/nest/synapses/excitatory_soma.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)       25 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/nest/synapses/inhibitory.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)       25 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/nest/synapses/inhibitory_distal.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)       25 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/nest/synapses/inhibitory_proximal.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)       25 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/nest/synapses/inhibitory_soma.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.515711 snudda-2.0.1/snudda/data/neurons/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.559714 snudda-2.0.1/snudda/data/neurons/mechanisms/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2111 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/Im_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1352 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/Kv3_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1375 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/NO.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2598 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/bk_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2511 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/bk_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2744 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/bk_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4351 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/ca_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1282 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/cadyn_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1609 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/cadyn_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4561 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/cal12_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4723 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/cal13_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2871 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/cal_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1663 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/caldyn_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3256 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/can_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4517 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/can_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2986 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/cap_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2424 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/caq_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2485 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/caq_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2814 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/car_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3855 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/car_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2413 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/cat32_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2414 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/cat33_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1074 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/concACh.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1084 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/concDA.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      907 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/concDAfile.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3903 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/hcn12_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2247 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/hd_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3028 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/im_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3099 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/it_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3406 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/kaf_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3407 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/kaf_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4335 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/kaf_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3334 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/kas_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3932 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/kas_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1189 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/kcnq_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1179 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/kdb_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1781 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/kdr_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2810 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/kdr_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1725 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/kdr_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1230 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/kdrb_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3594 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/kir23_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3595 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/kir23_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1665 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/kir2_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3586 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/kir_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4151 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/kir_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1254 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/kv2_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2679 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/kv4_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3111 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/na2_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3677 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/na3_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3119 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/na_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2833 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/naf_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3043 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/naf_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3245 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/naf_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      377 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/par_ggap.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1909 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/sk_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1896 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/sk_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1896 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/sk_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2370 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/tmampa.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4291 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/tmgabaa.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7671 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/tmglut.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7535 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/tmglut_M1RH_D1.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8029 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/tmglut_double.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1336 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/tmnmda.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1026 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms/vecevent.mod
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.567715 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1352 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/Kv3_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2225 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/bk_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2511 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/bk_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2744 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/bk_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3998 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/ca_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1282 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/cadyn_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1609 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/cadyn_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3249 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/cal12_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3452 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/cal13_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1800 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/cal_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1663 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/caldyn_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3256 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/can_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3256 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/can_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1686 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/cap_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2424 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/caq_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2485 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/caq_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2814 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/car_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2814 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/car_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2413 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/cat32_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2414 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/cat33_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1164 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/h_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2855 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/hcn12_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1724 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/im_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2061 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/it_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2364 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/kaf_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2993 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/kaf_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2292 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/kas_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2886 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/kas_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1189 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/kcnq_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1781 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/kdr_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1725 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/kdr_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1250 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/kdrbca1_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      605 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/kir2_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2543 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/kir_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2882 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/kir_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1254 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/kv2_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1642 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/kv4_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2082 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/na2_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2637 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/na3n_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2076 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/na_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1791 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/naf_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1980 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/naf_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      377 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/par_ggap.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1909 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/sk_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1896 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/sk_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1896 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/sk_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2370 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/tmampa.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2893 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/tmgabaa.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5773 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/tmglut.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1336 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/tmnmda.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1026 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/vecevent.mod
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.515711 snudda-2.0.1/snudda/data/neurons/striatum/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.515711 snudda-2.0.1/snudda/data/neurons/striatum/chin/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.567715 snudda-2.0.1/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      215 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    89390 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    69404 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/optim_chin_morph_renamed2019-11-08.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3194 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      403 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/protocols.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.515711 snudda-2.0.1/snudda/data/neurons/striatum/dspn/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.571715 snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   673225 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/WT-0728MSN01-cor-rep-ax.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      936 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/fix_indexing.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    92361 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    94239 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/modulationDAACh.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    80017 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.571715 snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   600711 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/WT-P270-20-15ak-cor.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    92630 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59991 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.571715 snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   183549 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/21-6-DE-cor-rep-ax.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    92630 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59972 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.575715 snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   660197 2023-02-15 16:15:38.000000 snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/WT-1215MSN03-cor-rep-ax2.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    92630 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    99934 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.515711 snudda-2.0.1/snudda/data/neurons/striatum/fs/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.579716 snudda-2.0.1/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   620377 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/MTC180800A-IDB-cor-rep.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      244 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1226312 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    21438 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.587716 snudda-2.0.1/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  4918863 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/DR-rat-Mar-13-08-1-536-R-cor-rep.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      244 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1226312 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19567 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.591717 snudda-2.0.1/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   620377 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/MTC180800A-IDB-cor-rep.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      244 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1226312 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5366 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.595717 snudda-2.0.1/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   826139 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/MTC251001A-IDB-cor-rep.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      244 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1226312 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5354 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.515711 snudda-2.0.1/snudda/data/neurons/striatum/ispn/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.595717 snudda-2.0.1/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1013802 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/51-5-DE-cor-rep-ax.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59125 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    69979 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.599717 snudda-2.0.1/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1153456 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/WT-MSN1-cor-rep-ax.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59125 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59905 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.599717 snudda-2.0.1/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   587827 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/WT-P270-09-15ak-cor.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59125 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    49989 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.599717 snudda-2.0.1/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   254041 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/46-3-DE-cor-rep-ax.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59125 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    29994 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.515711 snudda-2.0.1/snudda/data/neurons/striatum/lts/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.599717 snudda-2.0.1/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      582 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/fix_indexing.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19983 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/lts_morp_2019-11-07_centered_no_axon.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      289 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    32177 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/modulation.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.599717 snudda-2.0.1/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/morphologies/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19983 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/morphologies/lts_morp_2019-11-07_centered_noAxon.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3895 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      406 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/protocols.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.599717 snudda-2.0.1/snudda/data/synapses/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.599717 snudda-2.0.1/snudda/data/synapses/example_data/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   127486 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/example_data/10_MSN12_GBZ_CC_H20.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      644 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/example_data/M1LH-contra_dSPN.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1623 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/formatinfo.txt
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      238 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/pair_pulse_experiment_data.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.607718 snudda-2.0.1/snudda/data/synapses/striatum/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    15242 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/striatum/M1LH_Analysis_191001.h5-parameters-FS.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3494 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/striatum/M1LH_Analysis_191001.h5-parameters-LTS.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    50601 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/striatum/M1LH_Analysis_191001.h5-parameters-MS.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8102 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-CHAT.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    18630 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-FS.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    11632 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-LTS.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    97843 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-MS.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    39622 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/striatum/PlanertFitting-DD-tmgaba-fit.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    39725 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/striatum/PlanertFitting-DI-tmgaba-fit.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    39238 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/striatum/PlanertFitting-FD-tmgaba-fit.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    39455 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/striatum/PlanertFitting-FI-tmgaba-fit.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    39599 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/striatum/PlanertFitting-ID-tmgaba-fit.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    39624 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/striatum/PlanertFitting-II-tmgaba-fit.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3535 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-CHAT.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    28148 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-FS.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2277 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-LTS.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   140662 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-MS.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19848 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/striatum/TH_Analysis_191001.h5-parameters-CHAT.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    12939 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/striatum/TH_Analysis_191001.h5-parameters-FS.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   109072 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/striatum/TH_Analysis_191001.h5-parameters-MS.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.607718 snudda-2.0.1/snudda/data/synapses/striatum/partial/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1092 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-DD.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1079 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-DI.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3255 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-FD.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4345 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-FI.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8626 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-ID.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5339 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-II.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1093 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-LI.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      413 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/data/synapses/striatum/readme.txt
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.611718 snudda-2.0.1/snudda/data/synapses/v1/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     9657 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3482 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-LTS-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7077 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8386 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    13748 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    12464 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-LTS-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    13368 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8270 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19238 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8345 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-LTS-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    11827 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    11864 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    16683 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-CH-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     9737 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    15282 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    17464 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      751 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/v1/trace_table.txt-DD-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      738 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/v1/trace_table.txt-DI-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2213 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/v1/trace_table.txt-FD-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2943 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/v1/trace_table.txt-FI-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5839 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/v1/trace_table.txt-ID-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3600 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/data/synapses/v1/trace_table.txt-II-model-parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.611718 snudda-2.0.1/snudda/detect/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      138 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/detect/__init__.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   160627 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/detect/detect.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    16327 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/detect/project.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    15655 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/detect/projection_detection.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   102843 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/detect/prune.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      801 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/help.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.611718 snudda-2.0.1/snudda/init/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)       89 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/init/__init__.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    87135 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/init/init.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     6308 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/init/init_config.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3141 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/init/init_custom.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2308 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/init/init_wojtek.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.611718 snudda-2.0.1/snudda/input/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)       95 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/input/__init__.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   100929 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/input/input.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    88189 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/input/input_tuning.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2809 2023-02-15 16:15:38.000000 snudda-2.0.1/snudda/input/inspectinput.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5177 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/input/time_varying_input.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1088 2023-02-15 16:15:38.000000 snudda-2.0.1/snudda/input/virtual_input.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.611718 snudda-2.0.1/snudda/neuromodulation/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      177 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/neuromodulation/__init__.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2679 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/neuromodulation/modulation.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7470 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/neuromodulation/modulation_network.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4495 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/neuromodulation/modulation_synapse.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7179 2023-02-15 16:15:38.000000 snudda-2.0.1/snudda/neuromodulation/neuromodulation.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    21682 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/neuromodulation/neuromodulation_synapse.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      289 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/neuromodulation/translator.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.615718 snudda-2.0.1/snudda/neurons/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      203 2023-02-15 16:15:38.000000 snudda-2.0.1/snudda/neurons/__init__.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1617 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/neurons/index_tree.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    34627 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/neurons/morphology_data.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    18379 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/neurons/neuron_model_extended.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    54245 2023-02-15 16:15:38.000000 snudda-2.0.1/snudda/neurons/neuron_morphology.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    24463 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/neurons/neuron_morphology_extended.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    22279 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/neurons/neuron_prototype.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.615718 snudda-2.0.1/snudda/place/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      258 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/place/__init__.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    18897 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/place/bend_morphologies.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2747 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/place/create_cube_mesh.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3196 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/place/create_slice_mesh.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    64170 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/place/place.py
--rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)     4639 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/place/projection_map_finder.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    55259 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/place/region_mesh.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    12474 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/place/region_mesh_redux.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7724 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/place/rotation.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5670 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/place/volumetric_mapping.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.619719 snudda-2.0.1/snudda/plotting/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.619719 snudda-2.0.1/snudda/plotting/Blender/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)        0 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/plotting/Blender/__init__.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.619719 snudda-2.0.1/snudda/plotting/Blender/io_mesh_swc/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      661 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/plotting/Blender/io_mesh_swc/__init__.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     6031 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/plotting/Blender/io_mesh_swc/operator_swc_import.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.619719 snudda-2.0.1/snudda/plotting/Blender/visualisation/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)        0 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/plotting/Blender/visualisation/__init__.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1980 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/plotting/Blender/visualisation/drawHyperCubeSomas.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1429 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/plotting/Blender/visualisation/drawHyperCubeSomasRender.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1217 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/plotting/Blender/visualisation/drawHyperCubeSomasWithLTS.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4086 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/plotting/Blender/visualisation/makeNeuronCube.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4371 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/plotting/Blender/visualisation/makeNeuronCubeSubset.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5497 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/plotting/Blender/visualisation/visualiseCubeOfNeuronsWhiteBackground.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5109 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/plotting/Blender/visualisation/visualiseStriatumNeurons.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5250 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/plotting/Blender/visualisation/visualiseStriatumNeuronsWithSynapses.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    25826 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/plotting/Blender/visualisation/visualise_network.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    10089 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/plotting/Blender/visualisation/visualise_network_old.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5344 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/plotting/Blender/visualisation/visualise_touch_detection.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      455 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/plotting/__init__.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3414 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/plotting/plotLTSdensity.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2740 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/plotting/plot_connection_matrix.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     9403 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/plotting/plot_connectivity.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8658 2022-11-03 09:16:18.000000 snudda-2.0.1/snudda/plotting/plot_cross_correlogram.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2869 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/plotting/plot_degeneration.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     6935 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/plotting/plot_degeneration_and_growth.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1280 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/plotting/plot_density.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2782 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/plotting/plot_density_slice.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3415 2022-11-03 09:16:18.000000 snudda-2.0.1/snudda/plotting/plot_distance_statistics.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5368 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/plotting/plot_input.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    16837 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/plotting/plot_input_locations.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    12281 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/plotting/plot_network.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3081 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/plotting/plot_network_simulation.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     9755 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/plotting/plot_neuron_voltage.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3703 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/plotting/plot_node_benchmark.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8027 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/plotting/plot_period_experiment.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3397 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/plotting/plot_size_benchmark.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    25242 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/plotting/plot_spike_raster_v2.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5166 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/plotting/plot_synapse_distance.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19341 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/plotting/plot_traces.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.619719 snudda-2.0.1/snudda/prune/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      226 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/prune/__init__.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.619719 snudda-2.0.1/snudda/simulate/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)       52 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/simulate/__init__.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    24960 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/simulate/model_current_injections.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    22316 2023-02-15 16:15:38.000000 snudda-2.0.1/snudda/simulate/network_pair_pulse_simulation.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3729 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/simulate/nrn_simulator_parallel.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    23548 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/simulate/pair_recording.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    13557 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/simulate/save_network_recording.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    87170 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/simulate/simulate.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.623719 snudda-2.0.1/snudda/utils/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      437 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/utils/__init__.py
--rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)    22275 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/utils/ablate_network.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5292 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/utils/benchmark_logging.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1238 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/utils/cleanup.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2534 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/utils/clone_neurons.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    16656 2023-06-27 13:26:59.000000 snudda-2.0.1/snudda/utils/conv_hurt.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1230 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/utils/create_parameter_morphology_input_map.py
--rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)    17809 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/utils/cut.py
--rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)     7564 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/utils/export_connection_matrix.py
--rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)     4516 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/utils/export_eroded_connection_matrix.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    52278 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/utils/export_sonata.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2324 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/utils/fake_load.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)       80 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/utils/input_helper.py
--rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)    51896 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/utils/load.py
--rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)    16320 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/utils/load_network_simulation.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      278 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/utils/memory.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      593 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/utils/numpy_encoder.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      185 2022-09-19 09:45:08.000000 snudda-2.0.1/snudda/utils/pip_upgrade.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3931 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/utils/reposition_neurons.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4907 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/utils/snudda_path.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    38640 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/utils/swap_to_degenerated_morphologies.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    20793 2024-03-20 06:52:32.000000 snudda-2.0.1/snudda/utils/swap_to_degenerated_morphologies_extended.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-03-20 06:53:12.519711 snudda-2.0.1/snudda.egg-info/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4233 2024-03-20 06:53:12.000000 snudda-2.0.1/snudda.egg-info/PKG-INFO
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    24051 2024-03-20 06:53:12.000000 snudda-2.0.1/snudda.egg-info/SOURCES.txt
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)        1 2024-03-20 06:53:12.000000 snudda-2.0.1/snudda.egg-info/dependency_links.txt
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      417 2024-03-20 06:53:12.000000 snudda-2.0.1/snudda.egg-info/entry_points.txt
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      189 2024-03-20 06:53:12.000000 snudda-2.0.1/snudda.egg-info/requires.txt
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)        7 2024-03-20 06:53:12.000000 snudda-2.0.1/snudda.egg-info/top_level.txt
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:29:00.045733 snudda-2.0.2/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    35149 2022-09-19 09:45:08.000000 snudda-2.0.2/LICENSE
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4233 2024-04-16 09:29:00.041733 snudda-2.0.2/PKG-INFO
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3756 2023-06-27 13:26:59.000000 snudda-2.0.2/README.md
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)       38 2024-04-16 09:29:00.045733 snudda-2.0.2/setup.cfg
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2696 2023-06-27 13:26:59.000000 snudda-2.0.2/setup.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.925736 snudda-2.0.2/snudda/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      506 2024-04-16 09:28:27.000000 snudda-2.0.2/snudda/__init__.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.925736 snudda-2.0.2/snudda/analyse/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      199 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/analyse/__init__.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    98425 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/analyse/analyse.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7932 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/analyse/analyse_gap_junction_coupling.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3250 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/analyse/analyse_input.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5575 2022-11-03 09:16:18.000000 snudda-2.0.2/snudda/analyse/analyse_neuroinformatics2020.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8656 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/analyse/analyse_spike_trains.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19907 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/analyse/analyse_striatum.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5992 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/analyse/analyse_synapse_location.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7575 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/analyse/analyse_topology.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    12380 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/analyse/analyse_topology_activity.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     6277 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/analyse/spike_time_tiling_coefficient.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    12884 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/cli.py
+-rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)    38049 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/core.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.921736 snudda-2.0.2/snudda/data/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.921736 snudda-2.0.2/snudda/data/InputAxons/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.925736 snudda-2.0.2/snudda/data/InputAxons/Cortex/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   432939 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/InputAxons/Cortex/AA0059.swc
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.929736 snudda-2.0.2/snudda/data/InputAxons/Cortex/Reg10/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   900524 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/InputAxons/Cortex/Reg10/AA0059-reg10.swc
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.929736 snudda-2.0.2/snudda/data/InputAxons/Cortex/Reg15/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   597398 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/InputAxons/Cortex/Reg15/AA0059-reg15.swc
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.929736 snudda-2.0.2/snudda/data/InputAxons/Cortex/Reg5/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1809577 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/InputAxons/Cortex/Reg5/AA0059-reg5.swc
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.933736 snudda-2.0.2/snudda/data/InputAxons/GPe2Striatum/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1269 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/InputAxons/GPe2Striatum/example-projection-config.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   444324 2023-02-15 16:15:38.000000 snudda-2.0.2/snudda/data/InputAxons/GPe2Striatum/prototypical-axon.swc
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.933736 snudda-2.0.2/snudda/data/InputAxons/Thalamus/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   464916 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/InputAxons/Thalamus/AA0054.swc
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.933736 snudda-2.0.2/snudda/data/InputAxons/Thalamus/Reg10/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   513478 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/InputAxons/Thalamus/Reg10/AA0054-reg10.swc
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.937736 snudda-2.0.2/snudda/data/InputAxons/Thalamus/Reg15/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   346069 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/InputAxons/Thalamus/Reg15/AA0054-reg15.swc
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.937736 snudda-2.0.2/snudda/data/InputAxons/Thalamus/Reg5/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1022637 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/InputAxons/Thalamus/Reg5/AA0054-reg5.swc
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.941736 snudda-2.0.2/snudda/data/density/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    87096 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/density/1001_STRd_Sst_dens.csv
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    89256 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/density/1001_STRd_Sst_dens_smooth.csv
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    74510 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/density/252_STRd_Chat_dens.csv
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    77158 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/density/252_STRd_Chat_dens_smooth.csv
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    94468 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/density/352_STRd_Drd1_dens.csv
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    95346 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/density/352_STRd_Drd1_dens_smooth.csv
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    95932 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/density/72109410_STRd_Adora2a_dens.csv
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    96454 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/density/72109410_STRd_Adora2a_dens_smooth.csv
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    77578 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/density/79556738_STRd_Pvalb_dens.csv
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    79756 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/density/79556738_STRd_Pvalb_dens_smooth.csv
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1132 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/density/combine_densities.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  2256264 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/density/dorsal_striatum_density.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.921736 snudda-2.0.2/snudda/data/experiment_config/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.945736 snudda-2.0.2/snudda/data/experiment_config/pair_recording/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      477 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/data/experiment_config/pair_recording/experiment-config-1.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      591 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/data/experiment_config/pair_recording/experiment-config-2.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      645 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/data/experiment_config/pair_recording/experiment-config-3.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      646 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/data/experiment_config/pair_recording/experiment-config-4.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      461 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/data/experiment_config/pair_recording/experiment-config-5.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      605 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/data/experiment_config/pair_recording/experiment-config-6.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      695 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/data/experiment_config/pair_recording/experiment-config-7.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.945736 snudda-2.0.2/snudda/data/images/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    52659 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/images/snudda-video-qr-code.png
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.949735 snudda-2.0.2/snudda/data/input_config/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.949735 snudda-2.0.2/snudda/data/input_config/Kim2019/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3035 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/data/input_config/Kim2019/Kim et al., 2019 - Henry Yin - Extended2a.csv
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    25975 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/data/input_config/Kim2019/Kim et al., 2019 - Henry Yin - Extended2a.xlsx
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1433 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/data/input_config/Kim2019/get_experimental_firing_freq.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5834 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/input_config/external-input-dSTR-scaled-v2.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5827 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/input_config/external-input-dSTR-scaled-v3.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5827 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/input_config/external-input-dSTR-scaled-v3b.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5834 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/input_config/external-input-dSTR-scaled-v4-cluster-test.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5811 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/input_config/external-input-dSTR-scaled-v4.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5843 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/input_config/external-input-dSTR-scaled.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      768 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/input_config/input-tinytest-ChIN.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1831 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/input_config/input-tinytest-Channel-Activation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1803 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/input_config/input-tinytest-channel-1.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1803 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/input_config/input-tinytest-channel-2.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5395 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/input_config/input-tinytest-v7.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5409 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/input_config/input-tinytest-v8.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5547 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/input_config/input-tinytest-v9-freq-vectors.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5709 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/data/input_config/input-v10-scaled.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      506 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/input_config/input_output_dspn_template_IC.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.961735 snudda-2.0.2/snudda/data/mesh/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    88391 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/data/mesh/GPe-left.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    92643 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/data/mesh/GPe-right.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   192511 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/mesh/GPe.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    28420 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/data/mesh/GPi-left.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    30275 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/data/mesh/GPi-right.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    60912 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/mesh/GPi.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    32645 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/data/mesh/SNc-left.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    33562 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/data/mesh/SNc-right.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    68536 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/mesh/SNc.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    77916 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/data/mesh/SNr-left.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    78090 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/data/mesh/SNr-right.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   164445 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/mesh/SNr.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    20912 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/data/mesh/STN-left.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    21156 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/data/mesh/STN-right.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    44005 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/mesh/STN.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   507113 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/data/mesh/Striatum-d-left.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   531971 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/data/mesh/Striatum-d-right.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1069021 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/mesh/Striatum-d.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1733004 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/mesh/Striatum-dorsal-left-hemisphere.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1813629 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/mesh/Striatum-dorsal-right-hemisphere.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   363232 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/data/mesh/Striatum-v-left.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   374672 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/data/mesh/Striatum-v-right.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   763087 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/mesh/Striatum-v.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      828 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/data/mesh/cut_mesh.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2358 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/mesh/get_mesh.ipynb
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.921736 snudda-2.0.2/snudda/data/nest/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.961735 snudda-2.0.2/snudda/data/nest/models/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      272 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/nest/models/FS.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      278 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/nest/models/dSPN.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      276 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/nest/models/iSPN.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.965735 snudda-2.0.2/snudda/data/nest/synapses/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)       25 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/nest/synapses/excitatory.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)       25 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/nest/synapses/excitatory_distal.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)       25 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/nest/synapses/excitatory_proximal.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)       25 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/nest/synapses/excitatory_soma.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)       25 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/nest/synapses/inhibitory.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)       25 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/nest/synapses/inhibitory_distal.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)       25 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/nest/synapses/inhibitory_proximal.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)       25 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/nest/synapses/inhibitory_soma.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.921736 snudda-2.0.2/snudda/data/neurons/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.973735 snudda-2.0.2/snudda/data/neurons/mechanisms/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2111 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/Im_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1352 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/Kv3_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1375 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/NO.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2598 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/bk_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2511 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/bk_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2744 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/bk_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4351 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/ca_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1282 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/cadyn_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1609 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/cadyn_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4561 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/cal12_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4723 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/cal13_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2871 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/cal_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1663 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/caldyn_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3256 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/can_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4517 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/can_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2986 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/cap_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2424 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/caq_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2485 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/caq_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2814 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/car_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3855 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/car_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2413 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/cat32_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2414 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/cat33_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1074 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/concACh.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1084 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/concDA.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      907 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/concDAfile.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3903 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/hcn12_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2247 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/hd_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3028 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/im_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3099 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/it_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3406 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/kaf_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3407 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/kaf_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4335 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/kaf_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3334 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/kas_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3932 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/kas_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1189 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/kcnq_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1179 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/kdb_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1781 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/kdr_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2810 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/kdr_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1725 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/kdr_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1230 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/kdrb_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3594 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/kir23_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3595 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/kir23_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1665 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/kir2_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3586 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/kir_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4151 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/kir_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1254 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/kv2_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2679 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/kv4_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3111 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/na2_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3677 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/na3_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3119 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/na_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2833 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/naf_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3043 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/naf_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3245 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/naf_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      377 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/par_ggap.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1909 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/sk_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1896 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/sk_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1896 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/sk_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2370 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/tmampa.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4291 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/tmgabaa.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7671 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/tmglut.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7535 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/tmglut_M1RH_D1.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8029 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/tmglut_double.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1336 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/tmnmda.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1026 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms/vecevent.mod
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.981735 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1352 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/Kv3_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2225 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/bk_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2511 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/bk_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2744 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/bk_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3998 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/ca_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1282 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/cadyn_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1609 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/cadyn_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3249 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/cal12_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3452 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/cal13_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1800 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/cal_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1663 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/caldyn_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3256 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/can_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3256 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/can_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1686 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/cap_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2424 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/caq_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2485 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/caq_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2814 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/car_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2814 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/car_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2413 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/cat32_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2414 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/cat33_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1164 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/h_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2855 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/hcn12_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1724 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/im_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2061 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/it_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2364 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/kaf_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2993 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/kaf_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2292 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/kas_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2886 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/kas_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1189 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/kcnq_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1781 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/kdr_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1725 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/kdr_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1250 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/kdrbca1_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      605 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/kir2_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2543 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/kir_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2882 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/kir_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1254 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/kv2_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1642 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/kv4_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2082 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/na2_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2637 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/na3n_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2076 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/na_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1791 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/naf_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1980 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/naf_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      377 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/par_ggap.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1909 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/sk_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1896 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/sk_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1896 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/sk_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2370 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/tmampa.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2893 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/tmgabaa.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5773 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/tmglut.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1336 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/tmnmda.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1026 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/vecevent.mod
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.921736 snudda-2.0.2/snudda/data/neurons/striatum/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.921736 snudda-2.0.2/snudda/data/neurons/striatum/chin/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.981735 snudda-2.0.2/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      215 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    89390 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    69404 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/optim_chin_morph_renamed2019-11-08.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3194 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      403 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/protocols.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.921736 snudda-2.0.2/snudda/data/neurons/striatum/dspn/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.985735 snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   673225 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/WT-0728MSN01-cor-rep-ax.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      936 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/fix_indexing.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    92361 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    94239 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/modulationDAACh.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    80017 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.985735 snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   600711 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/WT-P270-20-15ak-cor.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    92630 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59991 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.989735 snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   183549 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/21-6-DE-cor-rep-ax.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    92630 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59972 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.989735 snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   660197 2023-02-15 16:15:38.000000 snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/WT-1215MSN03-cor-rep-ax2.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    92630 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    99934 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.921736 snudda-2.0.2/snudda/data/neurons/striatum/fs/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.993734 snudda-2.0.2/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   620377 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/MTC180800A-IDB-cor-rep.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      244 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1226312 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    21438 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:29:00.001734 snudda-2.0.2/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  4918863 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/DR-rat-Mar-13-08-1-536-R-cor-rep.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      244 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1226312 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19567 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:29:00.005734 snudda-2.0.2/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   620377 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/MTC180800A-IDB-cor-rep.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      244 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1226312 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5366 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:29:00.009734 snudda-2.0.2/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   826139 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/MTC251001A-IDB-cor-rep.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      244 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1226312 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5354 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.921736 snudda-2.0.2/snudda/data/neurons/striatum/ispn/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:29:00.009734 snudda-2.0.2/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1013802 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/51-5-DE-cor-rep-ax.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59125 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    69979 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:29:00.013734 snudda-2.0.2/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1153456 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/WT-MSN1-cor-rep-ax.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59125 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59905 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:29:00.013734 snudda-2.0.2/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   587827 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/WT-P270-09-15ak-cor.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59125 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    49989 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:29:00.013734 snudda-2.0.2/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   254041 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/46-3-DE-cor-rep-ax.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59125 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    29994 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.921736 snudda-2.0.2/snudda/data/neurons/striatum/lts/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:29:00.017734 snudda-2.0.2/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      582 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/fix_indexing.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19983 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/lts_morp_2019-11-07_centered_no_axon.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      289 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    32177 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/modulation.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:29:00.017734 snudda-2.0.2/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/morphologies/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19983 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/morphologies/lts_morp_2019-11-07_centered_noAxon.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3895 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      406 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/protocols.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:29:00.017734 snudda-2.0.2/snudda/data/synapses/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:29:00.017734 snudda-2.0.2/snudda/data/synapses/example_data/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   127486 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/example_data/10_MSN12_GBZ_CC_H20.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      644 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/example_data/M1LH-contra_dSPN.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1623 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/formatinfo.txt
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      238 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/pair_pulse_experiment_data.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:29:00.021734 snudda-2.0.2/snudda/data/synapses/striatum/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    15242 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/striatum/M1LH_Analysis_191001.h5-parameters-FS.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3494 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/striatum/M1LH_Analysis_191001.h5-parameters-LTS.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    50601 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/striatum/M1LH_Analysis_191001.h5-parameters-MS.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8102 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-CHAT.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    18630 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-FS.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    11632 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-LTS.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    97843 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-MS.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    39622 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/striatum/PlanertFitting-DD-tmgaba-fit.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    39725 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/striatum/PlanertFitting-DI-tmgaba-fit.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    39238 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/striatum/PlanertFitting-FD-tmgaba-fit.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    39455 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/striatum/PlanertFitting-FI-tmgaba-fit.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    39599 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/striatum/PlanertFitting-ID-tmgaba-fit.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    39624 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/striatum/PlanertFitting-II-tmgaba-fit.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3535 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-CHAT.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    28148 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-FS.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2277 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-LTS.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   140662 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-MS.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19848 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/striatum/TH_Analysis_191001.h5-parameters-CHAT.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    12939 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/striatum/TH_Analysis_191001.h5-parameters-FS.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   109072 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/striatum/TH_Analysis_191001.h5-parameters-MS.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:29:00.021734 snudda-2.0.2/snudda/data/synapses/striatum/partial/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1092 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-DD.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1079 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-DI.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3255 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-FD.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4345 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-FI.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8626 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-ID.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5339 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-II.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1093 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-LI.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      413 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/data/synapses/striatum/readme.txt
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:29:00.025734 snudda-2.0.2/snudda/data/synapses/v1/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     9657 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3482 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-LTS-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7077 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8386 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    13748 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    12464 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-LTS-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    13368 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8270 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19238 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8345 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-LTS-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    11827 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    11864 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    16683 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-CH-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     9737 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    15282 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    17464 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      751 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/v1/trace_table.txt-DD-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      738 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/v1/trace_table.txt-DI-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2213 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/v1/trace_table.txt-FD-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2943 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/v1/trace_table.txt-FI-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5839 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/v1/trace_table.txt-ID-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3600 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/data/synapses/v1/trace_table.txt-II-model-parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:29:00.025734 snudda-2.0.2/snudda/detect/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      138 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/detect/__init__.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   160627 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/detect/detect.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    16327 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/detect/project.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    15655 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/detect/projection_detection.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   102843 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/detect/prune.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      801 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/help.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:29:00.029734 snudda-2.0.2/snudda/init/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)       89 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/init/__init__.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    87135 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/init/init.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     6308 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/init/init_config.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3141 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/init/init_custom.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2308 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/init/init_wojtek.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:29:00.029734 snudda-2.0.2/snudda/input/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)       95 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/input/__init__.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   100929 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/input/input.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    88189 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/input/input_tuning.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2809 2023-02-15 16:15:38.000000 snudda-2.0.2/snudda/input/inspectinput.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5177 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/input/time_varying_input.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1088 2023-02-15 16:15:38.000000 snudda-2.0.2/snudda/input/virtual_input.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:29:00.029734 snudda-2.0.2/snudda/neuromodulation/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      177 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/neuromodulation/__init__.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2679 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/neuromodulation/modulation.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7470 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/neuromodulation/modulation_network.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4495 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/neuromodulation/modulation_synapse.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7179 2023-02-15 16:15:38.000000 snudda-2.0.2/snudda/neuromodulation/neuromodulation.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    21682 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/neuromodulation/neuromodulation_synapse.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      289 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/neuromodulation/translator.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:29:00.029734 snudda-2.0.2/snudda/neurons/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      203 2023-02-15 16:15:38.000000 snudda-2.0.2/snudda/neurons/__init__.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1617 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/neurons/index_tree.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    34627 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/neurons/morphology_data.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    18379 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/neurons/neuron_model_extended.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    54245 2023-02-15 16:15:38.000000 snudda-2.0.2/snudda/neurons/neuron_morphology.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    24463 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/neurons/neuron_morphology_extended.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    22279 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/neurons/neuron_prototype.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:29:00.033733 snudda-2.0.2/snudda/place/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      258 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/place/__init__.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    18897 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/place/bend_morphologies.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2747 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/place/create_cube_mesh.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3196 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/place/create_slice_mesh.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    64170 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/place/place.py
+-rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)     4639 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/place/projection_map_finder.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    55259 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/place/region_mesh.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    12474 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/place/region_mesh_redux.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7724 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/place/rotation.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5670 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/place/volumetric_mapping.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:29:00.037733 snudda-2.0.2/snudda/plotting/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:29:00.037733 snudda-2.0.2/snudda/plotting/Blender/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)        0 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/plotting/Blender/__init__.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:29:00.037733 snudda-2.0.2/snudda/plotting/Blender/io_mesh_swc/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      661 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/plotting/Blender/io_mesh_swc/__init__.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     6031 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/plotting/Blender/io_mesh_swc/operator_swc_import.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:29:00.037733 snudda-2.0.2/snudda/plotting/Blender/visualisation/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)        0 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/plotting/Blender/visualisation/__init__.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1980 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/plotting/Blender/visualisation/drawHyperCubeSomas.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1429 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/plotting/Blender/visualisation/drawHyperCubeSomasRender.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1217 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/plotting/Blender/visualisation/drawHyperCubeSomasWithLTS.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4086 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/plotting/Blender/visualisation/makeNeuronCube.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4371 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/plotting/Blender/visualisation/makeNeuronCubeSubset.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5497 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/plotting/Blender/visualisation/visualiseCubeOfNeuronsWhiteBackground.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5109 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/plotting/Blender/visualisation/visualiseStriatumNeurons.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5250 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/plotting/Blender/visualisation/visualiseStriatumNeuronsWithSynapses.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    25826 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/plotting/Blender/visualisation/visualise_network.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    10089 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/plotting/Blender/visualisation/visualise_network_old.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5344 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/plotting/Blender/visualisation/visualise_touch_detection.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      455 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/plotting/__init__.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3414 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/plotting/plotLTSdensity.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2740 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/plotting/plot_connection_matrix.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     9403 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/plotting/plot_connectivity.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8658 2022-11-03 09:16:18.000000 snudda-2.0.2/snudda/plotting/plot_cross_correlogram.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2869 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/plotting/plot_degeneration.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     6935 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/plotting/plot_degeneration_and_growth.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1280 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/plotting/plot_density.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2782 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/plotting/plot_density_slice.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3415 2022-11-03 09:16:18.000000 snudda-2.0.2/snudda/plotting/plot_distance_statistics.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5368 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/plotting/plot_input.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    16837 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/plotting/plot_input_locations.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    12281 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/plotting/plot_network.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3081 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/plotting/plot_network_simulation.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     9755 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/plotting/plot_neuron_voltage.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3703 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/plotting/plot_node_benchmark.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8027 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/plotting/plot_period_experiment.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3397 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/plotting/plot_size_benchmark.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    28628 2024-04-16 09:28:27.000000 snudda-2.0.2/snudda/plotting/plot_spike_raster_v2.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5166 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/plotting/plot_synapse_distance.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19341 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/plotting/plot_traces.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:29:00.037733 snudda-2.0.2/snudda/prune/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      226 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/prune/__init__.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:29:00.041733 snudda-2.0.2/snudda/simulate/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)       52 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/simulate/__init__.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    24960 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/simulate/model_current_injections.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    22316 2023-02-15 16:15:38.000000 snudda-2.0.2/snudda/simulate/network_pair_pulse_simulation.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3729 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/simulate/nrn_simulator_parallel.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    23548 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/simulate/pair_recording.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    13557 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/simulate/save_network_recording.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    87170 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/simulate/simulate.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:29:00.041733 snudda-2.0.2/snudda/utils/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      437 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/utils/__init__.py
+-rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)    22275 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/utils/ablate_network.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5292 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/utils/benchmark_logging.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1238 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/utils/cleanup.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2534 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/utils/clone_neurons.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    16656 2023-06-27 13:26:59.000000 snudda-2.0.2/snudda/utils/conv_hurt.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1230 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/utils/create_parameter_morphology_input_map.py
+-rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)    17809 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/utils/cut.py
+-rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)     7827 2024-04-16 09:28:27.000000 snudda-2.0.2/snudda/utils/export_connection_matrix.py
+-rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)     4516 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/utils/export_eroded_connection_matrix.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    52278 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/utils/export_sonata.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2324 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/utils/fake_load.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)       80 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/utils/input_helper.py
+-rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)    53240 2024-04-16 09:28:27.000000 snudda-2.0.2/snudda/utils/load.py
+-rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)    16609 2024-04-16 09:28:27.000000 snudda-2.0.2/snudda/utils/load_network_simulation.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      278 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/utils/memory.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      593 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/utils/numpy_encoder.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      185 2022-09-19 09:45:08.000000 snudda-2.0.2/snudda/utils/pip_upgrade.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3931 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/utils/reposition_neurons.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4907 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/utils/snudda_path.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    38640 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/utils/swap_to_degenerated_morphologies.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    20793 2024-03-20 06:52:32.000000 snudda-2.0.2/snudda/utils/swap_to_degenerated_morphologies_extended.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2024-04-16 09:28:59.925736 snudda-2.0.2/snudda.egg-info/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4233 2024-04-16 09:28:59.000000 snudda-2.0.2/snudda.egg-info/PKG-INFO
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    24051 2024-04-16 09:28:59.000000 snudda-2.0.2/snudda.egg-info/SOURCES.txt
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)        1 2024-04-16 09:28:59.000000 snudda-2.0.2/snudda.egg-info/dependency_links.txt
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      417 2024-04-16 09:28:59.000000 snudda-2.0.2/snudda.egg-info/entry_points.txt
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      189 2024-04-16 09:28:59.000000 snudda-2.0.2/snudda.egg-info/requires.txt
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)        7 2024-04-16 09:28:59.000000 snudda-2.0.2/snudda.egg-info/top_level.txt
```

### Comparing `snudda-2.0.1/LICENSE` & `snudda-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/PKG-INFO` & `snudda-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snudda
-Version: 2.0.1
+Version: 2.0.2
 Summary: Create realistic networks of neurons, synapses placed using touch detection between axons and dendrites.
 Home-page: https://github.com/Hjorthmedh/Snudda
 Author: Johannes Hjorth
 Author-email: hjorth@kth.se
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `snudda-2.0.1/README.md` & `snudda-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/setup.py` & `snudda-2.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/analyse/analyse.py` & `snudda-2.0.2/snudda/analyse/analyse.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/analyse/analyse_gap_junction_coupling.py` & `snudda-2.0.2/snudda/analyse/analyse_gap_junction_coupling.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/analyse/analyse_input.py` & `snudda-2.0.2/snudda/analyse/analyse_input.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/analyse/analyse_neuroinformatics2020.py` & `snudda-2.0.2/snudda/analyse/analyse_neuroinformatics2020.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/analyse/analyse_spike_trains.py` & `snudda-2.0.2/snudda/analyse/analyse_spike_trains.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/analyse/analyse_striatum.py` & `snudda-2.0.2/snudda/analyse/analyse_striatum.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/analyse/analyse_synapse_location.py` & `snudda-2.0.2/snudda/analyse/analyse_synapse_location.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/analyse/analyse_topology.py` & `snudda-2.0.2/snudda/analyse/analyse_topology.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/analyse/analyse_topology_activity.py` & `snudda-2.0.2/snudda/analyse/analyse_topology_activity.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/analyse/spike_time_tiling_coefficient.py` & `snudda-2.0.2/snudda/analyse/spike_time_tiling_coefficient.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/cli.py` & `snudda-2.0.2/snudda/cli.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/core.py` & `snudda-2.0.2/snudda/core.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/InputAxons/Cortex/AA0059.swc` & `snudda-2.0.2/snudda/data/InputAxons/Cortex/AA0059.swc`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/InputAxons/Cortex/Reg10/AA0059-reg10.swc` & `snudda-2.0.2/snudda/data/InputAxons/Cortex/Reg10/AA0059-reg10.swc`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/InputAxons/Cortex/Reg15/AA0059-reg15.swc` & `snudda-2.0.2/snudda/data/InputAxons/Cortex/Reg15/AA0059-reg15.swc`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/InputAxons/Cortex/Reg5/AA0059-reg5.swc` & `snudda-2.0.2/snudda/data/InputAxons/Cortex/Reg5/AA0059-reg5.swc`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/InputAxons/GPe2Striatum/example-projection-config.json` & `snudda-2.0.2/snudda/data/InputAxons/GPe2Striatum/example-projection-config.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/InputAxons/GPe2Striatum/prototypical-axon.swc` & `snudda-2.0.2/snudda/data/InputAxons/GPe2Striatum/prototypical-axon.swc`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/InputAxons/Thalamus/AA0054.swc` & `snudda-2.0.2/snudda/data/InputAxons/Thalamus/AA0054.swc`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/InputAxons/Thalamus/Reg10/AA0054-reg10.swc` & `snudda-2.0.2/snudda/data/InputAxons/Thalamus/Reg10/AA0054-reg10.swc`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/InputAxons/Thalamus/Reg15/AA0054-reg15.swc` & `snudda-2.0.2/snudda/data/InputAxons/Thalamus/Reg15/AA0054-reg15.swc`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/InputAxons/Thalamus/Reg5/AA0054-reg5.swc` & `snudda-2.0.2/snudda/data/InputAxons/Thalamus/Reg5/AA0054-reg5.swc`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/density/1001_STRd_Sst_dens.csv` & `snudda-2.0.2/snudda/data/density/1001_STRd_Sst_dens.csv`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/density/1001_STRd_Sst_dens_smooth.csv` & `snudda-2.0.2/snudda/data/density/1001_STRd_Sst_dens_smooth.csv`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/density/252_STRd_Chat_dens.csv` & `snudda-2.0.2/snudda/data/density/252_STRd_Chat_dens.csv`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/density/252_STRd_Chat_dens_smooth.csv` & `snudda-2.0.2/snudda/data/density/252_STRd_Chat_dens_smooth.csv`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/density/352_STRd_Drd1_dens.csv` & `snudda-2.0.2/snudda/data/density/352_STRd_Drd1_dens.csv`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/density/352_STRd_Drd1_dens_smooth.csv` & `snudda-2.0.2/snudda/data/density/352_STRd_Drd1_dens_smooth.csv`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/density/72109410_STRd_Adora2a_dens.csv` & `snudda-2.0.2/snudda/data/density/72109410_STRd_Adora2a_dens.csv`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/density/72109410_STRd_Adora2a_dens_smooth.csv` & `snudda-2.0.2/snudda/data/density/72109410_STRd_Adora2a_dens_smooth.csv`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/density/79556738_STRd_Pvalb_dens.csv` & `snudda-2.0.2/snudda/data/density/79556738_STRd_Pvalb_dens.csv`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/density/79556738_STRd_Pvalb_dens_smooth.csv` & `snudda-2.0.2/snudda/data/density/79556738_STRd_Pvalb_dens_smooth.csv`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/density/combine_densities.py` & `snudda-2.0.2/snudda/data/density/combine_densities.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/density/dorsal_striatum_density.json` & `snudda-2.0.2/snudda/data/density/dorsal_striatum_density.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/experiment_config/pair_recording/experiment-config-2.json` & `snudda-2.0.2/snudda/data/experiment_config/pair_recording/experiment-config-2.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/experiment_config/pair_recording/experiment-config-3.json` & `snudda-2.0.2/snudda/data/experiment_config/pair_recording/experiment-config-3.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/experiment_config/pair_recording/experiment-config-4.json` & `snudda-2.0.2/snudda/data/experiment_config/pair_recording/experiment-config-4.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/experiment_config/pair_recording/experiment-config-6.json` & `snudda-2.0.2/snudda/data/experiment_config/pair_recording/experiment-config-6.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/experiment_config/pair_recording/experiment-config-7.json` & `snudda-2.0.2/snudda/data/experiment_config/pair_recording/experiment-config-7.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/images/snudda-video-qr-code.png` & `snudda-2.0.2/snudda/data/images/snudda-video-qr-code.png`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/input_config/Kim2019/Kim et al., 2019 - Henry Yin - Extended2a.csv` & `snudda-2.0.2/snudda/data/input_config/Kim2019/Kim et al., 2019 - Henry Yin - Extended2a.csv`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/input_config/Kim2019/Kim et al., 2019 - Henry Yin - Extended2a.xlsx` & `snudda-2.0.2/snudda/data/input_config/Kim2019/Kim et al., 2019 - Henry Yin - Extended2a.xlsx`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/input_config/Kim2019/get_experimental_firing_freq.py` & `snudda-2.0.2/snudda/data/input_config/Kim2019/get_experimental_firing_freq.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/input_config/external-input-dSTR-scaled-v2.json` & `snudda-2.0.2/snudda/data/input_config/external-input-dSTR-scaled-v2.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/input_config/external-input-dSTR-scaled-v3.json` & `snudda-2.0.2/snudda/data/input_config/external-input-dSTR-scaled-v3.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/input_config/external-input-dSTR-scaled-v3b.json` & `snudda-2.0.2/snudda/data/input_config/external-input-dSTR-scaled-v3b.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/input_config/external-input-dSTR-scaled-v4-cluster-test.json` & `snudda-2.0.2/snudda/data/input_config/external-input-dSTR-scaled-v4-cluster-test.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/input_config/external-input-dSTR-scaled-v4.json` & `snudda-2.0.2/snudda/data/input_config/external-input-dSTR-scaled-v4.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/input_config/external-input-dSTR-scaled.json` & `snudda-2.0.2/snudda/data/input_config/external-input-dSTR-scaled.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/input_config/input-tinytest-ChIN.json` & `snudda-2.0.2/snudda/data/input_config/input-tinytest-ChIN.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/input_config/input-tinytest-Channel-Activation.json` & `snudda-2.0.2/snudda/data/input_config/input-tinytest-Channel-Activation.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/input_config/input-tinytest-channel-1.json` & `snudda-2.0.2/snudda/data/input_config/input-tinytest-channel-1.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/input_config/input-tinytest-channel-2.json` & `snudda-2.0.2/snudda/data/input_config/input-tinytest-channel-2.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/input_config/input-tinytest-v7.json` & `snudda-2.0.2/snudda/data/input_config/input-tinytest-v7.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/input_config/input-tinytest-v8.json` & `snudda-2.0.2/snudda/data/input_config/input-tinytest-v8.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/input_config/input-tinytest-v9-freq-vectors.json` & `snudda-2.0.2/snudda/data/input_config/input-tinytest-v9-freq-vectors.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/input_config/input-v10-scaled.json` & `snudda-2.0.2/snudda/data/input_config/input-v10-scaled.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/mesh/GPe-left.obj` & `snudda-2.0.2/snudda/data/mesh/GPe-left.obj`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/mesh/GPe-right.obj` & `snudda-2.0.2/snudda/data/mesh/GPe-right.obj`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/mesh/GPe.obj` & `snudda-2.0.2/snudda/data/mesh/GPe.obj`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/mesh/GPi-left.obj` & `snudda-2.0.2/snudda/data/mesh/GPi-left.obj`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/mesh/GPi-right.obj` & `snudda-2.0.2/snudda/data/mesh/GPi-right.obj`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/mesh/GPi.obj` & `snudda-2.0.2/snudda/data/mesh/GPi.obj`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/mesh/SNc-left.obj` & `snudda-2.0.2/snudda/data/mesh/SNc-left.obj`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/mesh/SNc-right.obj` & `snudda-2.0.2/snudda/data/mesh/SNc-right.obj`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/mesh/SNc.obj` & `snudda-2.0.2/snudda/data/mesh/SNc.obj`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/mesh/SNr-left.obj` & `snudda-2.0.2/snudda/data/mesh/SNr-left.obj`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/mesh/SNr-right.obj` & `snudda-2.0.2/snudda/data/mesh/SNr-right.obj`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/mesh/SNr.obj` & `snudda-2.0.2/snudda/data/mesh/SNr.obj`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/mesh/STN-left.obj` & `snudda-2.0.2/snudda/data/mesh/STN-left.obj`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/mesh/STN-right.obj` & `snudda-2.0.2/snudda/data/mesh/STN-right.obj`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/mesh/STN.obj` & `snudda-2.0.2/snudda/data/mesh/STN.obj`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/mesh/Striatum-d-left.obj` & `snudda-2.0.2/snudda/data/mesh/Striatum-d-left.obj`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/mesh/Striatum-d-right.obj` & `snudda-2.0.2/snudda/data/mesh/Striatum-d-right.obj`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/mesh/Striatum-d.obj` & `snudda-2.0.2/snudda/data/mesh/Striatum-d.obj`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/mesh/Striatum-dorsal-left-hemisphere.obj` & `snudda-2.0.2/snudda/data/mesh/Striatum-dorsal-left-hemisphere.obj`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/mesh/Striatum-dorsal-right-hemisphere.obj` & `snudda-2.0.2/snudda/data/mesh/Striatum-dorsal-right-hemisphere.obj`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/mesh/Striatum-v-left.obj` & `snudda-2.0.2/snudda/data/mesh/Striatum-v-left.obj`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/mesh/Striatum-v-right.obj` & `snudda-2.0.2/snudda/data/mesh/Striatum-v-right.obj`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/mesh/Striatum-v.obj` & `snudda-2.0.2/snudda/data/mesh/Striatum-v.obj`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/mesh/cut_mesh.py` & `snudda-2.0.2/snudda/data/mesh/cut_mesh.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/mesh/get_mesh.ipynb` & `snudda-2.0.2/snudda/data/mesh/get_mesh.ipynb`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/Im_ms.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/Im_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/Kv3_ch.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/Kv3_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/NO.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/NO.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/bk_ch.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/bk_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/bk_fs.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/bk_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/bk_ms.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/bk_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/ca_ch.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/ca_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/cadyn_fs.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/cadyn_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/cadyn_ms.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/cadyn_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/cal12_ms.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/cal12_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/cal13_ms.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/cal13_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/cal_ch.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/cal_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/caldyn_ms.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/caldyn_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/can_fs.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/can_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/can_ms.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/can_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/cap_ch.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/cap_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/caq_fs.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/caq_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/caq_ms.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/caq_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/car_fs.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/car_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/car_ms.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/car_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/cat32_ms.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/cat32_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/cat33_ms.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/cat33_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/concACh.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/concACh.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/concDA.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/concDA.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/concDAfile.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/concDAfile.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/hcn12_ch.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/hcn12_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/hd_lts.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/hd_lts.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/im_lts.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/im_lts.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/it_lts.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/it_lts.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/kaf_fs.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/kaf_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/kaf_lts.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/kaf_lts.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/kaf_ms.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/kaf_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/kas_fs.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/kas_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/kas_ms.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/kas_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/kcnq_ch.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/kcnq_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/kdb_lts.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/kdb_lts.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/kdr_fs.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/kdr_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/kdr_lts.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/kdr_lts.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/kdr_ms.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/kdr_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/kdrb_lts.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/kdrb_lts.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/kir23_ch.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/kir23_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/kir23_lts.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/kir23_lts.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/kir2_ch.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/kir2_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/kir_fs.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/kir_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/kir_ms.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/kir_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/kv2_ch.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/kv2_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/kv4_ch.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/kv4_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/na2_ch.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/na2_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/na3_lts.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/na3_lts.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/na_ch.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/na_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/naf_fs.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/naf_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/naf_lts.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/naf_lts.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/naf_ms.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/naf_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/sk_ch.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/sk_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/sk_fs.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/sk_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/sk_ms.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/sk_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/tmampa.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/tmampa.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/tmgabaa.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/tmgabaa.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/tmglut.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/tmglut.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/tmglut_M1RH_D1.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/tmglut_M1RH_D1.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/tmglut_double.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/tmglut_double.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/tmnmda.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/tmnmda.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms/vecevent.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms/vecevent.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/Kv3_ch.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/Kv3_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/bk_ch.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/bk_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/bk_fs.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/bk_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/bk_ms.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/bk_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/ca_ch.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/ca_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/cadyn_fs.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/cadyn_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/cadyn_ms.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/cadyn_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/cal12_ms.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/cal12_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/cal13_ms.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/cal13_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/cal_ch.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/cal_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/caldyn_ms.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/caldyn_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/can_fs.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/can_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/can_ms.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/can_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/cap_ch.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/cap_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/caq_fs.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/caq_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/caq_ms.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/caq_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/car_fs.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/car_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/car_ms.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/car_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/cat32_ms.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/cat32_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/cat33_ms.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/cat33_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/h_lts.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/h_lts.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/hcn12_ch.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/hcn12_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/im_lts.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/im_lts.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/it_lts.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/it_lts.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/kaf_fs.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/kaf_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/kaf_ms.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/kaf_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/kas_fs.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/kas_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/kas_ms.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/kas_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/kcnq_ch.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/kcnq_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/kdr_fs.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/kdr_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/kdr_ms.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/kdr_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/kdrbca1_lts.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/kdrbca1_lts.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/kir2_ch.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/kir2_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/kir_fs.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/kir_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/kir_ms.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/kir_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/kv2_ch.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/kv2_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/kv4_ch.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/kv4_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/na2_ch.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/na2_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/na3n_lts.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/na3n_lts.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/na_ch.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/na_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/naf_fs.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/naf_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/naf_ms.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/naf_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/sk_ch.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/sk_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/sk_fs.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/sk_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/sk_ms.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/sk_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/tmampa.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/tmampa.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/tmgabaa.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/tmgabaa.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/tmglut.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/tmglut.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/tmnmda.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/tmnmda.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/mechanisms.OLD/vecevent.mod` & `snudda-2.0.2/snudda/data/neurons/mechanisms.OLD/vecevent.mod`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/modulation.json` & `snudda-2.0.2/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/optim_chin_morph_renamed2019-11-08.swc` & `snudda-2.0.2/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/optim_chin_morph_renamed2019-11-08.swc`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/parameters.json` & `snudda-2.0.2/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/WT-0728MSN01-cor-rep-ax.swc` & `snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/WT-0728MSN01-cor-rep-ax.swc`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/fix_indexing.py` & `snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/fix_indexing.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/mechanisms.json` & `snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/mechanisms.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/modulation.json` & `snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/modulationDAACh.json` & `snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/modulationDAACh.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/parameters.json` & `snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/WT-P270-20-15ak-cor.swc` & `snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/WT-P270-20-15ak-cor.swc`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/mechanisms.json` & `snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/mechanisms.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/modulation.json` & `snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/parameters.json` & `snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/21-6-DE-cor-rep-ax.swc` & `snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/21-6-DE-cor-rep-ax.swc`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/mechanisms.json` & `snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/mechanisms.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/modulation.json` & `snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/parameters.json` & `snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/WT-1215MSN03-cor-rep-ax2.swc` & `snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/WT-1215MSN03-cor-rep-ax2.swc`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/mechanisms.json` & `snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/mechanisms.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/modulation.json` & `snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/parameters.json` & `snudda-2.0.2/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/MTC180800A-IDB-cor-rep.swc` & `snudda-2.0.2/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/MTC180800A-IDB-cor-rep.swc`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/modulation.json` & `snudda-2.0.2/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/parameters.json` & `snudda-2.0.2/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/DR-rat-Mar-13-08-1-536-R-cor-rep.swc` & `snudda-2.0.2/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/DR-rat-Mar-13-08-1-536-R-cor-rep.swc`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/modulation.json` & `snudda-2.0.2/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/parameters.json` & `snudda-2.0.2/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/MTC180800A-IDB-cor-rep.swc` & `snudda-2.0.2/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/MTC180800A-IDB-cor-rep.swc`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/modulation.json` & `snudda-2.0.2/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/parameters.json` & `snudda-2.0.2/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/MTC251001A-IDB-cor-rep.swc` & `snudda-2.0.2/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/MTC251001A-IDB-cor-rep.swc`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/modulation.json` & `snudda-2.0.2/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/parameters.json` & `snudda-2.0.2/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/51-5-DE-cor-rep-ax.swc` & `snudda-2.0.2/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/51-5-DE-cor-rep-ax.swc`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/mechanisms.json` & `snudda-2.0.2/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/mechanisms.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/modulation.json` & `snudda-2.0.2/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/parameters.json` & `snudda-2.0.2/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/WT-MSN1-cor-rep-ax.swc` & `snudda-2.0.2/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/WT-MSN1-cor-rep-ax.swc`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/mechanisms.json` & `snudda-2.0.2/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/mechanisms.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/modulation.json` & `snudda-2.0.2/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/parameters.json` & `snudda-2.0.2/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/WT-P270-09-15ak-cor.swc` & `snudda-2.0.2/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/WT-P270-09-15ak-cor.swc`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/mechanisms.json` & `snudda-2.0.2/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/mechanisms.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/modulation.json` & `snudda-2.0.2/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/parameters.json` & `snudda-2.0.2/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/46-3-DE-cor-rep-ax.swc` & `snudda-2.0.2/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/46-3-DE-cor-rep-ax.swc`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/mechanisms.json` & `snudda-2.0.2/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/mechanisms.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/modulation.json` & `snudda-2.0.2/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/parameters.json` & `snudda-2.0.2/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/fix_indexing.py` & `snudda-2.0.2/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/fix_indexing.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/lts_morp_2019-11-07_centered_no_axon.swc` & `snudda-2.0.2/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/lts_morp_2019-11-07_centered_no_axon.swc`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/modulation.json` & `snudda-2.0.2/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/morphologies/lts_morp_2019-11-07_centered_noAxon.swc` & `snudda-2.0.2/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/morphologies/lts_morp_2019-11-07_centered_noAxon.swc`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/parameters.json` & `snudda-2.0.2/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/example_data/10_MSN12_GBZ_CC_H20.json` & `snudda-2.0.2/snudda/data/synapses/example_data/10_MSN12_GBZ_CC_H20.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/example_data/M1LH-contra_dSPN.json` & `snudda-2.0.2/snudda/data/synapses/example_data/M1LH-contra_dSPN.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/formatinfo.txt` & `snudda-2.0.2/snudda/data/synapses/formatinfo.txt`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/striatum/M1LH_Analysis_191001.h5-parameters-FS.json` & `snudda-2.0.2/snudda/data/synapses/striatum/M1LH_Analysis_191001.h5-parameters-FS.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/striatum/M1LH_Analysis_191001.h5-parameters-LTS.json` & `snudda-2.0.2/snudda/data/synapses/striatum/M1LH_Analysis_191001.h5-parameters-LTS.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/striatum/M1LH_Analysis_191001.h5-parameters-MS.json` & `snudda-2.0.2/snudda/data/synapses/striatum/M1LH_Analysis_191001.h5-parameters-MS.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-CHAT.json` & `snudda-2.0.2/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-CHAT.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-FS.json` & `snudda-2.0.2/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-FS.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-LTS.json` & `snudda-2.0.2/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-LTS.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-MS.json` & `snudda-2.0.2/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-MS.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/striatum/PlanertFitting-DD-tmgaba-fit.json` & `snudda-2.0.2/snudda/data/synapses/striatum/PlanertFitting-DD-tmgaba-fit.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/striatum/PlanertFitting-DI-tmgaba-fit.json` & `snudda-2.0.2/snudda/data/synapses/striatum/PlanertFitting-DI-tmgaba-fit.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/striatum/PlanertFitting-FD-tmgaba-fit.json` & `snudda-2.0.2/snudda/data/synapses/striatum/PlanertFitting-FD-tmgaba-fit.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/striatum/PlanertFitting-FI-tmgaba-fit.json` & `snudda-2.0.2/snudda/data/synapses/striatum/PlanertFitting-FI-tmgaba-fit.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/striatum/PlanertFitting-ID-tmgaba-fit.json` & `snudda-2.0.2/snudda/data/synapses/striatum/PlanertFitting-ID-tmgaba-fit.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/striatum/PlanertFitting-II-tmgaba-fit.json` & `snudda-2.0.2/snudda/data/synapses/striatum/PlanertFitting-II-tmgaba-fit.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-CHAT.json` & `snudda-2.0.2/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-CHAT.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-FS.json` & `snudda-2.0.2/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-FS.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-LTS.json` & `snudda-2.0.2/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-LTS.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-MS.json` & `snudda-2.0.2/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-MS.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/striatum/TH_Analysis_191001.h5-parameters-CHAT.json` & `snudda-2.0.2/snudda/data/synapses/striatum/TH_Analysis_191001.h5-parameters-CHAT.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/striatum/TH_Analysis_191001.h5-parameters-FS.json` & `snudda-2.0.2/snudda/data/synapses/striatum/TH_Analysis_191001.h5-parameters-FS.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/striatum/TH_Analysis_191001.h5-parameters-MS.json` & `snudda-2.0.2/snudda/data/synapses/striatum/TH_Analysis_191001.h5-parameters-MS.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-DD.json` & `snudda-2.0.2/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-DD.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-DI.json` & `snudda-2.0.2/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-DI.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-FD.json` & `snudda-2.0.2/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-FD.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-FI.json` & `snudda-2.0.2/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-FI.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-ID.json` & `snudda-2.0.2/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-ID.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-II.json` & `snudda-2.0.2/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-II.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-LI.json` & `snudda-2.0.2/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-LI.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json` & `snudda-2.0.2/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-LTS-require-H20-model-parameters.json` & `snudda-2.0.2/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-LTS-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json` & `snudda-2.0.2/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json` & `snudda-2.0.2/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json` & `snudda-2.0.2/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-LTS-require-H20-model-parameters.json` & `snudda-2.0.2/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-LTS-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json` & `snudda-2.0.2/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json` & `snudda-2.0.2/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json` & `snudda-2.0.2/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-LTS-require-H20-model-parameters.json` & `snudda-2.0.2/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-LTS-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json` & `snudda-2.0.2/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json` & `snudda-2.0.2/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-CH-require-H20-model-parameters.json` & `snudda-2.0.2/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-CH-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json` & `snudda-2.0.2/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json` & `snudda-2.0.2/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json` & `snudda-2.0.2/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/v1/trace_table.txt-DD-model-parameters.json` & `snudda-2.0.2/snudda/data/synapses/v1/trace_table.txt-DD-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/v1/trace_table.txt-DI-model-parameters.json` & `snudda-2.0.2/snudda/data/synapses/v1/trace_table.txt-DI-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/v1/trace_table.txt-FD-model-parameters.json` & `snudda-2.0.2/snudda/data/synapses/v1/trace_table.txt-FD-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/v1/trace_table.txt-FI-model-parameters.json` & `snudda-2.0.2/snudda/data/synapses/v1/trace_table.txt-FI-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/v1/trace_table.txt-ID-model-parameters.json` & `snudda-2.0.2/snudda/data/synapses/v1/trace_table.txt-ID-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/data/synapses/v1/trace_table.txt-II-model-parameters.json` & `snudda-2.0.2/snudda/data/synapses/v1/trace_table.txt-II-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/detect/detect.py` & `snudda-2.0.2/snudda/detect/detect.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/detect/project.py` & `snudda-2.0.2/snudda/detect/project.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/detect/projection_detection.py` & `snudda-2.0.2/snudda/detect/projection_detection.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/detect/prune.py` & `snudda-2.0.2/snudda/detect/prune.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/help.py` & `snudda-2.0.2/snudda/help.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/init/init.py` & `snudda-2.0.2/snudda/init/init.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/init/init_config.py` & `snudda-2.0.2/snudda/init/init_config.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/init/init_custom.py` & `snudda-2.0.2/snudda/init/init_custom.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/init/init_wojtek.py` & `snudda-2.0.2/snudda/init/init_wojtek.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/input/input.py` & `snudda-2.0.2/snudda/input/input.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/input/input_tuning.py` & `snudda-2.0.2/snudda/input/input_tuning.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/input/inspectinput.py` & `snudda-2.0.2/snudda/input/inspectinput.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/input/time_varying_input.py` & `snudda-2.0.2/snudda/input/time_varying_input.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/input/virtual_input.py` & `snudda-2.0.2/snudda/input/virtual_input.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/neuromodulation/modulation.py` & `snudda-2.0.2/snudda/neuromodulation/modulation.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/neuromodulation/modulation_network.py` & `snudda-2.0.2/snudda/neuromodulation/modulation_network.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/neuromodulation/modulation_synapse.py` & `snudda-2.0.2/snudda/neuromodulation/modulation_synapse.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/neuromodulation/neuromodulation.py` & `snudda-2.0.2/snudda/neuromodulation/neuromodulation.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/neuromodulation/neuromodulation_synapse.py` & `snudda-2.0.2/snudda/neuromodulation/neuromodulation_synapse.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/neurons/index_tree.py` & `snudda-2.0.2/snudda/neurons/index_tree.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/neurons/morphology_data.py` & `snudda-2.0.2/snudda/neurons/morphology_data.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/neurons/neuron_model_extended.py` & `snudda-2.0.2/snudda/neurons/neuron_model_extended.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/neurons/neuron_morphology.py` & `snudda-2.0.2/snudda/neurons/neuron_morphology.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/neurons/neuron_morphology_extended.py` & `snudda-2.0.2/snudda/neurons/neuron_morphology_extended.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/neurons/neuron_prototype.py` & `snudda-2.0.2/snudda/neurons/neuron_prototype.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/place/bend_morphologies.py` & `snudda-2.0.2/snudda/place/bend_morphologies.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/place/create_cube_mesh.py` & `snudda-2.0.2/snudda/place/create_cube_mesh.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/place/create_slice_mesh.py` & `snudda-2.0.2/snudda/place/create_slice_mesh.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/place/place.py` & `snudda-2.0.2/snudda/place/place.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/place/projection_map_finder.py` & `snudda-2.0.2/snudda/place/projection_map_finder.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/place/region_mesh.py` & `snudda-2.0.2/snudda/place/region_mesh.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/place/region_mesh_redux.py` & `snudda-2.0.2/snudda/place/region_mesh_redux.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/place/rotation.py` & `snudda-2.0.2/snudda/place/rotation.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/place/volumetric_mapping.py` & `snudda-2.0.2/snudda/place/volumetric_mapping.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/plotting/Blender/io_mesh_swc/__init__.py` & `snudda-2.0.2/snudda/plotting/Blender/io_mesh_swc/__init__.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/plotting/Blender/io_mesh_swc/operator_swc_import.py` & `snudda-2.0.2/snudda/plotting/Blender/io_mesh_swc/operator_swc_import.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/plotting/Blender/visualisation/drawHyperCubeSomas.py` & `snudda-2.0.2/snudda/plotting/Blender/visualisation/drawHyperCubeSomas.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/plotting/Blender/visualisation/drawHyperCubeSomasRender.py` & `snudda-2.0.2/snudda/plotting/Blender/visualisation/drawHyperCubeSomasRender.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/plotting/Blender/visualisation/drawHyperCubeSomasWithLTS.py` & `snudda-2.0.2/snudda/plotting/Blender/visualisation/drawHyperCubeSomasWithLTS.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/plotting/Blender/visualisation/makeNeuronCube.py` & `snudda-2.0.2/snudda/plotting/Blender/visualisation/makeNeuronCube.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/plotting/Blender/visualisation/makeNeuronCubeSubset.py` & `snudda-2.0.2/snudda/plotting/Blender/visualisation/makeNeuronCubeSubset.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/plotting/Blender/visualisation/visualiseCubeOfNeuronsWhiteBackground.py` & `snudda-2.0.2/snudda/plotting/Blender/visualisation/visualiseCubeOfNeuronsWhiteBackground.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/plotting/Blender/visualisation/visualiseStriatumNeurons.py` & `snudda-2.0.2/snudda/plotting/Blender/visualisation/visualiseStriatumNeurons.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/plotting/Blender/visualisation/visualiseStriatumNeuronsWithSynapses.py` & `snudda-2.0.2/snudda/plotting/Blender/visualisation/visualiseStriatumNeuronsWithSynapses.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/plotting/Blender/visualisation/visualise_network.py` & `snudda-2.0.2/snudda/plotting/Blender/visualisation/visualise_network.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/plotting/Blender/visualisation/visualise_network_old.py` & `snudda-2.0.2/snudda/plotting/Blender/visualisation/visualise_network_old.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/plotting/Blender/visualisation/visualise_touch_detection.py` & `snudda-2.0.2/snudda/plotting/Blender/visualisation/visualise_touch_detection.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/plotting/plotLTSdensity.py` & `snudda-2.0.2/snudda/plotting/plotLTSdensity.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/plotting/plot_connection_matrix.py` & `snudda-2.0.2/snudda/plotting/plot_connection_matrix.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/plotting/plot_connectivity.py` & `snudda-2.0.2/snudda/plotting/plot_connectivity.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/plotting/plot_cross_correlogram.py` & `snudda-2.0.2/snudda/plotting/plot_cross_correlogram.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/plotting/plot_degeneration.py` & `snudda-2.0.2/snudda/plotting/plot_degeneration.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/plotting/plot_degeneration_and_growth.py` & `snudda-2.0.2/snudda/plotting/plot_degeneration_and_growth.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/plotting/plot_density.py` & `snudda-2.0.2/snudda/plotting/plot_density.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/plotting/plot_density_slice.py` & `snudda-2.0.2/snudda/plotting/plot_density_slice.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/plotting/plot_distance_statistics.py` & `snudda-2.0.2/snudda/plotting/plot_distance_statistics.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/plotting/plot_input.py` & `snudda-2.0.2/snudda/plotting/plot_input.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/plotting/plot_input_locations.py` & `snudda-2.0.2/snudda/plotting/plot_input_locations.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/plotting/plot_network.py` & `snudda-2.0.2/snudda/plotting/plot_network.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/plotting/plot_network_simulation.py` & `snudda-2.0.2/snudda/plotting/plot_network_simulation.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/plotting/plot_neuron_voltage.py` & `snudda-2.0.2/snudda/plotting/plot_neuron_voltage.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/plotting/plot_node_benchmark.py` & `snudda-2.0.2/snudda/plotting/plot_node_benchmark.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/plotting/plot_period_experiment.py` & `snudda-2.0.2/snudda/plotting/plot_period_experiment.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/plotting/plot_size_benchmark.py` & `snudda-2.0.2/snudda/plotting/plot_size_benchmark.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/plotting/plot_spike_raster_v2.py` & `snudda-2.0.2/snudda/plotting/plot_spike_raster_v2.py`

 * *Files 9% similar despite different names*

```diff
@@ -350,50 +350,78 @@
 
         if show_figure:
             plt.ion()
             plt.show()
 
         return ax
 
-    def plot_spike_histogram(self, population_id=None,
+    def plot_spike_histogram(self, population_id=None, neuron_type=None,
                              skip_time=0, end_time=None, fig_size=None, bin_size=50e-3,
                              fig_file=None, ax=None, label_text=None, show_figure=True, save_figure=True, colour=None,
-                             linestyle="-", legend_loc="best"):
+                             linestyle="-", legend_loc="best", title=None):
 
         if population_id is None:
             population_id = self.snudda_load.get_neuron_population_units(return_set=True)
 
+        if neuron_type is not None:
+
+            if type(neuron_type) != list:
+                neuron_type = [neuron_type]
+
+            keep_neuron_id = set()
+            for nt in neuron_type:
+                keep_neuron_id |= set(self.snudda_load.get_neuron_id_of_type(neuron_type=nt))
+
+            print(f"Processing {len(keep_neuron_id)} neurons of type {neuron_type}")
+        else:
+            keep_neuron_id = None
+
         self.make_figures_directory()
 
         plt.rcParams.update({'font.size': 24,
                              'xtick.labelsize': 20,
                              'ytick.labelsize': 20,
                              'legend.loc': legend_loc})
 
         if ax is None:
             fig = plt.figure(figsize=fig_size)
             ax = fig.add_subplot()
         
-        pop_members = OrderedDict()
-        pop_spikes = OrderedDict()
+        pop_members = dict()
+        pop_spikes = dict()
 
         if np.issubdtype(type(population_id), np.integer):
             population_id = np.array([population_id])
 
         for pid in population_id:
-            pop_members[pid] = self.snudda_load.get_population_unit_members(pid)
+            members = self.snudda_load.get_population_unit_members(pid)
+
+            if keep_neuron_id is not None:
+                members = np.array(list(set(members) & keep_neuron_id))
+
+            if len(members) == 0:
+                # No members, skip it
+                continue
+
+            pop_members[pid] = members
 
             spikes = self.snudda_simulation_load.get_spikes(pop_members[pid])
             pop_spikes[pid] = self.snudda_simulation_load.merge_spikes(spikes)[:, 0]
 
         if end_time is None:
             end_time = self.snudda_simulation_load.get_time()[-1]
 
-        bins = np.arange(skip_time, end_time+bin_size/2, bin_size)
-        weights = [np.full(y.shape, 1/(len(x)*bin_size)) for x, y in zip(pop_members.values(), pop_spikes.values())]
+        try:
+            bins = np.arange(skip_time, end_time+bin_size/2, bin_size)
+            weights = [np.full(y.shape, 1/(len(x)*bin_size)) for x, y in zip(pop_members.values(), pop_spikes.values())]
+        except:
+            import traceback
+            print(traceback.format_exc())
+            import pdb
+            pdb.set_trace()
 
         if label_text is None:
             label_text = ""
             
         N, bins, patches = ax.hist(x=pop_spikes.values(), bins=bins, weights=weights, linewidth=3, linestyle=linestyle,
                                    histtype="step", color=colour,
                                    label=[f"{label_text}{x}" for x in pop_spikes.keys()])
@@ -402,14 +430,17 @@
             for patch, col in zip(patches, colour):
                 patch[0].set_facecolor(col)
 
         plt.xlabel("Time (s)", fontsize=20)
         plt.ylabel("Frequency (Hz)", fontsize=20)
         ax.legend()
 
+        if title:
+            plt.title(title)
+
         if fig_file is None:
             fig_file = os.path.join(self.figure_path,
                                     f"spike-frequency-pop-units{'-'.join([f'{x}' for x in pop_members.keys()])}.pdf")
         else:
             fig_file = os.path.join(self.figure_path, fig_file)
 
         if save_figure:
@@ -419,14 +450,81 @@
 
         if show_figure:
             plt.ion()
             plt.show()
 
         return ax
 
+    # Use this to plot a histogram for an arbitrary group of neurons specified with neuron_id
+    def plot_group_spike_histogram(self, neuron_id=None,
+                                    skip_time=0, end_time=None, fig_size=None, bin_size=50e-3,
+                                    fig_file=None, ax=None, label_text=None, show_figure=True, save_figure=True, colour=None,
+                                    linestyle="-", legend_loc="best", title=None):
+
+        self.make_figures_directory()
+
+        plt.rcParams.update({'font.size': 24,
+                             'xtick.labelsize': 20,
+                             'ytick.labelsize': 20,
+                             'legend.loc': legend_loc})
+
+        if ax is None:
+            fig = plt.figure(figsize=fig_size)
+            ax = fig.add_subplot()
+
+        spikes = self.snudda_simulation_load.get_spikes(neuron_id)
+        spikes = self.snudda_simulation_load.merge_spikes(spikes)[:, 0]
+
+        if end_time is None:
+            end_time = self.snudda_simulation_load.get_time()[-1]
+
+        bins = np.arange(skip_time, end_time + bin_size / 2, bin_size)
+        weights = 1 / (len(neuron_id) * bin_size)
+
+        if label_text is None:
+            label_text = ""
+
+        try:
+            N, bins, patches = ax.hist(x=spikes, bins=bins, weights=np.full(spikes.shape, weights), linewidth=3, linestyle=linestyle,
+                                       histtype="step", color=colour,
+                                       label=label_text)
+        except:
+            import traceback
+            print(traceback.format_exc())
+            import pdb
+            pdb.set_trace()
+
+        if type(colour) == list:
+            for patch, col in zip(patches, colour):
+                patch[0].set_facecolor(col)
+
+        plt.xlabel("Time (s)", fontsize=20)
+        plt.ylabel("Frequency (Hz)", fontsize=20)
+        ax.legend()
+
+        if title:
+            plt.title(title)
+
+        if fig_file is None:
+            fig_file = os.path.join(self.figure_path,
+                                    f"spike-frequency-for-group.pdf")
+        else:
+            fig_file = os.path.join(self.figure_path, fig_file)
+
+        if save_figure:
+            print(f"Saving figure {fig_file}")
+            plt.tight_layout()
+            plt.savefig(fig_file, dpi=300)
+
+        if show_figure:
+            plt.ion()
+            plt.show()
+
+        return ax
+
     def plot_spike_raster(self, type_order=None, skip_time=0, end_time=None, fig_size=None, fig_file=None,
                           time_range=None):
 
         self.make_figures_directory()
 
         plt.rcParams.update({'font.size': 24,
                              'xtick.labelsize': 20,
@@ -614,15 +712,14 @@
         ax.set_xticks(x + width, x_labels)
         ax.legend(loc='upper left', ncols=3)
         ax.set_ylim(0, 250)
 
         plt.show()
 
 
-
 if __name__ == "__main__":
     from argparse import ArgumentParser
 
     parser = ArgumentParser("Scatter plot")
     parser.add_argument("network_path", type=str, help="Network path")
 
     args = parser.parse_args()
```

### Comparing `snudda-2.0.1/snudda/plotting/plot_synapse_distance.py` & `snudda-2.0.2/snudda/plotting/plot_synapse_distance.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/plotting/plot_traces.py` & `snudda-2.0.2/snudda/plotting/plot_traces.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/simulate/model_current_injections.py` & `snudda-2.0.2/snudda/simulate/model_current_injections.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/simulate/network_pair_pulse_simulation.py` & `snudda-2.0.2/snudda/simulate/network_pair_pulse_simulation.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/simulate/nrn_simulator_parallel.py` & `snudda-2.0.2/snudda/simulate/nrn_simulator_parallel.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/simulate/pair_recording.py` & `snudda-2.0.2/snudda/simulate/pair_recording.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/simulate/save_network_recording.py` & `snudda-2.0.2/snudda/simulate/save_network_recording.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/simulate/simulate.py` & `snudda-2.0.2/snudda/simulate/simulate.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/utils/ablate_network.py` & `snudda-2.0.2/snudda/utils/ablate_network.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/utils/benchmark_logging.py` & `snudda-2.0.2/snudda/utils/benchmark_logging.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/utils/cleanup.py` & `snudda-2.0.2/snudda/utils/cleanup.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/utils/clone_neurons.py` & `snudda-2.0.2/snudda/utils/clone_neurons.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/utils/conv_hurt.py` & `snudda-2.0.2/snudda/utils/conv_hurt.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/utils/create_parameter_morphology_input_map.py` & `snudda-2.0.2/snudda/utils/create_parameter_morphology_input_map.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/utils/cut.py` & `snudda-2.0.2/snudda/utils/cut.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/utils/export_connection_matrix.py` & `snudda-2.0.2/snudda/utils/export_connection_matrix.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,21 +45,23 @@
 
         if self.save_sparse:
             x_pos, y_pos = np.where(self.con_mat)
             sparse_data = np.zeros((len(x_pos), 3), dtype=int)
             for idx, (x, y) in enumerate(zip(x_pos, y_pos)):
                 sparse_data[idx, :] = [x, y, self.con_mat[x, y]]
 
-            np.savetxt(self.out_file, sparse_data, delimiter=",", fmt="%d")
+            # np.savetxt(self.out_file, sparse_data, delimiter=",", fmt="%d")
+            np.save(self.out_file, sparse_data.astype(np.int32))
 
             # Test to verify
             for row in sparse_data:
                 assert self.con_mat[row[0], row[1]] == row[2]
         else:
-            np.savetxt(self.out_file, self.con_mat, delimiter=",", fmt="%d")
+            np.save(self.out_file, self.con_mat.astype(np.int32))
+            # np.savetxt(self.out_file, self.con_mat, delimiter=",", fmt="%d")
 
         print("Writing " + self.out_file_meta)
         with open(self.out_file_meta, "w") as f_out_meta:
             for i, (nt, nn, p, mf, pu) in enumerate(zip(self.neuron_type, self.neuron_name, self.pos, self.neuron_morph,
                                                         self.population_unit)):
                 s = "%d,%s,%s,%f,%f,%f,%s, %d\n" % (i, nt, nn, p[0], p[1], p[2], mf, pu)
                 f_out_meta.write(s)
@@ -119,31 +121,34 @@
 
         axon_dend_distance = self.create_axon_dend_distance_matrix()
 
         if plot:
             self.plot_matrix(axon_dend_distance, hide_nan=True)
 
         save_matrix = axon_dend_distance.copy()
-        save_matrix[np.isnan(save_matrix)] = -1
+        save_matrix[np.isnan(save_matrix)] = np.inf
 
-        np.savetxt(delay_file, save_matrix, delimiter=",", fmt="%d")
+        # np.savetxt(delay_file, save_matrix, delimiter=",", fmt="%d")
+        np.save(delay_file, save_matrix.astype(np.float32))
 
     ############################################################################
 
     def save_distance_matrix(self, plot=False):
 
         dist_file = f"{self.out_file}-dist"
         print(f"Writing distance file: {dist_file}")
 
         dist_matrix = self.sl.create_distance_matrix()
 
         if plot:
             self.plot_matrix(dist_matrix)
 
-        np.savetxt(dist_file, dist_matrix, delimiter=",", fmt="%d")
+        np.save(dist_file, dist_matrix.astype(np.float32))
+
+        # np.savetxt(dist_file, dist_matrix, delimiter=",", fmt="%d")
 
     ############################################################################
 
     def create_connection_matrix(self):
 
         """ Creates the connection matrix from the synapse matrix data. """
```

### Comparing `snudda-2.0.1/snudda/utils/export_eroded_connection_matrix.py` & `snudda-2.0.2/snudda/utils/export_eroded_connection_matrix.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/utils/export_sonata.py` & `snudda-2.0.2/snudda/utils/export_sonata.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/utils/fake_load.py` & `snudda-2.0.2/snudda/utils/fake_load.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/utils/load.py` & `snudda-2.0.2/snudda/utils/load.py`

 * *Files 2% similar despite different names*

```diff
@@ -995,26 +995,58 @@
 
             if n_neurons is not None and neuron_ctr >= n_neurons:
                 # Stop iterator if n_neurons are delivered
                 return
 
     ############################################################################
 
-    def create_connection_matrix(self, sparse_matrix=True):
+    def create_connection_matrix(self, sparse_matrix=True, connection_type="synapses"):
 
         if sparse_matrix:
             connection_matrix = sparse.lil_matrix((self.data["num_neurons"], self.data["num_neurons"]), dtype=np.int16)
         else:
             connection_matrix = np.zeros((self.data["num_neurons"], self.data["num_neurons"]), dtype=np.int16)
 
-        for syn_row in self.data["synapses"]:
+        for syn_row in self.data[connection_type]:
             connection_matrix[syn_row[0], syn_row[1]] += 1
 
         return connection_matrix
 
+    def find_neighbours(self, neuron_id, connection_matrix=None, exclude_parent=True):
+
+        if connection_matrix is None:
+            connection_matrix = self.create_connection_matrix(sparse_matrix=False, connection_type="synapses")
+
+        pre_neighbours = set(np.where(np.sum(connection_matrix[:, list(neuron_id)], axis=1))[0])
+        post_neighbours = set(np.where(np.sum(connection_matrix[list(neuron_id), :], axis=0))[0])
+
+        if exclude_parent:
+            parent_id = set(neuron_id)
+            pre_neighbours -= parent_id
+            post_neighbours -= parent_id
+
+        return pre_neighbours, post_neighbours
+
+    def find_neighbours_gap_junctions(self, neuron_id, connection_matrix=None, exclude_parent=True):
+
+        if connection_matrix is None:
+            connection_matrix = self.create_connection_matrix(sparse_matrix=False, connection_type="gap_junctions")
+
+        # This matrix should be symmetric!
+        pre_neighbours = set(np.where(np.sum(connection_matrix[:, list(neuron_id)], axis=1))[0])
+        post_neighbours = set(np.where(np.sum(connection_matrix[list(neuron_id), :], axis=0))[0])
+
+        neighbours = pre_neighbours | post_neighbours
+
+        if exclude_parent:
+            parent_id = set(neuron_id)
+            neighbours -= parent_id
+
+        return neighbours
+
     def create_distance_matrix(self, neuron_id=None, pre_id=None, post_id=None):
 
         if neuron_id is not None and pre_id is not None and post_id is not None:
             raise ValueError("Specify either neuron_id or the two parameters pre_id and post_id.")
 
         if (pre_id is None) ^ (post_id is None):
             raise ValueError("pre_id and post_id must both either be specified, or neither")
```

### Comparing `snudda-2.0.1/snudda/utils/load_network_simulation.py` & `snudda-2.0.2/snudda/utils/load_network_simulation.py`

 * *Files 6% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 
         Args:
             neuron_id : Neuron ID, either integer or list / array
 
         """
 
         if neuron_id is None:
-            spike_data = OrderedDict()
+            spike_data = dict()
             for nid in self.network_simulation_file["neurons"]:
 
                 if "spikes" in self.network_simulation_file[f"neurons/{nid}"]:
                     spike_data[int(nid)] = self.network_simulation_file[f"neurons/{nid}/spikes"][()].copy()
 
             # If all neuronID not represented, add empty
             for nid in self.network_simulation_file["meta_data/id"]:
@@ -112,22 +112,30 @@
         elif np.issubdtype(type(neuron_id), np.integer):
             if str(neuron_id) in self.network_simulation_file["neurons"] \
                     and "spikes" in self.network_simulation_file[f"neurons/{neuron_id}"]:
                 spike_data = self.network_simulation_file[f"neurons/{neuron_id}/spikes"][()].copy()
             else:
                 spike_data = np.array([])
 
+        elif isinstance(neuron_id, np.ndarray) and neuron_id.size == 0:
+            spike_data = dict()
         else:
-            spike_data = OrderedDict()
-            for nid in neuron_id:
-                if str(nid) in self.network_simulation_file["neurons"] \
-                        and "spikes" in self.network_simulation_file[f"neurons/{nid}"]:
-                    spike_data[nid] = self.network_simulation_file[f"neurons/{nid}/spikes"][()].copy()
-                else:
-                    spike_data[nid] = np.array([])
+            spike_data = dict()
+            try:
+                for nid in neuron_id:
+                    if str(nid) in self.network_simulation_file["neurons"] \
+                            and "spikes" in self.network_simulation_file[f"neurons/{nid}"]:
+                        spike_data[nid] = self.network_simulation_file[f"neurons/{nid}/spikes"][()].copy()
+                    else:
+                        spike_data[nid] = np.array([])
+            except:
+                import traceback
+                print(traceback.format_exc())
+                import pdb
+                pdb.set_trace()
 
         return spike_data
 
     def get_frequency(self, neuron_id, time_ranges=None):
 
         # neuron_id must be a list or an array, time_ranges is a list of tuples
```

### Comparing `snudda-2.0.1/snudda/utils/numpy_encoder.py` & `snudda-2.0.2/snudda/utils/numpy_encoder.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/utils/reposition_neurons.py` & `snudda-2.0.2/snudda/utils/reposition_neurons.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/utils/snudda_path.py` & `snudda-2.0.2/snudda/utils/snudda_path.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/utils/swap_to_degenerated_morphologies.py` & `snudda-2.0.2/snudda/utils/swap_to_degenerated_morphologies.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda/utils/swap_to_degenerated_morphologies_extended.py` & `snudda-2.0.2/snudda/utils/swap_to_degenerated_morphologies_extended.py`

 * *Files identical despite different names*

### Comparing `snudda-2.0.1/snudda.egg-info/PKG-INFO` & `snudda-2.0.2/snudda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snudda
-Version: 2.0.1
+Version: 2.0.2
 Summary: Create realistic networks of neurons, synapses placed using touch detection between axons and dendrites.
 Home-page: https://github.com/Hjorthmedh/Snudda
 Author: Johannes Hjorth
 Author-email: hjorth@kth.se
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `snudda-2.0.1/snudda.egg-info/SOURCES.txt` & `snudda-2.0.2/snudda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

