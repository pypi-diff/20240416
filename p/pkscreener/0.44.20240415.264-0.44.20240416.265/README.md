# Comparing `tmp/pkscreener-0.44.20240415.264.tar.gz` & `tmp/pkscreener-0.44.20240416.265.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240415.264.tar", last modified: Mon Apr 15 17:39:20 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240416.265.tar", last modified: Tue Apr 16 06:24:08 2024, max compression
```

## Comparing `pkscreener-0.44.20240415.264.tar` & `pkscreener-0.44.20240416.265.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 17:39:20.881340 pkscreener-0.44.20240415.264/
--rw-rw-rw-   0        0        0     1086 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-04-15 17:39:20.881340 pkscreener-0.44.20240415.264/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 17:39:20.865721 pkscreener-0.44.20240415.264/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 17:39:20.881340 pkscreener-0.44.20240415.264/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5484 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    24554 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0     9291 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     3203 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    27587 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    20931 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    17381 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8037 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    17306 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    48885 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   113858 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    46266 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    76874 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-04-15 17:39:12.000000 pkscreener-0.44.20240415.264/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   113838 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/globals.py
--rw-rw-rw-   0        0        0      565 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    47815 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    18748 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-04-15 17:39:20.865721 pkscreener-0.44.20240415.264/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-04-15 17:39:20.000000 pkscreener-0.44.20240415.264/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1282 2024-04-15 17:39:20.000000 pkscreener-0.44.20240415.264/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 17:39:20.000000 pkscreener-0.44.20240415.264/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-04-15 17:39:20.000000 pkscreener-0.44.20240415.264/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-15 17:39:20.000000 pkscreener-0.44.20240415.264/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-04-15 17:39:20.000000 pkscreener-0.44.20240415.264/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-15 17:39:20.881340 pkscreener-0.44.20240415.264/setup.cfg
--rw-rw-rw-   0        0        0     4715 2024-04-15 17:34:34.000000 pkscreener-0.44.20240415.264/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 06:24:08.064062 pkscreener-0.44.20240416.265/
+-rw-rw-rw-   0        0        0     1086 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-04-16 06:24:08.064062 pkscreener-0.44.20240416.265/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 06:24:08.048444 pkscreener-0.44.20240416.265/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 06:24:08.064062 pkscreener-0.44.20240416.265/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5484 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    24554 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0     9291 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     3203 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    27587 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    20931 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    17381 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8037 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    17306 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    48885 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   113858 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    46266 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    76874 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-04-16 06:24:00.000000 pkscreener-0.44.20240416.265/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   114443 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      565 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    47815 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    19062 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-04-16 06:24:08.064062 pkscreener-0.44.20240416.265/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-04-16 06:24:07.000000 pkscreener-0.44.20240416.265/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1282 2024-04-16 06:24:08.000000 pkscreener-0.44.20240416.265/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 06:24:07.000000 pkscreener-0.44.20240416.265/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2024-04-16 06:24:07.000000 pkscreener-0.44.20240416.265/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 06:24:07.000000 pkscreener-0.44.20240416.265/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-04-16 06:24:07.000000 pkscreener-0.44.20240416.265/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-16 06:24:08.064062 pkscreener-0.44.20240416.265/setup.cfg
+-rw-rw-rw-   0        0        0     4715 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/setup.py
```

### Comparing `pkscreener-0.44.20240415.264/LICENSE` & `pkscreener-0.44.20240416.265/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.264/LICENSE-Others` & `pkscreener-0.44.20240416.265/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.264/PKG-INFO` & `pkscreener-0.44.20240416.265/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240415.264
+Version: 0.44.20240416.265
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240415.264.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240416.265.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240415.263/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240415.264/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240415.263/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240415.264/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240415.263/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240415.264/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240415.264/README.md` & `pkscreener-0.44.20240416.265/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240415.263/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240415.264/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240415.263/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240415.264/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240415.263/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240415.264/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240415.264/pkscreener/__init__.py` & `pkscreener-0.44.20240416.265/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.264/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240416.265/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.264/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240416.265/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.264/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240416.265/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.264/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240416.265/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.264/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240416.265/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.264/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240416.265/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.264/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240416.265/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.264/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240416.265/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.264/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240416.265/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.264/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240416.265/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.264/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240416.265/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.264/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240416.265/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.264/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240416.265/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.264/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240416.265/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.264/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240416.265/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.264/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240416.265/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.264/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240416.265/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.264/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240416.265/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.264/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240416.265/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.264/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240416.265/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.264/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240416.265/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.264/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240416.265/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.264/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240416.265/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.264/pkscreener/classes/keys.py` & `pkscreener-0.44.20240416.265/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.264/pkscreener/courbd.ttf` & `pkscreener-0.44.20240416.265/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.264/pkscreener/globals.py` & `pkscreener-0.44.20240416.265/pkscreener/globals.py`

 * *Files 1% similar despite different names*

```diff
@@ -1223,14 +1223,15 @@
                     shouldSend = False
                     for corp_df in corp_dfs:
                         if corp_df is None:
                             continue
                         tab_results = ""
                         if corp_df is not None and not corp_df.empty:
                             corp_df.set_index("Stock", inplace=True)
+                            corp_df = corp_df[~corp_df.index.duplicated(keep='first')]
                             tab_results = colorText.miniTabulator().tabulate(
                                 corp_df,
                                 headers="keys",
                                 tablefmt=colorText.No_Pad_GridFormat,
                                 # showindex = False,
                                 maxcolwidths=Utility.tools.getMaxColumnWidths(dividend_df)
                             ).encode("utf-8").decode(STD_ENCODING)
@@ -1632,14 +1633,22 @@
     MAX_ALLOWED = (100 if userPassedArgs.maxdisplayresults is None else min(int(userPassedArgs.maxdisplayresults),100)) if not testing else 1
     tabulated_backtest_summary = ""
     tabulated_backtest_detail = ""
     recordDate = PKDateUtilities.tradingDate().strftime('%Y-%m-%d') if (userPassedArgs.backtestdaysago is None) else (PKDateUtilities.nthPastTradingDateStringFromFutureDate(int(userPassedArgs.backtestdaysago)))
     if user is None and userPassedArgs.user is not None:
         user = userPassedArgs.user
     Utility.tools.clearScreen()
+    if screenResults is not None and len(screenResults) > 0:
+        screenResults = screenResults[~screenResults.index.duplicated(keep='first')]
+        saveResults = saveResults[~saveResults.index.duplicated(keep='first')]
+        if "Stock" in screenResults.columns:
+            screenResults.drop_duplicates(keep="first", inplace=True)
+        if "Stock" in saveResults.columns:
+            saveResults.drop_duplicates(keep="first", inplace=True)
+
     print(
         colorText.BOLD
         + colorText.FAIL
         + f"[+] You chose: {menuChoiceHierarchy}"
         + colorText.END
     )
     pngName = f'PKS_{PKScanRunner.getFormattedChoices(userPassedArgs,selectedChoice)}_{PKDateUtilities.currentDateTime().strftime("%d-%m-%y_%H.%M.%S")}'
@@ -1691,15 +1700,16 @@
                 saveResultsTrimmed = saveResults.copy()
                 # No point sending a photo with more than MAX_ALLOWED stocks.
                 warn_text = (
                     f" but showing only {MAX_ALLOWED}. "
                     if (len(saveResults) > MAX_ALLOWED)
                     else ""
                 )
-                caption = f"({len(saveResults)}{'+' if (len(saveResults) > MAX_ALLOWED) else ''} stocks found in {str(int(elapsed_time))} sec){warn_text}.{title}"
+                caption = f"{title}"
+                elapsed_text = f"<i>({len(saveResults)}{'+' if (len(saveResults) > MAX_ALLOWED) else ''} stocks found in {str(int(elapsed_time))} sec.){warn_text}</i>"
                 backtestExtension = "_backtest.png"
                 if len(screenResultsTrimmed) > MAX_ALLOWED:
                     screenResultsTrimmed = screenResultsTrimmed.head(MAX_ALLOWED)
                     saveResultsTrimmed = saveResultsTrimmed.head(MAX_ALLOWED)
                     if saveResultsTrimmed is not None and len(saveResultsTrimmed) > 0:
                         tabulated_results = colorText.miniTabulator().tabulate(
                             screenResultsTrimmed,
@@ -1730,15 +1740,15 @@
                         caption_df[col] = caption_df[col].astype(str)
                     caption_results = colorText.miniTabulator().tabulate(
                         caption_df,
                         headers="keys",
                         tablefmt=colorText.No_Pad_GridFormat,
                         maxcolwidths=[None,None,4,3]
                     ).encode("utf-8").decode(STD_ENCODING).replace("-+-----+-----+-----+","-+-----+----+---+").replace("%  ","% ").replace("=+=====+=====+=====+","=+=====+====+===+").replace("Vol  |","Vol|").replace("x  ","x")
-                    caption = f"{caption}.Open attached image for more. Samples:<pre>{caption_results}</pre>" #<i>Author is <u><b>NOT</b> a SEBI registered financial advisor</u> and MUST NOT be deemed as one.</i>"
+                    caption = f"{caption}.Open attached image for more. Samples:<pre>{caption_results}</pre>{elapsed_text}" #<i>Author is <u><b>NOT</b> a SEBI registered financial advisor</u> and MUST NOT be deemed as one.</i>"
                 if not testing and not userPassedArgs.runintradayanalysis:
                     sendQuickScanResult(
                         menuChoiceHierarchy,
                         user,
                         tabulated_results,
                         markdown_results,
                         caption,
```

### Comparing `pkscreener-0.44.20240415.264/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240416.265/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.264/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240416.265/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.264/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240416.265/pkscreener/pkscreenercli.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # Pyinstaller compile Linux  : pyinstaller --onefile --icon=screenshots/icon.ico pkscreener/pkscreenercli.py  --hidden-import cmath --hidden-import talib.stream --hidden-import numpy --hidden-import pandas --hidden-import alive-progress
 import warnings
 warnings.simplefilter("ignore", UserWarning,append=True)
 import argparse
 import builtins
 import logging
 import traceback
-
+import datetime
 # Keep module imports prior to classes
 import os
 import sys
 import tempfile
 os.environ["PYTHONWARNINGS"]="ignore::UserWarning"
 import multiprocessing
 
@@ -59,14 +59,16 @@
 os.environ["TF_CPP_MIN_LOG_LEVEL"] = "3"
 os.environ["AUTOGRAPH_VERBOSITY"] = "0"
 # from pkscreener.classes.IntradayMonitor import intradayMonitorInstance
 
 printenabled=False
 originalStdOut=None
 original__stdout=None
+cron_runs=0
+
 def decorator(func):
     def new_func(*args, **kwargs):
         if printenabled:
             try:
                 func(*args,**kwargs)
             except Exception as e:# pragma: no cover
                 default_logger().debug(e, exc_info=True)
@@ -476,18 +478,21 @@
         ):
             sleepUntilNextExecution = False
         if (PKDateUtilities.secondsBeforeOpenTime() <= -3600) and (
             PKDateUtilities.secondsBeforeOpenTime() >= (-3600 - 1.5 * int(args.croninterval))
         ):
             sleepUntilNextExecution = False
         sleep(int(args.croninterval))
-    print(
-        colorText.BOLD + colorText.GREEN + "=> Going to fetch again!" + colorText.END,
-        end="\r",
-        flush=True,
-    )
-    sleep(3)
+    global cron_runs
+    if cron_runs > 0:
+        print(
+            colorText.BOLD + colorText.GREEN + f'=> Going to fetch again in {int(args.croninterval)} sec. at {(PKDateUtilities.currentDateTime() + datetime.timedelta(seconds=120)).strftime("%Y-%m-%d %H:%M:%S")} IST...' + colorText.END,
+            end="\r",
+            flush=True,
+        )
+        sleep(int(args.croninterval) if not args.testbuild else 3)
     runApplication()
+    cron_runs += 1
 
 
 if __name__ == "__main__":
     pkscreenercli()
```

### Comparing `pkscreener-0.44.20240415.264/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240416.265/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240415.264
+Version: 0.44.20240416.265
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240415.264.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240416.265.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240415.263/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240415.264/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240415.263/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240415.264/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240415.263/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240415.264/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240415.264/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240416.265/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240415.264/setup.py` & `pkscreener-0.44.20240416.265/setup.py`

 * *Files identical despite different names*

