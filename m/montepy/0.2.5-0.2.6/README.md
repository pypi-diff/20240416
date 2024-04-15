# Comparing `tmp/montepy-0.2.5.tar.gz` & `tmp/montepy-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "montepy-0.2.5.tar", last modified: Tue Jan 16 17:36:17 2024, max compression
+gzip compressed data, was "montepy-0.2.6.tar", last modified: Mon Apr 15 21:59:32 2024, max compression
```

## Comparing `montepy-0.2.5.tar` & `montepy-0.2.6.tar`

### file list

```diff
@@ -1,102 +1,240 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:36:17.280699 montepy-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-01-16 17:36:08.000000 montepy-0.2.5/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-01-16 17:36:08.000000 montepy-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-01-16 17:36:08.000000 montepy-0.2.5/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-01-16 17:36:17.280699 montepy-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-01-16 17:36:08.000000 montepy-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:36:17.268699 montepy-0.2.5/montepy/
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/_cell_data_control.py
--rw-r--r--   0 runner    (1001) docker     (127)    24162 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/cells.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:36:17.272699 montepy-0.2.5/montepy/data_inputs/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/data_inputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10340 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/data_inputs/cell_modifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    10150 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/data_inputs/data_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/data_inputs/data_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/data_inputs/element.py
--rw-r--r--   0 runner    (1001) docker     (127)    19454 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/data_inputs/fill.py
--rw-r--r--   0 runner    (1001) docker     (127)    15591 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/data_inputs/importance.py
--rw-r--r--   0 runner    (1001) docker     (127)     5753 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/data_inputs/isotope.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/data_inputs/lattice.py
--rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/data_inputs/lattice_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/data_inputs/material.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/data_inputs/material_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/data_inputs/mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/data_inputs/tally.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/data_inputs/tally_multiplier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/data_inputs/thermal_scattering.py
--rw-r--r--   0 runner    (1001) docker     (127)     8779 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/data_inputs/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/data_inputs/universe_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     6873 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/data_inputs/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/geometry_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:36:17.276699 montepy-0.2.5/montepy/input_parser/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/input_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/input_parser/block_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     6398 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/input_parser/cell_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/input_parser/data_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/input_parser/input_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/input_parser/input_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/input_parser/input_syntax_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    12817 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/input_parser/mcnp_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    14577 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/input_parser/parser_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/input_parser/read_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/input_parser/shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/input_parser/surface_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    65555 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/input_parser/syntax_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/input_parser/tally_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/input_parser/thermal_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    11112 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/input_parser/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/materials.py
--rw-r--r--   0 runner    (1001) docker     (127)    15206 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/mcnp_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    17471 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/mcnp_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/numbered_mcnp_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    14849 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/numbered_object_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/particle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/surface_collection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:36:17.276699 montepy-0.2.5/montepy/surfaces/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/surfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/surfaces/axis_plane.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/surfaces/cylinder_on_axis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/surfaces/cylinder_par_axis.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/surfaces/general_plane.py
--rw-r--r--   0 runner    (1001) docker     (127)    22387 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/surfaces/half_space.py
--rw-r--r--   0 runner    (1001) docker     (127)    11238 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/surfaces/surface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/surfaces/surface_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/surfaces/surface_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/universe.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/universes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-01-16 17:36:08.000000 montepy-0.2.5/montepy/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:36:17.280699 montepy-0.2.5/montepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-01-16 17:36:17.000000 montepy-0.2.5/montepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-01-16 17:36:17.000000 montepy-0.2.5/montepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 17:36:17.000000 montepy-0.2.5/montepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-01-16 17:36:17.000000 montepy-0.2.5/montepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-16 17:36:17.000000 montepy-0.2.5/montepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-01-16 17:36:08.000000 montepy-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-16 17:36:17.280699 montepy-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:36:17.280699 montepy-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-01-16 17:36:08.000000 montepy-0.2.5/tests/test_cell_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)    12053 2024-01-16 17:36:08.000000 montepy-0.2.5/tests/test_data_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-01-16 17:36:08.000000 montepy-0.2.5/tests/test_edge_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)    17864 2024-01-16 17:36:08.000000 montepy-0.2.5/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-01-16 17:36:08.000000 montepy-0.2.5/tests/test_importance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-01-16 17:36:08.000000 montepy-0.2.5/tests/test_input_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    42653 2024-01-16 17:36:08.000000 montepy-0.2.5/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-01-16 17:36:08.000000 montepy-0.2.5/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-01-16 17:36:08.000000 montepy-0.2.5/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)    14900 2024-01-16 17:36:08.000000 montepy-0.2.5/tests/test_material.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-01-16 17:36:08.000000 montepy-0.2.5/tests/test_mcnp_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-01-16 17:36:08.000000 montepy-0.2.5/tests/test_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)    10482 2024-01-16 17:36:08.000000 montepy-0.2.5/tests/test_numbered_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-01-16 17:36:08.000000 montepy-0.2.5/tests/test_source_def.py
--rw-r--r--   0 runner    (1001) docker     (127)    11668 2024-01-16 17:36:08.000000 montepy-0.2.5/tests/test_surfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    57902 2024-01-16 17:36:08.000000 montepy-0.2.5/tests/test_syntax_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-01-16 17:36:08.000000 montepy-0.2.5/tests/test_tally.py
--rw-r--r--   0 runner    (1001) docker     (127)    10797 2024-01-16 17:36:08.000000 montepy-0.2.5/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)    14670 2024-01-16 17:36:08.000000 montepy-0.2.5/tests/test_universe.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-01-16 17:36:08.000000 montepy-0.2.5/tests/test_utilities.py
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:32.125330 montepy-0.2.6/
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:24.239627 montepy-0.2.6/.github/
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:24.297110 montepy-0.2.6/.github/ISSUE_TEMPLATE/
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     2491 2024-04-15 21:58:30.000000 montepy-0.2.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      773 2024-04-15 21:58:30.000000 montepy-0.2.6/.github/ISSUE_TEMPLATE/feature_request.md
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      668 2024-04-15 21:58:30.000000 montepy-0.2.6/.github/pull_request_template.md
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:24.348112 montepy-0.2.6/.github/workflows/
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     4475 2024-04-15 21:58:30.000000 montepy-0.2.6/.github/workflows/deploy.yml
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     3484 2024-04-15 21:58:30.000000 montepy-0.2.6/.github/workflows/main.yml
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      142 2024-04-15 21:58:30.000000 montepy-0.2.6/.gitignore
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      140 2024-01-10 03:00:18.000000 montepy-0.2.6/AUTHORS
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1086 2024-01-10 02:47:53.000000 montepy-0.2.6/LICENSE
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1742 2024-01-10 02:47:34.000000 montepy-0.2.6/NOTICE.txt
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     6597 2024-04-15 21:59:32.114337 montepy-0.2.6/PKG-INFO
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     3317 2024-04-15 21:58:30.000000 montepy-0.2.6/README.md
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:24.415146 montepy-0.2.6/demo/
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     3932 2024-01-12 01:37:19.000000 montepy-0.2.6/demo/Pin_cell.ipynb
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      620 2024-01-12 01:37:19.000000 montepy-0.2.6/demo/pin_cell.imcnp
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:24.477595 montepy-0.2.6/doc/
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      638 2024-01-10 03:00:18.000000 montepy-0.2.6/doc/Makefile
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      799 2024-01-10 03:00:18.000000 montepy-0.2.6/doc/make.bat
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:24.942703 montepy-0.2.6/doc/source/
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:24.981225 montepy-0.2.6/doc/source/_static/
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-01-10 03:00:18.000000 montepy-0.2.6/doc/source/_static/placeholder
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:25.023227 montepy-0.2.6/doc/source/_templates/
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-01-10 03:00:18.000000 montepy-0.2.6/doc/source/_templates/placeholder
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1026 2024-04-15 21:58:30.000000 montepy-0.2.6/doc/source/_test_for_missing_docs.py
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:27.447191 montepy-0.2.6/doc/source/api/
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       67 2024-04-15 21:58:25.000000 montepy-0.2.6/doc/source/api/modules.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      125 2024-04-15 21:58:25.000000 montepy-0.2.6/doc/source/api/montepy.cell.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      128 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.cells.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      140 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.constants.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      365 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.cell_modifier.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      248 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.data_input.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      186 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.data_parser.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      172 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.element.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      163 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.fill.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      181 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.importance.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      172 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.isotope.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      172 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.lattice.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      192 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.lattice_input.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      175 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.material.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      207 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.material_component.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      163 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.mode.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      816 2024-04-15 21:58:30.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      166 2024-04-15 21:58:30.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.tally.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      199 2024-04-15 21:58:30.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.tally_multiplier.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      207 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.thermal_scattering.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      178 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.transform.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      195 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.universe_input.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      169 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.data_inputs.volume.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      131 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.errors.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      169 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.geometry_operators.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      186 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.input_parser.block_type.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      189 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.input_parser.cell_parser.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      189 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.input_parser.data_parser.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      242 2024-04-15 21:58:30.000000 montepy-0.2.6/doc/source/api/montepy.input_parser.input_file.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      192 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.input_parser.input_reader.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      215 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.input_parser.input_syntax_reader.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      186 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.input_parser.mcnp_input.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      189 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.input_parser.parser_base.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      189 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.input_parser.read_parser.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      753 2024-04-15 21:58:30.000000 montepy-0.2.6/doc/source/api/montepy.input_parser.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      181 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.input_parser.shortcuts.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      198 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.input_parser.surface_parser.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      244 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.input_parser.syntax_node.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      192 2024-04-15 21:58:30.000000 montepy-0.2.6/doc/source/api/montepy.input_parser.tally_parser.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      198 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.input_parser.thermal_parser.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      172 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.input_parser.tokens.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      140 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.materials.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      208 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.mcnp_object.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      151 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.mcnp_problem.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      177 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.numbered_mcnp_object.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      195 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.numbered_object_collection.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      137 2024-01-12 01:37:19.000000 montepy-0.2.6/doc/source/api/montepy.particle.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      663 2024-04-15 21:58:25.000000 montepy-0.2.6/doc/source/api/montepy.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      169 2024-01-12 01:37:20.000000 montepy-0.2.6/doc/source/api/montepy.surface_collection.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      172 2024-01-12 01:37:20.000000 montepy-0.2.6/doc/source/api/montepy.surfaces.axis_plane.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      192 2024-01-12 01:37:20.000000 montepy-0.2.6/doc/source/api/montepy.surfaces.cylinder_on_axis.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      195 2024-01-12 01:37:20.000000 montepy-0.2.6/doc/source/api/montepy.surfaces.cylinder_par_axis.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      181 2024-01-12 01:37:20.000000 montepy-0.2.6/doc/source/api/montepy.surfaces.general_plane.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      172 2024-01-12 01:37:20.000000 montepy-0.2.6/doc/source/api/montepy.surfaces.half_space.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      461 2024-04-15 21:58:25.000000 montepy-0.2.6/doc/source/api/montepy.surfaces.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      161 2024-01-12 01:37:20.000000 montepy-0.2.6/doc/source/api/montepy.surfaces.surface.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      187 2024-01-12 01:37:20.000000 montepy-0.2.6/doc/source/api/montepy.surfaces.surface_builder.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      178 2024-01-12 01:37:20.000000 montepy-0.2.6/doc/source/api/montepy.surfaces.surface_type.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      143 2024-01-12 01:37:20.000000 montepy-0.2.6/doc/source/api/montepy.transforms.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      137 2024-01-12 01:37:20.000000 montepy-0.2.6/doc/source/api/montepy.universe.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      140 2024-01-12 01:37:20.000000 montepy-0.2.6/doc/source/api/montepy.universes.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      140 2024-01-12 01:37:20.000000 montepy-0.2.6/doc/source/api/montepy.utilities.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     2275 2024-04-15 21:58:30.000000 montepy-0.2.6/doc/source/conf.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    42074 2024-04-15 21:58:30.000000 montepy-0.2.6/doc/source/developing.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     3373 2024-04-15 21:58:30.000000 montepy-0.2.6/doc/source/faq.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      861 2024-04-15 21:58:30.000000 montepy-0.2.6/doc/source/index.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    98645 2024-01-12 01:37:20.000000 montepy-0.2.6/doc/source/monty.svg
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      362 2024-04-15 21:58:30.000000 montepy-0.2.6/doc/source/publications.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    28253 2024-01-12 01:37:20.000000 montepy-0.2.6/doc/source/starting.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     2141 2024-01-10 03:00:18.000000 montepy-0.2.6/doc/source/tricks.rst
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     4057 2024-04-15 21:58:30.000000 montepy-0.2.6/doc/source/utilities.rst
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:27.468191 montepy-0.2.6/graphics/
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    98645 2024-01-12 01:37:20.000000 montepy-0.2.6/graphics/monty.svg
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:28.097539 montepy-0.2.6/montepy/
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1383 2024-04-15 21:58:30.000000 montepy-0.2.6/montepy/__init__.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1784 2024-04-15 21:58:30.000000 montepy-0.2.6/montepy/__main__.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1182 2024-01-10 03:00:19.000000 montepy-0.2.6/montepy/_cell_data_control.py
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:28.267306 montepy-0.2.6/montepy/_scripts/
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:58:30.000000 montepy-0.2.6/montepy/_scripts/__init__.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     2566 2024-04-15 21:58:30.000000 montepy-0.2.6/montepy/_scripts/change_to_ascii.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      411 2024-04-15 21:59:20.000000 montepy-0.2.6/montepy/_version.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    24162 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/cell.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     6872 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/cells.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1818 2024-04-15 21:58:30.000000 montepy-0.2.6/montepy/constants.py
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:29.134337 montepy-0.2.6/montepy/data_inputs/
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      256 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/data_inputs/__init__.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    10340 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/data_inputs/cell_modifier.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    10150 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/data_inputs/data_input.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1271 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/data_inputs/data_parser.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     7752 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/data_inputs/element.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    19502 2024-04-15 21:58:30.000000 montepy-0.2.6/montepy/data_inputs/fill.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    15591 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/data_inputs/importance.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     5753 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/data_inputs/isotope.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      400 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/data_inputs/lattice.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     4238 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/data_inputs/lattice_input.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     7849 2024-04-15 21:58:30.000000 montepy-0.2.6/montepy/data_inputs/material.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1956 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/data_inputs/material_component.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     5451 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/data_inputs/mode.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      466 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/data_inputs/tally.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      449 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/data_inputs/tally_multiplier.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     4438 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/data_inputs/thermal_scattering.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     8779 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/data_inputs/transform.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     7412 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/data_inputs/universe_input.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     6873 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/data_inputs/volume.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     5935 2024-04-15 21:58:30.000000 montepy-0.2.6/montepy/errors.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      558 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/geometry_operators.py
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:29.705772 montepy-0.2.6/montepy/input_parser/
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      358 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/input_parser/__init__.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      478 2024-01-10 03:00:19.000000 montepy-0.2.6/montepy/input_parser/block_type.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     6467 2024-04-15 21:58:30.000000 montepy-0.2.6/montepy/input_parser/cell_parser.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     5014 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/input_parser/data_parser.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     4148 2024-04-15 21:58:30.000000 montepy-0.2.6/montepy/input_parser/input_file.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1321 2024-04-15 21:58:30.000000 montepy-0.2.6/montepy/input_parser/input_reader.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     7611 2024-04-15 21:58:30.000000 montepy-0.2.6/montepy/input_parser/input_syntax_reader.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    12817 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/input_parser/mcnp_input.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    14577 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/input_parser/parser_base.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1341 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/input_parser/read_parser.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      632 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/input_parser/shortcuts.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1839 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/input_parser/surface_parser.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    65199 2024-04-15 21:58:30.000000 montepy-0.2.6/montepy/input_parser/syntax_node.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     2192 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/input_parser/tally_parser.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1124 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/input_parser/thermal_parser.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    11112 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/input_parser/tokens.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      551 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/materials.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    15206 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/mcnp_object.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    17607 2024-04-15 21:58:30.000000 montepy-0.2.6/montepy/mcnp_problem.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      571 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/numbered_mcnp_object.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    14849 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/numbered_object_collection.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1245 2024-01-10 03:00:19.000000 montepy-0.2.6/montepy/particle.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1791 2024-01-10 03:00:19.000000 montepy-0.2.6/montepy/surface_collection.py
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:30.107340 montepy-0.2.6/montepy/surfaces/
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      360 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/surfaces/__init__.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     2364 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/surfaces/axis_plane.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     2454 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/surfaces/cylinder_on_axis.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     4234 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/surfaces/cylinder_par_axis.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      981 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/surfaces/general_plane.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    22387 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/surfaces/half_space.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    11238 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/surfaces/surface.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1288 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/surfaces/surface_builder.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     2549 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/surfaces/surface_type.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      451 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/transforms.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     3169 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/universe.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      421 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/universes.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     5136 2024-01-12 01:37:20.000000 montepy-0.2.6/montepy/utilities.py
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:32.100331 montepy-0.2.6/montepy.egg-info/
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     6597 2024-04-15 21:59:20.000000 montepy-0.2.6/montepy.egg-info/PKG-INFO
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     7513 2024-04-15 21:59:24.000000 montepy-0.2.6/montepy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)        1 2024-04-15 21:59:20.000000 montepy-0.2.6/montepy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       74 2024-04-15 21:59:20.000000 montepy-0.2.6/montepy.egg-info/entry_points.txt
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      236 2024-04-15 21:59:20.000000 montepy-0.2.6/montepy.egg-info/requires.txt
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)        8 2024-04-15 21:59:20.000000 montepy-0.2.6/montepy.egg-info/top_level.txt
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     2303 2024-04-15 21:58:30.000000 montepy-0.2.6/pyproject.toml
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       38 2024-04-15 21:59:32.126331 montepy-0.2.6/setup.cfg
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:30.891354 montepy-0.2.6/tests/
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/__init__.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      841 2024-04-15 21:58:30.000000 montepy-0.2.6/tests/constants.py
+drwxrwxrwx   0 mgale     (1000) mgale     (1000)        0 2024-04-15 21:59:32.070547 montepy-0.2.6/tests/inputs/
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      912 2024-04-15 21:58:30.000000 montepy-0.2.6/tests/inputs/bad_encoding.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      293 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/inputs/breaking_comments.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      626 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/inputs/number_conflict_pin_cell.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      887 2024-04-15 21:58:30.000000 montepy-0.2.6/tests/inputs/test.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       87 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/inputs/testRead.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       63 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/testReadRec1.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       29 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/testReadRec2.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)        7 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/testReadRec3.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)        8 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/inputs/testReadTarget.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       56 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/testVerticalMode.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       34 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/inputs/test_bad_syntax.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       79 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/test_broken_cell_surf_link.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       77 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/test_broken_complement.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       76 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/test_broken_mat_link.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       41 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/test_broken_surf_link.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       57 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/test_broken_transform_link.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      641 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/test_complement_edge.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      835 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/test_dos.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      125 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/inputs/test_excess_mt.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       77 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/inputs/test_extra_data_imp.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       51 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/inputs/test_extra_data_param.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       88 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/inputs/test_extra_params.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      766 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/test_imp_redundant.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      765 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/test_importance.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       84 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/test_interp_edge.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      957 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/test_long_lines.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       95 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/inputs/test_missing_mat_for_mt.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      355 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/test_redundant_surf.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)       62 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/test_surfaces.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      853 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/inputs/test_tab.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      937 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/inputs/test_universe.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      768 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/test_universe_data.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      782 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/inputs/test_vol_redundant.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      881 2024-04-15 21:58:30.000000 montepy-0.2.6/tests/inputs/unicode.imcnp
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     5775 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/test_cell_problem.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    12053 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/test_data_inputs.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     7255 2024-04-15 21:58:30.000000 montepy-0.2.6/tests/test_edge_cases.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    17864 2024-04-15 21:58:30.000000 montepy-0.2.6/tests/test_geometry.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     7097 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/test_importance.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     2249 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/test_input_file.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    43268 2024-04-15 21:58:30.000000 montepy-0.2.6/tests/test_integration.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1071 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/test_interface.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1379 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/test_main.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    14900 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/test_material.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      816 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/test_mcnp_problem.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     3579 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/test_mode.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    10482 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/test_numbered_collection.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     3356 2024-04-15 21:58:30.000000 montepy-0.2.6/tests/test_scripts.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      561 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/test_source_def.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    11668 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/test_surfaces.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    57902 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/test_syntax_parsing.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)     1266 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/test_tally.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    10797 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/test_transform.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)    14670 2024-01-12 01:37:20.000000 montepy-0.2.6/tests/test_universe.py
+-rwxrwxrwx   0 mgale     (1000) mgale     (1000)      748 2024-01-10 03:00:19.000000 montepy-0.2.6/tests/test_utilities.py
```

### Comparing `montepy-0.2.5/LICENSE` & `montepy-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/NOTICE.txt` & `montepy-0.2.6/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/PKG-INFO` & `montepy-0.2.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: montepy
-Version: 0.2.5
+Version: 0.2.6
 Summary: A library for reading, editing, and writing MCNP input files
 Author: Brenna Carbno
 Author-email: Micah Gale <micah.gale@inl.gov>, Travis Labossiere-Hickman <Travis.LabossiereHickman@inl.gov>
 Maintainer-email: Micah Gale <micah.gale@inl.gov>
 License: MIT License
         
         Copyright (c) 2024 Battelle Energy Alliance, LLC
@@ -43,29 +43,43 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE.txt
 License-File: AUTHORS
-Requires-Dist: numpy
+Requires-Dist: numpy>=1.18
 Requires-Dist: sly==0.5
 Provides-Extra: test
-Requires-Dist: coverage; extra == "test"
+Requires-Dist: coverage[toml]>=6.3.2; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == "doc"
 Requires-Dist: sphinxcontrib-apidoc; extra == "doc"
 Requires-Dist: sphinx_rtd_theme; extra == "doc"
+Provides-Extra: format
+Requires-Dist: black>=23.3.0; extra == "format"
+Provides-Extra: build
+Requires-Dist: build; extra == "build"
+Requires-Dist: setuptools_scm>=8; extra == "build"
+Provides-Extra: develop
+Requires-Dist: montepy[test]; extra == "develop"
+Requires-Dist: montepy[doc]; extra == "develop"
+Requires-Dist: montepy[format]; extra == "develop"
+Requires-Dist: montepy[build]; extra == "develop"
 
 # MontePy
 
 <img src="https://raw.githubusercontent.com/idaholab/MontePy/develop/graphics/monty.svg" width="180" alt="MontePY: a cute snek on a red over white circle"/>
 
-A python library to read, edit, and write MCNP input files. 
+[![license](https://img.shields.io/github/license/idaholab/MontePy.svg)](https://github.com/idaholab/MontePy/blob/develop/LICENSE)
+[![Coverage Status](https://coveralls.io/repos/github/idaholab/MontePy/badge.svg?branch=develop)](https://coveralls.io/github/idaholab/MontePy?branch=develop)
+[![PyPI version](https://badge.fury.io/py/montepy.svg)](https://badge.fury.io/py/montepy)
+
+MontePy is a python library to read, edit, and write MCNP input files. 
 
 ## Installing
 
 See the [Installing section in the user guide](https://idaholab.github.io/MontePy/starting.html#installing).
 
 
 ## User Documentation
@@ -78,15 +92,15 @@
 ## Features
 	
 * Handles almost all MCNP input syntax including: message blocks, & continue, comments, etc.
 * Parses Cells, surfaces, materials, and transforms very well.	
 * Can parse the following surfaces exactly P(X|Y|Z), C(X|Y|Z), C/(X|Y|Z) (I mean it can do PX, and PY, etc.)
 * Can read in all other inputs but not understand them	
 * Can write out full MCNP problem even if it doesn't fully understand an input.	
-* Can write out the MCNP problem verbatim, and try to match 
+* Can write out the MCNP problem verbatim, and try to match the original user formatting. 
 * Can quickly access cells, surfaces, and materials by their numbers. For example: `cell = problem.cells[105]`.
 * Can quickly update cell importances. For example `cell.importance.neutron = 2.0`.
 * Has over 240 test cases right now 
 
  
 Quick example for renumbering all of the cells in a problem:
```

### Comparing `montepy-0.2.5/README.md` & `montepy-0.2.6/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # MontePy
 
 <img src="https://raw.githubusercontent.com/idaholab/MontePy/develop/graphics/monty.svg" width="180" alt="MontePY: a cute snek on a red over white circle"/>
 
-A python library to read, edit, and write MCNP input files. 
+[![license](https://img.shields.io/github/license/idaholab/MontePy.svg)](https://github.com/idaholab/MontePy/blob/develop/LICENSE)
+[![Coverage Status](https://coveralls.io/repos/github/idaholab/MontePy/badge.svg?branch=develop)](https://coveralls.io/github/idaholab/MontePy?branch=develop)
+[![PyPI version](https://badge.fury.io/py/montepy.svg)](https://badge.fury.io/py/montepy)
+
+MontePy is a python library to read, edit, and write MCNP input files. 
 
 ## Installing
 
 See the [Installing section in the user guide](https://idaholab.github.io/MontePy/starting.html#installing).
 
 
 ## User Documentation
@@ -19,15 +23,15 @@
 ## Features
 	
 * Handles almost all MCNP input syntax including: message blocks, & continue, comments, etc.
 * Parses Cells, surfaces, materials, and transforms very well.	
 * Can parse the following surfaces exactly P(X|Y|Z), C(X|Y|Z), C/(X|Y|Z) (I mean it can do PX, and PY, etc.)
 * Can read in all other inputs but not understand them	
 * Can write out full MCNP problem even if it doesn't fully understand an input.	
-* Can write out the MCNP problem verbatim, and try to match 
+* Can write out the MCNP problem verbatim, and try to match the original user formatting. 
 * Can quickly access cells, surfaces, and materials by their numbers. For example: `cell = problem.cells[105]`.
 * Can quickly update cell importances. For example `cell.importance.neutron = 2.0`.
 * Has over 240 test cases right now 
 
  
 Quick example for renumbering all of the cells in a problem:
```

### Comparing `montepy-0.2.5/montepy/__init__.py` & `montepy-0.2.6/montepy/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,15 +19,27 @@
 from montepy import geometry_operators
 from montepy.input_parser.mcnp_input import Jump
 from montepy.particle import Particle
 from montepy.surfaces.surface_type import SurfaceType
 from montepy.universe import Universe
 import sys
 
-__version__ = "0.2.5"
+
+try:
+    from . import _version
+
+    __version__ = _version.version
+except ImportError:
+    try:
+        from setuptools_scm import get_version
+
+        __version__ = get_version()
+    except ImportError:
+        __version__ = "Undefined"
+
 
 # enable deprecated warnings for users
 if not sys.warnoptions:
     import os, warnings
 
     warnings.simplefilter("default")  # Change the filter in this process
     os.environ["PYTHONWARNINGS"] = "default"  # Also affect subprocesses
```

### Comparing `montepy-0.2.5/montepy/__main__.py` & `montepy-0.2.6/montepy/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 .. note::
     `__name__ == "__main__"` is unnecessary because this file is not
     run on import.
 """
 
 
-def define_args(args):
+def define_args(args=None):
     """
     Sets and parses the command line arguments.
 
     :returns: the arguments that were parsed
     :rtype: argparse.NameSpace
     """
     parser = argparse.ArgumentParser(
@@ -30,14 +30,20 @@
         "--check",
         action="store",
         nargs="*",
         type=str,
         help="Check the given input file(s) for errors. Accepts globs, and multiple arguments.",
         metavar="input_file",
     )
+    parser.add_argument(
+        "-v",
+        "--version",
+        action="store_true",
+        help="Print the version number",
+    )
     args = parser.parse_args(args)
     return args
 
 
 def check_inputs(files):
     """
     Checks input files for syntax errors.
@@ -54,14 +60,16 @@
         problem.parse_input(True)
 
 
 def main():  # pragma: no cover
     """
     The main function
     """
-    args = define_args(sys.argv[1:])
-    if "check" in args:
+    args = define_args()
+    if args.check:
         check_inputs(args.check)
+    if args.version:
+        print(montepy.__version__)
 
 
 if __name__ == "__main__":  # pragma: no cover
     main()
```

### Comparing `montepy-0.2.5/montepy/_cell_data_control.py` & `montepy-0.2.6/montepy/_cell_data_control.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/cell.py` & `montepy-0.2.6/montepy/cell.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/cells.py` & `montepy-0.2.6/montepy/cells.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/constants.py` & `montepy-0.2.6/montepy/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,14 +36,21 @@
 """
 
 TABSIZE = 8
 """
 How many spaces a tab is expand to.
 """
 
+ASCII_CEILING = 127
+"""
+The maximum allowed code point allowed by ASCII.
+
+Source: `Wikipedia <https://en.wikipedia.org/wiki/ASCII>`_
+"""
+
 
 def get_max_line_length(mcnp_version=DEFAULT_VERSION):
     """
     Gets the maximum allowed length for an input line for a specific MCNP version.
 
     The version must be a three component tuple e.g., (6, 2, 0) and (5, 1, 60).
     Line lengths inferred from:
```

### Comparing `montepy-0.2.5/montepy/data_inputs/cell_modifier.py` & `montepy-0.2.6/montepy/data_inputs/cell_modifier.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/data_inputs/data_input.py` & `montepy-0.2.6/montepy/data_inputs/data_input.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/data_inputs/data_parser.py` & `montepy-0.2.6/montepy/data_inputs/data_parser.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/data_inputs/element.py` & `montepy-0.2.6/montepy/data_inputs/element.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/data_inputs/fill.py` & `montepy-0.2.6/montepy/data_inputs/fill.py`

 * *Files 0% similar despite different names*

```diff
@@ -521,17 +521,19 @@
             payload = []
             for i in self._axis_range(0):
                 for j in self._axis_range(1):
                     for k in self._axis_range(2):
                         payload.append(self.universes[i][j][k].number)
         else:
             payload = [
-                self.universe.number
-                if self.universe is not None
-                else self.old_universe_number
+                (
+                    self.universe.number
+                    if self.universe is not None
+                    else self.old_universe_number
+                )
             ]
         try:
             start_transform = new_vals.index("(")
         except ValueError:
             start_transform = None
 
         reverse_list = new_vals.copy()
```

### Comparing `montepy-0.2.5/montepy/data_inputs/importance.py` & `montepy-0.2.6/montepy/data_inputs/importance.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/data_inputs/isotope.py` & `montepy-0.2.6/montepy/data_inputs/isotope.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/data_inputs/lattice_input.py` & `montepy-0.2.6/montepy/data_inputs/lattice_input.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/data_inputs/material.py` & `montepy-0.2.6/montepy/data_inputs/material.py`

 * *Files 8% similar despite different names*

```diff
@@ -112,14 +112,29 @@
         :rtype: generator
         """
         if self._problem:
             for cell in self._problem.cells:
                 if cell.material == self:
                     yield cell
 
+    def format_for_mcnp_input(self, mcnp_version):
+        """
+        Creates a string representation of this MCNP_Object that can be
+        written to file.
+
+        :param mcnp_version: The tuple for the MCNP version that must be exported to.
+        :type mcnp_version: tuple
+        :return: a list of strings for the lines that this input will occupy.
+        :rtype: list
+        """
+        lines = super().format_for_mcnp_input(mcnp_version)
+        if self.thermal_scattering is not None:
+            lines += self.thermal_scattering.format_for_mcnp_input(mcnp_version)
+        return lines
+
     def add_thermal_scattering(self, law):
         """
         Adds thermal scattering law to the material
 
         :param law: the law that is mcnp formatted
         :type law: str
         """
```

### Comparing `montepy-0.2.5/montepy/data_inputs/material_component.py` & `montepy-0.2.6/montepy/data_inputs/material_component.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/data_inputs/mode.py` & `montepy-0.2.6/montepy/data_inputs/mode.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/data_inputs/thermal_scattering.py` & `montepy-0.2.6/montepy/data_inputs/thermal_scattering.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/data_inputs/transform.py` & `montepy-0.2.6/montepy/data_inputs/transform.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/data_inputs/universe_input.py` & `montepy-0.2.6/montepy/data_inputs/universe_input.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/data_inputs/volume.py` & `montepy-0.2.6/montepy/data_inputs/volume.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/errors.py` & `montepy-0.2.6/montepy/errors.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/geometry_operators.py` & `montepy-0.2.6/montepy/geometry_operators.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/input_parser/cell_parser.py` & `montepy-0.2.6/montepy/input_parser/cell_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,15 +71,15 @@
             ret.append(node, is_comment)
         return ret
 
     @_("geometry_expr union geometry_term")
     def geometry_expr(self, p):
         left = p.geometry_expr
         right = p.geometry_term
-        nodes = {"left": left.nodes, "operator": p.union, "right": right.nodes}
+        nodes = {"left": left, "operator": p.union, "right": right}
         return syntax_node.GeometryTree("union", nodes, ":", left, right)
 
     @_("geometry_term")
     def geometry_expr(self, p):
         term = p.geometry_term
         if isinstance(term, syntax_node.ValueNode):
             term = syntax_node.GeometryTree("shift", {"left": term}, ">", term)
@@ -108,15 +108,15 @@
         if isinstance(p.geometry_term, syntax_node.GeometryTree):
             left = p.geometry_term
         else:
             left = next(node_iter)
         for node in node_iter:
             new_tree = syntax_node.GeometryTree(
                 "intersection",
-                {"left": left, "operator": None, "right": node},
+                {"left": left, "operator": syntax_node.PaddingNode(), "right": node},
                 "*",
                 left,
                 node,
             )
             left = new_tree
         return new_tree
 
@@ -138,15 +138,18 @@
 
     @_("geometry_factory")
     def geometry_factor(self, p):
         return p.geometry_factory
 
     @_("COMPLEMENT geometry_factory")
     def geometry_factor(self, p):
-        nodes = {"operator": p.COMPLEMENT, "left": p.geometry_factory}
+        nodes = {
+            "operator": syntax_node.PaddingNode(p.COMPLEMENT),
+            "left": p.geometry_factory,
+        }
         return syntax_node.GeometryTree(
             "complement",
             nodes,
             "#",
             p.geometry_factory,
         )
```

### Comparing `montepy-0.2.5/montepy/input_parser/data_parser.py` & `montepy-0.2.6/montepy/input_parser/data_parser.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/input_parser/input_reader.py` & `montepy-0.2.6/montepy/input_parser/input_reader.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 # Copyright 2024, Battelle Energy Alliance, LLC All Rights Reserved.
 from montepy import mcnp_problem
 from montepy.constants import DEFAULT_VERSION
 
 
-def read_input(input_file, mcnp_version=DEFAULT_VERSION):
+def read_input(input_file, mcnp_version=DEFAULT_VERSION, replace=True):
     """
     Reads the specified MCNP Input file.
 
     The MCNP version must be a three component tuple e.g., (6, 2, 0) and (5, 1, 60).
 
+
     :param input_file: the path to the input file to read.
     :type input_file: str
     :param mcnp_version: The version of MCNP that the input is intended for.
     :type mcnp_version: tuple
     :returns: The MCNP_Problem instance representing this file.
+    :param replace: replace all non-ASCII characters with a space (0x20)
+    :type replace: bool
     :rtype: MCNP_Problem
     :raises UnsupportedFeature: If an input format is used that MontePy does not support.
     :raises MalformedInputError: If an input has a broken syntax.
     :raises NumberConflictError: If two objects use the same number in the input file.
     :raises BrokenObjectLinkError: If a reference is made to an object that is not in the input file.
     :raises UnknownElement: If an isotope is specified for an unknown element.
     """
     problem = mcnp_problem.MCNP_Problem(input_file)
     problem.mcnp_version = mcnp_version
-    problem.parse_input()
+    problem.parse_input(replace=replace)
     return problem
```

### Comparing `montepy-0.2.5/montepy/input_parser/input_syntax_reader.py` & `montepy-0.2.6/montepy/input_parser/input_syntax_reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,35 +11,37 @@
 from montepy.input_parser.read_parser import ReadParser
 import os
 import warnings
 
 reading_queue = []
 
 
-def read_input_syntax(input_file, mcnp_version=DEFAULT_VERSION):
+def read_input_syntax(input_file, mcnp_version=DEFAULT_VERSION, replace=True):
     """
     Creates a generator function to return a new MCNP input for
     every new one that is encountered.
 
     This is meant to just handle the MCNP input syntax, it does not
     semantically parse the inputs.
 
     The version must be a three component tuple e.g., (6, 2, 0) and (5, 1, 60).
 
 
     :param input_file: the path to the input file to be read
     :type input_file: MCNP_InputFile
     :param mcnp_version: The version of MCNP that the input is intended for.
     :type mcnp_version: tuple
+    :param replace: replace all non-ASCII characters with a space (0x20)
+    :type replace: bool
     :returns: a generator of MCNP_Object objects
     :rtype: generator
     """
     global reading_queue
     reading_queue = deque()
-    with input_file.open("r") as fh:
+    with input_file.open("r", replace=replace) as fh:
         yield from read_front_matters(fh, mcnp_version)
         yield from read_data(fh, mcnp_version)
 
 
 def read_front_matters(fh, mcnp_version):
     """
     Reads the beginning of an MCNP file for all of the unusual data there.
@@ -182,15 +184,15 @@
             and not continue_input
             and not line_is_comment
             and has_non_comments
             and input_raw_lines
         ):
             yield from flush_input()
         # die if it is a vertical syntax format
-        if "#" in line[0:BLANK_SPACE_CONTINUE]:
+        if "#" in line[0:BLANK_SPACE_CONTINUE] and not line_is_comment:
             raise errors.UnsupportedFeature("Vertical Input format is not allowed")
         # cut line down to allowed length
         old_line = line
         line = line[:line_length]
         if len(old_line) != len(line):
             warnings.warn(
                 f"The line: {old_line} exceeded the allowed line length of: {line_length} for MCNP {mcnp_version}",
```

### Comparing `montepy-0.2.5/montepy/input_parser/mcnp_input.py` & `montepy-0.2.6/montepy/input_parser/mcnp_input.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/input_parser/parser_base.py` & `montepy-0.2.6/montepy/input_parser/parser_base.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/input_parser/read_parser.py` & `montepy-0.2.6/montepy/input_parser/read_parser.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/input_parser/shortcuts.py` & `montepy-0.2.6/montepy/input_parser/shortcuts.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/input_parser/surface_parser.py` & `montepy-0.2.6/montepy/input_parser/surface_parser.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/input_parser/syntax_node.py` & `montepy-0.2.6/montepy/input_parser/syntax_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,14 +218,15 @@
     :type left: GeometryTree, ValueNode
     :param right: the node of the right side of the binary tree.
     :type right: GeometryTree, ValueNode
     """
 
     def __init__(self, name, tokens, op, left, right=None):
         super().__init__(name)
+        assert all(list(map(lambda v: isinstance(v, SyntaxNodeBase), tokens.values())))
         self._nodes = tokens
         self._operator = Operator(op)
         self._left_side = left
         self._right_side = right
 
     def __str__(self):
         return f"Geometry: ( {self._left_side} {self._operator} {self._right_side} )"
@@ -237,27 +238,16 @@
         ret = ""
         for node in self.nodes.values():
             ret += node.format()
         return ret
 
     @property
     def comments(self):
-        for key, node in self.nodes.items():
-            if isinstance(node, SyntaxNodeBase):
-                yield from node.comments
-            elif isinstance(node, dict):
-                yield from GeometryTree._recurse_comments(node)
-
-    @staticmethod
-    def _recurse_comments(tree):
-        for node in tree.values():
-            if isinstance(node, SyntaxNodeBase):
-                yield from node.comments
-            elif isinstance(node, dict):
-                yield from GeometryTree._recurse_comments(node)
+        for node in self.nodes.values():
+            yield from node.comments
 
     @property
     def left(self):
         """
         The left side of the binary tree.
 
         :returns: the left node of the syntax tree.
```

### Comparing `montepy-0.2.5/montepy/input_parser/tally_parser.py` & `montepy-0.2.6/montepy/input_parser/tally_parser.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/input_parser/thermal_parser.py` & `montepy-0.2.6/montepy/input_parser/thermal_parser.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/input_parser/tokens.py` & `montepy-0.2.6/montepy/input_parser/tokens.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/materials.py` & `montepy-0.2.6/montepy/materials.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/mcnp_object.py` & `montepy-0.2.6/montepy/mcnp_object.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/mcnp_problem.py` & `montepy-0.2.6/montepy/mcnp_problem.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,35 +228,37 @@
         The collection of transform objects in this problem.
 
         :returns: a collection of transforms in the problem.
         :rtype: Transforms
         """
         return self._transforms
 
-    def parse_input(self, check_input=False):
+    def parse_input(self, check_input=False, replace=True):
         """
         Semantically parses the MCNP file provided to the constructor.
 
         :param check_input: If true, will try to find all errors with input and collect them as warnings to log.
         :type check_input: bool
+        :param replace: replace all non-ASCII characters with a space (0x20)
+        :type replace: bool
         """
         trailing_comment = None
         last_obj = None
         OBJ_MATCHER = {
             block_type.BlockType.CELL: (Cell, self._cells),
             block_type.BlockType.SURFACE: (
                 surface_builder.surface_builder,
                 self._surfaces,
             ),
             block_type.BlockType.DATA: (parse_data, self._data_inputs),
         }
         try:
             for i, input in enumerate(
                 input_syntax_reader.read_input_syntax(
-                    self._input_file, self.mcnp_version
+                    self._input_file, self.mcnp_version, replace=replace
                 )
             ):
                 self._original_inputs.append(input)
                 if i == 0 and isinstance(input, mcnp_input.Message):
                     self._message = input
 
                 elif isinstance(input, mcnp_input.Title) and self._title is None:
```

### Comparing `montepy-0.2.5/montepy/numbered_mcnp_object.py` & `montepy-0.2.6/montepy/numbered_mcnp_object.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/numbered_object_collection.py` & `montepy-0.2.6/montepy/numbered_object_collection.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/particle.py` & `montepy-0.2.6/montepy/particle.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/surface_collection.py` & `montepy-0.2.6/montepy/surface_collection.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/surfaces/axis_plane.py` & `montepy-0.2.6/montepy/surfaces/axis_plane.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/surfaces/cylinder_on_axis.py` & `montepy-0.2.6/montepy/surfaces/cylinder_on_axis.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/surfaces/cylinder_par_axis.py` & `montepy-0.2.6/montepy/surfaces/cylinder_par_axis.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/surfaces/general_plane.py` & `montepy-0.2.6/montepy/surfaces/general_plane.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/surfaces/half_space.py` & `montepy-0.2.6/montepy/surfaces/half_space.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/surfaces/surface.py` & `montepy-0.2.6/montepy/surfaces/surface.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/surfaces/surface_builder.py` & `montepy-0.2.6/montepy/surfaces/surface_builder.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/surfaces/surface_type.py` & `montepy-0.2.6/montepy/surfaces/surface_type.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/universe.py` & `montepy-0.2.6/montepy/universe.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy/utilities.py` & `montepy-0.2.6/montepy/utilities.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/montepy.egg-info/PKG-INFO` & `montepy-0.2.6/montepy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: montepy
-Version: 0.2.5
+Version: 0.2.6
 Summary: A library for reading, editing, and writing MCNP input files
 Author: Brenna Carbno
 Author-email: Micah Gale <micah.gale@inl.gov>, Travis Labossiere-Hickman <Travis.LabossiereHickman@inl.gov>
 Maintainer-email: Micah Gale <micah.gale@inl.gov>
 License: MIT License
         
         Copyright (c) 2024 Battelle Energy Alliance, LLC
@@ -43,29 +43,43 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE.txt
 License-File: AUTHORS
-Requires-Dist: numpy
+Requires-Dist: numpy>=1.18
 Requires-Dist: sly==0.5
 Provides-Extra: test
-Requires-Dist: coverage; extra == "test"
+Requires-Dist: coverage[toml]>=6.3.2; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == "doc"
 Requires-Dist: sphinxcontrib-apidoc; extra == "doc"
 Requires-Dist: sphinx_rtd_theme; extra == "doc"
+Provides-Extra: format
+Requires-Dist: black>=23.3.0; extra == "format"
+Provides-Extra: build
+Requires-Dist: build; extra == "build"
+Requires-Dist: setuptools_scm>=8; extra == "build"
+Provides-Extra: develop
+Requires-Dist: montepy[test]; extra == "develop"
+Requires-Dist: montepy[doc]; extra == "develop"
+Requires-Dist: montepy[format]; extra == "develop"
+Requires-Dist: montepy[build]; extra == "develop"
 
 # MontePy
 
 <img src="https://raw.githubusercontent.com/idaholab/MontePy/develop/graphics/monty.svg" width="180" alt="MontePY: a cute snek on a red over white circle"/>
 
-A python library to read, edit, and write MCNP input files. 
+[![license](https://img.shields.io/github/license/idaholab/MontePy.svg)](https://github.com/idaholab/MontePy/blob/develop/LICENSE)
+[![Coverage Status](https://coveralls.io/repos/github/idaholab/MontePy/badge.svg?branch=develop)](https://coveralls.io/github/idaholab/MontePy?branch=develop)
+[![PyPI version](https://badge.fury.io/py/montepy.svg)](https://badge.fury.io/py/montepy)
+
+MontePy is a python library to read, edit, and write MCNP input files. 
 
 ## Installing
 
 See the [Installing section in the user guide](https://idaholab.github.io/MontePy/starting.html#installing).
 
 
 ## User Documentation
@@ -78,15 +92,15 @@
 ## Features
 	
 * Handles almost all MCNP input syntax including: message blocks, & continue, comments, etc.
 * Parses Cells, surfaces, materials, and transforms very well.	
 * Can parse the following surfaces exactly P(X|Y|Z), C(X|Y|Z), C/(X|Y|Z) (I mean it can do PX, and PY, etc.)
 * Can read in all other inputs but not understand them	
 * Can write out full MCNP problem even if it doesn't fully understand an input.	
-* Can write out the MCNP problem verbatim, and try to match 
+* Can write out the MCNP problem verbatim, and try to match the original user formatting. 
 * Can quickly access cells, surfaces, and materials by their numbers. For example: `cell = problem.cells[105]`.
 * Can quickly update cell importances. For example `cell.importance.neutron = 2.0`.
 * Has over 240 test cases right now 
 
  
 Quick example for renumbering all of the cells in a problem:
```

### Comparing `montepy-0.2.5/pyproject.toml` & `montepy-0.2.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -26,46 +26,63 @@
        "Operating System :: OS Independent",
        "Topic :: Scientific/Engineering :: Physics",
        "Topic :: Scientific/Engineering",
        "Topic :: Scientific/Engineering :: Human Machine Interfaces",
 
 ]
 dependencies = [
-	"numpy",
+	"numpy>=1.18",
 	"sly==0.5"
 ]
 
 [project.optional-dependencies]
-test = ["coverage", "pytest"]
+test = ["coverage[toml]>=6.3.2", "pytest"]
 doc = ["sphinx", "sphinxcontrib-apidoc", "sphinx_rtd_theme"]
+format = ["black>=23.3.0"]
+build = [
+	"build",
+	"setuptools_scm>=8",
+]
+develop = [
+	"montepy[test]",
+	"montepy[doc]",
+	"montepy[format]",
+	"montepy[build]",
+]
+
 
 [project.urls]
 Homepage = "https://idaholab.github.io/MontePy/index.html"
 Repository = "https://github.com/idaholab/montepy.git"
 Documentation = "https://idaholab.github.io/MontePy/index.html"
 "Bug Tracker" = "https://github.com/idaholab/MontePy/issues"
 
+[project.scripts]
+"change_to_ascii" = "montepy._scripts.change_to_ascii:main"
+
 [build-system]
-requires = ["setuptools  >= 61.0.0"]
+requires = ["setuptools  >= 64.0.0", "setuptools_scm>=8"]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools_scm]
+version_file = "montepy/_version.py"
+
 [tool.setuptools.packages.find]
 include = ["montepy*"]
 
-[tool.setuptools.dynamic]
-version = {attr = "montepy.__version__"}
-
 [tool.coverage.run]
-source = ["montepy"]
+omit = ["montepy/_version.py","tests/*"]
 
 [tool.coverage.report]
 precision = 2
 show_missing = true
 fail_under = 90.0
 exclude_also = [
 	"\\s+@abstractmethod\\s*",
 	"pass",
 ]
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 junit_logging = "all"
+junit_family="xunit2"
+filterwarnings="error"
```

### Comparing `montepy-0.2.5/tests/test_cell_problem.py` & `montepy-0.2.6/tests/test_cell_problem.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/tests/test_data_inputs.py` & `montepy-0.2.6/tests/test_data_inputs.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/tests/test_edge_cases.py` & `montepy-0.2.6/tests/test_edge_cases.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,7 +172,8 @@
         )
         input = montepy.input_parser.mcnp_input.Input(
             in_strs, montepy.input_parser.block_type.BlockType.CELL
         )
         cell = montepy.Cell(input)
         # this step caused an error for #163
         cell.comments
+        cell._tree.format()
```

### Comparing `montepy-0.2.5/tests/test_geometry.py` & `montepy-0.2.6/tests/test_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from montepy.input_parser import syntax_node
 from montepy.surfaces.half_space import HalfSpace, UnitHalfSpace
 
 
 class TestHalfSpaceUnit(TestCase):
     def test_init(self):
         surface = montepy.surfaces.CylinderOnAxis()
-        node = montepy.input_parser.syntax_node.GeometryTree("hi", [], "*", " ", " ")
+        node = montepy.input_parser.syntax_node.GeometryTree("hi", {}, "*", " ", " ")
         half_space = HalfSpace(+surface, Operator.UNION, -surface, node)
         self.assertIs(half_space.operator, Operator.UNION)
         self.assertEqual(half_space.left, +surface)
         self.assertEqual(half_space.right, -surface)
         self.assertIs(half_space.node, node)
         with self.assertRaises(TypeError):
             HalfSpace(surface, Operator.UNION)
```

### Comparing `montepy-0.2.5/tests/test_importance.py` & `montepy-0.2.6/tests/test_importance.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/tests/test_input_file.py` & `montepy-0.2.6/tests/test_input_file.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/tests/test_integration.py` & `montepy-0.2.6/tests/test_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,14 +134,18 @@
                     self.assertEqual(gold, test)
             for i, surf in enumerate(self.simple_problem.surfaces):
                 num = surf.number
                 self.assertEqual(surf.number, test_problem.surfaces[num].number)
             for i, data in enumerate(self.simple_problem.data_inputs):
                 if isinstance(data, material.Material):
                     self.assertEqual(data.number, test_problem.data_inputs[i].number)
+                    if data.thermal_scattering is not None:
+                        assert (
+                            test_problem.data_inputs[i].thermal_scattering is not None
+                        )
                 elif isinstance(data, volume.Volume):
                     self.assertEqual(str(data), str(test_problem.data_inputs[i]))
                 else:
                     print("Rewritten data", data.data)
                     print("Original input data", test_problem.data_inputs[i].data)
                     self.assertEqual(data.data, test_problem.data_inputs[i].data)
         finally:
@@ -338,40 +342,41 @@
 
     def test_cell_card_pass_through(self):
         problem = copy.deepcopy(self.simple_problem)
         cell = problem.cells[1]
         # test input pass-through
         answer = [
             "C cells",
+            "c # hidden vertical Do not touch",
             "c",
             "1 1 20",
             "         -1000  $ dollar comment",
             "        imp:n,p=1 U=350 trcl=5 ",
         ]
         self.assertEqual(cell.format_for_mcnp_input((6, 2, 0)), answer)
         # test surface change
         new_prob = copy.deepcopy(problem)
         new_prob.surfaces[1000].number = 5
         cell = new_prob.cells[1]
         output = cell.format_for_mcnp_input((6, 2, 0))
         print(output)
-        self.assertEqual(int(output[3].split("$")[0]), -5)
+        self.assertEqual(int(output[4].split("$")[0]), -5)
         # test mass density printer
         cell.mass_density = 10.0
         with self.assertWarns(LineExpansionWarning):
             output = cell.format_for_mcnp_input((6, 2, 0))
         print(output)
-        self.assertAlmostEqual(float(output[2].split()[2]), -10)
+        self.assertAlmostEqual(float(output[3].split()[2]), -10)
         # ensure that surface number updated
         # Test material number change
         new_prob = copy.deepcopy(problem)
         new_prob.materials[1].number = 5
         cell = new_prob.cells[1]
         output = cell.format_for_mcnp_input((6, 2, 0))
-        self.assertEqual(int(output[2].split()[1]), 5)
+        self.assertEqual(int(output[3].split()[1]), 5)
 
     def test_thermal_scattering_pass_through(self):
         problem = copy.deepcopy(self.simple_problem)
         mat = problem.materials[3]
         therm = mat.thermal_scattering
         mat.number = 5
         self.assertEqual(
@@ -1027,7 +1032,16 @@
             with self.assertWarns(montepy.errors.LineExpansionWarning):
                 problem.write_to_file(out)
         finally:
             try:
                 os.remove(out)
             except FileNotFoundError:
                 pass
+
+    def test_alternate_encoding(self):
+        with self.assertRaises(UnicodeDecodeError):
+            problem = montepy.read_input(
+                os.path.join("tests", "inputs", "bad_encoding.imcnp"), replace=False
+            )
+        problem = montepy.read_input(
+            os.path.join("tests", "inputs", "bad_encoding.imcnp"), replace=True
+        )
```

### Comparing `montepy-0.2.5/tests/test_interface.py` & `montepy-0.2.6/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/tests/test_main.py` & `montepy-0.2.6/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/tests/test_material.py` & `montepy-0.2.6/tests/test_material.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/tests/test_mcnp_problem.py` & `montepy-0.2.6/tests/test_mcnp_problem.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/tests/test_mode.py` & `montepy-0.2.6/tests/test_mode.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/tests/test_numbered_collection.py` & `montepy-0.2.6/tests/test_numbered_collection.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/tests/test_source_def.py` & `montepy-0.2.6/tests/test_source_def.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/tests/test_surfaces.py` & `montepy-0.2.6/tests/test_surfaces.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/tests/test_syntax_parsing.py` & `montepy-0.2.6/tests/test_syntax_parsing.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/tests/test_tally.py` & `montepy-0.2.6/tests/test_tally.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/tests/test_transform.py` & `montepy-0.2.6/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/tests/test_universe.py` & `montepy-0.2.6/tests/test_universe.py`

 * *Files identical despite different names*

### Comparing `montepy-0.2.5/tests/test_utilities.py` & `montepy-0.2.6/tests/test_utilities.py`

 * *Files identical despite different names*

