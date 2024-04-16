# Comparing `tmp/scmopy-0.1.3.tar.gz` & `tmp/scmopy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scmopy-0.1.3.tar", last modified: Mon Apr 15 20:36:49 2024, max compression
+gzip compressed data, was "scmopy-0.1.4.tar", last modified: Mon Apr 15 20:59:51 2024, max compression
```

## Comparing `scmopy-0.1.3.tar` & `scmopy-0.1.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-15 20:36:49.119946 scmopy-0.1.3/
--rw-r--r--   0 soli      (1000) soli      (1000)     1077 2024-03-30 13:55:39.000000 scmopy-0.1.3/LICENSE
--rw-r--r--   0 soli      (1000) soli      (1000)       85 2024-04-14 17:50:35.000000 scmopy-0.1.3/MANIFEST.in
--rw-r--r--   0 soli      (1000) soli      (1000)    21327 2024-04-15 20:36:49.119946 scmopy-0.1.3/PKG-INFO
--rw-r--r--   0 soli      (1000) soli      (1000)    21011 2024-04-15 20:13:13.000000 scmopy-0.1.3/README.md
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-15 20:36:49.119946 scmopy-0.1.3/examples/
--rw-r--r--   0 soli      (1000) soli      (1000)   133028 2024-04-15 20:26:10.000000 scmopy-0.1.3/examples/ESA-2SCM_Example.ipynb
--rw-r--r--   0 soli      (1000) soli      (1000)        0 2024-04-14 19:31:15.000000 scmopy-0.1.3/examples/gngscm_placeholder.ipynb
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-15 20:36:49.119946 scmopy-0.1.3/scmopy/
--rw-r--r--   0 soli      (1000) soli      (1000)     1077 2024-03-30 10:40:19.000000 scmopy-0.1.3/scmopy/LICENSE
--rw-r--r--   0 soli      (1000) soli      (1000)      891 2024-04-15 20:36:07.000000 scmopy-0.1.3/scmopy/__init__.py
--rw-r--r--   0 soli      (1000) soli      (1000)     2036 2024-04-14 17:43:02.000000 scmopy-0.1.3/scmopy/base.py
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-15 20:36:49.119946 scmopy-0.1.3/scmopy/components/
--rw-r--r--   0 soli      (1000) soli      (1000)      905 2024-04-14 17:41:40.000000 scmopy-0.1.3/scmopy/components/__init__.py
--rw-r--r--   0 soli      (1000) soli      (1000)     5517 2024-04-14 17:42:11.000000 scmopy-0.1.3/scmopy/components/syniv.py
--rw-r--r--   0 soli      (1000) soli      (1000)     7089 2024-04-14 17:43:09.000000 scmopy-0.1.3/scmopy/gaussian_scm.py
--rw-r--r--   0 soli      (1000) soli      (1000)     5087 2024-04-15 20:14:24.000000 scmopy-0.1.3/scmopy/model_selection.py
--rw-r--r--   0 soli      (1000) soli      (1000)    14208 2024-04-15 20:16:14.000000 scmopy-0.1.3/scmopy/nongaussian_scm.py
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-15 20:36:49.119946 scmopy-0.1.3/scmopy.egg-info/
--rw-r--r--   0 soli      (1000) soli      (1000)    21327 2024-04-15 20:36:49.000000 scmopy-0.1.3/scmopy.egg-info/PKG-INFO
--rw-r--r--   0 soli      (1000) soli      (1000)      490 2024-04-15 20:36:49.000000 scmopy-0.1.3/scmopy.egg-info/SOURCES.txt
--rw-r--r--   0 soli      (1000) soli      (1000)        1 2024-04-15 20:36:49.000000 scmopy-0.1.3/scmopy.egg-info/dependency_links.txt
--rw-r--r--   0 soli      (1000) soli      (1000)       19 2024-04-15 20:36:49.000000 scmopy-0.1.3/scmopy.egg-info/requires.txt
--rw-r--r--   0 soli      (1000) soli      (1000)        7 2024-04-15 20:36:49.000000 scmopy-0.1.3/scmopy.egg-info/top_level.txt
--rw-r--r--   0 soli      (1000) soli      (1000)       38 2024-04-15 20:36:49.119946 scmopy-0.1.3/setup.cfg
--rw-r--r--   0 soli      (1000) soli      (1000)     1542 2024-04-15 20:36:08.000000 scmopy-0.1.3/setup.py
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-15 20:36:49.119946 scmopy-0.1.3/test/
--rw-r--r--   0 soli      (1000) soli      (1000)     2112 2024-04-15 20:26:41.000000 scmopy-0.1.3/test/test_ESA-2SCM_model.py
--rw-r--r--   0 soli      (1000) soli      (1000)     2630 2024-04-15 20:27:06.000000 scmopy-0.1.3/test/test_ESA-2SCM_syniv.py
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-15 20:59:51.415616 scmopy-0.1.4/
+-rw-r--r--   0 soli      (1000) soli      (1000)     1077 2024-03-30 13:55:39.000000 scmopy-0.1.4/LICENSE
+-rw-r--r--   0 soli      (1000) soli      (1000)       85 2024-04-14 17:50:35.000000 scmopy-0.1.4/MANIFEST.in
+-rw-r--r--   0 soli      (1000) soli      (1000)    21327 2024-04-15 20:59:51.415616 scmopy-0.1.4/PKG-INFO
+-rw-r--r--   0 soli      (1000) soli      (1000)    21011 2024-04-15 20:13:13.000000 scmopy-0.1.4/README.md
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-15 20:59:51.415616 scmopy-0.1.4/examples/
+-rw-r--r--   0 soli      (1000) soli      (1000)   133028 2024-04-15 20:26:10.000000 scmopy-0.1.4/examples/ESA-2SCM_Example.ipynb
+-rw-r--r--   0 soli      (1000) soli      (1000)        0 2024-04-14 19:31:15.000000 scmopy-0.1.4/examples/gngscm_placeholder.ipynb
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-15 20:59:51.415616 scmopy-0.1.4/scmopy/
+-rw-r--r--   0 soli      (1000) soli      (1000)     1077 2024-03-30 10:40:19.000000 scmopy-0.1.4/scmopy/LICENSE
+-rw-r--r--   0 soli      (1000) soli      (1000)      891 2024-04-15 20:59:18.000000 scmopy-0.1.4/scmopy/__init__.py
+-rw-r--r--   0 soli      (1000) soli      (1000)     2036 2024-04-14 17:43:02.000000 scmopy-0.1.4/scmopy/base.py
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-15 20:59:51.415616 scmopy-0.1.4/scmopy/components/
+-rw-r--r--   0 soli      (1000) soli      (1000)      905 2024-04-14 17:41:40.000000 scmopy-0.1.4/scmopy/components/__init__.py
+-rw-r--r--   0 soli      (1000) soli      (1000)     5517 2024-04-14 17:42:11.000000 scmopy-0.1.4/scmopy/components/syniv.py
+-rw-r--r--   0 soli      (1000) soli      (1000)     7089 2024-04-14 17:43:09.000000 scmopy-0.1.4/scmopy/gaussian_scm.py
+-rw-r--r--   0 soli      (1000) soli      (1000)     5087 2024-04-15 20:14:24.000000 scmopy-0.1.4/scmopy/model_selection.py
+-rw-r--r--   0 soli      (1000) soli      (1000)    14208 2024-04-15 20:57:05.000000 scmopy-0.1.4/scmopy/nongaussian_scm.py
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-15 20:59:51.415616 scmopy-0.1.4/scmopy.egg-info/
+-rw-r--r--   0 soli      (1000) soli      (1000)    21327 2024-04-15 20:59:51.000000 scmopy-0.1.4/scmopy.egg-info/PKG-INFO
+-rw-r--r--   0 soli      (1000) soli      (1000)      490 2024-04-15 20:59:51.000000 scmopy-0.1.4/scmopy.egg-info/SOURCES.txt
+-rw-r--r--   0 soli      (1000) soli      (1000)        1 2024-04-15 20:59:51.000000 scmopy-0.1.4/scmopy.egg-info/dependency_links.txt
+-rw-r--r--   0 soli      (1000) soli      (1000)       19 2024-04-15 20:59:51.000000 scmopy-0.1.4/scmopy.egg-info/requires.txt
+-rw-r--r--   0 soli      (1000) soli      (1000)        7 2024-04-15 20:59:51.000000 scmopy-0.1.4/scmopy.egg-info/top_level.txt
+-rw-r--r--   0 soli      (1000) soli      (1000)       38 2024-04-15 20:59:51.415616 scmopy-0.1.4/setup.cfg
+-rw-r--r--   0 soli      (1000) soli      (1000)     1542 2024-04-15 20:59:12.000000 scmopy-0.1.4/setup.py
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-15 20:59:51.415616 scmopy-0.1.4/test/
+-rw-r--r--   0 soli      (1000) soli      (1000)     2112 2024-04-15 20:26:41.000000 scmopy-0.1.4/test/test_ESA-2SCM_model.py
+-rw-r--r--   0 soli      (1000) soli      (1000)     2630 2024-04-15 20:27:06.000000 scmopy-0.1.4/test/test_ESA-2SCM_syniv.py
```

### Comparing `scmopy-0.1.3/LICENSE` & `scmopy-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scmopy-0.1.3/PKG-INFO` & `scmopy-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scmopy
-Version: 0.1.3
+Version: 0.1.4
 Summary: scmopy: Distribution-Agnostic Structural Causal Models Optimization in Python
 Home-page: https://github.com/DSsoli/scmopy.git
 Author: Sanghoon Lee (DSsoli)
 Author-email: solisoli3197@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `scmopy-0.1.3/README.md` & `scmopy-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `scmopy-0.1.3/examples/ESA-2SCM_Example.ipynb` & `scmopy-0.1.4/examples/ESA-2SCM_Example.ipynb`

 * *Files identical despite different names*

### Comparing `scmopy-0.1.3/scmopy/LICENSE` & `scmopy-0.1.4/scmopy/LICENSE`

 * *Files identical despite different names*

### Comparing `scmopy-0.1.3/scmopy/__init__.py` & `scmopy-0.1.4/scmopy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 
 Should you use the scmopy package, please cite the following articles.
 - Lee, Sanghoon (2024). ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable, SnB Political and Economic Research Institute, 1, 21. <snbperi.org/article/230>.
 - S.Shimizu and Y.Kano (2008). Use of non-normality in structural equation modeling: Application to direction of causation, Journal of Statistical Planning and Inference, 138, 11, 3483-3491.
 
 """
 
-__version__ = '0.1.3'
+__version__ = '0.1.4'
```

### Comparing `scmopy-0.1.3/scmopy/base.py` & `scmopy-0.1.4/scmopy/base.py`

 * *Files identical despite different names*

### Comparing `scmopy-0.1.3/scmopy/components/__init__.py` & `scmopy-0.1.4/scmopy/components/__init__.py`

 * *Files identical despite different names*

### Comparing `scmopy-0.1.3/scmopy/components/syniv.py` & `scmopy-0.1.4/scmopy/components/syniv.py`

 * *Files identical despite different names*

### Comparing `scmopy-0.1.3/scmopy/gaussian_scm.py` & `scmopy-0.1.4/scmopy/gaussian_scm.py`

 * *Files identical despite different names*

### Comparing `scmopy-0.1.3/scmopy/model_selection.py` & `scmopy-0.1.4/scmopy/model_selection.py`

 * *Files identical despite different names*

### Comparing `scmopy-0.1.3/scmopy/nongaussian_scm.py` & `scmopy-0.1.4/scmopy/nongaussian_scm.py`

 * *Files 0% similar despite different names*

```diff
@@ -292,15 +292,15 @@
             self._causal_dir = 'x2->x1' if self._T2_rev > self._T2 else 'x1->x2' if self._T2_rev < self._T2 else 'undetermined'
             
             self._true_causal_coef = self._b12 if self._causal_dir == 'x2->x1' else self._b21 if self._causal_dir == 'x1->x2' else 'undetermined'
             self._true_test_statistic = self._T2 if self._causal_dir == 'x2->x1' else self._T2_rev if self._causal_dir == 'x1->x2' else 'undetermined'
             self._true_p_value = self._p_value if self._causal_dir == 'x2->x1' else self._p_value_rev if self._causal_dir == 'x1->x2' else 'undetermined'
             
             self._score = round(r2_score(self._x1, self._b12 * self._x2), 5) if self._causal_dir == 'x2->x1' \
-                else round(r2_score(self._x1_rev, self._b21 * self._x2_rev), 5) if self._causal_dir == 'x2->x1' else 'undetermined'
+                else round(r2_score(self._x1_rev, self._b21 * self._x2_rev), 5) if self._causal_dir == 'x1->x2' else 'undetermined'
                 
         return self
 
     
     def _summary(self):
         
         summary_idx = ['Causal Direction', "Causal Coefficient",  'Test Statistic', 'P-value', "Reject H0", "Goodness of Fit"]
```

### Comparing `scmopy-0.1.3/scmopy.egg-info/PKG-INFO` & `scmopy-0.1.4/scmopy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scmopy
-Version: 0.1.3
+Version: 0.1.4
 Summary: scmopy: Distribution-Agnostic Structural Causal Models Optimization in Python
 Home-page: https://github.com/DSsoli/scmopy.git
 Author: Sanghoon Lee (DSsoli)
 Author-email: solisoli3197@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `scmopy-0.1.3/setup.py` & `scmopy-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 with open("README.md", "r", encoding='utf-8') as fh:
     README = fh.read()
 
 setup(
     author="Sanghoon Lee (DSsoli)",
     author_email="solisoli3197@gmail.com",
     name="scmopy",
-    version="0.1.3",
+    version="0.1.4",
     description="scmopy: Distribution-Agnostic Structural Causal Models Optimization in Python",
     long_description=README,
     long_description_content_type="text/markdown",
     install_requires=["numpy", "pandas", "scipy"],
     url="https://github.com/DSsoli/scmopy.git",
     packages=find_packages(include=['scmopy', 'scmopy.*']),
     package_data={"scmopy": ['LICENSE', 'examples/*']},
```

### Comparing `scmopy-0.1.3/test/test_ESA-2SCM_model.py` & `scmopy-0.1.4/test/test_ESA-2SCM_model.py`

 * *Files identical despite different names*

### Comparing `scmopy-0.1.3/test/test_ESA-2SCM_syniv.py` & `scmopy-0.1.4/test/test_ESA-2SCM_syniv.py`

 * *Files identical despite different names*

