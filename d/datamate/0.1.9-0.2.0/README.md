# Comparing `tmp/datamate-0.1.9.tar.gz` & `tmp/datamate-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamate-0.1.9.tar", last modified: Wed May  3 21:39:26 2023, max compression
+gzip compressed data, was "datamate-0.2.0.tar", last modified: Tue Apr 16 09:58:49 2024, max compression
```

## Comparing `datamate-0.1.9.tar` & `datamate-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,28 @@
-drwxr-xr-x   0 lappalainenj (1483866292) 1899195968        0 2023-05-03 21:39:26.627900 datamate-0.1.9/
--rw-r--r--   0 lappalainenj (1483866292) 1899195968     3829 2023-05-03 21:39:26.627236 datamate-0.1.9/PKG-INFO
--rw-r--r--   0 lappalainenj (1483866292) 1899195968     3642 2023-03-06 13:58:32.000000 datamate-0.1.9/README.md
-drwxr-xr-x   0 lappalainenj (1483866292) 1899195968        0 2023-05-03 21:39:26.622092 datamate-0.1.9/datamate/
--rw-r--r--   0 lappalainenj (1483866292) 1899195968      647 2023-05-03 21:21:07.000000 datamate-0.1.9/datamate/__init__.py
--rw-r--r--   0 lappalainenj (1483866292) 1899195968    58283 2023-05-03 21:30:55.000000 datamate-0.1.9/datamate/directory.py
--rw-r--r--   0 lappalainenj (1483866292) 1899195968    11921 2023-05-01 17:35:54.000000 datamate-0.1.9/datamate/namespaces.py
--rw-r--r--   0 lappalainenj (1483866292) 1899195968       22 2023-05-03 21:32:04.000000 datamate-0.1.9/datamate/version.py
-drwxr-xr-x   0 lappalainenj (1483866292) 1899195968        0 2023-05-03 21:39:26.625124 datamate-0.1.9/datamate.egg-info/
--rw-r--r--   0 lappalainenj (1483866292) 1899195968     3829 2023-05-03 21:39:26.000000 datamate-0.1.9/datamate.egg-info/PKG-INFO
--rw-r--r--   0 lappalainenj (1483866292) 1899195968      331 2023-05-03 21:39:26.000000 datamate-0.1.9/datamate.egg-info/SOURCES.txt
--rw-r--r--   0 lappalainenj (1483866292) 1899195968        1 2023-05-03 21:39:26.000000 datamate-0.1.9/datamate.egg-info/dependency_links.txt
--rw-r--r--   0 lappalainenj (1483866292) 1899195968      109 2023-05-03 21:39:26.000000 datamate-0.1.9/datamate.egg-info/requires.txt
--rw-r--r--   0 lappalainenj (1483866292) 1899195968        9 2023-05-03 21:39:26.000000 datamate-0.1.9/datamate.egg-info/top_level.txt
--rw-r--r--   0 lappalainenj (1483866292) 1899195968       38 2023-05-03 21:39:26.628046 datamate-0.1.9/setup.cfg
--rw-r--r--   0 lappalainenj (1483866292) 1899195968      926 2023-05-01 19:20:47.000000 datamate-0.1.9/setup.py
-drwxr-xr-x   0 lappalainenj (1483866292) 1899195968        0 2023-05-03 21:39:26.626639 datamate-0.1.9/tests/
--rwxr-xr-x   0 lappalainenj (1483866292) 1899195968    30672 2023-05-03 21:20:18.000000 datamate-0.1.9/tests/test_directory.py
--rw-r--r--   0 lappalainenj (1483866292) 1899195968     3734 2023-05-03 21:20:00.000000 datamate-0.1.9/tests/test_namespaces.py
--rw-r--r--   0 lappalainenj (1483866292) 1899195968     2299 2023-05-03 21:38:37.000000 datamate-0.1.9/tests/test_swmr.py
+drwxr-xr-x   0 janne      (501) staff       (20)        0 2024-04-16 09:58:49.361116 datamate-0.2.0/
+drwxr-xr-x   0 janne      (501) staff       (20)        0 2024-04-16 09:58:49.354644 datamate-0.2.0/.github/
+drwxr-xr-x   0 janne      (501) staff       (20)        0 2024-04-16 09:58:49.355602 datamate-0.2.0/.github/workflows/
+-rw-r--r--   0 janne      (501) staff       (20)     1064 2024-04-16 08:24:47.000000 datamate-0.2.0/.github/workflows/auto_test.yml
+-rw-r--r--   0 janne      (501) staff       (20)      131 2024-04-16 09:53:06.000000 datamate-0.2.0/.gitignore
+-rw-r--r--   0 janne      (501) staff       (20)     2934 2024-04-16 09:58:49.360942 datamate-0.2.0/PKG-INFO
+-rw-r--r--   0 janne      (501) staff       (20)     2473 2024-04-16 08:25:03.000000 datamate-0.2.0/README.md
+drwxr-xr-x   0 janne      (501) staff       (20)        0 2024-04-16 09:58:49.357393 datamate-0.2.0/datamate/
+-rwx------   0 janne      (501) staff       (20)      647 2023-05-03 21:21:07.000000 datamate-0.2.0/datamate/__init__.py
+-rw-r--r--   0 janne      (501) staff       (20)    62707 2024-04-16 08:25:03.000000 datamate-0.2.0/datamate/directory.py
+-rwx------   0 janne      (501) staff       (20)    11921 2023-05-01 17:35:54.000000 datamate-0.2.0/datamate/namespaces.py
+-rw-r--r--   0 janne      (501) staff       (20)       22 2024-04-16 09:55:36.000000 datamate-0.2.0/datamate/version.py
+drwxr-xr-x   0 janne      (501) staff       (20)        0 2024-04-16 09:58:49.357883 datamate-0.2.0/datamate.egg-info/
+-rw-r--r--   0 janne      (501) staff       (20)     2934 2024-04-16 09:58:49.000000 datamate-0.2.0/datamate.egg-info/PKG-INFO
+-rwx------   0 janne      (501) staff       (20)      456 2024-04-16 09:58:49.000000 datamate-0.2.0/datamate.egg-info/SOURCES.txt
+-rwx------   0 janne      (501) staff       (20)        1 2024-04-16 09:58:49.000000 datamate-0.2.0/datamate.egg-info/dependency_links.txt
+-rwx------   0 janne      (501) staff       (20)      109 2024-04-16 09:58:49.000000 datamate-0.2.0/datamate.egg-info/requires.txt
+-rwx------   0 janne      (501) staff       (20)        9 2024-04-16 09:58:49.000000 datamate-0.2.0/datamate.egg-info/top_level.txt
+drwxr-xr-x   0 janne      (501) staff       (20)        0 2024-04-16 09:58:49.359053 datamate-0.2.0/examples/
+-rwx------   0 janne      (501) staff       (20)   457250 2023-05-03 21:33:56.000000 datamate-0.2.0/examples/01. Introduction to Datamate.ipynb
+-rwx------   0 janne      (501) staff       (20)   139159 2023-05-03 21:34:34.000000 datamate-0.2.0/examples/another thread.ipynb
+-rw-r--r--   0 janne      (501) staff       (20)     1135 2024-04-16 09:47:23.000000 datamate-0.2.0/license
+-rw-r--r--   0 janne      (501) staff       (20)       38 2024-04-16 09:58:49.361150 datamate-0.2.0/setup.cfg
+-rw-r--r--   0 janne      (501) staff       (20)      926 2024-04-16 09:53:06.000000 datamate-0.2.0/setup.py
+drwxr-xr-x   0 janne      (501) staff       (20)        0 2024-04-16 09:58:49.360561 datamate-0.2.0/tests/
+-rwxr-xr-x   0 janne      (501) staff       (20)    32121 2024-04-16 08:25:03.000000 datamate-0.2.0/tests/test_directory.py
+-rwx------   0 janne      (501) staff       (20)     3734 2023-05-03 21:20:00.000000 datamate-0.2.0/tests/test_namespaces.py
+-rw-r--r--   0 janne      (501) staff       (20)      868 2024-04-16 08:25:03.000000 datamate-0.2.0/tests/test_swmr.py
```

### Comparing `datamate-0.1.9/datamate/__init__.py` & `datamate-0.2.0/datamate/__init__.py`

 * *Files identical despite different names*

### Comparing `datamate-0.1.9/datamate/directory.py` & `datamate-0.2.0/datamate/directory.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,20 +31,23 @@
     Union,
     cast,
     get_origin,
 )
 from typing_extensions import Protocol
 import datetime
 from traceback import format_tb
+from ruamel.yaml import YAML
+from importlib import import_module
 
 
 from contextlib import contextmanager
 
 import h5py as h5
 import numpy as np
+import pandas as pd
 from pandas import DataFrame
 
 from datamate.namespaces import (
     Namespace,
     namespacify,
     is_disjoint,
     is_superset,
@@ -467,15 +470,15 @@
         Yields field names corresponding to the public files in `self.path`
 
         Entries it understands (subdirectories and HDF5 files) are yielded
         without extensions. Non-public files (files whose names start with "_")
         are ignored.
         """
         for p in self.path.glob("[!_]*"):
-            yield p.name[:-3] if p.suffix == ".h5" else p.name
+            yield p.name.rpartition(".")[0] if p.suffix in [".h5", ".csv"] else p.name
 
     def __copy__(self):
         return Directory(self.path)
 
     def __deepcopy__(self, memodict={}):
         return self.__copy__()
 
@@ -551,14 +554,18 @@
                 )
             raise e
 
         # Return an array.
         if path.with_suffix(".h5").is_file():
             return _read_h5(path.with_suffix(".h5"))
 
+        # Return a csv
+        if path.with_suffix(".csv").is_file():
+            return pd.read_csv(path.with_suffix(".csv"))
+
         # Return the path to a file.
         elif path.is_file():
             return path
 
         # Return a subrecord
         else:
             return Directory(path)
@@ -589,18 +596,25 @@
             elif os.path.isdir(val):
                 _copy_dir(path, val)
 
         # Write a subDirectory.
         elif isinstance(val, (Mapping, Directory)):
             assert path.suffix == ""
             MutableMapping.update(Directory(path), val)  # type: ignore
+        
+        # Write a dataframe.
+        elif isinstance(val, DataFrame):
+            assert path.suffix == ""
+            val.to_csv(path.with_suffix(".csv"), index=False)
 
         # Write an array.
         else:
             assert path.suffix == ""
+            if isinstance(val, H5Reader):
+                val = val[()]
             try:
                 _write_h5(path.with_suffix(".h5"), val)
             except TypeError as err:
                 raise TypeError(
                     format_tb(err.__traceback__)[0]
                     + err.args[0]
                     + f"\nYou're trying to store {val} which cannot be converted to h5-file in {path}."
@@ -626,14 +640,18 @@
         #     object.__delitem__(self, key)
         #     return
         path = self.path / key
 
         # Delete an array file.
         if path.with_suffix(".h5").is_file():
             path.with_suffix(".h5").unlink()
+            
+        # Delete a csv file.
+        if path.with_suffix(".csv").is_file():
+            path.with_suffix(".csv").unlink()
 
         # Delete a non-array file.
         elif path.is_file():
             path.unlink()
 
         # Delete a Directory.
         else:
@@ -661,18 +679,29 @@
             _extend_file(path, val)
 
         # Append a subDirectory.
         elif isinstance(val, (Mapping, Directory)):
             assert path.suffix == ""
             for k in val:
                 Directory(path).extend(k, val[k])
+        
+        elif isinstance(val, pd.DataFrame):
+            assert path.suffix == ""
+            if path.with_suffix(".csv").is_file():
+                old_df = pd.read_csv(path.with_suffix(".csv"))
+                new_df = pd.concat([old_df, val], axis=0)
+            else:
+                new_df = val
+            new_df.to_csv(path.with_suffix(".csv"), index=False)
 
         # Append an array.
         else:
             assert path.suffix == ""
+            if isinstance(val, H5Reader):
+                val = val[()]
             _extend_h5(path.with_suffix(".h5"), val)
 
         if self.config is not None and self.status == "done":
             # Track if a Directory has been modified past __init__
             self._modified_past_init(True)
 
     # --- Views ---
@@ -725,14 +754,16 @@
                 limit_to_directories=limit_to_directories,
             )
         )
 
     # -- Attribute-style element access --------------------
 
     def __getattr__(self, key: str) -> Any:
+        if key.startswith("__") and key.endswith("__"): # exclude dunder attributes
+            return None
         return self.__getitem__(key.replace("__", "."))
 
     def __setattr__(self, key: str, value: object) -> None:
         # Fix autoreload related effect.
         if key.startswith("__") and key.endswith("__"):
             object.__setattr__(self, key, value)
             return
@@ -770,58 +801,49 @@
 
         config (Dict): update for meta.config
         status (str): status if config did not exist before, i.e. _overrid_config
             is used to store a _meta.yaml for the first time instead of build.
         """
         meta_path = self.path / "_meta.yaml"
 
-        def write_meta(**kwargs):
-            meta_path.write_text(json.dumps(_identify_elements(kwargs)))
-
         current_config = self.config
         if current_config is not None:
             with warnings.catch_warnings():
                 warnings.simplefilter("always")
                 warnings.warn(
                     (
                         f"Overriding config. Diff is:"
                         f'{config.diff(current_config, name1="passed", name2="stored")}'
                     ),
                     ConfigWarning,
                     stacklevel=2,
                 )
-            write_meta(config=config, status="overridden")
+            write_meta(path=meta_path, config=config, status="overridden")
         else:
-            write_meta(config=config, status=status or self.status)
+            write_meta(path=meta_path, config=config, status=status or self.status)
 
     def _override_status(self, status):
         meta_path = self.path / "_meta.yaml"
 
-        def write_meta(**kwargs):
-            meta_path.write_text(json.dumps(_identify_elements(kwargs)))
-
         current_status = self.status
         if current_status is not None:
             with warnings.catch_warnings():
                 warnings.simplefilter("always")
                 warnings.warn(
                     (f"Overriding status {current_status} to {status}"),
                     ConfigWarning,
                     stacklevel=2,
                 )
-        write_meta(config=self.config, status=status)
+        write_meta(path=meta_path, config=self.config, status=status)
 
     def _modified_past_init(self, is_modified):
         meta_path = self.path / "_meta.yaml"
 
-        def write_meta(**kwargs):
-            meta_path.write_text(json.dumps(_identify_elements(kwargs)))
-
         if is_modified:
-            write_meta(config=self.config, status=self.status, modified=True)
+            write_meta(path=meta_path, config=self.config, status=self.status, modified=True)
 
     def check_size(self, warning_at=20 * 1024**3, print_size=False) -> None:
         """Prints the size of the directory in bytes."""
         return check_size(self.path, warning_at, print_size)
 
     def to_df(self, dtypes: dict = None) -> DataFrame:
         """
@@ -1220,19 +1242,16 @@
         sleep(0.01)
         return _build(directory)
 
     directory.path.mkdir(parents=True)
 
     meta_path = directory.path / "_meta.yaml"
     config = Namespace(**directory._config)
-    write_meta = lambda **kwargs: meta_path.write_text(
-        json.dumps(_identify_elements(kwargs))
-    )
 
-    write_meta(config=config, status="running")
+    write_meta(path=meta_path, config=config, status="running")
 
     try:
         if callable(getattr(type(directory), "__init__", None)):
             n_build_args = directory.__init__.__code__.co_argcount
             # case 1: __init__(self)
             if n_build_args <= 1:
                 build_args = []
@@ -1245,17 +1264,17 @@
             else:
                 kwargs = namespacify(get_defaults_from_init(directory))
                 assert kwargs
                 build_args = []
                 build_kwargs = {k: directory._config[k] for k in kwargs}
             directory.__init__(*build_args, **build_kwargs)
 
-        write_meta(config=config, status="done")
+        write_meta(path=meta_path, config=config, status="done")
     except BaseException as e:
-        write_meta(config=config, status="stopped")
+        write_meta(path=meta_path, config=config, status="stopped")
         raise e
 
 
 def call_signature(cls):
     signature = """
 
 Example call signature:
@@ -1395,15 +1414,21 @@
 
     # Perform subclass forwarding.
     cls_override = config.pop("type", None)
     if isinstance(cls_override, type):
         cls = cls_override
     elif isinstance(cls_override, str):
         try:
-            cls = get_scope()[cls_override]
+            if "." in cls_override:  # hydra-style `type` field
+                paths = list(cls_override.split("."))
+                cls = import_module(paths[0])
+                for path in paths[1:]:
+                    cls = getattr(cls, path)
+            else:  # legacy scope management
+                cls = get_scope()[cls_override]
         except KeyError as e:
             cls = type(cls_override, (Directory,), {})
             with warnings.catch_warnings():
                 warnings.simplefilter("always")
                 warnings.warn(
                     (
                         "Casting to a new subclass of Directory because "
@@ -1436,38 +1461,79 @@
     object.__setattr__(obj, "_config", namespacify(config))
     return cast(Directory, obj)
 
 
 # -- I/O -----------------------------------------------------------------------
 
 
+class H5Reader:
+    """Wrapper around h5 read operations to prevent persistent file handles
+    by ensuring file handles are open only during each access operation. 
+    """
+    def __init__(self, path, assert_swmr=True, n_retries=10):
+        self.path = path
+        with h5.File(self.path, mode="r", libver="latest", swmr=True) as f:
+            if assert_swmr:
+                assert f.swmr_mode, "File is not in SWMR mode."
+            assert "data" in f
+            self.shape = f["data"].shape
+            self.dtype = f["data"].dtype
+        self.n_retries = n_retries
+
+    def __getitem__(self, key):
+        for retry_count in range(self.n_retries):
+            try:
+                with h5.File(self.path, mode="r", libver="latest", swmr=True) as f:
+                    data = f["data"][key]
+                break
+            except Exception as e:
+                if retry_count == self.n_retries - 1:
+                    raise e
+                sleep(0.1)
+        return data
+
+    def __len__(self):
+        return self.shape[0]
+
+    def __getattr__(self, key):
+        # get attribute from underlying h5.Dataset object
+        for retry_count in range(self.n_retries):
+            try:
+                with h5.File(self.path, mode="r", libver="latest", swmr=True) as f:
+                    value = getattr(f["data"], key, None)
+                break
+            except Exception as e:
+                if retry_count == self.n_retries - 1:
+                    raise e
+                sleep(0.1)
+        if value is None:
+            raise AttributeError(f"Attribute {key} not found.")
+        # wrap callable attributes to open file before calling function
+        if callable(value):
+            def safe_wrapper(*args, **kwargs):
+                # not trying `n_retries` times here, just for simplicity
+                with h5.File(self.path, mode="r", libver="latest", swmr=True) as f:
+                    output = getattr(f["data"], key)(*args, **kwargs)
+                return output
+            return safe_wrapper
+        # otherwise just return value
+        else:
+            return value
+
+
 def _read_h5(path: Path, assert_swmr=True) -> ArrayFile:
     try:
-        f = h5.File(path, "r", libver="latest", swmr=True)
-        if assert_swmr:
-            assert f.swmr_mode, "File is not in SWMR mode."
-        return f["data"]
+        return H5Reader(path, assert_swmr=assert_swmr)
     except OSError as e:
-        print(e)
+        print(f"{path}: {e}")
         if "errno = 2" in str(e):
             raise e
         sleep(0.1)
         return _read_h5(path)
 
-    # try:
-    #     f = h5.File(path, "r", libver="latest", swmr=True)
-    #     assert f.swmr_mode
-    #     return f["data"]
-    # except OSError as e:
-    #     print(e)
-    #     if "errno = 2" in str(e):  # 2 := File not found.
-    #         raise e
-    #     sleep(0.1)
-    #     return _read_h5(path)
-
 
 def _write_h5(path: Path, val: object) -> None:
     val = np.asarray(val)
     try:
         f = h5.File(path, libver="latest", mode="w")
         if f["data"].dtype != val.dtype:
             raise ValueError()
@@ -1483,14 +1549,15 @@
                 path.unlink()
             except FileNotFoundError:
                 pass
         f = h5.File(path, libver="latest", mode="w")
         f["data"] = val
         f.swmr_mode = True
         assert f.swmr_mode
+    f.close()
 
 
 def _extend_h5(path: Path, val: object, retry: int = 0, max_retries: int = 50) -> None:
     val = np.asarray(val)
     path.parent.mkdir(parents=True, exist_ok=True)
     # mode='a' to read file, create otherwise
     try:
@@ -1544,22 +1611,22 @@
         except TypeError as e:
             # workaround if dataset was first created as non-chunked
             # using __setitem__ and then extended using extend
             if "Only chunked datasets can be resized" in str(e):
                 _override_to_chunked(path, val)
             else:
                 raise e
+    f.close()
 
 
 def _copy_file(dst: Path, src: Path) -> None:
     # shutil.rmtree(dst, ignore_errors=True)
     dst.parent.mkdir(parents=True, exist_ok=True)
     shutil.copy(src, dst)
 
-
 def _copy_dir(dst: Path, src: Path) -> None:
     # shutil.rmtree(dst, ignore_errors=True)
     dst.parent.mkdir(parents=True, exist_ok=True)
     shutil.copytree(src, dst)
 
 
 def _copy_if_conflict(src):
@@ -1576,43 +1643,73 @@
         with open(dst, "ab+") as f_dst:
             f_dst.write(f_src.read())
 
 
 def read_meta(path: Path) -> Namespace:
     # TODO: Implement caching
     try:
-        # meta = namespacify(yaml.safe_load((path/'_meta.yaml').read_text()))
-        meta = namespacify(json.loads((path / "_meta.yaml").read_text()))
+        try:  # for backwards compatibility
+            meta = namespacify(json.loads((path / "_meta.yaml").read_text()))
+            warnings.warn(f"Directory {path} still has legacy JSON config. Please update to YAML when possible.")
+            # resp = input("Would you like to overwrite the existing config with an updated version? (y/n): ")
+            # if resp.strip().lower() == "y":
+            #     write_meta(path / "_meta.yaml", **meta)
+        except json.decoder.JSONDecodeError as e:
+            yaml = YAML()
+            with open(path / "_meta.yaml", "r") as f:
+                meta = yaml.load(f)
+            meta = namespacify(meta)
         assert isinstance(meta, Namespace)
         if hasattr(meta, "config"):
             assert isinstance(meta.config, Namespace)
         elif hasattr(meta, "spec"):  # for backwards compatibility
             assert isinstance(meta.spec, Namespace)
+            warnings.warn(f"Directory {path} has legacy `spec` attribute instead of `meta`. Please update when possible.")
             meta["config"] = meta.pop("spec")
-        assert isinstance(meta.status, str)
+            # resp = input("Would you like to overwrite the existing config with an updated version? (y/n): ")
+            # if resp.strip().lower() == "y":
+            #     write_meta(path / "_meta.yaml", **meta)
+            assert isinstance(meta.status, str)
         return meta
     except:
         return Namespace(config=None, status="done")
 
 
+def write_meta(path: Path, **kwargs):
+    yaml = YAML()
+    # support dumping numpy objects
+    def represent_numpy_float(self, value):
+        return self.represent_float(float(value))
+    def represent_numpy_int(self, value):
+        return self.represent_int(int(value))
+    def represent_numpy_array(self, value):
+        return self.represent_sequence(value.tolist())
+    yaml.Representer.add_multi_representer(np.ndarray, represent_numpy_array)
+    yaml.Representer.add_multi_representer(np.floating, represent_numpy_float)
+    yaml.Representer.add_multi_representer(np.integer, represent_numpy_int)
+    # dump config to yaml
+    with open(path, "w") as f:
+        yaml.dump(_identify_elements(kwargs), f)
+
+
 def directory_to_dict(directory: Directory) -> dict:
     dw_dict = {
         key: getattr(directory, key)[...]
         for key in list(directory.keys())
-        if isinstance(getattr(directory, key), h5.Dataset)
+        if isinstance(getattr(directory, key), H5Reader)
     }
     return dw_dict
 
 
 def directory_to_df(directory: Directory, dtypes: dict = None) -> DataFrame:
     """Convert a directory to a pandas DataFrame."""
     df_dict = {
         key: getattr(directory, key)[...]
         for key in list(directory.keys())
-        if isinstance(getattr(directory, key), h5.Dataset)
+        if isinstance(getattr(directory, key), H5Reader)
     }
 
     # Get the lengths of all datasets.
     nelements = {k: len(v) or 1 for k, v in df_dict.items()}
 
     lengths, counts = np.unique([val for val in nelements.values()], return_counts=True)
     most_frequent_length = lengths[np.argmax(counts)]
@@ -1743,10 +1840,10 @@
 
 def _identify_elements(obj: object) -> object:
     if isinstance(obj, type):
         return _identify(obj)
     elif isinstance(obj, list):
         return [_identify_elements(elem) for elem in obj]
     elif isinstance(obj, dict):
-        return Namespace({k: _identify_elements(obj[k]) for k in obj})
+        return {k: _identify_elements(obj[k]) for k in obj}
     else:
-        return obj
+        return obj
```

### Comparing `datamate-0.1.9/datamate/namespaces.py` & `datamate-0.2.0/datamate/namespaces.py`

 * *Files identical despite different names*

### Comparing `datamate-0.1.9/setup.py` & `datamate-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `datamate-0.1.9/tests/test_directory.py` & `datamate-0.2.0/tests/test_directory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import threading
 import time
 from pathlib import Path
 from typing import List
 
 import h5py as h5
 import numpy as np
+import pandas as pd
 import pytest
 import shutil
 
 from datamate import (
     Directory,
     Namespace,
     set_root_dir,
@@ -19,14 +20,15 @@
 from datamate.directory import (
     ModifiedError,
     ModifiedWarning,
     ConfigWarning,
     ImplementationWarning,
     ImplementationError,
     _auto_doc,
+    H5Reader,
 )
 
 # -- Helper functions ----------------------------------------------------------
 
 
 def data_file(path: Path) -> Path:
     path.parent.mkdir(parents=True, exist_ok=True)
@@ -76,19 +78,26 @@
             k_mod = k.replace(".", "__")
             assert (directory.path / k).is_file()
             assert isinstance(directory[k], Path)
             assert isinstance(getattr(directory, k), Path)
             assert directory[k].read_bytes() == v.read_bytes()
             assert getattr(directory, k).read_bytes() == v.read_bytes()
             assert getattr(directory, k_mod).read_bytes() == v.read_bytes()
+        
+        elif isinstance(v, pd.DataFrame):
+            assert (directory.path / k).with_suffix(".csv").is_file()
+            assert isinstance(directory[k], pd.DataFrame)
+            assert isinstance(getattr(directory, k), pd.DataFrame)
+            assert np.array_equal(directory[k].to_numpy(), v.to_numpy())
+            assert np.array_equal(getattr(directory, k).to_numpy(), v.to_numpy())
 
         else:
             assert (directory.path / k).with_suffix(".h5").is_file()
-            assert isinstance(directory[k], h5.Dataset)
-            assert isinstance(getattr(directory, k), h5.Dataset)
+            assert isinstance(directory[k], H5Reader)
+            assert isinstance(getattr(directory, k), H5Reader)
             assert np.array_equal(directory[k][()], v)
             assert np.array_equal(getattr(directory, k)[()], v)
             assert directory[k].dtype == np.asarray(v).dtype
             assert getattr(directory, k).dtype == np.asarray(v).dtype
 
 
 # -- [Base class tests] Empty directories --------------------------------------
@@ -162,14 +171,29 @@
         {
             "b": np.zeros((4, 5, 6), dtype="float32"),
             "c": np.ones((2, 3), dtype="uint16"),
         },
     )
 
 
+def test_dataframe_assignment(tmp_path: Path) -> None:
+    a = Directory(tmp_path)
+    a.b = pd.DataFrame({"a": [0, 1, 2], "b": [3, 4, 5]})
+    a.b = pd.DataFrame({"a": [3, 4, 5], "b": [0, 1, 2]})
+    a["c"] = pd.DataFrame({"a": [0, 1], "b": [3, 4]})
+    a["c"] = pd.DataFrame({"a": [3, 4], "b": [0, 1]})
+    assert_directory_equals(
+        a,
+        {
+            "b": pd.DataFrame({"a": [3, 4, 5], "b": [0, 1, 2]}),
+            "c": pd.DataFrame({"a": [3, 4], "b": [0, 1]}),
+        },
+    )
+
+
 def test_path_assignment(tmp_path: Path) -> None:
     a = Directory(tmp_path / "directory")
     a.b__bin = data_file(tmp_path / "b0.bin")
     a.b__bin = data_file(tmp_path / "b1.bin")
     a["c.bin"] = data_file(tmp_path / "c0.bin")
     a["c.bin"] = data_file(tmp_path / "c1.bin")
     assert_directory_equals(
@@ -223,14 +247,26 @@
     a.extend("b", np.uint16([[11, 12]]))
     assert_directory_equals(a, {"b": np.uint16([[7, 8], [9, 10], [11, 12]])})
 
     b = Directory(tmp_path)
     b.b = np.uint16([[7, 8], [9, 10]])
     b.extend("b", np.uint16([[11, 12]]))
     assert_directory_equals(b, {"b": np.uint16([[7, 8], [9, 10], [11, 12]])})
+    
+
+def test_dataframe_extension(tmp_path: Path) -> None:
+    a = Directory(tmp_path)
+    a.extend("b", pd.DataFrame({"a": [7, 9], "b": [8, 10]}))
+    a.extend("b", pd.DataFrame({"a": [11], "b": [12]}))
+    assert_directory_equals(a, {"b": pd.DataFrame({"a": [7, 9, 11], "b": [8, 10, 12]})})
+
+    b = Directory(tmp_path)
+    b.b = pd.DataFrame({"a": [7, 9], "b": [8, 10]})
+    b.extend("b", pd.DataFrame({"a": [11], "b": [12]}))
+    assert_directory_equals(b, {"b": pd.DataFrame({"a": [7, 9, 11], "b": [8, 10, 12]})})
 
 
 def test_path_extension(tmp_path: Path) -> None:
     a = Directory(tmp_path / "a")
     a.extend("b.bin", data_file(tmp_path / "b0.bin"))
     a.extend("b.bin", data_file(tmp_path / "b1.bin"))
     assert_directory_equals(
```

### Comparing `datamate-0.1.9/tests/test_namespaces.py` & `datamate-0.2.0/tests/test_namespaces.py`

 * *Files identical despite different names*

