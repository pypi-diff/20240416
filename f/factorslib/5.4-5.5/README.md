# Comparing `tmp/factorslib-5.4.tar.gz` & `tmp/factorslib-5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "factorslib-5.4.tar", last modified: Tue Apr  9 11:18:22 2024, max compression
+gzip compressed data, was "factorslib-5.5.tar", last modified: Tue Apr 16 07:56:11 2024, max compression
```

## Comparing `factorslib-5.4.tar` & `factorslib-5.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 11:18:22.942108 factorslib-5.4/
--rw-rw-rw-   0        0        0     1038 2023-12-04 06:04:59.000000 factorslib-5.4/LICENCE.txt
--rw-rw-rw-   0        0        0      325 2024-04-09 11:18:22.941112 factorslib-5.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-12-04 06:04:59.000000 factorslib-5.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 11:18:22.940113 factorslib-5.4/factorslib/
--rw-rw-rw-   0        0        0        0 2023-12-04 06:04:59.000000 factorslib-5.4/factorslib/__init__.py
--rw-rw-rw-   0        0        0    79678 2024-04-09 11:16:43.000000 factorslib-5.4/factorslib/factors.py
-drwxrwxrwx   0        0        0        0 2024-04-09 11:18:22.941112 factorslib-5.4/factorslib.egg-info/
--rw-rw-rw-   0        0        0      325 2024-04-09 11:18:22.000000 factorslib-5.4/factorslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2024-04-09 11:18:22.000000 factorslib-5.4/factorslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 11:18:22.000000 factorslib-5.4/factorslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-09 11:18:22.000000 factorslib-5.4/factorslib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 11:18:22.942108 factorslib-5.4/setup.cfg
--rw-rw-rw-   0        0        0      551 2024-04-09 11:18:21.000000 factorslib-5.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 07:56:11.060492 factorslib-5.5/
+-rw-rw-rw-   0        0        0     1038 2023-12-04 06:04:59.000000 factorslib-5.5/LICENCE.txt
+-rw-rw-rw-   0        0        0      325 2024-04-16 07:56:11.059868 factorslib-5.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-12-04 06:04:59.000000 factorslib-5.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 07:56:11.056973 factorslib-5.5/factorslib/
+-rw-rw-rw-   0        0        0        0 2023-12-04 06:04:59.000000 factorslib-5.5/factorslib/__init__.py
+-rw-rw-rw-   0        0        0    79489 2024-04-16 07:55:17.000000 factorslib-5.5/factorslib/factors.py
+drwxrwxrwx   0        0        0        0 2024-04-16 07:56:11.058975 factorslib-5.5/factorslib.egg-info/
+-rw-rw-rw-   0        0        0      325 2024-04-16 07:56:10.000000 factorslib-5.5/factorslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2024-04-16 07:56:11.000000 factorslib-5.5/factorslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 07:56:10.000000 factorslib-5.5/factorslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-16 07:56:10.000000 factorslib-5.5/factorslib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 07:56:11.060492 factorslib-5.5/setup.cfg
+-rw-rw-rw-   0        0        0      551 2024-04-16 07:56:09.000000 factorslib-5.5/setup.py
```

### Comparing `factorslib-5.4/LICENCE.txt` & `factorslib-5.5/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `factorslib-5.4/factorslib/factors.py` & `factorslib-5.5/factorslib/factors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1820,15 +1820,15 @@
     df1 = df.copy()
     df1['time'] = pd.to_datetime(df1['time'], utc=True)
 
     df2 = pdta.td_seq(close=close)
     df2.columns = ['setup', 'countdown']
     df_final = pd.concat([df1, df2], axis=1)
 
-    df_final['signalF'] = np.nan
+    df_final['signalF'] = 0
     df_final.loc[df_final['countdown'] >= 9, 'signalF'] = 1
     df_final.loc[df_final['setup'] >= 7, 'signalF'] = 0
     df_final.fillna(method='ffill', inplace=True)
 
     df_final.fillna(value=0, inplace=True)
 
     return df_final
@@ -1837,41 +1837,35 @@
 # --------------------------------------------------------20230608新增，择时，CCI
 def CCI_timing(df, close, high, low, N1, *args, **kwargs):
     df1 = df.copy()
     df1['time'] = pd.to_datetime(df1['time'], utc=True)
 
     df1['CCI'] = talib.CCI(close=close, high=high, low=low, timeperiod=N1)
 
-    df1['signalF'] = np.nan
+    df1['signalF'] = 0
     df1.loc[df1['CCI'] <= -100, 'signalF'] = 0
     df1.loc[df1['CCI'] >= 100, 'signalF'] = 1
 
-    df1.fillna(method='ffill', inplace=True)
-    df1.fillna(value=0, inplace=True)
-
     return df1
 
 
 def CCI1_timing(df, close, high, low, N1, N2, N3, MA_df, *args, **kwargs):
     df1 = df.copy()
     df1['time'] = pd.to_datetime(df1['time'], utc=True)
 
     df1['CCI'] = talib.CCI(close=close, high=high, low=low, timeperiod=N1)
 
     df1 = pd.merge(df1, MA_df, on='time', how='left')
     df1['bull'].fillna(method='ffill', inplace=True)
 
-    df1['signalF'] = np.nan
+    df1['signalF'] = 0
     df1.loc[df1['CCI'] <= -100, 'signalF'] = 0
     df1.loc[(df1['CCI'] >= 100) & (df1['bull'] == 1), 'signalF'] = N2
     df1.loc[(df1['CCI'] >= 100) & (df1['bull'] == 0), 'signalF'] = N3
 
-    df1.fillna(method='ffill', inplace=True)
-    df1.fillna(value=0, inplace=True)
-
     return df1
 
 
 # --------------------------------------------------------20240402新增，动量，STOCHk_N1_N2_N3 and STOCHd_N1_N2_N3
 def talib_STOCH(df, close, high, low, N1, N2, N3, *args, **kwargs):
     df1 = df.copy()
     df1['STOCHk_' + str(N1) + '_' + str(N2) + '_' + str(N3)], df1['STOCHd_' + str(N1) + '_' + str(N2) + '_' + str(N3)] = talib.STOCH(close=close, high=high, low=low, fastk_period=N1, slowd_period=N2, slowk_period=N3, slowk_matype=0)
```

### Comparing `factorslib-5.4/setup.py` & `factorslib-5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setuptools.setup(
     name="factorslib",
-    version="5.4",
+    version="5.5",
     author="wytxty",
     author_email="yvettewkkaa@gmail.com",
     description="financial factors calculation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wytxty/factorslib",
     packages=setuptools.find_packages(),
```

