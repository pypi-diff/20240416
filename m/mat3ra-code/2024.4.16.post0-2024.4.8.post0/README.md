# Comparing `tmp/mat3ra_code-2024.4.16.post0.tar.gz` & `tmp/mat3ra-code-2024.4.8.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mat3ra_code-2024.4.16.post0.tar", last modified: Tue Apr 16 21:16:04 2024, max compression
+gzip compressed data, was "mat3ra-code-2024.4.8.post0.tar", last modified: Mon Apr  8 02:12:44 2024, max compression
```

## Comparing `mat3ra_code-2024.4.16.post0.tar` & `mat3ra-code-2024.4.8.post0.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:16:04.374942 mat3ra_code-2024.4.16.post0/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/.babelrc
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/.eslintignore
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/.eslintrc.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:16:04.354942 mat3ra_code-2024.4.16.post0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:16:04.358942 mat3ra_code-2024.4.16.post0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/.github/workflows/cicd.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:16:04.358942 mat3ra_code-2024.4.16.post0/.husky/
--rwxr-xr-x   0 runner    (1001) docker     (127)       90 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/.husky/pre-commit
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/.mocharc.json
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/.nycrc
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/.prettierrc
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-16 21:16:04.374942 mat3ra_code-2024.4.16.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   350189 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/package.json
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 21:16:04.374942 mat3ra_code-2024.4.16.post0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:16:04.354942 mat3ra_code-2024.4.16.post0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:16:04.358942 mat3ra_code-2024.4.16.post0/src/js/
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/constants.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:16:04.358942 mat3ra_code-2024.4.16.post0/src/js/context/
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/context/index.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/context/json_schema_provider.ts
--rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/context/mixins.ts
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/context/pickers.js
--rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/context/provider.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/context/registry.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:16:04.362942 mat3ra_code-2024.4.16.post0/src/js/entity/
--rw-r--r--   0 runner    (1001) docker     (127)     7074 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/entity/in_memory.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/entity/index.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:16:04.362942 mat3ra_code-2024.4.16.post0/src/js/entity/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/entity/mixins/context.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/entity/mixins/context_runtime.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/entity/mixins/flowchart.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/entity/mixins/hash.ts
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/entity/mixins/props.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/entity/mixins/repetition.ts
--rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/entity/mixins/runtime_items.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/entity/other.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:16:04.362942 mat3ra_code-2024.4.16.post0/src/js/entity/set/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/entity/set/enums.ts
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/entity/set/factory.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/entity/set/mixins.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:16:04.362942 mat3ra_code-2024.4.16.post0/src/js/entity/set/ordered/
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/entity/set/ordered/mixins.ts
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/entity/set/ordered/utils.ts
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/entity/set/ordered.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/entity/set/selectors.ts
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/entity/set.ts
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/index.ts
--rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/math.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:16:04.366942 mat3ra_code-2024.4.16.post0/src/js/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/utils/array.js
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/utils/class.js
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/utils/clone.js
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/utils/codemirror.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/utils/file.js
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/utils/filter.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/utils/github.js
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/utils/graph.ts
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/utils/hash.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/utils/index.ts
--rw-r--r--   0 runner    (1001) docker     (127)     8775 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/utils/object.ts
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/utils/schemas.ts
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/utils/selector.js
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/utils/str.js
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/utils/tree.js
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/utils/url.js
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/utils/uuid.js
--rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/js/utils/yaml.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:16:04.366942 mat3ra_code-2024.4.16.post0/src/py/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:16:04.366942 mat3ra_code-2024.4.16.post0/src/py/mat3ra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/py/mat3ra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:16:04.366942 mat3ra_code-2024.4.16.post0/src/py/mat3ra/code/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/py/mat3ra/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/py/mat3ra/code/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/py/mat3ra/code/entity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:16:04.366942 mat3ra_code-2024.4.16.post0/src/py/mat3ra/code/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/src/py/mat3ra/code/mixins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:16:04.374942 mat3ra_code-2024.4.16.post0/src/py/mat3ra_code.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-16 21:16:04.000000 mat3ra_code-2024.4.16.post0/src/py/mat3ra_code.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-16 21:16:04.000000 mat3ra_code-2024.4.16.post0/src/py/mat3ra_code.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 21:16:04.000000 mat3ra_code-2024.4.16.post0/src/py/mat3ra_code.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-16 21:16:04.000000 mat3ra_code-2024.4.16.post0/src/py/mat3ra_code.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 21:16:04.000000 mat3ra_code-2024.4.16.post0/src/py/mat3ra_code.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:16:04.354942 mat3ra_code-2024.4.16.post0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:16:04.370942 mat3ra_code-2024.4.16.post0/tests/js/
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/context.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/enums.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:16:04.370942 mat3ra_code-2024.4.16.post0/tests/js/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:16:04.354942 mat3ra_code-2024.4.16.post0/tests/js/fixtures/json/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:16:04.370942 mat3ra_code-2024.4.16.post0/tests/js/fixtures/json/example/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/fixtures/json/example/1.json
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/fixtures/json/example/2.json
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/fixtures/json/example/3.json
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/fixtures/json/example/4.json
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/fixtures/json/example/5.json
--rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/fixtures/rjsf_schemas.js
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/fixtures/test_content.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/fixtures/yaml_combine_tag.yml
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/fixtures/yaml_concatString_tag.yml
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/fixtures/yaml_esse_tag.yml
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/fixtures/yaml_flatten_tag.yml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/fixtures/yaml_include_tag.yml
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/fixtures/yaml_listToString_tag.yml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/fixtures/yaml_parameter_ref.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/fixtures/yaml_parameter_tag.yml
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/fixtures/yaml_readFile_tag.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/in_memory.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/mixin.flowchart.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/provider.tests.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:16:04.374942 mat3ra_code-2024.4.16.post0/tests/js/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/utils/class.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/utils/file.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/utils/filter.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/utils/object.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/utils/schemas.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/utils/str.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/utils/tree.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/utils/utils.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/utils/yaml.combine.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/utils/yaml.concatString.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/utils/yaml.esse.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/utils/yaml.flatten.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/utils/yaml.include.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/utils/yaml.listToString.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/utils/yaml.parameter.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/utils/yaml.readFile.tests.ts
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/js/utils.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:16:04.354942 mat3ra_code-2024.4.16.post0/tests/py/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:16:04.374942 mat3ra_code-2024.4.16.post0/tests/py/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/py/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tests/py/unit/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tsconfig-transpile.json
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-16 21:15:48.000000 mat3ra_code-2024.4.16.post0/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.279558 mat3ra-code-2024.4.8.post0/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/.babelrc
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/.eslintignore
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/.eslintrc.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.251558 mat3ra-code-2024.4.8.post0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.259558 mat3ra-code-2024.4.8.post0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/.github/workflows/cicd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.259558 mat3ra-code-2024.4.8.post0/.husky/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       90 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/.husky/pre-commit
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/.mocharc.json
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/.nycrc
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/.prettierrc
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-08 02:12:44.279558 mat3ra-code-2024.4.8.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   350189 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 02:12:44.279558 mat3ra-code-2024.4.8.post0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.251558 mat3ra-code-2024.4.8.post0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.259558 mat3ra-code-2024.4.8.post0/src/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/constants.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.259558 mat3ra-code-2024.4.8.post0/src/js/context/
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/context/index.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/context/json_schema_provider.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/context/mixins.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/context/pickers.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/context/provider.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/context/registry.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.259558 mat3ra-code-2024.4.8.post0/src/js/entity/
+-rw-r--r--   0 runner    (1001) docker     (127)     7074 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/entity/in_memory.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/entity/index.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.263558 mat3ra-code-2024.4.8.post0/src/js/entity/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/entity/mixins/context.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/entity/mixins/context_runtime.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/entity/mixins/flowchart.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/entity/mixins/hash.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/entity/mixins/props.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/entity/mixins/repetition.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/entity/mixins/runtime_items.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/entity/other.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.263558 mat3ra-code-2024.4.8.post0/src/js/entity/set/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/entity/set/enums.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/entity/set/factory.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/entity/set/mixins.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.263558 mat3ra-code-2024.4.8.post0/src/js/entity/set/ordered/
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/entity/set/ordered/mixins.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/entity/set/ordered/utils.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/entity/set/ordered.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/entity/set/selectors.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/entity/set.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/index.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/math.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.267558 mat3ra-code-2024.4.8.post0/src/js/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/utils/array.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/utils/class.js
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/utils/clone.js
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/utils/codemirror.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/utils/file.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/utils/filter.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/utils/github.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/utils/graph.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/utils/hash.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/utils/index.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     8775 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/utils/object.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/utils/schemas.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/utils/selector.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/utils/str.js
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/utils/tree.js
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/utils/url.js
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/utils/uuid.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/js/utils/yaml.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.267558 mat3ra-code-2024.4.8.post0/src/py/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.267558 mat3ra-code-2024.4.8.post0/src/py/mat3ra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/py/mat3ra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.267558 mat3ra-code-2024.4.8.post0/src/py/mat3ra/code/
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/py/mat3ra/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/py/mat3ra/code/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/py/mat3ra/code/entity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.267558 mat3ra-code-2024.4.8.post0/src/py/mat3ra/code/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/src/py/mat3ra/code/mixins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.275558 mat3ra-code-2024.4.8.post0/src/py/mat3ra_code.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-08 02:12:44.000000 mat3ra-code-2024.4.8.post0/src/py/mat3ra_code.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-08 02:12:44.000000 mat3ra-code-2024.4.8.post0/src/py/mat3ra_code.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 02:12:44.000000 mat3ra-code-2024.4.8.post0/src/py/mat3ra_code.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-08 02:12:44.000000 mat3ra-code-2024.4.8.post0/src/py/mat3ra_code.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 02:12:44.000000 mat3ra-code-2024.4.8.post0/src/py/mat3ra_code.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.255558 mat3ra-code-2024.4.8.post0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.271558 mat3ra-code-2024.4.8.post0/tests/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/context.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/enums.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.271558 mat3ra-code-2024.4.8.post0/tests/js/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.255558 mat3ra-code-2024.4.8.post0/tests/js/fixtures/json/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.271558 mat3ra-code-2024.4.8.post0/tests/js/fixtures/json/example/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/fixtures/json/example/1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/fixtures/json/example/2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/fixtures/json/example/3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/fixtures/json/example/4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/fixtures/json/example/5.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/fixtures/rjsf_schemas.js
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/fixtures/test_content.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/fixtures/yaml_combine_tag.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/fixtures/yaml_concatString_tag.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/fixtures/yaml_esse_tag.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/fixtures/yaml_flatten_tag.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/fixtures/yaml_include_tag.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/fixtures/yaml_listToString_tag.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/fixtures/yaml_parameter_ref.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/fixtures/yaml_parameter_tag.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/fixtures/yaml_readFile_tag.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/in_memory.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/mixin.flowchart.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/provider.tests.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.275558 mat3ra-code-2024.4.8.post0/tests/js/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/utils/class.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/utils/file.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/utils/filter.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/utils/object.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/utils/schemas.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/utils/str.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/utils/tree.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/utils/utils.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/utils/yaml.combine.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/utils/yaml.concatString.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/utils/yaml.esse.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/utils/yaml.flatten.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/utils/yaml.include.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/utils/yaml.listToString.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/utils/yaml.parameter.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/utils/yaml.readFile.tests.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/js/utils.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.255558 mat3ra-code-2024.4.8.post0/tests/py/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:44.275558 mat3ra-code-2024.4.8.post0/tests/py/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/py/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tests/py/unit/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tsconfig-transpile.json
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-08 02:12:23.000000 mat3ra-code-2024.4.8.post0/tsconfig.json
```

### Comparing `mat3ra_code-2024.4.16.post0/.github/workflows/cicd.yml` & `mat3ra-code-2024.4.8.post0/.github/workflows/cicd.yml`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/.gitignore` & `mat3ra-code-2024.4.8.post0/.gitignore`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/LICENSE.md` & `mat3ra-code-2024.4.8.post0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/PKG-INFO` & `mat3ra-code-2024.4.8.post0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat3ra-code
-Version: 2024.4.16.post0
+Version: 2024.4.8.post0
 Summary: COre DEfinitions.
 Author-email: "Exabyte Inc." <info@mat3ra.com>
 License: # LICENSE
         
         Copyright 2022 Exabyte Inc.
         
         Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `mat3ra_code-2024.4.16.post0/README.md` & `mat3ra-code-2024.4.8.post0/README.md`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/package-lock.json` & `mat3ra-code-2024.4.8.post0/package-lock.json`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/package.json` & `mat3ra-code-2024.4.8.post0/package.json`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/pyproject.toml` & `mat3ra-code-2024.4.8.post0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/js/constants.js` & `mat3ra-code-2024.4.8.post0/src/js/constants.js`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/js/context/index.ts` & `mat3ra-code-2024.4.8.post0/src/js/context/index.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/js/context/json_schema_provider.ts` & `mat3ra-code-2024.4.8.post0/src/js/context/json_schema_provider.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/js/context/mixins.ts` & `mat3ra-code-2024.4.8.post0/src/js/context/mixins.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/js/context/provider.ts` & `mat3ra-code-2024.4.8.post0/src/js/context/provider.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/js/context/registry.js` & `mat3ra-code-2024.4.8.post0/src/js/context/registry.js`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/js/entity/in_memory.ts` & `mat3ra-code-2024.4.8.post0/src/js/entity/in_memory.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/js/entity/index.ts` & `mat3ra-code-2024.4.8.post0/src/js/entity/index.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/js/entity/mixins/context.ts` & `mat3ra-code-2024.4.8.post0/src/js/entity/mixins/context.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/js/entity/mixins/context_runtime.ts` & `mat3ra-code-2024.4.8.post0/src/js/entity/mixins/context_runtime.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/js/entity/mixins/flowchart.ts` & `mat3ra-code-2024.4.8.post0/src/js/entity/mixins/flowchart.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/js/entity/mixins/hash.ts` & `mat3ra-code-2024.4.8.post0/src/js/entity/mixins/hash.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/js/entity/mixins/props.ts` & `mat3ra-code-2024.4.8.post0/src/js/entity/mixins/props.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/js/entity/mixins/repetition.ts` & `mat3ra-code-2024.4.8.post0/src/js/entity/mixins/repetition.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/js/entity/mixins/runtime_items.ts` & `mat3ra-code-2024.4.8.post0/src/js/entity/mixins/runtime_items.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/js/entity/other.ts` & `mat3ra-code-2024.4.8.post0/src/js/entity/other.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/js/entity/set/factory.ts` & `mat3ra-code-2024.4.8.post0/src/js/entity/set/factory.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/js/entity/set/mixins.ts` & `mat3ra-code-2024.4.8.post0/src/js/entity/set/mixins.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/js/entity/set/ordered/mixins.ts` & `mat3ra-code-2024.4.8.post0/src/js/entity/set/ordered/mixins.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/js/entity/set/ordered/utils.ts` & `mat3ra-code-2024.4.8.post0/src/js/entity/set/ordered/utils.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/js/entity/set/selectors.ts` & `mat3ra-code-2024.4.8.post0/src/js/entity/set/selectors.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/js/entity/set.ts` & `mat3ra-code-2024.4.8.post0/src/js/entity/set.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/js/math.ts` & `mat3ra-code-2024.4.8.post0/src/js/math.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/js/utils/array.js` & `mat3ra-code-2024.4.8.post0/src/js/utils/array.js`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/js/utils/class.js` & `mat3ra-code-2024.4.8.post0/src/js/utils/class.js`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/js/utils/file.js` & `mat3ra-code-2024.4.8.post0/src/js/utils/file.js`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/js/utils/filter.ts` & `mat3ra-code-2024.4.8.post0/src/js/utils/filter.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/js/utils/github.js` & `mat3ra-code-2024.4.8.post0/src/js/utils/github.js`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/js/utils/graph.ts` & `mat3ra-code-2024.4.8.post0/src/js/utils/graph.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/js/utils/hash.ts` & `mat3ra-code-2024.4.8.post0/src/js/utils/hash.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/js/utils/index.ts` & `mat3ra-code-2024.4.8.post0/src/js/utils/index.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/js/utils/object.ts` & `mat3ra-code-2024.4.8.post0/src/js/utils/object.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/js/utils/schemas.ts` & `mat3ra-code-2024.4.8.post0/src/js/utils/schemas.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/js/utils/selector.js` & `mat3ra-code-2024.4.8.post0/src/js/utils/selector.js`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/js/utils/str.js` & `mat3ra-code-2024.4.8.post0/src/js/utils/str.js`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/js/utils/tree.js` & `mat3ra-code-2024.4.8.post0/src/js/utils/tree.js`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/js/utils/yaml.ts` & `mat3ra-code-2024.4.8.post0/src/js/utils/yaml.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/py/mat3ra/code/__init__.py` & `mat3ra-code-2024.4.8.post0/src/py/mat3ra/code/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict
+from typing import Any, Dict, Optional
 
 from mat3ra.utils import object as object_utils
 
 
 class BaseUnderscoreJsonPropsHandler(object):
     def __init__(self, config: Dict[str, Any] = {}) -> None:
         self._json = object_utils.clone_deep(config)
@@ -22,11 +22,11 @@
 
     def set_prop(self, name: str, value: Any) -> None:
         object_utils.set(self._json, name, value)
 
     def unset_prop(self, name: str) -> None:
         del self._json[name]
 
-    def set_props(self, json: Dict[str, Any] = {}) -> Any:
+    def set_props(self, json: Dict[str, Any] = {}) -> "BaseUnderscoreJsonPropsHandler":
         for key, value in json.items():
             self.set_prop(key, value)
         return self
```

### Comparing `mat3ra_code-2024.4.16.post0/src/py/mat3ra/code/entity.py` & `mat3ra-code-2024.4.8.post0/src/py/mat3ra/code/entity.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,20 +43,15 @@
     def create(cls, config: Dict[str, Any]) -> Any:
         return cls(config)
 
     def to_json(self, exclude: List[str] = []) -> Dict[str, Any]:
         return self.clean(object_utils.clone_deep(object_utils.omit(self._json, exclude)))
 
     def clone(self, extra_context: Dict[str, Any] = {}) -> Any:
-        config = self.to_json()
-        config.update(extra_context)
-        # To avoid:
-        #   Argument 1 to "__init__" of "BaseUnderscoreJsonPropsHandler" has incompatible type "Dict[str, Any]";
-        #   expected "BaseUnderscoreJsonPropsHandler"
-        return self.__class__.__init__(config)  # type: ignore[arg-type]
+        return self.__class__.__init__({**self.to_json(), **extra_context})
 
     @staticmethod
     def validate_data(data: Dict[str, Any], clean: bool = False):
         if clean:
             print("Error: clean is not supported for InMemoryEntity.validateData")
         if InMemoryEntity.jsonSchema:
             jsonschema.validate(data, InMemoryEntity.jsonSchema)
```

### Comparing `mat3ra_code-2024.4.16.post0/src/py/mat3ra/code/mixins/__init__.py` & `mat3ra-code-2024.4.8.post0/src/py/mat3ra/code/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/src/py/mat3ra_code.egg-info/PKG-INFO` & `mat3ra-code-2024.4.8.post0/src/py/mat3ra_code.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat3ra-code
-Version: 2024.4.16.post0
+Version: 2024.4.8.post0
 Summary: COre DEfinitions.
 Author-email: "Exabyte Inc." <info@mat3ra.com>
 License: # LICENSE
         
         Copyright 2022 Exabyte Inc.
         
         Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `mat3ra_code-2024.4.16.post0/src/py/mat3ra_code.egg-info/SOURCES.txt` & `mat3ra-code-2024.4.8.post0/src/py/mat3ra_code.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/tests/js/context.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/context.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/tests/js/enums.ts` & `mat3ra-code-2024.4.8.post0/tests/js/enums.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/tests/js/fixtures/json/example/5.json` & `mat3ra-code-2024.4.8.post0/tests/js/fixtures/json/example/5.json`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/tests/js/fixtures/rjsf_schemas.js` & `mat3ra-code-2024.4.8.post0/tests/js/fixtures/rjsf_schemas.js`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/tests/js/fixtures/yaml_combine_tag.yml` & `mat3ra-code-2024.4.8.post0/tests/js/fixtures/yaml_combine_tag.yml`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/tests/js/fixtures/yaml_parameter_tag.yml` & `mat3ra-code-2024.4.8.post0/tests/js/fixtures/yaml_parameter_tag.yml`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/tests/js/in_memory.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/in_memory.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/tests/js/mixin.flowchart.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/mixin.flowchart.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/tests/js/provider.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/provider.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/tests/js/utils/class.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/utils/class.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/tests/js/utils/filter.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/utils/filter.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/tests/js/utils/object.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/utils/object.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/tests/js/utils/schemas.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/utils/schemas.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/tests/js/utils/str.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/utils/str.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/tests/js/utils/tree.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/utils/tree.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/tests/js/utils/utils.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/utils/utils.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/tests/js/utils/yaml.combine.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/utils/yaml.combine.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/tests/js/utils/yaml.concatString.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/utils/yaml.concatString.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/tests/js/utils/yaml.esse.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/utils/yaml.esse.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/tests/js/utils/yaml.flatten.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/utils/yaml.flatten.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/tests/js/utils/yaml.include.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/utils/yaml.include.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/tests/js/utils/yaml.listToString.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/utils/yaml.listToString.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/tests/js/utils/yaml.parameter.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/utils/yaml.parameter.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/tests/js/utils/yaml.readFile.tests.ts` & `mat3ra-code-2024.4.8.post0/tests/js/utils/yaml.readFile.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_code-2024.4.16.post0/tests/py/unit/test_entity.py` & `mat3ra-code-2024.4.8.post0/tests/py/unit/test_entity.py`

 * *Files identical despite different names*

