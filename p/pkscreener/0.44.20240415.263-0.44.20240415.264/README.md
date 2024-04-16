# Comparing `tmp/pkscreener-0.44.20240415.263.tar.gz` & `tmp/pkscreener-0.44.20240415.264.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240415.263.tar", last modified: Mon Apr 15 10:23:21 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240415.264.tar", last modified: Mon Apr 15 17:39:20 2024, max compression
```

## Comparing `pkscreener-0.44.20240415.263.tar` & `pkscreener-0.44.20240415.264.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 10:23:21.238567 pkscreener-0.44.20240415.263/
--rw-rw-rw-   0        0        0     1086 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-04-15 10:23:21.238567 pkscreener-0.44.20240415.263/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 10:23:21.222944 pkscreener-0.44.20240415.263/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 10:23:21.238567 pkscreener-0.44.20240415.263/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0    17333 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    24554 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0     9291 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     2995 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    27587 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    20931 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    17381 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8037 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    17306 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    48885 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   113858 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    46266 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    74375 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-04-15 10:23:12.000000 pkscreener-0.44.20240415.263/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   113144 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/globals.py
--rw-rw-rw-   0        0        0      565 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    47815 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    18453 2024-04-15 10:20:07.000000 pkscreener-0.44.20240415.263/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-04-15 10:23:21.222944 pkscreener-0.44.20240415.263/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-04-15 10:23:21.000000 pkscreener-0.44.20240415.263/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1250 2024-04-15 10:23:21.000000 pkscreener-0.44.20240415.263/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 10:23:21.000000 pkscreener-0.44.20240415.263/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-04-15 10:23:21.000000 pkscreener-0.44.20240415.263/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-15 10:23:21.000000 pkscreener-0.44.20240415.263/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-04-15 10:23:21.000000 pkscreener-0.44.20240415.263/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-15 10:23:21.238567 pkscreener-0.44.20240415.263/setup.cfg
--rw-rw-rw-   0        0        0     4715 2024-04-15 10:20:08.000000 pkscreener-0.44.20240415.263/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:39:20.881340 pkscreener-0.44.20240415.264/
+-rw-rw-rw-   0        0        0     1086 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-04-15 17:39:20.881340 pkscreener-0.44.20240415.264/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 17:39:20.865721 pkscreener-0.44.20240415.264/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:39:20.881340 pkscreener-0.44.20240415.264/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5484 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    24554 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0     9291 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     3203 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    27587 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    20931 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    17381 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8037 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    17306 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    48885 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   113858 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    46266 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    76874 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-04-15 17:39:12.000000 pkscreener-0.44.20240415.264/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   113838 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      565 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    47815 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    18748 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:39:20.865721 pkscreener-0.44.20240415.264/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-04-15 17:39:20.000000 pkscreener-0.44.20240415.264/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1282 2024-04-15 17:39:20.000000 pkscreener-0.44.20240415.264/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 17:39:20.000000 pkscreener-0.44.20240415.264/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2024-04-15 17:39:20.000000 pkscreener-0.44.20240415.264/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-15 17:39:20.000000 pkscreener-0.44.20240415.264/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-04-15 17:39:20.000000 pkscreener-0.44.20240415.264/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-15 17:39:20.881340 pkscreener-0.44.20240415.264/setup.cfg
+-rw-rw-rw-   0        0        0     4715 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/setup.py
```

### Comparing `pkscreener-0.44.20240415.263/LICENSE` & `pkscreener-0.44.20240415.264/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.263/LICENSE-Others` & `pkscreener-0.44.20240415.264/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.263/PKG-INFO` & `pkscreener-0.44.20240415.264/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240415.263
+Version: 0.44.20240415.264
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240415.263.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240415.264.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.262/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240415.263/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.262/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240415.263/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.262/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240415.263/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240415.263/README.md` & `pkscreener-0.44.20240415.264/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.262/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240415.263/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.262/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240415.263/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.262/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240415.263/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240415.263/pkscreener/__init__.py` & `pkscreener-0.44.20240415.264/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.263/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240415.264/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.263/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240415.264/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.263/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240415.264/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.263/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240415.264/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.263/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240415.264/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.263/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240415.264/pkscreener/classes/MarketStatus.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,17 @@
 
     def getMarketStatus(self, progress=None, task_id=0, exchangeSymbol="^NSEI"):
         lngStatus = ""
         try:
             if progress:
                 progress[task_id] = {"progress": 0, "total": 1}
             _,lngStatus,_ = MarketStatus.nseFetcher.capitalMarketStatus(exchange=exchangeSymbol)
+            if exchangeSymbol in ["^NSEI","^BSESN"]:
+                _,bseStatus,_ = MarketStatus.nseFetcher.capitalMarketStatus(exchange="^BSESN")
+                lngStatus = f"{lngStatus} | {bseStatus}"
             if progress:
                 progress[task_id] = {"progress": 1, "total": 1}
         except Exception as e:# pragma: no cover
             default_logger().debug(e, exc_info=True)
             pass
         self.marketStatus = lngStatus
         return lngStatus
```

### Comparing `pkscreener-0.44.20240415.263/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240415.264/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.263/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240415.264/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.263/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240415.264/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.263/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240415.264/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.263/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240415.264/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.263/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240415.264/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.263/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240415.264/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.263/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240415.264/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.263/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240415.264/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.263/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240415.264/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.263/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240415.264/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.263/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240415.264/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.263/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240415.264/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.263/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240415.264/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.263/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240415.264/pkscreener/classes/Utility.py`

 * *Files 3% similar despite different names*

```diff
@@ -281,14 +281,58 @@
         return x
 
     def formatRatio(ratio, volumeRatio):
         if ratio >= volumeRatio and ratio != np.nan and (not math.isinf(ratio)):
             return colorText.BOLD + colorText.GREEN + str(ratio) + "x" + colorText.END
         return colorText.BOLD + colorText.FAIL + str(ratio) + "x" + colorText.END
 
+    def addQuickWatermark(sourceImage:Image, xVertical=None):
+        width, height = sourceImage.size
+        watermarkText = f"© {datetime.date.today().year} pkjmesra | PKScreener"
+        message_length = len(watermarkText)
+        # load font (tweak ratio based on a particular font)
+        FONT_RATIO = 1.5
+        DIAGONAL_PERCENTAGE = .85
+        diagonal_length = int(math.sqrt((width**2) + (height**2)))
+        diagonal_to_use = diagonal_length * DIAGONAL_PERCENTAGE
+        height_to_use = height * DIAGONAL_PERCENTAGE
+        font_size = int(diagonal_to_use / (message_length / FONT_RATIO))
+        font_size_vertical = int(height_to_use / (message_length / FONT_RATIO))
+        fontPath = tools.setupReportFont()
+        font = ImageFont.truetype(fontPath, font_size)
+        font_vertical = ImageFont.truetype(fontPath, font_size_vertical)
+        #font = ImageFont.load_default() # fallback
+
+        # watermark
+        opacity = int(256 * .6)
+        mark_width, mark_height = font.getsize(watermarkText)
+        watermark = Image.new('RGBA', (mark_width, mark_height), (0, 0, 0, 0))
+        draw = ImageDraw.Draw(watermark)
+        draw.text((0, 0), text=watermarkText, font=font, fill=(128, 128, 128, opacity))
+        angle = math.degrees(math.atan(height/width))
+        watermark_diag = watermark.rotate(angle, expand=1)
+        
+        mark_width_ver, mark_height_ver = font_vertical.getsize(watermarkText)
+        watermark_ver = Image.new('RGBA', (mark_width_ver, mark_height_ver), (0, 0, 0, 0))
+        draw = ImageDraw.Draw(watermark_ver)
+        draw.text((0, 0), text=watermarkText, font=font_vertical, fill=(128, 128, 128, opacity))
+        watermark_vertical = watermark_ver.rotate(90, expand=1)
+
+        # merge
+        wx, wy = watermark_diag.size
+        px = int((width - wx)/2)
+        py = int((height - wy)/2)
+        wxv, wyv = watermark_vertical.size
+        pxv =  int((width - wxv)/12) if xVertical is None else xVertical
+        pyv= int((height - wyv)/2)
+        sourceImage.paste(watermark_diag, (px, py, px + wx, py + wy), watermark_diag)
+        sourceImage.paste(watermark_vertical, (pxv, pyv, pxv + wxv, pyv + wyv), watermark_vertical)
+        # sourceImage.show()
+        return sourceImage
+
     def removeAllColorStyles(styledText):
         styles = [
             colorText.HEAD,
             colorText.END,
             colorText.BOLD,
             colorText.UNDR,
             colorText.BLUE,
@@ -370,15 +414,15 @@
             if (("RUNNER" in os.environ.keys() and os.environ["RUNNER"] == "LOCAL_RUN_SCANNER")):
                 return
         warnings.filterwarnings("ignore", category=DeprecationWarning)
         # First 4 lines are headers. Last 1 line is bottom grid line
         fontPath = tools.setupReportFont()
         artfont = ImageFont.truetype(fontPath, 30)
         stdfont = ImageFont.truetype(fontPath, 60)
-
+        
         bgColor, gridColor, artColor, menuColor = tools.getDefaultColors()
 
         dfs_to_print = [styledTable, backtestSummary, backtestDetail]
         unstyled_dfs = [table, backtestSummary, backtestDetail]
         reportTitle = f"[+] As of {PKDateUtilities.currentDateTime().strftime('%d-%m-%y %H.%M.%S')} IST > You chose {label}"
         titleLabels = [
             f"[+] Scan results for {label} :",
@@ -409,14 +453,15 @@
         legendText = tools.getLegendHelpText(table,backtestSummary)
         _, artfont_legendtext_height = artfont.getsize_multiline(legendText)
         column_separator = "|"
         line_separator = "+"
         stdfont_sep_width, _ = stdfont.getsize_multiline(column_separator)
 
         startColValue = 100
+        xVertical = startColValue
         rowPixelRunValue = 9
         im_width = max(
             artfont_arttext_width,
             stdFont_oneLinelabel_width,
             stdFont_scanResulttext_width,
             stdFont_backtestSummary_text_width,
             stdFont_backtestDetail_text_width,
@@ -524,14 +569,16 @@
                             draw.text(
                                 (colPixelRunValue, rowPixelRunValue),
                                 cleanValue,
                                 font=stdfont,
                                 fill=style,
                             )
                             colPixelRunValue = colPixelRunValue + col_width
+                            if columnNumber == 0:
+                                xVertical = int(columnNumber/2)
 
                         columnNumber = columnNumber + 1
                     if len(valueScreenCols) > 0:
                         # Close the row with the separator
                         draw.text(
                             (colPixelRunValue, rowPixelRunValue),
                             column_separator,
@@ -579,14 +626,15 @@
                 )
                 # Move to the next text in the same line
                 colPixelRunValue += col_width + 2
             # Let's go to the next line
             rowPixelRunValue += artfont_line_height + 1
 
         im = im.resize(im.size, Image.ANTIALIAS, reducing_gap=2)
+        im = tools.addQuickWatermark(im,xVertical)
         im.save(filename, format="png", bitmap_format="png", optimize=True, quality=20)
         # if 'RUNNER' not in os.environ.keys() and 'PKDevTools_Default_Log_Level' in os.environ.keys():
         # im.show()
 
     def wrapFitLegendText(table, backtestSummary, legendText):
         wrapper = textwrap.TextWrapper(
             width=2
```

### Comparing `pkscreener-0.44.20240415.263/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240415.264/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.263/pkscreener/classes/keys.py` & `pkscreener-0.44.20240415.264/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.263/pkscreener/courbd.ttf` & `pkscreener-0.44.20240415.264/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.263/pkscreener/globals.py` & `pkscreener-0.44.20240415.264/pkscreener/globals.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 from PKDevTools.classes.ColorText import colorText
 from PKDevTools.classes.PKDateUtilities import PKDateUtilities
 from PKDevTools.classes.log import default_logger #, tracelog
 from PKDevTools.classes.Telegram import (
     is_token_telegram_configured,
     send_document,
     send_message,
+    send_photo
 )
 from PKNSETools.morningstartools.PKMorningstarDataFetcher import morningstarDataFetcher
 from PKNSETools.Nasdaq.PKNasdaqIndex import PKNasdaqIndexFetcher
 from tabulate import tabulate
 
 import pkscreener.classes.ConfigManager as ConfigManager
 import pkscreener.classes.Fetcher as Fetcher
@@ -1729,15 +1730,15 @@
                         caption_df[col] = caption_df[col].astype(str)
                     caption_results = colorText.miniTabulator().tabulate(
                         caption_df,
                         headers="keys",
                         tablefmt=colorText.No_Pad_GridFormat,
                         maxcolwidths=[None,None,4,3]
                     ).encode("utf-8").decode(STD_ENCODING).replace("-+-----+-----+-----+","-+-----+----+---+").replace("%  ","% ").replace("=+=====+=====+=====+","=+=====+====+===+").replace("Vol  |","Vol|").replace("x  ","x")
-                    caption = f"{caption}.Open attached image for more. 5 samples:<pre>{caption_results}</pre>" #<i>Author is <u><b>NOT</b> a SEBI registered financial advisor</u> and MUST NOT be deemed as one.</i>"
+                    caption = f"{caption}.Open attached image for more. Samples:<pre>{caption_results}</pre>" #<i>Author is <u><b>NOT</b> a SEBI registered financial advisor</u> and MUST NOT be deemed as one.</i>"
                 if not testing and not userPassedArgs.runintradayanalysis:
                     sendQuickScanResult(
                         menuChoiceHierarchy,
                         user,
                         tabulated_results,
                         markdown_results,
                         caption,
@@ -1764,15 +1765,15 @@
                                 menuChoiceHierarchy,
                                 backtestSummary=tabulated_backtest_summary,
                                 backtestDetail=tabulated_backtest_detail,
                             )
                             caption = f"Backtest data for stocks listed in <b>{title}</b> scan results. See more past backtest data at https://pkjmesra.github.io/PKScreener/BacktestReports.html"
                             sendMessageToTelegramChannel(
                                 message=None,
-                                photo_filePath=pngName + backtestExtension,
+                                document_filePath=pngName + backtestExtension,
                                 caption=caption,
                                 user=user,
                             )
                             os.remove(pngName + backtestExtension)
                         except Exception as e:  # pragma: no cover
                             default_logger().debug(e, exc_info=True)
                             pass
@@ -1944,15 +1945,15 @@
             addendum=addendum,
             addendumLabel=addendumLabel,
             summaryLabel = summaryLabel,
             detailLabel = detailLabel
         )
         sendMessageToTelegramChannel(
             message=None,
-            photo_filePath=pngName + pngExtension,
+            document_filePath=pngName + pngExtension,
             caption=caption,
             user=user,
         )
         os.remove(pngName + pngExtension)
     except Exception as e:  # pragma: no cover
         default_logger().debug(e, exc_info=True)
         pass
@@ -2229,23 +2230,39 @@
         + colorText.GREEN
         + f"[+] Screening Completed. Found {len(screenResults) if screenResults is not None else 0} results in {round(elapsed_time,2)} sec.! Press Enter to Continue.."
         + colorText.END
     )
     if defaultAnswer is None:
         input("Press <Enter> to continue...")
 
+def sendGlobalMarketBarometer(userArgs=None):
+    from pkscreener.classes import Barometer
+    caption = "Global Market Barometer with India market Performance (top) and Valuation (bottom)"
+    gmbPath = Barometer.getGlobalMarketBarometerValuation()
+    try:
+        if gmbPath is not None:
+            sendMessageToTelegramChannel(
+                message=None,
+                photo_filePath=gmbPath,
+                caption=caption,
+                user=(userArgs.user if userArgs is not None else None),
+            )
+            os.remove(gmbPath)
+    except:
+        pass
 
 def sendMessageToTelegramChannel(
     message=None, photo_filePath=None, document_filePath=None, caption=None, user=None
 ):
     global userPassedArgs, test_messages_queue
-    test_messages_queue.append(f"message:{message}\ncaption:{caption}\nuser:{user}\ndocument:{document_filePath}")
-    if len(test_messages_queue) >10:
-        test_messages_queue.pop(0)
-    if user is None and userPassedArgs.user is not None:
+    if test_messages_queue is not None:
+        test_messages_queue.append(f"message:{message}\ncaption:{caption}\nuser:{user}\ndocument:{document_filePath}")
+        if len(test_messages_queue) >10:
+            test_messages_queue.pop(0)
+    if user is None and userPassedArgs is not None and userPassedArgs.user is not None:
         user = userPassedArgs.user
     if user is not None and caption is not None:
         caption = f"{caption.replace('&','n')}."
     if message is not None:
         try:
             message = message.replace("&", "n").replace("<","*")
             send_message(message, userID=user)
@@ -2253,26 +2270,26 @@
             default_logger().debug(e, exc_info=True)
     else:
         message = ""
     if photo_filePath is not None:
         try:
             if caption is not None:
                 caption = f"{caption.replace('&','n')}"
-            send_document(photo_filePath, caption, userID=user)
+            send_photo(photo_filePath, caption, userID=user)
             # Breather for the telegram API to be able to send the heavy photo
             sleep(2)
         except Exception as e:  # pragma: no cover
             default_logger().debug(e, exc_info=True)
     if document_filePath is not None:
         try:
             if caption is not None:
                 caption = f"{caption.replace('&','n')}"
             send_document(document_filePath, caption, userID=user)
             # Breather for the telegram API to be able to send the document
-            sleep(1)
+            sleep(2)
         except Exception as e:  # pragma: no cover
             default_logger().debug(e, exc_info=True)
     if user is not None:
         # Send an update to dev channel
         send_message(
             "Responded back to userId:{0} with {1}.{2}".format(user, caption, message),
             userID="-1001785195297",
```

### Comparing `pkscreener-0.44.20240415.263/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240415.264/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.263/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240415.264/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.263/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240415.264/pkscreener/pkscreenercli.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,14 +109,20 @@
 )
 argParser.add_argument(
     "--backtestdaysago",
     help="Run scanner for -b days ago from today.",
     required=False,
 )
 argParser.add_argument(
+    "--barometer",
+    action="store_true",
+    help="Send global market barometer to telegram channel or a user",
+    required=False,
+)
+argParser.add_argument(
     "-c",
     "--croninterval",
     help="Pass interval in seconds to wait before the program is run again with same parameters",
     required=False,
 )
 argParser.add_argument(
     "-d",
@@ -271,15 +277,15 @@
                 + colorText.FAIL
                 + "[+] Neither ta-lib nor pandas_ta was located. You need at least one of them to continue! \n[+] Please follow instructions from README file under PKScreener repo: https://github.com/pkjmesra/PKScreener"
                 + colorText.END
             )
             input("Press any key to try anyway...")
 
 def runApplication():
-    from pkscreener.globals import main, sendQuickScanResult
+    from pkscreener.globals import main, sendQuickScanResult, sendGlobalMarketBarometer
     # From a previous call to main with args, it may have been mutated.
     # Let's stock to the original args passed by user
     argsv = argParser.parse_known_args()
     args = argsv[0]
     if args.runintradayanalysis:
         from pkscreener.classes.MenuOptions import menus
         runOptions = menus.allMenus(topLevel="C", index=12)
@@ -318,15 +324,18 @@
                                 tabulated_results=mark_down,
                                 markdown_results=mark_down,
                                 caption="IntradayAnalysis - Morning alert vs Market Close",
                                 pngName= f"PKS_IA_{PKDateUtilities.currentDateTime().strftime('%Y-%m-%d_%H:%M:%S')}",
                                 pngExtension= ".png"
                                 )
     else:
-        main(userArgs=args)
+        if args.barometer:
+            sendGlobalMarketBarometer(userArgs=args)
+        else:
+            main(userArgs=args)
 
 
 def pkscreenercli():
     global originalStdOut
     if sys.platform.startswith("darwin"):
         try:
             multiprocessing.set_start_method("fork")
```

### Comparing `pkscreener-0.44.20240415.263/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240415.264/pkscreener.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240415.263
+Version: 0.44.20240415.264
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240415.263.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240415.264.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.262/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240415.263/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.262/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240415.263/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240414.262/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240415.263/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240415.263/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240415.264/pkscreener.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 pkscreener.egg-info/PKG-INFO
 pkscreener.egg-info/SOURCES.txt
 pkscreener.egg-info/dependency_links.txt
 pkscreener.egg-info/entry_points.txt
 pkscreener.egg-info/not-zip-safe
 pkscreener.egg-info/top_level.txt
 pkscreener/classes/Backtest.py
+pkscreener/classes/Barometer.py
 pkscreener/classes/CandlePatterns.py
 pkscreener/classes/Changelog.py
 pkscreener/classes/ConfigManager.py
 pkscreener/classes/Fetcher.py
 pkscreener/classes/MarketStatus.py
 pkscreener/classes/MenuOptions.py
 pkscreener/classes/OtaUpdater.py
```

### Comparing `pkscreener-0.44.20240415.263/setup.py` & `pkscreener-0.44.20240415.264/setup.py`

 * *Files identical despite different names*

