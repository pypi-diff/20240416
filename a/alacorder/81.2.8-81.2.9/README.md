# Comparing `tmp/alacorder-81.2.8.tar.gz` & `tmp/alacorder-81.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-81.2.8.tar", max compression
+gzip compressed data, was "alacorder-81.2.9.tar", max compression
```

## Comparing `alacorder-81.2.8.tar` & `alacorder-81.2.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1067 2023-04-18 14:01:34.633926 alacorder-81.2.8/LICENSE
--rw-r--r--   0        0        0     4828 2023-09-28 18:05:03.303177 alacorder-81.2.8/README.md
--rw-r--r--   0        0        0     5769 2023-09-28 16:21:15.145320 alacorder-81.2.8/alacorder/__init__.py
--rw-r--r--   0        0        0      759 2023-09-28 16:20:33.602586 alacorder-81.2.8/alacorder/__main__.py
--rwxr-xr-x   0        0        0   435126 2023-09-29 01:15:56.643057 alacorder-81.2.8/alacorder/alac.py
--rw-r--r--   0        0        0    35106 2023-09-28 13:19:12.784250 alacorder-81.2.8/alacorder/template.docx
--rw-r--r--   0        0        0     1061 2023-09-28 23:32:13.819108 alacorder-81.2.8/pyproject.toml
--rw-r--r--   0        0        0     5700 1970-01-01 00:00:00.000000 alacorder-81.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-18 14:01:34.633926 alacorder-81.2.9/LICENSE
+-rw-r--r--   0        0        0     4828 2023-09-28 18:05:03.303177 alacorder-81.2.9/README.md
+-rw-r--r--   0        0        0     5769 2023-09-28 16:21:15.145320 alacorder-81.2.9/alacorder/__init__.py
+-rw-r--r--   0        0        0      759 2023-09-28 16:20:33.602586 alacorder-81.2.9/alacorder/__main__.py
+-rwxr-xr-x   0        0        0   435636 2023-09-30 22:58:12.949837 alacorder-81.2.9/alacorder/alac.py
+-rw-r--r--   0        0        0    35106 2023-09-28 13:19:12.784250 alacorder-81.2.9/alacorder/template.docx
+-rw-r--r--   0        0        0     1070 2023-09-30 22:58:16.476281 alacorder-81.2.9/pyproject.toml
+-rw-r--r--   0        0        0     5700 1970-01-01 00:00:00.000000 alacorder-81.2.9/PKG-INFO
```

### Comparing `alacorder-81.2.8/LICENSE` & `alacorder-81.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-81.2.8/README.md` & `alacorder-81.2.9/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-81.2.8/alacorder/__init__.py` & `alacorder-81.2.9/alacorder/__init__.py`

 * *Files identical despite different names*

### Comparing `alacorder-81.2.8/alacorder/__main__.py` & `alacorder-81.2.9/alacorder/__main__.py`

 * *Files identical despite different names*

### Comparing `alacorder-81.2.8/alacorder/alac.py` & `alacorder-81.2.9/alacorder/alac.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,23 +18,23 @@
                 typer: 0.9.0+
                 xlsxwriter: 3.1.2+
                 xlsx2csv: 0.8.1+
                 Google Chrome: v75+
 """
 
 __author__ = "Sam Robson"
-__version__ = "81.2.8"
+__version__ = "81.2.9"
 
 import glob
 import locale
 import re
 import time
 from datetime import datetime
 from pathlib import Path
-from typing import Annotated, cast
+from typing import Annotated, Optional, cast
 
 import bs4
 import fitz
 import polars as pl
 import typer
 import xlsxwriter
 from docxtpl import DocxTemplate
@@ -2643,16 +2643,15 @@
         if isinstance(self._fees, pl.DataFrame):
             return self._fees
         if not self.is_read:
             self.read()
         assert isinstance(self.archive, pl.DataFrame)
         with console.status("Parsing fee sheets…"):
             df = (
-                self.archive.select("CaseNumber", "AllPagesText")
-                .select(
+                self.archive.select(
                     pl.col("CaseNumber"),
                     pl.col("AllPagesText")
                     .str.extract(r"(?s)Fee Sheet (.+Total:[^\n]+)")
                     .str.replace(
                         (
                             r"\s*\n\s*Admin Fee Balance Garnish Party Amount Due Fee"
                             r" Code Payor Amount Paid"
@@ -7512,14 +7511,15 @@
         write({"archive": out}, path, log=True)
         return out
 
     def write_summary_docs(
         self,
         pairs: str | Path | pl.DataFrame,
         output_dir: str | Path,
+        template_path: str | Path | None = None,
         include_ais: bool = False,
         include_dob: bool = True,
     ) -> None:
         """
         Create a docx summary in `output_dir` for each unique
         identifier in `pairs`.
         """
@@ -7553,15 +7553,19 @@
         )
 
         self.cases()
         self.disposition_charges()
         assert self._cases is not None
         assert self._disposition_charges is not None
 
-        doc = DocxTemplate(f"{Path(__file__).parent}/template.docx")
+        if template_path is None:
+            doc = DocxTemplate(f"{Path(__file__).parent}/template.docx")
+        else:
+            doc = DocxTemplate(template_path)
+
         locale.setlocale(locale.LC_ALL, "")  # set locale for number formatting
         progress_bar = Progress(*Progress.get_default_columns(), MofNCompleteColumn())
         with progress_bar as bar:
             for pair in bar.track(
                 pairs.iter_rows(named=True),
                 total=pairs.shape[0],
                 description="Writing…",
@@ -7605,15 +7609,15 @@
                 balance = "$" + locale.format_string(
                     "%.2f", cases["TotalBalance"].sum(), grouping=True
                 )
                 payment_to_restore = "$" + locale.format_string(
                     "%.2f",
                     (
                         charges.filter(pl.col("CERVConviction"))
-                        .unique("CaseNumber")["TotalBalance"]
+                        .unique("CaseNumber")["PaymentToRestore"]
                         .sum()
                     ),
                     grouping=True,
                 )
                 conviction_ct = str(charges.filter("Conviction").shape[0])
                 disq_conv_ct = str(
                     charges.filter(
@@ -8196,14 +8200,23 @@
     pairs: Annotated[
         Path, typer.Argument(help="Complete pairs template path.", show_default=False)
     ],
     output_dir: Annotated[
         Path,
         typer.Argument(help="Directory to write .docx files to.", show_default=False),
     ],
+    template: Annotated[
+        Optional[Path],
+        typer.Option(
+            "--template",
+            "-t",
+            help="Path to optional custom .docx template.",
+            show_default=False,
+        ),
+    ] = None,
     ais: Annotated[
         bool,
         typer.Option(
             "--ais / --no-ais", help="Include AIS # in output files.", show_default=True
         ),
     ] = False,
     dob: Annotated[
@@ -8214,15 +8227,17 @@
     ] = True,
 ) -> None:
     """
     Make .docx summaries with voting rights information for
     each unique identifier in `pairs` at `output_dir`.
     """
     cases = Cases(archive)
-    cases.write_summary_docs(pairs, output_dir, include_ais=ais, include_dob=dob)
+    cases.write_summary_docs(
+        pairs, output_dir, template_path=template, include_ais=ais, include_dob=dob
+    )
 
 
 @app.command(no_args_is_help=True)
 def autopair(
     archive: Annotated[
         Path,
         typer.Argument(
@@ -8285,36 +8300,39 @@
     assert isinstance(inmates, pl.DataFrame)
     if "Name" not in inmates.columns or "BirthYear" not in inmates.columns:
         msg = "One or more columns missing from `inmates_list`: 'Name', 'BirthYear'."
         raise Exception(msg)
 
     psr = read(party_search_results)
     assert isinstance(psr, pl.DataFrame)
-    if "Search" not in psr.columns:
+    if "Search" not in psr.columns or "DOB" not in psr.columns:
         msg = "'Search' column missing from `party_search_results`."
         raise Exception(msg)
 
     match psr["DOB"].dtype:
         case pl.Utf8:
             psr = psr.with_columns(
                 pl.col("DOB")
                 .str.extract(r"(\d\d\d\d)")
                 .cast(pl.Int64, strict=False)
                 .alias("ActualBirthYear")
             )
         case pl.Date:
             psr = psr.with_columns(pl.col("DOB").dt.year().alias("ActualBirthYear"))
+        case _:
+            msg = "DOB column must be string or date type."
+            raise Exception(msg)
 
-    psr = psr.with_columns(pl.col("Search").alias("NameMatch"))
     inmates = inmates.select(
         pl.col("Name").alias("NameMatch"),
         pl.col("BirthYear").alias("ExpectedBirthYear"),
     )
     psr = (
-        psr.join(inmates, on="NameMatch", how="left")
+        psr.with_columns(pl.col("Search").alias("NameMatch"))
+        .join(inmates, on="NameMatch", how="left")
         .filter(pl.col("ActualBirthYear") == pl.col("ExpectedBirthYear"))
         .select(pl.exclude("ActualBirthYear", "ExpectedBirthYear", "NameMatch"))
     )
     write({"filtered-party-search-results": psr}, output_path)
     return psr
```

### Comparing `alacorder-81.2.8/alacorder/template.docx` & `alacorder-81.2.9/alacorder/template.docx`

 * *Files identical despite different names*

### Comparing `alacorder-81.2.8/pyproject.toml` & `alacorder-81.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "81.2.8"
+version = "81.2.9"
 description = "Alacorder retrieves case detail PDFs from Alacourt.com and processes them into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 typer = {extras = ["all"], version = "^0.9.0"}
@@ -24,15 +24,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 select = ["B", "D", "E", "F", "I", "UP", "SIM", "FA", "ANN", "S", "C4", "EM", "RUF"]
 fixable = ["B", "E", "F", "I"]
-ignore = ["ANN101", "D212", "D205", "RUF001", "B008", "S101", "D400", "SIM102", "E711", "F403", "D415", "D203", "SIM105", "F401"]
+ignore = ["ANN101", "D212", "D205", "RUF001", "B008", "S101", "D400", "SIM102", "E711", "F403", "D415", "D203", "SIM105", "F401", "UP007"]
 line-length = 88
 target-version = "py310"
 
 [tool.black]
 line-length = 88
 preview = true
```

### Comparing `alacorder-81.2.8/PKG-INFO` & `alacorder-81.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 81.2.8
+Version: 81.2.9
 Summary: Alacorder retrieves case detail PDFs from Alacourt.com and processes them into data tables suitable for research purposes.
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

