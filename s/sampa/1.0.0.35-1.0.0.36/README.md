# Comparing `tmp/sampa-1.0.0.35.tar.gz` & `tmp/sampa-1.0.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sampa-1.0.0.35.tar", last modified: Tue Apr 16 02:59:16 2024, max compression
+gzip compressed data, was "sampa-1.0.0.36.tar", last modified: Tue Apr 16 11:34:38 2024, max compression
```

## Comparing `sampa-1.0.0.35.tar` & `sampa-1.0.0.36.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 02:59:16.837187 sampa-1.0.0.35/
--rw-rw-rw-   0        0        0       13 2024-04-09 02:21:11.000000 sampa-1.0.0.35/LICENSE.txt
--rw-rw-rw-   0        0        0      288 2024-04-16 02:59:16.838187 sampa-1.0.0.35/PKG-INFO
--rw-rw-rw-   0        0        0       51 2024-04-09 02:20:56.000000 sampa-1.0.0.35/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 02:59:16.331190 sampa-1.0.0.35/sampa/
--rw-rw-rw-   0        0        0       52 2024-04-09 02:21:40.000000 sampa-1.0.0.35/sampa/__init__.py
--rw-rw-rw-   0        0        0     8200 2024-04-16 02:59:02.000000 sampa-1.0.0.35/sampa/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 02:59:16.646187 sampa-1.0.0.35/sampa/src/
--rw-rw-rw-   0        0        0    67521 2024-04-11 11:50:38.000000 sampa-1.0.0.35/sampa/src/HeteroStructure_Generator.py
-drwxrwxrwx   0        0        0        0 2024-04-16 02:59:16.759191 sampa-1.0.0.35/sampa/src/INPUTS/
--rw-rw-rw-   0        0        0      247 2024-04-15 12:14:11.000000 sampa-1.0.0.35/sampa/src/INPUTS/INCAR_bader
--rw-rw-rw-   0        0        0      288 2024-04-15 12:14:24.000000 sampa-1.0.0.35/sampa/src/INPUTS/INCAR_bader.SO
--rw-rw-rw-   0        0        0      242 2024-04-15 12:14:33.000000 sampa-1.0.0.35/sampa/src/INPUTS/INCAR_bands
--rw-rw-rw-   0        0        0      283 2024-04-15 12:14:53.000000 sampa-1.0.0.35/sampa/src/INPUTS/INCAR_bands.SO
--rw-rw-rw-   0        0        0      231 2024-04-15 12:15:02.000000 sampa-1.0.0.35/sampa/src/INPUTS/INCAR_dos
--rw-rw-rw-   0        0        0      272 2024-04-15 12:15:11.000000 sampa-1.0.0.35/sampa/src/INPUTS/INCAR_dos.SO
--rw-rw-rw-   0        0        0      220 2024-04-15 12:15:20.000000 sampa-1.0.0.35/sampa/src/INPUTS/INCAR_relax
--rw-rw-rw-   0        0        0      233 2024-04-15 12:15:33.000000 sampa-1.0.0.35/sampa/src/INPUTS/INCAR_scf
--rw-rw-rw-   0        0        0      274 2024-04-15 12:15:59.000000 sampa-1.0.0.35/sampa/src/INPUTS/INCAR_scf.SO
--rw-rw-rw-   0        0        0      218 2024-04-15 12:16:08.000000 sampa-1.0.0.35/sampa/src/INPUTS/INCAR_xy-scan
--rw-rw-rw-   0        0        0      218 2024-04-15 12:16:19.000000 sampa-1.0.0.35/sampa/src/INPUTS/INCAR_z-scan
-drwxrwxrwx   0        0        0        0 2024-04-16 02:59:16.836249 sampa-1.0.0.35/sampa/src/INPUTS/inputs_VASProcar/
--rw-rw-rw-   0        0        0     4485 2024-03-20 16:04:46.000000 sampa-1.0.0.35/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.bands
--rw-rw-rw-   0        0        0     3123 2024-04-08 15:25:48.000000 sampa-1.0.0.35/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.chgcar
--rw-rw-rw-   0        0        0     2525 2024-03-20 16:04:58.000000 sampa-1.0.0.35/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.dos
--rw-rw-rw-   0        0        0     9603 2024-03-21 16:46:57.000000 sampa-1.0.0.35/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.location
--rw-rw-rw-   0        0        0     1187 2024-03-23 20:35:59.000000 sampa-1.0.0.35/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.locpot
--rw-rw-rw-   0        0        0     6378 2024-03-20 16:05:20.000000 sampa-1.0.0.35/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.orbitals
--rw-rw-rw-   0        0        0     7790 2024-03-20 16:06:00.000000 sampa-1.0.0.35/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.spin
--rw-rw-rw-   0        0        0     3968 2024-04-10 01:37:39.000000 sampa-1.0.0.35/sampa/src/SAMBA_HeteroStructure.input
--rw-rw-rw-   0        0        0     2934 2024-04-15 12:11:24.000000 sampa-1.0.0.35/sampa/src/SAMBA_WorkFlow.input
--rw-rw-rw-   0        0        0     1089 2024-04-10 12:48:10.000000 sampa-1.0.0.35/sampa/src/_info_pseudo.py
--rw-rw-rw-   0        0        0  4715152 2023-08-19 14:41:30.000000 sampa-1.0.0.35/sampa/src/bader
--rw-rw-rw-   0        0        0     4522 2024-04-11 12:25:07.000000 sampa-1.0.0.35/sampa/src/bader_poscar.py
--rw-rw-rw-   0        0        0     2522 2024-04-09 02:22:36.000000 sampa-1.0.0.35/sampa/src/bader_update.py
--rw-rw-rw-   0        0        0     7055 2024-04-09 02:22:30.000000 sampa-1.0.0.35/sampa/src/charge_transfer.py
--rw-rw-rw-   0        0        0     2139 2019-12-02 15:59:08.000000 sampa-1.0.0.35/sampa/src/chgsum.pl
--rw-rw-rw-   0        0        0      325 2024-04-09 02:22:24.000000 sampa-1.0.0.35/sampa/src/contcar_update.py
--rw-rw-rw-   0        0        0      595 2024-04-15 00:29:04.000000 sampa-1.0.0.35/sampa/src/energy_scan.py
--rw-rw-rw-   0        0        0    12994 2024-04-15 11:47:44.000000 sampa-1.0.0.35/sampa/src/job.py
--rw-rw-rw-   0        0        0     6676 2024-04-09 12:37:10.000000 sampa-1.0.0.35/sampa/src/kpoints.py
--rw-rw-rw-   0        0        0    19780 2024-04-15 12:19:21.000000 sampa-1.0.0.35/sampa/src/make_files.py
--rw-rw-rw-   0        0        0     5133 2024-04-16 02:58:43.000000 sampa-1.0.0.35/sampa/src/output.py
--rw-rw-rw-   0        0        0     1048 2024-04-10 01:31:22.000000 sampa-1.0.0.35/sampa/src/potcar.py
--rw-rw-rw-   0        0        0     7559 2024-04-14 20:39:23.000000 sampa-1.0.0.35/sampa/src/xy-scan.py
--rw-rw-rw-   0        0        0     3613 2024-04-16 02:58:14.000000 sampa-1.0.0.35/sampa/src/xy-scan_update.py
--rw-rw-rw-   0        0        0     9026 2024-04-15 14:24:31.000000 sampa-1.0.0.35/sampa/src/z-scan.py
--rw-rw-rw-   0        0        0     3635 2024-04-16 02:53:40.000000 sampa-1.0.0.35/sampa/src/z-scan_update.py
-drwxrwxrwx   0        0        0        0 2024-04-16 02:59:16.376223 sampa-1.0.0.35/sampa.egg-info/
--rw-rw-rw-   0        0        0      288 2024-04-16 02:59:16.000000 sampa-1.0.0.35/sampa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1477 2024-04-16 02:59:16.000000 sampa-1.0.0.35/sampa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 02:59:16.000000 sampa-1.0.0.35/sampa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-04-16 02:59:16.000000 sampa-1.0.0.35/sampa.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2024-04-16 02:59:16.000000 sampa-1.0.0.35/sampa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-16 02:59:16.000000 sampa-1.0.0.35/sampa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      167 2024-04-16 02:59:16.841187 sampa-1.0.0.35/setup.cfg
--rw-rw-rw-   0        0        0      719 2024-04-16 02:58:53.000000 sampa-1.0.0.35/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 11:34:38.515338 sampa-1.0.0.36/
+-rw-rw-rw-   0        0        0       13 2024-04-09 02:21:11.000000 sampa-1.0.0.36/LICENSE.txt
+-rw-rw-rw-   0        0        0      288 2024-04-16 11:34:38.515338 sampa-1.0.0.36/PKG-INFO
+-rw-rw-rw-   0        0        0       51 2024-04-09 02:20:56.000000 sampa-1.0.0.36/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 11:34:38.093466 sampa-1.0.0.36/sampa/
+-rw-rw-rw-   0        0        0       52 2024-04-09 02:21:40.000000 sampa-1.0.0.36/sampa/__init__.py
+-rw-rw-rw-   0        0        0     8200 2024-04-16 11:34:15.000000 sampa-1.0.0.36/sampa/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 11:34:38.374621 sampa-1.0.0.36/sampa/src/
+-rw-rw-rw-   0        0        0    67521 2024-04-11 11:50:38.000000 sampa-1.0.0.36/sampa/src/HeteroStructure_Generator.py
+drwxrwxrwx   0        0        0        0 2024-04-16 11:34:38.452746 sampa-1.0.0.36/sampa/src/INPUTS/
+-rw-rw-rw-   0        0        0      247 2024-04-15 12:14:11.000000 sampa-1.0.0.36/sampa/src/INPUTS/INCAR_bader
+-rw-rw-rw-   0        0        0      288 2024-04-15 12:14:24.000000 sampa-1.0.0.36/sampa/src/INPUTS/INCAR_bader.SO
+-rw-rw-rw-   0        0        0      242 2024-04-15 12:14:33.000000 sampa-1.0.0.36/sampa/src/INPUTS/INCAR_bands
+-rw-rw-rw-   0        0        0      283 2024-04-15 12:14:53.000000 sampa-1.0.0.36/sampa/src/INPUTS/INCAR_bands.SO
+-rw-rw-rw-   0        0        0      231 2024-04-15 12:15:02.000000 sampa-1.0.0.36/sampa/src/INPUTS/INCAR_dos
+-rw-rw-rw-   0        0        0      272 2024-04-15 12:15:11.000000 sampa-1.0.0.36/sampa/src/INPUTS/INCAR_dos.SO
+-rw-rw-rw-   0        0        0      220 2024-04-15 12:15:20.000000 sampa-1.0.0.36/sampa/src/INPUTS/INCAR_relax
+-rw-rw-rw-   0        0        0      233 2024-04-15 12:15:33.000000 sampa-1.0.0.36/sampa/src/INPUTS/INCAR_scf
+-rw-rw-rw-   0        0        0      274 2024-04-15 12:15:59.000000 sampa-1.0.0.36/sampa/src/INPUTS/INCAR_scf.SO
+-rw-rw-rw-   0        0        0      218 2024-04-15 12:16:08.000000 sampa-1.0.0.36/sampa/src/INPUTS/INCAR_xy-scan
+-rw-rw-rw-   0        0        0      218 2024-04-15 12:16:19.000000 sampa-1.0.0.36/sampa/src/INPUTS/INCAR_z-scan
+drwxrwxrwx   0        0        0        0 2024-04-16 11:34:38.515338 sampa-1.0.0.36/sampa/src/INPUTS/inputs_VASProcar/
+-rw-rw-rw-   0        0        0     4485 2024-03-20 16:04:46.000000 sampa-1.0.0.36/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.bands
+-rw-rw-rw-   0        0        0     3123 2024-04-08 15:25:48.000000 sampa-1.0.0.36/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.chgcar
+-rw-rw-rw-   0        0        0     2525 2024-03-20 16:04:58.000000 sampa-1.0.0.36/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.dos
+-rw-rw-rw-   0        0        0     9603 2024-03-21 16:46:57.000000 sampa-1.0.0.36/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.location
+-rw-rw-rw-   0        0        0     1187 2024-03-23 20:35:59.000000 sampa-1.0.0.36/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.locpot
+-rw-rw-rw-   0        0        0     6378 2024-03-20 16:05:20.000000 sampa-1.0.0.36/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.orbitals
+-rw-rw-rw-   0        0        0     7790 2024-03-20 16:06:00.000000 sampa-1.0.0.36/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.spin
+-rw-rw-rw-   0        0        0     3968 2024-04-10 01:37:39.000000 sampa-1.0.0.36/sampa/src/SAMBA_HeteroStructure.input
+-rw-rw-rw-   0        0        0     2934 2024-04-15 12:11:24.000000 sampa-1.0.0.36/sampa/src/SAMBA_WorkFlow.input
+-rw-rw-rw-   0        0        0     1089 2024-04-10 12:48:10.000000 sampa-1.0.0.36/sampa/src/_info_pseudo.py
+-rw-rw-rw-   0        0        0  4715152 2023-08-19 14:41:30.000000 sampa-1.0.0.36/sampa/src/bader
+-rw-rw-rw-   0        0        0     4522 2024-04-11 12:25:07.000000 sampa-1.0.0.36/sampa/src/bader_poscar.py
+-rw-rw-rw-   0        0        0     2522 2024-04-09 02:22:36.000000 sampa-1.0.0.36/sampa/src/bader_update.py
+-rw-rw-rw-   0        0        0     7055 2024-04-09 02:22:30.000000 sampa-1.0.0.36/sampa/src/charge_transfer.py
+-rw-rw-rw-   0        0        0     2139 2019-12-02 15:59:08.000000 sampa-1.0.0.36/sampa/src/chgsum.pl
+-rw-rw-rw-   0        0        0      325 2024-04-09 02:22:24.000000 sampa-1.0.0.36/sampa/src/contcar_update.py
+-rw-rw-rw-   0        0        0      595 2024-04-15 00:29:04.000000 sampa-1.0.0.36/sampa/src/energy_scan.py
+-rw-rw-rw-   0        0        0    12994 2024-04-15 11:47:44.000000 sampa-1.0.0.36/sampa/src/job.py
+-rw-rw-rw-   0        0        0     6676 2024-04-09 12:37:10.000000 sampa-1.0.0.36/sampa/src/kpoints.py
+-rw-rw-rw-   0        0        0    19780 2024-04-15 12:19:21.000000 sampa-1.0.0.36/sampa/src/make_files.py
+-rw-rw-rw-   0        0        0     5133 2024-04-16 02:58:43.000000 sampa-1.0.0.36/sampa/src/output.py
+-rw-rw-rw-   0        0        0     1048 2024-04-10 01:31:22.000000 sampa-1.0.0.36/sampa/src/potcar.py
+-rw-rw-rw-   0        0        0     7559 2024-04-14 20:39:23.000000 sampa-1.0.0.36/sampa/src/xy-scan.py
+-rw-rw-rw-   0        0        0     3635 2024-04-16 11:31:53.000000 sampa-1.0.0.36/sampa/src/xy-scan_update.py
+-rw-rw-rw-   0        0        0     9026 2024-04-15 14:24:31.000000 sampa-1.0.0.36/sampa/src/z-scan.py
+-rw-rw-rw-   0        0        0     3635 2024-04-16 02:53:40.000000 sampa-1.0.0.36/sampa/src/z-scan_update.py
+drwxrwxrwx   0        0        0        0 2024-04-16 11:34:38.124703 sampa-1.0.0.36/sampa.egg-info/
+-rw-rw-rw-   0        0        0      288 2024-04-16 11:34:37.000000 sampa-1.0.0.36/sampa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1477 2024-04-16 11:34:37.000000 sampa-1.0.0.36/sampa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 11:34:37.000000 sampa-1.0.0.36/sampa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-04-16 11:34:37.000000 sampa-1.0.0.36/sampa.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2024-04-16 11:34:37.000000 sampa-1.0.0.36/sampa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-16 11:34:37.000000 sampa-1.0.0.36/sampa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      167 2024-04-16 11:34:38.530876 sampa-1.0.0.36/setup.cfg
+-rw-rw-rw-   0        0        0      719 2024-04-16 11:34:07.000000 sampa-1.0.0.36/setup.py
```

### Comparing `sampa-1.0.0.35/sampa/__main__.py` & `sampa-1.0.0.36/sampa/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pyfiglet
 import shutil
 import time
 import sys
 import os
 
 
-version = '1.0.0.35'
+version = '1.0.0.36'
 
 
 print(" ")
 print("=============================================================")
 print(f'SAMBA v{version} Copyright (C) 2024 ---------------------------')
 print("Closed source: Adalberto Fazzio's research group (Ilum|CNPEM)")
 print("Author: Augusto de Lelis Araujo -----------------------------")
```

### Comparing `sampa-1.0.0.35/sampa/src/HeteroStructure_Generator.py` & `sampa-1.0.0.36/sampa/src/HeteroStructure_Generator.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.35/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.bands` & `sampa-1.0.0.36/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.bands`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.35/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.chgcar` & `sampa-1.0.0.36/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.chgcar`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.35/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.dos` & `sampa-1.0.0.36/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.dos`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.35/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.location` & `sampa-1.0.0.36/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.location`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.35/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.locpot` & `sampa-1.0.0.36/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.locpot`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.35/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.orbitals` & `sampa-1.0.0.36/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.orbitals`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.35/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.spin` & `sampa-1.0.0.36/sampa/src/INPUTS/inputs_VASProcar/input.vasprocar.spin`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.35/sampa/src/SAMBA_HeteroStructure.input` & `sampa-1.0.0.36/sampa/src/SAMBA_HeteroStructure.input`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.35/sampa/src/SAMBA_WorkFlow.input` & `sampa-1.0.0.36/sampa/src/SAMBA_WorkFlow.input`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.35/sampa/src/_info_pseudo.py` & `sampa-1.0.0.36/sampa/src/_info_pseudo.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.35/sampa/src/bader` & `sampa-1.0.0.36/sampa/src/bader`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.35/sampa/src/bader_poscar.py` & `sampa-1.0.0.36/sampa/src/bader_poscar.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.35/sampa/src/bader_update.py` & `sampa-1.0.0.36/sampa/src/bader_update.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.35/sampa/src/charge_transfer.py` & `sampa-1.0.0.36/sampa/src/charge_transfer.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.35/sampa/src/chgsum.pl` & `sampa-1.0.0.36/sampa/src/chgsum.pl`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.35/sampa/src/energy_scan.py` & `sampa-1.0.0.36/sampa/src/energy_scan.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.35/sampa/src/job.py` & `sampa-1.0.0.36/sampa/src/job.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.35/sampa/src/kpoints.py` & `sampa-1.0.0.36/sampa/src/kpoints.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.35/sampa/src/make_files.py` & `sampa-1.0.0.36/sampa/src/make_files.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.35/sampa/src/output.py` & `sampa-1.0.0.36/sampa/src/output.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.35/sampa/src/potcar.py` & `sampa-1.0.0.36/sampa/src/potcar.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.35/sampa/src/xy-scan.py` & `sampa-1.0.0.36/sampa/src/xy-scan.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.35/sampa/src/xy-scan_update.py` & `sampa-1.0.0.36/sampa/src/xy-scan_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 
 file0 = np.loadtxt('energy_scan.txt', dtype=str)
 file0.shape
 #--------------------
 date_xy  = file0[:,0]
-date_E   = file0[:,1]
+date_E   = np.array(file0[:,1],dtype=float)
 E_min    = min(date_E)
 E_max    = max(date_E)
 line     = np.argmin(date_E)
 delta_xy = date_xy[line]
 #===================================================
 shutil.copyfile(str(delta_xy) + '/POSCAR', 'POSCAR')
 #===================================================
```

### Comparing `sampa-1.0.0.35/sampa/src/z-scan.py` & `sampa-1.0.0.36/sampa/src/z-scan.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.35/sampa/src/z-scan_update.py` & `sampa-1.0.0.36/sampa/src/z-scan_update.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.35/sampa.egg-info/SOURCES.txt` & `sampa-1.0.0.36/sampa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.35/setup.py` & `sampa-1.0.0.36/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 import json
 from pathlib import Path
 from typing import Optional
 
 setup(
     name = "sampa",
-    version = "1.0.0.35",
+    version = "1.0.0.36",
     entry_points={'console_scripts': ['sampa = sampa:main']},
     description = "...",
     author = "Augusto de Lelis Araujo", 
     author_email = "augusto-lelis@outlook.com",
     license = "Closed source",
     install_requires=['numpy',
                       'requests',
```

