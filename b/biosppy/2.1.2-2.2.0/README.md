# Comparing `tmp/biosppy-2.1.2.tar.gz` & `tmp/biosppy-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biosppy-2.1.2.tar", last modified: Wed Jan 24 17:41:18 2024, max compression
+gzip compressed data, was "biosppy-2.2.0.tar", last modified: Tue Apr 16 14:31:27 2024, max compression
```

## Comparing `biosppy-2.1.2.tar` & `biosppy-2.2.0.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 17:41:18.537273 biosppy-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-01-24 17:41:08.000000 biosppy-2.1.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-01-24 17:41:08.000000 biosppy-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-24 17:41:08.000000 biosppy-2.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-01-24 17:41:18.537273 biosppy-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-01-24 17:41:08.000000 biosppy-2.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 17:41:18.529273 biosppy-2.1.2/biosppy/
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-01-24 17:41:08.000000 biosppy-2.1.2/biosppy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-01-24 17:41:08.000000 biosppy-2.1.2/biosppy/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    63249 2024-01-24 17:41:08.000000 biosppy-2.1.2/biosppy/biometrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    28599 2024-01-24 17:41:08.000000 biosppy-2.1.2/biosppy/clustering.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 17:41:18.533273 biosppy-2.1.2/biosppy/features/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-01-24 17:41:08.000000 biosppy-2.1.2/biosppy/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-01-24 17:41:08.000000 biosppy-2.1.2/biosppy/features/cepstral.py
--rw-r--r--   0 runner    (1001) docker     (127)     8647 2024-01-24 17:41:08.000000 biosppy-2.1.2/biosppy/features/frequency.py
--rw-r--r--   0 runner    (1001) docker     (127)    10975 2024-01-24 17:41:08.000000 biosppy-2.1.2/biosppy/features/phase_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-01-24 17:41:08.000000 biosppy-2.1.2/biosppy/features/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-01-24 17:41:08.000000 biosppy-2.1.2/biosppy/features/time_freq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 17:41:18.533273 biosppy-2.1.2/biosppy/inter_plotting/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-01-24 17:41:08.000000 biosppy-2.1.2/biosppy/inter_plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17678 2024-01-24 17:41:08.000000 biosppy-2.1.2/biosppy/inter_plotting/acc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-01-24 17:41:08.000000 biosppy-2.1.2/biosppy/inter_plotting/ecg.py
--rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-01-24 17:41:08.000000 biosppy-2.1.2/biosppy/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    70946 2024-01-24 17:41:08.000000 biosppy-2.1.2/biosppy/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6601 2024-01-24 17:41:08.000000 biosppy-2.1.2/biosppy/quality.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 17:41:18.537273 biosppy-2.1.2/biosppy/signals/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-01-24 17:41:08.000000 biosppy-2.1.2/biosppy/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6039 2024-01-24 17:41:08.000000 biosppy-2.1.2/biosppy/signals/abp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-01-24 17:41:08.000000 biosppy-2.1.2/biosppy/signals/acc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-01-24 17:41:08.000000 biosppy-2.1.2/biosppy/signals/bvp.py
--rw-r--r--   0 runner    (1001) docker     (127)    65972 2024-01-24 17:41:08.000000 biosppy-2.1.2/biosppy/signals/ecg.py
--rw-r--r--   0 runner    (1001) docker     (127)    23277 2024-01-24 17:41:08.000000 biosppy-2.1.2/biosppy/signals/eda.py
--rw-r--r--   0 runner    (1001) docker     (127)    12123 2024-01-24 17:41:08.000000 biosppy-2.1.2/biosppy/signals/eeg.py
--rw-r--r--   0 runner    (1001) docker     (127)    41783 2024-01-24 17:41:08.000000 biosppy-2.1.2/biosppy/signals/emg.py
--rw-r--r--   0 runner    (1001) docker     (127)    29473 2024-01-24 17:41:08.000000 biosppy-2.1.2/biosppy/signals/hrv.py
--rw-r--r--   0 runner    (1001) docker     (127)    15722 2024-01-24 17:41:08.000000 biosppy-2.1.2/biosppy/signals/pcg.py
--rw-r--r--   0 runner    (1001) docker     (127)    18044 2024-01-24 17:41:08.000000 biosppy-2.1.2/biosppy/signals/ppg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-01-24 17:41:08.000000 biosppy-2.1.2/biosppy/signals/resp.py
--rw-r--r--   0 runner    (1001) docker     (127)    58583 2024-01-24 17:41:08.000000 biosppy-2.1.2/biosppy/signals/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9686 2024-01-24 17:41:08.000000 biosppy-2.1.2/biosppy/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    25139 2024-01-24 17:41:08.000000 biosppy-2.1.2/biosppy/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 17:41:18.537273 biosppy-2.1.2/biosppy/synthesizers/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-24 17:41:08.000000 biosppy-2.1.2/biosppy/synthesizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20102 2024-01-24 17:41:08.000000 biosppy-2.1.2/biosppy/synthesizers/ecg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-01-24 17:41:08.000000 biosppy-2.1.2/biosppy/timing.py
--rw-r--r--   0 runner    (1001) docker     (127)    13487 2024-01-24 17:41:08.000000 biosppy-2.1.2/biosppy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 17:41:18.537273 biosppy-2.1.2/biosppy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-01-24 17:41:18.000000 biosppy-2.1.2/biosppy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-01-24 17:41:18.000000 biosppy-2.1.2/biosppy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-24 17:41:18.000000 biosppy-2.1.2/biosppy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-01-24 17:41:18.000000 biosppy-2.1.2/biosppy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-24 17:41:18.000000 biosppy-2.1.2/biosppy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-01-24 17:41:18.537273 biosppy-2.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-01-24 17:41:08.000000 biosppy-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:31:27.672315 biosppy-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-16 14:31:24.000000 biosppy-2.2.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-16 14:31:24.000000 biosppy-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-16 14:31:24.000000 biosppy-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-16 14:31:27.672315 biosppy-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-04-16 14:31:24.000000 biosppy-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:31:27.668315 biosppy-2.2.0/biosppy/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63249 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/biometrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28599 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/clustering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:31:27.668315 biosppy-2.2.0/biosppy/features/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/features/cepstral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8647 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/features/frequency.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10986 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/features/phase_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/features/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/features/time_freq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:31:27.668315 biosppy-2.2.0/biosppy/inter_plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/inter_plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17678 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/inter_plotting/acc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/inter_plotting/ecg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72253 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11234 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/quality.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:31:27.672315 biosppy-2.2.0/biosppy/signals/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/signals/abp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8067 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/signals/acc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/signals/bvp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65972 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/signals/ecg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23301 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/signals/eda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12123 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/signals/eeg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41783 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/signals/emg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29473 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/signals/hrv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15722 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/signals/pcg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18044 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/signals/ppg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/signals/resp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58646 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/signals/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9686 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25139 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:31:27.672315 biosppy-2.2.0/biosppy/synthesizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/synthesizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20118 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/synthesizers/ecg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29270 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/synthesizers/emg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13475 2024-04-16 14:31:24.000000 biosppy-2.2.0/biosppy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:31:27.672315 biosppy-2.2.0/biosppy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-16 14:31:27.000000 biosppy-2.2.0/biosppy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-16 14:31:27.000000 biosppy-2.2.0/biosppy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:31:27.000000 biosppy-2.2.0/biosppy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-16 14:31:27.000000 biosppy-2.2.0/biosppy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-16 14:31:27.000000 biosppy-2.2.0/biosppy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-16 14:31:27.672315 biosppy-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-04-16 14:31:24.000000 biosppy-2.2.0/setup.py
```

### Comparing `biosppy-2.1.2/AUTHORS.md` & `biosppy-2.2.0/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `biosppy-2.1.2/LICENSE` & `biosppy-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biosppy-2.1.2/PKG-INFO` & `biosppy-2.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biosppy
-Version: 2.1.2
+Version: 2.2.0
 Summary: A toolbox for biosignal processing written in Python.
 Home-page: https://github.com/scientisst/BioSPPy
 Author: Instituto de Telecomunicacoes
 Author-email: developer@scientisst.com
 License: BSD 3-clause
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -29,44 +29,39 @@
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
 Requires-Dist: shortuuid
 Requires-Dist: six
 Requires-Dist: joblib
 Requires-Dist: opencv-python
 Requires-Dist: pywavelets
+Requires-Dist: mock
 Provides-Extra: eda
 Requires-Dist: cvxopt; extra == "eda"
 
 
+### 🎙️ Announcements
+#### Latest
 ```
 🌀 New module for signal quality assessment 🌀
-With the signals.quality module you can now evaluate the quality of your signals!
+With the biosppy.quality module you can now evaluate the quality of your signals!
 So far, the EDA and ECG quality are available, but more could be added soon. 
 ```
-
-```
-🫀 New module for heart rate variability 🫀
-With the signals.hrv module you can now extract HRV features. Check it out! (PR #19)
-```
-```
-✨ New plotting design ✨
-New colors, new style and new features, check it out!
-```
+#### New features
 ```
-🎊 New module for feature extraction 🎊
-With the 'features' module you can easily extract features from your biosignals!
-(Check PR #4)
+🌀 New module for signal quality assessment (biosppy.quality)
+🫀 New module for heart rate variability (biosppy.signals.hrv)
+🎊 New module for feature extraction (biosppy.features)
 ```
 
 
 # BioSPPy - Biosignal Processing in Python
 
 *A toolbox for biosignal processing written in Python.*
 
-<a href="http://biosppy.readthedocs.org/">
+<a href="https://biosppy.readthedocs.org/">
 <picture>
   <source media="(prefers-color-scheme: light)" srcset="docs/logo/logo_400.png">
   <source media="(prefers-color-scheme: dark)" srcset="docs/logo/logo_inverted_400.png">
   <img alt="Image" title="I know you're listening! - xkcd.com/525">
 </picture>
 </a>
 
@@ -76,15 +71,15 @@
 Highlights:
 
 - Support for various biosignals: BVP, ECG, EDA, EEG, EMG, PCG, PPG, Respiration
 - Signal analysis primitives: filtering, frequency analysis
 - Clustering
 - Biometrics
 
-Documentation can be found at: <http://biosppy.readthedocs.org/>
+Documentation can be found at: <https://biosppy.readthedocs.org/>
 
 ## Installation
 
 Installation can be easily done with `pip`:
 
 ```bash
 $ pip install biosppy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: biosppy Version: 2.1.2 Summary: A toolbox for
+Metadata-Version: 2.1 Name: biosppy Version: 2.2.0 Summary: A toolbox for
 biosignal processing written in Python. Home-page: https://github.com/
 scientisst/BioSPPy Author: Instituto de Telecomunicacoes Author-email:
 developer@scientisst.com License: BSD 3-clause Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: BSD License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
@@ -10,29 +10,28 @@
 Python :: 3.6 Classifier: Programming Language :: Python :: Implementation ::
 CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent Requires-Python: >3.5.2
 Description-Content-Type: text/markdown License-File: LICENSE License-File:
 AUTHORS.md Requires-Dist: bidict Requires-Dist: h5py Requires-Dist: matplotlib
 Requires-Dist: numpy Requires-Dist: scikit-learn Requires-Dist: scipy Requires-
 Dist: shortuuid Requires-Dist: six Requires-Dist: joblib Requires-Dist: opencv-
-python Requires-Dist: pywavelets Provides-Extra: eda Requires-Dist: cvxopt;
-extra == "eda" ``` ð New module for signal quality assessment ð With the
-signals.quality module you can now evaluate the quality of your signals! So
-far, the EDA and ECG quality are available, but more could be added soon. ```
-``` ð« New module for heart rate variability ð« With the signals.hrv module
-you can now extract HRV features. Check it out! (PR #19) ``` ``` â¨ New
-plotting design â¨ New colors, new style and new features, check it out! ```
-``` ð New module for feature extraction ð With the 'features' module you
-can easily extract features from your biosignals! (Check PR #4) ``` # BioSPPy -
-Biosignal Processing in Python *A toolbox for biosignal processing written in
-Python.* _[_I_m_a_g_e_]The toolbox bundles together various signal processing and
-pattern recognition methods geared towards the analysis of biosignals.
-Highlights: - Support for various biosignals: BVP, ECG, EDA, EEG, EMG, PCG,
-PPG, Respiration - Signal analysis primitives: filtering, frequency analysis -
-Clustering - Biometrics Documentation can be found at:
+python Requires-Dist: pywavelets Requires-Dist: mock Provides-Extra: eda
+Requires-Dist: cvxopt; extra == "eda" ### ðï¸ Announcements #### Latest ```
+ð New module for signal quality assessment ð With the biosppy.quality
+module you can now evaluate the quality of your signals! So far, the EDA and
+ECG quality are available, but more could be added soon. ``` #### New features
+``` ð New module for signal quality assessment (biosppy.quality) ð« New
+module for heart rate variability (biosppy.signals.hrv) ð New module for
+feature extraction (biosppy.features) ``` # BioSPPy - Biosignal Processing in
+Python *A toolbox for biosignal processing written in Python.* _[_I_m_a_g_e_]The
+toolbox bundles together various signal processing and pattern recognition
+methods geared towards the analysis of biosignals. Highlights: - Support for
+various biosignals: BVP, ECG, EDA, EEG, EMG, PCG, PPG, Respiration - Signal
+analysis primitives: filtering, frequency analysis - Clustering - Biometrics
+Documentation can be found at:
 biosppy.readthedocs.org/> ## Installation Installation can be easily done with
 `pip`: ```bash $ pip install biosppy ``` Alternatively, you can install the
 latest version from the GitHub repository: ```bash $ pip install git+https://
 github.com/scientisst/BioSPPy.git ``` ## Simple Example The code below loads an
 ECG signal from the `examples` folder, filters it, performs R-peak detection,
 and computes the instantaneous heart rate. ```python from biosppy import
 storage from biosppy.signals import ecg # load raw ECG signal signal, mdata =
```

### Comparing `biosppy-2.1.2/README.md` & `biosppy-2.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,226 +1,218 @@
-00000000: 6060 600a f09f 8c80 204e 6577 206d 6f64  ```..... New mod
-00000010: 756c 6520 666f 7220 7369 676e 616c 2071  ule for signal q
-00000020: 7561 6c69 7479 2061 7373 6573 736d 656e  uality assessmen
-00000030: 7420 f09f 8c80 0a57 6974 6820 7468 6520  t .....With the 
-00000040: 7369 676e 616c 732e 7175 616c 6974 7920  signals.quality 
-00000050: 6d6f 6475 6c65 2079 6f75 2063 616e 206e  module you can n
-00000060: 6f77 2065 7661 6c75 6174 6520 7468 6520  ow evaluate the 
-00000070: 7175 616c 6974 7920 6f66 2079 6f75 7220  quality of your 
-00000080: 7369 676e 616c 7321 0a53 6f20 6661 722c  signals!.So far,
-00000090: 2074 6865 2045 4441 2061 6e64 2045 4347   the EDA and ECG
-000000a0: 2071 7561 6c69 7479 2061 7265 2061 7661   quality are ava
-000000b0: 696c 6162 6c65 2c20 6275 7420 6d6f 7265  ilable, but more
-000000c0: 2063 6f75 6c64 2062 6520 6164 6465 6420   could be added 
-000000d0: 736f 6f6e 2e20 0a60 6060 0a0a 6060 600a  soon. .```..```.
-000000e0: f09f ab80 204e 6577 206d 6f64 756c 6520  .... New module 
-000000f0: 666f 7220 6865 6172 7420 7261 7465 2076  for heart rate v
-00000100: 6172 6961 6269 6c69 7479 20f0 9fab 800a  ariability .....
-00000110: 5769 7468 2074 6865 2073 6967 6e61 6c73  With the signals
-00000120: 2e68 7276 206d 6f64 756c 6520 796f 7520  .hrv module you 
-00000130: 6361 6e20 6e6f 7720 6578 7472 6163 7420  can now extract 
-00000140: 4852 5620 6665 6174 7572 6573 2e20 4368  HRV features. Ch
-00000150: 6563 6b20 6974 206f 7574 2120 2850 5220  eck it out! (PR 
-00000160: 2331 3929 0a60 6060 0a60 6060 0ae2 9ca8  #19).```.```....
-00000170: 204e 6577 2070 6c6f 7474 696e 6720 6465   New plotting de
-00000180: 7369 676e 20e2 9ca8 0a4e 6577 2063 6f6c  sign ....New col
-00000190: 6f72 732c 206e 6577 2073 7479 6c65 2061  ors, new style a
-000001a0: 6e64 206e 6577 2066 6561 7475 7265 732c  nd new features,
-000001b0: 2063 6865 636b 2069 7420 6f75 7421 0a60   check it out!.`
-000001c0: 6060 0a60 6060 0af0 9f8e 8a20 4e65 7720  ``.```..... New 
-000001d0: 6d6f 6475 6c65 2066 6f72 2066 6561 7475  module for featu
-000001e0: 7265 2065 7874 7261 6374 696f 6e20 f09f  re extraction ..
-000001f0: 8e8a 0a57 6974 6820 7468 6520 2766 6561  ...With the 'fea
-00000200: 7475 7265 7327 206d 6f64 756c 6520 796f  tures' module yo
-00000210: 7520 6361 6e20 6561 7369 6c79 2065 7874  u can easily ext
-00000220: 7261 6374 2066 6561 7475 7265 7320 6672  ract features fr
-00000230: 6f6d 2079 6f75 7220 6269 6f73 6967 6e61  om your biosigna
-00000240: 6c73 210a 2843 6865 636b 2050 5220 2334  ls!.(Check PR #4
-00000250: 290a 6060 600a 0a0a 2320 4269 6f53 5050  ).```...# BioSPP
-00000260: 7920 2d20 4269 6f73 6967 6e61 6c20 5072  y - Biosignal Pr
-00000270: 6f63 6573 7369 6e67 2069 6e20 5079 7468  ocessing in Pyth
-00000280: 6f6e 0a0a 2a41 2074 6f6f 6c62 6f78 2066  on..*A toolbox f
-00000290: 6f72 2062 696f 7369 676e 616c 2070 726f  or biosignal pro
-000002a0: 6365 7373 696e 6720 7772 6974 7465 6e20  cessing written 
-000002b0: 696e 2050 7974 686f 6e2e 2a0a 0a3c 6120  in Python.*..<a 
-000002c0: 6872 6566 3d22 6874 7470 3a2f 2f62 696f  href="http://bio
-000002d0: 7370 7079 2e72 6561 6474 6865 646f 6373  sppy.readthedocs
-000002e0: 2e6f 7267 2f22 3e0a 3c70 6963 7475 7265  .org/">.<picture
-000002f0: 3e0a 2020 3c73 6f75 7263 6520 6d65 6469  >.  <source medi
-00000300: 613d 2228 7072 6566 6572 732d 636f 6c6f  a="(prefers-colo
-00000310: 722d 7363 6865 6d65 3a20 6c69 6768 7429  r-scheme: light)
-00000320: 2220 7372 6373 6574 3d22 646f 6373 2f6c  " srcset="docs/l
-00000330: 6f67 6f2f 6c6f 676f 5f34 3030 2e70 6e67  ogo/logo_400.png
-00000340: 223e 0a20 203c 736f 7572 6365 206d 6564  ">.  <source med
-00000350: 6961 3d22 2870 7265 6665 7273 2d63 6f6c  ia="(prefers-col
-00000360: 6f72 2d73 6368 656d 653a 2064 6172 6b29  or-scheme: dark)
-00000370: 2220 7372 6373 6574 3d22 646f 6373 2f6c  " srcset="docs/l
-00000380: 6f67 6f2f 6c6f 676f 5f69 6e76 6572 7465  ogo/logo_inverte
-00000390: 645f 3430 302e 706e 6722 3e0a 2020 3c69  d_400.png">.  <i
-000003a0: 6d67 2061 6c74 3d22 496d 6167 6522 2074  mg alt="Image" t
-000003b0: 6974 6c65 3d22 4920 6b6e 6f77 2079 6f75  itle="I know you
-000003c0: 2772 6520 6c69 7374 656e 696e 6721 202d  're listening! -
-000003d0: 2078 6b63 642e 636f 6d2f 3532 3522 3e0a   xkcd.com/525">.
-000003e0: 3c2f 7069 6374 7572 653e 0a3c 2f61 3e0a  </picture>.</a>.
-000003f0: 0a54 6865 2074 6f6f 6c62 6f78 2062 756e  .The toolbox bun
-00000400: 646c 6573 2074 6f67 6574 6865 7220 7661  dles together va
-00000410: 7269 6f75 7320 7369 676e 616c 2070 726f  rious signal pro
-00000420: 6365 7373 696e 6720 616e 6420 7061 7474  cessing and patt
-00000430: 6572 6e20 7265 636f 676e 6974 696f 6e0a  ern recognition.
-00000440: 6d65 7468 6f64 7320 6765 6172 6564 2074  methods geared t
-00000450: 6f77 6172 6473 2074 6865 2061 6e61 6c79  owards the analy
-00000460: 7369 7320 6f66 2062 696f 7369 676e 616c  sis of biosignal
-00000470: 732e 0a0a 4869 6768 6c69 6768 7473 3a0a  s...Highlights:.
-00000480: 0a2d 2053 7570 706f 7274 2066 6f72 2076  .- Support for v
-00000490: 6172 696f 7573 2062 696f 7369 676e 616c  arious biosignal
-000004a0: 733a 2042 5650 2c20 4543 472c 2045 4441  s: BVP, ECG, EDA
-000004b0: 2c20 4545 472c 2045 4d47 2c20 5043 472c  , EEG, EMG, PCG,
-000004c0: 2050 5047 2c20 5265 7370 6972 6174 696f   PPG, Respiratio
-000004d0: 6e0a 2d20 5369 676e 616c 2061 6e61 6c79  n.- Signal analy
-000004e0: 7369 7320 7072 696d 6974 6976 6573 3a20  sis primitives: 
-000004f0: 6669 6c74 6572 696e 672c 2066 7265 7175  filtering, frequ
-00000500: 656e 6379 2061 6e61 6c79 7369 730a 2d20  ency analysis.- 
-00000510: 436c 7573 7465 7269 6e67 0a2d 2042 696f  Clustering.- Bio
-00000520: 6d65 7472 6963 730a 0a44 6f63 756d 656e  metrics..Documen
-00000530: 7461 7469 6f6e 2063 616e 2062 6520 666f  tation can be fo
-00000540: 756e 6420 6174 3a20 3c68 7474 703a 2f2f  und at: <http://
-00000550: 6269 6f73 7070 792e 7265 6164 7468 6564  biosppy.readthed
-00000560: 6f63 732e 6f72 672f 3e0a 0a23 2320 496e  ocs.org/>..## In
-00000570: 7374 616c 6c61 7469 6f6e 0a0a 496e 7374  stallation..Inst
-00000580: 616c 6c61 7469 6f6e 2063 616e 2062 6520  allation can be 
-00000590: 6561 7369 6c79 2064 6f6e 6520 7769 7468  easily done with
-000005a0: 2060 7069 7060 3a0a 0a60 6060 6261 7368   `pip`:..```bash
-000005b0: 0a24 2070 6970 2069 6e73 7461 6c6c 2062  .$ pip install b
-000005c0: 696f 7370 7079 0a60 6060 0a0a 416c 7465  iosppy.```..Alte
-000005d0: 726e 6174 6976 656c 792c 2079 6f75 2063  rnatively, you c
-000005e0: 616e 2069 6e73 7461 6c6c 2074 6865 206c  an install the l
-000005f0: 6174 6573 7420 7665 7273 696f 6e20 6672  atest version fr
-00000600: 6f6d 2074 6865 2047 6974 4875 6220 7265  om the GitHub re
-00000610: 706f 7369 746f 7279 3a0a 0a60 6060 6261  pository:..```ba
-00000620: 7368 0a24 2070 6970 2069 6e73 7461 6c6c  sh.$ pip install
-00000630: 2067 6974 2b68 7474 7073 3a2f 2f67 6974   git+https://git
-00000640: 6875 622e 636f 6d2f 7363 6965 6e74 6973  hub.com/scientis
-00000650: 7374 2f42 696f 5350 5079 2e67 6974 0a60  st/BioSPPy.git.`
-00000660: 6060 0a0a 2323 2053 696d 706c 6520 4578  ``..## Simple Ex
-00000670: 616d 706c 650a 0a54 6865 2063 6f64 6520  ample..The code 
-00000680: 6265 6c6f 7720 6c6f 6164 7320 616e 2045  below loads an E
-00000690: 4347 2073 6967 6e61 6c20 6672 6f6d 2074  CG signal from t
-000006a0: 6865 2060 6578 616d 706c 6573 6020 666f  he `examples` fo
-000006b0: 6c64 6572 2c20 6669 6c74 6572 7320 6974  lder, filters it
-000006c0: 2c0a 7065 7266 6f72 6d73 2052 2d70 6561  ,.performs R-pea
-000006d0: 6b20 6465 7465 6374 696f 6e2c 2061 6e64  k detection, and
-000006e0: 2063 6f6d 7075 7465 7320 7468 6520 696e   computes the in
-000006f0: 7374 616e 7461 6e65 6f75 7320 6865 6172  stantaneous hear
-00000700: 7420 7261 7465 2e0a 0a60 6060 7079 7468  t rate...```pyth
-00000710: 6f6e 0a66 726f 6d20 6269 6f73 7070 7920  on.from biosppy 
-00000720: 696d 706f 7274 2073 746f 7261 6765 0a66  import storage.f
-00000730: 726f 6d20 6269 6f73 7070 792e 7369 676e  rom biosppy.sign
-00000740: 616c 7320 696d 706f 7274 2065 6367 0a0a  als import ecg..
-00000750: 2320 6c6f 6164 2072 6177 2045 4347 2073  # load raw ECG s
-00000760: 6967 6e61 6c0a 7369 676e 616c 2c20 6d64  ignal.signal, md
-00000770: 6174 6120 3d20 7374 6f72 6167 652e 6c6f  ata = storage.lo
-00000780: 6164 5f74 7874 2827 2e2f 6578 616d 706c  ad_txt('./exampl
-00000790: 6573 2f65 6367 2e74 7874 2729 0a0a 2320  es/ecg.txt')..# 
-000007a0: 7072 6f63 6573 7320 6974 2061 6e64 2070  process it and p
-000007b0: 6c6f 740a 6f75 7420 3d20 6563 672e 6563  lot.out = ecg.ec
-000007c0: 6728 7369 676e 616c 3d73 6967 6e61 6c2c  g(signal=signal,
-000007d0: 2073 616d 706c 696e 675f 7261 7465 3d31   sampling_rate=1
-000007e0: 3030 302e 2c20 7368 6f77 3d54 7275 6529  000., show=True)
-000007f0: 0a60 6060 0a0a 5468 6973 2073 686f 756c  .```..This shoul
-00000800: 6420 7072 6f64 7563 6520 6120 706c 6f74  d produce a plot
-00000810: 2073 696d 696c 6172 2074 6f20 7468 6520   similar to the 
-00000820: 6f6e 6520 6265 6c6f 772e 0a0a 215b 4543  one below...![EC
-00000830: 4720 7375 6d6d 6172 7920 6578 616d 706c  G summary exampl
-00000840: 655d 2864 6f63 732f 696d 6167 6573 2f45  e](docs/images/E
-00000850: 4347 5f73 756d 6d61 7279 2e70 6e67 290a  CG_summary.png).
-00000860: 0a23 2320 4465 7065 6e64 656e 6369 6573  .## Dependencies
-00000870: 0a0a 2d20 6269 6469 6374 0a2d 2068 3570  ..- bidict.- h5p
-00000880: 790a 2d20 6d61 7470 6c6f 746c 6962 0a2d  y.- matplotlib.-
-00000890: 206e 756d 7079 0a2d 2073 6369 6b69 742d   numpy.- scikit-
-000008a0: 6c65 6172 6e0a 2d20 7363 6970 790a 2d20  learn.- scipy.- 
-000008b0: 7368 6f72 7475 7569 640a 2d20 7369 780a  shortuuid.- six.
-000008c0: 2d20 6a6f 626c 6962 0a0a 2323 2043 6974  - joblib..## Cit
-000008d0: 696e 670a 506c 6561 7365 2075 7365 2074  ing.Please use t
-000008e0: 6865 2066 6f6c 6c6f 7769 6e67 2069 6620  he following if 
-000008f0: 796f 7520 6e65 6564 2074 6f20 6369 7465  you need to cite
-00000900: 2042 696f 5350 5079 3a0a 0a2d 2043 6172   BioSPPy:..- Car
-00000910: 7265 6972 6173 2043 2c20 416c 7665 7320  reiras C, Alves 
-00000920: 4150 2c20 4c6f 7572 656e c3a7 6f20 412c  AP, Louren..o A,
-00000930: 2043 616e 656e 746f 2046 2c20 5369 6c76   Canento F, Silv
-00000940: 6120 482c 2046 7265 6420 412c 202a 6574  a H, Fred A, *et
-00000950: 2061 6c2e 2a0a 2020 2a2a 4269 6f53 5050   al.*.  **BioSPP
-00000960: 7920 2d20 4269 6f73 6967 6e61 6c20 5072  y - Biosignal Pr
-00000970: 6f63 6573 7369 6e67 2069 6e20 5079 7468  ocessing in Pyth
-00000980: 6f6e 2a2a 2c20 3230 3135 2d2c 0a20 2068  on**, 2015-,.  h
-00000990: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000009a0: 6d2f 5049 412d 4772 6f75 702f 4269 6f53  m/PIA-Group/BioS
-000009b0: 5050 792f 205b 4f6e 6c69 6e65 3b20 6163  PPy/ [Online; ac
-000009c0: 6365 7373 6564 2060 6060 3c79 6561 723e  cessed ```<year>
-000009d0: 2d3c 6d6f 6e74 683e 2d3c 6461 793e 6060  -<month>-<day>``
-000009e0: 605d 2e0a 0a60 6060 6c61 7465 780a 404d  `]...```latex.@M
-000009f0: 6973 637b 2c0a 2020 6175 7468 6f72 203d  isc{,.  author =
-00000a00: 207b 4361 726c 6f73 2043 6172 7265 6972   {Carlos Carreir
-00000a10: 6173 2061 6e64 2041 6e61 2050 7269 7363  as and Ana Prisc
-00000a20: 696c 6120 416c 7665 7320 616e 6420 416e  ila Alves and An
-00000a30: 6472 5c27 7b65 7d20 4c6f 7572 656e 5c63  dr\'{e} Louren\c
-00000a40: 7b63 7d6f 2061 6e64 2046 696c 6970 6520  {c}o and Filipe 
-00000a50: 4361 6e65 6e74 6f20 616e 6420 4875 676f  Canento and Hugo
-00000a60: 2053 696c 7661 2061 6e64 2041 6e61 2046   Silva and Ana F
-00000a70: 7265 6420 616e 6420 6f74 6865 7273 7d2c  red and others},
-00000a80: 0a20 2074 6974 6c65 203d 207b 7b42 696f  .  title = {{Bio
-00000a90: 5350 5079 7d3a 2042 696f 7369 676e 616c  SPPy}: Biosignal
-00000aa0: 2050 726f 6365 7373 696e 6720 696e 207b   Processing in {
-00000ab0: 5079 7468 6f6e 7d7d 2c0a 2020 7965 6172  Python}},.  year
-00000ac0: 203d 207b 3230 3135 2d2d 7d2c 0a20 2075   = {2015--},.  u
-00000ad0: 726c 203d 2022 6874 7470 733a 2f2f 6769  rl = "https://gi
-00000ae0: 7468 7562 2e63 6f6d 2f50 4941 2d47 726f  thub.com/PIA-Gro
-00000af0: 7570 2f42 696f 5350 5079 2f22 2c0a 2020  up/BioSPPy/",.  
-00000b00: 6e6f 7465 203d 207b 5b4f 6e6c 696e 653b  note = {[Online;
-00000b10: 2061 6363 6573 7365 6420 3c74 6f64 6179   accessed <today
-00000b20: 3e5d 7d0a 7d0a 6060 600a 0a23 2320 4c69  >]}.}.```..## Li
-00000b30: 6365 6e73 650a 0a42 696f 5350 5079 2069  cense..BioSPPy i
-00000b40: 7320 7265 6c65 6173 6564 2075 6e64 6572  s released under
-00000b50: 2074 6865 2042 5344 2033 2d63 6c61 7573   the BSD 3-claus
-00000b60: 6520 6c69 6365 6e73 652e 2053 6565 204c  e license. See L
-00000b70: 4943 454e 5345 2066 6f72 206d 6f72 6520  ICENSE for more 
-00000b80: 6465 7461 696c 732e 0a0a 2323 2044 6973  details...## Dis
-00000b90: 636c 6169 6d65 720a 0a54 6869 7320 7072  claimer..This pr
-00000ba0: 6f67 7261 6d20 6973 2064 6973 7472 6962  ogram is distrib
-00000bb0: 7574 6564 2069 6e20 7468 6520 686f 7065  uted in the hope
-00000bc0: 2069 7420 7769 6c6c 2062 6520 7573 6566   it will be usef
-00000bd0: 756c 2061 6e64 2070 726f 7669 6465 640a  ul and provided.
-00000be0: 746f 2079 6f75 2022 6173 2069 7322 2c20  to you "as is", 
-00000bf0: 6275 7420 5749 5448 4f55 5420 414e 5920  but WITHOUT ANY 
-00000c00: 5741 5252 414e 5459 2c20 7769 7468 6f75  WARRANTY, withou
-00000c10: 7420 6576 656e 2074 6865 2069 6d70 6c69  t even the impli
-00000c20: 6564 0a77 6172 7261 6e74 7920 6f66 204d  ed.warranty of M
-00000c30: 4552 4348 414e 5441 4249 4c49 5459 206f  ERCHANTABILITY o
-00000c40: 7220 4649 544e 4553 5320 464f 5220 4120  r FITNESS FOR A 
-00000c50: 5041 5254 4943 554c 4152 2050 5552 504f  PARTICULAR PURPO
-00000c60: 5345 2e20 5468 6973 0a70 726f 6772 616d  SE. This.program
-00000c70: 2069 7320 4e4f 5420 696e 7465 6e64 6564   is NOT intended
-00000c80: 2066 6f72 206d 6564 6963 616c 2064 6961   for medical dia
-00000c90: 676e 6f73 6973 2e20 5765 2065 7870 7265  gnosis. We expre
-00000ca0: 7373 6c79 2064 6973 636c 6169 6d20 616e  ssly disclaim an
-00000cb0: 790a 6c69 6162 696c 6974 7920 7768 6174  y.liability what
-00000cc0: 736f 6576 6572 2066 6f72 2061 6e79 2064  soever for any d
-00000cd0: 6972 6563 742c 2069 6e64 6972 6563 742c  irect, indirect,
-00000ce0: 2063 6f6e 7365 7175 656e 7469 616c 2c20   consequential, 
-00000cf0: 696e 6369 6465 6e74 616c 0a6f 7220 7370  incidental.or sp
-00000d00: 6563 6961 6c20 6461 6d61 6765 732c 2069  ecial damages, i
-00000d10: 6e63 6c75 6469 6e67 2c20 7769 7468 6f75  ncluding, withou
-00000d20: 7420 6c69 6d69 7461 7469 6f6e 2c20 6c6f  t limitation, lo
-00000d30: 7374 2072 6576 656e 7565 732c 206c 6f73  st revenues, los
-00000d40: 740a 7072 6f66 6974 732c 206c 6f73 7365  t.profits, losse
-00000d50: 7320 7265 7375 6c74 696e 6720 6672 6f6d  s resulting from
-00000d60: 2062 7573 696e 6573 7320 696e 7465 7272   business interr
-00000d70: 7570 7469 6f6e 206f 7220 6c6f 7373 206f  uption or loss o
-00000d80: 6620 6461 7461 2c0a 7265 6761 7264 6c65  f data,.regardle
-00000d90: 7373 206f 6620 7468 6520 666f 726d 206f  ss of the form o
-00000da0: 6620 6163 7469 6f6e 206f 7220 6c65 6761  f action or lega
-00000db0: 6c20 7468 656f 7279 2075 6e64 6572 2077  l theory under w
-00000dc0: 6869 6368 2074 6865 0a6c 6961 6269 6c69  hich the.liabili
-00000dd0: 7479 206d 6179 2062 6520 6173 7365 7274  ty may be assert
-00000de0: 6564 2c20 6576 656e 2069 6620 6164 7669  ed, even if advi
-00000df0: 7365 6420 6f66 2074 6865 2070 6f73 7369  sed of the possi
-00000e00: 6269 6c69 7479 206f 6620 7375 6368 0a64  bility of such.d
-00000e10: 616d 6167 6573 2e0a                      amages..
+00000000: 2323 2320 f09f 8e99 efb8 8f20 416e 6e6f  ### ....... Anno
+00000010: 756e 6365 6d65 6e74 730a 2323 2323 204c  uncements.#### L
+00000020: 6174 6573 740a 6060 600a f09f 8c80 204e  atest.```..... N
+00000030: 6577 206d 6f64 756c 6520 666f 7220 7369  ew module for si
+00000040: 676e 616c 2071 7561 6c69 7479 2061 7373  gnal quality ass
+00000050: 6573 736d 656e 7420 f09f 8c80 0a57 6974  essment .....Wit
+00000060: 6820 7468 6520 6269 6f73 7070 792e 7175  h the biosppy.qu
+00000070: 616c 6974 7920 6d6f 6475 6c65 2079 6f75  ality module you
+00000080: 2063 616e 206e 6f77 2065 7661 6c75 6174   can now evaluat
+00000090: 6520 7468 6520 7175 616c 6974 7920 6f66  e the quality of
+000000a0: 2079 6f75 7220 7369 676e 616c 7321 0a53   your signals!.S
+000000b0: 6f20 6661 722c 2074 6865 2045 4441 2061  o far, the EDA a
+000000c0: 6e64 2045 4347 2071 7561 6c69 7479 2061  nd ECG quality a
+000000d0: 7265 2061 7661 696c 6162 6c65 2c20 6275  re available, bu
+000000e0: 7420 6d6f 7265 2063 6f75 6c64 2062 6520  t more could be 
+000000f0: 6164 6465 6420 736f 6f6e 2e20 0a60 6060  added soon. .```
+00000100: 0a23 2323 2320 4e65 7720 6665 6174 7572  .#### New featur
+00000110: 6573 0a60 6060 0af0 9f8c 8020 4e65 7720  es.```..... New 
+00000120: 6d6f 6475 6c65 2066 6f72 2073 6967 6e61  module for signa
+00000130: 6c20 7175 616c 6974 7920 6173 7365 7373  l quality assess
+00000140: 6d65 6e74 2028 6269 6f73 7070 792e 7175  ment (biosppy.qu
+00000150: 616c 6974 7929 0af0 9fab 8020 4e65 7720  ality)..... New 
+00000160: 6d6f 6475 6c65 2066 6f72 2068 6561 7274  module for heart
+00000170: 2072 6174 6520 7661 7269 6162 696c 6974   rate variabilit
+00000180: 7920 2862 696f 7370 7079 2e73 6967 6e61  y (biosppy.signa
+00000190: 6c73 2e68 7276 290a f09f 8e8a 204e 6577  ls.hrv)..... New
+000001a0: 206d 6f64 756c 6520 666f 7220 6665 6174   module for feat
+000001b0: 7572 6520 6578 7472 6163 7469 6f6e 2028  ure extraction (
+000001c0: 6269 6f73 7070 792e 6665 6174 7572 6573  biosppy.features
+000001d0: 290a 6060 600a 0a0a 2320 4269 6f53 5050  ).```...# BioSPP
+000001e0: 7920 2d20 4269 6f73 6967 6e61 6c20 5072  y - Biosignal Pr
+000001f0: 6f63 6573 7369 6e67 2069 6e20 5079 7468  ocessing in Pyth
+00000200: 6f6e 0a0a 2a41 2074 6f6f 6c62 6f78 2066  on..*A toolbox f
+00000210: 6f72 2062 696f 7369 676e 616c 2070 726f  or biosignal pro
+00000220: 6365 7373 696e 6720 7772 6974 7465 6e20  cessing written 
+00000230: 696e 2050 7974 686f 6e2e 2a0a 0a3c 6120  in Python.*..<a 
+00000240: 6872 6566 3d22 6874 7470 733a 2f2f 6269  href="https://bi
+00000250: 6f73 7070 792e 7265 6164 7468 6564 6f63  osppy.readthedoc
+00000260: 732e 6f72 672f 223e 0a3c 7069 6374 7572  s.org/">.<pictur
+00000270: 653e 0a20 203c 736f 7572 6365 206d 6564  e>.  <source med
+00000280: 6961 3d22 2870 7265 6665 7273 2d63 6f6c  ia="(prefers-col
+00000290: 6f72 2d73 6368 656d 653a 206c 6967 6874  or-scheme: light
+000002a0: 2922 2073 7263 7365 743d 2264 6f63 732f  )" srcset="docs/
+000002b0: 6c6f 676f 2f6c 6f67 6f5f 3430 302e 706e  logo/logo_400.pn
+000002c0: 6722 3e0a 2020 3c73 6f75 7263 6520 6d65  g">.  <source me
+000002d0: 6469 613d 2228 7072 6566 6572 732d 636f  dia="(prefers-co
+000002e0: 6c6f 722d 7363 6865 6d65 3a20 6461 726b  lor-scheme: dark
+000002f0: 2922 2073 7263 7365 743d 2264 6f63 732f  )" srcset="docs/
+00000300: 6c6f 676f 2f6c 6f67 6f5f 696e 7665 7274  logo/logo_invert
+00000310: 6564 5f34 3030 2e70 6e67 223e 0a20 203c  ed_400.png">.  <
+00000320: 696d 6720 616c 743d 2249 6d61 6765 2220  img alt="Image" 
+00000330: 7469 746c 653d 2249 206b 6e6f 7720 796f  title="I know yo
+00000340: 7527 7265 206c 6973 7465 6e69 6e67 2120  u're listening! 
+00000350: 2d20 786b 6364 2e63 6f6d 2f35 3235 223e  - xkcd.com/525">
+00000360: 0a3c 2f70 6963 7475 7265 3e0a 3c2f 613e  .</picture>.</a>
+00000370: 0a0a 5468 6520 746f 6f6c 626f 7820 6275  ..The toolbox bu
+00000380: 6e64 6c65 7320 746f 6765 7468 6572 2076  ndles together v
+00000390: 6172 696f 7573 2073 6967 6e61 6c20 7072  arious signal pr
+000003a0: 6f63 6573 7369 6e67 2061 6e64 2070 6174  ocessing and pat
+000003b0: 7465 726e 2072 6563 6f67 6e69 7469 6f6e  tern recognition
+000003c0: 0a6d 6574 686f 6473 2067 6561 7265 6420  .methods geared 
+000003d0: 746f 7761 7264 7320 7468 6520 616e 616c  towards the anal
+000003e0: 7973 6973 206f 6620 6269 6f73 6967 6e61  ysis of biosigna
+000003f0: 6c73 2e0a 0a48 6967 686c 6967 6874 733a  ls...Highlights:
+00000400: 0a0a 2d20 5375 7070 6f72 7420 666f 7220  ..- Support for 
+00000410: 7661 7269 6f75 7320 6269 6f73 6967 6e61  various biosigna
+00000420: 6c73 3a20 4256 502c 2045 4347 2c20 4544  ls: BVP, ECG, ED
+00000430: 412c 2045 4547 2c20 454d 472c 2050 4347  A, EEG, EMG, PCG
+00000440: 2c20 5050 472c 2052 6573 7069 7261 7469  , PPG, Respirati
+00000450: 6f6e 0a2d 2053 6967 6e61 6c20 616e 616c  on.- Signal anal
+00000460: 7973 6973 2070 7269 6d69 7469 7665 733a  ysis primitives:
+00000470: 2066 696c 7465 7269 6e67 2c20 6672 6571   filtering, freq
+00000480: 7565 6e63 7920 616e 616c 7973 6973 0a2d  uency analysis.-
+00000490: 2043 6c75 7374 6572 696e 670a 2d20 4269   Clustering.- Bi
+000004a0: 6f6d 6574 7269 6373 0a0a 446f 6375 6d65  ometrics..Docume
+000004b0: 6e74 6174 696f 6e20 6361 6e20 6265 2066  ntation can be f
+000004c0: 6f75 6e64 2061 743a 203c 6874 7470 733a  ound at: <https:
+000004d0: 2f2f 6269 6f73 7070 792e 7265 6164 7468  //biosppy.readth
+000004e0: 6564 6f63 732e 6f72 672f 3e0a 0a23 2320  edocs.org/>..## 
+000004f0: 496e 7374 616c 6c61 7469 6f6e 0a0a 496e  Installation..In
+00000500: 7374 616c 6c61 7469 6f6e 2063 616e 2062  stallation can b
+00000510: 6520 6561 7369 6c79 2064 6f6e 6520 7769  e easily done wi
+00000520: 7468 2060 7069 7060 3a0a 0a60 6060 6261  th `pip`:..```ba
+00000530: 7368 0a24 2070 6970 2069 6e73 7461 6c6c  sh.$ pip install
+00000540: 2062 696f 7370 7079 0a60 6060 0a0a 416c   biosppy.```..Al
+00000550: 7465 726e 6174 6976 656c 792c 2079 6f75  ternatively, you
+00000560: 2063 616e 2069 6e73 7461 6c6c 2074 6865   can install the
+00000570: 206c 6174 6573 7420 7665 7273 696f 6e20   latest version 
+00000580: 6672 6f6d 2074 6865 2047 6974 4875 6220  from the GitHub 
+00000590: 7265 706f 7369 746f 7279 3a0a 0a60 6060  repository:..```
+000005a0: 6261 7368 0a24 2070 6970 2069 6e73 7461  bash.$ pip insta
+000005b0: 6c6c 2067 6974 2b68 7474 7073 3a2f 2f67  ll git+https://g
+000005c0: 6974 6875 622e 636f 6d2f 7363 6965 6e74  ithub.com/scient
+000005d0: 6973 7374 2f42 696f 5350 5079 2e67 6974  isst/BioSPPy.git
+000005e0: 0a60 6060 0a0a 2323 2053 696d 706c 6520  .```..## Simple 
+000005f0: 4578 616d 706c 650a 0a54 6865 2063 6f64  Example..The cod
+00000600: 6520 6265 6c6f 7720 6c6f 6164 7320 616e  e below loads an
+00000610: 2045 4347 2073 6967 6e61 6c20 6672 6f6d   ECG signal from
+00000620: 2074 6865 2060 6578 616d 706c 6573 6020   the `examples` 
+00000630: 666f 6c64 6572 2c20 6669 6c74 6572 7320  folder, filters 
+00000640: 6974 2c0a 7065 7266 6f72 6d73 2052 2d70  it,.performs R-p
+00000650: 6561 6b20 6465 7465 6374 696f 6e2c 2061  eak detection, a
+00000660: 6e64 2063 6f6d 7075 7465 7320 7468 6520  nd computes the 
+00000670: 696e 7374 616e 7461 6e65 6f75 7320 6865  instantaneous he
+00000680: 6172 7420 7261 7465 2e0a 0a60 6060 7079  art rate...```py
+00000690: 7468 6f6e 0a66 726f 6d20 6269 6f73 7070  thon.from biospp
+000006a0: 7920 696d 706f 7274 2073 746f 7261 6765  y import storage
+000006b0: 0a66 726f 6d20 6269 6f73 7070 792e 7369  .from biosppy.si
+000006c0: 676e 616c 7320 696d 706f 7274 2065 6367  gnals import ecg
+000006d0: 0a0a 2320 6c6f 6164 2072 6177 2045 4347  ..# load raw ECG
+000006e0: 2073 6967 6e61 6c0a 7369 676e 616c 2c20   signal.signal, 
+000006f0: 6d64 6174 6120 3d20 7374 6f72 6167 652e  mdata = storage.
+00000700: 6c6f 6164 5f74 7874 2827 2e2f 6578 616d  load_txt('./exam
+00000710: 706c 6573 2f65 6367 2e74 7874 2729 0a0a  ples/ecg.txt')..
+00000720: 2320 7072 6f63 6573 7320 6974 2061 6e64  # process it and
+00000730: 2070 6c6f 740a 6f75 7420 3d20 6563 672e   plot.out = ecg.
+00000740: 6563 6728 7369 676e 616c 3d73 6967 6e61  ecg(signal=signa
+00000750: 6c2c 2073 616d 706c 696e 675f 7261 7465  l, sampling_rate
+00000760: 3d31 3030 302e 2c20 7368 6f77 3d54 7275  =1000., show=Tru
+00000770: 6529 0a60 6060 0a0a 5468 6973 2073 686f  e).```..This sho
+00000780: 756c 6420 7072 6f64 7563 6520 6120 706c  uld produce a pl
+00000790: 6f74 2073 696d 696c 6172 2074 6f20 7468  ot similar to th
+000007a0: 6520 6f6e 6520 6265 6c6f 772e 0a0a 215b  e one below...![
+000007b0: 4543 4720 7375 6d6d 6172 7920 6578 616d  ECG summary exam
+000007c0: 706c 655d 2864 6f63 732f 696d 6167 6573  ple](docs/images
+000007d0: 2f45 4347 5f73 756d 6d61 7279 2e70 6e67  /ECG_summary.png
+000007e0: 290a 0a23 2320 4465 7065 6e64 656e 6369  )..## Dependenci
+000007f0: 6573 0a0a 2d20 6269 6469 6374 0a2d 2068  es..- bidict.- h
+00000800: 3570 790a 2d20 6d61 7470 6c6f 746c 6962  5py.- matplotlib
+00000810: 0a2d 206e 756d 7079 0a2d 2073 6369 6b69  .- numpy.- sciki
+00000820: 742d 6c65 6172 6e0a 2d20 7363 6970 790a  t-learn.- scipy.
+00000830: 2d20 7368 6f72 7475 7569 640a 2d20 7369  - shortuuid.- si
+00000840: 780a 2d20 6a6f 626c 6962 0a0a 2323 2043  x.- joblib..## C
+00000850: 6974 696e 670a 506c 6561 7365 2075 7365  iting.Please use
+00000860: 2074 6865 2066 6f6c 6c6f 7769 6e67 2069   the following i
+00000870: 6620 796f 7520 6e65 6564 2074 6f20 6369  f you need to ci
+00000880: 7465 2042 696f 5350 5079 3a0a 0a2d 2043  te BioSPPy:..- C
+00000890: 6172 7265 6972 6173 2043 2c20 416c 7665  arreiras C, Alve
+000008a0: 7320 4150 2c20 4c6f 7572 656e c3a7 6f20  s AP, Louren..o 
+000008b0: 412c 2043 616e 656e 746f 2046 2c20 5369  A, Canento F, Si
+000008c0: 6c76 6120 482c 2046 7265 6420 412c 202a  lva H, Fred A, *
+000008d0: 6574 2061 6c2e 2a0a 2020 2a2a 4269 6f53  et al.*.  **BioS
+000008e0: 5050 7920 2d20 4269 6f73 6967 6e61 6c20  PPy - Biosignal 
+000008f0: 5072 6f63 6573 7369 6e67 2069 6e20 5079  Processing in Py
+00000900: 7468 6f6e 2a2a 2c20 3230 3135 2d2c 0a20  thon**, 2015-,. 
+00000910: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00000920: 636f 6d2f 5049 412d 4772 6f75 702f 4269  com/PIA-Group/Bi
+00000930: 6f53 5050 792f 205b 4f6e 6c69 6e65 3b20  oSPPy/ [Online; 
+00000940: 6163 6365 7373 6564 2060 6060 3c79 6561  accessed ```<yea
+00000950: 723e 2d3c 6d6f 6e74 683e 2d3c 6461 793e  r>-<month>-<day>
+00000960: 6060 605d 2e0a 0a60 6060 6c61 7465 780a  ```]...```latex.
+00000970: 404d 6973 637b 2c0a 2020 6175 7468 6f72  @Misc{,.  author
+00000980: 203d 207b 4361 726c 6f73 2043 6172 7265   = {Carlos Carre
+00000990: 6972 6173 2061 6e64 2041 6e61 2050 7269  iras and Ana Pri
+000009a0: 7363 696c 6120 416c 7665 7320 616e 6420  scila Alves and 
+000009b0: 416e 6472 5c27 7b65 7d20 4c6f 7572 656e  Andr\'{e} Louren
+000009c0: 5c63 7b63 7d6f 2061 6e64 2046 696c 6970  \c{c}o and Filip
+000009d0: 6520 4361 6e65 6e74 6f20 616e 6420 4875  e Canento and Hu
+000009e0: 676f 2053 696c 7661 2061 6e64 2041 6e61  go Silva and Ana
+000009f0: 2046 7265 6420 616e 6420 6f74 6865 7273   Fred and others
+00000a00: 7d2c 0a20 2074 6974 6c65 203d 207b 7b42  },.  title = {{B
+00000a10: 696f 5350 5079 7d3a 2042 696f 7369 676e  ioSPPy}: Biosign
+00000a20: 616c 2050 726f 6365 7373 696e 6720 696e  al Processing in
+00000a30: 207b 5079 7468 6f6e 7d7d 2c0a 2020 7965   {Python}},.  ye
+00000a40: 6172 203d 207b 3230 3135 2d2d 7d2c 0a20  ar = {2015--},. 
+00000a50: 2075 726c 203d 2022 6874 7470 733a 2f2f   url = "https://
+00000a60: 6769 7468 7562 2e63 6f6d 2f50 4941 2d47  github.com/PIA-G
+00000a70: 726f 7570 2f42 696f 5350 5079 2f22 2c0a  roup/BioSPPy/",.
+00000a80: 2020 6e6f 7465 203d 207b 5b4f 6e6c 696e    note = {[Onlin
+00000a90: 653b 2061 6363 6573 7365 6420 3c74 6f64  e; accessed <tod
+00000aa0: 6179 3e5d 7d0a 7d0a 6060 600a 0a23 2320  ay>]}.}.```..## 
+00000ab0: 4c69 6365 6e73 650a 0a42 696f 5350 5079  License..BioSPPy
+00000ac0: 2069 7320 7265 6c65 6173 6564 2075 6e64   is released und
+00000ad0: 6572 2074 6865 2042 5344 2033 2d63 6c61  er the BSD 3-cla
+00000ae0: 7573 6520 6c69 6365 6e73 652e 2053 6565  use license. See
+00000af0: 204c 4943 454e 5345 2066 6f72 206d 6f72   LICENSE for mor
+00000b00: 6520 6465 7461 696c 732e 0a0a 2323 2044  e details...## D
+00000b10: 6973 636c 6169 6d65 720a 0a54 6869 7320  isclaimer..This 
+00000b20: 7072 6f67 7261 6d20 6973 2064 6973 7472  program is distr
+00000b30: 6962 7574 6564 2069 6e20 7468 6520 686f  ibuted in the ho
+00000b40: 7065 2069 7420 7769 6c6c 2062 6520 7573  pe it will be us
+00000b50: 6566 756c 2061 6e64 2070 726f 7669 6465  eful and provide
+00000b60: 640a 746f 2079 6f75 2022 6173 2069 7322  d.to you "as is"
+00000b70: 2c20 6275 7420 5749 5448 4f55 5420 414e  , but WITHOUT AN
+00000b80: 5920 5741 5252 414e 5459 2c20 7769 7468  Y WARRANTY, with
+00000b90: 6f75 7420 6576 656e 2074 6865 2069 6d70  out even the imp
+00000ba0: 6c69 6564 0a77 6172 7261 6e74 7920 6f66  lied.warranty of
+00000bb0: 204d 4552 4348 414e 5441 4249 4c49 5459   MERCHANTABILITY
+00000bc0: 206f 7220 4649 544e 4553 5320 464f 5220   or FITNESS FOR 
+00000bd0: 4120 5041 5254 4943 554c 4152 2050 5552  A PARTICULAR PUR
+00000be0: 504f 5345 2e20 5468 6973 0a70 726f 6772  POSE. This.progr
+00000bf0: 616d 2069 7320 4e4f 5420 696e 7465 6e64  am is NOT intend
+00000c00: 6564 2066 6f72 206d 6564 6963 616c 2064  ed for medical d
+00000c10: 6961 676e 6f73 6973 2e20 5765 2065 7870  iagnosis. We exp
+00000c20: 7265 7373 6c79 2064 6973 636c 6169 6d20  ressly disclaim 
+00000c30: 616e 790a 6c69 6162 696c 6974 7920 7768  any.liability wh
+00000c40: 6174 736f 6576 6572 2066 6f72 2061 6e79  atsoever for any
+00000c50: 2064 6972 6563 742c 2069 6e64 6972 6563   direct, indirec
+00000c60: 742c 2063 6f6e 7365 7175 656e 7469 616c  t, consequential
+00000c70: 2c20 696e 6369 6465 6e74 616c 0a6f 7220  , incidental.or 
+00000c80: 7370 6563 6961 6c20 6461 6d61 6765 732c  special damages,
+00000c90: 2069 6e63 6c75 6469 6e67 2c20 7769 7468   including, with
+00000ca0: 6f75 7420 6c69 6d69 7461 7469 6f6e 2c20  out limitation, 
+00000cb0: 6c6f 7374 2072 6576 656e 7565 732c 206c  lost revenues, l
+00000cc0: 6f73 740a 7072 6f66 6974 732c 206c 6f73  ost.profits, los
+00000cd0: 7365 7320 7265 7375 6c74 696e 6720 6672  ses resulting fr
+00000ce0: 6f6d 2062 7573 696e 6573 7320 696e 7465  om business inte
+00000cf0: 7272 7570 7469 6f6e 206f 7220 6c6f 7373  rruption or loss
+00000d00: 206f 6620 6461 7461 2c0a 7265 6761 7264   of data,.regard
+00000d10: 6c65 7373 206f 6620 7468 6520 666f 726d  less of the form
+00000d20: 206f 6620 6163 7469 6f6e 206f 7220 6c65   of action or le
+00000d30: 6761 6c20 7468 656f 7279 2075 6e64 6572  gal theory under
+00000d40: 2077 6869 6368 2074 6865 0a6c 6961 6269   which the.liabi
+00000d50: 6c69 7479 206d 6179 2062 6520 6173 7365  lity may be asse
+00000d60: 7274 6564 2c20 6576 656e 2069 6620 6164  rted, even if ad
+00000d70: 7669 7365 6420 6f66 2074 6865 2070 6f73  vised of the pos
+00000d80: 7369 6269 6c69 7479 206f 6620 7375 6368  sibility of such
+00000d90: 0a64 616d 6167 6573 2e0a                 .damages..
```

### Comparing `biosppy-2.1.2/biosppy/__init__.py` & `biosppy-2.2.0/biosppy/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,10 +13,10 @@
 from __future__ import absolute_import, division, print_function
 
 # get version
 from .__version__ import __version__
 
 # allow lazy loading
 from .signals import acc, abp, bvp, ppg, pcg, ecg, eda, eeg, emg, resp, tools, hrv
-from .synthesizers import ecg
+from .synthesizers import ecg, emg
 from .inter_plotting import ecg, acc
-from .features import frequency, time, time_freq, cepstral, phase_space
+from .features import frequency, time, time_freq, cepstral, phase_space
```

### Comparing `biosppy-2.1.2/biosppy/biometrics.py` & `biosppy-2.2.0/biosppy/biometrics.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.1.2/biosppy/clustering.py` & `biosppy-2.2.0/biosppy/clustering.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.1.2/biosppy/features/__init__.py` & `biosppy-2.2.0/biosppy/features/__init__.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.1.2/biosppy/features/cepstral.py` & `biosppy-2.2.0/biosppy/features/cepstral.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     for arg, name in zip(time_feats, time_feats.keys()):
         feats = feats.append(arg, 'mfcc_' + name)
 
     return feats
 
 
 def freq_to_mel(hertz):
-    """Converts mel-frequencies to hertz frequencies.
+    """Converts mel-frequencies to hertz frequencies [Kool12]_.
     
     Parameters
     ----------
     hertz : array
         Hertz frequencies.
  
     Returns
@@ -125,23 +125,23 @@
     Returns
     -------
     mfcc : array
         Signal mel-frequency cepstral coefficients.
 
     References
     ----------
-    .. [Haytham16] Fayek, Haytham. "Speech Processing for Machine Learning: Filter
-    banks, Mel-Frequency Cepstral Coefficients (MFCCs) and What's In-Between."
-    Blog post. 2016. https://haythamfayek.com/2016/04/21/speech-processing-for-machine-learning.html
-    .. 'Vanilla STFT and MFCC' by brihijoshi, accessed in october 2022:
-    https://github.com/brihijoshi/vanilla-stft-mfcc/
-    .. 'Time Series Feature Extraction Library' by fraunhoferportugal, accessed in october 2022:
-    https://github.com/fraunhoferportugal/tsfel/
-    .. 'MFCC implementation and tutorial' by ilyamich, accessed in october 2022:
-    https://www.kaggle.com/code/ilyamich/mfcc-implementation-and-tutorial
+    .. [Haytham16] Fayek, Haytham. "Speech Processing for Machine Learning: Filter banks, 
+        Mel-Frequency Cepstral Coefficients (MFCCs) and What's In-Between."Blog post. 2016. 
+        https://haythamfayek.com/2016/04/21/speech-processing-for-machine-learning.html
+    .. [Brihijoshi] 'Vanilla STFT and MFCC' by brihijoshi, 
+        accessed in october 2022:https://github.com/brihijoshi/vanilla-stft-mfcc/
+    .. [Tsfel] 'Time Series Feature Extraction Library' by fraunhoferportugal, 
+        accessed in october 2022: https://github.com/fraunhoferportugal/tsfel/
+    .. [Ilyamich] 'MFCC implementation and tutorial' by ilyamich, accessed in october 2022:
+        https://www.kaggle.com/code/ilyamich/mfcc-implementation-and-tutorial
 
    """
 
     # check inputs
     if signal is None:
         raise TypeError("Please specify an input signal.")
```

### Comparing `biosppy-2.1.2/biosppy/features/frequency.py` & `biosppy-2.2.0/biosppy/features/frequency.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.1.2/biosppy/features/phase_space.py` & `biosppy-2.2.0/biosppy/features/phase_space.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,18 +14,14 @@
 import numpy as np
 from scipy.signal import resample
 from scipy.spatial.distance import pdist, squareform
 
 # local
 from .. import utils
 
-# variables
-MIN = 2
-
-
 def phase_space(signal=None):
     """Compute phase-space features describing the signal.
 
     Parameters
     ----------
     signal : array
         Input signal.
@@ -149,14 +145,17 @@
 
     # ensure numpy
     rec_matrix = np.array(rec_matrix)
 
     # initialize output
     feats = utils.ReturnTuple((), ())
 
+    # variables
+    MIN = 2
+    
     # compute features
     threshold = 0.5
     len_rec_matrix = len(rec_matrix)
     for l in range(len_rec_matrix):
         for c in range(len_rec_matrix):
             rec_matrix[l, c] = 1 if rec_matrix[l, c] < threshold else 0
     len_rec_matrix = len(rec_matrix)
```

### Comparing `biosppy-2.1.2/biosppy/features/time.py` & `biosppy-2.2.0/biosppy/features/time.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.1.2/biosppy/features/time_freq.py` & `biosppy-2.2.0/biosppy/features/time_freq.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.1.2/biosppy/inter_plotting/acc.py` & `biosppy-2.2.0/biosppy/inter_plotting/acc.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.1.2/biosppy/inter_plotting/ecg.py` & `biosppy-2.2.0/biosppy/inter_plotting/ecg.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.1.2/biosppy/metrics.py` & `biosppy-2.2.0/biosppy/metrics.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.1.2/biosppy/plotting.py` & `biosppy-2.2.0/biosppy/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,48 +20,61 @@
 
 # 3rd party
 import matplotlib.pyplot as plt
 import matplotlib.gridspec as gridspec
 import matplotlib.patches as patches
 import matplotlib.lines as lines
 import numpy as np
+from mock import MagicMock
 
 # local
 from . import utils
 from .signals import tools as st
 
 # Globals
 MAJOR_LW = 1.5
 MED_LW = 1.25
 MINOR_LW = 1.0
 MAX_ROWS = 10
 LOGOS_FOLDER = '.logos'
 BIOSPPY_LOGO = 'biosppy.png'
 SCIENTISST_LOGO = 'scientisst.png'
 
-# matplotlib settings
-plt.rcParams['text.color'] = '#495057'
-plt.rcParams['axes.labelcolor'] = '#495057'
-plt.rcParams['axes.labelsize'] = 10
-plt.rcParams['axes.edgecolor'] = '#495057'
-plt.rcParams['axes.facecolor'] = '#f8f9fa'
-plt.rcParams['axes.titlesize'] = 11
-plt.rcParams['xtick.color'] = '#495057'
-plt.rcParams['ytick.color'] = '#495057'
-plt.rcParams['grid.color'] = '#ebeef0'
-plt.rcParams['axes.spines.top'] = False
-plt.rcParams['axes.spines.right'] = False
-plt.rcParams['axes.grid'] = True
-plt.rcParams['grid.linestyle'] = '-'
-plt.rcParams['grid.color'] = '#ebeef0'
-plt.rcParams['legend.facecolor'] = 'white'
-plt.rcParams['legend.framealpha'] = 0.75
-plt.rcParams['legend.loc'] = 'upper right'
-plt.rcParams['legend.fontsize'] = 8
+def _get_params():
+    """Get matplotlib parameters.
 
+    Returns
+    -------
+    params : dict
+        Dictionary of matplotlib parameters.
+
+    """
+
+    params = {
+        'text.color': '#495057',
+        'axes.labelcolor': '#495057',
+        'axes.labelsize': 10,
+        'axes.edgecolor': '#495057',
+        'axes.facecolor': '#f8f9fa',
+        'axes.titlesize': 11,
+        'xtick.color': '#495057',
+        'ytick.color': '#495057',
+        'grid.color': '#ebeef0',
+        'axes.spines.top': False,
+        'axes.spines.right': False,
+        'axes.grid': True,
+        'grid.linestyle': '-',
+        'grid.color': '#ebeef0',
+        'legend.facecolor': 'white',
+        'legend.framealpha': 0.75,
+        'legend.loc': 'upper right',
+        'legend.fontsize': 8
+    }
+
+    return params
 
 def color_palette(idx):
     """Color palette to use throughout the biosppy package
 
     Parameters
     ----------
     idx: str or int
@@ -159,14 +172,17 @@
 
     """
 
     # compute frequency response
     freqs, resp = st._filter_resp(b, a,
                                   sampling_rate=sampling_rate,
                                   nfreqs=nfreqs)
+    
+    # get matplotlib parameters
+    plt.rcParams.update(_get_params())
 
     # plot
     if ax is None:
         fig = plt.figure(figsize=(8, 4))
         ax = fig.add_subplot(211)
         ax2 = fig.add_subplot(212)
     else:
@@ -304,14 +320,17 @@
     """
 
     freqs, power = st.power_spectrum(signal, sampling_rate,
                                      pad=0,
                                      pow2=False,
                                      decibel=True)
 
+    # get matplotlib parameters
+    plt.rcParams.update(_get_params())
+
     fig = plt.figure()
     ax = fig.add_subplot(111)
 
     ax.plot(freqs, power, linewidth=MAJOR_LW)
     ax.set_xlabel('Frequency (Hz)')
     ax.set_ylabel('Power (dB)')
     ax.grid()
@@ -365,14 +384,17 @@
         If True, show the plot immediately.
 
     """
 
     raw_t = np.transpose(raw)
     acc_x, acc_y, acc_z = raw_t[0], raw_t[1], raw_t[2]
 
+    # get matplotlib parameters
+    plt.rcParams.update(_get_params())
+
     fig = plt.figure(figsize=(10, 5))
     fig.suptitle('ACC Summary', fontsize=12, fontweight='bold')
     gs = gridspec.GridSpec(6, 2)
     fig.subplots_adjust(top=0.85, hspace=0.7, wspace=0.34, left=0.13,
                         right=0.96, bottom=0.18)
 
     # raw signal (acc_x)
@@ -492,14 +514,16 @@
         the units information. Default is None.
     path : str, optional
         If provided, the plot will be saved to the specified file.
     show : bool, optional
         If True, show the plot immediately.
 
     """
+    # get matplotlib parameters
+    plt.rcParams.update(_get_params())
 
     fig = plt.figure(figsize=(10, 5))
     fig.suptitle('PPG Summary', fontsize=12, fontweight='bold')
     gs = gridspec.GridSpec(6, 2)
     fig.subplots_adjust(top=0.88, bottom=0.12, hspace=0.9, wspace=0.3,
                         left=0.1, right=0.96)
 
@@ -608,14 +632,16 @@
         Instantaneous heart rate (bpm).
     path : str, optional
         If provided, the plot will be saved to the specified file.
     show : bool, optional
         If True, show the plot immediately.
 
     """
+    # get matplotlib parameters
+    plt.rcParams.update(_get_params())
 
     fig = plt.figure()
     fig.suptitle('BVP Summary')
 
     # raw signal
     ax1 = fig.add_subplot(311)
 
@@ -701,14 +727,16 @@
         Instantaneous heart rate (bpm).
     path : str, optional
         If provided, the plot will be saved to the specified file.
     show : bool, optional
         If True, show the plot immediately.
 
     """
+    # get matplotlib parameters
+    plt.rcParams.update(_get_params())
 
     fig = plt.figure()
     fig.suptitle('ABP Summary')
 
     # raw signal
     ax1 = fig.add_subplot(311)
 
@@ -804,14 +832,16 @@
         the units information. Default is None.
     path : str, optional
         If provided, the plot will be saved to the specified file.
     show : bool, optional
         If True, show the plot immediately.
 
     """
+    # get matplotlib parameters
+    plt.rcParams.update(_get_params())
 
     fig = plt.figure(figsize=(10, 5))
     fig.suptitle('EDA Summary', fontsize=14, fontweight='bold')
     gs = gridspec.GridSpec(6, 2)
     fig.subplots_adjust(top=0.85, hspace=0.7, wspace=0.34, left=0.13,
                         right=0.96, bottom=0.18)
 
@@ -942,14 +972,16 @@
         the units information. Default is None.
     path : str, optional
         If provided, the plot will be saved to the specified file.
     show : bool, optional
         If True, show the plot immediately.
 
     """
+    # get matplotlib parameters
+    plt.rcParams.update(_get_params())
 
     fig = plt.figure(figsize=(10, 5))
     fig.suptitle('EMG Summary', fontsize=12, fontweight='bold')
     fig.subplots_adjust(top=0.85, hspace=0.25, wspace=0.34, left=0.1,
                         right=0.96, bottom=0.18)
 
     if processed is not None:
@@ -1057,14 +1089,16 @@
         the units information. Default is None.
     path : str, optional
         If provided, the plot will be saved to the specified file.
     show : bool, optional
         If True, show the plot immediately.
 
     """
+    # get matplotlib parameters
+    plt.rcParams.update(_get_params())
 
     fig = plt.figure(figsize=(10, 5))
     fig.suptitle('RESP Summary', fontsize=12, fontweight='bold')
     fig.subplots_adjust(top=0.85, hspace=0.35, wspace=0.34, left=0.13,
                         right=0.96, bottom=0.18)
 
     # raw signal
@@ -1349,14 +1383,17 @@
         labels = ['Ch. %d' % i for i in range(nch)]
 
     if nch < nrows:
         nrows = nch
 
     ncols = int(np.ceil(nch / float(nrows)))
 
+    # get matplotlib parameters
+    plt.rcParams.update(_get_params())
+
     fig = plt.figure()
 
     # title
     if title is not None:
         fig.suptitle(title)
 
     gs = gridspec.GridSpec(nrows, ncols, hspace=0, wspace=0.2)
@@ -1451,14 +1488,16 @@
         the units information. Default is None.
     path : str, optional
         If provided, the plot will be saved to the specified file.
     show : bool, optional
         If True, show the plot immediately.
 
     """
+    # get matplotlib parameters
+    plt.rcParams.update(_get_params())
 
     fig = plt.figure(figsize=(10, 5))
     fig.suptitle('ECG Summary', fontsize=12, fontweight='bold')
     gs = gridspec.GridSpec(6, 2)
     fig.subplots_adjust(top=0.88, bottom=0.12, hspace=0.9, wspace=0.3,
                         left=0.1, right=0.96)
 
@@ -1573,14 +1612,16 @@
         Instantaneous heart rate (bpm).
     path : str, optional
         If provided, the plot will be saved to the specified file.
     show : bool, optional
         If True, show the plot immediately.
 
     """
+    # get matplotlib parameters
+    plt.rcParams.update(_get_params())
 
     fig = plt.figure()
     fig.suptitle('BCG Summary')
     gs = gridspec.GridSpec(6, 2)
 
     # raw signal
     ax1 = fig.add_subplot(gs[:2, 0])
@@ -1658,14 +1699,15 @@
              heart_sounds=None,
              heart_rate_ts=None,
              inst_heart_rate=None,
              units=None,
              path=None,
              show=False):
     """Create a summary plot from the output of signals.pcg.pcg.
+    
     Parameters
     ----------
     ts : array
         Signal time axis reference (seconds).
     raw : array
         Raw PCG signal.
     filtered : array
@@ -1683,14 +1725,16 @@
         the units information. Default is None.
     path : str, optional
         If provided, the plot will be saved to the specified file.
     show : bool, optional
         If True, show the plot immediately.
 
     """
+    # get matplotlib parameters
+    plt.rcParams.update(_get_params())
 
     fig = plt.figure(figsize=(12, 5))
     fig.suptitle('PCG Summary', fontsize=12, fontweight='bold')
     gs = gridspec.GridSpec(6, 2)
     fig.subplots_adjust(top=0.88, bottom=0.12, hspace=0.9, wspace=0.3,
                         left=0.1, right=0.96)
 
@@ -1810,14 +1854,16 @@
 
     Returns
     -------
     fig : Figure
         Figure object.
 
     """
+    # get matplotlib parameters
+    plt.rcParams.update(_get_params())
 
     if ax is None:
         fig = plt.figure()
         ax = fig.add_subplot(111)
     else:
         fig = ax.figure
 
@@ -1854,14 +1900,16 @@
         Classifier reference index for the Equal Error Rate.
     path : str, optional
         If provided, the plot will be saved to the specified file.
     show : bool, optional
         If True, show the plot immediately.
 
     """
+    # get matplotlib parameters
+    plt.rcParams.update(_get_params())
 
     fig = plt.figure()
     fig.suptitle('Biometrics Summary')
 
     c_sub = ['#008bff', '#8dd000']
     c_global = ['#0037ff', 'g']
 
@@ -1952,14 +2000,16 @@
         Dictionary with the sample indices (rows from `data`) for each cluster.
     path : str, optional
         If provided, the plot will be saved to the specified file.
     show : bool, optional
         If True, show the plot immediately.
 
     """
+    # get matplotlib parameters
+    plt.rcParams.update(_get_params())
 
     fig = plt.figure()
     fig.suptitle('Clustering Summary')
 
     ymin, ymax = _yscaling(data, alpha=1.2)
 
     # determine number of clusters
@@ -2379,14 +2429,17 @@
         td_out = td_out.as_dict()
     if nl_out is not None:
         nl_out = nl_out.as_dict()
     if fd_out is not None:
         fd_out = fd_out.as_dict()
 
     # plot
+    # get matplotlib parameters
+    plt.rcParams.update(_get_params())
+
     fig = plt.figure(figsize=(12, 6))
     fig.suptitle('HRV Summary', fontsize=12, fontweight='bold')
     gs = gridspec.GridSpec(6, 2)
 
     # plot rri and display time domain features
     ax1 = fig.add_subplot(gs[:2, 0])
     time_legends = {'Mean': (td_out['rr_mean'], 'ms'),
```

### Comparing `biosppy-2.1.2/biosppy/signals/__init__.py` & `biosppy-2.2.0/biosppy/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.1.2/biosppy/signals/abp.py` & `biosppy-2.2.0/biosppy/signals/abp.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,14 +113,15 @@
     wrange=None,
     d1_th=0,
     d2_th=None,
 ):
     """Determine onsets of ABP pulses.
     Skips corrupted signal parts.
     Based on the approach by Zong *et al.* [Zong03]_.
+
     Parameters
     ----------
     signal : array
         Input filtered ABP signal.
     sampling_rate : int, float, optional
         Sampling frequency (Hz).
     sm_size : int, optional
@@ -137,14 +138,15 @@
         Defaults to 0.1
     d1_th : int, optional
         Smallest allowed difference between maxima and minima.
         Defaults to 0
     d2_th : int, optional
         Smallest allowed time between maxima and minima (seconds),
         Defaults to 0.15
+        
     Returns
     -------
     onsets : array
         Indices of ABP pulse onsets.
 
     References
     ----------
```

### Comparing `biosppy-2.1.2/biosppy/signals/acc.py` & `biosppy-2.2.0/biosppy/signals/acc.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,18 +113,16 @@
 
     return utils.ReturnTuple(args, names)
 
 
 def activity_index(signal=None, sampling_rate=100.0, window_1=5, window_2=60):
     """
     Compute the activity index of an ACC signal.
-
     Follows the method described in [Lin18]_, the activity index is computed as
     follows:
-    
     1) Calculate the ACC magnitude if the signal is triaxial
     2) Calculate the standard deviation of the ACC magnitude for each
     'window_1' seconds
     3) The activity index will be the mean standard deviation for each
     'window_2' seconds
     
     Parameters
```

### Comparing `biosppy-2.1.2/biosppy/signals/bvp.py` & `biosppy-2.2.0/biosppy/signals/bvp.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.1.2/biosppy/signals/ecg.py` & `biosppy-2.2.0/biosppy/signals/ecg.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.1.2/biosppy/signals/eda.py` & `biosppy-2.2.0/biosppy/signals/eda.py`

 * *Files 1% similar despite different names*

```diff
@@ -292,17 +292,17 @@
 
     return utils.ReturnTuple(args, names)
 
 
 def cvx_decomposition(signal=None, sampling_rate=1000.0, tau0=2., tau1=0.7,
                       delta_knot=10., alpha=8e-4, gamma=1e-2, solver=None,
                       options={'reltol': 1e-9}):
-    """Performs EDA decomposition using the cvxEDA algorithm.
+    """Performs EDA decomposition using the cvxEDA algorithm [Figner2011]_.
 
-    This function was originally developed by Luca Citi and Alberto Greco. You
+    This function was originally developed by Luca Citi and Alberto Greco [cvxEDA]_. You
     can find the original code and repository at:
     https://github.com/lciti/cvxEDA
 
     If you use this function in your work, please cite the original authors
     as follows: A Greco, G Valenza, A Lanata, EP Scilingo, and L Citi
     "cvxEDA: a Convex Optimization Approach to Electrodermal Activity
     Processing" IEEE Transactions on Biomedical Engineering, 2015.
```

### Comparing `biosppy-2.1.2/biosppy/signals/eeg.py` & `biosppy-2.2.0/biosppy/signals/eeg.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.1.2/biosppy/signals/emg.py` & `biosppy-2.2.0/biosppy/signals/emg.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.1.2/biosppy/signals/hrv.py` & `biosppy-2.2.0/biosppy/signals/hrv.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.1.2/biosppy/signals/pcg.py` & `biosppy-2.2.0/biosppy/signals/pcg.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.1.2/biosppy/signals/ppg.py` & `biosppy-2.2.0/biosppy/signals/ppg.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.1.2/biosppy/signals/resp.py` & `biosppy-2.2.0/biosppy/signals/resp.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.1.2/biosppy/signals/tools.py` & `biosppy-2.2.0/biosppy/signals/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from six.moves import range
 import six
 
 # 3rd party
 import sys
 import numpy as np
 import scipy.signal as ss
+from scipy.signal import windows as ssw
 from scipy import interpolate, optimize
 from scipy.stats import stats
 from scipy.sparse import spdiags, eye, csr_matrix
 
 
 # local
 from .. import utils
@@ -187,57 +188,57 @@
     Returns
     -------
     window : array
         Created window.
 
     """
 
-    # mimics scipy.signal.get_window
+    # mimics scipy.signal.windows.get_window
     if kernel in ["blackman", "black", "blk"]:
-        winfunc = ss.blackman
+        winfunc = ssw.blackman
     elif kernel in ["triangle", "triang", "tri"]:
-        winfunc = ss.triang
+        winfunc = ssw.triang
     elif kernel in ["hamming", "hamm", "ham"]:
-        winfunc = ss.hamming
+        winfunc = ssw.hamming
     elif kernel in ["bartlett", "bart", "brt"]:
-        winfunc = ss.bartlett
+        winfunc = ssw.bartlett
     elif kernel in ["hanning", "hann", "han"]:
-        winfunc = ss.hann
+        winfunc = ssw.hann
     elif kernel in ["blackmanharris", "blackharr", "bkh"]:
-        winfunc = ss.blackmanharris
+        winfunc = ssw.blackmanharris
     elif kernel in ["parzen", "parz", "par"]:
-        winfunc = ss.parzen
+        winfunc = ssw.parzen
     elif kernel in ["bohman", "bman", "bmn"]:
-        winfunc = ss.bohman
+        winfunc = ssw.bohman
     elif kernel in ["nuttall", "nutl", "nut"]:
-        winfunc = ss.nuttall
+        winfunc = ssw.nuttall
     elif kernel in ["barthann", "brthan", "bth"]:
-        winfunc = ss.barthann
+        winfunc = ssw.barthann
     elif kernel in ["flattop", "flat", "flt"]:
-        winfunc = ss.flattop
+        winfunc = ssw.flattop
     elif kernel in ["kaiser", "ksr"]:
-        winfunc = ss.kaiser
+        winfunc = ssw.kaiser
     elif kernel in ["gaussian", "gauss", "gss"]:
-        winfunc = ss.gaussian
+        winfunc = ssw.gaussian
     elif kernel in [
         "general gaussian",
         "general_gaussian",
         "general gauss",
         "general_gauss",
         "ggs",
     ]:
-        winfunc = ss.general_gaussian
+        winfunc = ssw.general_gaussian
     elif kernel in ["boxcar", "box", "ones", "rect", "rectangular"]:
-        winfunc = ss.boxcar
+        winfunc = ssw.boxcar
     elif kernel in ["slepian", "slep", "optimal", "dpss", "dss"]:
-        winfunc = ss.slepian
+        winfunc = ssw.dpss
     elif kernel in ["cosine", "halfcosine"]:
-        winfunc = ss.cosine
+        winfunc = ssw.cosine
     elif kernel in ["chebwin", "cheb"]:
-        winfunc = ss.chebwin
+        winfunc = ssw.chebwin
     else:
         raise ValueError("Unknown window type.")
 
     try:
         window = winfunc(size, **kwargs)
     except TypeError as e:
         raise TypeError("Invalid window arguments: %s." % e)
```

### Comparing `biosppy-2.1.2/biosppy/stats.py` & `biosppy-2.2.0/biosppy/stats.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.1.2/biosppy/storage.py` & `biosppy-2.2.0/biosppy/storage.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.1.2/biosppy/synthesizers/ecg.py` & `biosppy-2.2.0/biosppy/synthesizers/ecg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-biosppy.signals.ecg
+biosppy.synthesizers.ecg
 -------------------
 
 This module provides methods to synthesize Electrocardiographic (ECG) signals.
 
 :copyright: (c) 2015-2021 by Instituto de Telecomunicacoes
 :license: BSD 3-clause, see LICENSE for more details.
 
@@ -23,15 +23,15 @@
 from biosppy.signals import tools as st
 from .. import plotting, utils
 
 
 def B(l, Kb):
     """Generates the amplitude values of the first isoelectric line (B segment) of the ECG signal.
 
-    Follows the approach by Dolinský, Andráš, Michaeli and Grimaldi [Model03].
+    Follows the approach by Dolinský, Andráš, Michaeli and Grimaldi [Model03]_.
 
     If the parameter introduced doesn't make sense in this context, an error will raise.
     Parameters
     ----------
     l  : float
         Inverse of the sampling rate.
     Kb : int
@@ -54,15 +54,15 @@
         B_segment = a.tolist()
     return B_segment
 
 
 def P(i, Ap, Kp):
     """Generates the amplitude values of the P wave in the ECG signal.
 
-    Follows the approach by Dolinský, Andráš, Michaeli and Grimaldi [Model03].
+    Follows the approach by Dolinský, Andráš, Michaeli and Grimaldi [Model03]_.
 
     If the parameters introduced don't make sense in this context, an error will raise.
     Parameters
     ----------
     i  : int
         Sampling rate.
     Ap : int
@@ -90,15 +90,15 @@
         P_wave = a.tolist()
     return P_wave
 
 
 def Pq(l, Kpq):
     """Generates the amplitude values of the PQ segment in the ECG signal.
 
-    Follows the approach by Dolinský, Andráš, Michaeli and Grimaldi [Model03].
+    Follows the approach by Dolinský, Andráš, Michaeli and Grimaldi [Model03]_.
 
     If the parameters introduced don't make sense in this context, an error will raise.
     Parameters
     ----------
     l  : float
         Inverse of the sampling rate.
     Kpq : int
@@ -121,15 +121,15 @@
         PQ_segment = a.tolist()
     return PQ_segment
 
 
 def Q1(i, Aq, Kq1):
     """Generates the amplitude values of the first 5/6 of the Q wave in the ECG signal.
 
-    Follows the approach by Dolinský, Andráš, Michaeli and Grimaldi [Model03].
+    Follows the approach by Dolinský, Andráš, Michaeli and Grimaldi [Model03]_.
 
     If the parameters introduced don't make sense in this context, an error will raise.
     Parameters
     ----------
     i   : int
         Sampling rate.
     Aq  : int
@@ -157,15 +157,15 @@
         Q1_wave = a.tolist()
     return Q1_wave
 
 
 def Q2(i, Aq, Kq2):
     """Generates the amplitude values of the last 1/6 of the Q wave in the ECG signal.
 
-    Follows the approach by Dolinský, Andráš, Michaeli and Grimaldi [Model03].
+    Follows the approach by Dolinský, Andráš, Michaeli and Grimaldi [Model03]_.
 
     If the parameters introduced don't make sense in this context, an error will raise.
     Parameters
     ----------
     i   : int
         Sampling rate.
     Aq  : int
@@ -193,15 +193,15 @@
         Q2_wave = a.tolist()
     return Q2_wave
 
 
 def R(i, Ar, Kr):
     """Generates the amplitude values of the R wave in the ECG signal.
 
-    Follows the approach by Dolinský, Andráš, Michaeli and Grimaldi [Model03].
+    Follows the approach by Dolinský, Andráš, Michaeli and Grimaldi [Model03]_.
 
     If the parameters introduced don't make sense in this context, an error will raise.
     Parameters
     ----------
     i  : int
         Sampling rate.
     Ar : int
@@ -229,15 +229,15 @@
         R_wave = a.tolist()
     return R_wave
 
 
 def S(i, As, Ks, Kcs, k=0):
     """Generates the amplitude values of the S wave in the ECG signal.
 
-    Follows the approach by Dolinský, Andráš, Michaeli and Grimaldi [Model03].
+    Follows the approach by Dolinský, Andráš, Michaeli and Grimaldi [Model03]_.
 
     If the parameters introduced don't make sense in this context, an error will raise.
     Parameters
     ----------
     i  : int
         Sampling rate.
     As : int
@@ -289,15 +289,15 @@
             )
     return S
 
 
 def St(i, As, Ks, Kcs, sm, Kst, k=0):
     """Generates the amplitude values of the ST segment in the ECG signal.
 
-    Follows the approach by Dolinský, Andráš, Michaeli and Grimaldi [Model03].
+    Follows the approach by Dolinský, Andráš, Michaeli and Grimaldi [Model03]_.
 
     If the parameters introduced don't make sense in this context, an error will raise.
     Parameters
     ----------
     i  : int
         Sampling rate.
     As : int
@@ -337,15 +337,15 @@
             ST = -S(i, As, Ks, Kcs, Ks - Kcs) * (k / sm) + S(i, As, Ks, Kcs, Ks - Kcs)
     return ST
 
 
 def T(i, As, Ks, Kcs, sm, Kst, At, Kt, k=0):
     """Generates the amplitude values of the T wave in the ECG signal.
 
-    Follows the approach by Dolinský, Andráš, Michaeli and Grimaldi [Model03].
+    Follows the approach by Dolinský, Andráš, Michaeli and Grimaldi [Model03]_.
 
     If the parameters introduced don't make sense in this context, an error will raise.
     Parameters
     ----------
     i  : int
         Sampling rate.
     As : int
@@ -397,15 +397,15 @@
             )
     return T
 
 
 def I(i, As, Ks, Kcs, sm, Kst, At, Kt, si, Ki):
     """Generates the amplitude values of the final isoelectric segment (I segment) in the ECG signal.
 
-    Follows the approach by Dolinský, Andráš, Michaeli and Grimaldi [Model03].
+    Follows the approach by Dolinský, Andráš, Michaeli and Grimaldi [Model03]_.
 
     If the parameters introduced don't make sense in this context, an error will raise.
     Parameters
     ----------
     i  : int
         Sampling rate.
     As : int
@@ -466,15 +466,15 @@
     si=2,
     Ki=200,
     var=0.01,
     sampling_rate=10000,
 ):  # normal values by default
     """Concatenates the segments and waves to make an ECG signal. The default values are physiological.
 
-    Follows the approach by Dolinský, Andráš, Michaeli and Grimaldi [Model03].
+    Follows the approach by Dolinský, Andráš, Michaeli and Grimaldi [Model03]_.
 
     If the parameters introduced aren't within physiological values (limits based on the website [ECGwaves]), a warning will raise.
 
     Parameters
     ----------
     Kb : int, optional
         B segment width (miliseconds).
```

### Comparing `biosppy-2.1.2/biosppy/timing.py` & `biosppy-2.2.0/biosppy/timing.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.1.2/biosppy/utils.py` & `biosppy-2.2.0/biosppy/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,17 +117,17 @@
     Parameters
     ----------
     top : str, optional
         Starting directory; if None, defaults to the current working directoty.
     spec : str, optional
         Regular expression to match the desired files;
         if None, matches all files; typical patterns:
-            * `r'\.txt$'` - matches files with '.txt' extension;
-            * `r'^File_'` - matches files starting with 'File\_'
-            * `r'^File_.+\.txt$'` - matches files starting with 'File\_' and ending with the '.txt' extension.
+        * `r'\.txt$'` - matches files with '.txt' extension;
+        * `r'^File_'` - matches files starting with 'File\_'
+        * `r'^File_.+\.txt$'` - matches files starting with 'File\_' and ending with the '.txt' extension.
 
     Yields
     ------
     fpath : str
         Absolute file path.
 
     Notes
```

### Comparing `biosppy-2.1.2/biosppy.egg-info/PKG-INFO` & `biosppy-2.2.0/biosppy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biosppy
-Version: 2.1.2
+Version: 2.2.0
 Summary: A toolbox for biosignal processing written in Python.
 Home-page: https://github.com/scientisst/BioSPPy
 Author: Instituto de Telecomunicacoes
 Author-email: developer@scientisst.com
 License: BSD 3-clause
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -29,44 +29,39 @@
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
 Requires-Dist: shortuuid
 Requires-Dist: six
 Requires-Dist: joblib
 Requires-Dist: opencv-python
 Requires-Dist: pywavelets
+Requires-Dist: mock
 Provides-Extra: eda
 Requires-Dist: cvxopt; extra == "eda"
 
 
+### 🎙️ Announcements
+#### Latest
 ```
 🌀 New module for signal quality assessment 🌀
-With the signals.quality module you can now evaluate the quality of your signals!
+With the biosppy.quality module you can now evaluate the quality of your signals!
 So far, the EDA and ECG quality are available, but more could be added soon. 
 ```
-
-```
-🫀 New module for heart rate variability 🫀
-With the signals.hrv module you can now extract HRV features. Check it out! (PR #19)
-```
-```
-✨ New plotting design ✨
-New colors, new style and new features, check it out!
-```
+#### New features
 ```
-🎊 New module for feature extraction 🎊
-With the 'features' module you can easily extract features from your biosignals!
-(Check PR #4)
+🌀 New module for signal quality assessment (biosppy.quality)
+🫀 New module for heart rate variability (biosppy.signals.hrv)
+🎊 New module for feature extraction (biosppy.features)
 ```
 
 
 # BioSPPy - Biosignal Processing in Python
 
 *A toolbox for biosignal processing written in Python.*
 
-<a href="http://biosppy.readthedocs.org/">
+<a href="https://biosppy.readthedocs.org/">
 <picture>
   <source media="(prefers-color-scheme: light)" srcset="docs/logo/logo_400.png">
   <source media="(prefers-color-scheme: dark)" srcset="docs/logo/logo_inverted_400.png">
   <img alt="Image" title="I know you're listening! - xkcd.com/525">
 </picture>
 </a>
 
@@ -76,15 +71,15 @@
 Highlights:
 
 - Support for various biosignals: BVP, ECG, EDA, EEG, EMG, PCG, PPG, Respiration
 - Signal analysis primitives: filtering, frequency analysis
 - Clustering
 - Biometrics
 
-Documentation can be found at: <http://biosppy.readthedocs.org/>
+Documentation can be found at: <https://biosppy.readthedocs.org/>
 
 ## Installation
 
 Installation can be easily done with `pip`:
 
 ```bash
 $ pip install biosppy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: biosppy Version: 2.1.2 Summary: A toolbox for
+Metadata-Version: 2.1 Name: biosppy Version: 2.2.0 Summary: A toolbox for
 biosignal processing written in Python. Home-page: https://github.com/
 scientisst/BioSPPy Author: Instituto de Telecomunicacoes Author-email:
 developer@scientisst.com License: BSD 3-clause Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: BSD License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
@@ -10,29 +10,28 @@
 Python :: 3.6 Classifier: Programming Language :: Python :: Implementation ::
 CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent Requires-Python: >3.5.2
 Description-Content-Type: text/markdown License-File: LICENSE License-File:
 AUTHORS.md Requires-Dist: bidict Requires-Dist: h5py Requires-Dist: matplotlib
 Requires-Dist: numpy Requires-Dist: scikit-learn Requires-Dist: scipy Requires-
 Dist: shortuuid Requires-Dist: six Requires-Dist: joblib Requires-Dist: opencv-
-python Requires-Dist: pywavelets Provides-Extra: eda Requires-Dist: cvxopt;
-extra == "eda" ``` ð New module for signal quality assessment ð With the
-signals.quality module you can now evaluate the quality of your signals! So
-far, the EDA and ECG quality are available, but more could be added soon. ```
-``` ð« New module for heart rate variability ð« With the signals.hrv module
-you can now extract HRV features. Check it out! (PR #19) ``` ``` â¨ New
-plotting design â¨ New colors, new style and new features, check it out! ```
-``` ð New module for feature extraction ð With the 'features' module you
-can easily extract features from your biosignals! (Check PR #4) ``` # BioSPPy -
-Biosignal Processing in Python *A toolbox for biosignal processing written in
-Python.* _[_I_m_a_g_e_]The toolbox bundles together various signal processing and
-pattern recognition methods geared towards the analysis of biosignals.
-Highlights: - Support for various biosignals: BVP, ECG, EDA, EEG, EMG, PCG,
-PPG, Respiration - Signal analysis primitives: filtering, frequency analysis -
-Clustering - Biometrics Documentation can be found at:
+python Requires-Dist: pywavelets Requires-Dist: mock Provides-Extra: eda
+Requires-Dist: cvxopt; extra == "eda" ### ðï¸ Announcements #### Latest ```
+ð New module for signal quality assessment ð With the biosppy.quality
+module you can now evaluate the quality of your signals! So far, the EDA and
+ECG quality are available, but more could be added soon. ``` #### New features
+``` ð New module for signal quality assessment (biosppy.quality) ð« New
+module for heart rate variability (biosppy.signals.hrv) ð New module for
+feature extraction (biosppy.features) ``` # BioSPPy - Biosignal Processing in
+Python *A toolbox for biosignal processing written in Python.* _[_I_m_a_g_e_]The
+toolbox bundles together various signal processing and pattern recognition
+methods geared towards the analysis of biosignals. Highlights: - Support for
+various biosignals: BVP, ECG, EDA, EEG, EMG, PCG, PPG, Respiration - Signal
+analysis primitives: filtering, frequency analysis - Clustering - Biometrics
+Documentation can be found at:
 biosppy.readthedocs.org/> ## Installation Installation can be easily done with
 `pip`: ```bash $ pip install biosppy ``` Alternatively, you can install the
 latest version from the GitHub repository: ```bash $ pip install git+https://
 github.com/scientisst/BioSPPy.git ``` ## Simple Example The code below loads an
 ECG signal from the `examples` folder, filters it, performs R-peak detection,
 and computes the instantaneous heart rate. ```python from biosppy import
 storage from biosppy.signals import ecg # load raw ECG signal signal, mdata =
```

### Comparing `biosppy-2.1.2/biosppy.egg-info/SOURCES.txt` & `biosppy-2.2.0/biosppy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -39,8 +39,9 @@
 biosppy/signals/emg.py
 biosppy/signals/hrv.py
 biosppy/signals/pcg.py
 biosppy/signals/ppg.py
 biosppy/signals/resp.py
 biosppy/signals/tools.py
 biosppy/synthesizers/__init__.py
-biosppy/synthesizers/ecg.py
+biosppy/synthesizers/ecg.py
+biosppy/synthesizers/emg.py
```

### Comparing `biosppy-2.1.2/setup.py` & `biosppy-2.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,28 +12,26 @@
 
 # Note: To use the 'upload' functionality of this file, you must:
 #   $ pip install twine
 
 import io
 import os
 import sys
-import re
-import ast
 from shutil import rmtree
 
 from setuptools import find_packages, setup, Command
 
 # Package meta-data.
 NAME = 'biosppy'
 DESCRIPTION = 'A toolbox for biosignal processing written in Python.'
 URL = 'https://github.com/scientisst/BioSPPy'
 EMAIL = 'developer@scientisst.com'
 AUTHOR = 'Instituto de Telecomunicacoes'
 REQUIRES_PYTHON = '>3.5.2'
-VERSION = '2.1.2'
+VERSION = '2.2.0'
 LICENSE = 'BSD 3-clause'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'bidict',
     'h5py',
     'matplotlib',
@@ -41,14 +39,15 @@
     'scikit-learn',
     'scipy',
     'shortuuid',
     'six',
     'joblib',
     'opencv-python',
     'pywavelets',
+    'mock',
 ]
 
 # What packages are optional?
 EXTRAS = {
     'eda': ['cvxopt'],
     # 'fancy feature': ['django'],
 }
```

