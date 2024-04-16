# Comparing `tmp/polars_qt-0.1.5.tar.gz` & `tmp/polars_qt-0.1.6.tar.gz`

## Comparing `polars_qt-0.1.5.tar` & `polars_qt-0.1.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      503 1970-01-01 00:00:00.000000 polars_qt-0.1.5/Cargo.toml
--rw-r--r--   0     1001      127     3716 2024-04-10 09:49:19.000000 polars_qt-0.1.5/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0     1001      127      111 2024-04-10 09:49:19.000000 polars_qt-0.1.5/.gitignore
--rw-r--r--   0     1001      127        8 2024-04-10 09:49:19.000000 polars_qt-0.1.5/.python-version
--rw-r--r--   0     1001      127      645 2024-04-10 09:49:19.000000 polars_qt-0.1.5/Makefile
--rw-r--r--   0     1001      127     1786 2024-04-10 09:49:19.000000 polars_qt-0.1.5/README.md
--rw-r--r--   0     1001      127       38 2024-04-10 09:49:19.000000 polars_qt-0.1.5/polars_qt/__init__.py
--rw-r--r--   0     1001      127     2898 2024-04-10 09:49:19.000000 polars_qt-0.1.5/polars_qt/funcs.py
--rw-r--r--   0     1001      127     3349 2024-04-10 09:49:19.000000 polars_qt-0.1.5/polars_qt/qt.py
--rw-r--r--   0     1001      127     3336 2024-04-10 09:49:19.000000 polars_qt-0.1.5/polars_qt/strategy.py
--rw-r--r--   0     1001      127     2567 2024-04-10 09:49:19.000000 polars_qt-0.1.5/polars_qt/utils.py
--rw-r--r--   0     1001      127       34 2024-04-10 09:49:19.000000 polars_qt-0.1.5/requirements.txt
--rw-r--r--   0     1001      127       42 2024-04-10 09:49:19.000000 polars_qt-0.1.5/rust-toolchain.toml
--rw-r--r--   0     1001      127    13211 2024-04-10 09:49:19.000000 polars_qt-0.1.5/src/equity.rs
--rw-r--r--   0     1001      127      649 2024-04-10 09:49:19.000000 polars_qt-0.1.5/src/if_then.rs
--rw-r--r--   0     1001      127      319 2024-04-10 09:49:19.000000 polars_qt-0.1.5/src/lib.rs
--rw-r--r--   0     1001      127     3250 2024-04-10 09:49:19.000000 polars_qt-0.1.5/src/rolling_rank.rs
--rw-r--r--   0     1001      127     7934 2024-04-10 09:49:19.000000 polars_qt-0.1.5/src/strategy/boll.rs
--rw-r--r--   0     1001      127     6306 2024-04-10 09:49:19.000000 polars_qt-0.1.5/src/strategy/boll_vol_stop.rs
--rw-r--r--   0     1001      127      636 2024-04-10 09:49:19.000000 polars_qt-0.1.5/src/strategy/mod.rs
--rw-r--r--   0     1001      127     1375 2024-04-10 09:49:19.000000 polars_qt-0.1.5/tests/test_equity.py
--rw-r--r--   0     1001      127      867 2024-04-10 09:49:19.000000 polars_qt-0.1.5/tests/test_if_then.py
--rw-r--r--   0     1001      127      662 2024-04-10 09:49:19.000000 polars_qt-0.1.5/tests/test_rolling_rank.py
--rw-r--r--   0     1001      127     1673 2024-04-10 09:49:19.000000 polars_qt-0.1.5/tests/test_strategy.py
--rw-r--r--   0     1001      127    41876 2024-04-10 09:49:31.000000 polars_qt-0.1.5/Cargo.lock
--rw-r--r--   0     1001      127     1773 2024-04-10 09:49:19.000000 polars_qt-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2192 1970-01-01 00:00:00.000000 polars_qt-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      779 1970-01-01 00:00:00.000000 polars_qt-0.1.6/Cargo.toml
+-rw-r--r--   0     1001      127     3716 2024-04-16 06:29:43.000000 polars_qt-0.1.6/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0     1001      127      111 2024-04-16 06:29:43.000000 polars_qt-0.1.6/.gitignore
+-rw-r--r--   0     1001      127        8 2024-04-16 06:29:43.000000 polars_qt-0.1.6/.python-version
+-rw-r--r--   0     1001      127      645 2024-04-16 06:29:43.000000 polars_qt-0.1.6/Makefile
+-rw-r--r--   0     1001      127     1786 2024-04-16 06:29:43.000000 polars_qt-0.1.6/README.md
+-rw-r--r--   0     1001      127       38 2024-04-16 06:29:43.000000 polars_qt-0.1.6/polars_qt/__init__.py
+-rw-r--r--   0     1001      127     2898 2024-04-16 06:29:43.000000 polars_qt-0.1.6/polars_qt/funcs.py
+-rw-r--r--   0     1001      127     3357 2024-04-16 06:29:43.000000 polars_qt-0.1.6/polars_qt/qt.py
+-rw-r--r--   0     1001      127     3210 2024-04-16 06:29:43.000000 polars_qt-0.1.6/polars_qt/strategy.py
+-rw-r--r--   0     1001      127     2567 2024-04-16 06:29:43.000000 polars_qt-0.1.6/polars_qt/utils.py
+-rw-r--r--   0     1001      127       34 2024-04-16 06:29:43.000000 polars_qt-0.1.6/requirements.txt
+-rw-r--r--   0     1001      127       42 2024-04-16 06:29:43.000000 polars_qt-0.1.6/rust-toolchain.toml
+-rw-r--r--   0     1001      127     2054 2024-04-16 06:29:43.000000 polars_qt-0.1.6/src/equity.rs
+-rw-r--r--   0     1001      127      649 2024-04-16 06:29:43.000000 polars_qt-0.1.6/src/if_then.rs
+-rw-r--r--   0     1001      127      319 2024-04-16 06:29:43.000000 polars_qt-0.1.6/src/lib.rs
+-rw-r--r--   0     1001      127     3250 2024-04-16 06:29:43.000000 polars_qt-0.1.6/src/rolling_rank.rs
+-rw-r--r--   0     1001      127      648 2024-04-16 06:29:43.000000 polars_qt-0.1.6/src/strategy/boll.rs
+-rw-r--r--   0     1001      127      580 2024-04-16 06:29:43.000000 polars_qt-0.1.6/src/strategy/from_input.rs
+-rw-r--r--   0     1001      127       26 2024-04-16 06:29:43.000000 polars_qt-0.1.6/src/strategy/mod.rs
+-rw-r--r--   0     1001      127     1375 2024-04-16 06:29:43.000000 polars_qt-0.1.6/tests/test_equity.py
+-rw-r--r--   0     1001      127      867 2024-04-16 06:29:43.000000 polars_qt-0.1.6/tests/test_if_then.py
+-rw-r--r--   0     1001      127      662 2024-04-16 06:29:43.000000 polars_qt-0.1.6/tests/test_rolling_rank.py
+-rw-r--r--   0     1001      127     1919 2024-04-16 06:29:43.000000 polars_qt-0.1.6/tests/test_strategy.py
+-rw-r--r--   0     1001      127    44016 2024-04-16 06:30:03.000000 polars_qt-0.1.6/Cargo.lock
+-rw-r--r--   0     1001      127     1773 2024-04-16 06:29:43.000000 polars_qt-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2192 1970-01-01 00:00:00.000000 polars_qt-0.1.6/PKG-INFO
```

### Comparing `polars_qt-0.1.5/.github/workflows/publish_to_pypi.yml` & `polars_qt-0.1.6/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.5/Makefile` & `polars_qt-0.1.6/Makefile`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.5/README.md` & `polars_qt-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.5/polars_qt/funcs.py` & `polars_qt-0.1.6/polars_qt/funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,30 +53,30 @@
     init_cash: int = 10_000_000,
     multiplier: int = 1,
     leverage: float = 1,
     slippage: float | IntoExpr = 0,
     ticksize: float = 0,
     c_rate: float = 3e-4,
     blowup: bool = False,
-    commision_type: str = "percent",
+    commision_type: str = "Percent",
     contract_chg_signal: IntoExpr | None = None,
 ) -> pl.Expr:
     open = parse_into_expr(open).cast(pl.Float64)
     close = parse_into_expr(close).cast(pl.Float64)
     signal = parse_into_expr(signal).cast(pl.Float64)
     pos = signal.shift(fill_value=0) if is_signal else signal
     base_config = {
         "init_cash": int(init_cash),
         "multiplier": multiplier,
         "leverage": leverage,
         "c_rate": c_rate,
         "blowup": blowup,
         "commision_type": commision_type,
     }
-    assert commision_type in ["percent", "absolute"]
+    assert commision_type in ["Percent", "Absolute"]
     from numbers import Number
 
     if isinstance(slippage, Number):
         base_config["slippage"] = slippage
         base_config["ticksize"] = ticksize
         args = [pos, open, close]
         if contract_chg_signal is not None:
```

### Comparing `polars_qt-0.1.5/polars_qt/qt.py` & `polars_qt-0.1.6/polars_qt/qt.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         init_cash: int = 10_000_000,
         multiplier: int = 1,
         leverage: float = 1,
         slippage: float | IntoExpr = 0,
         ticksize: float = 0,
         c_rate: float = 3e-4,
         blowup: bool = False,
-        commision_type: str = "percent",
+        commision_type: str = "Percent",
         contract_chg_signal: IntoExpr | None = None,
     ):
         return calc_future_ret(
             self.expr,
             open=open,
             close=close,
             is_signal=is_signal,
@@ -53,15 +53,15 @@
 
     def boll(
         self,
         params: tuple[int, float, float] | tuple[int, float] | int,
         min_periods: int | None = None,
         filters: tuple[IntoExpr, IntoExpr, IntoExpr, IntoExpr] | None = None,
         *,
-        fac_vol: IntoExpr | None=None,
+        # fac_vol: IntoExpr | None=None,
         rev=False,
         delay_open: bool = False,
         long_signal: float = 1,
         short_signal: float = -1,
         close_signal: float = 0,
     ) -> pl.Expr:
         """
@@ -73,25 +73,25 @@
             if we use fac_vol stop
                 params: window, open_width, close_width(default: 0.0), fac_vol_width
                 the last of the params will be parsed as fac_vol_width
         min_periods: minimum periods to calculate bollinger bands
         filters: long_open, long_stop, short_open, short_stop
             for open condition, if filter is False, open behavior is disabled
             for stop condition, if filter is True, return signal will be close_signal
-        fac_vol:
-            a expression to calculate fac_vol, if None, we will use the default bollinger bands
+        # fac_vol:
+        #     a expression to calculate fac_vol, if None, we will use the default bollinger bands
         rev: reverse the long and short signal, filters will also be reversed automatically
         delay_open: if open signal is blocked by filters, whether to delay the open signal when filters are True
         """
         return boll(
             self.expr,
             params=params,
             min_periods=min_periods,
             filters=filters,
-            fac_vol=fac_vol,
+            # fac_vol=fac_vol,
             rev=rev,
             delay_open=delay_open,
             long_signal=long_signal,
             short_signal=short_signal,
             close_signal=close_signal,
     )
```

### Comparing `polars_qt-0.1.5/polars_qt/strategy.py` & `polars_qt-0.1.6/polars_qt/strategy.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 def boll(
     fac: IntoExpr,
     params: tuple[int, float, float] | tuple[int, float] | int,
     min_periods: int | None=None,
     filters: tuple[IntoExpr, IntoExpr, IntoExpr, IntoExpr] | None=None,
     *,
-    fac_vol: IntoExpr | None=None,
+    # fac_vol: IntoExpr | None=None,
     rev=False,
     delay_open: bool=True,
     long_signal: float=1,
     short_signal: float=-1,
     close_signal: float=0,
 ) -> pl.Expr:
     """
@@ -32,58 +32,60 @@
         if we use fac_vol stop
             params: window, open_width, close_width(default: 0.0), fac_vol_width
             the last of the params will be parsed as fac_vol_width
     min_periods: minimum periods to calculate bollinger bands
     filters: long_open, long_stop, short_open, short_stop
         for open condition, if filter is False, open behavior is disabled
         for stop condition, if filter is True, return signal will be close_signal
-    fac_vol:
-        a expression to calculate fac_vol, if None, we will use the default bollinger bands
+    # fac_vol:
+    #     a expression to calculate fac_vol, if None, we will use the default bollinger bands
     rev: reverse the long and short signal, filters will also be reversed automatically
     delay_open: if open signal is blocked by filters, whether to delay the open signal when filters are True
     """
     fac = parse_into_expr(fac)
     # process params
-    params, last_param = (params[:-1], params[-1]) if fac_vol is not None else (params, None)
+    params, last_param = (params, None)
     if not isinstance(params, (tuple, list)):
         params = (params, 0., 0., last_param)
     elif len(params) == 1:
         params = (*params, 0., 0., last_param)
     elif len(params) == 2:
         params = (*params, 0., last_param)
     elif len(params) == 3:
         params = (*params, last_param)
     # process min_periods
     if min_periods is None:
         min_periods = params[0] // 2
     # calculate bollinger bands
-    middle = fac.rolling_mean(params[0], min_periods=min_periods)
-    std = fac.rolling_std(params[0], min_periods=min_periods)
+    # middle = fac.rolling_mean(params[0], min_periods=min_periods)
+    # std = fac.rolling_std(params[0], min_periods=min_periods)
 
     # process args and filters
-    args = [fac, middle, std] if fac_vol is None else [fac, middle, std, parse_into_expr(fac_vol).cast(pl.Float64)]
+    args = [fac]
     if filters is not None:
         assert len(filters) == 4, "filters must be a list of 4 elements"
-        filter_flag = True
+        # filter_flag = True
         filters = [parse_into_expr(f).cast(pl.Boolean) if not isinstance(f, bool) else pl.repeat(f, fac.len()) for f in filters]
         filters = [*filters[2:], *filters[:2]] if rev else filters
         args.extend(filters)
     else:
-        filter_flag = False
-        args.extend([pl.lit(None)*4])
+        pass
+        # filter_flag = False
+        # args.extend([pl.lit(None)*4])
     if rev:
         long_signal, short_signal = short_signal, long_signal
     kwargs = {
         "params": params,
-        "filter_flag": filter_flag,
+        # "filter_flag": filter_flag,
+        "min_periods": min_periods,
         "delay_open": delay_open,
         "long_signal": float(long_signal),
         "short_signal": float(short_signal),
         "close_signal": float(close_signal),
     }
     return register_plugin(
         args=args,
         kwargs=kwargs,
-        symbol="boll" if fac_vol is None else "boll_vol_stop",
+        symbol="boll",
         is_elementwise=False,
     )
```

### Comparing `polars_qt-0.1.5/polars_qt/utils.py` & `polars_qt-0.1.6/polars_qt/utils.py`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.5/src/if_then.rs` & `polars_qt-0.1.6/src/if_then.rs`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.5/src/rolling_rank.rs` & `polars_qt-0.1.6/src/rolling_rank.rs`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.5/tests/test_equity.py` & `polars_qt-0.1.6/tests/test_equity.py`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.5/tests/test_if_then.py` & `polars_qt-0.1.6/tests/test_if_then.py`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.5/tests/test_rolling_rank.py` & `polars_qt-0.1.6/tests/test_rolling_rank.py`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.5/tests/test_strategy.py` & `polars_qt-0.1.6/tests/test_strategy.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,34 +2,37 @@
 from polars.testing import assert_series_equal
 
 import polars_qt
 
 
 def test_boll():
     df = pl.DataFrame({
-        'close': [10., 11, 12, 10, 11, 12, 10, 11, 12, 13, 14, 10, 7, 5, 4, 3, 4, 4, 3, 2],
+        'close': [10., 11, 11.9, 10, 11, 12, 10, 11, 12, 13, 14, 10, 7, 5, 4, 3, 4, 4, 3, 2],
         'short_open_filter': [1] * 11 + [0, 0, 1, 1, 1] + [1] * 4,
     })
     df = df.with_columns([
+        pl.col('close').rolling_mean(4, min_periods=2).alias('mean'),
+        pl.col('close').rolling_std(4, min_periods=2).alias('std'),
         pl.col('close').qt.boll((4, 1), delay_open=False).alias('s1'), # base boll
         # boll with filters
         pl.col('close').qt.boll((4, 1), filters=[
             pl.col('close') > 0, False,  # long open, long stop
             'short_open_filter', False,  # short open, short stop
         ], delay_open=False).alias('s2'),
         # boll with filters and delay open
         pl.col('close').qt.boll((4, 1), filters=[
             pl.col('close') > 0, False,  # long open, long stop
             'short_open_filter', False,  # short open, short stop
         ], delay_open=True).alias('s3'),
-        # boll with fac_vol stop, take profit if close reaches 5 * fac_vol
-        pl.col('close').qt.boll((4, 1, 5), fac_vol=pl.repeat(1, pl.col('close').len())).alias('s4'),
-    ])
-    expect1 = pl.Series('s1', [0., 0, 1, 0, 0, 0, 0, 0, 0, 1, 1, -1, -1, -1, -1, -1, 0, 0, 0, -1])
+        # # boll with fac_vol stop, take profit if close reaches 5 * fac_vol
+        # pl.col('close').qt.boll((4, 1, 5), fac_vol=pl.repeat(1, pl.col('close').len())).alias('s4'),
+    ])#.with_columns(upper=pl.col('mean')+pl.col('std'), down=pl.col('mean')-pl.col('std')).to_pandas()
+
+    expect1 = pl.Series('s1', [0., 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, -1, -1, -1, -1, -1, 0, 0, 0, -1])
     assert_series_equal(df['s1'], expect1)
-    expect2 = pl.Series('s2', [0., 0, 1, 0, 0, 0, 0, 0, 0, 1, 1, 0, 0, 0, 0, -1, 0, 0, 0, -1])
+    expect2 = pl.Series('s2', [0., 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 0, 0, 0, 0, -1, 0, 0, 0, -1])
     assert_series_equal(df['s2'], expect2)
-    expect3 = pl.Series('s3', [0., 0, 1, 0, 0, 0, 0, 0, 0, 1, 1, 0, 0, -1, -1, -1, 0, 0, 0, -1])
+    expect3 = pl.Series('s3', [0., 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 0, 0, -1, -1, -1, 0, 0, 0, -1])
     assert_series_equal(df['s3'], expect3)
-    expect3 = pl.Series('s4', [0., 0, 1, 0, 0, 0, 0, 0, 0, 1, 1, -1, -1, 0, 0, -1, 0, 0, 0, -1])
-    assert_series_equal(df['s4'], expect3)
+    # expect3 = pl.Series('s4', [0., 0, 1, 0, 0, 0, 0, 0, 0, 1, 1, -1, -1, 0, 0, -1, 0, 0, 0, -1])
+    # assert_series_equal(df['s4'], expect3)
 test_boll()
```

### Comparing `polars_qt-0.1.5/Cargo.lock` & `polars_qt-0.1.6/Cargo.lock`

 * *Files 5% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "allocator-api2"
-version = "0.2.16"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0942ffc6dcaadf03badf6e6a2d0228460359d5e34b57ccdc720b7382dfbd5ec5"
+checksum = "5c6cb57a04249c6480766f7f7cef5467412af1490f8d1e243141daddada3264f"
 
 [[package]]
 name = "android-tzdata"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
 
@@ -118,15 +118,15 @@
 name = "bytemuck_derive"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4da9a32f3fed317401fa3c862968128267c3106685286e15d5aaa3d7389c2f60"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.59",
 ]
 
 [[package]]
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
@@ -135,38 +135,40 @@
 name = "bytes"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cc"
-version = "1.0.92"
+version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2678b2e3449475e95b0aa6f9b506a28e61b3dc8996592b983695e8ebb58a8b41"
+checksum = "17f6e324229dc011159fcc089755d1e2e216a90d43a7dea6853ca740b84f35e7"
 dependencies = [
  "jobserver",
  "libc",
 ]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.37"
+version = "0.4.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a0d04d43504c61aa6c7531f1871dd0d418d91130162063b789da00fd7057a5e"
+checksum = "a21f936df1771bf62b77f047b726c4625ff2e8aa607c01ec06e5a05bd8463401"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
+ "js-sys",
  "num-traits",
- "windows-targets 0.52.4",
+ "wasm-bindgen",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "core-foundation-sys"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
@@ -218,28 +220,28 @@
 name = "dyn-clone"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0d6ef0072f8a535281e4876be788938b528e9a1d43900b82c2569af7da799125"
 
 [[package]]
 name = "either"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
+checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
 
 [[package]]
 name = "enum_dispatch"
 version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa18ce2bc66555b3218614519ac839ddb759a7d6720732f979ef8d13be147ecd"
 dependencies = [
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.59",
 ]
 
 [[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
@@ -371,17 +373,17 @@
 name = "itoa"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "jobserver"
-version = "0.1.28"
+version = "0.1.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ab46a6e9526ddef3ae7f787c06f0f2600639ba80ea3eade3d8e670a2230f51d6"
+checksum = "685a7d121ee3f65ae4fddd72b25a04bb36b6af81bc0828f7d5434c0fe60fa3a2"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "js-sys"
 version = "0.3.69"
@@ -854,21 +856,23 @@
  "smartstring",
  "strum_macros",
  "version_check",
 ]
 
 [[package]]
 name = "polars-qt"
-version = "0.1.5"
+version = "0.1.6"
 dependencies = [
  "itertools",
  "polars",
  "pyo3",
  "pyo3-polars",
  "serde",
+ "tea-core 0.1.1 (git+https://github.com/Teamon9161/tevec.git?rev=4e89266)",
+ "tea_strategy",
 ]
 
 [[package]]
 name = "polars-row"
 version = "0.38.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "63029da56ff6a720b190490bbc7b6263f9b72d1134311b1f381fc8d306d37770"
@@ -928,17 +932,17 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.79"
+version = "1.0.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
+checksum = "a56dea16b0a29e94408b9aa5e2940a4eedbd128a1ba20e8f7ae60fd3d465af0e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.20.3"
@@ -982,28 +986,28 @@
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.59",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.59",
 ]
 
 [[package]]
 name = "pyo3-polars"
 version = "0.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c6ab8ad08494161085fb0d2d9de82c7fde7398da1778ee7e7a5a596ff4201f5b"
@@ -1026,15 +1030,15 @@
 checksum = "56c67d6b47b05d3827ef8e5f4449ae1a1861f5d7086ee18c5429e347b0d03c19"
 dependencies = [
  "polars-core",
  "polars-ffi",
  "polars-plan",
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.59",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
@@ -1199,15 +1203,15 @@
 name = "serde_derive"
 version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.59",
 ]
 
 [[package]]
 name = "simdutf8"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f27f6278552951f1f2b8cf9da965d10969b2efdea95a6ec47987ab46edfe263a"
@@ -1262,15 +1266,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23dc1fa9ac9c169a78ba62f0b841814b7abae11bdd047b9c58f893439e309ea0"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
  "rustversion",
- "syn 2.0.58",
+ "syn 2.0.59",
 ]
 
 [[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
@@ -1278,28 +1282,28 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.58"
+version = "2.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
+checksum = "4a6531ffc7b071655e4ce2e04bd464c4830bb585a61cabb96cf808f05172615a"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "sysinfo"
-version = "0.30.9"
+version = "0.30.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e9a84fe4cfc513b41cb2596b624e561ec9e7e1c4b46328e496ed56a53514ef2a"
+checksum = "26d7c217777061d5a2d652aea771fb9ba98b6dade657204b08c4b9604d11555b"
 dependencies = [
  "cfg-if",
  "core-foundation-sys",
  "libc",
  "ntapi",
  "once_cell",
  "windows",
@@ -1314,14 +1318,83 @@
 [[package]]
 name = "target-lexicon"
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
+name = "tea-core"
+version = "0.1.1"
+source = "git+https://github.com/Teamon9161/tevec.git?branch=master#4e89266ddddf077ded7e9804d5b04a0c1c872bd0"
+dependencies = [
+ "num-traits",
+ "polars",
+ "polars-arrow",
+ "serde",
+ "tea-dtype 0.1.1 (git+https://github.com/Teamon9161/tevec.git?branch=master)",
+]
+
+[[package]]
+name = "tea-core"
+version = "0.1.1"
+source = "git+https://github.com/Teamon9161/tevec.git?rev=4e89266#4e89266ddddf077ded7e9804d5b04a0c1c872bd0"
+dependencies = [
+ "num-traits",
+ "polars",
+ "polars-arrow",
+ "serde",
+ "tea-dtype 0.1.1 (git+https://github.com/Teamon9161/tevec.git?rev=4e89266)",
+]
+
+[[package]]
+name = "tea-dtype"
+version = "0.1.1"
+source = "git+https://github.com/Teamon9161/tevec.git?branch=master#4e89266ddddf077ded7e9804d5b04a0c1c872bd0"
+dependencies = [
+ "num-traits",
+ "tea-time",
+]
+
+[[package]]
+name = "tea-dtype"
+version = "0.1.1"
+source = "git+https://github.com/Teamon9161/tevec.git?rev=4e89266#4e89266ddddf077ded7e9804d5b04a0c1c872bd0"
+dependencies = [
+ "num-traits",
+]
+
+[[package]]
+name = "tea-rolling"
+version = "0.1.1"
+source = "git+https://github.com/Teamon9161/tevec.git?branch=master#4e89266ddddf077ded7e9804d5b04a0c1c872bd0"
+dependencies = [
+ "num-traits",
+ "tea-core 0.1.1 (git+https://github.com/Teamon9161/tevec.git?branch=master)",
+]
+
+[[package]]
+name = "tea-time"
+version = "0.1.1"
+source = "git+https://github.com/Teamon9161/tevec.git?branch=master#4e89266ddddf077ded7e9804d5b04a0c1c872bd0"
+dependencies = [
+ "chrono",
+]
+
+[[package]]
+name = "tea_strategy"
+version = "0.1.0"
+source = "git+https://github.com/Teamon9161/tea_strategy.git?rev=1d5db93#1d5db934079015e1329217603b374608aa993b41"
+dependencies = [
+ "itertools",
+ "serde",
+ "tea-core 0.1.1 (git+https://github.com/Teamon9161/tevec.git?branch=master)",
+ "tea-rolling",
+]
+
+[[package]]
 name = "thiserror"
 version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
 dependencies = [
  "thiserror-impl",
 ]
@@ -1330,15 +1403,15 @@
 name = "thiserror-impl"
 version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.59",
 ]
 
 [[package]]
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
@@ -1387,15 +1460,15 @@
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.59",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1409,15 +1482,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.59",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
@@ -1449,33 +1522,33 @@
 [[package]]
 name = "windows"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e48a53791691ab099e5e2ad123536d0fff50652600abaf43bbf952894110d0be"
 dependencies = [
  "windows-core",
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-core"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
 dependencies = [
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -1487,110 +1560,117 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.4",
- "windows_aarch64_msvc 0.52.4",
- "windows_i686_gnu 0.52.4",
- "windows_i686_msvc 0.52.4",
- "windows_x86_64_gnu 0.52.4",
- "windows_x86_64_gnullvm 0.52.4",
- "windows_x86_64_msvc 0.52.4",
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.4"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "xxhash-rust"
 version = "0.8.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "927da81e25be1e1a2901d59b81b37dd2efd1fc9c9345a55007f09bf5a2d3ee03"
 
@@ -1607,15 +1687,15 @@
 name = "zerocopy-derive"
 version = "0.7.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.59",
 ]
 
 [[package]]
 name = "zstd"
 version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2d789b1514203a1120ad2429eae43a7bd32b90976a7bb8a05f7ec02fa88cc23a"
```

### Comparing `polars_qt-0.1.5/pyproject.toml` & `polars_qt-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.5/PKG-INFO` & `polars_qt-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: polars-qt
-Version: 0.1.5
+Version: 0.1.6
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: polars >=0.20.16
 Author-email: Teamon9161 <teamon9161@163.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

