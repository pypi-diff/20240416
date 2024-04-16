# Comparing `tmp/cxzscxiezhifeng1-2.3.tar.gz` & `tmp/cxzscxiezhifeng1-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cxzscxiezhifeng1-2.3.tar", last modified: Tue Apr 16 06:56:10 2024, max compression
+gzip compressed data, was "cxzscxiezhifeng1-2.4.tar", last modified: Tue Apr 16 06:59:04 2024, max compression
```

## Comparing `cxzscxiezhifeng1-2.3.tar` & `cxzscxiezhifeng1-2.4.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 xzf        (501) staff       (20)        0 2024-04-16 06:56:10.059899 cxzscxiezhifeng1-2.3/
--rw-r--r--   0 xzf        (501) staff       (20)      553 2023-08-18 23:51:46.000000 cxzscxiezhifeng1-2.3/LICENSE
--rw-r--r--   0 xzf        (501) staff       (20)     7413 2024-04-16 06:56:10.059719 cxzscxiezhifeng1-2.3/PKG-INFO
--rw-r--r--   0 xzf        (501) staff       (20)     6773 2023-08-18 23:51:46.000000 cxzscxiezhifeng1-2.3/README.md
-drwxr-xr-x   0 xzf        (501) staff       (20)        0 2024-04-16 06:56:10.059537 cxzscxiezhifeng1-2.3/cxzscxiezhifeng1.egg-info/
--rw-r--r--   0 xzf        (501) staff       (20)     7413 2024-04-16 06:56:10.000000 cxzscxiezhifeng1-2.3/cxzscxiezhifeng1.egg-info/PKG-INFO
--rw-r--r--   0 xzf        (501) staff       (20)     1562 2024-04-16 06:56:10.000000 cxzscxiezhifeng1-2.3/cxzscxiezhifeng1.egg-info/SOURCES.txt
--rw-r--r--   0 xzf        (501) staff       (20)        1 2024-04-16 06:56:10.000000 cxzscxiezhifeng1-2.3/cxzscxiezhifeng1.egg-info/dependency_links.txt
--rw-r--r--   0 xzf        (501) staff       (20)        5 2024-04-16 06:56:10.000000 cxzscxiezhifeng1-2.3/cxzscxiezhifeng1.egg-info/top_level.txt
-drwxr-xr-x   0 xzf        (501) staff       (20)        0 2024-04-16 06:56:10.052773 cxzscxiezhifeng1-2.3/czsc/
--rw-r--r--   0 xzf        (501) staff       (20)     2164 2024-04-16 03:19:45.000000 cxzscxiezhifeng1-2.3/czsc/__init__.py
--rw-r--r--   0 xzf        (501) staff       (20)    15397 2024-04-16 03:18:02.000000 cxzscxiezhifeng1-2.3/czsc/analyze.py
--rw-r--r--   0 xzf        (501) staff       (20)    54710 2024-04-16 03:18:03.000000 cxzscxiezhifeng1-2.3/czsc/aphorism.py
--rw-r--r--   0 xzf        (501) staff       (20)      443 2024-04-16 03:18:03.000000 cxzscxiezhifeng1-2.3/czsc/cmd.py
-drwxr-xr-x   0 xzf        (501) staff       (20)        0 2024-04-16 06:56:10.053579 cxzscxiezhifeng1-2.3/czsc/connectors/
--rw-r--r--   0 xzf        (501) staff       (20)      156 2024-04-16 03:18:10.000000 cxzscxiezhifeng1-2.3/czsc/connectors/__init__.py
--rw-r--r--   0 xzf        (501) staff       (20)    29451 2024-04-16 03:18:08.000000 cxzscxiezhifeng1-2.3/czsc/connectors/gm_connector.py
--rw-r--r--   0 xzf        (501) staff       (20)    21725 2024-04-16 03:18:09.000000 cxzscxiezhifeng1-2.3/czsc/connectors/jq_connector.py
--rw-r--r--   0 xzf        (501) staff       (20)    35231 2024-04-16 03:18:09.000000 cxzscxiezhifeng1-2.3/czsc/connectors/qmt_connector.py
--rw-r--r--   0 xzf        (501) staff       (20)     2295 2024-04-16 03:18:10.000000 cxzscxiezhifeng1-2.3/czsc/connectors/research.py
--rw-r--r--   0 xzf        (501) staff       (20)     1067 2024-04-16 03:18:10.000000 cxzscxiezhifeng1-2.3/czsc/connectors/ts_connector.py
-drwxr-xr-x   0 xzf        (501) staff       (20)        0 2024-04-16 06:56:10.054058 cxzscxiezhifeng1-2.3/czsc/data/
--rw-r--r--   0 xzf        (501) staff       (20)     1417 2024-04-16 03:18:18.000000 cxzscxiezhifeng1-2.3/czsc/data/__init__.py
--rw-r--r--   0 xzf        (501) staff       (20)     4241 2024-04-16 03:18:17.000000 cxzscxiezhifeng1-2.3/czsc/data/base.py
--rw-r--r--   0 xzf        (501) staff       (20)     4813 2024-04-16 03:18:17.000000 cxzscxiezhifeng1-2.3/czsc/data/ts.py
--rw-r--r--   0 xzf        (501) staff       (20)    25951 2024-04-16 03:18:17.000000 cxzscxiezhifeng1-2.3/czsc/data/ts_cache.py
--rw-r--r--   0 xzf        (501) staff       (20)      614 2024-04-16 03:18:22.000000 cxzscxiezhifeng1-2.3/czsc/eda.py
--rw-r--r--   0 xzf        (501) staff       (20)      889 2024-04-16 03:18:23.000000 cxzscxiezhifeng1-2.3/czsc/enum.py
--rw-r--r--   0 xzf        (501) staff       (20)     1875 2024-04-16 03:18:23.000000 cxzscxiezhifeng1-2.3/czsc/envs.py
-drwxr-xr-x   0 xzf        (501) staff       (20)        0 2024-04-16 06:56:10.054666 cxzscxiezhifeng1-2.3/czsc/fsa/
--rw-r--r--   0 xzf        (501) staff       (20)     3964 2024-04-16 03:18:27.000000 cxzscxiezhifeng1-2.3/czsc/fsa/__init__.py
--rw-r--r--   0 xzf        (501) staff       (20)     6541 2024-04-16 03:18:25.000000 cxzscxiezhifeng1-2.3/czsc/fsa/base.py
--rw-r--r--   0 xzf        (501) staff       (20)     2472 2024-04-16 03:18:26.000000 cxzscxiezhifeng1-2.3/czsc/fsa/bi_table.py
--rw-r--r--   0 xzf        (501) staff       (20)     5173 2024-04-16 03:18:26.000000 cxzscxiezhifeng1-2.3/czsc/fsa/im.py
--rw-r--r--   0 xzf        (501) staff       (20)    13698 2024-04-16 03:18:26.000000 cxzscxiezhifeng1-2.3/czsc/fsa/spreed_sheets.py
--rw-r--r--   0 xzf        (501) staff       (20)    42520 2024-04-16 03:18:33.000000 cxzscxiezhifeng1-2.3/czsc/objects.py
-drwxr-xr-x   0 xzf        (501) staff       (20)        0 2024-04-16 06:56:10.055369 cxzscxiezhifeng1-2.3/czsc/sensors/
--rw-r--r--   0 xzf        (501) staff       (20)      338 2024-04-16 03:18:38.000000 cxzscxiezhifeng1-2.3/czsc/sensors/__init__.py
--rw-r--r--   0 xzf        (501) staff       (20)     5930 2024-04-16 03:18:36.000000 cxzscxiezhifeng1-2.3/czsc/sensors/cta.py
--rw-r--r--   0 xzf        (501) staff       (20)     6778 2024-04-16 03:18:36.000000 cxzscxiezhifeng1-2.3/czsc/sensors/event.py
--rw-r--r--   0 xzf        (501) staff       (20)    13361 2024-04-16 03:18:37.000000 cxzscxiezhifeng1-2.3/czsc/sensors/feature.py
--rw-r--r--   0 xzf        (501) staff       (20)    11218 2024-04-16 03:18:37.000000 cxzscxiezhifeng1-2.3/czsc/sensors/plates.py
--rw-r--r--   0 xzf        (501) staff       (20)     7219 2024-04-16 03:18:37.000000 cxzscxiezhifeng1-2.3/czsc/sensors/utils.py
-drwxr-xr-x   0 xzf        (501) staff       (20)        0 2024-04-16 06:56:10.056819 cxzscxiezhifeng1-2.3/czsc/signals/
--rw-r--r--   0 xzf        (501) staff       (20)     6292 2024-04-16 03:18:52.000000 cxzscxiezhifeng1-2.3/czsc/signals/__init__.py
--rw-r--r--   0 xzf        (501) staff       (20)    31015 2024-04-16 03:18:46.000000 cxzscxiezhifeng1-2.3/czsc/signals/ang.py
--rw-r--r--   0 xzf        (501) staff       (20)    58450 2024-04-16 03:18:47.000000 cxzscxiezhifeng1-2.3/czsc/signals/bar.py
--rw-r--r--   0 xzf        (501) staff       (20)    10013 2024-04-16 03:18:47.000000 cxzscxiezhifeng1-2.3/czsc/signals/byi.py
--rw-r--r--   0 xzf        (501) staff       (20)     9094 2024-04-16 03:18:47.000000 cxzscxiezhifeng1-2.3/czsc/signals/coo.py
--rw-r--r--   0 xzf        (501) staff       (20)    85142 2024-04-16 03:18:48.000000 cxzscxiezhifeng1-2.3/czsc/signals/cxt.py
--rw-r--r--   0 xzf        (501) staff       (20)    47010 2024-04-16 03:18:49.000000 cxzscxiezhifeng1-2.3/czsc/signals/jcc.py
--rw-r--r--   0 xzf        (501) staff       (20)    17354 2024-04-16 03:18:50.000000 cxzscxiezhifeng1-2.3/czsc/signals/pos.py
--rw-r--r--   0 xzf        (501) staff       (20)   154969 2024-04-16 03:18:50.000000 cxzscxiezhifeng1-2.3/czsc/signals/tas.py
--rw-r--r--   0 xzf        (501) staff       (20)    14562 2024-04-16 03:18:51.000000 cxzscxiezhifeng1-2.3/czsc/signals/vol.py
--rw-r--r--   0 xzf        (501) staff       (20)    45820 2024-04-16 03:18:52.000000 cxzscxiezhifeng1-2.3/czsc/signals/zdy.py
--rw-r--r--   0 xzf        (501) staff       (20)    40079 2024-04-16 03:19:06.000000 cxzscxiezhifeng1-2.3/czsc/strategies.py
-drwxr-xr-x   0 xzf        (501) staff       (20)        0 2024-04-16 06:56:10.057503 cxzscxiezhifeng1-2.3/czsc/traders/
--rw-r--r--   0 xzf        (501) staff       (20)      701 2024-04-16 03:19:10.000000 cxzscxiezhifeng1-2.3/czsc/traders/__init__.py
--rw-r--r--   0 xzf        (501) staff       (20)    20427 2024-04-16 03:19:09.000000 cxzscxiezhifeng1-2.3/czsc/traders/base.py
--rw-r--r--   0 xzf        (501) staff       (20)     7662 2024-04-16 03:19:09.000000 cxzscxiezhifeng1-2.3/czsc/traders/dummy.py
--rw-r--r--   0 xzf        (501) staff       (20)    16315 2024-04-16 03:19:09.000000 cxzscxiezhifeng1-2.3/czsc/traders/performance.py
--rw-r--r--   0 xzf        (501) staff       (20)     4675 2024-04-16 03:19:10.000000 cxzscxiezhifeng1-2.3/czsc/traders/sig_parse.py
--rw-r--r--   0 xzf        (501) staff       (20)    12350 2024-04-16 03:19:10.000000 cxzscxiezhifeng1-2.3/czsc/traders/weight_backtest.py
-drwxr-xr-x   0 xzf        (501) staff       (20)        0 2024-04-16 06:56:10.059378 cxzscxiezhifeng1-2.3/czsc/utils/
--rw-r--r--   0 xzf        (501) staff       (20)     4371 2024-04-16 03:19:29.000000 cxzscxiezhifeng1-2.3/czsc/utils/__init__.py
--rw-r--r--   0 xzf        (501) staff       (20)     7875 2024-04-16 03:19:23.000000 cxzscxiezhifeng1-2.3/czsc/utils/bar_generator.py
--rw-r--r--   0 xzf        (501) staff       (20)      732 2024-04-16 03:19:24.000000 cxzscxiezhifeng1-2.3/czsc/utils/cache.py
--rw-r--r--   0 xzf        (501) staff       (20)     4375 2024-04-16 03:19:24.000000 cxzscxiezhifeng1-2.3/czsc/utils/corr.py
--rw-r--r--   0 xzf        (501) staff       (20)     7877 2024-04-16 03:19:24.000000 cxzscxiezhifeng1-2.3/czsc/utils/cross.py
--rw-r--r--   0 xzf        (501) staff       (20)    18426 2024-04-16 03:19:24.000000 cxzscxiezhifeng1-2.3/czsc/utils/echarts_plot.py
--rw-r--r--   0 xzf        (501) staff       (20)     1286 2024-04-16 03:19:25.000000 cxzscxiezhifeng1-2.3/czsc/utils/io.py
--rw-r--r--   0 xzf        (501) staff       (20)     9423 2024-04-16 03:19:25.000000 cxzscxiezhifeng1-2.3/czsc/utils/oss.py
--rw-r--r--   0 xzf        (501) staff       (20)     9406 2024-04-16 03:19:25.000000 cxzscxiezhifeng1-2.3/czsc/utils/plotly_plot.py
--rw-r--r--   0 xzf        (501) staff       (20)     4351 2024-04-16 03:19:26.000000 cxzscxiezhifeng1-2.3/czsc/utils/plt_plot.py
--rw-r--r--   0 xzf        (501) staff       (20)     2704 2024-04-16 03:19:26.000000 cxzscxiezhifeng1-2.3/czsc/utils/qywx.py
--rw-r--r--   0 xzf        (501) staff       (20)    12209 2024-04-16 03:19:26.000000 cxzscxiezhifeng1-2.3/czsc/utils/sig.py
--rw-r--r--   0 xzf        (501) staff       (20)     9308 2024-04-16 03:19:27.000000 cxzscxiezhifeng1-2.3/czsc/utils/signal_analyzer.py
--rw-r--r--   0 xzf        (501) staff       (20)     8883 2024-04-16 03:19:27.000000 cxzscxiezhifeng1-2.3/czsc/utils/stats.py
--rw-r--r--   0 xzf        (501) staff       (20)     3862 2024-04-16 03:19:28.000000 cxzscxiezhifeng1-2.3/czsc/utils/ta.py
--rw-r--r--   0 xzf        (501) staff       (20)     2125 2024-04-16 03:19:28.000000 cxzscxiezhifeng1-2.3/czsc/utils/ta1.py
--rw-r--r--   0 xzf        (501) staff       (20)     3434 2024-04-16 03:19:28.000000 cxzscxiezhifeng1-2.3/czsc/utils/trade.py
--rw-r--r--   0 xzf        (501) staff       (20)       38 2024-04-16 06:56:10.059935 cxzscxiezhifeng1-2.3/setup.cfg
--rw-r--r--   0 xzf        (501) staff       (20)     1144 2024-04-16 06:56:03.000000 cxzscxiezhifeng1-2.3/setup.py
+drwxr-xr-x   0 xzf        (501) staff       (20)        0 2024-04-16 06:59:04.285859 cxzscxiezhifeng1-2.4/
+-rw-r--r--   0 xzf        (501) staff       (20)      553 2023-08-18 23:51:46.000000 cxzscxiezhifeng1-2.4/LICENSE
+-rw-r--r--   0 xzf        (501) staff       (20)     7413 2024-04-16 06:59:04.285671 cxzscxiezhifeng1-2.4/PKG-INFO
+-rw-r--r--   0 xzf        (501) staff       (20)     6773 2023-08-18 23:51:46.000000 cxzscxiezhifeng1-2.4/README.md
+drwxr-xr-x   0 xzf        (501) staff       (20)        0 2024-04-16 06:59:04.285489 cxzscxiezhifeng1-2.4/cxzscxiezhifeng1.egg-info/
+-rw-r--r--   0 xzf        (501) staff       (20)     7413 2024-04-16 06:59:04.000000 cxzscxiezhifeng1-2.4/cxzscxiezhifeng1.egg-info/PKG-INFO
+-rw-r--r--   0 xzf        (501) staff       (20)     1562 2024-04-16 06:59:04.000000 cxzscxiezhifeng1-2.4/cxzscxiezhifeng1.egg-info/SOURCES.txt
+-rw-r--r--   0 xzf        (501) staff       (20)        1 2024-04-16 06:59:04.000000 cxzscxiezhifeng1-2.4/cxzscxiezhifeng1.egg-info/dependency_links.txt
+-rw-r--r--   0 xzf        (501) staff       (20)        5 2024-04-16 06:59:04.000000 cxzscxiezhifeng1-2.4/cxzscxiezhifeng1.egg-info/top_level.txt
+drwxr-xr-x   0 xzf        (501) staff       (20)        0 2024-04-16 06:59:04.278437 cxzscxiezhifeng1-2.4/czsc/
+-rw-r--r--   0 xzf        (501) staff       (20)     2164 2024-04-16 03:19:45.000000 cxzscxiezhifeng1-2.4/czsc/__init__.py
+-rw-r--r--   0 xzf        (501) staff       (20)    15397 2024-04-16 03:18:02.000000 cxzscxiezhifeng1-2.4/czsc/analyze.py
+-rw-r--r--   0 xzf        (501) staff       (20)    54710 2024-04-16 03:18:03.000000 cxzscxiezhifeng1-2.4/czsc/aphorism.py
+-rw-r--r--   0 xzf        (501) staff       (20)      443 2024-04-16 03:18:03.000000 cxzscxiezhifeng1-2.4/czsc/cmd.py
+drwxr-xr-x   0 xzf        (501) staff       (20)        0 2024-04-16 06:59:04.279184 cxzscxiezhifeng1-2.4/czsc/connectors/
+-rw-r--r--   0 xzf        (501) staff       (20)      156 2024-04-16 03:18:10.000000 cxzscxiezhifeng1-2.4/czsc/connectors/__init__.py
+-rw-r--r--   0 xzf        (501) staff       (20)    29451 2024-04-16 03:18:08.000000 cxzscxiezhifeng1-2.4/czsc/connectors/gm_connector.py
+-rw-r--r--   0 xzf        (501) staff       (20)    21725 2024-04-16 03:18:09.000000 cxzscxiezhifeng1-2.4/czsc/connectors/jq_connector.py
+-rw-r--r--   0 xzf        (501) staff       (20)    35231 2024-04-16 03:18:09.000000 cxzscxiezhifeng1-2.4/czsc/connectors/qmt_connector.py
+-rw-r--r--   0 xzf        (501) staff       (20)     2295 2024-04-16 03:18:10.000000 cxzscxiezhifeng1-2.4/czsc/connectors/research.py
+-rw-r--r--   0 xzf        (501) staff       (20)     1067 2024-04-16 03:18:10.000000 cxzscxiezhifeng1-2.4/czsc/connectors/ts_connector.py
+drwxr-xr-x   0 xzf        (501) staff       (20)        0 2024-04-16 06:59:04.279685 cxzscxiezhifeng1-2.4/czsc/data/
+-rw-r--r--   0 xzf        (501) staff       (20)     1417 2024-04-16 03:18:18.000000 cxzscxiezhifeng1-2.4/czsc/data/__init__.py
+-rw-r--r--   0 xzf        (501) staff       (20)     4241 2024-04-16 03:18:17.000000 cxzscxiezhifeng1-2.4/czsc/data/base.py
+-rw-r--r--   0 xzf        (501) staff       (20)     4813 2024-04-16 03:18:17.000000 cxzscxiezhifeng1-2.4/czsc/data/ts.py
+-rw-r--r--   0 xzf        (501) staff       (20)    25951 2024-04-16 03:18:17.000000 cxzscxiezhifeng1-2.4/czsc/data/ts_cache.py
+-rw-r--r--   0 xzf        (501) staff       (20)      614 2024-04-16 03:18:22.000000 cxzscxiezhifeng1-2.4/czsc/eda.py
+-rw-r--r--   0 xzf        (501) staff       (20)      889 2024-04-16 03:18:23.000000 cxzscxiezhifeng1-2.4/czsc/enum.py
+-rw-r--r--   0 xzf        (501) staff       (20)     1875 2024-04-16 03:18:23.000000 cxzscxiezhifeng1-2.4/czsc/envs.py
+drwxr-xr-x   0 xzf        (501) staff       (20)        0 2024-04-16 06:59:04.280311 cxzscxiezhifeng1-2.4/czsc/fsa/
+-rw-r--r--   0 xzf        (501) staff       (20)     3964 2024-04-16 03:18:27.000000 cxzscxiezhifeng1-2.4/czsc/fsa/__init__.py
+-rw-r--r--   0 xzf        (501) staff       (20)     6541 2024-04-16 03:18:25.000000 cxzscxiezhifeng1-2.4/czsc/fsa/base.py
+-rw-r--r--   0 xzf        (501) staff       (20)     2472 2024-04-16 03:18:26.000000 cxzscxiezhifeng1-2.4/czsc/fsa/bi_table.py
+-rw-r--r--   0 xzf        (501) staff       (20)     5173 2024-04-16 03:18:26.000000 cxzscxiezhifeng1-2.4/czsc/fsa/im.py
+-rw-r--r--   0 xzf        (501) staff       (20)    13698 2024-04-16 03:18:26.000000 cxzscxiezhifeng1-2.4/czsc/fsa/spreed_sheets.py
+-rw-r--r--   0 xzf        (501) staff       (20)    42520 2024-04-16 03:18:33.000000 cxzscxiezhifeng1-2.4/czsc/objects.py
+drwxr-xr-x   0 xzf        (501) staff       (20)        0 2024-04-16 06:59:04.281040 cxzscxiezhifeng1-2.4/czsc/sensors/
+-rw-r--r--   0 xzf        (501) staff       (20)      338 2024-04-16 03:18:38.000000 cxzscxiezhifeng1-2.4/czsc/sensors/__init__.py
+-rw-r--r--   0 xzf        (501) staff       (20)     5930 2024-04-16 03:18:36.000000 cxzscxiezhifeng1-2.4/czsc/sensors/cta.py
+-rw-r--r--   0 xzf        (501) staff       (20)     6778 2024-04-16 03:18:36.000000 cxzscxiezhifeng1-2.4/czsc/sensors/event.py
+-rw-r--r--   0 xzf        (501) staff       (20)    13361 2024-04-16 03:18:37.000000 cxzscxiezhifeng1-2.4/czsc/sensors/feature.py
+-rw-r--r--   0 xzf        (501) staff       (20)    11218 2024-04-16 03:18:37.000000 cxzscxiezhifeng1-2.4/czsc/sensors/plates.py
+-rw-r--r--   0 xzf        (501) staff       (20)     7219 2024-04-16 03:18:37.000000 cxzscxiezhifeng1-2.4/czsc/sensors/utils.py
+drwxr-xr-x   0 xzf        (501) staff       (20)        0 2024-04-16 06:59:04.282594 cxzscxiezhifeng1-2.4/czsc/signals/
+-rw-r--r--   0 xzf        (501) staff       (20)     6292 2024-04-16 03:18:52.000000 cxzscxiezhifeng1-2.4/czsc/signals/__init__.py
+-rw-r--r--   0 xzf        (501) staff       (20)    31015 2024-04-16 03:18:46.000000 cxzscxiezhifeng1-2.4/czsc/signals/ang.py
+-rw-r--r--   0 xzf        (501) staff       (20)    58450 2024-04-16 03:18:47.000000 cxzscxiezhifeng1-2.4/czsc/signals/bar.py
+-rw-r--r--   0 xzf        (501) staff       (20)    10013 2024-04-16 03:18:47.000000 cxzscxiezhifeng1-2.4/czsc/signals/byi.py
+-rw-r--r--   0 xzf        (501) staff       (20)     9094 2024-04-16 03:18:47.000000 cxzscxiezhifeng1-2.4/czsc/signals/coo.py
+-rw-r--r--   0 xzf        (501) staff       (20)    85142 2024-04-16 03:18:48.000000 cxzscxiezhifeng1-2.4/czsc/signals/cxt.py
+-rw-r--r--   0 xzf        (501) staff       (20)    47010 2024-04-16 03:18:49.000000 cxzscxiezhifeng1-2.4/czsc/signals/jcc.py
+-rw-r--r--   0 xzf        (501) staff       (20)    17354 2024-04-16 03:18:50.000000 cxzscxiezhifeng1-2.4/czsc/signals/pos.py
+-rw-r--r--   0 xzf        (501) staff       (20)   154969 2024-04-16 03:18:50.000000 cxzscxiezhifeng1-2.4/czsc/signals/tas.py
+-rw-r--r--   0 xzf        (501) staff       (20)    14562 2024-04-16 03:18:51.000000 cxzscxiezhifeng1-2.4/czsc/signals/vol.py
+-rw-r--r--   0 xzf        (501) staff       (20)    45820 2024-04-16 03:18:52.000000 cxzscxiezhifeng1-2.4/czsc/signals/zdy.py
+-rw-r--r--   0 xzf        (501) staff       (20)    40079 2024-04-16 03:19:06.000000 cxzscxiezhifeng1-2.4/czsc/strategies.py
+drwxr-xr-x   0 xzf        (501) staff       (20)        0 2024-04-16 06:59:04.283303 cxzscxiezhifeng1-2.4/czsc/traders/
+-rw-r--r--   0 xzf        (501) staff       (20)      701 2024-04-16 03:19:10.000000 cxzscxiezhifeng1-2.4/czsc/traders/__init__.py
+-rw-r--r--   0 xzf        (501) staff       (20)    20427 2024-04-16 03:19:09.000000 cxzscxiezhifeng1-2.4/czsc/traders/base.py
+-rw-r--r--   0 xzf        (501) staff       (20)     7662 2024-04-16 03:19:09.000000 cxzscxiezhifeng1-2.4/czsc/traders/dummy.py
+-rw-r--r--   0 xzf        (501) staff       (20)    16315 2024-04-16 03:19:09.000000 cxzscxiezhifeng1-2.4/czsc/traders/performance.py
+-rw-r--r--   0 xzf        (501) staff       (20)     4675 2024-04-16 03:19:10.000000 cxzscxiezhifeng1-2.4/czsc/traders/sig_parse.py
+-rw-r--r--   0 xzf        (501) staff       (20)    12350 2024-04-16 03:19:10.000000 cxzscxiezhifeng1-2.4/czsc/traders/weight_backtest.py
+drwxr-xr-x   0 xzf        (501) staff       (20)        0 2024-04-16 06:59:04.285292 cxzscxiezhifeng1-2.4/czsc/utils/
+-rw-r--r--   0 xzf        (501) staff       (20)     4371 2024-04-16 03:19:29.000000 cxzscxiezhifeng1-2.4/czsc/utils/__init__.py
+-rw-r--r--   0 xzf        (501) staff       (20)     7875 2024-04-16 03:19:23.000000 cxzscxiezhifeng1-2.4/czsc/utils/bar_generator.py
+-rw-r--r--   0 xzf        (501) staff       (20)      732 2024-04-16 03:19:24.000000 cxzscxiezhifeng1-2.4/czsc/utils/cache.py
+-rw-r--r--   0 xzf        (501) staff       (20)     4375 2024-04-16 03:19:24.000000 cxzscxiezhifeng1-2.4/czsc/utils/corr.py
+-rw-r--r--   0 xzf        (501) staff       (20)     7877 2024-04-16 03:19:24.000000 cxzscxiezhifeng1-2.4/czsc/utils/cross.py
+-rw-r--r--   0 xzf        (501) staff       (20)    18426 2024-04-16 03:19:24.000000 cxzscxiezhifeng1-2.4/czsc/utils/echarts_plot.py
+-rw-r--r--   0 xzf        (501) staff       (20)     1286 2024-04-16 03:19:25.000000 cxzscxiezhifeng1-2.4/czsc/utils/io.py
+-rw-r--r--   0 xzf        (501) staff       (20)     9423 2024-04-16 03:19:25.000000 cxzscxiezhifeng1-2.4/czsc/utils/oss.py
+-rw-r--r--   0 xzf        (501) staff       (20)     9406 2024-04-16 03:19:25.000000 cxzscxiezhifeng1-2.4/czsc/utils/plotly_plot.py
+-rw-r--r--   0 xzf        (501) staff       (20)     4351 2024-04-16 03:19:26.000000 cxzscxiezhifeng1-2.4/czsc/utils/plt_plot.py
+-rw-r--r--   0 xzf        (501) staff       (20)     2704 2024-04-16 03:19:26.000000 cxzscxiezhifeng1-2.4/czsc/utils/qywx.py
+-rw-r--r--   0 xzf        (501) staff       (20)    12209 2024-04-16 03:19:26.000000 cxzscxiezhifeng1-2.4/czsc/utils/sig.py
+-rw-r--r--   0 xzf        (501) staff       (20)     9308 2024-04-16 03:19:27.000000 cxzscxiezhifeng1-2.4/czsc/utils/signal_analyzer.py
+-rw-r--r--   0 xzf        (501) staff       (20)     8883 2024-04-16 03:19:27.000000 cxzscxiezhifeng1-2.4/czsc/utils/stats.py
+-rw-r--r--   0 xzf        (501) staff       (20)     3862 2024-04-16 03:19:28.000000 cxzscxiezhifeng1-2.4/czsc/utils/ta.py
+-rw-r--r--   0 xzf        (501) staff       (20)     2125 2024-04-16 03:19:28.000000 cxzscxiezhifeng1-2.4/czsc/utils/ta1.py
+-rw-r--r--   0 xzf        (501) staff       (20)     3434 2024-04-16 03:19:28.000000 cxzscxiezhifeng1-2.4/czsc/utils/trade.py
+-rw-r--r--   0 xzf        (501) staff       (20)       38 2024-04-16 06:59:04.285899 cxzscxiezhifeng1-2.4/setup.cfg
+-rw-r--r--   0 xzf        (501) staff       (20)     1144 2024-04-16 06:58:53.000000 cxzscxiezhifeng1-2.4/setup.py
```

### Comparing `cxzscxiezhifeng1-2.3/LICENSE` & `cxzscxiezhifeng1-2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/PKG-INFO` & `cxzscxiezhifeng1-2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cxzscxiezhifeng1
-Version: 2.3
+Version: 2.4
 Summary: 缠中说禅技术分析工具
 Home-page: 
 Author: xiezhifeng
 Author-email: 
 License: Apache Software License
 Keywords: 技术分析
 Platform: all
```

### Comparing `cxzscxiezhifeng1-2.3/README.md` & `cxzscxiezhifeng1-2.4/README.md`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/cxzscxiezhifeng1.egg-info/PKG-INFO` & `cxzscxiezhifeng1-2.4/cxzscxiezhifeng1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cxzscxiezhifeng1
-Version: 2.3
+Version: 2.4
 Summary: 缠中说禅技术分析工具
 Home-page: 
 Author: xiezhifeng
 Author-email: 
 License: Apache Software License
 Keywords: 技术分析
 Platform: all
```

### Comparing `cxzscxiezhifeng1-2.3/cxzscxiezhifeng1.egg-info/SOURCES.txt` & `cxzscxiezhifeng1-2.4/cxzscxiezhifeng1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/__init__.py` & `cxzscxiezhifeng1-2.4/czsc/__init__.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/analyze.py` & `cxzscxiezhifeng1-2.4/czsc/analyze.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/aphorism.py` & `cxzscxiezhifeng1-2.4/czsc/aphorism.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/connectors/gm_connector.py` & `cxzscxiezhifeng1-2.4/czsc/connectors/gm_connector.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/connectors/jq_connector.py` & `cxzscxiezhifeng1-2.4/czsc/connectors/jq_connector.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/connectors/qmt_connector.py` & `cxzscxiezhifeng1-2.4/czsc/connectors/qmt_connector.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/connectors/research.py` & `cxzscxiezhifeng1-2.4/czsc/connectors/research.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/connectors/ts_connector.py` & `cxzscxiezhifeng1-2.4/czsc/connectors/ts_connector.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/data/__init__.py` & `cxzscxiezhifeng1-2.4/czsc/data/__init__.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/data/base.py` & `cxzscxiezhifeng1-2.4/czsc/data/base.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/data/ts.py` & `cxzscxiezhifeng1-2.4/czsc/data/ts.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/data/ts_cache.py` & `cxzscxiezhifeng1-2.4/czsc/data/ts_cache.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/eda.py` & `cxzscxiezhifeng1-2.4/czsc/eda.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/enum.py` & `cxzscxiezhifeng1-2.4/czsc/enum.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/envs.py` & `cxzscxiezhifeng1-2.4/czsc/envs.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/fsa/__init__.py` & `cxzscxiezhifeng1-2.4/czsc/fsa/__init__.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/fsa/base.py` & `cxzscxiezhifeng1-2.4/czsc/fsa/base.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/fsa/bi_table.py` & `cxzscxiezhifeng1-2.4/czsc/fsa/bi_table.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/fsa/im.py` & `cxzscxiezhifeng1-2.4/czsc/fsa/im.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/fsa/spreed_sheets.py` & `cxzscxiezhifeng1-2.4/czsc/fsa/spreed_sheets.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/objects.py` & `cxzscxiezhifeng1-2.4/czsc/objects.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/sensors/cta.py` & `cxzscxiezhifeng1-2.4/czsc/sensors/cta.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/sensors/event.py` & `cxzscxiezhifeng1-2.4/czsc/sensors/event.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/sensors/feature.py` & `cxzscxiezhifeng1-2.4/czsc/sensors/feature.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/sensors/plates.py` & `cxzscxiezhifeng1-2.4/czsc/sensors/plates.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/sensors/utils.py` & `cxzscxiezhifeng1-2.4/czsc/sensors/utils.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/signals/__init__.py` & `cxzscxiezhifeng1-2.4/czsc/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/signals/ang.py` & `cxzscxiezhifeng1-2.4/czsc/signals/ang.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/signals/bar.py` & `cxzscxiezhifeng1-2.4/czsc/signals/bar.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/signals/byi.py` & `cxzscxiezhifeng1-2.4/czsc/signals/byi.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/signals/coo.py` & `cxzscxiezhifeng1-2.4/czsc/signals/coo.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/signals/cxt.py` & `cxzscxiezhifeng1-2.4/czsc/signals/cxt.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/signals/jcc.py` & `cxzscxiezhifeng1-2.4/czsc/signals/jcc.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/signals/pos.py` & `cxzscxiezhifeng1-2.4/czsc/signals/pos.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/signals/tas.py` & `cxzscxiezhifeng1-2.4/czsc/signals/tas.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/signals/vol.py` & `cxzscxiezhifeng1-2.4/czsc/signals/vol.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/signals/zdy.py` & `cxzscxiezhifeng1-2.4/czsc/signals/zdy.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/strategies.py` & `cxzscxiezhifeng1-2.4/czsc/strategies.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/traders/__init__.py` & `cxzscxiezhifeng1-2.4/czsc/traders/__init__.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/traders/base.py` & `cxzscxiezhifeng1-2.4/czsc/traders/base.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/traders/dummy.py` & `cxzscxiezhifeng1-2.4/czsc/traders/dummy.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/traders/performance.py` & `cxzscxiezhifeng1-2.4/czsc/traders/performance.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/traders/sig_parse.py` & `cxzscxiezhifeng1-2.4/czsc/traders/sig_parse.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/traders/weight_backtest.py` & `cxzscxiezhifeng1-2.4/czsc/traders/weight_backtest.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/utils/__init__.py` & `cxzscxiezhifeng1-2.4/czsc/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/utils/bar_generator.py` & `cxzscxiezhifeng1-2.4/czsc/utils/bar_generator.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/utils/cache.py` & `cxzscxiezhifeng1-2.4/czsc/utils/cache.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/utils/corr.py` & `cxzscxiezhifeng1-2.4/czsc/utils/corr.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/utils/cross.py` & `cxzscxiezhifeng1-2.4/czsc/utils/cross.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/utils/echarts_plot.py` & `cxzscxiezhifeng1-2.4/czsc/utils/echarts_plot.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/utils/io.py` & `cxzscxiezhifeng1-2.4/czsc/utils/io.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/utils/oss.py` & `cxzscxiezhifeng1-2.4/czsc/utils/oss.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/utils/plotly_plot.py` & `cxzscxiezhifeng1-2.4/czsc/utils/plotly_plot.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/utils/plt_plot.py` & `cxzscxiezhifeng1-2.4/czsc/utils/plt_plot.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/utils/qywx.py` & `cxzscxiezhifeng1-2.4/czsc/utils/qywx.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/utils/sig.py` & `cxzscxiezhifeng1-2.4/czsc/utils/sig.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/utils/signal_analyzer.py` & `cxzscxiezhifeng1-2.4/czsc/utils/signal_analyzer.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/utils/stats.py` & `cxzscxiezhifeng1-2.4/czsc/utils/stats.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/utils/ta.py` & `cxzscxiezhifeng1-2.4/czsc/utils/ta.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/utils/ta1.py` & `cxzscxiezhifeng1-2.4/czsc/utils/ta1.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/czsc/utils/trade.py` & `cxzscxiezhifeng1-2.4/czsc/utils/trade.py`

 * *Files identical despite different names*

### Comparing `cxzscxiezhifeng1-2.3/setup.py` & `cxzscxiezhifeng1-2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = f.read()
 
 with open(path.join(here, 'requirements.txt'), encoding='utf-8') as f:
     install_requires = f.read().strip().split('\n')
 
 setup(
     name="cxzscxiezhifeng1",
-    version='2.3',
+    version='2.4',
     author='xiezhifeng',
     author_email='',
     keywords=["技术分析"],
     description="缠中说禅技术分析工具",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="Apache Software License",
```

