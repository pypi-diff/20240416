# Comparing `tmp/hyperdrivepy-0.9.2.tar.gz` & `tmp/hyperdrivepy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperdrivepy-0.9.2.tar", last modified: Mon Mar 18 17:18:26 2024, max compression
+gzip compressed data, was "hyperdrivepy-1.0.1.tar", last modified: Mon Apr 15 23:25:13 2024, max compression
```

## Comparing `hyperdrivepy-0.9.2.tar` & `hyperdrivepy-1.0.1.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:18:26.381579 hyperdrivepy-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-18 17:18:26.381579 hyperdrivepy-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:18:26.373579 hyperdrivepy-0.9.2/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:18:26.377579 hyperdrivepy-0.9.2/python/hyperdrivepy/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/python/hyperdrivepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15974 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/python/hyperdrivepy/hyperdrive_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/python/hyperdrivepy/hyperdrive_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:18:26.381579 hyperdrivepy-0.9.2/python/hyperdrivepy/pypechain_types/
--rw-r--r--   0 runner    (1001) docker     (127)   245208 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/python/hyperdrivepy/pypechain_types/IERC4626HyperdriveContract.py
--rw-r--r--   0 runner    (1001) docker     (127)    14272 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/python/hyperdrivepy/pypechain_types/IERC4626HyperdriveTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/python/hyperdrivepy/pypechain_types/IHyperdriveTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/python/hyperdrivepy/pypechain_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/python/hyperdrivepy/pypechain_types/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/python/hyperdrivepy/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/python/hyperdrivepy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:18:26.381579 hyperdrivepy-0.9.2/python/hyperdrivepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-18 17:18:26.000000 hyperdrivepy-0.9.2/python/hyperdrivepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-18 17:18:26.000000 hyperdrivepy-0.9.2/python/hyperdrivepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 17:18:26.000000 hyperdrivepy-0.9.2/python/hyperdrivepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 17:18:26.000000 hyperdrivepy-0.9.2/python/hyperdrivepy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-18 17:18:26.000000 hyperdrivepy-0.9.2/python/hyperdrivepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 17:18:26.381579 hyperdrivepy-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 17:18:26.381579 hyperdrivepy-0.9.2/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/src/hyperdrive_state.rs
--rw-r--r--   0 runner    (1001) docker     (127)    11261 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/src/hyperdrive_state_methods.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/src/hyperdrive_utils.rs
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/src/pool_config.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/src/pool_info.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-03-18 17:18:20.000000 hyperdrivepy-0.9.2/src/utils.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:25:13.421094 hyperdrivepy-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-15 23:25:09.000000 hyperdrivepy-1.0.1/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 23:25:09.000000 hyperdrivepy-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-15 23:25:09.000000 hyperdrivepy-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-15 23:25:13.421094 hyperdrivepy-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-15 23:25:09.000000 hyperdrivepy-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-15 23:25:09.000000 hyperdrivepy-1.0.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:25:13.417094 hyperdrivepy-1.0.1/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:25:13.417094 hyperdrivepy-1.0.1/python/hyperdrivepy/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-15 23:25:09.000000 hyperdrivepy-1.0.1/python/hyperdrivepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20283 2024-04-15 23:25:09.000000 hyperdrivepy-1.0.1/python/hyperdrivepy/hyperdrive_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-04-15 23:25:09.000000 hyperdrivepy-1.0.1/python/hyperdrivepy/hyperdrive_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:25:13.421094 hyperdrivepy-1.0.1/python/hyperdrivepy/pypechain_types/
+-rw-r--r--   0 runner    (1001) docker     (127)   251847 2024-04-15 23:25:09.000000 hyperdrivepy-1.0.1/python/hyperdrivepy/pypechain_types/IHyperdriveContract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16836 2024-04-15 23:25:09.000000 hyperdrivepy-1.0.1/python/hyperdrivepy/pypechain_types/IHyperdriveTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-15 23:25:09.000000 hyperdrivepy-1.0.1/python/hyperdrivepy/pypechain_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-04-15 23:25:09.000000 hyperdrivepy-1.0.1/python/hyperdrivepy/pypechain_types/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-15 23:25:09.000000 hyperdrivepy-1.0.1/python/hyperdrivepy/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-15 23:25:09.000000 hyperdrivepy-1.0.1/python/hyperdrivepy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:25:13.421094 hyperdrivepy-1.0.1/python/hyperdrivepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-15 23:25:13.000000 hyperdrivepy-1.0.1/python/hyperdrivepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-15 23:25:13.000000 hyperdrivepy-1.0.1/python/hyperdrivepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 23:25:13.000000 hyperdrivepy-1.0.1/python/hyperdrivepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 23:25:13.000000 hyperdrivepy-1.0.1/python/hyperdrivepy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-15 23:25:13.000000 hyperdrivepy-1.0.1/python/hyperdrivepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 23:25:13.421094 hyperdrivepy-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-15 23:25:09.000000 hyperdrivepy-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:25:13.421094 hyperdrivepy-1.0.1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-15 23:25:09.000000 hyperdrivepy-1.0.1/src/hyperdrive_state.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    16359 2024-04-15 23:25:09.000000 hyperdrivepy-1.0.1/src/hyperdrive_state_methods.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-15 23:25:09.000000 hyperdrivepy-1.0.1/src/hyperdrive_utils.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-15 23:25:09.000000 hyperdrivepy-1.0.1/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-15 23:25:09.000000 hyperdrivepy-1.0.1/src/pool_config.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-15 23:25:09.000000 hyperdrivepy-1.0.1/src/pool_info.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-15 23:25:09.000000 hyperdrivepy-1.0.1/src/utils.rs
```

### Comparing `hyperdrivepy-0.9.2/Cargo.toml` & `hyperdrivepy-1.0.1/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "hyperdrivepy"
 edition = "2021"
-version = "0.9.2"
+version = "1.0.1"
 authors = [
     "Dylan Paiton",
     "Matt Brown",
     "Sheng Lundquist",
 ]
 description = "Python wrappers for the Hyperdrive AMM"
```

### Comparing `hyperdrivepy-0.9.2/LICENSE` & `hyperdrivepy-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-0.9.2/PKG-INFO` & `hyperdrivepy-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperdrivepy
-Version: 0.9.2
+Version: 1.0.1
 Project-URL: Homepage, https://github.com/delvtech/hyperdrive-bindings
 Project-URL: Issues, https://github.com/delvtech/hyperdrive-bindings/issues
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `hyperdrivepy-0.9.2/pyproject.toml` & `hyperdrivepy-1.0.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hyperdrivepy"
-version = "0.9.2"
+version = "1.0.1"
 requires-python = ">=3.7"
 classifiers = [
   "Programming Language :: Rust",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 readme = "README.md"
```

### Comparing `hyperdrivepy-0.9.2/python/hyperdrivepy/hyperdrive_state.py` & `hyperdrivepy-1.0.1/python/hyperdrivepy/hyperdrive_state.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from . import types
 from .utils import _get_interface
 
 # We don't control the number of arguments when wrapping rust functions.
 # pylint: disable=too-many-arguments
 
 
-def get_max_spot_price(
+def calculate_max_spot_price(
     pool_config: types.PoolConfigType,
     pool_info: types.PoolInfoType,
 ) -> str:
     """Get the pool's max spot price.
 
     Arguments
     ---------
@@ -25,45 +25,78 @@
         Includes attributes like reserve levels and share prices.
 
     Returns
     -------
     str (FixedPoint)
         max_spot_price = 1/1 + curve_fee * (1 / (spot_price - 1))
     """
-    return _get_interface(pool_config, pool_info).get_max_spot_price()
+    return _get_interface(pool_config, pool_info).calculate_max_spot_price()
 
 
-def get_spot_price_after_long(
+def calculate_spot_price_after_long(
     pool_config: types.PoolConfigType,
     pool_info: types.PoolInfoType,
-    long_amount: str,
+    base_amount: str,
+    bond_amount: str | None = None,
 ) -> str:
-    """Get the spot price after opening the long on YieldSpace
-    and before calculating the fees.
+    """Get the spot price after opening a long on Hyperdrive, including fees.
 
     Arguments
     ---------
     pool_config: PoolConfig
         Static configuration for the hyperdrive contract.
         Set at deploy time.
     pool_info: PoolInfo
         Current state information of the hyperdrive contract.
         Includes attributes like reserve levels and share prices.
-    long_amount: str (FixedPoint)
-        The long amount.
+    base_amount: str (FixedPoint)
+        The amount base provided.
+    bond_amount: str (FixedPoint) | None, optional
+        The number of bonds purchased.
+        Defaults to the output of `calculate_open_long(base_amount)`.
 
     Returns
     -------
     str (FixedPoint)
         The spot price after opening the long.
     """
-    return _get_interface(pool_config, pool_info).get_spot_price_after_long(long_amount)
+    return _get_interface(pool_config, pool_info).calculate_spot_price_after_long(base_amount, bond_amount)
 
 
-def get_solvency(
+def calculate_spot_price_after_short(
+    pool_config: types.PoolConfigType,
+    pool_info: types.PoolInfoType,
+    bond_amount: str,
+    base_amount: str | None = None,
+) -> str:
+    """Get the spot price after opening a short on Hyperdrive, including fees.
+
+    Arguments
+    ---------
+    pool_config: PoolConfig
+        Static configuration for the hyperdrive contract.
+        Set at deploy time.
+    pool_info: PoolInfo
+        Current state information of the hyperdrive contract.
+        Includes attributes like reserve levels and share prices.
+    bond_amount: str (FixedPoint)
+        The amount bonds shorted.
+    base_amount: str (FixedPoint) | None, optional
+        The amount of base supplied.
+        Defaults to the output of `calculate_open_short(bond_amount)`.
+
+    Returns
+    -------
+    str (FixedPoint)
+        The spot price after opening the long.
+    """
+    return _get_interface(pool_config, pool_info).calculate_spot_price_after_short(bond_amount, base_amount)
+
+
+def calculate_solvency(
     pool_config: types.PoolConfigType,
     pool_info: types.PoolInfoType,
 ) -> str:
     """Get the pool's solvency.
 
     Arguments
     ---------
@@ -75,18 +108,48 @@
         Includes attributes like reserve levels and share prices.
 
     Returns
     -------
     str (FixedPoint)
         solvency = share_reserves - long_exposure / vault_share_price - minimum_share_reserves
     """
-    return _get_interface(pool_config, pool_info).get_solvency()
+    return _get_interface(pool_config, pool_info).calculate_solvency()
 
 
-def get_spot_rate(
+def calculate_spot_rate_after_long(
+    pool_config: types.PoolConfigType,
+    pool_info: types.PoolInfoType,
+    base_amount: str,
+    bond_amount: str | None = None,
+) -> str:
+    """Get the spot rate after opening a long on Hyperdrive, including fees.
+
+    Arguments
+    ---------
+    pool_config: PoolConfig
+        Static configuration for the hyperdrive contract.
+        Set at deploy time.
+    pool_info: PoolInfo
+        Current state information of the hyperdrive contract.
+        Includes attributes like reserve levels and share prices.
+    base_amount: str (FixedPoint)
+        The amount base provided.
+    bond_amount: str (FixedPoint) | None, optional
+        The number of bonds purchased.
+        Defaults to the output of `calculate_open_long(base_amount)`.
+
+    Returns
+    -------
+    str (FixedPoint)
+        The spot rate after opening the long.
+    """
+    return _get_interface(pool_config, pool_info).calculate_spot_rate_after_long(base_amount, bond_amount)
+
+
+def calculate_spot_rate(
     pool_config: types.PoolConfigType,
     pool_info: types.PoolInfoType,
 ) -> str:
     """Get the spot rate (fixed rate) for the market.
 
     Arguments
     ---------
@@ -98,18 +161,18 @@
         Includes attributes like reserve levels and share prices.
 
     Returns
     -------
     str (FixedPoint)
         The pool's spot rate.
     """
-    return _get_interface(pool_config, pool_info).get_spot_rate()
+    return _get_interface(pool_config, pool_info).calculate_spot_rate()
 
 
-def get_spot_price(
+def calculate_spot_price(
     pool_config: types.PoolConfigType,
     pool_info: types.PoolInfoType,
 ) -> str:
     """Get the spot price of the bond.
 
     Arguments
     ---------
@@ -121,15 +184,15 @@
         Includes attributes like reserve levels and share prices.
 
     Returns
     -------
     str (FixedPoint)
         The pool's spot price.
     """
-    return _get_interface(pool_config, pool_info).get_spot_price()
+    return _get_interface(pool_config, pool_info).calculate_spot_price()
 
 
 def calculate_open_long(
     pool_config: types.PoolConfigType,
     pool_info: types.PoolInfoType,
     base_amount: str,
 ) -> str:
@@ -154,37 +217,40 @@
     return _get_interface(pool_config, pool_info).calculate_open_long(base_amount)
 
 
 def calculate_close_long(
     pool_config: types.PoolConfigType,
     pool_info: types.PoolInfoType,
     bond_amount: str,
-    normalized_time_remaining: str,
+    maturity_time: str,
+    current_time: str,
 ) -> str:
     """Calculates the amount of shares that will be returned after fees for closing a long.
 
     Arguments
     ---------
     pool_config: PoolConfig
         Static configuration for the hyperdrive contract.
         Set at deploy time.
     pool_info: PoolInfo
         Current state information of the hyperdrive contract.
         Includes attributes like reserve levels and share prices.
     bond_amount: str (FixedPoint)
         The amount of bonds to sell.
-    normalized_time_remaining: str (FixedPoint)
-        The time remaining before the long reaches maturity, normalized such that 1 is at opening and 0 is at maturity.
+    maturity_time: str (FixedPoint)
+        The maturity time of the long.
+    current_time: str (FixedPoint)
+        The current block time.
 
     Returns
     -------
     str (FixedPoint)
         The amount of shares returned.
     """
-    return _get_interface(pool_config, pool_info).calculate_close_long(bond_amount, normalized_time_remaining)
+    return _get_interface(pool_config, pool_info).calculate_close_long(bond_amount, maturity_time, current_time)
 
 
 def calculate_open_short(
     pool_config: types.PoolConfigType,
     pool_info: types.PoolInfoType,
     short_amount: str,
     spot_price: str,
@@ -222,15 +288,16 @@
 
 def calculate_close_short(
     pool_config: types.PoolConfigType,
     pool_info: types.PoolInfoType,
     bond_amount: str,
     open_vault_share_price: str,
     close_vault_share_price: str,
-    normalized_time_remaining: str,
+    maturity_time: str,
+    current_time: str,
 ) -> str:
     """Gets the amount of shares the trader will receive from closing a short.
 
     Arguments
     ---------
     pool_config: PoolConfig
         Static configuration for the hyperdrive contract.
@@ -240,24 +307,26 @@
         Includes attributes like reserve levels and share prices.
     bond_amount: str (FixedPoint)
         The amount to of bonds provided.
     open_vault_share_price: str (FixedPoint)
         The share price when the short was opened.
     close_vault_share_price: str (FixedPoint)
         The share price when the short was closed.
-    normalized_time_remaining: str (FixedPoint)
-        The time remaining before the short reaches maturity, normalized such that 1 is at opening and 0 is at maturity.
+    maturity_time: str (FixedPoint)
+        The maturity time of the long.
+    current_time: str (FixedPoint)
+        The current block time.
 
     Returns
     -------
     str (FixedPoint)
         The amount of shares the trader will receive for closing the short.
     """
     return _get_interface(pool_config, pool_info).calculate_close_short(
-        bond_amount, open_vault_share_price, close_vault_share_price, normalized_time_remaining
+        bond_amount, open_vault_share_price, close_vault_share_price, maturity_time, current_time
     )
 
 
 def to_checkpoint(
     pool_config: types.PoolConfigType,
     pool_info: types.PoolInfoType,
     time: str,
@@ -279,15 +348,60 @@
     -------
     str (U256)
         The checkpoint timestamp.
     """
     return _get_interface(pool_config, pool_info).to_checkpoint(time)
 
 
-def get_max_long(
+def calculate_targeted_long(
+    pool_config: types.PoolConfigType,
+    pool_info: types.PoolInfoType,
+    budget: str,
+    target_rate: str,
+    checkpoint_exposure: str,
+    maybe_max_iterations: int | None,
+    maybe_allowable_error: str,
+) -> str:
+    """Calculate the amount of bonds that can be purchased for the given budget.
+
+    Arguments
+    ---------
+    pool_config: PoolConfig
+        Static configuration for the hyperdrive contract.
+        Set at deploy time.
+    pool_info: PoolInfo
+        Current state information of the hyperdrive contract.
+        Includes attributes like reserve levels and share prices.
+    budget: str (FixedPont)
+        The account budget in base for making a long.
+    target: str (FixedPoint)
+        The target fixed rate.
+    checkpoint_exposure: str (I256)
+        The net exposure for the given checkpoint.
+    maybe_max_iterations: int, optional
+        The number of iterations to use for the Newtonian method.
+    maybe_allowable_error: str, FixedPoint
+        The amount of error supported for reaching the target rate.
+
+
+    Returns
+    -------
+    str (FixedPoint)
+        The long to hit the target rate.
+    """
+    return _get_interface(pool_config, pool_info).calculate_targeted_long_with_budget(
+        budget,
+        target_rate,
+        checkpoint_exposure,
+        maybe_max_iterations,
+        maybe_allowable_error,
+    )
+
+
+def calculate_max_long(
     pool_config: types.PoolConfigType,
     pool_info: types.PoolInfoType,
     budget: str,
     checkpoint_exposure: str,
     maybe_max_iterations: int | None,
 ) -> str:
     """Get the max amount of bonds that can be purchased for the given budget.
@@ -308,18 +422,18 @@
         The number of iterations to use for the Newtonian method.
 
     Returns
     -------
     str (FixedPoint)
         The maximum long the pool and user's wallet can support.
     """
-    return _get_interface(pool_config, pool_info).get_max_long(budget, checkpoint_exposure, maybe_max_iterations)
+    return _get_interface(pool_config, pool_info).calculate_max_long(budget, checkpoint_exposure, maybe_max_iterations)
 
 
-def get_max_short(
+def calculate_max_short(
     pool_config: types.PoolConfigType,
     pool_info: types.PoolInfoType,
     budget: str,
     open_vault_share_price: str,
     checkpoint_exposure: str,
     maybe_conservative_price: str | None,
     maybe_max_iterations: int | None,
@@ -346,15 +460,15 @@
         The number of iterations to use for the Newtonian method.
 
     Returns
     -------
     str (FixedPoint)
         The maximum short the pool and user's wallet can handle.
     """
-    return _get_interface(pool_config, pool_info).get_max_short(
+    return _get_interface(pool_config, pool_info).calculate_max_short(
         budget,
         open_vault_share_price,
         checkpoint_exposure,
         maybe_conservative_price,
         maybe_max_iterations,
     )
 
@@ -491,7 +605,30 @@
 
     Returns
     -------
     str (FixedPoint)
         The present value of all LP capital in the pool.
     """
     return _get_interface(pool_config, pool_info).calculate_present_value(current_block_timestamp)
+
+
+def calculate_idle_share_reserves_in_base(
+    pool_config: types.PoolConfigType,
+    pool_info: types.PoolInfoType,
+) -> str:
+    """Calculates the idle share reserves in base of the pool.
+
+    Arguments
+    ---------
+    pool_config: PoolConfig
+        Static configuration for the hyperdrive contract.
+        Set at deploy time.
+    pool_info: PoolInfo
+        Current state information of the hyperdrive contract.
+        Includes attributes like reserve levels and share prices.
+
+    Returns
+    -------
+    str (FixedPoint)
+        The idle share reserves in base of the pool.
+    """
+    return _get_interface(pool_config, pool_info).calculate_idle_share_reserves_in_base()
```

### Comparing `hyperdrivepy-0.9.2/python/hyperdrivepy/hyperdrive_utils.py` & `hyperdrivepy-1.0.1/python/hyperdrivepy/hyperdrive_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import annotations
 
 # pylint: disable=no-name-in-module
 from . import hyperdrivepy as rust_module  # type: ignore
 
 
-def get_time_stretch(rate: str, position_duration: str) -> str:
+def calculate_time_stretch(rate: str, position_duration: str) -> str:
     """Calculate the time stretch parameter given a pool's spot rate.
 
     ..math::
         tau = 5.24592 / (0.4665 * r * 100)
 
     Arguments
     ---------
@@ -20,18 +20,18 @@
         The amount of time before a trade matures.
 
     Returns
     -------
     time_stretch: str (FixedPoint)
         The time stretch parameter (tau).
     """
-    return rust_module.get_time_stretch(rate, position_duration)
+    return rust_module.calculate_time_stretch(rate, position_duration)
 
 
-def get_effective_share_reserves(
+def calculate_effective_share_reserves(
     share_reserves: str,
     share_adjustment: str,
 ) -> str:
     r"""Calculate the effective share reserves given the share reserves and share adjustment.
 
     ..math::
         z_effective = z - \zeta
@@ -44,15 +44,15 @@
         The zeta factor for adjusting share reserves.
 
     Returns
     -------
     effective_share_reserves: str (FixedPoint)
         The adjusted share reserves, accounting for the zeta factor.
     """
-    return rust_module.get_effective_share_reserves(share_reserves, share_adjustment)
+    return rust_module.calculate_effective_share_reserves(share_reserves, share_adjustment)
 
 
 def calculate_initial_bond_reserves(
     effective_share_reserves: str,
     initial_vault_share_price: str,
     apr: str,
     position_duration: str,
```

### Comparing `hyperdrivepy-0.9.2/python/hyperdrivepy/pypechain_types/IERC4626HyperdriveContract.py` & `hyperdrivepy-1.0.1/python/hyperdrivepy/pypechain_types/IHyperdriveContract.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""A web3.py Contract class for the IERC4626Hyperdrive contract.
+"""A web3.py Contract class for the IHyperdrive contract.
 
 DO NOT EDIT.  This file was generated by pypechain.  See documentation at
 https://github.com/delvtech/pypechain"""
 
 # contracts have PascalCase names
 # pylint: disable=invalid-name
 
@@ -57,18 +57,18 @@
     "Fees": Fees,
     "PoolConfig": PoolConfig,
     "PoolInfo": PoolInfo,
     "WithdrawPool": WithdrawPool,
 }
 
 
-class IERC4626HyperdrivePERMIT_TYPEHASHContractFunction(ContractFunction):
+class IHyperdrivePERMIT_TYPEHASHContractFunction(ContractFunction):
     """ContractFunction for the PERMIT_TYPEHASH method."""
 
-    def __call__(self) -> IERC4626HyperdrivePERMIT_TYPEHASHContractFunction:  # type: ignore
+    def __call__(self) -> IHyperdrivePERMIT_TYPEHASHContractFunction:  # type: ignore
         clone = super().__call__()
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
     def call(
         self,
@@ -84,18 +84,18 @@
 
         # Call the function
 
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
         return cast(bytes, rename_returned_types(structs, return_types, raw_values))
 
 
-class IERC4626HyperdriveAddLiquidityContractFunction(ContractFunction):
+class IHyperdriveAddLiquidityContractFunction(ContractFunction):
     """ContractFunction for the addLiquidity method."""
 
-    def __call__(self, contribution: int, minLpSharePrice: int, minApr: int, maxApr: int, options: Options) -> IERC4626HyperdriveAddLiquidityContractFunction:  # type: ignore
+    def __call__(self, contribution: int, minLpSharePrice: int, minApr: int, maxApr: int, options: Options) -> IHyperdriveAddLiquidityContractFunction:  # type: ignore
         clone = super().__call__(
             dataclass_to_tuple(contribution),
             dataclass_to_tuple(minLpSharePrice),
             dataclass_to_tuple(minApr),
             dataclass_to_tuple(maxApr),
             dataclass_to_tuple(options),
         )
@@ -117,18 +117,18 @@
 
         # Call the function
 
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
         return cast(int, rename_returned_types(structs, return_types, raw_values))
 
 
-class IERC4626HyperdriveBalanceOfContractFunction(ContractFunction):
+class IHyperdriveBalanceOfContractFunction(ContractFunction):
     """ContractFunction for the balanceOf method."""
 
-    def __call__(self, tokenId: int, owner: str) -> IERC4626HyperdriveBalanceOfContractFunction:  # type: ignore
+    def __call__(self, tokenId: int, owner: str) -> IHyperdriveBalanceOfContractFunction:  # type: ignore
         clone = super().__call__(dataclass_to_tuple(tokenId), dataclass_to_tuple(owner))
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
     def call(
         self,
@@ -144,18 +144,18 @@
 
         # Call the function
 
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
         return cast(int, rename_returned_types(structs, return_types, raw_values))
 
 
-class IERC4626HyperdriveBaseTokenContractFunction(ContractFunction):
+class IHyperdriveBaseTokenContractFunction(ContractFunction):
     """ContractFunction for the baseToken method."""
 
-    def __call__(self) -> IERC4626HyperdriveBaseTokenContractFunction:  # type: ignore
+    def __call__(self) -> IHyperdriveBaseTokenContractFunction:  # type: ignore
         clone = super().__call__()
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
     def call(
         self,
@@ -171,18 +171,18 @@
 
         # Call the function
 
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
         return cast(str, rename_returned_types(structs, return_types, raw_values))
 
 
-class IERC4626HyperdriveBatchTransferFromContractFunction(ContractFunction):
+class IHyperdriveBatchTransferFromContractFunction(ContractFunction):
     """ContractFunction for the batchTransferFrom method."""
 
-    def __call__(self, _from: str, to: str, ids: list[int], values: list[int]) -> IERC4626HyperdriveBatchTransferFromContractFunction:  # type: ignore
+    def __call__(self, _from: str, to: str, ids: list[int], values: list[int]) -> IHyperdriveBatchTransferFromContractFunction:  # type: ignore
         clone = super().__call__(
             dataclass_to_tuple(_from), dataclass_to_tuple(to), dataclass_to_tuple(ids), dataclass_to_tuple(values)
         )
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
@@ -195,19 +195,19 @@
     ) -> None:
         """returns None."""
         # Define the expected return types from the smart contract call
 
         # Call the function
 
 
-class IERC4626HyperdriveCheckpointContractFunction(ContractFunction):
+class IHyperdriveCheckpointContractFunction(ContractFunction):
     """ContractFunction for the checkpoint method."""
 
-    def __call__(self, checkpointTime: int) -> IERC4626HyperdriveCheckpointContractFunction:  # type: ignore
-        clone = super().__call__(dataclass_to_tuple(checkpointTime))
+    def __call__(self, checkpointTime: int, maxIterations: int) -> IHyperdriveCheckpointContractFunction:  # type: ignore
+        clone = super().__call__(dataclass_to_tuple(checkpointTime), dataclass_to_tuple(maxIterations))
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
     def call(
         self,
         transaction: TxParams | None = None,
@@ -217,18 +217,18 @@
     ) -> None:
         """returns None."""
         # Define the expected return types from the smart contract call
 
         # Call the function
 
 
-class IERC4626HyperdriveCloseLongContractFunction(ContractFunction):
+class IHyperdriveCloseLongContractFunction(ContractFunction):
     """ContractFunction for the closeLong method."""
 
-    def __call__(self, maturityTime: int, bondAmount: int, minOutput: int, options: Options) -> IERC4626HyperdriveCloseLongContractFunction:  # type: ignore
+    def __call__(self, maturityTime: int, bondAmount: int, minOutput: int, options: Options) -> IHyperdriveCloseLongContractFunction:  # type: ignore
         clone = super().__call__(
             dataclass_to_tuple(maturityTime),
             dataclass_to_tuple(bondAmount),
             dataclass_to_tuple(minOutput),
             dataclass_to_tuple(options),
         )
         self.kwargs = clone.kwargs
@@ -249,18 +249,18 @@
 
         # Call the function
 
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
         return cast(int, rename_returned_types(structs, return_types, raw_values))
 
 
-class IERC4626HyperdriveCloseShortContractFunction(ContractFunction):
+class IHyperdriveCloseShortContractFunction(ContractFunction):
     """ContractFunction for the closeShort method."""
 
-    def __call__(self, maturityTime: int, bondAmount: int, minOutput: int, options: Options) -> IERC4626HyperdriveCloseShortContractFunction:  # type: ignore
+    def __call__(self, maturityTime: int, bondAmount: int, minOutput: int, options: Options) -> IHyperdriveCloseShortContractFunction:  # type: ignore
         clone = super().__call__(
             dataclass_to_tuple(maturityTime),
             dataclass_to_tuple(bondAmount),
             dataclass_to_tuple(minOutput),
             dataclass_to_tuple(options),
         )
         self.kwargs = clone.kwargs
@@ -281,18 +281,18 @@
 
         # Call the function
 
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
         return cast(int, rename_returned_types(structs, return_types, raw_values))
 
 
-class IERC4626HyperdriveCollectGovernanceFeeContractFunction(ContractFunction):
+class IHyperdriveCollectGovernanceFeeContractFunction(ContractFunction):
     """ContractFunction for the collectGovernanceFee method."""
 
-    def __call__(self, options: Options) -> IERC4626HyperdriveCollectGovernanceFeeContractFunction:  # type: ignore
+    def __call__(self, options: Options) -> IHyperdriveCollectGovernanceFeeContractFunction:  # type: ignore
         clone = super().__call__(dataclass_to_tuple(options))
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
     def call(
         self,
@@ -308,18 +308,18 @@
 
         # Call the function
 
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
         return cast(int, rename_returned_types(structs, return_types, raw_values))
 
 
-class IERC4626HyperdriveDecimalsContractFunction(ContractFunction):
+class IHyperdriveDecimalsContractFunction(ContractFunction):
     """ContractFunction for the decimals method."""
 
-    def __call__(self) -> IERC4626HyperdriveDecimalsContractFunction:  # type: ignore
+    def __call__(self) -> IHyperdriveDecimalsContractFunction:  # type: ignore
         clone = super().__call__()
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
     def call(
         self,
@@ -335,18 +335,18 @@
 
         # Call the function
 
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
         return cast(int, rename_returned_types(structs, return_types, raw_values))
 
 
-class IERC4626HyperdriveDomainSeparatorContractFunction(ContractFunction):
+class IHyperdriveDomainSeparatorContractFunction(ContractFunction):
     """ContractFunction for the domainSeparator method."""
 
-    def __call__(self) -> IERC4626HyperdriveDomainSeparatorContractFunction:  # type: ignore
+    def __call__(self) -> IHyperdriveDomainSeparatorContractFunction:  # type: ignore
         clone = super().__call__()
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
     def call(
         self,
@@ -362,18 +362,18 @@
 
         # Call the function
 
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
         return cast(bytes, rename_returned_types(structs, return_types, raw_values))
 
 
-class IERC4626HyperdriveGetCheckpointContractFunction(ContractFunction):
+class IHyperdriveGetCheckpointContractFunction(ContractFunction):
     """ContractFunction for the getCheckpoint method."""
 
-    def __call__(self, checkpointTime: int) -> IERC4626HyperdriveGetCheckpointContractFunction:  # type: ignore
+    def __call__(self, checkpointTime: int) -> IHyperdriveGetCheckpointContractFunction:  # type: ignore
         clone = super().__call__(dataclass_to_tuple(checkpointTime))
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
     def call(
         self,
@@ -389,18 +389,18 @@
 
         # Call the function
 
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
         return cast(Checkpoint, rename_returned_types(structs, return_types, raw_values))
 
 
-class IERC4626HyperdriveGetCheckpointExposureContractFunction(ContractFunction):
+class IHyperdriveGetCheckpointExposureContractFunction(ContractFunction):
     """ContractFunction for the getCheckpointExposure method."""
 
-    def __call__(self, checkpointTime: int) -> IERC4626HyperdriveGetCheckpointExposureContractFunction:  # type: ignore
+    def __call__(self, checkpointTime: int) -> IHyperdriveGetCheckpointExposureContractFunction:  # type: ignore
         clone = super().__call__(dataclass_to_tuple(checkpointTime))
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
     def call(
         self,
@@ -416,18 +416,18 @@
 
         # Call the function
 
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
         return cast(int, rename_returned_types(structs, return_types, raw_values))
 
 
-class IERC4626HyperdriveGetMarketStateContractFunction(ContractFunction):
+class IHyperdriveGetMarketStateContractFunction(ContractFunction):
     """ContractFunction for the getMarketState method."""
 
-    def __call__(self) -> IERC4626HyperdriveGetMarketStateContractFunction:  # type: ignore
+    def __call__(self) -> IHyperdriveGetMarketStateContractFunction:  # type: ignore
         clone = super().__call__()
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
     def call(
         self,
@@ -443,18 +443,18 @@
 
         # Call the function
 
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
         return cast(MarketState, rename_returned_types(structs, return_types, raw_values))
 
 
-class IERC4626HyperdriveGetPoolConfigContractFunction(ContractFunction):
+class IHyperdriveGetPoolConfigContractFunction(ContractFunction):
     """ContractFunction for the getPoolConfig method."""
 
-    def __call__(self) -> IERC4626HyperdriveGetPoolConfigContractFunction:  # type: ignore
+    def __call__(self) -> IHyperdriveGetPoolConfigContractFunction:  # type: ignore
         clone = super().__call__()
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
     def call(
         self,
@@ -470,18 +470,18 @@
 
         # Call the function
 
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
         return cast(PoolConfig, rename_returned_types(structs, return_types, raw_values))
 
 
-class IERC4626HyperdriveGetPoolInfoContractFunction(ContractFunction):
+class IHyperdriveGetPoolInfoContractFunction(ContractFunction):
     """ContractFunction for the getPoolInfo method."""
 
-    def __call__(self) -> IERC4626HyperdriveGetPoolInfoContractFunction:  # type: ignore
+    def __call__(self) -> IHyperdriveGetPoolInfoContractFunction:  # type: ignore
         clone = super().__call__()
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
     def call(
         self,
@@ -497,18 +497,18 @@
 
         # Call the function
 
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
         return cast(PoolInfo, rename_returned_types(structs, return_types, raw_values))
 
 
-class IERC4626HyperdriveGetUncollectedGovernanceFeesContractFunction(ContractFunction):
+class IHyperdriveGetUncollectedGovernanceFeesContractFunction(ContractFunction):
     """ContractFunction for the getUncollectedGovernanceFees method."""
 
-    def __call__(self) -> IERC4626HyperdriveGetUncollectedGovernanceFeesContractFunction:  # type: ignore
+    def __call__(self) -> IHyperdriveGetUncollectedGovernanceFeesContractFunction:  # type: ignore
         clone = super().__call__()
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
     def call(
         self,
@@ -524,18 +524,18 @@
 
         # Call the function
 
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
         return cast(int, rename_returned_types(structs, return_types, raw_values))
 
 
-class IERC4626HyperdriveGetWithdrawPoolContractFunction(ContractFunction):
+class IHyperdriveGetWithdrawPoolContractFunction(ContractFunction):
     """ContractFunction for the getWithdrawPool method."""
 
-    def __call__(self) -> IERC4626HyperdriveGetWithdrawPoolContractFunction:  # type: ignore
+    def __call__(self) -> IHyperdriveGetWithdrawPoolContractFunction:  # type: ignore
         clone = super().__call__()
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
     def call(
         self,
@@ -551,18 +551,18 @@
 
         # Call the function
 
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
         return cast(WithdrawPool, rename_returned_types(structs, return_types, raw_values))
 
 
-class IERC4626HyperdriveInitializeContractFunction(ContractFunction):
+class IHyperdriveInitializeContractFunction(ContractFunction):
     """ContractFunction for the initialize method."""
 
-    def __call__(self, contribution: int, apr: int, options: Options) -> IERC4626HyperdriveInitializeContractFunction:  # type: ignore
+    def __call__(self, contribution: int, apr: int, options: Options) -> IHyperdriveInitializeContractFunction:  # type: ignore
         clone = super().__call__(dataclass_to_tuple(contribution), dataclass_to_tuple(apr), dataclass_to_tuple(options))
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
     def call(
         self,
@@ -578,18 +578,18 @@
 
         # Call the function
 
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
         return cast(int, rename_returned_types(structs, return_types, raw_values))
 
 
-class IERC4626HyperdriveIsApprovedForAllContractFunction(ContractFunction):
+class IHyperdriveIsApprovedForAllContractFunction(ContractFunction):
     """ContractFunction for the isApprovedForAll method."""
 
-    def __call__(self, owner: str, spender: str) -> IERC4626HyperdriveIsApprovedForAllContractFunction:  # type: ignore
+    def __call__(self, owner: str, spender: str) -> IHyperdriveIsApprovedForAllContractFunction:  # type: ignore
         clone = super().__call__(dataclass_to_tuple(owner), dataclass_to_tuple(spender))
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
     def call(
         self,
@@ -605,18 +605,18 @@
 
         # Call the function
 
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
         return cast(bool, rename_returned_types(structs, return_types, raw_values))
 
 
-class IERC4626HyperdriveIsPauserContractFunction(ContractFunction):
+class IHyperdriveIsPauserContractFunction(ContractFunction):
     """ContractFunction for the isPauser method."""
 
-    def __call__(self, account: str) -> IERC4626HyperdriveIsPauserContractFunction:  # type: ignore
+    def __call__(self, account: str) -> IHyperdriveIsPauserContractFunction:  # type: ignore
         clone = super().__call__(dataclass_to_tuple(account))
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
     def call(
         self,
@@ -632,18 +632,18 @@
 
         # Call the function
 
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
         return cast(bool, rename_returned_types(structs, return_types, raw_values))
 
 
-class IERC4626HyperdriveLoadContractFunction(ContractFunction):
+class IHyperdriveLoadContractFunction(ContractFunction):
     """ContractFunction for the load method."""
 
-    def __call__(self, slots: list[int]) -> IERC4626HyperdriveLoadContractFunction:  # type: ignore
+    def __call__(self, slots: list[int]) -> IHyperdriveLoadContractFunction:  # type: ignore
         clone = super().__call__(dataclass_to_tuple(slots))
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
     def call(
         self,
@@ -659,18 +659,18 @@
 
         # Call the function
 
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
         return cast(list[bytes], rename_returned_types(structs, return_types, raw_values))
 
 
-class IERC4626HyperdriveNameContractFunction(ContractFunction):
+class IHyperdriveNameContractFunction(ContractFunction):
     """ContractFunction for the name method."""
 
-    def __call__(self, tokenId: int) -> IERC4626HyperdriveNameContractFunction:  # type: ignore
+    def __call__(self, tokenId: int) -> IHyperdriveNameContractFunction:  # type: ignore
         clone = super().__call__(dataclass_to_tuple(tokenId))
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
     def call(
         self,
@@ -686,18 +686,18 @@
 
         # Call the function
 
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
         return cast(str, rename_returned_types(structs, return_types, raw_values))
 
 
-class IERC4626HyperdriveNoncesContractFunction(ContractFunction):
+class IHyperdriveNoncesContractFunction(ContractFunction):
     """ContractFunction for the nonces method."""
 
-    def __call__(self, owner: str) -> IERC4626HyperdriveNoncesContractFunction:  # type: ignore
+    def __call__(self, owner: str) -> IHyperdriveNoncesContractFunction:  # type: ignore
         clone = super().__call__(dataclass_to_tuple(owner))
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
     def call(
         self,
@@ -713,24 +713,24 @@
 
         # Call the function
 
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
         return cast(int, rename_returned_types(structs, return_types, raw_values))
 
 
-class IERC4626HyperdriveOpenLongContractFunction(ContractFunction):
+class IHyperdriveOpenLongContractFunction(ContractFunction):
     """ContractFunction for the openLong method."""
 
     class ReturnValues(NamedTuple):
         """The return named tuple for OpenLong."""
 
-        arg1: int
-        arg2: int
+        maturityTime: int
+        bondProceeds: int
 
-    def __call__(self, amount: int, minOutput: int, minVaultSharePrice: int, options: Options) -> IERC4626HyperdriveOpenLongContractFunction:  # type: ignore
+    def __call__(self, amount: int, minOutput: int, minVaultSharePrice: int, options: Options) -> IHyperdriveOpenLongContractFunction:  # type: ignore
         clone = super().__call__(
             dataclass_to_tuple(amount),
             dataclass_to_tuple(minOutput),
             dataclass_to_tuple(minVaultSharePrice),
             dataclass_to_tuple(options),
         )
         self.kwargs = clone.kwargs
@@ -751,24 +751,24 @@
 
         # Call the function
 
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
         return self.ReturnValues(*rename_returned_types(structs, return_types, raw_values))
 
 
-class IERC4626HyperdriveOpenShortContractFunction(ContractFunction):
+class IHyperdriveOpenShortContractFunction(ContractFunction):
     """ContractFunction for the openShort method."""
 
     class ReturnValues(NamedTuple):
         """The return named tuple for OpenShort."""
 
-        arg1: int
-        arg2: int
+        maturityTime: int
+        deposit: int
 
-    def __call__(self, bondAmount: int, maxDeposit: int, minVaultSharePrice: int, options: Options) -> IERC4626HyperdriveOpenShortContractFunction:  # type: ignore
+    def __call__(self, bondAmount: int, maxDeposit: int, minVaultSharePrice: int, options: Options) -> IHyperdriveOpenShortContractFunction:  # type: ignore
         clone = super().__call__(
             dataclass_to_tuple(bondAmount),
             dataclass_to_tuple(maxDeposit),
             dataclass_to_tuple(minVaultSharePrice),
             dataclass_to_tuple(options),
         )
         self.kwargs = clone.kwargs
@@ -789,18 +789,18 @@
 
         # Call the function
 
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
         return self.ReturnValues(*rename_returned_types(structs, return_types, raw_values))
 
 
-class IERC4626HyperdrivePauseContractFunction(ContractFunction):
+class IHyperdrivePauseContractFunction(ContractFunction):
     """ContractFunction for the pause method."""
 
-    def __call__(self, status: bool) -> IERC4626HyperdrivePauseContractFunction:  # type: ignore
+    def __call__(self, status: bool) -> IHyperdrivePauseContractFunction:  # type: ignore
         clone = super().__call__(dataclass_to_tuple(status))
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
     def call(
         self,
@@ -811,18 +811,18 @@
     ) -> None:
         """returns None."""
         # Define the expected return types from the smart contract call
 
         # Call the function
 
 
-class IERC4626HyperdrivePerTokenApprovalsContractFunction(ContractFunction):
+class IHyperdrivePerTokenApprovalsContractFunction(ContractFunction):
     """ContractFunction for the perTokenApprovals method."""
 
-    def __call__(self, tokenId: int, owner: str, spender: str) -> IERC4626HyperdrivePerTokenApprovalsContractFunction:  # type: ignore
+    def __call__(self, tokenId: int, owner: str, spender: str) -> IHyperdrivePerTokenApprovalsContractFunction:  # type: ignore
         clone = super().__call__(dataclass_to_tuple(tokenId), dataclass_to_tuple(owner), dataclass_to_tuple(spender))
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
     def call(
         self,
@@ -838,18 +838,18 @@
 
         # Call the function
 
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
         return cast(int, rename_returned_types(structs, return_types, raw_values))
 
 
-class IERC4626HyperdrivePermitForAllContractFunction(ContractFunction):
+class IHyperdrivePermitForAllContractFunction(ContractFunction):
     """ContractFunction for the permitForAll method."""
 
-    def __call__(self, owner: str, spender: str, approved: bool, deadline: int, v: int, r: bytes, s: bytes) -> IERC4626HyperdrivePermitForAllContractFunction:  # type: ignore
+    def __call__(self, owner: str, spender: str, approved: bool, deadline: int, v: int, r: bytes, s: bytes) -> IHyperdrivePermitForAllContractFunction:  # type: ignore
         clone = super().__call__(
             dataclass_to_tuple(owner),
             dataclass_to_tuple(spender),
             dataclass_to_tuple(approved),
             dataclass_to_tuple(deadline),
             dataclass_to_tuple(v),
             dataclass_to_tuple(r),
@@ -868,24 +868,24 @@
     ) -> None:
         """returns None."""
         # Define the expected return types from the smart contract call
 
         # Call the function
 
 
-class IERC4626HyperdriveRedeemWithdrawalSharesContractFunction(ContractFunction):
+class IHyperdriveRedeemWithdrawalSharesContractFunction(ContractFunction):
     """ContractFunction for the redeemWithdrawalShares method."""
 
     class ReturnValues(NamedTuple):
         """The return named tuple for RedeemWithdrawalShares."""
 
-        arg1: int
-        arg2: int
+        proceeds: int
+        withdrawalSharesRedeemed: int
 
-    def __call__(self, withdrawalShares: int, minOutputPerShare: int, options: Options) -> IERC4626HyperdriveRedeemWithdrawalSharesContractFunction:  # type: ignore
+    def __call__(self, withdrawalShares: int, minOutputPerShare: int, options: Options) -> IHyperdriveRedeemWithdrawalSharesContractFunction:  # type: ignore
         clone = super().__call__(
             dataclass_to_tuple(withdrawalShares), dataclass_to_tuple(minOutputPerShare), dataclass_to_tuple(options)
         )
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
@@ -903,24 +903,24 @@
 
         # Call the function
 
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
         return self.ReturnValues(*rename_returned_types(structs, return_types, raw_values))
 
 
-class IERC4626HyperdriveRemoveLiquidityContractFunction(ContractFunction):
+class IHyperdriveRemoveLiquidityContractFunction(ContractFunction):
     """ContractFunction for the removeLiquidity method."""
 
     class ReturnValues(NamedTuple):
         """The return named tuple for RemoveLiquidity."""
 
-        arg1: int
-        arg2: int
+        proceeds: int
+        withdrawalShares: int
 
-    def __call__(self, lpShares: int, minOutputPerShare: int, options: Options) -> IERC4626HyperdriveRemoveLiquidityContractFunction:  # type: ignore
+    def __call__(self, lpShares: int, minOutputPerShare: int, options: Options) -> IHyperdriveRemoveLiquidityContractFunction:  # type: ignore
         clone = super().__call__(
             dataclass_to_tuple(lpShares), dataclass_to_tuple(minOutputPerShare), dataclass_to_tuple(options)
         )
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
@@ -938,18 +938,18 @@
 
         # Call the function
 
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
         return self.ReturnValues(*rename_returned_types(structs, return_types, raw_values))
 
 
-class IERC4626HyperdriveSetApprovalContractFunction(ContractFunction):
+class IHyperdriveSetApprovalContractFunction(ContractFunction):
     """ContractFunction for the setApproval method."""
 
-    def __call__(self, tokenID: int, operator: str, amount: int) -> IERC4626HyperdriveSetApprovalContractFunction:  # type: ignore
+    def __call__(self, tokenID: int, operator: str, amount: int) -> IHyperdriveSetApprovalContractFunction:  # type: ignore
         clone = super().__call__(dataclass_to_tuple(tokenID), dataclass_to_tuple(operator), dataclass_to_tuple(amount))
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
     def call(
         self,
@@ -960,18 +960,18 @@
     ) -> None:
         """returns None."""
         # Define the expected return types from the smart contract call
 
         # Call the function
 
 
-class IERC4626HyperdriveSetApprovalBridgeContractFunction(ContractFunction):
+class IHyperdriveSetApprovalBridgeContractFunction(ContractFunction):
     """ContractFunction for the setApprovalBridge method."""
 
-    def __call__(self, tokenID: int, operator: str, amount: int, caller: str) -> IERC4626HyperdriveSetApprovalBridgeContractFunction:  # type: ignore
+    def __call__(self, tokenID: int, operator: str, amount: int, caller: str) -> IHyperdriveSetApprovalBridgeContractFunction:  # type: ignore
         clone = super().__call__(
             dataclass_to_tuple(tokenID),
             dataclass_to_tuple(operator),
             dataclass_to_tuple(amount),
             dataclass_to_tuple(caller),
         )
         self.kwargs = clone.kwargs
@@ -987,18 +987,18 @@
     ) -> None:
         """returns None."""
         # Define the expected return types from the smart contract call
 
         # Call the function
 
 
-class IERC4626HyperdriveSetApprovalForAllContractFunction(ContractFunction):
+class IHyperdriveSetApprovalForAllContractFunction(ContractFunction):
     """ContractFunction for the setApprovalForAll method."""
 
-    def __call__(self, operator: str, approved: bool) -> IERC4626HyperdriveSetApprovalForAllContractFunction:  # type: ignore
+    def __call__(self, operator: str, approved: bool) -> IHyperdriveSetApprovalForAllContractFunction:  # type: ignore
         clone = super().__call__(dataclass_to_tuple(operator), dataclass_to_tuple(approved))
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
     def call(
         self,
@@ -1009,18 +1009,40 @@
     ) -> None:
         """returns None."""
         # Define the expected return types from the smart contract call
 
         # Call the function
 
 
-class IERC4626HyperdriveSetGovernanceContractFunction(ContractFunction):
+class IHyperdriveSetFeeCollectorContractFunction(ContractFunction):
+    """ContractFunction for the setFeeCollector method."""
+
+    def __call__(self, who: str) -> IHyperdriveSetFeeCollectorContractFunction:  # type: ignore
+        clone = super().__call__(dataclass_to_tuple(who))
+        self.kwargs = clone.kwargs
+        self.args = clone.args
+        return self
+
+    def call(
+        self,
+        transaction: TxParams | None = None,
+        block_identifier: BlockIdentifier = "latest",
+        state_override: CallOverride | None = None,
+        ccip_read_enabled: bool | None = None,
+    ) -> None:
+        """returns None."""
+        # Define the expected return types from the smart contract call
+
+        # Call the function
+
+
+class IHyperdriveSetGovernanceContractFunction(ContractFunction):
     """ContractFunction for the setGovernance method."""
 
-    def __call__(self, who: str) -> IERC4626HyperdriveSetGovernanceContractFunction:  # type: ignore
+    def __call__(self, who: str) -> IHyperdriveSetGovernanceContractFunction:  # type: ignore
         clone = super().__call__(dataclass_to_tuple(who))
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
     def call(
         self,
@@ -1031,18 +1053,18 @@
     ) -> None:
         """returns None."""
         # Define the expected return types from the smart contract call
 
         # Call the function
 
 
-class IERC4626HyperdriveSetPauserContractFunction(ContractFunction):
+class IHyperdriveSetPauserContractFunction(ContractFunction):
     """ContractFunction for the setPauser method."""
 
-    def __call__(self, who: str, status: bool) -> IERC4626HyperdriveSetPauserContractFunction:  # type: ignore
+    def __call__(self, who: str, status: bool) -> IHyperdriveSetPauserContractFunction:  # type: ignore
         clone = super().__call__(dataclass_to_tuple(who), dataclass_to_tuple(status))
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
     def call(
         self,
@@ -1053,18 +1075,40 @@
     ) -> None:
         """returns None."""
         # Define the expected return types from the smart contract call
 
         # Call the function
 
 
-class IERC4626HyperdriveSweepContractFunction(ContractFunction):
+class IHyperdriveSetSweepCollectorContractFunction(ContractFunction):
+    """ContractFunction for the setSweepCollector method."""
+
+    def __call__(self, who: str) -> IHyperdriveSetSweepCollectorContractFunction:  # type: ignore
+        clone = super().__call__(dataclass_to_tuple(who))
+        self.kwargs = clone.kwargs
+        self.args = clone.args
+        return self
+
+    def call(
+        self,
+        transaction: TxParams | None = None,
+        block_identifier: BlockIdentifier = "latest",
+        state_override: CallOverride | None = None,
+        ccip_read_enabled: bool | None = None,
+    ) -> None:
+        """returns None."""
+        # Define the expected return types from the smart contract call
+
+        # Call the function
+
+
+class IHyperdriveSweepContractFunction(ContractFunction):
     """ContractFunction for the sweep method."""
 
-    def __call__(self, target: str) -> IERC4626HyperdriveSweepContractFunction:  # type: ignore
+    def __call__(self, target: str) -> IHyperdriveSweepContractFunction:  # type: ignore
         clone = super().__call__(dataclass_to_tuple(target))
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
     def call(
         self,
@@ -1075,18 +1119,18 @@
     ) -> None:
         """returns None."""
         # Define the expected return types from the smart contract call
 
         # Call the function
 
 
-class IERC4626HyperdriveSymbolContractFunction(ContractFunction):
+class IHyperdriveSymbolContractFunction(ContractFunction):
     """ContractFunction for the symbol method."""
 
-    def __call__(self, tokenId: int) -> IERC4626HyperdriveSymbolContractFunction:  # type: ignore
+    def __call__(self, tokenId: int) -> IHyperdriveSymbolContractFunction:  # type: ignore
         clone = super().__call__(dataclass_to_tuple(tokenId))
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
     def call(
         self,
@@ -1102,18 +1146,18 @@
 
         # Call the function
 
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
         return cast(str, rename_returned_types(structs, return_types, raw_values))
 
 
-class IERC4626HyperdriveTarget0ContractFunction(ContractFunction):
+class IHyperdriveTarget0ContractFunction(ContractFunction):
     """ContractFunction for the target0 method."""
 
-    def __call__(self) -> IERC4626HyperdriveTarget0ContractFunction:  # type: ignore
+    def __call__(self) -> IHyperdriveTarget0ContractFunction:  # type: ignore
         clone = super().__call__()
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
     def call(
         self,
@@ -1129,18 +1173,18 @@
 
         # Call the function
 
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
         return cast(str, rename_returned_types(structs, return_types, raw_values))
 
 
-class IERC4626HyperdriveTarget1ContractFunction(ContractFunction):
+class IHyperdriveTarget1ContractFunction(ContractFunction):
     """ContractFunction for the target1 method."""
 
-    def __call__(self) -> IERC4626HyperdriveTarget1ContractFunction:  # type: ignore
+    def __call__(self) -> IHyperdriveTarget1ContractFunction:  # type: ignore
         clone = super().__call__()
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
     def call(
         self,
@@ -1156,18 +1200,18 @@
 
         # Call the function
 
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
         return cast(str, rename_returned_types(structs, return_types, raw_values))
 
 
-class IERC4626HyperdriveTarget2ContractFunction(ContractFunction):
+class IHyperdriveTarget2ContractFunction(ContractFunction):
     """ContractFunction for the target2 method."""
 
-    def __call__(self) -> IERC4626HyperdriveTarget2ContractFunction:  # type: ignore
+    def __call__(self) -> IHyperdriveTarget2ContractFunction:  # type: ignore
         clone = super().__call__()
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
     def call(
         self,
@@ -1183,18 +1227,18 @@
 
         # Call the function
 
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
         return cast(str, rename_returned_types(structs, return_types, raw_values))
 
 
-class IERC4626HyperdriveTarget3ContractFunction(ContractFunction):
+class IHyperdriveTarget3ContractFunction(ContractFunction):
     """ContractFunction for the target3 method."""
 
-    def __call__(self) -> IERC4626HyperdriveTarget3ContractFunction:  # type: ignore
+    def __call__(self) -> IHyperdriveTarget3ContractFunction:  # type: ignore
         clone = super().__call__()
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
     def call(
         self,
@@ -1210,18 +1254,18 @@
 
         # Call the function
 
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
         return cast(str, rename_returned_types(structs, return_types, raw_values))
 
 
-class IERC4626HyperdriveTarget4ContractFunction(ContractFunction):
+class IHyperdriveTarget4ContractFunction(ContractFunction):
     """ContractFunction for the target4 method."""
 
-    def __call__(self) -> IERC4626HyperdriveTarget4ContractFunction:  # type: ignore
+    def __call__(self) -> IHyperdriveTarget4ContractFunction:  # type: ignore
         clone = super().__call__()
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
     def call(
         self,
@@ -1237,18 +1281,18 @@
 
         # Call the function
 
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
         return cast(str, rename_returned_types(structs, return_types, raw_values))
 
 
-class IERC4626HyperdriveTotalSupplyContractFunction(ContractFunction):
+class IHyperdriveTotalSupplyContractFunction(ContractFunction):
     """ContractFunction for the totalSupply method."""
 
-    def __call__(self, tokenId: int) -> IERC4626HyperdriveTotalSupplyContractFunction:  # type: ignore
+    def __call__(self, tokenId: int) -> IHyperdriveTotalSupplyContractFunction:  # type: ignore
         clone = super().__call__(dataclass_to_tuple(tokenId))
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
     def call(
         self,
@@ -1264,18 +1308,18 @@
 
         # Call the function
 
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
         return cast(int, rename_returned_types(structs, return_types, raw_values))
 
 
-class IERC4626HyperdriveTransferFromContractFunction(ContractFunction):
+class IHyperdriveTransferFromContractFunction(ContractFunction):
     """ContractFunction for the transferFrom method."""
 
-    def __call__(self, tokenID: int, _from: str, to: str, amount: int) -> IERC4626HyperdriveTransferFromContractFunction:  # type: ignore
+    def __call__(self, tokenID: int, _from: str, to: str, amount: int) -> IHyperdriveTransferFromContractFunction:  # type: ignore
         clone = super().__call__(
             dataclass_to_tuple(tokenID), dataclass_to_tuple(_from), dataclass_to_tuple(to), dataclass_to_tuple(amount)
         )
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
@@ -1288,18 +1332,18 @@
     ) -> None:
         """returns None."""
         # Define the expected return types from the smart contract call
 
         # Call the function
 
 
-class IERC4626HyperdriveTransferFromBridgeContractFunction(ContractFunction):
+class IHyperdriveTransferFromBridgeContractFunction(ContractFunction):
     """ContractFunction for the transferFromBridge method."""
 
-    def __call__(self, tokenID: int, _from: str, to: str, amount: int, caller: str) -> IERC4626HyperdriveTransferFromBridgeContractFunction:  # type: ignore
+    def __call__(self, tokenID: int, _from: str, to: str, amount: int, caller: str) -> IHyperdriveTransferFromBridgeContractFunction:  # type: ignore
         clone = super().__call__(
             dataclass_to_tuple(tokenID),
             dataclass_to_tuple(_from),
             dataclass_to_tuple(to),
             dataclass_to_tuple(amount),
             dataclass_to_tuple(caller),
         )
@@ -1316,18 +1360,18 @@
     ) -> None:
         """returns None."""
         # Define the expected return types from the smart contract call
 
         # Call the function
 
 
-class IERC4626HyperdriveVaultContractFunction(ContractFunction):
-    """ContractFunction for the vault method."""
+class IHyperdriveVaultSharesTokenContractFunction(ContractFunction):
+    """ContractFunction for the vaultSharesToken method."""
 
-    def __call__(self) -> IERC4626HyperdriveVaultContractFunction:  # type: ignore
+    def __call__(self) -> IHyperdriveVaultSharesTokenContractFunction:  # type: ignore
         clone = super().__call__()
         self.kwargs = clone.kwargs
         self.args = clone.args
         return self
 
     def call(
         self,
@@ -1343,541 +1387,561 @@
 
         # Call the function
 
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
         return cast(str, rename_returned_types(structs, return_types, raw_values))
 
 
-class IERC4626HyperdriveContractFunctions(ContractFunctions):
-    """ContractFunctions for the IERC4626Hyperdrive contract."""
+class IHyperdriveContractFunctions(ContractFunctions):
+    """ContractFunctions for the IHyperdrive contract."""
+
+    PERMIT_TYPEHASH: IHyperdrivePERMIT_TYPEHASHContractFunction
+
+    addLiquidity: IHyperdriveAddLiquidityContractFunction
 
-    PERMIT_TYPEHASH: IERC4626HyperdrivePERMIT_TYPEHASHContractFunction
+    balanceOf: IHyperdriveBalanceOfContractFunction
 
-    addLiquidity: IERC4626HyperdriveAddLiquidityContractFunction
+    baseToken: IHyperdriveBaseTokenContractFunction
 
-    balanceOf: IERC4626HyperdriveBalanceOfContractFunction
+    batchTransferFrom: IHyperdriveBatchTransferFromContractFunction
 
-    baseToken: IERC4626HyperdriveBaseTokenContractFunction
+    checkpoint: IHyperdriveCheckpointContractFunction
 
-    batchTransferFrom: IERC4626HyperdriveBatchTransferFromContractFunction
+    closeLong: IHyperdriveCloseLongContractFunction
 
-    checkpoint: IERC4626HyperdriveCheckpointContractFunction
+    closeShort: IHyperdriveCloseShortContractFunction
 
-    closeLong: IERC4626HyperdriveCloseLongContractFunction
+    collectGovernanceFee: IHyperdriveCollectGovernanceFeeContractFunction
 
-    closeShort: IERC4626HyperdriveCloseShortContractFunction
+    decimals: IHyperdriveDecimalsContractFunction
 
-    collectGovernanceFee: IERC4626HyperdriveCollectGovernanceFeeContractFunction
+    domainSeparator: IHyperdriveDomainSeparatorContractFunction
 
-    decimals: IERC4626HyperdriveDecimalsContractFunction
+    getCheckpoint: IHyperdriveGetCheckpointContractFunction
 
-    domainSeparator: IERC4626HyperdriveDomainSeparatorContractFunction
+    getCheckpointExposure: IHyperdriveGetCheckpointExposureContractFunction
 
-    getCheckpoint: IERC4626HyperdriveGetCheckpointContractFunction
+    getMarketState: IHyperdriveGetMarketStateContractFunction
 
-    getCheckpointExposure: IERC4626HyperdriveGetCheckpointExposureContractFunction
+    getPoolConfig: IHyperdriveGetPoolConfigContractFunction
 
-    getMarketState: IERC4626HyperdriveGetMarketStateContractFunction
+    getPoolInfo: IHyperdriveGetPoolInfoContractFunction
 
-    getPoolConfig: IERC4626HyperdriveGetPoolConfigContractFunction
+    getUncollectedGovernanceFees: IHyperdriveGetUncollectedGovernanceFeesContractFunction
 
-    getPoolInfo: IERC4626HyperdriveGetPoolInfoContractFunction
+    getWithdrawPool: IHyperdriveGetWithdrawPoolContractFunction
 
-    getUncollectedGovernanceFees: IERC4626HyperdriveGetUncollectedGovernanceFeesContractFunction
+    initialize: IHyperdriveInitializeContractFunction
 
-    getWithdrawPool: IERC4626HyperdriveGetWithdrawPoolContractFunction
+    isApprovedForAll: IHyperdriveIsApprovedForAllContractFunction
 
-    initialize: IERC4626HyperdriveInitializeContractFunction
+    isPauser: IHyperdriveIsPauserContractFunction
 
-    isApprovedForAll: IERC4626HyperdriveIsApprovedForAllContractFunction
+    load: IHyperdriveLoadContractFunction
 
-    isPauser: IERC4626HyperdriveIsPauserContractFunction
+    name: IHyperdriveNameContractFunction
 
-    load: IERC4626HyperdriveLoadContractFunction
+    nonces: IHyperdriveNoncesContractFunction
 
-    name: IERC4626HyperdriveNameContractFunction
+    openLong: IHyperdriveOpenLongContractFunction
 
-    nonces: IERC4626HyperdriveNoncesContractFunction
+    openShort: IHyperdriveOpenShortContractFunction
 
-    openLong: IERC4626HyperdriveOpenLongContractFunction
+    pause: IHyperdrivePauseContractFunction
 
-    openShort: IERC4626HyperdriveOpenShortContractFunction
+    perTokenApprovals: IHyperdrivePerTokenApprovalsContractFunction
 
-    pause: IERC4626HyperdrivePauseContractFunction
+    permitForAll: IHyperdrivePermitForAllContractFunction
 
-    perTokenApprovals: IERC4626HyperdrivePerTokenApprovalsContractFunction
+    redeemWithdrawalShares: IHyperdriveRedeemWithdrawalSharesContractFunction
 
-    permitForAll: IERC4626HyperdrivePermitForAllContractFunction
+    removeLiquidity: IHyperdriveRemoveLiquidityContractFunction
 
-    redeemWithdrawalShares: IERC4626HyperdriveRedeemWithdrawalSharesContractFunction
+    setApproval: IHyperdriveSetApprovalContractFunction
 
-    removeLiquidity: IERC4626HyperdriveRemoveLiquidityContractFunction
+    setApprovalBridge: IHyperdriveSetApprovalBridgeContractFunction
 
-    setApproval: IERC4626HyperdriveSetApprovalContractFunction
+    setApprovalForAll: IHyperdriveSetApprovalForAllContractFunction
 
-    setApprovalBridge: IERC4626HyperdriveSetApprovalBridgeContractFunction
+    setFeeCollector: IHyperdriveSetFeeCollectorContractFunction
 
-    setApprovalForAll: IERC4626HyperdriveSetApprovalForAllContractFunction
+    setGovernance: IHyperdriveSetGovernanceContractFunction
 
-    setGovernance: IERC4626HyperdriveSetGovernanceContractFunction
+    setPauser: IHyperdriveSetPauserContractFunction
 
-    setPauser: IERC4626HyperdriveSetPauserContractFunction
+    setSweepCollector: IHyperdriveSetSweepCollectorContractFunction
 
-    sweep: IERC4626HyperdriveSweepContractFunction
+    sweep: IHyperdriveSweepContractFunction
 
-    symbol: IERC4626HyperdriveSymbolContractFunction
+    symbol: IHyperdriveSymbolContractFunction
 
-    target0: IERC4626HyperdriveTarget0ContractFunction
+    target0: IHyperdriveTarget0ContractFunction
 
-    target1: IERC4626HyperdriveTarget1ContractFunction
+    target1: IHyperdriveTarget1ContractFunction
 
-    target2: IERC4626HyperdriveTarget2ContractFunction
+    target2: IHyperdriveTarget2ContractFunction
 
-    target3: IERC4626HyperdriveTarget3ContractFunction
+    target3: IHyperdriveTarget3ContractFunction
 
-    target4: IERC4626HyperdriveTarget4ContractFunction
+    target4: IHyperdriveTarget4ContractFunction
 
-    totalSupply: IERC4626HyperdriveTotalSupplyContractFunction
+    totalSupply: IHyperdriveTotalSupplyContractFunction
 
-    transferFrom: IERC4626HyperdriveTransferFromContractFunction
+    transferFrom: IHyperdriveTransferFromContractFunction
 
-    transferFromBridge: IERC4626HyperdriveTransferFromBridgeContractFunction
+    transferFromBridge: IHyperdriveTransferFromBridgeContractFunction
 
-    vault: IERC4626HyperdriveVaultContractFunction
+    vaultSharesToken: IHyperdriveVaultSharesTokenContractFunction
 
     def __init__(
         self,
         abi: ABI,
         w3: "Web3",
         address: ChecksumAddress | None = None,
         decode_tuples: bool | None = False,
     ) -> None:
         super().__init__(abi, w3, address, decode_tuples)
-        self.PERMIT_TYPEHASH = IERC4626HyperdrivePERMIT_TYPEHASHContractFunction.factory(
+        self.PERMIT_TYPEHASH = IHyperdrivePERMIT_TYPEHASHContractFunction.factory(
             "PERMIT_TYPEHASH",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="PERMIT_TYPEHASH",
         )
-        self.addLiquidity = IERC4626HyperdriveAddLiquidityContractFunction.factory(
+        self.addLiquidity = IHyperdriveAddLiquidityContractFunction.factory(
             "addLiquidity",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="addLiquidity",
         )
-        self.balanceOf = IERC4626HyperdriveBalanceOfContractFunction.factory(
+        self.balanceOf = IHyperdriveBalanceOfContractFunction.factory(
             "balanceOf",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="balanceOf",
         )
-        self.baseToken = IERC4626HyperdriveBaseTokenContractFunction.factory(
+        self.baseToken = IHyperdriveBaseTokenContractFunction.factory(
             "baseToken",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="baseToken",
         )
-        self.batchTransferFrom = IERC4626HyperdriveBatchTransferFromContractFunction.factory(
+        self.batchTransferFrom = IHyperdriveBatchTransferFromContractFunction.factory(
             "batchTransferFrom",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="batchTransferFrom",
         )
-        self.checkpoint = IERC4626HyperdriveCheckpointContractFunction.factory(
+        self.checkpoint = IHyperdriveCheckpointContractFunction.factory(
             "checkpoint",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="checkpoint",
         )
-        self.closeLong = IERC4626HyperdriveCloseLongContractFunction.factory(
+        self.closeLong = IHyperdriveCloseLongContractFunction.factory(
             "closeLong",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="closeLong",
         )
-        self.closeShort = IERC4626HyperdriveCloseShortContractFunction.factory(
+        self.closeShort = IHyperdriveCloseShortContractFunction.factory(
             "closeShort",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="closeShort",
         )
-        self.collectGovernanceFee = IERC4626HyperdriveCollectGovernanceFeeContractFunction.factory(
+        self.collectGovernanceFee = IHyperdriveCollectGovernanceFeeContractFunction.factory(
             "collectGovernanceFee",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="collectGovernanceFee",
         )
-        self.decimals = IERC4626HyperdriveDecimalsContractFunction.factory(
+        self.decimals = IHyperdriveDecimalsContractFunction.factory(
             "decimals",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="decimals",
         )
-        self.domainSeparator = IERC4626HyperdriveDomainSeparatorContractFunction.factory(
+        self.domainSeparator = IHyperdriveDomainSeparatorContractFunction.factory(
             "domainSeparator",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="domainSeparator",
         )
-        self.getCheckpoint = IERC4626HyperdriveGetCheckpointContractFunction.factory(
+        self.getCheckpoint = IHyperdriveGetCheckpointContractFunction.factory(
             "getCheckpoint",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="getCheckpoint",
         )
-        self.getCheckpointExposure = IERC4626HyperdriveGetCheckpointExposureContractFunction.factory(
+        self.getCheckpointExposure = IHyperdriveGetCheckpointExposureContractFunction.factory(
             "getCheckpointExposure",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="getCheckpointExposure",
         )
-        self.getMarketState = IERC4626HyperdriveGetMarketStateContractFunction.factory(
+        self.getMarketState = IHyperdriveGetMarketStateContractFunction.factory(
             "getMarketState",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="getMarketState",
         )
-        self.getPoolConfig = IERC4626HyperdriveGetPoolConfigContractFunction.factory(
+        self.getPoolConfig = IHyperdriveGetPoolConfigContractFunction.factory(
             "getPoolConfig",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="getPoolConfig",
         )
-        self.getPoolInfo = IERC4626HyperdriveGetPoolInfoContractFunction.factory(
+        self.getPoolInfo = IHyperdriveGetPoolInfoContractFunction.factory(
             "getPoolInfo",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="getPoolInfo",
         )
-        self.getUncollectedGovernanceFees = IERC4626HyperdriveGetUncollectedGovernanceFeesContractFunction.factory(
+        self.getUncollectedGovernanceFees = IHyperdriveGetUncollectedGovernanceFeesContractFunction.factory(
             "getUncollectedGovernanceFees",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="getUncollectedGovernanceFees",
         )
-        self.getWithdrawPool = IERC4626HyperdriveGetWithdrawPoolContractFunction.factory(
+        self.getWithdrawPool = IHyperdriveGetWithdrawPoolContractFunction.factory(
             "getWithdrawPool",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="getWithdrawPool",
         )
-        self.initialize = IERC4626HyperdriveInitializeContractFunction.factory(
+        self.initialize = IHyperdriveInitializeContractFunction.factory(
             "initialize",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="initialize",
         )
-        self.isApprovedForAll = IERC4626HyperdriveIsApprovedForAllContractFunction.factory(
+        self.isApprovedForAll = IHyperdriveIsApprovedForAllContractFunction.factory(
             "isApprovedForAll",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="isApprovedForAll",
         )
-        self.isPauser = IERC4626HyperdriveIsPauserContractFunction.factory(
+        self.isPauser = IHyperdriveIsPauserContractFunction.factory(
             "isPauser",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="isPauser",
         )
-        self.load = IERC4626HyperdriveLoadContractFunction.factory(
+        self.load = IHyperdriveLoadContractFunction.factory(
             "load",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="load",
         )
-        self.name = IERC4626HyperdriveNameContractFunction.factory(
+        self.name = IHyperdriveNameContractFunction.factory(
             "name",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="name",
         )
-        self.nonces = IERC4626HyperdriveNoncesContractFunction.factory(
+        self.nonces = IHyperdriveNoncesContractFunction.factory(
             "nonces",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="nonces",
         )
-        self.openLong = IERC4626HyperdriveOpenLongContractFunction.factory(
+        self.openLong = IHyperdriveOpenLongContractFunction.factory(
             "openLong",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="openLong",
         )
-        self.openShort = IERC4626HyperdriveOpenShortContractFunction.factory(
+        self.openShort = IHyperdriveOpenShortContractFunction.factory(
             "openShort",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="openShort",
         )
-        self.pause = IERC4626HyperdrivePauseContractFunction.factory(
+        self.pause = IHyperdrivePauseContractFunction.factory(
             "pause",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="pause",
         )
-        self.perTokenApprovals = IERC4626HyperdrivePerTokenApprovalsContractFunction.factory(
+        self.perTokenApprovals = IHyperdrivePerTokenApprovalsContractFunction.factory(
             "perTokenApprovals",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="perTokenApprovals",
         )
-        self.permitForAll = IERC4626HyperdrivePermitForAllContractFunction.factory(
+        self.permitForAll = IHyperdrivePermitForAllContractFunction.factory(
             "permitForAll",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="permitForAll",
         )
-        self.redeemWithdrawalShares = IERC4626HyperdriveRedeemWithdrawalSharesContractFunction.factory(
+        self.redeemWithdrawalShares = IHyperdriveRedeemWithdrawalSharesContractFunction.factory(
             "redeemWithdrawalShares",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="redeemWithdrawalShares",
         )
-        self.removeLiquidity = IERC4626HyperdriveRemoveLiquidityContractFunction.factory(
+        self.removeLiquidity = IHyperdriveRemoveLiquidityContractFunction.factory(
             "removeLiquidity",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="removeLiquidity",
         )
-        self.setApproval = IERC4626HyperdriveSetApprovalContractFunction.factory(
+        self.setApproval = IHyperdriveSetApprovalContractFunction.factory(
             "setApproval",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="setApproval",
         )
-        self.setApprovalBridge = IERC4626HyperdriveSetApprovalBridgeContractFunction.factory(
+        self.setApprovalBridge = IHyperdriveSetApprovalBridgeContractFunction.factory(
             "setApprovalBridge",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="setApprovalBridge",
         )
-        self.setApprovalForAll = IERC4626HyperdriveSetApprovalForAllContractFunction.factory(
+        self.setApprovalForAll = IHyperdriveSetApprovalForAllContractFunction.factory(
             "setApprovalForAll",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="setApprovalForAll",
         )
-        self.setGovernance = IERC4626HyperdriveSetGovernanceContractFunction.factory(
+        self.setFeeCollector = IHyperdriveSetFeeCollectorContractFunction.factory(
+            "setFeeCollector",
+            w3=w3,
+            contract_abi=abi,
+            address=address,
+            decode_tuples=decode_tuples,
+            function_identifier="setFeeCollector",
+        )
+        self.setGovernance = IHyperdriveSetGovernanceContractFunction.factory(
             "setGovernance",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="setGovernance",
         )
-        self.setPauser = IERC4626HyperdriveSetPauserContractFunction.factory(
+        self.setPauser = IHyperdriveSetPauserContractFunction.factory(
             "setPauser",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="setPauser",
         )
-        self.sweep = IERC4626HyperdriveSweepContractFunction.factory(
+        self.setSweepCollector = IHyperdriveSetSweepCollectorContractFunction.factory(
+            "setSweepCollector",
+            w3=w3,
+            contract_abi=abi,
+            address=address,
+            decode_tuples=decode_tuples,
+            function_identifier="setSweepCollector",
+        )
+        self.sweep = IHyperdriveSweepContractFunction.factory(
             "sweep",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="sweep",
         )
-        self.symbol = IERC4626HyperdriveSymbolContractFunction.factory(
+        self.symbol = IHyperdriveSymbolContractFunction.factory(
             "symbol",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="symbol",
         )
-        self.target0 = IERC4626HyperdriveTarget0ContractFunction.factory(
+        self.target0 = IHyperdriveTarget0ContractFunction.factory(
             "target0",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="target0",
         )
-        self.target1 = IERC4626HyperdriveTarget1ContractFunction.factory(
+        self.target1 = IHyperdriveTarget1ContractFunction.factory(
             "target1",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="target1",
         )
-        self.target2 = IERC4626HyperdriveTarget2ContractFunction.factory(
+        self.target2 = IHyperdriveTarget2ContractFunction.factory(
             "target2",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="target2",
         )
-        self.target3 = IERC4626HyperdriveTarget3ContractFunction.factory(
+        self.target3 = IHyperdriveTarget3ContractFunction.factory(
             "target3",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="target3",
         )
-        self.target4 = IERC4626HyperdriveTarget4ContractFunction.factory(
+        self.target4 = IHyperdriveTarget4ContractFunction.factory(
             "target4",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="target4",
         )
-        self.totalSupply = IERC4626HyperdriveTotalSupplyContractFunction.factory(
+        self.totalSupply = IHyperdriveTotalSupplyContractFunction.factory(
             "totalSupply",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="totalSupply",
         )
-        self.transferFrom = IERC4626HyperdriveTransferFromContractFunction.factory(
+        self.transferFrom = IHyperdriveTransferFromContractFunction.factory(
             "transferFrom",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="transferFrom",
         )
-        self.transferFromBridge = IERC4626HyperdriveTransferFromBridgeContractFunction.factory(
+        self.transferFromBridge = IHyperdriveTransferFromBridgeContractFunction.factory(
             "transferFromBridge",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="transferFromBridge",
         )
-        self.vault = IERC4626HyperdriveVaultContractFunction.factory(
-            "vault",
+        self.vaultSharesToken = IHyperdriveVaultSharesTokenContractFunction.factory(
+            "vaultSharesToken",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
-            function_identifier="vault",
+            function_identifier="vaultSharesToken",
         )
 
 
-class IERC4626HyperdriveAddLiquidityContractEvent(ContractEvent):
+class IHyperdriveAddLiquidityContractEvent(ContractEvent):
     """ContractEvent for AddLiquidity."""
 
     # super() get_logs and create_filter methods are generic, while our version adds values & types
     # pylint: disable=arguments-differ
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # pylint: disable=useless-parent-delegation
     def __init__(self, *argument_names: tuple[str]) -> None:
         super().__init__(*argument_names)
 
     def get_logs(  # type: ignore
-        self: "IERC4626HyperdriveAddLiquidityContractEvent",
+        self: "IHyperdriveAddLiquidityContractEvent",
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier | None = None,
         block_hash: HexBytes | None = None,
     ) -> Iterable[EventData]:
         return cast(
             Iterable[EventData],
             super().get_logs(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
             ),
         )
 
     @classmethod
     def get_logs(  # type: ignore
-        cls: Type["IERC4626HyperdriveAddLiquidityContractEvent"],
+        cls: Type["IHyperdriveAddLiquidityContractEvent"],
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier | None = None,
         block_hash: HexBytes | None = None,
     ) -> Iterable[EventData]:
         return cast(
             Iterable[EventData],
             super().get_logs(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
             ),
         )
 
     def create_filter(  # type: ignore
-        self: "IERC4626HyperdriveAddLiquidityContractEvent",
+        self: "IHyperdriveAddLiquidityContractEvent",
         *,  # PEP 3102
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier = "latest",
         address: ChecksumAddress | None = None,
         topics: Sequence[Any] | None = None,
     ) -> LogFilter:
@@ -1886,15 +1950,15 @@
             super().create_filter(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
             ),
         )
 
     @classmethod
     def create_filter(  # type: ignore
-        cls: Type["IERC4626HyperdriveAddLiquidityContractEvent"],
+        cls: Type["IHyperdriveAddLiquidityContractEvent"],
         *,  # PEP 3102
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier = "latest",
         address: ChecksumAddress | None = None,
         topics: Sequence[Any] | None = None,
     ) -> LogFilter:
@@ -1902,58 +1966,58 @@
             LogFilter,
             super().create_filter(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
             ),
         )
 
 
-class IERC4626HyperdriveApprovalContractEvent(ContractEvent):
+class IHyperdriveApprovalContractEvent(ContractEvent):
     """ContractEvent for Approval."""
 
     # super() get_logs and create_filter methods are generic, while our version adds values & types
     # pylint: disable=arguments-differ
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # pylint: disable=useless-parent-delegation
     def __init__(self, *argument_names: tuple[str]) -> None:
         super().__init__(*argument_names)
 
     def get_logs(  # type: ignore
-        self: "IERC4626HyperdriveApprovalContractEvent",
+        self: "IHyperdriveApprovalContractEvent",
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier | None = None,
         block_hash: HexBytes | None = None,
     ) -> Iterable[EventData]:
         return cast(
             Iterable[EventData],
             super().get_logs(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
             ),
         )
 
     @classmethod
     def get_logs(  # type: ignore
-        cls: Type["IERC4626HyperdriveApprovalContractEvent"],
+        cls: Type["IHyperdriveApprovalContractEvent"],
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier | None = None,
         block_hash: HexBytes | None = None,
     ) -> Iterable[EventData]:
         return cast(
             Iterable[EventData],
             super().get_logs(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
             ),
         )
 
     def create_filter(  # type: ignore
-        self: "IERC4626HyperdriveApprovalContractEvent",
+        self: "IHyperdriveApprovalContractEvent",
         *,  # PEP 3102
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier = "latest",
         address: ChecksumAddress | None = None,
         topics: Sequence[Any] | None = None,
     ) -> LogFilter:
@@ -1962,15 +2026,15 @@
             super().create_filter(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
             ),
         )
 
     @classmethod
     def create_filter(  # type: ignore
-        cls: Type["IERC4626HyperdriveApprovalContractEvent"],
+        cls: Type["IHyperdriveApprovalContractEvent"],
         *,  # PEP 3102
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier = "latest",
         address: ChecksumAddress | None = None,
         topics: Sequence[Any] | None = None,
     ) -> LogFilter:
@@ -1978,58 +2042,58 @@
             LogFilter,
             super().create_filter(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
             ),
         )
 
 
-class IERC4626HyperdriveApprovalForAllContractEvent(ContractEvent):
+class IHyperdriveApprovalForAllContractEvent(ContractEvent):
     """ContractEvent for ApprovalForAll."""
 
     # super() get_logs and create_filter methods are generic, while our version adds values & types
     # pylint: disable=arguments-differ
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # pylint: disable=useless-parent-delegation
     def __init__(self, *argument_names: tuple[str]) -> None:
         super().__init__(*argument_names)
 
     def get_logs(  # type: ignore
-        self: "IERC4626HyperdriveApprovalForAllContractEvent",
+        self: "IHyperdriveApprovalForAllContractEvent",
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier | None = None,
         block_hash: HexBytes | None = None,
     ) -> Iterable[EventData]:
         return cast(
             Iterable[EventData],
             super().get_logs(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
             ),
         )
 
     @classmethod
     def get_logs(  # type: ignore
-        cls: Type["IERC4626HyperdriveApprovalForAllContractEvent"],
+        cls: Type["IHyperdriveApprovalForAllContractEvent"],
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier | None = None,
         block_hash: HexBytes | None = None,
     ) -> Iterable[EventData]:
         return cast(
             Iterable[EventData],
             super().get_logs(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
             ),
         )
 
     def create_filter(  # type: ignore
-        self: "IERC4626HyperdriveApprovalForAllContractEvent",
+        self: "IHyperdriveApprovalForAllContractEvent",
         *,  # PEP 3102
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier = "latest",
         address: ChecksumAddress | None = None,
         topics: Sequence[Any] | None = None,
     ) -> LogFilter:
@@ -2038,15 +2102,15 @@
             super().create_filter(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
             ),
         )
 
     @classmethod
     def create_filter(  # type: ignore
-        cls: Type["IERC4626HyperdriveApprovalForAllContractEvent"],
+        cls: Type["IHyperdriveApprovalForAllContractEvent"],
         *,  # PEP 3102
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier = "latest",
         address: ChecksumAddress | None = None,
         topics: Sequence[Any] | None = None,
     ) -> LogFilter:
@@ -2054,58 +2118,58 @@
             LogFilter,
             super().create_filter(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
             ),
         )
 
 
-class IERC4626HyperdriveCloseLongContractEvent(ContractEvent):
+class IHyperdriveCloseLongContractEvent(ContractEvent):
     """ContractEvent for CloseLong."""
 
     # super() get_logs and create_filter methods are generic, while our version adds values & types
     # pylint: disable=arguments-differ
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # pylint: disable=useless-parent-delegation
     def __init__(self, *argument_names: tuple[str]) -> None:
         super().__init__(*argument_names)
 
     def get_logs(  # type: ignore
-        self: "IERC4626HyperdriveCloseLongContractEvent",
+        self: "IHyperdriveCloseLongContractEvent",
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier | None = None,
         block_hash: HexBytes | None = None,
     ) -> Iterable[EventData]:
         return cast(
             Iterable[EventData],
             super().get_logs(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
             ),
         )
 
     @classmethod
     def get_logs(  # type: ignore
-        cls: Type["IERC4626HyperdriveCloseLongContractEvent"],
+        cls: Type["IHyperdriveCloseLongContractEvent"],
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier | None = None,
         block_hash: HexBytes | None = None,
     ) -> Iterable[EventData]:
         return cast(
             Iterable[EventData],
             super().get_logs(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
             ),
         )
 
     def create_filter(  # type: ignore
-        self: "IERC4626HyperdriveCloseLongContractEvent",
+        self: "IHyperdriveCloseLongContractEvent",
         *,  # PEP 3102
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier = "latest",
         address: ChecksumAddress | None = None,
         topics: Sequence[Any] | None = None,
     ) -> LogFilter:
@@ -2114,15 +2178,15 @@
             super().create_filter(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
             ),
         )
 
     @classmethod
     def create_filter(  # type: ignore
-        cls: Type["IERC4626HyperdriveCloseLongContractEvent"],
+        cls: Type["IHyperdriveCloseLongContractEvent"],
         *,  # PEP 3102
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier = "latest",
         address: ChecksumAddress | None = None,
         topics: Sequence[Any] | None = None,
     ) -> LogFilter:
@@ -2130,58 +2194,58 @@
             LogFilter,
             super().create_filter(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
             ),
         )
 
 
-class IERC4626HyperdriveCloseShortContractEvent(ContractEvent):
+class IHyperdriveCloseShortContractEvent(ContractEvent):
     """ContractEvent for CloseShort."""
 
     # super() get_logs and create_filter methods are generic, while our version adds values & types
     # pylint: disable=arguments-differ
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # pylint: disable=useless-parent-delegation
     def __init__(self, *argument_names: tuple[str]) -> None:
         super().__init__(*argument_names)
 
     def get_logs(  # type: ignore
-        self: "IERC4626HyperdriveCloseShortContractEvent",
+        self: "IHyperdriveCloseShortContractEvent",
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier | None = None,
         block_hash: HexBytes | None = None,
     ) -> Iterable[EventData]:
         return cast(
             Iterable[EventData],
             super().get_logs(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
             ),
         )
 
     @classmethod
     def get_logs(  # type: ignore
-        cls: Type["IERC4626HyperdriveCloseShortContractEvent"],
+        cls: Type["IHyperdriveCloseShortContractEvent"],
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier | None = None,
         block_hash: HexBytes | None = None,
     ) -> Iterable[EventData]:
         return cast(
             Iterable[EventData],
             super().get_logs(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
             ),
         )
 
     def create_filter(  # type: ignore
-        self: "IERC4626HyperdriveCloseShortContractEvent",
+        self: "IHyperdriveCloseShortContractEvent",
         *,  # PEP 3102
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier = "latest",
         address: ChecksumAddress | None = None,
         topics: Sequence[Any] | None = None,
     ) -> LogFilter:
@@ -2190,15 +2254,15 @@
             super().create_filter(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
             ),
         )
 
     @classmethod
     def create_filter(  # type: ignore
-        cls: Type["IERC4626HyperdriveCloseShortContractEvent"],
+        cls: Type["IHyperdriveCloseShortContractEvent"],
         *,  # PEP 3102
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier = "latest",
         address: ChecksumAddress | None = None,
         topics: Sequence[Any] | None = None,
     ) -> LogFilter:
@@ -2206,58 +2270,58 @@
             LogFilter,
             super().create_filter(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
             ),
         )
 
 
-class IERC4626HyperdriveCollectGovernanceFeeContractEvent(ContractEvent):
+class IHyperdriveCollectGovernanceFeeContractEvent(ContractEvent):
     """ContractEvent for CollectGovernanceFee."""
 
     # super() get_logs and create_filter methods are generic, while our version adds values & types
     # pylint: disable=arguments-differ
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # pylint: disable=useless-parent-delegation
     def __init__(self, *argument_names: tuple[str]) -> None:
         super().__init__(*argument_names)
 
     def get_logs(  # type: ignore
-        self: "IERC4626HyperdriveCollectGovernanceFeeContractEvent",
+        self: "IHyperdriveCollectGovernanceFeeContractEvent",
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier | None = None,
         block_hash: HexBytes | None = None,
     ) -> Iterable[EventData]:
         return cast(
             Iterable[EventData],
             super().get_logs(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
             ),
         )
 
     @classmethod
     def get_logs(  # type: ignore
-        cls: Type["IERC4626HyperdriveCollectGovernanceFeeContractEvent"],
+        cls: Type["IHyperdriveCollectGovernanceFeeContractEvent"],
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier | None = None,
         block_hash: HexBytes | None = None,
     ) -> Iterable[EventData]:
         return cast(
             Iterable[EventData],
             super().get_logs(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
             ),
         )
 
     def create_filter(  # type: ignore
-        self: "IERC4626HyperdriveCollectGovernanceFeeContractEvent",
+        self: "IHyperdriveCollectGovernanceFeeContractEvent",
         *,  # PEP 3102
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier = "latest",
         address: ChecksumAddress | None = None,
         topics: Sequence[Any] | None = None,
     ) -> LogFilter:
@@ -2266,15 +2330,15 @@
             super().create_filter(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
             ),
         )
 
     @classmethod
     def create_filter(  # type: ignore
-        cls: Type["IERC4626HyperdriveCollectGovernanceFeeContractEvent"],
+        cls: Type["IHyperdriveCollectGovernanceFeeContractEvent"],
         *,  # PEP 3102
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier = "latest",
         address: ChecksumAddress | None = None,
         topics: Sequence[Any] | None = None,
     ) -> LogFilter:
@@ -2282,58 +2346,58 @@
             LogFilter,
             super().create_filter(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
             ),
         )
 
 
-class IERC4626HyperdriveCreateCheckpointContractEvent(ContractEvent):
+class IHyperdriveCreateCheckpointContractEvent(ContractEvent):
     """ContractEvent for CreateCheckpoint."""
 
     # super() get_logs and create_filter methods are generic, while our version adds values & types
     # pylint: disable=arguments-differ
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # pylint: disable=useless-parent-delegation
     def __init__(self, *argument_names: tuple[str]) -> None:
         super().__init__(*argument_names)
 
     def get_logs(  # type: ignore
-        self: "IERC4626HyperdriveCreateCheckpointContractEvent",
+        self: "IHyperdriveCreateCheckpointContractEvent",
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier | None = None,
         block_hash: HexBytes | None = None,
     ) -> Iterable[EventData]:
         return cast(
             Iterable[EventData],
             super().get_logs(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
             ),
         )
 
     @classmethod
     def get_logs(  # type: ignore
-        cls: Type["IERC4626HyperdriveCreateCheckpointContractEvent"],
+        cls: Type["IHyperdriveCreateCheckpointContractEvent"],
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier | None = None,
         block_hash: HexBytes | None = None,
     ) -> Iterable[EventData]:
         return cast(
             Iterable[EventData],
             super().get_logs(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
             ),
         )
 
     def create_filter(  # type: ignore
-        self: "IERC4626HyperdriveCreateCheckpointContractEvent",
+        self: "IHyperdriveCreateCheckpointContractEvent",
         *,  # PEP 3102
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier = "latest",
         address: ChecksumAddress | None = None,
         topics: Sequence[Any] | None = None,
     ) -> LogFilter:
@@ -2342,15 +2406,15 @@
             super().create_filter(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
             ),
         )
 
     @classmethod
     def create_filter(  # type: ignore
-        cls: Type["IERC4626HyperdriveCreateCheckpointContractEvent"],
+        cls: Type["IHyperdriveCreateCheckpointContractEvent"],
         *,  # PEP 3102
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier = "latest",
         address: ChecksumAddress | None = None,
         topics: Sequence[Any] | None = None,
     ) -> LogFilter:
@@ -2358,58 +2422,134 @@
             LogFilter,
             super().create_filter(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
             ),
         )
 
 
-class IERC4626HyperdriveGovernanceUpdatedContractEvent(ContractEvent):
+class IHyperdriveFeeCollectorUpdatedContractEvent(ContractEvent):
+    """ContractEvent for FeeCollectorUpdated."""
+
+    # super() get_logs and create_filter methods are generic, while our version adds values & types
+    # pylint: disable=arguments-differ
+
+    # @combomethod destroys return types, so we are redefining functions as both class and instance
+    # pylint: disable=function-redefined
+
+    # pylint: disable=useless-parent-delegation
+    def __init__(self, *argument_names: tuple[str]) -> None:
+        super().__init__(*argument_names)
+
+    def get_logs(  # type: ignore
+        self: "IHyperdriveFeeCollectorUpdatedContractEvent",
+        argument_filters: dict[str, Any] | None = None,
+        fromBlock: BlockIdentifier | None = None,
+        toBlock: BlockIdentifier | None = None,
+        block_hash: HexBytes | None = None,
+    ) -> Iterable[EventData]:
+        return cast(
+            Iterable[EventData],
+            super().get_logs(
+                argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
+            ),
+        )
+
+    @classmethod
+    def get_logs(  # type: ignore
+        cls: Type["IHyperdriveFeeCollectorUpdatedContractEvent"],
+        argument_filters: dict[str, Any] | None = None,
+        fromBlock: BlockIdentifier | None = None,
+        toBlock: BlockIdentifier | None = None,
+        block_hash: HexBytes | None = None,
+    ) -> Iterable[EventData]:
+        return cast(
+            Iterable[EventData],
+            super().get_logs(
+                argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
+            ),
+        )
+
+    def create_filter(  # type: ignore
+        self: "IHyperdriveFeeCollectorUpdatedContractEvent",
+        *,  # PEP 3102
+        argument_filters: dict[str, Any] | None = None,
+        fromBlock: BlockIdentifier | None = None,
+        toBlock: BlockIdentifier = "latest",
+        address: ChecksumAddress | None = None,
+        topics: Sequence[Any] | None = None,
+    ) -> LogFilter:
+        return cast(
+            LogFilter,
+            super().create_filter(
+                argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
+            ),
+        )
+
+    @classmethod
+    def create_filter(  # type: ignore
+        cls: Type["IHyperdriveFeeCollectorUpdatedContractEvent"],
+        *,  # PEP 3102
+        argument_filters: dict[str, Any] | None = None,
+        fromBlock: BlockIdentifier | None = None,
+        toBlock: BlockIdentifier = "latest",
+        address: ChecksumAddress | None = None,
+        topics: Sequence[Any] | None = None,
+    ) -> LogFilter:
+        return cast(
+            LogFilter,
+            super().create_filter(
+                argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
+            ),
+        )
+
+
+class IHyperdriveGovernanceUpdatedContractEvent(ContractEvent):
     """ContractEvent for GovernanceUpdated."""
 
     # super() get_logs and create_filter methods are generic, while our version adds values & types
     # pylint: disable=arguments-differ
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # pylint: disable=useless-parent-delegation
     def __init__(self, *argument_names: tuple[str]) -> None:
         super().__init__(*argument_names)
 
     def get_logs(  # type: ignore
-        self: "IERC4626HyperdriveGovernanceUpdatedContractEvent",
+        self: "IHyperdriveGovernanceUpdatedContractEvent",
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier | None = None,
         block_hash: HexBytes | None = None,
     ) -> Iterable[EventData]:
         return cast(
             Iterable[EventData],
             super().get_logs(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
             ),
         )
 
     @classmethod
     def get_logs(  # type: ignore
-        cls: Type["IERC4626HyperdriveGovernanceUpdatedContractEvent"],
+        cls: Type["IHyperdriveGovernanceUpdatedContractEvent"],
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier | None = None,
         block_hash: HexBytes | None = None,
     ) -> Iterable[EventData]:
         return cast(
             Iterable[EventData],
             super().get_logs(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
             ),
         )
 
     def create_filter(  # type: ignore
-        self: "IERC4626HyperdriveGovernanceUpdatedContractEvent",
+        self: "IHyperdriveGovernanceUpdatedContractEvent",
         *,  # PEP 3102
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier = "latest",
         address: ChecksumAddress | None = None,
         topics: Sequence[Any] | None = None,
     ) -> LogFilter:
@@ -2418,15 +2558,15 @@
             super().create_filter(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
             ),
         )
 
     @classmethod
     def create_filter(  # type: ignore
-        cls: Type["IERC4626HyperdriveGovernanceUpdatedContractEvent"],
+        cls: Type["IHyperdriveGovernanceUpdatedContractEvent"],
         *,  # PEP 3102
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier = "latest",
         address: ChecksumAddress | None = None,
         topics: Sequence[Any] | None = None,
     ) -> LogFilter:
@@ -2434,58 +2574,58 @@
             LogFilter,
             super().create_filter(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
             ),
         )
 
 
-class IERC4626HyperdriveInitializeContractEvent(ContractEvent):
+class IHyperdriveInitializeContractEvent(ContractEvent):
     """ContractEvent for Initialize."""
 
     # super() get_logs and create_filter methods are generic, while our version adds values & types
     # pylint: disable=arguments-differ
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # pylint: disable=useless-parent-delegation
     def __init__(self, *argument_names: tuple[str]) -> None:
         super().__init__(*argument_names)
 
     def get_logs(  # type: ignore
-        self: "IERC4626HyperdriveInitializeContractEvent",
+        self: "IHyperdriveInitializeContractEvent",
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier | None = None,
         block_hash: HexBytes | None = None,
     ) -> Iterable[EventData]:
         return cast(
             Iterable[EventData],
             super().get_logs(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
             ),
         )
 
     @classmethod
     def get_logs(  # type: ignore
-        cls: Type["IERC4626HyperdriveInitializeContractEvent"],
+        cls: Type["IHyperdriveInitializeContractEvent"],
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier | None = None,
         block_hash: HexBytes | None = None,
     ) -> Iterable[EventData]:
         return cast(
             Iterable[EventData],
             super().get_logs(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
             ),
         )
 
     def create_filter(  # type: ignore
-        self: "IERC4626HyperdriveInitializeContractEvent",
+        self: "IHyperdriveInitializeContractEvent",
         *,  # PEP 3102
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier = "latest",
         address: ChecksumAddress | None = None,
         topics: Sequence[Any] | None = None,
     ) -> LogFilter:
@@ -2494,15 +2634,15 @@
             super().create_filter(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
             ),
         )
 
     @classmethod
     def create_filter(  # type: ignore
-        cls: Type["IERC4626HyperdriveInitializeContractEvent"],
+        cls: Type["IHyperdriveInitializeContractEvent"],
         *,  # PEP 3102
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier = "latest",
         address: ChecksumAddress | None = None,
         topics: Sequence[Any] | None = None,
     ) -> LogFilter:
@@ -2510,58 +2650,58 @@
             LogFilter,
             super().create_filter(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
             ),
         )
 
 
-class IERC4626HyperdriveOpenLongContractEvent(ContractEvent):
+class IHyperdriveOpenLongContractEvent(ContractEvent):
     """ContractEvent for OpenLong."""
 
     # super() get_logs and create_filter methods are generic, while our version adds values & types
     # pylint: disable=arguments-differ
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # pylint: disable=useless-parent-delegation
     def __init__(self, *argument_names: tuple[str]) -> None:
         super().__init__(*argument_names)
 
     def get_logs(  # type: ignore
-        self: "IERC4626HyperdriveOpenLongContractEvent",
+        self: "IHyperdriveOpenLongContractEvent",
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier | None = None,
         block_hash: HexBytes | None = None,
     ) -> Iterable[EventData]:
         return cast(
             Iterable[EventData],
             super().get_logs(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
             ),
         )
 
     @classmethod
     def get_logs(  # type: ignore
-        cls: Type["IERC4626HyperdriveOpenLongContractEvent"],
+        cls: Type["IHyperdriveOpenLongContractEvent"],
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier | None = None,
         block_hash: HexBytes | None = None,
     ) -> Iterable[EventData]:
         return cast(
             Iterable[EventData],
             super().get_logs(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
             ),
         )
 
     def create_filter(  # type: ignore
-        self: "IERC4626HyperdriveOpenLongContractEvent",
+        self: "IHyperdriveOpenLongContractEvent",
         *,  # PEP 3102
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier = "latest",
         address: ChecksumAddress | None = None,
         topics: Sequence[Any] | None = None,
     ) -> LogFilter:
@@ -2570,15 +2710,15 @@
             super().create_filter(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
             ),
         )
 
     @classmethod
     def create_filter(  # type: ignore
-        cls: Type["IERC4626HyperdriveOpenLongContractEvent"],
+        cls: Type["IHyperdriveOpenLongContractEvent"],
         *,  # PEP 3102
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier = "latest",
         address: ChecksumAddress | None = None,
         topics: Sequence[Any] | None = None,
     ) -> LogFilter:
@@ -2586,58 +2726,58 @@
             LogFilter,
             super().create_filter(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
             ),
         )
 
 
-class IERC4626HyperdriveOpenShortContractEvent(ContractEvent):
+class IHyperdriveOpenShortContractEvent(ContractEvent):
     """ContractEvent for OpenShort."""
 
     # super() get_logs and create_filter methods are generic, while our version adds values & types
     # pylint: disable=arguments-differ
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # pylint: disable=useless-parent-delegation
     def __init__(self, *argument_names: tuple[str]) -> None:
         super().__init__(*argument_names)
 
     def get_logs(  # type: ignore
-        self: "IERC4626HyperdriveOpenShortContractEvent",
+        self: "IHyperdriveOpenShortContractEvent",
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier | None = None,
         block_hash: HexBytes | None = None,
     ) -> Iterable[EventData]:
         return cast(
             Iterable[EventData],
             super().get_logs(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
             ),
         )
 
     @classmethod
     def get_logs(  # type: ignore
-        cls: Type["IERC4626HyperdriveOpenShortContractEvent"],
+        cls: Type["IHyperdriveOpenShortContractEvent"],
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier | None = None,
         block_hash: HexBytes | None = None,
     ) -> Iterable[EventData]:
         return cast(
             Iterable[EventData],
             super().get_logs(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
             ),
         )
 
     def create_filter(  # type: ignore
-        self: "IERC4626HyperdriveOpenShortContractEvent",
+        self: "IHyperdriveOpenShortContractEvent",
         *,  # PEP 3102
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier = "latest",
         address: ChecksumAddress | None = None,
         topics: Sequence[Any] | None = None,
     ) -> LogFilter:
@@ -2646,15 +2786,15 @@
             super().create_filter(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
             ),
         )
 
     @classmethod
     def create_filter(  # type: ignore
-        cls: Type["IERC4626HyperdriveOpenShortContractEvent"],
+        cls: Type["IHyperdriveOpenShortContractEvent"],
         *,  # PEP 3102
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier = "latest",
         address: ChecksumAddress | None = None,
         topics: Sequence[Any] | None = None,
     ) -> LogFilter:
@@ -2662,58 +2802,58 @@
             LogFilter,
             super().create_filter(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
             ),
         )
 
 
-class IERC4626HyperdrivePauseStatusUpdatedContractEvent(ContractEvent):
+class IHyperdrivePauseStatusUpdatedContractEvent(ContractEvent):
     """ContractEvent for PauseStatusUpdated."""
 
     # super() get_logs and create_filter methods are generic, while our version adds values & types
     # pylint: disable=arguments-differ
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # pylint: disable=useless-parent-delegation
     def __init__(self, *argument_names: tuple[str]) -> None:
         super().__init__(*argument_names)
 
     def get_logs(  # type: ignore
-        self: "IERC4626HyperdrivePauseStatusUpdatedContractEvent",
+        self: "IHyperdrivePauseStatusUpdatedContractEvent",
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier | None = None,
         block_hash: HexBytes | None = None,
     ) -> Iterable[EventData]:
         return cast(
             Iterable[EventData],
             super().get_logs(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
             ),
         )
 
     @classmethod
     def get_logs(  # type: ignore
-        cls: Type["IERC4626HyperdrivePauseStatusUpdatedContractEvent"],
+        cls: Type["IHyperdrivePauseStatusUpdatedContractEvent"],
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier | None = None,
         block_hash: HexBytes | None = None,
     ) -> Iterable[EventData]:
         return cast(
             Iterable[EventData],
             super().get_logs(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
             ),
         )
 
     def create_filter(  # type: ignore
-        self: "IERC4626HyperdrivePauseStatusUpdatedContractEvent",
+        self: "IHyperdrivePauseStatusUpdatedContractEvent",
         *,  # PEP 3102
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier = "latest",
         address: ChecksumAddress | None = None,
         topics: Sequence[Any] | None = None,
     ) -> LogFilter:
@@ -2722,15 +2862,15 @@
             super().create_filter(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
             ),
         )
 
     @classmethod
     def create_filter(  # type: ignore
-        cls: Type["IERC4626HyperdrivePauseStatusUpdatedContractEvent"],
+        cls: Type["IHyperdrivePauseStatusUpdatedContractEvent"],
         *,  # PEP 3102
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier = "latest",
         address: ChecksumAddress | None = None,
         topics: Sequence[Any] | None = None,
     ) -> LogFilter:
@@ -2738,58 +2878,58 @@
             LogFilter,
             super().create_filter(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
             ),
         )
 
 
-class IERC4626HyperdrivePauserUpdatedContractEvent(ContractEvent):
+class IHyperdrivePauserUpdatedContractEvent(ContractEvent):
     """ContractEvent for PauserUpdated."""
 
     # super() get_logs and create_filter methods are generic, while our version adds values & types
     # pylint: disable=arguments-differ
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # pylint: disable=useless-parent-delegation
     def __init__(self, *argument_names: tuple[str]) -> None:
         super().__init__(*argument_names)
 
     def get_logs(  # type: ignore
-        self: "IERC4626HyperdrivePauserUpdatedContractEvent",
+        self: "IHyperdrivePauserUpdatedContractEvent",
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier | None = None,
         block_hash: HexBytes | None = None,
     ) -> Iterable[EventData]:
         return cast(
             Iterable[EventData],
             super().get_logs(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
             ),
         )
 
     @classmethod
     def get_logs(  # type: ignore
-        cls: Type["IERC4626HyperdrivePauserUpdatedContractEvent"],
+        cls: Type["IHyperdrivePauserUpdatedContractEvent"],
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier | None = None,
         block_hash: HexBytes | None = None,
     ) -> Iterable[EventData]:
         return cast(
             Iterable[EventData],
             super().get_logs(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
             ),
         )
 
     def create_filter(  # type: ignore
-        self: "IERC4626HyperdrivePauserUpdatedContractEvent",
+        self: "IHyperdrivePauserUpdatedContractEvent",
         *,  # PEP 3102
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier = "latest",
         address: ChecksumAddress | None = None,
         topics: Sequence[Any] | None = None,
     ) -> LogFilter:
@@ -2798,15 +2938,15 @@
             super().create_filter(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
             ),
         )
 
     @classmethod
     def create_filter(  # type: ignore
-        cls: Type["IERC4626HyperdrivePauserUpdatedContractEvent"],
+        cls: Type["IHyperdrivePauserUpdatedContractEvent"],
         *,  # PEP 3102
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier = "latest",
         address: ChecksumAddress | None = None,
         topics: Sequence[Any] | None = None,
     ) -> LogFilter:
@@ -2814,58 +2954,58 @@
             LogFilter,
             super().create_filter(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
             ),
         )
 
 
-class IERC4626HyperdriveRedeemWithdrawalSharesContractEvent(ContractEvent):
+class IHyperdriveRedeemWithdrawalSharesContractEvent(ContractEvent):
     """ContractEvent for RedeemWithdrawalShares."""
 
     # super() get_logs and create_filter methods are generic, while our version adds values & types
     # pylint: disable=arguments-differ
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # pylint: disable=useless-parent-delegation
     def __init__(self, *argument_names: tuple[str]) -> None:
         super().__init__(*argument_names)
 
     def get_logs(  # type: ignore
-        self: "IERC4626HyperdriveRedeemWithdrawalSharesContractEvent",
+        self: "IHyperdriveRedeemWithdrawalSharesContractEvent",
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier | None = None,
         block_hash: HexBytes | None = None,
     ) -> Iterable[EventData]:
         return cast(
             Iterable[EventData],
             super().get_logs(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
             ),
         )
 
     @classmethod
     def get_logs(  # type: ignore
-        cls: Type["IERC4626HyperdriveRedeemWithdrawalSharesContractEvent"],
+        cls: Type["IHyperdriveRedeemWithdrawalSharesContractEvent"],
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier | None = None,
         block_hash: HexBytes | None = None,
     ) -> Iterable[EventData]:
         return cast(
             Iterable[EventData],
             super().get_logs(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
             ),
         )
 
     def create_filter(  # type: ignore
-        self: "IERC4626HyperdriveRedeemWithdrawalSharesContractEvent",
+        self: "IHyperdriveRedeemWithdrawalSharesContractEvent",
         *,  # PEP 3102
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier = "latest",
         address: ChecksumAddress | None = None,
         topics: Sequence[Any] | None = None,
     ) -> LogFilter:
@@ -2874,15 +3014,15 @@
             super().create_filter(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
             ),
         )
 
     @classmethod
     def create_filter(  # type: ignore
-        cls: Type["IERC4626HyperdriveRedeemWithdrawalSharesContractEvent"],
+        cls: Type["IHyperdriveRedeemWithdrawalSharesContractEvent"],
         *,  # PEP 3102
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier = "latest",
         address: ChecksumAddress | None = None,
         topics: Sequence[Any] | None = None,
     ) -> LogFilter:
@@ -2890,58 +3030,210 @@
             LogFilter,
             super().create_filter(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
             ),
         )
 
 
-class IERC4626HyperdriveRemoveLiquidityContractEvent(ContractEvent):
+class IHyperdriveRemoveLiquidityContractEvent(ContractEvent):
     """ContractEvent for RemoveLiquidity."""
 
     # super() get_logs and create_filter methods are generic, while our version adds values & types
     # pylint: disable=arguments-differ
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # pylint: disable=useless-parent-delegation
     def __init__(self, *argument_names: tuple[str]) -> None:
         super().__init__(*argument_names)
 
     def get_logs(  # type: ignore
-        self: "IERC4626HyperdriveRemoveLiquidityContractEvent",
+        self: "IHyperdriveRemoveLiquidityContractEvent",
+        argument_filters: dict[str, Any] | None = None,
+        fromBlock: BlockIdentifier | None = None,
+        toBlock: BlockIdentifier | None = None,
+        block_hash: HexBytes | None = None,
+    ) -> Iterable[EventData]:
+        return cast(
+            Iterable[EventData],
+            super().get_logs(
+                argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
+            ),
+        )
+
+    @classmethod
+    def get_logs(  # type: ignore
+        cls: Type["IHyperdriveRemoveLiquidityContractEvent"],
+        argument_filters: dict[str, Any] | None = None,
+        fromBlock: BlockIdentifier | None = None,
+        toBlock: BlockIdentifier | None = None,
+        block_hash: HexBytes | None = None,
+    ) -> Iterable[EventData]:
+        return cast(
+            Iterable[EventData],
+            super().get_logs(
+                argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
+            ),
+        )
+
+    def create_filter(  # type: ignore
+        self: "IHyperdriveRemoveLiquidityContractEvent",
+        *,  # PEP 3102
+        argument_filters: dict[str, Any] | None = None,
+        fromBlock: BlockIdentifier | None = None,
+        toBlock: BlockIdentifier = "latest",
+        address: ChecksumAddress | None = None,
+        topics: Sequence[Any] | None = None,
+    ) -> LogFilter:
+        return cast(
+            LogFilter,
+            super().create_filter(
+                argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
+            ),
+        )
+
+    @classmethod
+    def create_filter(  # type: ignore
+        cls: Type["IHyperdriveRemoveLiquidityContractEvent"],
+        *,  # PEP 3102
+        argument_filters: dict[str, Any] | None = None,
+        fromBlock: BlockIdentifier | None = None,
+        toBlock: BlockIdentifier = "latest",
+        address: ChecksumAddress | None = None,
+        topics: Sequence[Any] | None = None,
+    ) -> LogFilter:
+        return cast(
+            LogFilter,
+            super().create_filter(
+                argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
+            ),
+        )
+
+
+class IHyperdriveSweepContractEvent(ContractEvent):
+    """ContractEvent for Sweep."""
+
+    # super() get_logs and create_filter methods are generic, while our version adds values & types
+    # pylint: disable=arguments-differ
+
+    # @combomethod destroys return types, so we are redefining functions as both class and instance
+    # pylint: disable=function-redefined
+
+    # pylint: disable=useless-parent-delegation
+    def __init__(self, *argument_names: tuple[str]) -> None:
+        super().__init__(*argument_names)
+
+    def get_logs(  # type: ignore
+        self: "IHyperdriveSweepContractEvent",
+        argument_filters: dict[str, Any] | None = None,
+        fromBlock: BlockIdentifier | None = None,
+        toBlock: BlockIdentifier | None = None,
+        block_hash: HexBytes | None = None,
+    ) -> Iterable[EventData]:
+        return cast(
+            Iterable[EventData],
+            super().get_logs(
+                argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
+            ),
+        )
+
+    @classmethod
+    def get_logs(  # type: ignore
+        cls: Type["IHyperdriveSweepContractEvent"],
+        argument_filters: dict[str, Any] | None = None,
+        fromBlock: BlockIdentifier | None = None,
+        toBlock: BlockIdentifier | None = None,
+        block_hash: HexBytes | None = None,
+    ) -> Iterable[EventData]:
+        return cast(
+            Iterable[EventData],
+            super().get_logs(
+                argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
+            ),
+        )
+
+    def create_filter(  # type: ignore
+        self: "IHyperdriveSweepContractEvent",
+        *,  # PEP 3102
+        argument_filters: dict[str, Any] | None = None,
+        fromBlock: BlockIdentifier | None = None,
+        toBlock: BlockIdentifier = "latest",
+        address: ChecksumAddress | None = None,
+        topics: Sequence[Any] | None = None,
+    ) -> LogFilter:
+        return cast(
+            LogFilter,
+            super().create_filter(
+                argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
+            ),
+        )
+
+    @classmethod
+    def create_filter(  # type: ignore
+        cls: Type["IHyperdriveSweepContractEvent"],
+        *,  # PEP 3102
+        argument_filters: dict[str, Any] | None = None,
+        fromBlock: BlockIdentifier | None = None,
+        toBlock: BlockIdentifier = "latest",
+        address: ChecksumAddress | None = None,
+        topics: Sequence[Any] | None = None,
+    ) -> LogFilter:
+        return cast(
+            LogFilter,
+            super().create_filter(
+                argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
+            ),
+        )
+
+
+class IHyperdriveSweepCollectorUpdatedContractEvent(ContractEvent):
+    """ContractEvent for SweepCollectorUpdated."""
+
+    # super() get_logs and create_filter methods are generic, while our version adds values & types
+    # pylint: disable=arguments-differ
+
+    # @combomethod destroys return types, so we are redefining functions as both class and instance
+    # pylint: disable=function-redefined
+
+    # pylint: disable=useless-parent-delegation
+    def __init__(self, *argument_names: tuple[str]) -> None:
+        super().__init__(*argument_names)
+
+    def get_logs(  # type: ignore
+        self: "IHyperdriveSweepCollectorUpdatedContractEvent",
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier | None = None,
         block_hash: HexBytes | None = None,
     ) -> Iterable[EventData]:
         return cast(
             Iterable[EventData],
             super().get_logs(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
             ),
         )
 
     @classmethod
     def get_logs(  # type: ignore
-        cls: Type["IERC4626HyperdriveRemoveLiquidityContractEvent"],
+        cls: Type["IHyperdriveSweepCollectorUpdatedContractEvent"],
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier | None = None,
         block_hash: HexBytes | None = None,
     ) -> Iterable[EventData]:
         return cast(
             Iterable[EventData],
             super().get_logs(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
             ),
         )
 
     def create_filter(  # type: ignore
-        self: "IERC4626HyperdriveRemoveLiquidityContractEvent",
+        self: "IHyperdriveSweepCollectorUpdatedContractEvent",
         *,  # PEP 3102
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier = "latest",
         address: ChecksumAddress | None = None,
         topics: Sequence[Any] | None = None,
     ) -> LogFilter:
@@ -2950,15 +3242,15 @@
             super().create_filter(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
             ),
         )
 
     @classmethod
     def create_filter(  # type: ignore
-        cls: Type["IERC4626HyperdriveRemoveLiquidityContractEvent"],
+        cls: Type["IHyperdriveSweepCollectorUpdatedContractEvent"],
         *,  # PEP 3102
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier = "latest",
         address: ChecksumAddress | None = None,
         topics: Sequence[Any] | None = None,
     ) -> LogFilter:
@@ -2966,58 +3258,58 @@
             LogFilter,
             super().create_filter(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
             ),
         )
 
 
-class IERC4626HyperdriveTransferSingleContractEvent(ContractEvent):
+class IHyperdriveTransferSingleContractEvent(ContractEvent):
     """ContractEvent for TransferSingle."""
 
     # super() get_logs and create_filter methods are generic, while our version adds values & types
     # pylint: disable=arguments-differ
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # pylint: disable=useless-parent-delegation
     def __init__(self, *argument_names: tuple[str]) -> None:
         super().__init__(*argument_names)
 
     def get_logs(  # type: ignore
-        self: "IERC4626HyperdriveTransferSingleContractEvent",
+        self: "IHyperdriveTransferSingleContractEvent",
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier | None = None,
         block_hash: HexBytes | None = None,
     ) -> Iterable[EventData]:
         return cast(
             Iterable[EventData],
             super().get_logs(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
             ),
         )
 
     @classmethod
     def get_logs(  # type: ignore
-        cls: Type["IERC4626HyperdriveTransferSingleContractEvent"],
+        cls: Type["IHyperdriveTransferSingleContractEvent"],
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier | None = None,
         block_hash: HexBytes | None = None,
     ) -> Iterable[EventData]:
         return cast(
             Iterable[EventData],
             super().get_logs(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, block_hash=block_hash
             ),
         )
 
     def create_filter(  # type: ignore
-        self: "IERC4626HyperdriveTransferSingleContractEvent",
+        self: "IHyperdriveTransferSingleContractEvent",
         *,  # PEP 3102
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier = "latest",
         address: ChecksumAddress | None = None,
         topics: Sequence[Any] | None = None,
     ) -> LogFilter:
@@ -3026,15 +3318,15 @@
             super().create_filter(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
             ),
         )
 
     @classmethod
     def create_filter(  # type: ignore
-        cls: Type["IERC4626HyperdriveTransferSingleContractEvent"],
+        cls: Type["IHyperdriveTransferSingleContractEvent"],
         *,  # PEP 3102
         argument_filters: dict[str, Any] | None = None,
         fromBlock: BlockIdentifier | None = None,
         toBlock: BlockIdentifier = "latest",
         address: ChecksumAddress | None = None,
         topics: Sequence[Any] | None = None,
     ) -> LogFilter:
@@ -3042,2401 +3334,2295 @@
             LogFilter,
             super().create_filter(
                 argument_filters=argument_filters, fromBlock=fromBlock, toBlock=toBlock, address=address, topics=topics
             ),
         )
 
 
-class IERC4626HyperdriveContractEvents(ContractEvents):
-    """ContractEvents for the IERC4626Hyperdrive contract."""
+class IHyperdriveContractEvents(ContractEvents):
+    """ContractEvents for the IHyperdrive contract."""
+
+    AddLiquidity: IHyperdriveAddLiquidityContractEvent
 
-    AddLiquidity: IERC4626HyperdriveAddLiquidityContractEvent
+    Approval: IHyperdriveApprovalContractEvent
 
-    Approval: IERC4626HyperdriveApprovalContractEvent
+    ApprovalForAll: IHyperdriveApprovalForAllContractEvent
 
-    ApprovalForAll: IERC4626HyperdriveApprovalForAllContractEvent
+    CloseLong: IHyperdriveCloseLongContractEvent
 
-    CloseLong: IERC4626HyperdriveCloseLongContractEvent
+    CloseShort: IHyperdriveCloseShortContractEvent
 
-    CloseShort: IERC4626HyperdriveCloseShortContractEvent
+    CollectGovernanceFee: IHyperdriveCollectGovernanceFeeContractEvent
 
-    CollectGovernanceFee: IERC4626HyperdriveCollectGovernanceFeeContractEvent
+    CreateCheckpoint: IHyperdriveCreateCheckpointContractEvent
 
-    CreateCheckpoint: IERC4626HyperdriveCreateCheckpointContractEvent
+    FeeCollectorUpdated: IHyperdriveFeeCollectorUpdatedContractEvent
 
-    GovernanceUpdated: IERC4626HyperdriveGovernanceUpdatedContractEvent
+    GovernanceUpdated: IHyperdriveGovernanceUpdatedContractEvent
 
-    Initialize: IERC4626HyperdriveInitializeContractEvent
+    Initialize: IHyperdriveInitializeContractEvent
 
-    OpenLong: IERC4626HyperdriveOpenLongContractEvent
+    OpenLong: IHyperdriveOpenLongContractEvent
 
-    OpenShort: IERC4626HyperdriveOpenShortContractEvent
+    OpenShort: IHyperdriveOpenShortContractEvent
 
-    PauseStatusUpdated: IERC4626HyperdrivePauseStatusUpdatedContractEvent
+    PauseStatusUpdated: IHyperdrivePauseStatusUpdatedContractEvent
 
-    PauserUpdated: IERC4626HyperdrivePauserUpdatedContractEvent
+    PauserUpdated: IHyperdrivePauserUpdatedContractEvent
 
-    RedeemWithdrawalShares: IERC4626HyperdriveRedeemWithdrawalSharesContractEvent
+    RedeemWithdrawalShares: IHyperdriveRedeemWithdrawalSharesContractEvent
 
-    RemoveLiquidity: IERC4626HyperdriveRemoveLiquidityContractEvent
+    RemoveLiquidity: IHyperdriveRemoveLiquidityContractEvent
 
-    TransferSingle: IERC4626HyperdriveTransferSingleContractEvent
+    Sweep: IHyperdriveSweepContractEvent
+
+    SweepCollectorUpdated: IHyperdriveSweepCollectorUpdatedContractEvent
+
+    TransferSingle: IHyperdriveTransferSingleContractEvent
 
     def __init__(
         self,
         abi: ABI,
         w3: "Web3",
         address: ChecksumAddress | None = None,
     ) -> None:
         super().__init__(abi, w3, address)
         self.AddLiquidity = cast(
-            IERC4626HyperdriveAddLiquidityContractEvent,
-            IERC4626HyperdriveAddLiquidityContractEvent.factory(
+            IHyperdriveAddLiquidityContractEvent,
+            IHyperdriveAddLiquidityContractEvent.factory(
                 "AddLiquidity", w3=w3, contract_abi=abi, address=address, event_name="AddLiquidity"
             ),
         )
         self.Approval = cast(
-            IERC4626HyperdriveApprovalContractEvent,
-            IERC4626HyperdriveApprovalContractEvent.factory(
+            IHyperdriveApprovalContractEvent,
+            IHyperdriveApprovalContractEvent.factory(
                 "Approval", w3=w3, contract_abi=abi, address=address, event_name="Approval"
             ),
         )
         self.ApprovalForAll = cast(
-            IERC4626HyperdriveApprovalForAllContractEvent,
-            IERC4626HyperdriveApprovalForAllContractEvent.factory(
+            IHyperdriveApprovalForAllContractEvent,
+            IHyperdriveApprovalForAllContractEvent.factory(
                 "ApprovalForAll", w3=w3, contract_abi=abi, address=address, event_name="ApprovalForAll"
             ),
         )
         self.CloseLong = cast(
-            IERC4626HyperdriveCloseLongContractEvent,
-            IERC4626HyperdriveCloseLongContractEvent.factory(
+            IHyperdriveCloseLongContractEvent,
+            IHyperdriveCloseLongContractEvent.factory(
                 "CloseLong", w3=w3, contract_abi=abi, address=address, event_name="CloseLong"
             ),
         )
         self.CloseShort = cast(
-            IERC4626HyperdriveCloseShortContractEvent,
-            IERC4626HyperdriveCloseShortContractEvent.factory(
+            IHyperdriveCloseShortContractEvent,
+            IHyperdriveCloseShortContractEvent.factory(
                 "CloseShort", w3=w3, contract_abi=abi, address=address, event_name="CloseShort"
             ),
         )
         self.CollectGovernanceFee = cast(
-            IERC4626HyperdriveCollectGovernanceFeeContractEvent,
-            IERC4626HyperdriveCollectGovernanceFeeContractEvent.factory(
+            IHyperdriveCollectGovernanceFeeContractEvent,
+            IHyperdriveCollectGovernanceFeeContractEvent.factory(
                 "CollectGovernanceFee", w3=w3, contract_abi=abi, address=address, event_name="CollectGovernanceFee"
             ),
         )
         self.CreateCheckpoint = cast(
-            IERC4626HyperdriveCreateCheckpointContractEvent,
-            IERC4626HyperdriveCreateCheckpointContractEvent.factory(
+            IHyperdriveCreateCheckpointContractEvent,
+            IHyperdriveCreateCheckpointContractEvent.factory(
                 "CreateCheckpoint", w3=w3, contract_abi=abi, address=address, event_name="CreateCheckpoint"
             ),
         )
+        self.FeeCollectorUpdated = cast(
+            IHyperdriveFeeCollectorUpdatedContractEvent,
+            IHyperdriveFeeCollectorUpdatedContractEvent.factory(
+                "FeeCollectorUpdated", w3=w3, contract_abi=abi, address=address, event_name="FeeCollectorUpdated"
+            ),
+        )
         self.GovernanceUpdated = cast(
-            IERC4626HyperdriveGovernanceUpdatedContractEvent,
-            IERC4626HyperdriveGovernanceUpdatedContractEvent.factory(
+            IHyperdriveGovernanceUpdatedContractEvent,
+            IHyperdriveGovernanceUpdatedContractEvent.factory(
                 "GovernanceUpdated", w3=w3, contract_abi=abi, address=address, event_name="GovernanceUpdated"
             ),
         )
         self.Initialize = cast(
-            IERC4626HyperdriveInitializeContractEvent,
-            IERC4626HyperdriveInitializeContractEvent.factory(
+            IHyperdriveInitializeContractEvent,
+            IHyperdriveInitializeContractEvent.factory(
                 "Initialize", w3=w3, contract_abi=abi, address=address, event_name="Initialize"
             ),
         )
         self.OpenLong = cast(
-            IERC4626HyperdriveOpenLongContractEvent,
-            IERC4626HyperdriveOpenLongContractEvent.factory(
+            IHyperdriveOpenLongContractEvent,
+            IHyperdriveOpenLongContractEvent.factory(
                 "OpenLong", w3=w3, contract_abi=abi, address=address, event_name="OpenLong"
             ),
         )
         self.OpenShort = cast(
-            IERC4626HyperdriveOpenShortContractEvent,
-            IERC4626HyperdriveOpenShortContractEvent.factory(
+            IHyperdriveOpenShortContractEvent,
+            IHyperdriveOpenShortContractEvent.factory(
                 "OpenShort", w3=w3, contract_abi=abi, address=address, event_name="OpenShort"
             ),
         )
         self.PauseStatusUpdated = cast(
-            IERC4626HyperdrivePauseStatusUpdatedContractEvent,
-            IERC4626HyperdrivePauseStatusUpdatedContractEvent.factory(
+            IHyperdrivePauseStatusUpdatedContractEvent,
+            IHyperdrivePauseStatusUpdatedContractEvent.factory(
                 "PauseStatusUpdated", w3=w3, contract_abi=abi, address=address, event_name="PauseStatusUpdated"
             ),
         )
         self.PauserUpdated = cast(
-            IERC4626HyperdrivePauserUpdatedContractEvent,
-            IERC4626HyperdrivePauserUpdatedContractEvent.factory(
+            IHyperdrivePauserUpdatedContractEvent,
+            IHyperdrivePauserUpdatedContractEvent.factory(
                 "PauserUpdated", w3=w3, contract_abi=abi, address=address, event_name="PauserUpdated"
             ),
         )
         self.RedeemWithdrawalShares = cast(
-            IERC4626HyperdriveRedeemWithdrawalSharesContractEvent,
-            IERC4626HyperdriveRedeemWithdrawalSharesContractEvent.factory(
+            IHyperdriveRedeemWithdrawalSharesContractEvent,
+            IHyperdriveRedeemWithdrawalSharesContractEvent.factory(
                 "RedeemWithdrawalShares", w3=w3, contract_abi=abi, address=address, event_name="RedeemWithdrawalShares"
             ),
         )
         self.RemoveLiquidity = cast(
-            IERC4626HyperdriveRemoveLiquidityContractEvent,
-            IERC4626HyperdriveRemoveLiquidityContractEvent.factory(
+            IHyperdriveRemoveLiquidityContractEvent,
+            IHyperdriveRemoveLiquidityContractEvent.factory(
                 "RemoveLiquidity", w3=w3, contract_abi=abi, address=address, event_name="RemoveLiquidity"
             ),
         )
+        self.Sweep = cast(
+            IHyperdriveSweepContractEvent,
+            IHyperdriveSweepContractEvent.factory(
+                "Sweep", w3=w3, contract_abi=abi, address=address, event_name="Sweep"
+            ),
+        )
+        self.SweepCollectorUpdated = cast(
+            IHyperdriveSweepCollectorUpdatedContractEvent,
+            IHyperdriveSweepCollectorUpdatedContractEvent.factory(
+                "SweepCollectorUpdated", w3=w3, contract_abi=abi, address=address, event_name="SweepCollectorUpdated"
+            ),
+        )
         self.TransferSingle = cast(
-            IERC4626HyperdriveTransferSingleContractEvent,
-            IERC4626HyperdriveTransferSingleContractEvent.factory(
+            IHyperdriveTransferSingleContractEvent,
+            IHyperdriveTransferSingleContractEvent.factory(
                 "TransferSingle", w3=w3, contract_abi=abi, address=address, event_name="TransferSingle"
             ),
         )
 
 
-class IERC4626HyperdriveBatchInputLengthMismatchContractError:
+class IHyperdriveBatchInputLengthMismatchContractError:
     """ContractError for BatchInputLengthMismatch."""
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # 4 byte error selector
     selector: str
     # error signature, i.e. CustomError(uint256,bool)
     signature: str
 
     # pylint: disable=useless-parent-delegation
     def __init__(
-        self: "IERC4626HyperdriveBatchInputLengthMismatchContractError",
+        self: "IHyperdriveBatchInputLengthMismatchContractError",
     ) -> None:
         self.selector = "0xba430d38"
         self.signature = "BatchInputLengthMismatch()"
 
     def decode_error_data(  # type: ignore
-        self: "IERC4626HyperdriveBatchInputLengthMismatchContractError",
+        self: "IHyperdriveBatchInputLengthMismatchContractError",
         data: HexBytes,
         # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "BatchInputLengthMismatch" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
     @classmethod
     def decode_error_data(  # type: ignore
-        cls: Type["IERC4626HyperdriveBatchInputLengthMismatchContractError"],
+        cls: Type["IHyperdriveBatchInputLengthMismatchContractError"],
         data: HexBytes,
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "BatchInputLengthMismatch" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
 
-class IERC4626HyperdriveBelowMinimumContributionContractError:
+class IHyperdriveBelowMinimumContributionContractError:
     """ContractError for BelowMinimumContribution."""
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # 4 byte error selector
     selector: str
     # error signature, i.e. CustomError(uint256,bool)
     signature: str
 
     # pylint: disable=useless-parent-delegation
     def __init__(
-        self: "IERC4626HyperdriveBelowMinimumContributionContractError",
+        self: "IHyperdriveBelowMinimumContributionContractError",
     ) -> None:
         self.selector = "0xabed41c4"
         self.signature = "BelowMinimumContribution()"
 
     def decode_error_data(  # type: ignore
-        self: "IERC4626HyperdriveBelowMinimumContributionContractError",
+        self: "IHyperdriveBelowMinimumContributionContractError",
         data: HexBytes,
         # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "BelowMinimumContribution" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
     @classmethod
     def decode_error_data(  # type: ignore
-        cls: Type["IERC4626HyperdriveBelowMinimumContributionContractError"],
+        cls: Type["IHyperdriveBelowMinimumContributionContractError"],
         data: HexBytes,
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "BelowMinimumContribution" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
 
-class IERC4626HyperdriveDecreasedPresentValueWhenAddingLiquidityContractError:
+class IHyperdriveDecreasedPresentValueWhenAddingLiquidityContractError:
     """ContractError for DecreasedPresentValueWhenAddingLiquidity."""
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # 4 byte error selector
     selector: str
     # error signature, i.e. CustomError(uint256,bool)
     signature: str
 
     # pylint: disable=useless-parent-delegation
     def __init__(
-        self: "IERC4626HyperdriveDecreasedPresentValueWhenAddingLiquidityContractError",
+        self: "IHyperdriveDecreasedPresentValueWhenAddingLiquidityContractError",
     ) -> None:
         self.selector = "0x309b2a42"
         self.signature = "DecreasedPresentValueWhenAddingLiquidity()"
 
     def decode_error_data(  # type: ignore
-        self: "IERC4626HyperdriveDecreasedPresentValueWhenAddingLiquidityContractError",
+        self: "IHyperdriveDecreasedPresentValueWhenAddingLiquidityContractError",
         data: HexBytes,
         # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "DecreasedPresentValueWhenAddingLiquidity" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
     @classmethod
     def decode_error_data(  # type: ignore
-        cls: Type["IERC4626HyperdriveDecreasedPresentValueWhenAddingLiquidityContractError"],
+        cls: Type["IHyperdriveDecreasedPresentValueWhenAddingLiquidityContractError"],
         data: HexBytes,
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "DecreasedPresentValueWhenAddingLiquidity" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
 
-class IERC4626HyperdriveDistributeExcessIdleFailedContractError:
+class IHyperdriveDistributeExcessIdleFailedContractError:
     """ContractError for DistributeExcessIdleFailed."""
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # 4 byte error selector
     selector: str
     # error signature, i.e. CustomError(uint256,bool)
     signature: str
 
     # pylint: disable=useless-parent-delegation
     def __init__(
-        self: "IERC4626HyperdriveDistributeExcessIdleFailedContractError",
+        self: "IHyperdriveDistributeExcessIdleFailedContractError",
     ) -> None:
         self.selector = "0x8bdf918d"
         self.signature = "DistributeExcessIdleFailed()"
 
     def decode_error_data(  # type: ignore
-        self: "IERC4626HyperdriveDistributeExcessIdleFailedContractError",
+        self: "IHyperdriveDistributeExcessIdleFailedContractError",
         data: HexBytes,
         # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "DistributeExcessIdleFailed" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
     @classmethod
     def decode_error_data(  # type: ignore
-        cls: Type["IERC4626HyperdriveDistributeExcessIdleFailedContractError"],
+        cls: Type["IHyperdriveDistributeExcessIdleFailedContractError"],
         data: HexBytes,
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "DistributeExcessIdleFailed" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
 
-class IERC4626HyperdriveExpInvalidExponentContractError:
+class IHyperdriveExpInvalidExponentContractError:
     """ContractError for ExpInvalidExponent."""
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # 4 byte error selector
     selector: str
     # error signature, i.e. CustomError(uint256,bool)
     signature: str
 
     # pylint: disable=useless-parent-delegation
     def __init__(
-        self: "IERC4626HyperdriveExpInvalidExponentContractError",
+        self: "IHyperdriveExpInvalidExponentContractError",
     ) -> None:
         self.selector = "0x73a2d6b1"
         self.signature = "ExpInvalidExponent()"
 
     def decode_error_data(  # type: ignore
-        self: "IERC4626HyperdriveExpInvalidExponentContractError",
+        self: "IHyperdriveExpInvalidExponentContractError",
         data: HexBytes,
         # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "ExpInvalidExponent" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
     @classmethod
     def decode_error_data(  # type: ignore
-        cls: Type["IERC4626HyperdriveExpInvalidExponentContractError"],
+        cls: Type["IHyperdriveExpInvalidExponentContractError"],
         data: HexBytes,
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "ExpInvalidExponent" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
 
-class IERC4626HyperdriveExpiredDeadlineContractError:
+class IHyperdriveExpiredDeadlineContractError:
     """ContractError for ExpiredDeadline."""
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # 4 byte error selector
     selector: str
     # error signature, i.e. CustomError(uint256,bool)
     signature: str
 
     # pylint: disable=useless-parent-delegation
     def __init__(
-        self: "IERC4626HyperdriveExpiredDeadlineContractError",
+        self: "IHyperdriveExpiredDeadlineContractError",
     ) -> None:
         self.selector = "0xf87d9271"
         self.signature = "ExpiredDeadline()"
 
     def decode_error_data(  # type: ignore
-        self: "IERC4626HyperdriveExpiredDeadlineContractError",
+        self: "IHyperdriveExpiredDeadlineContractError",
         data: HexBytes,
         # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
-            [
-                item
-                for item in ierc4626hyperdrive_abi
-                if item.get("name") == "ExpiredDeadline" and item.get("type") == "error"
-            ][0],
+            [item for item in ihyperdrive_abi if item.get("name") == "ExpiredDeadline" and item.get("type") == "error"][
+                0
+            ],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
     @classmethod
     def decode_error_data(  # type: ignore
-        cls: Type["IERC4626HyperdriveExpiredDeadlineContractError"],
+        cls: Type["IHyperdriveExpiredDeadlineContractError"],
         data: HexBytes,
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
-            [
-                item
-                for item in ierc4626hyperdrive_abi
-                if item.get("name") == "ExpiredDeadline" and item.get("type") == "error"
-            ][0],
+            [item for item in ihyperdrive_abi if item.get("name") == "ExpiredDeadline" and item.get("type") == "error"][
+                0
+            ],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
 
-class IERC4626HyperdriveInsufficientBalanceContractError:
+class IHyperdriveInsufficientBalanceContractError:
     """ContractError for InsufficientBalance."""
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # 4 byte error selector
     selector: str
     # error signature, i.e. CustomError(uint256,bool)
     signature: str
 
     # pylint: disable=useless-parent-delegation
     def __init__(
-        self: "IERC4626HyperdriveInsufficientBalanceContractError",
+        self: "IHyperdriveInsufficientBalanceContractError",
     ) -> None:
         self.selector = "0xf4d678b8"
         self.signature = "InsufficientBalance()"
 
     def decode_error_data(  # type: ignore
-        self: "IERC4626HyperdriveInsufficientBalanceContractError",
+        self: "IHyperdriveInsufficientBalanceContractError",
         data: HexBytes,
         # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "InsufficientBalance" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
     @classmethod
     def decode_error_data(  # type: ignore
-        cls: Type["IERC4626HyperdriveInsufficientBalanceContractError"],
+        cls: Type["IHyperdriveInsufficientBalanceContractError"],
         data: HexBytes,
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "InsufficientBalance" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
 
-class IERC4626HyperdriveInsufficientLiquidityContractError:
+class IHyperdriveInsufficientLiquidityContractError:
     """ContractError for InsufficientLiquidity."""
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # 4 byte error selector
     selector: str
     # error signature, i.e. CustomError(uint256,bool)
     signature: str
 
     # pylint: disable=useless-parent-delegation
     def __init__(
-        self: "IERC4626HyperdriveInsufficientLiquidityContractError",
+        self: "IHyperdriveInsufficientLiquidityContractError",
     ) -> None:
-        self.selector = "0x780daf16"
-        self.signature = "InsufficientLiquidity(uint8)"
+        self.selector = "0xbb55fd27"
+        self.signature = "InsufficientLiquidity()"
 
     def decode_error_data(  # type: ignore
-        self: "IERC4626HyperdriveInsufficientLiquidityContractError",
+        self: "IHyperdriveInsufficientLiquidityContractError",
         data: HexBytes,
         # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "InsufficientLiquidity" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
     @classmethod
     def decode_error_data(  # type: ignore
-        cls: Type["IERC4626HyperdriveInsufficientLiquidityContractError"],
+        cls: Type["IHyperdriveInsufficientLiquidityContractError"],
         data: HexBytes,
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "InsufficientLiquidity" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
 
-class IERC4626HyperdriveInvalidAprContractError:
+class IHyperdriveInvalidAprContractError:
     """ContractError for InvalidApr."""
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # 4 byte error selector
     selector: str
     # error signature, i.e. CustomError(uint256,bool)
     signature: str
 
     # pylint: disable=useless-parent-delegation
     def __init__(
-        self: "IERC4626HyperdriveInvalidAprContractError",
+        self: "IHyperdriveInvalidAprContractError",
     ) -> None:
         self.selector = "0x76c22a22"
         self.signature = "InvalidApr()"
 
     def decode_error_data(  # type: ignore
-        self: "IERC4626HyperdriveInvalidAprContractError",
+        self: "IHyperdriveInvalidAprContractError",
         data: HexBytes,
         # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
-            [
-                item
-                for item in ierc4626hyperdrive_abi
-                if item.get("name") == "InvalidApr" and item.get("type") == "error"
-            ][0],
+            [item for item in ihyperdrive_abi if item.get("name") == "InvalidApr" and item.get("type") == "error"][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
     @classmethod
     def decode_error_data(  # type: ignore
-        cls: Type["IERC4626HyperdriveInvalidAprContractError"],
+        cls: Type["IHyperdriveInvalidAprContractError"],
         data: HexBytes,
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
-            [
-                item
-                for item in ierc4626hyperdrive_abi
-                if item.get("name") == "InvalidApr" and item.get("type") == "error"
-            ][0],
+            [item for item in ihyperdrive_abi if item.get("name") == "InvalidApr" and item.get("type") == "error"][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
 
-class IERC4626HyperdriveInvalidBaseTokenContractError:
-    """ContractError for InvalidBaseToken."""
-
-    # @combomethod destroys return types, so we are redefining functions as both class and instance
-    # pylint: disable=function-redefined
-
-    # 4 byte error selector
-    selector: str
-    # error signature, i.e. CustomError(uint256,bool)
-    signature: str
-
-    # pylint: disable=useless-parent-delegation
-    def __init__(
-        self: "IERC4626HyperdriveInvalidBaseTokenContractError",
-    ) -> None:
-        self.selector = "0x0e442a4a"
-        self.signature = "InvalidBaseToken()"
-
-    def decode_error_data(  # type: ignore
-        self: "IERC4626HyperdriveInvalidBaseTokenContractError",
-        data: HexBytes,
-        # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
-    ) -> tuple[Any, ...]:
-        """Decodes error data returns from a smart contract."""
-        error_abi = cast(
-            ABIFunction,
-            [
-                item
-                for item in ierc4626hyperdrive_abi
-                if item.get("name") == "InvalidBaseToken" and item.get("type") == "error"
-            ][0],
-        )
-        types = get_abi_input_types(error_abi)
-        abi_codec = ABICodec(default_registry)
-        decoded = abi_codec.decode(types, data)
-        return decoded
-
-    @classmethod
-    def decode_error_data(  # type: ignore
-        cls: Type["IERC4626HyperdriveInvalidBaseTokenContractError"],
-        data: HexBytes,
-    ) -> tuple[Any, ...]:
-        """Decodes error data returns from a smart contract."""
-        error_abi = cast(
-            ABIFunction,
-            [
-                item
-                for item in ierc4626hyperdrive_abi
-                if item.get("name") == "InvalidBaseToken" and item.get("type") == "error"
-            ][0],
-        )
-        types = get_abi_input_types(error_abi)
-        abi_codec = ABICodec(default_registry)
-        decoded = abi_codec.decode(types, data)
-        return decoded
-
-
-class IERC4626HyperdriveInvalidCheckpointTimeContractError:
+class IHyperdriveInvalidCheckpointTimeContractError:
     """ContractError for InvalidCheckpointTime."""
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # 4 byte error selector
     selector: str
     # error signature, i.e. CustomError(uint256,bool)
     signature: str
 
     # pylint: disable=useless-parent-delegation
     def __init__(
-        self: "IERC4626HyperdriveInvalidCheckpointTimeContractError",
+        self: "IHyperdriveInvalidCheckpointTimeContractError",
     ) -> None:
         self.selector = "0xecd29e81"
         self.signature = "InvalidCheckpointTime()"
 
     def decode_error_data(  # type: ignore
-        self: "IERC4626HyperdriveInvalidCheckpointTimeContractError",
+        self: "IHyperdriveInvalidCheckpointTimeContractError",
         data: HexBytes,
         # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "InvalidCheckpointTime" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
     @classmethod
     def decode_error_data(  # type: ignore
-        cls: Type["IERC4626HyperdriveInvalidCheckpointTimeContractError"],
+        cls: Type["IHyperdriveInvalidCheckpointTimeContractError"],
         data: HexBytes,
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "InvalidCheckpointTime" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
 
-class IERC4626HyperdriveInvalidERC20BridgeContractError:
+class IHyperdriveInvalidERC20BridgeContractError:
     """ContractError for InvalidERC20Bridge."""
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # 4 byte error selector
     selector: str
     # error signature, i.e. CustomError(uint256,bool)
     signature: str
 
     # pylint: disable=useless-parent-delegation
     def __init__(
-        self: "IERC4626HyperdriveInvalidERC20BridgeContractError",
+        self: "IHyperdriveInvalidERC20BridgeContractError",
     ) -> None:
         self.selector = "0x2aab8bd3"
         self.signature = "InvalidERC20Bridge()"
 
     def decode_error_data(  # type: ignore
-        self: "IERC4626HyperdriveInvalidERC20BridgeContractError",
+        self: "IHyperdriveInvalidERC20BridgeContractError",
         data: HexBytes,
         # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "InvalidERC20Bridge" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
     @classmethod
     def decode_error_data(  # type: ignore
-        cls: Type["IERC4626HyperdriveInvalidERC20BridgeContractError"],
+        cls: Type["IHyperdriveInvalidERC20BridgeContractError"],
         data: HexBytes,
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "InvalidERC20Bridge" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
 
-class IERC4626HyperdriveInvalidFeeDestinationContractError:
+class IHyperdriveInvalidFeeDestinationContractError:
     """ContractError for InvalidFeeDestination."""
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # 4 byte error selector
     selector: str
     # error signature, i.e. CustomError(uint256,bool)
     signature: str
 
     # pylint: disable=useless-parent-delegation
     def __init__(
-        self: "IERC4626HyperdriveInvalidFeeDestinationContractError",
+        self: "IHyperdriveInvalidFeeDestinationContractError",
     ) -> None:
         self.selector = "0x2b44eccc"
         self.signature = "InvalidFeeDestination()"
 
     def decode_error_data(  # type: ignore
-        self: "IERC4626HyperdriveInvalidFeeDestinationContractError",
+        self: "IHyperdriveInvalidFeeDestinationContractError",
         data: HexBytes,
         # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "InvalidFeeDestination" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
     @classmethod
     def decode_error_data(  # type: ignore
-        cls: Type["IERC4626HyperdriveInvalidFeeDestinationContractError"],
+        cls: Type["IHyperdriveInvalidFeeDestinationContractError"],
         data: HexBytes,
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "InvalidFeeDestination" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
 
-class IERC4626HyperdriveInvalidInitialVaultSharePriceContractError:
+class IHyperdriveInvalidInitialVaultSharePriceContractError:
     """ContractError for InvalidInitialVaultSharePrice."""
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # 4 byte error selector
     selector: str
     # error signature, i.e. CustomError(uint256,bool)
     signature: str
 
     # pylint: disable=useless-parent-delegation
     def __init__(
-        self: "IERC4626HyperdriveInvalidInitialVaultSharePriceContractError",
+        self: "IHyperdriveInvalidInitialVaultSharePriceContractError",
     ) -> None:
         self.selector = "0x094b19ad"
         self.signature = "InvalidInitialVaultSharePrice()"
 
     def decode_error_data(  # type: ignore
-        self: "IERC4626HyperdriveInvalidInitialVaultSharePriceContractError",
+        self: "IHyperdriveInvalidInitialVaultSharePriceContractError",
         data: HexBytes,
         # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "InvalidInitialVaultSharePrice" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
     @classmethod
     def decode_error_data(  # type: ignore
-        cls: Type["IERC4626HyperdriveInvalidInitialVaultSharePriceContractError"],
+        cls: Type["IHyperdriveInvalidInitialVaultSharePriceContractError"],
         data: HexBytes,
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "InvalidInitialVaultSharePrice" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
 
-class IERC4626HyperdriveInvalidLPSharePriceContractError:
+class IHyperdriveInvalidLPSharePriceContractError:
     """ContractError for InvalidLPSharePrice."""
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # 4 byte error selector
     selector: str
     # error signature, i.e. CustomError(uint256,bool)
     signature: str
 
     # pylint: disable=useless-parent-delegation
     def __init__(
-        self: "IERC4626HyperdriveInvalidLPSharePriceContractError",
+        self: "IHyperdriveInvalidLPSharePriceContractError",
     ) -> None:
         self.selector = "0xabeba7ee"
         self.signature = "InvalidLPSharePrice()"
 
     def decode_error_data(  # type: ignore
-        self: "IERC4626HyperdriveInvalidLPSharePriceContractError",
+        self: "IHyperdriveInvalidLPSharePriceContractError",
         data: HexBytes,
         # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "InvalidLPSharePrice" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
     @classmethod
     def decode_error_data(  # type: ignore
-        cls: Type["IERC4626HyperdriveInvalidLPSharePriceContractError"],
+        cls: Type["IHyperdriveInvalidLPSharePriceContractError"],
         data: HexBytes,
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "InvalidLPSharePrice" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
 
-class IERC4626HyperdriveInvalidPresentValueContractError:
+class IHyperdriveInvalidPresentValueContractError:
     """ContractError for InvalidPresentValue."""
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # 4 byte error selector
     selector: str
     # error signature, i.e. CustomError(uint256,bool)
     signature: str
 
     # pylint: disable=useless-parent-delegation
     def __init__(
-        self: "IERC4626HyperdriveInvalidPresentValueContractError",
+        self: "IHyperdriveInvalidPresentValueContractError",
     ) -> None:
         self.selector = "0xaa2c6516"
         self.signature = "InvalidPresentValue()"
 
     def decode_error_data(  # type: ignore
-        self: "IERC4626HyperdriveInvalidPresentValueContractError",
+        self: "IHyperdriveInvalidPresentValueContractError",
         data: HexBytes,
         # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "InvalidPresentValue" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
     @classmethod
     def decode_error_data(  # type: ignore
-        cls: Type["IERC4626HyperdriveInvalidPresentValueContractError"],
+        cls: Type["IHyperdriveInvalidPresentValueContractError"],
         data: HexBytes,
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "InvalidPresentValue" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
 
-class IERC4626HyperdriveInvalidShareReservesContractError:
-    """ContractError for InvalidShareReserves."""
-
-    # @combomethod destroys return types, so we are redefining functions as both class and instance
-    # pylint: disable=function-redefined
-
-    # 4 byte error selector
-    selector: str
-    # error signature, i.e. CustomError(uint256,bool)
-    signature: str
-
-    # pylint: disable=useless-parent-delegation
-    def __init__(
-        self: "IERC4626HyperdriveInvalidShareReservesContractError",
-    ) -> None:
-        self.selector = "0xb0bfcdbe"
-        self.signature = "InvalidShareReserves()"
-
-    def decode_error_data(  # type: ignore
-        self: "IERC4626HyperdriveInvalidShareReservesContractError",
-        data: HexBytes,
-        # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
-    ) -> tuple[Any, ...]:
-        """Decodes error data returns from a smart contract."""
-        error_abi = cast(
-            ABIFunction,
-            [
-                item
-                for item in ierc4626hyperdrive_abi
-                if item.get("name") == "InvalidShareReserves" and item.get("type") == "error"
-            ][0],
-        )
-        types = get_abi_input_types(error_abi)
-        abi_codec = ABICodec(default_registry)
-        decoded = abi_codec.decode(types, data)
-        return decoded
-
-    @classmethod
-    def decode_error_data(  # type: ignore
-        cls: Type["IERC4626HyperdriveInvalidShareReservesContractError"],
-        data: HexBytes,
-    ) -> tuple[Any, ...]:
-        """Decodes error data returns from a smart contract."""
-        error_abi = cast(
-            ABIFunction,
-            [
-                item
-                for item in ierc4626hyperdrive_abi
-                if item.get("name") == "InvalidShareReserves" and item.get("type") == "error"
-            ][0],
-        )
-        types = get_abi_input_types(error_abi)
-        abi_codec = ABICodec(default_registry)
-        decoded = abi_codec.decode(types, data)
-        return decoded
-
-
-class IERC4626HyperdriveInvalidSignatureContractError:
+class IHyperdriveInvalidSignatureContractError:
     """ContractError for InvalidSignature."""
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # 4 byte error selector
     selector: str
     # error signature, i.e. CustomError(uint256,bool)
     signature: str
 
     # pylint: disable=useless-parent-delegation
     def __init__(
-        self: "IERC4626HyperdriveInvalidSignatureContractError",
+        self: "IHyperdriveInvalidSignatureContractError",
     ) -> None:
         self.selector = "0x8baa579f"
         self.signature = "InvalidSignature()"
 
     def decode_error_data(  # type: ignore
-        self: "IERC4626HyperdriveInvalidSignatureContractError",
+        self: "IHyperdriveInvalidSignatureContractError",
         data: HexBytes,
         # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "InvalidSignature" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
     @classmethod
     def decode_error_data(  # type: ignore
-        cls: Type["IERC4626HyperdriveInvalidSignatureContractError"],
+        cls: Type["IHyperdriveInvalidSignatureContractError"],
         data: HexBytes,
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "InvalidSignature" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
 
-class IERC4626HyperdriveInvalidTimestampContractError:
+class IHyperdriveInvalidTimestampContractError:
     """ContractError for InvalidTimestamp."""
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # 4 byte error selector
     selector: str
     # error signature, i.e. CustomError(uint256,bool)
     signature: str
 
     # pylint: disable=useless-parent-delegation
     def __init__(
-        self: "IERC4626HyperdriveInvalidTimestampContractError",
+        self: "IHyperdriveInvalidTimestampContractError",
     ) -> None:
         self.selector = "0xb7d09497"
         self.signature = "InvalidTimestamp()"
 
     def decode_error_data(  # type: ignore
-        self: "IERC4626HyperdriveInvalidTimestampContractError",
+        self: "IHyperdriveInvalidTimestampContractError",
         data: HexBytes,
         # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "InvalidTimestamp" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
     @classmethod
     def decode_error_data(  # type: ignore
-        cls: Type["IERC4626HyperdriveInvalidTimestampContractError"],
+        cls: Type["IHyperdriveInvalidTimestampContractError"],
         data: HexBytes,
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "InvalidTimestamp" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
 
-class IERC4626HyperdriveLnInvalidInputContractError:
+class IHyperdriveLnInvalidInputContractError:
     """ContractError for LnInvalidInput."""
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # 4 byte error selector
     selector: str
     # error signature, i.e. CustomError(uint256,bool)
     signature: str
 
     # pylint: disable=useless-parent-delegation
     def __init__(
-        self: "IERC4626HyperdriveLnInvalidInputContractError",
+        self: "IHyperdriveLnInvalidInputContractError",
     ) -> None:
         self.selector = "0xe61b4975"
         self.signature = "LnInvalidInput()"
 
     def decode_error_data(  # type: ignore
-        self: "IERC4626HyperdriveLnInvalidInputContractError",
+        self: "IHyperdriveLnInvalidInputContractError",
         data: HexBytes,
         # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
-            [
-                item
-                for item in ierc4626hyperdrive_abi
-                if item.get("name") == "LnInvalidInput" and item.get("type") == "error"
-            ][0],
+            [item for item in ihyperdrive_abi if item.get("name") == "LnInvalidInput" and item.get("type") == "error"][
+                0
+            ],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
     @classmethod
     def decode_error_data(  # type: ignore
-        cls: Type["IERC4626HyperdriveLnInvalidInputContractError"],
+        cls: Type["IHyperdriveLnInvalidInputContractError"],
         data: HexBytes,
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
-            [
-                item
-                for item in ierc4626hyperdrive_abi
-                if item.get("name") == "LnInvalidInput" and item.get("type") == "error"
-            ][0],
+            [item for item in ihyperdrive_abi if item.get("name") == "LnInvalidInput" and item.get("type") == "error"][
+                0
+            ],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
 
-class IERC4626HyperdriveMinimumSharePriceContractError:
+class IHyperdriveMinimumSharePriceContractError:
     """ContractError for MinimumSharePrice."""
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # 4 byte error selector
     selector: str
     # error signature, i.e. CustomError(uint256,bool)
     signature: str
 
     # pylint: disable=useless-parent-delegation
     def __init__(
-        self: "IERC4626HyperdriveMinimumSharePriceContractError",
+        self: "IHyperdriveMinimumSharePriceContractError",
     ) -> None:
         self.selector = "0x42af972b"
         self.signature = "MinimumSharePrice()"
 
     def decode_error_data(  # type: ignore
-        self: "IERC4626HyperdriveMinimumSharePriceContractError",
+        self: "IHyperdriveMinimumSharePriceContractError",
         data: HexBytes,
         # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "MinimumSharePrice" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
     @classmethod
     def decode_error_data(  # type: ignore
-        cls: Type["IERC4626HyperdriveMinimumSharePriceContractError"],
+        cls: Type["IHyperdriveMinimumSharePriceContractError"],
         data: HexBytes,
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "MinimumSharePrice" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
 
-class IERC4626HyperdriveMinimumTransactionAmountContractError:
+class IHyperdriveMinimumTransactionAmountContractError:
     """ContractError for MinimumTransactionAmount."""
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # 4 byte error selector
     selector: str
     # error signature, i.e. CustomError(uint256,bool)
     signature: str
 
     # pylint: disable=useless-parent-delegation
     def __init__(
-        self: "IERC4626HyperdriveMinimumTransactionAmountContractError",
+        self: "IHyperdriveMinimumTransactionAmountContractError",
     ) -> None:
         self.selector = "0x423bbb46"
         self.signature = "MinimumTransactionAmount()"
 
     def decode_error_data(  # type: ignore
-        self: "IERC4626HyperdriveMinimumTransactionAmountContractError",
+        self: "IHyperdriveMinimumTransactionAmountContractError",
         data: HexBytes,
         # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "MinimumTransactionAmount" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
     @classmethod
     def decode_error_data(  # type: ignore
-        cls: Type["IERC4626HyperdriveMinimumTransactionAmountContractError"],
+        cls: Type["IHyperdriveMinimumTransactionAmountContractError"],
         data: HexBytes,
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "MinimumTransactionAmount" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
 
-class IERC4626HyperdriveNotPayableContractError:
+class IHyperdriveNotPayableContractError:
     """ContractError for NotPayable."""
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # 4 byte error selector
     selector: str
     # error signature, i.e. CustomError(uint256,bool)
     signature: str
 
     # pylint: disable=useless-parent-delegation
     def __init__(
-        self: "IERC4626HyperdriveNotPayableContractError",
+        self: "IHyperdriveNotPayableContractError",
     ) -> None:
         self.selector = "0x1574f9f3"
         self.signature = "NotPayable()"
 
     def decode_error_data(  # type: ignore
-        self: "IERC4626HyperdriveNotPayableContractError",
+        self: "IHyperdriveNotPayableContractError",
         data: HexBytes,
         # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
-            [
-                item
-                for item in ierc4626hyperdrive_abi
-                if item.get("name") == "NotPayable" and item.get("type") == "error"
-            ][0],
+            [item for item in ihyperdrive_abi if item.get("name") == "NotPayable" and item.get("type") == "error"][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
     @classmethod
     def decode_error_data(  # type: ignore
-        cls: Type["IERC4626HyperdriveNotPayableContractError"],
+        cls: Type["IHyperdriveNotPayableContractError"],
         data: HexBytes,
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
-            [
-                item
-                for item in ierc4626hyperdrive_abi
-                if item.get("name") == "NotPayable" and item.get("type") == "error"
-            ][0],
+            [item for item in ihyperdrive_abi if item.get("name") == "NotPayable" and item.get("type") == "error"][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
 
-class IERC4626HyperdriveOutputLimitContractError:
+class IHyperdriveOutputLimitContractError:
     """ContractError for OutputLimit."""
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # 4 byte error selector
     selector: str
     # error signature, i.e. CustomError(uint256,bool)
     signature: str
 
     # pylint: disable=useless-parent-delegation
     def __init__(
-        self: "IERC4626HyperdriveOutputLimitContractError",
+        self: "IHyperdriveOutputLimitContractError",
     ) -> None:
         self.selector = "0xc9726517"
         self.signature = "OutputLimit()"
 
     def decode_error_data(  # type: ignore
-        self: "IERC4626HyperdriveOutputLimitContractError",
+        self: "IHyperdriveOutputLimitContractError",
         data: HexBytes,
         # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
-            [
-                item
-                for item in ierc4626hyperdrive_abi
-                if item.get("name") == "OutputLimit" and item.get("type") == "error"
-            ][0],
+            [item for item in ihyperdrive_abi if item.get("name") == "OutputLimit" and item.get("type") == "error"][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
     @classmethod
     def decode_error_data(  # type: ignore
-        cls: Type["IERC4626HyperdriveOutputLimitContractError"],
+        cls: Type["IHyperdriveOutputLimitContractError"],
         data: HexBytes,
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
-            [
-                item
-                for item in ierc4626hyperdrive_abi
-                if item.get("name") == "OutputLimit" and item.get("type") == "error"
-            ][0],
+            [item for item in ihyperdrive_abi if item.get("name") == "OutputLimit" and item.get("type") == "error"][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
 
-class IERC4626HyperdrivePoolAlreadyInitializedContractError:
+class IHyperdrivePoolAlreadyInitializedContractError:
     """ContractError for PoolAlreadyInitialized."""
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # 4 byte error selector
     selector: str
     # error signature, i.e. CustomError(uint256,bool)
     signature: str
 
     # pylint: disable=useless-parent-delegation
     def __init__(
-        self: "IERC4626HyperdrivePoolAlreadyInitializedContractError",
+        self: "IHyperdrivePoolAlreadyInitializedContractError",
     ) -> None:
         self.selector = "0x7983c051"
         self.signature = "PoolAlreadyInitialized()"
 
     def decode_error_data(  # type: ignore
-        self: "IERC4626HyperdrivePoolAlreadyInitializedContractError",
+        self: "IHyperdrivePoolAlreadyInitializedContractError",
         data: HexBytes,
         # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "PoolAlreadyInitialized" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
     @classmethod
     def decode_error_data(  # type: ignore
-        cls: Type["IERC4626HyperdrivePoolAlreadyInitializedContractError"],
+        cls: Type["IHyperdrivePoolAlreadyInitializedContractError"],
         data: HexBytes,
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "PoolAlreadyInitialized" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
 
-class IERC4626HyperdrivePoolIsPausedContractError:
+class IHyperdrivePoolIsPausedContractError:
     """ContractError for PoolIsPaused."""
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # 4 byte error selector
     selector: str
     # error signature, i.e. CustomError(uint256,bool)
     signature: str
 
     # pylint: disable=useless-parent-delegation
     def __init__(
-        self: "IERC4626HyperdrivePoolIsPausedContractError",
+        self: "IHyperdrivePoolIsPausedContractError",
     ) -> None:
         self.selector = "0x21081abf"
         self.signature = "PoolIsPaused()"
 
     def decode_error_data(  # type: ignore
-        self: "IERC4626HyperdrivePoolIsPausedContractError",
+        self: "IHyperdrivePoolIsPausedContractError",
         data: HexBytes,
         # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
-            [
-                item
-                for item in ierc4626hyperdrive_abi
-                if item.get("name") == "PoolIsPaused" and item.get("type") == "error"
-            ][0],
+            [item for item in ihyperdrive_abi if item.get("name") == "PoolIsPaused" and item.get("type") == "error"][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
     @classmethod
     def decode_error_data(  # type: ignore
-        cls: Type["IERC4626HyperdrivePoolIsPausedContractError"],
+        cls: Type["IHyperdrivePoolIsPausedContractError"],
         data: HexBytes,
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
-            [
-                item
-                for item in ierc4626hyperdrive_abi
-                if item.get("name") == "PoolIsPaused" and item.get("type") == "error"
-            ][0],
+            [item for item in ihyperdrive_abi if item.get("name") == "PoolIsPaused" and item.get("type") == "error"][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
 
-class IERC4626HyperdriveRestrictedZeroAddressContractError:
+class IHyperdriveRestrictedZeroAddressContractError:
     """ContractError for RestrictedZeroAddress."""
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # 4 byte error selector
     selector: str
     # error signature, i.e. CustomError(uint256,bool)
     signature: str
 
     # pylint: disable=useless-parent-delegation
     def __init__(
-        self: "IERC4626HyperdriveRestrictedZeroAddressContractError",
+        self: "IHyperdriveRestrictedZeroAddressContractError",
     ) -> None:
         self.selector = "0xf0dd15fd"
         self.signature = "RestrictedZeroAddress()"
 
     def decode_error_data(  # type: ignore
-        self: "IERC4626HyperdriveRestrictedZeroAddressContractError",
+        self: "IHyperdriveRestrictedZeroAddressContractError",
         data: HexBytes,
         # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "RestrictedZeroAddress" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
     @classmethod
     def decode_error_data(  # type: ignore
-        cls: Type["IERC4626HyperdriveRestrictedZeroAddressContractError"],
+        cls: Type["IHyperdriveRestrictedZeroAddressContractError"],
         data: HexBytes,
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "RestrictedZeroAddress" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
 
-class IERC4626HyperdriveReturnDataContractError:
+class IHyperdriveReturnDataContractError:
     """ContractError for ReturnData."""
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # 4 byte error selector
     selector: str
     # error signature, i.e. CustomError(uint256,bool)
     signature: str
 
     # pylint: disable=useless-parent-delegation
     def __init__(
-        self: "IERC4626HyperdriveReturnDataContractError",
+        self: "IHyperdriveReturnDataContractError",
     ) -> None:
         self.selector = "0xdcc81126"
         self.signature = "ReturnData(bytes)"
 
     def decode_error_data(  # type: ignore
-        self: "IERC4626HyperdriveReturnDataContractError",
+        self: "IHyperdriveReturnDataContractError",
         data: HexBytes,
         # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
-            [
-                item
-                for item in ierc4626hyperdrive_abi
-                if item.get("name") == "ReturnData" and item.get("type") == "error"
-            ][0],
+            [item for item in ihyperdrive_abi if item.get("name") == "ReturnData" and item.get("type") == "error"][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
     @classmethod
     def decode_error_data(  # type: ignore
-        cls: Type["IERC4626HyperdriveReturnDataContractError"],
+        cls: Type["IHyperdriveReturnDataContractError"],
         data: HexBytes,
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
-            [
-                item
-                for item in ierc4626hyperdrive_abi
-                if item.get("name") == "ReturnData" and item.get("type") == "error"
-            ][0],
+            [item for item in ihyperdrive_abi if item.get("name") == "ReturnData" and item.get("type") == "error"][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
 
-class IERC4626HyperdriveSweepFailedContractError:
+class IHyperdriveSweepFailedContractError:
     """ContractError for SweepFailed."""
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # 4 byte error selector
     selector: str
     # error signature, i.e. CustomError(uint256,bool)
     signature: str
 
     # pylint: disable=useless-parent-delegation
     def __init__(
-        self: "IERC4626HyperdriveSweepFailedContractError",
+        self: "IHyperdriveSweepFailedContractError",
     ) -> None:
         self.selector = "0x9eec2ff8"
         self.signature = "SweepFailed()"
 
     def decode_error_data(  # type: ignore
-        self: "IERC4626HyperdriveSweepFailedContractError",
+        self: "IHyperdriveSweepFailedContractError",
         data: HexBytes,
         # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
-            [
-                item
-                for item in ierc4626hyperdrive_abi
-                if item.get("name") == "SweepFailed" and item.get("type") == "error"
-            ][0],
+            [item for item in ihyperdrive_abi if item.get("name") == "SweepFailed" and item.get("type") == "error"][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
     @classmethod
     def decode_error_data(  # type: ignore
-        cls: Type["IERC4626HyperdriveSweepFailedContractError"],
+        cls: Type["IHyperdriveSweepFailedContractError"],
         data: HexBytes,
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
-            [
-                item
-                for item in ierc4626hyperdrive_abi
-                if item.get("name") == "SweepFailed" and item.get("type") == "error"
-            ][0],
+            [item for item in ihyperdrive_abi if item.get("name") == "SweepFailed" and item.get("type") == "error"][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
 
-class IERC4626HyperdriveTransferFailedContractError:
+class IHyperdriveTransferFailedContractError:
     """ContractError for TransferFailed."""
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # 4 byte error selector
     selector: str
     # error signature, i.e. CustomError(uint256,bool)
     signature: str
 
     # pylint: disable=useless-parent-delegation
     def __init__(
-        self: "IERC4626HyperdriveTransferFailedContractError",
+        self: "IHyperdriveTransferFailedContractError",
     ) -> None:
         self.selector = "0x90b8ec18"
         self.signature = "TransferFailed()"
 
     def decode_error_data(  # type: ignore
-        self: "IERC4626HyperdriveTransferFailedContractError",
+        self: "IHyperdriveTransferFailedContractError",
         data: HexBytes,
         # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
-            [
-                item
-                for item in ierc4626hyperdrive_abi
-                if item.get("name") == "TransferFailed" and item.get("type") == "error"
-            ][0],
+            [item for item in ihyperdrive_abi if item.get("name") == "TransferFailed" and item.get("type") == "error"][
+                0
+            ],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
     @classmethod
     def decode_error_data(  # type: ignore
-        cls: Type["IERC4626HyperdriveTransferFailedContractError"],
+        cls: Type["IHyperdriveTransferFailedContractError"],
         data: HexBytes,
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
-            [
-                item
-                for item in ierc4626hyperdrive_abi
-                if item.get("name") == "TransferFailed" and item.get("type") == "error"
-            ][0],
+            [item for item in ihyperdrive_abi if item.get("name") == "TransferFailed" and item.get("type") == "error"][
+                0
+            ],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
 
-class IERC4626HyperdriveUnauthorizedContractError:
+class IHyperdriveUnauthorizedContractError:
     """ContractError for Unauthorized."""
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # 4 byte error selector
     selector: str
     # error signature, i.e. CustomError(uint256,bool)
     signature: str
 
     # pylint: disable=useless-parent-delegation
     def __init__(
-        self: "IERC4626HyperdriveUnauthorizedContractError",
+        self: "IHyperdriveUnauthorizedContractError",
     ) -> None:
         self.selector = "0x82b42900"
         self.signature = "Unauthorized()"
 
     def decode_error_data(  # type: ignore
-        self: "IERC4626HyperdriveUnauthorizedContractError",
+        self: "IHyperdriveUnauthorizedContractError",
         data: HexBytes,
         # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
-            [
-                item
-                for item in ierc4626hyperdrive_abi
-                if item.get("name") == "Unauthorized" and item.get("type") == "error"
-            ][0],
+            [item for item in ihyperdrive_abi if item.get("name") == "Unauthorized" and item.get("type") == "error"][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
     @classmethod
     def decode_error_data(  # type: ignore
-        cls: Type["IERC4626HyperdriveUnauthorizedContractError"],
+        cls: Type["IHyperdriveUnauthorizedContractError"],
         data: HexBytes,
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
-            [
-                item
-                for item in ierc4626hyperdrive_abi
-                if item.get("name") == "Unauthorized" and item.get("type") == "error"
-            ][0],
+            [item for item in ihyperdrive_abi if item.get("name") == "Unauthorized" and item.get("type") == "error"][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
 
-class IERC4626HyperdriveUnexpectedSuccessContractError:
+class IHyperdriveUnexpectedSuccessContractError:
     """ContractError for UnexpectedSuccess."""
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # 4 byte error selector
     selector: str
     # error signature, i.e. CustomError(uint256,bool)
     signature: str
 
     # pylint: disable=useless-parent-delegation
     def __init__(
-        self: "IERC4626HyperdriveUnexpectedSuccessContractError",
+        self: "IHyperdriveUnexpectedSuccessContractError",
     ) -> None:
         self.selector = "0x8bb0a34b"
         self.signature = "UnexpectedSuccess()"
 
     def decode_error_data(  # type: ignore
-        self: "IERC4626HyperdriveUnexpectedSuccessContractError",
+        self: "IHyperdriveUnexpectedSuccessContractError",
         data: HexBytes,
         # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "UnexpectedSuccess" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
     @classmethod
     def decode_error_data(  # type: ignore
-        cls: Type["IERC4626HyperdriveUnexpectedSuccessContractError"],
+        cls: Type["IHyperdriveUnexpectedSuccessContractError"],
         data: HexBytes,
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "UnexpectedSuccess" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
 
-class IERC4626HyperdriveUnsafeCastToInt128ContractError:
+class IHyperdriveUnsafeCastToInt128ContractError:
     """ContractError for UnsafeCastToInt128."""
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # 4 byte error selector
     selector: str
     # error signature, i.e. CustomError(uint256,bool)
     signature: str
 
     # pylint: disable=useless-parent-delegation
     def __init__(
-        self: "IERC4626HyperdriveUnsafeCastToInt128ContractError",
+        self: "IHyperdriveUnsafeCastToInt128ContractError",
     ) -> None:
         self.selector = "0xa5353be5"
         self.signature = "UnsafeCastToInt128()"
 
     def decode_error_data(  # type: ignore
-        self: "IERC4626HyperdriveUnsafeCastToInt128ContractError",
+        self: "IHyperdriveUnsafeCastToInt128ContractError",
         data: HexBytes,
         # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "UnsafeCastToInt128" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
     @classmethod
     def decode_error_data(  # type: ignore
-        cls: Type["IERC4626HyperdriveUnsafeCastToInt128ContractError"],
+        cls: Type["IHyperdriveUnsafeCastToInt128ContractError"],
         data: HexBytes,
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "UnsafeCastToInt128" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
 
-class IERC4626HyperdriveUnsafeCastToInt256ContractError:
+class IHyperdriveUnsafeCastToInt256ContractError:
     """ContractError for UnsafeCastToInt256."""
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # 4 byte error selector
     selector: str
     # error signature, i.e. CustomError(uint256,bool)
     signature: str
 
     # pylint: disable=useless-parent-delegation
     def __init__(
-        self: "IERC4626HyperdriveUnsafeCastToInt256ContractError",
+        self: "IHyperdriveUnsafeCastToInt256ContractError",
     ) -> None:
         self.selector = "0x72dd4e02"
         self.signature = "UnsafeCastToInt256()"
 
     def decode_error_data(  # type: ignore
-        self: "IERC4626HyperdriveUnsafeCastToInt256ContractError",
+        self: "IHyperdriveUnsafeCastToInt256ContractError",
         data: HexBytes,
         # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "UnsafeCastToInt256" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
     @classmethod
     def decode_error_data(  # type: ignore
-        cls: Type["IERC4626HyperdriveUnsafeCastToInt256ContractError"],
+        cls: Type["IHyperdriveUnsafeCastToInt256ContractError"],
         data: HexBytes,
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "UnsafeCastToInt256" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
 
-class IERC4626HyperdriveUnsafeCastToUint112ContractError:
+class IHyperdriveUnsafeCastToUint112ContractError:
     """ContractError for UnsafeCastToUint112."""
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # 4 byte error selector
     selector: str
     # error signature, i.e. CustomError(uint256,bool)
     signature: str
 
     # pylint: disable=useless-parent-delegation
     def __init__(
-        self: "IERC4626HyperdriveUnsafeCastToUint112ContractError",
+        self: "IHyperdriveUnsafeCastToUint112ContractError",
     ) -> None:
         self.selector = "0x10d62a2e"
         self.signature = "UnsafeCastToUint112()"
 
     def decode_error_data(  # type: ignore
-        self: "IERC4626HyperdriveUnsafeCastToUint112ContractError",
+        self: "IHyperdriveUnsafeCastToUint112ContractError",
         data: HexBytes,
         # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "UnsafeCastToUint112" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
     @classmethod
     def decode_error_data(  # type: ignore
-        cls: Type["IERC4626HyperdriveUnsafeCastToUint112ContractError"],
+        cls: Type["IHyperdriveUnsafeCastToUint112ContractError"],
         data: HexBytes,
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "UnsafeCastToUint112" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
 
-class IERC4626HyperdriveUnsafeCastToUint128ContractError:
+class IHyperdriveUnsafeCastToUint128ContractError:
     """ContractError for UnsafeCastToUint128."""
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # 4 byte error selector
     selector: str
     # error signature, i.e. CustomError(uint256,bool)
     signature: str
 
     # pylint: disable=useless-parent-delegation
     def __init__(
-        self: "IERC4626HyperdriveUnsafeCastToUint128ContractError",
+        self: "IHyperdriveUnsafeCastToUint128ContractError",
     ) -> None:
         self.selector = "0x1e15f2a2"
         self.signature = "UnsafeCastToUint128()"
 
     def decode_error_data(  # type: ignore
-        self: "IERC4626HyperdriveUnsafeCastToUint128ContractError",
+        self: "IHyperdriveUnsafeCastToUint128ContractError",
         data: HexBytes,
         # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "UnsafeCastToUint128" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
     @classmethod
     def decode_error_data(  # type: ignore
-        cls: Type["IERC4626HyperdriveUnsafeCastToUint128ContractError"],
+        cls: Type["IHyperdriveUnsafeCastToUint128ContractError"],
         data: HexBytes,
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "UnsafeCastToUint128" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
 
-class IERC4626HyperdriveUnsupportedTokenContractError:
+class IHyperdriveUnsupportedTokenContractError:
     """ContractError for UnsupportedToken."""
 
     # @combomethod destroys return types, so we are redefining functions as both class and instance
     # pylint: disable=function-redefined
 
     # 4 byte error selector
     selector: str
     # error signature, i.e. CustomError(uint256,bool)
     signature: str
 
     # pylint: disable=useless-parent-delegation
     def __init__(
-        self: "IERC4626HyperdriveUnsupportedTokenContractError",
+        self: "IHyperdriveUnsupportedTokenContractError",
     ) -> None:
         self.selector = "0x6a172882"
         self.signature = "UnsupportedToken()"
 
     def decode_error_data(  # type: ignore
-        self: "IERC4626HyperdriveUnsupportedTokenContractError",
+        self: "IHyperdriveUnsupportedTokenContractError",
         data: HexBytes,
         # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "UnsupportedToken" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
     @classmethod
     def decode_error_data(  # type: ignore
-        cls: Type["IERC4626HyperdriveUnsupportedTokenContractError"],
+        cls: Type["IHyperdriveUnsupportedTokenContractError"],
         data: HexBytes,
     ) -> tuple[Any, ...]:
         """Decodes error data returns from a smart contract."""
         error_abi = cast(
             ABIFunction,
             [
                 item
-                for item in ierc4626hyperdrive_abi
+                for item in ihyperdrive_abi
                 if item.get("name") == "UnsupportedToken" and item.get("type") == "error"
             ][0],
         )
         types = get_abi_input_types(error_abi)
         abi_codec = ABICodec(default_registry)
         decoded = abi_codec.decode(types, data)
         return decoded
 
 
-class IERC4626HyperdriveContractErrors:
-    """ContractErrors for the IERC4626Hyperdrive contract."""
+class IHyperdriveUpdateLiquidityFailedContractError:
+    """ContractError for UpdateLiquidityFailed."""
+
+    # @combomethod destroys return types, so we are redefining functions as both class and instance
+    # pylint: disable=function-redefined
+
+    # 4 byte error selector
+    selector: str
+    # error signature, i.e. CustomError(uint256,bool)
+    signature: str
+
+    # pylint: disable=useless-parent-delegation
+    def __init__(
+        self: "IHyperdriveUpdateLiquidityFailedContractError",
+    ) -> None:
+        self.selector = "0x5044b7f5"
+        self.signature = "UpdateLiquidityFailed()"
+
+    def decode_error_data(  # type: ignore
+        self: "IHyperdriveUpdateLiquidityFailedContractError",
+        data: HexBytes,
+        # TODO: instead of returning a tuple, return a dataclass with the input names and types just like we do for functions
+    ) -> tuple[Any, ...]:
+        """Decodes error data returns from a smart contract."""
+        error_abi = cast(
+            ABIFunction,
+            [
+                item
+                for item in ihyperdrive_abi
+                if item.get("name") == "UpdateLiquidityFailed" and item.get("type") == "error"
+            ][0],
+        )
+        types = get_abi_input_types(error_abi)
+        abi_codec = ABICodec(default_registry)
+        decoded = abi_codec.decode(types, data)
+        return decoded
+
+    @classmethod
+    def decode_error_data(  # type: ignore
+        cls: Type["IHyperdriveUpdateLiquidityFailedContractError"],
+        data: HexBytes,
+    ) -> tuple[Any, ...]:
+        """Decodes error data returns from a smart contract."""
+        error_abi = cast(
+            ABIFunction,
+            [
+                item
+                for item in ihyperdrive_abi
+                if item.get("name") == "UpdateLiquidityFailed" and item.get("type") == "error"
+            ][0],
+        )
+        types = get_abi_input_types(error_abi)
+        abi_codec = ABICodec(default_registry)
+        decoded = abi_codec.decode(types, data)
+        return decoded
+
 
-    BatchInputLengthMismatch: IERC4626HyperdriveBatchInputLengthMismatchContractError
+class IHyperdriveContractErrors:
+    """ContractErrors for the IHyperdrive contract."""
 
-    BelowMinimumContribution: IERC4626HyperdriveBelowMinimumContributionContractError
+    BatchInputLengthMismatch: IHyperdriveBatchInputLengthMismatchContractError
 
-    DecreasedPresentValueWhenAddingLiquidity: IERC4626HyperdriveDecreasedPresentValueWhenAddingLiquidityContractError
+    BelowMinimumContribution: IHyperdriveBelowMinimumContributionContractError
 
-    DistributeExcessIdleFailed: IERC4626HyperdriveDistributeExcessIdleFailedContractError
+    DecreasedPresentValueWhenAddingLiquidity: IHyperdriveDecreasedPresentValueWhenAddingLiquidityContractError
 
-    ExpInvalidExponent: IERC4626HyperdriveExpInvalidExponentContractError
+    DistributeExcessIdleFailed: IHyperdriveDistributeExcessIdleFailedContractError
 
-    ExpiredDeadline: IERC4626HyperdriveExpiredDeadlineContractError
+    ExpInvalidExponent: IHyperdriveExpInvalidExponentContractError
 
-    InsufficientBalance: IERC4626HyperdriveInsufficientBalanceContractError
+    ExpiredDeadline: IHyperdriveExpiredDeadlineContractError
 
-    InsufficientLiquidity: IERC4626HyperdriveInsufficientLiquidityContractError
+    InsufficientBalance: IHyperdriveInsufficientBalanceContractError
 
-    InvalidApr: IERC4626HyperdriveInvalidAprContractError
+    InsufficientLiquidity: IHyperdriveInsufficientLiquidityContractError
 
-    InvalidBaseToken: IERC4626HyperdriveInvalidBaseTokenContractError
+    InvalidApr: IHyperdriveInvalidAprContractError
 
-    InvalidCheckpointTime: IERC4626HyperdriveInvalidCheckpointTimeContractError
+    InvalidCheckpointTime: IHyperdriveInvalidCheckpointTimeContractError
 
-    InvalidERC20Bridge: IERC4626HyperdriveInvalidERC20BridgeContractError
+    InvalidERC20Bridge: IHyperdriveInvalidERC20BridgeContractError
 
-    InvalidFeeDestination: IERC4626HyperdriveInvalidFeeDestinationContractError
+    InvalidFeeDestination: IHyperdriveInvalidFeeDestinationContractError
 
-    InvalidInitialVaultSharePrice: IERC4626HyperdriveInvalidInitialVaultSharePriceContractError
+    InvalidInitialVaultSharePrice: IHyperdriveInvalidInitialVaultSharePriceContractError
 
-    InvalidLPSharePrice: IERC4626HyperdriveInvalidLPSharePriceContractError
+    InvalidLPSharePrice: IHyperdriveInvalidLPSharePriceContractError
 
-    InvalidPresentValue: IERC4626HyperdriveInvalidPresentValueContractError
+    InvalidPresentValue: IHyperdriveInvalidPresentValueContractError
 
-    InvalidShareReserves: IERC4626HyperdriveInvalidShareReservesContractError
+    InvalidSignature: IHyperdriveInvalidSignatureContractError
 
-    InvalidSignature: IERC4626HyperdriveInvalidSignatureContractError
+    InvalidTimestamp: IHyperdriveInvalidTimestampContractError
 
-    InvalidTimestamp: IERC4626HyperdriveInvalidTimestampContractError
+    LnInvalidInput: IHyperdriveLnInvalidInputContractError
 
-    LnInvalidInput: IERC4626HyperdriveLnInvalidInputContractError
+    MinimumSharePrice: IHyperdriveMinimumSharePriceContractError
 
-    MinimumSharePrice: IERC4626HyperdriveMinimumSharePriceContractError
+    MinimumTransactionAmount: IHyperdriveMinimumTransactionAmountContractError
 
-    MinimumTransactionAmount: IERC4626HyperdriveMinimumTransactionAmountContractError
+    NotPayable: IHyperdriveNotPayableContractError
 
-    NotPayable: IERC4626HyperdriveNotPayableContractError
+    OutputLimit: IHyperdriveOutputLimitContractError
 
-    OutputLimit: IERC4626HyperdriveOutputLimitContractError
+    PoolAlreadyInitialized: IHyperdrivePoolAlreadyInitializedContractError
 
-    PoolAlreadyInitialized: IERC4626HyperdrivePoolAlreadyInitializedContractError
+    PoolIsPaused: IHyperdrivePoolIsPausedContractError
 
-    PoolIsPaused: IERC4626HyperdrivePoolIsPausedContractError
+    RestrictedZeroAddress: IHyperdriveRestrictedZeroAddressContractError
 
-    RestrictedZeroAddress: IERC4626HyperdriveRestrictedZeroAddressContractError
+    ReturnData: IHyperdriveReturnDataContractError
 
-    ReturnData: IERC4626HyperdriveReturnDataContractError
+    SweepFailed: IHyperdriveSweepFailedContractError
 
-    SweepFailed: IERC4626HyperdriveSweepFailedContractError
+    TransferFailed: IHyperdriveTransferFailedContractError
 
-    TransferFailed: IERC4626HyperdriveTransferFailedContractError
+    Unauthorized: IHyperdriveUnauthorizedContractError
 
-    Unauthorized: IERC4626HyperdriveUnauthorizedContractError
+    UnexpectedSuccess: IHyperdriveUnexpectedSuccessContractError
 
-    UnexpectedSuccess: IERC4626HyperdriveUnexpectedSuccessContractError
+    UnsafeCastToInt128: IHyperdriveUnsafeCastToInt128ContractError
 
-    UnsafeCastToInt128: IERC4626HyperdriveUnsafeCastToInt128ContractError
+    UnsafeCastToInt256: IHyperdriveUnsafeCastToInt256ContractError
 
-    UnsafeCastToInt256: IERC4626HyperdriveUnsafeCastToInt256ContractError
+    UnsafeCastToUint112: IHyperdriveUnsafeCastToUint112ContractError
 
-    UnsafeCastToUint112: IERC4626HyperdriveUnsafeCastToUint112ContractError
+    UnsafeCastToUint128: IHyperdriveUnsafeCastToUint128ContractError
 
-    UnsafeCastToUint128: IERC4626HyperdriveUnsafeCastToUint128ContractError
+    UnsupportedToken: IHyperdriveUnsupportedTokenContractError
 
-    UnsupportedToken: IERC4626HyperdriveUnsupportedTokenContractError
+    UpdateLiquidityFailed: IHyperdriveUpdateLiquidityFailedContractError
 
     def __init__(
         self,
     ) -> None:
-        self.BatchInputLengthMismatch = IERC4626HyperdriveBatchInputLengthMismatchContractError()
-        self.BelowMinimumContribution = IERC4626HyperdriveBelowMinimumContributionContractError()
+        self.BatchInputLengthMismatch = IHyperdriveBatchInputLengthMismatchContractError()
+        self.BelowMinimumContribution = IHyperdriveBelowMinimumContributionContractError()
         self.DecreasedPresentValueWhenAddingLiquidity = (
-            IERC4626HyperdriveDecreasedPresentValueWhenAddingLiquidityContractError()
+            IHyperdriveDecreasedPresentValueWhenAddingLiquidityContractError()
         )
-        self.DistributeExcessIdleFailed = IERC4626HyperdriveDistributeExcessIdleFailedContractError()
-        self.ExpInvalidExponent = IERC4626HyperdriveExpInvalidExponentContractError()
-        self.ExpiredDeadline = IERC4626HyperdriveExpiredDeadlineContractError()
-        self.InsufficientBalance = IERC4626HyperdriveInsufficientBalanceContractError()
-        self.InsufficientLiquidity = IERC4626HyperdriveInsufficientLiquidityContractError()
-        self.InvalidApr = IERC4626HyperdriveInvalidAprContractError()
-        self.InvalidBaseToken = IERC4626HyperdriveInvalidBaseTokenContractError()
-        self.InvalidCheckpointTime = IERC4626HyperdriveInvalidCheckpointTimeContractError()
-        self.InvalidERC20Bridge = IERC4626HyperdriveInvalidERC20BridgeContractError()
-        self.InvalidFeeDestination = IERC4626HyperdriveInvalidFeeDestinationContractError()
-        self.InvalidInitialVaultSharePrice = IERC4626HyperdriveInvalidInitialVaultSharePriceContractError()
-        self.InvalidLPSharePrice = IERC4626HyperdriveInvalidLPSharePriceContractError()
-        self.InvalidPresentValue = IERC4626HyperdriveInvalidPresentValueContractError()
-        self.InvalidShareReserves = IERC4626HyperdriveInvalidShareReservesContractError()
-        self.InvalidSignature = IERC4626HyperdriveInvalidSignatureContractError()
-        self.InvalidTimestamp = IERC4626HyperdriveInvalidTimestampContractError()
-        self.LnInvalidInput = IERC4626HyperdriveLnInvalidInputContractError()
-        self.MinimumSharePrice = IERC4626HyperdriveMinimumSharePriceContractError()
-        self.MinimumTransactionAmount = IERC4626HyperdriveMinimumTransactionAmountContractError()
-        self.NotPayable = IERC4626HyperdriveNotPayableContractError()
-        self.OutputLimit = IERC4626HyperdriveOutputLimitContractError()
-        self.PoolAlreadyInitialized = IERC4626HyperdrivePoolAlreadyInitializedContractError()
-        self.PoolIsPaused = IERC4626HyperdrivePoolIsPausedContractError()
-        self.RestrictedZeroAddress = IERC4626HyperdriveRestrictedZeroAddressContractError()
-        self.ReturnData = IERC4626HyperdriveReturnDataContractError()
-        self.SweepFailed = IERC4626HyperdriveSweepFailedContractError()
-        self.TransferFailed = IERC4626HyperdriveTransferFailedContractError()
-        self.Unauthorized = IERC4626HyperdriveUnauthorizedContractError()
-        self.UnexpectedSuccess = IERC4626HyperdriveUnexpectedSuccessContractError()
-        self.UnsafeCastToInt128 = IERC4626HyperdriveUnsafeCastToInt128ContractError()
-        self.UnsafeCastToInt256 = IERC4626HyperdriveUnsafeCastToInt256ContractError()
-        self.UnsafeCastToUint112 = IERC4626HyperdriveUnsafeCastToUint112ContractError()
-        self.UnsafeCastToUint128 = IERC4626HyperdriveUnsafeCastToUint128ContractError()
-        self.UnsupportedToken = IERC4626HyperdriveUnsupportedTokenContractError()
+        self.DistributeExcessIdleFailed = IHyperdriveDistributeExcessIdleFailedContractError()
+        self.ExpInvalidExponent = IHyperdriveExpInvalidExponentContractError()
+        self.ExpiredDeadline = IHyperdriveExpiredDeadlineContractError()
+        self.InsufficientBalance = IHyperdriveInsufficientBalanceContractError()
+        self.InsufficientLiquidity = IHyperdriveInsufficientLiquidityContractError()
+        self.InvalidApr = IHyperdriveInvalidAprContractError()
+        self.InvalidCheckpointTime = IHyperdriveInvalidCheckpointTimeContractError()
+        self.InvalidERC20Bridge = IHyperdriveInvalidERC20BridgeContractError()
+        self.InvalidFeeDestination = IHyperdriveInvalidFeeDestinationContractError()
+        self.InvalidInitialVaultSharePrice = IHyperdriveInvalidInitialVaultSharePriceContractError()
+        self.InvalidLPSharePrice = IHyperdriveInvalidLPSharePriceContractError()
+        self.InvalidPresentValue = IHyperdriveInvalidPresentValueContractError()
+        self.InvalidSignature = IHyperdriveInvalidSignatureContractError()
+        self.InvalidTimestamp = IHyperdriveInvalidTimestampContractError()
+        self.LnInvalidInput = IHyperdriveLnInvalidInputContractError()
+        self.MinimumSharePrice = IHyperdriveMinimumSharePriceContractError()
+        self.MinimumTransactionAmount = IHyperdriveMinimumTransactionAmountContractError()
+        self.NotPayable = IHyperdriveNotPayableContractError()
+        self.OutputLimit = IHyperdriveOutputLimitContractError()
+        self.PoolAlreadyInitialized = IHyperdrivePoolAlreadyInitializedContractError()
+        self.PoolIsPaused = IHyperdrivePoolIsPausedContractError()
+        self.RestrictedZeroAddress = IHyperdriveRestrictedZeroAddressContractError()
+        self.ReturnData = IHyperdriveReturnDataContractError()
+        self.SweepFailed = IHyperdriveSweepFailedContractError()
+        self.TransferFailed = IHyperdriveTransferFailedContractError()
+        self.Unauthorized = IHyperdriveUnauthorizedContractError()
+        self.UnexpectedSuccess = IHyperdriveUnexpectedSuccessContractError()
+        self.UnsafeCastToInt128 = IHyperdriveUnsafeCastToInt128ContractError()
+        self.UnsafeCastToInt256 = IHyperdriveUnsafeCastToInt256ContractError()
+        self.UnsafeCastToUint112 = IHyperdriveUnsafeCastToUint112ContractError()
+        self.UnsafeCastToUint128 = IHyperdriveUnsafeCastToUint128ContractError()
+        self.UnsupportedToken = IHyperdriveUnsupportedTokenContractError()
+        self.UpdateLiquidityFailed = IHyperdriveUpdateLiquidityFailedContractError()
 
         self._all = [
             self.BatchInputLengthMismatch,
             self.BelowMinimumContribution,
             self.DecreasedPresentValueWhenAddingLiquidity,
             self.DistributeExcessIdleFailed,
             self.ExpInvalidExponent,
             self.ExpiredDeadline,
             self.InsufficientBalance,
             self.InsufficientLiquidity,
             self.InvalidApr,
-            self.InvalidBaseToken,
             self.InvalidCheckpointTime,
             self.InvalidERC20Bridge,
             self.InvalidFeeDestination,
             self.InvalidInitialVaultSharePrice,
             self.InvalidLPSharePrice,
             self.InvalidPresentValue,
-            self.InvalidShareReserves,
             self.InvalidSignature,
             self.InvalidTimestamp,
             self.LnInvalidInput,
             self.MinimumSharePrice,
             self.MinimumTransactionAmount,
             self.NotPayable,
             self.OutputLimit,
@@ -5449,27 +5635,28 @@
             self.Unauthorized,
             self.UnexpectedSuccess,
             self.UnsafeCastToInt128,
             self.UnsafeCastToInt256,
             self.UnsafeCastToUint112,
             self.UnsafeCastToUint128,
             self.UnsupportedToken,
+            self.UpdateLiquidityFailed,
         ]
 
     def decode_custom_error(self, data: str) -> tuple[Any, ...]:
         """Decodes a custom contract error."""
         selector = data[:10]
         for err in self._all:
             if err.selector == selector:
                 return err.decode_error_data(HexBytes(data[10:]))
 
-        raise ValueError(f"IERC4626Hyperdrive does not have a selector matching {selector}")
+        raise ValueError(f"IHyperdrive does not have a selector matching {selector}")
 
 
-ierc4626hyperdrive_abi: ABI = cast(
+ihyperdrive_abi: ABI = cast(
     ABI,
     [
         {
             "type": "function",
             "name": "PERMIT_TYPEHASH",
             "inputs": [],
             "outputs": [{"name": "", "type": "bytes32", "internalType": "bytes32"}],
@@ -5490,15 +5677,15 @@
                     "components": [
                         {"name": "destination", "type": "address", "internalType": "address"},
                         {"name": "asBase", "type": "bool", "internalType": "bool"},
                         {"name": "extraData", "type": "bytes", "internalType": "bytes"},
                     ],
                 },
             ],
-            "outputs": [{"name": "", "type": "uint256", "internalType": "uint256"}],
+            "outputs": [{"name": "lpShares", "type": "uint256", "internalType": "uint256"}],
             "stateMutability": "payable",
         },
         {
             "type": "function",
             "name": "balanceOf",
             "inputs": [
                 {"name": "tokenId", "type": "uint256", "internalType": "uint256"},
@@ -5525,15 +5712,18 @@
             ],
             "outputs": [],
             "stateMutability": "nonpayable",
         },
         {
             "type": "function",
             "name": "checkpoint",
-            "inputs": [{"name": "_checkpointTime", "type": "uint256", "internalType": "uint256"}],
+            "inputs": [
+                {"name": "_checkpointTime", "type": "uint256", "internalType": "uint256"},
+                {"name": "_maxIterations", "type": "uint256", "internalType": "uint256"},
+            ],
             "outputs": [],
             "stateMutability": "nonpayable",
         },
         {
             "type": "function",
             "name": "closeLong",
             "inputs": [
@@ -5547,15 +5737,15 @@
                     "components": [
                         {"name": "destination", "type": "address", "internalType": "address"},
                         {"name": "asBase", "type": "bool", "internalType": "bool"},
                         {"name": "extraData", "type": "bytes", "internalType": "bytes"},
                     ],
                 },
             ],
-            "outputs": [{"name": "", "type": "uint256", "internalType": "uint256"}],
+            "outputs": [{"name": "proceeds", "type": "uint256", "internalType": "uint256"}],
             "stateMutability": "nonpayable",
         },
         {
             "type": "function",
             "name": "closeShort",
             "inputs": [
                 {"name": "_maturityTime", "type": "uint256", "internalType": "uint256"},
@@ -5568,15 +5758,15 @@
                     "components": [
                         {"name": "destination", "type": "address", "internalType": "address"},
                         {"name": "asBase", "type": "bool", "internalType": "bool"},
                         {"name": "extraData", "type": "bytes", "internalType": "bytes"},
                     ],
                 },
             ],
-            "outputs": [{"name": "", "type": "uint256", "internalType": "uint256"}],
+            "outputs": [{"name": "proceeds", "type": "uint256", "internalType": "uint256"}],
             "stateMutability": "nonpayable",
         },
         {
             "type": "function",
             "name": "collectGovernanceFee",
             "inputs": [
                 {
@@ -5662,24 +5852,26 @@
             "outputs": [
                 {
                     "name": "",
                     "type": "tuple",
                     "internalType": "struct IHyperdrive.PoolConfig",
                     "components": [
                         {"name": "baseToken", "type": "address", "internalType": "contract IERC20"},
+                        {"name": "vaultSharesToken", "type": "address", "internalType": "contract IERC20"},
                         {"name": "linkerFactory", "type": "address", "internalType": "address"},
                         {"name": "linkerCodeHash", "type": "bytes32", "internalType": "bytes32"},
                         {"name": "initialVaultSharePrice", "type": "uint256", "internalType": "uint256"},
                         {"name": "minimumShareReserves", "type": "uint256", "internalType": "uint256"},
                         {"name": "minimumTransactionAmount", "type": "uint256", "internalType": "uint256"},
                         {"name": "positionDuration", "type": "uint256", "internalType": "uint256"},
                         {"name": "checkpointDuration", "type": "uint256", "internalType": "uint256"},
                         {"name": "timeStretch", "type": "uint256", "internalType": "uint256"},
                         {"name": "governance", "type": "address", "internalType": "address"},
                         {"name": "feeCollector", "type": "address", "internalType": "address"},
+                        {"name": "sweepCollector", "type": "address", "internalType": "address"},
                         {
                             "name": "fees",
                             "type": "tuple",
                             "internalType": "struct IHyperdrive.Fees",
                             "components": [
                                 {"name": "curve", "type": "uint256", "internalType": "uint256"},
                                 {"name": "flat", "type": "uint256", "internalType": "uint256"},
@@ -5759,15 +5951,15 @@
                     "components": [
                         {"name": "destination", "type": "address", "internalType": "address"},
                         {"name": "asBase", "type": "bool", "internalType": "bool"},
                         {"name": "extraData", "type": "bytes", "internalType": "bytes"},
                     ],
                 },
             ],
-            "outputs": [{"name": "", "type": "uint256", "internalType": "uint256"}],
+            "outputs": [{"name": "lpShares", "type": "uint256", "internalType": "uint256"}],
             "stateMutability": "payable",
         },
         {
             "type": "function",
             "name": "isApprovedForAll",
             "inputs": [
                 {"name": "owner", "type": "address", "internalType": "address"},
@@ -5819,16 +6011,16 @@
                         {"name": "destination", "type": "address", "internalType": "address"},
                         {"name": "asBase", "type": "bool", "internalType": "bool"},
                         {"name": "extraData", "type": "bytes", "internalType": "bytes"},
                     ],
                 },
             ],
             "outputs": [
-                {"name": "", "type": "uint256", "internalType": "uint256"},
-                {"name": "", "type": "uint256", "internalType": "uint256"},
+                {"name": "maturityTime", "type": "uint256", "internalType": "uint256"},
+                {"name": "bondProceeds", "type": "uint256", "internalType": "uint256"},
             ],
             "stateMutability": "payable",
         },
         {
             "type": "function",
             "name": "openShort",
             "inputs": [
@@ -5843,16 +6035,16 @@
                         {"name": "destination", "type": "address", "internalType": "address"},
                         {"name": "asBase", "type": "bool", "internalType": "bool"},
                         {"name": "extraData", "type": "bytes", "internalType": "bytes"},
                     ],
                 },
             ],
             "outputs": [
-                {"name": "", "type": "uint256", "internalType": "uint256"},
-                {"name": "", "type": "uint256", "internalType": "uint256"},
+                {"name": "maturityTime", "type": "uint256", "internalType": "uint256"},
+                {"name": "deposit", "type": "uint256", "internalType": "uint256"},
             ],
             "stateMutability": "payable",
         },
         {
             "type": "function",
             "name": "pause",
             "inputs": [{"name": "_status", "type": "bool", "internalType": "bool"}],
@@ -5899,16 +6091,16 @@
                         {"name": "destination", "type": "address", "internalType": "address"},
                         {"name": "asBase", "type": "bool", "internalType": "bool"},
                         {"name": "extraData", "type": "bytes", "internalType": "bytes"},
                     ],
                 },
             ],
             "outputs": [
-                {"name": "", "type": "uint256", "internalType": "uint256"},
-                {"name": "", "type": "uint256", "internalType": "uint256"},
+                {"name": "proceeds", "type": "uint256", "internalType": "uint256"},
+                {"name": "withdrawalSharesRedeemed", "type": "uint256", "internalType": "uint256"},
             ],
             "stateMutability": "nonpayable",
         },
         {
             "type": "function",
             "name": "removeLiquidity",
             "inputs": [
@@ -5922,16 +6114,16 @@
                         {"name": "destination", "type": "address", "internalType": "address"},
                         {"name": "asBase", "type": "bool", "internalType": "bool"},
                         {"name": "extraData", "type": "bytes", "internalType": "bytes"},
                     ],
                 },
             ],
             "outputs": [
-                {"name": "", "type": "uint256", "internalType": "uint256"},
-                {"name": "", "type": "uint256", "internalType": "uint256"},
+                {"name": "proceeds", "type": "uint256", "internalType": "uint256"},
+                {"name": "withdrawalShares", "type": "uint256", "internalType": "uint256"},
             ],
             "stateMutability": "nonpayable",
         },
         {
             "type": "function",
             "name": "setApproval",
             "inputs": [
@@ -5962,14 +6154,21 @@
                 {"name": "approved", "type": "bool", "internalType": "bool"},
             ],
             "outputs": [],
             "stateMutability": "nonpayable",
         },
         {
             "type": "function",
+            "name": "setFeeCollector",
+            "inputs": [{"name": "_who", "type": "address", "internalType": "address"}],
+            "outputs": [],
+            "stateMutability": "nonpayable",
+        },
+        {
+            "type": "function",
             "name": "setGovernance",
             "inputs": [{"name": "_who", "type": "address", "internalType": "address"}],
             "outputs": [],
             "stateMutability": "nonpayable",
         },
         {
             "type": "function",
@@ -5979,14 +6178,21 @@
                 {"name": "status", "type": "bool", "internalType": "bool"},
             ],
             "outputs": [],
             "stateMutability": "nonpayable",
         },
         {
             "type": "function",
+            "name": "setSweepCollector",
+            "inputs": [{"name": "_who", "type": "address", "internalType": "address"}],
+            "outputs": [],
+            "stateMutability": "nonpayable",
+        },
+        {
+            "type": "function",
             "name": "sweep",
             "inputs": [{"name": "_target", "type": "address", "internalType": "contract IERC20"}],
             "outputs": [],
             "stateMutability": "nonpayable",
         },
         {
             "type": "function",
@@ -6060,17 +6266,17 @@
                 {"name": "caller", "type": "address", "internalType": "address"},
             ],
             "outputs": [],
             "stateMutability": "nonpayable",
         },
         {
             "type": "function",
-            "name": "vault",
+            "name": "vaultSharesToken",
             "inputs": [],
-            "outputs": [{"name": "", "type": "address", "internalType": "contract IERC4626"}],
+            "outputs": [{"name": "", "type": "address", "internalType": "address"}],
             "stateMutability": "view",
         },
         {
             "type": "event",
             "name": "AddLiquidity",
             "inputs": [
                 {"name": "provider", "type": "address", "indexed": True, "internalType": "address"},
@@ -6103,33 +6309,36 @@
             "anonymous": False,
         },
         {
             "type": "event",
             "name": "CloseLong",
             "inputs": [
                 {"name": "trader", "type": "address", "indexed": True, "internalType": "address"},
+                {"name": "destination", "type": "address", "indexed": True, "internalType": "address"},
                 {"name": "assetId", "type": "uint256", "indexed": True, "internalType": "uint256"},
                 {"name": "maturityTime", "type": "uint256", "indexed": False, "internalType": "uint256"},
                 {"name": "baseAmount", "type": "uint256", "indexed": False, "internalType": "uint256"},
                 {"name": "vaultShareAmount", "type": "uint256", "indexed": False, "internalType": "uint256"},
                 {"name": "asBase", "type": "bool", "indexed": False, "internalType": "bool"},
                 {"name": "bondAmount", "type": "uint256", "indexed": False, "internalType": "uint256"},
             ],
             "anonymous": False,
         },
         {
             "type": "event",
             "name": "CloseShort",
             "inputs": [
                 {"name": "trader", "type": "address", "indexed": True, "internalType": "address"},
+                {"name": "destination", "type": "address", "indexed": True, "internalType": "address"},
                 {"name": "assetId", "type": "uint256", "indexed": True, "internalType": "uint256"},
                 {"name": "maturityTime", "type": "uint256", "indexed": False, "internalType": "uint256"},
                 {"name": "baseAmount", "type": "uint256", "indexed": False, "internalType": "uint256"},
                 {"name": "vaultShareAmount", "type": "uint256", "indexed": False, "internalType": "uint256"},
                 {"name": "asBase", "type": "bool", "indexed": False, "internalType": "bool"},
+                {"name": "basePayment", "type": "uint256", "indexed": False, "internalType": "uint256"},
                 {"name": "bondAmount", "type": "uint256", "indexed": False, "internalType": "uint256"},
             ],
             "anonymous": False,
         },
         {
             "type": "event",
             "name": "CollectGovernanceFee",
@@ -6140,23 +6349,30 @@
             "anonymous": False,
         },
         {
             "type": "event",
             "name": "CreateCheckpoint",
             "inputs": [
                 {"name": "checkpointTime", "type": "uint256", "indexed": True, "internalType": "uint256"},
+                {"name": "checkpointVaultSharePrice", "type": "uint256", "indexed": False, "internalType": "uint256"},
                 {"name": "vaultSharePrice", "type": "uint256", "indexed": False, "internalType": "uint256"},
                 {"name": "maturedShorts", "type": "uint256", "indexed": False, "internalType": "uint256"},
                 {"name": "maturedLongs", "type": "uint256", "indexed": False, "internalType": "uint256"},
                 {"name": "lpSharePrice", "type": "uint256", "indexed": False, "internalType": "uint256"},
             ],
             "anonymous": False,
         },
         {
             "type": "event",
+            "name": "FeeCollectorUpdated",
+            "inputs": [{"name": "newFeeCollector", "type": "address", "indexed": True, "internalType": "address"}],
+            "anonymous": False,
+        },
+        {
+            "type": "event",
             "name": "GovernanceUpdated",
             "inputs": [{"name": "newGovernance", "type": "address", "indexed": True, "internalType": "address"}],
             "anonymous": False,
         },
         {
             "type": "event",
             "name": "Initialize",
@@ -6215,37 +6431,54 @@
             "anonymous": False,
         },
         {
             "type": "event",
             "name": "RedeemWithdrawalShares",
             "inputs": [
                 {"name": "provider", "type": "address", "indexed": True, "internalType": "address"},
+                {"name": "destination", "type": "address", "indexed": True, "internalType": "address"},
                 {"name": "withdrawalShareAmount", "type": "uint256", "indexed": False, "internalType": "uint256"},
                 {"name": "baseAmount", "type": "uint256", "indexed": False, "internalType": "uint256"},
                 {"name": "vaultShareAmount", "type": "uint256", "indexed": False, "internalType": "uint256"},
                 {"name": "asBase", "type": "bool", "indexed": False, "internalType": "bool"},
             ],
             "anonymous": False,
         },
         {
             "type": "event",
             "name": "RemoveLiquidity",
             "inputs": [
                 {"name": "provider", "type": "address", "indexed": True, "internalType": "address"},
+                {"name": "destination", "type": "address", "indexed": True, "internalType": "address"},
                 {"name": "lpAmount", "type": "uint256", "indexed": False, "internalType": "uint256"},
                 {"name": "baseAmount", "type": "uint256", "indexed": False, "internalType": "uint256"},
                 {"name": "vaultShareAmount", "type": "uint256", "indexed": False, "internalType": "uint256"},
                 {"name": "asBase", "type": "bool", "indexed": False, "internalType": "bool"},
                 {"name": "withdrawalShareAmount", "type": "uint256", "indexed": False, "internalType": "uint256"},
                 {"name": "lpSharePrice", "type": "uint256", "indexed": False, "internalType": "uint256"},
             ],
             "anonymous": False,
         },
         {
             "type": "event",
+            "name": "Sweep",
+            "inputs": [
+                {"name": "collector", "type": "address", "indexed": True, "internalType": "address"},
+                {"name": "target", "type": "address", "indexed": True, "internalType": "address"},
+            ],
+            "anonymous": False,
+        },
+        {
+            "type": "event",
+            "name": "SweepCollectorUpdated",
+            "inputs": [{"name": "newSweepCollector", "type": "address", "indexed": True, "internalType": "address"}],
+            "anonymous": False,
+        },
+        {
+            "type": "event",
             "name": "TransferSingle",
             "inputs": [
                 {"name": "operator", "type": "address", "indexed": True, "internalType": "address"},
                 {"name": "from", "type": "address", "indexed": True, "internalType": "address"},
                 {"name": "to", "type": "address", "indexed": True, "internalType": "address"},
                 {"name": "id", "type": "uint256", "indexed": False, "internalType": "uint256"},
                 {"name": "value", "type": "uint256", "indexed": False, "internalType": "uint256"},
@@ -6255,30 +6488,22 @@
         {"type": "error", "name": "BatchInputLengthMismatch", "inputs": []},
         {"type": "error", "name": "BelowMinimumContribution", "inputs": []},
         {"type": "error", "name": "DecreasedPresentValueWhenAddingLiquidity", "inputs": []},
         {"type": "error", "name": "DistributeExcessIdleFailed", "inputs": []},
         {"type": "error", "name": "ExpInvalidExponent", "inputs": []},
         {"type": "error", "name": "ExpiredDeadline", "inputs": []},
         {"type": "error", "name": "InsufficientBalance", "inputs": []},
-        {
-            "type": "error",
-            "name": "InsufficientLiquidity",
-            "inputs": [
-                {"name": "reason", "type": "uint8", "internalType": "enum IHyperdrive.InsufficientLiquidityReason"}
-            ],
-        },
+        {"type": "error", "name": "InsufficientLiquidity", "inputs": []},
         {"type": "error", "name": "InvalidApr", "inputs": []},
-        {"type": "error", "name": "InvalidBaseToken", "inputs": []},
         {"type": "error", "name": "InvalidCheckpointTime", "inputs": []},
         {"type": "error", "name": "InvalidERC20Bridge", "inputs": []},
         {"type": "error", "name": "InvalidFeeDestination", "inputs": []},
         {"type": "error", "name": "InvalidInitialVaultSharePrice", "inputs": []},
         {"type": "error", "name": "InvalidLPSharePrice", "inputs": []},
         {"type": "error", "name": "InvalidPresentValue", "inputs": []},
-        {"type": "error", "name": "InvalidShareReserves", "inputs": []},
         {"type": "error", "name": "InvalidSignature", "inputs": []},
         {"type": "error", "name": "InvalidTimestamp", "inputs": []},
         {"type": "error", "name": "LnInvalidInput", "inputs": []},
         {"type": "error", "name": "MinimumSharePrice", "inputs": []},
         {"type": "error", "name": "MinimumTransactionAmount", "inputs": []},
         {"type": "error", "name": "NotPayable", "inputs": []},
         {"type": "error", "name": "OutputLimit", "inputs": []},
@@ -6291,42 +6516,43 @@
         {"type": "error", "name": "Unauthorized", "inputs": []},
         {"type": "error", "name": "UnexpectedSuccess", "inputs": []},
         {"type": "error", "name": "UnsafeCastToInt128", "inputs": []},
         {"type": "error", "name": "UnsafeCastToInt256", "inputs": []},
         {"type": "error", "name": "UnsafeCastToUint112", "inputs": []},
         {"type": "error", "name": "UnsafeCastToUint128", "inputs": []},
         {"type": "error", "name": "UnsupportedToken", "inputs": []},
+        {"type": "error", "name": "UpdateLiquidityFailed", "inputs": []},
     ],
 )
 # pylint: disable=line-too-long
-ierc4626hyperdrive_bytecode = HexStr("0x")
+ihyperdrive_bytecode = HexStr("0x")
 
 
-class IERC4626HyperdriveContract(Contract):
-    """A web3.py Contract class for the IERC4626Hyperdrive contract."""
+class IHyperdriveContract(Contract):
+    """A web3.py Contract class for the IHyperdrive contract."""
 
-    abi: ABI = ierc4626hyperdrive_abi
-    bytecode: bytes = HexBytes(ierc4626hyperdrive_bytecode)
+    abi: ABI = ihyperdrive_abi
+    bytecode: bytes = HexBytes(ihyperdrive_bytecode)
 
     def __init__(self, address: ChecksumAddress | None = None) -> None:
         try:
             # Initialize parent Contract class
             super().__init__(address=address)
-            self.functions = IERC4626HyperdriveContractFunctions(ierc4626hyperdrive_abi, self.w3, address)  # type: ignore
-            self.events = IERC4626HyperdriveContractEvents(ierc4626hyperdrive_abi, self.w3, address)  # type: ignore
-            self.errors = IERC4626HyperdriveContractErrors()
+            self.functions = IHyperdriveContractFunctions(ihyperdrive_abi, self.w3, address)  # type: ignore
+            self.events = IHyperdriveContractEvents(ihyperdrive_abi, self.w3, address)  # type: ignore
+            self.errors = IHyperdriveContractErrors()
 
         except FallbackNotFound:
             print("Fallback function not found. Continuing...")
 
-    events: IERC4626HyperdriveContractEvents
+    events: IHyperdriveContractEvents
 
-    errors: IERC4626HyperdriveContractErrors = IERC4626HyperdriveContractErrors()
+    errors: IHyperdriveContractErrors = IHyperdriveContractErrors()
 
-    functions: IERC4626HyperdriveContractFunctions
+    functions: IHyperdriveContractFunctions
 
     @classmethod
     def constructor(cls) -> ContractConstructor:  # type: ignore
         """Creates a transaction with the contract's constructor function.
 
         Parameters
         ----------
@@ -6400,11 +6626,11 @@
 
         Returns
         -------
         Self
             A deployed instance of the contract.
         """
         contract = super().factory(w3, class_name, **kwargs)
-        contract.functions = IERC4626HyperdriveContractFunctions(ierc4626hyperdrive_abi, w3, None)
-        contract.errors = IERC4626HyperdriveContractErrors()
+        contract.functions = IHyperdriveContractFunctions(ihyperdrive_abi, w3, None)
+        contract.errors = IHyperdriveContractErrors()
 
         return contract
```

### Comparing `hyperdrivepy-0.9.2/python/hyperdrivepy/pypechain_types/IHyperdriveTypes.py` & `hyperdrivepy-1.0.1/python/hyperdrivepy/types.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,131 +1,134 @@
-"""Dataclasses for all structs in the IHyperdrive contract.
-
-DO NOT EDIT.  This file was generated by pypechain.  See documentation at
-https://github.com/delvtech/pypechain """
-
-# super() call methods are generic, while our version adds values & types
-# pylint: disable=arguments-differ
+"""Types for the hyperdrive contract."""
 
 # contracts have PascalCase names
 # pylint: disable=invalid-name
-# contracts control how many attributes and arguments we have in generated code
+# We do not define the number of instance attributes
 # pylint: disable=too-many-instance-attributes
-# pylint: disable=too-many-arguments
-# unable to determine which imports will be used in the generated code
-# pylint: disable=unused-import
-# we don't need else statement if the other conditionals all have return,
-# but it's easier to generate
-# pylint: disable=no-else-return
+# pylint: disable=too-few-public-methods
 from __future__ import annotations
 
 from dataclasses import dataclass
+from typing import Any, Protocol
 
 
 @dataclass
-class Options:
-    """Options struct."""
+class Fees:
+    """Protocal Fees."""
 
-    destination: str
-    asBase: bool
-    extraData: bytes
+    curve: str
+    flat: str
+    governanceLP: str
+    governanceZombie: str
+
+
+@dataclass
+class PoolConfig:
+    """Static configuration for the hyperdrive contract. Set at deploy time."""
+
+    baseToken: str
+    vaultSharesToken: str
+    linkerFactory: str
+    linkerCodeHash: str
+    initialVaultSharePrice: str
+    minimumShareReserves: str
+    minimumTransactionAmount: str
+    positionDuration: str
+    checkpointDuration: str
+    timeStretch: str
+    governance: str
+    feeCollector: str
+    sweepCollector: str
+    fees: Fees
 
 
 @dataclass
-class Checkpoint:
+class PoolInfo:
+    """Current state information of the hyperdrive contract. Includes things like reserve levels and share prices."""
+
+    shareReserves: str
+    shareAdjustment: str
+    zombieBaseProceeds: str
+    zombieShareReserves: str
+    bondReserves: str
+    lpTotalSupply: str
+    vaultSharePrice: str
+    longsOutstanding: str
+    longAverageMaturityTime: str
+    shortsOutstanding: str
+    shortAverageMaturityTime: str
+    withdrawalSharesReadyToWithdraw: str
+    withdrawalSharesProceeds: str
+    lpSharePrice: str
+    longExposure: str
+
+
+# TODO: pypechain should either use TypedDicts or generate these interfaces.
+class CheckpointType(Protocol):
     """Checkpoint struct."""
 
     vaultSharePrice: int
+    longExposure: int
 
 
-@dataclass
-class MarketState:
+class MarketStateType(Protocol):
     """MarketState struct."""
 
     shareReserves: int
     bondReserves: int
+    shareAdjustment: int
     longExposure: int
     longsOutstanding: int
-    shareAdjustment: int
     shortsOutstanding: int
     longAverageMaturityTime: int
     shortAverageMaturityTime: int
     isInitialized: bool
     isPaused: bool
-    zombieBaseProceeds: int
-    zombieShareReserves: int
 
 
-@dataclass
-class Fees:
+class FeesType(Protocol):
     """Fees struct."""
 
     curve: int
     flat: int
     governanceLP: int
     governanceZombie: int
 
 
-@dataclass
-class PoolConfig:
+class PoolConfigType(Protocol):
     """PoolConfig struct."""
 
     baseToken: str
+    vaultSharesToken: str
     linkerFactory: str
     linkerCodeHash: bytes
     initialVaultSharePrice: int
     minimumShareReserves: int
     minimumTransactionAmount: int
     positionDuration: int
     checkpointDuration: int
     timeStretch: int
     governance: str
     feeCollector: str
-    fees: Fees
+    sweepCollector: str
+    # TODO: nested Protocol types do not play well with dataclasses.  use 'or Any' for now.
+    fees: FeesType | Any
 
 
-@dataclass
-class PoolInfo:
+class PoolInfoType(Protocol):
     """PoolInfo struct."""
 
     shareReserves: int
     shareAdjustment: int
     zombieBaseProceeds: int
     zombieShareReserves: int
-    bondReserves: int
     lpTotalSupply: int
     vaultSharePrice: int
     longsOutstanding: int
     longAverageMaturityTime: int
     shortsOutstanding: int
+    bondReserves: int
     shortAverageMaturityTime: int
     withdrawalSharesReadyToWithdraw: int
     withdrawalSharesProceeds: int
     lpSharePrice: int
     longExposure: int
-
-
-@dataclass
-class WithdrawPool:
-    """WithdrawPool struct."""
-
-    readyToWithdraw: int
-    proceeds: int
-
-
-@dataclass
-class ErrorInfo:
-    """Custom contract error information."""
-
-    name: str
-    selector: str
-    signature: str
-    inputs: list[ErrorParams]
-
-
-@dataclass
-class ErrorParams:
-    """Parameter info for custom contract errors."""
-
-    name: str
-    solidity_type: str
-    python_type: str
```

### Comparing `hyperdrivepy-0.9.2/python/hyperdrivepy/pypechain_types/utilities.py` & `hyperdrivepy-1.0.1/python/hyperdrivepy/pypechain_types/utilities.py`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-0.9.2/python/hyperdrivepy/utils.py` & `hyperdrivepy-1.0.1/python/hyperdrivepy/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,24 +15,26 @@
 
 
 def _serialize_pool_config(
     pool_config: types.PoolConfigType,
 ) -> types.PoolConfig:
     return types.PoolConfig(
         baseToken=str(pool_config.baseToken),
+        vaultSharesToken=str(pool_config.vaultSharesToken),
         linkerFactory=str(pool_config.linkerFactory),
         linkerCodeHash=pool_config.linkerCodeHash.hex(),  # bytes to string in hex format
         initialVaultSharePrice=str(pool_config.initialVaultSharePrice),
         minimumShareReserves=str(pool_config.minimumShareReserves),
         minimumTransactionAmount=str(pool_config.minimumTransactionAmount),
         positionDuration=str(pool_config.positionDuration),
         checkpointDuration=str(pool_config.checkpointDuration),
         timeStretch=str(pool_config.timeStretch),
         governance=str(pool_config.governance),
         feeCollector=str(pool_config.feeCollector),
+        sweepCollector=str(pool_config.sweepCollector),
         fees=types.Fees(
             curve=str(pool_config.fees.curve),
             flat=str(pool_config.fees.flat),
             governanceLP=str(pool_config.fees.governanceLP),
             governanceZombie=str(pool_config.fees.governanceZombie),
         ),
     )
```

### Comparing `hyperdrivepy-0.9.2/python/hyperdrivepy.egg-info/PKG-INFO` & `hyperdrivepy-1.0.1/python/hyperdrivepy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperdrivepy
-Version: 0.9.2
+Version: 1.0.1
 Project-URL: Homepage, https://github.com/delvtech/hyperdrive-bindings
 Project-URL: Issues, https://github.com/delvtech/hyperdrive-bindings/issues
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `hyperdrivepy-0.9.2/python/hyperdrivepy.egg-info/SOURCES.txt` & `hyperdrivepy-1.0.1/python/hyperdrivepy.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 python/hyperdrivepy/types.py
 python/hyperdrivepy/utils.py
 python/hyperdrivepy.egg-info/PKG-INFO
 python/hyperdrivepy.egg-info/SOURCES.txt
 python/hyperdrivepy.egg-info/dependency_links.txt
 python/hyperdrivepy.egg-info/not-zip-safe
 python/hyperdrivepy.egg-info/top_level.txt
-python/hyperdrivepy/pypechain_types/IERC4626HyperdriveContract.py
-python/hyperdrivepy/pypechain_types/IERC4626HyperdriveTypes.py
+python/hyperdrivepy/pypechain_types/IHyperdriveContract.py
 python/hyperdrivepy/pypechain_types/IHyperdriveTypes.py
 python/hyperdrivepy/pypechain_types/__init__.py
 python/hyperdrivepy/pypechain_types/utilities.py
 src/hyperdrive_state.rs
 src/hyperdrive_state_methods.rs
 src/hyperdrive_utils.rs
 src/lib.rs
```

### Comparing `hyperdrivepy-0.9.2/src/hyperdrive_state.rs` & `hyperdrivepy-1.0.1/src/hyperdrive_state.rs`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-0.9.2/src/hyperdrive_state_methods.rs` & `hyperdrivepy-1.0.1/src/hyperdrive_state_methods.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 use ethers::core::types::{I256, U256};
 use fixed_point::FixedPoint;
 
 use pyo3::exceptions::PyValueError;
 use pyo3::prelude::*;
-use pyo3::PyErr;
 
 pub use crate::utils::*;
 use crate::HyperdriveState;
 pub use crate::PyPoolConfig;
 pub use crate::PyPoolInfo;
 use hyperdrive_math::State;
 use hyperdrive_math::YieldSpace;
@@ -18,73 +17,141 @@
     pub fn __init__(pool_config: &PyAny, pool_info: &PyAny) -> PyResult<Self> {
         let rust_pool_config = PyPoolConfig::extract(pool_config)?.pool_config;
         let rust_pool_info = PyPoolInfo::extract(pool_info)?.pool_info;
         let state = State::new(rust_pool_config, rust_pool_info);
         Ok(HyperdriveState::new(state))
     }
 
-    pub fn get_max_spot_price(&self) -> PyResult<String> {
-        let result_fp = self.state.get_max_spot_price();
+    pub fn calculate_solvency(&self) -> PyResult<String> {
+        let result_fp = self.state.calculate_solvency();
         let result = U256::from(result_fp).to_string();
         return Ok(result);
     }
 
-    pub fn get_spot_price_after_long(&self, long_amount: &str) -> PyResult<String> {
-        let long_amount_fp = FixedPoint::from(U256::from_dec_str(long_amount).map_err(|_| {
-            PyErr::new::<PyValueError, _>("Failed to convert long_amount string to U256")
+    pub fn calculate_spot_price_after_long(
+        &self,
+        base_amount: &str,
+        maybe_bond_amount: Option<&str>,
+    ) -> PyResult<String> {
+        let base_amount_fp = FixedPoint::from(U256::from_dec_str(base_amount).map_err(|_| {
+            PyErr::new::<PyValueError, _>("Failed to convert base_amount string to U256")
         })?);
-        let result_fp = self.state.get_spot_price_after_long(long_amount_fp);
+        let maybe_bond_amount_fp = if let Some(bond_amount) = maybe_bond_amount {
+            Some(FixedPoint::from(U256::from_dec_str(bond_amount).map_err(
+                |_| {
+                    PyErr::new::<PyValueError, _>(
+                        "Failed to convert maybe_bond_amount string to U256",
+                    )
+                },
+            )?))
+        } else {
+            None
+        };
+        let result_fp = self
+            .state
+            .calculate_spot_price_after_long(base_amount_fp, maybe_bond_amount_fp)
+            .unwrap();
         let result = U256::from(result_fp).to_string();
         return Ok(result);
     }
 
-    pub fn get_solvency(&self) -> PyResult<String> {
-        let result_fp = self.state.get_solvency();
+    pub fn calculate_spot_price_after_short(
+        &self,
+        bond_amount: &str,
+        maybe_base_amount: Option<&str>,
+    ) -> PyResult<String> {
+        let bond_amount_fp = FixedPoint::from(U256::from_dec_str(bond_amount).map_err(|_| {
+            PyErr::new::<PyValueError, _>("Failed to convert bond_amount string to U256")
+        })?);
+        let maybe_base_amount_fp = if let Some(base_amount) = maybe_base_amount {
+            Some(FixedPoint::from(U256::from_dec_str(base_amount).map_err(
+                |_| {
+                    PyErr::new::<PyValueError, _>(
+                        "Failed to convert maybe_base_amount string to U256",
+                    )
+                },
+            )?))
+        } else {
+            None
+        };
+        let result_fp = self
+            .state
+            .calculate_spot_price_after_short(bond_amount_fp, maybe_base_amount_fp)
+            .unwrap();
         let result = U256::from(result_fp).to_string();
         return Ok(result);
     }
 
-    pub fn get_spot_price(&self) -> PyResult<String> {
-        let result_fp = self.state.get_spot_price();
+    pub fn calculate_spot_price(&self) -> PyResult<String> {
+        let result_fp = self.state.calculate_spot_price();
+        let result = U256::from(result_fp).to_string();
+        return Ok(result);
+    }
+
+    pub fn calculate_spot_rate_after_long(
+        &self,
+        base_amount: &str,
+        maybe_bond_amount: Option<&str>,
+    ) -> PyResult<String> {
+        let base_amount_fp = FixedPoint::from(U256::from_dec_str(base_amount).map_err(|_| {
+            PyErr::new::<PyValueError, _>("Failed to convert base_amount string to U256")
+        })?);
+        let maybe_bond_amount_fp = if let Some(bond_amount) = maybe_bond_amount {
+            Some(FixedPoint::from(U256::from_dec_str(bond_amount).map_err(
+                |_| {
+                    PyErr::new::<PyValueError, _>(
+                        "Failed to convert maybe_bond_amount string to U256",
+                    )
+                },
+            )?))
+        } else {
+            None
+        };
+        let result_fp = self
+            .state
+            .calculate_spot_rate_after_long(base_amount_fp, maybe_bond_amount_fp)
+            .unwrap();
         let result = U256::from(result_fp).to_string();
         return Ok(result);
     }
 
-    pub fn get_spot_rate(&self) -> PyResult<String> {
-        let result_fp = self.state.get_spot_rate();
+    pub fn calculate_spot_rate(&self) -> PyResult<String> {
+        let result_fp = self.state.calculate_spot_rate();
         let result = U256::from(result_fp).to_string();
         return Ok(result);
     }
 
     pub fn calculate_open_long(&self, base_amount: &str) -> PyResult<String> {
         let base_amount_fp = FixedPoint::from(U256::from_dec_str(base_amount).map_err(|_| {
             PyErr::new::<PyValueError, _>("Failed to convert base_amount string to U256")
         })?);
-        let result_fp = self.state.calculate_open_long(base_amount_fp);
+        let result_fp = self.state.calculate_open_long(base_amount_fp).unwrap();
         let result = U256::from(result_fp).to_string();
         return Ok(result);
     }
 
     pub fn calculate_close_long(
         &self,
         bond_amount: &str,
-        normalized_time_remaining: &str,
+        maturity_time: &str,
+        current_time: &str,
     ) -> PyResult<String> {
         let bond_amount_fp = FixedPoint::from(U256::from_dec_str(bond_amount).map_err(|_| {
             PyErr::new::<PyValueError, _>("Failed to convert bond_amount string to U256")
         })?);
-        let normalized_time_remaining_fp =
-            FixedPoint::from(U256::from_dec_str(normalized_time_remaining).map_err(|_| {
-                PyErr::new::<PyValueError, _>(
-                    "Failed to convert normalized_time_remaining string to U256",
-                )
-            })?);
-        let result_fp = self
-            .state
-            .calculate_close_long(bond_amount_fp, normalized_time_remaining_fp);
+        let maturity_time = U256::from_dec_str(maturity_time).map_err(|_| {
+            PyErr::new::<PyValueError, _>("Failed to convert maturity_time string to U256")
+        })?;
+        let current_time = U256::from_dec_str(current_time).map_err(|_| {
+            PyErr::new::<PyValueError, _>("Failed to convert current_time string to U256")
+        })?;
+
+        let result_fp =
+            self.state
+                .calculate_close_long(bond_amount_fp, maturity_time, current_time);
         let result = U256::from(result_fp).to_string();
         return Ok(result);
     }
 
     pub fn calculate_open_short(
         &self,
         short_amount: &str,
@@ -95,144 +162,154 @@
             PyErr::new::<PyValueError, _>("Failed to convert short_amount string to U256")
         })?);
         let spot_price_fp = FixedPoint::from(U256::from_dec_str(spot_price).map_err(|_| {
             PyErr::new::<PyValueError, _>("Failed to convert spot_price string to U256")
         })?);
         let open_vault_share_price_fp =
             FixedPoint::from(U256::from_dec_str(open_vault_share_price).map_err(|_| {
-                PyErr::new::<PyValueError, _>("Failed to convert open_vault_share_price string to U256")
+                PyErr::new::<PyValueError, _>(
+                    "Failed to convert open_vault_share_price string to U256",
+                )
             })?);
         let result_fp = self
             .state
             .calculate_open_short(short_amount_fp, spot_price_fp, open_vault_share_price_fp)
             .unwrap();
         let result = U256::from(result_fp).to_string();
         return Ok(result);
     }
 
     pub fn calculate_close_short(
         &self,
         bond_amount: &str,
         open_vault_share_price: &str,
         close_vault_share_price: &str,
-        normalized_time_remaining: &str,
+        maturity_time: &str,
+        current_time: &str,
     ) -> PyResult<String> {
         let bond_amount_fp = FixedPoint::from(U256::from_dec_str(bond_amount).map_err(|_| {
             PyErr::new::<PyValueError, _>("Failed to convert bond_amount string to U256")
         })?);
         let open_vault_share_price_fp =
             FixedPoint::from(U256::from_dec_str(open_vault_share_price).map_err(|_| {
-                PyErr::new::<PyValueError, _>("Failed to convert open_vault_share_price string to U256")
+                PyErr::new::<PyValueError, _>(
+                    "Failed to convert open_vault_share_price string to U256",
+                )
             })?);
         let close_vault_share_price_fp =
             FixedPoint::from(U256::from_dec_str(close_vault_share_price).map_err(|_| {
-                PyErr::new::<PyValueError, _>("Failed to convert close_vault_share_price string to U256")
-            })?);
-        let normalized_time_remaining_fp =
-            FixedPoint::from(U256::from_dec_str(normalized_time_remaining).map_err(|_| {
                 PyErr::new::<PyValueError, _>(
-                    "Failed to convert normalized_time_remaining string to U256",
+                    "Failed to convert close_vault_share_price string to U256",
                 )
             })?);
+        let maturity_time = U256::from_dec_str(maturity_time).map_err(|_| {
+            PyErr::new::<PyValueError, _>("Failed to convert maturity_time string to U256")
+        })?;
+        let current_time = U256::from_dec_str(current_time).map_err(|_| {
+            PyErr::new::<PyValueError, _>("Failed to convert current_time string to U256")
+        })?;
         let result_fp = self.state.calculate_close_short(
             bond_amount_fp,
             open_vault_share_price_fp,
             close_vault_share_price_fp,
-            normalized_time_remaining_fp,
+            maturity_time,
+            current_time,
         );
         let result = U256::from(result_fp).to_string();
         return Ok(result);
     }
 
-    pub fn calculate_bonds_out_given_shares_in_down(&self, amount_in: &str) -> PyResult<String> {
-        let amount_in_fp = FixedPoint::from(U256::from_dec_str(amount_in).map_err(|_| {
-            PyErr::new::<PyValueError, _>("Failed to convert amount_in string to U256")
-        })?);
-        let result_fp = self
-            .state
-            .calculate_bonds_out_given_shares_in_down(amount_in_fp);
-        let result = U256::from(result_fp).to_string();
-        return Ok(result);
-    }
-
-    pub fn calculate_shares_in_given_bonds_out_up(&self, amount_in: &str) -> PyResult<String> {
-        let amount_in_fp = FixedPoint::from(U256::from_dec_str(amount_in).map_err(|_| {
-            PyErr::new::<PyValueError, _>("Failed to convert amount_in string to U256")
-        })?);
-        // We unwrap the error here to throw panic error if this fails
-        let result_fp = self
-            .state
-            .calculate_shares_in_given_bonds_out_up_safe(amount_in_fp).unwrap();
+    pub fn calculate_max_spot_price(&self) -> PyResult<String> {
+        let result_fp = self.state.calculate_max_spot_price();
         let result = U256::from(result_fp).to_string();
         return Ok(result);
     }
 
-    pub fn calculate_shares_in_given_bonds_out_down(&self, amount_in: &str) -> PyResult<String> {
-        let amount_in_fp = FixedPoint::from(U256::from_dec_str(amount_in).map_err(|_| {
-            PyErr::new::<PyValueError, _>("Failed to convert amount_in string to U256")
+    pub fn calculate_targeted_long_with_budget(
+        &self,
+        budget: &str,
+        target_rate: &str,
+        checkpoint_exposure: &str,
+        maybe_max_iterations: Option<usize>,
+        maybe_allowable_error: Option<&str>,
+    ) -> PyResult<String> {
+        let budget_fp = FixedPoint::from(U256::from_dec_str(budget).map_err(|_| {
+            PyErr::new::<PyValueError, _>("Failed to convert budget string to U256")
         })?);
-        let result_fp = self
-            .state
-            .calculate_shares_in_given_bonds_out_down(amount_in_fp);
-        let result = U256::from(result_fp).to_string();
-        return Ok(result);
-    }
-
-    pub fn calculate_shares_out_given_bonds_in_down(&self, amount_in: &str) -> PyResult<String> {
-        let amount_in_fp = FixedPoint::from(U256::from_dec_str(amount_in).map_err(|_| {
-            PyErr::new::<PyValueError, _>("Failed to convert amount_in string to U256")
+        let target_rate_fp = FixedPoint::from(U256::from_dec_str(target_rate).map_err(|_| {
+            PyErr::new::<PyValueError, _>("Failed to convert target_rate string to U256")
         })?);
+        let checkpoint_exposure_i = I256::from_dec_str(checkpoint_exposure).map_err(|_| {
+            PyErr::new::<PyValueError, _>("Failed to convert checkpoint_exposure string to I256")
+        })?;
+        let maybe_allowable_error_fp = if let Some(allowable_error) = maybe_allowable_error {
+            Some(FixedPoint::from(
+                U256::from_dec_str(allowable_error).map_err(|_| {
+                    PyErr::new::<PyValueError, _>(
+                        "Failed to convert maybe_allowable_error string to U256",
+                    )
+                })?,
+            ))
+        } else {
+            None
+        };
         let result_fp = self
             .state
-            .calculate_shares_out_given_bonds_in_down(amount_in_fp);
+            .calculate_targeted_long_with_budget(
+                budget_fp,
+                target_rate_fp,
+                checkpoint_exposure_i,
+                maybe_max_iterations,
+                maybe_allowable_error_fp,
+            )
+            .map_err(|err| {
+                PyErr::new::<PyValueError, _>(format!(
+                    "Calculate_targeted_long_with_budget returned the error: {:?}",
+                    err
+                ))
+            })?;
         let result = U256::from(result_fp).to_string();
         return Ok(result);
     }
 
-    pub fn to_checkpoint(&self, time: &str) -> PyResult<String> {
-        let time_int = U256::from_dec_str(time)
-            .map_err(|_| PyErr::new::<PyValueError, _>("Failed to convert time string to U256"))?;
-        let result_int = self.state.to_checkpoint(time_int);
-        let result = result_int.to_string();
-        return Ok(result);
-    }
-
-    pub fn get_max_long(
+    pub fn calculate_max_long(
         &self,
         budget: &str,
         checkpoint_exposure: &str,
         maybe_max_iterations: Option<usize>,
     ) -> PyResult<String> {
         let budget_fp = FixedPoint::from(U256::from_dec_str(budget).map_err(|_| {
             PyErr::new::<PyValueError, _>("Failed to convert budget string to U256")
         })?);
         let checkpoint_exposure_i = I256::from_dec_str(checkpoint_exposure).map_err(|_| {
             PyErr::new::<PyValueError, _>("Failed to convert checkpoint_exposure string to I256")
         })?;
         let result_fp =
             self.state
-                .get_max_long(budget_fp, checkpoint_exposure_i, maybe_max_iterations);
+                .calculate_max_long(budget_fp, checkpoint_exposure_i, maybe_max_iterations);
         let result = U256::from(result_fp).to_string();
         return Ok(result);
     }
 
-    pub fn get_max_short(
+    pub fn calculate_max_short(
         &self,
         budget: &str,
         open_vault_share_price: &str,
         checkpoint_exposure: &str,
         maybe_conservative_price: Option<&str>,
         maybe_max_iterations: Option<usize>,
     ) -> PyResult<String> {
         let budget_fp = FixedPoint::from(U256::from_dec_str(budget).map_err(|_| {
             PyErr::new::<PyValueError, _>("Failed to convert budget string to U256")
         })?);
         let open_vault_share_price_fp =
             FixedPoint::from(U256::from_dec_str(open_vault_share_price).map_err(|_| {
-                PyErr::new::<PyValueError, _>("Failed to convert open_vault_share_price string to U256")
+                PyErr::new::<PyValueError, _>(
+                    "Failed to convert open_vault_share_price string to U256",
+                )
             })?);
         let checkpoint_exposure_i = I256::from_dec_str(checkpoint_exposure).map_err(|_| {
             PyErr::new::<PyValueError, _>("Failed to convert checkpoint_exposure string to I256")
         })?;
         let maybe_conservative_price_fp = if let Some(conservative_price) = maybe_conservative_price
         {
             Some(FixedPoint::from(
@@ -241,15 +318,15 @@
                         "Failed to convert maybe_conservative_price string to U256",
                     )
                 })?,
             ))
         } else {
             None
         };
-        let result_fp = self.state.get_max_short(
+        let result_fp = self.state.calculate_max_short(
             budget_fp,
             open_vault_share_price_fp,
             checkpoint_exposure_i,
             maybe_conservative_price_fp,
             maybe_max_iterations,
         );
         let result = U256::from(result_fp).to_string();
@@ -265,8 +342,68 @@
             })?;
         let result_fp = self
             .state
             .calculate_present_value(current_block_timestamp_int);
         let result = U256::from(result_fp).to_string();
         return Ok(result);
     }
+
+    pub fn calculate_idle_share_reserves_in_base(&self) -> PyResult<String> {
+        let result_fp = self.state.calculate_idle_share_reserves_in_base();
+        let result = U256::from(result_fp).to_string();
+        return Ok(result);
+    }
+
+    pub fn calculate_bonds_out_given_shares_in_down(&self, amount_in: &str) -> PyResult<String> {
+        let amount_in_fp = FixedPoint::from(U256::from_dec_str(amount_in).map_err(|_| {
+            PyErr::new::<PyValueError, _>("Failed to convert amount_in string to U256")
+        })?);
+        let result_fp = self
+            .state
+            .calculate_bonds_out_given_shares_in_down(amount_in_fp);
+        let result = U256::from(result_fp).to_string();
+        return Ok(result);
+    }
+
+    pub fn calculate_shares_in_given_bonds_out_up(&self, amount_in: &str) -> PyResult<String> {
+        let amount_in_fp = FixedPoint::from(U256::from_dec_str(amount_in).map_err(|_| {
+            PyErr::new::<PyValueError, _>("Failed to convert amount_in string to U256")
+        })?);
+        // We unwrap the error here to throw panic error if this fails
+        let result_fp = self
+            .state
+            .calculate_shares_in_given_bonds_out_up_safe(amount_in_fp)
+            .unwrap();
+        let result = U256::from(result_fp).to_string();
+        return Ok(result);
+    }
+
+    pub fn calculate_shares_in_given_bonds_out_down(&self, amount_in: &str) -> PyResult<String> {
+        let amount_in_fp = FixedPoint::from(U256::from_dec_str(amount_in).map_err(|_| {
+            PyErr::new::<PyValueError, _>("Failed to convert amount_in string to U256")
+        })?);
+        let result_fp = self
+            .state
+            .calculate_shares_in_given_bonds_out_down(amount_in_fp);
+        let result = U256::from(result_fp).to_string();
+        return Ok(result);
+    }
+
+    pub fn calculate_shares_out_given_bonds_in_down(&self, amount_in: &str) -> PyResult<String> {
+        let amount_in_fp = FixedPoint::from(U256::from_dec_str(amount_in).map_err(|_| {
+            PyErr::new::<PyValueError, _>("Failed to convert amount_in string to U256")
+        })?);
+        let result_fp = self
+            .state
+            .calculate_shares_out_given_bonds_in_down(amount_in_fp);
+        let result = U256::from(result_fp).to_string();
+        return Ok(result);
+    }
+
+    pub fn to_checkpoint(&self, time: &str) -> PyResult<String> {
+        let time_int = U256::from_dec_str(time)
+            .map_err(|_| PyErr::new::<PyValueError, _>("Failed to convert time string to U256"))?;
+        let result_int = self.state.to_checkpoint(time_int);
+        let result = result_int.to_string();
+        return Ok(result);
+    }
 }
```

### Comparing `hyperdrivepy-0.9.2/src/hyperdrive_utils.rs` & `hyperdrivepy-1.0.1/src/hyperdrive_utils.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 use ethers::core::types::{I256, U256};
 use fixed_point::FixedPoint;
 
+use pyo3::exceptions::PyValueError;
 use pyo3::prelude::*;
 use pyo3::PyErr;
-use pyo3::exceptions::PyValueError;
 
 use hyperdrive_math::{
+    calculate_effective_share_reserves as rs_calculate_effective_share_reserves,
     calculate_initial_bond_reserves as rs_calculate_initial_bond_reserves,
-    get_effective_share_reserves as rs_get_effective_share_reserves,
-    get_time_stretch as rs_get_time_stretch,
+    calculate_time_stretch as rs_calculate_time_stretch,
 };
 
 #[pyfunction]
 pub fn calculate_initial_bond_reserves(
     effective_share_reserves: &str,
     initial_vault_share_price: &str,
     apr: &str,
@@ -23,15 +23,17 @@
         FixedPoint::from(U256::from_dec_str(effective_share_reserves).map_err(|_| {
             PyErr::new::<PyValueError, _>(
                 "Failed to convert effective_share_reserves string to U256",
             )
         })?);
     let initial_vault_share_price_fp =
         FixedPoint::from(U256::from_dec_str(initial_vault_share_price).map_err(|_| {
-            PyErr::new::<PyValueError, _>("Failed to convert initial_vault_share_price string to U256")
+            PyErr::new::<PyValueError, _>(
+                "Failed to convert initial_vault_share_price string to U256",
+            )
         })?);
     let apr_fp = FixedPoint::from(
         U256::from_dec_str(apr)
             .map_err(|_| PyErr::new::<PyValueError, _>("Failed to convert apr string to U256"))?,
     );
     let position_duration_fp =
         FixedPoint::from(U256::from_dec_str(position_duration).map_err(|_| {
@@ -48,36 +50,36 @@
         time_stretch_fp,
     );
     let result = U256::from(result_fp).to_string();
     return Ok(result);
 }
 
 #[pyfunction]
-pub fn get_effective_share_reserves(
+pub fn calculate_effective_share_reserves(
     share_reserves: &str,
     share_adjustment: &str,
 ) -> PyResult<String> {
     let share_reserves_fp = FixedPoint::from(U256::from_dec_str(share_reserves).map_err(|_| {
         PyErr::new::<PyValueError, _>("Failed to convert share_reserves string to U256")
     })?);
     let share_adjustment_i = I256::from_dec_str(share_adjustment).map_err(|_| {
         PyErr::new::<PyValueError, _>("Failed to convert share_adjustment string to I256")
     })?;
-    let result_fp = rs_get_effective_share_reserves(share_reserves_fp, share_adjustment_i);
+    let result_fp = rs_calculate_effective_share_reserves(share_reserves_fp, share_adjustment_i);
     let result = U256::from(result_fp).to_string();
     return Ok(result);
 }
 
 #[pyfunction]
-pub fn get_time_stretch(rate: &str, position_duration: &str) -> PyResult<String> {
+pub fn calculate_time_stretch(rate: &str, position_duration: &str) -> PyResult<String> {
     let rate_fp = FixedPoint::from(
         U256::from_dec_str(rate)
             .map_err(|_| PyErr::new::<PyValueError, _>("Failed to convert rate string to U256"))?,
     );
     let position_duration_fp = FixedPoint::from(
         U256::from_dec_str(position_duration)
             .map_err(|_| PyErr::new::<PyValueError, _>("Failed to convert rate string to U256"))?,
     );
-    let result_fp = rs_get_time_stretch(rate_fp, position_duration_fp);
+    let result_fp = rs_calculate_time_stretch(rate_fp, position_duration_fp);
     let result = U256::from(result_fp).to_string();
     return Ok(result);
 }
```

### Comparing `hyperdrivepy-0.9.2/src/lib.rs` & `hyperdrivepy-1.0.1/src/lib.rs`

 * *Files 15% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 mod utils;
 
 use pyo3::prelude::*;
 
 use hyperdrive_state::HyperdriveState;
 pub use hyperdrive_state_methods::*;
 pub use hyperdrive_utils::{
-    calculate_initial_bond_reserves, get_effective_share_reserves, get_time_stretch,
+    calculate_effective_share_reserves, calculate_initial_bond_reserves, calculate_time_stretch,
 };
 pub use pool_config::PyPoolConfig;
 pub use pool_info::PyPoolInfo;
 
 /// Get the share reserves after subtracting the adjustment used for
 /// A pyO3 wrapper for the hyperdrive_math crate.
 #[pymodule]
 #[pyo3(name = "hyperdrivepy")]
 fn hyperdrivepy(_py: Python<'_>, m: &PyModule) -> PyResult<()> {
     m.add_class::<HyperdriveState>()?;
     m.add_function(wrap_pyfunction!(calculate_initial_bond_reserves, m)?)?;
-    m.add_function(wrap_pyfunction!(get_effective_share_reserves, m)?)?;
-    m.add_function(wrap_pyfunction!(get_time_stretch, m)?)?;
+    m.add_function(wrap_pyfunction!(calculate_effective_share_reserves, m)?)?;
+    m.add_function(wrap_pyfunction!(calculate_time_stretch, m)?)?;
     Ok(())
 }
```

### Comparing `hyperdrivepy-0.9.2/src/pool_config.rs` & `hyperdrivepy-1.0.1/src/pool_config.rs`

 * *Files 8% similar despite different names*

```diff
@@ -14,37 +14,41 @@
         PyPoolConfig { pool_config }
     }
 }
 
 impl FromPyObject<'_> for PyPoolConfig {
     fn extract(ob: &PyAny) -> PyResult<Self> {
         let base_token = extract_address_from_attr(ob, "baseToken")?;
+        let vault_shares_token= extract_address_from_attr(ob, "vaultSharesToken")?;
         let linker_factory = extract_address_from_attr(ob, "linkerFactory")?;
         let linker_code_hash = extract_bytes32_from_attr(ob, "linkerCodeHash")?;
         let initial_vault_share_price = extract_u256_from_attr(ob, "initialVaultSharePrice")?;
         let minimum_share_reserves = extract_u256_from_attr(ob, "minimumShareReserves")?;
         let minimum_transaction_amount = extract_u256_from_attr(ob, "minimumTransactionAmount")?;
         let position_duration = extract_u256_from_attr(ob, "positionDuration")?;
         let checkpoint_duration = extract_u256_from_attr(ob, "checkpointDuration")?;
         let time_stretch = extract_u256_from_attr(ob, "timeStretch")?;
         let governance = extract_address_from_attr(ob, "governance")?;
         let fee_collector = extract_address_from_attr(ob, "feeCollector")?;
+        let sweep_collector = extract_address_from_attr(ob, "sweepCollector")?;
         let fees = extract_fees_from_attr(ob, "fees")?;
 
         let pool_config = PoolConfig {
             base_token,
+            vault_shares_token,
             linker_factory,
             linker_code_hash,
-            initial_vault_share_price: initial_vault_share_price,
+            initial_vault_share_price,
             minimum_share_reserves,
             minimum_transaction_amount,
             position_duration,
             checkpoint_duration,
             time_stretch,
             governance,
             fee_collector,
+            sweep_collector,
             fees,
         };
 
         Ok(PyPoolConfig::new(pool_config))
     }
 }
```

### Comparing `hyperdrivepy-0.9.2/src/pool_info.rs` & `hyperdrivepy-1.0.1/src/pool_info.rs`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-0.9.2/src/utils.rs` & `hyperdrivepy-1.0.1/src/utils.rs`

 * *Files identical despite different names*

