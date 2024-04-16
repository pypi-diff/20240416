# Comparing `tmp/ewatercycle_hbv-1.8.0.tar.gz` & `tmp/ewatercycle_hbv-1.8.1.tar.gz`

## Comparing `ewatercycle_hbv-1.8.0.tar` & `ewatercycle_hbv-1.8.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/.readthedocs.yaml
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/CHANGELOG.md
--rw-r--r--   0        0        0     5813 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/plugin_guide.md
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/.idea/.gitignore
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/.idea/ewatercycle-hbv-numpy.iml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/.idea/misc.xml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/.idea/vcs.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/docs/Makefile
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/docs/conf.py
--rw-r--r--   0        0        0    55896 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/docs/example_model_run_HBV.ipynb
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/docs/index.rst
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/docs/make.bat
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/docs/model.rst
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/docs/requirements.txt
--rw-r--r--   0        0        0    92385 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/docs/_images/model_layout.png
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/docs/_static/README.rst
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/src/ewatercycle_HBV/__init__.py
--rw-r--r--   0        0        0    15335 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/src/ewatercycle_HBV/forcing.py
--rw-r--r--   0        0        0    10048 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/src/ewatercycle_HBV/model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/tests/__init__.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/tests/test_forcing.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/tests/test_model.py
--rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/LICENSE.txt
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/README.md
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/CHANGELOG.md
+-rw-r--r--   0        0        0     5813 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/plugin_guide.md
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/.idea/.gitignore
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/.idea/ewatercycle-hbv-numpy.iml
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/.idea/misc.xml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/.idea/vcs.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/docs/Makefile
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/docs/conf.py
+-rw-r--r--   0        0        0    55896 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/docs/example_model_run_HBV.ipynb
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/docs/index.rst
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/docs/make.bat
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/docs/model.rst
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/docs/requirements.txt
+-rw-r--r--   0        0        0    92385 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/docs/_images/model_layout.png
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/docs/_static/README.rst
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/src/ewatercycle_HBV/__init__.py
+-rw-r--r--   0        0        0    15335 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/src/ewatercycle_HBV/forcing.py
+-rw-r--r--   0        0        0    10036 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/src/ewatercycle_HBV/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/tests/__init__.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/tests/test_forcing.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/tests/test_model.py
+-rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/LICENSE.txt
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/README.md
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/pyproject.toml
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 ewatercycle_hbv-1.8.1/PKG-INFO
```

### Comparing `ewatercycle_hbv-1.8.0/.readthedocs.yaml` & `ewatercycle_hbv-1.8.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.0/CHANGELOG.md` & `ewatercycle_hbv-1.8.1/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -34,11 +34,13 @@
 - typo in bmi implementation: docker image 1.3.2
 ### 1.6.0
   - now compatible with ewatercycle V2.1 `LumpedMakkinkForcing` which generates evaporation from era5/CMIP.
 #### 1.6.1
   - bug fix occuring when loading makkink data
 ### 1.7.0
   - new version of HBV bmi which adds snow 
-### 1.7.1
+#### 1.7.1
   - bug fix with definitions of state variable names
 ### 1.8.0
-- Refactor potential evaporation from `pev` to `evspsblpot` & `tasmean` to `tas` to match convention
+- Refactor potential evaporation from `pev` to `evspsblpot` & `tasmean` to `tas` to match convention
+#### 1.8.1
+- Rename `LumpedCamelsForcing` to `CamelsForcing`
```

### Comparing `ewatercycle_hbv-1.8.0/plugin_guide.md` & `ewatercycle_hbv-1.8.1/plugin_guide.md`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.0/.github/workflows/python-publish.yml` & `ewatercycle_hbv-1.8.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.0/.github/workflows/test.yml` & `ewatercycle_hbv-1.8.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.0/docs/Makefile` & `ewatercycle_hbv-1.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.0/docs/conf.py` & `ewatercycle_hbv-1.8.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.0/docs/example_model_run_HBV.ipynb` & `ewatercycle_hbv-1.8.1/docs/example_model_run_HBV.ipynb`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.0/docs/index.rst` & `ewatercycle_hbv-1.8.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.0/docs/make.bat` & `ewatercycle_hbv-1.8.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.0/docs/model.rst` & `ewatercycle_hbv-1.8.1/docs/model.rst`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.0/docs/_images/model_layout.png` & `ewatercycle_hbv-1.8.1/docs/_images/model_layout.png`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.0/docs/_static/README.rst` & `ewatercycle_hbv-1.8.1/docs/_static/README.rst`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.0/src/ewatercycle_HBV/forcing.py` & `ewatercycle_hbv-1.8.1/src/ewatercycle_HBV/forcing.py`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.0/src/ewatercycle_HBV/model.py` & `ewatercycle_hbv-1.8.1/src/ewatercycle_HBV/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
             self._config["potential_evaporation_file"] = str(
                 self.forcing.directory / self.forcing.evspsblpot
             )
             self._config["mean_temperature_file"] = str(
                 self.forcing.directory / self.forcing.tas)
 
-        elif type(self.forcing).__name__ == 'LumpedCaravanForcing':
+        elif type(self.forcing).__name__ == 'CaravanForcing':
             self._config["precipitation_file"] = str(
                 self.forcing.directory / self.forcing['pr']
             )
 
             self._config["potential_evaporation_file"] = str(
                 self.forcing.directory / self.forcing['evspsblpot']
             )
@@ -103,15 +103,15 @@
                 ds.to_netcdf(temporary_evspsblpot_file)
                 ds.close()
 
             temporary_pr_file = (self.forcing.directory /
                                  self.forcing.filenames['pr'].replace('pr', 'pr_mm'))
             if not temporary_pr_file.is_file():
                 ds = xr.open_dataset(self.forcing.directory / self.forcing.filenames['pr'])
-                ds['pr'].attrs.attrs.update({'units':'mm'})
+                ds['pr'].attrs.update({'units':'mm'})
                 ds['pr'] = ds['pr'] * 86400
                 ds.to_netcdf(temporary_pr_file)
                 ds.close()
 
             temporary_tas_file = (self.forcing.directory /
                                   self.forcing.filenames['tas'].replace('tas', 'tas_deg'))
             if not temporary_tas_file.is_file():
```

### Comparing `ewatercycle_hbv-1.8.0/.gitignore` & `ewatercycle_hbv-1.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.0/LICENSE.txt` & `ewatercycle_hbv-1.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.0/README.md` & `ewatercycle_hbv-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `ewatercycle_hbv-1.8.0/pyproject.toml` & `ewatercycle_hbv-1.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 path = "src/ewatercycle_HBV/__init__.py"
 
 [project]
 name = "ewatercycle-HBV"
 description = "Implementation of HBV for eWaterCycle"
 readme = "README.md"
 license = "Apache-2.0"
-version = "1.8.0"
+version = "1.8.1"
 authors = [
   { name = "David Haasnoot", email = "davidhaasnoot@gmail.com" },
 ]
 keywords = ["ewatercycle", "hydrology"]
 classifiers = [
   "Intended Audience :: Developers",
   "License :: OSI Approved :: Apache Software License",
```

### Comparing `ewatercycle_hbv-1.8.0/PKG-INFO` & `ewatercycle_hbv-1.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ewatercycle-HBV
-Version: 1.8.0
+Version: 1.8.1
 Summary: Implementation of HBV for eWaterCycle
 Project-URL: homepage, https://github.com/Daafip/ewatercycle-hbv
 Author-email: David Haasnoot <davidhaasnoot@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
 Keywords: ewatercycle,hydrology
 Classifier: Intended Audience :: Developers
```

