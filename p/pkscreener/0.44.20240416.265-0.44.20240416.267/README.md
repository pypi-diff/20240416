# Comparing `tmp/pkscreener-0.44.20240416.265.tar.gz` & `tmp/pkscreener-0.44.20240416.267.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240416.265.tar", last modified: Tue Apr 16 06:24:08 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240416.267.tar", last modified: Tue Apr 16 18:31:15 2024, max compression
```

## Comparing `pkscreener-0.44.20240416.265.tar` & `pkscreener-0.44.20240416.267.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 06:24:08.064062 pkscreener-0.44.20240416.265/
--rw-rw-rw-   0        0        0     1086 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-04-16 06:24:08.064062 pkscreener-0.44.20240416.265/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 06:24:08.048444 pkscreener-0.44.20240416.265/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 06:24:08.064062 pkscreener-0.44.20240416.265/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5484 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    24554 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0     9291 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     3203 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    27587 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    20931 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    17381 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8037 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    17306 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    48885 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   113858 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    46266 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    76874 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-04-16 06:24:00.000000 pkscreener-0.44.20240416.265/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   114443 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/globals.py
--rw-rw-rw-   0        0        0      565 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    47815 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    19062 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-04-16 06:24:08.064062 pkscreener-0.44.20240416.265/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-04-16 06:24:07.000000 pkscreener-0.44.20240416.265/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1282 2024-04-16 06:24:08.000000 pkscreener-0.44.20240416.265/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 06:24:07.000000 pkscreener-0.44.20240416.265/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-04-16 06:24:07.000000 pkscreener-0.44.20240416.265/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 06:24:07.000000 pkscreener-0.44.20240416.265/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-04-16 06:24:07.000000 pkscreener-0.44.20240416.265/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-16 06:24:08.064062 pkscreener-0.44.20240416.265/setup.cfg
--rw-rw-rw-   0        0        0     4715 2024-04-16 06:21:01.000000 pkscreener-0.44.20240416.265/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 18:31:15.596118 pkscreener-0.44.20240416.267/
+-rw-rw-rw-   0        0        0     1086 2024-04-16 18:28:03.000000 pkscreener-0.44.20240416.267/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-04-16 18:28:03.000000 pkscreener-0.44.20240416.267/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-04-16 18:31:15.596118 pkscreener-0.44.20240416.267/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-04-16 18:28:03.000000 pkscreener-0.44.20240416.267/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 18:31:15.580490 pkscreener-0.44.20240416.267/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-04-16 18:28:03.000000 pkscreener-0.44.20240416.267/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 18:31:15.596118 pkscreener-0.44.20240416.267/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-04-16 18:28:03.000000 pkscreener-0.44.20240416.267/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5649 2024-04-16 18:28:03.000000 pkscreener-0.44.20240416.267/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-04-16 18:28:03.000000 pkscreener-0.44.20240416.267/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-04-16 18:28:03.000000 pkscreener-0.44.20240416.267/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    24554 2024-04-16 18:28:03.000000 pkscreener-0.44.20240416.267/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0     9291 2024-04-16 18:28:03.000000 pkscreener-0.44.20240416.267/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     3237 2024-04-16 18:28:03.000000 pkscreener-0.44.20240416.267/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    27587 2024-04-16 18:28:03.000000 pkscreener-0.44.20240416.267/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-04-16 18:28:03.000000 pkscreener-0.44.20240416.267/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    20931 2024-04-16 18:28:03.000000 pkscreener-0.44.20240416.267/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    17381 2024-04-16 18:28:03.000000 pkscreener-0.44.20240416.267/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-04-16 18:28:03.000000 pkscreener-0.44.20240416.267/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8037 2024-04-16 18:28:03.000000 pkscreener-0.44.20240416.267/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-04-16 18:28:03.000000 pkscreener-0.44.20240416.267/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-04-16 18:28:03.000000 pkscreener-0.44.20240416.267/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    17306 2024-04-16 18:28:03.000000 pkscreener-0.44.20240416.267/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-04-16 18:28:03.000000 pkscreener-0.44.20240416.267/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    48885 2024-04-16 18:28:03.000000 pkscreener-0.44.20240416.267/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   113858 2024-04-16 18:28:03.000000 pkscreener-0.44.20240416.267/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    46266 2024-04-16 18:28:03.000000 pkscreener-0.44.20240416.267/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-04-16 18:28:03.000000 pkscreener-0.44.20240416.267/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    77005 2024-04-16 18:28:03.000000 pkscreener-0.44.20240416.267/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-04-16 18:28:03.000000 pkscreener-0.44.20240416.267/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-04-16 18:31:07.000000 pkscreener-0.44.20240416.267/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-04-16 18:28:03.000000 pkscreener-0.44.20240416.267/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-04-16 18:28:03.000000 pkscreener-0.44.20240416.267/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   114653 2024-04-16 18:28:03.000000 pkscreener-0.44.20240416.267/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      565 2024-04-16 18:28:03.000000 pkscreener-0.44.20240416.267/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    47815 2024-04-16 18:28:03.000000 pkscreener-0.44.20240416.267/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    19391 2024-04-16 18:28:03.000000 pkscreener-0.44.20240416.267/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-04-16 18:31:15.580490 pkscreener-0.44.20240416.267/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-04-16 18:31:15.000000 pkscreener-0.44.20240416.267/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1282 2024-04-16 18:31:15.000000 pkscreener-0.44.20240416.267/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 18:31:15.000000 pkscreener-0.44.20240416.267/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2024-04-16 18:31:15.000000 pkscreener-0.44.20240416.267/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 18:31:15.000000 pkscreener-0.44.20240416.267/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-04-16 18:31:15.000000 pkscreener-0.44.20240416.267/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-16 18:31:15.596118 pkscreener-0.44.20240416.267/setup.cfg
+-rw-rw-rw-   0        0        0     4715 2024-04-16 18:28:04.000000 pkscreener-0.44.20240416.267/setup.py
```

### Comparing `pkscreener-0.44.20240416.265/LICENSE` & `pkscreener-0.44.20240416.267/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.265/LICENSE-Others` & `pkscreener-0.44.20240416.267/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.265/PKG-INFO` & `pkscreener-0.44.20240416.267/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240416.265
+Version: 0.44.20240416.267
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240416.265.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240416.267.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240415.264/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240416.265/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240415.264/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240416.265/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240415.264/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240416.265/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240416.265/README.md` & `pkscreener-0.44.20240416.267/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240415.264/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240416.265/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240415.264/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240416.265/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240415.264/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240416.265/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240416.265/pkscreener/__init__.py` & `pkscreener-0.44.20240416.267/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.265/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240416.267/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.265/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240416.267/pkscreener/classes/Barometer.py`

 * *Files 9% similar despite different names*

```diff
@@ -84,15 +84,18 @@
         # watermark = Utility.tools.getWatermarkImage(gmbPerformance)
         gmbPerformance = Utility.tools.addQuickWatermark(gmbPerformance)
         gmbValuation = Utility.tools.addQuickWatermark(gmbValuation)
         gmbCombined = Image.new('RGB',(gmbPerf_size[0], gmbPerf_size[1]+gmbValue_size[1]+gapHeight), bgColor)
         gmbCombined.paste(gmbPerformance,(0,0))
         draw = ImageDraw.Draw(gmbCombined)
         # artwork
-        repoText = f'https://GitHub.com/pkjmesra/pkscreener/ | © {datetime.date.today().year} pkjmesra | https://t.me/PKScreener\n{MarketStatus().getMarketStatus(exchangeSymbol="^NSEI")}\n{MarketStatus().getMarketStatus(exchangeSymbol="^BSESN")}\n{MarketStatus().getMarketStatus(exchangeSymbol="^IXIC")}'
+        nseMarketStatus = MarketStatus().getMarketStatus(exchangeSymbol="^NSEI",namedOnly=True)
+        bseMarketStatus = MarketStatus().getMarketStatus(exchangeSymbol="^BSESN",namedOnly=True)
+        nasdaqMarketStatus = MarketStatus().getMarketStatus(exchangeSymbol="^IXIC")
+        repoText = f'https://GitHub.com/pkjmesra/pkscreener/ | © {datetime.date.today().year} pkjmesra | https://t.me/PKScreener\n{nseMarketStatus}\n{bseMarketStatus}\n{nasdaqMarketStatus}'
         draw.text((5, gmbPerf_size[1]+5), Utility.tools.removeAllColorStyles(repoText), font=artfont, fill="lightgreen")
         gmbCombined.paste(gmbValuation,(0,gmbPerf_size[1]+gapHeight))
         gmbCombined.save(os.path.join(folderPath,"gmb.png"),"PNG")
         gmbPath = os.path.join(folderPath,"gmb.png")
         # gmbCombined.show()
     except: #Exception as e:
         # print(e)
```

### Comparing `pkscreener-0.44.20240416.265/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240416.267/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.265/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240416.267/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.265/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240416.267/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.265/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240416.267/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.265/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240416.267/pkscreener/classes/MarketStatus.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,21 +54,21 @@
             self.marketStatus = ""
             return self.marketStatus
     
     @marketStatus.setter
     def marketStatus(self, status):
         self.attributes["marketStatus"] = status
 
-    def getMarketStatus(self, progress=None, task_id=0, exchangeSymbol="^NSEI"):
+    def getMarketStatus(self, progress=None, task_id=0, exchangeSymbol="^NSEI",namedOnly=False):
         lngStatus = ""
         try:
             if progress:
                 progress[task_id] = {"progress": 0, "total": 1}
             _,lngStatus,_ = MarketStatus.nseFetcher.capitalMarketStatus(exchange=exchangeSymbol)
-            if exchangeSymbol in ["^NSEI","^BSESN"]:
+            if exchangeSymbol in ["^NSEI","^BSESN"] and not namedOnly:
                 _,bseStatus,_ = MarketStatus.nseFetcher.capitalMarketStatus(exchange="^BSESN")
                 lngStatus = f"{lngStatus} | {bseStatus}"
             if progress:
                 progress[task_id] = {"progress": 1, "total": 1}
         except Exception as e:# pragma: no cover
             default_logger().debug(e, exc_info=True)
             pass
```

### Comparing `pkscreener-0.44.20240416.265/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240416.267/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.265/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240416.267/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.265/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240416.267/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.265/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240416.267/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.265/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240416.267/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.265/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240416.267/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.265/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240416.267/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.265/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240416.267/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.265/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240416.267/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.265/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240416.267/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.265/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240416.267/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.265/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240416.267/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.265/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240416.267/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.265/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240416.267/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.265/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240416.267/pkscreener/classes/Utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -444,15 +444,15 @@
         if addendum is not None and len(addendum) > 0:
             unstyled_addendum = tools.removeAllColorStyles(addendum)
             stdfont_addendumtext_width , stdfont_addendumtext_height = stdfont.getsize_multiline(unstyled_addendum)
             titleLabels.append(addendumLabel)
             dfs_to_print.append(addendum)
             unstyled_dfs.append(unstyled_addendum)
 
-        repoText = tools.getRepoHelpText()
+        repoText = tools.getRepoHelpText(table,backtestSummary)
         artfont_repotext_width, artfont_repotext_height = artfont.getsize_multiline(repoText)
         legendText = tools.getLegendHelpText(table,backtestSummary)
         _, artfont_legendtext_height = artfont.getsize_multiline(legendText)
         column_separator = "|"
         line_separator = "+"
         stdfont_sep_width, _ = stdfont.getsize_multiline(column_separator)
 
@@ -504,15 +504,15 @@
             rowPixelRunValue += stdFont_oneLinelabel_height
             unstyledLines = unstyled_dfs[counter].splitlines()
             lineNumber = 0
             screenLines = df.splitlines()
             for line in screenLines:
                 _, stdfont_line_height = stdfont.getsize_multiline(line)
                 # Print the row separators
-                if (line.startswith(line_separator)):
+                if not (line.startswith(column_separator)):
                     draw.text(
                         (colPixelRunValue, rowPixelRunValue),
                         line,
                         font=stdfont,
                         fill=gridColor,
                     )
                     rowPixelRunValue += stdfont_line_height + 1
@@ -691,17 +691,18 @@
         legendText = f"{legendText} shows the market-cap weighted portfolio weight to consider investing.\n"
         legendText = tools.wrapFitLegendText(table,backtestSummary, legendText)
         # legendText = legendText.replace("***:", colorText.END + colorText.WHITE)
         # legendText = legendText.replace("*** ", colorText.END + colorText.FAIL)
         # return colorText.WHITE + legendText + colorText.END
         return legendText
 
-    def getRepoHelpText():
+    def getRepoHelpText(table,backtestSummary):
         repoText = f"Source: https://GitHub.com/pkjmesra/pkscreener/  | © {datetime.date.today().year} pkjmesra | Telegram: https://t.me/PKScreener |"
-        repoText = f"{repoText}\nThe author is NOT a financial advisor and is NOT SEBI registered. This report is for learning/analysis purposes ONLY. Author assumes no responsibility or liability for any errors or omissions in this report or repository, or gain/loss bearing out of this analysis. The user MUST take advise ONLY from registered SEBI financial advisors only.\n"
+        disclaimer = f"The author is NOT a financial advisor and is NOT SEBI registered. This report is for learning/analysis purposes ONLY. Author assumes no responsibility or liability for any errors or omissions in this report or repository, or gain/loss bearing out of this analysis. The user MUST take advise ONLY from registered SEBI financial advisors only."
+        repoText = f"{repoText}\n{tools.wrapFitLegendText(table,backtestSummary,disclaimer)}"
         repoText = f"{repoText}\n[+] Understanding this report:\n\n"
         return repoText
 
     def set_github_output(name, value):
         if "GITHUB_OUTPUT" in os.environ.keys():
             with open(os.environ["GITHUB_OUTPUT"], "a") as fh:
                 print(f"{name}={value}", file=fh)
```

### Comparing `pkscreener-0.44.20240416.265/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240416.267/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.265/pkscreener/classes/keys.py` & `pkscreener-0.44.20240416.267/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.265/pkscreener/courbd.ttf` & `pkscreener-0.44.20240416.267/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.265/pkscreener/globals.py` & `pkscreener-0.44.20240416.267/pkscreener/globals.py`

 * *Files 2% similar despite different names*

```diff
@@ -1169,36 +1169,36 @@
             if not downloadOnly and menuOption in ["X", "G", "C"]:
                 if menuOption == "G":
                     userPassedArgs.backtestdaysago = backtestPeriod
                 if screenResults is not None and len(screenResults) > 0:
                     screenResults, saveResults = labelDataForPrinting(
                         screenResults, saveResults, configManager, volumeRatio, executeOption, reversalOption or respChartPattern
                     )
-                    ticker_list = list(saveResults.index)
-                    marketCaps = fetcher.fetchAdditionalTickerInfo(ticker_list)
-                    saveResults["MCapWt%"] = 0
-                    numShares = []
-                    for ticker in ticker_list:
-                        try:
-                            mCap = marketCaps.get(f"{ticker}.NS")
-                            mCap = round(mCap.get("marketCap"),0)
-                        except:
-                            mCap = 0
-                            pass
-                        saveResults.loc[ticker, 'MCapWt%'] = mCap
-                    # Let's get the weighted no. of shares
-                    marketCapSum = sum(saveResults["MCapWt%"])
-                    for ticker in ticker_list:
-                        try:
-                            saveResults.loc[ticker, 'MCapWt%'] = int(round(saveResults.loc[ticker, 'MCapWt%']/marketCapSum,2)*100)
-                        except:
-                            saveResults.loc[ticker, 'MCapWt%'] = 0
-                            pass
-                        numShares.append(saveResults.loc[ticker, 'MCapWt%'])
-                    screenResults["MCapWt%"] = numShares
+                    # ticker_list = list(saveResults.index)
+                    # marketCaps = fetcher.fetchAdditionalTickerInfo(ticker_list)
+                    # saveResults["MCapWt%"] = 0
+                    # numShares = []
+                    # for ticker in ticker_list:
+                    #     try:
+                    #         mCap = marketCaps.get(f"{ticker}.NS")
+                    #         mCap = round(mCap.get("marketCap"),0)
+                    #     except:
+                    #         mCap = 0
+                    #         pass
+                    #     saveResults.loc[ticker, 'MCapWt%'] = mCap
+                    # # Let's get the weighted no. of shares
+                    # marketCapSum = sum(saveResults["MCapWt%"])
+                    # for ticker in ticker_list:
+                    #     try:
+                    #         saveResults.loc[ticker, 'MCapWt%'] = int(round(saveResults.loc[ticker, 'MCapWt%']/marketCapSum,2)*100)
+                    #     except:
+                    #         saveResults.loc[ticker, 'MCapWt%'] = 0
+                    #         pass
+                    #     numShares.append(saveResults.loc[ticker, 'MCapWt%'])
+                    # screenResults["MCapWt%"] = numShares
                 if not newlyListedOnly and not configManager.showunknowntrends and screenResults is not None and len(screenResults) > 0:
                     screenResults, saveResults = removeUnknowns(screenResults, saveResults)
                     print(colorText.FAIL + f"[+] Configuration to remove unknown cell values resulted into removing all rows!" + colorText.END)
                 if len(strategyFilter) > 0 and saveResults is not None and len(saveResults) > 0:
                     # We'd need to apply additional filters for selected strategy
                     df_screenResults = None
                     cleanedUpSaveResults = PortfolioXRay.cleanupData(saveResults)
@@ -1739,17 +1739,18 @@
                     for col in caption_df.columns:
                         caption_df[col] = caption_df[col].astype(str)
                     caption_results = colorText.miniTabulator().tabulate(
                         caption_df,
                         headers="keys",
                         tablefmt=colorText.No_Pad_GridFormat,
                         maxcolwidths=[None,None,4,3]
-                    ).encode("utf-8").decode(STD_ENCODING).replace("-+-----+-----+-----+","-+-----+----+---+").replace("%  ","% ").replace("=+=====+=====+=====+","=+=====+====+===+").replace("Vol  |","Vol|").replace("x  ","x")
+                    ).encode("utf-8").decode(STD_ENCODING).replace("-K-----S-----C-----R","-K-----S----C---R").replace("%  ","% ").replace("=K=====S=====C=====R","=K=====S====C===R").replace("Vol  |","Vol|").replace("x  ","x")
+                    caption_results = caption_results.replace("-E-----N-----E-----R","-E-----N----E---R").replace("=E=====N=====E=====R","=E=====N====E===R")
                     caption = f"{caption}.Open attached image for more. Samples:<pre>{caption_results}</pre>{elapsed_text}" #<i>Author is <u><b>NOT</b> a SEBI registered financial advisor</u> and MUST NOT be deemed as one.</i>"
-                if not testing and not userPassedArgs.runintradayanalysis:
+                if not testing: # and not userPassedArgs.runintradayanalysis:
                     sendQuickScanResult(
                         menuChoiceHierarchy,
                         user,
                         tabulated_results,
                         markdown_results,
                         caption,
                         pngName,
@@ -1862,16 +1863,16 @@
             #     ltp = saveResults[f"LTP"].replace("", np.nan).replace(np.inf, np.nan).replace(-np.inf, np.nan).astype(float)
             #     pdReturn = round(100*(sum(pdLTP * mktWeight)-sum(ltp * mktWeight))/sum(ltp * mktWeight),1)
             #               #round((sum(saveResults[f"LTP{period}"]) - sum(saveResults['LTP']))*100/sum(saveResults['LTP']),1)
             #     if pdReturn > -500:
             #         summaryReturns = f"{period}-Pd({pdReturn} %), {summaryReturns}"
             saveResults.drop(f"LTP{period}", axis=1, inplace=True, errors="ignore")
             saveResults.drop(f"Growth{period}", axis=1, inplace=True, errors="ignore")
-            saveResults.drop(f"MCapWt%", axis=1, inplace=True, errors="ignore")
-            screenResults.drop(f"MCapWt%", axis=1, inplace=True, errors="ignore")
+            # saveResults.drop(f"MCapWt%", axis=1, inplace=True, errors="ignore")
+            # screenResults.drop(f"MCapWt%", axis=1, inplace=True, errors="ignore")
             if len(dropAdditionalColumns) > 0:
                 for col in dropAdditionalColumns:
                     if col in saveResults.columns:
                         saveResults.drop(col, axis=1, inplace=True, errors="ignore")
         if screenResults is not None:
             screenResults.drop(f"LTP{period}", axis=1, inplace=True, errors="ignore")
             screenResults.drop(f"Growth{period}", axis=1, inplace=True, errors="ignore")
```

### Comparing `pkscreener-0.44.20240416.265/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240416.267/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.265/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240416.267/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.265/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240416.267/pkscreener/pkscreenercli.py`

 * *Files 3% similar despite different names*

```diff
@@ -310,14 +310,23 @@
             df_grouped = optionalFinalOutcome_df.groupby("Stock")
             for stock, df_group in df_grouped:
                 if stock == "PORTFOLIO":
                     if final_df is None:
                         final_df = df_group[["Pattern","LTP","SqrOffLTP","SqrOffDiff","EoDLTP","EoDDiff","%Chng"]]
                     else:
                         final_df = pd.concat([final_df, df_group[["Pattern","LTP","SqrOffLTP","SqrOffDiff","EoDLTP","EoDDiff","%Chng"]]], axis=0)
+            final_df.rename(
+                columns={
+                    "LTP": "Morning Portfolio",
+                    "SqrOffLTP": "SqrOff Portfolio",
+                    "EoDLTP": "EoD Portfolio",
+                    "%Chng": "EoD %Chng",
+                    },
+                    inplace=True,
+                )
             mark_down = colorText.miniTabulator().tabulate(
                                 final_df,
                                 headers="keys",
                                 tablefmt=colorText.No_Pad_GridFormat,
                                 showindex = False
                             ).encode("utf-8").decode(Utility.STD_ENCODING)
             print(mark_down)
```

### Comparing `pkscreener-0.44.20240416.265/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240416.267/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240416.265
+Version: 0.44.20240416.267
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240416.265.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240416.267.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240415.264/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240416.265/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240415.264/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240416.265/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240415.264/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240416.265/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240416.265/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240416.267/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240416.265/setup.py` & `pkscreener-0.44.20240416.267/setup.py`

 * *Files identical despite different names*

