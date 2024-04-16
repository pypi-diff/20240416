# Comparing `tmp/h3ronpy-0.20.2.tar.gz` & `tmp/h3ronpy-0.9.0.tar.gz`

## Comparing `h3ronpy-0.20.2.tar` & `h3ronpy-0.9.0.tar`

### file list

```diff
@@ -1,79 +1,99 @@
--rw-r--r--   0        0        0     1313 1970-01-01 00:00:00.000000 h3ronpy-0.20.2/Cargo.toml
--rw-r--r--   0     1001      127       58 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/.gitattributes
--rw-r--r--   0     1001      127     6384 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/.github/workflows/ci.yml
--rw-r--r--   0     1001      127      225 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/.gitignore
--rw-r--r--   0     1001      127      205 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/.readthedocs.yaml
--rw-r--r--   0     1001      127     7646 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/CHANGES.rst
--rw-r--r--   0     1001      127     1435 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/CONTRIBUTING.rst
--rw-r--r--   0     1001      127     1023 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/LICENSE.txt
--rw-r--r--   0     1001      127       90 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/MANIFEST.in
--rw-r--r--   0     1001      127     4057 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/README.rst
--rw-r--r--   0     1001      127   279250 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/data/europe-and-north-africa.tif
--rw-r--r--   0     1001      127   489248 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/data/naturalearth_110m_admin_0_countries.fgb
--rw-r--r--   0     1001      127   305198 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/data/population-841fa8bffffffff.parquet
--rw-r--r--   0     1001      127    90924 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/data/r.tiff
--rw-r--r--   0     1001      127      638 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/docs/Makefile
--rw-r--r--   0     1001      127      764 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/docs/make.bat
--rw-r--r--   0     1001      127      143 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/docs/requirements.txt
--rw-r--r--   0     1001      127      296 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/docs/source/api/arrow.rst
--rw-r--r--   0     1001      127       68 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/docs/source/api/core.rst
--rw-r--r--   0     1001      127       88 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/docs/source/api/index.rst
--rw-r--r--   0     1001      127      321 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/docs/source/api/pandas.rst
--rw-r--r--   0     1001      127     2101 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/docs/source/api/polars.rst
--rw-r--r--   0     1001      127       31 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/docs/source/changelog.rst
--rw-r--r--   0     1001      127      962 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/docs/source/conf.py
--rw-r--r--   0     1001      127       36 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/docs/source/contributing.rst
--rw-r--r--   0     1001      127      229 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/docs/source/index.rst
--rw-r--r--   0     1001      127     1076 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/docs/source/installation.rst
--rw-r--r--   0     1001      127       52 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/docs/source/license.rst
--rw-r--r--   0     1001      127     1575 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/docs/source/usage/grid.rst
--rw-r--r--   0     1001      127      394 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/docs/source/usage/index.rst
--rw-r--r--   0     1001      127     3124 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/docs/source/usage/raster.rst
--rw-r--r--   0     1001      127     2630 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/docs/source/usage/vector.rst
--rw-r--r--   0     1001      127     1609 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/install-dev-dependencies.py
--rw-r--r--   0     1001      127      300 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/justfile
--rw-r--r--   0     1001      127      773 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/pyproject.toml
--rw-r--r--   0     1001      127      455 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/python/h3ronpy/__init__.py
--rw-r--r--   0     1001      127     7569 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/python/h3ronpy/arrow/__init__.py
--rw-r--r--   0     1001      127     7706 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/python/h3ronpy/arrow/raster.py
--rw-r--r--   0     1001      127      994 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/python/h3ronpy/arrow/util.py
--rw-r--r--   0     1001      127     5893 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/python/h3ronpy/arrow/vector.py
--rw-r--r--   0     1001      127     3288 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/python/h3ronpy/pandas/__init__.py
--rw-r--r--   0     1001      127     1898 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/python/h3ronpy/pandas/raster.py
--rw-r--r--   0     1001      127     5076 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/python/h3ronpy/pandas/vector.py
--rw-r--r--   0     1001      127     8433 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/python/h3ronpy/polars/__init__.py
--rw-r--r--   0     1001      127      407 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/python/h3ronpy/polars/raster.py
--rw-r--r--   0     1001      127     1005 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/python/h3ronpy/polars/vector.py
--rw-r--r--   0     1001      127     2089 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/src/arrow_interop.rs
--rw-r--r--   0     1001      127     2910 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/src/error.rs
--rw-r--r--   0     1001      127     1607 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/src/lib.rs
--rw-r--r--   0     1001      127     1001 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/src/op/compact.rs
--rw-r--r--   0     1001      127      873 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/src/op/measure.rs
--rw-r--r--   0     1001      127     1716 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/src/op/mod.rs
--rw-r--r--   0     1001      127     4191 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/src/op/neighbor.rs
--rw-r--r--   0     1001      127     2314 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/src/op/resolution.rs
--rw-r--r--   0     1001      127     4121 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/src/op/string.rs
--rw-r--r--   0     1001      127     1476 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/src/op/valid.rs
--rw-r--r--   0     1001      127     8109 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/src/raster.rs
--rw-r--r--   0     1001      127     1508 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/src/transform.rs
--rw-r--r--   0     1001      127    14192 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/src/vector.rs
--rw-r--r--   0     1001      127      279 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/tests/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/tests/arrow/__init__.py
--rw-r--r--   0     1001      127      726 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/tests/arrow/test_vector.py
--rw-r--r--   0     1001      127        0 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/tests/pandas/__init__.py
--rw-r--r--   0     1001      127     1715 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/tests/pandas/test_raster.py
--rw-r--r--   0     1001      127     1553 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/tests/pandas/test_resolution.py
--rw-r--r--   0     1001      127     4084 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/tests/pandas/test_vector.py
--rw-r--r--   0     1001      127      267 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/tests/polars/__init__.py
--rw-r--r--   0     1001      127      747 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/tests/polars/test_benches.py
--rw-r--r--   0     1001      127     1055 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/tests/polars/test_compact.py
--rw-r--r--   0     1001      127     2177 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/tests/polars/test_coordinates.py
--rw-r--r--   0     1001      127      850 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/tests/polars/test_expr.py
--rw-r--r--   0     1001      127      541 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/tests/polars/test_measure.py
--rw-r--r--   0     1001      127     2410 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/tests/polars/test_neighbor.py
--rw-r--r--   0     1001      127     2726 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/tests/polars/test_raster.py
--rw-r--r--   0     1001      127      280 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/tests/polars/test_series.py
--rw-r--r--   0     1001      127     1809 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/tests/polars/test_utf8.py
--rw-r--r--   0     1001      127      211 2024-04-16 17:47:59.000000 h3ronpy-0.20.2/tests/test_transform.py
--rw-r--r--   0     1001      127    48959 2024-04-16 17:48:10.000000 h3ronpy-0.20.2/Cargo.lock
--rw-r--r--   0        0        0     5063 1970-01-01 00:00:00.000000 h3ronpy-0.20.2/PKG-INFO
+-rw-r--r--   0        0        0      734 1970-01-01 00:00:00.000000 h3ronpy-0.9.0/local_dependencies/h3ron/Cargo.toml
+-rw-rw-r--   0     1000     1000     3843 2021-04-08 12:23:38.000000 h3ronpy-0.9.0/local_dependencies/h3ron/src/algorithm.rs
+-rw-rw-r--   0     1000     1000    13471 2021-04-08 12:23:38.000000 h3ronpy-0.9.0/local_dependencies/h3ron/src/collections.rs
+-rw-rw-r--   0     1000     1000     1618 2021-04-05 19:34:20.000000 h3ronpy-0.9.0/local_dependencies/h3ron/src/error.rs
+-rw-rw-r--   0     1000     1000     2594 2021-04-11 12:23:33.000000 h3ronpy-0.9.0/local_dependencies/h3ron/src/experimental.rs
+-rw-rw-r--   0     1000     1000    16161 2021-04-08 12:24:15.000000 h3ronpy-0.9.0/local_dependencies/h3ron/src/index.rs
+-rw-rw-r--   0     1000     1000     6872 2021-04-08 12:23:38.000000 h3ronpy-0.9.0/local_dependencies/h3ron/src/lib.rs
+-rw-rw-r--   0     1000     1000     7546 2021-04-08 12:23:38.000000 h3ronpy-0.9.0/local_dependencies/h3ron/src/to_geo.rs
+-rw-rw-r--   0     1000     1000     4307 2021-04-08 12:23:38.000000 h3ronpy-0.9.0/local_dependencies/h3ron/src/to_h3.rs
+-rw-rw-r--   0     1000     1000      999 2021-04-05 19:34:20.000000 h3ronpy-0.9.0/local_dependencies/h3ron/src/util.rs
+-rw-r--r--   0        0        0      637 1970-01-01 00:00:00.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/Cargo.toml
+-rw-rw-r--   0     1000     1000      410 2021-03-05 18:52:26.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/README.md
+-rw-rw-r--   0     1000     1000     2058 2021-04-08 12:23:38.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/build.rs
+-rw-rw-r--   0     1000     1000       36 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/.clang-format
+-rw-rw-r--   0     1000     1000     1135 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/.clang-tidy
+-rw-rw-r--   0     1000     1000     1374 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/.gitignore
+-rw-rw-r--   0     1000     1000     1799 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/.travis.yml
+-rw-rw-r--   0     1000     1000     8707 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/CHANGELOG.md
+-rw-rw-r--   0     1000     1000    29799 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/CMakeLists.txt
+-rw-rw-r--   0     1000     1000     1483 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/CONTRIBUTING.md
+-rw-rw-r--   0     1000     1000     7611 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/KML/icosa.kml
+-rw-rw-r--   0     1000     1000    11354 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/LICENSE
+-rw-rw-r--   0     1000     1000     7575 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/README.md
+-rw-rw-r--   0     1000     1000      593 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/RELEASE.md
+-rw-rw-r--   0     1000     1000        6 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/VERSION
+-rw-rw-r--   0     1000     1000      125 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/cmake/Config.cmake.in
+-rw-rw-r--   0     1000     1000     1403 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/cmake/TestWrapValgrind.cmake
+-rw-rw-r--   0     1000     1000      643 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/cmake/toolchain.cmake
+-rw-rw-r--   0     1000     1000      966 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/scripts/binding_functions.ps1
+-rwxrwxr-x   0     1000     1000      945 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/scripts/binding_functions.sh
+-rwxrwxr-x   0     1000     1000     2364 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/scripts/coverage.sh.in
+-rwxrwxr-x   0     1000     1000      931 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/scripts/publish_website.sh
+-rwxrwxr-x   0     1000     1000     1761 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/scripts/update_version.sh
+-rw-rw-r--   0     1000     1000     1791 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/algos.h
+-rw-rw-r--   0     1000     1000     1286 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/alloc.h
+-rw-rw-r--   0     1000     1000     2114 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/baseCells.h
+-rw-rw-r--   0     1000     1000     1400 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/bbox.h
+-rw-rw-r--   0     1000     1000     2470 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/constants.h
+-rw-rw-r--   0     1000     1000     3744 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/coordijk.h
+-rw-rw-r--   0     1000     1000     3055 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/faceijk.h
+-rw-rw-r--   0     1000     1000     1588 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/geoCoord.h
+-rw-rw-r--   0     1000     1000     6091 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/h3Index.h
+-rw-rw-r--   0     1000     1000      841 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/h3UniEdge.h
+-rw-rw-r--   0     1000     1000    19625 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/h3api.h.in
+-rw-rw-r--   0     1000     1000     3343 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/linkedGeo.h
+-rw-rw-r--   0     1000     1000      902 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/localij.h
+-rw-rw-r--   0     1000     1000      955 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/mathExtensions.h
+-rw-rw-r--   0     1000     1000     2469 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/polygon.h
+-rw-rw-r--   0     1000     1000     7049 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/polygonAlgos.h
+-rw-rw-r--   0     1000     1000     1126 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/vec2d.h
+-rw-rw-r--   0     1000     1000     1042 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/vec3d.h
+-rw-rw-r--   0     1000     1000     1400 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/vertex.h
+-rw-rw-r--   0     1000     1000     2022 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/vertexGraph.h
+-rw-rw-r--   0     1000     1000    41264 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/lib/algos.c
+-rw-rw-r--   0     1000     1000    37442 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/lib/baseCells.c
+-rw-rw-r--   0     1000     1000     5538 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/lib/bbox.c
+-rw-rw-r--   0     1000     1000    13648 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/lib/coordijk.c
+-rw-rw-r--   0     1000     1000    33881 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/lib/faceijk.c
+-rw-rw-r--   0     1000     1000    12511 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/lib/geoCoord.c
+-rw-rw-r--   0     1000     1000    34041 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/lib/h3Index.c
+-rw-rw-r--   0     1000     1000     9668 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/lib/h3UniEdge.c
+-rw-rw-r--   0     1000     1000    12599 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/lib/linkedGeo.c
+-rw-rw-r--   0     1000     1000    23670 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/lib/localij.c
+-rw-rw-r--   0     1000     1000     1177 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/lib/mathExtensions.c
+-rw-rw-r--   0     1000     1000     2700 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/lib/polygon.c
+-rw-rw-r--   0     1000     1000     2127 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/lib/vec2d.c
+-rw-rw-r--   0     1000     1000     1608 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/lib/vec3d.c
+-rw-rw-r--   0     1000     1000     4930 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/lib/vertex.c
+-rw-rw-r--   0     1000     1000     7267 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/lib/vertexGraph.c
+-rw-rw-r--   0     1000     1000      298 2021-03-05 18:52:26.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/src/lib.rs
+-rw-r--r--   0        0        0      812 1970-01-01 00:00:00.000000 h3ronpy-0.9.0/local_dependencies/h3ron-ndarray/Cargo.toml
+-rw-rw-r--   0     1000     1000      434 2021-03-05 18:52:26.000000 h3ronpy-0.9.0/local_dependencies/h3ron-ndarray/README.md
+-rw-rw-r--   0     1000     1000     1546 2021-04-05 19:35:37.000000 h3ronpy-0.9.0/local_dependencies/h3ron-ndarray/benches/convert_dataset_r.rs
+-rw-rw-r--   0     1000     1000     2347 2021-04-05 19:35:42.000000 h3ronpy-0.9.0/local_dependencies/h3ron-ndarray/examples/h3ify_r_tiff.rs
+-rw-rw-r--   0     1000     1000    13670 2021-04-09 19:08:10.000000 h3ronpy-0.9.0/local_dependencies/h3ron-ndarray/src/array.rs
+-rw-rw-r--   0     1000     1000      517 2021-04-05 18:44:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-ndarray/src/error.rs
+-rw-rw-r--   0     1000     1000      788 2021-04-05 19:35:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-ndarray/src/lib.rs
+-rw-rw-r--   0     1000     1000     3840 2021-04-08 12:23:38.000000 h3ronpy-0.9.0/local_dependencies/h3ron-ndarray/src/resolution.rs
+-rw-rw-r--   0     1000     1000     1521 2021-04-05 19:35:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-ndarray/src/sphere.rs
+-rw-rw-r--   0     1000     1000     6369 2021-04-05 19:35:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-ndarray/src/transform.rs
+-rw-r--r--   0        0        0     1298 1970-01-01 00:00:00.000000 h3ronpy-0.9.0/Cargo.toml
+-rw-rw-r--   0     1000     1000     1023 2021-04-11 18:37:21.000000 h3ronpy-0.9.0/LICENSE.txt
+-rw-rw-r--   0     1000     1000     2581 2021-04-11 18:37:21.000000 h3ronpy-0.9.0/README.md
+-rw-rw-r--   0     1000     1000  2088546 2021-04-09 19:04:30.000000 h3ronpy-0.9.0/documentation.ipynb
+-rw-rw-r--   0     1000     1000      143 2021-04-09 19:04:30.000000 h3ronpy-0.9.0/h3ronpy/__init__.py
+-rw-rw-r--   0     1000     1000     3951 2021-04-09 19:04:30.000000 h3ronpy-0.9.0/h3ronpy/raster.py
+-rw-rw-r--   0     1000     1000     1245 2021-04-09 19:04:30.000000 h3ronpy-0.9.0/h3ronpy/util.py
+-rw-rw-r--   0     1000     1000     3208 2021-04-09 19:04:30.000000 h3ronpy-0.9.0/h3ronpy/vector.py
+-rw-rw-r--   0     1000     1000       78 2021-04-11 18:27:47.000000 h3ronpy-0.9.0/pyproject.toml
+-rw-rw-r--   0     1000     1000       16 2021-04-11 17:31:34.000000 h3ronpy-0.9.0/requirements.dev.txt
+-rw-rw-r--   0     1000     1000       62 2021-03-05 18:52:26.000000 h3ronpy-0.9.0/requirements.documentation.txt
+-rw-rw-r--   0     1000     1000     1780 2021-04-09 19:12:10.000000 h3ronpy-0.9.0/src/collections.rs
+-rw-rw-r--   0     1000     1000     1458 2021-04-05 19:36:14.000000 h3ronpy-0.9.0/src/error.rs
+-rw-rw-r--   0     1000     1000     1057 2021-04-09 19:07:16.000000 h3ronpy-0.9.0/src/lib.rs
+-rw-rw-r--   0     1000     1000     2197 2021-04-09 19:10:54.000000 h3ronpy-0.9.0/src/polygon.rs
+-rw-rw-r--   0     1000     1000     5446 2021-04-09 19:04:30.000000 h3ronpy-0.9.0/src/raster.rs
+-rw-rw-r--   0     1000     1000     1535 2021-04-05 19:36:15.000000 h3ronpy-0.9.0/src/transform.rs
+-rw-rw-r--   0     1000     1000     2658 2021-04-09 19:13:17.000000 h3ronpy-0.9.0/src/vector.rs
+-rw-r--r--   0        0        0     3176 1970-01-01 00:00:00.000000 h3ronpy-0.9.0/PKG-INFO
```

### Comparing `h3ronpy-0.20.2/LICENSE.txt` & `h3ronpy-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `h3ronpy-0.20.2/src/lib.rs` & `h3ronpy-0.9.0/src/lib.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,65 +1,39 @@
-#![warn(
-    clippy::all,
-    clippy::correctness,
-    clippy::suspicious,
-    clippy::style,
-    clippy::complexity,
-    clippy::perf,
-    nonstandard_style
-)]
+use pyo3::{prelude::*, wrap_pyfunction, PyNativeType, Python};
 
-use pyo3::{prelude::*, wrap_pyfunction, Python};
-
-use crate::op::init_op_submodule;
 use crate::raster::init_raster_submodule;
-use crate::vector::{init_vector_submodule, PyContainmentMode};
+use crate::vector::init_vector_submodule;
+use crate::{collections::H3CompactedVec, polygon::Polygon};
 
-mod arrow_interop;
+mod collections;
 mod error;
-mod op;
+mod polygon;
 mod raster;
 mod transform;
 mod vector;
 
-pub(crate) const DEFAULT_CELL_COLUMN_NAME: &str = "cell";
-
 /// version of the module
 #[pyfunction]
 fn version() -> String {
     env!("CARGO_PKG_VERSION").to_string()
 }
 
-/// indicates if this extension has been compiled in release-mode
-#[pyfunction]
-fn is_release_build() -> bool {
-    #[cfg(debug_assertions)]
-    return false;
-
-    #[cfg(not(debug_assertions))]
-    return true;
-}
-
+/// h3ron python bindings
 #[pymodule]
-fn h3ronpyrs(py: Python<'_>, m: &PyModule) -> PyResult<()> {
+fn h3ronpy(py: Python<'_>, m: &PyModule) -> PyResult<()> {
     env_logger::init(); // run with the environment variable RUST_LOG set to "debug" for log output
 
-    m.add_class::<PyContainmentMode>()?;
-    m.add_function(wrap_pyfunction!(version, m)?)?;
-    m.add_function(wrap_pyfunction!(is_release_build, m)?)?;
+    m.add("H3CompactedVec", m.py().get_type::<H3CompactedVec>())?;
+    m.add("Polygon", m.py().get_type::<Polygon>())?;
 
-    let raster_submod = PyModule::new(py, "raster")?;
-    init_raster_submodule(raster_submod)?;
-    m.add_submodule(raster_submod)?;
-
-    let op_submod = PyModule::new(py, "op")?;
-    init_op_submodule(op_submod)?;
-    m.add_submodule(op_submod)?;
+    m.add_function(wrap_pyfunction!(version, m)?)?;
 
     let vector_submod = PyModule::new(py, "vector")?;
     init_vector_submodule(vector_submod)?;
-    m.add_submodule(vector_submod)?;
+    m.add_submodule(&vector_submod)?;
 
-    m.add("DEFAULT_CELL_COLUMN_NAME", DEFAULT_CELL_COLUMN_NAME)?;
+    let raster_submod = PyModule::new(py, "raster")?;
+    init_raster_submodule(raster_submod)?;
+    m.add_submodule(&raster_submod)?;
 
     Ok(())
 }
```

