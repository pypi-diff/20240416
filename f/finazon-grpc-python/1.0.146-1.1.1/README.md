# Comparing `tmp/finazon_grpc_python-1.0.146.tar.gz` & `tmp/finazon_grpc_python-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finazon_grpc_python-1.0.146.tar", max compression
+gzip compressed data, was "finazon_grpc_python-1.1.1.tar", max compression
```

## Comparing `finazon_grpc_python-1.0.146.tar` & `finazon_grpc_python-1.1.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0     1064 2024-04-12 09:26:00.781227 finazon_grpc_python-1.0.146/LICENSE.txt
--rw-r--r--   0        0        0    13306 2024-04-12 09:26:01.001277 finazon_grpc_python-1.0.146/README.md
--rw-r--r--   0        0        0        0 2024-04-12 09:26:00.781227 finazon_grpc_python-1.0.146/finazon_grpc_python/__init__.py
--rw-r--r--   0        0        0     2030 2024-04-12 09:27:56.758993 finazon_grpc_python-1.0.146/finazon_grpc_python/api_usage_pb2.py
--rw-r--r--   0        0        0     2776 2024-04-12 09:27:56.758993 finazon_grpc_python-1.0.146/finazon_grpc_python/api_usage_pb2.pyi
--rw-r--r--   0        0        0     2715 2024-04-12 09:27:56.758993 finazon_grpc_python-1.0.146/finazon_grpc_python/api_usage_pb2_grpc.py
--rw-r--r--   0        0        0      504 2024-04-12 09:27:56.559063 finazon_grpc_python-1.0.146/finazon_grpc_python/api_usage_service.py
--rw-r--r--   0        0        0     9732 2024-04-12 09:27:56.758993 finazon_grpc_python-1.0.146/finazon_grpc_python/benzinga_pb2.py
--rw-r--r--   0        0        0    26705 2024-04-12 09:27:56.758993 finazon_grpc_python-1.0.146/finazon_grpc_python/benzinga_pb2.pyi
--rw-r--r--   0        0        0     7871 2024-04-12 09:27:56.758993 finazon_grpc_python-1.0.146/finazon_grpc_python/benzinga_pb2_grpc.py
--rw-r--r--   0        0        0     1175 2024-04-12 09:27:56.399119 finazon_grpc_python-1.0.146/finazon_grpc_python/benzinga_service.py
--rw-r--r--   0        0        0     2485 2024-04-12 09:27:56.758993 finazon_grpc_python-1.0.146/finazon_grpc_python/binance_pb2.py
--rw-r--r--   0        0        0     3890 2024-04-12 09:27:56.758993 finazon_grpc_python-1.0.146/finazon_grpc_python/binance_pb2.pyi
--rw-r--r--   0        0        0     2769 2024-04-12 09:27:56.758993 finazon_grpc_python-1.0.146/finazon_grpc_python/binance_pb2_grpc.py
--rw-r--r--   0        0        0      537 2024-04-12 09:27:56.539070 finazon_grpc_python-1.0.146/finazon_grpc_python/binance_service.py
--rw-r--r--   0        0        0        0 2024-04-12 09:26:00.785228 finazon_grpc_python-1.0.146/finazon_grpc_python/common/__init__.py
--rw-r--r--   0        0        0     1786 2024-04-12 09:26:00.785228 finazon_grpc_python-1.0.146/finazon_grpc_python/common/client.py
--rw-r--r--   0        0        0      496 2024-04-12 09:26:00.785228 finazon_grpc_python-1.0.146/finazon_grpc_python/common/errors.py
--rw-r--r--   0        0        0      177 2024-04-12 09:26:01.037285 finazon_grpc_python-1.0.146/finazon_grpc_python/common/settings.py
--rw-r--r--   0        0        0     1966 2024-04-12 09:26:00.785228 finazon_grpc_python-1.0.146/finazon_grpc_python/common/utils.py
--rw-r--r--   0        0        0     2254 2024-04-12 09:27:56.758993 finazon_grpc_python-1.0.146/finazon_grpc_python/crypto_pb2.py
--rw-r--r--   0        0        0     3113 2024-04-12 09:27:56.758993 finazon_grpc_python-1.0.146/finazon_grpc_python/crypto_pb2.pyi
--rw-r--r--   0        0        0     2737 2024-04-12 09:27:56.758993 finazon_grpc_python-1.0.146/finazon_grpc_python/crypto_pb2_grpc.py
--rw-r--r--   0        0        0      528 2024-04-12 09:27:56.551066 finazon_grpc_python-1.0.146/finazon_grpc_python/crypto_service.py
--rw-r--r--   0        0        0     1820 2024-04-12 09:27:56.758993 finazon_grpc_python-1.0.146/finazon_grpc_python/datasets_pb2.py
--rw-r--r--   0        0        0     2040 2024-04-12 09:27:56.758993 finazon_grpc_python-1.0.146/finazon_grpc_python/datasets_pb2.pyi
--rw-r--r--   0        0        0     2718 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/datasets_pb2_grpc.py
--rw-r--r--   0        0        0      501 2024-04-12 09:27:56.563061 finazon_grpc_python-1.0.146/finazon_grpc_python/datasets_service.py
--rw-r--r--   0        0        0        0 2024-04-12 09:26:00.785228 finazon_grpc_python-1.0.146/finazon_grpc_python/examples/__init__.py
--rw-r--r--   0        0        0      627 2024-04-12 09:26:00.785228 finazon_grpc_python-1.0.146/finazon_grpc_python/examples/indicator_atr.py
--rw-r--r--   0        0        0      598 2024-04-12 09:26:00.785228 finazon_grpc_python-1.0.146/finazon_grpc_python/examples/indicator_ma.py
--rw-r--r--   0        0        0      689 2024-04-12 09:26:00.785228 finazon_grpc_python-1.0.146/finazon_grpc_python/examples/indicator_ma_pandas.py
--rw-r--r--   0        0        0      489 2024-04-12 09:26:00.785228 finazon_grpc_python-1.0.146/finazon_grpc_python/examples/tickers.py
--rw-r--r--   0        0        0      635 2024-04-12 09:26:00.785228 finazon_grpc_python-1.0.146/finazon_grpc_python/examples/time_series.py
--rw-r--r--   0        0        0      619 2024-04-12 09:26:00.785228 finazon_grpc_python-1.0.146/finazon_grpc_python/examples/time_series_pandas.py
--rw-r--r--   0        0        0     2823 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/exchange_pb2.py
--rw-r--r--   0        0        0     4268 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/exchange_pb2.pyi
--rw-r--r--   0        0        0     4553 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/exchange_pb2_grpc.py
--rw-r--r--   0        0        0      771 2024-04-12 09:27:56.451100 finazon_grpc_python-1.0.146/finazon_grpc_python/exchange_service.py
--rw-r--r--   0        0        0     2210 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/forex_pb2.py
--rw-r--r--   0        0        0     2978 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/forex_pb2.pyi
--rw-r--r--   0        0        0     2713 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/forex_pb2_grpc.py
--rw-r--r--   0        0        0      519 2024-04-12 09:27:56.375127 finazon_grpc_python-1.0.146/finazon_grpc_python/forex_service.py
--rw-r--r--   0        0        0     1838 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/publishers_pb2.py
--rw-r--r--   0        0        0     2062 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/publishers_pb2.pyi
--rw-r--r--   0        0        0     2778 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/publishers_pb2_grpc.py
--rw-r--r--   0        0        0      520 2024-04-12 09:27:56.571058 finazon_grpc_python-1.0.146/finazon_grpc_python/publishers_service.py
--rw-r--r--   0        0        0     2667 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/sec_pb2.py
--rw-r--r--   0        0        0     5038 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/sec_pb2.pyi
--rw-r--r--   0        0        0     2711 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/sec_pb2_grpc.py
--rw-r--r--   0        0        0      486 2024-04-12 09:27:56.543068 finazon_grpc_python-1.0.146/finazon_grpc_python/sec_service.py
--rw-r--r--   0        0        0     3205 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/sip_pb2.py
--rw-r--r--   0        0        0     5780 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/sip_pb2.pyi
--rw-r--r--   0        0        0     4372 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/sip_pb2_grpc.py
--rw-r--r--   0        0        0      716 2024-04-12 09:27:56.411115 finazon_grpc_python-1.0.146/finazon_grpc_python/sip_service.py
--rw-r--r--   0        0        0     3662 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/snapshot_pb2.py
--rw-r--r--   0        0        0     7564 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/snapshot_pb2.pyi
--rw-r--r--   0        0        0     2822 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/snapshot_pb2_grpc.py
--rw-r--r--   0        0        0      501 2024-04-12 09:27:56.531072 finazon_grpc_python-1.0.146/finazon_grpc_python/snapshot_service.py
--rw-r--r--   0        0        0     5454 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/tickers_pb2.py
--rw-r--r--   0        0        0    11586 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/tickers_pb2.pyi
--rw-r--r--   0        0        0     8214 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/tickers_pb2_grpc.py
--rw-r--r--   0        0        0     1223 2024-04-12 09:27:56.439105 finazon_grpc_python-1.0.146/finazon_grpc_python/tickers_service.py
--rw-r--r--   0        0        0    11805 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/time_series_pb2.py
--rw-r--r--   0        0        0    27027 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/time_series_pb2.pyi
--rw-r--r--   0        0        0    19109 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/time_series_pb2_grpc.py
--rw-r--r--   0        0        0     2765 2024-04-12 09:27:56.527074 finazon_grpc_python-1.0.146/finazon_grpc_python/time_series_service.py
--rw-r--r--   0        0        0     2415 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/trade_pb2.py
--rw-r--r--   0        0        0     4127 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/trade_pb2.pyi
--rw-r--r--   0        0        0     2630 2024-04-12 09:27:56.762991 finazon_grpc_python-1.0.146/finazon_grpc_python/trade_pb2_grpc.py
--rw-r--r--   0        0        0      474 2024-04-12 09:27:56.459098 finazon_grpc_python-1.0.146/finazon_grpc_python/trade_service.py
--rw-r--r--   0        0        0      815 2024-04-12 09:26:01.037285 finazon_grpc_python-1.0.146/pyproject.toml
--rw-r--r--   0        0        0      443 2024-04-12 09:26:00.789229 finazon_grpc_python-1.0.146/requirements.txt
--rw-r--r--   0        0        0    14200 1970-01-01 00:00:00.000000 finazon_grpc_python-1.0.146/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-15 16:11:48.767794 finazon_grpc_python-1.1.1/LICENSE.txt
+-rw-r--r--   0        0        0    13306 2024-04-15 16:11:48.959802 finazon_grpc_python-1.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 16:11:48.767794 finazon_grpc_python-1.1.1/finazon_grpc_python/__init__.py
+-rw-r--r--   0        0        0     2030 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/api_usage_pb2.py
+-rw-r--r--   0        0        0     2776 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/api_usage_pb2.pyi
+-rw-r--r--   0        0        0     2715 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/api_usage_pb2_grpc.py
+-rw-r--r--   0        0        0      504 2024-04-15 16:12:10.080680 finazon_grpc_python-1.1.1/finazon_grpc_python/api_usage_service.py
+-rw-r--r--   0        0        0     9732 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/benzinga_pb2.py
+-rw-r--r--   0        0        0    26705 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/benzinga_pb2.pyi
+-rw-r--r--   0        0        0     7871 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/benzinga_pb2_grpc.py
+-rw-r--r--   0        0        0     1175 2024-04-15 16:12:09.968675 finazon_grpc_python-1.1.1/finazon_grpc_python/benzinga_service.py
+-rw-r--r--   0        0        0     2485 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/binance_pb2.py
+-rw-r--r--   0        0        0     3890 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/binance_pb2.pyi
+-rw-r--r--   0        0        0     2769 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/binance_pb2_grpc.py
+-rw-r--r--   0        0        0      537 2024-04-15 16:12:10.064679 finazon_grpc_python-1.1.1/finazon_grpc_python/binance_service.py
+-rw-r--r--   0        0        0        0 2024-04-15 16:11:48.767794 finazon_grpc_python-1.1.1/finazon_grpc_python/common/__init__.py
+-rw-r--r--   0        0        0     1786 2024-04-15 16:11:48.767794 finazon_grpc_python-1.1.1/finazon_grpc_python/common/client.py
+-rw-r--r--   0        0        0      496 2024-04-15 16:11:48.771794 finazon_grpc_python-1.1.1/finazon_grpc_python/common/errors.py
+-rw-r--r--   0        0        0      177 2024-04-15 16:11:48.975802 finazon_grpc_python-1.1.1/finazon_grpc_python/common/settings.py
+-rw-r--r--   0        0        0     1966 2024-04-15 16:11:48.771794 finazon_grpc_python-1.1.1/finazon_grpc_python/common/utils.py
+-rw-r--r--   0        0        0     2254 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/crypto_pb2.py
+-rw-r--r--   0        0        0     3113 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/crypto_pb2.pyi
+-rw-r--r--   0        0        0     2737 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/crypto_pb2_grpc.py
+-rw-r--r--   0        0        0      528 2024-04-15 16:12:10.076680 finazon_grpc_python-1.1.1/finazon_grpc_python/crypto_service.py
+-rw-r--r--   0        0        0     1820 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/datasets_pb2.py
+-rw-r--r--   0        0        0     2040 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/datasets_pb2.pyi
+-rw-r--r--   0        0        0     2718 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/datasets_pb2_grpc.py
+-rw-r--r--   0        0        0      501 2024-04-15 16:12:10.084680 finazon_grpc_python-1.1.1/finazon_grpc_python/datasets_service.py
+-rw-r--r--   0        0        0        0 2024-04-15 16:11:48.771794 finazon_grpc_python-1.1.1/finazon_grpc_python/examples/__init__.py
+-rw-r--r--   0        0        0      627 2024-04-15 16:11:48.771794 finazon_grpc_python-1.1.1/finazon_grpc_python/examples/indicator_atr.py
+-rw-r--r--   0        0        0      598 2024-04-15 16:11:48.771794 finazon_grpc_python-1.1.1/finazon_grpc_python/examples/indicator_ma.py
+-rw-r--r--   0        0        0      689 2024-04-15 16:11:48.771794 finazon_grpc_python-1.1.1/finazon_grpc_python/examples/indicator_ma_pandas.py
+-rw-r--r--   0        0        0      489 2024-04-15 16:11:48.771794 finazon_grpc_python-1.1.1/finazon_grpc_python/examples/tickers.py
+-rw-r--r--   0        0        0      635 2024-04-15 16:11:48.771794 finazon_grpc_python-1.1.1/finazon_grpc_python/examples/time_series.py
+-rw-r--r--   0        0        0      619 2024-04-15 16:11:48.771794 finazon_grpc_python-1.1.1/finazon_grpc_python/examples/time_series_pandas.py
+-rw-r--r--   0        0        0     2823 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/exchange_pb2.py
+-rw-r--r--   0        0        0     4268 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/exchange_pb2.pyi
+-rw-r--r--   0        0        0     4553 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/exchange_pb2_grpc.py
+-rw-r--r--   0        0        0      771 2024-04-15 16:12:10.000677 finazon_grpc_python-1.1.1/finazon_grpc_python/exchange_service.py
+-rw-r--r--   0        0        0     2210 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/forex_pb2.py
+-rw-r--r--   0        0        0     2978 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/forex_pb2.pyi
+-rw-r--r--   0        0        0     2713 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/forex_pb2_grpc.py
+-rw-r--r--   0        0        0      519 2024-04-15 16:12:09.952675 finazon_grpc_python-1.1.1/finazon_grpc_python/forex_service.py
+-rw-r--r--   0        0        0     1838 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/publishers_pb2.py
+-rw-r--r--   0        0        0     2062 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/publishers_pb2.pyi
+-rw-r--r--   0        0        0     2778 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/publishers_pb2_grpc.py
+-rw-r--r--   0        0        0      520 2024-04-15 16:12:10.092681 finazon_grpc_python-1.1.1/finazon_grpc_python/publishers_service.py
+-rw-r--r--   0        0        0     2667 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/sec_pb2.py
+-rw-r--r--   0        0        0     5038 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/sec_pb2.pyi
+-rw-r--r--   0        0        0     2711 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/sec_pb2_grpc.py
+-rw-r--r--   0        0        0      486 2024-04-15 16:12:10.068679 finazon_grpc_python-1.1.1/finazon_grpc_python/sec_service.py
+-rw-r--r--   0        0        0     3205 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/sip_pb2.py
+-rw-r--r--   0        0        0     5780 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/sip_pb2.pyi
+-rw-r--r--   0        0        0     4372 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/sip_pb2_grpc.py
+-rw-r--r--   0        0        0      716 2024-04-15 16:12:09.976676 finazon_grpc_python-1.1.1/finazon_grpc_python/sip_service.py
+-rw-r--r--   0        0        0     3662 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/snapshot_pb2.py
+-rw-r--r--   0        0        0     7564 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/snapshot_pb2.pyi
+-rw-r--r--   0        0        0     2822 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/snapshot_pb2_grpc.py
+-rw-r--r--   0        0        0      501 2024-04-15 16:12:10.060679 finazon_grpc_python-1.1.1/finazon_grpc_python/snapshot_service.py
+-rw-r--r--   0        0        0     5454 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/tickers_pb2.py
+-rw-r--r--   0        0        0    11586 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/tickers_pb2.pyi
+-rw-r--r--   0        0        0     8214 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/tickers_pb2_grpc.py
+-rw-r--r--   0        0        0     1223 2024-04-15 16:12:09.992676 finazon_grpc_python-1.1.1/finazon_grpc_python/tickers_service.py
+-rw-r--r--   0        0        0    11805 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/time_series_pb2.py
+-rw-r--r--   0        0        0    27027 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/time_series_pb2.pyi
+-rw-r--r--   0        0        0    19109 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/time_series_pb2_grpc.py
+-rw-r--r--   0        0        0     2765 2024-04-15 16:12:10.052679 finazon_grpc_python-1.1.1/finazon_grpc_python/time_series_service.py
+-rw-r--r--   0        0        0     2415 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/trade_pb2.py
+-rw-r--r--   0        0        0     4127 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/trade_pb2.pyi
+-rw-r--r--   0        0        0     2630 2024-04-15 16:12:10.220686 finazon_grpc_python-1.1.1/finazon_grpc_python/trade_pb2_grpc.py
+-rw-r--r--   0        0        0      474 2024-04-15 16:12:10.004677 finazon_grpc_python-1.1.1/finazon_grpc_python/trade_service.py
+-rw-r--r--   0        0        0      813 2024-04-15 16:11:48.975802 finazon_grpc_python-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      443 2024-04-15 16:11:48.775794 finazon_grpc_python-1.1.1/requirements.txt
+-rw-r--r--   0        0        0    14198 1970-01-01 00:00:00.000000 finazon_grpc_python-1.1.1/PKG-INFO
```

### Comparing `finazon_grpc_python-1.0.146/LICENSE.txt` & `finazon_grpc_python-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/README.md` & `finazon_grpc_python-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/api_usage_pb2.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/api_usage_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/api_usage_pb2.pyi` & `finazon_grpc_python-1.1.1/finazon_grpc_python/api_usage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/api_usage_pb2_grpc.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/api_usage_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/benzinga_pb2.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/benzinga_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/benzinga_pb2.pyi` & `finazon_grpc_python-1.1.1/finazon_grpc_python/benzinga_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/benzinga_pb2_grpc.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/benzinga_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/benzinga_service.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/benzinga_service.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/binance_pb2.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/binance_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/binance_pb2.pyi` & `finazon_grpc_python-1.1.1/finazon_grpc_python/binance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/binance_pb2_grpc.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/binance_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/binance_service.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/binance_service.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/common/client.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/common/client.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/common/utils.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/common/utils.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/crypto_pb2.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/crypto_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/crypto_pb2.pyi` & `finazon_grpc_python-1.1.1/finazon_grpc_python/crypto_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/crypto_pb2_grpc.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/crypto_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/crypto_service.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/crypto_service.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/datasets_pb2.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/datasets_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/datasets_pb2.pyi` & `finazon_grpc_python-1.1.1/finazon_grpc_python/datasets_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/datasets_pb2_grpc.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/datasets_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/examples/indicator_atr.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/examples/indicator_atr.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/examples/indicator_ma.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/examples/indicator_ma.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/examples/indicator_ma_pandas.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/examples/indicator_ma_pandas.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/examples/time_series.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/examples/time_series.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/examples/time_series_pandas.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/examples/time_series_pandas.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/exchange_pb2.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/exchange_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/exchange_pb2.pyi` & `finazon_grpc_python-1.1.1/finazon_grpc_python/exchange_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/exchange_pb2_grpc.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/exchange_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/exchange_service.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/exchange_service.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/forex_pb2.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/forex_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/forex_pb2.pyi` & `finazon_grpc_python-1.1.1/finazon_grpc_python/forex_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/forex_pb2_grpc.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/forex_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/forex_service.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/forex_service.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/publishers_pb2.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/publishers_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/publishers_pb2.pyi` & `finazon_grpc_python-1.1.1/finazon_grpc_python/publishers_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/publishers_pb2_grpc.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/publishers_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/publishers_service.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/publishers_service.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/sec_pb2.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/sec_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/sec_pb2.pyi` & `finazon_grpc_python-1.1.1/finazon_grpc_python/sec_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/sec_pb2_grpc.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/sec_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/sip_pb2.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/sip_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/sip_pb2.pyi` & `finazon_grpc_python-1.1.1/finazon_grpc_python/sip_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/sip_pb2_grpc.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/sip_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/sip_service.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/sip_service.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/snapshot_pb2.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/snapshot_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/snapshot_pb2.pyi` & `finazon_grpc_python-1.1.1/finazon_grpc_python/snapshot_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/snapshot_pb2_grpc.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/snapshot_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/tickers_pb2.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/tickers_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/tickers_pb2.pyi` & `finazon_grpc_python-1.1.1/finazon_grpc_python/tickers_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/tickers_pb2_grpc.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/tickers_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/tickers_service.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/tickers_service.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/time_series_pb2.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/time_series_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/time_series_pb2.pyi` & `finazon_grpc_python-1.1.1/finazon_grpc_python/time_series_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/time_series_pb2_grpc.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/time_series_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/time_series_service.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/time_series_service.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/trade_pb2.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/trade_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/trade_pb2.pyi` & `finazon_grpc_python-1.1.1/finazon_grpc_python/trade_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/finazon_grpc_python/trade_pb2_grpc.py` & `finazon_grpc_python-1.1.1/finazon_grpc_python/trade_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.0.146/pyproject.toml` & `finazon_grpc_python-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "finazon-grpc-python"
 packages = [{include = "finazon_grpc_python"}]
 include = ["requirements.txt", "finazon_grpc_python/*.p*"]
-version = "1.0.146"
+version = "1.1.1"
 description = "Finazon gRPC client library for Python"
 authors = ["Finazon <team@finazon.io>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/finazon-io/finazon-grpc-python"
 repository = "https://github.com/finazon-io/finazon-grpc-python"
```

### Comparing `finazon_grpc_python-1.0.146/PKG-INFO` & `finazon_grpc_python-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finazon-grpc-python
-Version: 1.0.146
+Version: 1.1.1
 Summary: Finazon gRPC client library for Python
 Home-page: https://github.com/finazon-io/finazon-grpc-python
 License: MIT
 Author: Finazon
 Author-email: team@finazon.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

