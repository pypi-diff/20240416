# Comparing `tmp/streamjoy-0.0.7.tar.gz` & `tmp/streamjoy-0.0.8.tar.gz`

## Comparing `streamjoy-0.0.7.tar` & `streamjoy-0.0.8.tar`

### file list

```diff
@@ -1,77 +1,78 @@
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 streamjoy-0.0.7/.editorconfig
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 streamjoy-0.0.7/CONTRIBUTING.md
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 streamjoy-0.0.7/HOWTOCONTRIBUTE.md
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 streamjoy-0.0.7/HOWTORELEASE.md
--rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 streamjoy-0.0.7/mkdocs.yml
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 streamjoy-0.0.7/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 streamjoy-0.0.7/.github/workflows/build.yml
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 streamjoy-0.0.7/.github/workflows/documentation.yml
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 streamjoy-0.0.7/.github/workflows/release.yml
--rw-r--r--   0        0        0     7033 2020-02-02 00:00:00.000000 streamjoy-0.0.7/docs/how_do_i.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 streamjoy-0.0.7/docs/index.md
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 streamjoy-0.0.7/docs/package_design.md
--rw-r--r--   0        0        0     4954 2020-02-02 00:00:00.000000 streamjoy-0.0.7/docs/supported_formats.md
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 streamjoy-0.0.7/docs/api_reference/core.md
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 streamjoy-0.0.7/docs/api_reference/models.md
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 streamjoy-0.0.7/docs/api_reference/renderers.md
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 streamjoy-0.0.7/docs/api_reference/settings.md
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 streamjoy-0.0.7/docs/api_reference/streams.md
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 streamjoy-0.0.7/docs/api_reference/wrappers.md
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 streamjoy-0.0.7/docs/example_recipes/air_temperature.md
--rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 streamjoy-0.0.7/docs/example_recipes/co2_timeseries.md
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 streamjoy-0.0.7/docs/example_recipes/gender_gapminder.md
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 streamjoy-0.0.7/docs/example_recipes/nice_orbit.md
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 streamjoy-0.0.7/docs/example_recipes/oisst_globe.md
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 streamjoy-0.0.7/docs/example_recipes/sea_ice.md
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 streamjoy-0.0.7/docs/example_recipes/sine_wave.md
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 streamjoy-0.0.7/docs/example_recipes/stream_code.md
--rw-r--r--   0        0        0     4128 2020-02-02 00:00:00.000000 streamjoy-0.0.7/docs/example_recipes/temperature_anomaly.md
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 streamjoy-0.0.7/docs/stylesheets/extra.css
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 streamjoy-0.0.7/streamjoy/.gitignore
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 streamjoy-0.0.7/streamjoy/__init__.py
--rw-r--r--   0        0        0    11727 2020-02-02 00:00:00.000000 streamjoy-0.0.7/streamjoy/_utils.py
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 streamjoy-0.0.7/streamjoy/core.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 streamjoy-0.0.7/streamjoy/models.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 streamjoy-0.0.7/streamjoy/pandas.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 streamjoy-0.0.7/streamjoy/polars.py
--rw-r--r--   0        0        0     4323 2020-02-02 00:00:00.000000 streamjoy-0.0.7/streamjoy/renderers.py
--rw-r--r--   0        0        0    22823 2020-02-02 00:00:00.000000 streamjoy-0.0.7/streamjoy/serializers.py
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 streamjoy-0.0.7/streamjoy/settings.py
--rw-r--r--   0        0        0    41748 2020-02-02 00:00:00.000000 streamjoy-0.0.7/streamjoy/streams.py
--rw-r--r--   0        0        0     5495 2020-02-02 00:00:00.000000 streamjoy-0.0.7/streamjoy/wrappers.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 streamjoy-0.0.7/streamjoy/xarray.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streamjoy-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 streamjoy-0.0.7/tests/conftest.py
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 streamjoy-0.0.7/tests/test_core.py
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 streamjoy-0.0.7/tests/test_models.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 streamjoy-0.0.7/tests/test_pandas.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 streamjoy-0.0.7/tests/test_polars.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 streamjoy-0.0.7/tests/test_renderers.py
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 streamjoy-0.0.7/tests/test_serializers.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 streamjoy-0.0.7/tests/test_settings.py
--rw-r--r--   0        0        0     5134 2020-02-02 00:00:00.000000 streamjoy-0.0.7/tests/test_streams.py
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 streamjoy-0.0.7/tests/test_wrappers.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 streamjoy-0.0.7/tests/test_xarray.py
--rw-r--r--   0        0        0    71503 2020-02-02 00:00:00.000000 streamjoy-0.0.7/tests/data/air.nc
--rw-r--r--   0        0        0     3685 2020-02-02 00:00:00.000000 streamjoy-0.0.7/tests/data/gapminder.csv
--rw-r--r--   0        0        0     8986 2020-02-02 00:00:00.000000 streamjoy-0.0.7/tests/data/gapminder.parquet
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 streamjoy-0.0.7/tests/data/air.zarr/.zattrs
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 streamjoy-0.0.7/tests/data/air.zarr/.zgroup
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 streamjoy-0.0.7/tests/data/air.zarr/.zmetadata
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 streamjoy-0.0.7/tests/data/air.zarr/air/.zarray
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 streamjoy-0.0.7/tests/data/air.zarr/air/.zattrs
--rw-r--r--   0        0        0    43023 2020-02-02 00:00:00.000000 streamjoy-0.0.7/tests/data/air.zarr/air/0.0.0
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 streamjoy-0.0.7/tests/data/air.zarr/lat/.zarray
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 streamjoy-0.0.7/tests/data/air.zarr/lat/.zattrs
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 streamjoy-0.0.7/tests/data/air.zarr/lat/0
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 streamjoy-0.0.7/tests/data/air.zarr/lon/.zarray
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 streamjoy-0.0.7/tests/data/air.zarr/lon/.zattrs
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 streamjoy-0.0.7/tests/data/air.zarr/lon/0
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 streamjoy-0.0.7/tests/data/air.zarr/time/.zarray
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 streamjoy-0.0.7/tests/data/air.zarr/time/.zattrs
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 streamjoy-0.0.7/tests/data/air.zarr/time/0
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 streamjoy-0.0.7/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 streamjoy-0.0.7/LICENSE
--rw-r--r--   0        0        0     6597 2020-02-02 00:00:00.000000 streamjoy-0.0.7/README.md
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 streamjoy-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 streamjoy-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 streamjoy-0.0.8/.editorconfig
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 streamjoy-0.0.8/CONTRIBUTING.md
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 streamjoy-0.0.8/HOWTOCONTRIBUTE.md
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 streamjoy-0.0.8/HOWTORELEASE.md
+-rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 streamjoy-0.0.8/mkdocs.yml
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 streamjoy-0.0.8/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 streamjoy-0.0.8/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 streamjoy-0.0.8/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 streamjoy-0.0.8/.github/workflows/release.yml
+-rw-r--r--   0        0        0     7033 2020-02-02 00:00:00.000000 streamjoy-0.0.8/docs/how_do_i.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 streamjoy-0.0.8/docs/index.md
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 streamjoy-0.0.8/docs/package_design.md
+-rw-r--r--   0        0        0     4954 2020-02-02 00:00:00.000000 streamjoy-0.0.8/docs/supported_formats.md
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 streamjoy-0.0.8/docs/api_reference/core.md
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 streamjoy-0.0.8/docs/api_reference/models.md
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 streamjoy-0.0.8/docs/api_reference/renderers.md
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 streamjoy-0.0.8/docs/api_reference/settings.md
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 streamjoy-0.0.8/docs/api_reference/streams.md
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 streamjoy-0.0.8/docs/api_reference/wrappers.md
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 streamjoy-0.0.8/docs/example_recipes/air_temperature.md
+-rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 streamjoy-0.0.8/docs/example_recipes/co2_timeseries.md
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 streamjoy-0.0.8/docs/example_recipes/gender_gapminder.md
+-rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 streamjoy-0.0.8/docs/example_recipes/nice_orbit.md
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 streamjoy-0.0.8/docs/example_recipes/nmme_forecast.md
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 streamjoy-0.0.8/docs/example_recipes/oisst_globe.md
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 streamjoy-0.0.8/docs/example_recipes/sea_ice.md
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 streamjoy-0.0.8/docs/example_recipes/sine_wave.md
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 streamjoy-0.0.8/docs/example_recipes/stream_code.md
+-rw-r--r--   0        0        0     4128 2020-02-02 00:00:00.000000 streamjoy-0.0.8/docs/example_recipes/temperature_anomaly.md
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 streamjoy-0.0.8/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 streamjoy-0.0.8/streamjoy/.gitignore
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 streamjoy-0.0.8/streamjoy/__init__.py
+-rw-r--r--   0        0        0    11727 2020-02-02 00:00:00.000000 streamjoy-0.0.8/streamjoy/_utils.py
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 streamjoy-0.0.8/streamjoy/core.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 streamjoy-0.0.8/streamjoy/models.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 streamjoy-0.0.8/streamjoy/pandas.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 streamjoy-0.0.8/streamjoy/polars.py
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 streamjoy-0.0.8/streamjoy/renderers.py
+-rw-r--r--   0        0        0    22823 2020-02-02 00:00:00.000000 streamjoy-0.0.8/streamjoy/serializers.py
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 streamjoy-0.0.8/streamjoy/settings.py
+-rw-r--r--   0        0        0    44179 2020-02-02 00:00:00.000000 streamjoy-0.0.8/streamjoy/streams.py
+-rw-r--r--   0        0        0     5495 2020-02-02 00:00:00.000000 streamjoy-0.0.8/streamjoy/wrappers.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 streamjoy-0.0.8/streamjoy/xarray.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streamjoy-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 streamjoy-0.0.8/tests/conftest.py
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 streamjoy-0.0.8/tests/test_core.py
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 streamjoy-0.0.8/tests/test_models.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 streamjoy-0.0.8/tests/test_pandas.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 streamjoy-0.0.8/tests/test_polars.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 streamjoy-0.0.8/tests/test_renderers.py
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 streamjoy-0.0.8/tests/test_serializers.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 streamjoy-0.0.8/tests/test_settings.py
+-rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 streamjoy-0.0.8/tests/test_streams.py
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 streamjoy-0.0.8/tests/test_wrappers.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 streamjoy-0.0.8/tests/test_xarray.py
+-rw-r--r--   0        0        0    71503 2020-02-02 00:00:00.000000 streamjoy-0.0.8/tests/data/air.nc
+-rw-r--r--   0        0        0     3685 2020-02-02 00:00:00.000000 streamjoy-0.0.8/tests/data/gapminder.csv
+-rw-r--r--   0        0        0     8986 2020-02-02 00:00:00.000000 streamjoy-0.0.8/tests/data/gapminder.parquet
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 streamjoy-0.0.8/tests/data/air.zarr/.zattrs
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 streamjoy-0.0.8/tests/data/air.zarr/.zgroup
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 streamjoy-0.0.8/tests/data/air.zarr/.zmetadata
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 streamjoy-0.0.8/tests/data/air.zarr/air/.zarray
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 streamjoy-0.0.8/tests/data/air.zarr/air/.zattrs
+-rw-r--r--   0        0        0    43023 2020-02-02 00:00:00.000000 streamjoy-0.0.8/tests/data/air.zarr/air/0.0.0
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 streamjoy-0.0.8/tests/data/air.zarr/lat/.zarray
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 streamjoy-0.0.8/tests/data/air.zarr/lat/.zattrs
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 streamjoy-0.0.8/tests/data/air.zarr/lat/0
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 streamjoy-0.0.8/tests/data/air.zarr/lon/.zarray
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 streamjoy-0.0.8/tests/data/air.zarr/lon/.zattrs
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 streamjoy-0.0.8/tests/data/air.zarr/lon/0
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 streamjoy-0.0.8/tests/data/air.zarr/time/.zarray
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 streamjoy-0.0.8/tests/data/air.zarr/time/.zattrs
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 streamjoy-0.0.8/tests/data/air.zarr/time/0
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 streamjoy-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 streamjoy-0.0.8/LICENSE
+-rw-r--r--   0        0        0     6597 2020-02-02 00:00:00.000000 streamjoy-0.0.8/README.md
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 streamjoy-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 streamjoy-0.0.8/PKG-INFO
```

### Comparing `streamjoy-0.0.7/CONTRIBUTING.md` & `streamjoy-0.0.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/HOWTOCONTRIBUTE.md` & `streamjoy-0.0.8/HOWTOCONTRIBUTE.md`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/mkdocs.yml` & `streamjoy-0.0.8/mkdocs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,15 @@
         - CO2 timeseries: example_recipes/co2_timeseries.md
         - Temperature anomaly: example_recipes/temperature_anomaly.md
         - Sea ice: example_recipes/sea_ice.md
         - OISST globe: example_recipes/oisst_globe.md
         - Gender gapminder: example_recipes/gender_gapminder.md
         - Stream code: example_recipes/stream_code.md
         - Nice orbit: example_recipes/nice_orbit.md
+        - NMME forecast: example_recipes/nmme_forecast.md
     - API reference:
         - Core: api_reference/core.md
         - Models: api_reference/models.md
         - Streams: api_reference/streams.md
         - Renderers: api_reference/renderers.md
         - Wrappers: api_reference/wrappers.md
         - Settings: api_reference/settings.md
```

### Comparing `streamjoy-0.0.7/.github/workflows/build.yml` & `streamjoy-0.0.8/.github/workflows/build.yml`

 * *Files 19% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 
 jobs:
   test:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python_version: ['3.9']
+        python_version: ['3.10']
 
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python
       uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python_version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install hatch
         hatch env create
-    - name: Lint and typecheck
-      run: |
-        hatch run lint-check
+    # - name: Lint and typecheck
+    #   run: |
+    #     hatch run lint-check
     - name: Test
       run: |
         hatch run test-cov-xml
     - uses: codecov/codecov-action@v4
       with:
         token: ${{ secrets.CODECOV_TOKEN }}
         fail_ci_if_error: true
```

### Comparing `streamjoy-0.0.7/.github/workflows/documentation.yml` & `streamjoy-0.0.8/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/.github/workflows/release.yml` & `streamjoy-0.0.8/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/docs/how_do_i.md` & `streamjoy-0.0.8/docs/how_do_i.md`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/docs/package_design.md` & `streamjoy-0.0.8/docs/package_design.md`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/docs/supported_formats.md` & `streamjoy-0.0.8/docs/supported_formats.md`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/docs/api_reference/settings.md` & `streamjoy-0.0.8/docs/api_reference/settings.md`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/docs/example_recipes/air_temperature.md` & `streamjoy-0.0.8/docs/example_recipes/air_temperature.md`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/docs/example_recipes/co2_timeseries.md` & `streamjoy-0.0.8/docs/example_recipes/co2_timeseries.md`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/docs/example_recipes/gender_gapminder.md` & `streamjoy-0.0.8/docs/example_recipes/gender_gapminder.md`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/docs/example_recipes/nice_orbit.md` & `streamjoy-0.0.8/docs/example_recipes/nice_orbit.md`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/docs/example_recipes/oisst_globe.md` & `streamjoy-0.0.8/docs/example_recipes/oisst_globe.md`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/docs/example_recipes/sea_ice.md` & `streamjoy-0.0.8/docs/example_recipes/sea_ice.md`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/docs/example_recipes/sine_wave.md` & `streamjoy-0.0.8/docs/example_recipes/sine_wave.md`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/docs/example_recipes/stream_code.md` & `streamjoy-0.0.8/docs/example_recipes/stream_code.md`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/docs/example_recipes/temperature_anomaly.md` & `streamjoy-0.0.8/docs/example_recipes/temperature_anomaly.md`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/streamjoy/__init__.py` & `streamjoy-0.0.8/streamjoy/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     default_pandas_renderer,
     default_xarray_renderer,
 )
 from .settings import config, file_handlers, obj_handlers
 from .streams import GifStream, HtmlStream, Mp4Stream
 from .wrappers import wrap_holoviews, wrap_matplotlib
 
-__version__ = "0.0.7"
+__version__ = "0.0.8"
 
 __all__ = [
     "GifStream",
     "HtmlStream",
     "ImageText",
     "Mp4Stream",
     "Paused",
```

### Comparing `streamjoy-0.0.7/streamjoy/_utils.py` & `streamjoy-0.0.8/streamjoy/_utils.py`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/streamjoy/core.py` & `streamjoy-0.0.8/streamjoy/core.py`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/streamjoy/models.py` & `streamjoy-0.0.8/streamjoy/models.py`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/streamjoy/polars.py` & `streamjoy-0.0.8/streamjoy/polars.py`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/streamjoy/renderers.py` & `streamjoy-0.0.8/streamjoy/renderers.py`

 * *Files 3% similar despite different names*

```diff
@@ -159,10 +159,18 @@
         if vdim in clims:
             hv_el.opts(clim=clims[vdim], backend=backend)
 
     if backend == "bokeh":
         kwargs["toolbar"] = None
     elif backend == "matplotlib":
         kwargs["cbar_extend"] = kwargs.get("cbar_extend", "both")
-    hv_obj.opts(**kwargs)
+
+    if isinstance(hv_obj, hv.Overlay):
+        for hv_el in hv_obj:
+            try:
+                hv_el.opts(**kwargs)
+            except Exception:
+                pass
+    else:
+        hv_obj.opts(**kwargs)
 
     return hv_obj
```

### Comparing `streamjoy-0.0.7/streamjoy/serializers.py` & `streamjoy-0.0.8/streamjoy/serializers.py`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/streamjoy/settings.py` & `streamjoy-0.0.8/streamjoy/settings.py`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/streamjoy/streams.py` & `streamjoy-0.0.8/streamjoy/streams.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from textwrap import indent
 from typing import TYPE_CHECKING, Any, Callable
 
 import dask.delayed
 import imageio.v3 as iio
 import numpy as np
 import param
+from dask.diagnostics import ProgressBar
 from dask.distributed import Client, Future, fire_and_forget
 from imageio.core.v3_plugin_api import PluginV3
 from PIL import Image, ImageDraw
 
 from . import _utils
 from .models import ImageText, Paused
 from .serializers import (
@@ -164,14 +165,19 @@
 
     threads_per_worker = param.Integer(
         default=None,
         bounds=(1, None),
         doc="The number of threads to use per worker.",
     )
 
+    show_progress = param.Boolean(
+        default=True,
+        doc="Whether to show the progress bar when rendering.",
+    )
+
     scratch_dir = param.Path(
         doc="The directory to use for temporary files.", check_exists=False
     )
 
     in_memory = param.Boolean(
         doc="Whether to store intermediate results in memory.",
     )
@@ -197,14 +203,15 @@
         # forward non recognized params to _tbd_kwargs
         params["_tbd_kwargs"] = {}
         for param_key in set(params):
             if param_key not in self.param:
                 params["_tbd_kwargs"][param_key] = params.pop(param_key)
 
         super().__init__(**params)
+        self._progress_bar = ProgressBar(minimum=3 if self.show_progress else np.inf)
 
     @classmethod
     def from_numpy(
         cls,
         array: np.ndarray,
         renderer: Callable | None = None,
         renderer_iterables: list[Any] | None = None,
@@ -412,15 +419,15 @@
             resource_0 = _utils.get_result(_utils.get_first(resources))
         except Exception as exc:
             raise ValueError(
                 f"The resources must be set in the class or passed to write; "
                 f"got {resources=!r}."
             ) from exc
 
-        if renderer:
+        if renderer and not renderer.__name__.startswith("default"):
             try:
                 iterable_0 = [iterable[0] for iterable in renderer_iterables]
                 renderer(resource_0, *iterable_0, **renderer_kwargs)
             except Exception as exc:
                 raise exc
 
         batch_size = self.batch_size
@@ -442,15 +449,16 @@
             )
         elif renderer and not self.processes:
             renderer = dask.delayed(renderer)
             jobs = [
                 renderer(resource, *iterable, **renderer_kwargs)
                 for resource, *iterable in zip_longest(resources, *renderer_iterables)
             ]
-            resources = dask.compute(jobs, scheduler="threads")[0]
+            with self._progress_bar:
+                resources = dask.compute(jobs, scheduler="threads")[0]
         resource_0 = _utils.get_result(_utils.get_first(resources))
 
         is_like_image = isinstance(resource_0, np.ndarray) and resource_0.ndim == 3
         if not is_like_image:
             try:
                 _utils.imread_with_pause(resource_0, fsspec_fs=self.fsspec_fs)
             except Exception as exc:
@@ -779,14 +787,17 @@
         """
         init = write_kwargs.pop("init", True)
         init_kwargs = _utils.pop_kwargs(buf.init_video_stream, write_kwargs)
         if init:
             init_kwargs["fps"] = self.fps
             buf.init_video_stream(self.codec, **init_kwargs)
 
+        if "crf" in write_kwargs:
+            buf._video_stream.options = {"crf": str(write_kwargs.pop("crf"))}
+
         intro_frame = self._create_intro(images)
         self._prepend_intro(buf, intro_frame, **write_kwargs)
 
         for i, image in enumerate(images):
             image = _utils.get_result(image)
 
             pause = None
@@ -1043,14 +1054,32 @@
         stream = self.materialize(uri, extension)
         return stream.write(uri=uri, resources=resources, **kwargs)
 
 
 class HtmlStream(MediaStream):
     _extension = ".html"
 
+    width = param.Integer(default=None, bounds=(1, None), doc="The width of the image.")
+    height = param.Integer(
+        default=None, bounds=(1, None), doc="The height of the image."
+    )
+    sizing_mode = param.Selector(
+        default="scale_width",
+        objects=[
+            "fixed",
+            "stretch_width",
+            "stretch_height",
+            "stretch_both",
+            "scale_width",
+            "scale_height",
+            "scale_both",
+        ],
+        doc="The sizing mode of the image.",
+    )
+
     def __init__(self, **params) -> None:
         import panel as pn
 
         pn.extension()
         super().__init__(**params)
         self._column = pn.Column()
 
@@ -1061,59 +1090,87 @@
         import panel as pn
 
         tabs = pn.Tabs(
             tabs_location="right",
             stylesheets=[
                 """
                 .bk-header {
-                    opacity: 0.1; /* Initially hide the element */
+                    opacity: 0.2; /* Initially hide the element */
                     transition: opacity 0.5s ease; /* Smooth transition for the opacity change */
                 }
 
                 .bk-header:hover {
                     opacity: 1; /* Make the element fully visible on hover */
                 }
                 """
             ],  # noqa: E501
         )
-        yield tabs
-        image = tabs.objects[0]
-        width = image.width
-        height = image.height
-        tabs.param.update(
-            width=width + 50,
-            height=height,
-        )
         player = pn.widgets.Player(
             name="Time",
             start=0,
-            end=len(tabs) - 1,
             value=0,
             loop_policy="loop",
             interval=int(1000 / self.fps),
-            width=width,
             stylesheets=[
                 """
                 :host(.bk-panel-models-widgets-Player) {
-                    opacity: 0.1;
+                    opacity: 0.2;
                     transition: opacity 0.5s ease;
                 }
 
                 :host(.bk-panel-models-widgets-Player:hover) {
                     opacity: 1;
                 }
                 """
             ],
         )
         player.jslink(tabs, value="active", bidirectional=True)
         self._column.objects = [tabs, player]
-        self._column.param.update(
-            width=width,
-            height=height + 100,
-        )
+        yield tabs
+        image = tabs.objects[0]
+        width = image.object.width
+        height = image.object.height
+        with param.parameterized.batch_call_watchers(self):
+            if self.sizing_mode == "fixed":
+                tabs.param.update(
+                    width=width + 50,
+                    height=height,
+                )
+                player.param.update(
+                    width=width,
+                    end=len(tabs) - 1,
+                )
+                self._column.param.update(
+                    width=width,
+                    height=height + 100,
+                )
+            else:
+                sizing_mode = self.sizing_mode.replace("both", "width")
+                tabs.param.update(
+                    min_height=300,
+                    max_height=int(height * 1.5),
+                    sizing_mode=sizing_mode,
+                )
+                player.param.update(
+                    max_height=150,
+                    max_width=450,
+                    sizing_mode=sizing_mode,
+                    end=len(tabs) - 1,
+                    stylesheets=[
+                        """
+                        :host {
+                            align-self: center;
+                        }
+                        """
+                    ],
+                )
+                self._column.param.update(
+                    min_height=300,
+                    max_height=int(height * 1.5),
+                )
         self._column.save(uri)
 
     def _write_images(self, buf: pn.Tabs, images: list[Future], **write_kwargs) -> None:
         import panel as pn
         from PIL import Image
 
         intro_frame = self._create_intro(images)
@@ -1123,20 +1180,28 @@
             image = Image.fromarray(_utils.get_result(image))
 
             pause = None
             if isinstance(image, Paused):
                 pause = image.seconds
                 image = image.output
 
+            sizing_mode = self.sizing_mode
             image_tuple = (
                 str(i),
                 pn.pane.Image(
                     image,
-                    width=image.width,
-                    height=image.height,
+                    width=(
+                        (self.width or image.width) if sizing_mode == "fixed" else None
+                    ),
+                    height=(
+                        (self.height or image.height)
+                        if sizing_mode == "fixed"
+                        else None
+                    ),
+                    sizing_mode=self.sizing_mode,
                 ),
             )
             buf.append(image_tuple, **write_kwargs)
 
             if pause is not None:
                 _utils.repeat_frame(
                     buf.append, image_tuple, pause, self.fps, **write_kwargs
@@ -1165,17 +1230,17 @@
             uri: The file path or BytesIO object to write to.
             resources: The resources to write to the file or in memory.
             **kwargs: Additional keyword arguments to pass.
 
         Returns:
             The file path or BytesIO object.
         """
+        self._display_in_notebook(self._column, display=self.display)
         uri = self._validate_uri(uri)
         uri = super().write(uri=uri, resources=resources, **kwargs)
-        self._display_in_notebook(self._column, display=self.display)
         return uri if not isinstance(uri, BytesIO) else self._column
 
 
 class ConnectedStreams(param.Parameterized):
     """
     Multiple streams connected together.
     """
```

### Comparing `streamjoy-0.0.7/streamjoy/wrappers.py` & `streamjoy-0.0.8/streamjoy/wrappers.py`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/streamjoy/xarray.py` & `streamjoy-0.0.8/streamjoy/xarray.py`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/tests/conftest.py` & `streamjoy-0.0.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/tests/test_core.py` & `streamjoy-0.0.8/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/tests/test_models.py` & `streamjoy-0.0.8/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/tests/test_pandas.py` & `streamjoy-0.0.8/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/tests/test_renderers.py` & `streamjoy-0.0.8/tests/test_renderers.py`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/tests/test_serializers.py` & `streamjoy-0.0.8/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/tests/test_settings.py` & `streamjoy-0.0.8/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/tests/test_streams.py` & `streamjoy-0.0.8/tests/test_streams.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,29 +117,38 @@
         tabs = buf[0]
         assert isinstance(tabs, pn.Tabs)
         image = tabs[0]
         assert isinstance(image, pn.pane.Image)
         assert len(tabs) == max_frames
         player = buf[1]
         assert isinstance(player, pn.widgets.Player)
-
-        assert tabs.width == image.width + 50
-        assert buf.height == image.height + 100
         return image
 
     @pytest.fixture(scope="class")
     def stream_cls(self):
         return HtmlStream
 
     def test_holoviews_matplotlib_backend(self, stream_cls, ds):
         sj = stream_cls.from_holoviews(
             ds.hvplot("lon", "lat", fig_size=200, backend="matplotlib")
         )
         image = self._assert_stream_and_props(sj, stream_cls)
-        assert image.width == 700
+        assert image.width is None
 
     def test_holoviews_bokeh_backend(self, stream_cls, ds):
         sj = stream_cls.from_holoviews(
             ds.hvplot("lon", "lat", width=300, backend="bokeh")
         )
         image = self._assert_stream_and_props(sj, stream_cls)
+        assert image.width is None
+
+    def test_fixed_width_height(self, stream_cls, df):
+        sj = stream_cls.from_pandas(df, width=300, height=300, sizing_mode="fixed")
+        image = self._assert_stream_and_props(sj, stream_cls)
         assert image.width == 300
+        assert image.height == 300
+
+    def test_stretch_width(self, stream_cls, df):
+        sj = stream_cls.from_pandas(df, height=300, sizing_mode="stretch_width")
+        image = self._assert_stream_and_props(sj, stream_cls)
+        assert image.width is None
+        assert image.height is None
```

### Comparing `streamjoy-0.0.7/tests/test_wrappers.py` & `streamjoy-0.0.8/tests/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/tests/test_xarray.py` & `streamjoy-0.0.8/tests/test_xarray.py`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/tests/data/air.nc` & `streamjoy-0.0.8/tests/data/air.nc`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/tests/data/gapminder.csv` & `streamjoy-0.0.8/tests/data/gapminder.csv`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/tests/data/gapminder.parquet` & `streamjoy-0.0.8/tests/data/gapminder.parquet`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/tests/data/air.zarr/.zmetadata` & `streamjoy-0.0.8/tests/data/air.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/tests/data/air.zarr/air/0.0.0` & `streamjoy-0.0.8/tests/data/air.zarr/air/0.0.0`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/.gitignore` & `streamjoy-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/LICENSE` & `streamjoy-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/README.md` & `streamjoy-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.7/pyproject.toml` & `streamjoy-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tool.ruff]
-target-version = "py39"
+target-version = "py310"
 
 [tool.ruff.lint]
 extend-select = ["I", "UP"]
 extend-ignore = ["TRY003"]
 
 [tool.ruff.lint.flake8-type-checking]
 quote-annotations = true
```

### Comparing `streamjoy-0.0.7/PKG-INFO` & `streamjoy-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: streamjoy
-Version: 0.0.7
+Version: 0.0.8
 Summary: Enjoy animating images into GIFs and MP4s!
 Project-URL: Documentation, https://ahuang11.github.io/streamjoy/
 Project-URL: Source, https://github.com/ahuang11/streamjoy
 Author-email: streamjoy <hey.at.py@gmail.com>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9
```

