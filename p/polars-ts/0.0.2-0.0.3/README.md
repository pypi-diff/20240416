# Comparing `tmp/polars_ts-0.0.2.tar.gz` & `tmp/polars_ts-0.0.3.tar.gz`

## Comparing `polars_ts-0.0.2.tar` & `polars_ts-0.0.3.tar`

### file list

```diff
@@ -1,36 +1,40 @@
--rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 polars_ts-0.0.2/Cargo.toml
--rw-r--r--   0     1001      127     3402 2024-04-08 15:15:12.000000 polars_ts-0.0.2/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0     1001      127     3107 2024-04-08 15:15:12.000000 polars_ts-0.0.2/.gitignore
--rw-r--r--   0     1001      127        7 2024-04-08 15:15:12.000000 polars_ts-0.0.2/.python-version
--rw-r--r--   0     1001      127      147 2024-04-08 15:15:12.000000 polars_ts-0.0.2/.vscode/settings.json
--rw-r--r--   0     1001      127    11357 2024-04-08 15:15:12.000000 polars_ts-0.0.2/LICENSE
--rw-r--r--   0     1001      127      709 2024-04-08 15:15:12.000000 polars_ts-0.0.2/Makefile
--rw-r--r--   0     1001      127     1002 2024-04-08 15:15:12.000000 polars_ts-0.0.2/README.md
--rw-r--r--   0     1001      127      861 2024-04-08 15:15:12.000000 polars_ts-0.0.2/polars_ts/__init__.py
--rw-r--r--   0     1001      127     2544 2024-04-08 15:15:12.000000 polars_ts-0.0.2/polars_ts/calendar.py
--rw-r--r--   0     1001      127      607 2024-04-08 15:15:12.000000 polars_ts-0.0.2/polars_ts/display.py
--rw-r--r--   0     1001      127     3732 2024-04-08 15:15:12.000000 polars_ts-0.0.2/polars_ts/dummy.py
--rw-r--r--   0     1001      127        0 2024-04-08 15:15:12.000000 polars_ts-0.0.2/polars_ts/expr/__init__.py
--rw-r--r--   0     1001      127     1580 2024-04-08 15:15:12.000000 polars_ts-0.0.2/polars_ts/expr/random.py
--rw-r--r--   0     1001      127      625 2024-04-08 15:15:12.000000 polars_ts-0.0.2/polars_ts/futures.py
--rw-r--r--   0     1001      127        0 2024-04-08 15:15:12.000000 polars_ts-0.0.2/polars_ts/futures_helper/__init__.py
--rw-r--r--   0     1001      127     6757 2024-04-08 15:15:12.000000 polars_ts-0.0.2/polars_ts/futures_helper/roll_calendar.py
--rw-r--r--   0     1001      127      556 2024-04-08 15:15:12.000000 polars_ts-0.0.2/polars_ts/futures_helper/util.py
--rw-r--r--   0     1001      127      483 2024-04-08 15:15:12.000000 polars_ts-0.0.2/polars_ts/helpers.py
--rw-r--r--   0     1001      127      910 2024-04-08 15:15:12.000000 polars_ts-0.0.2/polars_ts/resample.py
--rw-r--r--   0     1001      127     2142 2024-04-08 15:15:12.000000 polars_ts-0.0.2/polars_ts/sf.py
--rw-r--r--   0     1001      127     1202 2024-04-08 15:15:12.000000 polars_ts-0.0.2/polars_ts/time.py
--rw-r--r--   0     1001      127      324 2024-04-08 15:15:12.000000 polars_ts-0.0.2/polars_ts/tsf.py
--rw-r--r--   0     1001      127     1225 2024-04-08 15:15:12.000000 polars_ts-0.0.2/polars_ts/utils.py
--rw-r--r--   0     1001      127       32 2024-04-08 15:15:12.000000 polars_ts-0.0.2/requirements.txt
--rw-r--r--   0     1001      127      445 2024-04-08 15:15:12.000000 polars_ts-0.0.2/ruff.toml
--rw-r--r--   0     1001      127      212 2024-04-08 15:15:12.000000 polars_ts-0.0.2/run.py
--rw-r--r--   0     1001      127     2617 2024-04-08 15:15:12.000000 polars_ts-0.0.2/src/expressions.rs
--rw-r--r--   0     1001      127      385 2024-04-08 15:15:12.000000 polars_ts-0.0.2/src/lib.rs
--rw-r--r--   0     1001      127     1839 2024-04-08 15:15:12.000000 polars_ts-0.0.2/src/math/mod.rs
--rw-r--r--   0     1001      127     2712 2024-04-08 15:15:12.000000 polars_ts-0.0.2/src/utils.rs
--rw-r--r--   0     1001      127       27 2024-04-08 15:15:12.000000 polars_ts-0.0.2/tests/sf/test_sf.py
--rw-r--r--   0     1001      127      846 2024-04-08 15:15:12.000000 polars_ts-0.0.2/tests/test_rust_templates.py
--rw-r--r--   0     1001      127    34777 2024-04-08 15:15:12.000000 polars_ts-0.0.2/Cargo.lock
--rw-r--r--   0     1001      127      478 2024-04-08 15:15:12.000000 polars_ts-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1372 1970-01-01 00:00:00.000000 polars_ts-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 polars_ts-0.0.3/Cargo.toml
+-rw-r--r--   0     1001      127     3402 2024-04-14 23:41:19.000000 polars_ts-0.0.3/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0     1001      127     3107 2024-04-14 23:41:19.000000 polars_ts-0.0.3/.gitignore
+-rw-r--r--   0     1001      127        7 2024-04-14 23:41:19.000000 polars_ts-0.0.3/.python-version
+-rw-r--r--   0     1001      127      147 2024-04-14 23:41:19.000000 polars_ts-0.0.3/.vscode/settings.json
+-rw-r--r--   0     1001      127    11357 2024-04-14 23:41:19.000000 polars_ts-0.0.3/LICENSE
+-rw-r--r--   0     1001      127      704 2024-04-14 23:41:19.000000 polars_ts-0.0.3/Makefile
+-rw-r--r--   0     1001      127     1002 2024-04-14 23:41:19.000000 polars_ts-0.0.3/README.md
+-rw-r--r--   0     1001      127      933 2024-04-14 23:41:19.000000 polars_ts-0.0.3/polars_ts/__init__.py
+-rw-r--r--   0     1001      127     2918 2024-04-14 23:41:19.000000 polars_ts-0.0.3/polars_ts/calendar.py
+-rw-r--r--   0     1001      127      638 2024-04-14 23:41:19.000000 polars_ts-0.0.3/polars_ts/display.py
+-rw-r--r--   0     1001      127     3853 2024-04-14 23:41:19.000000 polars_ts-0.0.3/polars_ts/dummy.py
+-rw-r--r--   0     1001      127     2089 2024-04-14 23:41:19.000000 polars_ts-0.0.3/polars_ts/dummymkt.py
+-rw-r--r--   0     1001      127        0 2024-04-14 23:41:19.000000 polars_ts-0.0.3/polars_ts/expr/__init__.py
+-rw-r--r--   0     1001      127     1580 2024-04-14 23:41:19.000000 polars_ts-0.0.3/polars_ts/expr/random.py
+-rw-r--r--   0     1001      127     2852 2024-04-14 23:41:19.000000 polars_ts-0.0.3/polars_ts/futures.py
+-rw-r--r--   0     1001      127        0 2024-04-14 23:41:19.000000 polars_ts-0.0.3/polars_ts/futures_helper/__init__.py
+-rw-r--r--   0     1001      127      850 2024-04-14 23:41:19.000000 polars_ts-0.0.3/polars_ts/futures_helper/bbg_symbols.py
+-rw-r--r--   0     1001      127     1135 2024-04-14 23:41:19.000000 polars_ts-0.0.3/polars_ts/futures_helper/generic_symbols.py
+-rw-r--r--   0     1001      127     7757 2024-04-14 23:41:19.000000 polars_ts-0.0.3/polars_ts/futures_helper/roll_calendar.py
+-rw-r--r--   0     1001      127      890 2024-04-14 23:41:19.000000 polars_ts-0.0.3/polars_ts/futures_helper/util.py
+-rw-r--r--   0     1001      127      483 2024-04-14 23:41:19.000000 polars_ts-0.0.3/polars_ts/helpers.py
+-rw-r--r--   0     1001      127      437 2024-04-14 23:41:19.000000 polars_ts-0.0.3/polars_ts/loader.py
+-rw-r--r--   0     1001      127      930 2024-04-14 23:41:19.000000 polars_ts-0.0.3/polars_ts/resample.py
+-rw-r--r--   0     1001      127     2168 2024-04-14 23:41:19.000000 polars_ts-0.0.3/polars_ts/sf.py
+-rw-r--r--   0     1001      127     1211 2024-04-14 23:41:19.000000 polars_ts-0.0.3/polars_ts/time.py
+-rw-r--r--   0     1001      127      324 2024-04-14 23:41:19.000000 polars_ts-0.0.3/polars_ts/tsf.py
+-rw-r--r--   0     1001      127     1289 2024-04-14 23:41:19.000000 polars_ts-0.0.3/polars_ts/utils.py
+-rw-r--r--   0     1001      127       32 2024-04-14 23:41:19.000000 polars_ts-0.0.3/requirements.txt
+-rw-r--r--   0     1001      127      445 2024-04-14 23:41:19.000000 polars_ts-0.0.3/ruff.toml
+-rw-r--r--   0     1001      127      212 2024-04-14 23:41:19.000000 polars_ts-0.0.3/run.py
+-rw-r--r--   0     1001      127     2617 2024-04-14 23:41:19.000000 polars_ts-0.0.3/src/expressions.rs
+-rw-r--r--   0     1001      127      385 2024-04-14 23:41:19.000000 polars_ts-0.0.3/src/lib.rs
+-rw-r--r--   0     1001      127     1839 2024-04-14 23:41:19.000000 polars_ts-0.0.3/src/math/mod.rs
+-rw-r--r--   0     1001      127     2712 2024-04-14 23:41:19.000000 polars_ts-0.0.3/src/utils.rs
+-rw-r--r--   0     1001      127       27 2024-04-14 23:41:19.000000 polars_ts-0.0.3/tests/sf/test_sf.py
+-rw-r--r--   0     1001      127      846 2024-04-14 23:41:19.000000 polars_ts-0.0.3/tests/test_rust_templates.py
+-rw-r--r--   0     1001      127    34777 2024-04-14 23:41:19.000000 polars_ts-0.0.3/Cargo.lock
+-rw-r--r--   0     1001      127      478 2024-04-14 23:41:19.000000 polars_ts-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1372 1970-01-01 00:00:00.000000 polars_ts-0.0.3/PKG-INFO
```

### Comparing `polars_ts-0.0.2/Cargo.toml` & `polars_ts-0.0.3/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "polars-ts"
-version = "0.0.2"
+version = "0.0.3"
 edition = "2021"
 
 [lib]
 name = "polars_ts"
 crate-type= ["cdylib"]
 
 [dependencies]
```

### Comparing `polars_ts-0.0.2/.github/workflows/publish_to_pypi.yml` & `polars_ts-0.0.3/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.2/.gitignore` & `polars_ts-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.2/LICENSE` & `polars_ts-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.2/Makefile` & `polars_ts-0.0.3/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 	unset CONDA_PREFIX && \
 	source .venv/bin/activate && maturin develop --release
 
 pre-commit: .venv
 	cargo fmt --all && cargo clippy --all-features
 	.venv/bin/python -m ruff check . --fix --exit-non-zero-on-fix
 	.venv/bin/python -m ruff format polars_ts tests
-	echo .venv/bin/mypy polars_ts tests
+	.venv/bin/mypy polars_ts tests
 
 test: .venv
 	.venv/bin/python -m pytest tests
 
 run: install
 	source .venv/bin/activate && python run.py
```

### Comparing `polars_ts-0.0.2/README.md` & `polars_ts-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.2/polars_ts/__init__.py` & `polars_ts-0.0.3/polars_ts/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,20 +4,24 @@
 from typing import TYPE_CHECKING
 
 import polars as pl
 
 from .display import *
 from .sf import *
 from .tsf import *
+from .loader import *
 from .time import *
 from .dummy import *
 from .resample import *
 
 from .calendar import *
 from .futures import *
+from .dummymkt import *
+
+pl.enable_string_cache()
 
 
 if TYPE_CHECKING:
     from polars.type_aliases import IntoExpr
 
 
 def pig_latinnify(expr: IntoExpr) -> pl.Expr:
```

### Comparing `polars_ts-0.0.2/polars_ts/calendar.py` & `polars_ts-0.0.3/polars_ts/calendar.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,76 +1,86 @@
-from typing import Optional, Union
+from typing import Optional
 
 import polars as pl
+from polars.type_aliases import IntoExpr
 
 from .sf import SeriesFrame
-from .futures_helper.util import month_to_imm
+from .futures_helper.util import month_to_imm_dict
+from .utils import parse_into_expr
 
 
 __NAMESPACE = "calendar"
 
 
 @pl.api.register_lazyframe_namespace(__NAMESPACE)
 class CalendarFrame(SeriesFrame):
     def __init__(self, df: pl.LazyFrame):
         super().__init__(df)
 
     def date_to_imm_contract(
         self,
-        col_name: str,
-        contract_code: Union[pl.Expr, str] = "",
+        col_name: IntoExpr,
+        prefix: IntoExpr = pl.lit(""),
+        suffix: IntoExpr = pl.lit(""),
         out: Optional[str] = None,
-    ) -> pl.Expr:
-        imm_dict = month_to_imm(as_dict=True)
-        out = col_name if out is None else out
-        contract_code = (
-            pl.lit(contract_code) if isinstance(contract_code, str) else contract_code
-        )
+    ) -> pl.LazyFrame:
+        col_expr = parse_into_expr(col_name)
+        prefix = parse_into_expr(prefix)
+        suffix = parse_into_expr(suffix)
+        out = col_expr.meta.output_name() if out is None else out
 
+        imm_dict = month_to_imm_dict()
         self._df = self._df.with_columns(
-            pl.concat_str(
-                [
-                    contract_code,
-                    pl.struct(
-                        pl.col(col_name).dt.month().alias("month"),
-                        pl.col(col_name).dt.strftime("%y").alias("year"),
-                    ).map_elements(
-                        lambda se: f"{imm_dict[int(se['month'])]}{se['year']}",
-                        return_dtype=pl.String,
-                    ),
-                ]
-            ).alias(out)
+            pl.when(col_expr.is_null())
+            .then(pl.lit(None).cast(pl.String))
+            .otherwise(
+                pl.concat_str(
+                    [
+                        prefix,
+                        pl.struct(
+                            col_expr.dt.month().alias("month"),
+                            col_expr.dt.strftime("%y").alias("year"),
+                        ).map_elements(
+                            lambda se: f"""{imm_dict.get(se['month'], "@@")}{se['year']}""",
+                            return_dtype=pl.String,
+                        ),
+                        suffix,
+                    ]
+                )
+            )
+            .cast(pl.Categorical)
+            .alias(out)
         )
 
         return self.result_df
 
-    def imm_contract_to_date(self, col_name: str, default_day: int = 1) -> pl.Expr:
-        imm_dict = month_to_imm(as_dict=True, invert=True)
+    def imm_contract_to_date(self, col_name: str, default_day: int = 1) -> pl.LazyFrame:
+        imm_dict = month_to_imm_dict(invert=True)
         self._df = self._df.with_columns(
             pl.col(col_name)
             .str.extract_groups(".*(?<imm>[F-Z])(?<year>[0-9]{2})")
             .map_elements(
                 lambda se: (
                     f"{str(default_day).rjust(2, '0')}-{str(imm_dict[se['imm']]).rjust(2, '0')}-{se['year']}"
                 ),
                 return_dtype=pl.String,
             )
             .str.to_date("%d-%m-%y")
         )
 
         return self.result_df
 
-    def int_to_date(self, col_name: str) -> pl.Expr:
+    def int_to_date(self, col_name: str) -> pl.LazyFrame:
         self._df = self._df.with_columns(
             pl.col(col_name).cast(pl.String).str.strptime(pl.Date, "%Y%m%d")
         )
 
         return self.result_df
 
-    def date_to_int(self, col_name: str, out: Optional[str] = None) -> pl.Expr:
+    def date_to_int(self, col_name: str, out: Optional[str] = None) -> pl.LazyFrame:
         out = col_name if out is None else out
 
         self._df = self._df.with_columns(
             (
                 (pl.col(col_name).dt.year() * 10000)
                 + (pl.col(col_name).dt.month().cast(pl.UInt16) * 100)
                 + (pl.col(col_name).dt.day())
```

### Comparing `polars_ts-0.0.2/polars_ts/display.py` & `polars_ts-0.0.3/polars_ts/display.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,10 +14,10 @@
 
         cols = time_col + category_cols
 
         return oldrepr(
             self.select(*[pl.col(c) for c in cols], pl.exclude(cols)), **kwargs
         )
 
-    pl.DataFrame._repr_html_ = newrepr
+    pl.DataFrame._repr_html_ = newrepr  # type: ignore[method-assign]
 
     repr_overloaded = [1]
```

### Comparing `polars_ts-0.0.2/polars_ts/dummy.py` & `polars_ts-0.0.3/polars_ts/dummy.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Union, Literal, Mapping
+from typing import List, Union, Literal, Mapping, Optional
 
 import polars as pl
 
 from .sf import SeriesFrame
 from .expr.random import (
     random_normal as rand_normal,
     random_uniform as rand_uniform,
@@ -15,20 +15,20 @@
 @pl.api.register_lazyframe_namespace(__NAMESPACE)
 class DummyFrame(SeriesFrame):
     def __init__(self, df: pl.LazyFrame):
         super().__init__(df)
 
     def random_category_subgroups(
         self,
-        prefix: pl.Expr,
+        prefix: Union[str, pl.Expr],
         sizes: List[int],
         *,
-        max_num_subgroups: int = None,
+        max_num_subgroups: Optional[int] = None,
         seed: int = 42,
-        partition: Mapping[Literal["by", "but"], List[str]] = None,
+        partition: Optional[Mapping[Literal["by", "but"], List[str]]] = None,
         out: str = "subgroup",
     ) -> pl.LazyFrame:
         split = self.auto_partition(partition)
 
         if max_num_subgroups is None:
             max_num_subgroups = (
                 self._df.select(1 + (pl.len() // max(sizes))).collect().item(0, 0)
@@ -59,15 +59,15 @@
         return self.result_df
 
     def random_uniform(
         self,
         lower: Union[pl.Expr, float] = 0.0,
         upper: Union[pl.Expr, float] = 1.0,
         *,
-        partition: Mapping[Literal["by", "but"], List[str]] = None,
+        partition: Optional[Mapping[Literal["by", "but"], List[str]]] = None,
         out: str = "value",
     ) -> pl.LazyFrame:
         split = self.auto_partition(partition)
         self._df = self._df.with_columns(
             rand_uniform(lower, upper, seed=wyhash(pl.concat_str(split).first()))
             .over(split)
             .alias(out)
@@ -79,15 +79,15 @@
         return self.result_df
 
     def random_normal(
         self,
         mu: Union[pl.Expr, float] = 0.0,
         sigma: Union[pl.Expr, float] = 1.0,
         *,
-        partition: Mapping[Literal["by", "but"], List[str]] = None,
+        partition: Optional[Mapping[Literal["by", "but"], List[str]]] = None,
         out: str = "value",
     ) -> pl.LazyFrame:
         split = self.auto_partition(partition)
         self._df = self._df.with_columns(
             rand_normal(mu, sigma, seed=wyhash(pl.concat_str(split).first()))
             .over(split)
             .alias(out)
@@ -96,20 +96,22 @@
         return self.result_df
 
     def enum(
         self, names: Union[List[str], int], *, out: str = "category", prefix="ENUM_"
     ) -> pl.LazyFrame:
         if isinstance(names, int):
             names_expr = (
-                pl.int_ranges(0, 100, eager=True)
+                pl.int_ranges(0, 100)
                 .cast(pl.List(pl.Utf8))
                 .list.eval(pl.element().str.replace("^", prefix))
                 .alias(out)
             )
-            enum_dtype = pl.Enum(names_expr.explode().to_list())
+            enum_dtype = pl.Enum(
+                pl.DataFrame().with_columns(names_expr.explode()).to_series().to_list()
+            )
 
         else:
             names_expr = pl.lit(names).alias(out)
             enum_dtype = pl.Enum(names)
 
         # random nulls
```

### Comparing `polars_ts-0.0.2/polars_ts/expr/random.py` & `polars_ts-0.0.3/polars_ts/expr/random.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.2/polars_ts/futures_helper/roll_calendar.py` & `polars_ts-0.0.3/polars_ts/futures_helper/roll_calendar.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,57 @@
 import polars as pl
 
-from .util import month_to_imm
+from .util import month_to_imm_dict, make_generic_contract
 
 
-def load_roll_config(filename: str) -> pl.LazyFrame:
-    return pl.scan_csv(filename)
+def guess_security_meta(
+    generic_contracts: pl.LazyFrame, roll_config: pl.LazyFrame
+) -> pl.LazyFrame:
+    df = (
+        roll_config.join(generic_contracts, on="asset")
+        .filter(
+            pl.col("priced_roll_cycle").str.contains(
+                pl.col("instrument_id").struct.field("tenor").cast(pl.String)
+            )
+        )
+        .with_columns(
+            expiry_date=(
+                pl.col("time")
+                .dt.month_start()
+                .dt.offset_by(pl.col("approximate_expiry_offset").cast(pl.String))
+                .dt.date()
+            )
+        )
+        .select(
+            "asset",
+            "instrument_id",
+            fut_first_trade_dt=_guess_fut_first_trade_dt(pl.col("expiry_date")),
+            last_tradeable_dt="expiry_date",
+            fut_notice_first="expiry_date",
+        )
+        .unique(maintain_order=True)
+    )
+
+    return df
+
+
+def _guess_fut_first_trade_dt(
+    expiry_date: pl.Expr, min_trade_days: str = "-2y", buffer_days: str = "-30d"
+) -> pl.Expr:
+    first_trade_dt = pl.min_horizontal(
+        (
+            expiry_date.dt.month_start()
+            .dt.offset_by(pl.col("approximate_expiry_offset").cast(pl.String))
+            .dt.offset_by(pl.col("roll_offset").cast(pl.String))
+            .dt.offset_by(buffer_days)
+        ),
+        (expiry_date.dt.offset_by(min_trade_days)),
+    )
+
+    return first_trade_dt
 
 
 def asset_carry_contracts(roll_config: pl.LazyFrame) -> pl.LazyFrame:
     def _find_carry_month(hc: dict):
         allowed_contracts = hc["priced_roll_cycle"]
         current_contract = hc["hold_roll_cycle"]
         carry_offset = hc["carry_contract_offset"]
@@ -19,28 +62,28 @@
 
         return carry_imm_month
 
     return (
         roll_config.select(
             "asset",
             "carry_contract_offset",
-            pl.col("hold_roll_cycle").str.extract_all("[F-Z]"),
-            pl.col("priced_roll_cycle"),
+            pl.col("hold_roll_cycle").cast(pl.String).str.extract_all("[F-Z]"),
+            pl.col("priced_roll_cycle").cast(pl.String),
         )
         .explode("hold_roll_cycle")
         .with_columns(
             hold_month=pl.col("hold_roll_cycle")
-            .replace(month_to_imm(as_dict=True, invert=True))
+            .replace(month_to_imm_dict(invert=True))
             .cast(pl.Int8),
             carry_month=(
                 pl.struct(
                     "hold_roll_cycle", "carry_contract_offset", "priced_roll_cycle"
                 )
                 .map_elements(_find_carry_month, return_dtype=pl.String)
-                .replace(month_to_imm(as_dict=True, invert=True))
+                .replace(month_to_imm_dict(invert=True))
                 .cast(pl.Int8)
             ),
         )
         .with_columns(carry_month_offset=pl.col("carry_month") - pl.col("hold_month"))
         .with_columns(
             carry_month_offset=(
                 pl.concat_str(
@@ -65,27 +108,29 @@
     )
 
 
 def asset_near_far_contracts(roll_config: pl.LazyFrame) -> pl.LazyFrame:
     return (
         roll_config.select(
             "asset",
-            hold_near=pl.col("hold_roll_cycle").str.extract_all("[F-Z]"),
+            hold_near=pl.col("hold_roll_cycle")
+            .cast(pl.String)
+            .str.extract_all("[F-Z]"),
             hold_far=pl.concat_str(
-                pl.col("hold_roll_cycle").str.slice(1),
-                pl.col("hold_roll_cycle").str.slice(0, 1),
+                pl.col("hold_roll_cycle").cast(pl.String).str.slice(1),
+                pl.col("hold_roll_cycle").cast(pl.String).str.slice(0, 1),
             ).str.extract_all("[F-Z]"),
         )
         .explode("hold_near", "hold_far")
         .with_columns(
             hold_near_month=pl.col("hold_near")
-            .replace(month_to_imm(as_dict=True, invert=True))
+            .replace(month_to_imm_dict(invert=True))
             .cast(pl.Int8),
             hold_far_month=pl.col("hold_far")
-            .replace(month_to_imm(as_dict=True, invert=True))
+            .replace(month_to_imm_dict(invert=True))
             .cast(pl.Int8),
         )
         .with_columns(
             hold_far_month_offset=pl.col("hold_far_month") - pl.col("hold_near_month"),
         )
         .with_columns(
             pl.concat_str(
@@ -111,90 +156,84 @@
         )
         .select(
             "asset", "hold_near_month", "hold_far_month_offset", "carry_month_offset"
         )
     )
 
 
-def roll_calendar_time_grid(
-    roll_config: pl.LazyFrame, start_date, end_date
+def create_roll_calendar_helper(
+    roll_config: pl.LazyFrame, security_dates: pl.LazyFrame, include_debug: bool
 ) -> pl.LazyFrame:
-    start_end = (
-        roll_config.select(
-            asof_date_offset=pl.lit(start_date)
-            - (
-                pl.lit(start_date)
-                .dt.offset_by(pl.col("roll_offset"))
-                .dt.offset_by(pl.col("expiry_offset"))
-                .min()
-            )
-        )
-        .select(
-            start_date=pl.lit(start_date),
-            end_date=pl.lit(end_date) + pl.col("asof_date_offset"),
+    result_schema = [
+        "roll_date",
+        "asset",
+        "near_contract",
+        "far_contract",
+        "carry_contract",
+    ]
+
+    if include_debug:
+        result_schema.extend(
+            [
+                "has_instruments",
+            ]
         )
-        .collect()
-    )
-
-    start_end = list(start_end.iter_rows())[0]
-    start_end
-    time_grid = pl.LazyFrame().time.range(start_end[0], start_end[1])
 
-    return time_grid
+    imm2mo_dict = month_to_imm_dict(invert=True)
 
-
-def create_roll_calendars(
-    roll_config: pl.LazyFrame, start_date, end_date
-) -> pl.LazyFrame:
-    time_grid = roll_calendar_time_grid(roll_config, start_date, end_date)
-    return (
-        time_grid.join(
-            roll_config.select("asset", "expiry_offset", "roll_offset"), how="cross"
+    df = (
+        roll_config.join(security_dates, on="asset", how="left")
+        .select(
+            "asset",
+            "instrument_id",
+            "expiry_date",
+            has_instruments=pl.col("expiry_date").is_not_null(),
+            roll_date=(
+                pl.col("expiry_date").dt.offset_by(
+                    pl.col("roll_offset").cast(pl.String)
+                )
+            ),
         )
-        .with_columns(near_expiry_date=pl.lit(None).cast(pl.Date))
         .with_columns(
-            near_expiry_date=(
-                pl.when(pl.col("near_expiry_date").is_null()).then(
-                    # approximate expriy date
-                    pl.col("time")
-                    .dt.month_start()
-                    .dt.offset_by(pl.col("expiry_offset"))
-                    .dt.date()
-                )
+            hold_near_month=(
+                pl.col("instrument_id")
+                .struct.field("tenor")
+                .cast(pl.String)
+                .replace(imm2mo_dict)
+                .cast(pl.Int8)
             )
         )
-        .unique(subset=["asset", "near_expiry_date"], keep="first", maintain_order=True)
+        .join(
+            asset_contracts(roll_config), on=["asset", "hold_near_month"], how="inner"
+        )
         .with_columns(
-            roll_date=(
-                pl.col("near_expiry_date").dt.offset_by(pl.col("roll_offset")).dt.date()
-            )
+            pl.col("hold_near_month", "hold_far_month_offset", "carry_month_offset")
+            .backward_fill()
+            .over("asset")
         )
-        .with_columns(hold_near_month=pl.col("near_expiry_date").dt.month())
-        .join(asset_contracts(roll_config), on=["asset", "hold_near_month"], how="left")
-        .with_columns(pl.col("^hold_(near|far).*$").backward_fill().over("asset"))
         .with_columns(
-            near_contract=pl.date(
-                pl.col("near_expiry_date").dt.year(), pl.col("hold_near_month"), 1
+            near_contract_dt=pl.date(
+                pl.col("expiry_date").dt.year(), pl.col("hold_near_month"), 1
             )
         )
         .with_columns(
-            far_contract=pl.col("near_contract").dt.offset_by(
-                pl.col("hold_far_month_offset")
+            far_contract_dt=pl.col("near_contract_dt").dt.offset_by(
+                pl.col("hold_far_month_offset").cast(pl.String)
             )
         )
         .with_columns(
-            carry_contract=pl.col("near_contract").dt.offset_by(
-                pl.col("carry_month_offset")
+            carry_contract_dt=pl.col("near_contract_dt").dt.offset_by(
+                pl.col("carry_month_offset").cast(pl.String)
             )
         )
-        .select(
-            "roll_date",
-            "asset",
-            "near_contract",
-            "near_expiry_date",
-            "far_contract",
-            "carry_contract",
+        .with_columns(
+            near_contract=make_generic_contract("near_contract_dt"),
+            far_contract=make_generic_contract("far_contract_dt"),
+            carry_contract=make_generic_contract("carry_contract_dt"),
         )
-        .drop_nulls()
-        .filter(pl.col("roll_date") <= end_date)
+        .select(result_schema)
         .sort("asset", "roll_date")
+        # TODO: change this to drop nulls at end of table
+        .drop_nulls()
     )
+
+    return df
```

### Comparing `polars_ts-0.0.2/polars_ts/resample.py` & `polars_ts-0.0.3/polars_ts/resample.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Literal, Mapping
+from typing import List, Literal, Mapping, Optional
 
 import polars as pl
 
 from .tsf import TimeSeriesFrame
 
 __NAMESPACE = "rs"
 
@@ -12,15 +12,15 @@
     def __init__(self, df: pl.LazyFrame):
         super().__init__(df)
 
     def to_ohlc(
         self,
         period: str,
         *,
-        partition: Mapping[Literal["by", "but"], List[str]] = None,
+        partition: Optional[Mapping[Literal["by", "but"], List[str]]] = None,
         value_col: str = "value",
     ) -> pl.LazyFrame:
         split = self.auto_partition(partition)
 
         self._df = (
             self._df.sort("time")
             .group_by_dynamic("time", every=period, group_by=split)
```

### Comparing `polars_ts-0.0.2/polars_ts/sf.py` & `polars_ts-0.0.3/polars_ts/sf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Iterable, List, Mapping, Literal
+from typing import Iterable, List, Mapping, Literal, Union
 
 import polars as pl
 
 __NAMESPACE = "sf"
 
 
 @pl.api.register_lazyframe_namespace(__NAMESPACE)
@@ -31,25 +31,23 @@
     def values(self) -> pl.LazyFrame:
         return self._df.select(self.value_names())
 
     def categories(self) -> pl.LazyFrame:
         return self._df.select(pl.col(pl.Categorical, pl.Enum))
 
     def ht(self, nrows=3) -> pl.LazyFrame:
-        if len(self._df) <= (nrows + nrows):
-            return self._df
-
-        return pl.concat([self._df.head(nrows), self._df.tail(nrows)])
+        return pl.concat([self._df.head(nrows), self._df.tail(nrows)]).unique()
 
     def common_category_names(self, rhs: pl.LazyFrame) -> List[str]:
-        return sorted(set(self.category_names()).intersection(rhs.sf.category_names()))
+        rhs_categories = rhs.sf.category_names()  # type: ignore[attr-defined]
+        return sorted(set(self.category_names()).intersection(rhs_categories))
 
     def auto_partition(
         self,
-        partition: Mapping[Literal["by", "but"], List[str]],
+        partition: Union[Mapping[Literal["by", "but"], List[str]] | None],
     ) -> List[str]:
         cols = set(self.categories().columns).difference(["time"])
         if partition is not None:
             if len(set(partition.keys()).intersection(["by", "but"])) > 1:
                 raise ValueError("Must specify 'by' xor 'but'")
 
             if "by" in partition:
```

### Comparing `polars_ts-0.0.2/polars_ts/time.py` & `polars_ts-0.0.3/polars_ts/time.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,18 +28,18 @@
                 .list.unique()
                 .list.sort()
             )
         )
 
         return self.expand(interval)
 
-    def expand(self, interval: str = "1d") -> pl.Series:
+    def expand(self, interval: str = "1d") -> pl.LazyFrame:
         # pre: every row has a time: list[date] column
         # xdt doesnt support date_ranges?
         # fn = xdt.date_range if interval.endswith('bd') else pl.date_ranges
         fn = pl.date_ranges
 
         self._df = self._df.with_columns(
             fn(pl.col("time").list.min(), pl.col("time").list.max(), interval)
         ).explode("time")
 
-        return self._df
+        return self.result_df
```

### Comparing `polars_ts-0.0.2/polars_ts/utils.py` & `polars_ts-0.0.3/polars_ts/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,11 +38,13 @@
     """
     if isinstance(expr, pl.Expr):
         pass
     elif isinstance(expr, str) and not str_as_lit:
         expr = pl.col(expr)
     elif isinstance(expr, list) and not list_as_lit:
         expr = pl.lit(pl.Series(expr), dtype=dtype)
+    elif isinstance(expr, dict):
+        expr = pl.struct(expr)
     else:
         expr = pl.lit(expr, dtype=dtype)
 
     return expr
```

### Comparing `polars_ts-0.0.2/src/expressions.rs` & `polars_ts-0.0.3/src/expressions.rs`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.2/src/math/mod.rs` & `polars_ts-0.0.3/src/math/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.2/src/utils.rs` & `polars_ts-0.0.3/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.2/tests/test_rust_templates.py` & `polars_ts-0.0.3/tests/test_rust_templates.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.2/Cargo.lock` & `polars_ts-0.0.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -669,15 +669,15 @@
  "polars-arrow",
  "polars-error",
  "polars-utils",
 ]
 
 [[package]]
 name = "polars-ts"
-version = "0.0.2"
+version = "0.0.3"
 dependencies = [
  "jemallocator",
  "polars",
  "pyo3",
  "pyo3-polars",
  "rand",
  "rand_distr",
```

### Comparing `polars_ts-0.0.2/PKG-INFO` & `polars_ts-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.3
 Name: polars-ts
-Version: 0.0.2
-Requires-Dist: polars >=0.20.18
+Version: 0.0.3
+Requires-Dist: polars >=0.20.20
 Requires-Dist: polars-xdt
 Requires-Dist: hvplot
 Requires-Dist: pyarrow
 Requires-Dist: hvplot ; extra == 'dev'
 Requires-Dist: pyarrow ; extra == 'dev'
 Provides-Extra: dev
 License-File: LICENSE
```

