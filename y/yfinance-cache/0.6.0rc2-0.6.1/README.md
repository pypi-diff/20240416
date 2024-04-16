# Comparing `tmp/yfinance-cache-0.6.0rc2.tar.gz` & `tmp/yfinance_cache-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yfinance-cache-0.6.0rc2.tar", last modified: Sat Apr  6 09:32:20 2024, max compression
+gzip compressed data, was "yfinance_cache-0.6.1.tar", last modified: Tue Apr 16 20:50:13 2024, max compression
```

## Comparing `yfinance-cache-0.6.0rc2.tar` & `yfinance_cache-0.6.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 gonzo     (1000) gonzo     (1000)        0 2024-04-06 09:32:20.269808 yfinance-cache-0.6.0rc2/
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     1068 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/LICENSE
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     5989 2024-04-06 09:32:20.269808 yfinance-cache-0.6.0rc2/PKG-INFO
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     5294 2024-03-31 21:40:24.000000 yfinance-cache-0.6.0rc2/README.md
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)      104 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/pyproject.toml
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)      832 2024-04-06 09:32:20.270808 yfinance-cache-0.6.0rc2/setup.cfg
-drwxr-xr-x   0 gonzo     (1000) gonzo     (1000)        0 2024-04-06 09:32:20.269808 yfinance-cache-0.6.0rc2/tests/
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)       21 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/__init__.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     1675 2024-03-31 21:37:18.000000 yfinance-cache-0.6.0rc2/tests/context.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     8469 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_cache.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)      991 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_datetime-assumptions.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    74555 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_market_intervals_asx.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    70793 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_market_intervals_nze.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    74237 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_market_intervals_tlv.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    71006 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_market_intervals_usa.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    24913 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_market_schedules_asx.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    24789 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_market_schedules_nze.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    32509 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_market_schedules_tlv.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    23272 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_market_schedules_usa.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    12038 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_missing_intervals_asx.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    12079 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_missing_intervals_nze.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    13799 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_missing_intervals_tlv.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    13077 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_missing_intervals_usa.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    25165 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_price_data_aging_1d.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    16811 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_price_data_aging_1h.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    17013 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_price_data_aging_1w.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     2447 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_time_utils.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     1698 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_utils.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     2955 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_yf_assumptions.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    32294 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_yfc_adjust.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    12038 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_yfc_backend.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    12467 2024-03-31 21:37:18.000000 yfinance-cache-0.6.0rc2/tests/test_yfc_financials.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    40121 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_yfc_interface.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     4270 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_yfc_ticker.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     5085 2024-03-31 21:37:18.000000 yfinance-cache-0.6.0rc2/tests/utils.py
-drwxr-xr-x   0 gonzo     (1000) gonzo     (1000)        0 2024-04-06 09:32:20.263808 yfinance-cache-0.6.0rc2/yfinance_cache/
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)      354 2024-03-31 21:40:24.000000 yfinance-cache-0.6.0rc2/yfinance_cache/__init__.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    16324 2024-03-31 21:40:24.000000 yfinance-cache-0.6.0rc2/yfinance_cache/yfc_cache_manager.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    52610 2024-03-31 21:40:24.000000 yfinance-cache-0.6.0rc2/yfinance_cache/yfc_dat.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    89156 2024-04-05 21:52:36.000000 yfinance-cache-0.6.0rc2/yfinance_cache/yfc_financials_manager.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     2197 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/yfinance_cache/yfc_logging.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     6792 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/yfinance_cache/yfc_multi.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     1453 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/yfinance_cache/yfc_options.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)   204038 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/yfinance_cache/yfc_prices_manager.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    39045 2024-03-31 21:41:16.000000 yfinance-cache-0.6.0rc2/yfinance_cache/yfc_ticker.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    81302 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/yfinance_cache/yfc_time.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)      653 2024-02-25 13:22:49.000000 yfinance-cache-0.6.0rc2/yfinance_cache/yfc_upgrade.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    25378 2024-03-31 21:40:24.000000 yfinance-cache-0.6.0rc2/yfinance_cache/yfc_utils.py
-drwxr-xr-x   0 gonzo     (1000) gonzo     (1000)        0 2024-04-06 09:32:20.269808 yfinance-cache-0.6.0rc2/yfinance_cache.egg-info/
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     5989 2024-04-06 09:32:20.000000 yfinance-cache-0.6.0rc2/yfinance_cache.egg-info/PKG-INFO
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     2316 2024-04-06 09:32:20.000000 yfinance-cache-0.6.0rc2/yfinance_cache.egg-info/SOURCES.txt
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)        1 2024-04-06 09:32:20.000000 yfinance-cache-0.6.0rc2/yfinance_cache.egg-info/dependency_links.txt
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)       79 2024-04-06 09:32:20.000000 yfinance-cache-0.6.0rc2/yfinance_cache.egg-info/requires.txt
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)       21 2024-04-06 09:32:20.000000 yfinance-cache-0.6.0rc2/yfinance_cache.egg-info/top_level.txt
+drwxr-xr-x   0 gonzo     (1000) gonzo     (1000)        0 2024-04-16 20:50:13.234508 yfinance_cache-0.6.1/
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     1068 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/LICENSE
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     5986 2024-04-16 20:50:13.234508 yfinance_cache-0.6.1/PKG-INFO
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     5294 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/README.md
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)      104 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/pyproject.toml
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)      829 2024-04-16 20:50:13.235509 yfinance_cache-0.6.1/setup.cfg
+drwxr-xr-x   0 gonzo     (1000) gonzo     (1000)        0 2024-04-16 20:50:13.234508 yfinance_cache-0.6.1/tests/
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)       21 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/__init__.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     1675 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/context.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     8469 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_cache.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)      991 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_datetime-assumptions.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    74555 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_market_intervals_asx.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    70793 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_market_intervals_nze.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    74237 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_market_intervals_tlv.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    71006 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_market_intervals_usa.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    24913 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_market_schedules_asx.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    24789 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_market_schedules_nze.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    32509 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_market_schedules_tlv.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    23272 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_market_schedules_usa.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    12038 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_missing_intervals_asx.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    12079 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_missing_intervals_nze.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    13799 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_missing_intervals_tlv.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    13077 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_missing_intervals_usa.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    25165 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_price_data_aging_1d.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    16811 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_price_data_aging_1h.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    17013 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_price_data_aging_1w.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     2447 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_time_utils.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     1698 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_utils.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     2955 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_yf_assumptions.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    32294 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_yfc_adjust.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    12038 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_yfc_backend.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    12467 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_yfc_financials.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    40121 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_yfc_interface.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     4270 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/test_yfc_ticker.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     5085 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/tests/utils.py
+drwxr-xr-x   0 gonzo     (1000) gonzo     (1000)        0 2024-04-16 20:50:13.228508 yfinance_cache-0.6.1/yfinance_cache/
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)      354 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/yfinance_cache/__init__.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    16324 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/yfinance_cache/yfc_cache_manager.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    52610 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/yfinance_cache/yfc_dat.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    89428 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/yfinance_cache/yfc_financials_manager.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     2197 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/yfinance_cache/yfc_logging.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     6792 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/yfinance_cache/yfc_multi.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     1453 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/yfinance_cache/yfc_options.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)   204038 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/yfinance_cache/yfc_prices_manager.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    39338 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/yfinance_cache/yfc_ticker.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    81302 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/yfinance_cache/yfc_time.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)      653 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/yfinance_cache/yfc_upgrade.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    25372 2024-04-16 20:49:40.000000 yfinance_cache-0.6.1/yfinance_cache/yfc_utils.py
+drwxr-xr-x   0 gonzo     (1000) gonzo     (1000)        0 2024-04-16 20:50:13.234508 yfinance_cache-0.6.1/yfinance_cache.egg-info/
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     5986 2024-04-16 20:50:13.000000 yfinance_cache-0.6.1/yfinance_cache.egg-info/PKG-INFO
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     2316 2024-04-16 20:50:13.000000 yfinance_cache-0.6.1/yfinance_cache.egg-info/SOURCES.txt
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)        1 2024-04-16 20:50:13.000000 yfinance_cache-0.6.1/yfinance_cache.egg-info/dependency_links.txt
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)       79 2024-04-16 20:50:13.000000 yfinance_cache-0.6.1/yfinance_cache.egg-info/requires.txt
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)       21 2024-04-16 20:50:13.000000 yfinance_cache-0.6.1/yfinance_cache.egg-info/top_level.txt
```

### Comparing `yfinance-cache-0.6.0rc2/LICENSE` & `yfinance_cache-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc2/PKG-INFO` & `yfinance_cache-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yfinance-cache
-Version: 0.6.0rc2
+Version: 0.6.1
 Summary: Smart caching wrapper for 'yfinance' module
 Home-page: https://github.com/ValueRaider/yfinance-cache
 Author: ValueRaider
 Author-email: ValueRaider@protonmail.com
 Project-URL: Bug Tracker, https://github.com/ValueRaider/yfinance-cache/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `yfinance-cache-0.6.0rc2/README.md` & `yfinance_cache-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc2/setup.cfg` & `yfinance_cache-0.6.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = yfinance-cache
-version = 0.6.0rc2
+version = 0.6.1
 author = ValueRaider
 author_email = ValueRaider@protonmail.com
 description = Smart caching wrapper for 'yfinance' module
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ValueRaider/yfinance-cache
 project_urls =
```

### Comparing `yfinance-cache-0.6.0rc2/tests/context.py` & `yfinance_cache-0.6.1/tests/context.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc2/tests/test_cache.py` & `yfinance_cache-0.6.1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc2/tests/test_datetime-assumptions.py` & `yfinance_cache-0.6.1/tests/test_datetime-assumptions.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc2/tests/test_market_intervals_asx.py` & `yfinance_cache-0.6.1/tests/test_market_intervals_asx.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc2/tests/test_market_intervals_nze.py` & `yfinance_cache-0.6.1/tests/test_market_intervals_nze.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc2/tests/test_market_intervals_tlv.py` & `yfinance_cache-0.6.1/tests/test_market_intervals_tlv.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc2/tests/test_market_intervals_usa.py` & `yfinance_cache-0.6.1/tests/test_market_intervals_usa.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc2/tests/test_market_schedules_asx.py` & `yfinance_cache-0.6.1/tests/test_market_schedules_asx.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc2/tests/test_market_schedules_nze.py` & `yfinance_cache-0.6.1/tests/test_market_schedules_nze.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc2/tests/test_market_schedules_tlv.py` & `yfinance_cache-0.6.1/tests/test_market_schedules_tlv.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc2/tests/test_market_schedules_usa.py` & `yfinance_cache-0.6.1/tests/test_market_schedules_usa.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc2/tests/test_missing_intervals_asx.py` & `yfinance_cache-0.6.1/tests/test_missing_intervals_asx.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc2/tests/test_missing_intervals_nze.py` & `yfinance_cache-0.6.1/tests/test_missing_intervals_nze.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc2/tests/test_missing_intervals_tlv.py` & `yfinance_cache-0.6.1/tests/test_missing_intervals_tlv.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc2/tests/test_missing_intervals_usa.py` & `yfinance_cache-0.6.1/tests/test_missing_intervals_usa.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc2/tests/test_price_data_aging_1d.py` & `yfinance_cache-0.6.1/tests/test_price_data_aging_1d.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc2/tests/test_price_data_aging_1h.py` & `yfinance_cache-0.6.1/tests/test_price_data_aging_1h.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc2/tests/test_price_data_aging_1w.py` & `yfinance_cache-0.6.1/tests/test_price_data_aging_1w.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc2/tests/test_time_utils.py` & `yfinance_cache-0.6.1/tests/test_time_utils.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc2/tests/test_utils.py` & `yfinance_cache-0.6.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc2/tests/test_yf_assumptions.py` & `yfinance_cache-0.6.1/tests/test_yf_assumptions.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc2/tests/test_yfc_adjust.py` & `yfinance_cache-0.6.1/tests/test_yfc_adjust.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc2/tests/test_yfc_backend.py` & `yfinance_cache-0.6.1/tests/test_yfc_backend.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc2/tests/test_yfc_financials.py` & `yfinance_cache-0.6.1/tests/test_yfc_financials.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc2/tests/test_yfc_interface.py` & `yfinance_cache-0.6.1/tests/test_yfc_interface.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc2/tests/test_yfc_ticker.py` & `yfinance_cache-0.6.1/tests/test_yfc_ticker.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc2/tests/utils.py` & `yfinance_cache-0.6.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc2/yfinance_cache/yfc_cache_manager.py` & `yfinance_cache-0.6.1/yfinance_cache/yfc_cache_manager.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc2/yfinance_cache/yfc_dat.py` & `yfinance_cache-0.6.1/yfinance_cache/yfc_dat.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc2/yfinance_cache/yfc_financials_manager.py` & `yfinance_cache-0.6.1/yfinance_cache/yfc_financials_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -367,16 +367,16 @@
                     #             # print("- metadata old:") ; pprint(md_old)
                     #             raise Exception(f'Why asking Yahoo for {finType} when nothing new ready?')
                 elif not df_new.empty:
                     if df_pruned.empty:
                         df = df_new
                     else:
                         # Before merging, check for new/missing fields. Insert any with value NaN.
-                        missing_keys = [k for k in df_pruned.index if not k in df_new.index]
-                        new_keys = [k for k in df_new.index if not k in df_pruned.index]
+                        missing_keys = [k for k in df_pruned.index if k not in df_new.index]
+                        new_keys = [k for k in df_new.index if k not in df_pruned.index]
                         actions = []
                         for k in missing_keys:
                             actions.append((k, "missing", df_pruned.index.get_loc(k)))
                         for k in new_keys:
                             actions.append((k, "new", df_new.index.get_loc(k)))
                         actions = sorted(actions, key=lambda x: x[2])
                         for a in actions:
@@ -412,23 +412,27 @@
         if debug:
             print("- tbl:") ; print(tbl)
         if len(dates) <= 1:
             return yfcd.TimedeltaEstimate(yfcd.ComparableRelativedelta(months=6), yfcd.Confidence.Medium)
 
         interval = None
         intervals = [(dates[i-1] - dates[i]).days for i in range(1,len(dates))]
+        intervals = np.array(intervals)
         sdm_thresold = 0.1
         if len(intervals) == 1:
             interval = intervals[0]
         else:
-            avg = mean(intervals)
-            sdm = stdev(intervals) / avg
+            # First, discard impossibly small intervals:
+            f_too_small = intervals < 60
+            if f_too_small.any():
+                intervals = intervals[~f_too_small]
+            avg = np.mean(intervals)
+            sdm = np.std(intervals) / avg
             if sdm > sdm_thresold:
                 # Discard large outliers
-                intervals = np.array(intervals)
                 intervals = intervals[intervals<avg]
                 if len(intervals) == 1:
                     interval = intervals[0]
                 else:
                     avg = np.mean(intervals)
                     sdm = np.std(intervals) / avg
                     if sdm > sdm_thresold:
@@ -1158,18 +1162,23 @@
 
         if check:
             self._check_release_dates(releases, finType, period, refresh)
 
         return releases
 
     def _check_release_dates(self, releases, finType, period, refresh):
-        if period == yfcd.ReportingPeriod.Full:
-            interval_td = interval_str_to_days['ANNUAL']
-        else:
-            interval_td = self._get_interval(finType, refresh)
+        # if period == yfcd.ReportingPeriod.Full:
+        #     interval_td = interval_str_to_days['ANNUAL']
+        # else:
+        #     interval_td = self._get_interval(finType, refresh)
+
+        # Ignore releases with no date:
+        # - can happen with nonsense financials dates from Yahoo that
+        #   even my prune function couldn't safely remove
+        releases = [r for r in releases if r.release_date is not None]
 
         for i0 in range(len(releases)-1):
             r0 = releases[i0]
             r0rd = r0.release_date
             if hasattr(r0rd, 'confidence') and r0rd.confidence == yfcd.Confidence.Low:
                 continue
             for i1 in range(i0+1, len(releases)):
@@ -1191,16 +1200,14 @@
 
                 if not r0.is_end_of_year():
                     try:
                         # bad_order = r0.release_date > r1.period_end
                         bad_order = r0.release_date > (r1.period_end+timedelta(days=7))
                     except yfcd.AmbiguousComparisonException:
                         p = r0.release_date.prob_gt(r1.period_end+timedelta(days=7))
-                        if debug:
-                            print(f"- prob. that {r0.release_date} > {r1.period_end+timedelta(days=7)} = {p*100.0:.1f}%")
                         bad_order = p > 0.9
                     # try:
                     #     bad_order = bad_order and ((r1.period_end - r0.period_end)*2.0 > interval_td)
                     # except yfcd.AmbiguousComparisonException:
                     #     bad_order = False
                     if bad_order:
                         pprint(releases)
```

### Comparing `yfinance-cache-0.6.0rc2/yfinance_cache/yfc_logging.py` & `yfinance_cache-0.6.1/yfinance_cache/yfc_logging.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc2/yfinance_cache/yfc_multi.py` & `yfinance_cache-0.6.1/yfinance_cache/yfc_multi.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc2/yfinance_cache/yfc_options.py` & `yfinance_cache-0.6.1/yfinance_cache/yfc_options.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc2/yfinance_cache/yfc_prices_manager.py` & `yfinance_cache-0.6.1/yfinance_cache/yfc_prices_manager.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc2/yfinance_cache/yfc_ticker.py` & `yfinance_cache-0.6.1/yfinance_cache/yfc_ticker.py`

 * *Files 1% similar despite different names*

```diff
@@ -484,30 +484,34 @@
         if max_age is None:
             max_age = pd.Timedelta(yfcm._option_manager.max_ages.info)
         elif not isinstance(max_age, (datetime.timedelta, pd.Timedelta)):
             max_age = pd.Timedelta(max_age)
         if max_age < pd.Timedelta(0):
             raise Exception(f"'max_age' must be positive timedelta not {max_age}")
 
+        md = None
         if yfcm.IsDatumCached(self.ticker, "info"):
             self._info, md = yfcm.ReadCacheDatum(self.ticker, "info", True)
             if 'FetchDate' not in self._info.keys():
+                # Old bug meant this could happen
                 fp = yfcm.GetFilepath(self.ticker, 'info')
                 mod_dt = datetime.datetime.fromtimestamp(os.path.getmtime(fp))
                 self._info['FetchDate'] = mod_dt
-                yfcm.WriteCacheMetadata(self.ticker, "info", 'LastCheck', mod_dt)
+                md['LastCheck'] = mod_dt
+                yfcm.StoreCacheDatum(self.ticker, "info", self._info, metadata=md)
 
-        if self._info is not None:
-            if md is None:
-                md = {}
-            if not 'LastCheck' in md.keys():
-                md['LastCheck'] = self._info['FetchDate']
-                yfcm.WriteCacheMetadata(self.ticker, "info", 'LastCheck', md['LastCheck'])
-            if max(self._info['FetchDate'], md['LastCheck']) + max_age > pd.Timestamp.now():
-                return self._info
+            if self._info is not None:
+                if md is None:
+                    md = {}
+                if not 'LastCheck' in md.keys():
+                    # Old bug meant this could happen
+                    md['LastCheck'] = self._info['FetchDate']
+                    yfcm.WriteCacheMetadata(self.ticker, "info", 'LastCheck', md['LastCheck'])
+                if max(self._info['FetchDate'], md['LastCheck']) + max_age > pd.Timestamp.now():
+                    return self._info
 
         i = self.dat.info
         i['FetchDate'] = pd.Timestamp.now()
 
         if self._info is not None:
             # Check new info is not downgrade
             diff = len(i) - len(self._info)
@@ -528,15 +532,18 @@
                 #
                 msg += "\nDiscarding fetched info."
                 print(f'{self.ticker}: {msg}')
                 yfcm.WriteCacheMetadata(self.ticker, "info", 'LastCheck', i['FetchDate'])
                 return self._info
 
         self._info = i
-        yfcm.StoreCacheDatum(self.ticker, "info", self._info)
+        if md is None:
+            md = {}
+        mf['LastCheck'] = i['FetchDate']
+        yfcm.StoreCacheDatum(self.ticker, "info", self._info, metadata=md)
 
         exchange, tz_name = self._getExchangeAndTz()
         yfct.SetExchangeTzName(exchange, tz_name)
 
         return self._info
 
     @property
```

### Comparing `yfinance-cache-0.6.0rc2/yfinance_cache/yfc_time.py` & `yfinance_cache-0.6.1/yfinance_cache/yfc_time.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc2/yfinance_cache/yfc_upgrade.py` & `yfinance_cache-0.6.1/yfinance_cache/yfc_upgrade.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc2/yfinance_cache/yfc_utils.py` & `yfinance_cache-0.6.1/yfinance_cache/yfc_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         raise TypeError(f"'{varName}' if datetime must be timezone-aware".format(varName))
     elif not isinstance(var.tzinfo, ZoneInfo):
         raise TypeError(f"'{varName}' tzinfo must be ZoneInfo not {type(var.tzinfo)}")
 def TypeCheckYear(var, varName):
     if not isinstance(var, int):
         raise Exception("'{}' must be int not {}".format(varName, type(var)))
     if var < 1900 or var > 2200:
-        raise Exception("'{}' must be in range 1900-2200 not {}".format(varName, type(var)))
+        raise Exception("'{}' must be in range 1900-2200 not {}".format(varName, var))
 def TypeCheckTimedelta(var, varName):
     if not isinstance(var, timedelta):
         raise TypeError(f"'{varName}' must be timedelta not {type(var)}")
 def TypeCheckInterval(var, varName):
     if not isinstance(var, yfcd.Interval):
         raise TypeError(f"'{varName}' must be yfcd.Interval not {type(var)}")
 def TypeCheckIntervalDt(var, interval, varName, strict=True):
```

### Comparing `yfinance-cache-0.6.0rc2/yfinance_cache.egg-info/PKG-INFO` & `yfinance_cache-0.6.1/yfinance_cache.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yfinance-cache
-Version: 0.6.0rc2
+Version: 0.6.1
 Summary: Smart caching wrapper for 'yfinance' module
 Home-page: https://github.com/ValueRaider/yfinance-cache
 Author: ValueRaider
 Author-email: ValueRaider@protonmail.com
 Project-URL: Bug Tracker, https://github.com/ValueRaider/yfinance-cache/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `yfinance-cache-0.6.0rc2/yfinance_cache.egg-info/SOURCES.txt` & `yfinance_cache-0.6.1/yfinance_cache.egg-info/SOURCES.txt`

 * *Files identical despite different names*

