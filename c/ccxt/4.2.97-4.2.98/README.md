# Comparing `tmp/ccxt-4.2.97.tar.gz` & `tmp/ccxt-4.2.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ccxt-4.2.97.tar", last modified: Sun Apr 14 21:23:18 2024, max compression
+gzip compressed data, was "dist/ccxt-4.2.98.tar", last modified: Mon Apr 15 10:26:09 2024, max compression
```

## Comparing `ccxt-4.2.97.tar` & `ccxt-4.2.98.tar`

### file list

```diff
@@ -1,572 +1,572 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-14 21:23:18.413836 ccxt-4.2.97/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1068 2024-04-14 21:21:59.000000 ccxt-4.2.97/LICENSE.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      101 2024-04-14 20:49:57.000000 ccxt-4.2.97/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)   114404 2024-04-14 21:23:18.417836 ccxt-4.2.97/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)   102253 2024-04-14 20:49:57.000000 ccxt-4.2.97/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-14 21:23:18.029798 ccxt-4.2.97/ccxt/
--rw-rw-r--   0 travis    (2000) travis    (2000)    15656 2024-04-14 21:21:57.000000 ccxt-4.2.97/ccxt/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-14 21:23:18.109806 ccxt-4.2.97/ccxt/abstract/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/abstract/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1448 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/ace.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10382 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/alpaca.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11394 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/ascendex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/bequant.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4895 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/bigone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    91867 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/binance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    91867 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/binancecoinm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    98587 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/binanceus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    91867 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/binanceusdm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15876 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/bingx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2830 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/bit2c.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2735 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/bitbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5820 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/bitbay.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4082 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/bitbns.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/bitcoincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7605 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/bitfinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19194 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/bitfinex2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3576 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/bitflyer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    89841 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/bitget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3443 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/bithumb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14031 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/bitmart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10774 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/bitmex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3295 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/bitopro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3859 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/bitpanda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9379 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/bitrue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4025 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/bitso.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27930 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/bitstamp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3478 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/bitteam.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/bitvavo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2024 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/bl3p.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2638 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/blockchaincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3978 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/blofin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1380 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/btcalpha.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      849 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/btcbox.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3690 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/btcmarkets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1777 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/btcturk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48599 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/bybit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3311 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/cex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14574 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/coinbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4770 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/coinbaseinternational.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7162 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/coinbasepro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3417 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/coincheck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34678 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/coinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6538 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/coinlist.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6842 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/coinmate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3864 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/coinmetro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8291 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/coinone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8007 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/coinsph.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2707 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/coinspot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18475 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/cryptocom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7563 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/currencycom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5107 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/delta.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15499 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/deribit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11452 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/digifinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6177 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/exmo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/fmfwio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41994 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/gate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41994 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/gateio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6915 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/gemini.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/hitbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/hitbtc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2906 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/hollaex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    99311 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/htx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    99311 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/huobi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14331 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/huobijp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      240 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/hyperliquid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2129 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/idex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4165 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/independentreserve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2488 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/indodax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5877 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/kraken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3537 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/krakenfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25491 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/kucoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27937 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/kucoinfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24579 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/kuna.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7168 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/latoken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8675 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/lbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3373 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/luno.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2960 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/lykke.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/mercado.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25902 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/mexc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11878 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/ndax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3093 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/novadax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1721 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/oceanex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9414 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/okcoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45891 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/okx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3859 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/onetrading.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2054 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/p2b.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2843 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/paymium.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15203 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/phemex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8073 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/poloniex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5219 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/poloniexfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1969 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/probit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5875 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/timex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4094 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/tokocrypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1372 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/tradeogre.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3576 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/upbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19631 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/wavesexchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2782 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/wazirx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8029 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/whitebit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10216 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/woo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1339 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/yobit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3935 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/zaif.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5820 2024-04-14 20:52:00.000000 ccxt-4.2.97/ccxt/abstract/zonda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41420 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/ace.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46908 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/alpaca.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   151300 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/ascendex.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-14 21:23:18.245819 ccxt-4.2.97/ccxt/async_support/
--rw-rw-r--   0 travis    (2000) travis    (2000)    15409 2024-04-14 21:21:57.000000 ccxt-4.2.97/ccxt/async_support/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41644 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/ace.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    47120 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/alpaca.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   152088 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/ascendex.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-14 21:23:18.249820 ccxt-4.2.97/ccxt/async_support/base/
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/base/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    91521 2024-04-14 21:21:57.000000 ccxt-4.2.97/ccxt/async_support/base/exchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1847 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/base/throttler.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-14 21:23:18.253820 ccxt-4.2.97/ccxt/async_support/base/ws/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1791 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/base/ws/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5751 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/base/ws/aiohttp_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8100 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/base/ws/cache.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7289 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/base/ws/client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3864 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/base/ws/fast_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1499 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/base/ws/functions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2067 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/base/ws/future.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2894 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/base/ws/order_book.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6478 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/base/ws/order_book_side.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1188 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/bequant.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92639 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/bigone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   599554 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/binance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1683 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/binancecoinm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9177 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/binanceus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2518 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/binanceusdm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   182980 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/bingx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37113 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/bit2c.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41949 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/bitbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      492 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/bitbay.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48385 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/bitbns.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      516 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/bitcoincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    71968 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/bitfinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   158863 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/bitfinex2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41694 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/bitflyer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   414840 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/bitget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45564 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/bithumb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   200023 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/bitmart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   125968 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/bitmex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68685 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/bitopro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      485 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/bitpanda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   136831 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/bitrue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    71115 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/bitso.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92615 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/bitstamp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   102163 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/bitteam.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    91855 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/bitvavo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20460 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/bl3p.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    49180 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/blockchaincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    99698 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/blofin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36828 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/btcalpha.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23535 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/btcbox.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51678 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/btcmarkets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36724 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/btcturk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   403379 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/bybit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    70003 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/cex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   202728 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/coinbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    87677 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/coinbaseinternational.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    78883 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/coinbasepro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35719 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/coincheck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   248412 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/coinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   103489 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/coinlist.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46056 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/coinmate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    80729 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/coinmetro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46987 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/coinone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    90866 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/coinsph.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23615 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/coinspot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   128712 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/cryptocom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    87181 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/currencycom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   151045 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/delta.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   161224 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/deribit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   168841 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/digifinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   114835 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/exmo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1183 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/flowbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1250 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/fmfwio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   316838 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/gate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      459 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/gateio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    81127 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/gemini.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   153853 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/hitbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      469 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/hitbtc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    76327 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/hollaex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   421631 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/htx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      452 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/huobi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    88457 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/huobijp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92896 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/hyperliquid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    73285 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/idex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    32284 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/independentreserve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    52087 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/indodax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   124519 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/kraken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   116143 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/krakenfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   215759 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/kucoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   119121 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/kucoinfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    96396 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/kuna.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    79256 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/latoken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   115876 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/lbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45981 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/luno.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51143 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/lykke.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35425 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/mercado.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   237552 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/mexc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   108892 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/ndax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    64473 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/novadax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    38180 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/oceanex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   151629 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/okcoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   356176 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/okx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    88409 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/onetrading.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    54316 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/p2b.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24391 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/paymium.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   219437 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/phemex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   102496 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/poloniex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    77991 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/poloniexfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    76600 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/probit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    71498 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/timex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   123364 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/tokocrypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23955 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/tradeogre.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    82082 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/upbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   113950 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/wavesexchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51493 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/wazirx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   101482 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/whitebit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   132574 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/woo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    53350 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/yobit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28134 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/zaif.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    80866 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/async_support/zonda.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-14 21:23:18.257820 ccxt-4.2.97/ccxt/base/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1320 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/base/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6634 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/base/decimal_to_precision.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4107 2024-04-14 21:05:39.000000 ccxt-4.2.97/ccxt/base/errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   256006 2024-04-14 21:21:57.000000 ccxt-4.2.97/ccxt/base/exchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8565 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/base/precise.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7903 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/base/types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1174 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/bequant.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92185 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/bigone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   596976 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/binance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1645 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/binancecoinm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9163 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/binanceus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2480 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/binanceusdm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   181968 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/bingx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36901 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/bit2c.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41689 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/bitbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      478 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/bitbay.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48131 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/bitbns.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      502 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/bitcoincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    71528 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/bitfinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   158129 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/bitfinex2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41386 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/bitflyer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   413270 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/bitget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45334 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/bithumb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   199103 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/bitmart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   125408 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/bitmex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68281 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/bitopro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      471 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/bitpanda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   136173 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/bitrue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    70729 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/bitso.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92115 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/bitstamp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   101831 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/bitteam.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    91421 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/bitvavo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20332 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/bl3p.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48788 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/blockchaincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    99114 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/blofin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36550 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/btcalpha.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23341 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/btcbox.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51328 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/btcmarkets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36506 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/btcturk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   401635 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/bybit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    69653 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/cex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   201676 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/coinbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    87123 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/coinbaseinternational.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    78377 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/coinbasepro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35513 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/coincheck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   247142 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/coinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   103001 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/coinlist.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45790 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/coinmate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    80409 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/coinmetro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46745 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/coinone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    90432 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/coinsph.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23463 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/coinspot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   128158 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/cryptocom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    86759 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/currencycom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   150437 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/delta.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   160448 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/deribit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   167871 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/digifinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   114203 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/exmo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1169 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/flowbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1236 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/fmfwio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   315184 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/gate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      445 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/gateio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    80614 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/gemini.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   152807 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/hitbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      455 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/hitbtc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    75893 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/hollaex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   419293 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/htx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      438 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/huobi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    87957 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/huobijp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92412 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/hyperliquid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    72809 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/idex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    32024 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/independentreserve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51779 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/indodax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   123935 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/kraken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   115673 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/krakenfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   214705 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/kucoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   118519 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/kucoinfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    95980 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/kuna.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    78780 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/latoken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   115164 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/lbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45643 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/luno.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    50829 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/lykke.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35183 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/mercado.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   236392 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/mexc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   108368 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/ndax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    64105 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/novadax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37860 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/oceanex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   151105 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/okcoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   354715 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/okx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    87957 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/onetrading.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    54074 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/p2b.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24203 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/paymium.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   218625 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/phemex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   101948 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/poloniex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    77605 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/poloniexfutures.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-14 21:23:18.313826 ccxt-4.2.97/ccxt/pro/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6999 2024-04-14 21:21:57.000000 ccxt-4.2.97/ccxt/pro/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27167 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/alpaca.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35432 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/ascendex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1351 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/bequant.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   136683 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/binance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      976 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/binancecoinm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2321 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/binanceus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1357 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/binanceusdm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42110 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/bingx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1181 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/bitcoincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24826 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/bitfinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42744 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/bitfinex2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    71862 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/bitget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16799 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/bithumb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    62382 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/bitmart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68956 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/bitmex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18724 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/bitopro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      415 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/bitpanda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16448 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/bitrue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20886 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/bitstamp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    56143 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/bitvavo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29560 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/blockchaincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    75022 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/bybit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    58370 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/cex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24508 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/coinbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25428 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/coinbaseinternational.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    38945 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/coinbasepro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7789 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/coincheck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45042 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/coinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15652 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/coinone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42643 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/cryptocom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22355 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/currencycom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41035 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/deribit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24527 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/exmo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    52489 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/gate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      391 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/gateio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36641 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/gemini.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    56285 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/hitbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21957 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/hollaex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    95779 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/htx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      385 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/huobi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23174 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/huobijp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20613 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/hyperliquid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28282 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/idex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11063 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/independentreserve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    60657 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/kraken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    63917 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/krakenfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    50705 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/kucoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46006 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/kucoinfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35100 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/lbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12348 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/luno.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42551 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/mexc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22643 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/ndax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30385 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/okcoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68821 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/okx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    54634 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/onetrading.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17877 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/p2b.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    61032 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/phemex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51236 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/poloniex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41652 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/poloniexfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22822 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/probit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9654 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/upbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30004 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/wazirx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35021 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/whitebit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37022 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/pro/woo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    76208 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/probit.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-14 21:23:18.313826 ccxt-4.2.97/ccxt/static_dependencies/
--rw-rw-r--   0 travis    (2000) travis    (2000)       84 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-14 21:23:18.321827 ccxt-4.2.97/ccxt/static_dependencies/ecdsa/
--rw-rw-r--   0 travis    (2000) travis    (2000)      594 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ecdsa/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18461 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ecdsa/_version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1886 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ecdsa/curves.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6942 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ecdsa/der.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11336 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ecdsa/ecdsa.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5517 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ecdsa/ellipticcurve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14201 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ecdsa/keys.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13468 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ecdsa/numbertheory.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2572 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ecdsa/rfc6979.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10037 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ecdsa/util.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-14 21:23:18.321827 ccxt-4.2.97/ccxt/static_dependencies/ethereum/
--rw-rw-r--   0 travis    (2000) travis    (2000)      171 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-14 21:23:18.329827 ccxt-4.2.97/ccxt/static_dependencies/ethereum/abi/
--rw-rw-r--   0 travis    (2000) travis    (2000)      276 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/abi/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      490 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/abi/abi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4861 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/abi/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6871 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/abi/codec.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       51 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/abi/constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16828 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/abi/decoding.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20162 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/abi/encoding.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2941 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/abi/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12358 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/abi/grammar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      387 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/abi/packed.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/abi/py.typed
--rw-rw-r--   0 travis    (2000) travis    (2000)    19329 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/abi/registry.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-14 21:23:18.333828 ccxt-4.2.97/ccxt/static_dependencies/ethereum/abi/tools/
--rw-rw-r--   0 travis    (2000) travis    (2000)       65 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/abi/tools/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5742 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/abi/tools/_strategies.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-14 21:23:18.333828 ccxt-4.2.97/ccxt/static_dependencies/ethereum/abi/utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/abi/utils/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2097 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/abi/utils/numeric.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      426 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/abi/utils/padding.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      436 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/abi/utils/string.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-14 21:23:18.337828 ccxt-4.2.97/ccxt/static_dependencies/ethereum/account/
--rw-rw-r--   0 travis    (2000) travis    (2000)       48 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/account/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-14 21:23:18.341828 ccxt-4.2.97/ccxt/static_dependencies/ethereum/account/encode_typed_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)       80 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/account/encode_typed_data/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7126 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/account/encode_typed_data/encoding_and_hashing.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      982 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/account/encode_typed_data/helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10588 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/account/messages.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/account/py.typed
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-14 21:23:18.341828 ccxt-4.2.97/ccxt/static_dependencies/ethereum/hexbytes/
--rw-rw-r--   0 travis    (2000) travis    (2000)       60 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/hexbytes/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1687 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/hexbytes/_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1768 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/hexbytes/main.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/hexbytes/py.typed
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-14 21:23:18.349829 ccxt-4.2.97/ccxt/static_dependencies/ethereum/typing/
--rw-rw-r--   0 travis    (2000) travis    (2000)      913 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/typing/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       85 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/typing/abi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      191 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/typing/bls.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       71 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/typing/discovery.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      117 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/typing/encoding.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      458 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/typing/enums.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      173 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/typing/ethpm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      546 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/typing/evm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20845 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/typing/networks.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/typing/py.typed
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-14 21:23:18.365831 ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2162 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2123 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/abi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4364 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/address.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4342 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/applicators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5498 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/conversions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3021 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/currency.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-14 21:23:18.365831 ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/curried/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6398 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/curried/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      499 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/debug.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3997 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/decorators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      199 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/encoding.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      110 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2100 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/functional.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1826 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/hexadecimal.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4137 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/humanize.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5155 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/logging.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      842 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/module_loading.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1190 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/numeric.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/py.typed
--rw-rw-r--   0 travis    (2000) travis    (2000)     1001 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/toolz.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1074 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/types.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-14 21:23:18.365831 ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/typing/
--rw-rw-r--   0 travis    (2000) travis    (2000)      325 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/typing/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      189 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/typing/misc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1757 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/units.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-14 21:23:18.369831 ccxt-4.2.97/ccxt/static_dependencies/keccak/
--rw-rw-r--   0 travis    (2000) travis    (2000)       45 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/keccak/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6934 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/keccak/keccak.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-14 21:23:18.369831 ccxt-4.2.97/ccxt/static_dependencies/msgpack/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1077 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/msgpack/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1081 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/msgpack/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5629 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/msgpack/ext.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    33175 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/msgpack/fallback.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-14 21:23:18.373832 ccxt-4.2.97/ccxt/static_dependencies/parsimonious/
--rw-rw-r--   0 travis    (2000) travis    (2000)      385 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/parsimonious/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3603 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/parsimonious/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16864 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/parsimonious/expressions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19190 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/parsimonious/grammar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13084 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/parsimonious/nodes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1087 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/parsimonious/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-14 21:23:18.381832 ccxt-4.2.97/ccxt/static_dependencies/toolz/
--rw-rw-r--   0 travis    (2000) travis    (2000)      374 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/toolz/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20555 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/toolz/_signatures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18447 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/toolz/_version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      997 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/toolz/compatibility.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-14 21:23:18.385833 ccxt-4.2.97/ccxt/static_dependencies/toolz/curried/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2226 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/toolz/curried/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      344 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/toolz/curried/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      525 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/toolz/curried/operator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8955 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/toolz/dicttoolz.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29821 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/toolz/functoolz.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27612 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/toolz/itertoolz.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1256 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/toolz/recipes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      139 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/static_dependencies/toolz/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-14 21:23:18.385833 ccxt-4.2.97/ccxt/test/
--rw-rw-r--   0 travis    (2000) travis    (2000)      141 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/test/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-14 21:23:18.413836 ccxt-4.2.97/ccxt/test/base/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1889 2024-04-14 21:05:43.000000 ccxt-4.2.97/ccxt/test/base/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      978 2024-04-14 21:07:09.000000 ccxt-4.2.97/ccxt/test/base/test_account.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2931 2024-04-14 21:07:09.000000 ccxt-4.2.97/ccxt/test/base/test_balance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1808 2024-04-14 21:07:09.000000 ccxt-4.2.97/ccxt/test/base/test_borrow_interest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1500 2024-04-14 21:07:09.000000 ccxt-4.2.97/ccxt/test/base/test_borrow_rate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1177 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/test/base/test_calculate_fee.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7702 2024-04-14 21:05:41.000000 ccxt-4.2.97/ccxt/test/base/test_crypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4472 2024-04-14 21:07:09.000000 ccxt-4.2.97/ccxt/test/base/test_currency.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5235 2024-04-14 21:05:40.000000 ccxt-4.2.97/ccxt/test/base/test_datetime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20934 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/test/base/test_decimal_to_precision.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1402 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/test/base/test_deep_extend.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2452 2024-04-14 21:07:09.000000 ccxt-4.2.97/ccxt/test/base/test_deposit_withdrawal.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3592 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/test/base/test_exchange_datetime_functions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1351 2024-04-14 21:07:09.000000 ccxt-4.2.97/ccxt/test/base/test_funding_rate_history.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1332 2024-04-14 21:07:09.000000 ccxt-4.2.97/ccxt/test/base/test_last_price.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2283 2024-04-14 21:07:09.000000 ccxt-4.2.97/ccxt/test/base/test_ledger_entry.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2154 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/test/base/test_ledger_item.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1656 2024-04-14 21:07:09.000000 ccxt-4.2.97/ccxt/test/base/test_leverage_tier.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      869 2024-04-14 21:07:09.000000 ccxt-4.2.97/ccxt/test/base/test_margin_mode.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1730 2024-04-14 21:07:09.000000 ccxt-4.2.97/ccxt/test/base/test_margin_modification.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11632 2024-04-14 21:07:09.000000 ccxt-4.2.97/ccxt/test/base/test_market.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22083 2024-04-14 21:05:40.000000 ccxt-4.2.97/ccxt/test/base/test_number.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2036 2024-04-14 21:07:09.000000 ccxt-4.2.97/ccxt/test/base/test_ohlcv.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1547 2024-04-14 21:07:09.000000 ccxt-4.2.97/ccxt/test/base/test_open_interest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3964 2024-04-14 21:07:09.000000 ccxt-4.2.97/ccxt/test/base/test_order.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3949 2024-04-14 21:07:09.000000 ccxt-4.2.97/ccxt/test/base/test_order_book.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3884 2024-04-14 21:07:09.000000 ccxt-4.2.97/ccxt/test/base/test_position.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19998 2024-04-14 21:07:09.000000 ccxt-4.2.97/ccxt/test/base/test_shared_methods.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      722 2024-04-14 21:07:09.000000 ccxt-4.2.97/ccxt/test/base/test_status.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3123 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/test/base/test_throttle.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5810 2024-04-14 21:07:09.000000 ccxt-4.2.97/ccxt/test/base/test_ticker.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2336 2024-04-14 21:07:09.000000 ccxt-4.2.97/ccxt/test/base/test_trade.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1066 2024-04-14 21:07:09.000000 ccxt-4.2.97/ccxt/test/base/test_trading_fee.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1434 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/test/base/test_transaction.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    78570 2024-04-14 21:05:43.000000 ccxt-4.2.97/ccxt/test/test_async.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    77551 2024-04-14 21:05:43.000000 ccxt-4.2.97/ccxt/test/test_sync.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    71136 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/timex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   123002 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/tokocrypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23761 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/tradeogre.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    81600 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/upbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   113400 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/wavesexchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51191 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/wazirx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   100934 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/whitebit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   131756 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/woo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    53066 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/yobit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27952 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/zaif.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    80552 2024-04-14 20:49:57.000000 ccxt-4.2.97/ccxt/zonda.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-14 21:23:18.033799 ccxt-4.2.97/ccxt.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)   114404 2024-04-14 21:23:17.000000 ccxt-4.2.97/ccxt.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    15741 2024-04-14 21:23:17.000000 ccxt-4.2.97/ccxt.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-14 21:23:17.000000 ccxt-4.2.97/ccxt.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      218 2024-04-14 21:23:17.000000 ccxt-4.2.97/ccxt.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        5 2024-04-14 21:23:17.000000 ccxt-4.2.97/ccxt.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    12515 2024-04-14 21:21:58.000000 ccxt-4.2.97/package.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      205 2024-04-14 21:23:18.421836 ccxt-4.2.97/setup.cfg
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3071 2024-04-14 20:49:57.000000 ccxt-4.2.97/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-15 10:26:09.438033 ccxt-4.2.98/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1068 2024-04-15 10:21:20.000000 ccxt-4.2.98/LICENSE.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      101 2024-04-15 08:56:01.000000 ccxt-4.2.98/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)   114404 2024-04-15 10:26:09.438033 ccxt-4.2.98/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)   102253 2024-04-15 08:56:01.000000 ccxt-4.2.98/README.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-15 10:26:08.685967 ccxt-4.2.98/ccxt/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15656 2024-04-15 10:21:15.000000 ccxt-4.2.98/ccxt/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-15 10:26:08.821979 ccxt-4.2.98/ccxt/abstract/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-15 08:56:01.000000 ccxt-4.2.98/ccxt/abstract/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1448 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/ace.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10382 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/alpaca.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11394 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/ascendex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/bequant.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4895 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/bigone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    91867 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/binance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    91867 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/binancecoinm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    98587 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/binanceus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    91867 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/binanceusdm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15876 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/bingx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2830 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/bit2c.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2735 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/bitbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5820 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/bitbay.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4082 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/bitbns.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/bitcoincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7605 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/bitfinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19194 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/bitfinex2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3576 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/bitflyer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    89841 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/bitget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3443 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/bithumb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14031 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/bitmart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10774 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/bitmex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3295 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/bitopro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3859 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/bitpanda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9379 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/bitrue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4025 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/bitso.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27930 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/bitstamp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3478 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/bitteam.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/bitvavo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2024 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/bl3p.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2638 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/blockchaincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3978 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/blofin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1380 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/btcalpha.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      849 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/btcbox.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3690 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/btcmarkets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1777 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/btcturk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48599 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/bybit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3311 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/cex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14574 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/coinbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4770 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/coinbaseinternational.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7162 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/coinbasepro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3417 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/coincheck.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34678 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/coinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6538 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/coinlist.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6842 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/coinmate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3864 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/coinmetro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8291 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/coinone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8007 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/coinsph.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2707 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/coinspot.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18475 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/cryptocom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7563 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/currencycom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5107 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/delta.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15499 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/deribit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11452 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/digifinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6177 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/exmo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/fmfwio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41994 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/gate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41994 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/gateio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6915 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/gemini.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/hitbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/hitbtc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2906 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/hollaex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    99311 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/htx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    99311 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/huobi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14331 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/huobijp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      240 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/hyperliquid.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2129 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/idex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4165 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/independentreserve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2488 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/indodax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5877 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/kraken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3537 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/krakenfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25491 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/kucoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27937 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/kucoinfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24579 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/kuna.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7168 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/latoken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8675 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/lbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3373 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/luno.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2960 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/lykke.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/mercado.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25902 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/mexc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11878 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/ndax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3093 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/novadax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1721 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/oceanex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9414 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/okcoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45891 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/okx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3859 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/onetrading.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2054 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/p2b.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2843 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/paymium.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15203 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/phemex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8073 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/poloniex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5219 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/poloniexfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1969 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/probit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5875 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/timex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4094 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/tokocrypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1372 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/tradeogre.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3576 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/upbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19631 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/wavesexchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2782 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/wazirx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8029 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/whitebit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10216 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/woo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1339 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/yobit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3935 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/zaif.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5820 2024-04-15 08:57:55.000000 ccxt-4.2.98/ccxt/abstract/zonda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41420 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/ace.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46908 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/alpaca.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   151300 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/ascendex.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-15 10:26:09.066001 ccxt-4.2.98/ccxt/async_support/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15409 2024-04-15 10:21:15.000000 ccxt-4.2.98/ccxt/async_support/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41644 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/ace.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    47120 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/alpaca.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   152088 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/ascendex.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-15 10:26:09.066001 ccxt-4.2.98/ccxt/async_support/base/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       67 2024-04-15 08:56:01.000000 ccxt-4.2.98/ccxt/async_support/base/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    91521 2024-04-15 10:21:15.000000 ccxt-4.2.98/ccxt/async_support/base/exchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1847 2024-04-15 08:56:01.000000 ccxt-4.2.98/ccxt/async_support/base/throttler.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-15 10:26:09.074001 ccxt-4.2.98/ccxt/async_support/base/ws/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1791 2024-04-15 08:56:01.000000 ccxt-4.2.98/ccxt/async_support/base/ws/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5751 2024-04-15 08:56:01.000000 ccxt-4.2.98/ccxt/async_support/base/ws/aiohttp_client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8100 2024-04-15 08:56:01.000000 ccxt-4.2.98/ccxt/async_support/base/ws/cache.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7289 2024-04-15 08:56:01.000000 ccxt-4.2.98/ccxt/async_support/base/ws/client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3864 2024-04-15 08:56:01.000000 ccxt-4.2.98/ccxt/async_support/base/ws/fast_client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1499 2024-04-15 08:56:01.000000 ccxt-4.2.98/ccxt/async_support/base/ws/functions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2067 2024-04-15 08:56:01.000000 ccxt-4.2.98/ccxt/async_support/base/ws/future.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2894 2024-04-15 08:56:01.000000 ccxt-4.2.98/ccxt/async_support/base/ws/order_book.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6478 2024-04-15 08:56:01.000000 ccxt-4.2.98/ccxt/async_support/base/ws/order_book_side.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1188 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/bequant.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92639 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/bigone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   599554 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/binance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1683 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/binancecoinm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9177 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/binanceus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2518 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/binanceusdm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   182980 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/bingx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37113 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/bit2c.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41949 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/bitbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      492 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/bitbay.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48385 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/bitbns.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      516 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/bitcoincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    71968 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/bitfinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   158863 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/bitfinex2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41694 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/bitflyer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   414840 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/bitget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45564 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/bithumb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   200023 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/bitmart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   125968 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/bitmex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    68685 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/bitopro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      485 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/bitpanda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   136831 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/bitrue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    71115 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/bitso.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92615 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/bitstamp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   102163 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/bitteam.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    91855 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/bitvavo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20460 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/bl3p.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    49180 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/blockchaincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    99698 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/blofin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36828 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/btcalpha.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23535 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/btcbox.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51678 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/btcmarkets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36724 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/btcturk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   403379 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/bybit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    70003 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/cex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   202728 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/coinbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87677 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/coinbaseinternational.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    78883 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/coinbasepro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35719 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/coincheck.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   248412 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/coinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   103489 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/coinlist.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46056 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/coinmate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    80729 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/coinmetro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46987 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/coinone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    90866 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/coinsph.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23615 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/coinspot.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   128712 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/cryptocom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87181 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/currencycom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   151045 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/delta.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   161224 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/deribit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   168841 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/digifinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   114835 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/exmo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1183 2024-04-15 08:56:01.000000 ccxt-4.2.98/ccxt/async_support/flowbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1250 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/fmfwio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   316838 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/gate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      459 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/gateio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    81127 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/gemini.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   153853 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/hitbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      469 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/hitbtc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    76327 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/hollaex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   421631 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/htx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      452 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/huobi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    88457 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/huobijp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92896 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/hyperliquid.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    73285 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/idex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    32284 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/independentreserve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    52087 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/indodax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   124519 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/kraken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   116143 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/krakenfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   215759 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/kucoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   119121 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/kucoinfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    96396 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/kuna.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    79256 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/latoken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   115876 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/lbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45981 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/luno.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51143 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/lykke.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35425 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/mercado.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   237552 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/mexc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   108892 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/ndax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    64473 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/novadax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    38180 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/oceanex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   151629 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/okcoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   356176 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/okx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    88409 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/onetrading.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    54316 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/p2b.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24391 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/paymium.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   219437 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/phemex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   102496 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/poloniex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    77991 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/poloniexfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    76600 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/probit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    71498 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/timex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   123364 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/tokocrypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23955 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/tradeogre.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    82082 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/upbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   113950 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/wavesexchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51493 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/wazirx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   101482 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/whitebit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   132574 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/woo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    53350 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/yobit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28134 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/zaif.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    80866 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/async_support/zonda.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-15 10:26:09.078002 ccxt-4.2.98/ccxt/base/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1320 2024-04-15 08:56:01.000000 ccxt-4.2.98/ccxt/base/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6634 2024-04-15 08:56:01.000000 ccxt-4.2.98/ccxt/base/decimal_to_precision.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4107 2024-04-15 09:11:01.000000 ccxt-4.2.98/ccxt/base/errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   256006 2024-04-15 10:21:15.000000 ccxt-4.2.98/ccxt/base/exchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8565 2024-04-15 08:56:01.000000 ccxt-4.2.98/ccxt/base/precise.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7903 2024-04-15 08:56:01.000000 ccxt-4.2.98/ccxt/base/types.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1174 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/bequant.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92185 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/bigone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   596976 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/binance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1645 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/binancecoinm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9163 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/binanceus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2480 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/binanceusdm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   181968 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/bingx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36901 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/bit2c.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41689 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/bitbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      478 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/bitbay.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48131 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/bitbns.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      502 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/bitcoincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    71528 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/bitfinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   158129 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/bitfinex2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41386 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/bitflyer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   413270 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/bitget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45334 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/bithumb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   199103 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/bitmart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   125408 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/bitmex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    68281 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/bitopro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      471 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/bitpanda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   136173 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/bitrue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    70729 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/bitso.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92115 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/bitstamp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   101831 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/bitteam.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    91421 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/bitvavo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20332 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/bl3p.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48788 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/blockchaincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    99114 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/blofin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36550 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/btcalpha.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23341 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/btcbox.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51328 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/btcmarkets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36506 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/btcturk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   401635 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/bybit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    69653 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/cex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   201676 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/coinbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87123 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/coinbaseinternational.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    78377 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/coinbasepro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35513 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/coincheck.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   247142 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/coinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   103001 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/coinlist.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45790 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/coinmate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    80409 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/coinmetro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46745 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/coinone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    90432 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/coinsph.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23463 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/coinspot.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   128158 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/cryptocom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    86759 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/currencycom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   150437 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/delta.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   160448 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/deribit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   167871 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/digifinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   114203 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/exmo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1169 2024-04-15 08:56:01.000000 ccxt-4.2.98/ccxt/flowbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1236 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/fmfwio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   315184 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/gate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      445 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/gateio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    80614 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/gemini.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   152807 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/hitbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      455 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/hitbtc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    75893 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/hollaex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   419293 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/htx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      438 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/huobi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87957 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/huobijp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92412 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/hyperliquid.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    72809 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/idex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    32024 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/independentreserve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51779 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/indodax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   123935 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/kraken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   115673 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/krakenfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   214705 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/kucoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   118519 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/kucoinfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    95980 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/kuna.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    78780 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/latoken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   115164 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/lbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45643 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/luno.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    50829 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/lykke.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35183 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/mercado.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   236392 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/mexc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   108368 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/ndax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    64105 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/novadax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37860 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/oceanex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   151105 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/okcoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   354715 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/okx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87957 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/onetrading.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    54074 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/p2b.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24203 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/paymium.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   218625 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/phemex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   101948 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/poloniex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    77605 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/poloniexfutures.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-15 10:26:09.222015 ccxt-4.2.98/ccxt/pro/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6999 2024-04-15 10:21:15.000000 ccxt-4.2.98/ccxt/pro/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27167 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/alpaca.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35432 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/ascendex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1351 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/bequant.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   136683 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/binance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      976 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/binancecoinm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2321 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/binanceus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1357 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/binanceusdm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42110 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/bingx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1181 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/bitcoincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24826 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/bitfinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42744 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/bitfinex2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    71862 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/bitget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16799 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/bithumb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    62382 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/bitmart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    68956 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/bitmex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18724 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/bitopro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      415 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/bitpanda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16448 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/bitrue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20886 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/bitstamp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    56143 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/bitvavo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29560 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/blockchaincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    75022 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/bybit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    58370 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/cex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24508 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/coinbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25428 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/coinbaseinternational.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    38945 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/coinbasepro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7789 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/coincheck.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45042 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/coinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15652 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/coinone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42643 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/cryptocom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22355 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/currencycom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41035 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/deribit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24527 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/exmo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    52489 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/gate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      391 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/gateio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36641 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/gemini.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    56285 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/hitbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21957 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/hollaex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    95779 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/htx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      385 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/huobi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23174 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/huobijp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20613 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/hyperliquid.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28282 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/idex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11063 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/independentreserve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    60657 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/kraken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    63917 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/krakenfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    50705 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/kucoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46006 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/kucoinfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35100 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/lbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12348 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/luno.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42551 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/mexc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22643 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/ndax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30385 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/okcoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    68821 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/okx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    54634 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/onetrading.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17877 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/p2b.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    61032 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/phemex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51236 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/poloniex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41652 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/poloniexfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22822 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/probit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9654 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/upbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30004 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/wazirx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35021 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/whitebit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37022 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/pro/woo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    76208 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/probit.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-15 10:26:09.222015 ccxt-4.2.98/ccxt/static_dependencies/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       84 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-15 10:26:09.242016 ccxt-4.2.98/ccxt/static_dependencies/ecdsa/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      594 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ecdsa/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18461 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ecdsa/_version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1886 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ecdsa/curves.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6942 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ecdsa/der.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11336 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ecdsa/ecdsa.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5517 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ecdsa/ellipticcurve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14201 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ecdsa/keys.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13468 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ecdsa/numbertheory.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2572 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ecdsa/rfc6979.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10037 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ecdsa/util.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-15 10:26:09.242016 ccxt-4.2.98/ccxt/static_dependencies/ethereum/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      171 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-15 10:26:09.258018 ccxt-4.2.98/ccxt/static_dependencies/ethereum/abi/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      276 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/abi/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      490 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/abi/abi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4861 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/abi/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6871 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/abi/codec.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       51 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/abi/constants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16828 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/abi/decoding.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20162 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/abi/encoding.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2941 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/abi/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12358 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/abi/grammar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      387 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/abi/packed.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/abi/py.typed
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19329 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/abi/registry.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-15 10:26:09.262018 ccxt-4.2.98/ccxt/static_dependencies/ethereum/abi/tools/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       65 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/abi/tools/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5742 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/abi/tools/_strategies.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-15 10:26:09.270019 ccxt-4.2.98/ccxt/static_dependencies/ethereum/abi/utils/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/abi/utils/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2097 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/abi/utils/numeric.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      426 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/abi/utils/padding.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      436 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/abi/utils/string.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-15 10:26:09.278019 ccxt-4.2.98/ccxt/static_dependencies/ethereum/account/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       48 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/account/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-15 10:26:09.282020 ccxt-4.2.98/ccxt/static_dependencies/ethereum/account/encode_typed_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       80 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/account/encode_typed_data/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7126 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/account/encode_typed_data/encoding_and_hashing.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      982 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/account/encode_typed_data/helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10588 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/account/messages.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/account/py.typed
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-15 10:26:09.298021 ccxt-4.2.98/ccxt/static_dependencies/ethereum/hexbytes/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       60 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/hexbytes/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1687 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/hexbytes/_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1768 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/hexbytes/main.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/hexbytes/py.typed
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-15 10:26:09.310022 ccxt-4.2.98/ccxt/static_dependencies/ethereum/typing/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      913 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/typing/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       85 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/typing/abi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      191 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/typing/bls.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       71 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/typing/discovery.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      117 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/typing/encoding.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      458 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/typing/enums.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      173 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/typing/ethpm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      546 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/typing/evm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20845 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/typing/networks.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/typing/py.typed
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-15 10:26:09.346025 ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2162 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2123 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/abi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4364 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/address.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4342 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/applicators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5498 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/conversions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3021 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/currency.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-15 10:26:09.346025 ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/curried/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6398 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/curried/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      499 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/debug.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3997 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/decorators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      199 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/encoding.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      110 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2100 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/functional.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1826 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/hexadecimal.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4137 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/humanize.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5155 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/logging.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      842 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/module_loading.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1190 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/numeric.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/py.typed
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1001 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/toolz.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1074 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/types.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-15 10:26:09.350026 ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/typing/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      325 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/typing/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      189 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/typing/misc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1757 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/units.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-15 10:26:09.350026 ccxt-4.2.98/ccxt/static_dependencies/keccak/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       45 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/keccak/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6934 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/keccak/keccak.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-15 10:26:09.354026 ccxt-4.2.98/ccxt/static_dependencies/msgpack/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1077 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/msgpack/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1081 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/msgpack/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5629 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/msgpack/ext.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    33175 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/msgpack/fallback.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-15 10:26:09.366027 ccxt-4.2.98/ccxt/static_dependencies/parsimonious/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      385 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/parsimonious/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3603 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/parsimonious/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16864 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/parsimonious/expressions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19190 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/parsimonious/grammar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13084 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/parsimonious/nodes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1087 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/parsimonious/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-15 10:26:09.374028 ccxt-4.2.98/ccxt/static_dependencies/toolz/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      374 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/toolz/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20555 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/toolz/_signatures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18447 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/toolz/_version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      997 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/toolz/compatibility.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-15 10:26:09.374028 ccxt-4.2.98/ccxt/static_dependencies/toolz/curried/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2226 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/toolz/curried/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      344 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/toolz/curried/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      525 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/toolz/curried/operator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8955 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/toolz/dicttoolz.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29821 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/toolz/functoolz.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27612 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/toolz/itertoolz.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1256 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/toolz/recipes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      139 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/static_dependencies/toolz/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-15 10:26:09.378028 ccxt-4.2.98/ccxt/test/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      141 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/test/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-15 10:26:09.434033 ccxt-4.2.98/ccxt/test/base/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1889 2024-04-15 09:11:06.000000 ccxt-4.2.98/ccxt/test/base/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      978 2024-04-15 09:12:30.000000 ccxt-4.2.98/ccxt/test/base/test_account.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2931 2024-04-15 09:12:30.000000 ccxt-4.2.98/ccxt/test/base/test_balance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1808 2024-04-15 09:12:30.000000 ccxt-4.2.98/ccxt/test/base/test_borrow_interest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1500 2024-04-15 09:12:30.000000 ccxt-4.2.98/ccxt/test/base/test_borrow_rate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1177 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/test/base/test_calculate_fee.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7702 2024-04-15 09:11:03.000000 ccxt-4.2.98/ccxt/test/base/test_crypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4472 2024-04-15 09:12:30.000000 ccxt-4.2.98/ccxt/test/base/test_currency.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5235 2024-04-15 09:11:02.000000 ccxt-4.2.98/ccxt/test/base/test_datetime.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20934 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/test/base/test_decimal_to_precision.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1402 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/test/base/test_deep_extend.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2452 2024-04-15 09:12:30.000000 ccxt-4.2.98/ccxt/test/base/test_deposit_withdrawal.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3592 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/test/base/test_exchange_datetime_functions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1351 2024-04-15 09:12:30.000000 ccxt-4.2.98/ccxt/test/base/test_funding_rate_history.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1332 2024-04-15 09:12:30.000000 ccxt-4.2.98/ccxt/test/base/test_last_price.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2283 2024-04-15 09:12:30.000000 ccxt-4.2.98/ccxt/test/base/test_ledger_entry.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2154 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/test/base/test_ledger_item.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1656 2024-04-15 09:12:30.000000 ccxt-4.2.98/ccxt/test/base/test_leverage_tier.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      869 2024-04-15 09:12:30.000000 ccxt-4.2.98/ccxt/test/base/test_margin_mode.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1730 2024-04-15 09:12:30.000000 ccxt-4.2.98/ccxt/test/base/test_margin_modification.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11632 2024-04-15 09:12:30.000000 ccxt-4.2.98/ccxt/test/base/test_market.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22083 2024-04-15 09:11:02.000000 ccxt-4.2.98/ccxt/test/base/test_number.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2036 2024-04-15 09:12:30.000000 ccxt-4.2.98/ccxt/test/base/test_ohlcv.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1547 2024-04-15 09:12:30.000000 ccxt-4.2.98/ccxt/test/base/test_open_interest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3964 2024-04-15 09:12:30.000000 ccxt-4.2.98/ccxt/test/base/test_order.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3949 2024-04-15 09:12:30.000000 ccxt-4.2.98/ccxt/test/base/test_order_book.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3884 2024-04-15 09:12:30.000000 ccxt-4.2.98/ccxt/test/base/test_position.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19998 2024-04-15 09:12:30.000000 ccxt-4.2.98/ccxt/test/base/test_shared_methods.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      722 2024-04-15 09:12:30.000000 ccxt-4.2.98/ccxt/test/base/test_status.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3123 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/test/base/test_throttle.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5810 2024-04-15 09:12:30.000000 ccxt-4.2.98/ccxt/test/base/test_ticker.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2336 2024-04-15 09:12:30.000000 ccxt-4.2.98/ccxt/test/base/test_trade.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1066 2024-04-15 09:12:30.000000 ccxt-4.2.98/ccxt/test/base/test_trading_fee.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1434 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/test/base/test_transaction.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    78570 2024-04-15 09:11:06.000000 ccxt-4.2.98/ccxt/test/test_async.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    77551 2024-04-15 09:11:06.000000 ccxt-4.2.98/ccxt/test/test_sync.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    71136 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/timex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   123002 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/tokocrypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23761 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/tradeogre.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    81600 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/upbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   113400 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/wavesexchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51191 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/wazirx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   100934 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/whitebit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   131756 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/woo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    53066 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/yobit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27952 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/zaif.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    80552 2024-04-15 08:56:02.000000 ccxt-4.2.98/ccxt/zonda.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-15 10:26:08.689967 ccxt-4.2.98/ccxt.egg-info/
+-rw-r--r--   0 travis    (2000) travis    (2000)   114404 2024-04-15 10:26:07.000000 ccxt-4.2.98/ccxt.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15741 2024-04-15 10:26:08.000000 ccxt-4.2.98/ccxt.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-15 10:26:07.000000 ccxt-4.2.98/ccxt.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      218 2024-04-15 10:26:07.000000 ccxt-4.2.98/ccxt.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        5 2024-04-15 10:26:07.000000 ccxt-4.2.98/ccxt.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12515 2024-04-15 10:21:18.000000 ccxt-4.2.98/package.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      205 2024-04-15 10:26:09.450035 ccxt-4.2.98/setup.cfg
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3071 2024-04-15 08:56:02.000000 ccxt-4.2.98/setup.py
```

### Comparing `ccxt-4.2.97/LICENSE.txt` & `ccxt-4.2.98/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/PKG-INFO` & `ccxt-4.2.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccxt
-Version: 4.2.97
+Version: 4.2.98
 Summary: A JavaScript / TypeScript / Python / C# / PHP cryptocurrency trading library with support for 100+ exchanges
 Home-page: https://ccxt.com
 Author: Igor Kroitor
 Author-email: igor.kroitor@gmail.com
 License: MIT
 Project-URL: Homepage, https://ccxt.com
 Project-URL: Documentation, https://github.com/ccxt/ccxt/wiki
@@ -221,21 +221,21 @@
         console.log(version, Object.keys(exchanges));
         ```
         
         ### JavaScript (for use with the `<script>` tag):
         
         All-in-one browser bundle (dependencies included), served from a CDN of your choice:
         
-        * jsDelivr: https://cdn.jsdelivr.net/npm/ccxt@4.2.97/dist/ccxt.browser.js
-        * unpkg: https://unpkg.com/ccxt@4.2.97/dist/ccxt.browser.js
+        * jsDelivr: https://cdn.jsdelivr.net/npm/ccxt@4.2.98/dist/ccxt.browser.js
+        * unpkg: https://unpkg.com/ccxt@4.2.98/dist/ccxt.browser.js
         
         CDNs are not updated in real-time and may have delays. Defaulting to the most recent version without specifying the version number is not recommended. Please, keep in mind that we are not responsible for the correct operation of those CDN servers.
         
         ```HTML
-        <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ccxt@4.2.97/dist/ccxt.browser.js"></script>
+        <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ccxt@4.2.98/dist/ccxt.browser.js"></script>
         ```
         
         Creates a global `ccxt` object:
         
         ```JavaScript
         console.log (ccxt.exchanges) // print all available exchanges
         ```
```

### Comparing `ccxt-4.2.97/README.rst` & `ccxt-4.2.98/README.rst`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/__init__.py` & `ccxt-4.2.98/ccxt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 # ----------------------------------------------------------------------------
 
-__version__ = '4.2.97'
+__version__ = '4.2.98'
 
 # ----------------------------------------------------------------------------
 
 from ccxt.base.exchange import Exchange                     # noqa: F401
 from ccxt.base.precise import Precise                       # noqa: F401
 
 from ccxt.base.decimal_to_precision import decimal_to_precision  # noqa: F401
```

### Comparing `ccxt-4.2.97/ccxt/abstract/ace.py` & `ccxt-4.2.98/ccxt/abstract/ace.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/alpaca.py` & `ccxt-4.2.98/ccxt/abstract/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/ascendex.py` & `ccxt-4.2.98/ccxt/abstract/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/bequant.py` & `ccxt-4.2.98/ccxt/abstract/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/bigone.py` & `ccxt-4.2.98/ccxt/abstract/bigone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/binance.py` & `ccxt-4.2.98/ccxt/abstract/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/binancecoinm.py` & `ccxt-4.2.98/ccxt/abstract/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/binanceus.py` & `ccxt-4.2.98/ccxt/abstract/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/binanceusdm.py` & `ccxt-4.2.98/ccxt/abstract/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/bingx.py` & `ccxt-4.2.98/ccxt/abstract/bingx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/bit2c.py` & `ccxt-4.2.98/ccxt/abstract/bit2c.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/bitbank.py` & `ccxt-4.2.98/ccxt/abstract/bitbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/bitbay.py` & `ccxt-4.2.98/ccxt/abstract/bitbay.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/bitbns.py` & `ccxt-4.2.98/ccxt/abstract/bitbns.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/bitcoincom.py` & `ccxt-4.2.98/ccxt/abstract/bitcoincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/bitfinex.py` & `ccxt-4.2.98/ccxt/abstract/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/bitfinex2.py` & `ccxt-4.2.98/ccxt/abstract/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/bitflyer.py` & `ccxt-4.2.98/ccxt/abstract/bitflyer.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/bitget.py` & `ccxt-4.2.98/ccxt/abstract/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/bithumb.py` & `ccxt-4.2.98/ccxt/abstract/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/bitmart.py` & `ccxt-4.2.98/ccxt/abstract/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/bitmex.py` & `ccxt-4.2.98/ccxt/abstract/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/bitopro.py` & `ccxt-4.2.98/ccxt/abstract/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/bitpanda.py` & `ccxt-4.2.98/ccxt/abstract/bitpanda.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/bitrue.py` & `ccxt-4.2.98/ccxt/abstract/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/bitso.py` & `ccxt-4.2.98/ccxt/abstract/bitso.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/bitstamp.py` & `ccxt-4.2.98/ccxt/abstract/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/bitteam.py` & `ccxt-4.2.98/ccxt/abstract/bitteam.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/bitvavo.py` & `ccxt-4.2.98/ccxt/abstract/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/bl3p.py` & `ccxt-4.2.98/ccxt/abstract/bl3p.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/blockchaincom.py` & `ccxt-4.2.98/ccxt/abstract/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/blofin.py` & `ccxt-4.2.98/ccxt/abstract/blofin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/btcalpha.py` & `ccxt-4.2.98/ccxt/abstract/btcalpha.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/btcbox.py` & `ccxt-4.2.98/ccxt/abstract/btcbox.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/btcmarkets.py` & `ccxt-4.2.98/ccxt/abstract/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/btcturk.py` & `ccxt-4.2.98/ccxt/abstract/btcturk.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/bybit.py` & `ccxt-4.2.98/ccxt/abstract/bybit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/cex.py` & `ccxt-4.2.98/ccxt/abstract/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/coinbase.py` & `ccxt-4.2.98/ccxt/abstract/coinbase.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/coinbaseinternational.py` & `ccxt-4.2.98/ccxt/abstract/coinbaseinternational.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/coinbasepro.py` & `ccxt-4.2.98/ccxt/abstract/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/coincheck.py` & `ccxt-4.2.98/ccxt/abstract/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/coinex.py` & `ccxt-4.2.98/ccxt/abstract/coinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/coinlist.py` & `ccxt-4.2.98/ccxt/abstract/coinlist.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/coinmate.py` & `ccxt-4.2.98/ccxt/abstract/coinmate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/coinmetro.py` & `ccxt-4.2.98/ccxt/abstract/coinmetro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/coinone.py` & `ccxt-4.2.98/ccxt/abstract/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/coinsph.py` & `ccxt-4.2.98/ccxt/abstract/coinsph.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/coinspot.py` & `ccxt-4.2.98/ccxt/abstract/coinspot.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/cryptocom.py` & `ccxt-4.2.98/ccxt/abstract/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/currencycom.py` & `ccxt-4.2.98/ccxt/abstract/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/delta.py` & `ccxt-4.2.98/ccxt/abstract/delta.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/deribit.py` & `ccxt-4.2.98/ccxt/abstract/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/digifinex.py` & `ccxt-4.2.98/ccxt/abstract/digifinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/exmo.py` & `ccxt-4.2.98/ccxt/abstract/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/fmfwio.py` & `ccxt-4.2.98/ccxt/abstract/fmfwio.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/gate.py` & `ccxt-4.2.98/ccxt/abstract/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/gateio.py` & `ccxt-4.2.98/ccxt/abstract/gateio.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/gemini.py` & `ccxt-4.2.98/ccxt/abstract/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/hitbtc.py` & `ccxt-4.2.98/ccxt/abstract/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/hitbtc3.py` & `ccxt-4.2.98/ccxt/abstract/hitbtc3.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/hollaex.py` & `ccxt-4.2.98/ccxt/abstract/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/htx.py` & `ccxt-4.2.98/ccxt/abstract/htx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/huobi.py` & `ccxt-4.2.98/ccxt/abstract/huobi.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/huobijp.py` & `ccxt-4.2.98/ccxt/abstract/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/idex.py` & `ccxt-4.2.98/ccxt/abstract/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/independentreserve.py` & `ccxt-4.2.98/ccxt/abstract/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/indodax.py` & `ccxt-4.2.98/ccxt/abstract/indodax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/kraken.py` & `ccxt-4.2.98/ccxt/abstract/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/krakenfutures.py` & `ccxt-4.2.98/ccxt/abstract/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/kucoin.py` & `ccxt-4.2.98/ccxt/abstract/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/kucoinfutures.py` & `ccxt-4.2.98/ccxt/abstract/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/kuna.py` & `ccxt-4.2.98/ccxt/abstract/kuna.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/latoken.py` & `ccxt-4.2.98/ccxt/abstract/latoken.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/lbank.py` & `ccxt-4.2.98/ccxt/abstract/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/luno.py` & `ccxt-4.2.98/ccxt/abstract/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/lykke.py` & `ccxt-4.2.98/ccxt/abstract/lykke.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/mercado.py` & `ccxt-4.2.98/ccxt/abstract/mercado.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/mexc.py` & `ccxt-4.2.98/ccxt/abstract/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/ndax.py` & `ccxt-4.2.98/ccxt/abstract/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/novadax.py` & `ccxt-4.2.98/ccxt/abstract/novadax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/oceanex.py` & `ccxt-4.2.98/ccxt/abstract/oceanex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/okcoin.py` & `ccxt-4.2.98/ccxt/abstract/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/okx.py` & `ccxt-4.2.98/ccxt/abstract/okx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/onetrading.py` & `ccxt-4.2.98/ccxt/abstract/onetrading.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/p2b.py` & `ccxt-4.2.98/ccxt/abstract/p2b.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/paymium.py` & `ccxt-4.2.98/ccxt/abstract/paymium.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/phemex.py` & `ccxt-4.2.98/ccxt/abstract/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/poloniex.py` & `ccxt-4.2.98/ccxt/abstract/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/poloniexfutures.py` & `ccxt-4.2.98/ccxt/abstract/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/probit.py` & `ccxt-4.2.98/ccxt/abstract/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/timex.py` & `ccxt-4.2.98/ccxt/abstract/timex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/tokocrypto.py` & `ccxt-4.2.98/ccxt/abstract/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/tradeogre.py` & `ccxt-4.2.98/ccxt/abstract/tradeogre.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/upbit.py` & `ccxt-4.2.98/ccxt/abstract/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/wavesexchange.py` & `ccxt-4.2.98/ccxt/abstract/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/wazirx.py` & `ccxt-4.2.98/ccxt/abstract/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/whitebit.py` & `ccxt-4.2.98/ccxt/abstract/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/woo.py` & `ccxt-4.2.98/ccxt/abstract/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/yobit.py` & `ccxt-4.2.98/ccxt/abstract/yobit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/zaif.py` & `ccxt-4.2.98/ccxt/abstract/zaif.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/abstract/zonda.py` & `ccxt-4.2.98/ccxt/abstract/zonda.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/ace.py` & `ccxt-4.2.98/ccxt/ace.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/alpaca.py` & `ccxt-4.2.98/ccxt/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/ascendex.py` & `ccxt-4.2.98/ccxt/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/__init__.py` & `ccxt-4.2.98/ccxt/async_support/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """CCXT: CryptoCurrency eXchange Trading Library (Async)"""
 
 # -----------------------------------------------------------------------------
 
-__version__ = '4.2.97'
+__version__ = '4.2.98'
 
 # -----------------------------------------------------------------------------
 
 from ccxt.async_support.base.exchange import Exchange                   # noqa: F401
 
 from ccxt.base.decimal_to_precision import decimal_to_precision  # noqa: F401
 from ccxt.base.decimal_to_precision import TRUNCATE              # noqa: F401
```

### Comparing `ccxt-4.2.97/ccxt/async_support/ace.py` & `ccxt-4.2.98/ccxt/async_support/ace.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/alpaca.py` & `ccxt-4.2.98/ccxt/async_support/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/ascendex.py` & `ccxt-4.2.98/ccxt/async_support/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/base/exchange.py` & `ccxt-4.2.98/ccxt/async_support/base/exchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 # -----------------------------------------------------------------------------
 
-__version__ = '4.2.97'
+__version__ = '4.2.98'
 
 # -----------------------------------------------------------------------------
 
 import asyncio
 import concurrent.futures
 import socket
 import certifi
```

### Comparing `ccxt-4.2.97/ccxt/async_support/base/throttler.py` & `ccxt-4.2.98/ccxt/async_support/base/throttler.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/base/ws/__init__.py` & `ccxt-4.2.98/ccxt/async_support/base/ws/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/base/ws/aiohttp_client.py` & `ccxt-4.2.98/ccxt/async_support/base/ws/aiohttp_client.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/base/ws/cache.py` & `ccxt-4.2.98/ccxt/async_support/base/ws/cache.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/base/ws/client.py` & `ccxt-4.2.98/ccxt/async_support/base/ws/client.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/base/ws/fast_client.py` & `ccxt-4.2.98/ccxt/async_support/base/ws/fast_client.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/base/ws/functions.py` & `ccxt-4.2.98/ccxt/async_support/base/ws/functions.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/base/ws/future.py` & `ccxt-4.2.98/ccxt/async_support/base/ws/future.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/base/ws/order_book.py` & `ccxt-4.2.98/ccxt/async_support/base/ws/order_book.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/base/ws/order_book_side.py` & `ccxt-4.2.98/ccxt/async_support/base/ws/order_book_side.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/bequant.py` & `ccxt-4.2.98/ccxt/async_support/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/bigone.py` & `ccxt-4.2.98/ccxt/async_support/bigone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/binance.py` & `ccxt-4.2.98/ccxt/async_support/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/binancecoinm.py` & `ccxt-4.2.98/ccxt/async_support/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/binanceus.py` & `ccxt-4.2.98/ccxt/async_support/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/binanceusdm.py` & `ccxt-4.2.98/ccxt/async_support/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/bingx.py` & `ccxt-4.2.98/ccxt/async_support/bingx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/bit2c.py` & `ccxt-4.2.98/ccxt/async_support/bit2c.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/bitbank.py` & `ccxt-4.2.98/ccxt/async_support/bitbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/bitbns.py` & `ccxt-4.2.98/ccxt/async_support/bitbns.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/bitcoincom.py` & `ccxt-4.2.98/ccxt/async_support/bitcoincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/bitfinex.py` & `ccxt-4.2.98/ccxt/async_support/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/bitfinex2.py` & `ccxt-4.2.98/ccxt/async_support/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/bitflyer.py` & `ccxt-4.2.98/ccxt/async_support/bitflyer.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/bitget.py` & `ccxt-4.2.98/ccxt/async_support/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/bithumb.py` & `ccxt-4.2.98/ccxt/async_support/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/bitmart.py` & `ccxt-4.2.98/ccxt/async_support/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/bitmex.py` & `ccxt-4.2.98/ccxt/async_support/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/bitopro.py` & `ccxt-4.2.98/ccxt/async_support/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/bitrue.py` & `ccxt-4.2.98/ccxt/async_support/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/bitso.py` & `ccxt-4.2.98/ccxt/async_support/bitso.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/bitstamp.py` & `ccxt-4.2.98/ccxt/async_support/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/bitteam.py` & `ccxt-4.2.98/ccxt/async_support/bitteam.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/bitvavo.py` & `ccxt-4.2.98/ccxt/async_support/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/bl3p.py` & `ccxt-4.2.98/ccxt/async_support/bl3p.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/blockchaincom.py` & `ccxt-4.2.98/ccxt/async_support/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/blofin.py` & `ccxt-4.2.98/ccxt/async_support/blofin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/btcalpha.py` & `ccxt-4.2.98/ccxt/async_support/btcalpha.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/btcbox.py` & `ccxt-4.2.98/ccxt/async_support/btcbox.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/btcmarkets.py` & `ccxt-4.2.98/ccxt/async_support/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/btcturk.py` & `ccxt-4.2.98/ccxt/async_support/btcturk.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/bybit.py` & `ccxt-4.2.98/ccxt/async_support/bybit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/cex.py` & `ccxt-4.2.98/ccxt/async_support/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/coinbase.py` & `ccxt-4.2.98/ccxt/async_support/coinbase.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/coinbaseinternational.py` & `ccxt-4.2.98/ccxt/async_support/coinbaseinternational.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/coinbasepro.py` & `ccxt-4.2.98/ccxt/async_support/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/coincheck.py` & `ccxt-4.2.98/ccxt/async_support/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/coinex.py` & `ccxt-4.2.98/ccxt/async_support/coinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/coinlist.py` & `ccxt-4.2.98/ccxt/async_support/coinlist.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/coinmate.py` & `ccxt-4.2.98/ccxt/async_support/coinmate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/coinmetro.py` & `ccxt-4.2.98/ccxt/async_support/coinmetro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/coinone.py` & `ccxt-4.2.98/ccxt/async_support/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/coinsph.py` & `ccxt-4.2.98/ccxt/async_support/coinsph.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/coinspot.py` & `ccxt-4.2.98/ccxt/async_support/coinspot.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/cryptocom.py` & `ccxt-4.2.98/ccxt/async_support/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/currencycom.py` & `ccxt-4.2.98/ccxt/async_support/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/delta.py` & `ccxt-4.2.98/ccxt/async_support/delta.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/deribit.py` & `ccxt-4.2.98/ccxt/async_support/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/digifinex.py` & `ccxt-4.2.98/ccxt/async_support/digifinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/exmo.py` & `ccxt-4.2.98/ccxt/async_support/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/flowbtc.py` & `ccxt-4.2.98/ccxt/async_support/flowbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/fmfwio.py` & `ccxt-4.2.98/ccxt/async_support/fmfwio.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/gate.py` & `ccxt-4.2.98/ccxt/async_support/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/gemini.py` & `ccxt-4.2.98/ccxt/async_support/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/hitbtc.py` & `ccxt-4.2.98/ccxt/async_support/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/hollaex.py` & `ccxt-4.2.98/ccxt/async_support/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/htx.py` & `ccxt-4.2.98/ccxt/async_support/htx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/huobijp.py` & `ccxt-4.2.98/ccxt/async_support/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/hyperliquid.py` & `ccxt-4.2.98/ccxt/async_support/hyperliquid.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/idex.py` & `ccxt-4.2.98/ccxt/async_support/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/independentreserve.py` & `ccxt-4.2.98/ccxt/async_support/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/indodax.py` & `ccxt-4.2.98/ccxt/async_support/indodax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/kraken.py` & `ccxt-4.2.98/ccxt/async_support/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/krakenfutures.py` & `ccxt-4.2.98/ccxt/async_support/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/kucoin.py` & `ccxt-4.2.98/ccxt/async_support/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/kucoinfutures.py` & `ccxt-4.2.98/ccxt/async_support/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/kuna.py` & `ccxt-4.2.98/ccxt/async_support/kuna.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/latoken.py` & `ccxt-4.2.98/ccxt/async_support/latoken.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/lbank.py` & `ccxt-4.2.98/ccxt/async_support/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/luno.py` & `ccxt-4.2.98/ccxt/async_support/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/lykke.py` & `ccxt-4.2.98/ccxt/async_support/lykke.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/mercado.py` & `ccxt-4.2.98/ccxt/async_support/mercado.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/mexc.py` & `ccxt-4.2.98/ccxt/async_support/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/ndax.py` & `ccxt-4.2.98/ccxt/async_support/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/novadax.py` & `ccxt-4.2.98/ccxt/async_support/novadax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/oceanex.py` & `ccxt-4.2.98/ccxt/async_support/oceanex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/okcoin.py` & `ccxt-4.2.98/ccxt/async_support/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/okx.py` & `ccxt-4.2.98/ccxt/async_support/okx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/onetrading.py` & `ccxt-4.2.98/ccxt/async_support/onetrading.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/p2b.py` & `ccxt-4.2.98/ccxt/async_support/p2b.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/paymium.py` & `ccxt-4.2.98/ccxt/async_support/paymium.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/phemex.py` & `ccxt-4.2.98/ccxt/async_support/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/poloniex.py` & `ccxt-4.2.98/ccxt/async_support/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/poloniexfutures.py` & `ccxt-4.2.98/ccxt/async_support/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/probit.py` & `ccxt-4.2.98/ccxt/async_support/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/timex.py` & `ccxt-4.2.98/ccxt/async_support/timex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/tokocrypto.py` & `ccxt-4.2.98/ccxt/async_support/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/tradeogre.py` & `ccxt-4.2.98/ccxt/async_support/tradeogre.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/upbit.py` & `ccxt-4.2.98/ccxt/async_support/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/wavesexchange.py` & `ccxt-4.2.98/ccxt/async_support/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/wazirx.py` & `ccxt-4.2.98/ccxt/async_support/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/whitebit.py` & `ccxt-4.2.98/ccxt/async_support/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/woo.py` & `ccxt-4.2.98/ccxt/async_support/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/yobit.py` & `ccxt-4.2.98/ccxt/async_support/yobit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/zaif.py` & `ccxt-4.2.98/ccxt/async_support/zaif.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/async_support/zonda.py` & `ccxt-4.2.98/ccxt/async_support/zonda.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/base/__init__.py` & `ccxt-4.2.98/ccxt/base/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/base/decimal_to_precision.py` & `ccxt-4.2.98/ccxt/base/decimal_to_precision.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/base/errors.py` & `ccxt-4.2.98/ccxt/base/errors.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/base/exchange.py` & `ccxt-4.2.98/ccxt/base/exchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """Base exchange class"""
 
 # -----------------------------------------------------------------------------
 
-__version__ = '4.2.97'
+__version__ = '4.2.98'
 
 # -----------------------------------------------------------------------------
 
 from ccxt.base.errors import ExchangeError
 from ccxt.base.errors import NetworkError
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import AuthenticationError
```

### Comparing `ccxt-4.2.97/ccxt/base/precise.py` & `ccxt-4.2.98/ccxt/base/precise.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/base/types.py` & `ccxt-4.2.98/ccxt/base/types.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/bequant.py` & `ccxt-4.2.98/ccxt/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/bigone.py` & `ccxt-4.2.98/ccxt/bigone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/binance.py` & `ccxt-4.2.98/ccxt/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/binancecoinm.py` & `ccxt-4.2.98/ccxt/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/binanceus.py` & `ccxt-4.2.98/ccxt/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/binanceusdm.py` & `ccxt-4.2.98/ccxt/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/bingx.py` & `ccxt-4.2.98/ccxt/bingx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/bit2c.py` & `ccxt-4.2.98/ccxt/bit2c.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/bitbank.py` & `ccxt-4.2.98/ccxt/bitbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/bitbns.py` & `ccxt-4.2.98/ccxt/bitbns.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/bitfinex.py` & `ccxt-4.2.98/ccxt/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/bitfinex2.py` & `ccxt-4.2.98/ccxt/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/bitflyer.py` & `ccxt-4.2.98/ccxt/bitflyer.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/bitget.py` & `ccxt-4.2.98/ccxt/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/bithumb.py` & `ccxt-4.2.98/ccxt/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/bitmart.py` & `ccxt-4.2.98/ccxt/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/bitmex.py` & `ccxt-4.2.98/ccxt/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/bitopro.py` & `ccxt-4.2.98/ccxt/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/bitrue.py` & `ccxt-4.2.98/ccxt/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/bitso.py` & `ccxt-4.2.98/ccxt/bitso.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/bitstamp.py` & `ccxt-4.2.98/ccxt/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/bitteam.py` & `ccxt-4.2.98/ccxt/bitteam.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/bitvavo.py` & `ccxt-4.2.98/ccxt/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/bl3p.py` & `ccxt-4.2.98/ccxt/bl3p.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/blockchaincom.py` & `ccxt-4.2.98/ccxt/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/blofin.py` & `ccxt-4.2.98/ccxt/blofin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/btcalpha.py` & `ccxt-4.2.98/ccxt/btcalpha.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/btcbox.py` & `ccxt-4.2.98/ccxt/btcbox.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/btcmarkets.py` & `ccxt-4.2.98/ccxt/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/btcturk.py` & `ccxt-4.2.98/ccxt/btcturk.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/bybit.py` & `ccxt-4.2.98/ccxt/bybit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/cex.py` & `ccxt-4.2.98/ccxt/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/coinbase.py` & `ccxt-4.2.98/ccxt/coinbase.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/coinbaseinternational.py` & `ccxt-4.2.98/ccxt/coinbaseinternational.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/coinbasepro.py` & `ccxt-4.2.98/ccxt/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/coincheck.py` & `ccxt-4.2.98/ccxt/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/coinex.py` & `ccxt-4.2.98/ccxt/coinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/coinlist.py` & `ccxt-4.2.98/ccxt/coinlist.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/coinmate.py` & `ccxt-4.2.98/ccxt/coinmate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/coinmetro.py` & `ccxt-4.2.98/ccxt/coinmetro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/coinone.py` & `ccxt-4.2.98/ccxt/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/coinsph.py` & `ccxt-4.2.98/ccxt/coinsph.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/coinspot.py` & `ccxt-4.2.98/ccxt/coinspot.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/cryptocom.py` & `ccxt-4.2.98/ccxt/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/currencycom.py` & `ccxt-4.2.98/ccxt/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/delta.py` & `ccxt-4.2.98/ccxt/delta.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/deribit.py` & `ccxt-4.2.98/ccxt/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/digifinex.py` & `ccxt-4.2.98/ccxt/digifinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/exmo.py` & `ccxt-4.2.98/ccxt/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/flowbtc.py` & `ccxt-4.2.98/ccxt/flowbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/fmfwio.py` & `ccxt-4.2.98/ccxt/fmfwio.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/gate.py` & `ccxt-4.2.98/ccxt/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/gemini.py` & `ccxt-4.2.98/ccxt/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/hitbtc.py` & `ccxt-4.2.98/ccxt/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/hollaex.py` & `ccxt-4.2.98/ccxt/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/htx.py` & `ccxt-4.2.98/ccxt/htx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/huobijp.py` & `ccxt-4.2.98/ccxt/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/hyperliquid.py` & `ccxt-4.2.98/ccxt/hyperliquid.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/idex.py` & `ccxt-4.2.98/ccxt/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/independentreserve.py` & `ccxt-4.2.98/ccxt/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/indodax.py` & `ccxt-4.2.98/ccxt/indodax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/kraken.py` & `ccxt-4.2.98/ccxt/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/krakenfutures.py` & `ccxt-4.2.98/ccxt/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/kucoin.py` & `ccxt-4.2.98/ccxt/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/kucoinfutures.py` & `ccxt-4.2.98/ccxt/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/kuna.py` & `ccxt-4.2.98/ccxt/kuna.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/latoken.py` & `ccxt-4.2.98/ccxt/latoken.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/lbank.py` & `ccxt-4.2.98/ccxt/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/luno.py` & `ccxt-4.2.98/ccxt/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/lykke.py` & `ccxt-4.2.98/ccxt/lykke.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/mercado.py` & `ccxt-4.2.98/ccxt/mercado.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/mexc.py` & `ccxt-4.2.98/ccxt/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/ndax.py` & `ccxt-4.2.98/ccxt/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/novadax.py` & `ccxt-4.2.98/ccxt/novadax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/oceanex.py` & `ccxt-4.2.98/ccxt/oceanex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/okcoin.py` & `ccxt-4.2.98/ccxt/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/okx.py` & `ccxt-4.2.98/ccxt/okx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/onetrading.py` & `ccxt-4.2.98/ccxt/onetrading.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/p2b.py` & `ccxt-4.2.98/ccxt/p2b.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/paymium.py` & `ccxt-4.2.98/ccxt/paymium.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/phemex.py` & `ccxt-4.2.98/ccxt/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/poloniex.py` & `ccxt-4.2.98/ccxt/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/poloniexfutures.py` & `ccxt-4.2.98/ccxt/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/__init__.py` & `ccxt-4.2.98/ccxt/pro/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """CCXT: CryptoCurrency eXchange Trading Library (Async)"""
 
 # ----------------------------------------------------------------------------
 
-__version__ = '4.2.97'
+__version__ = '4.2.98'
 
 # ----------------------------------------------------------------------------
 
 from ccxt.async_support.base.exchange import Exchange  # noqa: F401
 
 # CCXT Pro exchanges (now this is mainly used for importing exchanges in WS tests)
```

### Comparing `ccxt-4.2.97/ccxt/pro/alpaca.py` & `ccxt-4.2.98/ccxt/pro/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/ascendex.py` & `ccxt-4.2.98/ccxt/pro/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/bequant.py` & `ccxt-4.2.98/ccxt/pro/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/binance.py` & `ccxt-4.2.98/ccxt/pro/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/binancecoinm.py` & `ccxt-4.2.98/ccxt/pro/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/binanceus.py` & `ccxt-4.2.98/ccxt/pro/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/binanceusdm.py` & `ccxt-4.2.98/ccxt/pro/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/bingx.py` & `ccxt-4.2.98/ccxt/pro/bingx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/bitcoincom.py` & `ccxt-4.2.98/ccxt/pro/bitcoincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/bitfinex.py` & `ccxt-4.2.98/ccxt/pro/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/bitfinex2.py` & `ccxt-4.2.98/ccxt/pro/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/bitget.py` & `ccxt-4.2.98/ccxt/pro/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/bithumb.py` & `ccxt-4.2.98/ccxt/pro/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/bitmart.py` & `ccxt-4.2.98/ccxt/pro/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/bitmex.py` & `ccxt-4.2.98/ccxt/pro/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/bitopro.py` & `ccxt-4.2.98/ccxt/pro/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/bitrue.py` & `ccxt-4.2.98/ccxt/pro/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/bitstamp.py` & `ccxt-4.2.98/ccxt/pro/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/bitvavo.py` & `ccxt-4.2.98/ccxt/pro/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/blockchaincom.py` & `ccxt-4.2.98/ccxt/pro/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/bybit.py` & `ccxt-4.2.98/ccxt/pro/bybit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/cex.py` & `ccxt-4.2.98/ccxt/pro/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/coinbase.py` & `ccxt-4.2.98/ccxt/pro/coinbase.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/coinbaseinternational.py` & `ccxt-4.2.98/ccxt/pro/coinbaseinternational.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/coinbasepro.py` & `ccxt-4.2.98/ccxt/pro/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/coincheck.py` & `ccxt-4.2.98/ccxt/pro/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/coinex.py` & `ccxt-4.2.98/ccxt/pro/coinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/coinone.py` & `ccxt-4.2.98/ccxt/pro/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/cryptocom.py` & `ccxt-4.2.98/ccxt/pro/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/currencycom.py` & `ccxt-4.2.98/ccxt/pro/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/deribit.py` & `ccxt-4.2.98/ccxt/pro/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/exmo.py` & `ccxt-4.2.98/ccxt/pro/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/gate.py` & `ccxt-4.2.98/ccxt/pro/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/gemini.py` & `ccxt-4.2.98/ccxt/pro/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/hitbtc.py` & `ccxt-4.2.98/ccxt/pro/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/hollaex.py` & `ccxt-4.2.98/ccxt/pro/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/htx.py` & `ccxt-4.2.98/ccxt/pro/htx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/huobijp.py` & `ccxt-4.2.98/ccxt/pro/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/hyperliquid.py` & `ccxt-4.2.98/ccxt/pro/hyperliquid.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/idex.py` & `ccxt-4.2.98/ccxt/pro/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/independentreserve.py` & `ccxt-4.2.98/ccxt/pro/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/kraken.py` & `ccxt-4.2.98/ccxt/pro/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/krakenfutures.py` & `ccxt-4.2.98/ccxt/pro/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/kucoin.py` & `ccxt-4.2.98/ccxt/pro/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/kucoinfutures.py` & `ccxt-4.2.98/ccxt/pro/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/lbank.py` & `ccxt-4.2.98/ccxt/pro/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/luno.py` & `ccxt-4.2.98/ccxt/pro/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/mexc.py` & `ccxt-4.2.98/ccxt/pro/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/ndax.py` & `ccxt-4.2.98/ccxt/pro/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/okcoin.py` & `ccxt-4.2.98/ccxt/pro/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/okx.py` & `ccxt-4.2.98/ccxt/pro/okx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/onetrading.py` & `ccxt-4.2.98/ccxt/pro/onetrading.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/p2b.py` & `ccxt-4.2.98/ccxt/pro/p2b.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/phemex.py` & `ccxt-4.2.98/ccxt/pro/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/poloniex.py` & `ccxt-4.2.98/ccxt/pro/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/poloniexfutures.py` & `ccxt-4.2.98/ccxt/pro/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/probit.py` & `ccxt-4.2.98/ccxt/pro/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/upbit.py` & `ccxt-4.2.98/ccxt/pro/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/wazirx.py` & `ccxt-4.2.98/ccxt/pro/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/whitebit.py` & `ccxt-4.2.98/ccxt/pro/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/pro/woo.py` & `ccxt-4.2.98/ccxt/pro/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/probit.py` & `ccxt-4.2.98/ccxt/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ecdsa/__init__.py` & `ccxt-4.2.98/ccxt/static_dependencies/ecdsa/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ecdsa/_version.py` & `ccxt-4.2.98/ccxt/static_dependencies/ecdsa/_version.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ecdsa/curves.py` & `ccxt-4.2.98/ccxt/static_dependencies/ecdsa/curves.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ecdsa/der.py` & `ccxt-4.2.98/ccxt/static_dependencies/ecdsa/der.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ecdsa/ecdsa.py` & `ccxt-4.2.98/ccxt/static_dependencies/ecdsa/ecdsa.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ecdsa/ellipticcurve.py` & `ccxt-4.2.98/ccxt/static_dependencies/ecdsa/ellipticcurve.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ecdsa/keys.py` & `ccxt-4.2.98/ccxt/static_dependencies/ecdsa/keys.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ecdsa/numbertheory.py` & `ccxt-4.2.98/ccxt/static_dependencies/ecdsa/numbertheory.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ecdsa/rfc6979.py` & `ccxt-4.2.98/ccxt/static_dependencies/ecdsa/rfc6979.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ecdsa/util.py` & `ccxt-4.2.98/ccxt/static_dependencies/ecdsa/util.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ethereum/abi/base.py` & `ccxt-4.2.98/ccxt/static_dependencies/ethereum/abi/base.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ethereum/abi/codec.py` & `ccxt-4.2.98/ccxt/static_dependencies/ethereum/abi/codec.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ethereum/abi/decoding.py` & `ccxt-4.2.98/ccxt/static_dependencies/ethereum/abi/decoding.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ethereum/abi/encoding.py` & `ccxt-4.2.98/ccxt/static_dependencies/ethereum/abi/encoding.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ethereum/abi/exceptions.py` & `ccxt-4.2.98/ccxt/static_dependencies/ethereum/abi/exceptions.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ethereum/abi/grammar.py` & `ccxt-4.2.98/ccxt/static_dependencies/ethereum/abi/grammar.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ethereum/abi/registry.py` & `ccxt-4.2.98/ccxt/static_dependencies/ethereum/abi/registry.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ethereum/abi/tools/_strategies.py` & `ccxt-4.2.98/ccxt/static_dependencies/ethereum/abi/tools/_strategies.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ethereum/abi/utils/numeric.py` & `ccxt-4.2.98/ccxt/static_dependencies/ethereum/abi/utils/numeric.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ethereum/account/encode_typed_data/encoding_and_hashing.py` & `ccxt-4.2.98/ccxt/static_dependencies/ethereum/account/encode_typed_data/encoding_and_hashing.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ethereum/account/encode_typed_data/helpers.py` & `ccxt-4.2.98/ccxt/static_dependencies/ethereum/account/encode_typed_data/helpers.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ethereum/account/messages.py` & `ccxt-4.2.98/ccxt/static_dependencies/ethereum/account/messages.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ethereum/hexbytes/_utils.py` & `ccxt-4.2.98/ccxt/static_dependencies/ethereum/hexbytes/_utils.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ethereum/hexbytes/main.py` & `ccxt-4.2.98/ccxt/static_dependencies/ethereum/hexbytes/main.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ethereum/typing/__init__.py` & `ccxt-4.2.98/ccxt/static_dependencies/ethereum/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ethereum/typing/evm.py` & `ccxt-4.2.98/ccxt/static_dependencies/ethereum/typing/evm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ethereum/typing/networks.py` & `ccxt-4.2.98/ccxt/static_dependencies/ethereum/typing/networks.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/__init__.py` & `ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/abi.py` & `ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/abi.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/address.py` & `ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/address.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/applicators.py` & `ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/applicators.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/conversions.py` & `ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/conversions.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/currency.py` & `ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/currency.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/curried/__init__.py` & `ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/curried/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/decorators.py` & `ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/functional.py` & `ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/functional.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/hexadecimal.py` & `ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/hexadecimal.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/humanize.py` & `ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/humanize.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/logging.py` & `ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/module_loading.py` & `ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/numeric.py` & `ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/numeric.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/toolz.py` & `ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/toolz.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/types.py` & `ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/types.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/ethereum/utils/units.py` & `ccxt-4.2.98/ccxt/static_dependencies/ethereum/utils/units.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/keccak/keccak.py` & `ccxt-4.2.98/ccxt/static_dependencies/keccak/keccak.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/msgpack/__init__.py` & `ccxt-4.2.98/ccxt/static_dependencies/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/msgpack/exceptions.py` & `ccxt-4.2.98/ccxt/static_dependencies/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/msgpack/ext.py` & `ccxt-4.2.98/ccxt/static_dependencies/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/msgpack/fallback.py` & `ccxt-4.2.98/ccxt/static_dependencies/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/parsimonious/exceptions.py` & `ccxt-4.2.98/ccxt/static_dependencies/parsimonious/exceptions.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/parsimonious/expressions.py` & `ccxt-4.2.98/ccxt/static_dependencies/parsimonious/expressions.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/parsimonious/grammar.py` & `ccxt-4.2.98/ccxt/static_dependencies/parsimonious/grammar.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/parsimonious/nodes.py` & `ccxt-4.2.98/ccxt/static_dependencies/parsimonious/nodes.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/parsimonious/utils.py` & `ccxt-4.2.98/ccxt/static_dependencies/parsimonious/utils.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/toolz/_signatures.py` & `ccxt-4.2.98/ccxt/static_dependencies/toolz/_signatures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/toolz/_version.py` & `ccxt-4.2.98/ccxt/static_dependencies/toolz/_version.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/toolz/compatibility.py` & `ccxt-4.2.98/ccxt/static_dependencies/toolz/compatibility.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/toolz/curried/__init__.py` & `ccxt-4.2.98/ccxt/static_dependencies/toolz/curried/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/toolz/curried/operator.py` & `ccxt-4.2.98/ccxt/static_dependencies/toolz/curried/operator.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/toolz/dicttoolz.py` & `ccxt-4.2.98/ccxt/static_dependencies/toolz/dicttoolz.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/toolz/functoolz.py` & `ccxt-4.2.98/ccxt/static_dependencies/toolz/functoolz.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/toolz/itertoolz.py` & `ccxt-4.2.98/ccxt/static_dependencies/toolz/itertoolz.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/static_dependencies/toolz/recipes.py` & `ccxt-4.2.98/ccxt/static_dependencies/toolz/recipes.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/test/base/__init__.py` & `ccxt-4.2.98/ccxt/test/base/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/test/base/test_account.py` & `ccxt-4.2.98/ccxt/test/base/test_account.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/test/base/test_balance.py` & `ccxt-4.2.98/ccxt/test/base/test_balance.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/test/base/test_borrow_interest.py` & `ccxt-4.2.98/ccxt/test/base/test_borrow_interest.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/test/base/test_borrow_rate.py` & `ccxt-4.2.98/ccxt/test/base/test_borrow_rate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/test/base/test_calculate_fee.py` & `ccxt-4.2.98/ccxt/test/base/test_calculate_fee.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/test/base/test_crypto.py` & `ccxt-4.2.98/ccxt/test/base/test_crypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/test/base/test_currency.py` & `ccxt-4.2.98/ccxt/test/base/test_currency.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/test/base/test_datetime.py` & `ccxt-4.2.98/ccxt/test/base/test_datetime.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/test/base/test_decimal_to_precision.py` & `ccxt-4.2.98/ccxt/test/base/test_decimal_to_precision.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/test/base/test_deep_extend.py` & `ccxt-4.2.98/ccxt/test/base/test_deep_extend.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/test/base/test_deposit_withdrawal.py` & `ccxt-4.2.98/ccxt/test/base/test_deposit_withdrawal.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/test/base/test_exchange_datetime_functions.py` & `ccxt-4.2.98/ccxt/test/base/test_exchange_datetime_functions.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/test/base/test_funding_rate_history.py` & `ccxt-4.2.98/ccxt/test/base/test_funding_rate_history.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/test/base/test_last_price.py` & `ccxt-4.2.98/ccxt/test/base/test_last_price.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/test/base/test_ledger_entry.py` & `ccxt-4.2.98/ccxt/test/base/test_ledger_entry.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/test/base/test_ledger_item.py` & `ccxt-4.2.98/ccxt/test/base/test_ledger_item.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/test/base/test_leverage_tier.py` & `ccxt-4.2.98/ccxt/test/base/test_leverage_tier.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/test/base/test_margin_mode.py` & `ccxt-4.2.98/ccxt/test/base/test_margin_mode.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/test/base/test_margin_modification.py` & `ccxt-4.2.98/ccxt/test/base/test_margin_modification.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/test/base/test_market.py` & `ccxt-4.2.98/ccxt/test/base/test_market.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/test/base/test_number.py` & `ccxt-4.2.98/ccxt/test/base/test_number.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/test/base/test_ohlcv.py` & `ccxt-4.2.98/ccxt/test/base/test_ohlcv.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/test/base/test_open_interest.py` & `ccxt-4.2.98/ccxt/test/base/test_open_interest.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/test/base/test_order.py` & `ccxt-4.2.98/ccxt/test/base/test_order.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/test/base/test_order_book.py` & `ccxt-4.2.98/ccxt/test/base/test_order_book.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/test/base/test_position.py` & `ccxt-4.2.98/ccxt/test/base/test_position.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/test/base/test_shared_methods.py` & `ccxt-4.2.98/ccxt/test/base/test_shared_methods.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/test/base/test_status.py` & `ccxt-4.2.98/ccxt/test/base/test_status.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/test/base/test_throttle.py` & `ccxt-4.2.98/ccxt/test/base/test_throttle.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/test/base/test_ticker.py` & `ccxt-4.2.98/ccxt/test/base/test_ticker.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/test/base/test_trade.py` & `ccxt-4.2.98/ccxt/test/base/test_trade.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/test/base/test_trading_fee.py` & `ccxt-4.2.98/ccxt/test/base/test_trading_fee.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/test/base/test_transaction.py` & `ccxt-4.2.98/ccxt/test/base/test_transaction.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/test/test_async.py` & `ccxt-4.2.98/ccxt/test/test_async.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/test/test_sync.py` & `ccxt-4.2.98/ccxt/test/test_sync.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/timex.py` & `ccxt-4.2.98/ccxt/timex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/tokocrypto.py` & `ccxt-4.2.98/ccxt/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/tradeogre.py` & `ccxt-4.2.98/ccxt/tradeogre.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/upbit.py` & `ccxt-4.2.98/ccxt/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/wavesexchange.py` & `ccxt-4.2.98/ccxt/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/wazirx.py` & `ccxt-4.2.98/ccxt/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/whitebit.py` & `ccxt-4.2.98/ccxt/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/woo.py` & `ccxt-4.2.98/ccxt/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/yobit.py` & `ccxt-4.2.98/ccxt/yobit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/zaif.py` & `ccxt-4.2.98/ccxt/zaif.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt/zonda.py` & `ccxt-4.2.98/ccxt/zonda.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/ccxt.egg-info/PKG-INFO` & `ccxt-4.2.98/ccxt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccxt
-Version: 4.2.97
+Version: 4.2.98
 Summary: A JavaScript / TypeScript / Python / C# / PHP cryptocurrency trading library with support for 100+ exchanges
 Home-page: https://ccxt.com
 Author: Igor Kroitor
 Author-email: igor.kroitor@gmail.com
 License: MIT
 Project-URL: Homepage, https://ccxt.com
 Project-URL: Documentation, https://github.com/ccxt/ccxt/wiki
@@ -221,21 +221,21 @@
         console.log(version, Object.keys(exchanges));
         ```
         
         ### JavaScript (for use with the `<script>` tag):
         
         All-in-one browser bundle (dependencies included), served from a CDN of your choice:
         
-        * jsDelivr: https://cdn.jsdelivr.net/npm/ccxt@4.2.97/dist/ccxt.browser.js
-        * unpkg: https://unpkg.com/ccxt@4.2.97/dist/ccxt.browser.js
+        * jsDelivr: https://cdn.jsdelivr.net/npm/ccxt@4.2.98/dist/ccxt.browser.js
+        * unpkg: https://unpkg.com/ccxt@4.2.98/dist/ccxt.browser.js
         
         CDNs are not updated in real-time and may have delays. Defaulting to the most recent version without specifying the version number is not recommended. Please, keep in mind that we are not responsible for the correct operation of those CDN servers.
         
         ```HTML
-        <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ccxt@4.2.97/dist/ccxt.browser.js"></script>
+        <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ccxt@4.2.98/dist/ccxt.browser.js"></script>
         ```
         
         Creates a global `ccxt` object:
         
         ```JavaScript
         console.log (ccxt.exchanges) // print all available exchanges
         ```
```

### Comparing `ccxt-4.2.97/ccxt.egg-info/SOURCES.txt` & `ccxt-4.2.98/ccxt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccxt-4.2.97/package.json` & `ccxt-4.2.98/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'4.2.98'"}*

```diff
@@ -265,9 +265,9 @@
         "update-links": "node build/update-links",
         "validate-types": "node --loader ts-node/esm build/validate-types.ts",
         "vss": "node build/vss"
     },
     "type": "module",
     "types": "./js/ccxt.d.ts",
     "unpkg": "dist/ccxt.browser.js",
-    "version": "4.2.97"
+    "version": "4.2.98"
 }
```

### Comparing `ccxt-4.2.97/setup.py` & `ccxt-4.2.98/setup.py`

 * *Files identical despite different names*

