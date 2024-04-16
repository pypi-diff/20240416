# Comparing `tmp/starsim-0.3.2.tar.gz` & `tmp/starsim-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starsim-0.3.2.tar", last modified: Fri Apr 12 07:22:13 2024, max compression
+gzip compressed data, was "starsim-0.3.3.tar", last modified: Tue Apr 16 13:12:03 2024, max compression
```

## Comparing `starsim-0.3.2.tar` & `starsim-0.3.3.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-12 07:22:13.627713 starsim-0.3.2/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1088 2024-03-30 07:25:13.000000 starsim-0.3.2/LICENSE
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3610 2024-04-12 07:22:13.627713 starsim-0.3.2/PKG-INFO
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2705 2024-03-30 07:25:13.000000 starsim-0.3.2/README.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       38 2024-04-12 07:22:13.627713 starsim-0.3.2/setup.cfg
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1619 2024-04-03 13:56:26.000000 starsim-0.3.2/setup.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-12 07:22:13.623713 starsim-0.3.2/starsim/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1046 2024-04-03 13:56:26.000000 starsim-0.3.2/starsim/__init__.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1191 2024-04-02 03:48:00.000000 starsim-0.3.2/starsim/connectors.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    19926 2024-04-05 21:02:35.000000 starsim-0.3.2/starsim/demographics.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    16370 2024-04-06 16:25:59.000000 starsim-0.3.2/starsim/disease.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-12 07:22:13.627713 starsim-0.3.2/starsim/diseases/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      285 2024-04-02 03:48:03.000000 starsim-0.3.2/starsim/diseases/__init__.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     9033 2024-04-11 11:28:46.000000 starsim-0.3.2/starsim/diseases/cholera.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5876 2024-04-11 11:28:46.000000 starsim-0.3.2/starsim/diseases/ebola.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3385 2024-04-05 21:02:35.000000 starsim-0.3.2/starsim/diseases/gonorrhea.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     4668 2024-04-05 21:02:35.000000 starsim-0.3.2/starsim/diseases/hiv.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3283 2024-04-11 11:28:46.000000 starsim-0.3.2/starsim/diseases/measles.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3423 2024-04-03 13:56:26.000000 starsim-0.3.2/starsim/diseases/ncd.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5895 2024-04-11 11:28:46.000000 starsim-0.3.2/starsim/diseases/sir.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    14752 2024-04-11 11:28:46.000000 starsim-0.3.2/starsim/diseases/syphilis.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    28830 2024-04-03 14:06:30.000000 starsim-0.3.2/starsim/distributions.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    22027 2024-04-03 13:56:26.000000 starsim-0.3.2/starsim/interventions.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     6672 2024-04-03 13:56:26.000000 starsim-0.3.2/starsim/modules.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    42277 2024-04-06 16:25:59.000000 starsim-0.3.2/starsim/network.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3979 2024-04-02 04:22:31.000000 starsim-0.3.2/starsim/parameters.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    15132 2024-04-12 07:22:08.000000 starsim-0.3.2/starsim/people.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5869 2024-04-03 13:56:26.000000 starsim-0.3.2/starsim/products.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2080 2024-04-03 13:56:26.000000 starsim-0.3.2/starsim/results.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    15347 2024-04-02 03:48:00.000000 starsim-0.3.2/starsim/run.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    13972 2024-04-02 03:48:00.000000 starsim-0.3.2/starsim/samples.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     7608 2024-04-03 13:56:26.000000 starsim-0.3.2/starsim/settings.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    45922 2024-04-03 13:56:26.000000 starsim-0.3.2/starsim/sim.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    24451 2024-04-12 07:22:08.000000 starsim-0.3.2/starsim/states.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    13010 2024-04-03 13:56:26.000000 starsim-0.3.2/starsim/utils.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      239 2024-04-11 11:28:46.000000 starsim-0.3.2/starsim/version.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-12 07:22:13.627713 starsim-0.3.2/starsim.egg-info/
--rw-r--r--   0 cliffk    (1000) cliffk    (1000)     3610 2024-04-12 07:22:13.000000 starsim-0.3.2/starsim.egg-info/PKG-INFO
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1014 2024-04-12 07:22:13.000000 starsim-0.3.2/starsim.egg-info/SOURCES.txt
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)        1 2024-04-12 07:22:13.000000 starsim-0.3.2/starsim.egg-info/dependency_links.txt
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       66 2024-04-12 07:22:13.000000 starsim-0.3.2/starsim.egg-info/requires.txt
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)        8 2024-04-12 07:22:13.000000 starsim-0.3.2/starsim.egg-info/top_level.txt
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-12 07:22:13.627713 starsim-0.3.2/tests/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3550 2024-04-03 13:56:26.000000 starsim-0.3.2/tests/test_base.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5666 2024-04-03 13:56:26.000000 starsim-0.3.2/tests/test_baselines.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      973 2024-04-03 13:56:26.000000 starsim-0.3.2/tests/test_dcp.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5702 2024-04-03 13:56:26.000000 starsim-0.3.2/tests/test_demographics.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3274 2024-04-03 13:56:26.000000 starsim-0.3.2/tests/test_diseases.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     7721 2024-04-03 13:56:26.000000 starsim-0.3.2/tests/test_dist.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5914 2024-04-03 13:56:26.000000 starsim-0.3.2/tests/test_dists.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1420 2024-04-03 13:56:26.000000 starsim-0.3.2/tests/test_samples.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5576 2024-04-03 13:56:26.000000 starsim-0.3.2/tests/test_simple.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     6159 2024-04-03 13:56:26.000000 starsim-0.3.2/tests/test_syphilis.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-16 13:12:03.485074 starsim-0.3.3/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1088 2024-03-30 07:25:13.000000 starsim-0.3.3/LICENSE
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3610 2024-04-16 13:12:03.485074 starsim-0.3.3/PKG-INFO
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2705 2024-03-30 07:25:13.000000 starsim-0.3.3/README.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       38 2024-04-16 13:12:03.485074 starsim-0.3.3/setup.cfg
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1619 2024-04-03 13:56:26.000000 starsim-0.3.3/setup.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-16 13:12:03.481074 starsim-0.3.3/starsim/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1046 2024-04-13 20:12:05.000000 starsim-0.3.3/starsim/__init__.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1191 2024-04-13 20:12:05.000000 starsim-0.3.3/starsim/connectors.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       37 2024-04-13 20:12:05.000000 starsim-0.3.3/starsim/demo.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    19926 2024-04-16 12:35:49.000000 starsim-0.3.3/starsim/demographics.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    16370 2024-04-16 12:35:49.000000 starsim-0.3.3/starsim/disease.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-16 13:12:03.481074 starsim-0.3.3/starsim/diseases/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      285 2024-04-13 20:12:07.000000 starsim-0.3.3/starsim/diseases/__init__.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     9033 2024-04-16 12:35:49.000000 starsim-0.3.3/starsim/diseases/cholera.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5839 2024-04-16 13:06:22.000000 starsim-0.3.3/starsim/diseases/ebola.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3385 2024-04-16 12:35:49.000000 starsim-0.3.3/starsim/diseases/gonorrhea.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     4668 2024-04-16 12:35:49.000000 starsim-0.3.3/starsim/diseases/hiv.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3283 2024-04-16 12:35:49.000000 starsim-0.3.3/starsim/diseases/measles.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3423 2024-04-16 12:35:49.000000 starsim-0.3.3/starsim/diseases/ncd.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5895 2024-04-16 12:35:49.000000 starsim-0.3.3/starsim/diseases/sir.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    14752 2024-04-16 12:35:49.000000 starsim-0.3.3/starsim/diseases/syphilis.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    28830 2024-04-13 20:12:05.000000 starsim-0.3.3/starsim/distributions.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    22027 2024-04-16 12:35:49.000000 starsim-0.3.3/starsim/interventions.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     6688 2024-04-16 13:02:13.000000 starsim-0.3.3/starsim/modules.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    42277 2024-04-16 12:35:49.000000 starsim-0.3.3/starsim/network.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3979 2024-04-16 12:35:49.000000 starsim-0.3.3/starsim/parameters.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    15132 2024-04-16 12:35:49.000000 starsim-0.3.3/starsim/people.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5869 2024-04-16 12:35:49.000000 starsim-0.3.3/starsim/products.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2080 2024-04-13 20:12:05.000000 starsim-0.3.3/starsim/results.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    15347 2024-04-13 20:12:05.000000 starsim-0.3.3/starsim/run.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    13972 2024-04-13 20:12:05.000000 starsim-0.3.3/starsim/samples.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     7608 2024-04-16 12:35:49.000000 starsim-0.3.3/starsim/settings.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    45922 2024-04-16 12:35:49.000000 starsim-0.3.3/starsim/sim.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    24451 2024-04-16 12:35:49.000000 starsim-0.3.3/starsim/states.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    13010 2024-04-16 12:35:49.000000 starsim-0.3.3/starsim/utils.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      239 2024-04-16 13:07:40.000000 starsim-0.3.3/starsim/version.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-16 13:12:03.481074 starsim-0.3.3/starsim.egg-info/
+-rw-r--r--   0 cliffk    (1000) cliffk    (1000)     3610 2024-04-16 13:12:03.000000 starsim-0.3.3/starsim.egg-info/PKG-INFO
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1030 2024-04-16 13:12:03.000000 starsim-0.3.3/starsim.egg-info/SOURCES.txt
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)        1 2024-04-16 13:12:03.000000 starsim-0.3.3/starsim.egg-info/dependency_links.txt
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       66 2024-04-16 13:12:03.000000 starsim-0.3.3/starsim.egg-info/requires.txt
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)        8 2024-04-16 13:12:03.000000 starsim-0.3.3/starsim.egg-info/top_level.txt
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-16 13:12:03.481074 starsim-0.3.3/tests/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3550 2024-04-16 12:35:49.000000 starsim-0.3.3/tests/test_base.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5666 2024-04-13 20:12:03.000000 starsim-0.3.3/tests/test_baselines.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      973 2024-04-13 20:12:03.000000 starsim-0.3.3/tests/test_dcp.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5702 2024-04-13 20:12:03.000000 starsim-0.3.3/tests/test_demographics.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3274 2024-04-13 20:12:03.000000 starsim-0.3.3/tests/test_diseases.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     7721 2024-04-13 20:12:03.000000 starsim-0.3.3/tests/test_dist.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5914 2024-04-13 20:12:03.000000 starsim-0.3.3/tests/test_dists.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1420 2024-04-13 20:12:03.000000 starsim-0.3.3/tests/test_samples.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5576 2024-04-13 20:12:03.000000 starsim-0.3.3/tests/test_simple.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     6159 2024-04-13 20:12:03.000000 starsim-0.3.3/tests/test_syphilis.py
```

### Comparing `starsim-0.3.2/LICENSE` & `starsim-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `starsim-0.3.2/PKG-INFO` & `starsim-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starsim
-Version: 0.3.2
+Version: 0.3.3
 Summary: Starsim
 Author: Robyn Stuart, Cliff Kerr, Romesh Abeysuriya, Paula Sanz-Leon, Jamie Cohen, and Daniel Klein on behalf of the Starsim Collective
 Keywords: agent-based model,simulation,disease,epidemiology
 Platform: OS Independent
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
```

### Comparing `starsim-0.3.2/README.rst` & `starsim-0.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `starsim-0.3.2/setup.py` & `starsim-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.2/starsim/__init__.py` & `starsim-0.3.3/starsim/__init__.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.2/starsim/connectors.py` & `starsim-0.3.3/starsim/connectors.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.2/starsim/demographics.py` & `starsim-0.3.3/starsim/demographics.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.2/starsim/disease.py` & `starsim-0.3.3/starsim/disease.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.2/starsim/diseases/cholera.py` & `starsim-0.3.3/starsim/diseases/cholera.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.2/starsim/diseases/ebola.py` & `starsim-0.3.3/starsim/diseases/ebola.py`

 * *Files 3% similar despite different names*

```diff
@@ -133,24 +133,20 @@
 
         # Determine time of burial - either immediate (safe burials) or after a delay (unsafe)
         safe_buried = p.p_safe_bury.filter(dead_uids)
         unsafe_buried = np.setdiff1d(dead_uids, safe_buried)
         self.ti_buried[safe_buried] = self.ti_dead[safe_buried]
         self.ti_buried[unsafe_buried] = self.ti_dead[unsafe_buried] + p.dur_dead2buried.rvs(unsafe_buried) / sim.dt
 
+        # Change rel_trans values
+        self.rel_trans[self.infectious] = 1
+        self.rel_trans[self.severe] = self.pars['sev_factor']  # Change for severe
+        unburied_uids = ss.true((self.ti_dead <= sim.ti) & (self.ti_buried > sim.ti))
+        self.rel_trans[unburied_uids] = self.pars['unburied_factor']  # Change for unburied
+
         return
 
     def update_death(self, sim, uids):
         # Reset infected/recovered flags for dead agents
         for state in ['susceptible', 'exposed', 'infected', 'severe', 'recovered']:
             self.statesdict[state][uids] = False
         return
-
-    def make_new_cases(self, sim):
-        self.rel_trans[self.infectious] = 1
-        self.rel_trans[self.severe] = self.pars['sev_factor']
-
-        # Unburied UIDs
-        unburied_uids = ss.true((self.ti_dead <= sim.ti) & (self.ti_buried > sim.ti))
-        self.rel_trans[unburied_uids] = self.pars['unburied_factor']
-        super().make_new_cases(sim)
-        return
```

### Comparing `starsim-0.3.2/starsim/diseases/gonorrhea.py` & `starsim-0.3.3/starsim/diseases/gonorrhea.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.2/starsim/diseases/hiv.py` & `starsim-0.3.3/starsim/diseases/hiv.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.2/starsim/diseases/measles.py` & `starsim-0.3.3/starsim/diseases/measles.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.2/starsim/diseases/ncd.py` & `starsim-0.3.3/starsim/diseases/ncd.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.2/starsim/diseases/sir.py` & `starsim-0.3.3/starsim/diseases/sir.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.2/starsim/diseases/syphilis.py` & `starsim-0.3.3/starsim/diseases/syphilis.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.2/starsim/distributions.py` & `starsim-0.3.3/starsim/distributions.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.2/starsim/interventions.py` & `starsim-0.3.3/starsim/interventions.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.2/starsim/modules.py` & `starsim-0.3.3/starsim/modules.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 
 class Module(sc.quickobj):
 
     def __init__(self, pars=None, par_dists=None, name=None, label=None, requires=None, **kwargs):
         self.pars = ss.omerge(pars, kwargs)
         self.par_dists = ss.omerge(par_dists)
-        self.name = name if (name is not None) else self.__class__.__name__.lower() # Default name is the class name
-        self.label = label if (label is not None) else self.name
+        self.name = sc.ifelse(name, getattr(self, 'name', self.__class__.__name__.lower())) # Default name is the class name
+        self.label = sc.ifelse(label, getattr(self, 'label', self.name))
         self.requires = sc.mergelists(requires)
         self.results = ss.Results(self.name)
         self.initialized = False
         self.finalized = False
         return
     
     def disp(self, output=False):
```

### Comparing `starsim-0.3.2/starsim/network.py` & `starsim-0.3.3/starsim/network.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.2/starsim/parameters.py` & `starsim-0.3.3/starsim/parameters.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.2/starsim/people.py` & `starsim-0.3.3/starsim/people.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.2/starsim/products.py` & `starsim-0.3.3/starsim/products.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.2/starsim/results.py` & `starsim-0.3.3/starsim/results.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.2/starsim/run.py` & `starsim-0.3.3/starsim/run.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.2/starsim/samples.py` & `starsim-0.3.3/starsim/samples.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.2/starsim/settings.py` & `starsim-0.3.3/starsim/settings.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.2/starsim/sim.py` & `starsim-0.3.3/starsim/sim.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.2/starsim/states.py` & `starsim-0.3.3/starsim/states.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.2/starsim/utils.py` & `starsim-0.3.3/starsim/utils.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.2/starsim.egg-info/PKG-INFO` & `starsim-0.3.3/starsim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starsim
-Version: 0.3.2
+Version: 0.3.3
 Summary: Starsim
 Author: Robyn Stuart, Cliff Kerr, Romesh Abeysuriya, Paula Sanz-Leon, Jamie Cohen, and Daniel Klein on behalf of the Starsim Collective
 Keywords: agent-based model,simulation,disease,epidemiology
 Platform: OS Independent
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
```

### Comparing `starsim-0.3.2/starsim.egg-info/SOURCES.txt` & `starsim-0.3.3/starsim.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.rst
 setup.py
 starsim/__init__.py
 starsim/connectors.py
+starsim/demo.py
 starsim/demographics.py
 starsim/disease.py
 starsim/distributions.py
 starsim/interventions.py
 starsim/modules.py
 starsim/network.py
 starsim/parameters.py
```

### Comparing `starsim-0.3.2/tests/test_base.py` & `starsim-0.3.3/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.2/tests/test_baselines.py` & `starsim-0.3.3/tests/test_baselines.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.2/tests/test_dcp.py` & `starsim-0.3.3/tests/test_dcp.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.2/tests/test_demographics.py` & `starsim-0.3.3/tests/test_demographics.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.2/tests/test_diseases.py` & `starsim-0.3.3/tests/test_diseases.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.2/tests/test_dist.py` & `starsim-0.3.3/tests/test_dist.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.2/tests/test_dists.py` & `starsim-0.3.3/tests/test_dists.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.2/tests/test_samples.py` & `starsim-0.3.3/tests/test_samples.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.2/tests/test_simple.py` & `starsim-0.3.3/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `starsim-0.3.2/tests/test_syphilis.py` & `starsim-0.3.3/tests/test_syphilis.py`

 * *Files identical despite different names*

