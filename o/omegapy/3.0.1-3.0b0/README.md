# Comparing `tmp/omegapy-3.0.1.tar.gz` & `tmp/omegapy-3.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omegapy-3.0.1.tar", last modified: Tue Apr 16 09:52:36 2024, max compression
+gzip compressed data, was "omegapy-3.0b0.tar", last modified: Thu Oct 19 05:32:58 2023, max compression
```

## Comparing `omegapy-3.0.1.tar` & `omegapy-3.0b0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:52:36.979098 omegapy-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-16 09:52:28.000000 omegapy-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-04-16 09:52:36.979098 omegapy-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-16 09:52:28.000000 omegapy-3.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:52:36.967098 omegapy-3.0.1/omegapy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:52:36.979098 omegapy-3.0.1/omegapy/OMEGA_dataref/
--rw-r--r--   0 runner    (1001) docker     (127)   143760 2024-04-16 09:52:28.000000 omegapy-3.0.1/omegapy/OMEGA_dataref/OBC_OMEGA_OCT2017.sav
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-04-16 09:52:28.000000 omegapy-3.0.1/omegapy/OMEGA_dataref/boundcur.dat
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-16 09:52:28.000000 omegapy-3.0.1/omegapy/OMEGA_dataref/corrupted_obs.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1495234 2024-04-16 09:52:28.000000 omegapy-3.0.1/omegapy/OMEGA_dataref/cubindex.ref
--rw-r--r--   0 runner    (1001) docker     (127)    49152 2024-04-16 09:52:28.000000 omegapy-3.0.1/omegapy/OMEGA_dataref/flatVIS050701.bin
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-16 09:52:28.000000 omegapy-3.0.1/omegapy/OMEGA_dataref/fond2.dat
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-04-16 09:52:28.000000 omegapy-3.0.1/omegapy/OMEGA_dataref/lambda_0403.dat
--rw-r--r--   0 runner    (1001) docker     (127)    48007 2024-04-16 09:52:28.000000 omegapy-3.0.1/omegapy/OMEGA_dataref/linearC.dat
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-04-16 09:52:28.000000 omegapy-3.0.1/omegapy/OMEGA_dataref/mtf120315_25.dat
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-04-16 09:52:28.000000 omegapy-3.0.1/omegapy/OMEGA_dataref/mtf120315_50.dat
--rw-r--r--   0 runner    (1001) docker     (127)   108892 2024-04-16 09:52:28.000000 omegapy-3.0.1/omegapy/OMEGA_dataref/omega128_interpol.sav
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-16 09:52:28.000000 omegapy-3.0.1/omegapy/OMEGA_dataref/omega_atmorap_CL.dat
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-16 09:52:28.000000 omegapy-3.0.1/omegapy/OMEGA_dataref/omega_wvl_CL.dat
--rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-04-16 09:52:28.000000 omegapy-3.0.1/omegapy/OMEGA_dataref/rapcur_25.dat
--rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-04-16 09:52:28.000000 omegapy-3.0.1/omegapy/OMEGA_dataref/rapcur_50.dat
--rw-r--r--   0 runner    (1001) docker     (127)  6723584 2024-04-16 09:52:29.000000 omegapy-3.0.1/omegapy/OMEGA_dataref/rapmtflcur.bin
--rw-r--r--   0 runner    (1001) docker     (127)     5720 2024-04-16 09:52:29.000000 omegapy-3.0.1/omegapy/OMEGA_dataref/refclair_sombr_omega_CL.dat
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-16 09:52:29.000000 omegapy-3.0.1/omegapy/OMEGA_dataref/specsol_0403.dat
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-16 09:52:29.000000 omegapy-3.0.1/omegapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   134170 2024-04-16 09:52:29.000000 omegapy-3.0.1/omegapy/omega_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    74612 2024-04-16 09:52:29.000000 omegapy-3.0.1/omegapy/omega_plots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:52:36.979098 omegapy-3.0.1/omegapy/res_findcube/
--rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-04-16 09:52:29.000000 omegapy-3.0.1/omegapy/res_findcube/cubelist
--rw-r--r--   0 runner    (1001) docker     (127)    15597 2024-04-16 09:52:29.000000 omegapy-3.0.1/omegapy/useful_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:52:36.979098 omegapy-3.0.1/omegapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-04-16 09:52:36.000000 omegapy-3.0.1/omegapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-16 09:52:36.000000 omegapy-3.0.1/omegapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 09:52:36.000000 omegapy-3.0.1/omegapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-16 09:52:36.000000 omegapy-3.0.1/omegapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-16 09:52:36.000000 omegapy-3.0.1/omegapy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 09:52:36.979098 omegapy-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-16 09:52:29.000000 omegapy-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 05:32:58.501486 omegapy-3.0b0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2023-10-19 05:32:47.000000 omegapy-3.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2023-10-19 05:32:58.497486 omegapy-3.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2023-10-19 05:32:47.000000 omegapy-3.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 05:32:58.477486 omegapy-3.0b0/omegapy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 05:32:58.497486 omegapy-3.0b0/omegapy/OMEGA_dataref/
+-rw-r--r--   0 runner    (1001) docker     (127)   143760 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/OBC_OMEGA_OCT2017.sav
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/boundcur.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/corrupted_obs.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1495234 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/cubindex.ref
+-rw-r--r--   0 runner    (1001) docker     (127)    49152 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/flatVIS050701.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/fond2.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/lambda_0403.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    48007 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/linearC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/mtf120315_25.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/mtf120315_50.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   108892 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/omega128_interpol.sav
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/omega_atmorap_CL.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/omega_wvl_CL.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    10240 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/rapcur_25.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    10240 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/rapcur_50.dat
+-rw-r--r--   0 runner    (1001) docker     (127)  6723584 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/rapmtflcur.bin
+-rw-r--r--   0 runner    (1001) docker     (127)     5720 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/refclair_sombr_omega_CL.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/OMEGA_dataref/specsol_0403.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   134170 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/omega_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74027 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/omega_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 05:32:58.497486 omegapy-3.0b0/omegapy/res_findcube/
+-rw-r--r--   0 runner    (1001) docker     (127)     5510 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/res_findcube/cubelist
+-rw-r--r--   0 runner    (1001) docker     (127)    15597 2023-10-19 05:32:47.000000 omegapy-3.0b0/omegapy/useful_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 05:32:58.481486 omegapy-3.0b0/omegapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2023-10-19 05:32:58.000000 omegapy-3.0b0/omegapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2023-10-19 05:32:58.000000 omegapy-3.0b0/omegapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-19 05:32:58.000000 omegapy-3.0b0/omegapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2023-10-19 05:32:58.000000 omegapy-3.0b0/omegapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2023-10-19 05:32:58.000000 omegapy-3.0b0/omegapy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-19 05:32:58.501486 omegapy-3.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2023-10-19 05:32:47.000000 omegapy-3.0b0/setup.py
```

### Comparing `omegapy-3.0.1/LICENSE` & `omegapy-3.0b0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Aurélien Stcherbinine
+Copyright (c) 2021 Aurélien Stcherbinine
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `omegapy-3.0.1/PKG-INFO` & `omegapy-3.0b0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 Metadata-Version: 2.1
 Name: omegapy
-Version: 3.0.1
+Version: 3.0b0
 Summary: Python tools for OMEGA/MEx observations analysis
 Home-page: https://astcherbinine.github.io/omegapy
 Author: Aurélien Stcherbinine
 Author-email: aurelien@stcherbinine.net
 Project-URL: Source, https://github.com/AStcherbinine/omegapy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy>=1.17
-Requires-Dist: matplotlib>=3.0
-Requires-Dist: tqdm>=4.31
-Requires-Dist: scipy>=1.3
-Requires-Dist: pandas>=0.25
 
-![version](https://img.shields.io/badge/version-3.0.1-blue)
+![version](https://img.shields.io/badge/version-3.0beta-blue)
 ![pythonversion](https://img.shields.io/badge/Python-3.7+-blue)
-[![DOI](https://zenodo.org/badge/349763849.svg)](https://zenodo.org/doi/10.5281/zenodo.7818828)
+[![DOI](https://zenodo.org/badge/349763849.svg)](https://zenodo.org/badge/latestdoi/349763849)
 
 
 <p align="center">
 <img width="250" height="250" src="https://github.com/AStcherbinine/omegapy/blob/master/docs/logo_omegapy_small2.png">
 </p>
 
 # OMEGA-Py : Python tools for OMEGA data
 
 Importation and display of OMEGA/MEx observations in Python 3, based on the IDL *SOFT10* routines developped in the IAS planetary team.
 
+> **Disclaimer:** This module is not the official software distributed by the OMEGA team.
+
 ## Installation & Update
 ### Method 1: from PyPI (recommended)
 **Installation:** `pip3 install omegapy`
 
 **Update:** `pip3 install omegapy --upgrade` 
 
 
@@ -57,30 +54,21 @@
 ~~~
 
 ## Documentation
 Full documentation of the OMEGA-Py module is available at [astcherbinine.github.io/omegapy](https://astcherbinine.github.io/omegapy/)
 
 Planetary Data Workshop 2023: [abstract](https://github.com/AStcherbinine/omegapy/blob/master/docs/Stcherbinine_PDW2023_7007_omegapy.pdf) & [slides](https://github.com/AStcherbinine/omegapy/blob/master/docs/PDW_Flagstaff_Stcherbinine_omegapy_upload.pdf)
 
-## Community guidelines
-To contribute to OMEGA-Py, report an issue or seek support, please refer to the community guidelines
-page of the documentation available [here](https://astcherbinine.github.io/omegapy/community/).
-
 ## Citing OMEGA-Py
 If you are using OMEGA-Py in your research, please cite it according to the guidelines available [here](https://astcherbinine.github.io/omegapy/credits/).
 
 ## Credits
 
-© Aurélien Stcherbinine (2020–2024)
+© Aurélien Stcherbinine (2020–2023)
 
 Institut d'Astrophysique Spatiale (IAS), Université Paris-Saclay, CNRS, Orsay, France
 
 LATMOS/IPSL, UVSQ Université Paris-Saclay, Sorbonne Université, CNRS, Guyancourt, France
 
-Department of Astronomy and Planetary Science, Northern Arizona University, Flagstaff, AZ, USA
-
-Institut de Recherche en Astrophysique et Planétologie (IRAP), CNES, Université Toulouse III,
-CNRS, Toulouse, France
-
 
 ## License
 This package is released under a MIT open source license. See [`LICENSE`](https://github.com/AStcherbinine/omegapy/blob/master/LICENSE) for more details.
```

### Comparing `omegapy-3.0.1/README.md` & `omegapy-3.0b0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-![version](https://img.shields.io/badge/version-3.0.1-blue)
+![version](https://img.shields.io/badge/version-3.0beta-blue)
 ![pythonversion](https://img.shields.io/badge/Python-3.7+-blue)
-[![DOI](https://zenodo.org/badge/349763849.svg)](https://zenodo.org/doi/10.5281/zenodo.7818828)
+[![DOI](https://zenodo.org/badge/349763849.svg)](https://zenodo.org/badge/latestdoi/349763849)
 
 
 <p align="center">
 <img width="250" height="250" src="https://github.com/AStcherbinine/omegapy/blob/master/docs/logo_omegapy_small2.png">
 </p>
 
 # OMEGA-Py : Python tools for OMEGA data
 
 Importation and display of OMEGA/MEx observations in Python 3, based on the IDL *SOFT10* routines developped in the IAS planetary team.
 
+> **Disclaimer:** This module is not the official software distributed by the OMEGA team.
+
 ## Installation & Update
 ### Method 1: from PyPI (recommended)
 **Installation:** `pip3 install omegapy`
 
 **Update:** `pip3 install omegapy --upgrade` 
 
 
@@ -35,30 +37,21 @@
 ~~~
 
 ## Documentation
 Full documentation of the OMEGA-Py module is available at [astcherbinine.github.io/omegapy](https://astcherbinine.github.io/omegapy/)
 
 Planetary Data Workshop 2023: [abstract](https://github.com/AStcherbinine/omegapy/blob/master/docs/Stcherbinine_PDW2023_7007_omegapy.pdf) & [slides](https://github.com/AStcherbinine/omegapy/blob/master/docs/PDW_Flagstaff_Stcherbinine_omegapy_upload.pdf)
 
-## Community guidelines
-To contribute to OMEGA-Py, report an issue or seek support, please refer to the community guidelines
-page of the documentation available [here](https://astcherbinine.github.io/omegapy/community/).
-
 ## Citing OMEGA-Py
 If you are using OMEGA-Py in your research, please cite it according to the guidelines available [here](https://astcherbinine.github.io/omegapy/credits/).
 
 ## Credits
 
-© Aurélien Stcherbinine (2020–2024)
+© Aurélien Stcherbinine (2020–2023)
 
 Institut d'Astrophysique Spatiale (IAS), Université Paris-Saclay, CNRS, Orsay, France
 
 LATMOS/IPSL, UVSQ Université Paris-Saclay, Sorbonne Université, CNRS, Guyancourt, France
 
-Department of Astronomy and Planetary Science, Northern Arizona University, Flagstaff, AZ, USA
-
-Institut de Recherche en Astrophysique et Planétologie (IRAP), CNES, Université Toulouse III,
-CNRS, Toulouse, France
-
 
 ## License
 This package is released under a MIT open source license. See [`LICENSE`](https://github.com/AStcherbinine/omegapy/blob/master/LICENSE) for more details.
```

### Comparing `omegapy-3.0.1/omegapy/OMEGA_dataref/OBC_OMEGA_OCT2017.sav` & `omegapy-3.0b0/omegapy/OMEGA_dataref/OBC_OMEGA_OCT2017.sav`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.1/omegapy/OMEGA_dataref/boundcur.dat` & `omegapy-3.0b0/omegapy/OMEGA_dataref/boundcur.dat`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.1/omegapy/OMEGA_dataref/corrupted_obs.csv` & `omegapy-3.0b0/omegapy/OMEGA_dataref/corrupted_obs.csv`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.1/omegapy/OMEGA_dataref/cubindex.ref` & `omegapy-3.0b0/omegapy/OMEGA_dataref/cubindex.ref`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.1/omegapy/OMEGA_dataref/flatVIS050701.bin` & `omegapy-3.0b0/omegapy/OMEGA_dataref/flatVIS050701.bin`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.1/omegapy/OMEGA_dataref/fond2.dat` & `omegapy-3.0b0/omegapy/OMEGA_dataref/fond2.dat`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.1/omegapy/OMEGA_dataref/lambda_0403.dat` & `omegapy-3.0b0/omegapy/OMEGA_dataref/lambda_0403.dat`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.1/omegapy/OMEGA_dataref/linearC.dat` & `omegapy-3.0b0/omegapy/OMEGA_dataref/linearC.dat`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.1/omegapy/OMEGA_dataref/mtf120315_25.dat` & `omegapy-3.0b0/omegapy/OMEGA_dataref/mtf120315_25.dat`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.1/omegapy/OMEGA_dataref/mtf120315_50.dat` & `omegapy-3.0b0/omegapy/OMEGA_dataref/mtf120315_50.dat`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.1/omegapy/OMEGA_dataref/omega128_interpol.sav` & `omegapy-3.0b0/omegapy/OMEGA_dataref/omega128_interpol.sav`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.1/omegapy/OMEGA_dataref/omega_atmorap_CL.dat` & `omegapy-3.0b0/omegapy/OMEGA_dataref/omega_atmorap_CL.dat`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.1/omegapy/OMEGA_dataref/omega_wvl_CL.dat` & `omegapy-3.0b0/omegapy/OMEGA_dataref/omega_wvl_CL.dat`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.1/omegapy/OMEGA_dataref/rapcur_25.dat` & `omegapy-3.0b0/omegapy/OMEGA_dataref/rapcur_25.dat`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.1/omegapy/OMEGA_dataref/rapcur_50.dat` & `omegapy-3.0b0/omegapy/OMEGA_dataref/rapcur_50.dat`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.1/omegapy/OMEGA_dataref/rapmtflcur.bin` & `omegapy-3.0b0/omegapy/OMEGA_dataref/rapmtflcur.bin`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.1/omegapy/OMEGA_dataref/refclair_sombr_omega_CL.dat` & `omegapy-3.0b0/omegapy/OMEGA_dataref/refclair_sombr_omega_CL.dat`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.1/omegapy/OMEGA_dataref/specsol_0403.dat` & `omegapy-3.0b0/omegapy/OMEGA_dataref/specsol_0403.dat`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.1/omegapy/omega_data.py` & `omegapy-3.0b0/omegapy/omega_data.py`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.1/omegapy/omega_plots.py` & `omegapy-3.0b0/omegapy/omega_plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 ## omega_plots.py
 ## Created by Aurélien STCHERBININE
-## Last modified by Aurélien STCHERBININE : 16/04/2024
+## Last modified by Aurélien STCHERBININE : 18/10/2023
 
 ##----------------------------------------------------------------------------------------
 """Display of `OMEGAdata` cubes.
 """
 ##----------------------------------------------------------------------------------------
 ##----------------------------------------------------------------------------------------
 ## Packages
@@ -178,15 +178,15 @@
     cmap : str, default 'Greys_r'
         The matplotlib colormap.
     vmin : float or None, default None
         The lower bound of the colorscale.
     vmax : float or None, default None
         The upper bound of the colorscale.
     alpha : float or None, default None
-        Opacity of the plot, from 0 (transparent) to 1 (opaque).
+        Opacity of the plot.
     title : str, default 'auto'
         The title of the figure.
     lonlim : tuple of int or None, default (None, None)
         The longitude bounds of the figure.
     latlim : tuple of int or None, default (None, None)
         The latitude bounds of the y-axis of the figure.
     Nfig : int or str or None, default None
@@ -619,15 +619,15 @@
     autoyscale : bool, default True
         | `True` --> Enable the auto-scaling of the spectra y-axis.</br>
         | `False` --> Force use of the (vmin, vmax) bounds for the spectra plots.
     ylim_sp : tuple of float or None, default (None, None)
         If autoyscale is False, can specify the bound values for the spectrum y-axis,
         other that `(vmin, vmax)`.
     alpha : float or None, default None
-        Opacity of the plot, from 0 (transparent) to 1 (opaque).
+        Opacity of the plot.
     lonlim : tuple of int or None, default (None, None)
         The longitude bounds of the figure.
     latlim : tuple of int or None, default (None, None)
         The latitude bounds of the y-axis of the figure.
     polar : bool, default False
         If `True` --> Use a polar projection for the plot.
     cbar : bool, default True
@@ -813,15 +813,15 @@
     cmap : str, default 'Greys_r'
         The matplotlib colormap.
     vmin : float or None, default None
         The lower bound of the colorscale.
     vmax : float or None, default None
         The upper bound of the colorscale.
     alpha : float or None, default None
-        Opacity of the plot, from 0 (transparent) to 1 (opaque).
+        Opacity of the plot.
     title : str, default 'auto'
         The title of the figure.
     cb_title : str, default 'data'
         The title of the colorbar.
     lonlim : tuple of int or None, default (None, None)
         The longitude bounds of the figure.
     latlim : tuple of int or None, default (None, None)
@@ -857,24 +857,16 @@
             negatives_longitudes = True
     if title == 'auto':
         title = ('OMEGA/MEx observation {0}'.format(omega.name))
     fig = plt.figure(Nfig)
     Nfig = fig.number   # get the actual figure number if Nfig=None
     if not (mask is None):
         data = deepcopy(data) * mask     # apply mask to remove bad pixels (turned to NaN)
-    if len(fig.get_axes()) != 0:    # If presence of axes
-        ax0 = fig.get_axes()[0]
-        is_ax0_polar = hasattr(ax0, 'set_theta_offset') # Test if ax has polar projection
-        if not polar == is_ax0_polar:
-            raise ValueError("Can not mix polar and non-polar projections in the same plot")
     if polar:
-        if len(fig.get_axes()) == 0:    # Test presence of axes in the figure
-            ax = plt.axes(polar=True)
-        else:
-            ax = fig.get_axes()[0]  # Do not create new axes instance
+        ax = plt.axes(polar=True)
         plt.pcolormesh(omega.lon_grid*np.pi/180, omega.lat_grid, data, cmap=cmap, 
                        alpha=alpha, vmin=vmin, vmax=vmax, **kwargs)
         ax.set_yticklabels([])  # remove the latitude values in the plot
         if latlim[0] is None:
             if np.max(omega.lat) > 0:
                 latlim = (90, np.min(omega.lat_grid)-1)
             else:
```

### Comparing `omegapy-3.0.1/omegapy/res_findcube/cubelist` & `omegapy-3.0b0/omegapy/res_findcube/cubelist`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.1/omegapy/useful_functions.py` & `omegapy-3.0b0/omegapy/useful_functions.py`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.1/omegapy.egg-info/PKG-INFO` & `omegapy-3.0b0/omegapy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 Metadata-Version: 2.1
 Name: omegapy
-Version: 3.0.1
+Version: 3.0b0
 Summary: Python tools for OMEGA/MEx observations analysis
 Home-page: https://astcherbinine.github.io/omegapy
 Author: Aurélien Stcherbinine
 Author-email: aurelien@stcherbinine.net
 Project-URL: Source, https://github.com/AStcherbinine/omegapy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy>=1.17
-Requires-Dist: matplotlib>=3.0
-Requires-Dist: tqdm>=4.31
-Requires-Dist: scipy>=1.3
-Requires-Dist: pandas>=0.25
 
-![version](https://img.shields.io/badge/version-3.0.1-blue)
+![version](https://img.shields.io/badge/version-3.0beta-blue)
 ![pythonversion](https://img.shields.io/badge/Python-3.7+-blue)
-[![DOI](https://zenodo.org/badge/349763849.svg)](https://zenodo.org/doi/10.5281/zenodo.7818828)
+[![DOI](https://zenodo.org/badge/349763849.svg)](https://zenodo.org/badge/latestdoi/349763849)
 
 
 <p align="center">
 <img width="250" height="250" src="https://github.com/AStcherbinine/omegapy/blob/master/docs/logo_omegapy_small2.png">
 </p>
 
 # OMEGA-Py : Python tools for OMEGA data
 
 Importation and display of OMEGA/MEx observations in Python 3, based on the IDL *SOFT10* routines developped in the IAS planetary team.
 
+> **Disclaimer:** This module is not the official software distributed by the OMEGA team.
+
 ## Installation & Update
 ### Method 1: from PyPI (recommended)
 **Installation:** `pip3 install omegapy`
 
 **Update:** `pip3 install omegapy --upgrade` 
 
 
@@ -57,30 +54,21 @@
 ~~~
 
 ## Documentation
 Full documentation of the OMEGA-Py module is available at [astcherbinine.github.io/omegapy](https://astcherbinine.github.io/omegapy/)
 
 Planetary Data Workshop 2023: [abstract](https://github.com/AStcherbinine/omegapy/blob/master/docs/Stcherbinine_PDW2023_7007_omegapy.pdf) & [slides](https://github.com/AStcherbinine/omegapy/blob/master/docs/PDW_Flagstaff_Stcherbinine_omegapy_upload.pdf)
 
-## Community guidelines
-To contribute to OMEGA-Py, report an issue or seek support, please refer to the community guidelines
-page of the documentation available [here](https://astcherbinine.github.io/omegapy/community/).
-
 ## Citing OMEGA-Py
 If you are using OMEGA-Py in your research, please cite it according to the guidelines available [here](https://astcherbinine.github.io/omegapy/credits/).
 
 ## Credits
 
-© Aurélien Stcherbinine (2020–2024)
+© Aurélien Stcherbinine (2020–2023)
 
 Institut d'Astrophysique Spatiale (IAS), Université Paris-Saclay, CNRS, Orsay, France
 
 LATMOS/IPSL, UVSQ Université Paris-Saclay, Sorbonne Université, CNRS, Guyancourt, France
 
-Department of Astronomy and Planetary Science, Northern Arizona University, Flagstaff, AZ, USA
-
-Institut de Recherche en Astrophysique et Planétologie (IRAP), CNES, Université Toulouse III,
-CNRS, Toulouse, France
-
 
 ## License
 This package is released under a MIT open source license. See [`LICENSE`](https://github.com/AStcherbinine/omegapy/blob/master/LICENSE) for more details.
```

### Comparing `omegapy-3.0.1/omegapy.egg-info/SOURCES.txt` & `omegapy-3.0b0/omegapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omegapy-3.0.1/setup.py` & `omegapy-3.0b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 package_data = {
     '': ['OMEGA_dataref/*', 'res_findcube/*'],
     }
 
 setuptools.setup(
     name='omegapy',
-    version='3.0.1',
+    version='3.0beta',
     author='Aurélien Stcherbinine',
     author_email='aurelien@stcherbinine.net',
     description='Python tools for OMEGA/MEx observations analysis',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://astcherbinine.github.io/omegapy',
     project_urls={
```

