# Comparing `tmp/euclidlib-0.0.4.tar.gz` & `tmp/euclidlib-0.0.5.tar.gz`

## Comparing `euclidlib-0.0.4.tar` & `euclidlib-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,21 @@
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 euclidlib-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 euclidlib-0.0.4/.github/workflows/release.yml
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 euclidlib-0.0.4/euclidlib/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 euclidlib-0.0.4/euclidlib/_version.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 euclidlib-0.0.4/euclidlib/photo/__init__.py
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 euclidlib-0.0.4/euclidlib/photo/_le3_pk_wl.py
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 euclidlib-0.0.4/euclidlib/photo/_phz.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 euclidlib-0.0.4/euclidlib/spectro/__init__.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 euclidlib-0.0.4/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 euclidlib-0.0.4/LICENSE
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 euclidlib-0.0.4/README.md
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 euclidlib-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 euclidlib-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 euclidlib-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 euclidlib-0.0.5/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 euclidlib-0.0.5/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 euclidlib-0.0.5/euclidlib/__init__.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 euclidlib-0.0.5/euclidlib/_util.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 euclidlib-0.0.5/euclidlib/_version.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 euclidlib-0.0.5/euclidlib/photo/__init__.py
+-rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 euclidlib-0.0.5/euclidlib/photo/_le3_pk_wl.py
+-rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 euclidlib-0.0.5/euclidlib/photo/_phz.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 euclidlib-0.0.5/euclidlib/spectro/__init__.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 euclidlib-0.0.5/tests/conftest.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 euclidlib-0.0.5/tests/test_util.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 euclidlib-0.0.5/tests/photo/test_le3_pk_wl.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 euclidlib-0.0.5/tests/photo/test_phz.py
+-rw-r--r--   0        0        0     4390 2020-02-02 00:00:00.000000 euclidlib-0.0.5/tests/photo/data/angular_power_spectra.fits.gz
+-rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 euclidlib-0.0.5/tests/photo/data/mixing_matrices.fits.gz
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 euclidlib-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 euclidlib-0.0.5/LICENSE
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 euclidlib-0.0.5/README.md
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 euclidlib-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 euclidlib-0.0.5/PKG-INFO
```

### Comparing `euclidlib-0.0.4/.pre-commit-config.yaml` & `euclidlib-0.0.5/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -24,8 +24,8 @@
       - id: trailing-whitespace
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.7.1
     hooks:
       - id: mypy
         args: [--strict, --python-version=3.12]
         additional_dependencies: [numpy]
-        exclude: ^.*/test_
+        exclude: ^tests
```

### Comparing `euclidlib-0.0.4/euclidlib/photo/_le3_pk_wl.py` & `euclidlib-0.0.5/euclidlib/photo/_le3_pk_wl.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,121 +1,125 @@
 from __future__ import annotations
 
-from collections.abc import Sequence
+import re
 from os import PathLike
-from typing import TYPE_CHECKING, Any, Tuple
+from typing import TYPE_CHECKING, Tuple, Union
 
 import fitsio  # type: ignore [import-not-found]
 import numpy as np
 from numpy.typing import NDArray
 
 if TYPE_CHECKING:
-    from typing import TypeAlias
+    from collections.abc import Iterator, Sequence
+    from typing import Any, TypeAlias
 
 
 # type alias
-TwoPointKey: TypeAlias = Tuple[str, str, int, int]
+_DictKey: "TypeAlias" = Union[str, int, Tuple["_DictKey", ...]]
 
 
 def toc_match(
-    key: tuple[Any, ...],
+    key: _DictKey,
     include: Sequence[tuple[Any, ...]] | None = None,
     exclude: Sequence[tuple[Any, ...]] | None = None,
 ) -> bool:
     """return whether a dict key matches include/exclude criteria"""
+    if not isinstance(key, tuple):
+        key = (key,)
     if include is not None:
         for pattern in include:
             if all(p is Ellipsis or p == k for p, k in zip(pattern, key)):
                 break
         else:
             return False
     if exclude is not None:
         for pattern in exclude:
             if all(p is Ellipsis or p == k for p, k in zip(pattern, key)):
                 return False
     return True
 
 
+def _key_from_string(s: str) -> _DictKey:
+    """return key from string representation"""
+    keys = s.split(";")
+    if len(keys) > 1:
+        return tuple(map(_key_from_string, keys))
+    keys = keys[0].split(",")
+    if len(keys) > 1:
+        return tuple(map(_key_from_string, keys))
+    key = keys[0]
+    return int(key) if key.isdigit() else key
+
+
 def _read_metadata(hdu: fitsio.TableHDU) -> dict[str, Any]:
     """read array metadata from FITS HDU"""
     h = hdu.read_header()
     md = {}
     for key in h:
         if key.startswith("META "):
             md[key[5:].lower()] = h[key]
     return md
 
 
-def _read_twopoint(fits: fitsio.FITS, ext: str) -> NDArray[Any]:
-    """read two-point data from FITS"""
+def _read_twopoint(hdu: fitsio.TableHDU) -> NDArray[Any]:
+    """read two-point data from FITS HDU"""
     # read data from extension
-    arr: NDArray[Any] = fits[ext].read()
+    arr: NDArray[Any] = hdu.read()
     # attach metadata to dtype
-    dt = np.dtype(arr.dtype, metadata=_read_metadata(fits[ext]))
+    dt = np.dtype(arr.dtype, metadata=_read_metadata(hdu))
     # return a copy (unfortunately) with changed dtype
     return arr.astype(dt, casting="no", copy=True)
 
 
+def _iterfits(
+    path: str | PathLike[str],
+    tag: str,
+    include: Sequence[tuple[Any, ...]] | None = None,
+    exclude: Sequence[tuple[Any, ...]] | None = None,
+) -> Iterator[fitsio.TableHDU]:
+    """
+    Iterate over HDUs that correspond to *tag* and have valid keys.
+    """
+    with fitsio.FITS(path) as fits:
+        for hdu in fits:
+            if not re.match(f"^{tag}\\d+$", hdu.get_extname()):
+                continue
+            h = hdu.read_header()
+            s = h.get("DICTKEY")
+            if s is None:
+                continue
+            key = _key_from_string(s)
+            if not toc_match(key, include=include, exclude=exclude):
+                continue
+            yield key, hdu
+
+
 def angular_power_spectra(
     path: str | PathLike[str],
     *,
     include: Sequence[tuple[Any, ...]] | None = None,
     exclude: Sequence[tuple[Any, ...]] | None = None,
-) -> dict[TwoPointKey, NDArray[Any]]:
+) -> dict[_DictKey, NDArray[Any]]:
     """
     Read angular power spectra from a Euclid data product.
     """
 
-    # the returned set of cls
     cls = {}
-
-    # open the FITS file for reading
-    with fitsio.FITS(path) as fits:
-        # get the TOC from the FITS file
-        fits_toc = fits["CLTOC"].read()
-
-        # read every entry in the TOC, add it to the list, then read the cls
-        for entry in fits_toc:
-            ext, k1, k2, i1, i2 = entry[["EXT", "NAME1", "NAME2", "BIN1", "BIN2"]]
-
-            # skip if not selected
-            if not toc_match((k1, k2, i1, i2), include=include, exclude=exclude):
-                continue
-
-            # read the cl from the extension and store in set of cls
-            cls[k1, k2, i1, i2] = _read_twopoint(fits, ext)
-
-    # return the dictionary of cls
+    for key, hdu in _iterfits(path, "CL", include, exclude):
+        cls[key] = _read_twopoint(hdu)
     return cls
 
 
 def mixing_matrices(
     path: str | PathLike[str],
     *,
     include: Sequence[tuple[Any, ...]] | None = None,
     exclude: Sequence[tuple[Any, ...]] | None = None,
-) -> dict[TwoPointKey, NDArray[Any]]:
+) -> dict[_DictKey, NDArray[Any]]:
     """
     Read mixing matrices from a Euclid data product.
     """
 
-    # the returned set of mms
     mms = {}
-
-    # open the FITS file for reading
-    with fitsio.FITS(path) as fits:
-        # get the TOC from the FITS file
-        fits_toc = fits["MMTOC"].read()
-
-        # read every entry in the TOC, add it to the list, then read the mms
-        for entry in fits_toc:
-            ext, k1, k2, i1, i2 = entry[["EXT", "NAME1", "NAME2", "BIN1", "BIN2"]]
-
-            # skip if not selected
-            if not toc_match((k1, k2, i1, i2), include=include, exclude=exclude):
-                continue
-
-            # read the mixing matrix from the extension and store in set of mms
-            mms[k1, k2, i1, i2] = _read_twopoint(fits, ext)
-
-    # return the dictionary of mms
+    for key, hdu in _iterfits(path, "MM", include, exclude):
+        mms[key] = _read_twopoint(hdu)
     return mms
```

### Comparing `euclidlib-0.0.4/LICENSE` & `euclidlib-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `euclidlib-0.0.4/pyproject.toml` & `euclidlib-0.0.5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -23,31 +23,29 @@
 requires-python = ">=3.7"
 dynamic = ["version"]
 dependencies = [
     "fitsio",
     "numpy",
 ]
 
+[project.urls]
+Repository = "https://github.com/euclidlib/euclidlib"
+Issues = "https://github.com/euclidlib/euclidlib/issues"
+
 [project.optional-dependencies]
 test = [
     "pytest>=6.0",
 ]
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.build.hooks.vcs]
 version-file = "euclidlib/_version.py"
 
 [tool.black]
-target-version = ["py312"]
 preview = true
 
-[tool.coverage.run]
-omit = [
-    "**/test_*",
-]
-
 [tool.coverage.report]
 exclude_also = [
     "if TYPE_CHECKING:",
 ]
```

### Comparing `euclidlib-0.0.4/PKG-INFO` & `euclidlib-0.0.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: euclidlib
-Version: 0.0.4
+Version: 0.0.5
 Summary: Unofficial package to read data from the Euclid mission
+Project-URL: Repository, https://github.com/euclidlib/euclidlib
+Project-URL: Issues, https://github.com/euclidlib/euclidlib/issues
 Author-email: Nicolas Tessore <n.tessore@ucl.ac.uk>, Guadalupe Canas-Herrera <guadalupe.canasherrera@esa.int>
 Maintainer-email: Nicolas Tessore <n.tessore@ucl.ac.uk>, Guadalupe Canas-Herrera <guadalupe.canasherrera@esa.int>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

