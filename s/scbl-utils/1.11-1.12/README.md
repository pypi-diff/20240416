# Comparing `tmp/scbl_utils-1.11.tar.gz` & `tmp/scbl_utils-1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scbl_utils-1.11.tar", max compression
+gzip compressed data, was "scbl_utils-1.12.tar", max compression
```

## Comparing `scbl_utils-1.11.tar` & `scbl_utils-1.12.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1079 2023-12-14 16:32:13.627049 scbl_utils-1.11/LICENSE
--rw-r--r--   0        0        0     8239 2024-01-23 19:13:12.443282 scbl_utils-1.11/README.md
--rw-r--r--   0        0        0      995 2024-03-27 18:02:18.227885 scbl_utils-1.11/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-14 16:32:13.628638 scbl_utils-1.11/scbl_utils/__init__.py
--rw-r--r--   0        0        0     8720 2024-03-05 16:41:07.480949 scbl_utils-1.11/scbl_utils/main.py
--rw-r--r--   0        0        0     7527 2024-03-27 18:02:48.976351 scbl_utils-1.11/scbl_utils/utils/defaults.py
--rw-r--r--   0        0        0     8982 2023-12-14 19:20:55.237861 scbl_utils-1.11/scbl_utils/utils/gdrive.py
--rw-r--r--   0        0        0    14379 2024-03-27 17:51:34.920949 scbl_utils-1.11/scbl_utils/utils/samplesheet.py
--rw-r--r--   0        0        0     4049 2023-12-14 16:32:13.629985 scbl_utils-1.11/scbl_utils/utils/validate.py
--rw-r--r--   0        0        0     9353 1970-01-01 00:00:00.000000 scbl_utils-1.11/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-12-14 16:32:13.627049 scbl_utils-1.12/LICENSE
+-rw-r--r--   0        0        0     8239 2024-01-23 19:13:12.443282 scbl_utils-1.12/README.md
+-rw-r--r--   0        0        0      995 2024-04-16 14:32:04.774493 scbl_utils-1.12/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-14 16:32:13.628638 scbl_utils-1.12/scbl_utils/__init__.py
+-rw-r--r--   0        0        0     8792 2024-04-16 14:23:51.980931 scbl_utils-1.12/scbl_utils/main.py
+-rw-r--r--   0        0        0     7527 2024-03-27 18:02:48.976351 scbl_utils-1.12/scbl_utils/utils/defaults.py
+-rw-r--r--   0        0        0     8982 2023-12-14 19:20:55.237861 scbl_utils-1.12/scbl_utils/utils/gdrive.py
+-rw-r--r--   0        0        0    14379 2024-03-27 17:51:34.920949 scbl_utils-1.12/scbl_utils/utils/samplesheet.py
+-rw-r--r--   0        0        0     4049 2023-12-14 16:32:13.629985 scbl_utils-1.12/scbl_utils/utils/validate.py
+-rw-r--r--   0        0        0     9353 1970-01-01 00:00:00.000000 scbl_utils-1.12/PKG-INFO
```

### Comparing `scbl_utils-1.11/LICENSE` & `scbl_utils-1.12/LICENSE`

 * *Files identical despite different names*

### Comparing `scbl_utils-1.11/README.md` & `scbl_utils-1.12/README.md`

 * *Files identical despite different names*

### Comparing `scbl_utils-1.11/pyproject.toml` & `scbl_utils-1.12/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scbl-utils"
-version = "1.11"
+version = "1.12"
 description = "A set of command-line utilities that facilitate data processing at the Single Cell Biology Lab at the Jackson Laboratory."
 authors = ["Ahmed Said <ahmed.said@jax.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/TheJacksonLaboratory/scbl-utils/"
 documentation = "https://github.com/TheJacksonLaboratory/scbl-utils/"
```

### Comparing `scbl_utils-1.11/scbl_utils/main.py` & `scbl_utils-1.12/scbl_utils/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,15 @@
     ][0]
     multiplexing_df = trackingsheet.to_df(
         sheet_id=multiplexing_sheet_id,
         col_renaming=multiplexing_spec['columns'],
         header_row=multiplexing_spec['header_row'],
         to_join=multiplexing_spec['join'],
     )
+    multiplexing_df['libraries'] = multiplexing_df['libraries'].ffill()
 
     # Filter df and fill with available information
     # # TODO: after the filtration, everything can be wrapped into a
     # function called "fill" or something
     samplesheet_df = tracking_df[tracking_df['libraries'].isin(lib_to_fastqdir.keys())].copy()  # type: ignore
     samplesheet_df['design'] = samplesheet_df['libraries'].apply(
         get_design, multiplexing_df=multiplexing_df
```

### Comparing `scbl_utils-1.11/scbl_utils/utils/defaults.py` & `scbl_utils-1.12/scbl_utils/utils/defaults.py`

 * *Files identical despite different names*

### Comparing `scbl_utils-1.11/scbl_utils/utils/gdrive.py` & `scbl_utils-1.12/scbl_utils/utils/gdrive.py`

 * *Files identical despite different names*

### Comparing `scbl_utils-1.11/scbl_utils/utils/samplesheet.py` & `scbl_utils-1.12/scbl_utils/utils/samplesheet.py`

 * *Files identical despite different names*

### Comparing `scbl_utils-1.11/scbl_utils/utils/validate.py` & `scbl_utils-1.12/scbl_utils/utils/validate.py`

 * *Files identical despite different names*

### Comparing `scbl_utils-1.11/PKG-INFO` & `scbl_utils-1.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scbl-utils
-Version: 1.11
+Version: 1.12
 Summary: A set of command-line utilities that facilitate data processing at the Single Cell Biology Lab at the Jackson Laboratory.
 Home-page: https://github.com/TheJacksonLaboratory/scbl-utils/
 License: MIT
 Author: Ahmed Said
 Author-email: ahmed.said@jax.org
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
```

