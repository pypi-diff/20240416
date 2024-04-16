# Comparing `tmp/hidrokit-0.4.1.tar.gz` & `tmp/hidrokit-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hidrokit-0.4.1.tar", last modified: Mon Jun 13 04:17:00 2022, max compression
+gzip compressed data, was "hidrokit-0.5.0.tar", last modified: Tue Apr 16 04:31:49 2024, max compression
```

## Comparing `hidrokit-0.4.1.tar` & `hidrokit-0.5.0.tar`

### file list

```diff
@@ -1,59 +1,67 @@
-drwxrwxrwx   0        0        0        0 2022-06-13 04:17:00.426825 hidrokit-0.4.1/
--rw-rw-rw-   0        0        0     6464 2022-04-04 10:29:37.000000 hidrokit-0.4.1/CHANGELOG.md
--rw-rw-rw-   0        0        0    15622 2022-04-04 10:29:37.000000 hidrokit-0.4.1/CHANGELOG_gen.md
--rw-rw-rw-   0        0        0     3369 2022-04-04 10:29:37.000000 hidrokit-0.4.1/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0      128 2022-03-30 12:08:06.000000 hidrokit-0.4.1/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     1109 2022-04-04 10:29:37.000000 hidrokit-0.4.1/LICENSE.txt
--rw-rw-rw-   0        0        0      141 2022-03-30 12:08:06.000000 hidrokit-0.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5789 2022-06-13 04:17:00.427822 hidrokit-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     4775 2022-06-13 03:56:59.000000 hidrokit-0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2022-06-13 04:17:00.365154 hidrokit-0.4.1/hidrokit/
--rw-rw-rw-   0        0        0      299 2022-03-30 12:08:06.000000 hidrokit-0.4.1/hidrokit/__init__.py
--rw-rw-rw-   0        0        0      126 2022-06-13 03:56:59.000000 hidrokit-0.4.1/hidrokit/__version__.py
-drwxrwxrwx   0        0        0        0 2022-06-13 04:17:00.376668 hidrokit-0.4.1/hidrokit/analysis/
--rw-rw-rw-   0        0        0        0 2022-03-30 12:08:06.000000 hidrokit-0.4.1/hidrokit/analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-13 04:17:00.377666 hidrokit-0.4.1/hidrokit/contrib/
--rw-rw-rw-   0        0        0       46 2022-03-30 12:08:06.000000 hidrokit-0.4.1/hidrokit/contrib/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-13 04:17:00.415854 hidrokit-0.4.1/hidrokit/contrib/taruma/
--rw-rw-rw-   0        0        0      967 2022-04-04 10:29:37.000000 hidrokit-0.4.1/hidrokit/contrib/taruma/__init__.py
--rw-rw-rw-   0        0        0      368 2022-04-04 10:29:37.000000 hidrokit-0.4.1/hidrokit/contrib/taruma/anfrek.py
--rw-rw-rw-   0        0        0      705 2022-04-04 10:29:37.000000 hidrokit-0.4.1/hidrokit/contrib/taruma/hk102.py
--rw-rw-rw-   0        0        0     8853 2022-03-30 12:08:06.000000 hidrokit-0.4.1/hidrokit/contrib/taruma/hk106.py
--rw-rw-rw-   0        0        0     2774 2022-04-04 10:29:37.000000 hidrokit-0.4.1/hidrokit/contrib/taruma/hk124.py
--rw-rw-rw-   0        0        0    18558 2022-06-13 03:56:59.000000 hidrokit-0.4.1/hidrokit/contrib/taruma/hk126.py
--rw-rw-rw-   0        0        0    11107 2022-04-04 10:29:37.000000 hidrokit-0.4.1/hidrokit/contrib/taruma/hk127.py
--rw-rw-rw-   0        0        0     5180 2022-06-13 03:56:59.000000 hidrokit-0.4.1/hidrokit/contrib/taruma/hk140.py
--rw-rw-rw-   0        0        0     6549 2022-06-13 03:56:59.000000 hidrokit-0.4.1/hidrokit/contrib/taruma/hk141.py
--rw-rw-rw-   0        0        0     2922 2022-04-04 10:29:37.000000 hidrokit-0.4.1/hidrokit/contrib/taruma/hk151.py
--rw-rw-rw-   0        0        0     2414 2022-04-04 10:29:37.000000 hidrokit-0.4.1/hidrokit/contrib/taruma/hk158.py
--rw-rw-rw-   0        0        0     2732 2022-04-04 10:29:37.000000 hidrokit-0.4.1/hidrokit/contrib/taruma/hk172.py
--rw-rw-rw-   0        0        0     2903 2022-03-30 12:08:06.000000 hidrokit-0.4.1/hidrokit/contrib/taruma/hk43.py
--rw-rw-rw-   0        0        0     1583 2022-03-30 12:08:06.000000 hidrokit-0.4.1/hidrokit/contrib/taruma/hk53.py
--rw-rw-rw-   0        0        0     2437 2022-03-30 12:08:06.000000 hidrokit-0.4.1/hidrokit/contrib/taruma/hk73.py
--rw-rw-rw-   0        0        0     2827 2022-03-30 12:08:06.000000 hidrokit-0.4.1/hidrokit/contrib/taruma/hk79.py
--rw-rw-rw-   0        0        0     2170 2022-03-30 12:08:06.000000 hidrokit-0.4.1/hidrokit/contrib/taruma/hk84.py
--rw-rw-rw-   0        0        0     1217 2022-03-30 12:08:06.000000 hidrokit-0.4.1/hidrokit/contrib/taruma/hk87.py
--rw-rw-rw-   0        0        0     2153 2022-04-04 10:29:37.000000 hidrokit-0.4.1/hidrokit/contrib/taruma/hk88.py
--rw-rw-rw-   0        0        0     4690 2022-03-30 12:08:06.000000 hidrokit-0.4.1/hidrokit/contrib/taruma/hk89.py
--rw-rw-rw-   0        0        0     1809 2022-03-30 12:08:06.000000 hidrokit-0.4.1/hidrokit/contrib/taruma/hk90.py
--rw-rw-rw-   0        0        0     4250 2022-03-30 12:08:06.000000 hidrokit-0.4.1/hidrokit/contrib/taruma/hk96.py
--rw-rw-rw-   0        0        0     1793 2022-06-13 03:56:59.000000 hidrokit-0.4.1/hidrokit/contrib/taruma/hk98.py
--rw-rw-rw-   0        0        0      798 2022-03-30 12:08:06.000000 hidrokit-0.4.1/hidrokit/contrib/taruma/hk99.py
--rw-rw-rw-   0        0        0      168 2022-04-04 10:29:37.000000 hidrokit-0.4.1/hidrokit/contrib/taruma/ujidist.py
-drwxrwxrwx   0        0        0        0 2022-06-13 04:17:00.421840 hidrokit-0.4.1/hidrokit/prep/
--rw-rw-rw-   0        0        0       86 2022-03-30 12:08:06.000000 hidrokit-0.4.1/hidrokit/prep/__init__.py
--rw-rw-rw-   0        0        0     3931 2022-03-30 12:08:06.000000 hidrokit-0.4.1/hidrokit/prep/excel.py
--rw-rw-rw-   0        0        0     2217 2022-03-30 12:08:06.000000 hidrokit-0.4.1/hidrokit/prep/read.py
--rw-rw-rw-   0        0        0     4217 2022-03-30 12:08:06.000000 hidrokit-0.4.1/hidrokit/prep/timeseries.py
-drwxrwxrwx   0        0        0        0 2022-06-13 04:17:00.425827 hidrokit-0.4.1/hidrokit/viz/
--rw-rw-rw-   0        0        0       62 2022-03-30 12:08:06.000000 hidrokit-0.4.1/hidrokit/viz/__init__.py
--rw-rw-rw-   0        0        0     1286 2022-03-30 12:08:06.000000 hidrokit-0.4.1/hidrokit/viz/graph.py
--rw-rw-rw-   0        0        0     1253 2022-03-30 12:08:06.000000 hidrokit-0.4.1/hidrokit/viz/table.py
-drwxrwxrwx   0        0        0        0 2022-06-13 04:17:00.375669 hidrokit-0.4.1/hidrokit.egg-info/
--rw-rw-rw-   0        0        0     5789 2022-06-13 04:16:59.000000 hidrokit-0.4.1/hidrokit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1367 2022-06-13 04:17:00.000000 hidrokit-0.4.1/hidrokit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-13 04:16:59.000000 hidrokit-0.4.1/hidrokit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2022-06-13 04:17:00.000000 hidrokit-0.4.1/hidrokit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-06-13 04:17:00.000000 hidrokit-0.4.1/hidrokit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      117 2022-06-13 04:17:00.428843 hidrokit-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0     3018 2022-06-13 03:36:31.000000 hidrokit-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 04:31:49.520059 hidrokit-0.5.0/
+-rw-rw-rw-   0        0        0     6060 2024-04-14 07:31:59.000000 hidrokit-0.5.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0    15622 2024-04-11 05:03:58.000000 hidrokit-0.5.0/CHANGELOG_gen.md
+-rw-rw-rw-   0        0        0     6464 2024-04-14 07:31:59.000000 hidrokit-0.5.0/CHANGELOG_old.md
+-rw-rw-rw-   0        0        0     3369 2024-04-11 05:03:58.000000 hidrokit-0.5.0/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0      128 2024-04-11 05:03:58.000000 hidrokit-0.5.0/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     1109 2024-04-14 07:31:59.000000 hidrokit-0.5.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      141 2024-04-11 05:03:58.000000 hidrokit-0.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5958 2024-04-16 04:31:49.518831 hidrokit-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4628 2024-04-14 07:31:59.000000 hidrokit-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 04:31:49.409858 hidrokit-0.5.0/hidrokit/
+-rw-rw-rw-   0        0        0      299 2024-04-11 05:03:58.000000 hidrokit-0.5.0/hidrokit/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-04-14 07:31:59.000000 hidrokit-0.5.0/hidrokit/__version__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 04:31:49.449004 hidrokit-0.5.0/hidrokit/analysis/
+-rw-rw-rw-   0        0        0        0 2024-04-11 05:03:58.000000 hidrokit-0.5.0/hidrokit/analysis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 04:31:49.450409 hidrokit-0.5.0/hidrokit/contrib/
+-rw-rw-rw-   0        0        0       46 2024-04-11 05:03:58.000000 hidrokit-0.5.0/hidrokit/contrib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 04:31:49.494658 hidrokit-0.5.0/hidrokit/contrib/taruma/
+-rw-rw-rw-   0        0        0     2436 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/__init__.py
+-rw-rw-rw-   0        0        0      549 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/anfrek.py
+-rw-rw-rw-   0        0        0     9158 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/bmkg_utils.py
+-rw-rw-rw-   0        0        0    11048 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/chi_square.py
+-rw-rw-rw-   0        0        0     4218 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/dataframe_to_tensor.py
+-rw-rw-rw-   0        0        0     4657 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/dependable_flow.py
+-rw-rw-rw-   0        0        0    20229 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/evapotranspiration.py
+-rw-rw-rw-   0        0        0     6927 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/fjmock_model.py
+-rw-rw-rw-   0        0        0    18688 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/gumbel.py
+-rw-rw-rw-   0        0        0     8396 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/hidrokit_excel_parser.py
+-rw-rw-rw-   0        0        0     6021 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/hidrokit_hourly_excel_parser.py
+-rw-rw-rw-   0        0        0     9264 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/kolmogorov_smirnov.py
+-rw-rw-rw-   0        0        0     7290 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/lognormal.py
+-rw-rw-rw-   0        0        0    24565 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/logpearson3.py
+-rw-rw-rw-   0        0        0     3293 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/model_calibration.py
+-rw-rw-rw-   0        0        0     8668 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/normal.py
+-rw-rw-rw-   0        0        0     8127 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/nreca_model.py
+-rw-rw-rw-   0        0        0     6436 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/outlier_hydrology.py
+-rw-rw-rw-   0        0        0    11543 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/pamarayan_excel_data_extraction.py
+-rw-rw-rw-   0        0        0     3827 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/statistic_summary.py
+-rw-rw-rw-   0        0        0     4156 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/statistical_coefficients.py
+-rw-rw-rw-   0        0        0     5752 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/summary_hourly.py
+-rw-rw-rw-   0        0        0     2484 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/thiessen.py
+-rw-rw-rw-   0        0        0      411 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/ujidist.py
+-rw-rw-rw-   0        0        0     3469 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/upsampling.py
+-rw-rw-rw-   0        0        0     1667 2024-04-16 04:13:00.000000 hidrokit-0.5.0/hidrokit/contrib/taruma/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-16 04:31:49.500779 hidrokit-0.5.0/hidrokit/prep/
+-rw-rw-rw-   0        0        0       86 2024-04-11 05:03:58.000000 hidrokit-0.5.0/hidrokit/prep/__init__.py
+-rw-rw-rw-   0        0        0     3931 2024-04-11 05:03:58.000000 hidrokit-0.5.0/hidrokit/prep/excel.py
+-rw-rw-rw-   0        0        0     2217 2024-04-11 05:03:58.000000 hidrokit-0.5.0/hidrokit/prep/read.py
+-rw-rw-rw-   0        0        0     4217 2024-04-11 05:03:58.000000 hidrokit-0.5.0/hidrokit/prep/timeseries.py
+drwxrwxrwx   0        0        0        0 2024-04-16 04:31:49.506052 hidrokit-0.5.0/hidrokit/viz/
+-rw-rw-rw-   0        0        0       62 2024-04-11 05:03:58.000000 hidrokit-0.5.0/hidrokit/viz/__init__.py
+-rw-rw-rw-   0        0        0     1286 2024-04-11 05:03:58.000000 hidrokit-0.5.0/hidrokit/viz/graph.py
+-rw-rw-rw-   0        0        0     1253 2024-04-11 05:03:58.000000 hidrokit-0.5.0/hidrokit/viz/table.py
+drwxrwxrwx   0        0        0        0 2024-04-16 04:31:49.447448 hidrokit-0.5.0/hidrokit.egg-info/
+-rw-rw-rw-   0        0        0     5958 2024-04-16 04:31:49.000000 hidrokit-0.5.0/hidrokit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1778 2024-04-16 04:31:49.000000 hidrokit-0.5.0/hidrokit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 04:31:49.000000 hidrokit-0.5.0/hidrokit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2024-04-16 04:31:49.000000 hidrokit-0.5.0/hidrokit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-16 04:31:49.000000 hidrokit-0.5.0/hidrokit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      117 2024-04-16 04:31:49.528183 hidrokit-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     3134 2024-04-14 07:33:33.000000 hidrokit-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 04:31:49.514300 hidrokit-0.5.0/tests/
+-rw-rw-rw-   0        0        0     1797 2024-04-11 05:03:58.000000 hidrokit-0.5.0/tests/test_prep_excel.py
+-rw-rw-rw-   0        0        0      844 2024-04-11 05:03:58.000000 hidrokit-0.5.0/tests/test_prep_read.py
+-rw-rw-rw-   0        0        0     5086 2024-04-11 05:03:58.000000 hidrokit-0.5.0/tests/test_prep_timeseries.py
+-rw-rw-rw-   0        0        0      477 2024-04-11 05:03:58.000000 hidrokit-0.5.0/tests/test_viz_graph.py
+-rw-rw-rw-   0        0        0     1632 2024-04-11 05:03:58.000000 hidrokit-0.5.0/tests/test_viz_table.py
```

### Comparing `hidrokit-0.4.1/CHANGELOG.md` & `hidrokit-0.5.0/CHANGELOG_old.md`

 * *Files identical despite different names*

### Comparing `hidrokit-0.4.1/CHANGELOG_gen.md` & `hidrokit-0.5.0/CHANGELOG_gen.md`

 * *Files identical despite different names*

### Comparing `hidrokit-0.4.1/CODE_OF_CONDUCT.md` & `hidrokit-0.5.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hidrokit-0.4.1/LICENSE.txt` & `hidrokit-0.5.0/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2018-2022, Taruma Sakti Megariansyah
+Copyright (c) 2018-2024, Taruma Sakti Megariansyah
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `hidrokit-0.4.1/PKG-INFO` & `hidrokit-0.5.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hidrokit
-Version: 0.4.1
+Version: 0.5.0
 Summary: analisis hidrologi dengan python
 Home-page: https://github.com/hidrokit/hidrokit
 Author: Taruma Sakti Megariansyah
 Author-email: hi@taruma.info
 License: MIT
 Project-URL: Documentation, https://hidrokit.github.io/hidrokit
 Project-URL: ReadTheDocs, https://hidrokit.readthedocs.io/en/stable/
@@ -12,28 +12,35 @@
 Project-URL: Source, https://github.com/hidrokit/hidrokit/
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.6.0
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
-Provides-Extra: excel
 License-File: LICENSE.txt
+Requires-Dist: matplotlib>=3.7
+Requires-Dist: numpy>=1.25
+Requires-Dist: pandas>=2.0
+Requires-Dist: scipy>=1.11
+Requires-Dist: xlrd>=2.0
+Provides-Extra: excel
+Requires-Dist: openpyxl; extra == "excel"
+Requires-Dist: xlrd; extra == "excel"
+Requires-Dist: xlwt; extra == "excel"
 
 
 
 <div align="center">
 <a href="https://hidrokit.github.io/hidrokit"><img src="https://hidrokit.github.io/hidrokit/assets/images/presskit/hidrokit-800x200-transparent.png" alt="logo hidrokit"></a><br>
 
-[![Sponsored by PT. FIAKO Enjiniring Indonesia](https://img.shields.io/badge/sponsored%20by-PT.%20FIAKO%20Enjiniring%20Indonesia-blue.svg)](http://www.fiako.co.id/)
-
 ![PyPI - Status](https://img.shields.io/pypi/status/hidrokit.svg)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hidrokit.svg)
 [![GitHub license](https://img.shields.io/github/license/hidrokit/hidrokit.svg)](https://github.com/hidrokit/hidrokit/blob/master/LICENSE)
 [![DOI](https://zenodo.org/badge/145389179.svg)](https://zenodo.org/badge/latestdoi/145389179)
 
 <a href="https://hidrokit.github.io/hidrokit"><b>Kunjungi situs resmi hidrokit.</b></a>
 </div>
@@ -110,11 +117,11 @@
 Tertarik menjadi kontributor? Baca [**berkontribusi**](https://hidrokit.github.io/hidrokit/berkontribusi) untuk kode etik, melakukan _pull request_, dan penjelasan lebih rinci hal lainnya. Proyek _open-source_ ini terbuka untuk siapa saja dengan berbagai latar belakang.
 
 ## Lisensi
 
 Paket hidrokit menggunakan [lisensi MIT](LICENSE.txt). Dokumentasi yang disertai pada proyek ini menggunakan lisensi [Creative Commons Attribution 4.0 International (CC-BY-4.0)](https://creativecommons.org/licenses/by/4.0/deed.id). 
 ## Acknowledgement
 
-- Terima kasih untuk [PT. FIAKO Enjiniring Indonesia](http://www.fiako.co.id/) (FIAKO ENGINEERING) yang telah mensponsori proyek ini sejak Februari 2022.
+- Terima kasih untuk [PT. FIAKO Enjiniring Indonesia](http://www.fiako.co.id/) (FIAKO ENGINEERING) yang telah mensponsori proyek ini sejak Februari 2022 hingga Februari 2024.
 - Terima kasih untuk **LKO** yang telah mensponsori proyek ini sejak versi 0.2.x hingga 0.3.6.
 - Terima kasih untuk tim hidrokit-syndicate (_Cahya Suryadi_, _Christine Dorty Hadi_, dan _Dicky Muhammad Fadli_) atas dukungannya dalam pengembangan hidrokit. 
 - Terima kasih untuk [@firmansennie](https://www.instagram.com/firmansenie/) untuk design logo hidrokit.
```

#### html2text {}

```diff
@@ -1,29 +1,31 @@
-Metadata-Version: 2.1 Name: hidrokit Version: 0.4.1 Summary: analisis hidrologi
+Metadata-Version: 2.1 Name: hidrokit Version: 0.5.0 Summary: analisis hidrologi
 dengan python Home-page: https://github.com/hidrokit/hidrokit Author: Taruma
 Sakti Megariansyah Author-email: hi@taruma.info License: MIT Project-URL:
 Documentation, https://hidrokit.github.io/hidrokit Project-URL: ReadTheDocs,
 https://hidrokit.readthedocs.io/en/stable/ Project-URL: Bug Reports, https://
 github.com/hidrokit/hidrokit/issues Project-URL: Source, https://github.com/
 hidrokit/hidrokit/ Classifier: Development Status :: 3 - Alpha Classifier:
 Intended Audience :: Science/Research Classifier: Topic :: Scientific/
 Engineering :: Hydrology Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Requires-Python: >=3.6.0 Description-
-Content-Type: text/markdown Provides-Extra: excel License-File: LICENSE.txt
+Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Requires-Python: >=3.9.0 Description-Content-Type: text/markdown
+License-File: LICENSE.txt Requires-Dist: matplotlib>=3.7 Requires-Dist:
+numpy>=1.25 Requires-Dist: pandas>=2.0 Requires-Dist: scipy>=1.11 Requires-
+Dist: xlrd>=2.0 Provides-Extra: excel Requires-Dist: openpyxl; extra == "excel"
+Requires-Dist: xlrd; extra == "excel" Requires-Dist: xlwt; extra == "excel"
                                 _[_l_o_g_o_ _h_i_d_r_o_k_i_t_]
- [![Sponsored by PT. FIAKO Enjiniring Indonesia](https://img.shields.io/badge/
-    sponsored%20by-PT.%20FIAKO%20Enjiniring%20Indonesia-blue.svg)](http://
-    www.fiako.co.id/) ![PyPI - Status](https://img.shields.io/pypi/status/
-hidrokit.svg) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
-    hidrokit.svg) [![GitHub license](https://img.shields.io/github/license/
-   hidrokit/hidrokit.svg)](https://github.com/hidrokit/hidrokit/blob/master/
- LICENSE) [![DOI](https://zenodo.org/badge/145389179.svg)](https://zenodo.org/
-           badge/latestdoi/145389179) _KK_uu_nn_jj_uu_nn_gg_ii_ _ss_ii_tt_uu_ss_ _rr_ee_ss_mm_ii_ _hh_ii_dd_rr_oo_kk_ii_tt_..
+  ![PyPI - Status](https://img.shields.io/pypi/status/hidrokit.svg) ![PyPI -
+Python Version](https://img.shields.io/pypi/pyversions/hidrokit.svg) [![GitHub
+license](https://img.shields.io/github/license/hidrokit/hidrokit.svg)](https://
+ github.com/hidrokit/hidrokit/blob/master/LICENSE) [![DOI](https://zenodo.org/
+ badge/145389179.svg)](https://zenodo.org/badge/latestdoi/145389179) _KK_uu_nn_jj_uu_nn_gg_ii
+                             _ss_ii_tt_uu_ss_ _rr_ee_ss_mm_ii_ _hh_ii_dd_rr_oo_kk_ii_tt_..
 `hidrokit` adalah proyek _open source_ paket *python* yang dapat digunakan
 untuk membantu proses analisis hidrologi dimulai dari pengolahan data, analisis
 data, dan visualisasi data. [Baca lebih lanjut mengenai hidrokit](https://
 hidrokit.github.io/hidrokit/tentang-hidrokit). ## Release
 RReelleeaassee  PPyyPPII             GGiitthhuubb          GGiitthhuubb ((PPrree--rreelleeaassee))
         [PyPI] [GitHub release]      [GitHub release]
 Date           [GitHub Release Date] [GitHub (Pre-)Release Date]
@@ -54,13 +56,13 @@
 kode etik, melakukan _pull request_, dan penjelasan lebih rinci hal lainnya.
 Proyek _open-source_ ini terbuka untuk siapa saja dengan berbagai latar
 belakang. ## Lisensi Paket hidrokit menggunakan [lisensi MIT](LICENSE.txt).
 Dokumentasi yang disertai pada proyek ini menggunakan lisensi [Creative Commons
 Attribution 4.0 International (CC-BY-4.0)](https://creativecommons.org/
 licenses/by/4.0/deed.id). ## Acknowledgement - Terima kasih untuk [PT. FIAKO
 Enjiniring Indonesia](http://www.fiako.co.id/) (FIAKO ENGINEERING) yang telah
-mensponsori proyek ini sejak Februari 2022. - Terima kasih untuk **LKO** yang
-telah mensponsori proyek ini sejak versi 0.2.x hingga 0.3.6. - Terima kasih
-untuk tim hidrokit-syndicate (_Cahya Suryadi_, _Christine Dorty Hadi_, dan
-_Dicky Muhammad Fadli_) atas dukungannya dalam pengembangan hidrokit. - Terima
-kasih untuk [@firmansennie](https://www.instagram.com/firmansenie/) untuk
-design logo hidrokit.
+mensponsori proyek ini sejak Februari 2022 hingga Februari 2024. - Terima kasih
+untuk **LKO** yang telah mensponsori proyek ini sejak versi 0.2.x hingga 0.3.6.
+- Terima kasih untuk tim hidrokit-syndicate (_Cahya Suryadi_, _Christine Dorty
+Hadi_, dan _Dicky Muhammad Fadli_) atas dukungannya dalam pengembangan
+hidrokit. - Terima kasih untuk [@firmansennie](https://www.instagram.com/
+firmansenie/) untuk design logo hidrokit.
```

### Comparing `hidrokit-0.4.1/README.md` & `hidrokit-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 
 <div align="center">
 <a href="https://hidrokit.github.io/hidrokit"><img src="https://hidrokit.github.io/hidrokit/assets/images/presskit/hidrokit-800x200-transparent.png" alt="logo hidrokit"></a><br>
 
-[![Sponsored by PT. FIAKO Enjiniring Indonesia](https://img.shields.io/badge/sponsored%20by-PT.%20FIAKO%20Enjiniring%20Indonesia-blue.svg)](http://www.fiako.co.id/)
-
 ![PyPI - Status](https://img.shields.io/pypi/status/hidrokit.svg)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hidrokit.svg)
 [![GitHub license](https://img.shields.io/github/license/hidrokit/hidrokit.svg)](https://github.com/hidrokit/hidrokit/blob/master/LICENSE)
 [![DOI](https://zenodo.org/badge/145389179.svg)](https://zenodo.org/badge/latestdoi/145389179)
 
 <a href="https://hidrokit.github.io/hidrokit"><b>Kunjungi situs resmi hidrokit.</b></a>
 </div>
@@ -84,11 +82,11 @@
 Tertarik menjadi kontributor? Baca [**berkontribusi**](https://hidrokit.github.io/hidrokit/berkontribusi) untuk kode etik, melakukan _pull request_, dan penjelasan lebih rinci hal lainnya. Proyek _open-source_ ini terbuka untuk siapa saja dengan berbagai latar belakang.
 
 ## Lisensi
 
 Paket hidrokit menggunakan [lisensi MIT](LICENSE.txt). Dokumentasi yang disertai pada proyek ini menggunakan lisensi [Creative Commons Attribution 4.0 International (CC-BY-4.0)](https://creativecommons.org/licenses/by/4.0/deed.id). 
 ## Acknowledgement
 
-- Terima kasih untuk [PT. FIAKO Enjiniring Indonesia](http://www.fiako.co.id/) (FIAKO ENGINEERING) yang telah mensponsori proyek ini sejak Februari 2022.
+- Terima kasih untuk [PT. FIAKO Enjiniring Indonesia](http://www.fiako.co.id/) (FIAKO ENGINEERING) yang telah mensponsori proyek ini sejak Februari 2022 hingga Februari 2024.
 - Terima kasih untuk **LKO** yang telah mensponsori proyek ini sejak versi 0.2.x hingga 0.3.6.
 - Terima kasih untuk tim hidrokit-syndicate (_Cahya Suryadi_, _Christine Dorty Hadi_, dan _Dicky Muhammad Fadli_) atas dukungannya dalam pengembangan hidrokit. 
 - Terima kasih untuk [@firmansennie](https://www.instagram.com/firmansenie/) untuk design logo hidrokit.
```

#### html2text {}

```diff
@@ -1,16 +1,14 @@
                                 _[_l_o_g_o_ _h_i_d_r_o_k_i_t_]
- [![Sponsored by PT. FIAKO Enjiniring Indonesia](https://img.shields.io/badge/
-    sponsored%20by-PT.%20FIAKO%20Enjiniring%20Indonesia-blue.svg)](http://
-    www.fiako.co.id/) ![PyPI - Status](https://img.shields.io/pypi/status/
-hidrokit.svg) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
-    hidrokit.svg) [![GitHub license](https://img.shields.io/github/license/
-   hidrokit/hidrokit.svg)](https://github.com/hidrokit/hidrokit/blob/master/
- LICENSE) [![DOI](https://zenodo.org/badge/145389179.svg)](https://zenodo.org/
-           badge/latestdoi/145389179) _KK_uu_nn_jj_uu_nn_gg_ii_ _ss_ii_tt_uu_ss_ _rr_ee_ss_mm_ii_ _hh_ii_dd_rr_oo_kk_ii_tt_..
+  ![PyPI - Status](https://img.shields.io/pypi/status/hidrokit.svg) ![PyPI -
+Python Version](https://img.shields.io/pypi/pyversions/hidrokit.svg) [![GitHub
+license](https://img.shields.io/github/license/hidrokit/hidrokit.svg)](https://
+ github.com/hidrokit/hidrokit/blob/master/LICENSE) [![DOI](https://zenodo.org/
+ badge/145389179.svg)](https://zenodo.org/badge/latestdoi/145389179) _KK_uu_nn_jj_uu_nn_gg_ii
+                             _ss_ii_tt_uu_ss_ _rr_ee_ss_mm_ii_ _hh_ii_dd_rr_oo_kk_ii_tt_..
 `hidrokit` adalah proyek _open source_ paket *python* yang dapat digunakan
 untuk membantu proses analisis hidrologi dimulai dari pengolahan data, analisis
 data, dan visualisasi data. [Baca lebih lanjut mengenai hidrokit](https://
 hidrokit.github.io/hidrokit/tentang-hidrokit). ## Release
 RReelleeaassee  PPyyPPII             GGiitthhuubb          GGiitthhuubb ((PPrree--rreelleeaassee))
         [PyPI] [GitHub release]      [GitHub release]
 Date           [GitHub Release Date] [GitHub (Pre-)Release Date]
@@ -41,13 +39,13 @@
 kode etik, melakukan _pull request_, dan penjelasan lebih rinci hal lainnya.
 Proyek _open-source_ ini terbuka untuk siapa saja dengan berbagai latar
 belakang. ## Lisensi Paket hidrokit menggunakan [lisensi MIT](LICENSE.txt).
 Dokumentasi yang disertai pada proyek ini menggunakan lisensi [Creative Commons
 Attribution 4.0 International (CC-BY-4.0)](https://creativecommons.org/
 licenses/by/4.0/deed.id). ## Acknowledgement - Terima kasih untuk [PT. FIAKO
 Enjiniring Indonesia](http://www.fiako.co.id/) (FIAKO ENGINEERING) yang telah
-mensponsori proyek ini sejak Februari 2022. - Terima kasih untuk **LKO** yang
-telah mensponsori proyek ini sejak versi 0.2.x hingga 0.3.6. - Terima kasih
-untuk tim hidrokit-syndicate (_Cahya Suryadi_, _Christine Dorty Hadi_, dan
-_Dicky Muhammad Fadli_) atas dukungannya dalam pengembangan hidrokit. - Terima
-kasih untuk [@firmansennie](https://www.instagram.com/firmansenie/) untuk
-design logo hidrokit.
+mensponsori proyek ini sejak Februari 2022 hingga Februari 2024. - Terima kasih
+untuk **LKO** yang telah mensponsori proyek ini sejak versi 0.2.x hingga 0.3.6.
+- Terima kasih untuk tim hidrokit-syndicate (_Cahya Suryadi_, _Christine Dorty
+Hadi_, dan _Dicky Muhammad Fadli_) atas dukungannya dalam pengembangan
+hidrokit. - Terima kasih untuk [@firmansennie](https://www.instagram.com/
+firmansenie/) untuk design logo hidrokit.
```

### Comparing `hidrokit-0.4.1/hidrokit/contrib/taruma/hk90.py` & `hidrokit-0.5.0/hidrokit/contrib/taruma/model_calibration.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,20 @@
-"""manual:
-https://gist.github.com/taruma/906e1577111208291e0725229c7d0a76
+"""
+hk90: model_calibration.py
+
+This module provides a calibration function that iterates over a parameter grid 
+    and evaluates the performance of a calibrated model using specified metrics.
+
+Functions:
+    calibration(
+        observed, func, calibration_parameter, func_parameter, 
+        metrics, met_names, met_sort, met_min=True, observed_func=None)
+
+For more details, refer to the manual: 
+    https://gist.github.com/taruma/906e1577111208291e0725229c7d0a76
 """
 
 from itertools import product
 import pandas as pd
 
 
 def _parameter_grid(parameter):
@@ -15,47 +26,70 @@
         yield grid
 
 
 def _best_parameter(results, calibration_parameter):
     key = list(calibration_parameter.keys())
     return dict(zip(key, results.iloc[0][key].values))
 
+# pylint: disable=too-many-arguments, too-many-locals
+def calibration(
+    observed,
+    func,
+    calibration_parameter,
+    func_parameter,
+    metrics,
+    met_names,
+    met_sort,
+    met_min=True,
+    observed_func=None,
+):
+    """
+    Perform calibration by iterating over a parameter grid and evaluating the
+    performance of the calibrated model using specified metrics.
+
+    Parameters:
+        observed (array-like): Observed data for calibration.
+        func (callable): Function that represents the model to be calibrated.
+        calibration_parameter (dict): Dictionary of calibration parameters and their values.
+        func_parameter (dict): Dictionary of additional parameters for the model function.
+        metrics (list or tuple): List of metric functions to evaluate the model performance.
+        met_names (list): List of names for the metrics.
+        met_sort (str): Name of the metric to sort the results by.
+        met_min (bool, optional): Whether to sort the results in ascending order of the metric.
+        observed_func (callable, optional): Function to preprocess the observed data.
+
+    Returns:
+        pandas.DataFrame: DataFrame containing the calibration results, including the
+        calibrated parameter values and the evaluation metrics.
 
-def calibration(observed, func, calibration_parameter, func_parameter,
-                metrics, met_names, met_sort, met_min=True,
-                observed_func=None):
-
+    """
     metrics = metrics if isinstance(metrics, (list, tuple)) else [metrics]
-    met_names = (met_names if isinstance(met_names, (list))
-                 else [met_names])
+    met_names = met_names if isinstance(met_names, (list)) else [met_names]
 
     param_grid = list(_parameter_grid(calibration_parameter))
     n_param = len(param_grid)
-    print('N = {}'.format(n_param))
+    print(f"N = {n_param}")
 
-    observed = (
-        observed_func(observed) if observed_func is not None else observed
-    )
+    observed = observed_func(observed) if observed_func is not None else observed
 
     results = []
 
-    print('PROGRESS 0 [-x--xx--x-] 100')
-    print('---------> [', end='')
+    print("PROGRESS 0 [-x--xx--x-] 100")
+    print("---------> [", end="")
 
     for i, p in enumerate(param_grid, start=1):
         simulated = func(**p, **func_parameter)
         met_res = [m(simulated, observed) for m in metrics]
-        results.append(
-            list(p.values()) + met_res
-        )
+        results.append(list(p.values()) + met_res)
         if (i % (n_param // 10)) == 0:
-            print('=', end='')
+            print("=", end="")
+        columns_name = list(p.keys()) + met_names
 
-    print('] DONE')
+    print("] DONE")
 
-    columns_name = list(p.keys()) + met_names
-
-    results = (pd.DataFrame(results, columns=columns_name)
-                 .sort_values(by=met_sort, ascending=met_min)
-                 .reset_index(drop=True))
+    results = (
+        pd.DataFrame(results, columns=columns_name)
+        .sort_values(by=met_sort, ascending=met_min)
+        .reset_index(drop=True)
+    )
 
     return results
```

### Comparing `hidrokit-0.4.1/hidrokit/prep/excel.py` & `hidrokit-0.5.0/hidrokit/prep/excel.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.4.1/hidrokit/prep/read.py` & `hidrokit-0.5.0/hidrokit/prep/read.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.4.1/hidrokit/prep/timeseries.py` & `hidrokit-0.5.0/hidrokit/prep/timeseries.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.4.1/hidrokit/viz/graph.py` & `hidrokit-0.5.0/hidrokit/viz/graph.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.4.1/hidrokit/viz/table.py` & `hidrokit-0.5.0/hidrokit/viz/table.py`

 * *Files identical despite different names*

### Comparing `hidrokit-0.4.1/hidrokit.egg-info/PKG-INFO` & `hidrokit-0.5.0/hidrokit.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hidrokit
-Version: 0.4.1
+Version: 0.5.0
 Summary: analisis hidrologi dengan python
 Home-page: https://github.com/hidrokit/hidrokit
 Author: Taruma Sakti Megariansyah
 Author-email: hi@taruma.info
 License: MIT
 Project-URL: Documentation, https://hidrokit.github.io/hidrokit
 Project-URL: ReadTheDocs, https://hidrokit.readthedocs.io/en/stable/
@@ -12,28 +12,35 @@
 Project-URL: Source, https://github.com/hidrokit/hidrokit/
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.6.0
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
-Provides-Extra: excel
 License-File: LICENSE.txt
+Requires-Dist: matplotlib>=3.7
+Requires-Dist: numpy>=1.25
+Requires-Dist: pandas>=2.0
+Requires-Dist: scipy>=1.11
+Requires-Dist: xlrd>=2.0
+Provides-Extra: excel
+Requires-Dist: openpyxl; extra == "excel"
+Requires-Dist: xlrd; extra == "excel"
+Requires-Dist: xlwt; extra == "excel"
 
 
 
 <div align="center">
 <a href="https://hidrokit.github.io/hidrokit"><img src="https://hidrokit.github.io/hidrokit/assets/images/presskit/hidrokit-800x200-transparent.png" alt="logo hidrokit"></a><br>
 
-[![Sponsored by PT. FIAKO Enjiniring Indonesia](https://img.shields.io/badge/sponsored%20by-PT.%20FIAKO%20Enjiniring%20Indonesia-blue.svg)](http://www.fiako.co.id/)
-
 ![PyPI - Status](https://img.shields.io/pypi/status/hidrokit.svg)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hidrokit.svg)
 [![GitHub license](https://img.shields.io/github/license/hidrokit/hidrokit.svg)](https://github.com/hidrokit/hidrokit/blob/master/LICENSE)
 [![DOI](https://zenodo.org/badge/145389179.svg)](https://zenodo.org/badge/latestdoi/145389179)
 
 <a href="https://hidrokit.github.io/hidrokit"><b>Kunjungi situs resmi hidrokit.</b></a>
 </div>
@@ -110,11 +117,11 @@
 Tertarik menjadi kontributor? Baca [**berkontribusi**](https://hidrokit.github.io/hidrokit/berkontribusi) untuk kode etik, melakukan _pull request_, dan penjelasan lebih rinci hal lainnya. Proyek _open-source_ ini terbuka untuk siapa saja dengan berbagai latar belakang.
 
 ## Lisensi
 
 Paket hidrokit menggunakan [lisensi MIT](LICENSE.txt). Dokumentasi yang disertai pada proyek ini menggunakan lisensi [Creative Commons Attribution 4.0 International (CC-BY-4.0)](https://creativecommons.org/licenses/by/4.0/deed.id). 
 ## Acknowledgement
 
-- Terima kasih untuk [PT. FIAKO Enjiniring Indonesia](http://www.fiako.co.id/) (FIAKO ENGINEERING) yang telah mensponsori proyek ini sejak Februari 2022.
+- Terima kasih untuk [PT. FIAKO Enjiniring Indonesia](http://www.fiako.co.id/) (FIAKO ENGINEERING) yang telah mensponsori proyek ini sejak Februari 2022 hingga Februari 2024.
 - Terima kasih untuk **LKO** yang telah mensponsori proyek ini sejak versi 0.2.x hingga 0.3.6.
 - Terima kasih untuk tim hidrokit-syndicate (_Cahya Suryadi_, _Christine Dorty Hadi_, dan _Dicky Muhammad Fadli_) atas dukungannya dalam pengembangan hidrokit. 
 - Terima kasih untuk [@firmansennie](https://www.instagram.com/firmansenie/) untuk design logo hidrokit.
```

#### html2text {}

```diff
@@ -1,29 +1,31 @@
-Metadata-Version: 2.1 Name: hidrokit Version: 0.4.1 Summary: analisis hidrologi
+Metadata-Version: 2.1 Name: hidrokit Version: 0.5.0 Summary: analisis hidrologi
 dengan python Home-page: https://github.com/hidrokit/hidrokit Author: Taruma
 Sakti Megariansyah Author-email: hi@taruma.info License: MIT Project-URL:
 Documentation, https://hidrokit.github.io/hidrokit Project-URL: ReadTheDocs,
 https://hidrokit.readthedocs.io/en/stable/ Project-URL: Bug Reports, https://
 github.com/hidrokit/hidrokit/issues Project-URL: Source, https://github.com/
 hidrokit/hidrokit/ Classifier: Development Status :: 3 - Alpha Classifier:
 Intended Audience :: Science/Research Classifier: Topic :: Scientific/
 Engineering :: Hydrology Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Requires-Python: >=3.6.0 Description-
-Content-Type: text/markdown Provides-Extra: excel License-File: LICENSE.txt
+Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Requires-Python: >=3.9.0 Description-Content-Type: text/markdown
+License-File: LICENSE.txt Requires-Dist: matplotlib>=3.7 Requires-Dist:
+numpy>=1.25 Requires-Dist: pandas>=2.0 Requires-Dist: scipy>=1.11 Requires-
+Dist: xlrd>=2.0 Provides-Extra: excel Requires-Dist: openpyxl; extra == "excel"
+Requires-Dist: xlrd; extra == "excel" Requires-Dist: xlwt; extra == "excel"
                                 _[_l_o_g_o_ _h_i_d_r_o_k_i_t_]
- [![Sponsored by PT. FIAKO Enjiniring Indonesia](https://img.shields.io/badge/
-    sponsored%20by-PT.%20FIAKO%20Enjiniring%20Indonesia-blue.svg)](http://
-    www.fiako.co.id/) ![PyPI - Status](https://img.shields.io/pypi/status/
-hidrokit.svg) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
-    hidrokit.svg) [![GitHub license](https://img.shields.io/github/license/
-   hidrokit/hidrokit.svg)](https://github.com/hidrokit/hidrokit/blob/master/
- LICENSE) [![DOI](https://zenodo.org/badge/145389179.svg)](https://zenodo.org/
-           badge/latestdoi/145389179) _KK_uu_nn_jj_uu_nn_gg_ii_ _ss_ii_tt_uu_ss_ _rr_ee_ss_mm_ii_ _hh_ii_dd_rr_oo_kk_ii_tt_..
+  ![PyPI - Status](https://img.shields.io/pypi/status/hidrokit.svg) ![PyPI -
+Python Version](https://img.shields.io/pypi/pyversions/hidrokit.svg) [![GitHub
+license](https://img.shields.io/github/license/hidrokit/hidrokit.svg)](https://
+ github.com/hidrokit/hidrokit/blob/master/LICENSE) [![DOI](https://zenodo.org/
+ badge/145389179.svg)](https://zenodo.org/badge/latestdoi/145389179) _KK_uu_nn_jj_uu_nn_gg_ii
+                             _ss_ii_tt_uu_ss_ _rr_ee_ss_mm_ii_ _hh_ii_dd_rr_oo_kk_ii_tt_..
 `hidrokit` adalah proyek _open source_ paket *python* yang dapat digunakan
 untuk membantu proses analisis hidrologi dimulai dari pengolahan data, analisis
 data, dan visualisasi data. [Baca lebih lanjut mengenai hidrokit](https://
 hidrokit.github.io/hidrokit/tentang-hidrokit). ## Release
 RReelleeaassee  PPyyPPII             GGiitthhuubb          GGiitthhuubb ((PPrree--rreelleeaassee))
         [PyPI] [GitHub release]      [GitHub release]
 Date           [GitHub Release Date] [GitHub (Pre-)Release Date]
@@ -54,13 +56,13 @@
 kode etik, melakukan _pull request_, dan penjelasan lebih rinci hal lainnya.
 Proyek _open-source_ ini terbuka untuk siapa saja dengan berbagai latar
 belakang. ## Lisensi Paket hidrokit menggunakan [lisensi MIT](LICENSE.txt).
 Dokumentasi yang disertai pada proyek ini menggunakan lisensi [Creative Commons
 Attribution 4.0 International (CC-BY-4.0)](https://creativecommons.org/
 licenses/by/4.0/deed.id). ## Acknowledgement - Terima kasih untuk [PT. FIAKO
 Enjiniring Indonesia](http://www.fiako.co.id/) (FIAKO ENGINEERING) yang telah
-mensponsori proyek ini sejak Februari 2022. - Terima kasih untuk **LKO** yang
-telah mensponsori proyek ini sejak versi 0.2.x hingga 0.3.6. - Terima kasih
-untuk tim hidrokit-syndicate (_Cahya Suryadi_, _Christine Dorty Hadi_, dan
-_Dicky Muhammad Fadli_) atas dukungannya dalam pengembangan hidrokit. - Terima
-kasih untuk [@firmansennie](https://www.instagram.com/firmansenie/) untuk
-design logo hidrokit.
+mensponsori proyek ini sejak Februari 2022 hingga Februari 2024. - Terima kasih
+untuk **LKO** yang telah mensponsori proyek ini sejak versi 0.2.x hingga 0.3.6.
+- Terima kasih untuk tim hidrokit-syndicate (_Cahya Suryadi_, _Christine Dorty
+Hadi_, dan _Dicky Muhammad Fadli_) atas dukungannya dalam pengembangan
+hidrokit. - Terima kasih untuk [@firmansennie](https://www.instagram.com/
+firmansenie/) untuk design logo hidrokit.
```

### Comparing `hidrokit-0.4.1/setup.py` & `hidrokit-0.5.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,20 +13,24 @@
 
 # Package meta-data.
 NAME = 'hidrokit'
 DESCRIPTION = 'analisis hidrologi dengan python'
 URL = 'https://github.com/hidrokit/hidrokit'
 EMAIL = 'hi@taruma.info'
 AUTHOR = 'Taruma Sakti Megariansyah'
-REQUIRES_PYTHON = '>=3.6.0'
+REQUIRES_PYTHON = '>=3.9.0'
 VERSION = ''
 
 # What packages are required for this module to be executed?
 REQUIRED = [
-    'numpy', 'pandas', 'matplotlib',
+    'matplotlib>=3.7',
+    'numpy>=1.25',
+    'pandas>=2.0',
+    'scipy>=1.11',
+    'xlrd>=2.0',
 ]
 
 # What packages are optional?
 EXTRAS = {
     'excel': ['openpyxl', 'xlrd', 'xlwt'],
 }
 
@@ -90,16 +94,17 @@
 
         # License
         'License :: OSI Approved :: MIT License',
 
         # Python Version
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
 
     project_urls={
         'Documentation': 'https://hidrokit.github.io/hidrokit',
         'ReadTheDocs': 'https://hidrokit.readthedocs.io/en/stable/',
         'Bug Reports': 'https://github.com/hidrokit/hidrokit/issues',
         'Source': 'https://github.com/hidrokit/hidrokit/',
```

