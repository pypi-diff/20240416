# Comparing `tmp/pyield-0.7.0.tar.gz` & `tmp/pyield-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyield-0.7.0.tar", last modified: Sun Apr 14 11:32:13 2024, max compression
+gzip compressed data, was "pyield-0.7.1.tar", last modified: Tue Apr 16 12:02:47 2024, max compression
```

## Comparing `pyield-0.7.0.tar` & `pyield-0.7.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0     1072 2023-12-14 08:54:49.496702 pyield-0.7.0/LICENSE
--rw-r--r--   0        0        0     5141 2024-04-14 11:20:50.781990 pyield-0.7.0/README.md
--rw-r--r--   0        0        0       22 2024-04-14 09:19:00.737098 pyield-0.7.0/pyield/__about__.py
--rw-r--r--   0        0        0      380 2024-04-14 09:19:55.868897 pyield-0.7.0/pyield/__init__.py
--rw-r--r--   0        0        0    13136 2024-04-13 12:39:44.026704 pyield-0.7.0/pyield/bday.py
--rw-r--r--   0        0        0     3239 2024-04-14 11:09:53.384322 pyield-0.7.0/pyield/data_access.py
--rw-r--r--   0        0        0     1250 2024-04-13 12:39:44.026704 pyield-0.7.0/pyield/data_analysis.py
--rw-r--r--   0        0        0       90 2024-04-13 12:39:44.026704 pyield-0.7.0/pyield/di/__init__.py
--rw-r--r--   0        0        0     6990 2024-04-13 12:39:44.026704 pyield-0.7.0/pyield/di/core.py
--rw-r--r--   0        0        0     9638 2024-04-13 12:39:44.027704 pyield-0.7.0/pyield/di/web.py
--rw-r--r--   0        0        0     9551 2024-04-13 12:39:44.027704 pyield-0.7.0/pyield/di/xml.py
--rw-r--r--   0        0        0       55 2024-04-06 05:23:30.068485 pyield-0.7.0/pyield/holidays/__init__.py
--rw-r--r--   0        0        0    14278 2024-01-16 09:33:28.571746 pyield-0.7.0/pyield/holidays/br_holidays_new.txt
--rw-r--r--   0        0        0    14314 2023-12-28 23:26:42.737321 pyield-0.7.0/pyield/holidays/br_holidays_old.txt
--rw-r--r--   0        0        0     2192 2024-04-07 10:57:52.523509 pyield-0.7.0/pyield/holidays/core.py
--rw-r--r--   0        0        0     2273 2024-04-14 11:04:04.016185 pyield-0.7.0/pyield/indicators.py
--rw-r--r--   0        0        0        0 2024-03-24 19:54:34.284748 pyield-0.7.0/pyield/py.typed
--rw-r--r--   0        0        0     6601 2024-04-14 09:38:16.555877 pyield-0.7.0/pyield/treasuries.py
--rw-r--r--   0        0        0     2111 2024-04-14 09:43:03.423065 pyield-0.7.0/pyield/utils.py
--rw-r--r--   0        0        0     1165 2024-04-14 11:32:13.110039 pyield-0.7.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-14 18:12:36.515393 pyield-0.7.0/tests/__init__.py
--rw-r--r--   0        0        0     1114 2024-04-13 12:39:44.028704 pyield-0.7.0/tests/test_br_calendar.py
--rw-r--r--   0        0        0     2503 2024-04-13 12:39:44.028704 pyield-0.7.0/tests/test_di.py
--rw-r--r--   0        0        0     7158 1970-01-01 00:00:00.000000 pyield-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-12-14 08:54:49.496702 pyield-0.7.1/LICENSE
+-rw-r--r--   0        0        0     5168 2024-04-16 12:01:55.675922 pyield-0.7.1/README.md
+-rw-r--r--   0        0        0       22 2024-04-16 12:01:55.675922 pyield-0.7.1/pyield/__about__.py
+-rw-r--r--   0        0        0      380 2024-04-14 09:19:55.868897 pyield-0.7.1/pyield/__init__.py
+-rw-r--r--   0        0        0    13136 2024-04-13 12:39:44.026704 pyield-0.7.1/pyield/bday.py
+-rw-r--r--   0        0        0     3446 2024-04-16 12:01:55.675922 pyield-0.7.1/pyield/data_access.py
+-rw-r--r--   0        0        0     1250 2024-04-13 12:39:44.026704 pyield-0.7.1/pyield/data_analysis.py
+-rw-r--r--   0        0        0      223 2024-04-16 12:01:55.675922 pyield-0.7.1/pyield/futures/__init__.py
+-rw-r--r--   0        0        0     5615 2024-04-16 12:01:55.676922 pyield-0.7.1/pyield/futures/common.py
+-rw-r--r--   0        0        0     5816 2024-04-16 12:01:55.676922 pyield-0.7.1/pyield/futures/ddi.py
+-rw-r--r--   0        0        0     5847 2024-04-16 12:01:55.676922 pyield-0.7.1/pyield/futures/di.py
+-rw-r--r--   0        0        0    11530 2024-04-16 12:01:55.676922 pyield-0.7.1/pyield/futures/di_xml.py
+-rw-r--r--   0        0        0       55 2024-04-06 05:23:30.068485 pyield-0.7.1/pyield/holidays/__init__.py
+-rw-r--r--   0        0        0    14278 2024-01-16 09:33:28.571746 pyield-0.7.1/pyield/holidays/br_holidays_new.txt
+-rw-r--r--   0        0        0    14314 2023-12-28 23:26:42.737321 pyield-0.7.1/pyield/holidays/br_holidays_old.txt
+-rw-r--r--   0        0        0     2192 2024-04-07 10:57:52.523509 pyield-0.7.1/pyield/holidays/core.py
+-rw-r--r--   0        0        0     2273 2024-04-14 11:04:04.016185 pyield-0.7.1/pyield/indicators.py
+-rw-r--r--   0        0        0        0 2024-03-24 19:54:34.284748 pyield-0.7.1/pyield/py.typed
+-rw-r--r--   0        0        0     6612 2024-04-16 12:01:55.676922 pyield-0.7.1/pyield/treasuries.py
+-rw-r--r--   0        0        0     2111 2024-04-14 09:43:03.423065 pyield-0.7.1/pyield/utils.py
+-rw-r--r--   0        0        0     1165 2024-04-16 12:02:47.053532 pyield-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-14 18:12:36.515393 pyield-0.7.1/tests/__init__.py
+-rw-r--r--   0        0        0     1114 2024-04-16 12:01:55.676922 pyield-0.7.1/tests/test_bday.py
+-rw-r--r--   0        0        0     2554 2024-04-16 12:01:55.677922 pyield-0.7.1/tests/test_futures.py
+-rw-r--r--   0        0        0     7185 1970-01-01 00:00:00.000000 pyield-0.7.1/PKG-INFO
```

### Comparing `pyield-0.7.0/LICENSE` & `pyield-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyield-0.7.0/README.md` & `pyield-0.7.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [![Made with Python](https://img.shields.io/badge/Python->=3.11-blue?logo=python&logoColor=white)](https://python.org "Go to Python homepage")
 [![License](https://img.shields.io/badge/License-MIT-blue)](#license)
 
 # PYield: Fixed Income Toolbox for Brazilian Markets
 
 ## Introduction
 
-Welcome to PYield, a Python library designed for the analysis of fixed income instruments in Brazil. This library is tailored for financial analysts, researchers, and enthusiasts interested in the Brazilian fixed income market. Leveraging the power of popular Python libraries like Pandas and Requests, PYield simplifies the process of obtaining and processing data from key sources such as ANBIMA and B3.
+Welcome to PYield, a Python library designed for the analysis of fixed income instruments in Brazil. This library is tailored for financial analysts, researchers, and enthusiasts interested in the Brazilian fixed income market. Leveraging the power of popular Python libraries like Pandas and Requests, PYield simplifies the process of obtaining and processing data from key sources such as ANBIMA, BCB, IBGE and B3.
 
 ## Features
 
 - **Data Collection**: Automated fetching of data from ANBIMA and B3.
 - **Data Processing**: Efficient processing and normalization of fixed income data.
 - **Analysis Tools**: Built-in functions for common analysis tasks in fixed income markets.
 - **Easy Integration**: Seamless integration with pandas data analysis workflows.
@@ -55,22 +55,22 @@
 ```
 
 ### Futures Data
 ```python
 # Fetch a DataFrame with the DI Futures data from B3
 >>> yd.fetch_asset(asset_code="DI1", reference_date='2024-03-08')
 
-TradeDate  ExpirationCode ExpirationDate BDToExpiration  ... LastRate LastAskRate LastBidRate SettlementRate
-2024-03-08 J24            2024-04-01     15              ... 10.952   10.952      10.956      10.956
-2024-03-08 K24            2024-05-02     37              ... 10.776   10.774      10.780      10.777
-2024-03-08 M24            2024-06-03     58              ... 10.604   10.602      10.604      10.608
-...        ...            ...            ...             ... ...      ...         ...         ...
-2024-03-08 F37            2037-01-02     3213            ... <NA>     <NA>        <NA>        10.859
-2024-03-08 F38            2038-01-04     3462            ... <NA>     <NA>        <NA>        10.859
-2024-03-08 F39            2039-01-03     3713            ... <NA>     <NA>        <NA>        10.85
+TradeDate  ExpirationCode ExpirationDate BDaysToExpiration ... LastRate LastAskRate LastBidRate SettlementRate
+2024-03-08 J24            2024-04-01     15                ... 10.952   10.952      10.956      10.956
+2024-03-08 K24            2024-05-02     37                ... 10.776   10.774      10.780      10.777
+2024-03-08 M24            2024-06-03     58                ... 10.604   10.602      10.604      10.608
+...        ...            ...            ...               ... ...      ...         ...         ...
+2024-03-08 F37            2037-01-02     3213              ... <NA>     <NA>        <NA>        10.859
+2024-03-08 F38            2038-01-04     3462              ... <NA>     <NA>        <NA>        10.859
+2024-03-08 F39            2039-01-03     3713              ... <NA>     <NA>        <NA>        10.85
 ```
 
 ### Treasury Bonds Data
 ```python
 # Fetch a DataFrame with the NTN-B data from ANBIMA
 # Anbima data is available for the last 5 working days
 # Obs: Anbima members have access to the full history
```

### Comparing `pyield-0.7.0/pyield/bday.py` & `pyield-0.7.1/pyield/bday.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.0/pyield/data_access.py` & `pyield-0.7.1/pyield/data_access.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
 
-from . import di
-from . import indicators as ir
+from . import futures as ft
+from . import indicators as it
 from . import treasuries as tr
 from .utils import _normalize_date
 
 
 def fetch_asset(
     asset_code: str,
     reference_date: str | pd.Timestamp | None = None,
@@ -16,15 +16,16 @@
 
     Args:
         asset_code (str): The asset code identifying the type of financial asset.
         Supported options:
             - "TRB": Treasury bonds (indicative rates from ANBIMA).
             - "LTN", "LFT", "NTN-F", "NTN-B": Specific types of Brazilian treasury bonds
                   (indicative rates from ANBIMA).
-            - "DI1": DI Futures rates from B3.
+            - "DI1": One-day Interbank Deposit Futures (Futuro de DI) from B3.
+            - "DDI": DI x U.S. Dollar Spread Futures (Futuro de Cupom Cambial) from B3.
         reference_date (str | pd.Timestamp | None): The reference date for which data is
             fetched. Defaults to the previous business day if None.
         **kwargs: Additional keyword arguments, specifically:
             - return_raw (bool): Whether to return raw data without processing. Defaults
               to False.
 
     Returns:
@@ -37,23 +38,23 @@
         >>> fetch_asset('TRB', '2023-04-01')
         >>> fetch_asset('DI1', '2023-04-01', return_raw=True)
     """
     return_raw = kwargs.get("return_raw", False)
     normalized_date = _normalize_date(reference_date)
 
     if asset_code.lower() == "trb":
-        return tr.fetch_data(reference_date=normalized_date, return_raw=return_raw)
+        return tr.fetch_bonds(reference_date=normalized_date, return_raw=return_raw)
     elif asset_code.lower() in ["ltn", "lft", "ntn-f", "ntn-b"]:
-        df = tr.fetch_data(reference_date=normalized_date)
+        df = tr.fetch_bonds(reference_date=normalized_date)
         return df.query(f"BondType == '{asset_code.upper()}'")
 
     elif asset_code.lower() == "di1":
-        return di.fetch_data(
-            trade_date=normalized_date, source_type="bmf", return_raw=return_raw
-        )
+        return ft.fetch_di(trade_date=normalized_date, return_raw=return_raw)
+    elif asset_code.lower() == "ddi":
+        return ft.fetch_ddi(trade_date=normalized_date, return_raw=return_raw)
     else:
         raise ValueError("Asset type not supported.")
 
 
 def fetch_indicator(
     indicator_code: str,
     reference_date: str | pd.Timestamp | None = None,
@@ -77,12 +78,12 @@
     Examples:
         >>> fetch_indicator('SELIC', '2023-04-01')
         >>> fetch_indicator('IPCA', '2023-04-01')
     """
     normalized_date = _normalize_date(reference_date)
 
     if indicator_code.lower() == "selic":
-        return ir.fetch_selic_target(reference_date=normalized_date)
+        return it.fetch_selic_target(reference_date=normalized_date)
     elif indicator_code.lower() == "ipca":
-        return ir.fetch_ipca_mr(reference_date=normalized_date)
+        return it.fetch_ipca_mr(reference_date=normalized_date)
     else:
         raise ValueError("Indicator type not supported.")
```

### Comparing `pyield-0.7.0/pyield/data_analysis.py` & `pyield-0.7.1/pyield/data_analysis.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.0/pyield/di/xml.py` & `pyield-0.7.1/pyield/futures/di_xml.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import pandas as pd
 import requests
 from lxml import etree
 from pandas import DataFrame, Timestamp
 
 from .. import bday
-from . import core as cr
+from . import common as cm
 
 
 def _get_file_from_url(trade_date: Timestamp, source_type: str) -> io.BytesIO:
     """
     Types of XML files available:
     Full Price Report (all assets)
         - aprox. 5 MB zipped file;
@@ -93,20 +93,20 @@
         else:
             # Handle the case where tckr_symb is not an _Element
             continue
 
         # Extrair a data de negociação
         if price_report is None:
             continue
-        trade_date = price_report.find(".//ns:TradDt/ns:Dt", namespaces)
+        trade_date = price_report.find(".//ns:TradeDate/ns:Dt", namespaces)
 
         # Preparar o dicionário de dados do ticker com a data de negociação
         if trade_date is None:
             continue
-        ticker_data = {"TradDt": trade_date.text, "TckrSymb": tckr_symb.text}
+        ticker_data = {"TradeDate": trade_date.text, "TckrSymb": tckr_symb.text}
 
         # Acessar o elemento FinInstrmAttrbts que contém o TckrSymb
         fin_instrm_attrbts = price_report.find(".//ns:FinInstrmAttrbts", namespaces)
         # Verificar se FinInstrmAttrbts existe
         if fin_instrm_attrbts is None:
             continue  # Pular para o próximo TckrSymb se FinInstrmAttrbts não existir
         # Extrair os dados de FinInstrmAttrbts
@@ -225,25 +225,25 @@
 
 
 def _process_di_df(df_raw: DataFrame) -> DataFrame:
     df = df_raw.copy()
     # Convert to datetime64[ns] since it is pandas default type for timestamps
     df["TradDt"] = df["TradDt"].astype("datetime64[ns]")
 
-    expiration = df["TckrSymb"].str[3:].apply(cr.get_expiration_date)
+    expiration = df["TckrSymb"].str[3:].apply(cm.get_expiration_date)
     df.insert(2, "ExpirationDate", expiration)
 
     business_days = bday.count_bdays(df["TradDt"], df["ExpirationDate"])
-    df.insert(3, "BDToExpiration", business_days)
+    df.insert(3, "BDaysToExpiration", business_days)
 
     # Convert to nullable integer, since other columns use this data type
-    df["BDToExpiration"] = df["BDToExpiration"].astype(pd.Int64Dtype())
+    df["BDaysToExpiration"] = df["BDaysToExpiration"].astype(pd.Int64Dtype())
 
     # Remove expired contracts
-    df.query("BDToExpiration > 0", inplace=True)
+    df.query("BDaysToExpiration > 0", inplace=True)
 
     return df.sort_values(by=["ExpirationDate"], ignore_index=True)
 
 
 def read_xml(trade_date: Timestamp, source_type: str, return_raw: bool) -> DataFrame:
     zip_file = _get_file_from_url(trade_date, source_type)
 
@@ -303,7 +303,47 @@
         # Standardize column names
         df_di = _standardize_column_names(df_di)
 
         return df_di
 
     else:
         raise ValueError("A file path must be provided.")
+
+
+def read_file(file_path: Path, return_raw: bool = False) -> pd.DataFrame:
+    """
+    Reads DI futures data from a file and returns it as a pandas DataFrame.
+
+    This function opens and reads a DI futures data file, returning the contents as a
+    pandas DataFrame. It supports reading from both XML files provided by B3, wich
+    are the simplified and complete Price Reports.
+
+    Args:
+        file_path (Path): The file path to the DI data file. This should be a valid
+            Path object pointing to the location of the file.
+        return_raw (bool, optional): If set to True, the function returns the raw data
+            without applying any transformation or processing. Useful for cases where
+            raw data inspection or custom processing is needed. Defaults to False.
+        source_type (Literal["bmf", "b3", "b3s"], optional): Indicates the source of
+            the data. Defaults to "bmf". Options include:
+                - "bmf": Fetches data from the old BM&FBOVESPA website. Fastest option.
+                - "b3": Fetches data from the complete Price Report (XML file) provided
+                    by B3.
+                - "b3s": Fetches data from the simplified Price Report (XML file)
+                    provided by B3. Faster than "b3" but less detailed.
+
+    Returns:
+        pd.DataFrame: A DataFrame containing the processed or raw DI futures data,
+            depending on the `return_raw` flag.
+
+    Examples:
+        >>> read_di(Path("path/to/di_data_file.xml"))
+        # returns a DataFrame with the DI futures data
+
+        >>> read_di(Path("path/to/di_data_file.xml"), return_raw=True)
+        # returns a DataFrame with the raw DI futures data, without processing
+
+    Note:
+        The ability to process and return raw data is primarily intended for advanced
+        users who require access to the data in its original form for custom analyses.
+    """
+    return read_di(file_path, return_raw=return_raw)
```

### Comparing `pyield-0.7.0/pyield/holidays/br_holidays_new.txt` & `pyield-0.7.1/pyield/holidays/br_holidays_new.txt`

 * *Files identical despite different names*

### Comparing `pyield-0.7.0/pyield/holidays/br_holidays_old.txt` & `pyield-0.7.1/pyield/holidays/br_holidays_old.txt`

 * *Files identical despite different names*

### Comparing `pyield-0.7.0/pyield/holidays/core.py` & `pyield-0.7.1/pyield/holidays/core.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.0/pyield/indicators.py` & `pyield-0.7.1/pyield/indicators.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.0/pyield/treasuries.py` & `pyield-0.7.1/pyield/treasuries.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import io
 
 import pandas as pd
 import requests
 
-from . import di
+from . import futures as ft
 
 # URL Constants
 ANBIMA_NON_MEMBER_URL = "https://www.anbima.com.br/informacoes/merc-sec/arqs/"
 ANBIMA_MEMBER_URL = "http://www.anbima.associados.rtm/merc_sec/arqs/"
 
 # Constant for conversion to basis points
 BPS_CONVERSION_FACTOR = 10_000
@@ -96,15 +96,15 @@
 
     df["ReferenceDate"] = pd.to_datetime(df["ReferenceDate"], format="%Y%m%d")
     df["MaturityDate"] = pd.to_datetime(df["MaturityDate"], format="%Y%m%d")
 
     return df.sort_values(["BondType", "MaturityDate"], ignore_index=True)
 
 
-def fetch_data(reference_date: pd.Timestamp, return_raw=False) -> pd.DataFrame:
+def fetch_bonds(reference_date: pd.Timestamp, return_raw=False) -> pd.DataFrame:
     """
     Fetches indicative treasury rates from ANBIMA for a specified reference date.
 
     This function retrieves the indicative rates for Brazilian treasury securities
     from ANBIMA, processing them into a structured pandas DataFrame.
     There is an option to return raw data directly from the source without processing.
 
@@ -146,24 +146,24 @@
 
     Returns:
         pd.DataFrame: A DataFrame containing the bond type, reference date, maturity
             date, and the calculated DI spread in basis points. The data is sorted by
             bond type and maturity date.
     """
     # Fetch DI rates and adjust the maturity date format for compatibility
-    df_di = di.fetch_data(reference_date)[["ExpirationDate", "SettlementRate"]]
+    df_di = ft.fetch_di(reference_date)[["ExpirationDate", "SettlementRate"]]
 
     # Renaming the columns to match the ANBIMA structure
     df_di.rename(columns={"ExpirationDate": "MaturityDate"}, inplace=True)
 
     # Adjusting maturity date to match bond data format
     df_di["MaturityDate"] = df_di["MaturityDate"].dt.to_period("M").dt.to_timestamp()
 
     # Fetch bond rates, filtering for LTN and NTN-F types
-    df_anbima = fetch_data(reference_date, False)
+    df_anbima = fetch_bonds(reference_date, False)
     df_anbima.query("BondType in ['LTN', 'NTN-F']", inplace=True)
 
     # Merge bond and DI rates by maturity date to calculate spreads
     df_final = pd.merge(df_anbima, df_di, how="left", on="MaturityDate")
 
     # Calculate the DI spread as the difference between indicative and settlement rates
     df_final["DISpread"] = df_final["IndicativeRate"] - df_final["SettlementRate"]
```

### Comparing `pyield-0.7.0/pyield/utils.py` & `pyield-0.7.1/pyield/utils.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.0/pyproject.toml` & `pyield-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "pandas>=2.0.0",
     "numpy",
     "beautifulsoup4",
     "html5lib",
     "lxml",
 ]
 dynamic = []
-version = "0.7.0"
+version = "0.7.1"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Source = "https://github.com/crdcj/PYield"
```

### Comparing `pyield-0.7.0/tests/test_br_calendar.py` & `pyield-0.7.1/tests/test_bday.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import pandas as pd
 import numpy as np
+import pandas as pd
 
 import pyield as yd
 
 
 def test_count_bdays_1():
     start = "2023-01-01"
     end = "2023-01-08"
```

### Comparing `pyield-0.7.0/tests/test_di.py` & `pyield-0.7.1/tests/test_futures.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 import pandas as pd
 import pytest
 
-from pyield.di import core as cr
-from pyield.di import web as web
+from pyield import futures as ft
 
 
 def test_valid_old_contract_code1():
     expiration_code = "JAN3"  # Valid contract code
     trade_date = pd.Timestamp("2001-05-21")
-    result = web.get_old_expiration_date(expiration_code, trade_date)
+    result = ft.get_old_expiration_date(expiration_code, trade_date)
     contract_expiration = pd.Timestamp("2003-01-02")
     assert result == contract_expiration
 
 
 def test_valid_old_contract_code2():
     expiration_code = "JAN3"  # Valid contract code
     trade_date = pd.Timestamp("1990-01-01")
-    result = web.get_old_expiration_date(expiration_code, trade_date)
+    result = ft.get_old_expiration_date(expiration_code, trade_date)
     contract_expiration = pd.Timestamp("1993-01-04")
     assert result == contract_expiration
 
 
 def test_invalid_old_contract_code():
     expiration_code = "J3"  # Invalid contract code
     trade_date = pd.Timestamp("2001-01-02")
     # Must return NaT
-    result = web.get_old_expiration_date(expiration_code, trade_date)
+    result = ft.get_old_expiration_date(expiration_code, trade_date)
     assert pd.isnull(result)
 
 
 def test_new_contract_code():
     expiration_code = "F23"  # Valid contract code
-    result = cr.get_expiration_date(expiration_code)
+    result = ft.get_expiration_date(expiration_code)
     contract_expiration = pd.Timestamp("2023-01-02")
     assert result == contract_expiration
 
 
 def test_settlement_rate_with_old_holiday_list():
     settlement_rates = {
         "N27": 0.09809,
         "F33": 0.10368,
     }
 
     # 22-12-2023 is before the new holiday calendar
-    df = cr.fetch_data(trade_date="2023-12-22")
+    test_date = pd.Timestamp("2023-12-22")
+    df = ft.fetch_di(trade_date=test_date)
     expiration_codes = list(settlement_rates.keys())  # noqa: F841
     result = df.query("ExpirationCode in @expiration_codes")["SettlementRate"].to_list()
     assert result == list(settlement_rates.values())
 
 
 def test_settlement_rates_with_current_holiday_list():
     settlement_rates = {
@@ -63,20 +63,20 @@
         "N26": 0.09631,
         "F27": 0.09683,
         "N27": 0.09794,
         "F29": 0.10042,
         "F31": 0.10240,
         "F33": 0.10331,
     }
-
-    df = cr.fetch_data(trade_date="2023-12-26")
+    test_date = pd.Timestamp("2023-12-26")
+    df = ft.fetch_di(trade_date=test_date)
     expiration_codes = list(settlement_rates.keys())  # noqa: F841
     results = df.query("ExpirationCode in @expiration_codes")[
         "SettlementRate"
     ].to_list()
     assert results == list(settlement_rates.values())
 
 
 def test_non_business_day():
-    non_business_day = "2023-12-24"
+    non_business_day = pd.Timestamp("2023-12-24")
     with pytest.raises(ValueError):
-        cr.fetch_data(trade_date=non_business_day)
+        ft.fetch_di(trade_date=non_business_day)
```

### Comparing `pyield-0.7.0/PKG-INFO` & `pyield-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PYield
-Version: 0.7.0
+Version: 0.7.1
 Summary: A Python library for analysis of fixed income instruments in Brazil
 Keywords: fixed-income, brazil, finance, analysis, bonds
 Author-Email: Carlos Carvalho <cr.cj@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Carlos Carvalho
         
@@ -44,15 +44,15 @@
 [![Made with Python](https://img.shields.io/badge/Python->=3.11-blue?logo=python&logoColor=white)](https://python.org "Go to Python homepage")
 [![License](https://img.shields.io/badge/License-MIT-blue)](#license)
 
 # PYield: Fixed Income Toolbox for Brazilian Markets
 
 ## Introduction
 
-Welcome to PYield, a Python library designed for the analysis of fixed income instruments in Brazil. This library is tailored for financial analysts, researchers, and enthusiasts interested in the Brazilian fixed income market. Leveraging the power of popular Python libraries like Pandas and Requests, PYield simplifies the process of obtaining and processing data from key sources such as ANBIMA and B3.
+Welcome to PYield, a Python library designed for the analysis of fixed income instruments in Brazil. This library is tailored for financial analysts, researchers, and enthusiasts interested in the Brazilian fixed income market. Leveraging the power of popular Python libraries like Pandas and Requests, PYield simplifies the process of obtaining and processing data from key sources such as ANBIMA, BCB, IBGE and B3.
 
 ## Features
 
 - **Data Collection**: Automated fetching of data from ANBIMA and B3.
 - **Data Processing**: Efficient processing and normalization of fixed income data.
 - **Analysis Tools**: Built-in functions for common analysis tasks in fixed income markets.
 - **Easy Integration**: Seamless integration with pandas data analysis workflows.
@@ -97,22 +97,22 @@
 ```
 
 ### Futures Data
 ```python
 # Fetch a DataFrame with the DI Futures data from B3
 >>> yd.fetch_asset(asset_code="DI1", reference_date='2024-03-08')
 
-TradeDate  ExpirationCode ExpirationDate BDToExpiration  ... LastRate LastAskRate LastBidRate SettlementRate
-2024-03-08 J24            2024-04-01     15              ... 10.952   10.952      10.956      10.956
-2024-03-08 K24            2024-05-02     37              ... 10.776   10.774      10.780      10.777
-2024-03-08 M24            2024-06-03     58              ... 10.604   10.602      10.604      10.608
-...        ...            ...            ...             ... ...      ...         ...         ...
-2024-03-08 F37            2037-01-02     3213            ... <NA>     <NA>        <NA>        10.859
-2024-03-08 F38            2038-01-04     3462            ... <NA>     <NA>        <NA>        10.859
-2024-03-08 F39            2039-01-03     3713            ... <NA>     <NA>        <NA>        10.85
+TradeDate  ExpirationCode ExpirationDate BDaysToExpiration ... LastRate LastAskRate LastBidRate SettlementRate
+2024-03-08 J24            2024-04-01     15                ... 10.952   10.952      10.956      10.956
+2024-03-08 K24            2024-05-02     37                ... 10.776   10.774      10.780      10.777
+2024-03-08 M24            2024-06-03     58                ... 10.604   10.602      10.604      10.608
+...        ...            ...            ...               ... ...      ...         ...         ...
+2024-03-08 F37            2037-01-02     3213              ... <NA>     <NA>        <NA>        10.859
+2024-03-08 F38            2038-01-04     3462              ... <NA>     <NA>        <NA>        10.859
+2024-03-08 F39            2039-01-03     3713              ... <NA>     <NA>        <NA>        10.85
 ```
 
 ### Treasury Bonds Data
 ```python
 # Fetch a DataFrame with the NTN-B data from ANBIMA
 # Anbima data is available for the last 5 working days
 # Obs: Anbima members have access to the full history
```

