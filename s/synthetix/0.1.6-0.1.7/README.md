# Comparing `tmp/synthetix-0.1.6.tar.gz` & `tmp/synthetix-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synthetix-0.1.6.tar", last modified: Wed Apr 10 20:24:07 2024, max compression
+gzip compressed data, was "synthetix-0.1.7.tar", last modified: Tue Apr 16 21:34:54 2024, max compression
```

## Comparing `synthetix-0.1.6.tar` & `synthetix-0.1.7.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:07.187604 synthetix-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-10 20:23:51.000000 synthetix-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-10 20:24:07.187604 synthetix-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-10 20:23:51.000000 synthetix-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 20:24:07.187604 synthetix-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-10 20:23:51.000000 synthetix-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:07.171604 synthetix-0.1.6/synthetix/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:07.175604 synthetix-0.1.6/synthetix/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/contracts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:07.175604 synthetix-0.1.6/synthetix/contracts/deployments/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:07.175604 synthetix-0.1.6/synthetix/contracts/deployments/1/
--rw-r--r--   0 runner    (1001) docker     (127)    16869 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/1/CannonRegistry.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:07.175604 synthetix-0.1.6/synthetix/contracts/deployments/10/
--rw-r--r--   0 runner    (1001) docker     (127)    47805 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/10/PerpsV2MarketData.json
--rw-r--r--   0 runner    (1001) docker     (127)    17125 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/10/USDProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/10/WETH.json
--rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/10/sUSD.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:07.179604 synthetix-0.1.6/synthetix/contracts/deployments/420/
--rw-r--r--   0 runner    (1001) docker     (127)    16597 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/420/AccountProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)   113611 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/420/CoreProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    16597 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/420/PerpsAccountProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    90963 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/420/PerpsMarketProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    42868 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/420/PerpsV2Market.json
--rw-r--r--   0 runner    (1001) docker     (127)    47805 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/420/PerpsV2MarketData.json
--rw-r--r--   0 runner    (1001) docker     (127)    86175 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/420/SpotMarketProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    15069 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/420/TrustedMulticallForwarder.json
--rw-r--r--   0 runner    (1001) docker     (127)    17125 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/420/USDProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/420/WETH.json
--rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/420/sUSD.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:07.179604 synthetix-0.1.6/synthetix/contracts/deployments/421614/
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/421614/WETH.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:07.179604 synthetix-0.1.6/synthetix/contracts/deployments/8453/
--rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/8453/AccountProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)   116534 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/8453/CoreProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/8453/PerpsAccountProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)   105067 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/8453/PerpsMarketProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/8453/PythERC7412Wrapper.json
--rw-r--r--   0 runner    (1001) docker     (127)    88477 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/8453/SpotMarketProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    20520 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/8453/TrustedMulticallForwarder.json
--rw-r--r--   0 runner    (1001) docker     (127)    34846 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/8453/USDC.json
--rw-r--r--   0 runner    (1001) docker     (127)    17180 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/8453/USDProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/8453/WETH.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:07.183604 synthetix-0.1.6/synthetix/contracts/deployments/84532/
--rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/84532/AccountProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)   116534 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/84532/CoreProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)     8137 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/84532/MintableToken.json
--rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/84532/PerpsAccountProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)   105067 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/84532/PerpsMarketProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    53394 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/84532/Pyth.json
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/84532/PythERC7412Wrapper.json
--rw-r--r--   0 runner    (1001) docker     (127)    90457 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/84532/SpotMarketProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    20520 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/84532/TrustedMulticallForwarder.json
--rw-r--r--   0 runner    (1001) docker     (127)    17180 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/84532/USDProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/84532/WETH.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/contracts/deployments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:07.183604 synthetix-0.1.6/synthetix/core/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12622 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/core/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:07.183604 synthetix-0.1.6/synthetix/perps/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/perps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37923 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/perps/perps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:07.183604 synthetix-0.1.6/synthetix/pyth/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/pyth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/pyth/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/pyth/pyth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:07.183604 synthetix-0.1.6/synthetix/queries/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/queries/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/queries/gql.py
--rw-r--r--   0 runner    (1001) docker     (127)    14181 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/queries/queries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:07.183604 synthetix-0.1.6/synthetix/spot/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/spot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25270 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/spot/spot.py
--rw-r--r--   0 runner    (1001) docker     (127)    21506 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/synthetix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:07.187604 synthetix-0.1.6/synthetix/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7842 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/utils/multicall.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-10 20:23:51.000000 synthetix-0.1.6/synthetix/utils/wei.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:07.187604 synthetix-0.1.6/synthetix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-10 20:24:07.000000 synthetix-0.1.6/synthetix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-10 20:24:07.000000 synthetix-0.1.6/synthetix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 20:24:07.000000 synthetix-0.1.6/synthetix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-10 20:24:07.000000 synthetix-0.1.6/synthetix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 20:24:07.000000 synthetix-0.1.6/synthetix.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:07.187604 synthetix-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9714 2024-04-10 20:23:51.000000 synthetix-0.1.6/tests/test_perps_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-10 20:23:51.000000 synthetix-0.1.6/tests/test_spot_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-10 20:23:51.000000 synthetix-0.1.6/tests/test_susd.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-10 20:23:51.000000 synthetix-0.1.6/tests/test_synthetix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.297219 synthetix-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-16 21:34:41.000000 synthetix-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-16 21:34:54.297219 synthetix-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-16 21:34:41.000000 synthetix-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 21:34:54.297219 synthetix-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-16 21:34:41.000000 synthetix-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.285219 synthetix-0.1.7/synthetix/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.285219 synthetix-0.1.7/synthetix/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/contracts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.285219 synthetix-0.1.7/synthetix/contracts/deployments/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.285219 synthetix-0.1.7/synthetix/contracts/deployments/1/
+-rw-r--r--   0 runner    (1001) docker     (127)    16869 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/1/CannonRegistry.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.285219 synthetix-0.1.7/synthetix/contracts/deployments/10/
+-rw-r--r--   0 runner    (1001) docker     (127)    47805 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/10/PerpsV2MarketData.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17125 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/10/USDProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/10/WETH.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/10/sUSD.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.289219 synthetix-0.1.7/synthetix/contracts/deployments/420/
+-rw-r--r--   0 runner    (1001) docker     (127)    16597 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/420/AccountProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)   113611 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/420/CoreProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16597 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/420/PerpsAccountProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    90963 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/420/PerpsMarketProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    42868 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/420/PerpsV2Market.json
+-rw-r--r--   0 runner    (1001) docker     (127)    47805 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/420/PerpsV2MarketData.json
+-rw-r--r--   0 runner    (1001) docker     (127)    86175 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/420/SpotMarketProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15069 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/420/TrustedMulticallForwarder.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17125 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/420/USDProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/420/WETH.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/420/sUSD.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.289219 synthetix-0.1.7/synthetix/contracts/deployments/421614/
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/421614/WETH.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.293219 synthetix-0.1.7/synthetix/contracts/deployments/8453/
+-rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/8453/AccountProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)   116534 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/8453/CoreProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/8453/PerpsAccountProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)   105067 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/8453/PerpsMarketProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/8453/PythERC7412Wrapper.json
+-rw-r--r--   0 runner    (1001) docker     (127)    88477 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/8453/SpotMarketProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20520 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/8453/TrustedMulticallForwarder.json
+-rw-r--r--   0 runner    (1001) docker     (127)    34846 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/8453/USDC.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17180 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/8453/USDProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/8453/WETH.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.293219 synthetix-0.1.7/synthetix/contracts/deployments/84532/
+-rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/84532/AccountProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)   116534 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/84532/CoreProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8137 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/84532/MintableToken.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16652 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/84532/PerpsAccountProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)   105067 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/84532/PerpsMarketProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    53394 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/84532/Pyth.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/84532/PythERC7412Wrapper.json
+-rw-r--r--   0 runner    (1001) docker     (127)    90457 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/84532/SpotMarketProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20520 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/84532/TrustedMulticallForwarder.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17180 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/84532/USDProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/84532/WETH.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/contracts/deployments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.293219 synthetix-0.1.7/synthetix/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12622 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/core/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.293219 synthetix-0.1.7/synthetix/perps/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/perps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37803 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/perps/perps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.293219 synthetix-0.1.7/synthetix/pyth/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/pyth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/pyth/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/pyth/pyth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.297219 synthetix-0.1.7/synthetix/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/queries/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/queries/gql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14181 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/queries/queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.297219 synthetix-0.1.7/synthetix/spot/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/spot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25270 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/spot/spot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22663 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/synthetix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.297219 synthetix-0.1.7/synthetix/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/utils/multicall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-16 21:34:41.000000 synthetix-0.1.7/synthetix/utils/wei.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.297219 synthetix-0.1.7/synthetix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-16 21:34:54.000000 synthetix-0.1.7/synthetix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-16 21:34:54.000000 synthetix-0.1.7/synthetix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 21:34:54.000000 synthetix-0.1.7/synthetix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-16 21:34:54.000000 synthetix-0.1.7/synthetix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 21:34:54.000000 synthetix-0.1.7/synthetix.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:34:54.297219 synthetix-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9714 2024-04-16 21:34:41.000000 synthetix-0.1.7/tests/test_perps_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-16 21:34:41.000000 synthetix-0.1.7/tests/test_spot_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-16 21:34:41.000000 synthetix-0.1.7/tests/test_susd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-16 21:34:41.000000 synthetix-0.1.7/tests/test_synthetix.py
```

### Comparing `synthetix-0.1.6/PKG-INFO` & `synthetix-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthetix
-Version: 0.1.6
+Version: 0.1.7
 Summary: Synthetix protocol SDK
 Author: Synthetix DAO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `synthetix-0.1.6/README.md` & `synthetix-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/setup.py` & `synthetix-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="synthetix",
-    version="0.1.6",
+    version="0.1.7",
     description="Synthetix protocol SDK",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Synthetix DAO",
     packages=find_packages(),
     install_requires=[
         "numpy",
```

### Comparing `synthetix-0.1.6/synthetix/constants.py` & `synthetix-0.1.7/synthetix/constants.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/contracts.py` & `synthetix-0.1.7/synthetix/contracts/contracts.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/1/CannonRegistry.json` & `synthetix-0.1.7/synthetix/contracts/deployments/1/CannonRegistry.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/10/PerpsV2MarketData.json` & `synthetix-0.1.7/synthetix/contracts/deployments/10/PerpsV2MarketData.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/10/USDProxy.json` & `synthetix-0.1.7/synthetix/contracts/deployments/10/USDProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/10/WETH.json` & `synthetix-0.1.7/synthetix/contracts/deployments/10/WETH.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/10/sUSD.json` & `synthetix-0.1.7/synthetix/contracts/deployments/10/sUSD.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/420/AccountProxy.json` & `synthetix-0.1.7/synthetix/contracts/deployments/420/AccountProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/420/CoreProxy.json` & `synthetix-0.1.7/synthetix/contracts/deployments/420/CoreProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/420/PerpsAccountProxy.json` & `synthetix-0.1.7/synthetix/contracts/deployments/420/PerpsAccountProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/420/PerpsMarketProxy.json` & `synthetix-0.1.7/synthetix/contracts/deployments/420/PerpsMarketProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/420/PerpsV2Market.json` & `synthetix-0.1.7/synthetix/contracts/deployments/420/PerpsV2Market.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/420/PerpsV2MarketData.json` & `synthetix-0.1.7/synthetix/contracts/deployments/420/PerpsV2MarketData.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/420/SpotMarketProxy.json` & `synthetix-0.1.7/synthetix/contracts/deployments/420/SpotMarketProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/420/TrustedMulticallForwarder.json` & `synthetix-0.1.7/synthetix/contracts/deployments/420/TrustedMulticallForwarder.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/420/USDProxy.json` & `synthetix-0.1.7/synthetix/contracts/deployments/420/USDProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/420/WETH.json` & `synthetix-0.1.7/synthetix/contracts/deployments/420/WETH.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/420/sUSD.json` & `synthetix-0.1.7/synthetix/contracts/deployments/420/sUSD.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/421614/WETH.json` & `synthetix-0.1.7/synthetix/contracts/deployments/421614/WETH.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/8453/AccountProxy.json` & `synthetix-0.1.7/synthetix/contracts/deployments/8453/AccountProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/8453/CoreProxy.json` & `synthetix-0.1.7/synthetix/contracts/deployments/8453/CoreProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/8453/PerpsAccountProxy.json` & `synthetix-0.1.7/synthetix/contracts/deployments/8453/PerpsAccountProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/8453/PerpsMarketProxy.json` & `synthetix-0.1.7/synthetix/contracts/deployments/8453/PerpsMarketProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/8453/PythERC7412Wrapper.json` & `synthetix-0.1.7/synthetix/contracts/deployments/8453/PythERC7412Wrapper.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/8453/SpotMarketProxy.json` & `synthetix-0.1.7/synthetix/contracts/deployments/8453/SpotMarketProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/8453/TrustedMulticallForwarder.json` & `synthetix-0.1.7/synthetix/contracts/deployments/8453/TrustedMulticallForwarder.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/8453/USDC.json` & `synthetix-0.1.7/synthetix/contracts/deployments/8453/USDC.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/8453/USDProxy.json` & `synthetix-0.1.7/synthetix/contracts/deployments/8453/USDProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/8453/WETH.json` & `synthetix-0.1.7/synthetix/contracts/deployments/8453/WETH.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/84532/AccountProxy.json` & `synthetix-0.1.7/synthetix/contracts/deployments/84532/AccountProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/84532/CoreProxy.json` & `synthetix-0.1.7/synthetix/contracts/deployments/84532/CoreProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/84532/MintableToken.json` & `synthetix-0.1.7/synthetix/contracts/deployments/84532/MintableToken.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/84532/PerpsAccountProxy.json` & `synthetix-0.1.7/synthetix/contracts/deployments/84532/PerpsAccountProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/84532/PerpsMarketProxy.json` & `synthetix-0.1.7/synthetix/contracts/deployments/84532/PerpsMarketProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/84532/Pyth.json` & `synthetix-0.1.7/synthetix/contracts/deployments/84532/Pyth.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/84532/PythERC7412Wrapper.json` & `synthetix-0.1.7/synthetix/contracts/deployments/84532/PythERC7412Wrapper.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/84532/SpotMarketProxy.json` & `synthetix-0.1.7/synthetix/contracts/deployments/84532/SpotMarketProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/84532/TrustedMulticallForwarder.json` & `synthetix-0.1.7/synthetix/contracts/deployments/84532/TrustedMulticallForwarder.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/84532/USDProxy.json` & `synthetix-0.1.7/synthetix/contracts/deployments/84532/USDProxy.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/contracts/deployments/84532/WETH.json` & `synthetix-0.1.7/synthetix/contracts/deployments/84532/WETH.json`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/core/core.py` & `synthetix-0.1.7/synthetix/core/core.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/perps/perps.py` & `synthetix-0.1.7/synthetix/perps/perps.py`

 * *Files 0% similar despite different names*

```diff
@@ -897,19 +897,17 @@
         order = self.get_order(account_id)
         settlement_strategy = order["settlement_strategy"]
         settlement_time = (
             order["commitment_time"] + settlement_strategy["settlement_delay"]
         )
 
         # check if order is ready to be settled
-        self.logger.info(f"settlement time: {settlement_time}")
-        self.logger.info(f"current time: {time.time()}")
         if settlement_time > time.time():
             duration = settlement_time - time.time()
-            self.logger.info(f"Waiting {duration} seconds until order can be settled")
+            self.logger.info(f"Waiting {round(duration, 4)} seconds to settle order")
             time.sleep(duration)
         else:
             # TODO: check if expired
             self.logger.info(f"Order is ready to be settled")
 
         # get fresh prices to provide to the oracle
         market_name = self._resolve_market(order["market_id"], None)[1]
@@ -927,26 +925,26 @@
                     self.snx,
                     self.market_proxy,
                     "settleOrder",
                     [account_id],
                     calls=calls,
                 )
             except Exception as e:
-                self.logger.info(f"settleOrder error: {e}")
+                self.logger.error(f"settleOrder error: {e}")
                 tx_tries += 1
                 time.sleep(tx_delay)
                 continue
 
             if submit:
                 tx_hash = self.snx.execute_transaction(tx_params)
                 self.logger.info(f"Settling order for account {account_id}")
                 self.logger.info(f"settle tx: {tx_hash}")
 
                 receipt = self.snx.wait(tx_hash)
-                self.logger.info(f"settle receipt: {receipt}")
+                self.logger.debug(f"settle receipt: {receipt}")
 
                 # check the order
                 order = self.get_order(account_id)
                 if order["size_delta"] == 0:
                     self.logger.info(
                         f"Order settlement successful for account {account_id}"
                     )
```

### Comparing `synthetix-0.1.6/synthetix/pyth/constants.py` & `synthetix-0.1.7/synthetix/pyth/constants.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/pyth/pyth.py` & `synthetix-0.1.7/synthetix/pyth/pyth.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/queries/config.py` & `synthetix-0.1.7/synthetix/queries/config.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/queries/gql.py` & `synthetix-0.1.7/synthetix/queries/gql.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/queries/queries.py` & `synthetix-0.1.7/synthetix/queries/queries.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/spot/spot.py` & `synthetix-0.1.7/synthetix/spot/spot.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix/synthetix.py` & `synthetix-0.1.7/synthetix/synthetix.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import argparse
 import logging
 import warnings
 from web3 import Web3
 from web3.constants import ADDRESS_ZERO
 from web3.types import TxParams
 from .constants import (
     DEFAULT_NETWORK_ID,
@@ -22,27 +23,51 @@
 from .spot import Spot
 
 from .queries import Queries
 
 warnings.filterwarnings("ignore")
 
 
-def setup_logging():
+def setup_logging(debug: bool, verbose: int):
+    if debug:
+        log_level = logging.DEBUG
+    elif verbose >= 2:
+        log_level = logging.DEBUG
+    else:
+        log_level = logging.INFO
+
     # set up logging
     logger = logging.getLogger(__name__)
-    logger.setLevel(logging.INFO)
+    logger.setLevel(log_level)
 
     handler = logging.StreamHandler()
     handler.setFormatter(logging.Formatter("%(asctime)s - %(levelname)s - %(message)s"))
 
     if not logger.handlers:
         logger.addHandler(handler)
     return logger
 
 
+def parse_args():
+    parser = argparse.ArgumentParser(description="Synthetix SDK")
+    parser.add_argument(
+        "-v",
+        "--verbose",
+        action="count",
+        default=0,
+        help="Increase verbosity (-v, -vv, -vvv)",
+    )
+    parser.add_argument("--debug", action="store_true", help="Enable debug logging")
+
+    # Add this line to handle the case when no arguments are provided
+    args, _ = parser.parse_known_args()
+
+    return args
+
+
 class Synthetix:
     """
     The main class for interacting with the Synthetix protocol. The class
     requires a provider RPC endpoint and a wallet address::
 
             snx = Synthetix(
                 provider_rpc='https://base-mainnet.infura.io/v3/...',
@@ -109,56 +134,70 @@
         use_estimate_gas: bool = True,
         cannon_config: dict = None,
         gql_endpoint_perps: str = None,
         gql_endpoint_rates: str = None,
         satsuma_api_key: str = None,
         price_service_endpoint: str = None,
         gas_multiplier: float = DEFAULT_GAS_MULTIPLIER,
+        is_fork: bool = False,
     ):
-        self.logger = setup_logging()
+        args = parse_args()
+        self.logger = setup_logging(args.debug, args.verbose)
 
         # init account variables
         self.private_key = private_key
         self.use_estimate_gas = use_estimate_gas
         self.cannon_config = cannon_config
         self.provider_rpc = provider_rpc
         self.mainnet_rpc = mainnet_rpc
         self.ipfs_gateway = ipfs_gateway
         self.gas_multiplier = gas_multiplier
         self.max_price_impact = max_price_impact
         self.tracking_code = tracking_code
         self.referrer = referrer
+        self.is_fork = is_fork
 
         # init chain provider
         if provider_rpc.startswith("http"):
             web3 = Web3(Web3.HTTPProvider(self.provider_rpc))
         elif provider_rpc.startswith("wss"):
             web3 = Web3(Web3.WebsocketProvider(self.provider_rpc))
         elif provider_rpc.endswith("ipc"):
             web3 = Web3(Web3.IPCProvider(self.provider_rpc))
         else:
             raise Exception("Provider RPC endpoint is invalid")
 
         # check for RPC signers
-        self.rpc_signers = web3.eth.accounts
-        if address == ADDRESS_ZERO and len(web3.eth.accounts) > 0:
-            self.address = web3.eth.accounts[0]
+        try:
+            self.rpc_signers = web3.eth.accounts
+        except Exception as e:
+            self.logger.error(f"Error getting RPC signers: {e}")
+            self.rpc_signers = []
+
+        if address == ADDRESS_ZERO and len(self.rpc_signers) > 0:
+            self.address = self.rpc_signers[0]
+            self.logger.info(f"Using RPC signer: {self.address}")
+        elif address in self.rpc_signers:
+            self.address = address
             self.logger.info(f"Using RPC signer: {self.address}")
         elif address == ADDRESS_ZERO and self.private_key is not None:
             self.address = web3.eth.account.from_key(self.private_key).address
             self.logger.info(f"Using private key signer: {self.address}")
         elif address != ADDRESS_ZERO and self.private_key is not None:
             # check the address matches the private key
             if web3.eth.account.from_key(self.private_key).address != address:
                 raise Exception("Private key does not match the provided address")
             self.address = address
+            self.logger.info(f"Using private key signer: {self.address}")
         else:
             # set address without private key
             self.address = address
-            self.logger.info(f"Using provided address without private key: {self.address}")
+            self.logger.info(
+                f"Using provided address without private key: {self.address}"
+            )
 
         # check network id
         if network_id is None:
             self.logger.info(
                 f"Setting network_id from RPC chain_id: {web3.eth.chain_id}"
             )
             network_id = web3.eth.chain_id
@@ -384,20 +423,20 @@
                 tx_data["gas"] = 1500000
 
         if reset_nonce:
             self.nonce = self.web3.eth.get_transaction_count(self.address)
             tx_data["nonce"] = self.nonce
 
         try:
-            self.logger.info(f"Tx data: {tx_data}")
+            self.logger.debug(f"Tx data: {tx_data}")
             tx_hash = self._send_transaction(tx_data)
             return tx_hash
         except ValueError as e:
             if "nonce too low" in str(e):
-                self.logger.info("Nonce too low, resetting nonce and retrying.")
+                self.logger.warning("Nonce too low, resetting nonce and retrying.")
                 return self.execute_transaction(tx_data, reset_nonce=True)
             else:
                 raise Exception(f"Transaction failed: {e}")
 
     def get_susd_balance(self, address: str = None, legacy: bool = False) -> dict:
         """
         Gets current sUSD balance in wallet. Supports both legacy and V3 sUSD.
```

### Comparing `synthetix-0.1.6/synthetix/utils/multicall.py` & `synthetix-0.1.7/synthetix/utils/multicall.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,15 +83,24 @@
     ):
         # decode error data
         address, feed_ids, args = decode_erc7412_error(snx, error.data)
         update_type = args[0]
 
         if update_type == 1:
             # fetch the data from pyth for those feed ids
-            price_update_data = snx.pyth.get_feeds_data(feed_ids)
+            if not snx.is_fork:
+                price_update_data = snx.pyth.get_feeds_data(feed_ids)
+            else:
+                # if it's a fork, get the price for the latest block
+                # this avoids providing "future" prices to the contract on a fork
+                block = snx.web3.eth.get_block("latest")
+                price_update_data = [
+                    snx.pyth.get_benchmark_data(feed_id, block.timestamp)[0]
+                    for feed_id in feed_ids
+                ]
 
             # create a new request
             to, data, value = make_fulfillment_request(
                 snx, address, price_update_data, args
             )
         elif update_type == 2:
             # fetch the data from pyth for those feed ids
@@ -104,15 +113,15 @@
         else:
             snx.logger.error(f"Unknown update type: {update_type}")
             raise error
 
         calls = [(to, True, value, data)] + calls
         return calls
     else:
-        snx.logger.error(f"Error is not related to oracle data: {error}")
+        snx.logger.debug(f"Error is not related to oracle data")
         raise error
 
 
 def write_erc7412(snx, contract, function_name, args, tx_params={}, calls=[]):
     # prepare the initial call
     this_call = [
         (
@@ -135,19 +144,19 @@
                 calls
             ).build_transaction(tx_params)
 
             # buffer the gas limit
             tx_params["gas"] = int(tx_params["gas"] * 1.15)
 
             # if simulation passes, return the transaction
-            snx.logger.info(f"Simulated tx successfully: {tx_params}")
+            snx.logger.debug(f"Simulated tx successfully: {tx_params}")
             return tx_params
         except Exception as e:
             # check if the error is related to oracle data
-            snx.logger.info(f"Simulation failed, decoding the error {e}")
+            snx.logger.debug(f"Simulation failed, decoding the error {e}")
 
             # handle the error by appending calls
             calls = handle_erc7412_error(snx, e, calls)
 
 
 def call_erc7412(snx, contract, function_name, args, calls=[], block="latest"):
     # fix args
@@ -174,15 +183,15 @@
 
             # call was successful, decode the result
             decoded_result = decode_result(contract, function_name, call[-1][1])
             return decoded_result if len(decoded_result) > 1 else decoded_result[0]
 
         except Exception as e:
             # check if the error is related to oracle data
-            snx.logger.info(f"Simulation failed, decoding the error {e}")
+            snx.logger.debug(f"Simulation failed, decoding the error {e}")
 
             # handle the error by appending calls
             calls = handle_erc7412_error(snx, e, calls)
 
 
 def multicall_erc7412(
     snx, contract, function_name, args_list, calls=[], block="latest"
@@ -227,11 +236,11 @@
                 decoded_result if len(decoded_result) > 1 else decoded_result[0]
                 for decoded_result in decoded_results
             ]
             return decoded_results
 
         except Exception as e:
             # check if the error is related to oracle data
-            snx.logger.info(f"Simulation failed, decoding the error {e}")
+            snx.logger.debug(f"Simulation failed, decoding the error {e}")
 
             # handle the error by appending calls
             calls = handle_erc7412_error(snx, e, calls)
```

### Comparing `synthetix-0.1.6/synthetix/utils/wei.py` & `synthetix-0.1.7/synthetix/utils/wei.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/synthetix.egg-info/PKG-INFO` & `synthetix-0.1.7/synthetix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthetix
-Version: 0.1.6
+Version: 0.1.7
 Summary: Synthetix protocol SDK
 Author: Synthetix DAO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `synthetix-0.1.6/synthetix.egg-info/SOURCES.txt` & `synthetix-0.1.7/synthetix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/tests/test_perps_v3.py` & `synthetix-0.1.7/tests/test_perps_v3.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/tests/test_spot_v3.py` & `synthetix-0.1.7/tests/test_spot_v3.py`

 * *Files identical despite different names*

### Comparing `synthetix-0.1.6/tests/test_susd.py` & `synthetix-0.1.7/tests/test_susd.py`

 * *Files identical despite different names*

