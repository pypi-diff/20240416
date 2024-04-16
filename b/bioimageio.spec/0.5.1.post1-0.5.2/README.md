# Comparing `tmp/bioimageio.spec-0.5.1.post1.tar.gz` & `tmp/bioimageio.spec-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioimageio.spec-0.5.1.post1.tar", last modified: Tue Apr  9 09:13:43 2024, max compression
+gzip compressed data, was "bioimageio.spec-0.5.2.tar", last modified: Tue Apr 16 15:31:26 2024, max compression
```

## Comparing `bioimageio.spec-0.5.1.post1.tar` & `bioimageio.spec-0.5.2.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.709106 bioimageio.spec-0.5.1.post1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    18775 2024-04-09 09:13:43.709106 bioimageio.spec-0.5.1.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17946 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.689105 bioimageio.spec-0.5.1.post1/bioimageio/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.697106 bioimageio.spec-0.5.1.post1/bioimageio/spec/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-09 09:13:41.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_build_description.py
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_description.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.701105 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10694 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/_generated_spdx_license_literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    16168 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/common_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/docs_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/field_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/field_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)    20406 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/io_basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/license_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/packaging_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/root_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-09 09:13:41.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/url.py
--rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/validated_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/validation_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/validator_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/version_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/warning_levels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_io.py
--rw-r--r--   0 runner    (1001) docker     (127)    11106 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.701105 bioimageio.spec-0.5.1.post1/bioimageio/spec/application/
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/application/v0_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/application/v0_3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.701105 bioimageio.spec-0.5.1.post1/bioimageio/spec/collection/
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11116 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/collection/v0_2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12553 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/collection/v0_3.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.701105 bioimageio.spec-0.5.1.post1/bioimageio/spec/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/dataset/v0_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/dataset/v0_3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.701105 bioimageio.spec-0.5.1.post1/bioimageio/spec/generic/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/generic/_v0_2_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/generic/_v0_3_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    15487 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/generic/v0_2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14245 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/generic/v0_3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.701105 bioimageio.spec-0.5.1.post1/bioimageio/spec/model/
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/model/_v0_3_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/model/_v0_4_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    40287 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/model/v0_4.py
--rw-r--r--   0 runner    (1001) docker     (127)    99793 2024-04-09 09:13:41.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/model/v0_5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.705105 bioimageio.spec-0.5.1.post1/bioimageio/spec/notebook/
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/notebook/v0_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/notebook/v0_3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.705105 bioimageio.spec-0.5.1.post1/bioimageio/spec/partner_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/partner_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.705105 bioimageio.spec-0.5.1.post1/bioimageio/spec/partner_utils/imjoy/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/partner_utils/imjoy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8530 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/partner_utils/imjoy/_plugin_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/pretty_validation_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.705105 bioimageio.spec-0.5.1.post1/bioimageio/spec/static/
--rw-r--r--   0 runner    (1001) docker     (127)   258617 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/static/spdx_licenses.json
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/static/tag_categories.json
--rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.693106 bioimageio.spec-0.5.1.post1/bioimageio.spec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18775 2024-04-09 09:13:43.000000 bioimageio.spec-0.5.1.post1/bioimageio.spec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-04-09 09:13:43.000000 bioimageio.spec-0.5.1.post1/bioimageio.spec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 09:13:43.000000 bioimageio.spec-0.5.1.post1/bioimageio.spec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-09 09:13:43.000000 bioimageio.spec-0.5.1.post1/bioimageio.spec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-09 09:13:43.000000 bioimageio.spec-0.5.1.post1/bioimageio.spec.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.693106 bioimageio.spec-0.5.1.post1/example_descriptions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.693106 bioimageio.spec-0.5.1.post1/example_descriptions/collections/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.705105 bioimageio.spec-0.5.1.post1/example_descriptions/collections/unet2d_nuclei_broad_coll/
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/example_descriptions/collections/unet2d_nuclei_broad_coll/unet2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.693106 bioimageio.spec-0.5.1.post1/example_descriptions/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.705105 bioimageio.spec-0.5.1.post1/example_descriptions/models/unet2d_diff_output_shape/
--rw-r--r--   0 runner    (1001) docker     (127)    12778 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/example_descriptions/models/unet2d_diff_output_shape/resize_unet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.705105 bioimageio.spec-0.5.1.post1/example_descriptions/models/unet2d_fixed_shape/
--rw-r--r--   0 runner    (1001) docker     (127)    21841 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/example_descriptions/models/unet2d_fixed_shape/unet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.705105 bioimageio.spec-0.5.1.post1/example_descriptions/models/unet2d_multi_tensor/
--rw-r--r--   0 runner    (1001) docker     (127)    12970 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/example_descriptions/models/unet2d_multi_tensor/multi_tensor_unet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.705105 bioimageio.spec-0.5.1.post1/example_descriptions/models/unet2d_nuclei_broad/
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/example_descriptions/models/unet2d_nuclei_broad/unet2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/example_descriptions/models/unet2d_nuclei_broad/unet2d_expand_output_shape.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.705105 bioimageio.spec-0.5.1.post1/example_descriptions/models/upsample_test_model/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/example_descriptions/models/upsample_test_model/upsample_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.705105 bioimageio.spec-0.5.1.post1/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/scripts/compare_yaml_syntax.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/scripts/generate_dtype_limits.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/scripts/generate_json_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)    17796 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/scripts/generate_spec_documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/scripts/generate_version_submodule_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)    12159 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/scripts/report_invalid_rdfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/scripts/update_spdx_licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 09:13:43.709106 bioimageio.spec-0.5.1.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-09 09:13:41.000000 bioimageio.spec-0.5.1.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.709106 bioimageio.spec-0.5.1.post1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    13449 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_bioimageio_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_description.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_example_specs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.709106 bioimageio.spec-0.5.1.post1/tests/test_generic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_generic/test_v0_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_generic/test_v0_3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.709106 bioimageio.spec-0.5.1.post1/tests/test_internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_internal/test_base_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_internal/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_internal/test_file_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_internal/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_internal/test_license_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_internal/test_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_internal/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_internal/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_internal/test_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_internal/test_validated_string.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_internal/test_version_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.709106 bioimageio.spec-0.5.1.post1/tests/test_model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16073 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_model/test_v0_4.py
--rw-r--r--   0 runner    (1001) docker     (127)    14867 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_model/test_v0_5.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_specific_reexports_generics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:31:26.073504 bioimageio.spec-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18938 2024-04-16 15:31:26.073504 bioimageio.spec-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18115 2024-04-16 15:31:24.000000 bioimageio.spec-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:31:26.053504 bioimageio.spec-0.5.2/bioimageio/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:31:26.057504 bioimageio.spec-0.5.2/bioimageio/spec/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-16 15:31:24.000000 bioimageio.spec-0.5.2/bioimageio/spec/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/_build_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/_description.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:31:26.061504 bioimageio.spec-0.5.2/bioimageio/spec/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10694 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/_internal/_generated_spdx_license_literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/_internal/_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16168 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/_internal/common_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/_internal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/_internal/docs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/_internal/field_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/_internal/field_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20499 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/_internal/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/_internal/io_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/_internal/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/_internal/license_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/_internal/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/_internal/packaging_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/_internal/root_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/_internal/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/_internal/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/_internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/_internal/validated_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/_internal/validation_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/_internal/validator_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/_internal/version_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/_internal/warning_levels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11106 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/_package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:31:26.061504 bioimageio.spec-0.5.2/bioimageio/spec/application/
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/application/v0_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/application/v0_3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:31:26.061504 bioimageio.spec-0.5.2/bioimageio/spec/collection/
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11116 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/collection/v0_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12553 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/collection/v0_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:31:26.061504 bioimageio.spec-0.5.2/bioimageio/spec/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/dataset/v0_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/dataset/v0_3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:31:26.061504 bioimageio.spec-0.5.2/bioimageio/spec/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/generic/_v0_2_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/generic/_v0_3_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15487 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/generic/v0_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14245 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/generic/v0_3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:31:26.065504 bioimageio.spec-0.5.2/bioimageio/spec/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/model/_v0_3_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/model/_v0_4_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40294 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/model/v0_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100937 2024-04-16 15:31:24.000000 bioimageio.spec-0.5.2/bioimageio/spec/model/v0_5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:31:26.065504 bioimageio.spec-0.5.2/bioimageio/spec/notebook/
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/notebook/v0_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/notebook/v0_3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:31:26.065504 bioimageio.spec-0.5.2/bioimageio/spec/partner_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/partner_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:31:26.065504 bioimageio.spec-0.5.2/bioimageio/spec/partner_utils/imjoy/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/partner_utils/imjoy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8530 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/partner_utils/imjoy/_plugin_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/pretty_validation_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:31:26.065504 bioimageio.spec-0.5.2/bioimageio/spec/static/
+-rw-r--r--   0 runner    (1001) docker     (127)   258617 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/static/spdx_licenses.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/static/tag_categories.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/bioimageio/spec/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:31:26.057504 bioimageio.spec-0.5.2/bioimageio.spec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18938 2024-04-16 15:31:26.000000 bioimageio.spec-0.5.2/bioimageio.spec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-04-16 15:31:26.000000 bioimageio.spec-0.5.2/bioimageio.spec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:31:26.000000 bioimageio.spec-0.5.2/bioimageio.spec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-16 15:31:26.000000 bioimageio.spec-0.5.2/bioimageio.spec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-16 15:31:26.000000 bioimageio.spec-0.5.2/bioimageio.spec.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:31:26.053504 bioimageio.spec-0.5.2/example_descriptions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:31:26.053504 bioimageio.spec-0.5.2/example_descriptions/collections/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:31:26.065504 bioimageio.spec-0.5.2/example_descriptions/collections/unet2d_nuclei_broad_coll/
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-16 15:28:57.000000 bioimageio.spec-0.5.2/example_descriptions/collections/unet2d_nuclei_broad_coll/unet2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:31:26.053504 bioimageio.spec-0.5.2/example_descriptions/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:31:26.065504 bioimageio.spec-0.5.2/example_descriptions/models/unet2d_diff_output_shape/
+-rw-r--r--   0 runner    (1001) docker     (127)    12778 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/example_descriptions/models/unet2d_diff_output_shape/resize_unet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:31:26.065504 bioimageio.spec-0.5.2/example_descriptions/models/unet2d_fixed_shape/
+-rw-r--r--   0 runner    (1001) docker     (127)    21841 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/example_descriptions/models/unet2d_fixed_shape/unet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:31:26.065504 bioimageio.spec-0.5.2/example_descriptions/models/unet2d_multi_tensor/
+-rw-r--r--   0 runner    (1001) docker     (127)    12970 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/example_descriptions/models/unet2d_multi_tensor/multi_tensor_unet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:31:26.065504 bioimageio.spec-0.5.2/example_descriptions/models/unet2d_nuclei_broad/
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/example_descriptions/models/unet2d_nuclei_broad/unet2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/example_descriptions/models/unet2d_nuclei_broad/unet2d_expand_output_shape.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:31:26.065504 bioimageio.spec-0.5.2/example_descriptions/models/upsample_test_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/example_descriptions/models/upsample_test_model/upsample_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:31:26.069504 bioimageio.spec-0.5.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/scripts/compare_yaml_syntax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/scripts/generate_dtype_limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/scripts/generate_json_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17796 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/scripts/generate_spec_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/scripts/generate_version_submodule_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12159 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/scripts/report_invalid_rdfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/scripts/update_spdx_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 15:31:26.073504 bioimageio.spec-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:31:26.069504 bioimageio.spec-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13449 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/tests/test_bioimageio_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/tests/test_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/tests/test_example_specs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:31:26.069504 bioimageio.spec-0.5.2/tests/test_generic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/tests/test_generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/tests/test_generic/test_v0_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/tests/test_generic/test_v0_3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:31:26.069504 bioimageio.spec-0.5.2/tests/test_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/tests/test_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/tests/test_internal/test_base_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/tests/test_internal/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/tests/test_internal/test_file_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/tests/test_internal/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/tests/test_internal/test_license_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/tests/test_internal/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/tests/test_internal/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/tests/test_internal/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/tests/test_internal/test_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/tests/test_internal/test_validated_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/tests/test_internal/test_version_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/tests/test_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:31:26.069504 bioimageio.spec-0.5.2/tests/test_model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/tests/test_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16073 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/tests/test_model/test_v0_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15505 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/tests/test_model/test_v0_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-16 15:28:58.000000 bioimageio.spec-0.5.2/tests/test_specific_reexports_generics.py
```

### Comparing `bioimageio.spec-0.5.1.post1/LICENSE` & `bioimageio.spec-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/PKG-INFO` & `bioimageio.spec-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioimageio.spec
-Version: 0.5.1.post1
+Version: 0.5.2
 Summary: Parser and validator library for bioimage.io specifications
 Home-page: https://github.com/bioimage-io/spec-bioimage-io
 Author: bioimage.io Team
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bioimage-io/spec-bioimage-io/issues
 Project-URL: Source, https://github.com/bioimage-io/spec-bioimage-io
 Platform: UNKNOWN
@@ -106,14 +106,18 @@
 
 Made with [contrib.rocks](https://contrib.rocks).
 
 ## Δ Changelog
 
 ### bioimageio.spec Python package
 
+#### bioimageio.spec 0.5.2
+
+* new patch version model 0.5.2
+
 #### bioimageio.spec 0.5.1
 
 * new patch version model 0.5.1
 
 #### bioimageio.spec 0.5.0post2
 
 * don't fail if CI env var is a string
@@ -253,14 +257,19 @@
 
 #### bioimageio.spec 0.4.0.post2
 
 * `load_raw_resource_description` accepts `update_to_format` kwarg
 
 ### Resource Description Format Versions
 
+#### model 0.5.2
+
+* Non-breaking changes
+  * added `concatenable` flag to index, time and space input axes
+
 #### model 0.5.1
 
 * Non-breaking changes
   * added `DataDependentSize` for `outputs.i.size` to specify an output shape that is not known before inference is run.
   * added optional `inputs.i.optional` field to indicate that a tensor may be `None`
   * made data type assumptions in `preprocessing` and `postprocessing` explicit by adding `'ensure_dtype'` operations per default.
   * allow to specify multiple thresholds (along an `axis`) in a 'binarize' processing step
```

### Comparing `bioimageio.spec-0.5.1.post1/README.md` & `bioimageio.spec-0.5.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,18 @@
 
 Made with [contrib.rocks](https://contrib.rocks).
 
 ## Δ Changelog
 
 ### bioimageio.spec Python package
 
+#### bioimageio.spec 0.5.2
+
+* new patch version model 0.5.2
+
 #### bioimageio.spec 0.5.1
 
 * new patch version model 0.5.1
 
 #### bioimageio.spec 0.5.0post2
 
 * don't fail if CI env var is a string
@@ -232,14 +236,19 @@
 
 #### bioimageio.spec 0.4.0.post2
 
 * `load_raw_resource_description` accepts `update_to_format` kwarg
 
 ### Resource Description Format Versions
 
+#### model 0.5.2
+
+* Non-breaking changes
+  * added `concatenable` flag to index, time and space input axes
+
 #### model 0.5.1
 
 * Non-breaking changes
   * added `DataDependentSize` for `outputs.i.size` to specify an output shape that is not known before inference is run.
   * added optional `inputs.i.optional` field to indicate that a tensor may be `None`
   * made data type assumptions in `preprocessing` and `postprocessing` explicit by adding `'ensure_dtype'` operations per default.
   * allow to specify multiple thresholds (along an `axis`) in a 'binarize' processing step
```

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/__init__.py` & `bioimageio.spec-0.5.2/bioimageio/spec/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/_build_description.py` & `bioimageio.spec-0.5.2/bioimageio/spec/_build_description.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/_description.py` & `bioimageio.spec-0.5.2/bioimageio/spec/_description.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/_generated_spdx_license_literals.py` & `bioimageio.spec-0.5.2/bioimageio/spec/_internal/_generated_spdx_license_literals.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/_settings.py` & `bioimageio.spec-0.5.2/bioimageio/spec/_internal/_settings.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/common_nodes.py` & `bioimageio.spec-0.5.2/bioimageio/spec/_internal/common_nodes.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/constants.py` & `bioimageio.spec-0.5.2/bioimageio/spec/_internal/constants.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/docs_utils.py` & `bioimageio.spec-0.5.2/bioimageio/spec/_internal/docs_utils.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/field_validation.py` & `bioimageio.spec-0.5.2/bioimageio/spec/_internal/field_validation.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/field_warning.py` & `bioimageio.spec-0.5.2/bioimageio/spec/_internal/field_warning.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/io.py` & `bioimageio.spec-0.5.2/bioimageio/spec/_internal/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,17 +63,15 @@
     FileName,
 )
 from .._internal.node import Node
 from .._internal.packaging_context import packaging_context_var
 from .._internal.root_url import RootHttpUrl
 from .._internal.url import HttpUrl
 from .._internal.validated_string import ValidatedString
-from .._internal.validation_context import (
-    validation_context_var,
-)
+from .._internal.validation_context import ValidationContext, validation_context_var
 from .validator_annotations import AfterValidator
 
 if sys.version_info < (3, 10):
     SLOTS: Dict[str, bool] = {}
 else:
     SLOTS = {"slots": True}
 
@@ -525,15 +523,18 @@
 def interprete_file_source(file_source: PermissiveFileSource) -> StrictFileSource:
     if isinstance(file_source, (HttpUrl, Path)):
         return file_source
 
     if isinstance(file_source, pydantic.AnyUrl):
         file_source = str(file_source)
 
-    return _strict_file_source_adapter.validate_python(file_source)
+    with ValidationContext(perform_io_checks=False):
+        strict = _strict_file_source_adapter.validate_python(file_source)
+
+    return strict
 
 
 def _get_known_hash(hash_kwargs: HashKwargs):
     if "sha256" in hash_kwargs and hash_kwargs["sha256"] is not None:
         return f"sha256:{hash_kwargs['sha256']}"
     else:
         return None
@@ -631,15 +632,15 @@
     def download(self):
 
         return download(self.source, sha256=self.sha256)
 
 
 def extract_file_name(
     src: Union[pydantic.HttpUrl, HttpUrl, PurePath, RelativeFilePath],
-) -> str:
+) -> FileName:
     if isinstance(src, RelativeFilePath):
         return src.path.name
     elif isinstance(src, PurePath):
         return src.name
     else:
         url = urlparse(str(src))
         if (
```

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/io_utils.py` & `bioimageio.spec-0.5.2/bioimageio/spec/_internal/io_utils.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/license_id.py` & `bioimageio.spec-0.5.2/bioimageio/spec/_internal/license_id.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/node.py` & `bioimageio.spec-0.5.2/bioimageio/spec/_internal/node.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/packaging_context.py` & `bioimageio.spec-0.5.2/bioimageio/spec/_internal/packaging_context.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/root_url.py` & `bioimageio.spec-0.5.2/bioimageio/spec/_internal/root_url.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/types.py` & `bioimageio.spec-0.5.2/bioimageio/spec/_internal/types.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/url.py` & `bioimageio.spec-0.5.2/bioimageio/spec/_internal/url.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/utils.py` & `bioimageio.spec-0.5.2/bioimageio/spec/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/validated_string.py` & `bioimageio.spec-0.5.2/bioimageio/spec/_internal/validated_string.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/validation_context.py` & `bioimageio.spec-0.5.2/bioimageio/spec/_internal/validation_context.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/validator_annotations.py` & `bioimageio.spec-0.5.2/bioimageio/spec/_internal/validator_annotations.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/version_type.py` & `bioimageio.spec-0.5.2/bioimageio/spec/_internal/version_type.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/warning_levels.py` & `bioimageio.spec-0.5.2/bioimageio/spec/_internal/warning_levels.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/_io.py` & `bioimageio.spec-0.5.2/bioimageio/spec/_io.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/_package.py` & `bioimageio.spec-0.5.2/bioimageio/spec/_package.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/application/__init__.py` & `bioimageio.spec-0.5.2/bioimageio/spec/application/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/application/v0_2.py` & `bioimageio.spec-0.5.2/bioimageio/spec/application/v0_2.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/application/v0_3.py` & `bioimageio.spec-0.5.2/bioimageio/spec/application/v0_3.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/collection/__init__.py` & `bioimageio.spec-0.5.2/bioimageio/spec/collection/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/collection/v0_2.py` & `bioimageio.spec-0.5.2/bioimageio/spec/collection/v0_2.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/collection/v0_3.py` & `bioimageio.spec-0.5.2/bioimageio/spec/collection/v0_3.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/common.py` & `bioimageio.spec-0.5.2/bioimageio/spec/common.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/dataset/__init__.py` & `bioimageio.spec-0.5.2/bioimageio/spec/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/dataset/v0_2.py` & `bioimageio.spec-0.5.2/bioimageio/spec/dataset/v0_2.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/dataset/v0_3.py` & `bioimageio.spec-0.5.2/bioimageio/spec/dataset/v0_3.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/generic/__init__.py` & `bioimageio.spec-0.5.2/bioimageio/spec/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/generic/_v0_2_converter.py` & `bioimageio.spec-0.5.2/bioimageio/spec/generic/_v0_2_converter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/generic/_v0_3_converter.py` & `bioimageio.spec-0.5.2/bioimageio/spec/generic/_v0_3_converter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/generic/v0_2.py` & `bioimageio.spec-0.5.2/bioimageio/spec/generic/v0_2.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/generic/v0_3.py` & `bioimageio.spec-0.5.2/bioimageio/spec/generic/v0_3.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/model/__init__.py` & `bioimageio.spec-0.5.2/bioimageio/spec/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/model/_v0_3_converter.py` & `bioimageio.spec-0.5.2/bioimageio/spec/model/_v0_3_converter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/model/_v0_4_converter.py` & `bioimageio.spec-0.5.2/bioimageio/spec/model/_v0_4_converter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/model/v0_4.py` & `bioimageio.spec-0.5.2/bioimageio/spec/model/v0_4.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 )
 
 import numpy as np
 from annotated_types import Ge, Interval, MaxLen, MinLen, MultipleOf
 from numpy.typing import NDArray
 from pydantic import (
     AllowInfNan,
+    Discriminator,
     Field,
     TypeAdapter,
     ValidationInfo,
     field_validator,
     model_validator,
 )
 from typing_extensions import Annotated, LiteralString, Self, assert_never
@@ -719,27 +720,27 @@
         BinarizeDescr,
         ClipDescr,
         ScaleLinearDescr,
         SigmoidDescr,
         ZeroMeanUnitVarianceDescr,
         ScaleRangeDescr,
     ],
-    Field(discriminator="name"),
+    Discriminator("name"),
 ]
 PostprocessingDescr = Annotated[
     Union[
         BinarizeDescr,
         ClipDescr,
         ScaleLinearDescr,
         SigmoidDescr,
         ZeroMeanUnitVarianceDescr,
         ScaleRangeDescr,
         ScaleMeanVarianceDescr,
     ],
-    Field(discriminator="name"),
+    Discriminator("name"),
 ]
 
 
 class InputTensorDescr(TensorDescrBase):
     data_type: Literal["float32", "uint8", "uint16"]
     """For now an input tensor is expected to be given as `float32`.
     The data flow in bioimage.io models is explained
```

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/model/v0_5.py` & `bioimageio.spec-0.5.2/bioimageio/spec/model/v0_5.py`

 * *Files 2% similar despite different names*

```diff
@@ -279,14 +279,16 @@
 
     `axis.size = reference.size * reference.scale / axis.scale + offset`
 
     note:
     1. The axis and the referenced axis need to have the same unit (or no unit).
     2. Batch axes may not be referenced.
     3. Fractions are rounded down.
+    4. If the reference axis is `concatenable` the referencing axis is assumed to be
+        `concatenable` as well with the same block order.
 
     example:
     An unisotropic input image of w*h=100*49 pixels depicts a phsical space of 200*196mm².
     Let's assume that we want to express the image height h in relation to its width w
     instead of only accepting input images of exactly 100*49 pixels
     (for example to express a range of valid image shapes by parametrizing w, see `ParameterizedSize`).
 
@@ -430,28 +432,36 @@
     otherwise (the default) it may be chosen arbitrarily depending on available memory"""
 
     @property
     def scale(self):
         return 1.0
 
     @property
+    def concatenable(self):
+        return True
+
+    @property
     def unit(self):
         return None
 
 
 class ChannelAxis(AxisBase):
     type: Literal["channel"] = "channel"
     id: NonBatchAxisId = AxisId("channel")
-    channel_names: List[Identifier]
+    channel_names: NotEmpty[List[Identifier]]
 
     @property
     def size(self) -> int:
         return len(self.channel_names)
 
     @property
+    def concatenable(self):
+        return False
+
+    @property
     def scale(self) -> float:
         return 1.0
 
     @property
     def unit(self):
         return None
 
@@ -486,15 +496,20 @@
     - fixed integer
     - parameterized series of valid sizes (`ParameterizedSize`)
     - reference to another axis with an optional offset (`SizeReference`)
     """
 
 
 class IndexInputAxis(IndexAxisBase, _WithInputAxisSize):
-    pass
+    concatenable: bool = False
+    """If a model has a `concatenable` input axis, it can be processed blockwise,
+    splitting a longer sample axis into blocks matching its input tensor description.
+    Output axes are concatenable if they have a `SizeReference` to a concatenable
+    input axis.
+    """
 
 
 class IndexOutputAxis(IndexAxisBase):
     size: Annotated[
         Union[Annotated[int, Gt(0)], SizeReference, DataDependentSize],
         Field(
             examples=[
@@ -516,32 +531,42 @@
     type: Literal["time"] = "time"
     id: NonBatchAxisId = AxisId("time")
     unit: Optional[TimeUnit] = None
     scale: Annotated[float, Gt(0)] = 1.0
 
 
 class TimeInputAxis(TimeAxisBase, _WithInputAxisSize):
-    pass
+    concatenable: bool = False
+    """If a model has a `concatenable` input axis, it can be processed blockwise,
+    splitting a longer sample axis into blocks matching its input tensor description.
+    Output axes are concatenable if they have a `SizeReference` to a concatenable
+    input axis.
+    """
 
 
 class SpaceAxisBase(AxisBase):
     type: Literal["space"] = "space"
     id: Annotated[NonBatchAxisId, Field(examples=["x", "y", "z"])] = AxisId("x")
     unit: Optional[SpaceUnit] = None
     scale: Annotated[float, Gt(0)] = 1.0
 
 
 class SpaceInputAxis(SpaceAxisBase, _WithInputAxisSize):
-    pass
+    concatenable: bool = False
+    """If a model has a `concatenable` input axis, it can be processed blockwise,
+    splitting a longer sample axis into blocks matching its input tensor description.
+    Output axes are concatenable if they have a `SizeReference` to a concatenable
+    input axis.
+    """
 
 
 _InputAxisUnion = Union[
     BatchAxis, ChannelAxis, IndexInputAxis, TimeInputAxis, SpaceInputAxis
 ]
-InputAxis = Annotated[_InputAxisUnion, Field(discriminator="type")]
+InputAxis = Annotated[_InputAxisUnion, Discriminator("type")]
 
 
 class _WithOutputAxisSize(Node):
     size: Annotated[
         Union[Annotated[int, Gt(0)], SizeReference],
         Field(
             examples=[
@@ -598,15 +623,15 @@
     Discriminator(_get_halo_axis_discriminator_value),
 ]
 
 
 _OutputAxisUnion = Union[
     BatchAxis, ChannelAxis, IndexOutputAxis, _TimeOutputAxisUnion, _SpaceOutputAxisUnion
 ]
-OutputAxis = Annotated[_OutputAxisUnion, Field(discriminator="type")]
+OutputAxis = Annotated[_OutputAxisUnion, Discriminator("type")]
 
 AnyAxis = Union[InputAxis, OutputAxis]
 
 TVs = Union[
     NotEmpty[List[int]],
     NotEmpty[List[float]],
     NotEmpty[List[bool]],
@@ -1008,29 +1033,29 @@
         EnsureDtypeDescr,
         ScaleLinearDescr,
         SigmoidDescr,
         FixedZeroMeanUnitVarianceDescr,
         ZeroMeanUnitVarianceDescr,
         ScaleRangeDescr,
     ],
-    Field(discriminator="id"),
+    Discriminator("id"),
 ]
 PostprocessingDescr = Annotated[
     Union[
         BinarizeDescr,
         ClipDescr,
         EnsureDtypeDescr,
         ScaleLinearDescr,
         SigmoidDescr,
         FixedZeroMeanUnitVarianceDescr,
         ZeroMeanUnitVarianceDescr,
         ScaleRangeDescr,
         ScaleMeanVarianceDescr,
     ],
-    Field(discriminator="id"),
+    Discriminator("id"),
 ]
 
 IO_AxisT = TypeVar("IO_AxisT", InputAxis, OutputAxis)
 
 
 class TensorDescrBase(Node, Generic[IO_AxisT]):
     id: TensorId
```

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/notebook/__init__.py` & `bioimageio.spec-0.5.2/bioimageio/spec/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/notebook/v0_2.py` & `bioimageio.spec-0.5.2/bioimageio/spec/notebook/v0_2.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/notebook/v0_3.py` & `bioimageio.spec-0.5.2/bioimageio/spec/notebook/v0_3.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/partner_utils/imjoy/_plugin_parser.py` & `bioimageio.spec-0.5.2/bioimageio/spec/partner_utils/imjoy/_plugin_parser.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/pretty_validation_errors.py` & `bioimageio.spec-0.5.2/bioimageio/spec/pretty_validation_errors.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/static/spdx_licenses.json` & `bioimageio.spec-0.5.2/bioimageio/spec/static/spdx_licenses.json`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/static/tag_categories.json` & `bioimageio.spec-0.5.2/bioimageio/spec/static/tag_categories.json`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio/spec/summary.py` & `bioimageio.spec-0.5.2/bioimageio/spec/summary.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio.spec.egg-info/PKG-INFO` & `bioimageio.spec-0.5.2/bioimageio.spec.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioimageio.spec
-Version: 0.5.1.post1
+Version: 0.5.2
 Summary: Parser and validator library for bioimage.io specifications
 Home-page: https://github.com/bioimage-io/spec-bioimage-io
 Author: bioimage.io Team
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bioimage-io/spec-bioimage-io/issues
 Project-URL: Source, https://github.com/bioimage-io/spec-bioimage-io
 Platform: UNKNOWN
@@ -106,14 +106,18 @@
 
 Made with [contrib.rocks](https://contrib.rocks).
 
 ## Δ Changelog
 
 ### bioimageio.spec Python package
 
+#### bioimageio.spec 0.5.2
+
+* new patch version model 0.5.2
+
 #### bioimageio.spec 0.5.1
 
 * new patch version model 0.5.1
 
 #### bioimageio.spec 0.5.0post2
 
 * don't fail if CI env var is a string
@@ -253,14 +257,19 @@
 
 #### bioimageio.spec 0.4.0.post2
 
 * `load_raw_resource_description` accepts `update_to_format` kwarg
 
 ### Resource Description Format Versions
 
+#### model 0.5.2
+
+* Non-breaking changes
+  * added `concatenable` flag to index, time and space input axes
+
 #### model 0.5.1
 
 * Non-breaking changes
   * added `DataDependentSize` for `outputs.i.size` to specify an output shape that is not known before inference is run.
   * added optional `inputs.i.optional` field to indicate that a tensor may be `None`
   * made data type assumptions in `preprocessing` and `postprocessing` explicit by adding `'ensure_dtype'` operations per default.
   * allow to specify multiple thresholds (along an `axis`) in a 'binarize' processing step
```

### Comparing `bioimageio.spec-0.5.1.post1/bioimageio.spec.egg-info/SOURCES.txt` & `bioimageio.spec-0.5.2/bioimageio.spec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/example_descriptions/collections/unet2d_nuclei_broad_coll/unet2d.py` & `bioimageio.spec-0.5.2/example_descriptions/collections/unet2d_nuclei_broad_coll/unet2d.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/example_descriptions/models/unet2d_diff_output_shape/resize_unet.py` & `bioimageio.spec-0.5.2/example_descriptions/models/unet2d_diff_output_shape/resize_unet.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/example_descriptions/models/unet2d_fixed_shape/unet.py` & `bioimageio.spec-0.5.2/example_descriptions/models/unet2d_fixed_shape/unet.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/example_descriptions/models/unet2d_multi_tensor/multi_tensor_unet.py` & `bioimageio.spec-0.5.2/example_descriptions/models/unet2d_multi_tensor/multi_tensor_unet.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/example_descriptions/models/unet2d_nuclei_broad/unet2d.py` & `bioimageio.spec-0.5.2/example_descriptions/models/unet2d_nuclei_broad/unet2d.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/example_descriptions/models/unet2d_nuclei_broad/unet2d_expand_output_shape.py` & `bioimageio.spec-0.5.2/example_descriptions/models/unet2d_nuclei_broad/unet2d_expand_output_shape.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/pyproject.toml` & `bioimageio.spec-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/scripts/compare_yaml_syntax.py` & `bioimageio.spec-0.5.2/scripts/compare_yaml_syntax.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/scripts/generate_json_schemas.py` & `bioimageio.spec-0.5.2/scripts/generate_json_schemas.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/scripts/generate_spec_documentation.py` & `bioimageio.spec-0.5.2/scripts/generate_spec_documentation.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/scripts/generate_version_submodule_imports.py` & `bioimageio.spec-0.5.2/scripts/generate_version_submodule_imports.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/scripts/report_invalid_rdfs.py` & `bioimageio.spec-0.5.2/scripts/report_invalid_rdfs.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/scripts/update_spdx_licenses.py` & `bioimageio.spec-0.5.2/scripts/update_spdx_licenses.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/setup.py` & `bioimageio.spec-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/tests/test_bioimageio_collection.py` & `bioimageio.spec-0.5.2/tests/test_bioimageio_collection.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/tests/test_description.py` & `bioimageio.spec-0.5.2/tests/test_description.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/tests/test_example_specs.py` & `bioimageio.spec-0.5.2/tests/test_example_specs.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/tests/test_generic/test_v0_2.py` & `bioimageio.spec-0.5.2/tests/test_generic/test_v0_2.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/tests/test_generic/test_v0_3.py` & `bioimageio.spec-0.5.2/tests/test_generic/test_v0_3.py`

 * *Files 15% similar despite different names*

```diff
@@ -143,23 +143,17 @@
 
 
 @pytest.mark.parametrize(
     "src,adapter",
     [
         (UNET2D_ROOT / "README.md", a)
         for a in [
-            TypeAdapter(
-                Annotated[FilePath, WithSuffix(".md", case_sensitive=True)]
-            ),  # pyright: ignore[reportCallIssue]
-            TypeAdapter(
-                Annotated[Path, WithSuffix(".md", case_sensitive=True)]
-            ),  # pyright: ignore[reportCallIssue]
-            TypeAdapter(
-                Annotated[PurePath, WithSuffix(".md", case_sensitive=True)]
-            ),  # pyright: ignore[reportCallIssue]
+            TypeAdapter(Annotated[FilePath, WithSuffix(".md", case_sensitive=True)]),
+            TypeAdapter(Annotated[Path, WithSuffix(".md", case_sensitive=True)]),
+            TypeAdapter(Annotated[PurePath, WithSuffix(".md", case_sensitive=True)]),
             TypeAdapter(
                 Annotated[
                     Union[PurePath, HttpUrl], WithSuffix(".md", case_sensitive=True)
                 ]
             ),
             TypeAdapter(
                 Annotated[
@@ -172,17 +166,15 @@
                 Annotated[DocumentationSource, WithSuffix(".md", case_sensitive=True)]
             ),
         ]
     ]
     + [
         (text_md_url, a)
         for a in [
-            TypeAdapter(
-                Annotated[HttpUrl, WithSuffix(".md", case_sensitive=True)]
-            ),  # pyright: ignore[reportCallIssue]
+            TypeAdapter(Annotated[HttpUrl, WithSuffix(".md", case_sensitive=True)]),
             TypeAdapter(
                 Annotated[
                     Union[PurePath, HttpUrl], WithSuffix(".md", case_sensitive=True)
                 ]
             ),
             TypeAdapter(
                 Annotated[
```

### Comparing `bioimageio.spec-0.5.1.post1/tests/test_internal/test_constants.py` & `bioimageio.spec-0.5.2/tests/test_internal/test_constants.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/tests/test_internal/test_file_source.py` & `bioimageio.spec-0.5.2/tests/test_internal/test_file_source.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/tests/test_internal/test_io.py` & `bioimageio.spec-0.5.2/tests/test_internal/test_io.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/tests/test_internal/test_license_id.py` & `bioimageio.spec-0.5.2/tests/test_internal/test_license_id.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/tests/test_internal/test_node.py` & `bioimageio.spec-0.5.2/tests/test_internal/test_node.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/tests/test_internal/test_types.py` & `bioimageio.spec-0.5.2/tests/test_internal/test_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,15 +151,15 @@
 )
 def test_datetime_more(value: str):
     from bioimageio.spec._internal.types import (
         _serialize_datetime_json,  # pyright: ignore[reportPrivateUsage]
     )
 
     root_adapter = TypeAdapter(Datetime)
-    datetime_adapter = TypeAdapter(  # pyright: ignore[reportCallIssue]
+    datetime_adapter = TypeAdapter(
         Annotated[
             datetime,
             PlainSerializer(_serialize_datetime_json, when_used="json-unless-none"),
         ]
     )
 
     expected = isoparse(value)
```

### Comparing `bioimageio.spec-0.5.1.post1/tests/test_internal/test_utils.py` & `bioimageio.spec-0.5.2/tests/test_internal/test_utils.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/tests/test_internal/test_validate.py` & `bioimageio.spec-0.5.2/tests/test_internal/test_validate.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/tests/test_internal/test_validated_string.py` & `bioimageio.spec-0.5.2/tests/test_internal/test_validated_string.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/tests/test_model/test_v0_4.py` & `bioimageio.spec-0.5.2/tests/test_model/test_v0_4.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/tests/test_model/test_v0_5.py` & `bioimageio.spec-0.5.2/tests/test_model/test_v0_5.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,14 +172,31 @@
         InputTensorDescr,
         kwargs,
         is_invalid=True,
         context=ValidationContext(perform_io_checks=False),
     )
 
 
+@pytest.mark.skip(
+    "possibly bug in pydantic? in some envs it passes, in ohters not"
+)  # TODO: fix
+def test_input_tensor_error_count(model_data: Dict[str, Any]):
+    """this test checks that the discrminated union for `InputAxis` does its
+    thing and we don't get errors for all options"""
+    from bioimageio.spec import build_description
+
+    model_data["inputs"][0]["axes"][0]["id"] = 42
+    invalid = build_description(
+        model_data, context=ValidationContext(perform_io_checks=False)
+    )
+    assert (
+        len(invalid.validation_summary.details[1].errors) == 1
+    ), invalid.validation_summary.details[1].errors
+
+
 @pytest.mark.parametrize(
     "kwargs",
     [{}, {"type": "batch"}],
 )
 def test_batch_axis(kwargs: Dict[str, Any]):
     check_node(
         BatchAxis,
```

### Comparing `bioimageio.spec-0.5.1.post1/tests/test_package.py` & `bioimageio.spec-0.5.2/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1.post1/tests/test_specific_reexports_generics.py` & `bioimageio.spec-0.5.2/tests/test_specific_reexports_generics.py`

 * *Files identical despite different names*

