# Comparing `tmp/rollercoaster-2.1.1.tar.gz` & `tmp/rollercoaster-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rollercoaster-2.1.1.tar", last modified: Thu Apr  4 23:37:58 2024, max compression
+gzip compressed data, was "rollercoaster-2.1.2.tar", max compression
```

## Comparing `rollercoaster-2.1.1.tar` & `rollercoaster-2.1.2.tar`

### file list

```diff
@@ -1,381 +1,265 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.940750 rollercoaster-2.1.1/
--rw-r--r--   0 root         (0) root         (0)     3309 2024-04-04 23:37:58.940750 rollercoaster-2.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2130 2024-04-04 23:36:36.000000 rollercoaster-2.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2102 2024-04-04 23:37:49.000000 rollercoaster-2.1.1/readme.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 23:37:58.940750 rollercoaster-2.1.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.872750 rollercoaster-2.1.1/venues/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.872750 rollercoaster-2.1.1/venues/stages/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.888750 rollercoaster-2.1.1/venues/stages/rollercoaster/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.888750 rollercoaster-2.1.1/venues/stages/rollercoaster/___itinerary/
--rw-r--r--   0 root         (0) root         (0)      245 2024-03-17 02:25:28.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/___itinerary/itinerary.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.892750 rollercoaster-2.1.1/venues/stages/rollercoaster/___itinerary/sporatic/
--rw-rw-r--   0 root         (0) root         (0)      381 2024-03-31 19:05:52.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/___itinerary/sporatic/itinerary.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.872750 rollercoaster-2.1.1/venues/stages/rollercoaster/__data_nodes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.892750 rollercoaster-2.1.1/venues/stages/rollercoaster/__data_nodes/mongo/
--rw-rw-r--   0 root         (0) root         (0)      405 2024-04-04 18:34:18.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/__data_nodes/mongo/mongo.S.HTML
--rw-r--r--   0 root         (0) root         (0)       45 2024-04-04 18:35:08.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.872750 rollercoaster-2.1.1/venues/stages/rollercoaster/_interfaces/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.892750 rollercoaster-2.1.1/venues/stages/rollercoaster/_interfaces/clique/
--rw-r--r--   0 root         (0) root         (0)     1862 2024-04-04 23:34:28.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/_interfaces/clique/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.892750 rollercoaster-2.1.1/venues/stages/rollercoaster/_interfaces/clique/group/
--rw-r--r--   0 root         (0) root         (0)      294 2023-12-01 19:53:30.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/_interfaces/clique/group/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.892750 rollercoaster-2.1.1/venues/stages/rollercoaster/_interfaces/sanic_trails/
--rw-rw-r--   0 root         (0) root         (0)       53 2024-03-31 19:15:22.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/_interfaces/sanic_trails/strails.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.892750 rollercoaster-2.1.1/venues/stages/rollercoaster/_status/
--rw-r--r--   0 root         (0) root         (0)     1163 2024-04-04 23:37:06.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/_status/insurance.proc.py
--rw-r--r--   0 root         (0) root         (0)     1310 2024-04-04 23:37:28.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/_status/insurance_clouds.proc.py
--rw-rw-r--   0 root         (0) root         (0)      114 2024-03-17 06:14:54.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/_status/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.892750 rollercoaster-2.1.1/venues/stages/rollercoaster/autopilot/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.872750 rollercoaster-2.1.1/venues/stages/rollercoaster/autopilot/bt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.892750 rollercoaster-2.1.1/venues/stages/rollercoaster/autopilot/bt/strategies/
--rw-r--r--   0 root         (0) root         (0)     2589 2023-11-14 05:42:13.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/autopilot/bt/strategies/example_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.892750 rollercoaster-2.1.1/venues/stages/rollercoaster/autopilot/lumi/
--rw-r--r--   0 root         (0) root         (0)      121 2023-11-28 03:26:29.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/autopilot/lumi/lumi.s.HTML
--rw-r--r--   0 root         (0) root         (0)       76 2023-12-19 03:57:24.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/autopilot/priorities.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.892750 rollercoaster-2.1.1/venues/stages/rollercoaster/autopilot/rover_1/
--rw-r--r--   0 root         (0) root         (0)      100 2023-12-19 04:49:40.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/autopilot/rover_1/rover_1.s.HTML
--rw-r--r--   0 root         (0) root         (0)      732 2024-03-17 04:45:46.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/autopilot/rovers.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.892750 rollercoaster-2.1.1/venues/stages/rollercoaster/charts/
--rw-r--r--   0 root         (0) root         (0)      129 2024-01-26 16:01:45.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/charts/charts.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.892750 rollercoaster-2.1.1/venues/stages/rollercoaster/charts/plotly/
--rw-r--r--   0 root         (0) root         (0)      821 2024-03-17 23:24:26.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/charts/plotly/plotly.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.896750 rollercoaster-2.1.1/venues/stages/rollercoaster/climate/
--rw-r--r--   0 root         (0) root         (0)      661 2024-03-31 20:40:53.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/climate/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.896750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.896750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/AV/
--rw-r--r--   0 root         (0) root         (0)      170 2024-04-04 19:34:53.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/AV/AV.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.896750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Alpaca/
--rw-r--r--   0 root         (0) root         (0)      276 2024-03-17 21:13:24.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Alpaca/Alpaca.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.896750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Alpaca/crypto/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.896750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Alpaca/crypto/_status/
--rw-r--r--   0 root         (0) root         (0)      764 2024-04-04 18:30:31.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Alpaca/crypto/_status/API_status_1.py
--rw-rw-r--   0 root         (0) root         (0)      448 2024-04-04 18:32:49.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Alpaca/crypto/crypto.S.HTML
--rw-r--r--   0 root         (0) root         (0)      980 2024-03-17 20:48:31.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Alpaca/crypto/retrieve.py
--rw-r--r--   0 root         (0) root         (0)     1764 2024-04-04 18:31:47.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Alpaca/crypto/structure_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.896750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Alpaca/options/
--rw-rw-r--   0 root         (0) root         (0)       83 2024-04-04 20:04:06.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Alpaca/options/options.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.896750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Alpaca/shares/
--rw-rw-r--   0 root         (0) root         (0)      390 2024-03-22 18:49:35.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Alpaca/shares/retrieve_one.py
--rw-rw-r--   0 root         (0) root         (0)      982 2024-03-22 18:48:12.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Alpaca/shares/retrieve_spans.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.896750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Bybit/
--rw-rw-r--   0 root         (0) root         (0)      107 2024-03-17 18:08:13.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Bybit/Bybit.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.896750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/CCXT/
--rw-r--r--   0 root         (0) root         (0)      174 2024-03-18 17:15:52.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/CCXT/CCXT.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.896750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/CCXT/OHLCV/
--rw-r--r--   0 root         (0) root         (0)     1039 2024-02-28 18:15:51.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/CCXT/OHLCV/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.900750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/CCXT/OHLCV/candles/
--rw-r--r--   0 root         (0) root         (0)     1594 2024-02-28 18:15:51.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/CCXT/OHLCV/candles/__init__.py
--rw-r--r--   0 root         (0) root         (0)      565 2024-01-03 02:25:01.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/CCXT/OHLCV/candles/candles.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.900750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/CCXT/OHLCV/candles_v1/
--rw-r--r--   0 root         (0) root         (0)     2513 2024-02-28 18:15:51.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/CCXT/OHLCV/candles_v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      565 2024-01-03 02:25:01.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/CCXT/OHLCV/candles_v1/candles.s.HTML
--rw-r--r--   0 root         (0) root         (0)        3 2023-12-28 22:53:18.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/CCXT/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.900750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/CCXT/coinbase/
--rw-r--r--   0 root         (0) root         (0)       62 2023-12-28 22:54:25.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/CCXT/coinbase/coinbase.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.900750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/CCXT/symbols/
--rw-r--r--   0 root         (0) root         (0)      362 2024-02-28 18:15:51.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/CCXT/symbols/array.py
--rw-rw-r--   0 root         (0) root         (0)      284 2024-03-31 19:49:32.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Clouds Crypto.S.HTML
--rw-rw-r--   0 root         (0) root         (0)     1008 2024-03-31 19:49:32.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Clouds Shares.S.HTML
--rw-r--r--   0 root         (0) root         (0)      597 2024-03-31 19:49:32.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Clouds.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.900750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Coinbase/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.900750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Coinbase/API/
--rw-r--r--   0 root         (0) root         (0)     2726 2024-02-28 18:15:51.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Coinbase/API/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.900750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Coinbase/API/accounts/
--rw-r--r--   0 root         (0) root         (0)      717 2024-02-28 18:15:51.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Coinbase/API/accounts/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2042 2024-02-28 18:15:51.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Coinbase/API/build_JWT.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.900750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Coinbase/API/orders/
--rw-r--r--   0 root         (0) root         (0)     1260 2024-02-28 18:15:51.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Coinbase/API/orders/order_IDs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.900750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Coinbase/API/products/
--rw-r--r--   0 root         (0) root         (0)     3281 2024-02-28 18:15:51.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Coinbase/API/products/candles.py
--rw-r--r--   0 root         (0) root         (0)      978 2024-02-28 18:15:51.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Coinbase/API/products/catalogue.py
--rw-r--r--   0 root         (0) root         (0)      699 2024-02-28 18:15:51.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Coinbase/Coinbase.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.900750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Coinbase/orders/
--rw-r--r--   0 root         (0) root         (0)     1543 2024-02-28 18:15:51.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Coinbase/orders/place.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.900750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/DOGE/
--rw-r--r--   0 root         (0) root         (0)      614 2023-11-25 04:03:55.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/DOGE/doge.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.900750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Finnhub/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-17 22:41:32.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Finnhub/Finnhub.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.900750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/LedgerX/
--rw-r--r--   0 root         (0) root         (0)      193 2023-11-25 19:05:12.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/LedgerX/LedgerX.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.904750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/MQL5/
--rw-r--r--   0 root         (0) root         (0)       10 2023-12-12 05:12:16.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/MQL5/MQL5.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.904750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Robinhood/
--rw-r--r--   0 root         (0) root         (0)      226 2023-11-20 05:36:28.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Robinhood/Robinhood.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.904750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Tiingo/
--rw-rw-r--   0 root         (0) root         (0)       80 2024-03-17 22:16:54.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Tiingo/Tiingo.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.904750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Tradier/
--rw-r--r--   0 root         (0) root         (0)      129 2024-03-31 18:42:05.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Tradier/Tradier.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.904750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Tradier/_status/
--rw-r--r--   0 root         (0) root         (0)      534 2024-04-04 18:44:17.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Tradier/_status/API_status_combine_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.876751 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Tradier/procedures/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.904750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Tradier/procedures/exchanges/
--rw-rw-r--   0 root         (0) root         (0)       36 2024-04-04 19:14:12.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Tradier/procedures/exchanges/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      122 2024-04-04 19:13:46.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Tradier/procedures/exchanges/exchanges.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.904750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Tradier/procedures/options/
--rw-r--r--   0 root         (0) root         (0)     1351 2024-04-04 19:00:55.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Tradier/procedures/options/combine.py
--rw-r--r--   0 root         (0) root         (0)      212 2023-10-19 20:16:35.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Tradier/uo_tradier_api.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.876751 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Tradier/v1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.876751 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Tradier/v1/markets/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.904750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Tradier/v1/markets/lookup/
--rw-rw-r--   0 root         (0) root         (0)     1134 2024-04-04 19:45:42.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Tradier/v1/markets/lookup/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.876751 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Tradier/v1/markets/options/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.904750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Tradier/v1/markets/options/chains/
--rw-r--r--   0 root         (0) root         (0)     1234 2024-04-04 19:24:22.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Tradier/v1/markets/options/chains/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1769 2024-04-04 20:05:04.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Tradier/v1/markets/options/chains/parse_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.904750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Tradier/v1/markets/options/expirations/
--rw-r--r--   0 root         (0) root         (0)      634 2024-02-28 18:15:51.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Tradier/v1/markets/options/expirations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.904750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/TradingView/
--rw-r--r--   0 root         (0) root         (0)      216 2024-03-18 04:26:59.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/TradingView/TV.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.904750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/TradingView/sensors/
--rw-r--r--   0 root         (0) root         (0)      300 2023-12-12 05:03:24.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/TradingView/sensors/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      237 2024-03-22 19:42:45.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/TradingView/sensors/sensors.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.880751 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/TradingView/treasure/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.904750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/TradingView/treasure/indicators/
--rw-rw-r--   0 root         (0) root         (0)      163 2024-03-17 05:34:46.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/TradingView/treasure/indicators/indicators.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.908750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals/
--rw-rw-r--   0 root         (0) root         (0)     3836 2024-03-24 04:00:45.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.908750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals_v2/
--rw-rw-r--   0 root         (0) root         (0)     1514 2024-03-31 20:03:17.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals_v2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.908750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals_v2/rooms/
--rw-rw-r--   0 root         (0) root         (0)      813 2024-03-22 19:47:25.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals_v2/rooms/print_symbols_table.py
--rw-rw-r--   0 root         (0) root         (0)     1829 2024-03-22 19:46:48.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals_v2/rooms/scan_symbol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.880751 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/USA/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.880751 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/USA/IRS/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.908750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/USA/IRS/IRA/
--rw-rw-r--   0 root         (0) root         (0)      495 2024-03-28 00:15:40.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/USA/IRS/IRA/IRA.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.880751 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/USA/IRS/taxes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.908750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/USA/IRS/taxes/income/
--rw-rw-r--   0 root         (0) root         (0)      410 2024-03-27 18:27:21.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/USA/IRS/taxes/income/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.908750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/USA/SEC/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.908750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/USA/SEC/6K/
--rw-r--r--   0 root         (0) root         (0)       60 2023-11-10 17:23:06.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/USA/SEC/6K/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.908750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/USA/SEC/balance_sheets/
--rw-r--r--   0 root         (0) root         (0)      496 2023-11-10 17:40:32.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/USA/SEC/balance_sheets/__init__.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-11-10 17:15:04.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/USA/SEC/balance_sheets/balance_sheets.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.908750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/USA/SEC/balance_sheets/equity/
--rw-r--r--   0 root         (0) root         (0)      198 2023-11-10 17:28:03.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/USA/SEC/balance_sheets/equity/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.908750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/USA/SEC/income/
--rw-r--r--   0 root         (0) root         (0)      420 2023-11-10 17:53:32.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/USA/SEC/income/__init__.py
--rw-r--r--   0 root         (0) root         (0)       51 2023-11-10 17:34:28.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/USA/SEC/income/income.s.HTML
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-09 20:40:55.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/USA/SEC/statements.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.908750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Yahoo/
--rw-r--r--   0 root         (0) root         (0)      212 2023-11-14 04:12:06.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Yahoo/Yahoo.s.HTML
--rw-r--r--   0 root         (0) root         (0)     1824 2024-03-18 19:45:43.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Yahoo/retrieve.py
--rw-rw-r--   0 root         (0) root         (0)      934 2024-03-22 19:39:27.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Yahoo/retrieve_change.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.908750 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/twelve_data/
--rw-r--r--   0 root         (0) root         (0)       32 2023-11-14 05:19:00.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/twelve_data/twelve_data.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.912750 rollercoaster-2.1.1/venues/stages/rollercoaster/gadgets/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.912750 rollercoaster-2.1.1/venues/stages/rollercoaster/gadgets/clock/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.912750 rollercoaster-2.1.1/venues/stages/rollercoaster/gadgets/clock/UTC/
--rw-r--r--   0 root         (0) root         (0)      446 2024-02-28 18:15:51.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/gadgets/clock/UTC/ISO.py
--rw-r--r--   0 root         (0) root         (0)      984 2024-02-28 18:15:51.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/gadgets/clock/UTC/greatness_1.py
--rw-r--r--   0 root         (0) root         (0)      233 2023-12-28 21:05:42.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/gadgets/clock/clock.s.HTML
--rw-r--r--   0 root         (0) root         (0)      620 2023-11-09 20:46:40.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/gadgets/format_percentage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.880751 rollercoaster-2.1.1/venues/stages/rollercoaster/gadgets/math/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.912750 rollercoaster-2.1.1/venues/stages/rollercoaster/gadgets/math/slope/
--rw-r--r--   0 root         (0) root         (0)      151 2023-11-23 05:19:27.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/gadgets/math/slope/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.912750 rollercoaster-2.1.1/venues/stages/rollercoaster/gadgets/pandas/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.912750 rollercoaster-2.1.1/venues/stages/rollercoaster/gadgets/pandas/DF/
--rw-r--r--   0 root         (0) root         (0)       79 2024-01-10 05:54:37.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/gadgets/pandas/DF/DF.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.912750 rollercoaster-2.1.1/venues/stages/rollercoaster/gadgets/pandas/DF/_status/
--rw-r--r--   0 root         (0) root         (0)      519 2024-02-28 18:15:51.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/gadgets/pandas/DF/_status/status_from_1.py
--rw-r--r--   0 root         (0) root         (0)      252 2024-02-28 18:15:51.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/gadgets/pandas/DF/from_list.py
--rw-r--r--   0 root         (0) root         (0)      326 2024-03-17 21:21:47.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/gadgets/pandas/DF/to_list.py
--rw-r--r--   0 root         (0) root         (0)      690 2024-01-13 06:12:46.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/gadgets/pandas/pandas.s.HTML
--rw-r--r--   0 root         (0) root         (0)      402 2024-02-28 18:15:51.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/gadgets/ratio.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.912750 rollercoaster-2.1.1/venues/stages/rollercoaster/gadgets/summation/
--rw-r--r--   0 root         (0) root         (0)      457 2024-02-28 18:15:51.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/gadgets/summation/__init__.py
--rw-r--r--   0 root         (0) root         (0)      377 2024-02-28 18:15:51.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/gadgets/summation/status_1.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-11 02:12:51.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/gadgets/tools.s.HTML
--rw-r--r--   0 root         (0) root         (0)      760 2024-03-31 18:37:48.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/home.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.916750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/
--rw-rw-r--   0 root         (0) root         (0)      457 2024-03-24 04:04:16.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/rides.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.916750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.916750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/ATR/
--rw-r--r--   0 root         (0) root         (0)      489 2023-12-31 05:03:05.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/ATR/ATR.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.916750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/ATR/ChatGPT_ATR_1/
--rw-r--r--   0 root         (0) root         (0)     2944 2024-03-18 04:08:14.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/ATR/ChatGPT_ATR_1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1591 2024-03-18 04:08:14.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/ATR/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.916750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/ATR/_status/
--rw-r--r--   0 root         (0) root         (0)     1242 2024-03-18 04:08:14.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/ATR/_status/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.916750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/Andean_Oscillator/
--rw-r--r--   0 root         (0) root         (0)      134 2023-12-01 02:49:14.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/Andean_Oscillator/Andean.r.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.916750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/EMA/
--rw-r--r--   0 root         (0) root         (0)      273 2023-12-31 06:36:06.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/EMA/EMA.s.HTML
--rw-r--r--   0 root         (0) root         (0)       82 2023-11-14 05:05:08.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/EMA/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.916750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/MA/
--rw-r--r--   0 root         (0) root         (0)       72 2023-12-03 22:10:44.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/MA/MA.r.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.916750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/MACD/
--rw-r--r--   0 root         (0) root         (0)       91 2023-12-12 04:16:31.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/MACD/MACD.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.920750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/QQE/
--rw-r--r--   0 root         (0) root         (0)       48 2023-12-02 00:37:47.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/QQE/QQE.r.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.920750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/RSI/
--rw-r--r--   0 root         (0) root         (0)      201 2023-12-03 02:58:48.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/RSI/RSI.r.HTML
--rw-r--r--   0 root         (0) root         (0)      782 2024-03-18 04:08:14.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/RSI/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.920750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/SMA/
--rw-r--r--   0 root         (0) root         (0)      250 2024-01-02 06:36:59.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/SMA/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.920750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/TR/
--rw-r--r--   0 root         (0) root         (0)      397 2024-01-02 03:23:31.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/TR/TR.s.HTML
--rw-r--r--   0 root         (0) root         (0)     1628 2024-03-18 04:08:14.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/TR/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.920750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/TR/_status/
--rw-r--r--   0 root         (0) root         (0)      523 2024-03-18 04:08:14.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/TR/_status/status_1.py
--rw-r--r--   0 root         (0) root         (0)      792 2024-03-18 04:08:15.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/TR/_status/status_2.py
--rw-r--r--   0 root         (0) root         (0)      254 2023-11-29 18:25:15.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/TV.r.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.920750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/VWAP/
--rw-r--r--   0 root         (0) root         (0)       46 2023-11-21 16:46:45.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/VWAP/VWAP.r.HTML
--rw-r--r--   0 root         (0) root         (0)      593 2024-03-18 04:08:15.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/VWAP/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.920750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/VWMA/
--rw-r--r--   0 root         (0) root         (0)       47 2023-11-21 16:46:17.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/VWMA/VWMA.r.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.920750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/bolinger_bands/
--rw-r--r--   0 root         (0) root         (0)       24 2023-11-14 04:28:20.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/bolinger_bands/bolinger_bands.r.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.920750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/chandlier_exit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-30 18:13:51.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/chandlier_exit/chandelier exit.r.HTML
--rw-r--r--   0 root         (0) root         (0)      546 2024-02-28 18:15:52.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/indicators.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.920750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/pivot_point/
--rw-r--r--   0 root         (0) root         (0)     1266 2024-01-02 03:23:31.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/pivot_point/pivot_point.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.924750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/relative_volume/
--rw-r--r--   0 root         (0) root         (0)       28 2023-11-21 16:43:07.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/relative_volume/relative volume.r.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.924750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/supertrend/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.924750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/supertrend/ST_1_ChatGPT/
--rw-r--r--   0 root         (0) root         (0)     2832 2024-03-18 04:08:14.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/supertrend/ST_1_ChatGPT/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1098 2024-03-18 04:08:14.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/supertrend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.924750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/supertrend/_status/
--rw-r--r--   0 root         (0) root         (0)     1243 2024-03-18 04:08:14.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/supertrend/_status/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.924750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/supertrend/pandas_ta/
--rw-r--r--   0 root         (0) root         (0)      358 2024-01-06 00:03:10.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/supertrend/pandas_ta/__init__.py
--rw-r--r--   0 root         (0) root         (0)      225 2023-12-03 02:59:17.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/supertrend/supertrend.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.924750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/supertrend2/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-02 03:30:08.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/supertrend2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.884750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.924750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_2/AAS/
--rw-r--r--   0 root         (0) root         (0)     1215 2024-03-18 04:08:15.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_2/AAS/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.924750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_2/AAS/_status/
--rw-r--r--   0 root         (0) root         (0)     1230 2024-03-18 04:08:15.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_2/AAS/_status/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.924750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_2/AS/
--rw-r--r--   0 root         (0) root         (0)      334 2024-01-06 07:25:23.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_2/AS/AS.s.HTML
--rw-r--r--   0 root         (0) root         (0)     1544 2024-03-18 04:08:15.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_2/AS/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.924750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_2/AS/_status/
--rw-r--r--   0 root         (0) root         (0)      511 2024-03-18 04:08:15.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_2/AS/_status/status_1.py
--rw-r--r--   0 root         (0) root         (0)      783 2024-03-18 04:08:15.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_2/AS/_status/status_2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.924750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_2/pecdency/
--rw-r--r--   0 root         (0) root         (0)     1093 2024-01-06 07:15:37.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_2/pecdency/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1350 2024-03-18 04:08:15.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_2/pecdency/__init__v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.884750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.924750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/ST/
--rw-r--r--   0 root         (0) root         (0)     4116 2024-03-18 04:08:15.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/ST/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.924750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/VDA/
--rw-r--r--   0 root         (0) root         (0)      433 2024-03-18 04:08:15.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/VDA/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.924750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/VSA/
--rw-r--r--   0 root         (0) root         (0)      567 2024-03-18 04:08:15.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/VSA/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.924750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/physical_span/
--rw-r--r--   0 root         (0) root         (0)      334 2024-01-09 01:54:38.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/physical_span/AS.s.HTML
--rw-r--r--   0 root         (0) root         (0)     1557 2024-03-18 04:08:15.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/physical_span/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.928750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/physical_span/_status/
--rw-r--r--   0 root         (0) root         (0)      522 2024-03-18 04:08:15.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/physical_span/_status/status_1.py
--rw-r--r--   0 root         (0) root         (0)      790 2024-03-18 04:08:15.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/physical_span/_status/status_2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.928750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/physical_span_average/
--rw-r--r--   0 root         (0) root         (0)     1183 2024-03-18 04:08:15.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/physical_span_average/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.928750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/physical_span_average/_status/
--rw-r--r--   0 root         (0) root         (0)     1248 2024-03-18 04:08:15.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/physical_span_average/_status/status_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.928750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/physical_span_reversals/
--rw-r--r--   0 root         (0) root         (0)     3688 2024-03-18 04:08:15.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/physical_span_reversals/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.928750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/physical_span_roads_v1/
--rw-r--r--   0 root         (0) root         (0)     3586 2024-03-18 04:08:15.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/physical_span_roads_v1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.928750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/super_hero_trend/
--rw-r--r--   0 root         (0) root         (0)     3862 2024-03-18 04:08:15.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/super_hero_trend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.928750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/super_hero_trend/win_rates/
--rw-r--r--   0 root         (0) root         (0)     1759 2024-03-18 04:08:15.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/super_hero_trend/win_rates/shares_trading.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.928750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/supertrend/
--rw-r--r--   0 root         (0) root         (0)      961 2024-03-18 04:08:15.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/supertrend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.884750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_4/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.928750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_4/AO/
--rw-r--r--   0 root         (0) root         (0)     1825 2024-03-18 04:08:15.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_4/AO/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.928750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_4/superb/
--rw-r--r--   0 root         (0) root         (0)     3926 2024-03-18 04:08:15.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_4/superb/__init__.py
--rw-r--r--   0 root         (0) root         (0)       13 2024-02-01 15:34:15.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_4/superb/superb.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.928750 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_4/superb/win_rates/
--rw-r--r--   0 root         (0) root         (0)     1786 2024-03-18 04:08:15.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_4/superb/win_rates/shares_trading.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.928750 rollercoaster-2.1.1/venues/stages/rollercoaster/scans/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.928750 rollercoaster-2.1.1/venues/stages/rollercoaster/scans/_clique/
--rw-rw-r--   0 root         (0) root         (0)     4000 2024-04-04 17:03:41.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/scans/_clique/ETF.py
--rw-rw-r--   0 root         (0) root         (0)        2 2024-04-04 18:06:03.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/scans/_clique/REIT.py
--rw-rw-r--   0 root         (0) root         (0)     2162 2024-04-04 18:22:34.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/scans/_clique/TV.py
--rw-rw-r--   0 root         (0) root         (0)     1411 2024-04-04 17:36:52.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/scans/_clique/currency.py
--rw-rw-r--   0 root         (0) root         (0)       42 2024-04-04 18:06:43.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/scans/_clique/penny_stocks.py
--rw-rw-r--   0 root         (0) root         (0)      415 2024-04-04 18:22:24.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/scans/clique.py
--rw-rw-r--   0 root         (0) root         (0)      122 2024-03-31 19:49:32.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/scans/screeners.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.928750 rollercoaster-2.1.1/venues/stages/rollercoaster/scans/symbol/
--rw-rw-r--   0 root         (0) root         (0)      119 2024-03-31 19:49:32.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/scans/symbol/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      775 2024-03-28 00:19:55.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/scans/symbol/symbols.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.932750 rollercoaster-2.1.1/venues/stages/rollercoaster/stats/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.932750 rollercoaster-2.1.1/venues/stages/rollercoaster/stats/aggregate_PC_ratio/
--rw-r--r--   0 root         (0) root         (0)     5120 2024-04-04 18:12:45.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/stats/aggregate_PC_ratio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1958 2024-03-31 19:02:25.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/stats/aggregate_PC_ratio/squeeze pc ratios.r.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.932750 rollercoaster-2.1.1/venues/stages/rollercoaster/stats/aggregate_PC_ratio/status/
--rw-r--r--   0 root         (0) root         (0)      593 2024-02-28 18:15:51.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/stats/aggregate_PC_ratio/status/status_1.py
--rw-r--r--   0 root         (0) root         (0)     1860 2024-02-28 18:15:52.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/stats/aggregate_PC_ratio/status/status_2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.932750 rollercoaster-2.1.1/venues/stages/rollercoaster/stats/aggregate_break_even/
--rw-r--r--   0 root         (0) root         (0)     2905 2024-03-31 18:52:09.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/stats/aggregate_break_even/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.932750 rollercoaster-2.1.1/venues/stages/rollercoaster/stats/aggregate_break_even/_status/
--rw-r--r--   0 root         (0) root         (0)     1508 2024-02-28 18:15:51.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/stats/aggregate_break_even/_status/status_1.py
--rw-r--r--   0 root         (0) root         (0)      794 2024-02-28 18:15:51.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/stats/aggregate_break_even/_status/status_2.py
--rw-r--r--   0 root         (0) root         (0)     1021 2024-03-31 18:59:30.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/stats/aggregate_break_even/aggregate break even.s.HTML
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-31 19:07:37.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/stats/aggregate_break_even/clique.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.932750 rollercoaster-2.1.1/venues/stages/rollercoaster/stats/aggregate_break_even/show/
--rw-r--r--   0 root         (0) root         (0)      892 2024-02-28 18:15:51.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/stats/aggregate_break_even/show/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.932750 rollercoaster-2.1.1/venues/stages/rollercoaster/stats/aggregate_multiplier/
--rw-r--r--   0 root         (0) root         (0)     1599 2024-03-31 18:39:18.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/stats/aggregate_multiplier/aggregate_multipliers.r.HTML
--rw-rw-r--   0 root         (0) root         (0)      297 2024-03-31 19:16:52.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/stats/clique.py
--rw-r--r--   0 root         (0) root         (0)      520 2024-03-24 04:43:24.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/stats/stats.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.932750 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.932750 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/commodities/
--rw-r--r--   0 root         (0) root         (0)      911 2024-03-17 21:11:40.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/commodities/commodities.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.932750 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/forex/
--rw-r--r--   0 root         (0) root         (0)       29 2023-11-21 17:46:09.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/forex/forex.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.932750 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/futures/
--rw-r--r--   0 root         (0) root         (0)       75 2024-01-30 00:33:10.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/futures/futures.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.936750 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/options/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.936750 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/options/movement_calculator/
--rw-r--r--   0 root         (0) root         (0)     1565 2024-02-28 18:15:52.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/options/movement_calculator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1167 2023-11-23 05:20:06.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/options/movement_calculator/slope.s.HTML
--rw-r--r--   0 root         (0) root         (0)      301 2023-11-23 04:39:41.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/options/options.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.888750 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/options/shapes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.936750 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/options/shapes/shape_1/
--rw-r--r--   0 root         (0) root         (0)     1498 2024-02-28 18:15:52.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/options/shapes/shape_1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      489 2023-11-21 17:09:02.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/options/shapes/shape_1/shape_1.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.936750 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/real_estate/
--rw-r--r--   0 root         (0) root         (0)       84 2023-11-29 18:30:38.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/real_estate/real_estate.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.936750 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/shares/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.936750 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/shares/ETF/
--rw-r--r--   0 root         (0) root         (0)     1190 2024-03-31 19:49:32.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/shares/ETF/ETF.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.936750 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/shares/ETF/comprehensive/
--rw-r--r--   0 root         (0) root         (0)      114 2023-11-15 06:29:25.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/shares/ETF/comprehensive/comprehensive.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.936750 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/shares/ETF/sectors/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.940750 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/shares/ETF/sectors/airlines/
--rw-r--r--   0 root         (0) root         (0)       42 2023-11-15 06:37:06.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/shares/ETF/sectors/airlines/airlines.r.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.940750 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/shares/ETF/sectors/electronics/
--rw-r--r--   0 root         (0) root         (0)       45 2023-11-15 06:38:49.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/shares/ETF/sectors/electronics/semiconductors.r.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.940750 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/shares/ETF/sectors/farming/
--rw-r--r--   0 root         (0) root         (0)       81 2023-11-15 06:34:55.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/shares/ETF/sectors/farming/farming.r.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.940750 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/shares/ETF/sectors/real estate/
--rw-r--r--   0 root         (0) root         (0)       84 2023-11-15 06:37:33.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/shares/ETF/sectors/real estate/real estate.r.HTML
--rw-rw-r--   0 root         (0) root         (0)      157 2024-03-17 04:50:30.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/shares/ETF/sectors/sectors.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.940750 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/shares/ETF/sectors/vehicles/
--rw-r--r--   0 root         (0) root         (0)       14 2023-11-15 06:36:56.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/shares/ETF/sectors/vehicles/vehicles.r.HTML
--rw-rw-r--   0 root         (0) root         (0)        7 2024-03-24 04:01:12.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/shares/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.940750 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/shares/companies/
--rw-r--r--   0 root         (0) root         (0)       13 2023-11-15 06:11:36.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/shares/companies/companies.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.888750 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/shares/shapes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.940750 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/shares/shapes/shape_1/
--rw-r--r--   0 root         (0) root         (0)       11 2023-11-21 16:53:15.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/shares/shapes/shape_1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      135 2023-11-21 16:52:53.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/shares/shapes/shape_1/shape_1.s.HTML
--rw-r--r--   0 root         (0) root         (0)       75 2024-03-17 04:21:22.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/shares/shares.s.HTML
--rw-r--r--   0 root         (0) root         (0)       43 2023-11-17 19:16:25.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/shares/splits.s.HTML
--rw-r--r--   0 root         (0) root         (0)       89 2024-03-18 18:23:30.000000 rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/treasures.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:37:58.940750 rollercoaster-2.1.1/venues/stages/rollercoaster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3309 2024-04-04 23:37:58.000000 rollercoaster-2.1.1/venues/stages/rollercoaster.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)    13574 2024-04-04 23:37:58.000000 rollercoaster-2.1.1/venues/stages/rollercoaster.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2024-04-04 23:37:58.000000 rollercoaster-2.1.1/venues/stages/rollercoaster.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       55 2024-04-04 23:37:58.000000 rollercoaster-2.1.1/venues/stages/rollercoaster.egg-info/entry_points.txt
--rw-rw-r--   0 root         (0) root         (0)      363 2024-04-04 23:37:58.000000 rollercoaster-2.1.1/venues/stages/rollercoaster.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)       14 2024-04-04 23:37:58.000000 rollercoaster-2.1.1/venues/stages/rollercoaster.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1659 2024-04-16 17:59:34.434028 rollercoaster-2.1.2/pyproject.toml
+-rwxr-xr-x   0        0        0     2102 2024-04-04 23:37:49.640824 rollercoaster-2.1.2/readme.md
+-rwxr-xr-x   0        0        0     1312 2024-04-16 18:04:08.058879 rollercoaster-2.1.2/venue.S.HTML
+-rw-r--r--   0        0        0       74 2024-04-08 20:59:40.730227 rollercoaster-2.1.2/venues/stages/rollercoaster/___itinerary/itinerary - aspirations.S.HTML
+-rwxr-xr-x   0        0        0      635 2024-04-09 00:03:01.343222 rollercoaster-2.1.2/venues/stages/rollercoaster/___itinerary/itinerary.S.HTML
+-rwxr-xr-x   0        0        0      574 2024-04-08 21:03:27.655704 rollercoaster-2.1.2/venues/stages/rollercoaster/___itinerary/sequentials/sequentials.S.HTML
+-rwxr-xr-x   0        0        0    51873 2024-03-17 02:26:50.689331 rollercoaster-2.1.2/venues/stages/rollercoaster/___itinerary/sporatic/TradingView Screen.png
+-rwxr-xr-x   0        0        0      381 2024-03-31 19:05:52.370949 rollercoaster-2.1.2/venues/stages/rollercoaster/___itinerary/sporatic/itinerary.S.HTML
+-rwxr-xr-x   0        0        0      384 2024-04-05 03:51:30.492335 rollercoaster-2.1.2/venues/stages/rollercoaster/__bin/rollercoaster_1
+-rwxr-xr-x   0        0        0      225 2024-04-09 02:15:48.675989 rollercoaster-2.1.2/venues/stages/rollercoaster/__data_nodes/moon/clique.py
+-rwxr-xr-x   0        0        0   845985 2024-04-05 04:00:12.449831 rollercoaster-2.1.2/venues/stages/rollercoaster/__data_nodes/moon/listing_status.csv
+-rwxr-xr-x   0        0        0      508 2024-04-05 04:00:10.553855 rollercoaster-2.1.2/venues/stages/rollercoaster/__data_nodes/moon/mongo.S.HTML
+-rwxr-xr-x   0        0        0       45 2024-04-04 18:35:08.441995 rollercoaster-2.1.2/venues/stages/rollercoaster/__init__.py
+-rwxr-xr-x   0        0        0     1960 2024-04-09 02:16:01.627837 rollercoaster-2.1.2/venues/stages/rollercoaster/_interfaces/clique/__init__.py
+-rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 rollercoaster-2.1.2/venues/stages/rollercoaster/_interfaces/clique/group/__init__.py
+-rwxr-xr-x   0        0        0       53 2024-03-31 19:15:22.692288 rollercoaster-2.1.2/venues/stages/rollercoaster/_interfaces/sanic_trails/strails.S.HTML
+-rwxr-xr-x   0        0        0   223468 2024-04-16 18:05:36.317922 rollercoaster-2.1.2/venues/stages/rollercoaster/_status/DB/records.json
+-rwxr-xr-x   0        0        0     1310 2024-04-04 23:37:28.076995 rollercoaster-2.1.2/venues/stages/rollercoaster/_status/clouds_status.proc.py
+-rwxr-xr-x   0        0        0     1203 2024-04-16 18:05:32.053968 rollercoaster-2.1.2/venues/stages/rollercoaster/_status/status.proc.py
+-rwxr-xr-x   0        0        0      114 2024-03-17 06:14:54.911123 rollercoaster-2.1.2/venues/stages/rollercoaster/_status/status_1.py
+-rwxr-xr-x   0        0        0      129 2024-01-26 16:01:45.729782 rollercoaster-2.1.2/venues/stages/rollercoaster/charts/charts.s.HTML
+-rwxr-xr-x   0        0        0      821 2024-03-17 23:24:26.718972 rollercoaster-2.1.2/venues/stages/rollercoaster/charts/plotly/plotly.s.HTML
+-rwxr-xr-x   0        0        0      661 2024-03-31 20:40:53.750991 rollercoaster-2.1.2/venues/stages/rollercoaster/climate/__init__.py
+-rwxr-xr-x   0        0        0      170 2024-04-04 19:34:53.736179 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/AV/AV.s.HTML
+-rwxr-xr-x   0        0        0      276 2024-03-17 21:13:24.014422 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Alpaca/Alpaca.s.HTML
+-rw-r--r--   0        0        0      160 2024-04-09 00:53:14.647459 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Alpaca/_data_API/data.S.HTML
+-rw-r--r--   0        0        0      798 2024-04-09 02:17:59.726458 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Alpaca/_data_API/v2/stock/symbol/bars.py
+-rwxr-xr-x   0        0        0      764 2024-04-04 18:30:31.938755 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Alpaca/crypto/_status/API_status_1.py
+-rwxr-xr-x   0        0        0      448 2024-04-04 18:32:49.240261 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Alpaca/crypto/crypto.S.HTML
+-rwxr-xr-x   0        0        0      980 2024-03-17 20:48:31.394211 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Alpaca/crypto/retrieve.py
+-rwxr-xr-x   0        0        0     1764 2024-04-04 18:31:47.681343 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Alpaca/crypto/structure_1.py
+-rwxr-xr-x   0        0        0       83 2024-04-04 20:04:06.732691 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Alpaca/options/options.S.HTML
+-rwxr-xr-x   0        0        0      390 2024-03-22 18:49:35.640871 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Alpaca/shares/retrieve_one.py
+-rwxr-xr-x   0        0        0      982 2024-03-22 18:48:12.109972 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Alpaca/shares/retrieve_spans.py
+-rwxr-xr-x   0        0        0      107 2024-03-17 18:08:13.242881 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Bybit/Bybit.S.HTML
+-rwxr-xr-x   0        0        0      174 2024-03-18 17:15:52.070050 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/CCXT/CCXT.s.HTML
+-rwxr-xr-x   0        0        0     1039 2024-02-28 18:15:51.229428 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/CCXT/OHLCV/__init__.py
+-rwxr-xr-x   0        0        0     1594 2024-02-28 18:15:51.249428 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/CCXT/OHLCV/candles/__init__.py
+-rwxr-xr-x   0        0        0      565 2024-01-03 02:25:01.331601 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/CCXT/OHLCV/candles/candles.s.HTML
+-rwxr-xr-x   0        0        0     2513 2024-02-28 18:15:51.265428 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/CCXT/OHLCV/candles_v1/__init__.py
+-rwxr-xr-x   0        0        0      565 2024-01-03 02:25:01.331601 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/CCXT/OHLCV/candles_v1/candles.s.HTML
+-rwxr-xr-x   0        0        0        3 2023-12-28 22:53:18.327445 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/CCXT/__init__.py
+-rwxr-xr-x   0        0        0       62 2023-12-28 22:54:25.050671 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/CCXT/coinbase/coinbase.s.HTML
+-rwxr-xr-x   0        0        0      362 2024-02-28 18:15:51.285428 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/CCXT/symbols/array.py
+-rwxr-xr-x   0        0        0      331 2024-04-05 17:46:08.984778 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Clouds Crypto.S.HTML
+-rwxr-xr-x   0        0        0     1030 2024-04-09 00:30:02.259836 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Clouds Shares.S.HTML
+-rwxr-xr-x   0        0        0      597 2024-03-31 19:49:32.345940 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Clouds.S.HTML
+-rwxr-xr-x   0        0        0     2726 2024-02-28 18:15:51.305427 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Coinbase/API/__init__.py
+-rwxr-xr-x   0        0        0      717 2024-02-28 18:15:51.321427 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Coinbase/API/accounts/__init__.py
+-rwxr-xr-x   0        0        0     2042 2024-02-28 18:15:51.341427 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Coinbase/API/build_JWT.py
+-rwxr-xr-x   0        0        0     1260 2024-02-28 18:15:51.361427 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Coinbase/API/orders/order_IDs.py
+-rwxr-xr-x   0        0        0     3281 2024-02-28 18:15:51.381427 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Coinbase/API/products/candles.py
+-rwxr-xr-x   0        0        0      978 2024-02-28 18:15:51.397426 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Coinbase/API/products/catalogue.py
+-rwxr-xr-x   0        0        0      699 2024-02-28 18:15:51.417426 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Coinbase/Coinbase.s.HTML
+-rwxr-xr-x   0        0        0     1543 2024-02-28 18:15:51.437426 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Coinbase/orders/place.py
+-rwxr-xr-x   0        0        0      614 2023-11-25 04:03:55.921174 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/DOGE/doge.s.HTML
+-rwxr-xr-x   0        0        0        0 2024-03-17 22:41:32.234375 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Finnhub/Finnhub.S.HTML
+-rwxr-xr-x   0        0        0       47 2024-03-24 04:04:49.775241 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Finviz.com/Finviz.com.S.HTML
+-rwxr-xr-x   0        0        0      193 2023-11-25 19:05:12.524729 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/LedgerX/LedgerX.s.HTML
+-rwxr-xr-x   0        0        0       10 2023-12-12 05:12:16.566568 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/MQL5/MQL5.s.HTML
+-rwxr-xr-x   0        0        0      226 2023-11-20 05:36:28.995516 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Robinhood/Robinhood.s.HTML
+-rwxr-xr-x   0        0        0       80 2024-03-17 22:16:54.374127 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Tiingo/Tiingo.S.HTML
+-rwxr-xr-x   0        0        0      129 2024-03-31 18:42:05.191819 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Tradier/Tradier.s.HTML
+-rwxr-xr-x   0        0        0      534 2024-04-04 18:44:17.394615 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Tradier/_status/API_status_combine_1.py
+-rwxr-xr-x   0        0        0       36 2024-04-04 19:14:12.097804 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Tradier/procedures/exchanges/__init__.py
+-rwxr-xr-x   0        0        0      122 2024-04-04 19:13:46.242103 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Tradier/procedures/exchanges/exchanges.S.HTML
+-rwxr-xr-x   0        0        0     1351 2024-04-04 19:00:55.635642 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Tradier/procedures/options/combine.py
+-rwxr-xr-x   0        0        0   220164 2023-11-21 17:07:07.643477 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Tradier/procedures/options/example_responses/NOVA_options_chain.JSON
+-rwxr-xr-x   0        0        0      212 2023-10-19 20:16:35.898645 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Tradier/uo_tradier_api.s.HTML
+-rwxr-xr-x   0        0        0     1134 2024-04-04 19:45:42.235028 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Tradier/v1/markets/lookup/__init__.py
+-rwxr-xr-x   0        0        0     1234 2024-04-04 19:24:22.482995 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Tradier/v1/markets/options/chains/__init__.py
+-rwxr-xr-x   0        0        0     1769 2024-04-04 20:05:04.392129 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Tradier/v1/markets/options/chains/parse_1.py
+-rwxr-xr-x   0        0        0      634 2024-02-28 18:15:51.513425 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Tradier/v1/markets/options/expirations/__init__.py
+-rwxr-xr-x   0        0        0      216 2024-03-18 04:26:59.460093 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/TradingView/TV.s.HTML
+-rw-r--r--   0        0        0       80 2024-04-08 21:18:57.873149 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/TradingView/fluctuators/fluctuators.S.HTML
+-rwxr-xr-x   0        0        0      300 2023-12-12 05:03:24.406023 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/TradingView/sensors/__init__.py
+-rwxr-xr-x   0        0        0      237 2024-03-22 19:42:45.277679 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/TradingView/sensors/sensors.S.HTML
+-rwxr-xr-x   0        0        0     3458 2024-03-17 05:35:01.529000 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/TradingView/treasure/indicators/RMI_Trend_Sniper.pine
+-rwxr-xr-x   0        0        0      163 2024-03-17 05:34:46.185162 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/TradingView/treasure/indicators/indicators.S.HTML
+-rwxr-xr-x   0        0        0     3836 2024-03-24 04:00:45.321327 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals/__init__.py
+-rwxr-xr-x   0        0        0     1514 2024-03-31 20:03:17.529323 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals_v2/__init__.py
+-rwxr-xr-x   0        0        0      813 2024-03-22 19:47:25.962582 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals_v2/rooms/print_symbols_table.py
+-rwxr-xr-x   0        0        0     1829 2024-03-22 19:46:48.770994 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals_v2/rooms/scan_symbol.py
+-rwxr-xr-x   0        0        0      495 2024-03-28 00:15:40.797119 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/USA/IRS/IRA/IRA.S.HTML
+-rwxr-xr-x   0        0        0      410 2024-03-27 18:27:21.899277 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/USA/IRS/taxes/income/__init__.py
+-rwxr-xr-x   0        0        0       60 2023-11-10 17:23:06.947404 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/USA/SEC/6K/__init__.py
+-rwxr-xr-x   0        0        0      496 2023-11-10 17:40:32.497079 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/USA/SEC/balance_sheets/__init__.py
+-rwxr-xr-x   0        0        0       18 2023-11-10 17:15:04.345938 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/USA/SEC/balance_sheets/balance_sheets.s.HTML
+-rwxr-xr-x   0        0        0      198 2023-11-10 17:28:03.521299 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/USA/SEC/balance_sheets/equity/__init__.py
+-rwxr-xr-x   0        0        0      420 2023-11-10 17:53:32.039501 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/USA/SEC/income/__init__.py
+-rwxr-xr-x   0        0        0       51 2023-11-10 17:34:28.536151 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/USA/SEC/income/income.s.HTML
+-rwxr-xr-x   0        0        0        0 2023-11-09 20:40:55.437403 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/USA/SEC/statements.s.HTML
+-rwxr-xr-x   0        0        0      212 2023-11-14 04:12:06.841989 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Yahoo/Yahoo.s.HTML
+-rwxr-xr-x   0        0        0     1824 2024-03-18 19:45:43.465891 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Yahoo/retrieve.py
+-rwxr-xr-x   0        0        0      934 2024-03-22 19:39:27.891844 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Yahoo/retrieve_change.py
+-rwxr-xr-x   0        0        0       32 2023-11-14 05:19:00.214473 rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/twelve_data/twelve_data.s.HTML
+-rwxr-xr-x   0        0        0       16 2024-03-24 03:14:51.054648 rollercoaster-2.1.2/venues/stages/rollercoaster/emojis.MD
+-rwxr-xr-x   0        0        0     2589 2023-11-14 05:42:13.790956 rollercoaster-2.1.2/venues/stages/rollercoaster/fluctuators/bt/strategies/example_1.py
+-rwxr-xr-x   0        0        0      130 2024-04-08 20:48:05.178188 rollercoaster-2.1.2/venues/stages/rollercoaster/fluctuators/fluctuators - itinerary.s.HTML
+-rwxr-xr-x   0        0        0      787 2024-04-08 20:48:43.589745 rollercoaster-2.1.2/venues/stages/rollercoaster/fluctuators/fluctuators.S.HTML
+-rwxr-xr-x   0        0        0      121 2023-11-28 03:26:29.420655 rollercoaster-2.1.2/venues/stages/rollercoaster/fluctuators/lumi/lumi.s.HTML
+-rwxr-xr-x   0        0        0      100 2023-12-19 04:49:40.656260 rollercoaster-2.1.2/venues/stages/rollercoaster/fluctuators/rover_1/rover_1.s.HTML
+-rwxr-xr-x   0        0        0      446 2024-02-28 18:15:51.581424 rollercoaster-2.1.2/venues/stages/rollercoaster/gadgets/clock/UTC/ISO.py
+-rw-r--r--   0        0        0      352 2024-04-09 02:17:43.626646 rollercoaster-2.1.2/venues/stages/rollercoaster/gadgets/clock/UTC/current.py
+-rwxr-xr-x   0        0        0      984 2024-02-28 18:15:51.565425 rollercoaster-2.1.2/venues/stages/rollercoaster/gadgets/clock/UTC/greatness_1.py
+-rwxr-xr-x   0        0        0      288 2024-04-09 02:03:24.336835 rollercoaster-2.1.2/venues/stages/rollercoaster/gadgets/clock/clock.s.HTML
+-rwxr-xr-x   0        0        0      620 2023-11-09 20:46:40.432504 rollercoaster-2.1.2/venues/stages/rollercoaster/gadgets/format_percentage.py
+-rwxr-xr-x   0        0        0      151 2023-11-23 05:19:27.179399 rollercoaster-2.1.2/venues/stages/rollercoaster/gadgets/math/slope/__init__.py
+-rwxr-xr-x   0        0        0       79 2024-01-10 05:54:37.773115 rollercoaster-2.1.2/venues/stages/rollercoaster/gadgets/pandas/DF/DF.s.HTML
+-rwxr-xr-x   0        0        0      519 2024-02-28 18:15:51.653423 rollercoaster-2.1.2/venues/stages/rollercoaster/gadgets/pandas/DF/_status/status_from_1.py
+-rwxr-xr-x   0        0        0      252 2024-02-28 18:15:51.673423 rollercoaster-2.1.2/venues/stages/rollercoaster/gadgets/pandas/DF/from_list.py
+-rwxr-xr-x   0        0        0      326 2024-03-17 21:21:47.633007 rollercoaster-2.1.2/venues/stages/rollercoaster/gadgets/pandas/DF/to_list.py
+-rwxr-xr-x   0        0        0      690 2024-01-13 06:12:46.871796 rollercoaster-2.1.2/venues/stages/rollercoaster/gadgets/pandas/pandas.s.HTML
+-rwxr-xr-x   0        0        0      402 2024-02-28 18:15:51.689423 rollercoaster-2.1.2/venues/stages/rollercoaster/gadgets/ratio.py
+-rwxr-xr-x   0        0        0      457 2024-02-28 18:15:51.709423 rollercoaster-2.1.2/venues/stages/rollercoaster/gadgets/summation/__init__.py
+-rwxr-xr-x   0        0        0      377 2024-02-28 18:15:51.761422 rollercoaster-2.1.2/venues/stages/rollercoaster/gadgets/summation/status_1.py
+-rwxr-xr-x   0        0        0    18282 2023-12-28 23:17:20.176165 rollercoaster-2.1.2/venues/stages/rollercoaster/gadgets/summation/summation.svg
+-rwxr-xr-x   0        0        0      100 2024-04-09 02:03:10.212995 rollercoaster-2.1.2/venues/stages/rollercoaster/gadgets/tools.s.HTML
+-rwxr-xr-x   0        0        0     2102 2024-04-04 20:32:10.597520 rollercoaster-2.1.2/venues/stages/rollercoaster/home.MD
+-rwxr-xr-x   0        0        0     1081 2024-04-09 00:01:58.996000 rollercoaster-2.1.2/venues/stages/rollercoaster/home.s.HTML
+-rw-r--r--   0        0        0      425 2024-04-09 02:33:16.647876 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/rides - formats.S.HTML
+-rw-r--r--   0        0        0      319 2024-04-08 17:38:46.213186 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/rides - itinerary.S.HTML
+-rwxr-xr-x   0        0        0     1334 2024-04-08 20:50:23.708590 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/rides.S.HTML
+-rwxr-xr-x   0        0        0      489 2023-12-31 05:03:05.192136 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/ATR/ATR.s.HTML
+-rwxr-xr-x   0        0        0     2944 2024-03-18 04:08:14.882175 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/ATR/ChatGPT_ATR_1/__init__.py
+-rwxr-xr-x   0        0        0     1591 2024-03-18 04:08:14.838176 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/ATR/__init__.py
+-rwxr-xr-x   0        0        0     1242 2024-03-18 04:08:14.866176 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/ATR/_status/status_1.py
+-rwxr-xr-x   0        0        0     1731 2024-01-02 03:23:31.042432 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/Andean_Oscillator/AO.pine
+-rwxr-xr-x   0        0        0      134 2023-12-01 02:49:14.211328 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/Andean_Oscillator/Andean.r.HTML
+-rwxr-xr-x   0        0        0      273 2023-12-31 06:36:06.223233 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/EMA/EMA.s.HTML
+-rwxr-xr-x   0        0        0       82 2023-11-14 05:05:08.114737 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/EMA/__init__.py
+-rwxr-xr-x   0        0        0     4821 2024-01-02 03:23:31.085431 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/HHLL/indicator.pine
+-rwxr-xr-x   0        0        0       72 2023-12-03 22:10:44.686991 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/MA/MA.r.HTML
+-rwxr-xr-x   0        0        0       91 2023-12-12 04:16:31.428608 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/MACD/MACD.s.HTML
+-rwxr-xr-x   0        0        0       48 2023-12-02 00:37:47.807470 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/QQE/QQE.r.HTML
+-rwxr-xr-x   0        0        0      201 2023-12-03 02:58:48.769709 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/RSI/RSI.r.HTML
+-rwxr-xr-x   0        0        0      782 2024-03-18 04:08:14.894175 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/RSI/__init__.py
+-rwxr-xr-x   0        0        0      250 2024-01-02 06:36:59.547427 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/SMA/__init__.py
+-rwxr-xr-x   0        0        0      397 2024-01-02 03:23:31.177430 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/TR/TR.s.HTML
+-rwxr-xr-x   0        0        0    47171 2023-12-28 18:38:03.620071 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/TR/True Range.svg
+-rwxr-xr-x   0        0        0     1628 2024-03-18 04:08:14.978174 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/TR/__init__.py
+-rwxr-xr-x   0        0        0      523 2024-03-18 04:08:14.994174 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/TR/_status/status_1.py
+-rwxr-xr-x   0        0        0      792 2024-03-18 04:08:15.006173 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/TR/_status/status_2.py
+-rwxr-xr-x   0        0        0      254 2023-11-29 18:25:15.058846 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/TV.r.HTML
+-rwxr-xr-x   0        0        0       46 2023-11-21 16:46:45.097491 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/VWAP/VWAP.r.HTML
+-rwxr-xr-x   0        0        0      593 2024-03-18 04:08:15.014173 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/VWAP/__init__.py
+-rwxr-xr-x   0        0        0       47 2023-11-21 16:46:17.697805 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/VWMA/VWMA.r.HTML
+-rwxr-xr-x   0        0        0       24 2023-11-14 04:28:20.239207 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/bolinger_bands/bolinger_bands.r.html
+-rwxr-xr-x   0        0        0        0 2023-11-30 18:13:51.268620 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/chandlier_exit/chandelier exit.r.HTML
+-rwxr-xr-x   0        0        0      546 2024-02-28 18:15:52.105418 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/indicators.s.HTML
+-rwxr-xr-x   0        0        0     1266 2024-01-02 03:23:31.097431 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/pivot_point/pivot_point.s.HTML
+-rwxr-xr-x   0        0        0       28 2023-11-21 16:43:07.835981 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/relative_volume/relative volume.r.HTML
+-rwxr-xr-x   0        0        0     2832 2024-03-18 04:08:14.950174 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/supertrend/ST_1_ChatGPT/__init__.py
+-rwxr-xr-x   0        0        0     1098 2024-03-18 04:08:14.910175 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/supertrend/__init__.py
+-rwxr-xr-x   0        0        0     1243 2024-03-18 04:08:14.942175 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/supertrend/_status/status_1.py
+-rwxr-xr-x   0        0        0      358 2024-01-06 00:03:10.850549 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/supertrend/pandas_ta/__init__.py
+-rwxr-xr-x   0        0        0      225 2023-12-03 02:59:17.552392 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/supertrend/supertrend.s.HTML
+-rwxr-xr-x   0        0        0        0 2024-01-02 03:30:08.272935 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/supertrend2/__init__.py
+-rwxr-xr-x   0        0        0     1215 2024-03-18 04:08:15.046173 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_2/AAS/__init__.py
+-rwxr-xr-x   0        0        0     1230 2024-03-18 04:08:15.066173 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_2/AAS/_status/status_1.py
+-rwxr-xr-x   0        0        0      334 2024-01-06 07:25:23.819962 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_2/AS/AS.s.HTML
+-rwxr-xr-x   0        0        0    47171 2023-12-28 18:38:03.620071 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_2/AS/AS.svg
+-rwxr-xr-x   0        0        0     1544 2024-03-18 04:08:15.074173 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_2/AS/__init__.py
+-rwxr-xr-x   0        0        0      511 2024-03-18 04:08:15.094172 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_2/AS/_status/status_1.py
+-rwxr-xr-x   0        0        0      783 2024-03-18 04:08:15.106172 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_2/AS/_status/status_2.py
+-rwxr-xr-x   0        0        0     1093 2024-01-06 07:15:37.995569 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_2/pecdency/__init__.py
+-rwxr-xr-x   0        0        0     1350 2024-03-18 04:08:15.118172 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_2/pecdency/__init__v1.py
+-rwxr-xr-x   0        0        0     4116 2024-03-18 04:08:15.278170 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_3/ST/__init__.py
+-rwxr-xr-x   0        0        0      433 2024-03-18 04:08:15.362168 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_3/VDA/__init__.py
+-rwxr-xr-x   0        0        0      567 2024-03-18 04:08:15.382168 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_3/VSA/__init__.py
+-rwxr-xr-x   0        0        0      334 2024-01-09 01:54:38.423714 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_3/physical_span/AS.s.HTML
+-rwxr-xr-x   0        0        0    47171 2023-12-28 18:38:03.620071 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_3/physical_span/AS.svg
+-rwxr-xr-x   0        0        0     1557 2024-03-18 04:08:15.146171 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_3/physical_span/__init__.py
+-rwxr-xr-x   0        0        0      522 2024-03-18 04:08:15.166171 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_3/physical_span/_status/status_1.py
+-rwxr-xr-x   0        0        0      790 2024-03-18 04:08:15.178171 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_3/physical_span/_status/status_2.py
+-rwxr-xr-x   0        0        0     1183 2024-03-18 04:08:15.190171 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_3/physical_span_average/__init__.py
+-rwxr-xr-x   0        0        0     1248 2024-03-18 04:08:15.210171 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_3/physical_span_average/_status/status_1.py
+-rwxr-xr-x   0        0        0     3688 2024-03-18 04:08:15.222170 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_3/physical_span_reversals/__init__.py
+-rwxr-xr-x   0        0        0     3586 2024-03-18 04:08:15.250170 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_3/physical_span_roads_v1/__init__.py
+-rwxr-xr-x   0        0        0     3862 2024-03-18 04:08:15.306169 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_3/super_hero_trend/__init__.py
+-rwxr-xr-x   0        0        0     1759 2024-03-18 04:08:15.322169 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_3/super_hero_trend/win_rates/shares_trading.py
+-rwxr-xr-x   0        0        0      961 2024-03-18 04:08:15.334169 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_3/supertrend/__init__.py
+-rwxr-xr-x   0        0        0     1825 2024-03-18 04:08:15.406168 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_4/AO/__init__.py
+-rw-r--r--   0        0        0     5968 2024-04-11 03:49:19.489710 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_4/ML_Lorentzian/KernelFunctions.ps
+-rw-r--r--   0        0        0    36151 2024-04-11 03:49:38.505474 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_4/ML_Lorentzian/Lorentzian Classification.ps
+-rw-r--r--   0        0        0    18799 2024-04-11 03:48:20.246452 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_4/ML_Lorentzian/MLExtensions.ps
+-rwxr-xr-x   0        0        0     3926 2024-03-18 04:08:15.418168 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_4/superb/__init__.py
+-rwxr-xr-x   0        0        0       13 2024-02-01 15:34:15.615610 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_4/superb/superb.s.HTML
+-rwxr-xr-x   0        0        0     1786 2024-03-18 04:08:15.430168 rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_4/superb/win_rates/shares_trading.py
+-rwxr-xr-x   0        0        0     4000 2024-04-04 17:03:41.281223 rollercoaster-2.1.2/venues/stages/rollercoaster/scans/_clique/ETF.py
+-rwxr-xr-x   0        0        0        2 2024-04-04 18:06:03.015402 rollercoaster-2.1.2/venues/stages/rollercoaster/scans/_clique/REIT.py
+-rwxr-xr-x   0        0        0     2162 2024-04-04 18:22:34.680804 rollercoaster-2.1.2/venues/stages/rollercoaster/scans/_clique/TV.py
+-rwxr-xr-x   0        0        0     1411 2024-04-04 17:36:52.196339 rollercoaster-2.1.2/venues/stages/rollercoaster/scans/_clique/currency.py
+-rwxr-xr-x   0        0        0       42 2024-04-04 18:06:43.814870 rollercoaster-2.1.2/venues/stages/rollercoaster/scans/_clique/penny_stocks.py
+-rwxr-xr-x   0        0        0      415 2024-04-04 18:22:24.940895 rollercoaster-2.1.2/venues/stages/rollercoaster/scans/clique.py
+-rwxr-xr-x   0        0        0      180 2024-04-15 19:29:36.357014 rollercoaster-2.1.2/venues/stages/rollercoaster/scans/screeners.S.HTML
+-rwxr-xr-x   0        0        0      119 2024-03-31 19:49:32.365940 rollercoaster-2.1.2/venues/stages/rollercoaster/scans/symbol/__init__.py
+-rwxr-xr-x   0        0        0      941 2024-04-15 19:25:57.778780 rollercoaster-2.1.2/venues/stages/rollercoaster/scans/symbol/symbols.S.HTML
+-rw-r--r--   0        0        0       84 2024-04-08 20:53:48.054233 rollercoaster-2.1.2/venues/stages/rollercoaster/stats/VHLOC/MACD/MACD.S.HTML
+-rw-r--r--   0        0        0      105 2024-04-08 20:51:20.623934 rollercoaster-2.1.2/venues/stages/rollercoaster/stats/VHLOC/MACD/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 20:53:19.026568 rollercoaster-2.1.2/venues/stages/rollercoaster/stats/VHLOC/MACD/procedure.ps
+-rwxr-xr-x   0        0        0     5120 2024-04-04 18:12:45.242647 rollercoaster-2.1.2/venues/stages/rollercoaster/stats/aggregate_PC_ratio/__init__.py
+-rwxr-xr-x   0        0        0     1958 2024-03-31 19:02:25.517446 rollercoaster-2.1.2/venues/stages/rollercoaster/stats/aggregate_PC_ratio/squeeze pc ratios.r.HTML
+-rwxr-xr-x   0        0        0   388314 2023-11-09 20:42:52.592079 rollercoaster-2.1.2/venues/stages/rollercoaster/stats/aggregate_PC_ratio/status/examples/1.JSON
+-rwxr-xr-x   0        0        0     1567 2023-11-09 20:42:52.591079 rollercoaster-2.1.2/venues/stages/rollercoaster/stats/aggregate_PC_ratio/status/examples/2.JSON
+-rwxr-xr-x   0        0        0      593 2024-02-28 18:15:51.993420 rollercoaster-2.1.2/venues/stages/rollercoaster/stats/aggregate_PC_ratio/status/status_1.py
+-rwxr-xr-x   0        0        0     1860 2024-02-28 18:15:52.009419 rollercoaster-2.1.2/venues/stages/rollercoaster/stats/aggregate_PC_ratio/status/status_2.py
+-rwxr-xr-x   0        0        0     2905 2024-03-31 18:52:09.009522 rollercoaster-2.1.2/venues/stages/rollercoaster/stats/aggregate_break_even/__init__.py
+-rwxr-xr-x   0        0        0     2290 2023-12-04 02:47:32.197228 rollercoaster-2.1.2/venues/stages/rollercoaster/stats/aggregate_break_even/_status/examples/0.JSON
+-rwxr-xr-x   0        0        0   388314 2023-11-09 20:42:52.592079 rollercoaster-2.1.2/venues/stages/rollercoaster/stats/aggregate_break_even/_status/examples/1.JSON
+-rwxr-xr-x   0        0        0     1567 2023-11-09 20:42:52.591079 rollercoaster-2.1.2/venues/stages/rollercoaster/stats/aggregate_break_even/_status/examples/2.JSON
+-rwxr-xr-x   0        0        0     1508 2024-02-28 18:15:51.849421 rollercoaster-2.1.2/venues/stages/rollercoaster/stats/aggregate_break_even/_status/status_1.py
+-rwxr-xr-x   0        0        0      794 2024-02-28 18:15:51.869421 rollercoaster-2.1.2/venues/stages/rollercoaster/stats/aggregate_break_even/_status/status_2.py
+-rwxr-xr-x   0        0        0     1000 2024-04-05 04:05:45.569767 rollercoaster-2.1.2/venues/stages/rollercoaster/stats/aggregate_break_even/aggregate break even.s.HTML
+-rwxr-xr-x   0        0        0        0 2024-03-31 19:07:37.005708 rollercoaster-2.1.2/venues/stages/rollercoaster/stats/aggregate_break_even/clique.py
+-rwxr-xr-x   0        0        0      892 2024-02-28 18:15:51.889421 rollercoaster-2.1.2/venues/stages/rollercoaster/stats/aggregate_break_even/show/__init__.py
+-rwxr-xr-x   0        0        0     1599 2024-03-31 18:39:18.393448 rollercoaster-2.1.2/venues/stages/rollercoaster/stats/aggregate_multiplier/aggregate_multipliers.r.HTML
+-rwxr-xr-x   0        0        0     1427 2024-04-05 03:53:28.182846 rollercoaster-2.1.2/venues/stages/rollercoaster/stats/clique.py
+-rwxr-xr-x   0        0        0      311 2024-04-05 04:21:31.280203 rollercoaster-2.1.2/venues/stages/rollercoaster/stats/option_priceyness/option_priceyness.S.HTML
+-rwxr-xr-x   0        0        0      562 2024-04-05 04:33:13.144392 rollercoaster-2.1.2/venues/stages/rollercoaster/stats/stats.s.HTML
+-rwxr-xr-x   0        0        0      352 2024-04-05 04:38:34.656724 rollercoaster-2.1.2/venues/stages/rollercoaster/stats/the_multiplier/__init__.py
+-rwxr-xr-x   0        0        0      911 2024-03-17 21:11:40.987538 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/commodities/commodities.s.HTML
+-rw-r--r--   0        0        0       89 2024-04-08 22:27:54.205084 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/contracts/contracts.S.HTML
+-rw-r--r--   0        0        0      339 2024-04-13 19:27:27.156565 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/crypto/L1/L1.S.HTML
+-rw-r--r--   0        0        0      725 2024-04-13 19:19:01.872575 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/crypto/crypto.S.HTML
+-rw-r--r--   0        0        0       61 2024-04-13 19:26:04.032669 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/crypto/crypto_rust.S.HTML
+-rw-r--r--   0        0        0      641 2024-04-13 19:19:32.260629 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/crypto/crypto_usual_features.S.HTML
+-rwxr-xr-x   0        0        0       29 2023-11-21 17:46:09.752570 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/forex/forex.s.HTML
+-rwxr-xr-x   0        0        0       75 2024-01-30 00:33:10.380046 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/futures/futures.s.HTML
+-rw-r--r--   0        0        0      177 2024-04-16 18:07:20.864815 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/gems/gems.S.HTML
+-rw-r--r--   0        0        0       48 2024-04-08 17:11:40.338334 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/options/greeks/greeks.S.HTML
+-rwxr-xr-x   0        0        0     1565 2024-02-28 18:15:52.809410 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/options/movement_calculator/__init__.py
+-rwxr-xr-x   0        0        0     1167 2023-11-23 05:20:06.387999 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/options/movement_calculator/slope.s.HTML
+-rwxr-xr-x   0        0        0     2572 2024-04-05 05:24:21.970535 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/options/multipliers/__init__.py
+-rwxr-xr-x   0        0        0      358 2024-04-08 17:12:06.086114 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/options/options.s.HTML
+-rwxr-xr-x   0        0        0     1498 2024-02-28 18:15:52.809410 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/options/shapes/shape_1/__init__.py
+-rwxr-xr-x   0        0        0      489 2023-11-21 17:09:02.275163 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/options/shapes/shape_1/shape_1.s.HTML
+-rw-r--r--   0        0        0      147 2024-04-08 21:43:35.583640 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/real_estate/__init__.py
+-rw-r--r--   0        0        0      156 2024-04-08 23:27:06.857428 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/real_estate/loans/loans.S.HTML
+-rw-r--r--   0        0        0      431 2024-04-08 21:38:29.659326 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/real_estate/loans/mortgages/constant.py
+-rw-r--r--   0        0        0       95 2024-04-08 21:54:20.848024 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/real_estate/loans/mortgages/insurance/insurance.S.HTML
+-rw-r--r--   0        0        0      587 2024-04-08 22:05:05.892491 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/real_estate/loans/mortgages/loan - varieties.S.HTML
+-rw-r--r--   0        0        0     1202 2024-04-08 22:40:59.788117 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/real_estate/loans/mortgages/loan.S.HTML
+-rw-r--r--   0        0        0     1463 2024-04-09 00:50:23.861466 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/real_estate/loans/mortgages/sources/sources.S.HTML
+-rwxr-xr-x   0        0        0      414 2024-04-08 22:42:58.322845 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/real_estate/real_estate.S.HTML
+-rw-r--r--   0        0        0      437 2024-04-08 21:43:11.491928 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/real_estate/sends.S.HTML
+-rw-r--r--   0        0        0      127 2024-04-08 21:37:42.099907 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/real_estate/tax/__init__.py
+-rw-r--r--   0        0        0       97 2024-04-08 21:48:11.608365 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/real_estate/tax/tax.S.HTML
+-rw-r--r--   0        0        0     2434 2024-04-08 22:08:51.961985 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/real_estate/varieties/varieties.S.HTML
+-rwxr-xr-x   0        0        0     1190 2024-03-31 19:49:32.365940 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/shares/ETF/ETF.s.HTML
+-rwxr-xr-x   0        0        0      114 2023-11-15 06:29:25.238807 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/shares/ETF/comprehensive/comprehensive.s.HTML
+-rwxr-xr-x   0        0        0       42 2023-11-15 06:37:06.461104 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/shares/ETF/sectors/airlines/airlines.r.HTML
+-rwxr-xr-x   0        0        0       45 2023-11-15 06:38:49.083268 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/shares/ETF/sectors/electronics/semiconductors.r.HTML
+-rwxr-xr-x   0        0        0       81 2023-11-15 06:34:55.671168 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/shares/ETF/sectors/farming/farming.r.HTML
+-rwxr-xr-x   0        0        0       84 2023-11-15 06:37:33.924880 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/shares/ETF/sectors/real estate/real estate.r.HTML
+-rwxr-xr-x   0        0        0      157 2024-03-17 04:50:30.861349 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/shares/ETF/sectors/sectors.S.HTML
+-rwxr-xr-x   0        0        0       14 2023-11-15 06:36:56.273187 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/shares/ETF/sectors/vehicles/vehicles.r.HTML
+-rwxr-xr-x   0        0        0        7 2024-03-24 04:01:12.905095 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/shares/__init__.py
+-rwxr-xr-x   0        0        0       13 2023-11-15 06:11:36.293215 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/shares/companies/companies.s.HTML
+-rwxr-xr-x   0        0        0       11 2023-11-21 16:53:15.238020 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/shares/shapes/shape_1/__init__.py
+-rwxr-xr-x   0        0        0      135 2023-11-21 16:52:53.862265 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/shares/shapes/shape_1/shape_1.s.HTML
+-rwxr-xr-x   0        0        0      106 2024-04-08 19:07:13.173774 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/shares/shares.s.HTML
+-rwxr-xr-x   0        0        0       43 2023-11-17 19:16:25.824071 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/shares/splits.s.HTML
+-rwxr-xr-x   0        0        0       90 2024-04-08 19:06:53.069998 rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/treasures.s.HTML
+-rw-r--r--   0        0        0     4395 1970-01-01 00:00:00.000000 rollercoaster-2.1.2/PKG-INFO
```

### Comparing `rollercoaster-2.1.1/readme.md` & `rollercoaster-2.1.2/readme.md`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/_interfaces/clique/__init__.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/_interfaces/clique/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 
 
 from .group import clique as clique_group
 
 from rollercoaster.stats.clique import stats_group
 from rollercoaster.scans.clique import scans_group
+from rollercoaster.__data_nodes.moon.clique import moon_group
 
 def clique ():
 	import click
 	@click.group ()
 	def group ():
 		pass
 
@@ -76,14 +77,15 @@
 	group.add_command (example_command)
 	group.add_command (open_sphene)
 
 	group.add_command (clique_group ())
 	group.add_command (stats_group ())	
 	group.add_command (scans_group ())	
 	
+	group.add_command (moon_group ())	
 	
 	group ()
 
 
 
 
 #
```

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/_status/insurance.proc.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/_status/clouds_status.proc.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,29 +18,34 @@
 ])
 
 
 import json
 import pathlib
 from os.path import dirname, join, normpath
 
+
+this_module_name = ""
+
 this_folder = pathlib.Path (__file__).parent.resolve ()
 structures = str (normpath (join (this_folder, "../../../../venues")))
 
+this_module = str (normpath (join (structures, "stages", this_module_name)))
+
+#status_assurances_path = str (normpath (join (this_folder, "insurance")))
 status_assurances_path = str (normpath (join (this_folder, "..")))
 
 import sys
 if (len (sys.argv) >= 2):
 	glob_string = status_assurances_path + '/' + sys.argv [1]
 	db_directory = False
 else:
-	glob_string = status_assurances_path + '/**/status_*.py'
+	glob_string = status_assurances_path + '/**/API_status_*.py'
 	db_directory = normpath (join (this_folder, "DB"))
 
 print ("glob string:", glob_string)
-print ("structures:", structures)
 
 import volts
 scan = volts.start (
 	glob_string = glob_string,
 	simultaneous = True,
 	module_paths = [
 		normpath (join (structures, "stages")),
```

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/autopilot/bt/strategies/example_1.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/fluctuators/bt/strategies/example_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/autopilot/rovers.s.HTML` & `rollercoaster-2.1.2/venues/stages/rollercoaster/fluctuators/fluctuators.S.HTML`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 
 
 <pre>
 
-	<h1>rovers</h1>
+	<h1>fluctuators</h1>
+		# rovers
 		# autopilot
-
+		# player
+		# pivoter
+		# fluctuator
+	
 	<h2>priorities</h2>
 		stop loss
 			dump position if:
 				after 5 minutes
 				share price is less than or equal to 100
 				share price is greater than or equal to 150
```

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/charts/plotly/plotly.s.HTML` & `rollercoaster-2.1.2/venues/stages/rollercoaster/charts/plotly/plotly.s.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/climate/__init__.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/climate/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Alpaca/crypto/_status/API_status_1.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Alpaca/crypto/_status/API_status_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Alpaca/crypto/retrieve.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Alpaca/crypto/retrieve.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Alpaca/crypto/structure_1.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Alpaca/crypto/structure_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Alpaca/shares/retrieve_spans.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Alpaca/shares/retrieve_spans.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/CCXT/OHLCV/__init__.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/CCXT/OHLCV/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/CCXT/OHLCV/candles/__init__.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/CCXT/OHLCV/candles/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/CCXT/OHLCV/candles/candles.s.HTML` & `rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/CCXT/OHLCV/candles/candles.s.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/CCXT/OHLCV/candles_v1/__init__.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/CCXT/OHLCV/candles_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/CCXT/OHLCV/candles_v1/candles.s.HTML` & `rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/CCXT/OHLCV/candles_v1/candles.s.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Clouds Shares.S.HTML` & `rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Clouds Shares.S.HTML`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 
 
 <pre>
 
 	<h1>Shares</h1>
 		scans:
 			tradingview
-			
 			finviz
 	
+		VLOCH:
+			# candles
+	
+	
 		trading:
 			alpaca
 			finnhub
 			tradier
 			iexcloud
 	
 			https://www.composer.trade/
```

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Clouds.S.HTML` & `rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Clouds.S.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Coinbase/API/__init__.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Coinbase/API/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Coinbase/API/accounts/__init__.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Coinbase/API/accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Coinbase/API/build_JWT.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Coinbase/API/build_JWT.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Coinbase/API/orders/order_IDs.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Coinbase/API/orders/order_IDs.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Coinbase/API/products/candles.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Coinbase/API/products/candles.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Coinbase/API/products/catalogue.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Coinbase/API/products/catalogue.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Coinbase/Coinbase.s.HTML` & `rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Coinbase/Coinbase.s.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Coinbase/orders/place.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Coinbase/orders/place.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/DOGE/doge.s.HTML` & `rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/DOGE/doge.s.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Tradier/_status/API_status_combine_1.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Tradier/_status/API_status_combine_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Tradier/procedures/options/combine.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Tradier/procedures/options/combine.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Tradier/v1/markets/lookup/__init__.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Tradier/v1/markets/lookup/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Tradier/v1/markets/options/chains/__init__.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Tradier/v1/markets/options/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Tradier/v1/markets/options/chains/parse_1.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Tradier/v1/markets/options/chains/parse_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Tradier/v1/markets/options/expirations/__init__.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Tradier/v1/markets/options/expirations/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals/__init__.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals_v2/__init__.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals_v2/rooms/print_symbols_table.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals_v2/rooms/print_symbols_table.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals_v2/rooms/scan_symbol.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/TradingView/treasure/technicals_v2/rooms/scan_symbol.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Yahoo/retrieve.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Yahoo/retrieve.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/clouds/Yahoo/retrieve_change.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/clouds/Yahoo/retrieve_change.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/gadgets/clock/UTC/greatness_1.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/gadgets/clock/UTC/greatness_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/gadgets/format_percentage.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/gadgets/format_percentage.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/gadgets/pandas/DF/_status/status_from_1.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/gadgets/pandas/DF/_status/status_from_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/gadgets/pandas/pandas.s.HTML` & `rollercoaster-2.1.2/venues/stages/rollercoaster/gadgets/pandas/pandas.s.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/home.s.HTML` & `rollercoaster-2.1.2/venues/stages/rollercoaster/home.s.HTML`

 * *Files 27% similar despite different names*

```diff
@@ -4,15 +4,44 @@
 
 	<h1>rollercoaster</h1>
 		# treasury
 		# rollercoaster or oppression
 		# reign or poor
 			# rain or pour
 		
+	
+	<h2>vernacular</h2>
+		
+		trader
+			# fluctuator
+				# pie fluctuator
+				# vote fluctuator
+				
+				# whimsical
+			
+			# modulator
+			
+			# oscillator
+				# currency oscillator
+			
+			# shifter
+			
+			# modifier
+			
+			
+			# swapper
+			# mutator
+			
+			# converter
+			# transformer
+			
+			# transitioner
 			
+			# dealer
+	
 
 	<h2>relevant</h2>
 		"sphene" documentation:
 		
 		
 		
 		"onesie" checks:
```

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/ATR/ChatGPT_ATR_1/__init__.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/ATR/ChatGPT_ATR_1/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/ATR/__init__.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/ATR/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/ATR/_status/status_1.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/ATR/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/RSI/__init__.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/RSI/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/TR/__init__.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/TR/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/TR/_status/status_1.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/TR/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/TR/_status/status_2.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/TR/_status/status_2.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/VWAP/__init__.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/VWAP/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/indicators.s.HTML` & `rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/indicators.s.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/pivot_point/pivot_point.s.HTML` & `rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/pivot_point/pivot_point.s.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/supertrend/ST_1_ChatGPT/__init__.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/supertrend/ST_1_ChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/supertrend/__init__.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/supertrend/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_1/supertrend/_status/status_1.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_1/supertrend/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_2/AAS/__init__.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_2/AAS/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_2/AAS/_status/status_1.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_2/AAS/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_2/AS/__init__.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_2/AS/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_2/AS/_status/status_2.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_2/AS/_status/status_2.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_2/pecdency/__init__.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_2/pecdency/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_2/pecdency/__init__v1.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_2/pecdency/__init__v1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/ST/__init__.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_3/ST/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/VSA/__init__.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_3/VSA/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/physical_span/__init__.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_3/physical_span/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/physical_span/_status/status_1.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_3/physical_span/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/physical_span/_status/status_2.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_3/physical_span/_status/status_2.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/physical_span_average/__init__.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_3/physical_span_average/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/physical_span_average/_status/status_1.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_3/physical_span_average/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/physical_span_reversals/__init__.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_3/physical_span_reversals/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/physical_span_roads_v1/__init__.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_3/physical_span_roads_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/super_hero_trend/__init__.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_3/super_hero_trend/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/super_hero_trend/win_rates/shares_trading.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_3/super_hero_trend/win_rates/shares_trading.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_3/supertrend/__init__.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_3/supertrend/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_4/AO/__init__.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_4/AO/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_4/superb/__init__.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_4/superb/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/rides/season_4/superb/win_rates/shares_trading.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/rides/season_4/superb/win_rates/shares_trading.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/scans/_clique/ETF.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/scans/_clique/ETF.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/scans/_clique/TV.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/scans/_clique/TV.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/scans/_clique/currency.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/scans/_clique/currency.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/scans/symbol/symbols.S.HTML` & `rollercoaster-2.1.2/venues/stages/rollercoaster/scans/symbol/symbols.S.HTML`

 * *Files 22% similar despite different names*

```diff
@@ -26,22 +26,31 @@
 			
 			rich.print_json (data = symbols_indicators)
 			TV_treasure_tech.print_symbols_table (symbols_indicators)
 
 		
 		<h3>Options Indicators</h3>
 
-
+		<h3>Whales</h3>
+			# Big Trades
+			# Empire Trades
+			#
+		
+			https://unusualwhales.com/flow/overview
+			https://whalewisdom.com/
 
 		<h3>Analyst Opinions</h3>
 
 
 
 		<h3>Change Percentages</h3>
 			<h3>Market Cap</h3>
 			
 			
 		
 		<h3>Shareholder Equity</h3>
 			
+			
+		<h3>Sentiments</h3>
+			# LLM
 
 </pre>
```

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/stats/aggregate_PC_ratio/__init__.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/stats/aggregate_PC_ratio/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/stats/aggregate_PC_ratio/squeeze pc ratios.r.HTML` & `rollercoaster-2.1.2/venues/stages/rollercoaster/stats/aggregate_PC_ratio/squeeze pc ratios.r.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/stats/aggregate_PC_ratio/status/status_1.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/stats/aggregate_PC_ratio/status/status_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/stats/aggregate_PC_ratio/status/status_2.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/stats/aggregate_PC_ratio/status/status_2.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/stats/aggregate_break_even/__init__.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/stats/aggregate_break_even/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/stats/aggregate_break_even/_status/status_1.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/stats/aggregate_break_even/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/stats/aggregate_break_even/_status/status_2.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/stats/aggregate_break_even/_status/status_2.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/stats/aggregate_break_even/aggregate break even.s.HTML` & `rollercoaster-2.1.2/venues/stages/rollercoaster/stats/aggregate_break_even/aggregate break even.s.HTML`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 
 <pre>
 
 	<h1>aggregate break even</h1>
 		
-		<h2>tutorial</h2>
+	<h2>tutorial</h2>
 		<code>
 		
 			Tradier_API_authorization = ""
 		
 			import rollercoaster.stats.aggregate_break_even as aggregate_break_even
 			break_evens = aggregate_break_even.calc ({
 				"expirations": combine_options.presently ({
 					"symbol": "OTLY",
 					"authorization": Tradier_API_authorization
 				})
 			})
 		
 		</code>
-		
-		<b>priorities:</b>
-		
-			[ ] perhaps a version that is exclusively about
-				the ask price, and doesn't care about "open interest"
-		
-				A version like this would essentially show how 
-				expensive the options contracts are.
-		
-		<b>formulas</b>
-		
-			[ 
-				for every contract,
-				for every call,
-				for every put,
-				for every call at an expiration,
-				for every put at an expiration,			
-			]
-				summation (contract price * break even * open interest * shares per contract)
-				---
-				summation (contract price * open interest * shares per contract) 
+	
+	<h2>itinerary</h2>
+	
+		[ ] perhaps a version that is exclusively about
+			the ask price, and doesn't care about "open interest"
+	
+			A version like this would essentially show how 
+			expensive the options contracts are.
+	
+	<h2>formulas</h2>
+	
+		[ 
+			for every contract,
+			for every call,
+			for every put,
+			for every call at an expiration,
+			for every put at an expiration,			
+		]
+			summation (contract price * break even * open interest * shares per contract)
+			---
+			summation (contract price * open interest * shares per contract) 
 
-		<b>description</b>
-			<b>aggregates the break even value</b>
-			
+	<h2>description</h2>
+		<b>aggregates the break even value</b>
+		
 			
 </pre>
```

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/stats/aggregate_break_even/show/__init__.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/stats/aggregate_break_even/show/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/stats/aggregate_multiplier/aggregate_multipliers.r.HTML` & `rollercoaster-2.1.2/venues/stages/rollercoaster/stats/aggregate_multiplier/aggregate_multipliers.r.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/stats/stats.s.HTML` & `rollercoaster-2.1.2/venues/stages/rollercoaster/stats/stats.s.HTML`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,20 @@
 	<h2>best</h2>
 		
 		
 	<h2>relevant</h2>
 		https://optionstrat.com/
 	
 	<h2>itinerary, ranked</h2>
-		1:
+		
+		multiplier:
+			
+		
+		
+		option priceyness
 			The distance between the nearest 2 call 
 			option prices and the break even prices
 			at the options contracts last expiration.
 			
 			The distance between the nearest 2 put 
 			option prices and the break even prices
 			at the options contracts last expiration.
```

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/commodities/commodities.s.HTML` & `rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/commodities/commodities.s.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/options/movement_calculator/__init__.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/options/movement_calculator/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/options/movement_calculator/slope.s.HTML` & `rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/options/movement_calculator/slope.s.HTML`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/options/shapes/shape_1/__init__.py` & `rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/options/shapes/shape_1/__init__.py`

 * *Files identical despite different names*

### Comparing `rollercoaster-2.1.1/venues/stages/rollercoaster/treasures/shares/ETF/ETF.s.HTML` & `rollercoaster-2.1.2/venues/stages/rollercoaster/treasures/shares/ETF/ETF.s.HTML`

 * *Files identical despite different names*

