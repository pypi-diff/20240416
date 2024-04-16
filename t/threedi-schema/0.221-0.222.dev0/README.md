# Comparing `tmp/threedi-schema-0.221.tar.gz` & `tmp/threedi-schema-0.222.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threedi-schema-0.221.tar", last modified: Mon Apr  8 08:01:56 2024, max compression
+gzip compressed data, was "threedi-schema-0.222.dev0.tar", last modified: Tue Apr  9 12:50:11 2024, max compression
```

## Comparing `threedi-schema-0.221.tar` & `threedi-schema-0.222.dev0.tar`

### file list

```diff
@@ -1,73 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:01:56.591983 threedi-schema-0.221/
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-08 08:01:47.000000 threedi-schema-0.221/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-08 08:01:47.000000 threedi-schema-0.221/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-08 08:01:47.000000 threedi-schema-0.221/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7141 2024-04-08 08:01:56.591983 threedi-schema-0.221/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-08 08:01:47.000000 threedi-schema-0.221/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-08 08:01:47.000000 threedi-schema-0.221/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 08:01:56.591983 threedi-schema-0.221/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:01:56.583983 threedi-schema-0.221/threedi_schema/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:01:56.583983 threedi-schema-0.221/threedi_schema/application/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/application/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    13339 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/application/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/application/threedi_database.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/beta_features.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:01:56.583983 threedi-schema-0.221/threedi_schema/domain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/domain/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/domain/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/domain/indexes.py
--rw-r--r--   0 runner    (1001) docker     (127)    32154 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/domain/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/domain/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:01:56.587983 threedi-schema-0.221/threedi_schema/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/infrastructure/spatial_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/infrastructure/spatialite_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/infrastructure/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:01:56.587983 threedi-schema-0.221/threedi_schema/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:01:56.591983 threedi-schema-0.221/threedi_schema/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (127)    46413 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0200_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0201_migrate_friction_type_4.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0202_remove_unused_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0203_remove_unused_cols.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0204_reset_nullable_foreign_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0205_settings_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0206_control_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0207_fix_schema_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0208_tables_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0209_remove_surface_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0210_global_raster_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0211_breach_and_exchange.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0212_breach_and_exchange_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0213_connected_points_to_breaches.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0214_drop_cpoints_levees.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0215_groundwater_1d2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0216_vegetation_drag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0217_rename_vegetation_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0218_1d_vegetation_and_variable_friction.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0219_nullable_cross_section_location_friction_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0220_geopackage_compatiblility.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/0221_remove_vegetation_drag_coeficients_col.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/migrations/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:01:56.591983 threedi-schema-0.221/threedi_schema/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:01:56.591983 threedi-schema-0.221/threedi_schema/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:01:47.000000 threedi-schema-0.221/threedi_schema/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-08 08:01:48.000000 threedi-schema-0.221/threedi_schema/tests/test_beta_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-08 08:01:48.000000 threedi-schema-0.221/threedi_schema/tests/test_gpkg.py
--rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-04-08 08:01:48.000000 threedi-schema-0.221/threedi_schema/tests/test_migration_213.py
--rw-r--r--   0 runner    (1001) docker     (127)     8873 2024-04-08 08:01:48.000000 threedi-schema-0.221/threedi_schema/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-08 08:01:48.000000 threedi-schema-0.221/threedi_schema/tests/test_spatalite_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:01:56.591983 threedi-schema-0.221/threedi_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7141 2024-04-08 08:01:56.000000 threedi-schema-0.221/threedi_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-08 08:01:56.000000 threedi-schema-0.221/threedi_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 08:01:56.000000 threedi-schema-0.221/threedi_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-08 08:01:56.000000 threedi-schema-0.221/threedi_schema.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-08 08:01:56.000000 threedi-schema-0.221/threedi_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-08 08:01:56.000000 threedi-schema-0.221/threedi_schema.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:50:11.759864 threedi-schema-0.222.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-04-09 12:50:11.759864 threedi-schema-0.222.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 12:50:11.759864 threedi-schema-0.222.dev0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:50:11.747864 threedi-schema-0.222.dev0/threedi_schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:50:11.751864 threedi-schema-0.222.dev0/threedi_schema/application/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/application/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13339 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/application/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/application/threedi_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/beta_features.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:50:11.751864 threedi-schema-0.222.dev0/threedi_schema/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/domain/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/domain/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/domain/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30374 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/domain/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/domain/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:50:11.751864 threedi-schema-0.222.dev0/threedi_schema/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/infrastructure/spatial_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/infrastructure/spatialite_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/infrastructure/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:50:11.751864 threedi-schema-0.222.dev0/threedi_schema/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:50:11.755864 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)    46413 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0200_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0201_migrate_friction_type_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0202_remove_unused_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0203_remove_unused_cols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0204_reset_nullable_foreign_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0205_settings_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0206_control_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0207_fix_schema_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0208_tables_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0209_remove_surface_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0210_global_raster_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0211_breach_and_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0212_breach_and_exchange_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0213_connected_points_to_breaches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0214_drop_cpoints_levees.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0215_groundwater_1d2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0216_vegetation_drag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0217_rename_vegetation_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0218_1d_vegetation_and_variable_friction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0219_nullable_cross_section_location_friction_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0220_geopackage_compatiblility.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0221_remove_vegetation_drag_coeficients_col.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13165 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0222_upgrade_db_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:50:11.755864 threedi-schema-0.222.dev0/threedi_schema/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:50:11.755864 threedi-schema-0.222.dev0/threedi_schema/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/tests/test_beta_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/tests/test_gpkg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/tests/test_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/tests/test_migration_213.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8873 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/tests/test_spatalite_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:50:11.759864 threedi-schema-0.222.dev0/threedi_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-04-09 12:50:11.000000 threedi-schema-0.222.dev0/threedi_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-09 12:50:11.000000 threedi-schema-0.222.dev0/threedi_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 12:50:11.000000 threedi-schema-0.222.dev0/threedi_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-09 12:50:11.000000 threedi-schema-0.222.dev0/threedi_schema.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-09 12:50:11.000000 threedi-schema-0.222.dev0/threedi_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-09 12:50:11.000000 threedi-schema-0.222.dev0/threedi_schema.egg-info/top_level.txt
```

### Comparing `threedi-schema-0.221/CHANGES.rst` & `threedi-schema-0.222.dev0/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 Changelog of threedi-schema
 ===================================================
 
 
+0.222 (unreleased)
+------------------
+
+- Nothing changed yet.
+
+
 0.221 (2024-04-08)
 ------------------
 - Remove column vegetation_drag_coeficients from v2_cross_section_location (sqlite only) that was added in migration 218
 
 0.220 (2024-02-29)
 ------------------
 - Add support for geopackage
```

### Comparing `threedi-schema-0.221/LICENSE` & `threedi-schema-0.222.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/PKG-INFO` & `threedi-schema-0.222.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi-schema
-Version: 0.221
+Version: 0.222.dev0
 Summary: The schema of 3Di schematization files
 Author-email: Nelen & Schuurmans <info@nelen-schuurmans.nl>
 License: MIT
 Project-URL: Repository, https://github.com/nens/threedi-schema
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
@@ -86,14 +86,20 @@
 
   $ pip install threedi-schema
 
 Changelog of threedi-schema
 ===================================================
 
 
+0.222 (unreleased)
+------------------
+
+- Nothing changed yet.
+
+
 0.221 (2024-04-08)
 ------------------
 - Remove column vegetation_drag_coeficients from v2_cross_section_location (sqlite only) that was added in migration 218
 
 0.220 (2024-02-29)
 ------------------
 - Add support for geopackage
```

### Comparing `threedi-schema-0.221/README.rst` & `threedi-schema-0.222.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/pyproject.toml` & `threedi-schema-0.222.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/application/schema.py` & `threedi-schema-0.222.dev0/threedi_schema/application/schema.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/application/threedi_database.py` & `threedi-schema-0.222.dev0/threedi_schema/application/threedi_database.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/beta_features.py` & `threedi-schema-0.222.dev0/threedi_schema/beta_features.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/domain/constants.py` & `threedi-schema-0.222.dev0/threedi_schema/domain/constants.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/domain/custom_types.py` & `threedi-schema-0.222.dev0/threedi_schema/domain/custom_types.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/domain/indexes.py` & `threedi-schema-0.222.dev0/threedi_schema/domain/indexes.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/domain/models.py` & `threedi-schema-0.222.dev0/threedi_schema/domain/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -130,43 +130,35 @@
     __tablename__ = "v2_floodfill"
     id = Column(Integer, primary_key=True)
     waterlevel = Column(Float)
     the_geom = Column(Geometry("POINT"))
 
 
 class Interflow(Base):
-    __tablename__ = "v2_interflow"
+    __tablename__ = "interflow"
     id = Column(Integer, primary_key=True)
-    interflow_type = Column(IntegerEnum(constants.InterflowType), nullable=False)
+    interflow_type = Column(IntegerEnum(constants.InterflowType))
     porosity = Column(Float)
     porosity_file = Column(String(255))
     porosity_layer_thickness = Column(Float)
     impervious_layer_elevation = Column(Float)
     hydraulic_conductivity = Column(Float)
     hydraulic_conductivity_file = Column(String(255))
-    display_name = Column(String(255))
-
-    global_settings = relationship("GlobalSetting", back_populates="interflow_settings")
 
 
 class SimpleInfiltration(Base):
-    __tablename__ = "v2_simple_infiltration"
+    __tablename__ = "simple_infiltration"
     id = Column(Integer, primary_key=True)
     infiltration_rate = Column(Float)
     infiltration_rate_file = Column(String(255))
     infiltration_surface_option = Column(
         IntegerEnum(constants.InfiltrationSurfaceOption)
     )
-    max_infiltration_capacity = Column(Float)
-    max_infiltration_capacity_file = Column(Text)
-    display_name = Column(String(255))
-
-    global_settings = relationship(
-        "GlobalSetting", back_populates="simple_infiltration_settings"
-    )
+    max_infiltration_volume = Column(Float)
+    max_infiltration_volume_file = Column(Text)
 
 
 class SurfaceParameter(Base):
     __tablename__ = "v2_surface_parameters"
     id = Column(Integer, primary_key=True)
     outflow_delay = Column(Float, nullable=False)
     surface_layer_thickness = Column(Float, nullable=False)
@@ -201,49 +193,50 @@
     )
     surface_parameters = relationship(
         SurfaceParameter, foreign_keys=surface_parameters_id, back_populates="surface"
     )
 
 
 class GroundWater(Base):
-    __tablename__ = "v2_groundwater"
+    __tablename__ = "groundwater"
     id = Column(Integer, primary_key=True)
 
     groundwater_impervious_layer_level = Column(Float)
     groundwater_impervious_layer_level_file = Column(String(255))
-    groundwater_impervious_layer_level_type = Column(
+    groundwater_impervious_layer_level_aggregation = Column(
         IntegerEnum(constants.InitializationType)
     )
     phreatic_storage_capacity = Column(Float)
     phreatic_storage_capacity_file = Column(String(255))
-    phreatic_storage_capacity_type = Column(IntegerEnum(constants.InitializationType))
+    phreatic_storage_capacity_aggregation = Column(
+        IntegerEnum(constants.InitializationType)
+    )
     equilibrium_infiltration_rate = Column(Float)
     equilibrium_infiltration_rate_file = Column(String(255))
     equilibrium_infiltration_rate_type = Column(
         IntegerEnum(constants.InitializationType)
     )
     initial_infiltration_rate = Column(Float)
     initial_infiltration_rate_file = Column(String(255))
-    initial_infiltration_rate_type = Column(IntegerEnum(constants.InitializationType))
+    initial_infiltration_rate_aggregation = Column(
+        IntegerEnum(constants.InitializationType)
+    )
     infiltration_decay_period = Column(Float)
     infiltration_decay_period_file = Column(String(255))
-    infiltration_decay_period_type = Column(IntegerEnum(constants.InitializationType))
-    groundwater_hydro_connectivity = Column(Float)
-    groundwater_hydro_connectivity_file = Column(String(255))
-    groundwater_hydro_connectivity_type = Column(
+    infiltration_decay_period_aggregation = Column(
+        IntegerEnum(constants.InitializationType)
+    )
+    groundwater_hydraulic_conductivity = Column(Float)
+    groundwater_hydraulic_conductivity_file = Column(String(255))
+    groundwater_hydraulic_conductivity_aggregation = Column(
         IntegerEnum(constants.InitializationType)
     )
-    display_name = Column(String(255))
     leakage = Column(Float)
     leakage_file = Column(String(255))
 
-    global_settings = relationship(
-        "GlobalSetting", back_populates="groundwater_settings"
-    )
-
 
 class GridRefinement(Base):
     __tablename__ = "v2_grid_refinement"
     id = Column(Integer, primary_key=True)
 
     display_name = Column(String(255))
     refinement_level = Column(Integer, nullable=False)
@@ -328,170 +321,143 @@
         nullable=False,
         unique=True,
     )
     connection_node = relationship(ConnectionNode, back_populates="manholes")
 
 
 class NumericalSettings(Base):
-    __tablename__ = "v2_numerical_settings"
+    __tablename__ = "numerical_settings"
     id = Column(Integer, primary_key=True)
     cfl_strictness_factor_1d = Column(Float)
     cfl_strictness_factor_2d = Column(Float)
     convergence_cg = Column(Float)
     convergence_eps = Column(Float)
     flow_direction_threshold = Column(Float)
-    frict_shallow_water_correction = Column(
+    friction_shallow_water_depth_correction = Column(
         IntegerEnum(constants.FrictionShallowWaterDepthCorrection)
     )
     general_numerical_threshold = Column(Float)
-    integration_method = Column(IntegerEnum(constants.IntegrationMethod))
-    limiter_grad_1d = Column(IntegerEnum(constants.OffOrStandard))
-    limiter_grad_2d = Column(IntegerEnum(constants.OffOrStandard))
+    time_integration_method = Column(IntegerEnum(constants.IntegrationMethod))
+    limiter_waterlevel_gradient_1d = Column(IntegerEnum(constants.OffOrStandard))
+    limiter_waterlevel_gradient_2d = Column(IntegerEnum(constants.OffOrStandard))
     limiter_slope_crossectional_area_2d = Column(
         IntegerEnum(constants.LimiterSlopeXArea)
     )
     limiter_slope_friction_2d = Column(IntegerEnum(constants.OffOrStandard))
-    max_nonlin_iterations = Column(Integer)
-    max_degree = Column(Integer)
-    minimum_friction_velocity = Column(Float)
-    minimum_surface_area = Column(Float)
-    precon_cg = Column(IntegerEnum(constants.OffOrStandard))
+    max_non_linear_newton_iterations = Column(Integer)
+    max_degree_gauss_seidel = Column(Integer)
+    min_friction_velocity = Column(Float)
+    min_surface_area = Column(Float)
+    use_preconditioner_cg = Column(IntegerEnum(constants.OffOrStandard))
     preissmann_slot = Column(Float)
     pump_implicit_ratio = Column(Float)
-    thin_water_layer_definition = Column(Float)
+    limiter_slope_thin_water_layer = Column(Float)
     use_of_cg = Column(Integer)
-    use_of_nested_newton = Column(IntegerEnum(constants.OffOrStandard))
-
-    global_settings = relationship("GlobalSetting", back_populates="numerical_settings")
+    use_nested_newton = Column(IntegerEnum(constants.OffOrStandard))
+    flooding_threshold = Column(Float)
 
 
 class VegetationDrag(Base):
-    __tablename__ = "v2_vegetation_drag"
+    __tablename__ = "vegetation_drag_2d"
     id = Column(Integer, primary_key=True)
-    display_name = Column(String(255))
 
     vegetation_height = Column(Float)
     vegetation_height_file = Column(String(255))
 
     vegetation_stem_count = Column(Float)
     vegetation_stem_count_file = Column(String(255))
 
     vegetation_stem_diameter = Column(Float)
     vegetation_stem_diameter_file = Column(String(255))
 
     vegetation_drag_coefficient = Column(Float)
     vegetation_drag_coefficient_file = Column(String(255))
 
-    global_settings = relationship(
-        "GlobalSetting", back_populates="vegetation_drag_settings"
-    )
-
 
-class GlobalSetting(Base):
-    __tablename__ = "v2_global_settings"
+class ModelSettings(Base):
+    __tablename__ = "model_settings"
     id = Column(Integer, primary_key=True)
-    use_2d_flow = Column(Boolean, nullable=False)
-    use_1d_flow = Column(Boolean, nullable=False)
-    manhole_storage_area = Column(Float)
-    name = Column(String(128))
-    sim_time_step = Column(Float, nullable=False)
-    output_time_step = Column(Float, nullable=False)
-    nr_timesteps = Column(Integer)
-    start_time = Column(Text)
-    start_date = Column(Text)
-    grid_space = Column(Float, nullable=False)
-    dist_calc_points = Column(Float, nullable=False)
-    kmax = Column(Integer, nullable=False)
-    guess_dams = Column(Integer)
-    table_step_size = Column(Float, nullable=False)
+    use_2d_flow = Column(Boolean)
+    use_1d_flow = Column(Boolean)
+    manhole_aboveground_storage_area = Column(Float)
+    minimum_cell_size = Column(Float)
+    calculation_point_distance_1d = Column(Float)
+    nr_grid_levels = Column(Integer)
+    minimum_table_step_size = Column(Float)
     maximum_table_step_size = Column(Float)
-    flooding_threshold = Column(Float, nullable=False)
-    advection_1d = Column(IntegerEnum(constants.OffOrStandard), nullable=False)
-    advection_2d = Column(IntegerEnum(constants.OffOrStandard), nullable=False)
     dem_file = Column(String(255))
-    frict_type = Column(IntegerEnum(constants.FrictionType), nullable=False)
-    frict_coef = Column(Float, nullable=False)
-    frict_coef_file = Column(String(255))
-    water_level_ini_type = Column(IntegerEnum(constants.InitializationType))
-    initial_waterlevel = Column(Float, nullable=False)
-    initial_waterlevel_file = Column(String(255))
-    interception_global = Column(Float)
-    interception_file = Column(String(255))
-    dem_obstacle_detection = Column(Boolean, nullable=False)
-    dem_obstacle_height = Column(Float)
+    friction_type = Column(IntegerEnum(constants.FrictionType))
+    friction_coefficient = Column(Float)
+    friction_coefficient_file = Column(String(255))
     embedded_cutoff_threshold = Column(Float)
     epsg_code = Column(Integer)
-    timestep_plus = Column(Boolean, nullable=False)
     max_angle_1d_advection = Column(Float)
-    minimum_sim_time_step = Column(Float, nullable=False)
-    maximum_sim_time_step = Column(Float)
-    frict_avg = Column(IntegerEnum(constants.OffOrStandard), nullable=False)
-    wind_shielding_file = Column(String(255))
-    use_0d_inflow = Column(IntegerEnum(constants.InflowType), nullable=False)
+    friction_averaging = Column(IntegerEnum(constants.OffOrStandard))
     table_step_size_1d = Column(Float)
-    use_2d_rain = Column(Integer, nullable=False)
+    use_2d_rain = Column(Integer)
+    use_interflow = Column(Boolean)
+    use_interception = Column(Boolean)
+    use_structure_control = Column(Boolean)
+    use_simple_infiltration = Column(Boolean)
+    use_groundwater_flow = Column(Boolean)
+    use_groundwater_storage = Column(Boolean)
+    use_vegetation_drag_2d = Column(Boolean)
+
+
+class InitialConditions(Base):
+    __tablename__ = "initial_conditions"
+    id = Column(Integer, primary_key=True)
     initial_groundwater_level = Column(Float)
     initial_groundwater_level_file = Column(String(255))
-    initial_groundwater_level_type = Column(IntegerEnum(constants.InitializationType))
-
-    numerical_settings_id = Column(
-        Integer, ForeignKey(NumericalSettings.__tablename__ + ".id"), nullable=False
-    )
-    numerical_settings = relationship(
-        NumericalSettings,
-        foreign_keys=numerical_settings_id,
-        back_populates="global_settings",
-    )
-    interflow_settings_id = Column(Integer, ForeignKey(Interflow.__tablename__ + ".id"))
-    interflow_settings = relationship(
-        Interflow,
-        foreign_keys=interflow_settings_id,
-        back_populates="global_settings",
-    )
-    control_group_id = Column(Integer, ForeignKey(ControlGroup.__tablename__ + ".id"))
-    simple_infiltration_settings_id = Column(
-        Integer, ForeignKey(SimpleInfiltration.__tablename__ + ".id")
-    )
-    simple_infiltration_settings = relationship(
-        SimpleInfiltration,
-        foreign_keys=simple_infiltration_settings_id,
-        back_populates="global_settings",
-    )
-    groundwater_settings_id = Column(
-        Integer, ForeignKey(GroundWater.__tablename__ + ".id")
-    )
-    groundwater_settings = relationship(
-        GroundWater,
-        foreign_keys=groundwater_settings_id,
-        back_populates="global_settings",
-    )
-    vegetation_drag_settings_id = Column(
-        Integer, ForeignKey(VegetationDrag.__tablename__ + ".id")
-    )
-    vegetation_drag_settings = relationship(
-        VegetationDrag,
-        foreign_keys=vegetation_drag_settings_id,
-        back_populates="global_settings",
+    initial_groundwater_level_aggregation = Column(
+        IntegerEnum(constants.InitializationType)
     )
+    initial_water_level = Column(Float)
+    initial_water_level_aggregation = Column(IntegerEnum(constants.InitializationType))
+    initial_water_level_file = Column(String(255))
+
+
+class Interception(Base):
+    __tablename__ = "interception"
+    id = Column(Integer, primary_key=True)
+    interception = Column(Float)
+    interception_file = Column(String(255))
 
 
+# class PhysicalSettings
 class AggregationSettings(Base):
-    __tablename__ = "v2_aggregation_settings"
+    __tablename__ = "aggregation_settings"
     id = Column(Integer, primary_key=True)
+    flow_variable = Column(VarcharEnum(constants.FlowVariable))
+    aggregation_method = Column(VarcharEnum(constants.AggregationMethod))
+    interval = Column(Integer)
 
-    global_settings_id = Column(
-        Integer, ForeignKey(GlobalSetting.__tablename__ + ".id")
-    )
 
-    var_name = Column(String(100), nullable=False)
-    flow_variable = Column(VarcharEnum(constants.FlowVariable), nullable=False)
-    aggregation_method = Column(
-        VarcharEnum(constants.AggregationMethod), nullable=False
-    )
-    timestep = Column(Integer, nullable=False)
+class PhysicalSettings(Base):
+    __tablename__ = "physical_settings"
+    id = Column(Integer, primary_key=True)
+    use_advection_1d = Column(IntegerEnum(constants.OffOrStandard))
+    use_advection_2d = Column(IntegerEnum(constants.OffOrStandard))
+
+
+class SimulationTemplateSettings(Base):
+    __tablename__ = "simulation_template_settings"
+    id = Column(Integer, primary_key=True)
+    name = Column(String(128))
+    use_0d_inflow = Column(IntegerEnum(constants.InflowType))
+
+
+class TimeStepSettings(Base):
+    __tablename__ = "time_step_settings"
+    id = Column(Integer, primary_key=True)
+    time_step = Column(Float)
+    min_time_step = Column(Float)
+    max_time_step = Column(Float)
+    output_time_step = Column(Float)
+    use_time_step_stretch = Column(Boolean)
 
 
 class BoundaryCondition1D(Base):
     __tablename__ = "v2_1d_boundary_conditions"
 
     id = Column(Integer, primary_key=True)
     boundary_type = Column(IntegerEnum(constants.BoundaryType), nullable=False)
@@ -874,15 +840,15 @@
     ControlTimed,
     CrossSectionDefinition,
     CrossSectionLocation,
     Culvert,
     DemAverageArea,
     ExchangeLine,
     Floodfill,
-    GlobalSetting,
+    ModelSettings,
     GridRefinement,
     GridRefinementArea,
     GroundWater,
     ImperviousSurface,
     ImperviousSurfaceMap,
     Interflow,
     Lateral1d,
```

### Comparing `threedi-schema-0.221/threedi_schema/domain/views.py` & `threedi-schema-0.222.dev0/threedi_schema/domain/views.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/infrastructure/spatial_index.py` & `threedi-schema-0.222.dev0/threedi_schema/infrastructure/spatial_index.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/infrastructure/spatialite_versions.py` & `threedi-schema-0.222.dev0/threedi_schema/infrastructure/spatialite_versions.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/infrastructure/views.py` & `threedi-schema-0.222.dev0/threedi_schema/infrastructure/views.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/migrations/env.py` & `threedi-schema-0.222.dev0/threedi_schema/migrations/env.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/migrations/versions/0200_initial.py` & `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0200_initial.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/migrations/versions/0201_migrate_friction_type_4.py` & `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0201_migrate_friction_type_4.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/migrations/versions/0202_remove_unused_tables.py` & `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0202_remove_unused_tables.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/migrations/versions/0203_remove_unused_cols.py` & `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0203_remove_unused_cols.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/migrations/versions/0204_reset_nullable_foreign_keys.py` & `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0204_reset_nullable_foreign_keys.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/migrations/versions/0205_settings_defaults.py` & `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0205_settings_defaults.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/migrations/versions/0206_control_structures.py` & `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0206_control_structures.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/migrations/versions/0207_fix_schema_constraints.py` & `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0207_fix_schema_constraints.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/migrations/versions/0208_tables_settings.py` & `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0208_tables_settings.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/migrations/versions/0209_remove_surface_type.py` & `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0209_remove_surface_type.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/migrations/versions/0210_global_raster_values.py` & `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0210_global_raster_values.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/migrations/versions/0211_breach_and_exchange.py` & `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0211_breach_and_exchange.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/migrations/versions/0212_breach_and_exchange_properties.py` & `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0212_breach_and_exchange_properties.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/migrations/versions/0213_connected_points_to_breaches.py` & `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0213_connected_points_to_breaches.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/migrations/versions/0214_drop_cpoints_levees.py` & `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0214_drop_cpoints_levees.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/migrations/versions/0215_groundwater_1d2d.py` & `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0215_groundwater_1d2d.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/migrations/versions/0216_vegetation_drag.py` & `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0216_vegetation_drag.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/migrations/versions/0217_rename_vegetation_columns.py` & `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0217_rename_vegetation_columns.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/migrations/versions/0218_1d_vegetation_and_variable_friction.py` & `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0218_1d_vegetation_and_variable_friction.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/migrations/versions/0219_nullable_cross_section_location_friction_value.py` & `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0219_nullable_cross_section_location_friction_value.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/migrations/versions/0220_geopackage_compatiblility.py` & `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0220_geopackage_compatiblility.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/migrations/versions/0221_remove_vegetation_drag_coeficients_col.py` & `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0221_remove_vegetation_drag_coeficients_col.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/scripts.py` & `threedi-schema-0.222.dev0/threedi_schema/scripts.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/tests/conftest.py` & `threedi-schema-0.222.dev0/threedi_schema/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/tests/test_beta_features.py` & `threedi-schema-0.222.dev0/threedi_schema/tests/test_beta_features.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/tests/test_gpkg.py` & `threedi-schema-0.222.dev0/threedi_schema/tests/test_gpkg.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/tests/test_migration_213.py` & `threedi-schema-0.222.dev0/threedi_schema/tests/test_migration_213.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/tests/test_schema.py` & `threedi-schema-0.222.dev0/threedi_schema/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema/tests/test_spatalite_versions.py` & `threedi-schema-0.222.dev0/threedi_schema/tests/test_spatalite_versions.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.221/threedi_schema.egg-info/PKG-INFO` & `threedi-schema-0.222.dev0/threedi_schema.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi-schema
-Version: 0.221
+Version: 0.222.dev0
 Summary: The schema of 3Di schematization files
 Author-email: Nelen & Schuurmans <info@nelen-schuurmans.nl>
 License: MIT
 Project-URL: Repository, https://github.com/nens/threedi-schema
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
@@ -86,14 +86,20 @@
 
   $ pip install threedi-schema
 
 Changelog of threedi-schema
 ===================================================
 
 
+0.222 (unreleased)
+------------------
+
+- Nothing changed yet.
+
+
 0.221 (2024-04-08)
 ------------------
 - Remove column vegetation_drag_coeficients from v2_cross_section_location (sqlite only) that was added in migration 218
 
 0.220 (2024-02-29)
 ------------------
 - Add support for geopackage
```

### Comparing `threedi-schema-0.221/threedi_schema.egg-info/SOURCES.txt` & `threedi-schema-0.222.dev0/threedi_schema.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,18 @@
 threedi_schema/migrations/versions/0215_groundwater_1d2d.py
 threedi_schema/migrations/versions/0216_vegetation_drag.py
 threedi_schema/migrations/versions/0217_rename_vegetation_columns.py
 threedi_schema/migrations/versions/0218_1d_vegetation_and_variable_friction.py
 threedi_schema/migrations/versions/0219_nullable_cross_section_location_friction_value.py
 threedi_schema/migrations/versions/0220_geopackage_compatiblility.py
 threedi_schema/migrations/versions/0221_remove_vegetation_drag_coeficients_col.py
+threedi_schema/migrations/versions/0222_upgrade_db_settings.py
 threedi_schema/migrations/versions/__init__.py
 threedi_schema/tests/__init__.py
 threedi_schema/tests/conftest.py
 threedi_schema/tests/test_beta_features.py
 threedi_schema/tests/test_gpkg.py
+threedi_schema/tests/test_migration.py
 threedi_schema/tests/test_migration_213.py
 threedi_schema/tests/test_schema.py
 threedi_schema/tests/test_spatalite_versions.py
 threedi_schema/tests/data/__init__.py
```

