# Comparing `tmp/healpix_alchemy-1.0.2.tar.gz` & `tmp/healpix_alchemy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "healpix_alchemy-1.0.2.tar", max compression
+gzip compressed data, was "healpix_alchemy-1.1.0.tar", max compression
```

## Comparing `healpix_alchemy-1.0.2.tar` & `healpix_alchemy-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1526 2023-03-03 13:25:37.685804 healpix_alchemy-1.0.2/LICENSE
--rw-r--r--   0        0        0    21119 2023-03-03 13:25:37.685804 healpix_alchemy-1.0.2/README.md
--rw-r--r--   0        0        0       93 2023-03-03 13:25:37.685804 healpix_alchemy-1.0.2/healpix_alchemy/__init__.py
--rw-r--r--   0        0        0      592 2023-03-03 13:25:37.685804 healpix_alchemy-1.0.2/healpix_alchemy/constants.py
--rw-r--r--   0        0        0      180 2023-03-03 13:25:37.685804 healpix_alchemy-1.0.2/healpix_alchemy/func.py
--rw-r--r--   0        0        0        0 2023-03-03 13:25:37.685804 healpix_alchemy-1.0.2/healpix_alchemy/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-03-03 13:25:37.685804 healpix_alchemy-1.0.2/healpix_alchemy/tests/benchmarks/__init__.py
--rw-r--r--   0        0        0      947 2023-03-03 13:25:37.685804 healpix_alchemy-1.0.2/healpix_alchemy/tests/benchmarks/conftest.py
--rw-r--r--   0        0        0     3984 2023-03-03 13:25:37.685804 healpix_alchemy-1.0.2/healpix_alchemy/tests/benchmarks/data.py
--rw-r--r--   0        0        0      874 2023-03-03 13:25:37.685804 healpix_alchemy-1.0.2/healpix_alchemy/tests/benchmarks/models.py
--rw-r--r--   0        0        0     2660 2023-03-03 13:25:37.685804 healpix_alchemy-1.0.2/healpix_alchemy/tests/benchmarks/test_benchmarks.py
--rw-r--r--   0        0        0     2814 2023-03-03 13:25:37.685804 healpix_alchemy-1.0.2/healpix_alchemy/types.py
--rw-r--r--   0        0        0     1236 2023-03-03 13:25:37.685804 healpix_alchemy-1.0.2/pyproject.toml
--rw-r--r--   0        0        0    22076 1970-01-01 00:00:00.000000 healpix_alchemy-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1526 2024-04-16 15:22:19.183814 healpix_alchemy-1.1.0/LICENSE
+-rw-r--r--   0        0        0    21119 2024-04-16 15:22:19.183814 healpix_alchemy-1.1.0/README.md
+-rw-r--r--   0        0        0       93 2024-04-16 15:22:19.183814 healpix_alchemy-1.1.0/healpix_alchemy/__init__.py
+-rw-r--r--   0        0        0      592 2024-04-16 15:22:19.183814 healpix_alchemy-1.1.0/healpix_alchemy/constants.py
+-rw-r--r--   0        0        0      180 2024-04-16 15:22:19.183814 healpix_alchemy-1.1.0/healpix_alchemy/func.py
+-rw-r--r--   0        0        0     2814 2024-04-16 15:22:19.183814 healpix_alchemy-1.1.0/healpix_alchemy/types.py
+-rw-r--r--   0        0        0     1244 2024-04-16 15:22:19.183814 healpix_alchemy-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 15:22:19.183814 healpix_alchemy-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 15:22:19.183814 healpix_alchemy-1.1.0/tests/benchmarks/__init__.py
+-rw-r--r--   0        0        0      750 2024-04-16 15:22:19.183814 healpix_alchemy-1.1.0/tests/benchmarks/conftest.py
+-rw-r--r--   0        0        0     4152 2024-04-16 15:22:19.183814 healpix_alchemy-1.1.0/tests/benchmarks/data.py
+-rw-r--r--   0        0        0      887 2024-04-16 15:22:19.183814 healpix_alchemy-1.1.0/tests/benchmarks/models.py
+-rw-r--r--   0        0        0     2673 2024-04-16 15:22:19.183814 healpix_alchemy-1.1.0/tests/benchmarks/test_benchmarks.py
+-rw-r--r--   0        0        0    22077 1970-01-01 00:00:00.000000 healpix_alchemy-1.1.0/PKG-INFO
```

### Comparing `healpix_alchemy-1.0.2/LICENSE` & `healpix_alchemy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `healpix_alchemy-1.0.2/README.md` & `healpix_alchemy-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `healpix_alchemy-1.0.2/healpix_alchemy/constants.py` & `healpix_alchemy-1.1.0/healpix_alchemy/constants.py`

 * *Files identical despite different names*

### Comparing `healpix_alchemy-1.0.2/healpix_alchemy/tests/benchmarks/data.py` & `healpix_alchemy-1.1.0/tests/benchmarks/data.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """SQLAlchemy sample data for unit tests.
 
 Notes
 -----
-We use the psycopg2 ``copy_from`` rather than SQLAlchemy for fast insertion.
+We use the psycopg ``copy`` rather than SQLAlchemy for fast insertion.
 
 """
-import io
-
 from astropy.coordinates import SkyCoord, uniform_spherical_random_surface
 from astropy import units as u
 from mocpy import MOC
 import numpy as np
 import pytest
 
-from ...constants import HPX, LEVEL, PIXEL_AREA
-from ...types import Tile
+from healpix_alchemy.constants import HPX, LEVEL, PIXEL_AREA
+from healpix_alchemy.types import Tile
+
 from .models import Galaxy, Field, FieldTile, Skymap, SkymapTile
 
 (
     RANDOM_GALAXIES_SEED,
     RANDOM_FIELDS_SEED,
     RANDOM_SKY_MAP_SEED
 ) = np.random.SeedSequence(12345).spawn(3)
@@ -72,35 +71,35 @@
         return uniform_spherical_random_surface(n)
 
 
 def get_random_galaxies(n, cursor):
     points = SkyCoord(get_random_points(n, RANDOM_GALAXIES_SEED))
     hpx = HPX.skycoord_to_healpix(points)
 
-    f = io.StringIO('\n'.join(f'{i}' for i in hpx))
-    cursor.copy_from(f, Galaxy.__tablename__, columns=('hpx',))
+    with cursor.copy(f'COPY {Galaxy.__tablename__} (hpx) FROM STDIN') as copy:
+        copy.write('\n'.join(f'{i}' for i in hpx))
 
     return points
 
 
 def get_random_fields(n, cursor):
     centers = SkyCoord(get_random_points(n, RANDOM_FIELDS_SEED))
     footprints = get_footprints_grid(*get_ztf_footprint_corners(), centers)
     mocs = [MOC.from_polygon_skycoord(footprint) for footprint in footprints]
 
-    f = io.StringIO('\n'.join(f'{i}' for i in range(len(mocs))))
-    cursor.copy_from(f, Field.__tablename__)
+    with cursor.copy(f'COPY {Field.__tablename__} FROM STDIN') as copy:
+        copy.write('\n'.join(f'{i}' for i in range(len(mocs))))
 
-    f = io.StringIO(
-        '\n'.join(
-            f'{i}\t{hpx}'
-            for i, moc in enumerate(mocs) for hpx in Tile.tiles_from(moc)
+    with cursor.copy(f'COPY {FieldTile.__tablename__} FROM STDIN') as copy:
+        copy.write(
+            '\n'.join(
+                f'{i}\t{hpx}'
+                for i, moc in enumerate(mocs) for hpx in Tile.tiles_from(moc)
+            )
         )
-    )
-    cursor.copy_from(f, FieldTile.__tablename__)
 
     return mocs
 
 
 def get_random_sky_map(n, cursor):
     rng = np.random.default_rng(RANDOM_SKY_MAP_SEED)
     # Make a randomly subdivided sky map
@@ -116,19 +115,19 @@
         tiles.insert(i, hi - diff)
         tiles.insert(i, hi - 2 * diff)
         tiles.insert(i, hi - 3 * diff)
 
     probdensity = rng.uniform(0, 1, size=len(tiles) - 1)
     probdensity /= np.sum(np.diff(tiles) * probdensity) * PIXEL_AREA
 
-    f = io.StringIO('1')
-    cursor.copy_from(f, Skymap.__tablename__)
+    with cursor.copy(f'COPY {Skymap.__tablename__} FROM STDIN') as copy:
+        copy.write('1')
 
-    f = io.StringIO(
-        '\n'.join(
-            f'1\t[{lo},{hi})\t{p}'
-            for lo, hi, p in zip(tiles[:-1], tiles[1:], probdensity)
+    with cursor.copy(f'COPY {SkymapTile.__tablename__} FROM STDIN') as copy:
+        copy.write(
+            '\n'.join(
+                f'1\t[{lo},{hi})\t{p}'
+                for lo, hi, p in zip(tiles[:-1], tiles[1:], probdensity)
+            )
         )
-    )
-    cursor.copy_from(f, SkymapTile.__tablename__)
 
     return tiles, probdensity
```

### Comparing `healpix_alchemy-1.0.2/healpix_alchemy/tests/benchmarks/models.py` & `healpix_alchemy-1.1.0/tests/benchmarks/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """SQLAlchemy ORM models for unit tests."""
 import sqlalchemy as sa
 from sqlalchemy import orm
 
-from ...types import Point, Tile
+from healpix_alchemy.types import Point, Tile
 
 
 @orm.as_declarative()
 class Base:
 
     @orm.declared_attr
     def __tablename__(cls):
```

### Comparing `healpix_alchemy-1.0.2/healpix_alchemy/tests/benchmarks/test_benchmarks.py` & `healpix_alchemy-1.1.0/tests/benchmarks/test_benchmarks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from functools import reduce
 
 import numpy as np
 import sqlalchemy as sa
 import pytest
 
-from ... import func
+from healpix_alchemy import func
+
 from .models import Galaxy, FieldTile, SkymapTile
 
 
 @pytest.fixture
 def bench(benchmark, session):
 
     def _func(query):
```

### Comparing `healpix_alchemy-1.0.2/healpix_alchemy/types.py` & `healpix_alchemy-1.1.0/healpix_alchemy/types.py`

 * *Files identical despite different names*

### Comparing `healpix_alchemy-1.0.2/pyproject.toml` & `healpix_alchemy-1.1.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 [tool.poetry]
 name = "healpix-alchemy"
-version = "1.0.2"
+version = "1.1.0"
 description = "SQLAlchemy extensions for HEALPix spatially indexed astronomy data"
 readme = "README.md"
 authors = ["Leo Singer <leo.singer@ligo.org>"]
 license = "BSD-3-clause"
 repository = "https://github.com/skyportal/healpix-alchemy"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Topic :: Database",
     "Topic :: Scientific/Engineering :: Astronomy"
 ]
+include = [
+    { path = "tests", format = "sdist" },
+]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 astropy = "*"
 astropy_healpix = "*"
 mocpy = ">=0.12.2"
 sqlalchemy = ">=1.4"
 
 [tool.poetry.group.dev.dependencies]
 astroquery = "*"
 numpy = "*"
 pandas = "*"
-psycopg2-binary = "*"
+psycopg = { version = "*", extras = ["binary"] }
 pytest = "*"
 pytest-benchmark = "*"
 pytest-doctestplus = "*"
-pytest-postgresql = "<4.0.0"  # pytest-postgresql 4.0.0 uses psycopg3, but sqlalchemy does not yet support it
+pytest-postgresql = ">=4.0.0"
 
 [tool.pytest.ini_options]
 addopts = "--doctest-glob *.md"
 doctest_plus = true
 doctest_optionflags = [
     "ELLIPSIS",
     "FLOAT_CMP"
@@ -46,8 +49,8 @@
 omit = [
     "*/conftest.py",
     "*/tests/*"
 ]
 
 [build-system]
 requires = ["poetry-core"]
-build-backend = "poetry.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `healpix_alchemy-1.0.2/PKG-INFO` & `healpix_alchemy-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: healpix-alchemy
-Version: 1.0.2
+Version: 1.1.0
 Summary: SQLAlchemy extensions for HEALPix spatially indexed astronomy data
 Home-page: https://github.com/skyportal/healpix-alchemy
 License: BSD-3-Clause
 Author: Leo Singer
 Author-email: leo.singer@ligo.org
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Dist: astropy
 Requires-Dist: astropy_healpix
 Requires-Dist: mocpy (>=0.12.2)
 Requires-Dist: sqlalchemy (>=1.4)
 Project-URL: Repository, https://github.com/skyportal/healpix-alchemy
```

