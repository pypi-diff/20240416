# Comparing `tmp/ecbdata-0.0.5.tar.gz` & `tmp/ecbdata-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecbdata-0.0.5.tar", last modified: Tue Apr 16 10:49:51 2024, max compression
+gzip compressed data, was "ecbdata-0.0.6.tar", last modified: Tue Apr 16 11:28:42 2024, max compression
```

## Comparing `ecbdata-0.0.5.tar` & `ecbdata-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 metellis   (501) staff       (20)        0 2024-04-16 10:49:51.852042 ecbdata-0.0.5/
--rw-r--r--   0 metellis   (501) staff       (20)     1075 2024-04-16 09:46:02.000000 ecbdata-0.0.5/LICENSE.md
--rw-r--r--   0 metellis   (501) staff       (20)     2627 2024-04-16 10:49:51.851803 ecbdata-0.0.5/PKG-INFO
--rw-r--r--   0 metellis   (501) staff       (20)     2160 2024-04-16 10:49:36.000000 ecbdata-0.0.5/README.md
-drwxr-xr-x   0 metellis   (501) staff       (20)        0 2024-04-16 10:49:51.849893 ecbdata-0.0.5/ecbdata/
--rw-r--r--   0 metellis   (501) staff       (20)      188 2024-04-16 10:49:36.000000 ecbdata-0.0.5/ecbdata/__about__.py
--rw-r--r--   0 metellis   (501) staff       (20)      137 2024-04-16 10:49:36.000000 ecbdata-0.0.5/ecbdata/__init__.py
--rw-r--r--   0 metellis   (501) staff       (20)     9648 2024-04-16 10:49:36.000000 ecbdata-0.0.5/ecbdata/api.py
-drwxr-xr-x   0 metellis   (501) staff       (20)        0 2024-04-16 10:49:51.851374 ecbdata-0.0.5/ecbdata/tests/
--rw-r--r--   0 metellis   (501) staff       (20)      102 2024-04-16 10:49:36.000000 ecbdata-0.0.5/ecbdata/tests/__init__.py
--rw-r--r--   0 metellis   (501) staff       (20)     1167 2024-04-16 10:49:36.000000 ecbdata-0.0.5/ecbdata/tests/test.py
-drwxr-xr-x   0 metellis   (501) staff       (20)        0 2024-04-16 10:49:51.850933 ecbdata-0.0.5/ecbdata.egg-info/
--rw-r--r--   0 metellis   (501) staff       (20)     2627 2024-04-16 10:49:51.000000 ecbdata-0.0.5/ecbdata.egg-info/PKG-INFO
--rw-r--r--   0 metellis   (501) staff       (20)      287 2024-04-16 10:49:51.000000 ecbdata-0.0.5/ecbdata.egg-info/SOURCES.txt
--rw-r--r--   0 metellis   (501) staff       (20)        1 2024-04-16 10:49:51.000000 ecbdata-0.0.5/ecbdata.egg-info/dependency_links.txt
--rw-r--r--   0 metellis   (501) staff       (20)       16 2024-04-16 10:49:51.000000 ecbdata-0.0.5/ecbdata.egg-info/requires.txt
--rw-r--r--   0 metellis   (501) staff       (20)        8 2024-04-16 10:49:51.000000 ecbdata-0.0.5/ecbdata.egg-info/top_level.txt
--rw-r--r--   0 metellis   (501) staff       (20)       38 2024-04-16 10:49:51.852115 ecbdata-0.0.5/setup.cfg
--rw-r--r--   0 metellis   (501) staff       (20)      978 2024-04-16 09:49:54.000000 ecbdata-0.0.5/setup.py
+drwxr-xr-x   0 metellis   (501) staff       (20)        0 2024-04-16 11:28:42.677534 ecbdata-0.0.6/
+-rw-r--r--   0 metellis   (501) staff       (20)     1075 2024-04-16 09:46:02.000000 ecbdata-0.0.6/LICENSE.md
+-rw-r--r--   0 metellis   (501) staff       (20)     2581 2024-04-16 11:28:42.677407 ecbdata-0.0.6/PKG-INFO
+-rw-r--r--   0 metellis   (501) staff       (20)     2160 2024-04-16 11:28:26.000000 ecbdata-0.0.6/README.md
+drwxr-xr-x   0 metellis   (501) staff       (20)        0 2024-04-16 11:28:42.675854 ecbdata-0.0.6/ecbdata/
+-rw-r--r--   0 metellis   (501) staff       (20)      188 2024-04-16 11:28:26.000000 ecbdata-0.0.6/ecbdata/__about__.py
+-rw-r--r--   0 metellis   (501) staff       (20)      137 2024-04-16 10:49:36.000000 ecbdata-0.0.6/ecbdata/__init__.py
+-rw-r--r--   0 metellis   (501) staff       (20)     9854 2024-04-16 11:28:26.000000 ecbdata-0.0.6/ecbdata/api.py
+drwxr-xr-x   0 metellis   (501) staff       (20)        0 2024-04-16 11:28:42.677114 ecbdata-0.0.6/ecbdata/tests/
+-rw-r--r--   0 metellis   (501) staff       (20)      102 2024-04-16 10:49:36.000000 ecbdata-0.0.6/ecbdata/tests/__init__.py
+-rw-r--r--   0 metellis   (501) staff       (20)     1390 2024-04-16 11:28:26.000000 ecbdata-0.0.6/ecbdata/tests/test.py
+drwxr-xr-x   0 metellis   (501) staff       (20)        0 2024-04-16 11:28:42.676743 ecbdata-0.0.6/ecbdata.egg-info/
+-rw-r--r--   0 metellis   (501) staff       (20)     2581 2024-04-16 11:28:42.000000 ecbdata-0.0.6/ecbdata.egg-info/PKG-INFO
+-rw-r--r--   0 metellis   (501) staff       (20)      287 2024-04-16 11:28:42.000000 ecbdata-0.0.6/ecbdata.egg-info/SOURCES.txt
+-rw-r--r--   0 metellis   (501) staff       (20)        1 2024-04-16 11:28:42.000000 ecbdata-0.0.6/ecbdata.egg-info/dependency_links.txt
+-rw-r--r--   0 metellis   (501) staff       (20)       16 2024-04-16 11:28:42.000000 ecbdata-0.0.6/ecbdata.egg-info/requires.txt
+-rw-r--r--   0 metellis   (501) staff       (20)        8 2024-04-16 11:28:42.000000 ecbdata-0.0.6/ecbdata.egg-info/top_level.txt
+-rw-r--r--   0 metellis   (501) staff       (20)       38 2024-04-16 11:28:42.677581 ecbdata-0.0.6/setup.cfg
+-rw-r--r--   0 metellis   (501) staff       (20)      978 2024-04-16 09:49:54.000000 ecbdata-0.0.6/setup.py
```

### Comparing `ecbdata-0.0.5/LICENSE.md` & `ecbdata-0.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ecbdata-0.0.5/PKG-INFO` & `ecbdata-0.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: ecbdata
-Version: 0.0.5
+Version: 0.0.6
 Home-page: https://github.com/LucaMingarelli/ecbdata
 Author: Luca Mingarelli
 Author-email: luca.mingarelli@ecb.europa.eu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: requests
-Requires-Dist: pandas
 
 # ecbdata <img src="https://raw.githubusercontent.com/LucaMingarelli/ecbdata/master/ecbdata/res/Logo_European_Central_Bank.svg"  width="80">
 
 [![CircleCI](https://circleci.com/gh/LucaMingarelli/ecbdata.svg?style=svg&circle-token=cd9c300380d25c24c66cd6637693cc50a7e00248)](https://app.circleci.com/pipelines/github/LucaMingarelli/ecbdata)
-[![version](https://img.shields.io/badge/version-0.0.5-success.svg)](#)
+[![version](https://img.shields.io/badge/version-0.0.6-success.svg)](#)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/ecbdata.svg)](https://pypi.org/project/ecbdata/)
 [![License](https://img.shields.io/pypi/l/ecbdata.svg)](https://github.com/LucaMingarelli/ecbdata/blob/master/LICENSE.txt)
 [![Downloads](https://static.pepy.tech/badge/ecbdata)](https://pepy.tech/project/ecbdata)
 <a href="https://www.buymeacoffee.com/lucamingarelli" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/arial-yellow.png" alt="Buy Me A Coffee" style="height: 30px !important;width: 109px !important;" ></a>
 
 ## About
 
@@ -42,15 +40,16 @@
 
 ```
 
 When behind a proxy server, one can establish a connection as
 
 ```python
 from ecbdata import ecbdata
-ecbdata.connect(proxies={'https': '<https-proxy>', 
+
+ecbdata.connect(proxies={'https': '<https-proxy>',
                          'http': '<http-proxy>'})
 
 df = ecbdata.get_series('ICP.M.U2.Y.XEF000.3.INX', start='2024-01', end='2024-03')
 
 ```
 
 For details on available series and filters,
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: ecbdata Version: 0.0.5 Home-page: https://
+Metadata-Version: 2.1 Name: ecbdata Version: 0.0.6 Home-page: https://
 github.com/LucaMingarelli/ecbdata Author: Luca Mingarelli Author-email:
 luca.mingarelli@ecb.europa.eu License: MIT Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
-Type: text/markdown License-File: LICENSE.md Requires-Dist: requests Requires-
-Dist: pandas # ecbdata [https://raw.githubusercontent.com/LucaMingarelli/
-ecbdata/master/ecbdata/res/Logo_European_Central_Bank.svg][![CircleCI](https://
-circleci.com/gh/LucaMingarelli/ecbdata.svg?style=svg&circle-
+Type: text/markdown License-File: LICENSE.md # ecbdata [https://
+raw.githubusercontent.com/LucaMingarelli/ecbdata/master/ecbdata/res/
+Logo_European_Central_Bank.svg][![CircleCI](https://circleci.com/gh/
+LucaMingarelli/ecbdata.svg?style=svg&circle-
 token=cd9c300380d25c24c66cd6637693cc50a7e00248)](https://app.circleci.com/
 pipelines/github/LucaMingarelli/ecbdata) [![version](https://img.shields.io/
-badge/version-0.0.5-success.svg)](#) [![PyPI Latest Release](https://
+badge/version-0.0.6-success.svg)](#) [![PyPI Latest Release](https://
 img.shields.io/pypi/v/ecbdata.svg)](https://pypi.org/project/ecbdata/) [!
 [License](https://img.shields.io/pypi/l/ecbdata.svg)](https://github.com/
 LucaMingarelli/ecbdata/blob/master/LICENSE.txt) [![Downloads](https://
 static.pepy.tech/badge/ecbdata)](https://pepy.tech/project/ecbdata) _[_B_u_y_ _M_e_ _A
 _C_o_f_f_e_e_]## About The **ecbdata** API allows for easy querying of data from the
 [ECB Data Portal](https://data.ecb.europa.eu/help/data/overview). ##
 Installation You can install with pip as: `pip install ecbdata` ### Example
```

### Comparing `ecbdata-0.0.5/README.md` & `ecbdata-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # ecbdata <img src="https://raw.githubusercontent.com/LucaMingarelli/ecbdata/master/ecbdata/res/Logo_European_Central_Bank.svg"  width="80">
 
 [![CircleCI](https://circleci.com/gh/LucaMingarelli/ecbdata.svg?style=svg&circle-token=cd9c300380d25c24c66cd6637693cc50a7e00248)](https://app.circleci.com/pipelines/github/LucaMingarelli/ecbdata)
-[![version](https://img.shields.io/badge/version-0.0.5-success.svg)](#)
+[![version](https://img.shields.io/badge/version-0.0.6-success.svg)](#)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/ecbdata.svg)](https://pypi.org/project/ecbdata/)
 [![License](https://img.shields.io/pypi/l/ecbdata.svg)](https://github.com/LucaMingarelli/ecbdata/blob/master/LICENSE.txt)
 [![Downloads](https://static.pepy.tech/badge/ecbdata)](https://pepy.tech/project/ecbdata)
 <a href="https://www.buymeacoffee.com/lucamingarelli" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/arial-yellow.png" alt="Buy Me A Coffee" style="height: 30px !important;width: 109px !important;" ></a>
 
 ## About
 
@@ -26,15 +26,16 @@
 
 ```
 
 When behind a proxy server, one can establish a connection as
 
 ```python
 from ecbdata import ecbdata
-ecbdata.connect(proxies={'https': '<https-proxy>', 
+
+ecbdata.connect(proxies={'https': '<https-proxy>',
                          'http': '<http-proxy>'})
 
 df = ecbdata.get_series('ICP.M.U2.Y.XEF000.3.INX', start='2024-01', end='2024-03')
 
 ```
 
 For details on available series and filters,
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # ecbdata [https://raw.githubusercontent.com/LucaMingarelli/ecbdata/master/
 ecbdata/res/Logo_European_Central_Bank.svg][![CircleCI](https://circleci.com/
 gh/LucaMingarelli/ecbdata.svg?style=svg&circle-
 token=cd9c300380d25c24c66cd6637693cc50a7e00248)](https://app.circleci.com/
 pipelines/github/LucaMingarelli/ecbdata) [![version](https://img.shields.io/
-badge/version-0.0.5-success.svg)](#) [![PyPI Latest Release](https://
+badge/version-0.0.6-success.svg)](#) [![PyPI Latest Release](https://
 img.shields.io/pypi/v/ecbdata.svg)](https://pypi.org/project/ecbdata/) [!
 [License](https://img.shields.io/pypi/l/ecbdata.svg)](https://github.com/
 LucaMingarelli/ecbdata/blob/master/LICENSE.txt) [![Downloads](https://
 static.pepy.tech/badge/ecbdata)](https://pepy.tech/project/ecbdata) _[_B_u_y_ _M_e_ _A
 _C_o_f_f_e_e_]## About The **ecbdata** API allows for easy querying of data from the
 [ECB Data Portal](https://data.ecb.europa.eu/help/data/overview). ##
 Installation You can install with pip as: `pip install ecbdata` ### Example
```

### Comparing `ecbdata-0.0.5/ecbdata/api.py` & `ecbdata-0.0.6/ecbdata/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,25 +55,25 @@
         session = requests.Session()
         session.proxies = proxies or {}
         if verify:
             session.verify = verify
         self._session = session
 
 
-    def _search_string(self, ticker, start=None, end=None,
+    def _search_string(self, series_key, start=None, end=None,
                        detail=None, updatedafter=None,
                        firstnobservations=None, lastnobservations=None,
                        includehistory=False
                        ):
         """Constructs the url string for the options specified."""
         includehistory = 'true' if includehistory else 'false'
 
-        decoded = re.findall(r"(\w+)\.", ticker)
+        decoded = re.findall(r"(\w+)\.", series_key)
         db = decoded[0]
-        ticker_str = '.'.join(re.findall(r"\.(\w+)", ticker))
+        ticker_str = '.'.join(re.findall(r"\.(\w+)", series_key))
         url = f"{WSENTRYPOINT}/service/data/{db}/{ticker_str}?format=csvdata"
         if start: url += f'&startPeriod={start}'
         if end:   url += f'&endPeriod={end}'
         if detail: url += f"&detail={detail}"
         if updatedafter: url += f"&updatedafter={updatedafter}"
         if firstnobservations: url += f"&firstnobservations={firstnobservations}"
         if lastnobservations: url += f"&lastnobservations={lastnobservations}"
@@ -94,22 +94,22 @@
         if response.status_code!=200:
             if response.status_code in errors_msgs:
                 raise Exception(f'REQUEST ERROR {response.status_code}: '+errors_msgs[response.status_code])
             else:
                 print(f'REQUEST ERROR {response.status_code}: ')
                 response.raise_for_status()
 
-    def get_series(self, ticker, start: str=None, end: str=None,
+    def get_series(self, series_key, start: str=None, end: str=None,
                    detail: str=None, updatedafter: str=None,
                    firstnobservations: int=None, lastnobservations: int=None, includehistory: bool=False):
         """
         Downloads data for selected ticker.
 
         Args:
-            ticker:
+            series_key: Series' key for the data to be retrieved. This can be obtained from the ECB Data Portal https://data.ecb.europa.eu/. E.g. HICP inflation that would be "ICP.M.U2.N.000000.4.ANR".
             start: It is possible to define a start date for which observations are to be returned. The values should be given according to the syntax defined in ISO 8601 or as SDMX reporting periods. The format will vary depending on the frequency. The supported formats are: YYYY for annual data (e.g. 2013); YYYY-S[1-2]  for semi-annual data (e.g. 2013-S1); YYYY-Q[1-4]  for quarterly data (e.g. 2013-Q1); YYYY-MM  for monthly data (e.g. 2013-01); YYYY-W[01-53]  for weekly data (e.g. 2013-W01); YYYY-MM-DD  for daily data (e.g. 2013-01-01).
             end:   It is possible to define an end date for which observations are to be returned. The values should be given according to the syntax defined in ISO 8601 or as SDMX reporting periods. The format will vary depending on the frequency. The supported formats are: YYYY for annual data (e.g. 2013); YYYY-S[1-2]  for semi-annual data (e.g. 2013-S1); YYYY-Q[1-4]  for quarterly data (e.g. 2013-Q1); YYYY-MM  for monthly data (e.g. 2013-01); YYYY-W[01-53]  for weekly data (e.g. 2013-W01); YYYY-MM-DD  for daily data (e.g. 2013-01-01).
             detail: Using the detail parameter, it is possible to specify the desired amount of information to be returned by the web service. Possible options are as follows. full: the data (Time series and Observations) and the Attributes will be returned. This is the default. dataonly: the Attributes will be excluded from the returned message. serieskeysonly: only the Time series will be returned, excluding the Attributes and the Observations. This can be used to list Time series that match a certain query without returning the actual data. nodata: the Time series will be returned, including the Attributes, but the Observations will not.
             updatedafter: By supplying a percent-encoded ISO 8601 timestamp for the updatedafter parameter, it is possible to retrieve the latest version of changed values in the database after a certain point in time (i.e. updates and revisions). This will include: the observations that have been added since the supplied timestamp; the observations that have been revised since the supplied timestamp; the observations that have been deleted since the supplied timestamp. For example, the percent-encoded representation for 2009-05-15T14:15:00+01:00 would be: 2009-05-15T14%3A15%3A00%2B01%3A00. Developers who update their local databases with data stored in the ECB Data Portal should make use of the updatedafter parameter, as this will significantly improve performance. Instead of systematically downloading data that have not changed, you will only receive the changes that were made in the database after you last performed the same query. If nothing has changed, the server will respond with a HTTP 304 response code.
             firstnobservations:  returns first `firstnobservations` observations.
             lastnobservations: returns last `lastnobservations` observations.
             includehistory: Using the includehistory parameter, you can instruct the web service to return previous versions of the matching data. This allows you to see how the data have evolved over time (i.e. see when new data were released, revised or deleted). Possible options are: false: only the version currently in production will be returned. This is the default. true: the version currently in production and all previous versions will be returned.
@@ -117,16 +117,16 @@
             pandas.DataFrame
 
         Examples:
             >>> from ecbdata import ecbdata
             >>> df = ecbdata.get_series('ICP.M.U2.Y.XEF000.3.INX')
         """
         # response = _session.get(url=f"{WSENTRYPOINT}/service/data/{db}/{ticker_str}?format=csvdata")
-        response = self._session.get(url=self._search_string(ticker=ticker, start=start, end=end,
-                                                             detail=detail, updatedafter=updatedafter,
+        response = self._session.get(url=self._search_string(series_key=series_key, start=start, end=end, detail=detail,
+                                                             updatedafter=updatedafter,
                                                              firstnobservations=firstnobservations,
                                                              lastnobservations=lastnobservations,
                                                              includehistory=includehistory))
         self.__response_handler(response=response)
         df = pd.read_csv(io.StringIO(response.content.decode()))
         return df
```

### Comparing `ecbdata-0.0.5/ecbdata/tests/test.py` & `ecbdata-0.0.6/ecbdata/tests/test.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,38 +3,47 @@
  
 **Authors**: L. Mingarelli
 """
 from ecbdata import ecbdata
 import pytest
 
 _MANUAL = False
-tickers = ['ICP.M.U2.Y.XEF000.3.INX',                        # Inflation
-           'MNA.Q.Y.I8.W2.S1.S1.B.B1GQ._Z._Z._Z.EUR.LR.N',   # GDP
-           'FM.M.U2.EUR.4F.MM.EONIA.HSTA',                   # EONIA
-           'ENA.Q.Y.I8.W2.S1.S1._Z.EMP._Z._T._Z.HW._Z.N',    # Employment in hour worked
-           ]
+series_keys = ['ICP.M.U2.Y.XEF000.3.INX',                        # Inflation
+               'MNA.Q.Y.I8.W2.S1.S1.B.B1GQ._Z._Z._Z.EUR.LR.N',   # GDP
+               'FM.M.U2.EUR.4F.MM.EONIA.HSTA',                   # EONIA
+               'ENA.Q.Y.I8.W2.S1.S1._Z.EMP._Z._T._Z.HW._Z.N',    # Employment in hour worked
+               ]
 
 class TestECBDATA:
     def test_get_series(self):
-        df = ecbdata.get_series(ticker=tickers[0])
+        df = ecbdata.get_series(series_key=series_keys[0])
         assert not df.empty
-        df = ecbdata.get_series(ticker=tickers[0], start='2024-01', end='2024-03')
+        df = ecbdata.get_series(series_key=series_keys[0], start='2024-01', end='2024-03')
         assert df.TIME_PERIOD.min() == '2024-01'
         assert df.TIME_PERIOD.max() == '2024-03'
         print(df)
 
     def test_error(self):
         with pytest.raises(Exception):
-            ecbdata.get_series(ticker="ABC.CBA", start='2024-01-01', end='2024-03-01')
+            ecbdata.get_series(series_key="ABC.CBA", start='2024-01-01', end='2024-03-01')
 
 
 
 
 if _MANUAL:
 
     from connectors.certificates import where
     from connectors.certificates.proxies import PROXIES
 
     ecbdata.connect(proxies=PROXIES, verify=where())
 
-    ecbdata.get_series(ticker=tickers[0])
+    df = ecbdata.get_series(series_key=series_keys[0])
+
+    import pandas as pd, pylab as plt
+    df.TIME_PERIOD = pd.to_datetime(df.TIME_PERIOD)
+    df = df.set_index('TIME_PERIOD')
+    df.OBS_VALUE.plot()
+    plt.show()
+
+
+
```

### Comparing `ecbdata-0.0.5/ecbdata.egg-info/PKG-INFO` & `ecbdata-0.0.6/ecbdata.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: ecbdata
-Version: 0.0.5
+Version: 0.0.6
 Home-page: https://github.com/LucaMingarelli/ecbdata
 Author: Luca Mingarelli
 Author-email: luca.mingarelli@ecb.europa.eu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: requests
-Requires-Dist: pandas
 
 # ecbdata <img src="https://raw.githubusercontent.com/LucaMingarelli/ecbdata/master/ecbdata/res/Logo_European_Central_Bank.svg"  width="80">
 
 [![CircleCI](https://circleci.com/gh/LucaMingarelli/ecbdata.svg?style=svg&circle-token=cd9c300380d25c24c66cd6637693cc50a7e00248)](https://app.circleci.com/pipelines/github/LucaMingarelli/ecbdata)
-[![version](https://img.shields.io/badge/version-0.0.5-success.svg)](#)
+[![version](https://img.shields.io/badge/version-0.0.6-success.svg)](#)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/ecbdata.svg)](https://pypi.org/project/ecbdata/)
 [![License](https://img.shields.io/pypi/l/ecbdata.svg)](https://github.com/LucaMingarelli/ecbdata/blob/master/LICENSE.txt)
 [![Downloads](https://static.pepy.tech/badge/ecbdata)](https://pepy.tech/project/ecbdata)
 <a href="https://www.buymeacoffee.com/lucamingarelli" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/arial-yellow.png" alt="Buy Me A Coffee" style="height: 30px !important;width: 109px !important;" ></a>
 
 ## About
 
@@ -42,15 +40,16 @@
 
 ```
 
 When behind a proxy server, one can establish a connection as
 
 ```python
 from ecbdata import ecbdata
-ecbdata.connect(proxies={'https': '<https-proxy>', 
+
+ecbdata.connect(proxies={'https': '<https-proxy>',
                          'http': '<http-proxy>'})
 
 df = ecbdata.get_series('ICP.M.U2.Y.XEF000.3.INX', start='2024-01', end='2024-03')
 
 ```
 
 For details on available series and filters,
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: ecbdata Version: 0.0.5 Home-page: https://
+Metadata-Version: 2.1 Name: ecbdata Version: 0.0.6 Home-page: https://
 github.com/LucaMingarelli/ecbdata Author: Luca Mingarelli Author-email:
 luca.mingarelli@ecb.europa.eu License: MIT Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
-Type: text/markdown License-File: LICENSE.md Requires-Dist: requests Requires-
-Dist: pandas # ecbdata [https://raw.githubusercontent.com/LucaMingarelli/
-ecbdata/master/ecbdata/res/Logo_European_Central_Bank.svg][![CircleCI](https://
-circleci.com/gh/LucaMingarelli/ecbdata.svg?style=svg&circle-
+Type: text/markdown License-File: LICENSE.md # ecbdata [https://
+raw.githubusercontent.com/LucaMingarelli/ecbdata/master/ecbdata/res/
+Logo_European_Central_Bank.svg][![CircleCI](https://circleci.com/gh/
+LucaMingarelli/ecbdata.svg?style=svg&circle-
 token=cd9c300380d25c24c66cd6637693cc50a7e00248)](https://app.circleci.com/
 pipelines/github/LucaMingarelli/ecbdata) [![version](https://img.shields.io/
-badge/version-0.0.5-success.svg)](#) [![PyPI Latest Release](https://
+badge/version-0.0.6-success.svg)](#) [![PyPI Latest Release](https://
 img.shields.io/pypi/v/ecbdata.svg)](https://pypi.org/project/ecbdata/) [!
 [License](https://img.shields.io/pypi/l/ecbdata.svg)](https://github.com/
 LucaMingarelli/ecbdata/blob/master/LICENSE.txt) [![Downloads](https://
 static.pepy.tech/badge/ecbdata)](https://pepy.tech/project/ecbdata) _[_B_u_y_ _M_e_ _A
 _C_o_f_f_e_e_]## About The **ecbdata** API allows for easy querying of data from the
 [ECB Data Portal](https://data.ecb.europa.eu/help/data/overview). ##
 Installation You can install with pip as: `pip install ecbdata` ### Example
```

### Comparing `ecbdata-0.0.5/setup.py` & `ecbdata-0.0.6/setup.py`

 * *Files identical despite different names*

