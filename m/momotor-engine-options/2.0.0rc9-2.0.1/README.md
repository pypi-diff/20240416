# Comparing `tmp/momotor-engine-options-2.0.0rc9.tar.gz` & `tmp/momotor_engine_options-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "momotor-engine-options-2.0.0rc9.tar", last modified: Tue Jan 16 09:23:36 2024, max compression
+gzip compressed data, was "momotor_engine_options-2.0.1.tar", last modified: Tue Apr 16 07:31:38 2024, max compression
```

## Comparing `momotor-engine-options-2.0.0rc9.tar` & `momotor_engine_options-2.0.1.tar`

### file list

```diff
@@ -1,128 +1,127 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/
--rw-rw-rw-   0 root         (0) root         (0)     1215 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     3251 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/.gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/.idea/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/.idea/inspectionProfiles/
--rw-rw-rw-   0 root         (0) root         (0)      779 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/.idea/inspectionProfiles/Project_Default.xml
--rw-rw-rw-   0 root         (0) root         (0)      174 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/.idea/inspectionProfiles/profiles_settings.xml
--rw-rw-rw-   0 root         (0) root         (0)      296 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/.idea/modules.xml
--rw-rw-rw-   0 root         (0) root         (0)      566 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/.idea/momotor.lib.engine-options.iml
--rw-rw-rw-   0 root         (0) root         (0)      238 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/.idea/workspace.xml
--rw-rw-rw-   0 root         (0) root         (0)    18559 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     2483 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      778 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/docs/
--rw-rw-rw-   0 root         (0) root         (0)      638 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      764 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/docs/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/docs/source/_static/
--rw-rw-rw-   0 root         (0) root         (0)     6988 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/source/_static/logo-text-negative.png
--rw-rw-rw-   0 root         (0) root         (0)     6887 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/source/_static/logo-text.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/docs/source/_templates/
--rw-rw-rw-   0 root         (0) root         (0)      672 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/source/_templates/projectlinks.html
--rw-rw-rw-   0 root         (0) root         (0)     4895 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/source/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      146 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/source/dependencies.rst
--rw-rw-rw-   0 root         (0) root         (0)      161 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/source/exceptions.rst
--rw-rw-rw-   0 root         (0) root         (0)      583 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/source/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      162 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/source/option.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/docs/source/options/
--rw-rw-rw-   0 root         (0) root         (0)      516 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/source/options/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      411 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/source/options/scheduler.rst
--rw-rw-rw-   0 root         (0) root         (0)      895 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/source/options/tools.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/docs/source/parser/
--rw-rw-rw-   0 root         (0) root         (0)      654 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/source/parser/index.rst
--rw-rw-rw-   0 root         (0) root         (0)    30840 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/source/parser/syntax.rst
--rw-rw-rw-   0 root         (0) root         (0)      134 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/source/providers.rst
--rw-rw-rw-   0 root         (0) root         (0)     6989 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/source/registry.rst
--rw-rw-rw-   0 root         (0) root         (0)    11586 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/source/result_query.rst
--rw-rw-rw-   0 root         (0) root         (0)      126 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/source/task_id.rst
--rw-rw-rw-   0 root         (0) root         (0)      618 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/source/utilities.rst
--rw-rw-rw-   0 root         (0) root         (0)      423 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/publish-docs.sh
--rw-rw-rw-   0 root         (0) root         (0)     2470 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      411 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/semver.sh
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/src/momotor/
--rw-rw-rw-   0 root         (0) root         (0)       65 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/
--rw-rw-rw-   0 root         (0) root         (0)      120 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7428 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/convert.py
--rw-rw-rw-   0 root         (0) root         (0)     8331 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/dependencies.py
--rw-rw-rw-   0 root         (0) root         (0)     1181 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/doc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/domain/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/domain/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/domain/scheduler/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/domain/scheduler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/domain/scheduler/_domain.py
--rw-rw-rw-   0 root         (0) root         (0)    11572 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/domain/scheduler/preflight.py
--rw-rw-rw-   0 root         (0) root         (0)     8274 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/domain/scheduler/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     4367 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/domain/scheduler/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/domain/tools/
--rw-rw-rw-   0 root         (0) root         (0)     6185 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/domain/tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       17 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/domain/tools/_domain.py
--rw-rw-rw-   0 root         (0) root         (0)      630 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/exception.py
--rw-rw-rw-   0 root         (0) root         (0)     1696 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/filter_files.py
--rw-rw-rw-   0 root         (0) root         (0)    13301 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/option.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/parser/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/parser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1965 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/parser/consts.py
--rw-rw-rw-   0 root         (0) root         (0)     3560 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/parser/keyvalue.py
--rw-rw-rw-   0 root         (0) root         (0)     4024 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/parser/modifier.py
--rw-rw-rw-   0 root         (0) root         (0)     2071 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/parser/placeholders.py
--rw-rw-rw-   0 root         (0) root         (0)    24823 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/parser/reference.py
--rw-rw-rw-   0 root         (0) root         (0)     8308 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/parser/selector.py
--rw-rw-rw-   0 root         (0) root         (0)     1710 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/parser/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     1055 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/providers.py
--rw-rw-rw-   0 root         (0) root         (0)     6463 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/result_query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/sphinx/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/sphinx/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2555 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/sphinx/fixextref.py
--rw-rw-rw-   0 root         (0) root         (0)    15739 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/sphinx/option.py
--rw-rw-rw-   0 root         (0) root         (0)     1434 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/split.py
--rw-rw-rw-   0 root         (0) root         (0)     9149 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/task_id.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/tools/
--rw-rw-rw-   0 root         (0) root         (0)      919 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6210 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/tools/registry.py
--rw-rw-rw-   0 root         (0) root         (0)    12393 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/tools/tool.py
--rw-rw-rw-   0 root         (0) root         (0)      473 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/tools/types.py
--rw-rw-rw-   0 root         (0) root         (0)     6068 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/tools/version.py
--rw-rw-rw-   0 root         (0) root         (0)      564 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/types.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2024-01-16 09:23:31.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/src/momotor_engine_options.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2483 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/src/momotor_engine_options.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3338 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/src/momotor_engine_options.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/src/momotor_engine_options.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      267 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/src/momotor_engine_options.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/src/momotor_engine_options.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/tests/
--rw-rw-rw-   0 root         (0) root         (0)     7508 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/test_option_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     4365 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/test_parser_modifier.py
--rw-rw-rw-   0 root         (0) root         (0)     6167 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/test_parser_placeholders.py
--rw-rw-rw-   0 root         (0) root         (0)     9529 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/test_parser_reference.py
--rw-rw-rw-   0 root         (0) root         (0)     8543 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/test_parser_selector.py
--rw-rw-rw-   0 root         (0) root         (0)     8110 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/test_utils_dependencies.py
--rw-rw-rw-   0 root         (0) root         (0)     9006 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/test_utils_tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/tests/tools/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/toolregistry.d/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/toolregistry.d/nodefault/
--rw-rw-rw-   0 root         (0) root         (0)       20 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/toolregistry.d/nodefault/1
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/toolregistry.d/nodefault/2.1
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/toolregistry.d/nodefault/named
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/toolregistry.d/tool/
--rw-rw-rw-   0 root         (0) root         (0)       20 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/toolregistry.d/tool/1
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/toolregistry.d/tool/2.1
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/toolregistry.d/tool/2.2
--rw-rw-rw-   0 root         (0) root         (0)       26 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/toolregistry.d/tool/_default
--rw-rw-rw-   0 root         (0) root         (0)       47 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/toolregistry.d/tool/envs
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/toolregistry.d/variant/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/toolregistry.d/variant/2.0/
--rw-rw-rw-   0 root         (0) root         (0)       32 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/toolregistry.d/variant/2.0/a
--rw-rw-rw-   0 root         (0) root         (0)       32 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/toolregistry.d/variant/2.0/b
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/toolregistry.d/variant/2.1/
--rw-rw-rw-   0 root         (0) root         (0)       32 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/toolregistry.d/variant/2.1/b
--rw-rw-rw-   0 root         (0) root         (0)       32 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/toolregistry.d/variant/2.1/c
--rw-rw-rw-   0 root         (0) root         (0)     3834 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/tools/test_tool_registry.py
--rw-rw-rw-   0 root         (0) root         (0)     2995 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/tools/test_tools_match.py
--rw-rw-rw-   0 root         (0) root         (0)     3221 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/tools/test_tools_options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1215 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     3220 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/.gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/.idea/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/.idea/inspectionProfiles/
+-rw-rw-rw-   0 root         (0) root         (0)      779 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/.idea/inspectionProfiles/Project_Default.xml
+-rw-rw-rw-   0 root         (0) root         (0)      174 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-rw-   0 root         (0) root         (0)      296 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/.idea/modules.xml
+-rw-rw-rw-   0 root         (0) root         (0)      566 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/.idea/momotor.lib.engine-options.iml
+-rw-rw-rw-   0 root         (0) root         (0)      238 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/.idea/workspace.xml
+-rw-rw-rw-   0 root         (0) root         (0)    17342 2024-04-16 07:31:33.000000 momotor_engine_options-2.0.1/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     2658 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      778 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      638 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      764 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/docs/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/docs/source/_static/
+-rw-rw-rw-   0 root         (0) root         (0)     6988 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/source/_static/logo-text-negative.png
+-rw-rw-rw-   0 root         (0) root         (0)     6887 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/source/_static/logo-text.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/docs/source/_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      672 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/source/_templates/projectlinks.html
+-rw-rw-rw-   0 root         (0) root         (0)     4647 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      146 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/source/dependencies.rst
+-rw-rw-rw-   0 root         (0) root         (0)      161 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/source/exceptions.rst
+-rw-rw-rw-   0 root         (0) root         (0)      583 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/source/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/source/option.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/docs/source/options/
+-rw-rw-rw-   0 root         (0) root         (0)      516 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/source/options/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      411 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/source/options/scheduler.rst
+-rw-rw-rw-   0 root         (0) root         (0)      895 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/source/options/tools.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/docs/source/parser/
+-rw-rw-rw-   0 root         (0) root         (0)      654 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/source/parser/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)    31565 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/source/parser/syntax.rst
+-rw-rw-rw-   0 root         (0) root         (0)      134 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/source/providers.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6992 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/source/registry.rst
+-rw-rw-rw-   0 root         (0) root         (0)    11618 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/source/result_query.rst
+-rw-rw-rw-   0 root         (0) root         (0)      126 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/source/task_id.rst
+-rw-rw-rw-   0 root         (0) root         (0)      618 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/docs/source/utilities.rst
+-rw-rw-rw-   0 root         (0) root         (0)      436 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/publish-docs.sh
+-rw-rw-rw-   0 root         (0) root         (0)     2673 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      413 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/semver.sh
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/src/momotor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/src/momotor/options/
+-rw-rw-rw-   0 root         (0) root         (0)      120 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7428 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/convert.py
+-rw-rw-rw-   0 root         (0) root         (0)     8438 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/dependencies.py
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/doc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/src/momotor/options/domain/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/domain/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/src/momotor/options/domain/scheduler/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/domain/scheduler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/domain/scheduler/_domain.py
+-rw-rw-rw-   0 root         (0) root         (0)    11580 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/domain/scheduler/preflight.py
+-rw-rw-rw-   0 root         (0) root         (0)     8274 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/domain/scheduler/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     4367 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/domain/scheduler/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/src/momotor/options/domain/tools/
+-rw-rw-rw-   0 root         (0) root         (0)     6226 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/domain/tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/domain/tools/_domain.py
+-rw-rw-rw-   0 root         (0) root         (0)      630 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/exception.py
+-rw-rw-rw-   0 root         (0) root         (0)     1723 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/filter_files.py
+-rw-rw-rw-   0 root         (0) root         (0)    13396 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/option.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/src/momotor/options/parser/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/parser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1996 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/parser/consts.py
+-rw-rw-rw-   0 root         (0) root         (0)     3581 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/parser/keyvalue.py
+-rw-rw-rw-   0 root         (0) root         (0)     4151 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/parser/modifier.py
+-rw-rw-rw-   0 root         (0) root         (0)     2103 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/parser/placeholders.py
+-rw-rw-rw-   0 root         (0) root         (0)    24967 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/parser/reference.py
+-rw-rw-rw-   0 root         (0) root         (0)     8335 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/parser/selector.py
+-rw-rw-rw-   0 root         (0) root         (0)     1710 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/parser/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1055 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/providers.py
+-rw-rw-rw-   0 root         (0) root         (0)     6490 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/result_query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/src/momotor/options/sphinx/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/sphinx/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2555 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/sphinx/fixextref.py
+-rw-rw-rw-   0 root         (0) root         (0)    16823 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/sphinx/option.py
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/split.py
+-rw-rw-rw-   0 root         (0) root         (0)     9202 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/task_id.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/src/momotor/options/tools/
+-rw-rw-rw-   0 root         (0) root         (0)      919 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6312 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/tools/registry.py
+-rw-rw-rw-   0 root         (0) root         (0)    12546 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/tools/tool.py
+-rw-rw-rw-   0 root         (0) root         (0)      507 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/tools/types.py
+-rw-rw-rw-   0 root         (0) root         (0)     6103 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/tools/version.py
+-rw-rw-rw-   0 root         (0) root         (0)      776 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/src/momotor/options/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/src/momotor_engine_options.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2658 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/src/momotor_engine_options.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3296 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/src/momotor_engine_options.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/src/momotor_engine_options.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      360 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/src/momotor_engine_options.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/src/momotor_engine_options.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     7508 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/test_option_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     4365 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/test_parser_modifier.py
+-rw-rw-rw-   0 root         (0) root         (0)     6167 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/test_parser_placeholders.py
+-rw-rw-rw-   0 root         (0) root         (0)     9529 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/test_parser_reference.py
+-rw-rw-rw-   0 root         (0) root         (0)     8543 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/test_parser_selector.py
+-rw-rw-rw-   0 root         (0) root         (0)     8110 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/test_utils_dependencies.py
+-rw-rw-rw-   0 root         (0) root         (0)     9006 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/test_utils_tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/tests/tools/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/tests/tools/files/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/tests/tools/files/toolregistry.d/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/tests/tools/files/toolregistry.d/nodefault/
+-rw-rw-rw-   0 root         (0) root         (0)       20 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/tools/files/toolregistry.d/nodefault/1
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/tools/files/toolregistry.d/nodefault/2.1
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/tools/files/toolregistry.d/nodefault/named
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/tests/tools/files/toolregistry.d/tool/
+-rw-rw-rw-   0 root         (0) root         (0)       20 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/tools/files/toolregistry.d/tool/1
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/tools/files/toolregistry.d/tool/2.1
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/tools/files/toolregistry.d/tool/2.2
+-rw-rw-rw-   0 root         (0) root         (0)       26 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/tools/files/toolregistry.d/tool/_default
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/tools/files/toolregistry.d/tool/envs
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/tests/tools/files/toolregistry.d/variant/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/tests/tools/files/toolregistry.d/variant/2.0/
+-rw-rw-rw-   0 root         (0) root         (0)       32 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/tools/files/toolregistry.d/variant/2.0/a
+-rw-rw-rw-   0 root         (0) root         (0)       32 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/tools/files/toolregistry.d/variant/2.0/b
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:31:38.000000 momotor_engine_options-2.0.1/tests/tools/files/toolregistry.d/variant/2.1/
+-rw-rw-rw-   0 root         (0) root         (0)       32 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/tools/files/toolregistry.d/variant/2.1/b
+-rw-rw-rw-   0 root         (0) root         (0)       32 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/tools/files/toolregistry.d/variant/2.1/c
+-rw-rw-rw-   0 root         (0) root         (0)     3834 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/tools/test_tool_registry.py
+-rw-rw-rw-   0 root         (0) root         (0)     2995 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/tools/test_tools_match.py
+-rw-rw-rw-   0 root         (0) root         (0)     3221 2024-04-16 07:31:02.000000 momotor_engine_options-2.0.1/tests/tools/test_tools_options.py
+-rw-rw-rw-   0 root         (0) root         (0)       37 2024-04-16 07:31:33.000000 momotor_engine_options-2.0.1/version.toml
```

### Comparing `momotor-engine-options-2.0.0rc9/.gitignore` & `momotor_engine_options-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc9/.idea/inspectionProfiles/Project_Default.xml` & `momotor_engine_options-2.0.1/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc9/.idea/momotor.lib.engine-options.iml` & `momotor_engine_options-2.0.1/.idea/momotor.lib.engine-options.iml`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc9/CHANGELOG.md` & `momotor_engine_options-2.0.1/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,178 +1,389 @@
-# Changelog
+# CHANGELOG
+
+
+
+## v2.0.1 (2024-04-16)
+
+### Fix
+
+* fix: update dependencies ([`1b4261a`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/1b4261a04486ff6174ae9cd1b7f3109b4f2684ed))
+
+
+## v2.0.0 (2024-04-15)
+
+
+## v2.0.0-rc.11 (2024-03-19)
+
+### Breaking
+
+* feat: convert to PEP420 namespace packages
+
+requires all other momotor.* packages to be PEP420 too
+
+BREAKING CHANGE: convert to PEP420 namespace packages ([`1b01285`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/1b01285620e39f7882e5a68590afdc5e2ee2e1b5))
+
+### Refactor
+
+* refactor: replace all deprecated uses from typing (PEP-0585) ([`00021e8`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/00021e8ea1111d2112e611bd93975082678997d1))
+
+
+## v2.0.0-rc.10 (2024-03-04)
+
+### Feature
+
+* feat: extend `document_option_definition` to document step options ([`83bbd22`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/83bbd22735b19f60c6ee7d2165dd0bc1e3f86876))
+
+### Refactor
+
+* refactor: update type hints for Python 3.9 ([`9705bb8`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/9705bb832c19673b6fd8f0016ca0fc342bced1cf))
+
+### Unknown
+
+* doc: make production lists consistent ([`cdb8721`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/cdb87219a0ad6f965bd2f9e4690f5068d54d7c56))
+
+* doc: correct reference syntax documentation ([`e26f1d7`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/e26f1d745bceae8ddf411c14d269008b4ad3bd3e))
+
+* doc: correct reference syntax documentation ([`f4f4fe8`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/f4f4fe84a09a035ed8cdbf45ed08ecc27b3bbded))
+
+* doc: documentation update/clarifications ([`c61e8fc`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/c61e8fc30cdc40c5821cd152e009ab8285b521d0))
+
+* doc: several documentation fixes/clarifications ([`048016d`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/048016d44a3721b58cd9bf5114acdee64ee72beb))
+
+
+## v2.0.0-rc.9 (2024-01-16)
+
+### Breaking
+
+* feat: add Sphinx extension to handle external references to local package
+
+BREAKING CHANGE: moved `momotor.options.sphinx_ext` to `momotor.options.sphinx.option` ([`297382e`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/297382e142841a1211c2452261e12fdbcd1e22c2))
+
+* feat: remove deprecated interface of get_scheduler_tools_option()
+
+BREAKING CHANGE: deprecated interface of get_scheduler_tools_option() removed ([`130078d`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/130078d9c1d6d97397918565f71e3a7bbb1b41df))
+
+### Fix
+
+* fix: docutils is an optional dependency ([`1942882`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/1942882b2762b9cb14c78ff28e29e94c0b37093e))
+
+* fix: allow comparing of OptionNameDomain with other types ([`9cb473b`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/9cb473b9841614fe4a64f3dca9ac8629e706cadc))
+
+
+## v2.0.0-rc.8 (2024-01-12)
+
+### Feature
+
+* feat: add `annotate_docstring` ([`3033245`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/3033245069fe1ef9b56ffe67d14bfa62fdb2a52d))
+
+* feat: make it possible to xref a local option in the same checklet ([`a3ee72e`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/a3ee72e60c639713a07ac3560f56e5e9d95e50d8))
+
+### Fix
+
+* fix: always include domain in option name ids ([`71fdf62`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/71fdf62552c86f6886875514856f2e6c3aaf2b4d))
+
+* fix: correct toc entries ([`0ef4f2f`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/0ef4f2fa049d4e60f5f46a4ad6281988cff41bf2))
+
+* fix: change rendering of option attributes ([`a301d2d`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/a301d2d44ba9fd7004b6a24630c41ea7241a1a98))
+
+### Refactor
+
+* refactor: remove __all__ from __init__ ([`d55e4e4`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/d55e4e49c6b46d35e5540e7fca6ccf839705fb6c))
+
+### Unknown
+
+* doc: update docs ([`cdc7a36`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/cdc7a361d86e9d96b4a12842363175f6fcda5bb3))
+
+* doc: update conf.py ([`6e2a503`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/6e2a503ea5b50dbbf1fabd7439ca278784cbec1a))
+
+
+## v2.0.0-rc.7 (2024-01-09)
+
+
+## v2.0.0-rc.6 (2024-01-09)
+
+### Feature
+
+* feat: extract and document task id placeholder replacement into a separate function that can be used by checklet base ([`ad6a189`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/ad6a189f2b4b5dbbd472c11d5b010828d52d229c))
+
+* feat: add &#39;canonical&#39; option location link ([`f35bbf4`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/f35bbf4a0e8e9fc5d171e0044448ce0dae0773cf))
+
+### Fix
+
+* fix: correct xref anchors ([`e22d78c`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/e22d78cb5cccc2d876680b1e2ea9418272f3c5a6))
+
+* fix: iterate over all references ([`156cf7d`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/156cf7d571c0f87741bd644b2a8d06164d53193d))
+
+### Unknown
+
+* doc: small doc update ([`36a526d`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/36a526da74d136d5054964c754ab7686e559c3a1))
+
+* doc: use full path to reference Checklet options ([`5b1d1f1`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/5b1d1f1ecc705949ce1927031fe9840131567540))
+
+* doc: update intersphinx links for momotor.org docs ([`590d9e8`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/590d9e87cba36e75c13272b1cf2a625ce6e89204))
+
+
+## v1.2.0 (2023-10-26)
+
+### Chore
+
+* chore: show exact reference used in exception message ([`177fed1`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/177fed1379073bab8738a9b3785d1d0be7966ef0))
+
+### Feature
+
+* feat: change `get_scheduler_tools_option` to include results bundle in option resolution, so references to step results can be used ([`39e2183`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/39e218353d7eea2297b992e273bdc4550b3ba14b))
 
-<!--next-version-placeholder-->
 
 ## v1.1.1 (2023-08-29)
 
 ### Fix
 
-* Regression: preflight option selector placeholders are not expanded ([`bdfa8c0`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/bdfa8c09ef7544342e4aaa451ce2bed7a834a207))
+* fix: regression: preflight option selector placeholders are not expanded ([`bdfa8c0`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/bdfa8c09ef7544342e4aaa451ce2bed7a834a207))
+
+### Unknown
+
+* 1.1.1
+
+&#39;chore: bump version number&#39; ([`d37b901`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/d37b9011fe384c6dd84b7848e12477504b662f1e))
+
+* Merge remote-tracking branch &#39;origin/master&#39; ([`5e9d94f`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/5e9d94f6740b22274b0abac32ef031407cd38309))
+
 
 ## v1.1.0 (2023-08-29)
 
 ### Feature
 
-* Add json style preflight status ([`a346c6d`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/a346c6d09905b92f61cbaaae39795e1d2aaddd43))
+* feat: add json style preflight status ([`a346c6d`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/a346c6d09905b92f61cbaaae39795e1d2aaddd43))
 
 ### Fix
 
-* Emulate LabelOptionMixin's handling of the label option when preflight causes step to not execute ([`6383900`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/63839005e2e5ea4d401330fbc25c4e3e28ff94e9))
+* fix: emulate LabelOptionMixin&#39;s handling of the label option when preflight causes step to not execute ([`6383900`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/63839005e2e5ea4d401330fbc25c4e3e28ff94e9))
+
+### Test
+
+* test: update to latest Pytest ([`2b2bb42`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/2b2bb425e0af16a6151d816933bcb678e010f1a7))
+
+### Unknown
+
+* 1.1.0
+
+&#39;chore: bump version number&#39; ([`7608914`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/7608914796a3de95da1b924724424e0ac14a4f84))
+
 
 ## v1.0.0 (2023-07-06)
 
+### Breaking
+
+* chore: update supported Python versions
+
+BREAKING CHANGE: Dropped Python 3.7 support ([`e1a3d05`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/e1a3d05abcfbaaec61b24ad21e94e599e1e869c3))
+
 ### Feature
 
-* Support sub versions (dashed suffixes) in tool versions, to support Anaconda 2023.03-1 ([`aee2c3f`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/aee2c3f1d266b78deb2c2a8bb20c756cb382d361))
+* feat: support sub versions (dashed suffixes) in tool versions, to support Anaconda 2023.03-1 ([`aee2c3f`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/aee2c3f1d266b78deb2c2a8bb20c756cb382d361))
 
-### Breaking
+### Unknown
+
+* 1.0.0
+
+&#39;chore: bump version number&#39; ([`ac3dbca`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/ac3dbcacbcccf1277f6df7701ff7a8121151f3d3))
+
+* doc: fix typo ([`dc46cea`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/dc46cea160e2b667bbfd991a709e5c9b3bda0e77))
 
-* Dropped Python 3.7 support ([`e1a3d05`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/e1a3d05abcfbaaec61b24ad21e94e599e1e869c3))
 
 ## v0.10.1 (2023-06-19)
 
 ### Fix
 
-* Some error messages were incomplete/cryptic ([`3b37a8c`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/3b37a8c1a2998e68b0661ff3999d4ab41a063571))
+* fix: some error messages were incomplete/cryptic ([`3b37a8c`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/3b37a8c1a2998e68b0661ff3999d4ab41a063571))
+
+### Unknown
+
+* 0.10.1
+
+&#39;chore: bump version number&#39; ([`20fe626`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/20fe6260d57f06d0ddecaae8eb36daa893b6258d))
+
+* doc: fix layout issues in doctests ([`51ab28c`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/51ab28c36ce504f074de295d785d11087699acb9))
+
 
 ## v0.10.0 (2022-11-15)
+
 ### Feature
-* Add 'pass-hidden' and 'fail-hidden' preflight actions ([`c749a05`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/c749a0560083ee6395ccdb829714626ff1f67796))
+
+* feat: add &#39;pass-hidden&#39; and &#39;fail-hidden&#39; preflight actions ([`c749a05`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/c749a0560083ee6395ccdb829714626ff1f67796))
+
+### Unknown
+
+* 0.10.0
+
+&#39;chore: bump version number&#39; ([`328d6ed`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/328d6edde51b6899a30837f8686d8d97193de077))
+
 
 ## v0.9.1 (2022-10-27)
+
 ### Fix
-* Strip leading and trailing whitespace from selectors and references ([`929d233`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/929d23349700132234848921ed19de1f16628374))
+
+* fix: strip leading and trailing whitespace from selectors and references ([`929d233`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/929d23349700132234848921ed19de1f16628374))
+
+### Test
+
+* test: update doctest ([`271174c`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/271174c31817d30434bc6a1e83e01efa45f99e27))
+
+### Unknown
+
+* 0.9.1
+
+&#39;chore: bump version number&#39; ([`13648de`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/13648de60b78547ca878116fb4c78ba9fb03aa74))
+
 
 ## v0.9.0 (2022-10-21)
+
+### Chore
+
+* chore: clearer error message ([`3b81567`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/3b81567c15e1c95bda3811a0dc5d617aa6f3e8b8))
+
+* chore: clean up tests ([`07b254c`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/07b254ce97e10f0f86ac91c4bf2a4e772d670bde))
+
 ### Feature
-* Restore `!` selector operator ([`d4581ba`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/d4581ba2bbb5356e12c639597396eafe76d0acf4))
+
+* feat: restore `!` selector operator ([`d4581ba`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/d4581ba2bbb5356e12c639597396eafe76d0acf4))
+
+### Unknown
+
+* 0.9.0
+
+&#39;chore: bump version number&#39; ([`b4cbb39`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/b4cbb39b665e0abf95070d4a19a87c8cfcdd6225))
+
 
 ## v0.8.0 (2022-10-06)
+
+### Chore
+
+* chore: update version pins ([`508c7d9`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/508c7d994d3ce7e7b366f8a2bc635e4fa0e5679d))
+
 ### Feature
-* Add optional dimensions to `tasks@scheduler` option ([`9a4c768`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/9a4c7684392c10b9dfbc43d4525335ca3d2e1b60))
+
+* feat: add optional dimensions to `tasks@scheduler` option ([`9a4c768`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/9a4c7684392c10b9dfbc43d4525335ca3d2e1b60))
+
+### Unknown
+
+* 0.8.0
+
+&#39;chore: bump version number&#39; ([`d66893b`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/d66893bb59c84ce41feff487c223cfacc58594a9))
+
+* doc: fix typo ([`a7b237d`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/a7b237d9bd94891eeadcd2e858396e579d3a5220))
+
 
 ## v0.7.0 (2022-07-19)
+
 ### Feature
-* Add key-value list parser ([`825d5ac`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/825d5ac277b3d687a4a2b0d1190a6dfdc047b307))
+
+* feat: add key-value list parser ([`825d5ac`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/825d5ac277b3d687a4a2b0d1190a6dfdc047b307))
+
+### Unknown
+
+* 0.7.0
+
+&#39;chore: bump version number&#39; ([`1bd7a5c`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/1bd7a5c46054cba897e32170d24049a5d3968812))
+
 
 ## v0.6.0 (2022-07-07)
+
 ### Feature
-* Add `sumf` and `sumr` modifiers ([`533f0cb`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/533f0cb7033cc2ff5d4e005852bd75b259ae7923))
-* Add `empty_values` argument to `convert_intlist` ([`6be2ea1`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/6be2ea14c10d60fb2967424fe691df28eb95ed5f))
-* Add convert.convert_intlist ([`9a071c8`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/9a071c8816ea8e913baac322ab409bafe8fb7bd8))
-* Update ToolName.factory to accept a deconstructed tool base name and versions list ([`7d1b8e2`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/7d1b8e283d9c99bd3ab5effc03f9d0692fbb7267))
+
+* feat: add `sumf` and `sumr` modifiers ([`533f0cb`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/533f0cb7033cc2ff5d4e005852bd75b259ae7923))
+
+* feat: add `empty_values` argument to `convert_intlist` ([`6be2ea1`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/6be2ea14c10d60fb2967424fe691df28eb95ed5f))
+
+* feat: add convert.convert_intlist ([`9a071c8`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/9a071c8816ea8e913baac322ab409bafe8fb7bd8))
+
+* feat: update ToolName.factory to accept a deconstructed tool base name and versions list ([`7d1b8e2`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/7d1b8e283d9c99bd3ab5effc03f9d0692fbb7267))
 
 ### Fix
-* Handle tool options provided as child content ([`1a99ffb`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/1a99ffbbcbafdaba7e2451dec8e5bf46ee893e6a))
-* Relax task reference parsing even more. the initial dot is now not required anymore. the $ and internal operators can be escaped to ignore them ([`f353e7d`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/f353e7d6d52f772f76c326611bdbdb5513b8113b))
-* Relax task reference parsing, allowing trailing text immediately after the references without a dot as seperator ([`829b40c`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/829b40cee42ad376d4d000d3a3f0f780953eac94))
-* Expand task-id placeholders in references ([`545a619`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/545a619b495e7ab0f9c12d9ee4b9ab41b77d1c76))
-* Support placeholders in tool options ([`796f3ce`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/796f3ce75ebc404e08f86234154270215357c3fb))
+
+* fix: handle tool options provided as child content ([`1a99ffb`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/1a99ffbbcbafdaba7e2451dec8e5bf46ee893e6a))
+
+* fix: relax task reference parsing even more. the initial dot is now not required anymore. the $ and internal operators can be escaped to ignore them ([`f353e7d`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/f353e7d6d52f772f76c326611bdbdb5513b8113b))
+
+* fix: relax task reference parsing, allowing trailing text immediately after the references without a dot as seperator ([`829b40c`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/829b40cee42ad376d4d000d3a3f0f780953eac94))
+
+* fix: expand task-id placeholders in references ([`545a619`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/545a619b495e7ab0f9c12d9ee4b9ab41b77d1c76))
+
+* fix: support placeholders in tool options ([`796f3ce`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/796f3ce75ebc404e08f86234154270215357c3fb))
+
+### Unknown
+
+* 0.6.0
+
+&#39;chore: bump version number&#39; ([`aecb98d`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/aecb98daa08021acd3f9e6f6e6b4357d8ce84c85))
+
+* doc: update documentation and doctest for convert.convert_duration to include that seconds can contain decimals ([`71a1202`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/71a12029b48a486483ddd05e0384f26e0182bea2))
+
+* doc: update documentation of convert.convert_size() ([`2af0a09`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/2af0a0939dca4389ffca56340cff3468fdeed284))
+
 
 ## v0.5.0 (2022-04-08)
+
 ### Feature
-* Add duration and size conversion methods ([`424815f`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/424815fcc9c57d2e62dbd79e017e5e039a660a62))
+
+* feat: add duration and size conversion methods ([`424815f`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/424815fcc9c57d2e62dbd79e017e5e039a660a62))
 
 ### Fix
-* Correct option type usage and handling ([`2a0a537`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/2a0a537a2d2dfdab43fa3ab49c6c355c41170311))
-* Use option types as defined by the momotor-bundles package ([`e53b4c3`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/e53b4c3fddc5dd03ea18d8d99a87c19d3012c50f))
+
+* fix: correct option type usage and handling ([`2a0a537`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/2a0a537a2d2dfdab43fa3ab49c6c355c41170311))
+
+* fix: use option types as defined by the momotor-bundles package ([`e53b4c3`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/e53b4c3fddc5dd03ea18d8d99a87c19d3012c50f))
+
+### Unknown
+
+* 0.5.0
+
+&#39;chore: bump version number&#39; ([`69eaaed`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/69eaaed595ff3324d51918e468e782697bf1921e))
+
+* doc: document filter_files.py ([`abd3253`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/abd32531105f5effe0267b9b7c4f80e25b5351da))
+
+* doc: fix several Sphinx errors and warnings ([`2c63f18`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/2c63f1840aac4d83b8f3ced7772a03b00a96e891))
+
+* doc: add utility functions to docs ([`ec8c8b3`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/ec8c8b3f6a6cdc84cd071be4481497773ceb9928))
+
 
 ## v0.4.0 (2022-04-04)
+
 ### Feature
-* Add OptionDefinition.deprecated ([`9a98031`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/9a98031723833fc5717027b56d890f47f3bd0e76))
+
+* feat: add OptionDefinition.deprecated
+
+(redo from commit 5cbfdf4834ad5bafc9c91972371f5978ee2c0a13 to fix commit message) ([`9a98031`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/9a98031723833fc5717027b56d890f47f3bd0e76))
+
+### Unknown
+
+* 0.4.0
+
+&#39;chore: bump version number&#39; ([`a6d53f4`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/a6d53f4fc8e48ca9ac8a2dac8f296afa48fc68df))
+
+* Revert &#34;add OptionDefinition.deprecated&#34;
+
+This reverts commit 5cbfdf4834ad5bafc9c91972371f5978ee2c0a13. ([`279d15c`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/279d15cb7e294d3febeedee4fde2fb60fe2e4703))
+
+* add OptionDefinition.deprecated ([`5cbfdf4`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/5cbfdf4834ad5bafc9c91972371f5978ee2c0a13))
+
 
 ## v0.3.0 (2022-03-14)
-### Feature
-* Added `match_tool_requirements`. Also refactored types ([`2dd834b`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/2dd834be877c596ea79f7ee68ae55b43d67f07c9))
-* Add ToolRequirements type alias, cleanup imports ([`5012876`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/50128762927fae7413f0658feb92c3b12841ac61))
-* Add momotor.options.domain.scheduler.tools.get_scheduler_tools_option ([`3f16a99`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/3f16a9983a59d85fec01d326de8b8b84c9adf8a7))
-* Allow multiple version preferences to be supplied in the tools option ([`4f4f6ba`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/4f4f6ba55bbf284213ed502bbfa9a4fc3c05ab9b))
-* Add ToolOptionDefinition ([`ab5f387`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/ab5f387b64c71fb6e853c0532b98a3baf73b65ef))
-* Add function to match tool from a list of alternatives ([`1c25d2d`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/1c25d2d95100f2a541fb1a931ac9b5a2be8342e2))
-* Allow parts of tool name to be a wildcard when resolving, correctly merge versions in multiple registries ([`1064f69`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/1064f69247445dc87f77e46cc543f355f4e3eb38))
-* Add functions to access tool registry ([`935d0df`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/935d0dfc9184a9fd6fa90b9469d104b4dad1b2d7))
-
-### Fix
-* Add more unit tests for cases with defaults ([`fd425a2`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/fd425a211f4d34bbc10b9a1d84204d5f4563ca26))
-* Hide hidden fields from repr ([`cddbd6f`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/cddbd6fc8cac215343cd39001d3e3bc1f7f7ec27))
-* ToolVersion.is_partial should also return True if either version is DEFAULT ([`fd382f8`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/fd382f8d6ddc20f135d258743c1049bb1a588aa8))
-* Unit tests ([`b2a2871`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/b2a28712077097c0ff74c15edfbaad33f65241e9))
-* Set fixed location for tools domain options, use ToolName.SEPARATOR constant ([`d7db33a`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/d7db33a97e6f0020c9cc7c7aee8a806d5f330945))
-* Consistent argument naming ([`b0f8af5`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/b0f8af5cf430acbdc490309159f65d6b5cb73e6b))
-* Correctly handle symlinks in registry ([`3b70e30`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/3b70e30860a3f7c5c1cbf5a6b11338e0c45f7d0a))
-* Unit test ([`7755c6e`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/7755c6e24bd0589d4f9ad7967d77c4fb6346cda4))
-* Various fixes, cleanups and changes ([`273a1ea`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/273a1ea7ee741dcd1de266328e1a2e2b9adcbf4f))
-* Move NO_DEFAULT into OptionDefinition ([`7382692`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/73826926ea91293d249b7cef8b2491fba12903ea))
-* Make Tool.name the resolved name, add Tool.__hash__ ([`3d084a5`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/3d084a5bc97f5b51ca4dabd9ae0ad147075f3119))
-* When numeric versions and named versions are mixed, the numeric versions should be preferred over named versions ([`b352fce`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/b352fce768044ef910df9c1b27e58fccf6c57b67))
-* Use `_default` as default tool version or name ([`cc551de`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/cc551de6a5aecfffeaee3404d983d95dedf9f9fb))
-* Add SimpleVersion.__str__ for consistency with ToolName ([`0b37ae0`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/0b37ae0453a937cbed346ae7a7769ed1b78f94e4))
-* ToolName and SimpleVersion hash should be based on version(s) ([`69eae79`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/69eae79300e808f052842a807abb8e9c207800ee))
-* Match_tool should return the exact value from tools argument ([`ed324ab`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/ed324abf0dc848485e54bdc40655c1a5e6d4ae20))
-* Convert tool_info.name to str ([`ba157aa`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/ba157aa1ea007c9a4ce324542c839bd6a7475ee3))
-* Correct handling of version directories ([`785d674`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/785d67403012facd45c5483d59d8a54a7b66cf03))
 
-## v0.2.3 (2022-01-24)
 ### Fix
-* Replace_placeholders() should accept any non-string value argument ([`0035b68`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/0035b6854bbd37decdbabf25c2132eace308cc27))
 
-## v0.2.2 (2022-01-21)
-### Fix
-* Add unittests for all combiner modifiers, fix issues with the combiner modifiers ([`adc6475`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/adc6475dfe54d85871b554d6b3da3aba433c61c4))
+* fix: add more unit tests for cases with defaults ([`fd425a2`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/fd425a211f4d34bbc10b9a1d84204d5f4563ca26))
 
-## v0.2.1 (2022-01-18)
-### Fix
-* Use 'skip-error' action as default error action ([`c98e3da`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/c98e3da587ecaed17c935e21f11800f34787031c))
-* Include options from step in preflight result ([`ba5070b`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/ba5070b8335732ab8849e5afc6eeafe7bc09134f))
-
-## v0.2.0 (2022-01-18)
-### Feature
-* Added 'no' match modifier, removed '!' operator ([`39f6f12`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/39f6f1229a881d27688a9684de75325cbf3317be))
-* Allow multiple providers in references (close #9) ([`9ae0b1a`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/9ae0b1afeec9c250d828b4e917c8618091d1b343))
-
-### Fix
-* Make %not an alias for %notany ([`0884717`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/088471781b977985976019b2baaa31d7ee297fd3))
-* Change 'no'/'none' into 'notall'/'notany', implement same for value references ([`0599591`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/05995916a914e68d02080458e9166e7ade1f9ef6))
-* Handle invalid selectors ([`e136e41`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/e136e410b699bed4f4c9b55528b9284aba99469a))
-* Correctly handle option domain defaults ([`11e3ca8`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/11e3ca85192802e6a472d6fa265e167eeaca19d0))
-* Handle ids with wildcards in references (closes #7) ([`9370fe8`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/9370fe8dffd8e112bfdfc22a8de7f33a50443ad5))
-* Add logging ([`0369311`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/0369311bb5c94d00c8b139d09aa958b35476d6a3))
-* Preflight option can have mod ([`208ac07`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/208ac079b28c29773fe6403c81db2a66915037c8))
-
-## v0.1.0 (2022-01-17)
-### Feature
-* Generate default option subdomains (closes #7) ([`8e39f09`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/8e39f0954b5c3b982b9a651dca2632d2d9cbf28a))
-* Add 'always' preflight option action ([`5459dcb`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/5459dcbbc12d2c60239a3b028f97f2adcbf8d832))
-* Allow OptionDefinition.name to be an OptionNameDomain object ([`eb9da99`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/eb9da99dfc82383bf720b0cce1f8f3252355aa48))
-* Restore the select_by_XXX_reference methods ([`e7ce22b`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/e7ce22bf3d89d2f50e659b6366fe19681de751da))
-* Add argument to change default modifier for resolve_value_reference ([`59bbe20`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/59bbe20b94c582c432dc83e081487cde2f9ea685))
-* Add `result` reference type ([`ac52431`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/ac52431385fb98c0cae276470396a8df2f656cbb))
-* Replace placeholders in tasks@scheduler option ([`72798b9`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/72798b93afe10488e0c60e87d82e0b940966153b))
-* Restored filter_result_query function ([`e20003a`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/e20003af48e9313ea170a1f1d72bf3c691c9d2b1))
-* Add `value_processor` to apply_template ([`3dabf78`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/3dabf78e4bc82139e99f0aac694a5a8778184f12))
-* Make OptionsProviders more generic and also use it for the parsers ([`f03bd77`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/f03bd77778155d27de43025c4abe6d680799dc7c))
-* Add task-number expansion ([`16f6442`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/16f64425e5e44243b42e013f16107065e01fe5d4))
-* Add '!' and '!=' operations since there is no more "not-prop" type ([`cc3b698`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/cc3b69836ffa3e50138e68214ad7972310cc51d0))
-* Add template parser ([`cd7c1ea`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/cd7c1ea1896e121aaf8d9202a2cb692c8e9be8d7))
-* Add new selector methods ([`0d30ac5`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/0d30ac5005124b3e3c6324b112bb0e733f481991))
-* Change reference resolver to return both the containing element and the resolved objects ([`9f8f054`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/9f8f05452e853f7a7d8135fda8db6d5b0d3e1c83))
-* Add generalized parser and resolvers for outcome/property/file/option references ([`03a6dc1`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/03a6dc1df9b18abea51d165cafddf70ee1019257))
-
-### Fix
-* Properly document and validate required OptionDefinition.location and OptionDefinition.domain attributes ([`ecb287e`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/ecb287e6af5143b15ded809974aea03331a52d21))
-* Properly document and validate required OptionDefinition.location and OptionDefinition.domain attributes ([`14ea4e0`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/14ea4e0679dc18035e4845ffcf2f6858320dfe90))
-* Generate correct subdomains and collect all options for preflight option ([`2a9bfeb`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/2a9bfeb681e21e3bf09d3a1a33557210a5e70675))
-* Filter invalid refs ([`217194b`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/217194b874df5c1dcff785a00ad22b20c426df57))
-* Match_by_selector should always return False if no objects match ([`131bd6b`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/131bd6bf5f2da1766333bbff7f3f05bef012f8d1))
-* Restore tests for select_by_XXX_reference ([`d21d72b`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/d21d72bd5c959d38811b6d8cfab6e4346f7c5319))
-* File-references class part is default ([`c9095d0`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/c9095d06b03e49097b1d58de20544622331b8ea3))
-* Swap "?" and (no oper) operations ([`92523b9`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/92523b92ea44596c46b82261385ec57b3c704fed))
-* Remove mod parsing from `parse_selector` ([`3b975fe`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/3b975fef5ae0e0fa96e35b4caee81c739983db95))
-* Only raise InvalidDependencies for explicit dependencies, not for wildcard or placeholder ones ([`50f54ac`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/50f54acc44899f0d3987a3585cca3a61be302651))
-* Correct providers for tasks@scheduler value ([`5a5c803`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/5a5c8034b563c282641efeddf307eff8535b1997))
-* Change default pre-flight error action to 'error' ([`ea21419`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/ea21419a31f49e919961fa95afec8213aeb8a605))
-* For 'sum', 'min' and 'max' modifier, cast items to numbers ([`77fd72e`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/77fd72ec052a99d6f4bfb7c663a8d5818a9e0411))
-* With task numbers available, step option is no longer needed ([`a5b898f`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/a5b898fcad77e5e81f7822fa1660d62dbede978f))
-* Make VALID_LOCATIONS a set ([`70b2dd6`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/70b2dd692520d1795c951aad24a4b0f4a4e692df))
-* Remove unused function ([`46762aa`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/46762aa0b93a4101492f6ea12db48bbbb3ac10c1))
-* Refs have multiple id's, but only a single class/name part; return all elements even if there's no match (needed for match selector) ([`17c47fa`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/17c47fa7ae03bfe9644bfc5cd0025a002b20cea8))
-* Conditions as part of selectors can contain '#' ([`9c47283`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/9c47283eb75e63b5465bc51e9fe27b8d9e8b04c9))
+### Unknown
+
+* 0.3.0
+
+&#39;chore: bump version number&#39; ([`3439b8a`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/3439b8a8eb29b2d4976b2374873aec6f22e45347))
+
+
+## v0.2.3 (2022-01-24)
+
+### Unknown
+
+* 0.2.3
+
+&#39;chore: bump version number&#39; ([`be35ea1`](https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/-/commit/be35ea1b1c0ff327d209d74360ef7e0df0126c84))
```

### Comparing `momotor-engine-options-2.0.0rc9/PKG-INFO` & `momotor_engine_options-2.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: momotor-engine-options
-Version: 2.0.0rc9
+Version: 2.0.1
 Summary: Momotor Engine Options Library
 Author-email: Erik Scheffers <e.t.j.scheffers@tue.nl>
 License: GNU Lesser General Public License v3 (LGPLv3)
 Project-URL: Homepage, https://momotor.org
 Project-URL: Documentation, https://momotor.org/doc/engine/momotor-engine-options/
 Project-URL: Repository, https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/
 Project-URL: Tracker, https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/issues
@@ -14,31 +14,34 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: momotor-bundles~=8.0rc
+Requires-Dist: momotor-bundles~=8.0
 Requires-Dist: typing-extensions; python_version < "3.11"
 Provides-Extra: test
-Requires-Dist: pytest~=7.4; extra == "test"
+Requires-Dist: pytest~=8.1; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-doctestplus; extra == "test"
 Provides-Extra: docs
-Requires-Dist: docutils; extra == "docs"
+Requires-Dist: momotor-engine-options[test]; extra == "docs"
 Requires-Dist: Sphinx; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints!=1.14.0; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Provides-Extra: dev
-Requires-Dist: setuptools; extra == "dev"
-Requires-Dist: build[virtualenv]; extra == "dev"
+Requires-Dist: momotor-engine-options[docs]; extra == "dev"
 Requires-Dist: docutils-stubs; extra == "dev"
-Requires-Dist: python-semantic-release~=8.0; extra == "dev"
-Requires-Dist: twine; extra == "dev"
+Provides-Extra: build
+Requires-Dist: momotor-engine-options[dev]; extra == "build"
+Requires-Dist: setuptools; extra == "build"
+Requires-Dist: setuptools-scm; extra == "build"
+Requires-Dist: build[virtualenv]; extra == "build"
+Requires-Dist: python-semantic-release~=9.0; extra == "build"
 
 This package is a part of [Momotor](https://momotor.org/), a tool for automated processing of digital content. 
 
 Momotor accepts digital content as a product bundle and generates a result bundle from this product under 
 control of a recipe bundle. 
 
 Momotor is like a continuous integration system, but broader in scope. The
```

### Comparing `momotor-engine-options-2.0.0rc9/README.md` & `momotor_engine_options-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc9/docs/Makefile` & `momotor_engine_options-2.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc9/docs/make.bat` & `momotor_engine_options-2.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc9/docs/source/_static/logo-text-negative.png` & `momotor_engine_options-2.0.1/docs/source/_static/logo-text-negative.png`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc9/docs/source/_static/logo-text.png` & `momotor_engine_options-2.0.1/docs/source/_static/logo-text.png`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc9/docs/source/_templates/projectlinks.html` & `momotor_engine_options-2.0.1/docs/source/_templates/projectlinks.html`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc9/docs/source/conf.py` & `momotor_engine_options-2.0.1/docs/source/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,47 +7,37 @@
 # -- Path setup --------------------------------------------------------------
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import datetime
+import importlib.metadata
 import os
 import re
 import sys
 
 project_dir = os.path.join(os.path.dirname(os.path.abspath(__file__)), '..', '..')
 src_dir = os.path.join(project_dir, 'src')
 sys.path.insert(0, src_dir)
 
 
-def get_version():
-    import os.path
-
-    version_tag = os.environ.get('VERSION_TAG', '')
-
-    with open(os.path.join(src_dir, 'momotor', 'options', 'version.py'), 'r') as version_file:
-        loc = {}
-        exec(version_file.readline(), {}, loc)
-        return loc['__VERSION__'] + version_tag
-
-
 # -- Project information -----------------------------------------------------
 
 package_name = 'momotor-engine-options'
 project = 'Momotor Engine Options'
 copyright = '2021-%d, Eindhoven University of Technology' % datetime.datetime.now().year
 author = 'E.T.J. Scheffers'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The full version, including alpha/beta/rc tags.
-release = get_version()
+release = importlib.metadata.version(package_name)
 # The short X.Y version.
 version = re.match(r'\d+\.\d+', release).group(0)
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
```

### Comparing `momotor-engine-options-2.0.0rc9/docs/source/index.rst` & `momotor_engine_options-2.0.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc9/docs/source/options/index.rst` & `momotor_engine_options-2.0.1/docs/source/options/index.rst`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc9/docs/source/options/tools.rst` & `momotor_engine_options-2.0.1/docs/source/options/tools.rst`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc9/docs/source/parser/index.rst` & `momotor_engine_options-2.0.1/docs/source/parser/index.rst`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc9/docs/source/parser/syntax.rst` & `momotor_engine_options-2.0.1/docs/source/parser/syntax.rst`

 * *Files 8% similar despite different names*

```diff
@@ -9,30 +9,34 @@
 Usually these references are used in the recipe and config bundle options.
 
 .. _reference:
 
 Reference
 =========
 
-A reference refers to one or more
+A *reference* refers to one or more
 :py:class:`~momotor.bundles.elements.result.Result`,
 :py:class:`~momotor.bundles.elements.properties.Property`,
 :py:class:`~momotor.bundles.elements.files.File` or
 :py:class:`~momotor.bundles.elements.options.Option` elements in bundles.
 
-The syntax for a reference is:
+The syntax for a *reference* is:
 
 .. productionlist:: reference
    typed_reference: `type` "[" `reference` [ "," `reference` ]* "]"
    type: "file" | "prop" | "opt" | "result" | `outcome` | `not_outcome`
-   reference: [ "@" `provider` ] [ "#" id ( "," id )* ] [ ":" `ref` ]
    outcome: "pass" | "fail" | "error" | "skip"
    not_outcome: "not-" `outcome`
+   reference: ( `provider_id` [ ":" `typeref` ] ) | `typeref`
+   provider_id: "@" `provider` ] [ "#" `id` ( "," `id` )* ]
    provider: "recipe" | "config" | "product" | "step" | "result"
-   ref: name | class "#" name | name "@" domain
+   typeref: `propref` | `fileref` | `optref`
+   propref: `name`
+   fileref: `class` | [ `class` ] "#" `name`
+   optref: `name` [ "@" `domain` ]
 
 The :token:`~reference:type` defines the element type which is referenced. Choices are
 
 +----------------------------------------------+---------------------------------------------------------------------+
 | :token:`~reference:type`                     | element referenced                                                  |
 +==============================================+=====================================================================+
 | :token:`prop <reference:type>`               | One or more                                                         |
@@ -83,33 +87,40 @@
 For the :token:`opt <reference:type>` and :token:`file <reference:type>` types, all providers are valid.
 
 Since :py:class:`~momotor.bundles.ResultsBundle` bundles contain multiple results, one or more ``id`` tokens
 can be specified to limit the list of results. If no ``id`` is given, all results in the bundle are referenced.
 ``id`` is not used with other providers. The ``id`` can contain :ref:`task id <task_id>` placeholders and these
 will be expanded with the task numbers for the currently active task.
 
-The :token:`prop <reference:type>`, :token:`file <reference:type>` and :token:`opt <reference:type>` types
-require an additional name and a class (for :token:`file <reference:type>` types) or a domain
-(for :token:`opt <reference:type>` types).
-For :token:`file <reference:type>` types, the name can contain glob-like wildcards and can be quoted if it
-contains space or any other special characters.
-For :token:`opt <reference:type>` types, if domain is not provided it defaults to ``checklet``.
+The :token:`file <reference:type>` reference type requires an additional :token:`name and/or class <reference:fileref>`
+to select the file(s). The name can contain glob-like wildcards and can be quoted if it contains space or any
+other special characters.
+
+The :token:`prop <reference:type>` reference type requires an additional :token:`name <reference:propref>` to
+select the property.
+
+The :token:`opt <reference:type>` reference type requires an additional
+:token:`name with optional domain <reference:optref>` to select the option.
+If domain is not provided it defaults to ``checklet``.
+
 Similar to ``id``, :ref:`task id <task_id>` placeholders will be expanded in references too.
 
 Examples of references are:
 
 =========================================== =============================================================================================
 reference                                   result
 ------------------------------------------- ---------------------------------------------------------------------------------------------
 ``prop[:name1]``                            Selects properties with name ``name1`` from all results in the results bundle
 ``prop[#id1:name1]``                        Selects properties with name ``name1`` from result with result id ``#id1``
 ``prop[@result#id1:name1]``                 Same as above (``@result`` is optional and implied)
 ``file[@config:class1#name1]``              Selects the file with class ``class1`` and exact name ``name1`` from the config
 ``file[@config:class1#*.txt]``              Selects all files with class ``class1`` and name ending with ``.txt`` from the config
-``file[@recipe:class1#"doc 1.txt"]``        Selects all files with class ``class1`` and exact name ``doc 1.txt`` from the recipe
+``file[@recipe:class1#doc.txt]``            Selects all files with class ``class1`` and exact name ``doc.txt`` from the recipe
+``file[@recipe:class1#"doc 1.txt"]``        Selects all files with class ``class1`` and exact name ``doc 1.txt`` from the recipe.
+                                            Because of the whitespace, the name has to be quoted
 ``opt[@step:name1]``                        Selects the option with name ``name1`` in (default) domain ``checklet`` of the current step
 ``opt[@step:name1@domain1]``                Selects the option with name ``name1`` in domain ``domain1`` of the current step
 ``result``                                  Select all results from the results bundle
 ``result[#id1]``                            Select result with id ``id1`` from the results bundle
 ``pass``                                    Select all passed results from the results bundle
 ``pass[#id1,#id2]``                         Select results with result id ``id1`` and ``id2``, if they passed
 ``pass[@result#id1,#id2]``                  Same as above (``@result`` is optional and implied)
@@ -117,28 +128,29 @@
 =========================================== =============================================================================================
 
 .. _reference value:
 
 Reference value
 ===============
 
-A reference value is a single value generated from a :ref:`reference`. Checklets can use reference values in
-options to resolve those options into values.
-References are also used as part of the :ref:`placeholder` syntax.
+A *reference value* is a single value generated from a :ref:`reference <reference>`.
+Checklets can use *reference values* in options to resolve those options into values.
+*Reference values* are also used as part of the :ref:`placeholder <placeholder>` syntax.
 
-A reference value is a :ref:`reference` optionally prefixed with a modifier:
+A *reference value* is a :ref:`reference <reference>`, optionally prefixed with a modifier:
 
 .. productionlist:: reference_value
    value_reference: [ "%" `mod` ] `~reference:typed_reference`
-   mod: "all" | "any" | "sum" | "max" | "min" | "cat" | "join"
+   mod: "all" | "any" | "notall" | "notany" | "not" | "sum"
+      : | "sumf" | "sumr" | "max" | "min" | "cat" | "join"
       : | "joinc" | "joins" | "joincs" | "json" | "first" | "last"
 
 .. _reference type value:
 
-What value is produced by a reference is determined by the reference :token:`~reference:type`:
+What value is produced by a *reference value* is determined by the reference :token:`~reference:type`:
 
 +------------------------------------------------+---------------------------------------------------------------------+
 | :token:`~reference:type`                       | value                                                               |
 +================================================+=====================================================================+
 | :token:`prop <reference:type>` /               | The :attr:`value` attribute of the referenced                       |
 | :token:`opt <reference:type>`                  | :py:class:`~momotor.bundles.elements.properties.Property` or        |
 |                                                | :py:class:`~momotor.bundles.elements.options.Option` elements       |
@@ -161,17 +173,20 @@
 +------------------------------------------------+---------------------------------------------------------------------+
 
 .. [#resultvalue]
 
    The :token:`result <reference:type>` and :token:`~reference:outcome` / :token:`~reference:not_outcome` types
    produce different values, although they both reference :py:class:`~momotor.bundles.elements.result.Result` elements.
 
-The :token:`~reference_value:mod` modifier indicates how the list of values produced by the reference is converted
-into a single value. The default modifier is :token:`join <reference_value:mod>`, but this can be changed by the
-caller of the :py:meth:`~momotor.options.parser.reference.resolve_value_reference` method.
+.. _reference value modifier:
+
+The :token:`~reference_value:mod` modifier indicates how the list of values produced by the :ref:`reference <reference>`
+is converted into a *reference value*.
+The default modifier is :token:`join <reference_value:mod>`, but this can be changed by the
+caller of the :py:meth:`~momotor.options.parser.reference.resolve_reference_value` method.
 
 +------------------------------------------------+---------------------------------------------------------------------+
 | :token:`~reference_value:mod`                  | result                                                              |
 +================================================+=====================================================================+
 | :token:`%all <reference_value:mod>`            | `True` if all values are considered `True` [#anyall]_               |
 +------------------------------------------------+---------------------------------------------------------------------+
 | :token:`%any <reference_value:mod>`            | `True` if at least one value is considered `True` [#anyall]_        |
@@ -238,22 +253,22 @@
 All other modifiers convert the values to a string before joining.
 
 .. _selector:
 
 Selector
 ========
 
-A :ref:`selector` filters references on the referenced value. The value is one of the attributes of the referenced
+A *selector* filters :ref:`references <reference>` on the value. The value is one of the attributes of the referenced
 elements, the same attribute as used for :ref:`value references <reference type value>`.
 
-A selector has the following syntax:
+A *selector* has the following syntax:
 
 .. productionlist:: selector
    selector: `~reference:typed_reference` [ `selection` ]
-   selection: `unary_oper` | `binary_oper` value
+   selection: `unary_oper` | `binary_oper` `value`
    unary_oper: "?" | "!"
    binary_oper: "==" | "!=" | ">" | ">=" | "<" | "<="
 
 +------------------------------------------------+---------------------------------------------------------------------+
 | operator                                       | action                                                              |
 +================================================+=====================================================================+
 | (no selector)                                  | Selects all elements (i.e. same as the reference)                   |
@@ -261,15 +276,15 @@
 | :token:`? <selector:unary_oper>`               | Unary operator which selects the elements whose value is            |
 |                                                | considered `True` [#queexl]_                                        |
 +------------------------------------------------+---------------------------------------------------------------------+
 | :token:`\! <selector:unary_oper>`              | Unary operator which selects the elements whose value is            |
 |                                                | considered `False` [#queexl]_                                       |
 +------------------------------------------------+---------------------------------------------------------------------+
 | :token:`== <selector:binary_oper>` /           | Binary operators.                                                   |
-| :token:`~= <selector:binary_oper>` /           | Selects the elements whose value matches the equation.              |
+| :token:`\!= <selector:binary_oper>` /          | Selects the elements whose value matches the equation.              |
 | :token:`> <selector:binary_oper>` /            | String values to compare with need to be quoted.                    |
 | :token:`>= <selector:binary_oper>` /           |                                                                     |
 | :token:`< <selector:binary_oper>` /            |                                                                     |
 | :token:`<= <selector:binary_oper>`             |                                                                     |
 +------------------------------------------------+---------------------------------------------------------------------+
 
 .. [#queexl]
@@ -297,25 +312,25 @@
 Match
 =====
 
 .. productionlist:: match
    match: [ "%" `mod` ] `~selector:selector`
    mod: "all" | "any" | "not" | "notall" | "notany"
 
-A :ref:`match` takes a :ref:`selector` and collapses it into a boolean, depending on the :token:`~match:mod`
+A *match* takes a :ref:`selector <selector>` and collapses it into a boolean, depending on the :token:`~match:mod`
 modifier.
 
 +-----------------------------------------------------------+--------------------------------------------------------------+
 | :token:`~match:mod`                                       | match                                                        |
 +===========================================================+==============================================================+
 | No modifier or :token:`%all <match:mod>`                  | Matches if the selector is "true" for all referenced elements|
 +-----------------------------------------------------------+--------------------------------------------------------------+
 | :token:`%any <match:mod>`                                 | Matches if there is at least one selected element "true"     |
 +-----------------------------------------------------------+--------------------------------------------------------------+
-| :token:`%notall <match:mod>`                              | Matches if not all or the selected elements are "true"       |
+| :token:`%notall <match:mod>`                              | Matches if not all of the selected elements are "true"       |
 +-----------------------------------------------------------+--------------------------------------------------------------+
 | :token:`%not <match:mod>` or :token:`%notany <match:mod>` | Matches if not any of the selected elements is "true"        |
 +-----------------------------------------------------------+--------------------------------------------------------------+
 
 +--------------+-----------------------------+---------------------------+------------------------------+--------------------------------+
 | elements     | | no modifier or            | :token:`%any <match:mod>` | :token:`%notall <match:mod>` | | :token:`%not <match:mod>`    |
 |              | | :token:`%all <match:mod>` |                           |                              | | :token:`%notany <match:mod>` |
@@ -331,53 +346,52 @@
 Example matches:
 
 +------------------------------------------------+---------------------------------------------------------------------+
 | match                                          |                                                                     |
 +================================================+=====================================================================+
 | ``pass``                                       | Matches if all results passed                                       |
 +------------------------------------------------+---------------------------------------------------------------------+
-| ``%any pass``                                  | Matches if at least one result passed                               |
+| ``%any pass``                                  | Matches if at least one result passed                               |
 +------------------------------------------------+---------------------------------------------------------------------+
-| ``%notall pass``                               | Matches if not all results passed                                   |
+| ``%notall pass``                               | Matches if not all results passed                                   |
 +------------------------------------------------+---------------------------------------------------------------------+
-| ``%notany pass``                               | Matches if at least one result did not pass                         |
+| ``%notany pass``                               | Matches if at least one result did not pass                         |
 +------------------------------------------------+---------------------------------------------------------------------+
 | ``prop[score]``                                | Matches if all results contain a score property                     |
 +------------------------------------------------+---------------------------------------------------------------------+
-| ``%any prop[score]``                           | Matches if at least one result contains a score property            |
+| ``%any prop[score]``                           | Matches if at least one result contains a score property            |
 +------------------------------------------------+---------------------------------------------------------------------+
 | ``prop[score]>1``                              | Matches if all results contain a score of more than 1               |
 +------------------------------------------------+---------------------------------------------------------------------+
 
 .. _placeholder:
 .. _reference placeholder:
 
 Reference placeholder
 =====================
 
-Placeholders can be used inside a longer string. The placeholder will be replaced by the value produced by
-the :ref:`reference value`
+*Reference placeholders* can be used inside a longer string. The placeholder will be replaced by the value produced by
+the :ref:`reference value <reference value>`.
 
 .. productionlist:: placeholder
    placeholder: "${" `~reference_value:value_reference` "}"
 
-Placeholders are reference values wrapped inside a ``${...}``. To include a literal ``${`` in the string, use
-``$${`` to escape the placeholder syntax.
-
+Placeholders are :ref:`reference values <reference value>` wrapped inside a ``${...}``.
+To include a literal ``${`` in the string, use ``$${`` to escape the placeholder syntax.
 
 .. _task id placeholder:
 
 Task id placeholder
 ===================
 
-Task id placeholders can be used inside a longer string. The placeholder will be replaced by the sub-task number of the
-currently active task, either zero-based or one-based.
+*Task id placeholders* can be used inside a longer string. The placeholder will be replaced by the
+sub-task number of the currently active task, either zero-based or one-based.
 
 .. productionlist:: task_id_placeholder
-   task_id_placeholder: "$" [ task_id_base ] "#"
+   task_id_placeholder: "$" [ `task_id_base` ] "#"
    task_id_base: "0" | "1"
 
 Task id placeholders are ``$#``, ``$0#`` and ``$1#``. The ``0`` and ``1`` indicate whether the task id is zero-based or
 one-based. If no base is given, the default is zero-based. If there is no task, the placeholder will be
 replaced by a ``-``.
 
 Examples, for a task with id ``task.0.1``:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `momotor-engine-options-2.0.0rc9/docs/source/registry.rst` & `momotor_engine_options-2.0.1/docs/source/registry.rst`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 To configure a checklet to use a certain tool version, two options are needed: the
 :momotor:option:`tools@scheduler option <tools@scheduler>` in each step that requires external tools,
 to indicate to the scheduler which tools are required by the step's checklet, and options in the
 :ref:`tools domain <tools domain>` to define the actual tool versions to use.
 
 The options in the :ref:`tools domain <tools domain>` can be defined in the recipe or config bundles,
 and can contain :ref:`placeholders <placeholder>`. This makes it possible to define
-the tool version based a property generated by earlier executed steps, for example:
+the tool version based a on property generated by earlier executed steps, for example:
 
 .. code-block:: xml
 
    <options domain="tools">
      <option name="java" value="${prop[#build-java:exectool]}" />
    </options>
```

### Comparing `momotor-engine-options-2.0.0rc9/docs/source/result_query.rst` & `momotor_engine_options-2.0.1/docs/source/result_query.rst`

 * *Files 5% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 Result queries allows selection of these result ids using wildcards and with a replacement for some of the task
 numbers based on another task number.
 
 The syntax for a result query is
 
 .. productionlist:: result-query
    queries: `query` ( "," `query` )*
-   query: step-id [ `task_query` ] | [ step-id ] "*" [ `task_query` ] | [ step-id ] "**"
+   query: `step_id` [ `task_query` ]
+        : | [ `step_id` ] "*" [ `task_query` ]
+        : | [ `step_id` ] "**"
    task_query: ( "." `task_number` )* | ".$@"
-   task_number: integer | `task_wildcard` | `task_reference`
+   task_number: `integer` | `task_wildcard` | `task_reference`
    task_wildcard: "*" | "?"
-   task_reference: "$" integer [ `oper` integer ]
+   task_reference: "$" `integer` [ `oper` `integer` ]
    oper: "+" | "-" | "*" | "/" | "%"
 
 Where `step-id` is a (XML) id without periods (``.``), and `integer` is a positive natural number
 (including zero).
 
 The most simple result queries are just the result id and will match that single result id:
```

### Comparing `momotor-engine-options-2.0.0rc9/docs/source/utilities.rst` & `momotor_engine_options-2.0.1/docs/source/utilities.rst`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc9/pyproject.toml` & `momotor_engine_options-2.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -18,36 +18,40 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3 :: Only"
 ]
 dependencies = [
-    'momotor-bundles~=8.0rc',
+    'momotor-bundles~=8.0',
     "typing-extensions; python_version < '3.11'",
 ]
 
 [project.optional-dependencies]
 test = [
-    'pytest~=7.4',
+    'pytest~=8.1',
     'pytest-cov',
-    'pytest-doctestplus'
+    'pytest-doctestplus',
 ]
 docs = [
-    'docutils',
+    'momotor-engine-options[test]',
     'Sphinx',
     'sphinx-autodoc-typehints!=1.14.0',
     'furo',
 ]
 dev = [
+    'momotor-engine-options[docs]',
+    'docutils-stubs',
+]
+build = [
+    'momotor-engine-options[dev]',
     'setuptools',
+    'setuptools-scm',
     'build[virtualenv]',
-    'docutils-stubs',
-    'python-semantic-release~=8.0',
-    'twine'
+    'python-semantic-release~=9.0',
 ]
 
 [project.urls]
 Homepage = "https://momotor.org"
 Documentation = "https://momotor.org/doc/engine/momotor-engine-options/"
 Repository = "https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/"
 Tracker = 'https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/issues'
@@ -55,29 +59,35 @@
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["momotor.*"]
 
+[tool.setuptools.package-data]
+"momotor.bundles.schema" = ["*.xsd"]
+
 [tool.setuptools.dynamic]
-version = { attr = "momotor.options.version.__VERSION__" }
 readme = { file = ["README.md"], content-type = "text/markdown" }
 
+[tool.setuptools_scm]
+
 [tool.pytest.ini_options]
 required_plugins = ["pytest-doctestplus"]
 norecursedirs = [".git", "files"]
 pythonpath = "src"
 addopts = "--cov=src --doctest-plus --doctest-rst --doctest-modules -p no:django"
 xfail_strict = true
 
 [tool.semantic_release]
-version_variables = ["src/momotor/options/version.py:__VERSION__"]
+version_toml = ["version.toml:semantic_release.version"]
 commit_message = 'chore: bump version number'
-build_command = "python -m build --outdir ."
+
+[tool.semantic_release.changelog]
+exclude_commit_patterns = ["^Merge branch ", "^ci\\s*[:(]", "^build\\s*[:(]"]
 
 [tool.semantic_release.release]
 upload_to_vcs_release = false
 
 [tool.semantic_release.remote]
 type = "gitlab"
 token = { env = "GL_TOKEN" }
```

### Comparing `momotor-engine-options-2.0.0rc9/src/momotor/options/convert.py` & `momotor_engine_options-2.0.1/src/momotor/options/convert.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc9/src/momotor/options/dependencies.py` & `momotor_engine_options-2.0.1/src/momotor/options/dependencies.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 """ Methods for resolving result dependencies
 """
 from __future__ import annotations
 
+import collections.abc
 from collections import deque
 
-import typing
-
 from momotor.bundles import RecipeBundle, ConfigBundle
 from momotor.options.domain.scheduler.tasks import get_scheduler_tasks_option
 from momotor.options.exception import CircularDependencies, InvalidDependencies
 from momotor.options.result_query import make_result_id_re
 from momotor.options.task_id import StepTaskId, iter_task_numbers, iter_task_ids, \
     get_task_id_lookup, apply_task_number
 from momotor.options.types import StepTasksType
 
 __all__ = [
     'get_full_task_dependencies', 'reverse_task_dependencies', 'get_task_dependencies'
 ]
 
 
 def _extract_deps(recipe: RecipeBundle, config: ConfigBundle | None) \
-        -> typing.Mapping[str, tuple[typing.Sequence[str], StepTasksType | None]]:
+        -> collections.abc.Mapping[str, tuple[collections.abc.Sequence[str], StepTasksType | None]]:
     """ Extract step dependency info from recipe and config
     """
     return {
         step_id: (
             tuple(step.get_dependencies_ids()),
             get_scheduler_tasks_option(recipe, config, step_id)
         )
         for step_id, step in recipe.steps.items()
     }
 
 
 def _collect_dependency_matches(depend_id_str: str, task_id: StepTaskId, task_ids_map: dict[str, StepTaskId]) \
-        -> typing.Generator[StepTaskId, None, None]:
+        -> collections.abc.Generator[StepTaskId, None, None]:
 
     applied_id = apply_task_number(depend_id_str, task_id)
     if '#' in applied_id:
         # A `#` in the applied_id indicates an arithmetic error
         # Ignoring this allows tasks to depend on a previous task, with the first task not having such
         # dependency
         return
@@ -54,32 +53,32 @@
             yield dep_task_id
         elif applied_id == depend_id_str:
             raise InvalidDependencies(
                 f"Task {str(task_id)!r} depends on non-existent task(s) {depend_id_str!r}"
             )
 
 
-def _reorder_taskids(task_ids: typing.Container[StepTaskId], ordering: typing.Iterable[StepTaskId]) \
+def _reorder_taskids(task_ids: collections.abc.Container[StepTaskId], ordering: collections.abc.Iterable[StepTaskId]) \
         -> tuple[StepTaskId, ...]:
 
     # Convert a container of StepTaskIds into a tuple, using the order given by `ordering`
     return tuple(
         task_id
         for task_id in ordering
         if task_id in task_ids
     )
 
 
 def _get_full_deps(
-            step_dep_info: typing.Mapping[str, tuple[typing.Sequence[str], StepTasksType | None]]
+            step_dep_info: collections.abc.Mapping[str, tuple[collections.abc.Sequence[str], StepTasksType | None]]
         ) -> dict[StepTaskId, tuple[StepTaskId, ...]]:
 
     # collect all step and task ids
     # step_ids: frozenset[str] = frozenset(step_dep_info.keys())  # all step ids
-    step_task_ids: dict[str, typing.Sequence[StepTaskId]] = {}  # task ids for each step
+    step_task_ids: dict[str, collections.abc.Sequence[StepTaskId]] = {}  # task ids for each step
 
     task_ids = deque()  # all task ids
     for step_id, (depends, tasks) in step_dep_info.items():
         ids = list(iter_task_ids(step_id, tasks))
         step_task_ids[step_id] = ids
         task_ids.extend(ids)
 
@@ -124,15 +123,15 @@
         task_id: _collect(task_id, frozenset())
         for task_id in task_ids
     }
 
 
 def _get_direct_deps(
     task_id: StepTaskId,
-    step_dep_info: typing.Mapping[str, tuple[typing.Sequence[str], StepTasksType | None]]
+    step_dep_info: collections.abc.Mapping[str, tuple[collections.abc.Sequence[str], StepTasksType | None]]
 ) -> tuple[StepTaskId, ...]:
 
     # collect all step and task ids
     # step_ids: frozenset[str] = frozenset(step_dep_info.keys())  # all step ids
     step_task_ids: dict[str, frozenset[StepTaskId]] = {}  # task ids for each step
     task_ids = deque()  # all task ids
     for step_id, (step_deps, tasks) in step_dep_info.items():
@@ -182,15 +181,15 @@
     :raises CircularDependencies: if the recipe contains circular dependencies
     :raises InvalidDependencies: if the recipe contains invalid dependencies
     """
 
     return _get_direct_deps(task_id, _extract_deps(recipe, config))
 
 
-def reverse_task_dependencies(dependencies: dict[StepTaskId, typing.Iterable[StepTaskId]]) \
+def reverse_task_dependencies(dependencies: dict[StepTaskId, collections.abc.Iterable[StepTaskId]]) \
         -> dict[StepTaskId, tuple[StepTaskId, ...]]:
     """ Reverses the dependency tree generated by :py:func:`get_task_dependencies`,
     i.e. for each step it lists which other steps depend on it.
 
     Task ordering is preserved: the tasks listed in the result, both the dict keys and the tuple values,
     are in the same order as in the `dependencies` argument.
```

### Comparing `momotor-engine-options-2.0.0rc9/src/momotor/options/doc.py` & `momotor_engine_options-2.0.1/src/momotor/options/doc.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc9/src/momotor/options/domain/scheduler/preflight.py` & `momotor_engine_options-2.0.1/src/momotor/options/domain/scheduler/preflight.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,18 +40,19 @@
         A preflight check handled by the scheduler. This allows recipes to indicate situations in which the
         checklet does not have to be executed.
         
         The expected format for the option value is: 
         
         .. productionlist:: preflight-option
            preflight_option: [ `~selector:selector` ] "{ACTION_SEPARATOR}" [ `preflight_status` | `preflight_props` ]
-           preflight_status: free text status message
-           preflight_props: "{{" `prop` ":" `value` [ "," `prop` ":" `value` ]* "}}"
-           action: "run" | "pass" | "pass-secret" | "pass-hidden" | "fail" | "fail-secret" | "fail-hidden" | "skip" 
-                   | "error" | "skip-error"
+           preflight_status: text status message
+           preflight_props: "{{" `prop` ":" `value` ( "," `prop` ":" `value` )* "}}"
+           action: "run" | "pass" | "pass-secret" | "pass-hidden" 
+                 : | "fail" | "fail-secret" | "fail-hidden" | "skip" 
+                 : | "error" | "skip-error"
         
         If a :ref:`selector <selector>` matches or is empty, a results bundle based on the action and status message 
         is created (unless the action is :token:`run <preflight-option:action>`). 
         If no selectors match, or a selector matches with action :token:`run <preflight-option:action>`, 
         no result is created and the step should execute as normal.
                          
         Possible values for :token:`~preflight-option:action` are:
@@ -120,15 +121,15 @@
 
 # Properties for the 'skip-error' action
 SKIP_ERROR_PROPERTIES = {
     **SKIP_PROPERTIES,
     'deps-error': True,
 }
 
-ActionType: TypeAlias = tuple[Outcome, typing.Dict]
+ActionType: TypeAlias = tuple[Outcome, dict]
 
 PREFLIGHT_ACTIONS: dict[str, ActionType | None] = {
     'run': None,
     'pass': (Outcome.PASS, {}),
     'pass-secret': (Outcome.PASS, SECRET_PROPERTIES),
     'pass-hidden': (Outcome.PASS, HIDDEN_PROPERTIES),
     'fail': (Outcome.FAIL, {}),
```

### Comparing `momotor-engine-options-2.0.0rc9/src/momotor/options/domain/scheduler/tasks.py` & `momotor_engine_options-2.0.1/src/momotor/options/domain/scheduler/tasks.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc9/src/momotor/options/domain/scheduler/tools.py` & `momotor_engine_options-2.0.1/src/momotor/options/domain/scheduler/tools.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc9/src/momotor/options/domain/tools/__init__.py` & `momotor_engine_options-2.0.1/src/momotor/options/domain/tools/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import collections.abc
 import logging
 import typing
 from dataclasses import dataclass
 from textwrap import dedent
 
 from momotor.options.doc import annotate_docstring
 from momotor.options.option import OptionDefinition, OptionNameDomain
@@ -12,15 +13,15 @@
 from momotor.options.split import multi_split
 from momotor.options.tools import ToolName, Tool, resolve_tool
 from momotor.options.types import SubDomainDefinitionType
 from ._domain import DOMAIN as TOOLS_DOMAIN
 
 if typing.TYPE_CHECKING:
     from os import PathLike
-    PathList = typing.Optional[typing.Iterable[typing.Union[str, PathLike]]]
+    PathList = typing.Optional[collections.abc.Iterable[typing.Union[str, PathLike]]]
 
 
 __all__ = ['ToolOptionDefinition', 'ToolOptionName', 'TOOLS_DOMAIN']
 
 
 logger = logging.getLogger(__name__)
 
@@ -97,15 +98,15 @@
                 """)
             )
 
     def resolve(
             self,
             providers: Providers,
             subdomains: SubDomainDefinitionType | bool | None = None
-    ) -> typing.Iterable[ToolName]:
+    ) -> collections.abc.Iterable[ToolName]:
         result = super().resolve(providers, subdomains)
         if result is None:
             raise FileNotFoundError
 
         if isinstance(result, bytes):
             result = result.decode('utf-8', errors='replace')
```

### Comparing `momotor-engine-options-2.0.0rc9/src/momotor/options/exception.py` & `momotor_engine_options-2.0.1/src/momotor/options/exception.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc9/src/momotor/options/filter_files.py` & `momotor_engine_options-2.0.1/src/momotor/options/filter_files.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-import typing
+import collections.abc
 from momotor.bundles.elements.files import FilesType, File
 from momotor.bundles.utils.filters import F
 
 __all__ = ["filter_files", "ifilter_files"]
 
 
-def file_class_name_filters(class_name) -> typing.Iterable[F]:
+def file_class_name_filters(class_name) -> collections.abc.Iterable[F]:
     if '#' in class_name:
         class_, name = class_name.split('#', 1)
     else:
         class_, name = class_name, None
 
     if name:
         yield F(name__glob=name.strip())
@@ -29,15 +29,15 @@
     :param files: List of files to filter
     :param class_name: class/name to filter on
     :return:
     """
     return files.filter(*file_class_name_filters(class_name))
 
 
-def ifilter_files(files: FilesType, class_name: str) -> typing.Iterable[File]:
+def ifilter_files(files: FilesType, class_name: str) -> collections.abc.Iterable[File]:
     """ Return an iterable that filters a :py:class:`~momotor.bundles.utils.filters.FilterableTuple` of
     :py:class:`~momotor.bundles.elements.files.File` objects on the `name` and `class`
     attributes.
 
     The `class_name` argument contains the class and name to filter on, in the format
     `<class>`\ ``#``\ `<name>`. The `name` part can contain wildcards, and is optional.
```

### Comparing `momotor-engine-options-2.0.0rc9/src/momotor/options/option.py` & `momotor_engine_options-2.0.1/src/momotor/options/option.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import collections.abc
 import dataclasses
 import logging
 import typing
 import warnings
 from dataclasses import dataclass
 
 from momotor.bundles.elements.content import NoContent
@@ -31,15 +32,15 @@
 
     # Legacy type names
     'str': str,
     'bool': bool,
     'int': int,
 }
 
-OPTION_TYPE_CAST_MAP: dict[OptionTypeLiteral | OptionDeprecatedTypeLiteral, typing.Callable] = {
+OPTION_TYPE_CAST_MAP: dict[OptionTypeLiteral | OptionDeprecatedTypeLiteral, collections.abc.Callable] = {
     **OPTION_TYPE_MAP,
     'boolean': to_bool,
 
     # Legacy type names
     'bool': to_bool,
 }
 
@@ -138,15 +139,15 @@
     #: Has no effect when :py:attr:`.multiple` is False.
     all: bool = False
 
     #: The names and order of the providers :py:meth:`.resolve` looks for the options. Can be provided as a
     #: comma separated string, or as a sequence of strings. Required.
     #: :py:class:`~mtrchk.org.momotor.base.checklet.meta.CheckletBaseMeta` provides the default.
     #: When accessing, will always be a sequence
-    location: str | typing.Sequence[str] | None = None
+    location: str | collections.abc.Sequence[str] | None = None
 
     #: The domain of the option:
     #: Momotor defines the following values for :py:attr:`.domain`:
     #:
     #: * checklet: (Default) Options defined and used by checklets.
     #: * :ref:`scheduler <scheduler domain>`: Options used by the Momotor Broker for executing and scheduling the step.
     #: * :ref:`tools <tools domain>`: Options used by the Momotor Broker to declare tools used by the checklet.
@@ -165,15 +166,15 @@
     enable: bool = True
 
     #: If this option is deprecated, set to the reason for deprecation.
     #: Should describe which option(s) - if any - replace this option
     deprecated: str | None = None
 
     # Cast a value into the correct type for this option
-    _cast: typing.Callable[[typing.Any], typing.Any] = dataclasses.field(init=False)
+    _cast: collections.abc.Callable[[typing.Any], typing.Any] = dataclasses.field(init=False)
 
     @property
     def fullname(self) -> OptionNameDomain:
         """ Full name, including domain """
         return OptionNameDomain(self.name, self.domain)
 
     def __post_init__(self):
@@ -198,15 +199,16 @@
         elif isinstance(location, str):
             location_seq = tuple(loc.strip() for loc in location.split(','))
         else:
             location_seq = tuple(location)
 
         assert location_seq is None or set(location_seq) <= VALID_LOCATIONS
 
-        object.__setattr__(self, 'location', typing.cast(typing.Sequence[typing.Optional[LocationLiteral]], location_seq))
+        object.__setattr__(self, 'location',
+                           typing.cast(collections.abc.Sequence[typing.Optional[LocationLiteral]], location_seq))
 
         type_ = self.type
         if type_ in LEGACY_OPTION_TYPES:
             correct_type = LEGACY_OPTION_TYPES[typing.cast(OptionDeprecatedTypeLiteral, type_)]
             warnings.warn(f'Option type {type_!r} is deprecated, use {correct_type!r} instead', DeprecationWarning)
             object.__setattr__(self, 'type', correct_type)
             type_ = correct_type
@@ -245,15 +247,15 @@
 
         if self.domain is None:
             raise ValueError('domain not defined')
 
         if self.location is None:
             raise ValueError('location not defined')
 
-        def _get_loc_domain() -> typing.Generator[tuple[OptionsMixin, str], None, None]:
+        def _get_loc_domain() -> collections.abc.Generator[tuple[OptionsMixin, str], None, None]:
             # Collect pairs of (provider, domain). In order to guarantee priority for the most-specified domains, we
             # do two loops here, one for domains with subdomains, one for domains without.
             loc: LocationLiteral
 
             if subdomains:
                 for loc in self.location:
                     prov = getattr(providers, loc)
```

### Comparing `momotor-engine-options-2.0.0rc9/src/momotor/options/parser/consts.py` & `momotor_engine_options-2.0.1/src/momotor/options/parser/consts.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+import collections.abc
 import operator
 import re
 import typing
 
-from typing_extensions import TypeAlias  # Python 3.10+
-
 from momotor.options.task_id import ID_RE_STR
+from typing_extensions import TypeAlias  # Python 3.10+
 
 MOD_RE = re.compile(
     r"^\s*"
     r"(?:%(?P<mod>[\w-]+))?"
 )
 
 VALUE_ATTR: dict[typing.Optional[str], str] = {
@@ -36,15 +36,15 @@
     r')?'
     r'\s*'
     r'(?:'
         r':\s*(?P<name>(?:[^\'",\s]+|"[^"]*"|\'[^\']*\')*)'
     r')?'
 )
 
-OperatorCallable: TypeAlias = typing.Callable[[typing.Any, typing.Any], bool]
+OperatorCallable: TypeAlias = collections.abc.Callable[[typing.Any, typing.Any], bool]
 
 # All operators and functions to check them
 OPERATIONS: dict[typing.Optional[str], OperatorCallable] = {
     None: lambda prop_value, value: True,
     '?': lambda prop_value, value: bool(prop_value),
     '!': lambda prop_value, value: not bool(prop_value),
     '==': operator.eq,
```

### Comparing `momotor-engine-options-2.0.0rc9/src/momotor/options/parser/keyvalue.py` & `momotor_engine_options-2.0.1/src/momotor/options/parser/keyvalue.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
-import typing
+import collections.abc
 
 
-def parse_key_value_list(s: str) -> typing.Generator[typing.Tuple[str, str | int | float | bool | None], None, None]:
+def parse_key_value_list(s: str) \
+        -> collections.abc.Generator[tuple[str, str | int | float | bool | None], None, None]:
     """
     Parse a string of key=value pairs into a sequence of (key, value) pairs.
 
     Value can be a string, integer, float or boolean. If value needs to contain spaces, it must be quoted.
 
     If the value is empty, but the `=` is present, the value will be `None`.
     A single key (without `=`) will result in a value of `True`
```

### Comparing `momotor-engine-options-2.0.0rc9/src/momotor/options/parser/modifier.py` & `momotor_engine_options-2.0.1/src/momotor/options/parser/modifier.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
     A modifier converts a list of values into a single value
 """
 from __future__ import annotations
 
+import collections.abc
 import json
 import typing
 
 from momotor.options.parser.consts import MOD_RE
 
 
 def parse_mod(modded_ref: str) -> tuple[str | None, str]:
@@ -37,21 +38,21 @@
         mod = m_mod.group('mod')
         if mod:
             return mod, modded_ref[m_mod.end(m_mod.lastindex):].strip()
 
     return None, modded_ref
 
 
-def exclude_none(values: typing.Iterable[typing.Any]) -> typing.Generator[typing.Any, None, None]:
+def exclude_none(values: collections.abc.Iterable[typing.Any]) -> collections.abc.Generator[typing.Any, None, None]:
     for v in values:
         if v is not None:
             yield v
 
 
-def cast_number(values: typing.Iterable[typing.Any]) -> typing.Generator[int | float, None, None]:
+def cast_number(values: collections.abc.Iterable[typing.Any]) -> collections.abc.Generator[int | float, None, None]:
     for v in values:
         if v is None:
             continue
 
         if isinstance(v, (int, float)):
             yield v
         else:
@@ -70,16 +71,16 @@
             return '"' + value.replace('"', '\\"') + '"'
         else:
             return "'" + value + "'"
 
     return str(value)
 
 
-def none_if_empty(fn: typing.Callable[[typing.Iterable[typing.Any]], bool], values: typing.Iterable[typing.Any]) \
-        -> str | int | bool | None:
+def none_if_empty(fn: collections.abc.Callable[[collections.abc.Iterable[typing.Any]], bool],
+                  values: collections.abc.Iterable[typing.Any]) -> str | int | bool | None:
     values = list(values)
     return fn(values) if values else None
 
 
 def round_safe(value: typing.Any) -> typing.Any:
     if isinstance(value, float):
         return int(round(value))
@@ -91,15 +92,17 @@
     if isinstance(value, float):
         return int(value)
 
     return value
 
 
 # All modifiers
-COMBINER_MODIFIERS: dict[str, typing.Callable[[typing.Iterable[typing.Any]], str | int | bool | None]] = {
+COMBINER_MODIFIERS: dict[
+    str, collections.abc.Callable[[collections.abc.Iterable[typing.Any]], str | int | bool | None]
+] = {
     'all': lambda values: none_if_empty(all, values),
     'any': lambda values: none_if_empty(any, values),
     'notall': lambda values: none_if_empty(lambda v: not all(v), values),
     'not': lambda values: none_if_empty(lambda v: not any(v), values),
     'notany': lambda values: none_if_empty(lambda v: not any(v), values),
     'sum': lambda values: none_if_empty(sum, cast_number(values)),
     'sumr': lambda values: round_safe(none_if_empty(sum, cast_number(values))),
@@ -114,15 +117,15 @@
     'json': lambda values: json.dumps(list(values) if len(values) > 1 else (values[0] if len(values) == 1 else None),
                                       separators=(',', ':')),
     'first': lambda values: list(exclude_none(values))[0],
     'last': lambda values: list(exclude_none(values))[-1],
 }
 
 
-def apply_combiner_modifier(mod: str, values: typing.Sequence[str | int | float | bool]) \
+def apply_combiner_modifier(mod: str, values: collections.abc.Sequence[str | int | float | bool]) \
         -> str | int | float | bool | None:
 
     try:
         mod_fn = COMBINER_MODIFIERS[mod]
     except KeyError:
         raise ValueError(f"invalid modifier {mod!r}")
```

### Comparing `momotor-engine-options-2.0.0rc9/src/momotor/options/parser/placeholders.py` & `momotor_engine_options-2.0.1/src/momotor/options/parser/placeholders.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from __future__ import annotations
 
+import collections.abc
 import typing
 
 from momotor.options.providers import Providers
 from momotor.options.parser.reference import resolve_reference_value
 
 
 VT = typing.TypeVar('VT')
 
 
 def replace_placeholders(
     value: VT, bundles: Providers, *,
-    value_processor: typing.Callable[[str | None], str] = None,
+    value_processor: collections.abc.Callable[[str | None], str] = None,
     mod: str = 'join'
 ) -> VT:
     """ Replace all :ref:`placeholders <placeholder>` in `value` with their resolved values.
     Placeholders are resolved recursively, i.e. if a resolved value contains more placeholders,
     these will be resolved as well.
 
     :param value: the string containing placeholders to resolve. If :py:attr:`value` is not a string,
```

### Comparing `momotor-engine-options-2.0.0rc9/src/momotor/options/parser/reference.py` & `momotor_engine_options-2.0.1/src/momotor/options/parser/reference.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,15 +182,15 @@
     # provider = m_provider.group('provider')
     # if provider:
     #     remaining = ref_option[m_provider.end(m_provider.lastindex):]
     # else:
     #     remaining = ref_option
 
     remaining = (ref_option or '').strip()
-    refs: typing.MutableSequence[Reference] = collections.deque()
+    refs: collections.abc.MutableSequence[Reference] = collections.deque()
     any_options = False
     while remaining.strip():
         m_ref = REF_OPTION_RE.match(remaining)
         if not m_ref:
             break
 
         provider = m_ref.group('provider') or None
@@ -257,16 +257,16 @@
     refs, ref_remainder = _split_options(ref_option)
     if ref_remainder and ref_remainder.strip():
         raise ValueError(f"Invalid reference {reference.strip()}")
 
     return type_, refs, remainder
 
 
-# def _resolve_id_references(objects: typing.Mapping, refs: typing.Sequence[Reference]) \
-#         -> typing.Generator[tuple[typing.Any, Reference | None], None, None]:
+# def _resolve_id_references(objects: collections.abc.Mapping, refs: collections.abc.Sequence[Reference]) \
+#         -> collections.abc.Generator[tuple[typing.Any, Reference | None], None, None]:
 #
 #     if not refs:
 #         for obj in objects.values():
 #             yield obj, None
 #
 #     for ref in refs:
 #         if ref.id:
@@ -350,16 +350,16 @@
         name, domain = nd.split('@', 1)
     else:
         name, domain = nd, None
 
     return name, domain
 
 
-def _match_result_reference(type_: str, objects: typing.Iterable[tuple[Result, Reference]]) \
-        -> typing.Generator[ReferenceMatch, None, None]:
+def _match_result_reference(type_: str, objects: collections.abc.Iterable[tuple[Result, Reference]]) \
+        -> collections.abc.Generator[ReferenceMatch, None, None]:
     """ A generator to generate :py:class:`ReferenceMatch` objects for result and outcome references
 
     :param type_: The :token:`~reference:type`
     :param objects:
     :raises ValueError: the reference is invalid
     """
     type_ = type_.strip()
@@ -391,17 +391,17 @@
             )
 
         result = (obj,) if _test(obj) else tuple()
         yield ReferenceMatch(obj, result)
 
 
 def _match_prop_reference(
-        objects: typing.Iterable[tuple[typing.Union[ProviderElement, PropertiesMixin], Reference]],
+        objects: collections.abc.Iterable[tuple[typing.Union[ProviderElement, PropertiesMixin], Reference]],
         task_id: StepTaskId | None = None
-) -> typing.Generator[ReferenceMatch, None, None]:
+) -> collections.abc.Generator[ReferenceMatch, None, None]:
 
     for obj, ref in objects:
         if ref is None:
             raise ValueError("a name is required")
         elif ref.name is None:
             # noinspection PyProtectedMember
             raise ValueError(
@@ -417,17 +417,17 @@
                 raise ValueError(f"{ref._source!r} is not valid, {e!s}")
 
         properties = obj.properties.filter(name=name)
         yield ReferenceMatch(obj, properties)
 
 
 def _match_file_reference(
-        objects: typing.Iterable[tuple[typing.Union[ProviderElement, FilesMixin], Reference]],
+        objects: collections.abc.Iterable[tuple[typing.Union[ProviderElement, FilesMixin], Reference]],
         task_id: StepTaskId | None = None
-) -> typing.Generator[ReferenceMatch, None, None]:
+) -> collections.abc.Generator[ReferenceMatch, None, None]:
 
     for obj, ref in objects:
         files = obj.files
         if ref and ref.name:
             class_, name = _split_name_class(ref.name)
             if task_id:
                 if class_:
@@ -452,17 +452,17 @@
 
             files = files.filter(**filters)
 
         yield ReferenceMatch(obj, files)
 
 
 def _match_opt_reference(
-        objects: typing.Iterable[tuple[typing.Union[ProviderElement, OptionsMixin], Reference]],
+        objects: collections.abc.Iterable[tuple[typing.Union[ProviderElement, OptionsMixin], Reference]],
         task_id: StepTaskId
-) -> typing.Generator[ReferenceMatch, None, None]:
+) -> collections.abc.Generator[ReferenceMatch, None, None]:
 
     for obj, ref in objects:
         if ref is None:
             raise ValueError("a name is required")
         elif ref.name is None:
             # noinspection PyProtectedMember
             raise ValueError(
@@ -493,16 +493,16 @@
     None: ('result', {'result'}),
     'prop': ('result', {'result'}),
     'file': (None, None),
     'opt': (None, None),
 }
 
 
-def _get_bundle_objects(type_: str, refs: typing.Sequence[Reference], bundles: Providers) \
-        -> typing.Generator[tuple[ProviderElement, Reference], None, None]:
+def _get_bundle_objects(type_: str, refs: collections.abc.Sequence[Reference], bundles: Providers) \
+        -> collections.abc.Generator[tuple[ProviderElement, Reference], None, None]:
     type_ = type_.strip()
 
     if type_ in DEFAULT_VALID_PROVIDERS:
         default_provider, valid_providers = DEFAULT_VALID_PROVIDERS[type_]
     else:
         default_provider, valid_providers = DEFAULT_VALID_PROVIDERS[None]
 
@@ -549,16 +549,16 @@
                 if query_fn(result):
                     yield result, ref
 
         else:
             raise ValueError(f"invalid provider {provider!r}")
 
 
-def generate_reference(type_: str, refs: typing.Sequence[Reference], bundles: Providers) \
-        -> typing.Generator[ReferenceMatch, None, None]:
+def generate_reference(type_: str, refs: collections.abc.Sequence[Reference], bundles: Providers) \
+        -> collections.abc.Generator[ReferenceMatch, None, None]:
     """ A generator producing reference matches.
 
     Each :py:class:`ReferenceMatch` object generated is a single reference resolved.
 
     :param type_: The reference :token:`~reference:type`
     :param refs: The reference options
     :param bundles: The bundles to resolve the references too
```

### Comparing `momotor-engine-options-2.0.0rc9/src/momotor/options/parser/selector.py` & `momotor_engine_options-2.0.1/src/momotor/options/parser/selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import collections
-import typing
+import collections.abc
 
 from momotor.bundles.elements.base import Element
 from momotor.options.parser.modifier import parse_mod
 from momotor.options.parser.reference import parse_reference, generate_reference, Reference, ReferenceMatch
 from momotor.options.parser.consts import VALUE_ATTR, OPERATIONS, OPERATIONS_WITHOUT_VALUE, CONDITION_RE, \
     OperatorCallable
 from momotor.options.providers import Providers
@@ -117,15 +117,15 @@
 
     return type_, refs, oper, value, remainder
 
 
 def resolve_selector(selector: str, bundles: Providers) \
         -> tuple[
             str,
-            typing.Iterable[ReferenceMatch],
+            collections.abc.Iterable[ReferenceMatch],
             OperatorCallable,
             str | int | float | None,
             str
         ]:
     """ Resolve all parts of a :ref:`selector <selector>`
 
     :param selector: the :token:`~selector:selector` to parse
@@ -160,15 +160,15 @@
     :return: a 2-tuple containing
              a tuple with the selected elements, and
              a string with the rest of the `selector` string remaining after parsing.
     :raises ValueError: if the selector is not valid
     """
     attr, matches, oper, value, remainder = resolve_selector(selector.strip(), bundles)
 
-    results: typing.MutableSequence[Element] = collections.deque()
+    results: collections.abc.MutableSequence[Element] = collections.deque()
     for match in matches:
         obj_values = [getattr(mv, attr, None) for mv in match.values]
         for obj_value in obj_values:
             if oper(obj_value, value):
                 results.append(match.provider)
                 break
```

### Comparing `momotor-engine-options-2.0.0rc9/src/momotor/options/parser/tasks.py` & `momotor_engine_options-2.0.1/src/momotor/options/parser/tasks.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc9/src/momotor/options/providers.py` & `momotor_engine_options-2.0.1/src/momotor/options/providers.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc9/src/momotor/options/result_query.py` & `momotor_engine_options-2.0.1/src/momotor/options/result_query.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """ Methods for querying and filtering results
 """
 
+import collections.abc
 import re
-import typing
 from collections import deque
 
 from momotor.bundles.elements.result import Result
 from momotor.options.task_id import StepTaskId, apply_task_number
 
 
-def make_result_id_re(query: str) -> "typing.re.Pattern":
+def make_result_id_re(query: str) -> re.Pattern:
     """ Make a regex that matches a :ref:`result query <result query>` to the query.
 
     Uses a glob-like pattern matching on the dot-separated elements of the selector.
     For the first element (the step-id part), a ``*`` will match zero or more characters except ``.``
     For all the other elements (the task number parts), a ``*`` matches one or more elements starting at that position
     and a ``?`` matches a single element in that position.
 
@@ -136,15 +136,15 @@
             first = False
 
         regex = r'^' + r'\.'.join(regex_parts) + r'$'
 
     return re.compile(regex)
 
 
-def result_query_fn(query: str, task_id: StepTaskId = None) -> typing.Callable[[Result], bool]:
+def result_query_fn(query: str, task_id: StepTaskId = None) -> collections.abc.Callable[[Result], bool]:
     """ Make a function to match a result with a :ref:`result query <result query>`.
 
     The query is either a literal id (e.g. ``step``, ``step.1`` etc), or a glob-like query to select
     multiple id's, (e.g. ``*``, ``step.*``, ``step.?``). Also applies task numbers if `task_id` is provided.
 
     Multiple queries are possible, separated with a comma.
 
@@ -188,16 +188,16 @@
 
     def _match(result: Result) -> bool:
         return any(fn(result.step_id) for fn in fns)
 
     return _match
 
 
-def filter_result_query(results: typing.Iterable[Result], query: str, task_id: StepTaskId = None) \
-        -> typing.Iterator[Result]:
+def filter_result_query(results: collections.abc.Iterable[Result], query: str, task_id: StepTaskId = None) \
+        -> collections.abc.Iterator[Result]:
     """ Filter an iterable of :py:class:`~momotor.bundles.elements.result.Result` objects on a
     :ref:`result query <result query>`
 
     Returns an iterator that iterates all the :py:class:`~momotor.bundles.elements.result.Result` objects
     from `results` that match the `query`
 
     :param results: an iterable with the results to query
```

### Comparing `momotor-engine-options-2.0.0rc9/src/momotor/options/sphinx/fixextref.py` & `momotor_engine_options-2.0.1/src/momotor/options/sphinx/fixextref.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc9/src/momotor/options/sphinx/option.py` & `momotor_engine_options-2.0.1/src/momotor/options/sphinx/option.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """ Sphinx extension for documenting checklet option definitions. """
 from __future__ import annotations
 
+import collections.abc
 import textwrap
 import typing
 
 from momotor.bundles.elements.options import Option
 from momotor.options import OptionDefinition, OptionNameDomain
 
 try:
@@ -48,31 +49,47 @@
             qualsig = sig
             sig = sig.split('@')[0]
         else:
             qualsig = sig
 
         return sig, qualsig
 
+    def format_value(typ: str | None, value: typing.Any) -> str:
+        if typ in {'bool', 'boolean'} or isinstance(value, bool):
+            return repr(value)
+        elif typ in {'str', 'string'} or isinstance(value, str):
+            if value:
+                return f'``{value}``'
+            else:
+                return '*Empty string*'
+
+        return repr(value)
+
     def document_option_definition(
-            option: OptionDefinition, tab_width: int = 8, *,
+            option: OptionDefinition, tab_width: int = 8, style: str = 'checklet', *,
             checklet: str | None = None,
             canonical: str | None = None,
             step: str | None = None,
             no_index_entry: bool = False,
             no_contents_entry: bool = False,
-    ) -> typing.Generator[str, None, None]:
+            values: list[typing.Any] | None = None,
+            default: typing.Any = OptionDefinition.NO_DEFAULT,
+    ) -> collections.abc.Generator[str, None, None]:
         """ Generate a reStructuredText description for the given option definition.
 
         :param option: The option definition to document.
         :param tab_width: The tab width to use for indentation.
+        :param style: The style to use for the option ('checklet' or 'step').
         :param no_index_entry: Whether to suppress the index entry for this option.
         :param no_contents_entry: Whether to suppress the contents entry for this option.
         :param checklet: The checklet name (full path including module) to use for the option.
         :param canonical: The canonical checklet (full path including module) that defines this option.
         :param step: The step name to use for the option.
+        :param values: The values to use for the option. If provided, the option's default value is ignored.
+        :param default: Alternate default value to use for the option. Overrides the option's default value.
         :return: A generator yielding the lines of the reStructuredText description.
         """
         yield f'.. momotor:option:: {option.fullname}'
 
         if checklet:
             yield f'   :checklet: {checklet}'
         if canonical:
@@ -99,29 +116,36 @@
         if option.doc is not None:
             for line in prepare_docstring(option.doc, tab_width):
                 yield f'   {line}'
 
         yield f'   :type: {"Any" if option.type is None else option.type}'
         yield f'   :required: {option.required!r}'
         yield f'   :multiple: {option.multiple!r}'
-        yield f'   :all: {option.all!r}'
-        yield f'   :location: {", ".join(option.location)}'
-
-        default = option.default
-        if default is option.NO_DEFAULT:
-            yield f'   :default: *No default*'
-        elif option.type in {'bool', 'boolean'} or isinstance(default, bool):
-            yield f'   :default: {default!r}'
-        elif option.type in {'str', 'string'} or isinstance(default, str):
-            if default:
-                yield f'   :default: ``{default}``'
+        if option.multiple:
+            yield f'   :all: {option.all!r}'
+        if style == 'checklet':
+            yield f'   :location: {", ".join(option.location)}'
+
+        if values is not None:
+            if len(values) == 0:
+                yield '   :value: *No values*'
+            elif len(values) == 1:
+                yield '   :value: ' + format_value(option.type, values[0])
             else:
-                yield f'   :default: *Empty string*'
+                yield '   :value:'
+                for value in values:
+                    yield f'      - {format_value(option.type, value)}'
         else:
-            yield f'   :default: {default!r}'
+            if default is OptionDefinition.NO_DEFAULT:
+                default = option.default
+
+            if default is OptionDefinition.NO_DEFAULT:
+                yield '   :default: *No default*'
+            else:
+                yield '   :default: ' + format_value(option.type, default)
 
         yield ''
 
     def parse_rst(rst: str, state: RSTState) -> list[nodes.Node]:
         vl = ViewList(textwrap.dedent(rst).splitlines(), source='')
         node = nodes.paragraph()
         # noinspection PyTypeChecker
@@ -338,15 +362,15 @@
                     # duplicated
                     logger.warning('duplicate object description of %s, '
                                    'other instance in %s, use :no-index: for one of them',
                                    name, other.docname, location=location)
 
             self.objects[name] = ObjectEntry(self.env.docname, node_id, objtype, aliased)
 
-        def get_objects(self) -> typing.Iterator[tuple[str, str, str, str, str, int]]:
+        def get_objects(self) -> collections.abc.Iterator[tuple[str, str, str, str, str, int]]:
             for refname, obj in self.objects.items():
                 yield refname, refname, obj.objtype, obj.docname, obj.node_id, (-1 if obj.aliased else 1)
 
         def resolve_xref(self, env, fromdocname, builder, typ, target, node, contnode) -> nodes.reference | None:
             if typ == 'option':
                 target = qualified_option_sig(target)[1]  # option refs are always qualified with domain
                 targets = [target]
```

### Comparing `momotor-engine-options-2.0.0rc9/src/momotor/options/split.py` & `momotor_engine_options-2.0.1/src/momotor/options/split.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+import collections.abc
 import re
-import typing
 
 
-def multi_split(s: str, extra_sep: typing.Iterable = None, maxsplit: int = 0) -> typing.Iterable[str]:
+def multi_split(s: str, extra_sep: collections.abc.Iterable = None, maxsplit: int = 0) -> collections.abc.Iterable[str]:
     """ Split a string on multiple separators.
 
     Only splits on whitespace by default, but `extra_sep` can provide other separators to split the string on.
     If `maxsplit` is nonzero, at most maxsplit splits occur, and the remainder of the string is returned as the
     final element.
 
     :param s: string to process
```

### Comparing `momotor-engine-options-2.0.0rc9/src/momotor/options/task_id.py` & `momotor_engine_options-2.0.1/src/momotor/options/task_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 """ Methods to handle task id's
 """
 from __future__ import annotations
 
+import collections.abc
+import itertools
 import operator
 import re
 from collections import deque
-
-import itertools
-import typing
 from dataclasses import dataclass
 
 from momotor.options.exception import InvalidDependencies
 from momotor.options.types import StepTasksType, StepTaskNumberType
 
-TASK_OPERATORS: dict[str, typing.Callable[[int, int], int]] = {
+TASK_OPERATORS: dict[str, collections.abc.Callable[[int, int], int]] = {
     '+': operator.add,
     '-': operator.sub,
     '*': operator.mul,
     '/': operator.floordiv,
     '%': operator.mod,
 }
 TASK_OPER_RE_STR = "|".join(re.escape(oper) for oper in TASK_OPERATORS.keys())
 TASK_OPER_RE = re.compile(rf'({TASK_OPER_RE_STR})')
 TASK_REF_RE = re.compile(rf'(\\?\$(?:@|(?:\d+(?:(?<!\\)(?:{TASK_OPER_RE_STR})\$?\d+)*)))')
 
 ID_RE_STR = rf'(?:[\w.$@]|{TASK_OPER_RE_STR})+'
 
 
-def task_id_from_number(task_number: typing.Iterable[int] | None) -> str:
+def task_id_from_number(task_number: collections.abc.Iterable[int] | None) -> str:
     """ Convert a task number (tuple of ints) into a task id (dotted string)
 
     >>> task_id_from_number(None)
     ''
 
     >>> task_id_from_number((1,))
     '1'
@@ -74,15 +73,15 @@
     def __str__(self):
         if self.task_number:
             return self.step_id + '.' + task_id_from_number(self.task_number)
         else:
             return self.step_id
 
 
-def iter_task_numbers(sub_tasks: StepTasksType) -> typing.Generator[StepTaskNumberType, None, None]:
+def iter_task_numbers(sub_tasks: StepTasksType) -> collections.abc.Generator[StepTaskNumberType, None, None]:
     """ Generate all the task-numbers for the subtasks.
 
     >>> list(iter_task_numbers(tuple()))
     [None]
 
     >>> list(iter_task_numbers((1,)))
     [(0,)]
@@ -101,15 +100,15 @@
     """
     if sub_tasks:
         yield from itertools.product(*(range(st) for st in sub_tasks))
     else:
         yield None
 
 
-def iter_task_ids(step_id: str, sub_tasks: StepTasksType) -> typing.Generator[StepTaskId, None, None]:
+def iter_task_ids(step_id: str, sub_tasks: StepTasksType) -> collections.abc.Generator[StepTaskId, None, None]:
     """ Generate all the task-ids for the subtasks.
 
     >>> list(str(t) for t in iter_task_ids('step', tuple()))
     ['step']
 
     >>> list(str(t) for t in iter_task_ids('step', (2,)))
     ['step.0', 'step.1']
@@ -121,15 +120,15 @@
     :param sub_tasks: sequence of integers with the number of sub-tasks for each level
     :return: the task numbers
     """
     for task_number in iter_task_numbers(sub_tasks):
         yield StepTaskId(step_id, task_number)
 
 
-def get_task_id_lookup(task_ids: typing.Iterable[StepTaskId]) -> dict[str, StepTaskId]:
+def get_task_id_lookup(task_ids: collections.abc.Iterable[StepTaskId]) -> dict[str, StepTaskId]:
     """ Convert an iterable of :py:const:`StepTaskId` objects into a lookup table to convert a string representation of
     a task-id to the :py:const:`StepTaskId`
 
     >>> get_task_id_lookup({StepTaskId('step', (0, 0))})
     {'step.0.0': StepTaskId(step_id='step', task_number=(0, 0))}
 
     :param task_ids: the task ids to convert
```

### Comparing `momotor-engine-options-2.0.0rc9/src/momotor/options/tools/__init__.py` & `momotor_engine_options-2.0.1/src/momotor/options/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc9/src/momotor/options/tools/registry.py` & `momotor_engine_options-2.0.1/src/momotor/options/tools/registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import collections.abc
 import functools
 import logging
 import os
 import pathlib
 import textwrap
 import typing
 
@@ -18,15 +19,15 @@
 
 TOOL_REGISTRY_ENVNAME = 'TOOLREGISTRY'
 DEFAULT_TOOL_REGISTRY_LOCATION = ['~/.toolregistry.d', '/etc/toolregistry.d']
 
 logger = logging.getLogger(__name__)
 
 
-def need_posix(f: typing.Callable) -> typing.Callable:
+def need_posix(f: collections.abc.Callable) -> collections.abc.Callable:
     """ Decorator that will throw an assertion error if the current system is not a Posix system
     """
     @functools.wraps(f)
     def wrapper(*args, **kwargs):
         assert os.name == 'posix', 'Tool registry only supported on Posix systems'
         return f(*args, **kwargs)
 
@@ -36,15 +37,16 @@
     else:
         doc = ''
 
     wrapper.__doc__ = doc + '*Only available on Posix systems, does not work on Windows*'
     return wrapper
 
 
-def tool_registry_paths(paths: "PathList" = None, include_default_paths: bool = True) -> typing.Iterable[pathlib.Path]:
+def tool_registry_paths(paths: "PathList" = None, include_default_paths: bool = True) \
+        -> collections.abc.Iterable[pathlib.Path]:
     """ Collect the tool registry paths
     """
     paths = list(paths) if paths is not None else list()
 
     if include_default_paths:
         tool_registry: str = os.environ.get(TOOL_REGISTRY_ENVNAME)
         if tool_registry:
@@ -121,16 +123,16 @@
         paths: "PathList" = None, *,
         include_default_paths: bool = True,
         include_missing: bool = False,
 ) -> dict[ToolName, Tool]:
     """
     Return a mapping with all locally installed tools.
 
-    If `include_default_paths` is True (default), this reads the tool registry from `.toolregistry.d` in
-    the current user's home directory and `/etc/toolregistry.d`. If `paths` is provided, registry will be read from
+    If **include_default_paths** is `True` (default), this reads the tool registry from `.toolregistry.d` in
+    the current user's home directory and `/etc/toolregistry.d`. If **paths** is provided, registry will be read from
     all paths in the path list as well.
 
     :param paths: paths to read the tool registry from. prepended to the default paths
     :param include_default_paths: include the default paths
     :param include_missing: include tools that are registered but the executable does not actually exist
     :return: a mapping from tool name to tool dataclass
     """
@@ -141,18 +143,18 @@
         include_missing=include_missing,
     )
 
 
 @need_posix
 def resolve_tool(name: "StrPathOrToolName", *, paths: "PathList" = None, include_default_paths: bool = True) -> Tool:
     """
-    Resolve a tool `name` to a :py:class:`Tool` dataclass.
+    Resolve a tool **name** to a :py:class:`~momotor.options.tools.tool.Tool` dataclass.
 
-    If `include_default_paths` is True (default), this reads the tool registry from `.toolregistry.d` in
-    the current user's home directory and `/etc/toolregistry.d`. If `paths` is provided, registry will be read from
+    If **include_default_paths** is `True` (default), this reads the tool registry from `.toolregistry.d` in
+    the current user's home directory and `/etc/toolregistry.d`. If **paths** is provided, registry will be read from
     all paths in the path list as well.
 
     :param name: Name of the tool to resolve
     :param paths: paths to read the tool registry from. prepended to the default paths
     :param include_default_paths: include the default paths
     :return: The tool info object.
     :raises FileNotFoundError: if the name could not be resolved
```

### Comparing `momotor-engine-options-2.0.0rc9/src/momotor/options/tools/tool.py` & `momotor_engine_options-2.0.1/src/momotor/options/tools/tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import collections
+import collections.abc
 import dataclasses
 import functools
 import logging
 import os
 import pathlib
 import typing
 from string import Template
@@ -90,15 +91,15 @@
     @classmethod
     def factory(cls: type[TN], name: typing.Union["StrPathOrToolName", ToolVersion],
                 *parts: str | ToolVersion) -> TN:
         """ Helper factory to create a :py:class:`ToolName` from a :py:class:`str`, :py:class:`pathlib.PurePath`,
         another :py:class:`ToolName`, or a sequence of :py:class:`str` or
         :py:class:`~momotor.options.tools.version.ToolVersion` elements.
 
-        If `name` is a :py:class:`ToolName`, returns `name` unmodified, otherwise instantiates
+        If **name** is a :py:class:`ToolName`, returns **name** unmodified, otherwise instantiates
         a new :py:class:`ToolName` object for the given name.
         """
         if parts or isinstance(name, ToolVersion) or (isinstance(name, str) and cls.SEPARATOR not in name):
             if not isinstance(name, (ToolVersion, str)):
                 raise TypeError
             return cls(cls.SEPARATOR.join([str(name)] + [str(part) for part in parts]))
         elif isinstance(name, cls):
@@ -134,16 +135,16 @@
                 other_versions += padding
             else:
                 self_versions += padding
 
         return self_versions, other_versions
 
     def is_partial(self, other: "StrPathOrToolName") -> bool:
-        """ Checks if all elements of :py:attr:`self.versions` are the same or a partial version of
-        :py:attr:`other.versions`.
+        """ Checks if all elements of :py:attr:`self.versions <versions>` are the same or a partial version of
+        :py:attr:`other.versions <versions>`.
 
         >>> ToolName('test').is_partial(ToolName('test/1.0'))
         True
 
         >>> ToolName('test/1').is_partial(ToolName('test/1.0'))
         True
 
@@ -188,25 +189,26 @@
     """ Data class representing the contents of a tool registry file.
     """
 
     #: Canonical name of the tool after resolving soft links
     name: ToolName
 
     #: Environment variables for the tool as indicated by the tool file
-    environment: typing.Mapping[str, str]
+    environment: collections.abc.Mapping[str, str]
 
     #: Path to the tool as indicated by the tool file
     path: pathlib.Path
 
     # Cached `path.exists`
     _exists_cache: bool = dataclasses.field(init=False, hash=False, default=None)
 
     @classmethod
     def from_file_factory(cls, registry_path: pathlib.Path, tool_file_path: pathlib.PurePath) -> "Tool":
-        """ Read a tool definition file and return a populated :py:class:`Tool` dataclass.
+        """ Read a :ref:`tool registry file <tool registry file>` file and return a populated :py:class:`Tool`
+        dataclass.
 
         :param registry_path: path to the registry
         :param tool_file_path: path to the tool file, relative to `registry_path`
         :return: the tool
         """
         path = registry_path / tool_file_path
         tool_name = ToolName(tool_file_path)
@@ -246,15 +248,15 @@
         #     logger.debug(f'tool {tool_name!r} resolved to {tool_path!s} (using {path!s})')
         #     for key, value in environment.items():
         #         logger.debug(f'tool {tool_name!r} environment {key}={value}')
 
         return cls(tool_name, environment.maps[0], tool_path)
 
     def exists(self) -> bool:
-        """ Shortcut for :py:func:`.path.exists`. Result is cached.
+        """ Shortcut for :py:meth:`path.exists() <pathlib.Path.exists>`. Result is cached.
 
         :return: `True` if the tool exists.
         """
         exists = self._exists_cache
         if exists is None:
             exists = self.path.exists()
             object.__setattr__(self, '_exists_cache', exists)
@@ -334,25 +336,25 @@
                 idx += 1
 
     return value.strip()
 
 
 def match_tool(
         name: "StrPathOrToolName",
-        tools: typing.Iterable["StrPathOrToolName"]
+        tools: collections.abc.Iterable["StrPathOrToolName"]
 ) -> typing.Optional["StrPathOrToolName"]:
     """
-    Match tool `name` with :py:const:`~~momotor.options.tools.version.ToolVersion.DEFAULT` placeholders
-    and (partial) version numbers to a tool name in the `tools` container.
+    Match tool **name** with :py:const:`~~momotor.options.tools.version.ToolVersion.DEFAULT` placeholders
+    and (partial) version numbers to a tool name in the **tools** container.
 
-    Returns the most specific matched name from `tools`, or None if no match could be made.
+    Returns the most specific matched name from **tools**, or `None` if no match could be made.
 
     :param name: Name of the tool to match
     :param tools: An iterable of tool names to match `name` against
-    :return: The matched name from `tools`, or `None`
+    :return: The matched name from **tools**, or `None`
     """
     name, best_name, best_candidate = ToolName.factory(name), None, None
     for cname in tools:
         candidate = ToolName.factory(cname)
         if name.is_partial(candidate) and (best_candidate is None or candidate > best_candidate):
             best_name, best_candidate = cname, candidate
 
@@ -360,26 +362,26 @@
 
 
 def match_tool_requirements(
         requirements: "ToolRequirements",
         toolset: "ToolSet"
 ) -> dict[str, "StrPathOrToolName"]:
     """
-    Match tools in `requirements` with tools in `tools` using :py:func:`match_tool` and return
+    Match tools in **requirements** with tools in **tools** using :py:func:`match_tool` and return
     a sequence with the most specific matched.
 
     :param requirements: tool requirements
     :param toolset: list of available tools
     :return: mapping of requirement name (key of the `requirements` mapping) to matched tool name
     :raises ValueError: when requirements cannot be fulfilled
     """
     matches: dict[str, "StrPathOrToolName"] = {}
 
     for req_name, req_tools in requirements.items():
-        match: "StrPathOrToolName" | None = None
+        match: typing.Optional["StrPathOrToolName"] = None
 
         for req_tool in req_tools:
             match = match_tool(req_tool, toolset)
             if match:
                 matches[req_name] = match
                 break
```

### Comparing `momotor-engine-options-2.0.0rc9/src/momotor/options/tools/version.py` & `momotor_engine_options-2.0.1/src/momotor/options/tools/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 @functools.total_ordering
 @dataclasses.dataclass(frozen=True, init=False)
 class ToolVersion:
     """ Represents a tool version string (i.e., a string with dotted version-number parts)
     and makes it possible to order these. Also handles sub-version suffixes like 1.0-0, 1.0-1, 1.0-2, etc.
 
-    :py:const:`ToolVersion.DEFAULT` is a version constant which is always better than any other version number
+    :py:const:`ToolVersion.DEFAULT` is a version constant which is always better than any other version number.
 
     >>> _test = lambda x, y: (x < y, x == y, x > y)
 
     >>> _test(ToolVersion('1'), ToolVersion('2'))
     (True, False, False)
 
     >>> _test(ToolVersion('1'), ToolVersion('1.1'))
@@ -100,15 +100,15 @@
 
         object.__setattr__(self, 'value', value)
         object.__setattr__(self, '_version', None)
 
     @property
     def version(self) -> tuple[str | tuple[int, ...]]:
         """ A tuple representing the :py:attr:`value` split on the dot and dash characters (``.``, ``-``)
-        and each part converted to :py:class:`int` if possible, and otherwise an :py:class:`str`.
+        and each part converted to :py:class:`int` if possible, and otherwise a :py:class:`str`.
 
         The special value :py:const:`~ToolVersion.DEFAULT` is converted into an empty tuple.
         """
         def _convert(value):
             if value != self.DEFAULT:
                 for part in value.split('.'):
                     try:
@@ -118,15 +118,15 @@
 
         if self._version is None:
             object.__setattr__(self, '_version', tuple(_convert(self.value)))
 
         return self._version
 
     def is_partial(self, other: "ToolVersion") -> bool:
-        """ Returns True if `self` is equal to or a partial version of `other`.
+        """ Returns `True` if **self** is equal to or a partial version of **other**.
 
         >>> ToolVersion('1').is_partial(ToolVersion('1'))
         True
 
         >>> ToolVersion('1').is_partial(ToolVersion('1.0'))
         True
 
@@ -190,9 +190,9 @@
     def __hash__(self):
         return hash(self.version)
 
     def __str__(self):
         return self.value
 
 
-#: Constant ``ToolVersion(ToolVersion.DEFAULT)``
+#: Constant :py:attr:`ToolVersion(ToolVersion.DEFAULT) <ToolVersion.DEFAULT>`
 default_tool_version = ToolVersion(ToolVersion.DEFAULT)
```

### Comparing `momotor-engine-options-2.0.0rc9/src/momotor_engine_options.egg-info/PKG-INFO` & `momotor_engine_options-2.0.1/src/momotor_engine_options.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: momotor-engine-options
-Version: 2.0.0rc9
+Version: 2.0.1
 Summary: Momotor Engine Options Library
 Author-email: Erik Scheffers <e.t.j.scheffers@tue.nl>
 License: GNU Lesser General Public License v3 (LGPLv3)
 Project-URL: Homepage, https://momotor.org
 Project-URL: Documentation, https://momotor.org/doc/engine/momotor-engine-options/
 Project-URL: Repository, https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/
 Project-URL: Tracker, https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/issues
@@ -14,31 +14,34 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: momotor-bundles~=8.0rc
+Requires-Dist: momotor-bundles~=8.0
 Requires-Dist: typing-extensions; python_version < "3.11"
 Provides-Extra: test
-Requires-Dist: pytest~=7.4; extra == "test"
+Requires-Dist: pytest~=8.1; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-doctestplus; extra == "test"
 Provides-Extra: docs
-Requires-Dist: docutils; extra == "docs"
+Requires-Dist: momotor-engine-options[test]; extra == "docs"
 Requires-Dist: Sphinx; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints!=1.14.0; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Provides-Extra: dev
-Requires-Dist: setuptools; extra == "dev"
-Requires-Dist: build[virtualenv]; extra == "dev"
+Requires-Dist: momotor-engine-options[docs]; extra == "dev"
 Requires-Dist: docutils-stubs; extra == "dev"
-Requires-Dist: python-semantic-release~=8.0; extra == "dev"
-Requires-Dist: twine; extra == "dev"
+Provides-Extra: build
+Requires-Dist: momotor-engine-options[dev]; extra == "build"
+Requires-Dist: setuptools; extra == "build"
+Requires-Dist: setuptools-scm; extra == "build"
+Requires-Dist: build[virtualenv]; extra == "build"
+Requires-Dist: python-semantic-release~=9.0; extra == "build"
 
 This package is a part of [Momotor](https://momotor.org/), a tool for automated processing of digital content. 
 
 Momotor accepts digital content as a product bundle and generates a result bundle from this product under 
 control of a recipe bundle. 
 
 Momotor is like a continuous integration system, but broader in scope. The
```

### Comparing `momotor-engine-options-2.0.0rc9/src/momotor_engine_options.egg-info/SOURCES.txt` & `momotor_engine_options-2.0.1/src/momotor_engine_options.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 .gitlab-ci.yml
 CHANGELOG.md
 README.md
 publish-docs.sh
 pyproject.toml
 semver.sh
 setup.py
+version.toml
 .idea/modules.xml
 .idea/momotor.lib.engine-options.iml
 .idea/workspace.xml
 .idea/inspectionProfiles/Project_Default.xml
 .idea/inspectionProfiles/profiles_settings.xml
 docs/Makefile
 docs/make.bat
@@ -27,28 +28,26 @@
 docs/source/_static/logo-text.png
 docs/source/_templates/projectlinks.html
 docs/source/options/index.rst
 docs/source/options/scheduler.rst
 docs/source/options/tools.rst
 docs/source/parser/index.rst
 docs/source/parser/syntax.rst
-src/momotor/__init__.py
 src/momotor/options/__init__.py
 src/momotor/options/convert.py
 src/momotor/options/dependencies.py
 src/momotor/options/doc.py
 src/momotor/options/exception.py
 src/momotor/options/filter_files.py
 src/momotor/options/option.py
 src/momotor/options/providers.py
 src/momotor/options/result_query.py
 src/momotor/options/split.py
 src/momotor/options/task_id.py
 src/momotor/options/types.py
-src/momotor/options/version.py
 src/momotor/options/domain/__init__.py
 src/momotor/options/domain/scheduler/__init__.py
 src/momotor/options/domain/scheduler/_domain.py
 src/momotor/options/domain/scheduler/preflight.py
 src/momotor/options/domain/scheduler/tasks.py
 src/momotor/options/domain/scheduler/tools.py
 src/momotor/options/domain/tools/__init__.py
```

### Comparing `momotor-engine-options-2.0.0rc9/tests/test_option_definition.py` & `momotor_engine_options-2.0.1/tests/test_option_definition.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc9/tests/test_parser_modifier.py` & `momotor_engine_options-2.0.1/tests/test_parser_modifier.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc9/tests/test_parser_placeholders.py` & `momotor_engine_options-2.0.1/tests/test_parser_placeholders.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc9/tests/test_parser_reference.py` & `momotor_engine_options-2.0.1/tests/test_parser_reference.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc9/tests/test_parser_selector.py` & `momotor_engine_options-2.0.1/tests/test_parser_selector.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc9/tests/test_utils_dependencies.py` & `momotor_engine_options-2.0.1/tests/test_utils_dependencies.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc9/tests/test_utils_tasks.py` & `momotor_engine_options-2.0.1/tests/test_utils_tasks.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc9/tests/tools/test_tool_registry.py` & `momotor_engine_options-2.0.1/tests/tools/test_tool_registry.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc9/tests/tools/test_tools_match.py` & `momotor_engine_options-2.0.1/tests/tools/test_tools_match.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc9/tests/tools/test_tools_options.py` & `momotor_engine_options-2.0.1/tests/tools/test_tools_options.py`

 * *Files identical despite different names*

