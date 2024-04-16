# Comparing `tmp/ssb_arbmark_fagfunksjoner-0.0.8.tar.gz` & `tmp/ssb_arbmark_fagfunksjoner-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_arbmark_fagfunksjoner-0.0.8.tar", max compression
+gzip compressed data, was "ssb_arbmark_fagfunksjoner-0.0.9.tar", max compression
```

## Comparing `ssb_arbmark_fagfunksjoner-0.0.8.tar` & `ssb_arbmark_fagfunksjoner-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1073 2024-02-22 15:02:23.916463 ssb_arbmark_fagfunksjoner-0.0.8/LICENSE
--rw-r--r--   0        0        0     3260 2024-02-22 15:02:23.916463 ssb_arbmark_fagfunksjoner-0.0.8/README.md
--rw-r--r--   0        0        0     3698 2024-02-22 15:02:34.804578 ssb_arbmark_fagfunksjoner-0.0.8/pyproject.toml
--rw-r--r--   0        0        0       55 2024-02-22 15:02:23.920463 ssb_arbmark_fagfunksjoner-0.0.8/src/ssb_arbmark_fagfunksjoner/__init__.py
--rw-r--r--   0        0        0      263 2024-02-22 15:02:23.920463 ssb_arbmark_fagfunksjoner-0.0.8/src/ssb_arbmark_fagfunksjoner/__main__.py
--rw-r--r--   0        0        0    23978 2024-02-22 15:02:34.804578 ssb_arbmark_fagfunksjoner-0.0.8/src/ssb_arbmark_fagfunksjoner/functions.py
--rw-r--r--   0        0        0    22829 2024-02-22 15:02:34.804578 ssb_arbmark_fagfunksjoner-0.0.8/src/ssb_arbmark_fagfunksjoner/groups.py
--rw-r--r--   0        0        0        0 2024-02-22 15:02:23.920463 ssb_arbmark_fagfunksjoner-0.0.8/src/ssb_arbmark_fagfunksjoner/py.typed
--rw-r--r--   0        0        0     4576 1970-01-01 00:00:00.000000 ssb_arbmark_fagfunksjoner-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-02-29 07:01:26.307740 ssb_arbmark_fagfunksjoner-0.0.9/LICENSE
+-rw-r--r--   0        0        0     3260 2024-02-29 07:01:26.307740 ssb_arbmark_fagfunksjoner-0.0.9/README.md
+-rw-r--r--   0        0        0     3726 2024-02-29 07:01:36.559748 ssb_arbmark_fagfunksjoner-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0       55 2024-02-29 07:01:26.311740 ssb_arbmark_fagfunksjoner-0.0.9/src/ssb_arbmark_fagfunksjoner/__init__.py
+-rw-r--r--   0        0        0      263 2024-02-29 07:01:26.311740 ssb_arbmark_fagfunksjoner-0.0.9/src/ssb_arbmark_fagfunksjoner/__main__.py
+-rw-r--r--   0        0        0    23856 2024-02-29 07:01:36.559748 ssb_arbmark_fagfunksjoner-0.0.9/src/ssb_arbmark_fagfunksjoner/functions.py
+-rw-r--r--   0        0        0    20925 2024-02-29 07:01:36.559748 ssb_arbmark_fagfunksjoner-0.0.9/src/ssb_arbmark_fagfunksjoner/groups.py
+-rw-r--r--   0        0        0        0 2024-02-29 07:01:26.311740 ssb_arbmark_fagfunksjoner-0.0.9/src/ssb_arbmark_fagfunksjoner/py.typed
+-rw-r--r--   0        0        0     4626 1970-01-01 00:00:00.000000 ssb_arbmark_fagfunksjoner-0.0.9/PKG-INFO
```

### Comparing `ssb_arbmark_fagfunksjoner-0.0.8/LICENSE` & `ssb_arbmark_fagfunksjoner-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_arbmark_fagfunksjoner-0.0.8/README.md` & `ssb_arbmark_fagfunksjoner-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ssb_arbmark_fagfunksjoner-0.0.8/pyproject.toml` & `ssb_arbmark_fagfunksjoner-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-arbmark-fagfunksjoner"
-version = "0.0.8"
+version = "0.0.9"
 description = "SSB Arbeidsmarked og lønn Fag-fellesfunksjoner"
 authors = ["Jan Sebastian Rothe <jsr@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/ssb-arbmark-fagfunksjoner"
 repository = "https://github.com/statisticsnorway/ssb-arbmark-fagfunksjoner"
 documentation = "https://statisticsnorway.github.io/ssb-arbmark-fagfunksjoner"
@@ -21,14 +21,15 @@
 nox = "^2023.4.22"
 pandas = ">=1.5.3"
 numpy = "^1.26.2"
 holidays = "^0.37"
 pandas-stubs = "^2.1.1.230928"
 poetry-plugin-export = "^1.6.0"
 dapla-toolbelt = "^2.0.6"
+ssb-klass-python = "^0.0.9"
 
 [tool.poetry.group.dev.dependencies]
 pygments = ">=2.10.0"
 black = { extras = ["jupyter"], version = ">=23.1.0" }
 coverage = { extras = ["toml"], version = ">=6.2" }
 darglint = ">=1.8.1"
 furo = ">=2021.11.12"
```

### Comparing `ssb_arbmark_fagfunksjoner-0.0.8/src/ssb_arbmark_fagfunksjoner/functions.py` & `ssb_arbmark_fagfunksjoner-0.0.9/src/ssb_arbmark_fagfunksjoner/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -566,39 +566,32 @@
 
     # Define the pattern to search for files based on the provided name and file type
     file_name_pattern = f"{name}*{dottype}"
 
     # Join directory and file name
     file_path = os.path.join(path, file_name_pattern)
 
-    # Checking environment
-    wenv = os.environ.get("DAPLA_REGION")
-
-    # If environment is Dapla
-    if wenv == "BIP":
+    # If path is a google cloud bucket
+    if path[:4] in ["ssb-", "gs:/"]:
 
         # Get filesystem
         fs = FileClient.get_gcs_file_system()
 
         # Use glob to find all files matching the pattern
         file_list = fs.glob(file_path)
 
     else:
 
         # Use glob to find all files matching the pattern
         file_list = glob.glob(file_path)
 
-    # Sorting key based on file modification time
+    # Sorting key based on file version
     file_versions = sorted(
         file_list,
-        key=lambda x: (
-            os.path.getmtime(x),
-            # Fallback to filename sorting
-            x,
-        ),
+        key=lambda x: int(x.split("_v")[-1].split(".")[0]),
     )
 
     # Check if any files were found. If not, inform the user and return None
     if not file_versions:
         print("No files found.")
         return None
```

### Comparing `ssb_arbmark_fagfunksjoner-0.0.8/src/ssb_arbmark_fagfunksjoner/groups.py` & `ssb_arbmark_fagfunksjoner-0.0.9/src/ssb_arbmark_fagfunksjoner/groups.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 # Numpy for data wrangling
 import numpy as np
 import numpy.typing as npt
 
 # Pandas for table management
 import pandas as pd
 
+# Klass for standard classifications
+from klass.classes.variant import KlassVariant
+
 if TYPE_CHECKING:
     PdSeriesInt = pd.Series[int]  # type: ignore[misc]
     PdSeriesStr = pd.Series[str]  # type: ignore[misc]
     NpArrayInt = npt.NDArray[np.int_]  # type: ignore[misc]
     NpArrayStr = npt.NDArray[np.str_]  # type: ignore[misc]
 else:
     PdSeriesInt = pd.Series
@@ -266,101 +269,49 @@
     else:
         results = [f"{key} {value}" for key, value in groups.items()]
         default_code = "99 Uoppgitt"
     grouped = np.select(conditions, results, default=default_code)
     return grouped
 
 
-def nace_sn07_17grp(nace_sn07: PdSeriesStr, display: str = "label") -> NpArrayStr:
-    """Categorize a pandas Series of NACE-codes (SN07) into predefined groups.
+def nace_to_17_groups(nace: PdSeriesStr, label: bool = False) -> PdSeriesStr:
+    """Converts NACE codes in a Pandas Series to their corresponding group codes or labels.
+
+    NACE (Nomenclature of Economic Activities) is the European industry standard classification system.
+    This function maps NACE codes to a higher-level group (level 2) and optionally returns the group's name instead of its code.
 
     Parameters:
-        nace_sn07: A pandas Series containing the NACE-codes.
-        display: If 'label', returns group labels; if 'number', returns keys;
-                       for any other string, returns a combination of keys and labels.
+        nace: A Pandas Series containing NACE codes.
+        label: If True, returns the names of the groups instead of their codes. Defaults to False.
 
     Returns:
-        A numpy Array where the original NACE-codes are replaced by group labels or keys.
-    """
-    # Split the series by space and take the first part
-    first_parts = nace_sn07.str.split(" ", n=1).str[0]
-
-    # Check if the maximum length of the first parts exceeds 2
-    max_length = first_parts.str.len().max()
+        A Pandas Series with the mapped group codes or names, depending on the 'label' argument.
 
-    # Check if nace codes are already grouped into 47-groups
-    if max_length > 2:
-        print(
-            "Warning: The function first groups the input into the 47 groups standard."
-        )
-        nace_str2_np = pd.to_numeric(nace_sn07_47grp(nace_sn07, "number"))
-    else:
-        # Convert series to numpy array
-        nace_str2_np = pd.to_numeric(first_parts).to_numpy()
-
-    # Define the conditions for each group
-    conditions = [
-        (nace_str2_np == 1),  # 01-03 Jordbruk, skogbruk og fiske
-        np.isin(nace_str2_np, [2, 3]),  # 05-09 Bergverksdrift og utvinning
-        np.logical_and(nace_str2_np >= 4, nace_str2_np <= 16),  # 10-33 Industri
-        np.isin(nace_str2_np, [17, 18]),  # 35-39 Elektrisitet, vann og renovasjon
-        (nace_str2_np == 19),  # 41-43 Bygge- og anleggsvirksomhet
-        np.isin(
-            nace_str2_np, [20, 21, 22]
-        ),  # 45-47 Varehandel, reparasjon av motorvogner
-        np.logical_and(
-            nace_str2_np >= 23, nace_str2_np <= 27
-        ),  # 49-53 Transport og lagring
-        np.isin(nace_str2_np, [28, 29]),  # 55-56 Overnattings- og serveringsvirksomhet
-        np.isin(nace_str2_np, [30, 31]),  # 58-63 Informasjon og kommunikasjon
-        np.isin(nace_str2_np, [32, 33, 34]),  # 64-66 Finansiering og forsikring
-        np.logical_and(
-            nace_str2_np >= 35, nace_str2_np <= 38
-        ),  # 68-75 Teknisk tjenesteyting, eiendomsdrift
-        (nace_str2_np == 39),  # 77-82 Forretningsmessig tjenesteyting
-        (nace_str2_np == 40),  # 84 Off.adm., forsvar, sosialforsikring
-        (nace_str2_np == 41),  # 85 Undervisning
-        np.isin(nace_str2_np, [42, 43]),  # 86-88 Helse- og sosialtjenester
-        np.logical_and(
-            nace_str2_np >= 44, nace_str2_np <= 47
-        ),  # 90-99 Personlig tjenesteyting
-    ]
-
-    # Define the group labels with string keys
-    groups = {
-        "01-03": "Jordbruk, skogbruk og fiske",
-        "05-09": "Bergverksdrift og utvinning",
-        "10-33": "Industri",
-        "35-39": "Elektrisitet, vann og renovasjon",
-        "41-43": "Bygge- og anleggsvirksomhet",
-        "45-47": "Varehandel, reparasjon av motorvogner",
-        "49-53": "Transport og lagring",
-        "55-56": "Overnattings- og serveringsvirksomhet",
-        "58-63": "Informasjon og kommunikasjon",
-        "64-66": "Finansiering og forsikring",
-        "68-75": "Teknisk tjenesteyting, eiendomsdrift",
-        "77-82": "Forretningsmessig tjenesteyting",
-        "84": "Off.adm., forsvar, sosialforsikring",
-        "85": "Undervisning",
-        "86-88": "Helse- og sosialtjenester",
-        "90-99": "Personlig tjenesteyting",
-    }
-
-    # Determine and apply the selected format based on the labels parameter
-    if display == "label":
-        results = [str(value) for value in groups.values()]
-        default_code = "Uoppgitt"
-    elif display == "number":
-        results = [str(key) for key in groups.keys()]
-        default_code = "999"
+    Note:
+        The function relies on a predefined mapping ('KlassVariant(1616).data') to perform the conversion.
+        It assumes that this mapping has a specific structure, with 'level', 'code', and 'parentCode' (or 'name' if labels are requested) columns.
+    """
+    # Retrieve the predefined mapping data for NACE codes
+    kv = KlassVariant("1616").data
+    # Filter the mapping to include only level 2 categories
+    kv_level = kv.query('level == "2"')
+    # Create a mapping dictionary from NACE codes to their parent codes
+    mapping = kv_level.set_index("code").to_dict()
+    # Map the first two characters of each NACE code in the input series to their corresponding group codes
+    nace_groups = nace.str[0:2].map(mapping["parentCode"])
+
+    if label:
+        # If labels are requested, create a mapping for NACE code names at level 1
+        kv_label = kv.query('level == "1"')
+        mapping_label = kv_label.set_index("code").to_dict()
+        # Map the group codes to their names, filling in 'Uoppgitt' for any missing mappings
+        return nace_groups.map(mapping_label["name"]).fillna("Uoppgitt")
     else:
-        results = [f"{key} {value}" for key, value in groups.items()]
-        default_code = "999 Uoppgitt"
-    grouped = np.select(conditions, results, default=default_code)
-    return grouped
+        # If labels are not requested, return the group codes directly
+        return nace_groups
 
 
 def sektor2_grp(
     sektor: PdSeriesStr, undersektor: PdSeriesStr, display: str = "label"
 ) -> NpArrayStr:
     """Categorize a pandas Series of sectors and subsectors into predefined groups.
```

### Comparing `ssb_arbmark_fagfunksjoner-0.0.8/PKG-INFO` & `ssb_arbmark_fagfunksjoner-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssb-arbmark-fagfunksjoner
-Version: 0.0.8
+Version: 0.0.9
 Summary: SSB Arbeidsmarked og lønn Fag-fellesfunksjoner
 Home-page: https://github.com/statisticsnorway/ssb-arbmark-fagfunksjoner
 License: MIT
 Author: Jan Sebastian Rothe
 Author-email: jsr@ssb.no
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -19,14 +19,15 @@
 Requires-Dist: holidays (>=0.37,<0.38)
 Requires-Dist: nox (>=2023.4.22,<2024.0.0)
 Requires-Dist: numpy (>=1.26.2,<2.0.0)
 Requires-Dist: pandas (>=1.5.3)
 Requires-Dist: pandas-stubs (>=2.1.1.230928,<3.0.0.0)
 Requires-Dist: pipx (>=1.3.2,<2.0.0)
 Requires-Dist: poetry-plugin-export (>=1.6.0,<2.0.0)
+Requires-Dist: ssb-klass-python (>=0.0.9,<0.0.10)
 Project-URL: Changelog, https://github.com/statisticsnorway/ssb-arbmark-fagfunksjoner/releases
 Project-URL: Documentation, https://statisticsnorway.github.io/ssb-arbmark-fagfunksjoner
 Project-URL: Repository, https://github.com/statisticsnorway/ssb-arbmark-fagfunksjoner
 Description-Content-Type: text/markdown
 
 # SSB Arbeidsmarked og lønn Fag-fellesfunksjoner
```

