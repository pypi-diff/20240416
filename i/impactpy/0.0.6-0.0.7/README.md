# Comparing `tmp/impactpy-0.0.6.tar.gz` & `tmp/impactpy-0.0.7.tar.gz`

## Comparing `impactpy-0.0.6.tar` & `impactpy-0.0.7.tar`

### file list

```diff
@@ -1,45 +1,41 @@
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 impactpy-0.0.6/ImpactPy.egg-info/PKG-INFO
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 impactpy-0.0.6/ImpactPy.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 impactpy-0.0.6/ImpactPy.egg-info/dependency_links.txt
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 impactpy-0.0.6/ImpactPy.egg-info/requires.txt
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 impactpy-0.0.6/ImpactPy.egg-info/top_level.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impactpy-0.0.6/build/lib/src/__init__.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 impactpy-0.0.6/build/lib/src/alpha/__init__.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 impactpy-0.0.6/build/lib/src/alpha/base_alpha.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impactpy-0.0.6/build/lib/src/alpha/intraday_alpha.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impactpy-0.0.6/build/lib/src/alpha/overnight_alpha.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 impactpy-0.0.6/build/lib/src/alpha/trading_alpha.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 impactpy-0.0.6/build/lib/src/models/__init__.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 impactpy-0.0.6/build/lib/src/models/afs_model.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 impactpy-0.0.6/build/lib/src/models/impact_model.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 impactpy-0.0.6/build/lib/src/models/ow_model.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 impactpy-0.0.6/build/lib/src/schedule/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 impactpy-0.0.6/build/lib/src/schedule/schedule.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 impactpy-0.0.6/build/lib/src/tca/__init__.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 impactpy-0.0.6/build/lib/src/tca/tca_report.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impactpy-0.0.6/build/lib/testing/__init__.py
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 impactpy-0.0.6/build/lib/testing/test_cfg.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impactpy-0.0.6/impactpy/__init__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 impactpy-0.0.6/impactpy/alpha/__init__.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 impactpy-0.0.6/impactpy/alpha/base_alpha.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 impactpy-0.0.6/impactpy/alpha/intraday_alpha.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impactpy-0.0.6/impactpy/alpha/overnight_alpha.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 impactpy-0.0.6/impactpy/alpha/trading_alpha.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 impactpy-0.0.6/impactpy/data/__init__.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 impactpy-0.0.6/impactpy/data/market_data.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 impactpy-0.0.6/impactpy/models/__init__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 impactpy-0.0.6/impactpy/models/afs_model.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 impactpy-0.0.6/impactpy/models/impact_model.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 impactpy-0.0.6/impactpy/models/ow_model.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 impactpy-0.0.6/impactpy/schedule/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 impactpy-0.0.6/impactpy/schedule/schedule.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 impactpy-0.0.6/impactpy/tca/__init__.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 impactpy-0.0.6/impactpy/tca/tca_report.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 impactpy-0.0.6/impactpy_lachlanbaxter.egg-info/PKG-INFO
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 impactpy-0.0.6/impactpy_lachlanbaxter.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 impactpy-0.0.6/impactpy_lachlanbaxter.egg-info/dependency_links.txt
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 impactpy-0.0.6/impactpy_lachlanbaxter.egg-info/requires.txt
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 impactpy-0.0.6/impactpy_lachlanbaxter.egg-info/top_level.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impactpy-0.0.6/README.md
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 impactpy-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 impactpy-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 impactpy-0.0.7/ImpactPy.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 impactpy-0.0.7/ImpactPy.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 impactpy-0.0.7/ImpactPy.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 impactpy-0.0.7/ImpactPy.egg-info/requires.txt
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 impactpy-0.0.7/ImpactPy.egg-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impactpy-0.0.7/build/lib/src/__init__.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 impactpy-0.0.7/build/lib/src/alpha/__init__.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 impactpy-0.0.7/build/lib/src/alpha/base_alpha.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impactpy-0.0.7/build/lib/src/alpha/intraday_alpha.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impactpy-0.0.7/build/lib/src/alpha/overnight_alpha.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 impactpy-0.0.7/build/lib/src/alpha/trading_alpha.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 impactpy-0.0.7/build/lib/src/models/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 impactpy-0.0.7/build/lib/src/models/afs_model.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 impactpy-0.0.7/build/lib/src/models/impact_model.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 impactpy-0.0.7/build/lib/src/models/ow_model.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 impactpy-0.0.7/build/lib/src/schedule/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 impactpy-0.0.7/build/lib/src/schedule/schedule.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 impactpy-0.0.7/build/lib/src/tca/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 impactpy-0.0.7/build/lib/src/tca/tca_report.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impactpy-0.0.7/build/lib/testing/__init__.py
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 impactpy-0.0.7/build/lib/testing/test_cfg.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impactpy-0.0.7/impactpy/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 impactpy-0.0.7/impactpy/data/__init__.py
+-rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 impactpy-0.0.7/impactpy/data/bin_schedule.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 impactpy-0.0.7/impactpy/data/market_data.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 impactpy-0.0.7/impactpy/data/schema.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 impactpy-0.0.7/impactpy/models/__init__.py
+-rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 impactpy-0.0.7/impactpy/models/model.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 impactpy-0.0.7/impactpy/trading/__init__.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 impactpy-0.0.7/impactpy/trading/alpha.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 impactpy-0.0.7/impactpy/trading/order.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 impactpy-0.0.7/impactpy/trading/tca.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 impactpy-0.0.7/impactpy_lachlanbaxter.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 impactpy-0.0.7/impactpy_lachlanbaxter.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 impactpy-0.0.7/impactpy_lachlanbaxter.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 impactpy-0.0.7/impactpy_lachlanbaxter.egg-info/requires.txt
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 impactpy-0.0.7/impactpy_lachlanbaxter.egg-info/top_level.txt
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 impactpy-0.0.7/tests/data/test_bin_schedule.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impactpy-0.0.7/README.md
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 impactpy-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 impactpy-0.0.7/PKG-INFO
```

### Comparing `impactpy-0.0.6/ImpactPy.egg-info/SOURCES.txt` & `impactpy-0.0.7/ImpactPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `impactpy-0.0.6/build/lib/src/models/impact_model.py` & `impactpy-0.0.7/build/lib/src/models/impact_model.py`

 * *Files identical despite different names*

### Comparing `impactpy-0.0.6/build/lib/testing/test_cfg.py` & `impactpy-0.0.7/build/lib/testing/test_cfg.py`

 * *Files identical despite different names*

### Comparing `impactpy-0.0.6/impactpy/models/impact_model.py` & `impactpy-0.0.7/impactpy/models/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,8 +64,11 @@
 	# TODO maybe this doesn't need to be abstract?
 	def compute_impact(self, df: pl.DataFrame) -> pl.LazyFrame:
 		lf = df.lazy()
 		lf = lf.with_columns((pl.col('trade') / pl.col('adv')).alias('_trade'))
 		lf = lf.with_columns(self.kernel(pl.col('_trade')).alias('_trade'))
 		lf = lf.with_columns((pl.col('_trade') * pl.col('vol')).alias('_trade'))
 		lf = self.aggregate_impact(lf)
-		return lf
+		return lf
+
+
+class AFSModel(ImpactModel): ...
```

### Comparing `impactpy-0.0.6/impactpy_lachlanbaxter.egg-info/PKG-INFO` & `impactpy-0.0.7/impactpy_lachlanbaxter.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `impactpy-0.0.6/impactpy_lachlanbaxter.egg-info/SOURCES.txt` & `impactpy-0.0.7/impactpy_lachlanbaxter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `impactpy-0.0.6/pyproject.toml` & `impactpy-0.0.7/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["impactpy"]
 
 [project]
 name = "impactpy"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Lachlan Baxter", email="lachlan.baxter@outlook.com" },
 ]
 description = "Toolset for calibrating price impact models to LOB data"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers= [
```

