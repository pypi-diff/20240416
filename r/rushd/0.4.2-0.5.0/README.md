# Comparing `tmp/rushd-0.4.2.tar.gz` & `tmp/rushd-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rushd-0.4.2.tar", last modified: Thu Jul 27 22:21:58 2023, max compression
+gzip compressed data, was "rushd-0.5.0.tar", last modified: Mon Apr 15 23:16:04 2024, max compression
```

## Comparing `rushd-0.4.2.tar` & `rushd-0.5.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 kaseylove   (501) staff       (20)        0 2023-07-27 22:21:58.528868 rushd-0.4.2/
--rw-r--r--   0 kaseylove   (501) staff       (20)     1069 2022-01-21 15:10:03.000000 rushd-0.4.2/LICENSE
--rw-r--r--   0 kaseylove   (501) staff       (20)     3962 2023-07-27 22:21:58.528437 rushd-0.4.2/PKG-INFO
--rw-r--r--   0 kaseylove   (501) staff       (20)     2994 2023-07-27 21:59:34.000000 rushd-0.4.2/README.md
--rw-r--r--   0 kaseylove   (501) staff       (20)      527 2023-03-01 18:01:20.000000 rushd-0.4.2/pyproject.toml
--rw-r--r--   0 kaseylove   (501) staff       (20)       38 2023-07-27 22:21:58.528993 rushd-0.4.2/setup.cfg
--rw-r--r--   0 kaseylove   (501) staff       (20)     1885 2023-07-27 22:21:23.000000 rushd-0.4.2/setup.py
-drwxr-xr-x   0 kaseylove   (501) staff       (20)        0 2023-07-27 22:21:58.510642 rushd-0.4.2/src/
-drwxr-xr-x   0 kaseylove   (501) staff       (20)        0 2023-07-27 22:21:58.517656 rushd-0.4.2/src/rushd/
--rw-r--r--   0 kaseylove   (501) staff       (20)      651 2023-07-26 21:44:53.000000 rushd-0.4.2/src/rushd/__init__.py
--rw-r--r--   0 kaseylove   (501) staff       (20)    15035 2023-07-26 21:44:53.000000 rushd-0.4.2/src/rushd/flow.py
--rw-r--r--   0 kaseylove   (501) staff       (20)    11323 2023-07-26 21:44:53.000000 rushd-0.4.2/src/rushd/io.py
--rw-r--r--   0 kaseylove   (501) staff       (20)     9791 2023-07-27 21:47:05.000000 rushd-0.4.2/src/rushd/plot.py
--rw-r--r--   0 kaseylove   (501) staff       (20)     6268 2023-07-26 21:44:53.000000 rushd-0.4.2/src/rushd/well_mapper.py
-drwxr-xr-x   0 kaseylove   (501) staff       (20)        0 2023-07-27 22:21:58.522591 rushd-0.4.2/src/rushd.egg-info/
--rw-r--r--   0 kaseylove   (501) staff       (20)     3962 2023-07-27 22:21:58.000000 rushd-0.4.2/src/rushd.egg-info/PKG-INFO
--rw-r--r--   0 kaseylove   (501) staff       (20)      440 2023-07-27 22:21:58.000000 rushd-0.4.2/src/rushd.egg-info/SOURCES.txt
--rw-r--r--   0 kaseylove   (501) staff       (20)        1 2023-07-27 22:21:58.000000 rushd-0.4.2/src/rushd.egg-info/dependency_links.txt
--rw-r--r--   0 kaseylove   (501) staff       (20)      210 2023-07-27 22:21:58.000000 rushd-0.4.2/src/rushd.egg-info/requires.txt
--rw-r--r--   0 kaseylove   (501) staff       (20)        6 2023-07-27 22:21:58.000000 rushd-0.4.2/src/rushd.egg-info/top_level.txt
-drwxr-xr-x   0 kaseylove   (501) staff       (20)        0 2023-07-27 22:21:58.527781 rushd-0.4.2/tests/
--rw-r--r--   0 kaseylove   (501) staff       (20)    11898 2023-03-01 18:01:20.000000 rushd-0.4.2/tests/test_file_io.py
--rw-r--r--   0 kaseylove   (501) staff       (20)     3607 2023-03-01 18:01:20.000000 rushd-0.4.2/tests/test_file_moi.py
--rw-r--r--   0 kaseylove   (501) staff       (20)    18337 2023-03-01 18:03:58.000000 rushd-0.4.2/tests/test_flow.py
--rw-r--r--   0 kaseylove   (501) staff       (20)      891 2023-03-01 18:01:20.000000 rushd-0.4.2/tests/test_pandas_cache.py
--rw-r--r--   0 kaseylove   (501) staff       (20)     5431 2023-07-27 17:35:52.000000 rushd-0.4.2/tests/test_plot.py
--rw-r--r--   0 kaseylove   (501) staff       (20)     3274 2023-03-01 18:01:20.000000 rushd-0.4.2/tests/test_well_mapper.py
+drwxr-xr-x   0 christopher  (1000) christopher  (1000)        0 2024-04-15 23:16:04.317502 rushd-0.5.0/
+-rw-r--r--   0 christopher  (1000) christopher  (1000)     1069 2022-08-30 19:04:22.000000 rushd-0.5.0/LICENSE
+-rw-r--r--   0 christopher  (1000) christopher  (1000)     5267 2024-04-15 23:16:04.317502 rushd-0.5.0/PKG-INFO
+-rw-r--r--   0 christopher  (1000) christopher  (1000)     3562 2024-04-15 23:12:39.000000 rushd-0.5.0/README.md
+-rw-r--r--   0 christopher  (1000) christopher  (1000)      527 2023-02-02 22:08:57.000000 rushd-0.5.0/pyproject.toml
+-rw-r--r--   0 christopher  (1000) christopher  (1000)       38 2024-04-15 23:16:04.317502 rushd-0.5.0/setup.cfg
+-rw-r--r--   0 christopher  (1000) christopher  (1000)     1958 2024-04-15 23:12:34.000000 rushd-0.5.0/setup.py
+drwxr-xr-x   0 christopher  (1000) christopher  (1000)        0 2024-04-15 23:16:04.310835 rushd-0.5.0/src/
+drwxr-xr-x   0 christopher  (1000) christopher  (1000)        0 2024-04-15 23:16:04.310835 rushd-0.5.0/src/rushd/
+-rw-r--r--   0 christopher  (1000) christopher  (1000)      651 2023-04-19 21:24:37.000000 rushd-0.5.0/src/rushd/__init__.py
+-rw-r--r--   0 christopher  (1000) christopher  (1000)    15897 2024-04-15 20:16:32.000000 rushd-0.5.0/src/rushd/flow.py
+-rw-r--r--   0 christopher  (1000) christopher  (1000)    11336 2024-04-15 19:14:31.000000 rushd-0.5.0/src/rushd/io.py
+-rw-r--r--   0 christopher  (1000) christopher  (1000)    13305 2024-04-15 23:02:42.000000 rushd-0.5.0/src/rushd/plot.py
+-rw-r--r--   0 christopher  (1000) christopher  (1000)     6268 2023-06-08 19:55:12.000000 rushd-0.5.0/src/rushd/well_mapper.py
+drwxr-xr-x   0 christopher  (1000) christopher  (1000)        0 2024-04-15 23:16:04.314168 rushd-0.5.0/src/rushd.egg-info/
+-rw-r--r--   0 christopher  (1000) christopher  (1000)     5267 2024-04-15 23:16:04.000000 rushd-0.5.0/src/rushd.egg-info/PKG-INFO
+-rw-r--r--   0 christopher  (1000) christopher  (1000)      440 2024-04-15 23:16:04.000000 rushd-0.5.0/src/rushd.egg-info/SOURCES.txt
+-rw-r--r--   0 christopher  (1000) christopher  (1000)        1 2024-04-15 23:16:04.000000 rushd-0.5.0/src/rushd.egg-info/dependency_links.txt
+-rw-r--r--   0 christopher  (1000) christopher  (1000)      218 2024-04-15 23:16:04.000000 rushd-0.5.0/src/rushd.egg-info/requires.txt
+-rw-r--r--   0 christopher  (1000) christopher  (1000)        6 2024-04-15 23:16:04.000000 rushd-0.5.0/src/rushd.egg-info/top_level.txt
+drwxr-xr-x   0 christopher  (1000) christopher  (1000)        0 2024-04-15 23:16:04.314168 rushd-0.5.0/tests/
+-rw-r--r--   0 christopher  (1000) christopher  (1000)    12242 2024-04-15 19:15:26.000000 rushd-0.5.0/tests/test_file_io.py
+-rw-r--r--   0 christopher  (1000) christopher  (1000)     3607 2023-02-02 22:12:16.000000 rushd-0.5.0/tests/test_file_moi.py
+-rw-r--r--   0 christopher  (1000) christopher  (1000)    19979 2024-04-15 20:16:33.000000 rushd-0.5.0/tests/test_flow.py
+-rw-r--r--   0 christopher  (1000) christopher  (1000)      891 2023-02-02 22:12:16.000000 rushd-0.5.0/tests/test_pandas_cache.py
+-rw-r--r--   0 christopher  (1000) christopher  (1000)     8458 2024-04-15 23:12:18.000000 rushd-0.5.0/tests/test_plot.py
+-rw-r--r--   0 christopher  (1000) christopher  (1000)     3274 2023-02-02 22:12:16.000000 rushd-0.5.0/tests/test_well_mapper.py
```

### Comparing `rushd-0.4.2/LICENSE` & `rushd-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rushd-0.4.2/PKG-INFO` & `rushd-0.5.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: rushd
-Version: 0.4.2
-Summary: Package for maintaining robust, reproducible data management.
-Home-page: https://github.com/GallowayLabMIT/rushd
-Author: Christopher Johnstone, Kasey Love, Conrad Oakes
-Author-email: meson800@gmail.com
-Project-URL: Bug Tracker, https://github.com/GallowayLabMIT/rushd/issues
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Utilities
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # rushd
 [![Stable documentation](https://img.shields.io/badge/Documentation-stable-blue)](https://gallowaylabmit.github.io/rushd/en/main/)
 [![PyPI-downloads](https://img.shields.io/pypi/dm/rushd)](https://pypi.org/project/rushd)
 [![PyPI-version](https://img.shields.io/pypi/v/rushd)](https://pypi.org/project/rushd)
 [![PyPI-license](https://img.shields.io/pypi/l/rushd)](https://pypi.org/project/rushd)
 [![Supported python versions](https://img.shields.io/pypi/pyversions/rushd)](https://pypi.org/project/rushd)
 [![codecov](https://codecov.io/gh/GallowayLabMIT/rushd/branch/main/graph/badge.svg?token=ALaU8lQxt5)](https://codecov.io/gh/GallowayLabMIT/rushd)
@@ -60,28 +36,36 @@
 ```
 you can create a local virtual environment, and install `rushd` in "development (editable) mode"
 with the extra requirements for tests.
 ```
 $ python -m venv env
 $ .\env\Scripts\activate    (on Windows)
 $ source env/bin/activate   (on Mac/Linux)
-$ pip install -e .[dev]
+$ pip install -e .[dev]     (on most shells)
+$ pip install -e '.[dev]'   (on zsh)
 ```
 After this 'local install', you can use and import `rushd` freely without
 having to re-install after each update.
 
 ## Changelog
 See the [CHANGELOG](CHANGELOG.md) for detailed changes.
 ```
-## [0.4.2] - 2023-07-27
+## [0.5.0] - 2024-04-15
 ### Added
-- `rd.plot.generate_xticklabels` replaces a plot's existing xticklabels with specified metadata in a table-like format
-## [0.4.1] - 2023-06-27
+- Added new `rd.plot.debug_axes` which draws guide lines to help with axis alignment.
+- Added new `rd.plot.adjust_subplot_margins_inches` which allows subplot configuring
+  using inch offsets (instead of subfigure coordinate offsets)
+
 ### Modified
-- Updated the `rd.plot.plot_mapping` command to properly handle the single-numeric case.
+- `rd.flow.load_csv_with_metadata` and
+  `rd.flow.load_groups_with_metadata` can now load a subset of columns.
+- The `datadir.txt` can include paths that use `~` to represent the home directory.
+- `rd.plot.generate_xticklabels` does not include metadata key labels in plots without yticklabels
+- `rd.plot.generate_xticklabels` no longer throws an error when xticklabels don't match the dictionary passed (instead leaves labels as-is)
+- `rd.plot.generate_xticklabels` now enables user-specified line spacing
 ```
 
 ## License
 This is licensed by the MIT license. Use freely!
 
 ## What does the name mean?
 The name is a reference to [Ibn Rushd](https://en.wikipedia.org/wiki/Averroes), a Muslim scholar born in Córdoba who was responsible for translating and adding scholastic commentary to ancient Greek works, especially Aristotle. His translations spurred further translations into Latin and Hebrew, reigniting interest in ancient Greek works for the first time since the fall of the Roman empire.
```

### Comparing `rushd-0.4.2/pyproject.toml` & `rushd-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rushd-0.4.2/setup.py` & `rushd-0.5.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rushd",
-    version="0.4.2",
+    version="0.5.0",
     author="Christopher Johnstone, Kasey Love, Conrad Oakes",
     author_email="meson800@gmail.com",
     description="Package for maintaining robust, reproducible data management.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/GallowayLabMIT/rushd",
     project_urls={
@@ -26,14 +26,15 @@
         "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering",
         "Topic :: Utilities",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
@@ -50,14 +51,15 @@
             "pyarrow",
             "pytest",
             "pytest-pep8",
             "pytest-cov",
             "pytest-mock",
             "pre-commit",
             "ruff",
+            "seaborn",
             "build",
             "twine",
             "sphinx",
             "sphinx-rtd-theme",
             "sphinx-autodoc-typehints",
         ]
     },
```

### Comparing `rushd-0.4.2/src/rushd/__init__.py` & `rushd-0.5.0/src/rushd/__init__.py`

 * *Files identical despite different names*

### Comparing `rushd-0.4.2/src/rushd/flow.py` & `rushd-0.5.0/src/rushd/flow.py`

 * *Files 10% similar despite different names*

```diff
@@ -75,15 +75,19 @@
                     MetadataWarning,
                     stacklevel=2,
                 )
     return {k: well_mapper.well_mapping(v) for k, v in metadata["metadata"].items()}
 
 
 def load_csv_with_metadata(
-    data_path: Union[str, Path], yaml_path: Union[str, Path], filename_regex: Optional[str] = None
+    data_path: Union[str, Path],
+    yaml_path: Union[str, Path],
+    filename_regex: Optional[str] = None,
+    *,
+    columns: Optional[List[str]] = None,
 ) -> pd.DataFrame:
     """
     Load .csv data into DataFrame with associated metadata.
 
     Generates a pandas DataFrame from a set of .csv files located at the given path,
     adding columns for metadata encoded by a given .yaml file. Metadata is associated
     with the data based on well IDs encoded in the data filenames.
@@ -96,14 +100,18 @@
         Path to .yaml file to use for associating metadata with well IDs.
         All metadata must be contained under the header 'metadata'.
     filename_regex: str or raw str (optional)
         Regular expression to use to extract well IDs from data filenames.
         Must contain the capturing group 'well' for the sample well IDs.
         If not included, the filenames are assumed to follow this format (default
         export format from FlowJo): 'export_[well]_[population].csv'
+    columns: Optional list of strings
+        If specified, only the specified columns are loaded out of the CSV files.
+        This can drastically reduce the amount of memory required to load
+        flow data.
 
     Returns
     -------
     A single pandas DataFrame containing all data with associated metadata.
     """
     if not isinstance(data_path, Path):
         data_path = Path(data_path)
@@ -125,16 +133,21 @@
         regex = re.compile(filename_regex)
         if "well" not in regex.groupindex:
             raise RegexError("Regular expression does not contain capturing group 'well'")
         match = regex.match(file.name)
         if match is None:
             continue
 
-        # Load data
-        df = pd.read_csv(file)
+        # Load the first row so we get the column names
+        df_onerow = pd.read_csv(file, nrows=1)
+        # Load data: we allow extra columns in our column list, so subset it
+        valid_cols = (
+            list(set(columns).intersection(set(df_onerow.columns))) if columns is not None else None
+        )
+        df = pd.read_csv(file, usecols=valid_cols)
 
         # Add metadata to DataFrame
         well = match.group("well")
         index = 0
         for k, v in metadata_map.items():
             # Replace custom metadata keys with <NA> if not present
             df.insert(index, k, v[well] if well in v else [pd.NA] * len(df))
@@ -155,14 +168,16 @@
     return data
 
 
 def load_groups_with_metadata(
     groups_df: pd.DataFrame,
     base_path: Optional[Union[str, Path]] = "",
     filename_regex: Optional[str] = None,
+    *,
+    columns: Optional[List[str]] = None,
 ) -> pd.DataFrame:
     """
     Load .csv data into DataFrame with associated metadata by group.
 
     Each group of .csv files may be located at a different path and be
     associated with additional user-defined metadata.
 
@@ -182,14 +197,18 @@
         Must contain the capturing group 'well' for the sample well IDs.
         Other capturing groups in the regex will be added as metadata.
         This value applies to all groups; to specify different regexes for each group,
         add the column 'filename_regex' to groups_df (this will override the
         'filename_regex' argument).
         If not included, the filenames are assumed to follow this format (default
         export format from FlowJo): 'export_[well]_[population].csv'
+    columns: Optional list of strings
+        If specified, only the specified columns are loaded out of the CSV files.
+        This can drastically reduce the amount of memory required to load
+        flow data.
 
     Returns
     -------
     A single pandas DataFrame containing data from all groups with associated metadata.
     """
     if "data_path" not in groups_df.columns:
         raise GroupsError("'groups_df' must contain column 'data_path'")
@@ -205,15 +224,15 @@
     for group in groups_df.to_dict(orient="index").values():
 
         # Load data in group
         data_path = base_path / Path(group["data_path"])
         yaml_path = base_path / Path(group["yaml_path"])
         if "filename_regex" in groups_df.columns:
             filename_regex = group["filename_regex"]
-        group_data = load_csv_with_metadata(data_path, yaml_path, filename_regex)
+        group_data = load_csv_with_metadata(data_path, yaml_path, filename_regex, columns=columns)
 
         # Add associated metadata (not paths)
         for k, v in group.items():
             if not (k == "data_path") and not (k == "yaml_path"):
                 group_data[k] = v
 
         group_list.append(group_data)
```

### Comparing `rushd-0.4.2/src/rushd/io.py` & `rushd-0.5.0/src/rushd/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     -------
     A tuple containing (rootdir, datadir). Each tuple component is None
     if the desired directory is not a accessible directory.
     """
     if datadir_txt is None:
         return (None, None)
     rootdir = datadir_txt.parent
-    datadir = Path(datadir_txt.read_text().strip("\n"))
+    datadir = Path(datadir_txt.read_text().strip("\n")).expanduser()
     return (rootdir if rootdir.is_dir() else None, datadir if datadir.is_dir() else None)
 
 
 _rootdir, _datadir = _load_root_datadir(_locate_datadir_txt())
 if _datadir is None:
     warnings.warn("Unable to locate datadir.txt", category=ImportWarning, stacklevel=2)
```

### Comparing `rushd-0.4.2/src/rushd/well_mapper.py` & `rushd-0.5.0/src/rushd/well_mapper.py`

 * *Files identical despite different names*

### Comparing `rushd-0.4.2/tests/test_file_io.py` & `rushd-0.5.0/tests/test_file_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,25 @@
 
 import pytest
 import rushd
 import rushd.io
 import yaml
 
 
+def test_datadir_home_dir(tmp_path: Path):
+    """Tests that home directory (tilde) expansion works"""
+    (tmp_path / "root").mkdir()
+
+    with (tmp_path / "root" / "datadir.txt").open("w") as datadir_txt:
+        datadir_txt.write("~")
+    os.chdir(tmp_path / "root")
+    reload(rushd.io)
+    assert rushd.datadir == Path("~").expanduser()
+
+
 def test_datadir_rootdir(tmp_path: Path):
     """
     Tests datadir/rootdir discovery, for
     a datadir.txt in the same directory and in
     a parent directory.
     """
     (tmp_path / "root").mkdir()
```

### Comparing `rushd-0.4.2/tests/test_file_moi.py` & `rushd-0.5.0/tests/test_file_moi.py`

 * *Files identical despite different names*

### Comparing `rushd-0.4.2/tests/test_flow.py` & `rushd-0.5.0/tests/test_flow.py`

 * *Files 4% similar despite different names*

```diff
@@ -320,14 +320,63 @@
     with open(str(tmp_path / "bad-name1.csv"), "w") as f:
         f.write("""channel1,channel2\n10,20""")
     yaml_path = str(tmp_path) + "/test.yaml"
     with pytest.raises(flow.RegexError):
         _ = flow.load_csv_with_metadata(str(tmp_path), yaml_path)
 
 
+def test_subcolumn_loading(tmp_path: Path):
+    """
+    Tests that column subsets can be loaded from CSV files.
+    """
+    with open(str(tmp_path / "test.yaml"), "w") as f:
+        f.write(
+            """
+        metadata:
+            condition:
+            - cond1: A1,G12
+        """
+        )
+    with open(str(tmp_path / "export_A1_singlets.csv"), "w") as f:
+        f.write("""channel1,channel2\n1,2""")
+    with open(str(tmp_path / "export_G12_singlets.csv"), "w") as f:
+        f.write("""channel1,channel2\n10,20""")
+    yaml_path = str(tmp_path) + "/test.yaml"
+    df = flow.load_csv_with_metadata(str(tmp_path), yaml_path)
+    # Make sure both are present first
+    assert "channel1" in df.columns
+    assert "channel2" in df.columns
+    # Reload specifying columns
+    df = flow.load_csv_with_metadata(str(tmp_path), yaml_path, columns=["channel1"])
+    assert "channel1" in df.columns
+    assert "channel2" not in df.columns
+
+
+def test_extra_columns(tmp_path: Path):
+    """
+    Tests that extra unused columns can be specified when loading
+    """
+    with open(str(tmp_path / "test.yaml"), "w") as f:
+        f.write(
+            """
+        metadata:
+            condition:
+            - cond1: A1
+        """
+        )
+    with open(str(tmp_path / "export_A1_singlets.csv"), "w") as f:
+        f.write("""channel1,channel2\n1,2""")
+    yaml_path = str(tmp_path) + "/test.yaml"
+    # Reload specifying columns
+    df = flow.load_csv_with_metadata(str(tmp_path), yaml_path, columns=["channel1", "channel3"])
+    assert "channel1" in df.columns
+    assert "channel2" not in df.columns
+    assert "channel3" not in df.columns
+
+
 def test_group_valid(tmp_path: Path):
     """
     Tests that groups of files can be loaded (no base path)
     """
     # Create data
     sub_dir = ["dir1", "dir2"]
     os.mkdir(tmp_path / sub_dir[0])
```

### Comparing `rushd-0.4.2/tests/test_pandas_cache.py` & `rushd-0.5.0/tests/test_pandas_cache.py`

 * *Files identical despite different names*

### Comparing `rushd-0.4.2/tests/test_well_mapper.py` & `rushd-0.5.0/tests/test_well_mapper.py`

 * *Files identical despite different names*

