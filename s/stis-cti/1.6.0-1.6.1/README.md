# Comparing `tmp/stis_cti-1.6.0.tar.gz` & `tmp/stis_cti-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stis_cti-1.6.0.tar", last modified: Fri Apr 12 15:24:51 2024, max compression
+gzip compressed data, was "stis_cti-1.6.1.tar", last modified: Tue Apr 16 02:58:10 2024, max compression
```

## Comparing `stis_cti-1.6.0.tar` & `stis_cti-1.6.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 lockwood  (4945) STSCI\science  (1031)        0 2024-04-12 15:24:51.330191 stis_cti-1.6.0/
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)     1464 2020-12-15 11:24:35.000000 stis_cti-1.6.0/LICENSE.txt
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)      306 2020-12-15 11:24:35.000000 stis_cti-1.6.0/MANIFEST.in
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)     2459 2024-04-12 15:24:51.330021 stis_cti-1.6.0/PKG-INFO
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)     1154 2024-03-05 17:37:38.000000 stis_cti-1.6.0/README.rst
-drwxr-xr-x   0 lockwood  (4945) STSCI\science  (1031)        0 2024-04-12 15:24:51.323955 stis_cti-1.6.0/doc/
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)     6770 2020-12-15 11:24:35.000000 stis_cti-1.6.0/doc/Makefile
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)    10828 2024-04-12 15:21:44.000000 stis_cti-1.6.0/doc/conf.py
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)      344 2024-03-01 19:23:31.000000 stis_cti-1.6.0/doc/index.rst
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)     6705 2020-12-15 11:24:35.000000 stis_cti-1.6.0/doc/make.bat
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)  1108934 2020-12-15 11:24:35.000000 stis_cti-1.6.0/doc/obr101010_comparison.png
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)     5748 2024-03-01 21:43:38.000000 stis_cti-1.6.0/doc/qsg.rst
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)    20583 2024-04-12 15:21:44.000000 stis_cti-1.6.0/doc/readme.rst
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)      621 2024-03-01 19:23:45.000000 stis_cti-1.6.0/doc/stis_cti.rst
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)       38 2024-04-12 15:24:51.330242 stis_cti-1.6.0/setup.cfg
--rwxr-xr-x   0 lockwood  (4945) STSCI\science  (1031)     2378 2024-04-12 15:21:44.000000 stis_cti-1.6.0/setup.py
-drwxr-xr-x   0 lockwood  (4945) STSCI\science  (1031)        0 2024-04-12 15:24:51.325096 stis_cti-1.6.0/src/
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)    11110 2020-12-15 11:24:35.000000 stis_cti-1.6.0/src/StisFixYCte.c
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)     2759 2020-12-15 11:24:35.000000 stis_cti-1.6.0/src/StisPixCteCorr.h
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)    13400 2020-12-15 11:24:35.000000 stis_cti-1.6.0/src/StisPixCteCorr_funcs.c
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)    15113 2021-07-27 15:04:12.000000 stis_cti-1.6.0/src/StisPixCte_FixY.c
-drwxr-xr-x   0 lockwood  (4945) STSCI\science  (1031)        0 2024-04-12 15:24:51.326862 stis_cti-1.6.0/stis_cti/
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)    33710 2024-02-26 20:40:16.000000 stis_cti-1.6.0/stis_cti/StisPixCteCorr.py
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)      437 2021-07-27 15:04:12.000000 stis_cti-1.6.0/stis_cti/__init__.py
--rwxr-xr-x   0 lockwood  (4945) STSCI\science  (1031)    13815 2024-02-26 22:03:22.000000 stis_cti-1.6.0/stis_cti/archive_dark_query.py
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)     3378 2021-07-27 15:04:12.000000 stis_cti-1.6.0/stis_cti/custom_superdark_info.py
-drwxr-xr-x   0 lockwood  (4945) STSCI\science  (1031)        0 2024-04-12 15:24:51.329111 stis_cti-1.6.0/stis_cti/data/
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)    51840 2020-12-15 11:24:35.000000 stis_cti-1.6.0/stis_cti/data/a01_stis_pcte.fits
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)    51840 2024-04-12 15:21:44.000000 stis_cti-1.6.0/stis_cti/data/a02_stis_pcte.fits
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)    58980 2024-04-12 15:21:44.000000 stis_cti-1.6.0/stis_cti/stis_cti.py
--rwxr-xr-x   0 lockwood  (4945) STSCI\science  (1031)    21193 2021-07-27 15:04:12.000000 stis_cti-1.6.0/stis_cti/unit_tests.py
-drwxr-xr-x   0 lockwood  (4945) STSCI\science  (1031)        0 2024-04-12 15:24:51.328142 stis_cti-1.6.0/stis_cti.egg-info/
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)     2459 2024-04-12 15:24:51.000000 stis_cti-1.6.0/stis_cti.egg-info/PKG-INFO
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)      673 2024-04-12 15:24:51.000000 stis_cti-1.6.0/stis_cti.egg-info/SOURCES.txt
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)        1 2024-04-12 15:24:51.000000 stis_cti-1.6.0/stis_cti.egg-info/dependency_links.txt
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)      134 2024-04-12 15:24:51.000000 stis_cti-1.6.0/stis_cti.egg-info/entry_points.txt
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)       88 2024-04-12 15:24:51.000000 stis_cti-1.6.0/stis_cti.egg-info/requires.txt
--rw-r--r--   0 lockwood  (4945) STSCI\science  (1031)        9 2024-04-12 15:24:51.000000 stis_cti-1.6.0/stis_cti.egg-info/top_level.txt
+drwxr-xr-x   0 lockwood  (4945)     1031        0 2024-04-16 02:58:10.502390 stis_cti-1.6.1/
+-rw-r--r--   0 lockwood  (4945)     1031     1464 2020-12-15 11:24:35.000000 stis_cti-1.6.1/LICENSE.txt
+-rw-r--r--   0 lockwood  (4945)     1031      306 2020-12-15 11:24:35.000000 stis_cti-1.6.1/MANIFEST.in
+-rw-r--r--   0 lockwood  (4945)     1031     2667 2024-04-16 02:58:10.502115 stis_cti-1.6.1/PKG-INFO
+-rw-r--r--   0 lockwood  (4945)     1031     1154 2024-03-05 17:37:38.000000 stis_cti-1.6.1/README.rst
+drwxr-xr-x   0 lockwood  (4945)     1031        0 2024-04-16 02:58:10.497015 stis_cti-1.6.1/doc/
+-rw-r--r--   0 lockwood  (4945)     1031     6770 2020-12-15 11:24:35.000000 stis_cti-1.6.1/doc/Makefile
+-rw-r--r--   0 lockwood  (4945)     1031    10828 2024-04-16 02:49:41.000000 stis_cti-1.6.1/doc/conf.py
+-rw-r--r--   0 lockwood  (4945)     1031      344 2024-03-01 19:23:31.000000 stis_cti-1.6.1/doc/index.rst
+-rw-r--r--   0 lockwood  (4945)     1031     6705 2020-12-15 11:24:35.000000 stis_cti-1.6.1/doc/make.bat
+-rw-r--r--   0 lockwood  (4945)     1031  1108934 2020-12-15 11:24:35.000000 stis_cti-1.6.1/doc/obr101010_comparison.png
+-rw-r--r--   0 lockwood  (4945)     1031     5748 2024-03-01 21:43:38.000000 stis_cti-1.6.1/doc/qsg.rst
+-rw-r--r--   0 lockwood  (4945)     1031    20583 2024-04-16 02:49:41.000000 stis_cti-1.6.1/doc/readme.rst
+-rw-r--r--   0 lockwood  (4945)     1031      621 2024-03-01 19:23:45.000000 stis_cti-1.6.1/doc/stis_cti.rst
+-rw-r--r--   0 lockwood  (4945)     1031       38 2024-04-16 02:58:10.502447 stis_cti-1.6.1/setup.cfg
+-rwxr-xr-x   0 lockwood  (4945)     1031     2449 2024-04-16 02:49:41.000000 stis_cti-1.6.1/setup.py
+drwxr-xr-x   0 lockwood  (4945)     1031        0 2024-04-16 02:58:10.497738 stis_cti-1.6.1/src/
+-rw-r--r--   0 lockwood  (4945)     1031    11110 2020-12-15 11:24:35.000000 stis_cti-1.6.1/src/StisFixYCte.c
+-rw-r--r--   0 lockwood  (4945)     1031     2766 2024-04-16 00:43:37.000000 stis_cti-1.6.1/src/StisPixCteCorr.h
+-rw-r--r--   0 lockwood  (4945)     1031    13400 2020-12-15 11:24:35.000000 stis_cti-1.6.1/src/StisPixCteCorr_funcs.c
+-rw-r--r--   0 lockwood  (4945)     1031    15263 2024-04-16 00:43:37.000000 stis_cti-1.6.1/src/StisPixCte_FixY.c
+drwxr-xr-x   0 lockwood  (4945)     1031        0 2024-04-16 02:58:10.499246 stis_cti-1.6.1/stis_cti/
+-rw-r--r--   0 lockwood  (4945)     1031    33710 2024-02-26 20:40:16.000000 stis_cti-1.6.1/stis_cti/StisPixCteCorr.py
+-rw-r--r--   0 lockwood  (4945)     1031      437 2021-07-27 15:04:12.000000 stis_cti-1.6.1/stis_cti/__init__.py
+-rwxr-xr-x   0 lockwood  (4945)     1031    13815 2024-02-26 22:03:22.000000 stis_cti-1.6.1/stis_cti/archive_dark_query.py
+-rw-r--r--   0 lockwood  (4945)     1031     3378 2021-07-27 15:04:12.000000 stis_cti-1.6.1/stis_cti/custom_superdark_info.py
+drwxr-xr-x   0 lockwood  (4945)     1031        0 2024-04-16 02:58:10.501059 stis_cti-1.6.1/stis_cti/data/
+-rw-r--r--   0 lockwood  (4945)     1031    51840 2020-12-15 11:24:35.000000 stis_cti-1.6.1/stis_cti/data/a01_stis_pcte.fits
+-rw-r--r--   0 lockwood  (4945)     1031    51840 2024-04-12 15:21:44.000000 stis_cti-1.6.1/stis_cti/data/a02_stis_pcte.fits
+-rw-r--r--   0 lockwood  (4945)     1031    58980 2024-04-16 02:49:41.000000 stis_cti-1.6.1/stis_cti/stis_cti.py
+-rwxr-xr-x   0 lockwood  (4945)     1031    21339 2024-04-16 02:49:41.000000 stis_cti-1.6.1/stis_cti/unit_tests.py
+drwxr-xr-x   0 lockwood  (4945)     1031        0 2024-04-16 02:58:10.501744 stis_cti-1.6.1/stis_cti.egg-info/
+-rw-r--r--   0 lockwood  (4945)     1031     2667 2024-04-16 02:58:10.000000 stis_cti-1.6.1/stis_cti.egg-info/PKG-INFO
+-rw-r--r--   0 lockwood  (4945)     1031      673 2024-04-16 02:58:10.000000 stis_cti-1.6.1/stis_cti.egg-info/SOURCES.txt
+-rw-r--r--   0 lockwood  (4945)     1031        1 2024-04-16 02:58:10.000000 stis_cti-1.6.1/stis_cti.egg-info/dependency_links.txt
+-rw-r--r--   0 lockwood  (4945)     1031      134 2024-04-16 02:58:10.000000 stis_cti-1.6.1/stis_cti.egg-info/entry_points.txt
+-rw-r--r--   0 lockwood  (4945)     1031       88 2024-04-16 02:58:10.000000 stis_cti-1.6.1/stis_cti.egg-info/requires.txt
+-rw-r--r--   0 lockwood  (4945)     1031        9 2024-04-16 02:58:10.000000 stis_cti-1.6.1/stis_cti.egg-info/top_level.txt
```

### Comparing `stis_cti-1.6.0/LICENSE.txt` & `stis_cti-1.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stis_cti-1.6.0/PKG-INFO` & `stis_cti-1.6.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stis_cti
-Version: 1.6.0
+Version: 1.6.1
 Summary: Pixel-based CTI-correction for HST/STIS CCD data
 Home-page: https://www.stsci.edu/hst/instrumentation/stis/data-analysis-and-software-tools/pixel-based-cti
 Author: Sean Lockwood, Phil Hodge, Pey Lian Lim, W.J. Hack, J. Anderson, Matt Davis
 Author-email: lockwood@stsci.edu
 Maintainer: Sean Lockwood
 Maintainer-email: lockwood@stsci.edu
 License: BSD-new
@@ -20,14 +20,22 @@
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE.txt
+Requires-Dist: setuptools
+Requires-Dist: numpy
+Requires-Dist: astropy>=4.0
+Requires-Dist: stistools>=1.2
+Requires-Dist: refstis>=0.8.1
+Requires-Dist: crds
+Requires-Dist: stsci.tools>=3.2.2
+Requires-Dist: six
 
 HST/STIS Pixel-Based CTI-Correction Scripts
 ===========================================
 
 Utilities needed to correct for Charge Transfer Inefficiency (CTI) in the Hubble
 Space Telescope (HST) STIS CCD.
```

### Comparing `stis_cti-1.6.0/README.rst` & `stis_cti-1.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `stis_cti-1.6.0/doc/Makefile` & `stis_cti-1.6.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `stis_cti-1.6.0/doc/conf.py` & `stis_cti-1.6.1/doc/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,17 +52,17 @@
 copyright = '2015, AURA-STScI'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '1.6.0'
+version = '1.6.1'
 # The full version, including alpha/beta/rc tags.
-release = '1.6.0'
+release = '1.6.1'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
```

### Comparing `stis_cti-1.6.0/doc/make.bat` & `stis_cti-1.6.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `stis_cti-1.6.0/doc/obr101010_comparison.png` & `stis_cti-1.6.1/doc/obr101010_comparison.png`

 * *Files identical despite different names*

### Comparing `stis_cti-1.6.0/doc/qsg.rst` & `stis_cti-1.6.1/doc/qsg.rst`

 * *Files identical despite different names*

### Comparing `stis_cti-1.6.0/doc/readme.rst` & `stis_cti-1.6.1/doc/readme.rst`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
     --clean           remove intermediate and final products from previous runs
                       of this script ('*.txt' files are skipped and clobbered)
     --clean_all       '--clean' + remove previous super-darks and CTI-corrected
                       component darks
     --ignore_missing  process data even with an incomplete set of dark FLTs
     -v VERBOSE_LEVEL  verbosity ({0,1,2}; default=1)
 
-  Written by Sean Lockwood; v1.6.0
+  Written by Sean Lockwood; v1.6.1
 
 The script is designed to run the pixel-based correction in parallel on the component 
 darks, and in parallel on the science files.  The maximum number of processes may be 
 specified via the ``-n #`` option.
 
 A typical call looks like::
```

### Comparing `stis_cti-1.6.0/doc/stis_cti.rst` & `stis_cti-1.6.1/doc/stis_cti.rst`

 * *Files identical despite different names*

### Comparing `stis_cti-1.6.0/setup.py` & `stis_cti-1.6.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,26 +6,27 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(here, 'README.rst')) as f:
     long_description = f.read()
 
 StisPixCteCorr_module = Extension('stis_cti.StisPixCte_FixY',
     sources=['src/StisFixYCte.c', 'src/StisPixCteCorr_funcs.c', 'src/StisPixCte_FixY.c'],
-    include_dirs=[numpy.get_include(), 'src/'])
+    include_dirs=[numpy.get_include(), 'src/'],
+    define_macros=[('NPY_NO_DEPRECATED_API', 'NPY_1_7_API_VERSION')],)
 
 setup(
     name = 'stis_cti',
     url = 'https://www.stsci.edu/hst/instrumentation/stis/data-analysis-and-software-tools/pixel-based-cti',
     project_urls={
         'Homepage': 'https://www.stsci.edu/hst/instrumentation/stis/data-analysis-and-software-tools/pixel-based-cti',
         'Documentation': 'https://stis-cti.readthedocs.io',
         'Help Desk': 'https://hsthelp.stsci.edu',
         'Source Code': 'https://github.com/spacetelescope/stis_cti',
         'Issues': 'https://github.com/spacetelescope/stis_cti/issues',},
-    version = '1.6.0',
+    version = '1.6.1',
     description = 'Pixel-based CTI-correction for HST/STIS CCD data',
     long_description = long_description,
     author = 'Sean Lockwood, Phil Hodge, Pey Lian Lim, W.J. Hack, J. Anderson, Matt Davis',
     author_email = 'lockwood@stsci.edu',
     maintainer = 'Sean Lockwood',
     maintainer_email = 'lockwood@stsci.edu',
     license = 'BSD-new',
```

### Comparing `stis_cti-1.6.0/src/StisFixYCte.c` & `stis_cti-1.6.1/src/StisFixYCte.c`

 * *Files identical despite different names*

### Comparing `stis_cti-1.6.0/src/StisPixCteCorr.h` & `stis_cti-1.6.1/src/StisPixCteCorr.h`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 /* parameters of readout noise decomposition routines */
 #define NOISE_MODEL 1
 
 /* function prototypes */
 double CalcCteFrac(const double expstart, const double scalemjd[NUM_SCALE],
                    const double scaleval[NUM_SCALE]);
-int InterpolatePsi(const double chg_leak[NUM_PSI*NUM_LOGQ], const int psi_node[],
+int InterpolatePsi(const double chg_leak[NUM_PSI*NUM_LOGQ], const int psi_node[NUM_PSI],
                    double chg_leak_interp[MAX_TAIL_LEN*NUM_LOGQ],
                    double chg_open_interp[MAX_TAIL_LEN*NUM_LOGQ]);
 int InterpolatePhi(const double dtde_l[NUM_PHI], const int q_dtde[NUM_PHI],
                    const int shft_nit, double dtde_q[MAX_PHI]);
 int FillLevelArrays(const double chg_leak_kt[MAX_TAIL_LEN*NUM_LOGQ],
                     const double chg_open_kt[MAX_TAIL_LEN*NUM_LOGQ],
                     const double dtde_q[MAX_PHI], const int levels[NUM_LEV],
```

### Comparing `stis_cti-1.6.0/src/StisPixCteCorr_funcs.c` & `stis_cti-1.6.1/src/StisPixCteCorr_funcs.c`

 * *Files identical despite different names*

### Comparing `stis_cti-1.6.0/src/StisPixCte_FixY.c` & `stis_cti-1.6.1/src/StisPixCte_FixY.c`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
   
   /* put arguments into variables */
   if (!PyArg_ParseTuple(args, "dOO", &mjd, &opy_scale_mjd, &opy_scale_val)) {
     return NULL;
   }
   
   py_scale_mjd = (PyArrayObject *) PyArray_FROMANY(opy_scale_mjd, NPY_DOUBLE, 
-                                                    1, 1, NPY_IN_ARRAY);
+                                                    1, 1, NPY_ARRAY_IN_ARRAY);
   py_scale_val = (PyArrayObject *) PyArray_FROMANY(opy_scale_val, NPY_DOUBLE, 
-                                                    1, 1, NPY_IN_ARRAY);
+                                                    1, 1, NPY_ARRAY_IN_ARRAY);
   
   /* get cte_frac */
   cte_frac = CalcCteFrac(mjd, (double *) PyArray_DATA(py_scale_mjd),
                          (double *) PyArray_DATA(py_scale_val));
   
   /* test whether it's good */
   if (cte_frac < 0) {
@@ -61,16 +61,16 @@
   }
   
   /* put arguments into variables */
   if (!PyArg_ParseTuple(args, "OO", &opy_chg_leak, &opy_psi_node)) {
     return NULL;
   }
   
-  py_psi_node = (PyArrayObject *) PyArray_FROMANY(opy_psi_node, NPY_INT, 1, 1, NPY_IN_ARRAY);
-  py_chg_leak = (PyArrayObject *) PyArray_FROMANY(opy_chg_leak, NPY_DOUBLE, 2, 2, NPY_IN_ARRAY);
+  py_psi_node = (PyArrayObject *) PyArray_FROMANY(opy_psi_node, NPY_INT, 1, 1, NPY_ARRAY_IN_ARRAY);
+  py_chg_leak = (PyArrayObject *) PyArray_FROMANY(opy_chg_leak, NPY_DOUBLE, 2, 2, NPY_ARRAY_IN_ARRAY);
   if (!py_psi_node || !py_chg_leak) {
     return NULL;
   }
   
   /* call InterpolatePsi */
   status = InterpolatePsi((double *) PyArray_DATA(py_chg_leak), 
                           (int *) PyArray_DATA(py_psi_node), 
@@ -106,16 +106,16 @@
   }
  
   /* put arguments into variables */
   if (!PyArg_ParseTuple(args, "OOi", &opy_dtde_l, &opy_q_dtde, &shft_nit)) {
     return NULL;
   }
    
-  py_dtde_l = (PyArrayObject *) PyArray_FROMANY(opy_dtde_l, NPY_DOUBLE, 1, 1, NPY_IN_ARRAY);
-  py_q_dtde = (PyArrayObject *) PyArray_FROMANY(opy_q_dtde, NPY_INT, 1, 1, NPY_IN_ARRAY);
+  py_dtde_l = (PyArrayObject *) PyArray_FROMANY(opy_dtde_l, NPY_DOUBLE, 1, 1, NPY_ARRAY_IN_ARRAY);
+  py_q_dtde = (PyArrayObject *) PyArray_FROMANY(opy_q_dtde, NPY_INT, 1, 1, NPY_ARRAY_IN_ARRAY);
   if (!py_dtde_l || !py_q_dtde) {
     return NULL;
   }
   
   /* call InterpolatePhi */
   status = InterpolatePhi((double *) PyArray_DATA(py_dtde_l),
                           (int *) PyArray_DATA(py_q_dtde), shft_nit,
@@ -156,19 +156,19 @@
   /* put input arguments into variables */
   if (!PyArg_ParseTuple(args, "OOOO", &opy_chg_leak_kt, &opy_chg_open_kt,
                                       &opy_dtde_q, &opy_levels)) {
     return NULL;
   }
   
   py_chg_leak_kt = 
-    (PyArrayObject *) PyArray_FROMANY(opy_chg_leak_kt, NPY_DOUBLE, 2, 2, NPY_IN_ARRAY);
+    (PyArrayObject *) PyArray_FROMANY(opy_chg_leak_kt, NPY_DOUBLE, 2, 2, NPY_ARRAY_IN_ARRAY);
   py_chg_open_kt = 
-    (PyArrayObject *) PyArray_FROMANY(opy_chg_open_kt, NPY_DOUBLE, 2, 2, NPY_IN_ARRAY);
-  py_dtde_q = (PyArrayObject *) PyArray_FROMANY(opy_dtde_q, NPY_DOUBLE, 1, 1, NPY_IN_ARRAY);
-  py_levels = (PyArrayObject *) PyArray_FROMANY(opy_levels, NPY_INT, 1, 1, NPY_IN_ARRAY);
+    (PyArrayObject *) PyArray_FROMANY(opy_chg_open_kt, NPY_DOUBLE, 2, 2, NPY_ARRAY_IN_ARRAY);
+  py_dtde_q = (PyArrayObject *) PyArray_FROMANY(opy_dtde_q, NPY_DOUBLE, 1, 1, NPY_ARRAY_IN_ARRAY);
+  py_levels = (PyArrayObject *) PyArray_FROMANY(opy_levels, NPY_INT, 1, 1, NPY_ARRAY_IN_ARRAY);
   if (!py_chg_leak_kt || !py_chg_open_kt || !py_dtde_q || !py_levels) {
     return NULL;
   }
   
   /* call FillLevelArrays */
   status = FillLevelArrays((double *) PyArray_DATA(py_chg_leak_kt),
                            (double *) PyArray_DATA(py_chg_open_kt),
@@ -208,22 +208,22 @@
   PyArrayObject * py_noise;
   
   /* put arguments into variables */
   if (!PyArg_ParseTuple(args, "Odi", &opy_data, &pclip, &noise_model)) {
     return NULL;
   }
   
-  py_data = (PyArrayObject *) PyArray_FROMANY(opy_data, NPY_DOUBLE, 2, 2, NPY_IN_ARRAY);
+  py_data = (PyArrayObject *) PyArray_FROMANY(opy_data, NPY_DOUBLE, 2, 2, NPY_ARRAY_IN_ARRAY);
   if (!py_data) {
     return NULL;
   }
   
   /* assign/allocate local variables */
-  arrx = py_data->dimensions[0];
-  arry = py_data->dimensions[1];
+  arrx = PyArray_DIMS(py_data)[0];
+  arry = PyArray_DIMS(py_data)[1];
   
   /* return variables */
   out_dim = (npy_intp *) malloc(2 * sizeof(npy_intp));
   out_dim[0] = (npy_intp) arrx;
   out_dim[1] = (npy_intp) arry;  
   py_sig = (PyArrayObject *) PyArray_SimpleNew(2, out_dim, NPY_DOUBLE);
   py_noise = (PyArrayObject *) PyArray_SimpleNew(2, out_dim, NPY_DOUBLE);
@@ -269,33 +269,33 @@
   if (!PyArg_ParseTuple(args, "OiidOOOOO", &opy_sig_cte, &sim_nit, &shft_nit,
                         &sub_thresh, &opy_cte_frac, &opy_levels, &opy_dpde_l, 
                         &opy_chg_leak_lt, &opy_chg_open_lt)) {
     return NULL;
   }
   
   py_sig_cte = (PyArrayObject *) PyArray_FROMANY(opy_sig_cte, NPY_DOUBLE,
-                                                 2, 2, NPY_IN_ARRAY);
+                                                 2, 2, NPY_ARRAY_IN_ARRAY);
   py_cte_frac = (PyArrayObject *) PyArray_FROMANY(opy_cte_frac, NPY_DOUBLE,
-                                                  2, 2, NPY_IN_ARRAY);
+                                                  2, 2, NPY_ARRAY_IN_ARRAY);
   py_levels = (PyArrayObject *) PyArray_FROMANY(opy_levels, NPY_INT,
-                                                1, 1, NPY_IN_ARRAY);
+                                                1, 1, NPY_ARRAY_IN_ARRAY);
   py_dpde_l = (PyArrayObject *) PyArray_FROMANY(opy_dpde_l, NPY_DOUBLE,
-                                                1, 1, NPY_IN_ARRAY);
+                                                1, 1, NPY_ARRAY_IN_ARRAY);
   py_chg_leak_lt = (PyArrayObject *) PyArray_FROMANY(opy_chg_leak_lt, NPY_DOUBLE, 
-                                                     2, 2, NPY_IN_ARRAY);
+                                                     2, 2, NPY_ARRAY_IN_ARRAY);
   py_chg_open_lt = (PyArrayObject *) PyArray_FROMANY(opy_chg_open_lt, NPY_DOUBLE, 
-                                                     2, 2, NPY_IN_ARRAY);
+                                                     2, 2, NPY_ARRAY_IN_ARRAY);
   if (!py_sig_cte || !py_cte_frac || !py_levels || !py_dpde_l || 
       !py_chg_leak_lt || !py_chg_open_lt) {
     return NULL;
   }
   
   /* local variables */
-  arrx = py_sig_cte->dimensions[0];
-  arry = py_sig_cte->dimensions[1];
+  arrx = PyArray_DIMS(py_sig_cte)[0];
+  arry = PyArray_DIMS(py_sig_cte)[1];
   
   /* return variables */
   out_dim = (npy_intp *) malloc(2 * sizeof(npy_intp));
   out_dim[0] = (npy_intp) arrx;
   out_dim[1] = (npy_intp) arry;
   py_sig_cor = (PyArrayObject *) PyArray_SimpleNew(2, out_dim, NPY_DOUBLE);
   if (!py_sig_cor) {
@@ -348,33 +348,33 @@
   if (!PyArg_ParseTuple(args, "OiOOOOO", &opy_sig_cte, &shft_nit, 
                         &opy_cte_frac, &opy_levels, &opy_dpde_l, 
                         &opy_chg_leak_lt, &opy_chg_open_lt)) {
     return NULL;
   }
   
   py_sig_cte = (PyArrayObject *) PyArray_FROMANY(opy_sig_cte, NPY_DOUBLE,
-                                                 2, 2, NPY_IN_ARRAY);
+                                                 2, 2, NPY_ARRAY_IN_ARRAY);
   py_cte_frac = (PyArrayObject *) PyArray_FROMANY(opy_cte_frac, NPY_DOUBLE,
-                                                  2, 2, NPY_IN_ARRAY);
+                                                  2, 2, NPY_ARRAY_IN_ARRAY);
   py_levels = (PyArrayObject *) PyArray_FROMANY(opy_levels, NPY_INT,
-                                                1, 1, NPY_IN_ARRAY);
+                                                1, 1, NPY_ARRAY_IN_ARRAY);
   py_dpde_l = (PyArrayObject *) PyArray_FROMANY(opy_dpde_l, NPY_DOUBLE,
-                                                1, 1, NPY_IN_ARRAY);
+                                                1, 1, NPY_ARRAY_IN_ARRAY);
   py_chg_leak_lt = (PyArrayObject *) PyArray_FROMANY(opy_chg_leak_lt, NPY_DOUBLE, 
-                                                     2, 2, NPY_IN_ARRAY);
+                                                     2, 2, NPY_ARRAY_IN_ARRAY);
   py_chg_open_lt = (PyArrayObject *) PyArray_FROMANY(opy_chg_open_lt, NPY_DOUBLE, 
-                                                     2, 2, NPY_IN_ARRAY);
+                                                     2, 2, NPY_ARRAY_IN_ARRAY);
   if (!py_sig_cte || !py_cte_frac || !py_levels || !py_dpde_l || 
       !py_chg_leak_lt || !py_chg_open_lt) {
     return NULL;
   }
   
   /* local variables */
-  arrx = py_sig_cte->dimensions[0];
-  arry = py_sig_cte->dimensions[1];
+  arrx = PyArray_DIMS(py_sig_cte)[0];
+  arry = PyArray_DIMS(py_sig_cte)[1];
   
   /* return variables */
   out_dim = (npy_intp *) malloc(2 * sizeof(npy_intp));
   out_dim[0] = (npy_intp) arrx;
   out_dim[1] = (npy_intp) arry;
   py_sig_cor = (PyArrayObject *) PyArray_SimpleNew(2, out_dim, NPY_DOUBLE);
   if (!py_sig_cor) {
```

### Comparing `stis_cti-1.6.0/stis_cti/StisPixCteCorr.py` & `stis_cti-1.6.1/stis_cti/StisPixCteCorr.py`

 * *Files identical despite different names*

### Comparing `stis_cti-1.6.0/stis_cti/archive_dark_query.py` & `stis_cti-1.6.1/stis_cti/archive_dark_query.py`

 * *Files identical despite different names*

### Comparing `stis_cti-1.6.0/stis_cti/custom_superdark_info.py` & `stis_cti-1.6.1/stis_cti/custom_superdark_info.py`

 * *Files identical despite different names*

### Comparing `stis_cti-1.6.0/stis_cti/data/a01_stis_pcte.fits` & `stis_cti-1.6.1/stis_cti/data/a01_stis_pcte.fits`

 * *Files identical despite different names*

### Comparing `stis_cti-1.6.0/stis_cti/data/a02_stis_pcte.fits` & `stis_cti-1.6.1/stis_cti/data/a02_stis_pcte.fits`

 * *Files identical despite different names*

### Comparing `stis_cti-1.6.0/stis_cti/stis_cti.py` & `stis_cti-1.6.1/stis_cti/stis_cti.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from . import archive_dark_query
 from . import StisPixCteCorr
 from crds.bestrefs import BestrefsScript
 from multiprocessing import cpu_count
 
 
 __author__  = 'Sean Lockwood'
-__version__ = '1.6.0'
+__version__ = '1.6.1'
 
 crds_server_url = 'https://hst-crds.stsci.edu'
 
 class FileError(Exception):
     pass
 
 class VersionError(Exception):
```

### Comparing `stis_cti-1.6.0/stis_cti/unit_tests.py` & `stis_cti-1.6.1/stis_cti/unit_tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python
 
-from nose.tools import assert_equals, assert_false, assert_raises, assert_not_equals
+import pytest
+import sys
 import os
 import copy
 import datetime
 from astropy.io import fits
 
 from .stis_cti import *
 from .archive_dark_query import archive_dark_query
@@ -29,15 +30,15 @@
     hdu.header['DETECTOR'] = ('CCD',           'detector in use: NUV-MAMA, FUV-MAMA, or CCD')
     hdu.header['CCDAMP']   = ('D',             'CCD amplifier read out (A,B,C,D)')
     hdu.header['CCDGAIN']  = (1,               'commanded gain of CCD')
     hdu.header['CCDOFFST'] = (3,               'commanded CCD bias offset')
     hdu.header['BINAXIS1'] = (1,               'axis1 data bin size in unbinned detector pixels')
     hdu.header['BINAXIS2'] = (1,               'axis2 data bin size in unbinned detector pixels')
     
-    hdu.writeto(test_file, output_verify='exception', clobber=True)
+    hdu.writeto(test_file, output_verify='exception', overwrite=True)
 
 
 def write_pctetab(pctetab):
     if not os.access(os.path.curdir, os.W_OK):
         raise Exception('Can\'t write test PCTETAB file to CWD!')
     
     hdu = fits.PrimaryHDU()
@@ -54,15 +55,15 @@
     hdu.header['SIM_NIT']  = (7, 'number of readout simulations done per column')
     hdu.header['SHFT_NIT'] = (4, 'the number of shifts each column readout simula')
     hdu.header['RN_CLIP']  = (5.6, 'Read noise level in electrons.')
     hdu.header['NSEMODEL'] = (1, 'Read noise smoothing algorithm.')
     hdu.header['SUBTHRSH'] = (-30.0, 'Over-subtraction correction threshold.')
     hdu.header['PCTE_VER'] = ('0.1_alpha', 'Version of PCTETAB')
     
-    hdu.writeto(pctetab, output_verify='exception', clobber=True)
+    hdu.writeto(pctetab, output_verify='exception', overwrite=True)
 
 
 def write_superdark(superdark):
     if not os.access(os.path.curdir, os.W_OK):
         raise Exception('Can\'t write test superdark file to CWD!')
     
     hdu = fits.PrimaryHDU()
@@ -95,403 +96,407 @@
     hdu.header['HISTORY'] = 'The following input files were used:'
     hdu.header['HISTORY'] = 'abc_cte.fits'
     hdu.header['HISTORY'] = 'def_cte.fits'
     hdu.header['HISTORY'] = 'hij_cte.fits'
     hdu.header['HISTORY'] = ''
     hdu.header['HISTORY'] = 'blah2, blah2, blah2'
     
-    hdu.writeto(superdark, output_verify='exception', clobber=True)
+    hdu.writeto(superdark, output_verify='exception', overwrite=True)
 
 
 # ----------------------------------------------------------------------------------------
 # Here are the unit tests:
 
 class TestPaths(object):
-    '''
-    Tests functionality of stis_cti.resolve_iraf_file
+    '''Tests functionality of stis_cti.resolve_iraf_file
     '''
     @classmethod
     def setup_class(cls):
         os.environ['toref'] = '/grp/hst/cdbs/oref/'
         # Undefine undoref if it exists:
         if 'undoref' in os.environ:
             os.environ.pop('undoref')
     
     @classmethod
     def teardown_class(cls):
         os.environ.pop('toref')
     
     def test_no_dollar(self):
-        assert_equals(resolve_iraf_file('filename.fits'), 'filename.fits')
-        assert_equals(resolve_iraf_file('/dir/filename.fits'), '/dir/filename.fits')
-        assert_equals(resolve_iraf_file('dir/filename.fits'), 'dir/filename.fits')
+        assert resolve_iraf_file('filename.fits') == 'filename.fits'
+        assert resolve_iraf_file('/dir/filename.fits') == '/dir/filename.fits'
+        assert resolve_iraf_file('dir/filename.fits') == 'dir/filename.fits'
     
     def test_dollar_at_beginning(self):
-        assert_equals(resolve_iraf_file('$toref/filename.fits'), '/grp/hst/cdbs/oref/filename.fits')
-        assert_equals(resolve_iraf_file('$toref/path/filename.fits'), '/grp/hst/cdbs/oref/path/filename.fits')
+        assert resolve_iraf_file('$toref/filename.fits') == '/grp/hst/cdbs/oref/filename.fits'
+        assert resolve_iraf_file('$toref/path/filename.fits') == '/grp/hst/cdbs/oref/path/filename.fits'
     
     def test_dollar_in_middle(self):
-        assert_equals(resolve_iraf_file('toref$filename.fits'), '/grp/hst/cdbs/oref/filename.fits')
-        assert_equals(resolve_iraf_file('toref$path/filename.fits'), '/grp/hst/cdbs/oref/path/filename.fits')
+        assert resolve_iraf_file('toref$filename.fits') == '/grp/hst/cdbs/oref/filename.fits'
+        assert resolve_iraf_file('toref$path/filename.fits') == '/grp/hst/cdbs/oref/path/filename.fits'
     
     def test_environ_var_undefined(self):
-        with assert_raises(IOError) as cm:
+        with pytest.raises(IOError) as cm:
             resolve_iraf_file('undoref$filename.fits')
-        ex = cm.exception
-        assert_equals(ex.message, "Can't resolve environmental variable 'undoref'.")
+        assert str(cm.value) == "Can\'t resolve environmental variable \'undoref\'."
 
 
 class TestFileFiltering(object):
+    '''Tests functionality of stis_cti.viable_ccd_file
     '''
-    Tests functionality of stis_cti.viable_ccd_file
-    '''
-    test_file = 'testfits_2334134234_raw.fits'
+    @classmethod
+    def setup_class(cls):
+        cls.test_file = 'testfits_2334134234_raw.fits'
     
-    def setup(self):
+    def setup_method(self, method):
         write_file(self.test_file)
-    
-    def teardown(self):
+
+    def teardown_method(self, method):
         os.remove(self.test_file)
-    
+
     def test_viable_file(self):
         assert viable_ccd_file(self.test_file)
     
     def test_viable_file_lenient(self):
         assert viable_ccd_file(self.test_file, \
             earliest_date_allowed = datetime.datetime(1990,1,1,0,0,0), \
             amplifiers_allowed = ['A','B','C','D'], \
             gains_allowed = [1,2,4,8], \
             offsts_allowed = list(range(9)))
     
     def test_acq_file_reject(self):
         fits.setval(self.test_file, 'OBSMODE', value='ACQ')
-        assert_false(viable_ccd_file(self.test_file))
+        assert not viable_ccd_file(self.test_file)
     
     def test_gain3_file_reject(self):
         fits.setval(self.test_file, 'CCDGAIN', value=3)
-        assert_false(viable_ccd_file(self.test_file))
+        assert not viable_ccd_file(self.test_file)
     
     def test_gain4_file(self):
         fits.setval(self.test_file, 'CCDGAIN', value=4)
         assert viable_ccd_file(self.test_file)
 
     def test_pre_sm4_reject(self):
         fits.setval(self.test_file, 'TDATEOBS', value='1990-01-01')
-        assert_false(viable_ccd_file(self.test_file))
+        assert not viable_ccd_file(self.test_file)
 
     def test_binned_data_reject1(self):
         fits.setval(self.test_file, 'BINAXIS1', value=2)
-        assert_false(viable_ccd_file(self.test_file))
+        assert not viable_ccd_file(self.test_file)
     
     def test_binned_data_reject2(self):
         fits.setval(self.test_file, 'BINAXIS2', value=2)
-        assert_false(viable_ccd_file(self.test_file))
+        assert not viable_ccd_file(self.test_file)
     
     def test_subarray_reject(self):
         fits.setval(self.test_file, 'SUBARRAY', value=True)
-        assert_false(viable_ccd_file(self.test_file))
+        assert not viable_ccd_file(self.test_file)
 
 
 class Test_determine_input_science(object):
+    '''Tests functionality of stis_cti.determine_input_science
     '''
-    Tests functionality of stis_cti.determine_input_science
-    '''
-    test_dir   = 'dir_2334134234'
-    test_file  = os.path.join(test_dir, 'testfits_001_raw.fits')
-    test_file2 = os.path.join(test_dir, 'testfits_002_raw.fits')
-    
-    def setup(self):
+    @classmethod
+    def setup_class(cls):
+        cls.test_dir   = 'dir_2334134234'
+        cls.test_file  = os.path.join(cls.test_dir, 'testfits_001_raw.fits')
+        cls.test_file2 = os.path.join(cls.test_dir, 'testfits_002_raw.fits')
+
         if not os.access(os.path.curdir, os.W_OK):
             raise Exception('Can\'t write test dir and file to CWD!')
-        
+
+    def setup_method(self, method):
         # Setup directory structure:
         if os.path.exists(self.test_file):
             os.remove(self.test_file)
         if os.path.exists(self.test_file2):
             os.remove(self.test_file2)
         if os.path.exists(self.test_dir):
             os.rmdir(self.test_dir)
         os.mkdir(self.test_dir)
-        
+
         # Write FITS file:
         write_file(self.test_file)
-    
-    def teardown(self):
+
+    def teardown_method(self, method):
         os.remove(self.test_file)
         if os.path.exists(self.test_file2):
             os.remove(self.test_file2)
         os.rmdir(self.test_dir)
-    
+
     def test_file_written(self):
         assert os.path.exists(self.test_file)
     
     def test_filter_pass(self):
-        assert_equals(determine_input_science(self.test_dir, False, False), [self.test_file])
+        assert determine_input_science(self.test_dir, False, False) == [self.test_file]
     
     def test_filter_date_reject(self):
         fits.setval(self.test_file, 'TDATEOBS', value='1992-01-01')
-        assert_raises(FileError, determine_input_science, self.test_dir, False, False)
+        with pytest.raises(FileError):
+            determine_input_science(self.test_dir, False, False)
     
     def test_filter_date_allow_pass(self):
         fits.setval(self.test_file, 'TDATEOBS', value='1992-01-01')
         assert determine_input_science(self.test_dir, True, False)
     
     def test_filter_date_partial_reject(self):
         write_file(self.test_file2)
         fits.setval(self.test_file2, 'TDATEOBS', value='1992-01-01')
-        assert_equals(determine_input_science(self.test_dir, False, False), [self.test_file])
+        assert determine_input_science(self.test_dir, False, False) == [self.test_file]
 
 
 class Test_check_pctetab_version(object):
+    '''Tests functionality of stis_cti.check_pctetab_version
     '''
-    Tests functionality of stis_cti.check_pctetab_version
-    '''
-    pctetab = 'a00_stis_000test37155_pcte.fits'
-    
-    def setup(self):
+    @classmethod
+    def setup_class(cls):
+        cls.pctetab = 'a00_stis_000test37155_pcte.fits'
+
+    def setup_method(self, method):
         write_pctetab(self.pctetab)
-    
-    def teardown(self):
+
+    def teardown_method(self, method):
         os.remove(self.pctetab)
-     
+
     def test_pctetab_ver_pass(self):
         assert check_pctetab_version(self.pctetab, False, '0.1', '1.999')
-    
+
     def test_pctetab_ver_reject(self):
-        assert_raises(VersionError, check_pctetab_version, self.pctetab, False, '1.0', '1.999')
-    
+        with pytest.raises(VersionError):
+            check_pctetab_version(self.pctetab, False, '1.0', '1.999')
+
     def test_pctetab_ver_file_reject(self):
         fits.setval(self.pctetab, 'PCTE_VER', value='3.0_beta')
-        assert_raises(VersionError, check_pctetab_version, self.pctetab, False, '0.1', '1.999')
+        with pytest.raises(VersionError):
+            check_pctetab_version(self.pctetab, False, '0.1', '1.999')
 
 
 class Test_superdark_hash(object):
+    '''Tests functionality of stis_cti.superdark_hash
     '''
-    Tests functionality of stis_cti.superdark_hash
-    '''
-    pctetab = 'a00_stis_000test37166_pcte.fits'
-    superdark = 'd001_testfile57254_drk.fits'
-    
-    def setup(self):
+    @classmethod
+    def setup_class(cls):
+        cls.pctetab = 'a00_stis_000test37166_pcte.fits'
+        cls.superdark = 'd001_testfile57254_drk.fits'
+
+    def setup_method(self, method):
         write_superdark(self.superdark)
         write_pctetab(self.pctetab)
-    
-    def teardown(self):
+
+    def teardown_method(self, method):
         os.remove(self.superdark)
         os.remove(self.pctetab)
-    
+
     def test_manual_inputs_pass(self):
-        assert_equals(
+        assert \
             superdark_hash(sim_nit=7, shft_nit=4, rn_clip=5.6, nsemodel=1, subthrsh=-30.0, 
-                           pcte_ver='0.1_alpha', files=[]), 
-            superdark_hash(pctetab=self.pctetab, files=[]))
-    
+                           pcte_ver='0.1_alpha', files=[]) == \
+            superdark_hash(pctetab=self.pctetab, files=[])
+
     def test_manual_inputs2_pass(self):
        # superdark_hash should ignore text after '_' in pcte_ver
-        assert_equals(
+        assert \
             superdark_hash(sim_nit=7, shft_nit=4, rn_clip=5.6, nsemodel=1, subthrsh=-30.0, 
-                           pcte_ver='0.1_beta', files=[]), 
-            superdark_hash(pctetab=self.pctetab, files=[]))
-    
+                           pcte_ver='0.1_beta', files=[]) == \
+            superdark_hash(pctetab=self.pctetab, files=[])
+
     def test_manual_inputs3_pass(self):
         # try with a file list specified
-        assert_equals(
+        assert \
             superdark_hash(sim_nit=7, shft_nit=4, rn_clip=5.6, nsemodel=1, subthrsh=-30.0, 
-                           pcte_ver='0.1_alpha', files=['abc_cte.fits', 'def_cte.fits', 'hij_cte.fits']), 
-            superdark_hash(pctetab=self.pctetab, files=['abc_cte.fits', 'def_cte.fits', 'hij_cte.fits']))
-    
+                           pcte_ver='0.1_alpha', files=['abc_cte.fits', 'def_cte.fits', 'hij_cte.fits']) == \
+            superdark_hash(pctetab=self.pctetab, files=['abc_cte.fits', 'def_cte.fits', 'hij_cte.fits'])
+
     def test_manual_inputs4_pass(self):
-        assert_equals(
+        assert \
             superdark_hash(sim_nit=7, shft_nit=4, rn_clip=5.6, nsemodel=1, subthrsh=-30.0, 
-                           pcte_ver='0.1_alpha', files=['abc_cte.fits', 'def_cte.fits', 'hij_cte.fits']), 
-            superdark_hash(superdark=self.superdark))
-    
+                           pcte_ver='0.1_alpha', files=['abc_cte.fits', 'def_cte.fits', 'hij_cte.fits']) == \
+            superdark_hash(superdark=self.superdark)
+
     def test_manual_inputs_reject(self):
         # changed file list
-        assert_not_equals(
+        assert \
             superdark_hash(sim_nit=7, shft_nit=4, rn_clip=5.6, nsemodel=1, subthrsh=-30.0, 
-                           pcte_ver='0.1_alpha', files=[]), 
-            superdark_hash(pctetab=self.pctetab, files=['otherfile_cte.fits']))
-    
+                           pcte_ver='0.1_alpha', files=[]) != \
+            superdark_hash(pctetab=self.pctetab, files=['otherfile_cte.fits'])
+
     def test_manual_inputs2_reject(self):
         # changed sim_nit
-        assert_not_equals(
+        assert \
             superdark_hash(sim_nit=70, shft_nit=4, rn_clip=5.6, nsemodel=1, subthrsh=-30.0, 
-                           pcte_ver='0.1_alpha', files=[]), 
-            superdark_hash(pctetab=self.pctetab, files=[]))
-    
+                           pcte_ver='0.1_alpha', files=[]) != \
+            superdark_hash(pctetab=self.pctetab, files=[])
+
     def test_manual_inputs3_reject(self):
         # changed pcte_ver
-        assert_not_equals(
+        assert \
             superdark_hash(sim_nit=7, shft_nit=4, rn_clip=5.6, nsemodel=1, subthrsh=-30.0, 
-                           pcte_ver='0.2_alpha', files=[]), 
-            superdark_hash(pctetab=self.pctetab, files=[]))
-    
+                           pcte_ver='0.2_alpha', files=[]) != \
+            superdark_hash(pctetab=self.pctetab, files=[])
+
     def test_superdark_pass(self):
-        assert_equals(
-            superdark_hash(superdark=self.superdark, files=[]), 
-            superdark_hash(pctetab=self.pctetab, files=[]))
-    
+        assert \
+            superdark_hash(superdark=self.superdark, files=[]) == \
+            superdark_hash(pctetab=self.pctetab, files=[])
+
     def test_superdark2_pass(self):
-        assert_equals(
-            superdark_hash(superdark=self.superdark), 
-            superdark_hash(pctetab=self.pctetab, files=['abc_cte.fits', 'def_cte.fits', 'hij_cte.fits']))
-    
+        assert \
+            superdark_hash(superdark=self.superdark) == \
+            superdark_hash(pctetab=self.pctetab, files=['abc_cte.fits', 'def_cte.fits', 'hij_cte.fits'])
+
     def test_superdark3_pass(self):
         fits.setval(self.superdark, 'PCTE_VER', value='0.1_gamma')
-        assert_equals(
-            superdark_hash(superdark=self.superdark), 
-            superdark_hash(pctetab=self.pctetab, files=['abc_cte.fits', 'def_cte.fits', 'hij_cte.fits']))
-    
+        assert \
+            superdark_hash(superdark=self.superdark) == \
+            superdark_hash(pctetab=self.pctetab, files=['abc_cte.fits', 'def_cte.fits', 'hij_cte.fits'])
+
     def test_superdark_reject(self):
-        assert_not_equals(
-            superdark_hash(superdark=self.superdark), 
-            superdark_hash(pctetab=self.pctetab, files=[]))
-    
+        assert \
+            superdark_hash(superdark=self.superdark) != \
+            superdark_hash(pctetab=self.pctetab, files=[])
+
     def test_superdark2_reject(self):
         fits.setval(self.superdark, 'PCTENSMD', value=5)
-        assert_not_equals(
-            superdark_hash(superdark=self.superdark), 
-            superdark_hash(pctetab=self.pctetab, files=['abc_cte.fits', 'def_cte.fits', 'hij_cte.fits']))
-    
+        assert \
+            superdark_hash(superdark=self.superdark) != \
+            superdark_hash(pctetab=self.pctetab, files=['abc_cte.fits', 'def_cte.fits', 'hij_cte.fits'])
+
     def test_superdark3_reject(self):
         fits.setval(self.pctetab, 'nsemodel', value=6)
-        assert_not_equals(
-            superdark_hash(superdark=self.superdark), 
-            superdark_hash(pctetab=self.pctetab, files=['abc_cte.fits', 'def_cte.fits', 'hij_cte.fits']))
-    
+        assert \
+            superdark_hash(superdark=self.superdark) != \
+            superdark_hash(pctetab=self.pctetab, files=['abc_cte.fits', 'def_cte.fits', 'hij_cte.fits'])
+
     def test_superdark4_reject(self):
         fits.setval(self.superdark, 'PCTE_VER', value='0.2_alpha')
-        assert_not_equals(
-            superdark_hash(superdark=self.superdark), 
-            superdark_hash(pctetab=self.pctetab, files=['abc_cte.fits', 'def_cte.fits', 'hij_cte.fits']))
-    
+        assert \
+            superdark_hash(superdark=self.superdark) != \
+            superdark_hash(pctetab=self.pctetab, files=['abc_cte.fits', 'def_cte.fits', 'hij_cte.fits'])
+
     def test_superdark4_reject(self):
         fits.setval(self.pctetab, 'PCTE_VER', value='0.2_alpha')
-        assert_not_equals(
-            superdark_hash(superdark=self.superdark), 
-            superdark_hash(pctetab=self.pctetab, files=['abc_cte.fits', 'def_cte.fits', 'hij_cte.fits']))
-    
+        assert \
+            superdark_hash(superdark=self.superdark) != \
+            superdark_hash(pctetab=self.pctetab, files=['abc_cte.fits', 'def_cte.fits', 'hij_cte.fits'])
+
 
 class Test_archive_dark_query(object):
+    '''Tests functionality of stis_cti.archive_dark_query
     '''
-    Tests functionality of stis_cti.archive_dark_query
-    '''
-    test_file = 'testfits_2334134667_raw.fits'
-    
     @classmethod
     def setup_class(cls):
+        cls.test_file = 'testfits_2334134667_raw.fits'
         write_file(cls.test_file)
         cls.anneal = archive_dark_query([cls.test_file], None, None, False, False)
     
     @classmethod
     def teardown_class(cls):
         os.remove(cls.test_file)
     
     def test_number_of_anneals(self):
-        assert_equals(len(self.anneal), 1)
+        assert len(self.anneal) == 1
     
     def test_anneal_index(self):
-        assert_equals(self.anneal[0]['index'], 133)
+        assert self.anneal[0]['index'] == 133
     
     def test_anneal_darks(self):
         darks = [d['exposure'] for d in self.anneal[0]['darks']]
-        assert_equals(set(darks), \
+        assert set(darks) == \
             set(['OBVM3XH9Q', 'OBVM3YHHQ', 'OBVM3ZN5Q', 'OBVM40NCQ', 'OBVM41T2Q', 'OBVM42TFQ', 
                  'OBVM43YEQ', 'OBVM44YOQ', 'OBVM45FQQ', 'OBVM46G7Q', 'OBVM47LNQ', 'OBVM48MCQ', 
                  'OBVM49ANQ', 'OBVM4AAVQ', 'OBVM4BH5Q', 'OBVM4CHJQ', 'OBVM4DLRQ', 'OBVM4EM2Q', 
                  'OBVM4FRJQ', 'OBVM4GRQQ', 'OBVM4HYVQ', 'OBVM4IZ5Q', 'OBVM4JG4Q', 'OBVM4KGCQ', 
                  'OBVM4LO1S', 'OBVM4MOIS', 'OBVM4NABQ', 'OBVM4OAMQ', 'OBVM4PI2Q', 'OBVM4QIAQ', 
                  'OBVM4RPDQ', 'OBVM4SPJQ', 'OBVM4TW9Q', 'OBVM4UWDQ', 'OBVM4VCOQ', 'OBVM4WCXQ', 
                  'OBVM4XJ6Q', 'OBVM4YJCQ', 'OBVM4ZOMQ', 'OBVM50POQ', 'OBVM51A4Q', 'OBVM52ABQ', 
                  'OBVM53FIQ', 'OBVM54FNQ', 'OBVM55LTQ', 'OBVM56M5Q', 'OBVM57T3S', 'OBVM58T8S', 
                  'OBVM59W6S', 'OBVM5AWDS', 'OBVM5BBQQ', 'OBVM5CBUQ', 'OBVM5DG7Q', 'OBVM5EGBQ', 
-                 'OBVM5FALQ', 'OBVM5GAUQ', 'OBVM5HFTQ', 'OBVM5IFPQ', 'OBVM5JKLQ', 'OBVM5KLPQ']))
+                 'OBVM5FALQ', 'OBVM5GAUQ', 'OBVM5HFTQ', 'OBVM5IFPQ', 'OBVM5JKLQ', 'OBVM5KLPQ'])
     
     def test_undefined_fits_file(self):
         undefined_filename = 'testfits_undefined_28739723_raw.fits'
-        assert_raises(IOError, archive_dark_query, [undefined_filename], None, None, False, False)
+        with pytest.raises(IOError):
+            archive_dark_query([undefined_filename], None, None, False, False)
 
 
 class Test_check_for_old_output_files(object):
+    '''Tests functionality of stis_cti.check_for_old_output_files
     '''
-    Tests functionality of stis_cti.check_for_old_output_files
-    '''
-    test_dir = 'dir_8364834236'
-    rootname = 'testfits67733'
-    
-    test_files_leave  = [rootname + '_raw.fits', rootname + '_flt.fits']
-    test_files_remove = [rootname + '_s2c.fits', rootname + '_flc.fits',
-                         rootname + '_blt.fits', rootname + '_cte_flt.fits']
-    # Prepend these files with test_dir:
-    test_files_leave  = [os.path.join(test_dir, f) for f in test_files_leave]
-    test_files_remove = [os.path.join(test_dir, f) for f in test_files_remove]
-    
-    # Combine both of these arrays into one:
-    test_files = copy.deepcopy(test_files_leave)
-    test_files.extend(test_files_remove)
-    
-    output_mapping = {
-        'cte_flt.fits' : 'flc.fits' ,
-        'cte_crj.fits' : 'crc.fits' ,
-        'cte_sx2.fits' : 's2c.fits' ,
-        'cte_x2d.fits' : 'x2c.fits' ,
-        'cte_sx1.fits' : 's1c.fits' ,
-        'cte_x1d.fits' : 'x1c.fits' ,
-        'blt_tra.txt'  : 'trb.txt'  ,
-        'cte_tra.txt'  : 'trc.txt'  ,
-        'blt.fits'     : '<pass>'   ,
-        'cte.fits'     : '<pass>'   }
+    @classmethod
+    def setup_class(cls):
+        cls.test_dir = 'dir_8364834236'
+        cls.rootname = 'testfits67733'
+
+        cls.test_files_leave  = [cls.rootname + '_raw.fits', cls.rootname + '_flt.fits']
+        cls.test_files_remove = [cls.rootname + '_s2c.fits', cls.rootname + '_flc.fits',
+                                 cls.rootname + '_blt.fits', cls.rootname + '_cte_flt.fits']
+        # Prepend these files with test_dir:
+        cls.test_files_leave  = [os.path.join(cls.test_dir, f) for f in cls.test_files_leave]
+        cls.test_files_remove = [os.path.join(cls.test_dir, f) for f in cls.test_files_remove]
+
+        # Combine both of these arrays into one:
+        cls.test_files = copy.deepcopy(cls.test_files_leave)
+        cls.test_files.extend(cls.test_files_remove)
+
+        cls.output_mapping = {
+            'cte_flt.fits' : 'flc.fits' ,
+            'cte_crj.fits' : 'crc.fits' ,
+            'cte_sx2.fits' : 's2c.fits' ,
+            'cte_x2d.fits' : 'x2c.fits' ,
+            'cte_sx1.fits' : 's1c.fits' ,
+            'cte_x1d.fits' : 'x1c.fits' ,
+            'blt_tra.txt'  : 'trb.txt'  ,
+            'cte_tra.txt'  : 'trc.txt'  ,
+            'blt.fits'     : '<pass>'   ,
+            'cte.fits'     : '<pass>'   }
     
-    def setup(self):
-        if os.path.exists(self.test_dir):
+        if os.path.exists(cls.test_dir):
             raise IOError('test_dir already exists: {}'.format(self.test_dir))
         else:
-            os.mkdir(self.test_dir)
-    
-    def teardown(self):
-        for file in self.test_files:
+            os.mkdir(cls.test_dir)
+
+    @classmethod
+    def teardown_class(cls):
+        for file in cls.test_files:
             if os.path.exists(file):
                 os.remove(file)
-        os.rmdir(self.test_dir)
-    
+        os.rmdir(cls.test_dir)
+
     def test_only_good_files(self):
         for file in self.test_files_leave:
             write_file(file)
         assert check_for_old_output_files([self.rootname], self.test_dir, 
             self.output_mapping, False, False)
-    
+
     def test_files_already_exist_exception(self):
         for file in self.test_files:
             write_file(file)
-        assert_raises(IOError, check_for_old_output_files, [self.rootname], self.test_dir, 
-            self.output_mapping, False, False)
-    
+        with pytest.raises(IOError):
+            check_for_old_output_files([self.rootname], self.test_dir, self.output_mapping, False, False)
+
     def test_files_already_exist_exception_none_left(self):
         for file in self.test_files_remove:
             write_file(file)
-        assert_raises(IOError, check_for_old_output_files, [self.rootname], self.test_dir, 
-            self.output_mapping, False, False)
-    
+        with pytest.raises(IOError):
+            check_for_old_output_files([self.rootname], self.test_dir, self.output_mapping, False, False)
+
     def test_files_already_exist_clean(self):
         for file in self.test_files:
             write_file(file)
         assert check_for_old_output_files([self.rootname], self.test_dir, 
             self.output_mapping, True, False)
-    
+
     def test_only_good_files_clean(self):
         for file in self.test_files_leave:
             write_file(file)
         assert check_for_old_output_files([self.rootname], self.test_dir, 
             self.output_mapping, True, False)
-    
+
     def test_only_bad_files_clean(self):
         for file in self.test_files_remove:
             write_file(file)
         assert check_for_old_output_files([self.rootname], self.test_dir, 
             self.output_mapping, True, False)
 
 
 # ----------------------------------------------------------------------------------------
 if __name__ == '__main__':
-    import nose
-    nose.runmodule(argv=['nose', '--verbosity=2'])
+    sys.exit(pytest.main())
```

### Comparing `stis_cti-1.6.0/stis_cti.egg-info/PKG-INFO` & `stis_cti-1.6.1/stis_cti.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: stis-cti
-Version: 1.6.0
+Name: stis_cti
+Version: 1.6.1
 Summary: Pixel-based CTI-correction for HST/STIS CCD data
 Home-page: https://www.stsci.edu/hst/instrumentation/stis/data-analysis-and-software-tools/pixel-based-cti
 Author: Sean Lockwood, Phil Hodge, Pey Lian Lim, W.J. Hack, J. Anderson, Matt Davis
 Author-email: lockwood@stsci.edu
 Maintainer: Sean Lockwood
 Maintainer-email: lockwood@stsci.edu
 License: BSD-new
@@ -20,14 +20,22 @@
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE.txt
+Requires-Dist: setuptools
+Requires-Dist: numpy
+Requires-Dist: astropy>=4.0
+Requires-Dist: stistools>=1.2
+Requires-Dist: refstis>=0.8.1
+Requires-Dist: crds
+Requires-Dist: stsci.tools>=3.2.2
+Requires-Dist: six
 
 HST/STIS Pixel-Based CTI-Correction Scripts
 ===========================================
 
 Utilities needed to correct for Charge Transfer Inefficiency (CTI) in the Hubble
 Space Telescope (HST) STIS CCD.
```

### Comparing `stis_cti-1.6.0/stis_cti.egg-info/SOURCES.txt` & `stis_cti-1.6.1/stis_cti.egg-info/SOURCES.txt`

 * *Files identical despite different names*

