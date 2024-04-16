# Comparing `tmp/openseries-1.5.1.tar.gz` & `tmp/openseries-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openseries-1.5.1.tar", max compression
+gzip compressed data, was "openseries-1.5.2.tar", max compression
```

## Comparing `openseries-1.5.1.tar` & `openseries-1.5.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1521 2024-03-30 15:10:24.019535 openseries-1.5.1/LICENSE.md
--rw-r--r--   0        0        0    42093 2024-03-30 15:10:24.019535 openseries-1.5.1/README.md
--rw-r--r--   0        0        0       41 2024-03-30 15:10:24.019535 openseries-1.5.1/openseries/__init__.py
--rw-r--r--   0        0        0    72469 2024-03-30 15:10:24.019535 openseries-1.5.1/openseries/_common_model.py
--rw-r--r--   0        0        0     3299 2024-03-30 15:10:24.019535 openseries-1.5.1/openseries/_risk.py
--rw-r--r--   0        0        0    12423 2024-03-30 15:10:24.019535 openseries-1.5.1/openseries/datefixer.py
--rw-r--r--   0        0        0    73772 2024-03-30 15:10:24.019535 openseries-1.5.1/openseries/frame.py
--rw-r--r--   0        0        0     1807 2024-03-30 15:10:24.019535 openseries-1.5.1/openseries/load_plotly.py
--rw-r--r--   0        0        0      178 2024-03-30 15:10:24.019535 openseries-1.5.1/openseries/plotly_captor_logo.json
--rw-r--r--   0        0        0     1429 2024-03-30 15:10:24.019535 openseries-1.5.1/openseries/plotly_layouts.json
--rw-r--r--   0        0        0    28312 2024-03-30 15:10:24.019535 openseries-1.5.1/openseries/series.py
--rw-r--r--   0        0        0    13550 2024-03-30 15:10:24.019535 openseries-1.5.1/openseries/simulation.py
--rw-r--r--   0        0        0     7660 2024-03-30 15:10:24.019535 openseries-1.5.1/openseries/types.py
--rw-r--r--   0        0        0     2712 2024-03-30 15:10:24.023535 openseries-1.5.1/pyproject.toml
--rw-r--r--   0        0        0    43665 1970-01-01 00:00:00.000000 openseries-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1521 2024-04-16 08:07:42.908003 openseries-1.5.2/LICENSE.md
+-rw-r--r--   0        0        0    42091 2024-04-16 08:07:42.908003 openseries-1.5.2/README.md
+-rw-r--r--   0        0        0       41 2024-04-16 08:07:42.908003 openseries-1.5.2/openseries/__init__.py
+-rw-r--r--   0        0        0    72468 2024-04-16 08:07:42.908003 openseries-1.5.2/openseries/_common_model.py
+-rw-r--r--   0        0        0     3299 2024-04-16 08:07:42.908003 openseries-1.5.2/openseries/_risk.py
+-rw-r--r--   0        0        0    12377 2024-04-16 08:07:42.908003 openseries-1.5.2/openseries/datefixer.py
+-rw-r--r--   0        0        0    73772 2024-04-16 08:07:42.908003 openseries-1.5.2/openseries/frame.py
+-rw-r--r--   0        0        0     1807 2024-04-16 08:07:42.908003 openseries-1.5.2/openseries/load_plotly.py
+-rw-r--r--   0        0        0      178 2024-04-16 08:07:42.908003 openseries-1.5.2/openseries/plotly_captor_logo.json
+-rw-r--r--   0        0        0     1429 2024-04-16 08:07:42.908003 openseries-1.5.2/openseries/plotly_layouts.json
+-rw-r--r--   0        0        0    28312 2024-04-16 08:07:42.908003 openseries-1.5.2/openseries/series.py
+-rw-r--r--   0        0        0    13549 2024-04-16 08:07:42.908003 openseries-1.5.2/openseries/simulation.py
+-rw-r--r--   0        0        0     7597 2024-04-16 08:07:42.908003 openseries-1.5.2/openseries/types.py
+-rw-r--r--   0        0        0     2664 2024-04-16 08:07:42.908003 openseries-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0    43661 1970-01-01 00:00:00.000000 openseries-1.5.2/PKG-INFO
```

### Comparing `openseries-1.5.1/LICENSE.md` & `openseries-1.5.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openseries-1.5.1/README.md` & `openseries-1.5.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 <img src="https://sales.captor.se/captor_logo_sv_1600_icketransparent.png" alt="Captor
 Fund Management AB"
 width="81" height="100" align="left" float="right"/><br/>
 
 <br><br>
 
-# OpenSeries
+# openseries
 
 [![PyPI version](https://img.shields.io/pypi/v/openseries.svg)](https://pypi.org/project/openseries/)
 [![Conda version](https://img.shields.io/conda/vn/conda-forge/openseries.svg)](https://anaconda.org/conda-forge/openseries)
 [![Conda platforms](https://img.shields.io/conda/pn/conda-forge/openseries.svg)](https://anaconda.org/conda-forge/openseries)
 [![Python version](https://img.shields.io/pypi/pyversions/openseries.svg)](https://www.python.org/)
-[![GitHub Action Test Suite](https://github.com/CaptorAB/OpenSeries/actions/workflows/test.yml/badge.svg)](https://github.com/CaptorAB/OpenSeries/actions/workflows/test.yml)
-[![Coverage](https://cdn.jsdelivr.net/gh/CaptorAB/OpenSeries@master/coverage.svg)](https://github.com/CaptorAB/OpenSeries/actions/workflows/test.yml)
-[![Styling, Linting & Type checks](https://github.com/CaptorAB/OpenSeries/actions/workflows/check.yml/badge.svg)](https://github.com/CaptorAB/OpenSeries/actions/workflows/check.yml)
+[![GitHub Action Test Suite](https://github.com/CaptorAB/openseries/actions/workflows/test.yml/badge.svg)](https://github.com/CaptorAB/openseries/actions/workflows/test.yml)
+[![Coverage](https://cdn.jsdelivr.net/gh/CaptorAB/openseries@master/coverage.svg)](https://github.com/CaptorAB/openseries/actions/workflows/test.yml)
+[![Styling, Linting & Type checks](https://github.com/CaptorAB/openseries/actions/workflows/check.yml/badge.svg)](https://github.com/CaptorAB/openseries/actions/workflows/check.yml)
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://beta.ruff.rs/docs/)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 
-**OpenSeries** is a project with tools to analyse financial timeseries of a single
+`openseries` is a project with tools to analyse financial timeseries of a single
 asset or a group of assets. It is solely made for daily or less frequent data.
 
-<span style="font-size:2em;">[CHANGELOG](https://github.com/CaptorAB/OpenSeries/blob/master/CHANGELOG.md)</span>
+<span style="font-size:2em;">[CHANGELOG](https://github.com/CaptorAB/openseries/blob/master/CHANGELOG.md)</span>
 
 
 ## Basic Usage
 
 To install:
 
 ```bash
@@ -98,38 +98,38 @@
 the [Pydantic BaseModel](https://docs.pydantic.dev/usage/models/). Please refer to its documentation for information
 on any attributes or methods inherited from this model.
 
 
 ### Windows Powershell
 
 ```powershell
-git clone https://github.com/CaptorAB/OpenSeries.git
-cd OpenSeries
+git clone https://github.com/CaptorAB/openseries.git
+cd openseries
 ./make.ps1 make
 
 ```
 
 ### Mac Terminal/Linux
 
 ```bash
-git clone https://github.com/CaptorAB/OpenSeries.git
-cd OpenSeries
+git clone https://github.com/CaptorAB/openseries.git
+cd openseries
 make
 source source_me
 make install
 
 ```
 
 ## Testing and Linting / Type-checking
 
 Ruff and Mypy checking is embedded in the pre-commit hook. Both
 are also used in the project's GitHub workflows and are run when the `lint`
 alternative is chosen in the below commands.
 Any silenced error codes can be found in the
-[pyproject.toml](https://github.com/CaptorAB/OpenSeries/blob/master/pyproject.toml)
+[pyproject.toml](https://github.com/CaptorAB/openseries/blob/master/pyproject.toml)
 file or in in-line comments.
 
 ### Windows Powershell
 
 ```powershell
 ./make.ps1 test
 ./make.ps1 lint
@@ -161,28 +161,28 @@
 - [Numerical properties for both classes](#numerical-properties-available-for-individual-opentimeseries-or-on-all-series-in-an-openframe)
 - [Numerical methods with period arguments for both classes](#methods-below-are-identical-to-the-numerical-properties-above)
 
 ### On some files in the project
 
 | File                                                                                                             | Description                                                                                                                                                                                                                               |
 |:-----------------------------------------------------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| [series.py](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/series.py)                             | Defines the class _OpenTimeSeries_ for managing and analyzing a single timeseries. The module also defines a function `timeseries_chain` that can be used to chain two timeseries objects together.                                       |
-| [frame.py](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/frame.py)                               | Defines the class _OpenFrame_ for managing a group of timeseries, and e.g. calculate a portfolio timeseries from a rebalancing strategy between timeseries. The module also defines functions to simulate, optimize, and plot portfolios. |
-| [simulation.py](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/simulation.py)                     | Defines the class _ReturnSimulation_ to create simulated financial timeseries. Used in the project's test suite                                                                                                                           |
+| [series.py](https://github.com/CaptorAB/openseries/blob/master/openseries/series.py)                             | Defines the class _OpenTimeSeries_ for managing and analyzing a single timeseries. The module also defines a function `timeseries_chain` that can be used to chain two timeseries objects together.                                       |
+| [frame.py](https://github.com/CaptorAB/openseries/blob/master/openseries/frame.py)                               | Defines the class _OpenFrame_ for managing a group of timeseries, and e.g. calculate a portfolio timeseries from a rebalancing strategy between timeseries. The module also defines functions to simulate, optimize, and plot portfolios. |
+| [simulation.py](https://github.com/CaptorAB/openseries/blob/master/openseries/simulation.py)                     | Defines the class _ReturnSimulation_ to create simulated financial timeseries. Used in the project's test suite                                                                                                                           |
 
 ### Class methods used to construct objects.
 
 | Method            | Applies to                    | Description                                                                                        |
 |:------------------|:------------------------------|:---------------------------------------------------------------------------------------------------|
 | `from_arrays`     | `OpenTimeSeries`              | Class method to create an OpenTimeSeries object from a list of date strings and a list of values.  |
 | `from_df`         | `OpenTimeSeries`              | Class method to create an OpenTimeSeries object from a pandas.DataFrame or pandas.Series.          |
 | `from_fixed_rate` | `OpenTimeSeries`              | Class method to create an OpenTimeSeries object from a fixed rate, number of days and an end date. |
 | `from_deepcopy`   | `OpenTimeSeries`, `OpenFrame` | Creates a copy of an OpenTimeSeries object.                                                        |
 
-### Non-numerical or "helper" properties that apply only to the [OpenTimeSeries](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/series.py) class.
+### Non-numerical or "helper" properties that apply only to the [OpenTimeSeries](https://github.com/CaptorAB/openseries/blob/master/openseries/series.py) class.
 
 | Property        | type            | Applies to       | Description                                                                                                                                  |
 |:----------------|:----------------|:-----------------|:---------------------------------------------------------------------------------------------------------------------------------------------|
 | `timeseries_id` | `str`           | `OpenTimeSeries` | Placeholder for database identifier for the timeseries. Can be left as empty string.                                                         |
 | `instrument_id` | `str`           | `OpenTimeSeries` | Placeholder for database identifier for the instrument associated with the timeseries. Can be left as empty string.                          |
 | `dates`         | `list[str]`     | `OpenTimeSeries` | Dates of the timeseries. Not edited by any method to allow reversion to original.                                                            |
 | `values`        | `list[float]`   | `OpenTimeSeries` | Values of the timeseries. Not edited by any method to allow reversion to original.                                                           |
@@ -191,54 +191,54 @@
 | `local_ccy`     | `bool`          | `OpenTimeSeries` | Indicates if series should be in its local currency or the domestic currency of the user. Only used if conversion/hedging methods are added. |
 | `name`          | `str`           | `OpenTimeSeries` | An identifier field.                                                                                                                         |
 | `isin`          | `str`           | `OpenTimeSeries` | ISIN code of the associated instrument. If any.                                                                                              |
 | `label`         | `str`           | `OpenTimeSeries` | Field used in outputs. Derived from name as default.                                                                                         |
 | `countries`     | `list` or `str` | `OpenTimeSeries` | (List of) country code(s) according to ISO 3166-1 alpha-2 used to generate business days.                                                    |
 | `valuetype`     | `ValueType`     | `OpenTimeSeries` | Field identifies the type of values in the series. ValueType is an Enum.                                                                     |
 
-### Non-numerical or "helper" properties that apply only to the [OpenFrame](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/frame.py) class.
+### Non-numerical or "helper" properties that apply only to the [OpenFrame](https://github.com/CaptorAB/openseries/blob/master/openseries/frame.py) class.
 
 | Property           | type                   | Applies to  | Description                                                              |
 |:-------------------|:-----------------------|:------------|:-------------------------------------------------------------------------|
 | `constituents`     | `list[OpenTimeSeries]` | `OpenFrame` | A list of the OpenTimeSeries that make up an OpenFrame.                  |
 | `columns_lvl_zero` | `list`                 | `OpenFrame` | A list of the level zero column names in the OpenFrame pandas.DataFrame. |
 | `columns_lvl_one`  | `list`                 | `OpenFrame` | A list of the level one column names in the OpenFrame pandas.DataFrame.  |
 | `item_count`       | `int`                  | `OpenFrame` | Number of columns in the OpenFrame pandas.DataFrame.                     |
 | `weights`          | `list[float]`          | `OpenFrame` | Weights used in the method `make_portfolio`.                             |
 | `first_indices`    | `pandas.Series`        | `OpenFrame` | First dates of all the series in the OpenFrame.                          |
 | `last_indices`     | `pandas.Series`        | `OpenFrame` | Last dates of all the series in the OpenFrame.                           |
 | `lengths_of_items` | `pandas.Series`        | `OpenFrame` | Number of items in each of the series in the OpenFrame.                  |
 | `span_of_days_all` | `pandas.Series`        | `OpenFrame` | Number of days from the first to the last in each of the series.         |
 
-### Non-numerical or "helper" properties that apply to both the [OpenTimeSeries](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/series.py) and the [OpenFrame](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/frame.py) class.
+### Non-numerical or "helper" properties that apply to both the [OpenTimeSeries](https://github.com/CaptorAB/openseries/blob/master/openseries/series.py) and the [OpenFrame](https://github.com/CaptorAB/openseries/blob/master/openseries/frame.py) class.
 
 | Property            | type                             | Applies to                    | Description                                                                       |
 |:--------------------|:---------------------------------|:------------------------------|:----------------------------------------------------------------------------------|
 | `first_idx`         | `datetime.date`                  | `OpenTimeSeries`, `OpenFrame` | First date of the series.                                                         |
 | `last_idx`          | `datetime.date`                  | `OpenTimeSeries`, `OpenFrame` | Last date of the series.                                                          |
 | `length`            | `int`                            | `OpenTimeSeries`, `OpenFrame` | Number of items in the series.                                                    |
 | `span_of_days`      | `int`                            | `OpenTimeSeries`, `OpenFrame` | Number of days from the first to the last date in the series.                     |
 | `tsdf`              | `pandas.DataFrame`               | `OpenTimeSeries`, `OpenFrame` | The Pandas DataFrame which gets edited by the class methods.                      |
 | `max_drawdown_date` | `datetime.date`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Date when the maximum drawdown occurred.                                          |
 | `periods_in_a_year` | `float`                          | `OpenTimeSeries`, `OpenFrame` | The number of observations in an average year for all days in the data.           |
 | `yearfrac`          | `float`                          | `OpenTimeSeries`, `OpenFrame` | Length of timeseries expressed as np.float64 fraction of a year with 365.25 days. |
 
-### Methods that apply only to the [OpenTimeSeries](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/series.py) class.
+### Methods that apply only to the [OpenTimeSeries](https://github.com/CaptorAB/openseries/blob/master/openseries/series.py) class.
 
 | Method                   | Applies to       | Description                                                                                                                                    |
 |:-------------------------|:-----------------|:-----------------------------------------------------------------------------------------------------------------------------------------------|
 | `setup_class`            | `OpenTimeSeries` | Class method that defines the `domestic` home currency and the `countries` home countries attributes.                                          |
 | `pandas_df`              | `OpenTimeSeries` | Method to create the `tsdf` pandas.DataFrame from the `dates` and `values`.                                                                    |
 | `set_new_label`          | `OpenTimeSeries` | Method to change the pandas.DataFrame column MultiIndex.                                                                                       |
 | `running_adjustment`     | `OpenTimeSeries` | Adjusts the series performance with a `float` factor.                                                                                          |
 | `ewma_vol_func`          | `OpenTimeSeries` | Returns a `pandas.Series` with volatility based on [Exponentially Weighted Moving Average](https://www.investopedia.com/articles/07/ewma.asp). |
 | `from_1d_rate_to_cumret` | `OpenTimeSeries` | Converts a series of 1-day rates into a cumulative valueseries.                                                                                |
                                                                            |
 
-### Methods that apply only to the [OpenFrame](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/frame.py) class.
+### Methods that apply only to the [OpenFrame](https://github.com/CaptorAB/openseries/blob/master/openseries/frame.py) class.
 
 | Method                  | Applies to  | Description                                                                                                                                                                        |
 |:------------------------|:------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | `merge_series`          | `OpenFrame` | Merges the Pandas Dataframes of the constituent OpenTimeSeries.                                                                                                                    |
 | `trunc_frame`           | `OpenFrame` | Truncates the OpenFrame to a common period.                                                                                                                                        |
 | `add_timeseries`        | `OpenFrame` | Adds a given OpenTimeSeries to the OpenFrame.                                                                                                                                      |
 | `delete_timeseries`     | `OpenFrame` | Deletes an OpenTimeSeries from the OpenFrame.                                                                                                                                      |
@@ -251,15 +251,15 @@
 | `info_ratio_func`       | `OpenFrame` | Calculates the [information ratios](https://www.investopedia.com/terms/i/informationratio.asp) relative to a selected series in the OpenFrame.                                     |
 | `capture_ratio_func`    | `OpenFrame` | Calculates up, down and up/down [capture ratios](https://www.investopedia.com/terms/d/down-market-capture-ratio.asp) relative to a selected series.                                |
 | `rolling_info_ratio`    | `OpenFrame` | Returns a pandas.DataFrame with the rolling [information ratio](https://www.investopedia.com/terms/i/informationratio.asp) between two series.                                     |
 | `rolling_beta`          | `OpenFrame` | Returns a pandas.DataFrame with the rolling [Beta](https://www.investopedia.com/terms/b/beta.asp) of an asset relative a market.                                                   |
 | `rolling_corr`          | `OpenFrame` | Calculates and adds a series of rolling [correlations](https://www.investopedia.com/terms/c/correlation.asp) between two other series.                                             |
 | `ewma_risk`             | `OpenFrame` | Returns a `pandas.DataFrame` with volatility and correlation based on [Exponentially Weighted Moving Average](https://www.investopedia.com/articles/07/ewma.asp).                  |
 
-### Methods that apply to both the [OpenTimeSeries](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/series.py) and the [OpenFrame](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/frame.py) class.
+### Methods that apply to both the [OpenTimeSeries](https://github.com/CaptorAB/openseries/blob/master/openseries/series.py) and the [OpenFrame](https://github.com/CaptorAB/openseries/blob/master/openseries/frame.py) class.
 
 | Method                             | Applies to                    | Description                                                                                                                                              |
 |:-----------------------------------|:------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
 | `align_index_to_local_cdays`       | `OpenTimeSeries`, `OpenFrame` | Aligns the series dates to a business calendar. Defaults to Sweden.                                                                                      |
 | `resample`                         | `OpenTimeSeries`, `OpenFrame` | Resamples the series to a specific frequency.                                                                                                            |
 | `resample_to_business_period_ends` | `OpenTimeSeries`, `OpenFrame` | Resamples the series to month-end dates with monthly, quarterly or annual frequency.                                                                     |
 | `value_nan_handle`                 | `OpenTimeSeries`, `OpenFrame` | Fills `Nan` in a value series with the preceding non-Nan value.                                                                                          |
@@ -276,15 +276,15 @@
 | `to_drawdown_series`               | `OpenTimeSeries`, `OpenFrame` | Converts the series into drawdown series.                                                                                                                |
 | `rolling_return`                   | `OpenTimeSeries`, `OpenFrame` | Returns a pandas.DataFrame with rolling returns.                                                                                                         |
 | `rolling_vol`                      | `OpenTimeSeries`, `OpenFrame` | Returns a pandas.DataFrame with rolling volatilities.                                                                                                    |
 | `rolling_var_down`                 | `OpenTimeSeries`, `OpenFrame` | Returns a pandas.DataFrame with rolling VaR figures.                                                                                                     |
 | `rolling_cvar_down`                | `OpenTimeSeries`, `OpenFrame` | Returns a pandas.DataFrame with rolling CVaR figures.                                                                                                    |
 | `calc_range`                       | `OpenTimeSeries`, `OpenFrame` | Returns the start and end dates of a range from specific period definitions. Used by the below numerical methods and not meant to be used independently. |
 
-### Numerical properties available for individual [OpenTimeSeries](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/series.py) or on all series in an [OpenFrame](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/frame.py).
+### Numerical properties available for individual [OpenTimeSeries](https://github.com/CaptorAB/openseries/blob/master/openseries/series.py) or on all series in an [OpenFrame](https://github.com/CaptorAB/openseries/blob/master/openseries/frame.py).
 
 | Property                | type                     | Applies to                    | Description                                                                                                                                                                                                             |
 |:------------------------|:-------------------------|:------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | `all_properties`        | `pandas.DataFrame`       | `OpenTimeSeries`, `OpenFrame` | Returns most of the properties in one go.                                                                                                                                                                               |
 | `arithmetic_ret`        | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | [Annualized arithmetic mean of returns](https://www.investopedia.com/terms/a/arithmeticmean.asp).                                                                                                                       |
 | `geo_ret`               | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | [Compound Annual Growth Rate(CAGR)](https://www.investopedia.com/terms/c/cagr.asp), a specific implementation of geometric mean.                                                                                        |
 | `value_ret`             | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Simple return from first to last observation.                                                                                                                                                                           |
```

### Comparing `openseries-1.5.1/openseries/_common_model.py` & `openseries-1.5.2/openseries/_common_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """Defining the _CommonModel class."""
-
 from __future__ import annotations
 
 import datetime as dt
 from inspect import stack
 from json import dump
 from math import ceil
 from pathlib import Path
```

### Comparing `openseries-1.5.1/openseries/_risk.py` & `openseries-1.5.2/openseries/_risk.py`

 * *Files identical despite different names*

### Comparing `openseries-1.5.1/openseries/datefixer.py` & `openseries-1.5.2/openseries/datefixer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Date related utilities."""
 from __future__ import annotations
 
 import datetime as dt
 from typing import Optional, Union, cast
 
 from dateutil.relativedelta import relativedelta
-from holidays import (  # type: ignore[import-untyped,unused-ignore]
+from holidays import (
     country_holidays,
     list_supported_countries,
 )
 from numpy import array, busdaycalendar, datetime64, is_busday, where
 from pandas import (
     DataFrame,
     DatetimeIndex,
```

### Comparing `openseries-1.5.1/openseries/frame.py` & `openseries-1.5.2/openseries/frame.py`

 * *Files identical despite different names*

### Comparing `openseries-1.5.1/openseries/load_plotly.py` & `openseries-1.5.2/openseries/load_plotly.py`

 * *Files identical despite different names*

### Comparing `openseries-1.5.1/openseries/plotly_layouts.json` & `openseries-1.5.2/openseries/plotly_layouts.json`

 * *Files identical despite different names*

### Comparing `openseries-1.5.1/openseries/series.py` & `openseries-1.5.2/openseries/series.py`

 * *Files identical despite different names*

### Comparing `openseries-1.5.1/openseries/simulation.py` & `openseries-1.5.2/openseries/simulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """Defining the ReturnSimulation class."""
-
 from __future__ import annotations
 
 import datetime as dt
 from typing import Optional, cast
 
 from numpy import multiply, sqrt
 from numpy.random import PCG64, Generator, SeedSequence
```

### Comparing `openseries-1.5.1/openseries/types.py` & `openseries-1.5.2/openseries/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Declaring types used throughout the project."""
+
 from __future__ import annotations
 
 import datetime as dt
 from enum import Enum
 from typing import Annotated, ClassVar, Literal, Union
 
 from numpy import datetime64
 from pandas import Timestamp
 from pydantic import BaseModel, Field, StringConstraints, conlist, conset
+from typing_extensions import Self
 
 CountryStringType = Annotated[
     str,
     StringConstraints(
         strip_whitespace=True,
         pattern=r"^[A-Z]{2}$",
         to_upper=True,
@@ -115,14 +117,15 @@
 LiteralLinePlotMode = Literal[
     "lines",
     "markers",
     "lines+markers",
     "lines+text",
     "markers+text",
     "lines+markers+text",
+    None,
 ]
 LiteralHowMerge = Literal["outer", "inner"]
 LiteralQuantileInterp = Literal["linear", "lower", "higher", "midpoint", "nearest"]
 LiteralBizDayFreq = Literal["B", "BME", "BQE", "BYE"]
 LiteralPandasReindexMethod = Literal[
     None,
     "pad",
@@ -133,15 +136,15 @@
 ]
 LiteralNanMethod = Literal["fill", "drop"]
 LiteralCaptureRatio = Literal["up", "down", "both"]
 LiteralBarPlotMode = Literal["stack", "group", "overlay", "relative"]
 LiteralPlotlyOutput = Literal["file", "div"]
 LiteralPlotlyJSlib = Literal[True, False, "cdn"]
 LiteralOlsFitMethod = Literal["pinv", "qr"]
-LiteralPortfolioWeightings = Literal["eq_weights", "eq_risk", "inv_vol", "mean_var"]
+LiteralPortfolioWeightings = Literal["eq_weights", "inv_vol"]
 LiteralOlsFitCovType = Literal[
     "nonrobust",
     "fixed scale",
     "HC0",
     "HC1",
     "HC2",
     "HC3",
@@ -234,22 +237,22 @@
         "length",
         "span_of_days",
         "yearfrac",
         "periods_in_a_year",
     }
 
     def __init__(
-        self: OpenTimeSeriesPropertiesList,
+        self: Self,
         *args: LiteralSeriesProps,
     ) -> None:
         """Property arguments for the OpenTimeSeries class."""
         super().__init__(args)
         self._validate()
 
-    def _validate(self: OpenTimeSeriesPropertiesList) -> None:
+    def _validate(self: Self) -> None:
         seen = set()
         for item in self:
             if item not in self.allowed_strings:
                 msg = (
                     f"Invalid string: {item}. Allowed strings: {self.allowed_strings}"
                 )
                 raise ValueError(
@@ -287,20 +290,20 @@
         "max_drawdown_cal_year",
         "first_indices",
         "last_indices",
         "lengths_of_items",
         "span_of_days_all",
     }
 
-    def __init__(self: OpenFramePropertiesList, *args: LiteralFrameProps) -> None:
+    def __init__(self: Self, *args: LiteralFrameProps) -> None:
         """Property arguments for the OpenFrame class."""
         super().__init__(args)
         self._validate()
 
-    def _validate(self: OpenFramePropertiesList) -> None:
+    def _validate(self: Self) -> None:
         seen = set()
         for item in self:
             if item not in self.allowed_strings:
                 msg = (
                     f"Invalid string: {item}. Allowed strings: {self.allowed_strings}"
                 )
                 raise ValueError(
```

### Comparing `openseries-1.5.1/pyproject.toml` & `openseries-1.5.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "openseries"
-version = "1.5.1"
-description = "Package for analyzing financial timeseries."
+version = "1.5.2"
+description = "Tools for analyzing financial timeseries."
 authors = ["Martin Karrin <martin.karrin@captor.se>"]
-repository = "https://github.com/CaptorAB/OpenSeries"
+repository = "https://github.com/CaptorAB/openseries"
 license = "BSD-3-Clause"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
@@ -49,53 +49,48 @@
 [tool.poetry.group.dev.dependencies]
 coverage = "^7.4.4"
 coverage-badge = "^1.1.0"
 mypy = "^1.9.0"
 pandas-stubs = "^2.2.1.240316"
 pre-commit = "^3.7.0"
 pytest = "^8.1.1"
-ruff = "^0.3.4"
-types-openpyxl = "^3.1.0.20240311"
+ruff = "^0.3.7"
+types-openpyxl = "^3.1.0.20240408"
 types-python-dateutil = "^2.9.0.20240316"
-types-requests = "^2.31.0.20240311"
+types-requests = "^2.31.0.20240406"
 
 [build-system]
 requires = ["poetry-core>=1.8.2"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.setuptools_scm]
-
-[poetry.virtualenvs]
-create = true
-in-project = true
-path = "venv"
-
 [tool.pytest.ini_options]
 filterwarnings = [
-    "ignore::RuntimeWarning:pandas.*:"
+    "ignore::DeprecationWarning:openpyxl.*:"
 ]
 
 [tool.coverage.run]
 omit = ["venv/*"]
 include = ["openseries/*"]
 
 [tool.coverage.report]
 skip_empty = true
 fail_under = 99
 
 [tool.mypy]
+exclude = ["venv/*"]
 strict = true
-follow_imports = "silent"
+pretty = true
+warn_unreachable = false
 warn_redundant_casts = true
 warn_unused_ignores = true
 disallow_any_generics = true
 check_untyped_defs = true
 no_implicit_reexport = true
 disallow_untyped_defs = true
-exclude = ["venv/*"]
+follow_imports = "normal"
 plugins = [
     "pydantic.mypy",
     "numpy.typing.mypy_plugin"
 ]
 
 [tool.pydantic-mypy]
 init_forbid_extra = true
```

### Comparing `openseries-1.5.1/PKG-INFO` & `openseries-1.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: openseries
-Version: 1.5.1
-Summary: Package for analyzing financial timeseries.
-Home-page: https://github.com/CaptorAB/OpenSeries
+Version: 1.5.2
+Summary: Tools for analyzing financial timeseries.
+Home-page: https://github.com/CaptorAB/openseries
 License: BSD-3-Clause
 Keywords: python,finance,fintech,data-science,timeseries,timeseries-data,timeseries-analysis,investment,investment-analysis,investing
 Author: Martin Karrin
 Author-email: martin.karrin@captor.se
 Requires-Python: >=3.9,<3.13
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pydantic
@@ -27,40 +27,40 @@
 Requires-Dist: plotly (>=5.18.0,<6.0.0)
 Requires-Dist: pyarrow (>=14.0.2,<16.0.0)
 Requires-Dist: pydantic (>=2.5.2,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: requests (>=2.20.0,<3.0.0)
 Requires-Dist: scipy (>=1.11.4,<2.0.0)
 Requires-Dist: statsmodels (>=0.14.0,<1.0.0)
-Project-URL: Repository, https://github.com/CaptorAB/OpenSeries
+Project-URL: Repository, https://github.com/CaptorAB/openseries
 Description-Content-Type: text/markdown
 
 <img src="https://sales.captor.se/captor_logo_sv_1600_icketransparent.png" alt="Captor
 Fund Management AB"
 width="81" height="100" align="left" float="right"/><br/>
 
 <br><br>
 
-# OpenSeries
+# openseries
 
 [![PyPI version](https://img.shields.io/pypi/v/openseries.svg)](https://pypi.org/project/openseries/)
 [![Conda version](https://img.shields.io/conda/vn/conda-forge/openseries.svg)](https://anaconda.org/conda-forge/openseries)
 [![Conda platforms](https://img.shields.io/conda/pn/conda-forge/openseries.svg)](https://anaconda.org/conda-forge/openseries)
 [![Python version](https://img.shields.io/pypi/pyversions/openseries.svg)](https://www.python.org/)
-[![GitHub Action Test Suite](https://github.com/CaptorAB/OpenSeries/actions/workflows/test.yml/badge.svg)](https://github.com/CaptorAB/OpenSeries/actions/workflows/test.yml)
-[![Coverage](https://cdn.jsdelivr.net/gh/CaptorAB/OpenSeries@master/coverage.svg)](https://github.com/CaptorAB/OpenSeries/actions/workflows/test.yml)
-[![Styling, Linting & Type checks](https://github.com/CaptorAB/OpenSeries/actions/workflows/check.yml/badge.svg)](https://github.com/CaptorAB/OpenSeries/actions/workflows/check.yml)
+[![GitHub Action Test Suite](https://github.com/CaptorAB/openseries/actions/workflows/test.yml/badge.svg)](https://github.com/CaptorAB/openseries/actions/workflows/test.yml)
+[![Coverage](https://cdn.jsdelivr.net/gh/CaptorAB/openseries@master/coverage.svg)](https://github.com/CaptorAB/openseries/actions/workflows/test.yml)
+[![Styling, Linting & Type checks](https://github.com/CaptorAB/openseries/actions/workflows/check.yml/badge.svg)](https://github.com/CaptorAB/openseries/actions/workflows/check.yml)
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://beta.ruff.rs/docs/)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 
-**OpenSeries** is a project with tools to analyse financial timeseries of a single
+`openseries` is a project with tools to analyse financial timeseries of a single
 asset or a group of assets. It is solely made for daily or less frequent data.
 
-<span style="font-size:2em;">[CHANGELOG](https://github.com/CaptorAB/OpenSeries/blob/master/CHANGELOG.md)</span>
+<span style="font-size:2em;">[CHANGELOG](https://github.com/CaptorAB/openseries/blob/master/CHANGELOG.md)</span>
 
 
 ## Basic Usage
 
 To install:
 
 ```bash
@@ -134,38 +134,38 @@
 the [Pydantic BaseModel](https://docs.pydantic.dev/usage/models/). Please refer to its documentation for information
 on any attributes or methods inherited from this model.
 
 
 ### Windows Powershell
 
 ```powershell
-git clone https://github.com/CaptorAB/OpenSeries.git
-cd OpenSeries
+git clone https://github.com/CaptorAB/openseries.git
+cd openseries
 ./make.ps1 make
 
 ```
 
 ### Mac Terminal/Linux
 
 ```bash
-git clone https://github.com/CaptorAB/OpenSeries.git
-cd OpenSeries
+git clone https://github.com/CaptorAB/openseries.git
+cd openseries
 make
 source source_me
 make install
 
 ```
 
 ## Testing and Linting / Type-checking
 
 Ruff and Mypy checking is embedded in the pre-commit hook. Both
 are also used in the project's GitHub workflows and are run when the `lint`
 alternative is chosen in the below commands.
 Any silenced error codes can be found in the
-[pyproject.toml](https://github.com/CaptorAB/OpenSeries/blob/master/pyproject.toml)
+[pyproject.toml](https://github.com/CaptorAB/openseries/blob/master/pyproject.toml)
 file or in in-line comments.
 
 ### Windows Powershell
 
 ```powershell
 ./make.ps1 test
 ./make.ps1 lint
@@ -197,28 +197,28 @@
 - [Numerical properties for both classes](#numerical-properties-available-for-individual-opentimeseries-or-on-all-series-in-an-openframe)
 - [Numerical methods with period arguments for both classes](#methods-below-are-identical-to-the-numerical-properties-above)
 
 ### On some files in the project
 
 | File                                                                                                             | Description                                                                                                                                                                                                                               |
 |:-----------------------------------------------------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| [series.py](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/series.py)                             | Defines the class _OpenTimeSeries_ for managing and analyzing a single timeseries. The module also defines a function `timeseries_chain` that can be used to chain two timeseries objects together.                                       |
-| [frame.py](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/frame.py)                               | Defines the class _OpenFrame_ for managing a group of timeseries, and e.g. calculate a portfolio timeseries from a rebalancing strategy between timeseries. The module also defines functions to simulate, optimize, and plot portfolios. |
-| [simulation.py](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/simulation.py)                     | Defines the class _ReturnSimulation_ to create simulated financial timeseries. Used in the project's test suite                                                                                                                           |
+| [series.py](https://github.com/CaptorAB/openseries/blob/master/openseries/series.py)                             | Defines the class _OpenTimeSeries_ for managing and analyzing a single timeseries. The module also defines a function `timeseries_chain` that can be used to chain two timeseries objects together.                                       |
+| [frame.py](https://github.com/CaptorAB/openseries/blob/master/openseries/frame.py)                               | Defines the class _OpenFrame_ for managing a group of timeseries, and e.g. calculate a portfolio timeseries from a rebalancing strategy between timeseries. The module also defines functions to simulate, optimize, and plot portfolios. |
+| [simulation.py](https://github.com/CaptorAB/openseries/blob/master/openseries/simulation.py)                     | Defines the class _ReturnSimulation_ to create simulated financial timeseries. Used in the project's test suite                                                                                                                           |
 
 ### Class methods used to construct objects.
 
 | Method            | Applies to                    | Description                                                                                        |
 |:------------------|:------------------------------|:---------------------------------------------------------------------------------------------------|
 | `from_arrays`     | `OpenTimeSeries`              | Class method to create an OpenTimeSeries object from a list of date strings and a list of values.  |
 | `from_df`         | `OpenTimeSeries`              | Class method to create an OpenTimeSeries object from a pandas.DataFrame or pandas.Series.          |
 | `from_fixed_rate` | `OpenTimeSeries`              | Class method to create an OpenTimeSeries object from a fixed rate, number of days and an end date. |
 | `from_deepcopy`   | `OpenTimeSeries`, `OpenFrame` | Creates a copy of an OpenTimeSeries object.                                                        |
 
-### Non-numerical or "helper" properties that apply only to the [OpenTimeSeries](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/series.py) class.
+### Non-numerical or "helper" properties that apply only to the [OpenTimeSeries](https://github.com/CaptorAB/openseries/blob/master/openseries/series.py) class.
 
 | Property        | type            | Applies to       | Description                                                                                                                                  |
 |:----------------|:----------------|:-----------------|:---------------------------------------------------------------------------------------------------------------------------------------------|
 | `timeseries_id` | `str`           | `OpenTimeSeries` | Placeholder for database identifier for the timeseries. Can be left as empty string.                                                         |
 | `instrument_id` | `str`           | `OpenTimeSeries` | Placeholder for database identifier for the instrument associated with the timeseries. Can be left as empty string.                          |
 | `dates`         | `list[str]`     | `OpenTimeSeries` | Dates of the timeseries. Not edited by any method to allow reversion to original.                                                            |
 | `values`        | `list[float]`   | `OpenTimeSeries` | Values of the timeseries. Not edited by any method to allow reversion to original.                                                           |
@@ -227,54 +227,54 @@
 | `local_ccy`     | `bool`          | `OpenTimeSeries` | Indicates if series should be in its local currency or the domestic currency of the user. Only used if conversion/hedging methods are added. |
 | `name`          | `str`           | `OpenTimeSeries` | An identifier field.                                                                                                                         |
 | `isin`          | `str`           | `OpenTimeSeries` | ISIN code of the associated instrument. If any.                                                                                              |
 | `label`         | `str`           | `OpenTimeSeries` | Field used in outputs. Derived from name as default.                                                                                         |
 | `countries`     | `list` or `str` | `OpenTimeSeries` | (List of) country code(s) according to ISO 3166-1 alpha-2 used to generate business days.                                                    |
 | `valuetype`     | `ValueType`     | `OpenTimeSeries` | Field identifies the type of values in the series. ValueType is an Enum.                                                                     |
 
-### Non-numerical or "helper" properties that apply only to the [OpenFrame](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/frame.py) class.
+### Non-numerical or "helper" properties that apply only to the [OpenFrame](https://github.com/CaptorAB/openseries/blob/master/openseries/frame.py) class.
 
 | Property           | type                   | Applies to  | Description                                                              |
 |:-------------------|:-----------------------|:------------|:-------------------------------------------------------------------------|
 | `constituents`     | `list[OpenTimeSeries]` | `OpenFrame` | A list of the OpenTimeSeries that make up an OpenFrame.                  |
 | `columns_lvl_zero` | `list`                 | `OpenFrame` | A list of the level zero column names in the OpenFrame pandas.DataFrame. |
 | `columns_lvl_one`  | `list`                 | `OpenFrame` | A list of the level one column names in the OpenFrame pandas.DataFrame.  |
 | `item_count`       | `int`                  | `OpenFrame` | Number of columns in the OpenFrame pandas.DataFrame.                     |
 | `weights`          | `list[float]`          | `OpenFrame` | Weights used in the method `make_portfolio`.                             |
 | `first_indices`    | `pandas.Series`        | `OpenFrame` | First dates of all the series in the OpenFrame.                          |
 | `last_indices`     | `pandas.Series`        | `OpenFrame` | Last dates of all the series in the OpenFrame.                           |
 | `lengths_of_items` | `pandas.Series`        | `OpenFrame` | Number of items in each of the series in the OpenFrame.                  |
 | `span_of_days_all` | `pandas.Series`        | `OpenFrame` | Number of days from the first to the last in each of the series.         |
 
-### Non-numerical or "helper" properties that apply to both the [OpenTimeSeries](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/series.py) and the [OpenFrame](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/frame.py) class.
+### Non-numerical or "helper" properties that apply to both the [OpenTimeSeries](https://github.com/CaptorAB/openseries/blob/master/openseries/series.py) and the [OpenFrame](https://github.com/CaptorAB/openseries/blob/master/openseries/frame.py) class.
 
 | Property            | type                             | Applies to                    | Description                                                                       |
 |:--------------------|:---------------------------------|:------------------------------|:----------------------------------------------------------------------------------|
 | `first_idx`         | `datetime.date`                  | `OpenTimeSeries`, `OpenFrame` | First date of the series.                                                         |
 | `last_idx`          | `datetime.date`                  | `OpenTimeSeries`, `OpenFrame` | Last date of the series.                                                          |
 | `length`            | `int`                            | `OpenTimeSeries`, `OpenFrame` | Number of items in the series.                                                    |
 | `span_of_days`      | `int`                            | `OpenTimeSeries`, `OpenFrame` | Number of days from the first to the last date in the series.                     |
 | `tsdf`              | `pandas.DataFrame`               | `OpenTimeSeries`, `OpenFrame` | The Pandas DataFrame which gets edited by the class methods.                      |
 | `max_drawdown_date` | `datetime.date`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Date when the maximum drawdown occurred.                                          |
 | `periods_in_a_year` | `float`                          | `OpenTimeSeries`, `OpenFrame` | The number of observations in an average year for all days in the data.           |
 | `yearfrac`          | `float`                          | `OpenTimeSeries`, `OpenFrame` | Length of timeseries expressed as np.float64 fraction of a year with 365.25 days. |
 
-### Methods that apply only to the [OpenTimeSeries](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/series.py) class.
+### Methods that apply only to the [OpenTimeSeries](https://github.com/CaptorAB/openseries/blob/master/openseries/series.py) class.
 
 | Method                   | Applies to       | Description                                                                                                                                    |
 |:-------------------------|:-----------------|:-----------------------------------------------------------------------------------------------------------------------------------------------|
 | `setup_class`            | `OpenTimeSeries` | Class method that defines the `domestic` home currency and the `countries` home countries attributes.                                          |
 | `pandas_df`              | `OpenTimeSeries` | Method to create the `tsdf` pandas.DataFrame from the `dates` and `values`.                                                                    |
 | `set_new_label`          | `OpenTimeSeries` | Method to change the pandas.DataFrame column MultiIndex.                                                                                       |
 | `running_adjustment`     | `OpenTimeSeries` | Adjusts the series performance with a `float` factor.                                                                                          |
 | `ewma_vol_func`          | `OpenTimeSeries` | Returns a `pandas.Series` with volatility based on [Exponentially Weighted Moving Average](https://www.investopedia.com/articles/07/ewma.asp). |
 | `from_1d_rate_to_cumret` | `OpenTimeSeries` | Converts a series of 1-day rates into a cumulative valueseries.                                                                                |
                                                                            |
 
-### Methods that apply only to the [OpenFrame](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/frame.py) class.
+### Methods that apply only to the [OpenFrame](https://github.com/CaptorAB/openseries/blob/master/openseries/frame.py) class.
 
 | Method                  | Applies to  | Description                                                                                                                                                                        |
 |:------------------------|:------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | `merge_series`          | `OpenFrame` | Merges the Pandas Dataframes of the constituent OpenTimeSeries.                                                                                                                    |
 | `trunc_frame`           | `OpenFrame` | Truncates the OpenFrame to a common period.                                                                                                                                        |
 | `add_timeseries`        | `OpenFrame` | Adds a given OpenTimeSeries to the OpenFrame.                                                                                                                                      |
 | `delete_timeseries`     | `OpenFrame` | Deletes an OpenTimeSeries from the OpenFrame.                                                                                                                                      |
@@ -287,15 +287,15 @@
 | `info_ratio_func`       | `OpenFrame` | Calculates the [information ratios](https://www.investopedia.com/terms/i/informationratio.asp) relative to a selected series in the OpenFrame.                                     |
 | `capture_ratio_func`    | `OpenFrame` | Calculates up, down and up/down [capture ratios](https://www.investopedia.com/terms/d/down-market-capture-ratio.asp) relative to a selected series.                                |
 | `rolling_info_ratio`    | `OpenFrame` | Returns a pandas.DataFrame with the rolling [information ratio](https://www.investopedia.com/terms/i/informationratio.asp) between two series.                                     |
 | `rolling_beta`          | `OpenFrame` | Returns a pandas.DataFrame with the rolling [Beta](https://www.investopedia.com/terms/b/beta.asp) of an asset relative a market.                                                   |
 | `rolling_corr`          | `OpenFrame` | Calculates and adds a series of rolling [correlations](https://www.investopedia.com/terms/c/correlation.asp) between two other series.                                             |
 | `ewma_risk`             | `OpenFrame` | Returns a `pandas.DataFrame` with volatility and correlation based on [Exponentially Weighted Moving Average](https://www.investopedia.com/articles/07/ewma.asp).                  |
 
-### Methods that apply to both the [OpenTimeSeries](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/series.py) and the [OpenFrame](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/frame.py) class.
+### Methods that apply to both the [OpenTimeSeries](https://github.com/CaptorAB/openseries/blob/master/openseries/series.py) and the [OpenFrame](https://github.com/CaptorAB/openseries/blob/master/openseries/frame.py) class.
 
 | Method                             | Applies to                    | Description                                                                                                                                              |
 |:-----------------------------------|:------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
 | `align_index_to_local_cdays`       | `OpenTimeSeries`, `OpenFrame` | Aligns the series dates to a business calendar. Defaults to Sweden.                                                                                      |
 | `resample`                         | `OpenTimeSeries`, `OpenFrame` | Resamples the series to a specific frequency.                                                                                                            |
 | `resample_to_business_period_ends` | `OpenTimeSeries`, `OpenFrame` | Resamples the series to month-end dates with monthly, quarterly or annual frequency.                                                                     |
 | `value_nan_handle`                 | `OpenTimeSeries`, `OpenFrame` | Fills `Nan` in a value series with the preceding non-Nan value.                                                                                          |
@@ -312,15 +312,15 @@
 | `to_drawdown_series`               | `OpenTimeSeries`, `OpenFrame` | Converts the series into drawdown series.                                                                                                                |
 | `rolling_return`                   | `OpenTimeSeries`, `OpenFrame` | Returns a pandas.DataFrame with rolling returns.                                                                                                         |
 | `rolling_vol`                      | `OpenTimeSeries`, `OpenFrame` | Returns a pandas.DataFrame with rolling volatilities.                                                                                                    |
 | `rolling_var_down`                 | `OpenTimeSeries`, `OpenFrame` | Returns a pandas.DataFrame with rolling VaR figures.                                                                                                     |
 | `rolling_cvar_down`                | `OpenTimeSeries`, `OpenFrame` | Returns a pandas.DataFrame with rolling CVaR figures.                                                                                                    |
 | `calc_range`                       | `OpenTimeSeries`, `OpenFrame` | Returns the start and end dates of a range from specific period definitions. Used by the below numerical methods and not meant to be used independently. |
 
-### Numerical properties available for individual [OpenTimeSeries](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/series.py) or on all series in an [OpenFrame](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/frame.py).
+### Numerical properties available for individual [OpenTimeSeries](https://github.com/CaptorAB/openseries/blob/master/openseries/series.py) or on all series in an [OpenFrame](https://github.com/CaptorAB/openseries/blob/master/openseries/frame.py).
 
 | Property                | type                     | Applies to                    | Description                                                                                                                                                                                                             |
 |:------------------------|:-------------------------|:------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | `all_properties`        | `pandas.DataFrame`       | `OpenTimeSeries`, `OpenFrame` | Returns most of the properties in one go.                                                                                                                                                                               |
 | `arithmetic_ret`        | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | [Annualized arithmetic mean of returns](https://www.investopedia.com/terms/a/arithmeticmean.asp).                                                                                                                       |
 | `geo_ret`               | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | [Compound Annual Growth Rate(CAGR)](https://www.investopedia.com/terms/c/cagr.asp), a specific implementation of geometric mean.                                                                                        |
 | `value_ret`             | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Simple return from first to last observation.                                                                                                                                                                           |
```

