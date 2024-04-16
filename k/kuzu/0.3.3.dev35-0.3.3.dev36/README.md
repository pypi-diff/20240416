# Comparing `tmp/kuzu-0.3.3.dev35.tar.gz` & `tmp/kuzu-0.3.3.dev36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuzu-0.3.3.dev35.tar", last modified: Mon Apr 15 08:03:59 2024, max compression
+gzip compressed data, was "kuzu-0.3.3.dev36.tar", last modified: Tue Apr 16 08:04:22 2024, max compression
```

## Comparing `kuzu-0.3.3.dev35.tar` & `kuzu-0.3.3.dev36.tar`

### file list

```diff
@@ -1,2603 +1,2604 @@
-drwx------   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:59.024579 sdist/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-15 08:03:52.672616 sdist/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-15 08:03:54.148607 sdist/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-15 08:03:52.672616 sdist/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-04-15 08:03:54.148607 sdist/README_PYTHON_BUILD.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:57.788585 sdist/kuzu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:57.788585 sdist/kuzu-source/
--rw-rw-r--   0 runner    (1001) docker     (127)     5560 2024-04-15 08:03:54.000000 sdist/kuzu-source/.clang-format
--rw-rw-r--   0 runner    (1001) docker     (127)      948 2024-04-15 08:03:54.000000 sdist/kuzu-source/.clang-tidy
--rw-rw-r--   0 runner    (1001) docker     (127)      332 2024-04-15 08:03:54.000000 sdist/kuzu-source/.clang-tidy-analyzer
--rw-rw-r--   0 runner    (1001) docker     (127)     1000 2024-04-15 08:03:54.000000 sdist/kuzu-source/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (127)       47 2024-04-15 08:03:54.000000 sdist/kuzu-source/.lcovrc
--rw-rw-r--   0 runner    (1001) docker     (127)     8632 2024-04-15 08:03:54.000000 sdist/kuzu-source/CLA.md
--rw-rw-r--   0 runner    (1001) docker     (127)     8433 2024-04-15 08:03:54.000000 sdist/kuzu-source/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      632 2024-04-15 08:03:54.000000 sdist/kuzu-source/CODE_OF_CONDUCT.md
--rw-rw-r--   0 runner    (1001) docker     (127)     2052 2024-04-15 08:03:54.000000 sdist/kuzu-source/CONTRIBUTING.md
--rw-rw-r--   0 runner    (1001) docker     (127)     1072 2024-04-15 08:03:54.000000 sdist/kuzu-source/LICENSE
--rw-rw-r--   0 runner    (1001) docker     (127)     6365 2024-04-15 08:03:54.000000 sdist/kuzu-source/Makefile
--rw-rw-r--   0 runner    (1001) docker     (127)     3881 2024-04-15 08:03:54.000000 sdist/kuzu-source/README.md
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/scripts/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/scripts/antlr4/
--rw-rw-r--   0 runner    (1001) docker     (127)    26195 2024-04-15 08:03:54.000000 sdist/kuzu-source/scripts/antlr4/Cypher.g4.copy
--rw-rw-r--   0 runner    (1001) docker     (127)     2085 2024-04-15 08:03:54.000000 sdist/kuzu-source/scripts/antlr4/generate_grammar.cmake
--rwxrwxr-x   0 runner    (1001) docker     (127)      299 2024-04-15 08:03:54.000000 sdist/kuzu-source/scripts/check-include-guards.sh
--rwxrwxr-x   0 runner    (1001) docker     (127)       76 2024-04-15 08:03:54.000000 sdist/kuzu-source/scripts/check-no-std-assert.sh
--rwxrwxr-x   0 runner    (1001) docker     (127)     2837 2024-04-15 08:03:54.000000 sdist/kuzu-source/scripts/collect-single-file-header.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/scripts/generate-cpp-docs/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/scripts/generate-cpp-docs/c/
--rw-rw-r--   0 runner    (1001) docker     (127)   126290 2024-04-15 08:03:54.000000 sdist/kuzu-source/scripts/generate-cpp-docs/c/Doxyfile
--rw-rw-r--   0 runner    (1001) docker     (127)     4738 2024-04-15 08:03:54.000000 sdist/kuzu-source/scripts/generate-cpp-docs/collect_files.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/scripts/generate-cpp-docs/cpp/
--rw-rw-r--   0 runner    (1001) docker     (127)   126295 2024-04-15 08:03:54.000000 sdist/kuzu-source/scripts/generate-cpp-docs/cpp/Doxyfile
--rwxrwxr-x   0 runner    (1001) docker     (127)      225 2024-04-15 08:03:54.000000 sdist/kuzu-source/scripts/generate-cpp-docs/doxygen.sh
--rwxrwxr-x   0 runner    (1001) docker     (127)     6998 2024-04-15 08:03:54.000000 sdist/kuzu-source/scripts/get-clangd-diagnostics.py
--rw-rw-r--   0 runner    (1001) docker     (127)      173 2024-04-15 08:03:54.000000 sdist/kuzu-source/scripts/http-server.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/scripts/multiplatform-test-helper/
--rw-rw-r--   0 runner    (1001) docker     (127)     2130 2024-04-15 08:03:54.000000 sdist/kuzu-source/scripts/multiplatform-test-helper/collect-results.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1585 2024-04-15 08:03:54.000000 sdist/kuzu-source/scripts/multiplatform-test-helper/notify-discord.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/scripts/pip-package/
--rw-rw-r--   0 runner    (1001) docker     (127)       37 2024-04-15 08:03:54.000000 sdist/kuzu-source/scripts/pip-package/MANIFEST.in
--rw-rw-r--   0 runner    (1001) docker     (127)     3276 2024-04-15 08:03:54.000000 sdist/kuzu-source/scripts/pip-package/README.md
--rwxrwxr-x   0 runner    (1001) docker     (127)     3277 2024-04-15 08:03:54.000000 sdist/kuzu-source/scripts/pip-package/package_tar.py
--rw-rw-r--   0 runner    (1001) docker     (127)      200 2024-04-15 08:03:54.000000 sdist/kuzu-source/scripts/pip-package/setup.cfg
--rw-rw-r--   0 runner    (1001) docker     (127)     4441 2024-04-15 08:03:54.000000 sdist/kuzu-source/scripts/pip-package/setup.py
--rwxrwxr-x   0 runner    (1001) docker     (127)    12359 2024-04-15 08:03:54.000000 sdist/kuzu-source/scripts/run-clang-format.py
--rw-rw-r--   0 runner    (1001) docker     (127)     3060 2024-04-15 08:03:54.000000 sdist/kuzu-source/scripts/update-nightly-build-version.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/
--rw-rw-r--   0 runner    (1001) docker     (127)     2525 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/antlr4/
--rw-rw-r--   0 runner    (1001) docker     (127)    26195 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/antlr4/Cypher.g4
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/
--rw-rw-r--   0 runner    (1001) docker     (127)      519 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind/
--rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      520 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind/bind_attach_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      740 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind/bind_comment_on.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1323 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind/bind_create_macro.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    18649 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind/bind_ddl.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      516 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind/bind_detach_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      518 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind/bind_explain.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4631 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind/bind_export_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      579 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind/bind_extension.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5298 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind/bind_file_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    33112 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind/bind_graph_pattern.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3113 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind/bind_import_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11859 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind/bind_projection_clause.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4787 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind/bind_query.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      702 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind/bind_reading_clause.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1260 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind/bind_standalone_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      566 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind/bind_transaction.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    17251 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind/bind_updating_clause.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind/copy/
--rw-rw-r--   0 runner    (1001) docker     (127)      246 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind/copy/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    10625 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind/copy/bind_copy_from.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7684 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind/copy/bind_copy_rdf_graph.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1613 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind/copy/bind_copy_to.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind/ddl/
--rw-rw-r--   0 runner    (1001) docker     (127)      194 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind/ddl/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     3534 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind/ddl/bind_create_rdf_graph.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind/read/
--rw-rw-r--   0 runner    (1001) docker     (127)      267 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind/read/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2626 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind/read/bind_in_query_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5056 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind/read/bind_load_from.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3009 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind/read/bind_match.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1268 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind/read/bind_unwind.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind_expression/
--rw-rw-r--   0 runner    (1001) docker     (127)      555 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind_expression/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2201 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind_expression/bind_boolean_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3487 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind_expression/bind_case_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3376 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind_expression/bind_comparison_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    16259 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind_expression/bind_function_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1410 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind_expression/bind_literal_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1676 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind_expression/bind_null_operator_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      926 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind_expression/bind_parameter_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5174 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind_expression/bind_property_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3213 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind_expression/bind_subquery_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1531 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bind_expression/bind_variable_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8636 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/binder.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/binder_scope.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      585 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bound_statement_result.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      801 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bound_statement_rewriter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5434 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/bound_statement_visitor.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/expression/
--rw-rw-r--   0 runner    (1001) docker     (127)      348 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/expression/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      498 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/expression/case_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      764 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/expression/expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5664 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/expression/expression_util.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1438 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/expression/function_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      596 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/expression/literal_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      602 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/expression/parameter_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6345 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/expression_binder.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5779 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/expression_visitor.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/query/
--rw-rw-r--   0 runner    (1001) docker     (127)      350 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/query/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      707 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/query/bound_delete_clause.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      707 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/query/bound_insert_clause.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1963 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/query/bound_merge_clause.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      718 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/query/bound_set_clause.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9670 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/query/query_graph.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6621 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/query/query_graph_label_analyzer.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/rewriter/
--rw-rw-r--   0 runner    (1001) docker     (127)      261 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/rewriter/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      742 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/rewriter/match_clause_pattern_label_rewriter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2547 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/rewriter/with_clause_projection_rewriter.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/visitor/
--rw-rw-r--   0 runner    (1001) docker     (127)      230 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/visitor/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      638 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/visitor/default_type_solver.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4801 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/binder/visitor/property_collector.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/c_api/
--rw-rw-r--   0 runner    (1001) docker     (127)      369 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/c_api/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     4034 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/c_api/connection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2689 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/c_api/data_type.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1237 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/c_api/database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1412 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/c_api/flat_tuple.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      286 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/c_api/helpers.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7841 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/c_api/prepared_statement.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4402 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/c_api/query_result.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      745 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/c_api/query_summary.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    19820 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/c_api/value.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      271 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/c_api/version.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/catalog/
--rw-rw-r--   0 runner    (1001) docker     (127)      270 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/catalog/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    10617 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/catalog/catalog.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    13978 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/catalog/catalog_content.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/catalog/catalog_entry/
--rw-rw-r--   0 runner    (1001) docker     (127)      433 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/catalog/catalog_entry/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1198 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/catalog/catalog_entry/catalog_entry.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      605 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/catalog/catalog_entry/function_catalog_entry.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2023 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/catalog/catalog_entry/node_table_catalog_entry.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3144 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/catalog/catalog_entry/rdf_graph_catalog_entry.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1483 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/catalog/catalog_entry/rel_group_catalog_entry.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4001 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/catalog/catalog_entry/rel_table_catalog_entry.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1224 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/catalog/catalog_entry/scalar_macro_catalog_entry.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4261 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/catalog/catalog_entry/table_catalog_entry.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2691 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/catalog/catalog_set.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1483 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/catalog/property.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/
--rw-rw-r--   0 runner    (1001) docker     (127)      810 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/arrow/
--rw-rw-r--   0 runner    (1001) docker     (127)      295 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/arrow/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    23959 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/arrow/arrow_array_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    10319 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/arrow/arrow_converter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8717 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/arrow/arrow_null_mask_tree.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    39407 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/arrow/arrow_row_batch.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5389 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/arrow/arrow_type.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      478 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/case_insensitive_map.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      106 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/constants.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/copier_config/
--rw-rw-r--   0 runner    (1001) docker     (127)      256 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/copier_config/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     3078 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/copier_config/csv_reader_config.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/copier_config/rdf_reader_config.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1727 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/copier_config/reader_config.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/data_chunk/
--rw-rw-r--   0 runner    (1001) docker     (127)      250 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/data_chunk/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      470 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/data_chunk/data_chunk.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2645 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/data_chunk/data_chunk_collection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    12603 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/data_chunk/data_chunk_state.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/enums/
--rw-rw-r--   0 runner    (1001) docker     (127)      258 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/enums/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1050 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/enums/path_semantic.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      413 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/enums/rel_direction.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1069 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/enums/rel_multiplicity.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      578 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/enums/table_type.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/exception/
--rw-rw-r--   0 runner    (1001) docker     (127)      182 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/exception/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2494 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/exception/message.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3201 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/expression_type.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/file_system/
--rw-rw-r--   0 runner    (1001) docker     (127)      306 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/file_system/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      917 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/file_system/file_info.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1279 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/file_system/file_system.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    13769 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/file_system/local_file_system.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2609 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/file_system/virtual_file_system.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      663 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/in_mem_overflow_buffer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/keyword_utils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      743 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/logging_level_utils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8157 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/md5.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      995 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/metric.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6819 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/null_mask.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1452 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/profiler.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      349 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/random_engine.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/serializer/
--rw-rw-r--   0 runner    (1001) docker     (127)      270 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/serializer/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2602 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/serializer/buffered_file.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      948 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/serializer/buffered_serializer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      347 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/serializer/deserializer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      356 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/serializer/serializer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1355 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/sha256.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4819 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/string_utils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      884 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/system_message.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/task_system/
--rw-rw-r--   0 runner    (1001) docker     (127)      236 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/task_system/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2720 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/task_system/progress_bar.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      772 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/task_system/task.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4596 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/task_system/task_scheduler.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9684 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/type_utils.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/types/
--rw-rw-r--   0 runner    (1001) docker     (127)      406 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/types/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     4772 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/types/blob.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    19741 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/types/date_t.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6196 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/types/dtime_t.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    19061 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/types/int128_t.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1173 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/types/internal_id_t.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    17620 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/types/interval_t.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      834 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/types/ku_list.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2364 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/types/ku_string.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11000 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/types/timestamp_t.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    35317 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/types/types.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4363 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/types/uuid.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/types/value/
--rw-rw-r--   0 runner    (1001) docker     (127)      286 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/types/value/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      512 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/types/value/nested.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2409 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/types/value/node.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      354 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/types/value/rdf_variant.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      840 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/types/value/recursive_rel.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2799 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/types/value/rel.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    27055 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/types/value/value.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2142 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/utils.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/vector/
--rw-rw-r--   0 runner    (1001) docker     (127)      210 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/vector/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     3468 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/vector/auxiliary_buffer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    28631 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/vector/value_vector.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1261 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/common/windows_utils.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/expression_evaluator/
--rw-rw-r--   0 runner    (1001) docker     (127)      420 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/expression_evaluator/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     4615 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/expression_evaluator/case_evaluator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      965 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/expression_evaluator/expression_evaluator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      885 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/expression_evaluator/expression_evaluator_utils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3490 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/expression_evaluator/function_evaluator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1130 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/expression_evaluator/literal_evaluator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1556 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/expression_evaluator/node_rel_evaluator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9766 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/expression_evaluator/path_evaluator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1275 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/expression_evaluator/reference_evaluator.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/extension/
--rw-rw-r--   0 runner    (1001) docker     (127)      170 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/extension/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2157 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/extension/extension.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/
--rw-rw-r--   0 runner    (1001) docker     (127)     1259 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/aggregate/
--rw-rw-r--   0 runner    (1001) docker     (127)      227 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/aggregate/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     3939 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/aggregate/collect.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1841 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/aggregate/count.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1044 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/aggregate/count_star.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    12187 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/aggregate_function.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/arithmetic/
--rw-rw-r--   0 runner    (1001) docker     (127)      299 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/arithmetic/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2611 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/arithmetic/abs.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5505 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/arithmetic/add.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5953 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/arithmetic/divide.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4379 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/arithmetic/modulo.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8121 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/arithmetic/multiply.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2427 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/arithmetic/negate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5848 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/arithmetic/subtract.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2494 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/base_lower_upper_operation.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    18957 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/built_in_function_utils.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/cast/
--rw-rw-r--   0 runner    (1001) docker     (127)      208 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/cast/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     5405 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/cast/cast_array.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11953 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/cast/cast_rdf_variant.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    33753 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/cast_from_string_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2442 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/cast_string_non_nested_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8637 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/comparison_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5169 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/find_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    12306 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/function_collection.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/pattern/
--rw-rw-r--   0 runner    (1001) docker     (127)      186 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/pattern/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1872 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/pattern/id_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2683 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/scalar_macro_function.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/table/
--rw-rw-r--   0 runner    (1001) docker     (127)      218 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/table/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/table/call/
--rw-rw-r--   0 runner    (1001) docker     (127)      301 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/table/call/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2314 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/table/call/current_setting.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1428 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/table/call/db_version.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5207 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/table/call/show_connection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2909 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/table/call/show_tables.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11166 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/table/call/storage_info.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4397 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/table/call/table_info.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1139 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/table/call_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      364 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/table/scan_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    18420 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/vector_arithmetic_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6890 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/vector_array_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1498 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/vector_blob_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4267 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/vector_boolean_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    43230 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/vector_cast_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4887 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/vector_date_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    10173 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/vector_hash_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    49369 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/vector_list_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7341 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/vector_map_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      888 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/vector_node_rel_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1516 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/vector_null_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6879 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/vector_path_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      913 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/vector_rdf_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    15223 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/vector_string_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5543 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/vector_struct_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1205 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/vector_timestamp_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2856 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/vector_union_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      552 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/function/vector_uuid_functions.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/
--rw-rw-r--   0 runner    (1001) docker     (127)    12622 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/binder.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2756 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/binder_scope.h
--rw-rw-r--   0 runner    (1001) docker     (127)      592 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/bound_attach_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      862 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/bound_comment_on.h
--rw-rw-r--   0 runner    (1001) docker     (127)      842 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/bound_create_macro.h
--rw-rw-r--   0 runner    (1001) docker     (127)      503 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/bound_detach_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      891 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/bound_explain.h
--rw-rw-r--   0 runner    (1001) docker     (127)      700 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/bound_extension_statement.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2466 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/bound_scan_source.h
--rw-rw-r--   0 runner    (1001) docker     (127)      790 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/bound_standalone_call.h
--rw-rw-r--   0 runner    (1001) docker     (127)      787 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/bound_statement.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1034 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/bound_statement_result.h
--rw-rw-r--   0 runner    (1001) docker     (127)      348 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/bound_statement_rewriter.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2606 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/bound_statement_visitor.h
--rw-rw-r--   0 runner    (1001) docker     (127)      661 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/bound_transaction_statement.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/copy/
--rw-rw-r--   0 runner    (1001) docker     (127)     3164 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/copy/bound_copy_from.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1071 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/copy/bound_copy_to.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1888 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/copy/bound_export_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      813 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/copy/bound_file_scan_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)      626 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/copy/bound_import_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1014 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/copy/index_look_up_info.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/ddl/
--rw-rw-r--   0 runner    (1001) docker     (127)      530 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/ddl/bound_alter.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3274 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/ddl/bound_alter_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)      574 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/ddl/bound_create_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5498 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/ddl/bound_create_table_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)      664 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/ddl/bound_drop_table.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/expression/
--rw-rw-r--   0 runner    (1001) docker     (127)     1468 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/expression/case_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4519 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/expression/expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1962 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/expression/expression_util.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4586 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/expression/function_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)      878 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/expression/literal_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)      786 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/expression/node_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4200 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/expression/node_rel_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)      937 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/expression/parameter_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1129 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/expression/path_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2561 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/expression/property_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4586 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/expression/rel_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2112 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/expression/subquery_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)      796 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/expression/variable_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6024 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/expression_binder.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2678 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/expression_visitor.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/query/
--rw-rw-r--   0 runner    (1001) docker     (127)     1069 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/query/bound_regular_query.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2487 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/query/normalized_query_part.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1013 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/query/normalized_single_query.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6508 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/query/query_graph.h
--rw-rw-r--   0 runner    (1001) docker     (127)      572 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/query/query_graph_label_analyzer.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/
--rw-rw-r--   0 runner    (1001) docker     (127)     1225 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_in_query_call.h
--rw-rw-r--   0 runner    (1001) docker     (127)      482 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_load_from.h
--rw-rw-r--   0 runner    (1001) docker     (127)      813 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_match_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1010 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_reading_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      869 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_unwind_clause.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/query/return_with_clause/
--rw-rw-r--   0 runner    (1001) docker     (127)     3072 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/query/return_with_clause/bound_projection_body.h
--rw-rw-r--   0 runner    (1001) docker     (127)      923 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/query/return_with_clause/bound_return_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      687 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/query/return_with_clause/bound_with_clause.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/
--rw-rw-r--   0 runner    (1001) docker     (127)     1445 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_delete_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      871 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_delete_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1470 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_insert_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1520 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_insert_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5606 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_merge_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1570 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_set_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      797 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_set_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)      424 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_updating_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      163 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/update_table_type.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/rewriter/
--rw-rw-r--   0 runner    (1001) docker     (127)      515 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/rewriter/match_clause_pattern_label_rewriter.h
--rw-rw-r--   0 runner    (1001) docker     (127)      693 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/rewriter/with_clause_projection_rewriter.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/visitor/
--rw-rw-r--   0 runner    (1001) docker     (127)      781 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/visitor/default_type_solver.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1211 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/binder/visitor/property_collector.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/c_api/
--rw-rw-r--   0 runner    (1001) docker     (127)       86 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/c_api/helpers.h
--rw-rw-r--   0 runner    (1001) docker     (127)    51266 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/c_api/kuzu.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/catalog/
--rw-rw-r--   0 runner    (1001) docker     (127)     4618 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/catalog/catalog.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3595 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/catalog/catalog_content.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/
--rw-rw-r--   0 runner    (1001) docker     (127)     1612 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/catalog_entry.h
--rw-rw-r--   0 runner    (1001) docker     (127)      444 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/catalog_entry_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1331 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/function_catalog_entry.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2508 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/node_table_catalog_entry.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2311 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/rdf_graph_catalog_entry.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1522 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/rel_group_catalog_entry.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2361 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/rel_table_catalog_entry.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1449 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/scalar_macro_catalog_entry.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3199 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/table_catalog_entry.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1283 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/catalog/catalog_set.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1693 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/catalog/property.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/
--rw-rw-r--   0 runner    (1001) docker     (127)      975 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/api.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/arrow/
--rw-rw-r--   0 runner    (1001) docker     (127)     1542 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/arrow/arrow.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1943 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/arrow/arrow_buffer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1862 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/arrow/arrow_converter.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1341 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/arrow/arrow_nullmask_tree.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3505 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/arrow/arrow_row_batch.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1139 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/assert.h
--rw-rw-r--   0 runner    (1001) docker     (127)      578 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/case_insensitive_map.h
--rw-rw-r--   0 runner    (1001) docker     (127)      559 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/cast.h
--rw-rw-r--   0 runner    (1001) docker     (127)      178 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/column_data_format.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9693 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/constants.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/copier_config/
--rw-rw-r--   0 runner    (1001) docker     (127)     1633 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/copier_config/csv_reader_config.h
--rw-rw-r--   0 runner    (1001) docker     (127)      468 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/copier_config/rdf_reader_config.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1302 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/copier_config/reader_config.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3648 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/copy_constructors.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/data_chunk/
--rw-rw-r--   0 runner    (1001) docker     (127)     1575 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/data_chunk/data_chunk.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1261 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/data_chunk/data_chunk_collection.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1882 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/data_chunk/data_chunk_state.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1540 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/data_chunk/sel_vector.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/enums/
--rw-rw-r--   0 runner    (1001) docker     (127)      246 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/enums/alter_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      575 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/enums/clause_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      194 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/enums/conflict_action.h
--rw-rw-r--   0 runner    (1001) docker     (127)      194 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/enums/delete_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      192 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/enums/explain_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1221 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/enums/expression_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      285 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/enums/join_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      364 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/enums/path_semantic.h
--rw-rw-r--   0 runner    (1001) docker     (127)      402 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/enums/query_rel_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      300 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/enums/rel_direction.h
--rw-rw-r--   0 runner    (1001) docker     (127)      359 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/enums/rel_multiplicity.h
--rw-rw-r--   0 runner    (1001) docker     (127)      195 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/enums/scan_source_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      915 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/enums/statement_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      164 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/enums/subquery_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      431 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/enums/table_type.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/exception/
--rw-rw-r--   0 runner    (1001) docker     (127)      301 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/exception/binder.h
--rw-rw-r--   0 runner    (1001) docker     (127)      331 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/exception/buffer_manager.h
--rw-rw-r--   0 runner    (1001) docker     (127)      304 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/exception/catalog.h
--rw-rw-r--   0 runner    (1001) docker     (127)      286 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/exception/connection.h
--rw-rw-r--   0 runner    (1001) docker     (127)      321 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/exception/conversion.h
--rw-rw-r--   0 runner    (1001) docker     (127)      295 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/exception/copy.h
--rw-rw-r--   0 runner    (1001) docker     (127)      455 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/exception/exception.h
--rw-rw-r--   0 runner    (1001) docker     (127)      294 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/exception/extension.h
--rw-rw-r--   0 runner    (1001) docker     (127)      282 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/exception/internal.h
--rw-rw-r--   0 runner    (1001) docker     (127)      273 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/exception/interrupt.h
--rw-rw-r--   0 runner    (1001) docker     (127)      265 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/exception/io.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1185 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/exception/message.h
--rw-rw-r--   0 runner    (1001) docker     (127)      294 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/exception/not_implemented.h
--rw-rw-r--   0 runner    (1001) docker     (127)      307 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/exception/overflow.h
--rw-rw-r--   0 runner    (1001) docker     (127)      301 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/exception/parser.h
--rw-rw-r--   0 runner    (1001) docker     (127)      304 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/exception/runtime.h
--rw-rw-r--   0 runner    (1001) docker     (127)      304 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/exception/storage.h
--rw-rw-r--   0 runner    (1001) docker     (127)      262 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/exception/test.h
--rw-rw-r--   0 runner    (1001) docker     (127)      302 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/exception/transaction_manager.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/file_system/
--rw-rw-r--   0 runner    (1001) docker     (127)      784 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/file_system/file_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2006 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/file_system/file_system.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1976 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/file_system/local_file_system.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1738 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/file_system/virtual_file_system.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2203 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/in_mem_overflow_buffer.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/keyword/
--rw-rw-r--   0 runner    (1001) docker     (127)     1576 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/keyword/rdf_keyword.h
--rw-rw-r--   0 runner    (1001) docker     (127)      294 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/logging_level_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3271 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/md5.h
--rw-rw-r--   0 runner    (1001) docker     (127)      745 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/metric.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3921 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/mpsc_queue.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1346 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/mutex.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1155 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/null_buffer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8464 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/null_mask.h
--rw-rw-r--   0 runner    (1001) docker     (127)      702 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/profiler.h
--rw-rw-r--   0 runner    (1001) docker     (127)      349 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/random_engine.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/serializer/
--rw-rw-r--   0 runner    (1001) docker     (127)     1391 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/serializer/buffered_file.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1716 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/serializer/buffered_serializer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2495 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/serializer/deserializer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      264 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/serializer/reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2467 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/serializer/serializer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      237 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/serializer/writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      557 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/sha256.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2228 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/static_vector.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3858 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/string_format.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4679 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/string_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)      596 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/system_message.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/task_system/
--rw-rw-r--   0 runner    (1001) docker     (127)     1469 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/task_system/progress_bar.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3420 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/task_system/task.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3059 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/task_system/task_scheduler.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1205 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/timer.h
--rw-rw-r--   0 runner    (1001) docker     (127)    11010 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/type_utils.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/types/
--rw-rw-r--   0 runner    (1001) docker     (127)     1666 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/types/blob.h
--rw-rw-r--   0 runner    (1001) docker     (127)    10927 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/types/cast_helpers.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4563 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/types/date_t.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2446 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/types/dtime_t.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6090 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/types/int128_t.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1063 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/types/internal_id_t.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4658 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/types/interval_t.h
--rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/types/ku_list.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2887 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/types/ku_string.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4667 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/types/timestamp_t.h
--rw-rw-r--   0 runner    (1001) docker     (127)    22301 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/types/types.h
--rw-rw-r--   0 runner    (1001) docker     (127)      940 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/types/uuid.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/types/value/
--rw-rw-r--   0 runner    (1001) docker     (127)      319 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/types/value/nested.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1670 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/types/value/node.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1145 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/types/value/rdf_variant.h
--rw-rw-r--   0 runner    (1001) docker     (127)      635 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/types/value/recursive_rel.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1968 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/types/value/rel.h
--rw-rw-r--   0 runner    (1001) docker     (127)    20925 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/types/value/value.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1172 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/utils.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/vector/
--rw-rw-r--   0 runner    (1001) docker     (127)     3218 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/vector/auxiliary_buffer.h
--rw-rw-r--   0 runner    (1001) docker     (127)    13715 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/vector/value_vector.h
--rw-rw-r--   0 runner    (1001) docker     (127)      298 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/common/windows_utils.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/expression_evaluator/
--rw-rw-r--   0 runner    (1001) docker     (127)     2419 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/expression_evaluator/case_evaluator.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1382 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/expression_evaluator/expression_evaluator.h
--rw-rw-r--   0 runner    (1001) docker     (127)      450 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/expression_evaluator/expression_evaluator_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1267 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/expression_evaluator/function_evaluator.h
--rw-rw-r--   0 runner    (1001) docker     (127)      972 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/expression_evaluator/literal_evaluator.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1399 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/expression_evaluator/node_rel_evaluator.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2884 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/expression_evaluator/path_evaluator.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1082 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/expression_evaluator/reference_evaluator.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/extension/
--rw-rw-r--   0 runner    (1001) docker     (127)     1103 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/extension/extension.h
--rw-rw-r--   0 runner    (1001) docker     (127)      193 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/extension/extension_action.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/aggregate/
--rw-rw-r--   0 runner    (1001) docker     (127)     3538 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/aggregate/avg.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1139 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/aggregate/base_count.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2409 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/aggregate/collect.h
--rw-rw-r--   0 runner    (1001) docker     (127)      821 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/aggregate/count.h
--rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/aggregate/count_star.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4106 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/aggregate/min_max.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2918 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/aggregate/sum.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7021 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/aggregate_function.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/arithmetic/
--rw-rw-r--   0 runner    (1001) docker     (127)      740 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/arithmetic/abs.h
--rw-rw-r--   0 runner    (1001) docker     (127)      930 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/arithmetic/add.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5133 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/arithmetic/arithmetic_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      957 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/arithmetic/divide.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1109 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/arithmetic/modulo.h
--rw-rw-r--   0 runner    (1001) docker     (127)      975 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/arithmetic/multiply.h
--rw-rw-r--   0 runner    (1001) docker     (127)      520 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/arithmetic/negate.h
--rw-rw-r--   0 runner    (1001) docker     (127)      975 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/arithmetic/subtract.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4696 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/arithmetic/vector_arithmetic_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/array/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/array/functions/
--rw-rw-r--   0 runner    (1001) docker     (127)     1096 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/array/functions/array_cosine_similarity.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1078 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/array/functions/array_cross_product.h
--rw-rw-r--   0 runner    (1001) docker     (127)      824 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/array/functions/array_distance.h
--rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/array/functions/array_inner_product.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2034 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/array/vector_array_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)    25289 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/binary_function_executor.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/blob/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/blob/functions/
--rw-rw-r--   0 runner    (1001) docker     (127)      828 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/blob/functions/decode_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      402 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/blob/functions/encode_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      269 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/blob/functions/octet_length_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      506 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/blob/vector_blob_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/boolean/
--rw-rw-r--   0 runner    (1001) docker     (127)    15140 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/boolean/boolean_function_executor.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4678 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/boolean/boolean_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2493 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/boolean/vector_boolean_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3210 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/built_in_function_utils.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/cast/
--rw-rw-r--   0 runner    (1001) docker     (127)      674 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/cast/cast_function_bind_data.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/cast/functions/
--rw-rw-r--   0 runner    (1001) docker     (127)      525 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_array.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7564 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_from_string_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)    13672 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      993 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_rdf_variant.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7994 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_string_non_nested_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5149 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/cast/functions/numeric_cast.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1795 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/cast/functions/numeric_limits.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3693 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/cast/vector_cast_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/comparison/
--rw-rw-r--   0 runner    (1001) docker     (127)     2928 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/comparison/comparison_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)    10609 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/comparison/vector_comparison_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      523 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/const_function_executor.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/date/
--rw-rw-r--   0 runner    (1001) docker     (127)     4625 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/date/date_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1236 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/date/vector_date_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2083 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      455 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/function_collection.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/hash/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/hash/functions/
--rw-rw-r--   0 runner    (1001) docker     (127)      519 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/hash/functions/md5_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      571 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/hash/functions/sha256_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6058 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/hash/hash_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      945 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/hash/vector_hash_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/interval/
--rw-rw-r--   0 runner    (1001) docker     (127)     1758 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/interval/interval_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2341 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/interval/vector_interval_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/list/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/list/functions/
--rw-rw-r--   0 runner    (1001) docker     (127)     3521 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/list/functions/base_list_sort_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      924 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/list/functions/list_any_value_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1098 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/list/functions/list_append_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1186 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/list/functions/list_concat_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      587 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/list/functions/list_contains_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1369 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/list/functions/list_distinct_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1987 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/list/functions/list_extract_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1058 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/list/functions/list_len_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1215 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/list/functions/list_position_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1078 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/list/functions/list_prepend_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      680 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/list/functions/list_product_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1550 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/list/functions/list_range_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      802 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/list/functions/list_reverse_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1309 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/list/functions/list_reverse_sort_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1928 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/list/functions/list_slice_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1333 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/list/functions/list_sort_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      676 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/list/functions/list_sum_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      846 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/list/functions/list_unique_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3175 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/list/vector_list_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/map/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/map/functions/
--rw-rw-r--   0 runner    (1001) docker     (127)      872 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/map/functions/base_map_extract_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1580 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/map/functions/map_creation_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1515 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/map/functions/map_extract_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      658 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/map/functions/map_keys_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      712 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/map/functions/map_values_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/map/vector_map_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/null/
--rw-rw-r--   0 runner    (1001) docker     (127)     2772 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/null/null_function_executor.h
--rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/null/null_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1154 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/null/vector_null_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/path/
--rw-rw-r--   0 runner    (1001) docker     (127)     6252 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/path/path_function_executor.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1090 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/path/vector_path_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      791 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/pointer_function_executor.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/rdf/
--rw-rw-r--   0 runner    (1001) docker     (127)     1299 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/rdf/rdf_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      393 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/rdf/vector_rdf_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      905 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/rewrite_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)    10009 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/scalar_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1403 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/scalar_macro_function.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/schema/
--rw-rw-r--   0 runner    (1001) docker     (127)      649 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/schema/label_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      276 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/schema/offset_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      642 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/schema/vector_label_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      529 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/schema/vector_node_rel_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/string/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/string/functions/
--rw-rw-r--   0 runner    (1001) docker     (127)     2242 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/string/functions/array_extract_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      669 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/string/functions/base_lower_upper_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2303 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/string/functions/base_pad_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      809 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/string/functions/base_regexp_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      429 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/string/functions/base_str_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/string/functions/contains_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      450 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/string/functions/ends_with_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1459 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/string/functions/find_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      575 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/string/functions/initcap_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      656 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/string/functions/left_operation.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1738 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/string/functions/levenshtein_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      444 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/string/functions/lower_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1035 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/string/functions/lpad_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      732 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/string/functions/ltrim_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      874 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/string/functions/pad_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3067 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_extract_all_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1778 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_extract_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      476 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_full_match_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      477 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_matches_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      710 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_replace_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      640 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/string/functions/repeat_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      570 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/string/functions/reverse_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      673 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/string/functions/right_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1035 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/string/functions/rpad_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      664 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/string/functions/rtrim_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      401 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/string/functions/starts_with_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2808 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/string/functions/substr_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      587 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/string/functions/trim_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      509 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/string/functions/upper_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5574 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/string/vector_string_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/struct/
--rw-rw-r--   0 runner    (1001) docker     (127)     1383 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/struct/vector_struct_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/table/
--rw-rw-r--   0 runner    (1001) docker     (127)     1540 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/table/bind_data.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1717 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/table/bind_input.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2713 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/table/call_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1105 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/table/scan_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      527 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/table/scan_replacement.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4030 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/table_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)    22251 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/ternary_function_executor.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/timestamp/
--rw-rw-r--   0 runner    (1001) docker     (127)     1036 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/timestamp/timestamp_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      508 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/timestamp/vector_timestamp_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)    10907 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/udf_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8481 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/unary_function_executor.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/union/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/union/functions/
--rw-rw-r--   0 runner    (1001) docker     (127)     1249 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/union/functions/union_tag.h
--rw-rw-r--   0 runner    (1001) docker     (127)      519 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/union/vector_union_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/uuid/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/uuid/functions/
--rw-rw-r--   0 runner    (1001) docker     (127)      395 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/uuid/functions/gen_random_uuid.h
--rw-rw-r--   0 runner    (1001) docker     (127)      266 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/function/uuid/vector_uuid_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/main/
--rw-rw-r--   0 runner    (1001) docker     (127)      607 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/main/attached_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1561 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/main/client_config.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6386 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/main/client_context.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7548 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/main/connection.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5801 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/main/database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      450 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/main/database_manager.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1546 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/main/db_config.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1394 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/main/kuzu.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1248 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/main/kuzu_fwd.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3548 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/main/plan_printer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1992 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/main/prepared_statement.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4873 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/main/query_result.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1015 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/main/query_summary.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6746 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/main/settings.h
--rw-rw-r--   0 runner    (1001) docker     (127)      830 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/main/storage_driver.h
--rw-rw-r--   0 runner    (1001) docker     (127)      528 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/main/version.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/optimizer/
--rw-rw-r--   0 runner    (1001) docker     (127)     2295 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/optimizer/acc_hash_join_optimizer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      821 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/optimizer/agg_key_dependency_optimizer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      895 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/optimizer/correlated_subquery_unnest_solver.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2050 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/optimizer/factorization_rewriter.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3150 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/optimizer/filter_push_down_optimizer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1376 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/optimizer/logical_operator_collector.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6889 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/optimizer/logical_operator_visitor.h
--rw-rw-r--   0 runner    (1001) docker     (127)      298 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/optimizer/optimizer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2461 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/optimizer/projection_push_down_optimizer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      572 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/optimizer/remove_factorization_rewriter.h
--rw-rw-r--   0 runner    (1001) docker     (127)      936 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/optimizer/remove_unnecessary_join_optimizer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      556 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/optimizer/top_k_optimizer.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/antlr_parser/
--rw-rw-r--   0 runner    (1001) docker     (127)      895 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/antlr_parser/kuzu_cypher_parser.h
--rw-rw-r--   0 runner    (1001) docker     (127)      620 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/antlr_parser/parser_error_listener.h
--rw-rw-r--   0 runner    (1001) docker     (127)      373 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/antlr_parser/parser_error_strategy.h
--rw-rw-r--   0 runner    (1001) docker     (127)      468 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/attach_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      541 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/comment_on.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1793 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/copy.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1237 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/create_macro.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/ddl/
--rw-rw-r--   0 runner    (1001) docker     (127)      397 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/ddl/alter.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1748 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/ddl/alter_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)      447 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/ddl/create_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1782 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/ddl/create_table_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/ddl/drop.h
--rw-rw-r--   0 runner    (1001) docker     (127)      429 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/detach_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      748 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/explain_statement.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/expression/
--rw-rw-r--   0 runner    (1001) docker     (127)     3933 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/expression/parsed_case_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3025 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/expression/parsed_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2663 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/expression/parsed_function_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1552 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/expression/parsed_literal_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)      858 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/expression/parsed_parameter_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1688 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/expression/parsed_property_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/expression/parsed_subquery_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1546 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/expression/parsed_variable_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)      626 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/extension_statement.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/parsed_data/
--rw-rw-r--   0 runner    (1001) docker     (127)      177 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/parsed_data/attach_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1163 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/parsed_expression_visitor.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2544 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/parsed_statement_visitor.h
--rw-rw-r--   0 runner    (1001) docker     (127)      292 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/parser.h
--rw-rw-r--   0 runner    (1001) docker     (127)      975 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/port_db.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/query/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/
--rw-rw-r--   0 runner    (1001) docker     (127)      946 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/node_pattern.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1100 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/pattern_element.h
--rw-rw-r--   0 runner    (1001) docker     (127)      587 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/pattern_element_chain.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1599 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/rel_pattern.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1309 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/query/query_part.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/
--rw-rw-r--   0 runner    (1001) docker     (127)      982 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/in_query_call_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1521 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/load_from.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1212 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/match_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      587 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/reading_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      657 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/unwind_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      928 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/query/regular_query.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/query/return_with_clause/
--rw-rw-r--   0 runner    (1001) docker     (127)     2155 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/query/return_with_clause/projection_body.h
--rw-rw-r--   0 runner    (1001) docker     (127)      485 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/query/return_with_clause/return_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/query/return_with_clause/with_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1798 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/query/single_query.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/
--rw-rw-r--   0 runner    (1001) docker     (127)      898 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/delete_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      601 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/insert_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1341 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/merge_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      538 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/set_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/updating_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1543 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/scan_source.h
--rw-rw-r--   0 runner    (1001) docker     (127)      712 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/standalone_call.h
--rw-rw-r--   0 runner    (1001) docker     (127)      945 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/statement.h
--rw-rw-r--   0 runner    (1001) docker     (127)      568 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/transaction_statement.h
--rw-rw-r--   0 runner    (1001) docker     (127)    12840 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/transformer.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/visitor/
--rw-rw-r--   0 runner    (1001) docker     (127)     1164 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/parser/visitor/statement_read_write_analyzer.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/join_order/
--rw-rw-r--   0 runner    (1001) docker     (127)     2656 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/join_order/cardinality_estimator.h
--rw-rw-r--   0 runner    (1001) docker     (127)      801 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/join_order/cost_model.h
--rw-rw-r--   0 runner    (1001) docker     (127)      469 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/join_order/join_order_util.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2304 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/join_order_enumerator_context.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/ddl/
--rw-rw-r--   0 runner    (1001) docker     (127)      754 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/ddl/logical_alter.h
--rw-rw-r--   0 runner    (1001) docker     (127)      841 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/ddl/logical_create_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)      920 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/ddl/logical_ddl.h
--rw-rw-r--   0 runner    (1001) docker     (127)      795 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/ddl/logical_drop_table.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/extend/
--rw-rw-r--   0 runner    (1001) docker     (127)     1426 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/extend/base_logical_extend.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1121 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/extend/extend_direction.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1278 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/extend/logical_extend.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4582 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/extend/logical_recursive_extend.h
--rw-rw-r--   0 runner    (1001) docker     (127)      200 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/extend/recursive_join_type.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/factorization/
--rw-rw-r--   0 runner    (1001) docker     (127)      442 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/factorization/flatten_resolver.h
--rw-rw-r--   0 runner    (1001) docker     (127)      950 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/factorization/sink_util.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2011 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_accumulate.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2430 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_aggregate.h
--rw-rw-r--   0 runner    (1001) docker     (127)      900 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_attach_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1376 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_comment_on.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1381 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_create_macro.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1079 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_cross_product.h
--rw-rw-r--   0 runner    (1001) docker     (127)      791 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_detach_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1632 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_distinct.h
--rw-rw-r--   0 runner    (1001) docker     (127)      784 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_empty_result.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1603 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_explain.h
--rw-rw-r--   0 runner    (1001) docker     (127)      991 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_extension.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1117 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_filter.h
--rw-rw-r--   0 runner    (1001) docker     (127)      804 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_flatten.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3562 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_hash_join.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_in_query_call.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1843 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_intersect.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1297 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_limit.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1147 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_mark_accmulate.h
--rw-rw-r--   0 runner    (1001) docker     (127)      769 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_multiplcity_reducer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1224 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_node_label_filter.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3398 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_operator.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1616 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_order_by.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2156 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_partitioner.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1176 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_plan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1179 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_plan_util.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1117 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_projection.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1094 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_standalone_call.h
--rw-rw-r--   0 runner    (1001) docker     (127)      969 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_transaction.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1199 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_union.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1413 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/logical_unwind.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/persistent/
--rw-rw-r--   0 runner    (1001) docker     (127)     1473 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_copy_from.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1835 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_copy_to.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2791 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_delete.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1413 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_export_db.h
--rw-rw-r--   0 runner    (1001) docker     (127)      742 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_import_db.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2037 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_insert.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3728 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_merge.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2803 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_set.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/scan/
--rw-rw-r--   0 runner    (1001) docker     (127)      643 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_dummy_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1290 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_expressions_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_index_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1217 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_scan_file.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1089 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_scan_internal_id.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1486 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_scan_node_property.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6001 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/schema.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/sip/
--rw-rw-r--   0 runner    (1001) docker     (127)     1588 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/sip/logical_semi_masker.h
--rw-rw-r--   0 runner    (1001) docker     (127)      308 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/operator/sip/side_way_info_passing.h
--rw-rw-r--   0 runner    (1001) docker     (127)    16498 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/planner.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3416 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/planner/subplans_table.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/
--rw-rw-r--   0 runner    (1001) docker     (127)     1252 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/data_pos.h
--rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/execution_context.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2051 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/expression_mapper.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/
--rw-rw-r--   0 runner    (1001) docker     (127)    11146 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/aggregate_hash_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1255 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/aggregate_input.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1824 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/base_aggregate.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1374 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/base_aggregate_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3698 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/hash_aggregate.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1905 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/hash_aggregate_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2811 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/simple_aggregate.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1565 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/simple_aggregate_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)      855 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/attach_database.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/call/
--rw-rw-r--   0 runner    (1001) docker     (127)     2956 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/call/in_query_call.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1382 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/call/standalone_call.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1712 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/comment_on.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2858 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/cross_product.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/ddl/
--rw-rw-r--   0 runner    (1001) docker     (127)     1402 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/ddl/alter.h
--rw-rw-r--   0 runner    (1001) docker     (127)      779 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/ddl/create_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)      945 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/ddl/ddl.h
--rw-rw-r--   0 runner    (1001) docker     (127)      777 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/ddl/drop_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)      777 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/detach_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      583 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/empty_result.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2713 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/filter.h
--rw-rw-r--   0 runner    (1001) docker     (127)      795 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/filtering_operator.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1255 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/flatten.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/hash_join/
--rw-rw-r--   0 runner    (1001) docker     (127)     4460 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/hash_join/hash_join_build.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4761 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/hash_join/hash_join_probe.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3299 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/hash_join/join_hash_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2359 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/index_lookup.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1541 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/index_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1025 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/install_extension.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/intersect/
--rw-rw-r--   0 runner    (1001) docker     (127)     3204 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/intersect/intersect.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1057 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/intersect/intersect_build.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1208 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/limit.h
--rw-rw-r--   0 runner    (1001) docker     (127)      942 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/load_extension.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/macro/
--rw-rw-r--   0 runner    (1001) docker     (127)     1852 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/macro/create_macro.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5181 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/mask.h
--rw-rw-r--   0 runner    (1001) docker     (127)      972 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/multiplicity_reducer.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/order_by/
--rw-rw-r--   0 runner    (1001) docker     (127)     7982 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/order_by/key_block_merger.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1868 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1742 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by_data_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6358 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by_key_encoder.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2060 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by_merge.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2533 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3873 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/order_by/radix_sort.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2942 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/order_by/sort_state.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6218 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/order_by/top_k.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1694 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/order_by/top_k_scanner.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5655 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/partitioner.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/
--rw-rw-r--   0 runner    (1001) docker     (127)     2873 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/batch_insert.h
--rw-rw-r--   0 runner    (1001) docker     (127)      983 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/copy_rdf.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2150 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/copy_to.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3177 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/copy_to_csv.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2821 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/copy_to_parquet.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1604 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/delete.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6124 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/delete_executor.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1005 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/export_db.h
--rw-rw-r--   0 runner    (1001) docker     (127)      840 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/file_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      734 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/import_db.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5477 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/index_builder.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1163 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/insert.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3808 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/insert_executor.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2702 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/merge.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4654 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/node_batch_insert.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/
--rw-rw-r--   0 runner    (1001) docker     (127)     2367 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/base_csv_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1831 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/driver.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1862 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/parallel_csv_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1888 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/serial_csv_reader.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/npy/
--rw-rw-r--   0 runner    (1001) docker     (127)     1754 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/npy/npy_reader.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/
--rw-rw-r--   0 runner    (1001) docker     (127)     1480 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/boolean_column_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1616 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/callback_column_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5214 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/column_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1962 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/decode_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1358 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/interval_column_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1842 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/list_column_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4613 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/parquet_dbp_decoder.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4702 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/parquet_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4238 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/parquet_rle_bp_decoder.h
--rw-rw-r--   0 runner    (1001) docker     (127)      976 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/parquet_timestamp.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1842 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/resizable_buffer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1327 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/string_column_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1262 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/struct_column_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3426 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/templated_column_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6781 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/thrift_tools.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/
--rw-rw-r--   0 runner    (1001) docker     (127)     5911 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/rdf_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7416 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/rdf_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)      380 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/rdf_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2388 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/triple_store.h
--rw-rw-r--   0 runner    (1001) docker     (127)      865 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/reader_bind_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4368 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/rel_batch_insert.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1938 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/set.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6617 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/set_executor.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/
--rw-rw-r--   0 runner    (1001) docker     (127)     3914 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/basic_column_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2248 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/boolean_column_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4075 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/column_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1063 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/interval_column_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1729 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/list_column_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1087 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/parquet_rle_bp_encoder.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3213 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/parquet_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3898 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/standard_column_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5245 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/string_column_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1711 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/struct_column_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4992 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/physical_operator.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1356 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/profile.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1518 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/projection.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/
--rw-rw-r--   0 runner    (1001) docker     (127)     2317 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/all_shortest_path_state.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3932 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/bfs_state.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1693 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/frontier.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6119 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/frontier_scanner.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4590 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/path_property_probe.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5732 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/recursive_join.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1380 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/scan_frontier.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1684 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/shortest_path_state.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1050 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/variable_length_state.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2908 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/result_collector.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/scan/
--rw-rw-r--   0 runner    (1001) docker     (127)     1769 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_multi_node_tables.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2072 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_multi_rel_tables.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2318 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_node_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2495 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_rel_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)      840 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3474 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/scan_node_id.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5060 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/semi_masker.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1777 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1435 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/skip.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/table_scan/
--rw-rw-r--   0 runner    (1001) docker     (127)     1102 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/table_scan/ftable_scan_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3006 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/table_scan/union_all_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1095 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/transaction.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1499 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/operator/unwind.h
--rw-rw-r--   0 runner    (1001) docker     (127)      388 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/physical_plan.h
--rw-rw-r--   0 runner    (1001) docker     (127)    12305 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/plan_mapper.h
--rw-rw-r--   0 runner    (1001) docker     (127)      638 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/processor.h
--rw-rw-r--   0 runner    (1001) docker     (127)      621 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/processor_task.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/result/
--rw-rw-r--   0 runner    (1001) docker     (127)     1737 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/result/base_hash_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)    16632 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/result/factorized_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1187 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/result/flat_tuple.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1061 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/result/mark_hash_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1547 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/result/result_set.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1063 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/processor/result/result_set_descriptor.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/buffer_manager/
--rw-rw-r--   0 runner    (1001) docker     (127)     9404 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/buffer_manager/bm_file_handle.h
--rw-rw-r--   0 runner    (1001) docker     (127)    13079 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/buffer_manager/buffer_manager.h
--rw-rw-r--   0 runner    (1001) docker     (127)      527 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/buffer_manager/locked_queue.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2759 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/buffer_manager/memory_manager.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1714 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/buffer_manager/vm_region.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/compression/
--rw-rw-r--   0 runner    (1001) docker     (127)    15336 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/compression/compression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1695 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/compression/sign_extend.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3328 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/file_handle.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/index/
--rw-rw-r--   0 runner    (1001) docker     (127)    10995 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/index/hash_index.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8325 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/index/hash_index_builder.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1141 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/index/hash_index_header.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2132 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/index/hash_index_slot.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2450 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/index/hash_index_utils.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/local_storage/
--rw-rw-r--   0 runner    (1001) docker     (127)     2704 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/local_storage/local_node_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3256 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/local_storage/local_rel_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1052 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/local_storage/local_storage.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8905 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/local_storage/local_table.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/stats/
--rw-rw-r--   0 runner    (1001) docker     (127)      999 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/stats/metadata_dah_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3254 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/stats/node_table_statistics.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4474 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/stats/nodes_store_statistics.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1594 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/stats/property_statistics.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3873 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/stats/rel_table_statistics.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3236 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/stats/rels_store_statistics.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1947 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/stats/table_statistics.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4425 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/stats/table_statistics_collection.h
--rw-rw-r--   0 runner    (1001) docker     (127)      821 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/storage_extension.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2909 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/storage_manager.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/storage_structure/
--rw-rw-r--   0 runner    (1001) docker     (127)     1571 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/storage_structure/db_file_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)    13833 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/storage_structure/disk_array.h
--rw-rw-r--   0 runner    (1001) docker     (127)      368 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/storage_structure/in_mem_page.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5363 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/storage_structure/overflow_file.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7895 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/storage_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)      774 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/storage_version_info.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/store/
--rw-rw-r--   0 runner    (1001) docker     (127)     4606 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/store/chunked_node_group.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1626 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/store/chunked_node_group_collection.h
--rw-rw-r--   0 runner    (1001) docker     (127)    13510 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/store/column.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9490 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/store/column_chunk.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2508 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/store/dictionary_chunk.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2908 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/store/dictionary_column.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5783 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/store/list_column.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3534 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/store/list_column_chunk.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5363 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/store/node_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1973 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/store/node_table_data.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2607 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/store/null_column.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8048 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/store/rel_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)    12143 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/store/rel_table_data.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3509 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/store/string_column.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2511 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/store/string_column_chunk.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3320 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/store/struct_column.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1968 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/store/struct_column_chunk.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3604 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/store/table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2552 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/store/table_data.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/wal/
--rw-rw-r--   0 runner    (1001) docker     (127)     3663 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/wal/wal.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8162 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/wal/wal_record.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2356 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/wal_replayer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      725 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/storage/wal_replayer_utils.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/transaction/
--rw-rw-r--   0 runner    (1001) docker     (127)     1893 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/transaction/transaction.h
--rw-rw-r--   0 runner    (1001) docker     (127)      294 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/transaction/transaction_action.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2414 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/transaction/transaction_context.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3747 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/include/transaction/transaction_manager.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/main/
--rw-rw-r--   0 runner    (1001) docker     (127)      414 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/main/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    20077 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/main/client_context.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3262 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/main/connection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11631 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/main/database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1232 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/main/database_manager.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1268 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/main/db_config.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    13980 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/main/plan_printer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      956 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/main/prepared_statement.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4090 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/main/query_result.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      578 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/main/query_summary.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3755 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/main/storage_driver.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      317 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/main/version.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/optimizer/
--rw-rw-r--   0 runner    (1001) docker     (127)      602 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/optimizer/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    10541 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/optimizer/acc_hash_join_optimizer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3540 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/optimizer/agg_key_dependency_optimizer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1488 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/optimizer/correlated_subquery_unnest_solver.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    10339 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/optimizer/factorization_rewriter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    10504 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/optimizer/filter_push_down_optimizer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      340 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/optimizer/logical_operator_collector.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5558 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/optimizer/logical_operator_visitor.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2087 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/optimizer/optimizer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    13109 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/optimizer/projection_push_down_optimizer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1201 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/optimizer/remove_factorization_rewriter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1537 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/optimizer/remove_unnecessary_join_optimizer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1902 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/optimizer/top_k_optimizer.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/
--rw-rw-r--   0 runner    (1001) docker     (127)      400 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/antlr_parser/
--rw-rw-r--   0 runner    (1001) docker     (127)      267 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/antlr_parser/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1595 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/antlr_parser/kuzu_cypher_parser.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1391 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/antlr_parser/parser_error_listener.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      827 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/antlr_parser/parser_error_strategy.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      455 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/create_macro.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/expression/
--rw-rw-r--   0 runner    (1001) docker     (127)      346 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/expression/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2127 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/expression/parsed_case_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3281 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/expression/parsed_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      785 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/expression/parsed_function_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      491 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/expression/parsed_property_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      491 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/expression/parsed_variable_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3506 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/parsed_expression_visitor.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4309 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/parsed_statement_visitor.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1259 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/parser.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/transform/
--rw-rw-r--   0 runner    (1001) docker     (127)      691 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/transform/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      646 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/transform/transform_attach_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      450 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/transform/transform_comment_on.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3602 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/transform/transform_copy.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7632 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/transform/transform_ddl.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      392 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/transform/transform_detach_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    27904 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/transform/transform_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      858 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/transform/transform_extension.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7789 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/transform/transform_graph_pattern.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1272 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/transform/transform_macro.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      833 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/transform/transform_port_db.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2587 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/transform/transform_projection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2253 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/transform/transform_query.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2715 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/transform/transform_reading_clause.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      484 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/transform/transform_standalone_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1209 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/transform/transform_transaction.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2681 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/transform/transform_updating_clause.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4394 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/transformer.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/visitor/
--rw-rw-r--   0 runner    (1001) docker     (127)      209 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/visitor/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      258 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/parser/visitor/statement_read_write_analyzer.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/
--rw-rw-r--   0 runner    (1001) docker     (127)      339 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/join_order/
--rw-rw-r--   0 runner    (1001) docker     (127)      251 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/join_order/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     5776 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/join_order/cardinality_estimator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1652 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/join_order/cost_model.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      745 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/join_order/join_order_util.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1233 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/join_order_enumerator_context.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/
--rw-rw-r--   0 runner    (1001) docker     (127)     1000 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/ddl/
--rw-rw-r--   0 runner    (1001) docker     (127)      175 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/ddl/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/ddl/logical_ddl.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/extend/
--rw-rw-r--   0 runner    (1001) docker     (127)      253 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/extend/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1348 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/extend/base_logical_extend.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1169 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/extend/logical_extend.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2914 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/extend/logical_recursive_extend.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/factorization/
--rw-rw-r--   0 runner    (1001) docker     (127)      223 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/factorization/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1007 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/factorization/flatten_resolver.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2591 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/factorization/sink_util.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1552 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/logical_accumulate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2870 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/logical_aggregate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      517 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/logical_comment_on.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      523 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/logical_create_macro.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      829 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/logical_cross_product.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1523 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/logical_distinct.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      764 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/logical_dummy_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      800 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/logical_explain.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      822 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/logical_filter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      407 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/logical_flatten.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7224 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/logical_hash_join.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      726 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/logical_in_query_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2606 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/logical_intersect.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1039 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/logical_limit.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1514 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/logical_mark_accumulate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6201 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/logical_operator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2805 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/logical_order_by.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      939 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/logical_partitioner.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1065 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/logical_plan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3973 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/logical_plan_util.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2197 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/logical_projection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1947 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/logical_union.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      980 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/logical_unwind.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/persistent/
--rw-rw-r--   0 runner    (1001) docker     (127)      388 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/persistent/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      853 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_copy_from.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      620 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_copy_to.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1732 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_delete.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      303 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_export_db.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      303 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_import_db.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2031 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_insert.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1366 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_merge.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2384 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_set.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/scan/
--rw-rw-r--   0 runner    (1001) docker     (127)      328 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/scan/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      347 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/scan/logical_expressions_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      935 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/scan/logical_index_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      643 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/scan/logical_scan_file.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      481 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/scan/logical_scan_internal_id.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      561 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/scan/logical_scan_node_property.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5563 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/operator/schema.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/plan/
--rw-rw-r--   0 runner    (1001) docker     (127)     1042 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/plan/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1329 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/plan/append_accumulate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      814 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/plan/append_aggregate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      816 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/plan/append_cross_product.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1971 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/plan/append_delete.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      553 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/plan/append_distinct.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      399 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/plan/append_dummy_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      473 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/plan/append_expressions_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    13525 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/plan/append_extend.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      913 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/plan/append_filter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      800 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/plan/append_flatten.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      740 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/plan/append_in_query_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2692 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/plan/append_insert.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4805 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/plan/append_join.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      552 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/plan/append_limit.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      658 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/plan/append_mark_accumulate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      439 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/plan/append_multiplicity_reducer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      615 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/plan/append_order_by.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1452 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/plan/append_projection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      684 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/plan/append_scan_file.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1596 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/plan/append_scan_node.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2066 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/plan/append_set.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5734 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/plan/append_simple.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/plan/append_standalone_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      826 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/plan/append_unwind.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8216 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/plan/plan_copy.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    27166 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/plan/plan_join_order.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2531 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/plan/plan_port_db.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3074 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/plan/plan_projection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5987 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/plan/plan_read.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1829 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/plan/plan_single_query.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/plan/plan_standalone_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8673 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/plan/plan_subquery.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6119 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/plan/plan_update.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3409 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/planner.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5305 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/query_planner.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3769 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/planner/subplans_table.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/
--rw-rw-r--   0 runner    (1001) docker     (127)      272 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/
--rw-rw-r--   0 runner    (1001) docker     (127)     1577 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     4774 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/create_factorized_table_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2148 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/create_result_collector.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8285 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/expression_mapper.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      702 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_acc_hash_join.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1102 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_accumulate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9380 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_aggregate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      638 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_attach_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1046 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_comment_on.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    15120 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_copy_from.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4729 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_copy_to.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_create_macro.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1880 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_cross_product.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_ddl.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6221 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_delete.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      634 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_detach_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      750 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_distinct.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1595 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_dummy_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      345 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_empty_result.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1956 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_explain.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1871 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_expressions_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6300 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_extend.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1014 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_extension.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      822 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_filter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      606 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_flatten.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5998 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_hash_join.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1217 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_in_query_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2425 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_index_scan_node.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5186 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_insert.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3182 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_intersect.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      933 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_label_filter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1344 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_limit.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      784 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_mark_accumulate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2627 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_merge.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      533 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_multiplicity_reducer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4327 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_order_by.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6873 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_path_property_probe.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2256 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_port_db.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1251 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_projection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3488 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_recursive_extend.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1457 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_scan_file.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      816 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_scan_frontier.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1090 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_scan_node.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3525 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_scan_node_property.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3246 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_semi_masker.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6610 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_set.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      982 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_standalone_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      593 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_transaction.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2083 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_union.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1096 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/map_unwind.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8226 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/map/plan_mapper.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/
--rw-rw-r--   0 runner    (1001) docker     (127)     1054 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/aggregate/
--rw-rw-r--   0 runner    (1001) docker     (127)      400 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/aggregate/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    37374 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/aggregate/aggregate_hash_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1691 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/aggregate/base_aggregate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      755 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/aggregate/base_aggregate_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5470 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/aggregate/hash_aggregate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2004 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/aggregate/hash_aggregate_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4848 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/aggregate/simple_aggregate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1344 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/aggregate/simple_aggregate_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      720 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/attach_database.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/call/
--rw-rw-r--   0 runner    (1001) docker     (127)      230 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/call/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2958 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/call/in_query_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      997 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/call/standalone_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      803 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/comment_on.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1383 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/cross_product.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/ddl/
--rw-rw-r--   0 runner    (1001) docker     (127)      256 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/ddl/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2464 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/ddl/alter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      725 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/ddl/create_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      570 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/ddl/ddl.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      504 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/ddl/drop_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      413 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/detach_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      213 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/empty_result.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2463 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/filter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1043 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/filtering_operator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1306 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/flatten.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/hash_join/
--rw-rw-r--   0 runner    (1001) docker     (127)      270 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/hash_join/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2057 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/hash_join/hash_join_build.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8290 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/hash_join/hash_join_probe.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9252 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/hash_join/join_hash_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5915 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/index_lookup.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1779 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/index_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2359 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/install_extension.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/intersect/
--rw-rw-r--   0 runner    (1001) docker     (127)      208 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/intersect/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     9664 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/intersect/intersect.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1389 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/limit.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2167 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/load_extension.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/macro/
--rw-rw-r--   0 runner    (1001) docker     (127)      217 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/macro/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      727 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/macro/create_macro.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      538 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/multiplicity_reducer.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/order_by/
--rw-rw-r--   0 runner    (1001) docker     (127)      410 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/order_by/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    16047 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/order_by/key_block_merger.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1082 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/order_by/order_by.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    14058 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/order_by/order_by_key_encoder.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1554 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/order_by/order_by_merge.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1438 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/order_by/order_by_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    12968 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/order_by/radix_sort.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9014 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/order_by/sort_state.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    12786 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/order_by/top_k.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      834 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/order_by/top_k_scanner.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7795 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/partitioner.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/
--rw-rw-r--   0 runner    (1001) docker     (127)      647 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      472 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/batch_insert.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      473 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/copy_rdf.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      760 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/copy_to.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8388 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/copy_to_csv.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1782 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/copy_to_parquet.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1751 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/delete.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5443 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/delete_executor.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3552 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/export_db.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      393 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/import_db.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4762 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/index_builder.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      861 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/insert.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7316 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/insert_executor.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3038 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/merge.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8703 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/node_batch_insert.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/
--rw-rw-r--   0 runner    (1001) docker     (127)      325 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/
--rw-rw-r--   0 runner    (1001) docker     (127)      297 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    14378 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/base_csv_reader.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4380 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/driver.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8564 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/parallel_csv_reader.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6543 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/serial_csv_reader.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/npy/
--rw-rw-r--   0 runner    (1001) docker     (127)      211 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/npy/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    13865 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/npy/npy_reader.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/
--rw-rw-r--   0 runner    (1001) docker     (127)      445 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      850 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/boolean_column_reader.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    23447 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/column_reader.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1234 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/interval_column_reader.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5995 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/list_column_reader.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    29865 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/parquet_reader.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1369 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/parquet_timestamp.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3928 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/string_column_reader.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3449 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/struct_column_reader.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/
--rw-rw-r--   0 runner    (1001) docker     (127)      254 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    13988 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/rdf_reader.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    13452 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/rdf_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2966 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/rdf_utils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2052 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/reader_bind_utils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11355 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/rel_batch_insert.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      997 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/set.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6592 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/set_executor.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/
--rw-rw-r--   0 runner    (1001) docker     (127)      564 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    12826 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/basic_column_writer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1538 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/boolean_column_writer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    16464 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/column_writer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1539 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/interval_column_writer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4734 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/list_column_writer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2633 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/parquet_rle_bp_encoder.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11697 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/parquet_writer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8703 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/string_column_writer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4078 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/struct_column_writer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8457 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/physical_operator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1033 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/profile.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1757 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/projection.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/
--rw-rw-r--   0 runner    (1001) docker     (127)      337 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      790 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/frontier.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6736 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/frontier_scanner.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5067 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/path_property_probe.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    12653 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/recursive_join.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      323 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/scan_frontier.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2479 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/result_collector.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/scan/
--rw-rw-r--   0 runner    (1001) docker     (127)      323 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/scan/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      825 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/scan/scan_multi_node_tables.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3865 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/scan/scan_multi_rel_tables.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      625 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/scan/scan_node_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      651 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/scan/scan_rel_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      463 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/scan/scan_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5110 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/scan_node_id.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4582 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/semi_masker.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2403 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/skip.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/table_scan/
--rw-rw-r--   0 runner    (1001) docker     (127)      248 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/table_scan/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2486 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/table_scan/ftable_scan_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1832 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/table_scan/union_all_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1256 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/transaction.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2659 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/operator/unwind.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2709 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/processor.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1788 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/processor_task.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/result/
--rw-rw-r--   0 runner    (1001) docker     (127)      336 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/result/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     7142 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/result/base_hash_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    34515 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/result/factorized_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2119 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/result/flat_tuple.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2304 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/result/mark_hash_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1494 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/result/result_set.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1170 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/processor/result/result_set_descriptor.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/
--rw-rw-r--   0 runner    (1001) docker     (127)      537 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/buffer_manager/
--rw-rw-r--   0 runner    (1001) docker     (127)      277 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/buffer_manager/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     7039 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/buffer_manager/bm_file_handle.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    15692 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/buffer_manager/buffer_manager.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2101 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/buffer_manager/memory_manager.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3721 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/buffer_manager/vm_region.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/compression/
--rw-rw-r--   0 runner    (1001) docker     (127)      258 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/compression/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    35565 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/compression/compression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1880 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/file_handle.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/index/
--rw-rw-r--   0 runner    (1001) docker     (127)      210 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/index/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    19280 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/index/hash_index.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    13484 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/index/hash_index_builder.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/local_storage/
--rw-rw-r--   0 runner    (1001) docker     (127)      279 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/local_storage/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     8095 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/local_storage/local_node_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    12529 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/local_storage/local_rel_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1723 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/local_storage/local_storage.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5406 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/local_storage/local_table.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/stats/
--rw-rw-r--   0 runner    (1001) docker     (127)      415 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/stats/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1201 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/stats/metadata_dah_info.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7957 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/stats/node_table_statistics.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4352 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/stats/nodes_store_statistics.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2446 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/stats/property_statistics.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5129 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/stats/rel_table_statistics.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4017 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/stats/rels_store_statistics.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2843 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/stats/table_statistics.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5914 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/stats/table_statistics_collection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    10057 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/storage_manager.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/storage_structure/
--rw-rw-r--   0 runner    (1001) docker     (127)      263 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/storage_structure/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     5596 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/storage_structure/db_file_utils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    20740 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/storage_structure/disk_array.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      557 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/storage_structure/in_mem_page.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9484 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/storage_structure/overflow_file.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4286 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/storage_utils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      737 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/storage_version_info.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/store/
--rw-rw-r--   0 runner    (1001) docker     (127)      649 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/store/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     6855 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/store/chunked_node_group.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2126 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/store/chunked_node_group_collection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    44076 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/store/column.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    28200 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/store/column_chunk.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3687 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/store/dictionary_chunk.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    10487 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/store/dictionary_column.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    22685 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/store/list_column.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    16128 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/store/list_column_chunk.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9981 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/store/node_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4163 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/store/node_table_data.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9068 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/store/null_column.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8480 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/store/rel_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    48499 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/store/rel_table_data.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11550 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/store/string_column.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7843 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/store/string_column_chunk.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11743 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/store/struct_column.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6206 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/store/struct_column_chunk.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1779 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/store/table_data.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/wal/
--rw-rw-r--   0 runner    (1001) docker     (127)      191 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/wal/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     6348 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/wal/wal.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6783 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/wal/wal_record.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    17846 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/wal_replayer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1169 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/storage/wal_replayer_utils.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/transaction/
--rw-rw-r--   0 runner    (1001) docker     (127)      216 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/transaction/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     3894 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/transaction/transaction_context.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4629 2024-04-15 08:03:54.000000 sdist/kuzu-source/src/transaction/transaction_manager.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/
--rw-rw-r--   0 runner    (1001) docker     (127)      436 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_cypher/
--rw-rw-r--   0 runner    (1001) docker     (127)      949 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_cypher/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    56460 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_cypher/cypher_lexer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)   467402 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_cypher/cypher_parser.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_cypher/include/
--rw-rw-r--   0 runner    (1001) docker     (127)     3261 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_cypher/include/cypher_lexer.h
--rw-rw-r--   0 runner    (1001) docker     (127)    87738 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_cypher/include/cypher_parser.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/
--rw-rw-r--   0 runner    (1001) docker     (127)    10564 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     4237 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/LICENSE
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/
--rw-rw-r--   0 runner    (1001) docker     (127)      285 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRErrorListener.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     8375 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRErrorListener.h
--rw-rw-r--   0 runner    (1001) docker     (127)      285 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRErrorStrategy.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     5269 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRErrorStrategy.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      552 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRFileStream.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1018 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRFileStream.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     4326 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRInputStream.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2623 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRInputStream.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1804 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BailErrorStrategy.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2483 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BailErrorStrategy.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1163 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BaseErrorListener.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1377 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BaseErrorListener.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     9946 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BufferedTokenStream.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     8014 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BufferedTokenStream.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      281 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CharStream.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1479 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CharStream.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     4459 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonToken.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     4918 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonToken.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1327 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonTokenFactory.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2564 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonTokenFactory.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1767 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonTokenStream.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2713 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonTokenStream.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      597 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ConsoleErrorListener.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1060 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ConsoleErrorListener.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    11864 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/DefaultErrorStrategy.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)    20289 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/DefaultErrorStrategy.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     3484 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/DiagnosticErrorListener.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3600 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/DiagnosticErrorListener.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2152 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Exceptions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3868 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Exceptions.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1867 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/FailedPredicateException.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1096 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/FailedPredicateException.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2767 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/FlatHashMap.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2676 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/FlatHashSet.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      559 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/InputMismatchException.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      783 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/InputMismatchException.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      350 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/IntStream.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)    10251 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/IntStream.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      615 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/InterpreterRuleContext.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1604 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/InterpreterRuleContext.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     6878 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Lexer.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     7038 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Lexer.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1867 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/LexerInterpreter.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1564 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/LexerInterpreter.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1234 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/LexerNoViableAltException.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      916 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/LexerNoViableAltException.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     2412 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ListTokenSource.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3795 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ListTokenSource.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1585 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/NoViableAltException.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1693 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/NoViableAltException.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    19305 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Parser.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)    19393 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Parser.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    10523 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ParserInterpreter.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     7171 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ParserInterpreter.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     3952 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ParserRuleContext.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     5666 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ParserRuleContext.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1958 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ProxyErrorListener.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1657 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ProxyErrorListener.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1916 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RecognitionException.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3961 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RecognitionException.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     4572 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Recognizer.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     5733 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Recognizer.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     3588 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuleContext.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     5561 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuleContext.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      725 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuleContextWithAltNum.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      985 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuleContextWithAltNum.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     2091 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuntimeMetaData.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     7393 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuntimeMetaData.h
--rw-rw-r--   0 runner    (1001) docker     (127)      246 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Token.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3462 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Token.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1217 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenFactory.h
--rw-rw-r--   0 runner    (1001) docker     (127)      264 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenSource.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3839 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenSource.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      284 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenStream.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     6098 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenStream.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    15023 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenStreamRewriter.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)    12507 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenStreamRewriter.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     5847 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/UnbufferedCharStream.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     4351 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/UnbufferedCharStream.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     7467 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/UnbufferedTokenStream.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     4241 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/UnbufferedTokenStream.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2105 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Version.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1907 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Vocabulary.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     6943 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Vocabulary.h
--rw-rw-r--   0 runner    (1001) docker     (127)      270 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/WritableToken.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      676 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/WritableToken.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2560 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/antlr4-common.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5524 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/antlr4-runtime.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/
--rwxrwxr-x   0 runner    (1001) docker     (127)     4193 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATN.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     4845 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATN.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     4158 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNConfig.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     5513 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNConfig.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     6500 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNConfigSet.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     5185 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNConfigSet.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1252 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNDeserializationOptions.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1302 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNDeserializationOptions.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    21573 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNDeserializer.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      835 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNDeserializer.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1216 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNSimulator.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2761 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNSimulator.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1538 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNState.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     4374 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNState.h
--rw-rw-r--   0 runner    (1001) docker     (127)      990 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNStateType.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      796 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNStateType.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      439 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNType.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1214 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ActionTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1104 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ActionTransition.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      604 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/AmbiguityInfo.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3295 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/AmbiguityInfo.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     4211 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ArrayPredictionContext.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1900 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ArrayPredictionContext.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      840 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/AtomTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1084 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/AtomTransition.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      729 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/BasicBlockStartState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      649 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/BasicState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      762 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/BlockEndState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      853 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/BlockStartState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      520 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ContextSensitivityInfo.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2123 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ContextSensitivityInfo.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      561 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionEventInfo.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2459 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionEventInfo.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      934 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionInfo.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     9762 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionInfo.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      342 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionState.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      960 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      969 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/EpsilonTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1402 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/EpsilonTransition.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      527 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ErrorInfo.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1861 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ErrorInfo.h
--rw-rw-r--   0 runner    (1001) docker     (127)      416 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/HashUtils.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     7271 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LL1Analyzer.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3275 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LL1Analyzer.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     2950 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerATNConfig.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1666 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerATNConfig.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    22025 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerATNSimulator.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     8819 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerATNSimulator.h
--rw-rw-r--   0 runner    (1001) docker     (127)      324 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3494 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     4031 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerActionExecutor.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     6150 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerActionExecutor.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1460 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerActionType.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1306 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerChannelAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1908 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerChannelAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1555 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerCustomAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2772 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerCustomAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1784 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerIndexedCustomAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3046 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerIndexedCustomAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1269 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerModeAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1780 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerModeAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      977 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerMoreAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1701 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerMoreAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1010 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerPopModeAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1735 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerPopModeAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1311 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerPushModeAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1817 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerPushModeAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      977 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerSkipAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1664 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerSkipAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1269 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerTypeAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1717 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerTypeAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      584 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LookaheadEventInfo.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1914 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LookaheadEventInfo.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      736 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LoopEndState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      868 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/NotSetTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      854 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/NotSetTransition.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      484 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/OrderedATNConfigSet.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      631 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/OrderedATNConfigSet.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     2789 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParseInfo.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3665 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParseInfo.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    53167 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParserATNSimulator.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)    45705 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParserATNSimulator.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2278 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParserATNSimulatorOptions.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1052 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PlusBlockStartState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      842 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PlusLoopbackState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      901 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PrecedencePredicateTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1187 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PrecedencePredicateTransition.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      685 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredicateEvalInfo.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2885 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredicateEvalInfo.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1009 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredicateTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1674 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredicateTransition.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    20987 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContext.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     9173 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContext.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2360 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextCache.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2738 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextCache.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5386 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextMergeCache.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4033 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextMergeCache.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2602 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextMergeCacheOptions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextType.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     5939 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionMode.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)    20991 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionMode.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     7943 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ProfilingATNSimulator.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2982 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ProfilingATNSimulator.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      891 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RangeTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      944 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RangeTransition.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      746 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RuleStartState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      911 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RuleStopState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1156 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RuleTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1484 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RuleTransition.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    14979 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SemanticContext.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     9030 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SemanticContext.h
--rw-rw-r--   0 runner    (1001) docker     (127)      451 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SemanticContextType.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3246 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SerializedATNView.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      898 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SetTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1267 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SetTransition.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     2870 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SingletonPredictionContext.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1834 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SingletonPredictionContext.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      754 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/StarBlockStartState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1140 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/StarLoopEntryState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      644 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/StarLoopbackState.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      733 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/StarLoopbackState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      762 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/TokensStartState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      911 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/Transition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2164 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/Transition.h
--rw-rw-r--   0 runner    (1001) docker     (127)      730 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/TransitionType.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      778 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/TransitionType.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      680 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/WildcardTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      839 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/WildcardTransition.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/
--rwxrwxr-x   0 runner    (1001) docker     (127)     2868 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFA.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3045 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFA.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1726 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFASerializer.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      772 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFASerializer.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1490 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFAState.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     6068 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFAState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      509 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/LexerDFASerializer.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      533 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/LexerDFASerializer.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/internal/
--rw-rw-r--   0 runner    (1001) docker     (127)     2694 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/internal/Synchronization.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5499 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/internal/Synchronization.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/
--rwxrwxr-x   0 runner    (1001) docker     (127)     3098 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/InterpreterDataReader.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      989 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/InterpreterDataReader.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1671 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/Interval.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3009 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/Interval.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    13209 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/IntervalSet.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     6478 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/IntervalSet.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     2820 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/MurmurHash.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3595 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/MurmurHash.h
--rw-rw-r--   0 runner    (1001) docker     (127)       71 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/Predicate.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      446 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/Predicate.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/
--rw-rw-r--   0 runner    (1001) docker     (127)      242 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Any.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      370 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Any.h
--rw-rw-r--   0 runner    (1001) docker     (127)      966 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Arrays.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3620 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Arrays.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1828 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/BitSet.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     4837 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/CPPUtils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2582 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/CPPUtils.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1195 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Casts.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4122 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Declarations.h
--rw-rw-r--   0 runner    (1001) docker     (127)      901 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/StringUtils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      425 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/StringUtils.h
--rw-rw-r--   0 runner    (1001) docker     (127)      723 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Unicode.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8728 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Utf8.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2148 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Utf8.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/
--rwxrwxr-x   0 runner    (1001) docker     (127)     5650 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/AbstractParseTreeVisitor.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      677 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ErrorNode.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1255 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ErrorNodeImpl.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1429 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ErrorNodeImpl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1906 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/IterativeParseTreeWalker.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2124 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/IterativeParseTreeWalker.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      349 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTree.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     4224 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTree.h
--rw-rw-r--   0 runner    (1001) docker     (127)      288 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeListener.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1213 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeListener.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1434 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeProperty.h
--rw-rw-r--   0 runner    (1001) docker     (127)      430 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeType.h
--rw-rw-r--   0 runner    (1001) docker     (127)      285 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeVisitor.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2212 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeVisitor.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1381 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeWalker.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2031 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeWalker.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1145 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/TerminalNode.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1281 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/TerminalNodeImpl.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1003 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/TerminalNodeImpl.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     6872 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/Trees.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3060 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/Trees.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/
--rw-rw-r--   0 runner    (1001) docker     (127)      274 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/Chunk.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1460 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/Chunk.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1868 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreeMatch.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     5768 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreeMatch.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1800 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreePattern.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     4384 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreePattern.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    12574 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreePatternMatcher.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     8715 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreePatternMatcher.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1820 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/RuleTagToken.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     4742 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/RuleTagToken.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      811 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TagChunk.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3030 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TagChunk.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      623 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TextChunk.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1464 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TextChunk.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      959 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TokenTagToken.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2786 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TokenTagToken.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/
--rwxrwxr-x   0 runner    (1001) docker     (127)     4960 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPath.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2824 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPath.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      747 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathElement.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1029 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathElement.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6047 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1169 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexer.g4
--rw-rw-r--   0 runner    (1001) docker     (127)     1349 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexer.h
--rw-rw-r--   0 runner    (1001) docker     (127)       98 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexer.tokens
--rwxrwxr-x   0 runner    (1001) docker     (127)      506 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexerErrorListener.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      635 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexerErrorListener.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      647 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathRuleAnywhereElement.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      709 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathRuleAnywhereElement.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      966 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathRuleElement.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      620 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathRuleElement.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      647 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathTokenAnywhereElement.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      631 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathTokenAnywhereElement.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1054 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathTokenElement.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      623 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathTokenElement.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      665 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathWildcardAnywhereElement.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      558 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathWildcardAnywhereElement.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      621 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathWildcardElement.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      542 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathWildcardElement.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/fast_float/
--rw-rw-r--   0 runner    (1001) docker     (127)       92 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/fast_float/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/fast_float/include/
--rw-rw-r--   0 runner    (1001) docker     (127)    94376 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/fast_float/include/fast_float.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/fastpfor/
--rw-rw-r--   0 runner    (1001) docker     (127)      150 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/fastpfor/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    10273 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/fastpfor/LICENSE
--rw-rw-r--   0 runner    (1001) docker     (127)     1278 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/fastpfor/README
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/
--rw-rw-r--   0 runner    (1001) docker     (127)    59414 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/bitpacking.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    32124 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/bitpacking.h
--rw-rw-r--   0 runner    (1001) docker     (127)    23572 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/bitpackinghelpers.h
--rw-rw-r--   0 runner    (1001) docker     (127)      273 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/common.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/glob/
--rw-rw-r--   0 runner    (1001) docker     (127)      100 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/glob/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/glob/glob/
--rw-rw-r--   0 runner    (1001) docker     (127)    13001 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/glob/glob/glob.hpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/httplib/
--rw-rw-r--   0 runner    (1001) docker     (127)   311527 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/httplib/httplib.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/
--rw-rw-r--   0 runner    (1001) docker     (127)      918 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    11358 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/LICENSE
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/include/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/
--rw-rw-r--   0 runner    (1001) docker     (127)    26550 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/aes.h
--rw-rw-r--   0 runner    (1001) docker     (127)    15024 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/aria.h
--rw-rw-r--   0 runner    (1001) docker     (127)    25694 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/asn1.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3085 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/base64.h
--rw-rw-r--   0 runner    (1001) docker     (127)    42463 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/bignum.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2394 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/build_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)    13062 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/camellia.h
--rw-rw-r--   0 runner    (1001) docker     (127)    25326 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/ccm.h
--rw-rw-r--   0 runner    (1001) docker     (127)    38245 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/check_config.h
--rw-rw-r--   0 runner    (1001) docker     (127)    51905 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/cipher.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1452 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/constant_time.h
--rw-rw-r--   0 runner    (1001) docker     (127)    11057 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/des.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9867 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/entropy.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7031 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/error.h
--rw-rw-r--   0 runner    (1001) docker     (127)    16632 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/gcm.h
--rw-rw-r--   0 runner    (1001) docker     (127)      531 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/mbedtls_config.h
--rw-rw-r--   0 runner    (1001) docker     (127)    17120 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/md.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4949 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/memory_buffer_alloc.h
--rw-rw-r--   0 runner    (1001) docker     (127)    41167 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/oid.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5270 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/pem.h
--rw-rw-r--   0 runner    (1001) docker     (127)    35543 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/pk.h
--rw-rw-r--   0 runner    (1001) docker     (127)    14433 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/platform.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1973 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/platform_time.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8667 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/platform_util.h
--rw-rw-r--   0 runner    (1001) docker     (127)      978 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/private_access.h
--rw-rw-r--   0 runner    (1001) docker     (127)    51957 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/rsa.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7854 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/sha1.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6640 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/sha256.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7084 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/sha512.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/library/
--rw-rw-r--   0 runner    (1001) docker     (127)    73166 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/library/aes.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    36996 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/library/aria.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11007 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/library/asn1parse.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6762 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/library/base64.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    79733 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/library/bignum.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    56414 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/library/bn_mul.h
--rw-rw-r--   0 runner    (1001) docker     (127)    36100 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/library/camellia.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    47452 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/library/cipher.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    49271 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/library/cipher_wrap.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4532 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/library/cipher_wrap.h
--rw-rw-r--   0 runner    (1001) docker     (127)    17543 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/library/common.h
--rw-rw-r--   0 runner    (1001) docker     (127)    26144 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/library/constant_time.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    12167 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/library/constant_time_internal.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1638 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/library/constant_time_invasive.h
--rw-rw-r--   0 runner    (1001) docker     (127)    18774 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/library/entropy.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6513 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/library/entropy_poll.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2139 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/library/entropy_poll.h
--rw-rw-r--   0 runner    (1001) docker     (127)    34742 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/library/gcm.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    21294 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/library/md.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2086 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/library/md_wrap.h
--rw-rw-r--   0 runner    (1001) docker     (127)    27822 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/library/oid.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    14294 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/library/pem.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    17719 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/library/pk.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    29099 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/library/pk_wrap.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4205 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/library/pk_wrap.h
--rw-rw-r--   0 runner    (1001) docker     (127)    44156 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/library/pkparse.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5125 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/library/platform_util.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    69416 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/library/rsa.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    13253 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/library/rsa_alt_helpers.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8442 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/library/rsa_alt_helpers.h
--rw-rw-r--   0 runner    (1001) docker     (127)    15171 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/library/sha1.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    16212 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/library/sha256.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    18253 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/mbedtls/library/sha512.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/
--rw-rw-r--   0 runner    (1001) docker     (127)     1079 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       46 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/LICENSE
--rw-rw-r--   0 runner    (1001) docker     (127)      976 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/Makefile
--rw-rw-r--   0 runner    (1001) docker     (127)     1879 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/README.md
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/
--rw-rw-r--   0 runner    (1001) docker     (127)      320 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/parquet_constants.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      406 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/parquet_constants.h
--rw-rw-r--   0 runner    (1001) docker     (127)   200148 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/parquet_types.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    72715 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/parquet_types.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1262 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/windows_compatibility.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/
--rwxrwxr-x   0 runner    (1001) docker     (127)     9816 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-internal.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     3296 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-sinksource.cc
--rwxrwxr-x   0 runner    (1001) docker     (127)     7266 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-sinksource.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1837 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-stubs-internal.cc
--rwxrwxr-x   0 runner    (1001) docker     (127)    15040 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-stubs-internal.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     2900 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-stubs-public.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    59102 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy.cc
--rwxrwxr-x   0 runner    (1001) docker     (127)     9748 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/
--rw-rw-r--   0 runner    (1001) docker     (127)     3555 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/TApplicationException.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1208 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/TBase.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     6849 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/TLogging.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     3185 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/TToString.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     3290 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/Thrift.h
--rw-rw-r--   0 runner    (1001) docker     (127)       65 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/config.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/
--rwxrwxr-x   0 runner    (1001) docker     (127)     7931 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TCompactProtocol.h
--rw-rw-r--   0 runner    (1001) docker     (127)    23953 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TCompactProtocol.tcc
--rwxrwxr-x   0 runner    (1001) docker     (127)     1140 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocol.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)    21319 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocol.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     6374 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocolDecorator.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     3216 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocolException.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1151 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocolTypes.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    18266 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TVirtualProtocol.h
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/stdcxx.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      896 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/thrift-config.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      460 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/thrift_export.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/
--rw-rw-r--   0 runner    (1001) docker     (127)     4624 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/PlatformSocket.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     3699 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TBufferTransports.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)    15004 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TBufferTransports.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     9004 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TTransport.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1862 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TTransportException.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3335 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TTransportException.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     5167 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TVirtualTransport.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniz/
--rw-rw-r--   0 runner    (1001) docker     (127)      192 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniz/CMakeLists.txt
--rwxrwxr-x   0 runner    (1001) docker     (127)     1184 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniz/LICENSE
--rwxrwxr-x   0 runner    (1001) docker     (127)   313123 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniz/miniz.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)    66103 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniz/miniz.hpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5058 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/miniz/miniz_wrapper.hpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/nlohmann_json/
--rw-rw-r--   0 runner    (1001) docker     (127)   907860 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/nlohmann_json/json.hpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6268 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/nlohmann_json/json_fwd.hpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pcg/
--rw-rw-r--   0 runner    (1001) docker     (127)     1092 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pcg/LICENSE
--rw-rw-r--   0 runner    (1001) docker     (127)    20241 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pcg/pcg_extras.hpp
--rw-rw-r--   0 runner    (1001) docker     (127)    73551 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pcg/pcg_random.hpp
--rw-rw-r--   0 runner    (1001) docker     (127)    24875 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pcg/pcg_uint128.hpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/
--rw-rw-r--   0 runner    (1001) docker     (127)    11983 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1684 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/LICENSE
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/include/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/
--rw-rw-r--   0 runner    (1001) docker     (127)    23979 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/attr.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7069 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/buffer_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)    65560 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/cast.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8458 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/chrono.h
--rw-rw-r--   0 runner    (1001) docker     (127)      120 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/common.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2096 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/complex.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/
--rw-rw-r--   0 runner    (1001) docker     (127)    28251 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/class.h
--rw-rw-r--   0 runner    (1001) docker     (127)    52330 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/common.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5491 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/descr.h
--rw-rw-r--   0 runner    (1001) docker     (127)    17932 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/init.h
--rw-rw-r--   0 runner    (1001) docker     (127)    26305 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/internals.h
--rw-rw-r--   0 runner    (1001) docker     (127)    42266 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/type_caster_base.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1625 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/typeid.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eigen/
--rw-rw-r--   0 runner    (1001) docker     (127)    31418 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eigen/matrix.h
--rw-rw-r--   0 runner    (1001) docker     (127)    18120 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eigen/tensor.h
--rw-rw-r--   0 runner    (1001) docker     (127)      316 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eigen.h
--rw-rw-r--   0 runner    (1001) docker     (127)    11889 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/embed.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4731 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eval.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5002 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/functional.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8262 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/gil.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8862 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/iostream.h
--rw-rw-r--   0 runner    (1001) docker     (127)    79412 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/numpy.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9103 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/operators.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/options.h
--rw-rw-r--   0 runner    (1001) docker     (127)   126075 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/pybind11.h
--rw-rw-r--   0 runner    (1001) docker     (127)    93433 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/pytypes.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/stl/
--rw-rw-r--   0 runner    (1001) docker     (127)     4185 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/stl/filesystem.h
--rw-rw-r--   0 runner    (1001) docker     (127)    15337 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/stl.h
--rw-rw-r--   0 runner    (1001) docker     (127)    27013 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/stl_bind.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/tools/
--rw-rw-r--   0 runner    (1001) docker     (127)     2350 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/tools/FindCatch.cmake
--rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/tools/FindEigen3.cmake
--rw-rw-r--   0 runner    (1001) docker     (127)    11103 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/tools/FindPythonLibsNew.cmake
--rw-rw-r--   0 runner    (1001) docker     (127)      817 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/tools/JoinPaths.cmake
--rw-rw-r--   0 runner    (1001) docker     (127)     1423 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/tools/check-style.sh
--rw-rw-r--   0 runner    (1001) docker     (127)      952 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/tools/cmake_uninstall.cmake.in
--rw-rw-r--   0 runner    (1001) docker     (127)     1040 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/tools/codespell_ignore_lines_from_errors.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1031 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/tools/libsize.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1282 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/tools/make_changelog.py
--rw-rw-r--   0 runner    (1001) docker     (127)      196 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11.pc.in
--rw-rw-r--   0 runner    (1001) docker     (127)    13487 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11Common.cmake
--rw-rw-r--   0 runner    (1001) docker     (127)     6930 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11Config.cmake.in
--rw-rw-r--   0 runner    (1001) docker     (127)     8957 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11NewTools.cmake
--rw-rw-r--   0 runner    (1001) docker     (127)     8361 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11Tools.cmake
--rw-rw-r--   0 runner    (1001) docker     (127)       94 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/tools/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)     2104 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/tools/setup_global.py.in
--rw-rw-r--   0 runner    (1001) docker     (127)     1234 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pybind11/tools/setup_main.py.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pyparse/
--rw-rw-r--   0 runner    (1001) docker     (127)     4660 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/pyparse/pyparse.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/
--rw-rw-r--   0 runner    (1001) docker     (127)     2716 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1558 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/LICENSE
--rw-rw-r--   0 runner    (1001) docker     (127)    12166 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/bitstate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    40923 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/compile.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    77669 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/dfa.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3379 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/filtered_re2.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/include/
--rw-rw-r--   0 runner    (1001) docker     (127)     2794 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/include/bitmap256.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4074 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/include/filtered_re2.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3685 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/include/logging.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1027 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/include/mix.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4596 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/include/mutex.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1051 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/include/pod_array.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4107 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/include/prefilter.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5397 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/include/prefilter_tree.h
--rw-rw-r--   0 runner    (1001) docker     (127)    20055 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/include/prog.h
--rw-rw-r--   0 runner    (1001) docker     (127)    41735 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/include/re2.h
--rw-rw-r--   0 runner    (1001) docker     (127)    25053 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/include/regexp.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2528 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/include/set.h
--rw-rw-r--   0 runner    (1001) docker     (127)    12285 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/include/sparse_array.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7425 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/include/sparse_set.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6625 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/include/stringpiece.h
--rw-rw-r--   0 runner    (1001) docker     (127)      644 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/include/strutil.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2606 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/include/unicode_casefold.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1595 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/include/unicode_groups.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1575 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/include/utf.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1028 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/include/util.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7825 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/include/walker-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6308 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/mimics_pcre.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    22890 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/nfa.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    22239 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/onepass.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    81544 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/parse.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3448 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/perl_groups.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    18698 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/prefilter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    13255 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/prefilter_tree.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    40537 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/prog.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    42418 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/re2.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    28640 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/regexp.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5872 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/rune.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4636 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/set.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    20853 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/simplify.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2118 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/stringpiece.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5691 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/strutil.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9029 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/tostring.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    13413 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/unicode_casefold.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)   122482 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/re2/unicode_groups.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/serd/
--rw-rw-r--   0 runner    (1001) docker     (127)     1247 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/serd/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/serd/include/
--rw-rw-r--   0 runner    (1001) docker     (127)    33294 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/serd/include/serd.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/serd/src/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/serd/src/LICENSES/
--rw-rw-r--   0 runner    (1001) docker     (127)     1424 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/serd/src/LICENSES/BSD-3-Clause.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      660 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/serd/src/LICENSES/OBSD.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      555 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/serd/src/attributes.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3172 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/serd/src/base64.c
--rw-rw-r--   0 runner    (1001) docker     (127)     1024 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/serd/src/base64.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1966 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/serd/src/byte_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2643 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/serd/src/byte_source.c
--rw-rw-r--   0 runner    (1001) docker     (127)     3444 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/serd/src/byte_source.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6676 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/serd/src/env.c
--rw-rw-r--   0 runner    (1001) docker     (127)    46487 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/serd/src/n3.c
--rw-rw-r--   0 runner    (1001) docker     (127)     9699 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/serd/src/node.c
--rw-rw-r--   0 runner    (1001) docker     (127)      871 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/serd/src/node.h
--rw-rw-r--   0 runner    (1001) docker     (127)    12064 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/serd/src/reader.c
--rw-rw-r--   0 runner    (1001) docker     (127)     4376 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/serd/src/reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3187 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/serd/src/serd_config.h
--rw-rw-r--   0 runner    (1001) docker     (127)      730 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/serd/src/serd_internal.h
--rw-rw-r--   0 runner    (1001) docker     (127)    10745 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/serd/src/serdi.c
--rw-rw-r--   0 runner    (1001) docker     (127)     2552 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/serd/src/stack.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3507 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/serd/src/string.c
--rw-rw-r--   0 runner    (1001) docker     (127)     3394 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/serd/src/string_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1233 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/serd/src/system.c
--rw-rw-r--   0 runner    (1001) docker     (127)      650 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/serd/src/system.h
--rw-rw-r--   0 runner    (1001) docker     (127)      546 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/serd/src/try.h
--rw-rw-r--   0 runner    (1001) docker     (127)    11749 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/serd/src/uri.c
--rw-rw-r--   0 runner    (1001) docker     (127)     2843 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/serd/src/uri_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)    36427 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/serd/src/writer.c
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/
--rw-rw-r--   0 runner    (1001) docker     (127)     1348 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/LICENSE
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/
--rw-rw-r--   0 runner    (1001) docker     (127)     4021 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/async.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2817 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/async_logger-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2560 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/async_logger.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/
--rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/argv.h
--rw-rw-r--   0 runner    (1001) docker     (127)      986 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/env.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3170 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/helpers-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)      718 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/helpers.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2050 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/common-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)    13194 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/common.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/
--rw-rw-r--   0 runner    (1001) docker     (127)     2004 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/backtracer-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1165 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/backtracer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3349 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/circular_q.h
--rw-rw-r--   0 runner    (1001) docker     (127)      603 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/console_globals.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4707 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/file_helper-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1758 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/file_helper.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4471 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/fmt_helper.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1396 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/log_msg-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1204 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/log_msg.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1668 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/log_msg_buffer-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)      935 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/log_msg_buffer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5285 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/mpmc_blocking_q.h
--rw-rw-r--   0 runner    (1001) docker     (127)      930 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/null_mutex.h
--rw-rw-r--   0 runner    (1001) docker     (127)    17897 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/os-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3922 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/os.h
--rw-rw-r--   0 runner    (1001) docker     (127)      620 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/periodic_worker-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1756 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/periodic_worker.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8695 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/registry-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4013 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/registry.h
--rw-rw-r--   0 runner    (1001) docker     (127)      751 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/synchronous_factory.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4252 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/tcp_client-windows.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3885 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/tcp_client.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4275 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/thread_pool-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3519 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/thread_pool.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3134 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/udp_client-windows.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2237 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/udp_client.h
--rw-rw-r--   0 runner    (1001) docker     (127)      188 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/windows_include.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/
--rw-rw-r--   0 runner    (1001) docker     (127)     7380 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bin_to_hex.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/
--rw-rw-r--   0 runner    (1001) docker     (127)     7420 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/args.h
--rw-rw-r--   0 runner    (1001) docker     (127)    68076 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/chrono.h
--rw-rw-r--   0 runner    (1001) docker     (127)    24896 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/color.h
--rw-rw-r--   0 runner    (1001) docker     (127)    21245 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/compile.h
--rw-rw-r--   0 runner    (1001) docker     (127)   111215 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/core.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1408 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/fmt.license.rst
--rw-rw-r--   0 runner    (1001) docker     (127)    74272 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/format-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)   154181 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/format.h
--rw-rw-r--   0 runner    (1001) docker     (127)      100 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/locale.h
--rw-rw-r--   0 runner    (1001) docker     (127)    14123 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/os.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7586 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/ostream.h
--rw-rw-r--   0 runner    (1001) docker     (127)    20023 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/printf.h
--rw-rw-r--   0 runner    (1001) docker     (127)    23218 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/ranges.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4880 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/std.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9001 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/xchar.h
--rw-rw-r--   0 runner    (1001) docker     (127)      551 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/chrono.h
--rw-rw-r--   0 runner    (1001) docker     (127)      559 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/compile.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1042 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/fmt.h
--rw-rw-r--   0 runner    (1001) docker     (127)      554 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/ostr.h
--rw-rw-r--   0 runner    (1001) docker     (127)      551 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/ranges.h
--rw-rw-r--   0 runner    (1001) docker     (127)      641 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/std.h
--rw-rw-r--   0 runner    (1001) docker     (127)      548 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/xchar.h
--rw-rw-r--   0 runner    (1001) docker     (127)      463 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/formatter.h
--rw-rw-r--   0 runner    (1001) docker     (127)      305 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fwd.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6725 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/logger-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)    13412 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/logger.h
--rw-rw-r--   0 runner    (1001) docker     (127)    44468 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/pattern_formatter-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3758 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/pattern_formatter.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/
--rw-rw-r--   0 runner    (1001) docker     (127)     4777 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/android_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4875 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/ansicolor_sink-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3959 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/ansicolor_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1808 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/base_sink-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1568 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/base_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1216 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/basic_file_sink-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2295 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/basic_file_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1705 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/callback_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9452 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/daily_file_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2373 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/dist_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3243 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/dup_filter_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7121 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/hourly_file_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4445 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/kafka_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4003 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/mongo_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2049 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/msvc_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1234 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/null_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1222 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/ostream_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)    12408 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/qt_sinks.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2081 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/ringbuffer_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4917 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/rotating_file_sink-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3229 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/rotating_file_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)      725 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/sink-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)      893 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1435 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/stdout_color_sinks-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1792 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/stdout_color_sinks.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4347 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/stdout_sinks-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2429 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/stdout_sinks.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4239 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/syslog_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4872 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/systemd_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2127 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/tcp_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1858 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/udp_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8888 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/win_eventlog_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6651 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/wincolor_sink-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2716 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/wincolor_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3118 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/spdlog-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)    11771 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/spdlog.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1711 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/stopwatch.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6360 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/tweakme.h
--rw-rw-r--   0 runner    (1001) docker     (127)      417 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/spdlog/spdlog/version.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/taywee_args/
--rw-rw-r--   0 runner    (1001) docker     (127)     1105 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/taywee_args/LICENSE
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/taywee_args/include/
--rw-rw-r--   0 runner    (1001) docker     (127)   152995 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/taywee_args/include/args.hxx
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/utf8proc/
--rw-rw-r--   0 runner    (1001) docker     (127)      142 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/utf8proc/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     5125 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/utf8proc/LICENSE.md
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/utf8proc/include/
--rw-rw-r--   0 runner    (1001) docker     (127)    32757 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/utf8proc/include/utf8proc.h
--rw-rw-r--   0 runner    (1001) docker     (127)  1944550 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/utf8proc/include/utf8proc_data.h
--rw-rw-r--   0 runner    (1001) docker     (127)      888 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/utf8proc/include/utf8proc_wrapper.h
--rw-rw-r--   0 runner    (1001) docker     (127)    37876 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/utf8proc/utf8proc.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4483 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/utf8proc/utf8proc_wrapper.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/
--rw-rw-r--   0 runner    (1001) docker     (127)     1194 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1529 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/LICENSE
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/common/
--rw-rw-r--   0 runner    (1001) docker     (127)     8580 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/common/entropy_common.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2982 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/common/error_private.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    10089 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/common/fse_decompress.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    28008 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/common/xxhash.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2721 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/common/zstd_common.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/compress/
--rw-rw-r--   0 runner    (1001) docker     (127)    26469 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/compress/fse_compress.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7555 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/compress/hist.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    32726 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/compress/huf_compress.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)   183732 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_compress.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6293 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_compress_literals.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    19309 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_compress_sequences.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    43614 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_compress_superblock.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    25428 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_double_fast.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    22459 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_fast.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    52956 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_lazy.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    25024 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_ldm.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    55766 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_opt.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/decompress/
--rw-rw-r--   0 runner    (1001) docker     (127)    51287 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/decompress/huf_decompress.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9136 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/decompress/zstd_ddict.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    83312 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/decompress/zstd_decompress.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    61618 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/decompress/zstd_decompress_block.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/include/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/
--rw-rw-r--   0 runner    (1001) docker     (127)    17857 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/bitstream.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5734 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/compiler.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3893 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/debug.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2396 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/error_private.h
--rw-rw-r--   0 runner    (1001) docker     (127)    14574 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/fse.h
--rw-rw-r--   0 runner    (1001) docker     (127)    18012 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/fse_static.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4717 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/huf.h
--rw-rw-r--   0 runner    (1001) docker     (127)    14332 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/huf_static.h
--rw-rw-r--   0 runner    (1001) docker     (127)    12217 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/mem.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9897 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/xxhash.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1779 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/xxhash_static.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3730 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/zstd_errors.h
--rw-rw-r--   0 runner    (1001) docker     (127)    13604 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/zstd_internal.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/
--rw-rw-r--   0 runner    (1001) docker     (127)     3464 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/hist.h
--rw-rw-r--   0 runner    (1001) docker     (127)    46030 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_compress_internal.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1262 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_compress_literals.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2210 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_compress_sequences.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1194 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_compress_superblock.h
--rw-rw-r--   0 runner    (1001) docker     (127)    18777 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_cwksp.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1250 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_double_fast.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1171 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_fast.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2701 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_lazy.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4010 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_ldm.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1972 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_opt.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/decompress/
--rw-rw-r--   0 runner    (1001) docker     (127)     1329 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/decompress/zstd_ddict.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2081 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/decompress/zstd_decompress_block.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6147 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd/decompress/zstd_decompress_internal.h
--rw-rw-r--   0 runner    (1001) docker     (127)    61165 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd.h
--rw-rw-r--   0 runner    (1001) docker     (127)    60974 2024-04-15 08:03:54.000000 sdist/kuzu-source/third_party/zstd/include/zstd_static.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/
--rw-rw-r--   0 runner    (1001) docker     (127)      297 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/benchmark/
--rw-rw-r--   0 runner    (1001) docker     (127)      251 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/benchmark/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     3132 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/benchmark/benchmark.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3400 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/benchmark/benchmark_runner.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/benchmark/example/
--rw-rw-r--   0 runner    (1001) docker     (127)       73 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/benchmark/example/example.benchmark
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/benchmark/include/
--rw-rw-r--   0 runner    (1001) docker     (127)      994 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/benchmark/include/benchmark.h
--rw-rw-r--   0 runner    (1001) docker     (127)      561 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/benchmark/include/benchmark_config.h
--rw-rw-r--   0 runner    (1001) docker     (127)      836 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/benchmark/include/benchmark_runner.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2195 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/benchmark/main.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/
--rw-rw-r--   0 runner    (1001) docker     (127)     1846 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      332 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/README.md
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/jni/
--rw-rw-r--   0 runner    (1001) docker     (127)    51926 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/jni/kuzu_java.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/main/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/
--rw-rw-r--   0 runner    (1001) docker     (127)     4861 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuConnection.java
--rw-rw-r--   0 runner    (1001) docker     (127)     3587 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuDataType.java
--rw-rw-r--   0 runner    (1001) docker     (127)      716 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuDataTypeID.java
--rw-rw-r--   0 runner    (1001) docker     (127)     2944 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuDatabase.java
--rw-rw-r--   0 runner    (1001) docker     (127)     1734 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuFlatTuple.java
--rw-rw-r--   0 runner    (1001) docker     (127)      495 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuInternalID.java
--rw-rw-r--   0 runner    (1001) docker     (127)     9740 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuNative.java
--rw-rw-r--   0 runner    (1001) docker     (127)      334 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuObjectRefDestroyedException.java
--rw-rw-r--   0 runner    (1001) docker     (127)     2490 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuPreparedStatement.java
--rw-rw-r--   0 runner    (1001) docker     (127)     5236 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuQueryResult.java
--rw-rw-r--   0 runner    (1001) docker     (127)      853 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuQuerySummary.java
--rw-rw-r--   0 runner    (1001) docker     (127)     4622 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValue.java
--rw-rw-r--   0 runner    (1001) docker     (127)     1077 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueListUtil.java
--rw-rw-r--   0 runner    (1001) docker     (127)     2984 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueNodeUtil.java
--rw-rw-r--   0 runner    (1001) docker     (127)     1034 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueRdfVariantUtil.java
--rw-rw-r--   0 runner    (1001) docker     (127)     1024 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueRecursiveRelUtil.java
--rw-rw-r--   0 runner    (1001) docker     (127)     3397 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueRelUtil.java
--rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueStructUtil.java
--rw-rw-r--   0 runner    (1001) docker     (127)      520 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuVersion.java
--rw-rw-r--   0 runner    (1001) docker     (127)      178 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/package-info.java
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/test/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/test/java/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/
--rw-rw-r--   0 runner    (1001) docker     (127)    11911 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/ConnectionTest.java
--rw-rw-r--   0 runner    (1001) docker     (127)     5025 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/DataTypeTest.java
--rw-rw-r--   0 runner    (1001) docker     (127)     1946 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/DatabaseTest.java
--rw-rw-r--   0 runner    (1001) docker     (127)      525 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/ExtensionTest.java
--rw-rw-r--   0 runner    (1001) docker     (127)     1865 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/FlatTupleTest.java
--rw-rw-r--   0 runner    (1001) docker     (127)     2476 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/PreparedStatementTest.java
--rw-rw-r--   0 runner    (1001) docker     (127)     4789 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/QueryResultTest.java
--rw-rw-r--   0 runner    (1001) docker     (127)      940 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/TestBase.java
--rw-rw-r--   0 runner    (1001) docker     (127)     2504 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/TestHelper.java
--rw-rw-r--   0 runner    (1001) docker     (127)    45229 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/ValueTest.java
--rw-rw-r--   0 runner    (1001) docker     (127)      471 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/VersionTest.java
--rw-rw-r--   0 runner    (1001) docker     (127)     2271 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/test.java
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/third_party/
--rw-rw-r--   0 runner    (1001) docker     (127)  2614186 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/java_api/third_party/junit-platform-console-standalone-1.9.3.jar
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/
--rw-rw-r--   0 runner    (1001) docker     (127)     1777 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     3043 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/README.md
--rw-rw-r--   0 runner    (1001) docker     (127)      397 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/build.js
--rw-rw-r--   0 runner    (1001) docker     (127)      615 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/clean.js
--rw-rw-r--   0 runner    (1001) docker     (127)     4452 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/install.js
--rw-rw-r--   0 runner    (1001) docker     (127)     5577 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/package.js
--rw-rw-r--   0 runner    (1001) docker     (127)      672 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/package.json
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/
--rw-rw-r--   0 runner    (1001) docker     (127)     4353 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_connection.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1577 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1635 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_prepared_statement.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4369 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_query_result.h
--rw-rw-r--   0 runner    (1001) docker     (127)      637 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_util.h
--rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/main.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4010 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_connection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2461 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2110 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_prepared_statement.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3361 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_query_result.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    19925 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_util.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/src_js/
--rw-rw-r--   0 runner    (1001) docker     (127)     7782 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/src_js/connection.js
--rw-rw-r--   0 runner    (1001) docker     (127)     4045 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/src_js/database.js
--rw-rw-r--   0 runner    (1001) docker     (127)      499 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/src_js/index.js
--rw-rw-r--   0 runner    (1001) docker     (127)      686 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/src_js/kuzu_native.js
--rw-rw-r--   0 runner    (1001) docker     (127)      238 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/src_js/logging_level.js
--rw-rw-r--   0 runner    (1001) docker     (127)     1210 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/src_js/prepared_statement.js
--rw-rw-r--   0 runner    (1001) docker     (127)     4244 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/src_js/query_result.js
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/test/
--rw-rw-r--   0 runner    (1001) docker     (127)     2099 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/test/common.js
--rw-rw-r--   0 runner    (1001) docker     (127)      629 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/test/test.js
--rw-rw-r--   0 runner    (1001) docker     (127)     3089 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/test/test_concurrency.js
--rw-rw-r--   0 runner    (1001) docker     (127)     7822 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/test/test_connection.js
--rw-rw-r--   0 runner    (1001) docker     (127)    19348 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/test/test_data_type.js
--rw-rw-r--   0 runner    (1001) docker     (127)     7243 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/test/test_database.js
--rw-rw-r--   0 runner    (1001) docker     (127)      266 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/test/test_extension.js
--rw-rw-r--   0 runner    (1001) docker     (127)    22522 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/test/test_parameter.js
--rw-rw-r--   0 runner    (1001) docker     (127)     5730 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/test/test_query_result.js
--rw-rw-r--   0 runner    (1001) docker     (127)      384 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/nodejs_api/test/test_version.js
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/
--rw-rw-r--   0 runner    (1001) docker     (127)     1295 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1136 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/Makefile
--rw-rw-r--   0 runner    (1001) docker     (127)       23 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/README.md
--rw-rw-r--   0 runner    (1001) docker     (127)     2381 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      203 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/requirements_dev.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/cached_import/
--rw-rw-r--   0 runner    (1001) docker     (127)      376 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/cached_import/py_cached_import.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      618 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/cached_import/py_cached_item.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/
--rw-rw-r--   0 runner    (1001) docker     (127)      335 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/arrow_array.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/cached_import/
--rw-rw-r--   0 runner    (1001) docker     (127)      682 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/cached_import/py_cached_import.h
--rw-rw-r--   0 runner    (1001) docker     (127)      521 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/cached_import/py_cached_item.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3624 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/cached_import/py_cached_modules.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/numpy/
--rw-rw-r--   0 runner    (1001) docker     (127)      430 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/numpy/numpy_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1379 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/numpy/numpy_type.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/
--rw-rw-r--   0 runner    (1001) docker     (127)      718 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/pandas_analyzer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1290 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/pandas_bind.h
--rw-rw-r--   0 runner    (1001) docker     (127)      931 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/pandas_column.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1942 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/pandas_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1266 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_connection.h
--rw-rw-r--   0 runner    (1001) docker     (127)      714 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_conversion.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1050 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      676 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_object_container.h
--rw-rw-r--   0 runner    (1001) docker     (127)      381 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_prepared_statement.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1369 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_query_result.h
--rw-rw-r--   0 runner    (1001) docker     (127)      709 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_query_result_converter.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1031 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_str_utils.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pyarrow/
--rw-rw-r--   0 runner    (1001) docker     (127)      383 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pyarrow/pyarrow_bind.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2211 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pyarrow/pyarrow_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)      202 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pybind_include.h
--rw-rw-r--   0 runner    (1001) docker     (127)      549 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/kuzu_binding.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/numpy/
--rw-rw-r--   0 runner    (1001) docker     (127)     9493 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/numpy/numpy_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5514 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/numpy/numpy_type.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/pandas/
--rw-rw-r--   0 runner    (1001) docker     (127)     3949 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/pandas/pandas_analyzer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3943 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/pandas/pandas_bind.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7556 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/pandas/pandas_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    18204 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_connection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4462 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_conversion.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3622 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      564 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_prepared_statement.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    15476 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_query_result.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7635 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_query_result_converter.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/pyarrow/
--rw-rw-r--   0 runner    (1001) docker     (127)      866 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/pyarrow/pyarrow_bind.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4295 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_cpp/pyarrow/pyarrow_scan.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_py/
--rw-rw-r--   0 runner    (1001) docker     (127)     2111 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_py/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6092 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_py/connection.py
--rw-rw-r--   0 runner    (1001) docker     (127)     8124 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_py/database.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1167 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_py/prepared_statement.py
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_py/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)    14457 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_py/query_result.py
--rw-rw-r--   0 runner    (1001) docker     (127)     7586 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_py/torch_geometric_feature_store.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4893 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_py/torch_geometric_graph_store.py
--rw-rw-r--   0 runner    (1001) docker     (127)    13467 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_py/torch_geometric_result_converter.py
--rw-rw-r--   0 runner    (1001) docker     (127)      839 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/src_py/types.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/test/
--rw-rw-r--   0 runner    (1001) docker     (127)     5545 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/test/conftest.py
--rw-rw-r--   0 runner    (1001) docker     (127)      303 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/test/example.py
--rw-rw-r--   0 runner    (1001) docker     (127)    14350 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/test/ground_truth.py
--rw-rw-r--   0 runner    (1001) docker     (127)    22117 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/test/test_arrow.py
--rw-rw-r--   0 runner    (1001) docker     (127)    12786 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/test/test_datatype.py
--rw-rw-r--   0 runner    (1001) docker     (127)    19806 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/test/test_df.py
--rw-rw-r--   0 runner    (1001) docker     (127)    17869 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/test/test_df_pyarrow.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2292 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/test/test_exception.py
--rw-rw-r--   0 runner    (1001) docker     (127)      247 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/test/test_extension.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1947 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/test/test_get_header.py
--rw-rw-r--   0 runner    (1001) docker     (127)      222 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/test/test_helper.py
--rw-rw-r--   0 runner    (1001) docker     (127)    10889 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/test/test_networkx.py
--rw-rw-r--   0 runner    (1001) docker     (127)     8377 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/test/test_parameter.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4511 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/test/test_prepared_statement.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1421 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/test/test_query_result.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1258 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/test/test_query_result_close.py
--rw-rw-r--   0 runner    (1001) docker     (127)    12731 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/test/test_scan_pandas.py
--rw-rw-r--   0 runner    (1001) docker     (127)      345 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/test/test_timeout.py
--rw-rw-r--   0 runner    (1001) docker     (127)    30361 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/test/test_torch_geometric.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4105 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/test/test_torch_geometric_remote_backend.py
--rw-rw-r--   0 runner    (1001) docker     (127)      155 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/test/test_version.py
--rw-rw-r--   0 runner    (1001) docker     (127)      215 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/python_api/test/type_aliases.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/rust_api/
--rw-rw-r--   0 runner    (1001) docker     (127)        7 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/rust_api/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (127)    25753 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/rust_api/Cargo.lock
--rw-rw-r--   0 runner    (1001) docker     (127)     1099 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/rust_api/Cargo.toml
--rw-rw-r--   0 runner    (1001) docker     (127)     5609 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/rust_api/build.rs
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/rust_api/include/
--rw-rw-r--   0 runner    (1001) docker     (127)      345 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/rust_api/include/kuzu_arrow.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9633 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/rust_api/include/kuzu_rs.h
-lrwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:57.564586 sdist/kuzu-source/tools/rust_api/kuzu-src -> ../..
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/rust_api/src/
--rw-rw-r--   0 runner    (1001) docker     (127)      380 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/rust_api/src/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    13653 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/rust_api/src/connection.rs
--rw-rw-r--   0 runner    (1001) docker     (127)     6682 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/rust_api/src/database.rs
--rw-rw-r--   0 runner    (1001) docker     (127)     1763 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/rust_api/src/error.rs
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/rust_api/src/ffi/
--rw-rw-r--   0 runner    (1001) docker     (127)     1123 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/rust_api/src/ffi/arrow.rs
--rw-rw-r--   0 runner    (1001) docker     (127)    12920 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/rust_api/src/ffi.rs
--rw-rw-r--   0 runner    (1001) docker     (127)      471 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/rust_api/src/kuzu_arrow.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11961 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/rust_api/src/kuzu_rs.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2523 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/rust_api/src/lib.rs
--rw-rw-r--   0 runner    (1001) docker     (127)    12498 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/rust_api/src/logical_type.rs
--rw-rw-r--   0 runner    (1001) docker     (127)     9355 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/rust_api/src/query_result.rs
--rw-rw-r--   0 runner    (1001) docker     (127)     2629 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/rust_api/src/rdf_variant.rs
--rw-rw-r--   0 runner    (1001) docker     (127)    67772 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/rust_api/src/value.rs
--rw-rw-r--   0 runner    (1001) docker     (127)     1730 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/rust_api/update_version.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/shell/
--rw-rw-r--   0 runner    (1001) docker     (127)      321 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/shell/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    27718 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/shell/embedded_shell.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/shell/include/
--rw-rw-r--   0 runner    (1001) docker     (127)      912 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/shell/include/embedded_shell.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3116 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/shell/include/linenoise.h
--rw-rw-r--   0 runner    (1001) docker     (127)    79992 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/shell/linenoise.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3257 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/shell/shell_runner.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/shell/test/
--rw-rw-r--   0 runner    (1001) docker     (127)     5371 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/shell/test/conftest.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/shell/test/files/
--rw-rw-r--   0 runner    (1001) docker     (127)     3075 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/shell/test/files/vPerson.csv
--rw-rw-r--   0 runner    (1001) docker     (127)     1399 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/shell/test/test_helper.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4780 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/shell/test/test_shell_basics.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4811 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/shell/test/test_shell_commands.py
--rw-rw-r--   0 runner    (1001) docker     (127)    11969 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/shell/test/test_shell_control_edit.py
--rw-rw-r--   0 runner    (1001) docker     (127)    12995 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/shell/test/test_shell_control_search.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4297 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/shell/test/test_shell_esc_edit.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4571 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/shell/test/test_shell_esc_search.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4904 2024-04-15 08:03:54.000000 sdist/kuzu-source/tools/shell/test/test_shell_flags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:03:59.024579 sdist/kuzu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-04-15 08:03:59.024579 sdist/kuzu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-15 08:03:59.028579 sdist/kuzu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:03:59.024579 sdist/kuzu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-15 08:03:59.024579 sdist/kuzu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:03:59.024579 sdist/kuzu.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-15 08:03:57.788585 sdist/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-15 08:03:54.148607 sdist/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-04-15 08:03:54.148607 sdist/setup.py
+drwx------   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:22.322006 sdist/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-16 08:04:17.426007 sdist/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-16 08:04:18.874008 sdist/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-16 08:04:17.426007 sdist/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-04-16 08:04:18.874008 sdist/README_PYTHON_BUILD.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:22.110007 sdist/kuzu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:22.110007 sdist/kuzu-source/
+-rw-rw-r--   0 runner    (1001) docker     (127)     5560 2024-04-16 08:04:19.000000 sdist/kuzu-source/.clang-format
+-rw-rw-r--   0 runner    (1001) docker     (127)      948 2024-04-16 08:04:19.000000 sdist/kuzu-source/.clang-tidy
+-rw-rw-r--   0 runner    (1001) docker     (127)      332 2024-04-16 08:04:19.000000 sdist/kuzu-source/.clang-tidy-analyzer
+-rw-rw-r--   0 runner    (1001) docker     (127)     1000 2024-04-16 08:04:19.000000 sdist/kuzu-source/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (127)       47 2024-04-16 08:04:19.000000 sdist/kuzu-source/.lcovrc
+-rw-rw-r--   0 runner    (1001) docker     (127)     8632 2024-04-16 08:04:19.000000 sdist/kuzu-source/CLA.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     8435 2024-04-16 08:04:19.000000 sdist/kuzu-source/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      632 2024-04-16 08:04:19.000000 sdist/kuzu-source/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     2052 2024-04-16 08:04:19.000000 sdist/kuzu-source/CONTRIBUTING.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     1072 2024-04-16 08:04:19.000000 sdist/kuzu-source/LICENSE
+-rw-rw-r--   0 runner    (1001) docker     (127)     6365 2024-04-16 08:04:19.000000 sdist/kuzu-source/Makefile
+-rw-rw-r--   0 runner    (1001) docker     (127)     3881 2024-04-16 08:04:19.000000 sdist/kuzu-source/README.md
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/scripts/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/scripts/antlr4/
+-rw-rw-r--   0 runner    (1001) docker     (127)    26195 2024-04-16 08:04:19.000000 sdist/kuzu-source/scripts/antlr4/Cypher.g4.copy
+-rw-rw-r--   0 runner    (1001) docker     (127)     2085 2024-04-16 08:04:19.000000 sdist/kuzu-source/scripts/antlr4/generate_grammar.cmake
+-rwxrwxr-x   0 runner    (1001) docker     (127)      299 2024-04-16 08:04:19.000000 sdist/kuzu-source/scripts/check-include-guards.sh
+-rwxrwxr-x   0 runner    (1001) docker     (127)       76 2024-04-16 08:04:19.000000 sdist/kuzu-source/scripts/check-no-std-assert.sh
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2837 2024-04-16 08:04:19.000000 sdist/kuzu-source/scripts/collect-single-file-header.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/scripts/generate-cpp-docs/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/scripts/generate-cpp-docs/c/
+-rw-rw-r--   0 runner    (1001) docker     (127)   126290 2024-04-16 08:04:19.000000 sdist/kuzu-source/scripts/generate-cpp-docs/c/Doxyfile
+-rw-rw-r--   0 runner    (1001) docker     (127)     4738 2024-04-16 08:04:19.000000 sdist/kuzu-source/scripts/generate-cpp-docs/collect_files.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/scripts/generate-cpp-docs/cpp/
+-rw-rw-r--   0 runner    (1001) docker     (127)   126295 2024-04-16 08:04:19.000000 sdist/kuzu-source/scripts/generate-cpp-docs/cpp/Doxyfile
+-rwxrwxr-x   0 runner    (1001) docker     (127)      225 2024-04-16 08:04:19.000000 sdist/kuzu-source/scripts/generate-cpp-docs/doxygen.sh
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6998 2024-04-16 08:04:19.000000 sdist/kuzu-source/scripts/get-clangd-diagnostics.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      173 2024-04-16 08:04:19.000000 sdist/kuzu-source/scripts/http-server.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/scripts/multiplatform-test-helper/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2130 2024-04-16 08:04:19.000000 sdist/kuzu-source/scripts/multiplatform-test-helper/collect-results.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1585 2024-04-16 08:04:19.000000 sdist/kuzu-source/scripts/multiplatform-test-helper/notify-discord.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/scripts/pip-package/
+-rw-rw-r--   0 runner    (1001) docker     (127)       37 2024-04-16 08:04:19.000000 sdist/kuzu-source/scripts/pip-package/MANIFEST.in
+-rw-rw-r--   0 runner    (1001) docker     (127)     3276 2024-04-16 08:04:19.000000 sdist/kuzu-source/scripts/pip-package/README.md
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3277 2024-04-16 08:04:19.000000 sdist/kuzu-source/scripts/pip-package/package_tar.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      200 2024-04-16 08:04:19.000000 sdist/kuzu-source/scripts/pip-package/setup.cfg
+-rw-rw-r--   0 runner    (1001) docker     (127)     4441 2024-04-16 08:04:19.000000 sdist/kuzu-source/scripts/pip-package/setup.py
+-rwxrwxr-x   0 runner    (1001) docker     (127)    12359 2024-04-16 08:04:19.000000 sdist/kuzu-source/scripts/run-clang-format.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     3060 2024-04-16 08:04:19.000000 sdist/kuzu-source/scripts/update-nightly-build-version.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2525 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/antlr4/
+-rw-rw-r--   0 runner    (1001) docker     (127)    26195 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/antlr4/Cypher.g4
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/
+-rw-rw-r--   0 runner    (1001) docker     (127)      519 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind/
+-rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      520 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind/bind_attach_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      740 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind/bind_comment_on.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1323 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind/bind_create_macro.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    18649 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind/bind_ddl.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      516 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind/bind_detach_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      518 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind/bind_explain.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4631 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind/bind_export_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      579 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind/bind_extension.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5298 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind/bind_file_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    33112 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind/bind_graph_pattern.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3113 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind/bind_import_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11859 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind/bind_projection_clause.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4787 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind/bind_query.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      702 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind/bind_reading_clause.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1260 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind/bind_standalone_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      566 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind/bind_transaction.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    17251 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind/bind_updating_clause.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind/copy/
+-rw-rw-r--   0 runner    (1001) docker     (127)      246 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind/copy/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    10625 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind/copy/bind_copy_from.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7684 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind/copy/bind_copy_rdf_graph.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1613 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind/copy/bind_copy_to.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind/ddl/
+-rw-rw-r--   0 runner    (1001) docker     (127)      194 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind/ddl/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     3534 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind/ddl/bind_create_rdf_graph.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind/read/
+-rw-rw-r--   0 runner    (1001) docker     (127)      267 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind/read/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2996 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind/read/bind_in_query_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5056 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind/read/bind_load_from.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3009 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind/read/bind_match.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1268 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind/read/bind_unwind.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind_expression/
+-rw-rw-r--   0 runner    (1001) docker     (127)      555 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind_expression/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2201 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind_expression/bind_boolean_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3487 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind_expression/bind_case_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3376 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind_expression/bind_comparison_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    16408 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind_expression/bind_function_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1410 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind_expression/bind_literal_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1676 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind_expression/bind_null_operator_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      926 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind_expression/bind_parameter_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5174 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind_expression/bind_property_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3213 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind_expression/bind_subquery_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1531 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bind_expression/bind_variable_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8623 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/binder.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/binder_scope.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      585 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bound_statement_result.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      801 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bound_statement_rewriter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5434 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/bound_statement_visitor.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/expression/
+-rw-rw-r--   0 runner    (1001) docker     (127)      348 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/expression/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      498 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/expression/case_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      764 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/expression/expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5664 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/expression/expression_util.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1438 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/expression/function_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      596 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/expression/literal_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      602 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/expression/parameter_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6345 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/expression_binder.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5779 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/expression_visitor.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/query/
+-rw-rw-r--   0 runner    (1001) docker     (127)      350 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/query/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      707 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/query/bound_delete_clause.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      707 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/query/bound_insert_clause.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1963 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/query/bound_merge_clause.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      718 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/query/bound_set_clause.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9670 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/query/query_graph.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6621 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/query/query_graph_label_analyzer.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/rewriter/
+-rw-rw-r--   0 runner    (1001) docker     (127)      261 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/rewriter/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      742 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/rewriter/match_clause_pattern_label_rewriter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2547 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/rewriter/with_clause_projection_rewriter.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/visitor/
+-rw-rw-r--   0 runner    (1001) docker     (127)      230 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/visitor/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      638 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/visitor/default_type_solver.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4801 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/binder/visitor/property_collector.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/c_api/
+-rw-rw-r--   0 runner    (1001) docker     (127)      369 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/c_api/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     4034 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/c_api/connection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2689 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/c_api/data_type.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1237 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/c_api/database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1412 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/c_api/flat_tuple.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      286 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/c_api/helpers.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7841 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/c_api/prepared_statement.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4402 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/c_api/query_result.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      745 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/c_api/query_summary.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    19820 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/c_api/value.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      271 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/c_api/version.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/catalog/
+-rw-rw-r--   0 runner    (1001) docker     (127)      270 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/catalog/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    10703 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/catalog/catalog.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    13980 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/catalog/catalog_content.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/catalog/catalog_entry/
+-rw-rw-r--   0 runner    (1001) docker     (127)      464 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/catalog/catalog_entry/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1198 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/catalog/catalog_entry/catalog_entry.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1149 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/catalog/catalog_entry/catalog_entry_type.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      605 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/catalog/catalog_entry/function_catalog_entry.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2023 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/catalog/catalog_entry/node_table_catalog_entry.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3144 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/catalog/catalog_entry/rdf_graph_catalog_entry.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1483 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/catalog/catalog_entry/rel_group_catalog_entry.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4001 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/catalog/catalog_entry/rel_table_catalog_entry.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1224 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/catalog/catalog_entry/scalar_macro_catalog_entry.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4261 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/catalog/catalog_entry/table_catalog_entry.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2691 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/catalog/catalog_set.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1483 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/catalog/property.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/
+-rw-rw-r--   0 runner    (1001) docker     (127)      810 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/arrow/
+-rw-rw-r--   0 runner    (1001) docker     (127)      295 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/arrow/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    23959 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/arrow/arrow_array_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    10319 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/arrow/arrow_converter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8717 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/arrow/arrow_null_mask_tree.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    39407 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/arrow/arrow_row_batch.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5389 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/arrow/arrow_type.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      478 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/case_insensitive_map.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      106 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/constants.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/copier_config/
+-rw-rw-r--   0 runner    (1001) docker     (127)      256 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/copier_config/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     3078 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/copier_config/csv_reader_config.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/copier_config/rdf_reader_config.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1727 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/copier_config/reader_config.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/data_chunk/
+-rw-rw-r--   0 runner    (1001) docker     (127)      250 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/data_chunk/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      470 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/data_chunk/data_chunk.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2645 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/data_chunk/data_chunk_collection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    12603 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/data_chunk/data_chunk_state.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/enums/
+-rw-rw-r--   0 runner    (1001) docker     (127)      258 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/enums/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1050 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/enums/path_semantic.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      413 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/enums/rel_direction.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1069 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/enums/rel_multiplicity.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      578 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/enums/table_type.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/exception/
+-rw-rw-r--   0 runner    (1001) docker     (127)      182 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/exception/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2494 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/exception/message.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3201 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/expression_type.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/file_system/
+-rw-rw-r--   0 runner    (1001) docker     (127)      306 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/file_system/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      999 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/file_system/file_info.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1279 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/file_system/file_system.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    14488 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/file_system/local_file_system.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2726 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/file_system/virtual_file_system.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      663 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/in_mem_overflow_buffer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/keyword_utils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      743 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/logging_level_utils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8157 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/md5.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      995 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/metric.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6819 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/null_mask.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1452 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/profiler.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      349 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/random_engine.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/serializer/
+-rw-rw-r--   0 runner    (1001) docker     (127)      270 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/serializer/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2602 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/serializer/buffered_file.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      948 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/serializer/buffered_serializer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      347 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/serializer/deserializer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      356 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/serializer/serializer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1355 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/sha256.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4819 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/string_utils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      884 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/system_message.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/task_system/
+-rw-rw-r--   0 runner    (1001) docker     (127)      236 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/task_system/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2720 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/task_system/progress_bar.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      772 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/task_system/task.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4596 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/task_system/task_scheduler.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9684 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/type_utils.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/types/
+-rw-rw-r--   0 runner    (1001) docker     (127)      406 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/types/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     4772 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/types/blob.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    19741 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/types/date_t.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6196 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/types/dtime_t.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    19061 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/types/int128_t.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1173 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/types/internal_id_t.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    17620 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/types/interval_t.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      834 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/types/ku_list.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2364 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/types/ku_string.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11000 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/types/timestamp_t.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    35498 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/types/types.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4363 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/types/uuid.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/types/value/
+-rw-rw-r--   0 runner    (1001) docker     (127)      286 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/types/value/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      512 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/types/value/nested.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2409 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/types/value/node.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      354 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/types/value/rdf_variant.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      840 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/types/value/recursive_rel.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2799 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/types/value/rel.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    27055 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/types/value/value.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2142 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/utils.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/vector/
+-rw-rw-r--   0 runner    (1001) docker     (127)      210 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/vector/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     3468 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/vector/auxiliary_buffer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    28631 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/vector/value_vector.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1261 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/common/windows_utils.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/expression_evaluator/
+-rw-rw-r--   0 runner    (1001) docker     (127)      420 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/expression_evaluator/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     4615 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/expression_evaluator/case_evaluator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      965 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/expression_evaluator/expression_evaluator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      885 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/expression_evaluator/expression_evaluator_utils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3490 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/expression_evaluator/function_evaluator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1130 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/expression_evaluator/literal_evaluator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1556 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/expression_evaluator/node_rel_evaluator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9766 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/expression_evaluator/path_evaluator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1275 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/expression_evaluator/reference_evaluator.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/extension/
+-rw-rw-r--   0 runner    (1001) docker     (127)      170 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/extension/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2157 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/extension/extension.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1259 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/aggregate/
+-rw-rw-r--   0 runner    (1001) docker     (127)      227 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/aggregate/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     3939 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/aggregate/collect.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1841 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/aggregate/count.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1044 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/aggregate/count_star.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    12187 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/aggregate_function.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/arithmetic/
+-rw-rw-r--   0 runner    (1001) docker     (127)      299 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/arithmetic/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2611 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/arithmetic/abs.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5505 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/arithmetic/add.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5953 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/arithmetic/divide.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4379 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/arithmetic/modulo.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8121 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/arithmetic/multiply.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2427 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/arithmetic/negate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5848 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/arithmetic/subtract.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2494 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/base_lower_upper_operation.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    19408 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/built_in_function_utils.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/cast/
+-rw-rw-r--   0 runner    (1001) docker     (127)      208 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/cast/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     5405 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/cast/cast_array.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11953 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/cast/cast_rdf_variant.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    33753 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/cast_from_string_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2442 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/cast_string_non_nested_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8637 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/comparison_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5169 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/find_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    12306 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/function_collection.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/pattern/
+-rw-rw-r--   0 runner    (1001) docker     (127)      186 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/pattern/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1872 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/pattern/id_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2683 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/scalar_macro_function.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/table/
+-rw-rw-r--   0 runner    (1001) docker     (127)      218 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/table/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/table/call/
+-rw-rw-r--   0 runner    (1001) docker     (127)      301 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/table/call/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2314 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/table/call/current_setting.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1428 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/table/call/db_version.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5207 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/table/call/show_connection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2909 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/table/call/show_tables.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11166 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/table/call/storage_info.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4397 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/table/call/table_info.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1139 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/table/call_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      364 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/table/scan_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    18420 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/vector_arithmetic_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6890 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/vector_array_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1498 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/vector_blob_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4267 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/vector_boolean_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    43230 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/vector_cast_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4887 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/vector_date_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    10173 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/vector_hash_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    49369 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/vector_list_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7341 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/vector_map_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      888 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/vector_node_rel_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1516 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/vector_null_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6879 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/vector_path_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      913 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/vector_rdf_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    15223 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/vector_string_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5543 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/vector_struct_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1205 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/vector_timestamp_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2856 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/vector_union_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      552 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/function/vector_uuid_functions.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/
+-rw-rw-r--   0 runner    (1001) docker     (127)    12622 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/binder.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2756 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/binder_scope.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      592 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/bound_attach_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      862 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/bound_comment_on.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      842 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/bound_create_macro.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      503 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/bound_detach_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      891 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/bound_explain.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      700 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/bound_extension_statement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2466 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/bound_scan_source.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      790 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/bound_standalone_call.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      787 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/bound_statement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1034 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/bound_statement_result.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      348 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/bound_statement_rewriter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2606 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/bound_statement_visitor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      661 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/bound_transaction_statement.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/copy/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3164 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/copy/bound_copy_from.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1071 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/copy/bound_copy_to.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1888 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/copy/bound_export_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      813 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/copy/bound_file_scan_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      626 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/copy/bound_import_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1014 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/copy/index_look_up_info.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/ddl/
+-rw-rw-r--   0 runner    (1001) docker     (127)      530 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/ddl/bound_alter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3274 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/ddl/bound_alter_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      574 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/ddl/bound_create_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5498 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/ddl/bound_create_table_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      664 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/ddl/bound_drop_table.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/expression/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1468 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/expression/case_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4519 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/expression/expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1962 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/expression/expression_util.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4586 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/expression/function_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      878 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/expression/literal_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      786 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/expression/node_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4200 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/expression/node_rel_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      937 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/expression/parameter_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1129 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/expression/path_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2561 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/expression/property_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4586 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/expression/rel_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2112 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/expression/subquery_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      796 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/expression/variable_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6024 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/expression_binder.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2678 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/expression_visitor.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/query/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1069 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/query/bound_regular_query.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2487 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/query/normalized_query_part.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1013 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/query/normalized_single_query.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6508 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/query/query_graph.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      572 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/query/query_graph_label_analyzer.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1225 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_in_query_call.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      482 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_load_from.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      813 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_match_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1010 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_reading_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      869 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_unwind_clause.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/query/return_with_clause/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3072 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/query/return_with_clause/bound_projection_body.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      923 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/query/return_with_clause/bound_return_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      687 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/query/return_with_clause/bound_with_clause.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1445 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_delete_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      871 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_delete_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1470 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_insert_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1520 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_insert_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5606 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_merge_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1570 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_set_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      797 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_set_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      424 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_updating_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      163 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/update_table_type.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/rewriter/
+-rw-rw-r--   0 runner    (1001) docker     (127)      515 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/rewriter/match_clause_pattern_label_rewriter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      693 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/rewriter/with_clause_projection_rewriter.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/visitor/
+-rw-rw-r--   0 runner    (1001) docker     (127)      781 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/visitor/default_type_solver.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1211 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/binder/visitor/property_collector.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/c_api/
+-rw-rw-r--   0 runner    (1001) docker     (127)       86 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/c_api/helpers.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    51266 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/c_api/kuzu.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/catalog/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4690 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/catalog/catalog.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3631 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/catalog/catalog_content.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1769 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/catalog_entry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      553 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/catalog_entry_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1343 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/function_catalog_entry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2508 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/node_table_catalog_entry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2311 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/rdf_graph_catalog_entry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1522 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/rel_group_catalog_entry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2361 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/rel_table_catalog_entry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1449 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/scalar_macro_catalog_entry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3199 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/table_catalog_entry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1283 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/catalog/catalog_set.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1693 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/catalog/property.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/
+-rw-rw-r--   0 runner    (1001) docker     (127)      975 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/api.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/arrow/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1542 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/arrow/arrow.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1943 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/arrow/arrow_buffer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1862 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/arrow/arrow_converter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1341 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/arrow/arrow_nullmask_tree.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3505 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/arrow/arrow_row_batch.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1139 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/assert.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      578 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/case_insensitive_map.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      559 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/cast.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      178 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/column_data_format.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9693 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/constants.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/copier_config/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1633 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/copier_config/csv_reader_config.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      468 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/copier_config/rdf_reader_config.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1302 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/copier_config/reader_config.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3648 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/copy_constructors.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/data_chunk/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1575 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/data_chunk/data_chunk.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1261 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/data_chunk/data_chunk_collection.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1882 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/data_chunk/data_chunk_state.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1540 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/data_chunk/sel_vector.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/enums/
+-rw-rw-r--   0 runner    (1001) docker     (127)      246 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/enums/alter_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      575 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/enums/clause_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      194 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/enums/conflict_action.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      194 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/enums/delete_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      192 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/enums/explain_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1221 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/enums/expression_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      285 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/enums/join_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      364 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/enums/path_semantic.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      402 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/enums/query_rel_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      300 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/enums/rel_direction.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      359 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/enums/rel_multiplicity.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      195 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/enums/scan_source_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      915 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/enums/statement_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      164 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/enums/subquery_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      431 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/enums/table_type.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/exception/
+-rw-rw-r--   0 runner    (1001) docker     (127)      301 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/exception/binder.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      331 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/exception/buffer_manager.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      304 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/exception/catalog.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      286 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/exception/connection.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      321 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/exception/conversion.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      295 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/exception/copy.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      455 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/exception/exception.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      294 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/exception/extension.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      282 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/exception/internal.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      273 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/exception/interrupt.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      265 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/exception/io.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1185 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/exception/message.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      294 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/exception/not_implemented.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      307 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/exception/overflow.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      301 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/exception/parser.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      304 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/exception/runtime.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      304 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/exception/storage.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      262 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/exception/test.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      302 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/exception/transaction_manager.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/file_system/
+-rw-rw-r--   0 runner    (1001) docker     (127)      764 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/file_system/file_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2076 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/file_system/file_system.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2043 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/file_system/local_file_system.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1805 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/file_system/virtual_file_system.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2203 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/in_mem_overflow_buffer.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/keyword/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1576 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/keyword/rdf_keyword.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      294 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/logging_level_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3271 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/md5.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      745 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/metric.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3921 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/mpsc_queue.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1346 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/mutex.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1155 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/null_buffer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8464 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/null_mask.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      702 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/profiler.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      349 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/random_engine.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/serializer/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1391 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/serializer/buffered_file.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1716 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/serializer/buffered_serializer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2495 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/serializer/deserializer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      264 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/serializer/reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2467 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/serializer/serializer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      237 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/serializer/writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      557 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/sha256.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2228 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/static_vector.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3858 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/string_format.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4679 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/string_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      596 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/system_message.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/task_system/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1469 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/task_system/progress_bar.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3420 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/task_system/task.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3059 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/task_system/task_scheduler.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1205 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/timer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    11010 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/type_utils.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/types/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1666 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/types/blob.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    10927 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/types/cast_helpers.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4563 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/types/date_t.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2446 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/types/dtime_t.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6090 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/types/int128_t.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1063 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/types/internal_id_t.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4658 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/types/interval_t.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/types/ku_list.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2887 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/types/ku_string.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4667 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/types/timestamp_t.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    21355 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/types/types.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      940 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/types/uuid.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/types/value/
+-rw-rw-r--   0 runner    (1001) docker     (127)      319 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/types/value/nested.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1670 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/types/value/node.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1145 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/types/value/rdf_variant.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      635 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/types/value/recursive_rel.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1968 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/types/value/rel.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    20925 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/types/value/value.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1172 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/utils.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/vector/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3218 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/vector/auxiliary_buffer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    13715 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/vector/value_vector.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      298 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/common/windows_utils.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/expression_evaluator/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2419 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/expression_evaluator/case_evaluator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1382 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/expression_evaluator/expression_evaluator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      450 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/expression_evaluator/expression_evaluator_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1267 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/expression_evaluator/function_evaluator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      972 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/expression_evaluator/literal_evaluator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1399 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/expression_evaluator/node_rel_evaluator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2884 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/expression_evaluator/path_evaluator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1082 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/expression_evaluator/reference_evaluator.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/extension/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1103 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/extension/extension.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      193 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/extension/extension_action.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/aggregate/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3538 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/aggregate/avg.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1139 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/aggregate/base_count.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2409 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/aggregate/collect.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      821 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/aggregate/count.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/aggregate/count_star.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4106 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/aggregate/min_max.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2918 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/aggregate/sum.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7021 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/aggregate_function.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/arithmetic/
+-rw-rw-r--   0 runner    (1001) docker     (127)      740 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/arithmetic/abs.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      930 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/arithmetic/add.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5133 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/arithmetic/arithmetic_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      957 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/arithmetic/divide.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1109 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/arithmetic/modulo.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      975 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/arithmetic/multiply.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      520 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/arithmetic/negate.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      975 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/arithmetic/subtract.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4696 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/arithmetic/vector_arithmetic_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/array/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/array/functions/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1096 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/array/functions/array_cosine_similarity.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1078 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/array/functions/array_cross_product.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      824 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/array/functions/array_distance.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/array/functions/array_inner_product.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2034 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/array/vector_array_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    25289 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/binary_function_executor.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/blob/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/blob/functions/
+-rw-rw-r--   0 runner    (1001) docker     (127)      828 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/blob/functions/decode_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      402 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/blob/functions/encode_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      269 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/blob/functions/octet_length_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      506 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/blob/vector_blob_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/boolean/
+-rw-rw-r--   0 runner    (1001) docker     (127)    15140 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/boolean/boolean_function_executor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4678 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/boolean/boolean_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2493 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/boolean/vector_boolean_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3533 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/built_in_function_utils.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/cast/
+-rw-rw-r--   0 runner    (1001) docker     (127)      674 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/cast/cast_function_bind_data.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/cast/functions/
+-rw-rw-r--   0 runner    (1001) docker     (127)      525 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_array.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7564 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_from_string_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    13672 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      993 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_rdf_variant.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7994 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_string_non_nested_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5149 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/cast/functions/numeric_cast.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1795 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/cast/functions/numeric_limits.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3693 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/cast/vector_cast_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/comparison/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2928 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/comparison/comparison_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    10609 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/comparison/vector_comparison_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      523 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/const_function_executor.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/date/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4625 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/date/date_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1236 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/date/vector_date_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2236 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      455 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/function_collection.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/hash/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/hash/functions/
+-rw-rw-r--   0 runner    (1001) docker     (127)      519 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/hash/functions/md5_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      571 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/hash/functions/sha256_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6058 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/hash/hash_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      945 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/hash/vector_hash_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/interval/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1758 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/interval/interval_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2341 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/interval/vector_interval_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/list/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/list/functions/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3521 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/list/functions/base_list_sort_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      924 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/list/functions/list_any_value_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1098 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/list/functions/list_append_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1186 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/list/functions/list_concat_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      587 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/list/functions/list_contains_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1369 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/list/functions/list_distinct_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1987 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/list/functions/list_extract_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1058 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/list/functions/list_len_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1215 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/list/functions/list_position_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1078 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/list/functions/list_prepend_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      680 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/list/functions/list_product_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1550 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/list/functions/list_range_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      802 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/list/functions/list_reverse_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1309 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/list/functions/list_reverse_sort_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1928 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/list/functions/list_slice_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1333 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/list/functions/list_sort_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      676 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/list/functions/list_sum_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      846 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/list/functions/list_unique_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3175 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/list/vector_list_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/map/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/map/functions/
+-rw-rw-r--   0 runner    (1001) docker     (127)      872 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/map/functions/base_map_extract_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1580 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/map/functions/map_creation_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1515 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/map/functions/map_extract_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      658 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/map/functions/map_keys_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      712 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/map/functions/map_values_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/map/vector_map_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/null/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2772 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/null/null_function_executor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/null/null_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1154 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/null/vector_null_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/path/
+-rw-rw-r--   0 runner    (1001) docker     (127)     6252 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/path/path_function_executor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1090 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/path/vector_path_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      791 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/pointer_function_executor.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/rdf/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1299 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/rdf/rdf_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      393 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/rdf/vector_rdf_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      905 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/rewrite_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    10009 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/scalar_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1403 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/scalar_macro_function.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/schema/
+-rw-rw-r--   0 runner    (1001) docker     (127)      649 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/schema/label_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      276 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/schema/offset_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      642 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/schema/vector_label_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      529 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/schema/vector_node_rel_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/string/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/string/functions/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2242 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/string/functions/array_extract_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      669 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/string/functions/base_lower_upper_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2303 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/string/functions/base_pad_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      809 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/string/functions/base_regexp_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      429 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/string/functions/base_str_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/string/functions/contains_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      450 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/string/functions/ends_with_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1459 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/string/functions/find_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      575 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/string/functions/initcap_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      656 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/string/functions/left_operation.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1738 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/string/functions/levenshtein_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      444 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/string/functions/lower_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1035 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/string/functions/lpad_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      732 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/string/functions/ltrim_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      874 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/string/functions/pad_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3067 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_extract_all_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1778 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_extract_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      476 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_full_match_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      477 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_matches_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      710 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_replace_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      640 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/string/functions/repeat_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      570 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/string/functions/reverse_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      673 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/string/functions/right_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1035 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/string/functions/rpad_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      664 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/string/functions/rtrim_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      401 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/string/functions/starts_with_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2808 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/string/functions/substr_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      587 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/string/functions/trim_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      509 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/string/functions/upper_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5574 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/string/vector_string_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/struct/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1383 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/struct/vector_struct_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/table/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1540 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/table/bind_data.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1717 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/table/bind_input.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2713 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/table/call_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1105 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/table/scan_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      527 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/table/scan_replacement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4030 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/table_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    22251 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/ternary_function_executor.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/timestamp/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1036 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/timestamp/timestamp_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      508 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/timestamp/vector_timestamp_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    10907 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/udf_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8481 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/unary_function_executor.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/union/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/union/functions/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1249 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/union/functions/union_tag.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      519 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/union/vector_union_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/uuid/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/uuid/functions/
+-rw-rw-r--   0 runner    (1001) docker     (127)      395 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/uuid/functions/gen_random_uuid.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      266 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/function/uuid/vector_uuid_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/main/
+-rw-rw-r--   0 runner    (1001) docker     (127)      607 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/main/attached_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1561 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/main/client_config.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6386 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/main/client_context.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7548 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/main/connection.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5799 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/main/database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      450 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/main/database_manager.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1546 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/main/db_config.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1394 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/main/kuzu.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1248 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/main/kuzu_fwd.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3548 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/main/plan_printer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1992 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/main/prepared_statement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4873 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/main/query_result.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1015 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/main/query_summary.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6746 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/main/settings.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      830 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/main/storage_driver.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      528 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/main/version.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/optimizer/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2295 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/optimizer/acc_hash_join_optimizer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      821 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/optimizer/agg_key_dependency_optimizer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      895 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/optimizer/correlated_subquery_unnest_solver.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2050 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/optimizer/factorization_rewriter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3150 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/optimizer/filter_push_down_optimizer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1376 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/optimizer/logical_operator_collector.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6889 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/optimizer/logical_operator_visitor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      298 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/optimizer/optimizer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2461 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/optimizer/projection_push_down_optimizer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      572 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/optimizer/remove_factorization_rewriter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      936 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/optimizer/remove_unnecessary_join_optimizer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      556 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/optimizer/top_k_optimizer.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/antlr_parser/
+-rw-rw-r--   0 runner    (1001) docker     (127)      895 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/antlr_parser/kuzu_cypher_parser.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      620 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/antlr_parser/parser_error_listener.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      373 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/antlr_parser/parser_error_strategy.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      468 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/attach_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      541 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/comment_on.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1793 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/copy.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1237 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/create_macro.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/ddl/
+-rw-rw-r--   0 runner    (1001) docker     (127)      397 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/ddl/alter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1748 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/ddl/alter_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      447 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/ddl/create_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1782 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/ddl/create_table_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/ddl/drop.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      429 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/detach_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      748 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/explain_statement.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/expression/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3933 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/expression/parsed_case_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3025 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/expression/parsed_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2663 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/expression/parsed_function_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1552 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/expression/parsed_literal_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      858 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/expression/parsed_parameter_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1688 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/expression/parsed_property_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/expression/parsed_subquery_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1546 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/expression/parsed_variable_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      626 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/extension_statement.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/parsed_data/
+-rw-rw-r--   0 runner    (1001) docker     (127)      177 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/parsed_data/attach_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1163 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/parsed_expression_visitor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2544 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/parsed_statement_visitor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      292 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/parser.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      975 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/port_db.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/query/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/
+-rw-rw-r--   0 runner    (1001) docker     (127)      946 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/node_pattern.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1100 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/pattern_element.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      587 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/pattern_element_chain.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1599 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/rel_pattern.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1309 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/query/query_part.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/
+-rw-rw-r--   0 runner    (1001) docker     (127)      982 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/in_query_call_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1521 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/load_from.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1212 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/match_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      587 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/reading_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      657 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/unwind_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      928 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/query/regular_query.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/query/return_with_clause/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2155 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/query/return_with_clause/projection_body.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      485 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/query/return_with_clause/return_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/query/return_with_clause/with_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1798 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/query/single_query.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/
+-rw-rw-r--   0 runner    (1001) docker     (127)      898 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/delete_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      601 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/insert_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1341 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/merge_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      538 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/set_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/updating_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1543 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/scan_source.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      712 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/standalone_call.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      945 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/statement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      568 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/transaction_statement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    12840 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/transformer.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/visitor/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1164 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/parser/visitor/statement_read_write_analyzer.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/join_order/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2656 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/join_order/cardinality_estimator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      801 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/join_order/cost_model.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      469 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/join_order/join_order_util.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2304 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/join_order_enumerator_context.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/ddl/
+-rw-rw-r--   0 runner    (1001) docker     (127)      754 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/ddl/logical_alter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      841 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/ddl/logical_create_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      920 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/ddl/logical_ddl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      795 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/ddl/logical_drop_table.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/extend/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1426 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/extend/base_logical_extend.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1121 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/extend/extend_direction.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1278 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/extend/logical_extend.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4582 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/extend/logical_recursive_extend.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      200 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/extend/recursive_join_type.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/factorization/
+-rw-rw-r--   0 runner    (1001) docker     (127)      442 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/factorization/flatten_resolver.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      950 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/factorization/sink_util.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2011 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/logical_accumulate.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2430 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/logical_aggregate.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      900 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/logical_attach_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1376 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/logical_comment_on.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1381 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/logical_create_macro.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1079 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/logical_cross_product.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      791 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/logical_detach_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1632 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/logical_distinct.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      784 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/logical_empty_result.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1603 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/logical_explain.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      991 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/logical_extension.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1117 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/logical_filter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      804 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/logical_flatten.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3562 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/logical_hash_join.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/logical_in_query_call.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1843 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/logical_intersect.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1297 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/logical_limit.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1147 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/logical_mark_accmulate.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      769 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/logical_multiplcity_reducer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1224 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/logical_node_label_filter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3398 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/logical_operator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1616 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/logical_order_by.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2156 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/logical_partitioner.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1176 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/logical_plan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1179 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/logical_plan_util.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1117 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/logical_projection.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1094 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/logical_standalone_call.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      969 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/logical_transaction.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1199 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/logical_union.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1413 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/logical_unwind.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/persistent/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1473 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_copy_from.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1835 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_copy_to.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2791 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_delete.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1413 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_export_db.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      742 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_import_db.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2037 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_insert.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3728 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_merge.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2803 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_set.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/scan/
+-rw-rw-r--   0 runner    (1001) docker     (127)      643 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_dummy_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1290 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_expressions_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_index_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1217 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_scan_file.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1089 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_scan_internal_id.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1486 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_scan_node_property.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6001 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/schema.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/sip/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1588 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/sip/logical_semi_masker.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      308 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/operator/sip/side_way_info_passing.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    16498 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/planner.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3416 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/planner/subplans_table.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1252 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/data_pos.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/execution_context.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2051 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/expression_mapper.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/
+-rw-rw-r--   0 runner    (1001) docker     (127)    11146 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/aggregate_hash_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1255 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/aggregate_input.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1824 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/base_aggregate.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1374 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/base_aggregate_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3698 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/hash_aggregate.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1905 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/hash_aggregate_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2811 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/simple_aggregate.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1565 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/simple_aggregate_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      855 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/attach_database.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/call/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2956 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/call/in_query_call.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1382 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/call/standalone_call.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1712 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/comment_on.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2858 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/cross_product.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/ddl/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1402 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/ddl/alter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      779 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/ddl/create_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      945 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/ddl/ddl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      777 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/ddl/drop_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      777 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/detach_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      583 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/empty_result.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2713 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/filter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      795 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/filtering_operator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1255 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/flatten.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/hash_join/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4460 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/hash_join/hash_join_build.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4761 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/hash_join/hash_join_probe.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3299 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/hash_join/join_hash_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2359 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/index_lookup.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1541 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/index_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1025 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/install_extension.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/intersect/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3204 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/intersect/intersect.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1057 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/intersect/intersect_build.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1208 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/limit.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      942 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/load_extension.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/macro/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1852 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/macro/create_macro.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5181 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/mask.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      972 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/multiplicity_reducer.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/order_by/
+-rw-rw-r--   0 runner    (1001) docker     (127)     7982 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/order_by/key_block_merger.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1868 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1742 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by_data_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6358 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by_key_encoder.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2060 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by_merge.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2533 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3873 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/order_by/radix_sort.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2942 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/order_by/sort_state.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6218 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/order_by/top_k.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1694 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/order_by/top_k_scanner.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5655 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/partitioner.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2873 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/batch_insert.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      983 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/copy_rdf.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2150 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/copy_to.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3177 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/copy_to_csv.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2821 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/copy_to_parquet.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1604 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/delete.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6124 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/delete_executor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1005 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/export_db.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      840 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/file_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      734 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/import_db.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5477 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/index_builder.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1163 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/insert.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3808 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/insert_executor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2702 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/merge.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4654 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/node_batch_insert.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2367 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/base_csv_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1831 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/driver.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1862 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/parallel_csv_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1888 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/serial_csv_reader.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/npy/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1754 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/npy/npy_reader.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1480 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/boolean_column_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1616 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/callback_column_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5214 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/column_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1962 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/decode_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1358 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/interval_column_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1842 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/list_column_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4613 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/parquet_dbp_decoder.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4702 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/parquet_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4238 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/parquet_rle_bp_decoder.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      976 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/parquet_timestamp.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1842 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/resizable_buffer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1327 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/string_column_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1262 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/struct_column_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3426 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/templated_column_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6781 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/thrift_tools.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/
+-rw-rw-r--   0 runner    (1001) docker     (127)     5911 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/rdf_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7416 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/rdf_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      380 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/rdf_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2388 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/triple_store.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      865 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/reader_bind_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4368 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/rel_batch_insert.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1938 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/set.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6617 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/set_executor.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3914 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/basic_column_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2248 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/boolean_column_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4075 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/column_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1063 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/interval_column_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1729 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/list_column_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1087 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/parquet_rle_bp_encoder.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3213 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/parquet_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3898 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/standard_column_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5245 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/string_column_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1711 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/struct_column_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4992 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/physical_operator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1356 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/profile.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1518 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/projection.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2317 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/all_shortest_path_state.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3932 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/bfs_state.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1693 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/frontier.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6119 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/frontier_scanner.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4590 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/path_property_probe.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5732 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/recursive_join.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1380 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/scan_frontier.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1684 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/shortest_path_state.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1050 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/variable_length_state.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2908 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/result_collector.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/scan/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1769 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_multi_node_tables.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2072 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_multi_rel_tables.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2318 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_node_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2495 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_rel_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      840 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3474 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/scan_node_id.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5060 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/semi_masker.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1777 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1435 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/skip.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/table_scan/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1102 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/table_scan/ftable_scan_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3006 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/table_scan/union_all_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1095 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/transaction.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1499 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/operator/unwind.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      388 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/physical_plan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    12305 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/plan_mapper.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      638 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/processor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      621 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/processor_task.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/result/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1737 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/result/base_hash_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    16632 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/result/factorized_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1187 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/result/flat_tuple.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1061 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/result/mark_hash_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1547 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/result/result_set.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1063 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/processor/result/result_set_descriptor.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/buffer_manager/
+-rw-rw-r--   0 runner    (1001) docker     (127)     9404 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/buffer_manager/bm_file_handle.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    13079 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/buffer_manager/buffer_manager.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      527 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/buffer_manager/locked_queue.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2759 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/buffer_manager/memory_manager.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1714 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/buffer_manager/vm_region.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/compression/
+-rw-rw-r--   0 runner    (1001) docker     (127)    15336 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/compression/compression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1695 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/compression/sign_extend.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3328 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/file_handle.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/index/
+-rw-rw-r--   0 runner    (1001) docker     (127)    10995 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/index/hash_index.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8325 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/index/hash_index_builder.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1141 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/index/hash_index_header.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2132 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/index/hash_index_slot.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2450 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/index/hash_index_utils.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/local_storage/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2704 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/local_storage/local_node_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3256 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/local_storage/local_rel_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1052 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/local_storage/local_storage.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8905 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/local_storage/local_table.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/stats/
+-rw-rw-r--   0 runner    (1001) docker     (127)      999 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/stats/metadata_dah_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3254 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/stats/node_table_statistics.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4474 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/stats/nodes_store_statistics.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1594 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/stats/property_statistics.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3873 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/stats/rel_table_statistics.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3236 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/stats/rels_store_statistics.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1947 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/stats/table_statistics.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4425 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/stats/table_statistics_collection.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      821 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/storage_extension.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2909 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/storage_manager.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/storage_structure/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1571 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/storage_structure/db_file_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    13833 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/storage_structure/disk_array.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      368 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/storage_structure/in_mem_page.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5363 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/storage_structure/overflow_file.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7895 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/storage_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      774 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/storage_version_info.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/store/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4606 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/store/chunked_node_group.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1626 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/store/chunked_node_group_collection.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    13510 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/store/column.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9421 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/store/column_chunk.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2508 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/store/dictionary_chunk.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2908 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/store/dictionary_column.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5783 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/store/list_column.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3534 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/store/list_column_chunk.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5363 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/store/node_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1973 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/store/node_table_data.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2607 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/store/null_column.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8048 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/store/rel_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    11916 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/store/rel_table_data.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3509 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/store/string_column.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2511 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/store/string_column_chunk.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3320 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/store/struct_column.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1968 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/store/struct_column_chunk.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3604 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/store/table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2552 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/store/table_data.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/wal/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3663 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/wal/wal.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8162 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/wal/wal_record.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2356 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/wal_replayer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      725 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/storage/wal_replayer_utils.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/transaction/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1893 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/transaction/transaction.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      294 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/transaction/transaction_action.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2414 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/transaction/transaction_context.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3747 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/include/transaction/transaction_manager.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/main/
+-rw-rw-r--   0 runner    (1001) docker     (127)      414 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/main/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    20126 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/main/client_context.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3262 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/main/connection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11677 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/main/database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1232 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/main/database_manager.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1268 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/main/db_config.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    13980 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/main/plan_printer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      956 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/main/prepared_statement.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4090 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/main/query_result.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      578 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/main/query_summary.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3755 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/main/storage_driver.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      317 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/main/version.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/optimizer/
+-rw-rw-r--   0 runner    (1001) docker     (127)      602 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/optimizer/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    10541 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/optimizer/acc_hash_join_optimizer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3540 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/optimizer/agg_key_dependency_optimizer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1488 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/optimizer/correlated_subquery_unnest_solver.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    10339 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/optimizer/factorization_rewriter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    10504 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/optimizer/filter_push_down_optimizer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      340 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/optimizer/logical_operator_collector.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5558 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/optimizer/logical_operator_visitor.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2087 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/optimizer/optimizer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    13109 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/optimizer/projection_push_down_optimizer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1201 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/optimizer/remove_factorization_rewriter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1537 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/optimizer/remove_unnecessary_join_optimizer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1902 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/optimizer/top_k_optimizer.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/
+-rw-rw-r--   0 runner    (1001) docker     (127)      400 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/antlr_parser/
+-rw-rw-r--   0 runner    (1001) docker     (127)      267 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/antlr_parser/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1595 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/antlr_parser/kuzu_cypher_parser.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1391 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/antlr_parser/parser_error_listener.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      827 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/antlr_parser/parser_error_strategy.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      455 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/create_macro.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/expression/
+-rw-rw-r--   0 runner    (1001) docker     (127)      346 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/expression/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2127 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/expression/parsed_case_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3281 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/expression/parsed_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      785 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/expression/parsed_function_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      491 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/expression/parsed_property_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      491 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/expression/parsed_variable_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3506 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/parsed_expression_visitor.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4309 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/parsed_statement_visitor.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1259 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/parser.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/transform/
+-rw-rw-r--   0 runner    (1001) docker     (127)      691 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/transform/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      646 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/transform/transform_attach_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      450 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/transform/transform_comment_on.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3602 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/transform/transform_copy.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7632 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/transform/transform_ddl.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      392 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/transform/transform_detach_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    27904 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/transform/transform_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      858 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/transform/transform_extension.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7789 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/transform/transform_graph_pattern.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1272 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/transform/transform_macro.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      833 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/transform/transform_port_db.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2587 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/transform/transform_projection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2253 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/transform/transform_query.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2715 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/transform/transform_reading_clause.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      484 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/transform/transform_standalone_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1209 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/transform/transform_transaction.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2681 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/transform/transform_updating_clause.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4394 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/transformer.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/visitor/
+-rw-rw-r--   0 runner    (1001) docker     (127)      209 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/visitor/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      258 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/parser/visitor/statement_read_write_analyzer.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/
+-rw-rw-r--   0 runner    (1001) docker     (127)      339 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/join_order/
+-rw-rw-r--   0 runner    (1001) docker     (127)      251 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/join_order/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     5776 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/join_order/cardinality_estimator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1652 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/join_order/cost_model.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      745 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/join_order/join_order_util.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1233 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/join_order_enumerator_context.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1000 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/ddl/
+-rw-rw-r--   0 runner    (1001) docker     (127)      175 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/ddl/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/ddl/logical_ddl.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/extend/
+-rw-rw-r--   0 runner    (1001) docker     (127)      253 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/extend/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1348 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/extend/base_logical_extend.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1169 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/extend/logical_extend.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2914 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/extend/logical_recursive_extend.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/factorization/
+-rw-rw-r--   0 runner    (1001) docker     (127)      223 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/factorization/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1007 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/factorization/flatten_resolver.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2591 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/factorization/sink_util.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1552 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/logical_accumulate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2870 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/logical_aggregate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      517 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/logical_comment_on.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      523 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/logical_create_macro.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      829 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/logical_cross_product.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1523 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/logical_distinct.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      764 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/logical_dummy_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      800 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/logical_explain.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      822 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/logical_filter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      407 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/logical_flatten.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7224 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/logical_hash_join.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      726 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/logical_in_query_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2606 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/logical_intersect.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1039 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/logical_limit.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1514 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/logical_mark_accumulate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6201 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/logical_operator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2805 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/logical_order_by.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      939 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/logical_partitioner.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1065 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/logical_plan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3973 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/logical_plan_util.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2197 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/logical_projection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1947 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/logical_union.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      980 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/logical_unwind.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/persistent/
+-rw-rw-r--   0 runner    (1001) docker     (127)      388 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/persistent/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      853 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_copy_from.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      620 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_copy_to.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1732 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_delete.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      303 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_export_db.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      303 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_import_db.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2031 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_insert.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1366 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_merge.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2384 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_set.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/scan/
+-rw-rw-r--   0 runner    (1001) docker     (127)      328 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/scan/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      347 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/scan/logical_expressions_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      935 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/scan/logical_index_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      643 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/scan/logical_scan_file.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      481 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/scan/logical_scan_internal_id.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      561 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/scan/logical_scan_node_property.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5563 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/operator/schema.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/plan/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1042 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/plan/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1329 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/plan/append_accumulate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      814 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/plan/append_aggregate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      816 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/plan/append_cross_product.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1971 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/plan/append_delete.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      553 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/plan/append_distinct.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      399 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/plan/append_dummy_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      473 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/plan/append_expressions_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    13525 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/plan/append_extend.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      913 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/plan/append_filter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      800 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/plan/append_flatten.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      740 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/plan/append_in_query_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2692 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/plan/append_insert.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4805 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/plan/append_join.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      552 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/plan/append_limit.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      658 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/plan/append_mark_accumulate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      439 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/plan/append_multiplicity_reducer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      615 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/plan/append_order_by.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1452 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/plan/append_projection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      684 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/plan/append_scan_file.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1596 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/plan/append_scan_node.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2066 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/plan/append_set.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5734 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/plan/append_simple.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/plan/append_standalone_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      826 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/plan/append_unwind.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8216 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/plan/plan_copy.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    27166 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/plan/plan_join_order.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2531 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/plan/plan_port_db.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3074 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/plan/plan_projection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5987 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/plan/plan_read.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1829 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/plan/plan_single_query.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/plan/plan_standalone_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8673 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/plan/plan_subquery.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6119 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/plan/plan_update.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3409 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/planner.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5305 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/query_planner.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3769 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/planner/subplans_table.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/
+-rw-rw-r--   0 runner    (1001) docker     (127)      272 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1577 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     4774 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/create_factorized_table_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2148 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/create_result_collector.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8285 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/expression_mapper.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      702 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_acc_hash_join.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1102 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_accumulate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9380 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_aggregate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      638 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_attach_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1046 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_comment_on.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    15120 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_copy_from.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4729 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_copy_to.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_create_macro.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1880 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_cross_product.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_ddl.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6221 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_delete.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      634 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_detach_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      750 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_distinct.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1595 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_dummy_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      345 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_empty_result.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1956 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_explain.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1871 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_expressions_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6300 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_extend.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1014 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_extension.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      822 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_filter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      606 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_flatten.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5998 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_hash_join.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1217 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_in_query_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2425 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_index_scan_node.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5186 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_insert.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3182 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_intersect.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      933 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_label_filter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1344 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_limit.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      784 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_mark_accumulate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2627 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_merge.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      533 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_multiplicity_reducer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4327 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_order_by.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6873 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_path_property_probe.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2256 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_port_db.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1251 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_projection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3488 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_recursive_extend.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1457 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_scan_file.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      816 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_scan_frontier.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1090 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_scan_node.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3525 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_scan_node_property.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3246 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_semi_masker.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6610 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_set.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      982 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_standalone_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      593 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_transaction.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2083 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_union.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1096 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/map_unwind.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8226 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/map/plan_mapper.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1054 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/aggregate/
+-rw-rw-r--   0 runner    (1001) docker     (127)      400 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/aggregate/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    37374 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/aggregate/aggregate_hash_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1691 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/aggregate/base_aggregate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      755 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/aggregate/base_aggregate_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5470 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/aggregate/hash_aggregate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2004 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/aggregate/hash_aggregate_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4848 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/aggregate/simple_aggregate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1344 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/aggregate/simple_aggregate_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      720 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/attach_database.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/call/
+-rw-rw-r--   0 runner    (1001) docker     (127)      230 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/call/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2958 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/call/in_query_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      997 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/call/standalone_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      803 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/comment_on.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1383 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/cross_product.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/ddl/
+-rw-rw-r--   0 runner    (1001) docker     (127)      256 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/ddl/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2464 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/ddl/alter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      725 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/ddl/create_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      570 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/ddl/ddl.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      504 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/ddl/drop_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      413 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/detach_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      213 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/empty_result.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2463 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/filter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1043 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/filtering_operator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1306 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/flatten.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/hash_join/
+-rw-rw-r--   0 runner    (1001) docker     (127)      270 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/hash_join/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2057 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/hash_join/hash_join_build.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8290 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/hash_join/hash_join_probe.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9252 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/hash_join/join_hash_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5915 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/index_lookup.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1779 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/index_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2359 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/install_extension.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/intersect/
+-rw-rw-r--   0 runner    (1001) docker     (127)      208 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/intersect/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     9664 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/intersect/intersect.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1389 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/limit.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2167 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/load_extension.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/macro/
+-rw-rw-r--   0 runner    (1001) docker     (127)      217 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/macro/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      727 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/macro/create_macro.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      538 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/multiplicity_reducer.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/order_by/
+-rw-rw-r--   0 runner    (1001) docker     (127)      410 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/order_by/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    16047 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/order_by/key_block_merger.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1082 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/order_by/order_by.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    14058 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/order_by/order_by_key_encoder.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1554 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/order_by/order_by_merge.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1438 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/order_by/order_by_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    12968 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/order_by/radix_sort.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9014 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/order_by/sort_state.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    12786 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/order_by/top_k.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      834 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/order_by/top_k_scanner.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7795 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/partitioner.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/
+-rw-rw-r--   0 runner    (1001) docker     (127)      647 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      472 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/batch_insert.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      473 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/copy_rdf.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      760 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/copy_to.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8388 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/copy_to_csv.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1782 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/copy_to_parquet.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1751 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/delete.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5443 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/delete_executor.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3552 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/export_db.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      393 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/import_db.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4762 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/index_builder.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      861 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/insert.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7316 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/insert_executor.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3038 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/merge.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8703 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/node_batch_insert.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/
+-rw-rw-r--   0 runner    (1001) docker     (127)      325 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/
+-rw-rw-r--   0 runner    (1001) docker     (127)      297 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    14378 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/base_csv_reader.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4367 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/driver.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8564 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/parallel_csv_reader.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6543 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/serial_csv_reader.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/npy/
+-rw-rw-r--   0 runner    (1001) docker     (127)      211 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/npy/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    13865 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/npy/npy_reader.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/
+-rw-rw-r--   0 runner    (1001) docker     (127)      445 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      850 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/boolean_column_reader.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    23447 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/column_reader.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1234 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/interval_column_reader.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5995 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/list_column_reader.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    29865 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/parquet_reader.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1369 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/parquet_timestamp.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3928 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/string_column_reader.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3449 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/struct_column_reader.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/
+-rw-rw-r--   0 runner    (1001) docker     (127)      254 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    13988 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/rdf_reader.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    13452 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/rdf_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2966 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/rdf_utils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2052 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/reader_bind_utils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11395 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/rel_batch_insert.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      997 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/set.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6592 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/set_executor.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/
+-rw-rw-r--   0 runner    (1001) docker     (127)      564 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    12826 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/basic_column_writer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1538 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/boolean_column_writer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    16464 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/column_writer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1539 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/interval_column_writer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4734 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/list_column_writer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2633 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/parquet_rle_bp_encoder.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11697 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/parquet_writer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8703 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/string_column_writer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4078 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/struct_column_writer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8457 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/physical_operator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1033 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/profile.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1757 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/projection.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/
+-rw-rw-r--   0 runner    (1001) docker     (127)      337 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      790 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/frontier.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6736 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/frontier_scanner.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5067 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/path_property_probe.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    12653 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/recursive_join.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      323 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/scan_frontier.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2479 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/result_collector.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/scan/
+-rw-rw-r--   0 runner    (1001) docker     (127)      323 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/scan/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      825 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/scan/scan_multi_node_tables.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3865 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/scan/scan_multi_rel_tables.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      625 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/scan/scan_node_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      651 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/scan/scan_rel_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      463 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/scan/scan_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5110 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/scan_node_id.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4582 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/semi_masker.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2403 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/skip.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/table_scan/
+-rw-rw-r--   0 runner    (1001) docker     (127)      248 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/table_scan/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2486 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/table_scan/ftable_scan_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1832 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/table_scan/union_all_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1256 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/transaction.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2659 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/operator/unwind.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2709 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/processor.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1788 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/processor_task.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/result/
+-rw-rw-r--   0 runner    (1001) docker     (127)      336 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/result/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     7142 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/result/base_hash_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    34515 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/result/factorized_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2119 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/result/flat_tuple.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2304 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/result/mark_hash_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1494 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/result/result_set.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1170 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/processor/result/result_set_descriptor.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/
+-rw-rw-r--   0 runner    (1001) docker     (127)      537 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/buffer_manager/
+-rw-rw-r--   0 runner    (1001) docker     (127)      277 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/buffer_manager/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     7039 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/buffer_manager/bm_file_handle.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    15692 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/buffer_manager/buffer_manager.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2101 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/buffer_manager/memory_manager.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3721 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/buffer_manager/vm_region.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/compression/
+-rw-rw-r--   0 runner    (1001) docker     (127)      258 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/compression/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    35565 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/compression/compression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1880 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/file_handle.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/index/
+-rw-rw-r--   0 runner    (1001) docker     (127)      210 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/index/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    19280 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/index/hash_index.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    13484 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/index/hash_index_builder.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/local_storage/
+-rw-rw-r--   0 runner    (1001) docker     (127)      279 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/local_storage/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     8095 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/local_storage/local_node_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    12529 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/local_storage/local_rel_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1723 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/local_storage/local_storage.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5406 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/local_storage/local_table.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/stats/
+-rw-rw-r--   0 runner    (1001) docker     (127)      415 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/stats/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1201 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/stats/metadata_dah_info.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7957 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/stats/node_table_statistics.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4352 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/stats/nodes_store_statistics.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2446 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/stats/property_statistics.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5129 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/stats/rel_table_statistics.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4017 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/stats/rels_store_statistics.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2843 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/stats/table_statistics.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5914 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/stats/table_statistics_collection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    10057 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/storage_manager.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/storage_structure/
+-rw-rw-r--   0 runner    (1001) docker     (127)      263 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/storage_structure/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     5596 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/storage_structure/db_file_utils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    20740 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/storage_structure/disk_array.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      557 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/storage_structure/in_mem_page.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9484 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/storage_structure/overflow_file.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4286 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/storage_utils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      737 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/storage_version_info.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/store/
+-rw-rw-r--   0 runner    (1001) docker     (127)      649 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/store/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     6855 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/store/chunked_node_group.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2126 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/store/chunked_node_group_collection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    43789 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/store/column.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    27598 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/store/column_chunk.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3687 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/store/dictionary_chunk.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    10487 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/store/dictionary_column.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    22685 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/store/list_column.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    16128 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/store/list_column_chunk.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9981 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/store/node_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4163 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/store/node_table_data.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9068 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/store/null_column.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8480 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/store/rel_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    48499 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/store/rel_table_data.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11550 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/store/string_column.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7831 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/store/string_column_chunk.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11743 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/store/struct_column.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6206 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/store/struct_column_chunk.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1779 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/store/table_data.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/wal/
+-rw-rw-r--   0 runner    (1001) docker     (127)      191 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/wal/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     6531 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/wal/wal.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6783 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/wal/wal_record.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    17846 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/wal_replayer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1169 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/storage/wal_replayer_utils.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/transaction/
+-rw-rw-r--   0 runner    (1001) docker     (127)      216 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/transaction/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     3894 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/transaction/transaction_context.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4629 2024-04-16 08:04:19.000000 sdist/kuzu-source/src/transaction/transaction_manager.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/
+-rw-rw-r--   0 runner    (1001) docker     (127)      436 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_cypher/
+-rw-rw-r--   0 runner    (1001) docker     (127)      949 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_cypher/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    56460 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_cypher/cypher_lexer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)   467402 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_cypher/cypher_parser.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_cypher/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3261 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_cypher/include/cypher_lexer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    87738 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_cypher/include/cypher_parser.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/
+-rw-rw-r--   0 runner    (1001) docker     (127)    10564 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     4237 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/LICENSE
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/
+-rw-rw-r--   0 runner    (1001) docker     (127)      285 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRErrorListener.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     8375 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRErrorListener.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      285 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRErrorStrategy.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5269 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRErrorStrategy.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      552 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRFileStream.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1018 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRFileStream.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4326 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRInputStream.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2623 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRInputStream.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1804 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BailErrorStrategy.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2483 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BailErrorStrategy.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1163 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BaseErrorListener.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1377 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BaseErrorListener.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     9946 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BufferedTokenStream.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     8014 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BufferedTokenStream.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      281 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CharStream.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1479 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CharStream.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4459 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonToken.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4918 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonToken.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1327 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonTokenFactory.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2564 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonTokenFactory.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1767 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonTokenStream.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2713 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonTokenStream.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      597 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ConsoleErrorListener.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1060 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ConsoleErrorListener.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    11864 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/DefaultErrorStrategy.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)    20289 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/DefaultErrorStrategy.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3484 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/DiagnosticErrorListener.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3600 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/DiagnosticErrorListener.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2152 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Exceptions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3868 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Exceptions.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1867 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/FailedPredicateException.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1096 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/FailedPredicateException.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2767 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/FlatHashMap.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2676 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/FlatHashSet.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      559 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/InputMismatchException.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      783 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/InputMismatchException.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      350 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/IntStream.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)    10251 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/IntStream.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      615 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/InterpreterRuleContext.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1604 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/InterpreterRuleContext.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6878 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Lexer.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     7038 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Lexer.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1867 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/LexerInterpreter.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1564 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/LexerInterpreter.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1234 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/LexerNoViableAltException.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      916 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/LexerNoViableAltException.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2412 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ListTokenSource.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3795 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ListTokenSource.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1585 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/NoViableAltException.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1693 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/NoViableAltException.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    19305 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Parser.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)    19393 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Parser.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    10523 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ParserInterpreter.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     7171 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ParserInterpreter.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3952 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ParserRuleContext.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5666 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ParserRuleContext.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1958 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ProxyErrorListener.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1657 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ProxyErrorListener.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1916 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RecognitionException.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3961 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RecognitionException.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4572 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Recognizer.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5733 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Recognizer.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3588 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuleContext.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5561 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuleContext.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      725 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuleContextWithAltNum.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      985 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuleContextWithAltNum.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2091 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuntimeMetaData.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     7393 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuntimeMetaData.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      246 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Token.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3462 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Token.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1217 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenFactory.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      264 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenSource.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3839 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenSource.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      284 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenStream.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6098 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenStream.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    15023 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenStreamRewriter.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)    12507 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenStreamRewriter.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5847 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/UnbufferedCharStream.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4351 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/UnbufferedCharStream.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     7467 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/UnbufferedTokenStream.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4241 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/UnbufferedTokenStream.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2105 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Version.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1907 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Vocabulary.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6943 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Vocabulary.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      270 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/WritableToken.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      676 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/WritableToken.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2560 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/antlr4-common.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5524 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/antlr4-runtime.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4193 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATN.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4845 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATN.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4158 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNConfig.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5513 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNConfig.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6500 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNConfigSet.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5185 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNConfigSet.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1252 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNDeserializationOptions.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1302 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNDeserializationOptions.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    21573 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNDeserializer.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      835 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNDeserializer.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1216 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNSimulator.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2761 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNSimulator.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1538 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNState.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4374 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNState.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      990 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNStateType.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      796 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNStateType.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      439 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNType.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1214 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ActionTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1104 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ActionTransition.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      604 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/AmbiguityInfo.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3295 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/AmbiguityInfo.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4211 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ArrayPredictionContext.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1900 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ArrayPredictionContext.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      840 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/AtomTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1084 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/AtomTransition.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      729 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/BasicBlockStartState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      649 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/BasicState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      762 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/BlockEndState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      853 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/BlockStartState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      520 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ContextSensitivityInfo.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2123 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ContextSensitivityInfo.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      561 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionEventInfo.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2459 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionEventInfo.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      934 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionInfo.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     9762 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionInfo.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      342 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionState.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      960 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      969 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/EpsilonTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1402 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/EpsilonTransition.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      527 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ErrorInfo.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1861 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ErrorInfo.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      416 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/HashUtils.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     7271 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LL1Analyzer.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3275 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LL1Analyzer.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2950 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerATNConfig.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1666 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerATNConfig.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    22025 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerATNSimulator.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     8819 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerATNSimulator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      324 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3494 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4031 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerActionExecutor.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6150 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerActionExecutor.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1460 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerActionType.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1306 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerChannelAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1908 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerChannelAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1555 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerCustomAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2772 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerCustomAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1784 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerIndexedCustomAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3046 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerIndexedCustomAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1269 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerModeAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1780 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerModeAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      977 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerMoreAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1701 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerMoreAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1010 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerPopModeAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1735 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerPopModeAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1311 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerPushModeAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1817 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerPushModeAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      977 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerSkipAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1664 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerSkipAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1269 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerTypeAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1717 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerTypeAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      584 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LookaheadEventInfo.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1914 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LookaheadEventInfo.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      736 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LoopEndState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      868 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/NotSetTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      854 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/NotSetTransition.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      484 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/OrderedATNConfigSet.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      631 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/OrderedATNConfigSet.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2789 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParseInfo.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3665 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParseInfo.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    53167 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParserATNSimulator.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)    45705 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParserATNSimulator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2278 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParserATNSimulatorOptions.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1052 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PlusBlockStartState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      842 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PlusLoopbackState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      901 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PrecedencePredicateTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1187 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PrecedencePredicateTransition.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      685 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredicateEvalInfo.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2885 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredicateEvalInfo.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1009 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredicateTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1674 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredicateTransition.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    20987 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContext.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     9173 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContext.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2360 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextCache.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2738 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextCache.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5386 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextMergeCache.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4033 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextMergeCache.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2602 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextMergeCacheOptions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextType.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5939 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionMode.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)    20991 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionMode.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     7943 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ProfilingATNSimulator.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2982 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ProfilingATNSimulator.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      891 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RangeTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      944 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RangeTransition.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      746 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RuleStartState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      911 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RuleStopState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1156 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RuleTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1484 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RuleTransition.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    14979 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SemanticContext.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     9030 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SemanticContext.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      451 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SemanticContextType.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3246 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SerializedATNView.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      898 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SetTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1267 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SetTransition.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2870 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SingletonPredictionContext.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1834 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SingletonPredictionContext.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      754 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/StarBlockStartState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1140 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/StarLoopEntryState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      644 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/StarLoopbackState.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      733 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/StarLoopbackState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      762 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/TokensStartState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      911 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/Transition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2164 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/Transition.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      730 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/TransitionType.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      778 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/TransitionType.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      680 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/WildcardTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      839 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/WildcardTransition.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2868 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFA.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3045 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFA.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1726 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFASerializer.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      772 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFASerializer.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1490 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFAState.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6068 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFAState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      509 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/LexerDFASerializer.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      533 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/LexerDFASerializer.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/internal/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2694 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/internal/Synchronization.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5499 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/internal/Synchronization.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3098 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/InterpreterDataReader.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      989 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/InterpreterDataReader.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1671 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/Interval.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3009 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/Interval.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    13209 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/IntervalSet.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6478 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/IntervalSet.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2820 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/MurmurHash.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3595 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/MurmurHash.h
+-rw-rw-r--   0 runner    (1001) docker     (127)       71 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/Predicate.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      446 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/Predicate.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/
+-rw-rw-r--   0 runner    (1001) docker     (127)      242 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Any.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      370 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Any.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      966 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Arrays.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3620 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Arrays.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1828 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/BitSet.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4837 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/CPPUtils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2582 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/CPPUtils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1195 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Casts.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4122 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Declarations.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      901 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/StringUtils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      425 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/StringUtils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      723 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Unicode.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8728 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Utf8.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2148 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Utf8.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5650 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/AbstractParseTreeVisitor.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      677 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ErrorNode.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1255 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ErrorNodeImpl.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1429 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ErrorNodeImpl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1906 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/IterativeParseTreeWalker.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2124 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/IterativeParseTreeWalker.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      349 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTree.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4224 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTree.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      288 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeListener.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1213 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeListener.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1434 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeProperty.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      430 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeType.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      285 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeVisitor.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2212 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeVisitor.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1381 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeWalker.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2031 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeWalker.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1145 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/TerminalNode.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1281 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/TerminalNodeImpl.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1003 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/TerminalNodeImpl.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6872 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/Trees.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3060 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/Trees.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/
+-rw-rw-r--   0 runner    (1001) docker     (127)      274 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/Chunk.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1460 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/Chunk.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1868 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreeMatch.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5768 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreeMatch.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1800 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreePattern.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4384 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreePattern.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    12574 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreePatternMatcher.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     8715 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreePatternMatcher.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1820 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/RuleTagToken.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4742 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/RuleTagToken.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      811 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TagChunk.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3030 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TagChunk.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      623 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TextChunk.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1464 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TextChunk.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      959 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TokenTagToken.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2786 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TokenTagToken.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4960 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPath.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2824 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPath.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      747 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathElement.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1029 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathElement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6047 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1169 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexer.g4
+-rw-rw-r--   0 runner    (1001) docker     (127)     1349 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)       98 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexer.tokens
+-rwxrwxr-x   0 runner    (1001) docker     (127)      506 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexerErrorListener.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      635 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexerErrorListener.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      647 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathRuleAnywhereElement.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      709 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathRuleAnywhereElement.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      966 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathRuleElement.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      620 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathRuleElement.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      647 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathTokenAnywhereElement.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      631 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathTokenAnywhereElement.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1054 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathTokenElement.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      623 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathTokenElement.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      665 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathWildcardAnywhereElement.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      558 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathWildcardAnywhereElement.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      621 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathWildcardElement.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      542 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathWildcardElement.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/fast_float/
+-rw-rw-r--   0 runner    (1001) docker     (127)       92 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/fast_float/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/fast_float/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)    94376 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/fast_float/include/fast_float.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/fastpfor/
+-rw-rw-r--   0 runner    (1001) docker     (127)      150 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/fastpfor/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    10273 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/fastpfor/LICENSE
+-rw-rw-r--   0 runner    (1001) docker     (127)     1278 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/fastpfor/README
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/
+-rw-rw-r--   0 runner    (1001) docker     (127)    59414 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/bitpacking.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    32124 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/bitpacking.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    23572 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/bitpackinghelpers.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      273 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/common.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/glob/
+-rw-rw-r--   0 runner    (1001) docker     (127)      100 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/glob/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/glob/glob/
+-rw-rw-r--   0 runner    (1001) docker     (127)    13001 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/glob/glob/glob.hpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/httplib/
+-rw-rw-r--   0 runner    (1001) docker     (127)   311527 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/httplib/httplib.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/
+-rw-rw-r--   0 runner    (1001) docker     (127)      918 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    11358 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/LICENSE
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/include/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/
+-rw-rw-r--   0 runner    (1001) docker     (127)    26550 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/aes.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    15024 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/aria.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    25694 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/asn1.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3085 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/base64.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    42463 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/bignum.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2394 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/build_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    13062 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/camellia.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    25326 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/ccm.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    38245 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/check_config.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    51905 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/cipher.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1452 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/constant_time.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    11057 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/des.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9867 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/entropy.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7031 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/error.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    16632 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/gcm.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      531 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/mbedtls_config.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    17120 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/md.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4949 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/memory_buffer_alloc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    41167 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/oid.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5270 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/pem.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    35543 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/pk.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    14433 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/platform.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1973 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/platform_time.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8667 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/platform_util.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      978 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/private_access.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    51957 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/rsa.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7854 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/sha1.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6640 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/sha256.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7084 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/sha512.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/library/
+-rw-rw-r--   0 runner    (1001) docker     (127)    73166 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/library/aes.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    36996 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/library/aria.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11007 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/library/asn1parse.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6762 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/library/base64.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    79733 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/library/bignum.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    56414 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/library/bn_mul.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    36100 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/library/camellia.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    47452 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/library/cipher.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    49271 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/library/cipher_wrap.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4532 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/library/cipher_wrap.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    17543 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/library/common.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    26144 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/library/constant_time.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    12167 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/library/constant_time_internal.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1638 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/library/constant_time_invasive.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    18774 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/library/entropy.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6513 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/library/entropy_poll.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2139 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/library/entropy_poll.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    34742 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/library/gcm.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    21294 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/library/md.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2086 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/library/md_wrap.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    27822 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/library/oid.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    14294 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/library/pem.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    17719 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/library/pk.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    29099 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/library/pk_wrap.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4205 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/library/pk_wrap.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    44156 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/library/pkparse.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5125 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/library/platform_util.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    69416 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/library/rsa.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    13253 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/library/rsa_alt_helpers.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8442 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/library/rsa_alt_helpers.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    15171 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/library/sha1.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    16212 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/library/sha256.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    18253 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/mbedtls/library/sha512.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1079 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       46 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/LICENSE
+-rw-rw-r--   0 runner    (1001) docker     (127)      976 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/Makefile
+-rw-rw-r--   0 runner    (1001) docker     (127)     1879 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/README.md
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/
+-rw-rw-r--   0 runner    (1001) docker     (127)      320 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/parquet_constants.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      406 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/parquet_constants.h
+-rw-rw-r--   0 runner    (1001) docker     (127)   200148 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/parquet_types.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    72715 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/parquet_types.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1262 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/windows_compatibility.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/
+-rwxrwxr-x   0 runner    (1001) docker     (127)     9816 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-internal.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3296 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-sinksource.cc
+-rwxrwxr-x   0 runner    (1001) docker     (127)     7266 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-sinksource.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1837 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-stubs-internal.cc
+-rwxrwxr-x   0 runner    (1001) docker     (127)    15040 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-stubs-internal.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2900 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-stubs-public.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    59102 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy.cc
+-rwxrwxr-x   0 runner    (1001) docker     (127)     9748 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3555 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/TApplicationException.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1208 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/TBase.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6849 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/TLogging.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3185 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/TToString.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3290 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/Thrift.h
+-rw-rw-r--   0 runner    (1001) docker     (127)       65 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/config.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/
+-rwxrwxr-x   0 runner    (1001) docker     (127)     7931 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TCompactProtocol.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    23953 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TCompactProtocol.tcc
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1140 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocol.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)    21319 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocol.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6374 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocolDecorator.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3216 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocolException.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1151 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocolTypes.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    18266 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TVirtualProtocol.h
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/stdcxx.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      896 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/thrift-config.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      460 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/thrift_export.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4624 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/PlatformSocket.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3699 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TBufferTransports.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)    15004 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TBufferTransports.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     9004 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TTransport.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1862 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TTransportException.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3335 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TTransportException.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5167 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TVirtualTransport.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniz/
+-rw-rw-r--   0 runner    (1001) docker     (127)      192 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniz/CMakeLists.txt
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1184 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniz/LICENSE
+-rwxrwxr-x   0 runner    (1001) docker     (127)   313123 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniz/miniz.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)    66103 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniz/miniz.hpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5058 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/miniz/miniz_wrapper.hpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/nlohmann_json/
+-rw-rw-r--   0 runner    (1001) docker     (127)   907860 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/nlohmann_json/json.hpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6268 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/nlohmann_json/json_fwd.hpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pcg/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1092 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pcg/LICENSE
+-rw-rw-r--   0 runner    (1001) docker     (127)    20241 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pcg/pcg_extras.hpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    73551 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pcg/pcg_random.hpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    24875 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pcg/pcg_uint128.hpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/
+-rw-rw-r--   0 runner    (1001) docker     (127)    11983 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1684 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/LICENSE
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/include/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/
+-rw-rw-r--   0 runner    (1001) docker     (127)    23979 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/attr.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7069 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/buffer_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    65560 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/cast.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8458 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/chrono.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      120 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/common.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2096 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/complex.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/
+-rw-rw-r--   0 runner    (1001) docker     (127)    28251 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/class.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    52330 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/common.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5491 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/descr.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    17932 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/init.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    26305 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/internals.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    42266 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1625 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/typeid.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eigen/
+-rw-rw-r--   0 runner    (1001) docker     (127)    31418 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eigen/matrix.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    18120 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eigen/tensor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      316 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eigen.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    11889 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/embed.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4731 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eval.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5002 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/functional.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8262 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/gil.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8862 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/iostream.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    79412 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/numpy.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9103 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/operators.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/options.h
+-rw-rw-r--   0 runner    (1001) docker     (127)   126075 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/pybind11.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    93433 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/pytypes.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/stl/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4185 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/stl/filesystem.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    15337 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/stl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    27013 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/stl_bind.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/tools/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2350 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/tools/FindCatch.cmake
+-rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/tools/FindEigen3.cmake
+-rw-rw-r--   0 runner    (1001) docker     (127)    11103 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/tools/FindPythonLibsNew.cmake
+-rw-rw-r--   0 runner    (1001) docker     (127)      817 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/tools/JoinPaths.cmake
+-rw-rw-r--   0 runner    (1001) docker     (127)     1423 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/tools/check-style.sh
+-rw-rw-r--   0 runner    (1001) docker     (127)      952 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/tools/cmake_uninstall.cmake.in
+-rw-rw-r--   0 runner    (1001) docker     (127)     1040 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1031 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/tools/libsize.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1282 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/tools/make_changelog.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      196 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11.pc.in
+-rw-rw-r--   0 runner    (1001) docker     (127)    13487 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11Common.cmake
+-rw-rw-r--   0 runner    (1001) docker     (127)     6930 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11Config.cmake.in
+-rw-rw-r--   0 runner    (1001) docker     (127)     8957 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11NewTools.cmake
+-rw-rw-r--   0 runner    (1001) docker     (127)     8361 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11Tools.cmake
+-rw-rw-r--   0 runner    (1001) docker     (127)       94 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/tools/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)     2104 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/tools/setup_global.py.in
+-rw-rw-r--   0 runner    (1001) docker     (127)     1234 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pybind11/tools/setup_main.py.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pyparse/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4660 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/pyparse/pyparse.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2716 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1558 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/LICENSE
+-rw-rw-r--   0 runner    (1001) docker     (127)    12166 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/bitstate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    40923 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/compile.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    77669 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/dfa.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3379 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/filtered_re2.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2794 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/include/bitmap256.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4074 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/include/filtered_re2.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3685 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/include/logging.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1027 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/include/mix.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4596 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/include/mutex.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1051 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/include/pod_array.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4107 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/include/prefilter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5397 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/include/prefilter_tree.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    20055 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/include/prog.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    41735 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/include/re2.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    25053 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/include/regexp.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2528 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/include/set.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    12285 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/include/sparse_array.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7425 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/include/sparse_set.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6625 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/include/stringpiece.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      644 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/include/strutil.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2606 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/include/unicode_casefold.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1595 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/include/unicode_groups.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1575 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/include/utf.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1028 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/include/util.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7825 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/include/walker-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6308 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/mimics_pcre.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    22890 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/nfa.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    22239 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/onepass.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    81544 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/parse.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3448 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/perl_groups.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    18698 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/prefilter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    13255 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/prefilter_tree.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    40537 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/prog.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    42418 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/re2.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    28640 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/regexp.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5872 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/rune.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4636 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/set.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    20853 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/simplify.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2118 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/stringpiece.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5691 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/strutil.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9029 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/tostring.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    13413 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/unicode_casefold.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)   122482 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/re2/unicode_groups.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/serd/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1247 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/serd/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/serd/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)    33294 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/serd/include/serd.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/serd/src/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/serd/src/LICENSES/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1424 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/serd/src/LICENSES/BSD-3-Clause.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      660 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/serd/src/LICENSES/OBSD.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      555 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/serd/src/attributes.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3172 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/serd/src/base64.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     1024 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/serd/src/base64.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1966 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/serd/src/byte_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2643 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/serd/src/byte_source.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     3444 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/serd/src/byte_source.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6676 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/serd/src/env.c
+-rw-rw-r--   0 runner    (1001) docker     (127)    46487 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/serd/src/n3.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     9699 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/serd/src/node.c
+-rw-rw-r--   0 runner    (1001) docker     (127)      871 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/serd/src/node.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    12064 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/serd/src/reader.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     4376 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/serd/src/reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3187 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/serd/src/serd_config.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      730 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/serd/src/serd_internal.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    10745 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/serd/src/serdi.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     2552 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/serd/src/stack.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3507 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/serd/src/string.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     3394 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/serd/src/string_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1233 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/serd/src/system.c
+-rw-rw-r--   0 runner    (1001) docker     (127)      650 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/serd/src/system.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      546 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/serd/src/try.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    11749 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/serd/src/uri.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     2843 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/serd/src/uri_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    36427 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/serd/src/writer.c
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1348 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/LICENSE
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4021 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/async.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2817 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/async_logger-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2560 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/async_logger.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/argv.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      986 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/env.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3170 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/helpers-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      718 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/helpers.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2050 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/common-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    13194 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/common.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2004 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/backtracer-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1165 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/backtracer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3349 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/circular_q.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      603 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/console_globals.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4707 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/file_helper-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1758 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/file_helper.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4471 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/fmt_helper.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1396 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/log_msg-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1204 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/log_msg.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1668 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/log_msg_buffer-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      935 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/log_msg_buffer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5285 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/mpmc_blocking_q.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      930 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/null_mutex.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    17897 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/os-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3922 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/os.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      620 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/periodic_worker-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1756 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/periodic_worker.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8695 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/registry-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4013 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/registry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      751 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/synchronous_factory.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4252 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/tcp_client-windows.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3885 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/tcp_client.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4275 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/thread_pool-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3519 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/thread_pool.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3134 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/udp_client-windows.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2237 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/udp_client.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      188 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/windows_include.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/
+-rw-rw-r--   0 runner    (1001) docker     (127)     7380 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bin_to_hex.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/
+-rw-rw-r--   0 runner    (1001) docker     (127)     7420 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/args.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    68076 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/chrono.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    24896 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/color.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    21245 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/compile.h
+-rw-rw-r--   0 runner    (1001) docker     (127)   111215 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/core.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1408 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/fmt.license.rst
+-rw-rw-r--   0 runner    (1001) docker     (127)    74272 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/format-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)   154181 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/format.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      100 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/locale.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    14123 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/os.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7586 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/ostream.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    20023 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/printf.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    23218 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/ranges.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4880 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/std.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9001 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/xchar.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      551 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/chrono.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      559 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/compile.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1042 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/fmt.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      554 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/ostr.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      551 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/ranges.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      641 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/std.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      548 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/xchar.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      463 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/formatter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      305 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fwd.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6725 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/logger-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    13412 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/logger.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    44468 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/pattern_formatter-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3758 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/pattern_formatter.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4777 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/android_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4875 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/ansicolor_sink-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3959 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/ansicolor_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1808 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/base_sink-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1568 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/base_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1216 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/basic_file_sink-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2295 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/basic_file_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1705 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/callback_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9452 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/daily_file_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2373 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/dist_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3243 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/dup_filter_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7121 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/hourly_file_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4445 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/kafka_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4003 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/mongo_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2049 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/msvc_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1234 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/null_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1222 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/ostream_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    12408 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/qt_sinks.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2081 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/ringbuffer_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4917 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/rotating_file_sink-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3229 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/rotating_file_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      725 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/sink-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      893 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1435 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/stdout_color_sinks-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1792 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/stdout_color_sinks.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4347 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/stdout_sinks-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2429 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/stdout_sinks.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4239 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/syslog_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4872 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/systemd_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2127 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/tcp_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1858 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/udp_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8888 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/win_eventlog_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6651 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/wincolor_sink-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2716 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/wincolor_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3118 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/spdlog-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    11771 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/spdlog.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1711 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/stopwatch.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6360 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/tweakme.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      417 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/spdlog/spdlog/version.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/taywee_args/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1105 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/taywee_args/LICENSE
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/taywee_args/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)   152995 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/taywee_args/include/args.hxx
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/utf8proc/
+-rw-rw-r--   0 runner    (1001) docker     (127)      142 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/utf8proc/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     5125 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/utf8proc/LICENSE.md
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/utf8proc/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)    32757 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/utf8proc/include/utf8proc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)  1944550 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/utf8proc/include/utf8proc_data.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      888 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/utf8proc/include/utf8proc_wrapper.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    37876 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/utf8proc/utf8proc.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4483 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/utf8proc/utf8proc_wrapper.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1194 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1529 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/LICENSE
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/common/
+-rw-rw-r--   0 runner    (1001) docker     (127)     8580 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/common/entropy_common.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2982 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/common/error_private.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    10089 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/common/fse_decompress.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    28008 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/common/xxhash.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2721 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/common/zstd_common.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/compress/
+-rw-rw-r--   0 runner    (1001) docker     (127)    26469 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/compress/fse_compress.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7555 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/compress/hist.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    32726 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/compress/huf_compress.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)   183732 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_compress.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6293 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_compress_literals.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    19309 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_compress_sequences.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    43614 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_compress_superblock.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    25428 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_double_fast.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    22459 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_fast.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    52956 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_lazy.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    25024 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_ldm.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    55766 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_opt.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/decompress/
+-rw-rw-r--   0 runner    (1001) docker     (127)    51287 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/decompress/huf_decompress.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9136 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/decompress/zstd_ddict.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    83312 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/decompress/zstd_decompress.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    61618 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/decompress/zstd_decompress_block.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/include/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/include/zstd/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/
+-rw-rw-r--   0 runner    (1001) docker     (127)    17857 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/bitstream.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5734 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/compiler.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3893 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/debug.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2396 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/error_private.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    14574 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/fse.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    18012 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/fse_static.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4717 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/huf.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    14332 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/huf_static.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    12217 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/mem.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9897 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/xxhash.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1779 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/xxhash_static.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3730 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/zstd_errors.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    13604 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/zstd_internal.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3464 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/hist.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    46030 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_compress_internal.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1262 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_compress_literals.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2210 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_compress_sequences.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1194 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_compress_superblock.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    18777 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_cwksp.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1250 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_double_fast.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1171 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_fast.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2701 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_lazy.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4010 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_ldm.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1972 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_opt.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/include/zstd/decompress/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1329 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/include/zstd/decompress/zstd_ddict.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2081 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/include/zstd/decompress/zstd_decompress_block.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6147 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/include/zstd/decompress/zstd_decompress_internal.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    61165 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/include/zstd.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    60974 2024-04-16 08:04:19.000000 sdist/kuzu-source/third_party/zstd/include/zstd_static.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/
+-rw-rw-r--   0 runner    (1001) docker     (127)      297 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/benchmark/
+-rw-rw-r--   0 runner    (1001) docker     (127)      251 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/benchmark/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     3132 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/benchmark/benchmark.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3400 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/benchmark/benchmark_runner.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/benchmark/example/
+-rw-rw-r--   0 runner    (1001) docker     (127)       73 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/benchmark/example/example.benchmark
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/benchmark/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)      994 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/benchmark/include/benchmark.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      561 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/benchmark/include/benchmark_config.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      836 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/benchmark/include/benchmark_runner.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2195 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/benchmark/main.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1846 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      332 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/README.md
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/jni/
+-rw-rw-r--   0 runner    (1001) docker     (127)    51926 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/jni/kuzu_java.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/main/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/main/java/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4861 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuConnection.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     3587 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuDataType.java
+-rw-rw-r--   0 runner    (1001) docker     (127)      716 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuDataTypeID.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     2944 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuDatabase.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     1734 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuFlatTuple.java
+-rw-rw-r--   0 runner    (1001) docker     (127)      495 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuInternalID.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     9740 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuNative.java
+-rw-rw-r--   0 runner    (1001) docker     (127)      334 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuObjectRefDestroyedException.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     2490 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuPreparedStatement.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     5236 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuQueryResult.java
+-rw-rw-r--   0 runner    (1001) docker     (127)      853 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuQuerySummary.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     4622 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValue.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     1077 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueListUtil.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     2984 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueNodeUtil.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     1034 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueRdfVariantUtil.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     1024 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueRecursiveRelUtil.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     3397 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueRelUtil.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueStructUtil.java
+-rw-rw-r--   0 runner    (1001) docker     (127)      520 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuVersion.java
+-rw-rw-r--   0 runner    (1001) docker     (127)      178 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/package-info.java
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/test/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/test/java/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/
+-rw-rw-r--   0 runner    (1001) docker     (127)    11911 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/ConnectionTest.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     5025 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/DataTypeTest.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     1946 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/DatabaseTest.java
+-rw-rw-r--   0 runner    (1001) docker     (127)      525 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/ExtensionTest.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     1865 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/FlatTupleTest.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     2476 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/PreparedStatementTest.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     4789 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/QueryResultTest.java
+-rw-rw-r--   0 runner    (1001) docker     (127)      940 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/TestBase.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     2504 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/TestHelper.java
+-rw-rw-r--   0 runner    (1001) docker     (127)    45229 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/ValueTest.java
+-rw-rw-r--   0 runner    (1001) docker     (127)      471 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/VersionTest.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     2271 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/test.java
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/third_party/
+-rw-rw-r--   0 runner    (1001) docker     (127)  2614186 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/java_api/third_party/junit-platform-console-standalone-1.9.3.jar
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1777 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     3043 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/README.md
+-rw-rw-r--   0 runner    (1001) docker     (127)      397 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/build.js
+-rw-rw-r--   0 runner    (1001) docker     (127)      615 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/clean.js
+-rw-rw-r--   0 runner    (1001) docker     (127)     4452 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/install.js
+-rw-rw-r--   0 runner    (1001) docker     (127)     5577 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/package.js
+-rw-rw-r--   0 runner    (1001) docker     (127)      672 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/package.json
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4353 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_connection.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1577 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1635 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_prepared_statement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4369 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_query_result.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      637 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_util.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/main.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4010 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_connection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2461 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2110 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_prepared_statement.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3361 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_query_result.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    19925 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_util.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/src_js/
+-rw-rw-r--   0 runner    (1001) docker     (127)     7782 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/src_js/connection.js
+-rw-rw-r--   0 runner    (1001) docker     (127)     4045 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/src_js/database.js
+-rw-rw-r--   0 runner    (1001) docker     (127)      499 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/src_js/index.js
+-rw-rw-r--   0 runner    (1001) docker     (127)      686 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/src_js/kuzu_native.js
+-rw-rw-r--   0 runner    (1001) docker     (127)      238 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/src_js/logging_level.js
+-rw-rw-r--   0 runner    (1001) docker     (127)     1210 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/src_js/prepared_statement.js
+-rw-rw-r--   0 runner    (1001) docker     (127)     4244 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/src_js/query_result.js
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/test/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2099 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/test/common.js
+-rw-rw-r--   0 runner    (1001) docker     (127)      629 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/test/test.js
+-rw-rw-r--   0 runner    (1001) docker     (127)     3089 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/test/test_concurrency.js
+-rw-rw-r--   0 runner    (1001) docker     (127)     7822 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/test/test_connection.js
+-rw-rw-r--   0 runner    (1001) docker     (127)    19348 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/test/test_data_type.js
+-rw-rw-r--   0 runner    (1001) docker     (127)     7243 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/test/test_database.js
+-rw-rw-r--   0 runner    (1001) docker     (127)      266 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/test/test_extension.js
+-rw-rw-r--   0 runner    (1001) docker     (127)    22522 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/test/test_parameter.js
+-rw-rw-r--   0 runner    (1001) docker     (127)     5730 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/test/test_query_result.js
+-rw-rw-r--   0 runner    (1001) docker     (127)      384 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/nodejs_api/test/test_version.js
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1295 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1136 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/Makefile
+-rw-rw-r--   0 runner    (1001) docker     (127)       23 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/README.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     2381 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      203 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/requirements_dev.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/cached_import/
+-rw-rw-r--   0 runner    (1001) docker     (127)      376 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/cached_import/py_cached_import.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      618 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/cached_import/py_cached_item.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)      335 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/arrow_array.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/cached_import/
+-rw-rw-r--   0 runner    (1001) docker     (127)      682 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/cached_import/py_cached_import.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      521 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/cached_import/py_cached_item.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3624 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/cached_import/py_cached_modules.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/numpy/
+-rw-rw-r--   0 runner    (1001) docker     (127)      430 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/numpy/numpy_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1379 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/numpy/numpy_type.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/
+-rw-rw-r--   0 runner    (1001) docker     (127)      718 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/pandas_analyzer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1290 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/pandas_bind.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      931 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/pandas_column.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1942 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/pandas_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1266 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_connection.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      714 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_conversion.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1050 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      676 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_object_container.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      381 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_prepared_statement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1369 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_query_result.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      709 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_query_result_converter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1031 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_str_utils.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pyarrow/
+-rw-rw-r--   0 runner    (1001) docker     (127)      383 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pyarrow/pyarrow_bind.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2211 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pyarrow/pyarrow_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      202 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pybind_include.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      549 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/kuzu_binding.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/numpy/
+-rw-rw-r--   0 runner    (1001) docker     (127)     9493 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/numpy/numpy_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5514 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/numpy/numpy_type.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/pandas/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3949 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/pandas/pandas_analyzer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3943 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/pandas/pandas_bind.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7556 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/pandas/pandas_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    18204 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_connection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4462 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_conversion.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3620 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      564 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_prepared_statement.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    15476 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_query_result.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7635 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_query_result_converter.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/pyarrow/
+-rw-rw-r--   0 runner    (1001) docker     (127)      866 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/pyarrow/pyarrow_bind.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4295 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_cpp/pyarrow/pyarrow_scan.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_py/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2111 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_py/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6092 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_py/connection.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     8124 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_py/database.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1167 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_py/prepared_statement.py
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_py/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)    14470 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_py/query_result.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     7586 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_py/torch_geometric_feature_store.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4893 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_py/torch_geometric_graph_store.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    13467 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_py/torch_geometric_result_converter.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      839 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/src_py/types.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/test/
+-rw-rw-r--   0 runner    (1001) docker     (127)     5545 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/test/conftest.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      303 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/test/example.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    14350 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/test/ground_truth.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    22117 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/test/test_arrow.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    12786 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/test/test_datatype.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    19806 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/test/test_df.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    17869 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/test/test_df_pyarrow.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2292 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/test/test_exception.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      247 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/test/test_extension.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1947 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/test/test_get_header.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      222 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/test/test_helper.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    10889 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/test/test_networkx.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     8377 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/test/test_parameter.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4511 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/test/test_prepared_statement.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1421 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/test/test_query_result.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1258 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/test/test_query_result_close.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    12731 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/test/test_scan_pandas.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      345 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/test/test_timeout.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    30361 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/test/test_torch_geometric.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4105 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/test/test_torch_geometric_remote_backend.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      155 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/test/test_version.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      215 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/python_api/test/type_aliases.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/rust_api/
+-rw-rw-r--   0 runner    (1001) docker     (127)        7 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/rust_api/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (127)    25753 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/rust_api/Cargo.lock
+-rw-rw-r--   0 runner    (1001) docker     (127)     1099 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/rust_api/Cargo.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)     5609 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/rust_api/build.rs
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/rust_api/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)      345 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/rust_api/include/kuzu_arrow.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9633 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/rust_api/include/kuzu_rs.h
+lrwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:21.894007 sdist/kuzu-source/tools/rust_api/kuzu-src -> ../..
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/rust_api/src/
+-rw-rw-r--   0 runner    (1001) docker     (127)      380 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/rust_api/src/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    13653 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/rust_api/src/connection.rs
+-rw-rw-r--   0 runner    (1001) docker     (127)     6642 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/rust_api/src/database.rs
+-rw-rw-r--   0 runner    (1001) docker     (127)     1763 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/rust_api/src/error.rs
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/rust_api/src/ffi/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1123 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/rust_api/src/ffi/arrow.rs
+-rw-rw-r--   0 runner    (1001) docker     (127)    12920 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/rust_api/src/ffi.rs
+-rw-rw-r--   0 runner    (1001) docker     (127)      471 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/rust_api/src/kuzu_arrow.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11961 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/rust_api/src/kuzu_rs.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2523 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/rust_api/src/lib.rs
+-rw-rw-r--   0 runner    (1001) docker     (127)    12498 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/rust_api/src/logical_type.rs
+-rw-rw-r--   0 runner    (1001) docker     (127)     9355 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/rust_api/src/query_result.rs
+-rw-rw-r--   0 runner    (1001) docker     (127)     2629 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/rust_api/src/rdf_variant.rs
+-rw-rw-r--   0 runner    (1001) docker     (127)    67772 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/rust_api/src/value.rs
+-rw-rw-r--   0 runner    (1001) docker     (127)     1730 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/rust_api/update_version.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/shell/
+-rw-rw-r--   0 runner    (1001) docker     (127)      321 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/shell/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    27718 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/shell/embedded_shell.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/shell/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)      912 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/shell/include/embedded_shell.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3116 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/shell/include/linenoise.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    79992 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/shell/linenoise.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3257 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/shell/shell_runner.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/shell/test/
+-rw-rw-r--   0 runner    (1001) docker     (127)     5371 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/shell/test/conftest.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/shell/test/files/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3075 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/shell/test/files/vPerson.csv
+-rw-rw-r--   0 runner    (1001) docker     (127)     1399 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/shell/test/test_helper.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4780 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/shell/test/test_shell_basics.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4811 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/shell/test/test_shell_commands.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    11969 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/shell/test/test_shell_control_edit.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    12995 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/shell/test/test_shell_control_search.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4297 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/shell/test/test_shell_esc_edit.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4571 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/shell/test/test_shell_esc_search.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4904 2024-04-16 08:04:19.000000 sdist/kuzu-source/tools/shell/test/test_shell_flags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:04:22.322006 sdist/kuzu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-04-16 08:04:22.322006 sdist/kuzu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-16 08:04:22.322006 sdist/kuzu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 08:04:22.322006 sdist/kuzu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-16 08:04:22.322006 sdist/kuzu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 08:04:22.322006 sdist/kuzu.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-16 08:04:22.110007 sdist/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-16 08:04:18.874008 sdist/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-04-16 08:04:18.874008 sdist/setup.py
```

### sdist/kuzu-source/CMakeLists.txt

```diff
@@ -1,10 +1,10 @@
 cmake_minimum_required(VERSION 3.15)
 
-project(Kuzu VERSION 0.3.3.35 LANGUAGES CXX C)
+project(Kuzu VERSION 0.3.3.36 LANGUAGES CXX C)
 
 find_package(Threads REQUIRED)
 
 set(CMAKE_CXX_STANDARD 20)
 set(CMAKE_CXX_STANDARD_REQUIRED TRUE)
 set(CMAKE_CXX_VISIBILITY_PRESET hidden)
 set(CMAKE_C_VISIBILITY_PRESET hidden)
@@ -190,20 +190,14 @@
 endfunction()
 
 # Windows doesn't support dynamic lookup, so we have to link extensions against kuzu.
 if (MSVC AND (NOT BUILD_EXTENSIONS EQUAL ""))
     set(BUILD_KUZU TRUE)
 endif ()
 
-if(${BUILD_KUZU})
-add_definitions(-DKUZU_ROOT_DIRECTORY="${PROJECT_SOURCE_DIR}")
-add_definitions(-DKUZU_CMAKE_VERSION="${CMAKE_PROJECT_VERSION}")
-add_definitions(-DKUZU_EXTENSION_VERSION="0.2.5")
-
-include_directories(src/include)
 include_directories(third_party/antlr4_cypher/include)
 include_directories(third_party/antlr4_runtime/src)
 include_directories(third_party/fast_float/include)
 include_directories(third_party/mbedtls/include)
 include_directories(third_party/miniparquet/src)
 include_directories(third_party/miniz)
 include_directories(third_party/nlohmann_json)
@@ -214,14 +208,22 @@
 include_directories(third_party/spdlog)
 include_directories(third_party/utf8proc/include)
 include_directories(third_party/zstd/include)
 include_directories(third_party/httplib)
 include_directories(third_party/pcg)
 
 add_subdirectory(third_party)
+
+if(${BUILD_KUZU})
+add_definitions(-DKUZU_ROOT_DIRECTORY="${PROJECT_SOURCE_DIR}")
+add_definitions(-DKUZU_CMAKE_VERSION="${CMAKE_PROJECT_VERSION}")
+add_definitions(-DKUZU_EXTENSION_VERSION="0.2.6")
+
+include_directories(src/include)
+
 add_subdirectory(src)
 if (${BUILD_TESTS})
     add_definitions(-DTEST_FILES_DIR="test/test_files")
     add_subdirectory(test)
 elseif (${BUILD_BENCHMARK})
     add_definitions(-DTEST_FILES_DIR="test/test_files")
     add_subdirectory(test/test_helper)
```

### sdist/kuzu-source/src/binder/bind/read/bind_in_query_call.cpp

```diff
@@ -1,45 +1,52 @@
 #include "binder/binder.h"
 #include "binder/expression/expression_util.h"
 #include "binder/expression/literal_expression.h"
 #include "binder/query/reading_clause/bound_in_query_call.h"
 #include "catalog/catalog.h"
+#include "common/exception/binder.h"
 #include "function/built_in_function_utils.h"
 #include "parser/expression/parsed_function_expression.h"
 #include "parser/query/reading_clause/in_query_call_clause.h"
 
 using namespace kuzu::common;
 using namespace kuzu::parser;
 using namespace kuzu::function;
+using namespace kuzu::catalog;
 
 namespace kuzu {
 namespace binder {
 
 std::unique_ptr<BoundReadingClause> Binder::bindInQueryCall(const ReadingClause& readingClause) {
     auto& call = readingClause.constCast<InQueryCallClause>();
     auto expr = call.getFunctionExpression();
     auto functionExpr = expr->constPtrCast<ParsedFunctionExpression>();
+    auto functionName = functionExpr->getFunctionName();
     expression_vector params;
     for (auto i = 0u; i < functionExpr->getNumChildren(); i++) {
         auto child = functionExpr->getChild(i);
         params.push_back(expressionBinder.bindExpression(*child));
     }
     TableFunction tableFunction;
     std::vector<Value> inputValues;
     std::vector<LogicalType> inputTypes;
     for (auto& param : params) {
         ExpressionUtil::validateExpressionType(*param, ExpressionType::LITERAL);
         auto literalExpr = param->constPtrCast<LiteralExpression>();
         inputTypes.push_back(literalExpr->getDataType());
         inputValues.push_back(*literalExpr->getValue());
     }
-    auto functions = clientContext->getCatalog()->getFunctions(clientContext->getTx());
+    auto catalogSet = clientContext->getCatalog()->getFunctions(clientContext->getTx());
+    auto functionEntry = BuiltInFunctionsUtils::getFunctionCatalogEntry(functionName, catalogSet);
+    if (functionEntry->getType() != CatalogEntryType::TABLE_FUNCTION_ENTRY) {
+        throw BinderException(stringFormat("{} is not a table function.", functionName));
+    }
     auto func = BuiltInFunctionsUtils::matchFunction(functionExpr->getFunctionName(), inputTypes,
-        functions);
-    tableFunction = *ku_dynamic_cast<function::Function*, function::TableFunction*>(func);
+        functionEntry);
+    tableFunction = *func->constPtrCast<TableFunction>();
     auto bindInput = function::TableFuncBindInput();
     bindInput.inputs = std::move(inputValues);
     auto bindData = tableFunction.bindFunc(clientContext, &bindInput);
     expression_vector columns;
     for (auto i = 0u; i < bindData->columnTypes.size(); i++) {
         columns.push_back(createVariable(bindData->columnNames[i], bindData->columnTypes[i]));
     }
```

### sdist/kuzu-source/src/binder/bind_expression/bind_function_expression.cpp

```diff
@@ -23,33 +23,34 @@
 using namespace kuzu::function;
 using namespace kuzu::catalog;
 
 namespace kuzu {
 namespace binder {
 
 std::shared_ptr<Expression> ExpressionBinder::bindFunctionExpression(const ParsedExpression& expr) {
-    auto& funcExpr =
-        ku_dynamic_cast<const ParsedExpression&, const ParsedFunctionExpression&>(expr);
-    auto functionName = funcExpr.getNormalizedFunctionName();
+    auto funcExpr = expr.constPtrCast<ParsedFunctionExpression>();
+    auto functionName = funcExpr->getNormalizedFunctionName();
     auto result = rewriteFunctionExpression(expr, functionName);
     if (result != nullptr) {
         return result;
     }
     auto entry = context->getCatalog()->getFunctionEntry(context->getTx(), functionName);
     switch (entry->getType()) {
     case CatalogEntryType::SCALAR_FUNCTION_ENTRY:
         return bindScalarFunctionExpression(expr, functionName);
     case CatalogEntryType::REWRITE_FUNCTION_ENTRY:
         return bindRewriteFunctionExpression(expr);
     case CatalogEntryType::AGGREGATE_FUNCTION_ENTRY:
-        return bindAggregateFunctionExpression(expr, functionName, funcExpr.getIsDistinct());
+        return bindAggregateFunctionExpression(expr, functionName, funcExpr->getIsDistinct());
     case CatalogEntryType::SCALAR_MACRO_ENTRY:
         return bindMacroExpression(expr, functionName);
     default:
-        KU_UNREACHABLE;
+        throw BinderException(
+            stringFormat("{} is a {}. Scalar function, aggregate function or macro was expected. ",
+                functionName, CatalogEntryTypeUtils::toString(entry->getType())));
     }
 }
 
 std::shared_ptr<Expression> ExpressionBinder::bindScalarFunctionExpression(
     const ParsedExpression& parsedExpression, const std::string& functionName) {
     expression_vector children;
     for (auto i = 0u; i < parsedExpression.getNumChildren(); ++i) {
```

### sdist/kuzu-source/src/binder/binder.cpp

```diff
@@ -114,15 +114,15 @@
     auto expression = expressionBinder.createVariableExpression(dataType, name);
     expression->setAlias(name);
     scope.addExpression(name, expression);
     return expression;
 }
 
 std::unique_ptr<LogicalType> Binder::bindDataType(const std::string& dataType) {
-    auto boundType = LogicalTypeUtils::dataTypeFromString(dataType);
+    auto boundType = LogicalType::fromString(dataType);
     if (boundType.getLogicalTypeID() == LogicalTypeID::ARRAY) {
         auto numElementsInArray = ArrayType::getNumElements(&boundType);
         if (numElementsInArray == 0) {
             // Note: the parser already guarantees that the number of elements is a non-negative
             // number. However, we still need to check whether the number of elements is 0.
             throw BinderException(
                 "The number of elements in an array must be greater than 0. Given: " +
```

### sdist/kuzu-source/src/catalog/catalog.cpp

```diff
@@ -216,23 +216,25 @@
     } break;
     default: {
         // DO NOTHING.
     }
     }
 }
 
-void Catalog::addFunction(std::string name, function::function_set functionSet) {
+void Catalog::addFunction(CatalogEntryType entryType, std::string name,
+    function::function_set functionSet) {
     initCatalogContentForWriteTrxIfNecessary();
     KU_ASSERT(readWriteVersion != nullptr);
     setToUpdated();
-    readWriteVersion->addFunction(std::move(name), std::move(functionSet));
+    readWriteVersion->addFunction(entryType, std::move(name), std::move(functionSet));
 }
 
-void Catalog::addBuiltInFunction(std::string name, function::function_set functionSet) {
-    readOnlyVersion->addFunction(std::move(name), std::move(functionSet));
+void Catalog::addBuiltInFunction(CatalogEntryType entryType, std::string name,
+    function::function_set functionSet) {
+    readOnlyVersion->addFunction(entryType, std::move(name), std::move(functionSet));
 }
 
 CatalogSet* Catalog::getFunctions(Transaction* tx) const {
     return getVersion(tx)->functions.get();
 }
 
 CatalogEntry* Catalog::getFunctionEntry(Transaction* tx, const std::string& name) {
```

### sdist/kuzu-source/src/catalog/catalog_content.cpp

```diff
@@ -261,20 +261,21 @@
     deserializer.deserializeValue(savedStorageVersion);
     validateStorageVersion(savedStorageVersion);
     tables = CatalogSet::deserialize(deserializer);
     deserializer.deserializeValue(nextTableID);
     functions = CatalogSet::deserialize(deserializer);
 }
 
-void CatalogContent::addFunction(std::string name, function::function_set definitions) {
+void CatalogContent::addFunction(CatalogEntryType entryType, std::string name,
+    function::function_set definitions) {
     if (functions->containsEntry(name)) {
         throw CatalogException{stringFormat("function {} already exists.", name)};
     }
-    functions->createEntry(std::make_unique<FunctionCatalogEntry>(
-        CatalogEntryType::SCALAR_FUNCTION_ENTRY, std::move(name), std::move(definitions)));
+    functions->createEntry(
+        std::make_unique<FunctionCatalogEntry>(entryType, std::move(name), std::move(definitions)));
 }
 
 function::ScalarMacroFunction* CatalogContent::getScalarMacroFunction(
     const std::string& name) const {
     return ku_dynamic_cast<CatalogEntry*, ScalarMacroCatalogEntry*>(functions->getEntry(name))
         ->getMacroFunction();
 }
```

### sdist/kuzu-source/src/catalog/catalog_entry/CMakeLists.txt

```diff
@@ -1,10 +1,11 @@
 add_library(kuzu_catalog_entry
         OBJECT
         catalog_entry.cpp
+        catalog_entry_type.cpp
         function_catalog_entry.cpp
         table_catalog_entry.cpp
         node_table_catalog_entry.cpp
         rel_table_catalog_entry.cpp
         rel_group_catalog_entry.cpp
         rdf_graph_catalog_entry.cpp
         scalar_macro_catalog_entry.cpp)
```

### sdist/kuzu-source/src/common/file_system/file_info.cpp

```diff
@@ -7,33 +7,37 @@
 #else
 #include <unistd.h>
 #endif
 
 namespace kuzu {
 namespace common {
 
-uint64_t FileInfo::getFileSize() {
-    return fileSystem->getFileSize(this);
+uint64_t FileInfo::getFileSize() const {
+    return fileSystem->getFileSize(*this);
 }
 
 void FileInfo::readFromFile(void* buffer, uint64_t numBytes, uint64_t position) {
-    fileSystem->readFromFile(this, buffer, numBytes, position);
+    fileSystem->readFromFile(*this, buffer, numBytes, position);
 }
 
 int64_t FileInfo::readFile(void* buf, size_t nbyte) {
-    return fileSystem->readFile(this, buf, nbyte);
+    return fileSystem->readFile(*this, buf, nbyte);
 }
 
 void FileInfo::writeFile(const uint8_t* buffer, uint64_t numBytes, uint64_t offset) {
-    fileSystem->writeFile(this, buffer, numBytes, offset);
+    fileSystem->writeFile(*this, buffer, numBytes, offset);
+}
+
+void FileInfo::syncFile() const {
+    fileSystem->syncFile(*this);
 }
 
 int64_t FileInfo::seek(uint64_t offset, int whence) {
-    return fileSystem->seek(this, offset, whence);
+    return fileSystem->seek(*this, offset, whence);
 }
 
 void FileInfo::truncate(uint64_t size) {
-    fileSystem->truncate(this, size);
+    fileSystem->truncate(*this, size);
 }
 
 } // namespace common
 } // namespace kuzu
```

### sdist/kuzu-source/src/common/file_system/file_system.cpp

```diff
@@ -32,18 +32,18 @@
     return (std::filesystem::path{base} / part).string();
 }
 
 std::string FileSystem::getFileExtension(const std::filesystem::path& path) {
     return path.extension().string();
 }
 
-void FileSystem::writeFile(FileInfo* /*fileInfo*/, const uint8_t* /*buffer*/, uint64_t /*numBytes*/,
+void FileSystem::writeFile(FileInfo& /*fileInfo*/, const uint8_t* /*buffer*/, uint64_t /*numBytes*/,
     uint64_t /*offset*/) const {
     KU_UNREACHABLE;
 }
 
-void FileSystem::truncate(FileInfo* /*fileInfo*/, uint64_t /*size*/) const {
+void FileSystem::truncate(FileInfo& /*fileInfo*/, uint64_t /*size*/) const {
     KU_UNREACHABLE;
 }
 
 } // namespace common
 } // namespace kuzu
```

### sdist/kuzu-source/src/common/file_system/local_file_system.cpp

```diff
@@ -1,11 +1,16 @@
 #include "common/file_system/local_file_system.h"
 
+#include "common/assert.h"
 #include "common/cast.h"
+#include "common/exception/io.h"
+#include "common/string_format.h"
 #include "common/string_utils.h"
+#include "common/system_message.h"
+#include "glob/glob.hpp"
 #include "main/client_context.h"
 #include "main/settings.h"
 
 #if defined(_WIN32)
 #include <fileapi.h>
 #include <io.h>
 #include <windows.h>
@@ -14,20 +19,14 @@
 #include <unistd.h>
 #endif
 
 #include <fcntl.h>
 
 #include <cstring>
 
-#include "common/assert.h"
-#include "common/exception/exception.h"
-#include "common/string_format.h"
-#include "common/system_message.h"
-#include "glob/glob.hpp"
-
 namespace kuzu {
 namespace common {
 
 LocalFileInfo::~LocalFileInfo() {
 #ifdef _WIN32
     if (handle != nullptr) {
         CloseHandle((HANDLE)handle);
@@ -53,44 +52,44 @@
     if (!(flags & O_WRONLY)) {
         dwDesiredAccess |= GENERIC_READ;
     }
 
     HANDLE handle = CreateFileA(fullPath.c_str(), dwDesiredAccess, dwShareMode, nullptr,
         dwCreationDisposition, FILE_ATTRIBUTE_NORMAL, nullptr);
     if (handle == INVALID_HANDLE_VALUE) {
-        throw Exception(stringFormat("Cannot open file. path: {} - Error {}: {}", fullPath,
+        throw IOException(stringFormat("Cannot open file. path: {} - Error {}: {}", fullPath,
             GetLastError(), std::system_category().message(GetLastError())));
     }
     if (lock_type != FileLockType::NO_LOCK) {
         DWORD dwFlags = lock_type == FileLockType::READ_LOCK ?
                             LOCKFILE_FAIL_IMMEDIATELY :
                             LOCKFILE_FAIL_IMMEDIATELY | LOCKFILE_EXCLUSIVE_LOCK;
         OVERLAPPED overlapped = {0};
         overlapped.Offset = 0;
         BOOL rc = LockFileEx(handle, dwFlags, 0, 0, 0, &overlapped);
         if (!rc) {
-            throw Exception("Could not set lock on file : " + fullPath);
+            throw IOException("Could not set lock on file : " + fullPath);
         }
     }
     return std::make_unique<LocalFileInfo>(fullPath, handle, this);
 #else
     int fd = open(fullPath.c_str(), flags, 0644);
     if (fd == -1) {
-        throw Exception(stringFormat("Cannot open file {}: {}", fullPath, posixErrMessage()));
+        throw IOException(stringFormat("Cannot open file {}: {}", fullPath, posixErrMessage()));
     }
     if (lock_type != FileLockType::NO_LOCK) {
         struct flock fl;
         memset(&fl, 0, sizeof fl);
         fl.l_type = lock_type == FileLockType::READ_LOCK ? F_RDLCK : F_WRLCK;
         fl.l_whence = SEEK_SET;
         fl.l_start = 0;
         fl.l_len = 0;
         int rc = fcntl(fd, F_SETLK, &fl);
         if (rc == -1) {
-            throw Exception("Could not set lock on file : " + fullPath);
+            throw IOException("Could not set lock on file : " + fullPath);
         }
     }
     return std::make_unique<LocalFileInfo>(fullPath, fd, this);
 #endif
 }
 
 std::vector<std::string> LocalFileSystem::glob(main::ClientContext* context,
@@ -132,58 +131,58 @@
 void LocalFileSystem::overwriteFile(const std::string& from, const std::string& to) const {
     if (!fileOrPathExists(from) || !fileOrPathExists(to))
         return;
     std::error_code errorCode;
     if (!std::filesystem::copy_file(from, to, std::filesystem::copy_options::overwrite_existing,
             errorCode)) {
         // LCOV_EXCL_START
-        throw Exception(stringFormat("Error copying file {} to {}.  ErrorMessage: {}", from, to,
+        throw IOException(stringFormat("Error copying file {} to {}.  ErrorMessage: {}", from, to,
             errorCode.message()));
         // LCOV_EXCL_STOP
     }
 }
 
 void LocalFileSystem::copyFile(const std::string& from, const std::string& to) const {
     if (!fileOrPathExists(from))
         return;
     std::error_code errorCode;
     if (!std::filesystem::copy_file(from, to, std::filesystem::copy_options::none, errorCode)) {
         // LCOV_EXCL_START
-        throw Exception(stringFormat("Error copying file {} to {}.  ErrorMessage: {}", from, to,
+        throw IOException(stringFormat("Error copying file {} to {}.  ErrorMessage: {}", from, to,
             errorCode.message()));
         // LCOV_EXCL_STOP
     }
 }
 
 void LocalFileSystem::createDir(const std::string& dir) const {
     try {
         if (std::filesystem::exists(dir)) {
             // LCOV_EXCL_START
-            throw Exception(stringFormat("Directory {} already exists.", dir));
+            throw IOException(stringFormat("Directory {} already exists.", dir));
             // LCOV_EXCL_STOP
         }
         if (!std::filesystem::create_directories(dir)) {
             // LCOV_EXCL_START
-            throw Exception(stringFormat(
+            throw IOException(stringFormat(
                 "Directory {} cannot be created. Check if it exists and remove it.", dir));
             // LCOV_EXCL_STOP
         }
     } catch (std::exception& e) {
         // LCOV_EXCL_START
-        throw Exception(stringFormat("Failed to create directory {} due to: {}", dir, e.what()));
+        throw IOException(stringFormat("Failed to create directory {} due to: {}", dir, e.what()));
         // LCOV_EXCL_STOP
     }
 }
 
 void LocalFileSystem::removeFileIfExists(const std::string& path) const {
     if (!fileOrPathExists(path))
         return;
     if (remove(path.c_str()) != 0) {
         // LCOV_EXCL_START
-        throw Exception(stringFormat("Error removing directory or file {}.  Error Message: {}",
+        throw IOException(stringFormat("Error removing directory or file {}.  Error Message: {}",
             path, posixErrMessage()));
         // LCOV_EXCL_STOP
     }
 }
 
 bool LocalFileSystem::fileOrPathExists(const std::string& path) const {
     return std::filesystem::exists(path);
@@ -196,162 +195,178 @@
         fullPath =
             context->getCurrentSetting(main::HomeDirectorySetting::name).getValue<std::string>() +
             fullPath.substr(1);
     }
     return fullPath;
 }
 
-void LocalFileSystem::readFromFile(FileInfo* fileInfo, void* buffer, uint64_t numBytes,
+void LocalFileSystem::readFromFile(FileInfo& fileInfo, void* buffer, uint64_t numBytes,
     uint64_t position) const {
-    auto localFileInfo = ku_dynamic_cast<FileInfo*, LocalFileInfo*>(fileInfo);
+    auto& localFileInfo = ku_dynamic_cast<const FileInfo&, const LocalFileInfo&>(fileInfo);
 #if defined(_WIN32)
     DWORD numBytesRead;
     OVERLAPPED overlapped{0, 0, 0, 0};
     overlapped.Offset = position & 0xffffffff;
     overlapped.OffsetHigh = position >> 32;
-    if (!ReadFile((HANDLE)localFileInfo->handle, buffer, numBytes, &numBytesRead, &overlapped)) {
+    if (!ReadFile((HANDLE)localFileInfo.handle, buffer, numBytes, &numBytesRead, &overlapped)) {
         auto error = GetLastError();
-        throw Exception(
+        throw IOException(
             stringFormat("Cannot read from file: {} handle: {} "
                          "numBytesRead: {} numBytesToRead: {} position: {}. Error {}: {}",
-                fileInfo->path, (intptr_t)localFileInfo->handle, numBytesRead, numBytes, position,
+                fileInfo.path, (intptr_t)localFileInfo.handle, numBytesRead, numBytes, position,
                 error, std::system_category().message(error)));
     }
-    if (numBytesRead != numBytes && fileInfo->getFileSize() != position + numBytesRead) {
-        throw Exception(stringFormat("Cannot read from file: {} handle: {} "
-                                     "numBytesRead: {} numBytesToRead: {} position: {}",
-            fileInfo->path, (intptr_t)localFileInfo->handle, numBytesRead, numBytes, position));
+    if (numBytesRead != numBytes && fileInfo.getFileSize() != position + numBytesRead) {
+        throw IOException(stringFormat("Cannot read from file: {} handle: {} "
+                                       "numBytesRead: {} numBytesToRead: {} position: {}",
+            fileInfo.path, (intptr_t)localFileInfo.handle, numBytesRead, numBytes, position));
     }
 #else
-    auto numBytesRead = pread(localFileInfo->fd, buffer, numBytes, position);
+    auto numBytesRead = pread(localFileInfo.fd, buffer, numBytes, position);
     if ((uint64_t)numBytesRead != numBytes &&
-        localFileInfo->getFileSize() != position + numBytesRead) {
+        localFileInfo.getFileSize() != position + numBytesRead) {
         // LCOV_EXCL_START
-        throw Exception(stringFormat("Cannot read from file: {} fileDescriptor: {} "
-                                     "numBytesRead: {} numBytesToRead: {} position: {}",
-            fileInfo->path, localFileInfo->fd, numBytesRead, numBytes, position));
+        throw IOException(stringFormat("Cannot read from file: {} fileDescriptor: {} "
+                                       "numBytesRead: {} numBytesToRead: {} position: {}",
+            fileInfo.path, localFileInfo.fd, numBytesRead, numBytes, position));
         // LCOV_EXCL_STOP
     }
 #endif
 }
 
-int64_t LocalFileSystem::readFile(FileInfo* fileInfo, void* buf, size_t nbyte) const {
-    auto localFileInfo = ku_dynamic_cast<FileInfo*, LocalFileInfo*>(fileInfo);
+int64_t LocalFileSystem::readFile(FileInfo& fileInfo, void* buf, size_t nbyte) const {
+    auto& localFileInfo = ku_dynamic_cast<const FileInfo&, const LocalFileInfo&>(fileInfo);
 #if defined(_WIN32)
     DWORD numBytesRead;
-    ReadFile((HANDLE)localFileInfo->handle, buf, nbyte, &numBytesRead, nullptr);
+    ReadFile((HANDLE)localFileInfo.handle, buf, nbyte, &numBytesRead, nullptr);
     return numBytesRead;
 #else
-    return read(localFileInfo->fd, buf, nbyte);
+    return read(localFileInfo.fd, buf, nbyte);
 #endif
 }
 
-void LocalFileSystem::writeFile(FileInfo* fileInfo, const uint8_t* buffer, uint64_t numBytes,
+void LocalFileSystem::writeFile(FileInfo& fileInfo, const uint8_t* buffer, uint64_t numBytes,
     uint64_t offset) const {
-    auto localFileInfo = ku_dynamic_cast<FileInfo*, LocalFileInfo*>(fileInfo);
+    auto& localFileInfo = ku_dynamic_cast<FileInfo&, LocalFileInfo&>(fileInfo);
     uint64_t remainingNumBytesToWrite = numBytes;
     uint64_t bufferOffset = 0;
     // Split large writes to 1GB at a time
     uint64_t maxBytesToWriteAtOnce = 1ull << 30; // 1ull << 30 = 1G
     while (remainingNumBytesToWrite > 0) {
         uint64_t numBytesToWrite = std::min(remainingNumBytesToWrite, maxBytesToWriteAtOnce);
 
 #if defined(_WIN32)
         DWORD numBytesWritten;
         OVERLAPPED overlapped{0, 0, 0, 0};
         overlapped.Offset = offset & 0xffffffff;
         overlapped.OffsetHigh = offset >> 32;
-        if (!WriteFile((HANDLE)localFileInfo->handle, buffer + bufferOffset, numBytesToWrite,
+        if (!WriteFile((HANDLE)localFileInfo.handle, buffer + bufferOffset, numBytesToWrite,
                 &numBytesWritten, &overlapped)) {
             auto error = GetLastError();
-            throw Exception(
+            throw IOException(
                 stringFormat("Cannot write to file. path: {} handle: {} offsetToWrite: {} "
                              "numBytesToWrite: {} numBytesWritten: {}. Error {}: {}.",
-                    fileInfo->path, (intptr_t)localFileInfo->handle, offset, numBytesToWrite,
+                    fileInfo.path, (intptr_t)localFileInfo.handle, offset, numBytesToWrite,
                     numBytesWritten, error, std::system_category().message(error)));
         }
 #else
         auto numBytesWritten =
-            pwrite(localFileInfo->fd, buffer + bufferOffset, numBytesToWrite, offset);
+            pwrite(localFileInfo.fd, buffer + bufferOffset, numBytesToWrite, offset);
         if (numBytesWritten != (int64_t)numBytesToWrite) {
             // LCOV_EXCL_START
-            throw Exception(
+            throw IOException(
                 stringFormat("Cannot write to file. path: {} fileDescriptor: {} offsetToWrite: {} "
                              "numBytesToWrite: {} numBytesWritten: {}. Error: {}",
-                    fileInfo->path, localFileInfo->fd, offset, numBytesToWrite, numBytesWritten,
+                    fileInfo.path, localFileInfo.fd, offset, numBytesToWrite, numBytesWritten,
                     posixErrMessage()));
             // LCOV_EXCL_STOP
         }
 #endif
         remainingNumBytesToWrite -= numBytesWritten;
         offset += numBytesWritten;
         bufferOffset += numBytesWritten;
     }
 }
 
-int64_t LocalFileSystem::seek(FileInfo* fileInfo, uint64_t offset, int whence) const {
-    auto localFileInfo = ku_dynamic_cast<FileInfo*, LocalFileInfo*>(fileInfo);
+void LocalFileSystem::syncFile(const FileInfo& fileInfo) const {
+    auto& localFileInfo = ku_dynamic_cast<const FileInfo&, const LocalFileInfo&>(fileInfo);
+#if defined(_WIN32)
+    // Note that `FlushFileBuffers` returns 0 when fail, while `fsync` returns 0 when succeed.
+    if (FlushFileBuffers((HANDLE)localFileInfo.handle) == 0) {
+        auto error = GetLastError();
+        throw IOException(stringFormat("Failed to sync file {}. Error {}: {}", fileInfo.path, error,
+            std::system_category().message(error)));
+    }
+#else
+    if (fsync(localFileInfo.fd) != 0) {
+        throw IOException(stringFormat("Failed to sync file {}.", fileInfo.path));
+    }
+#endif
+}
+
+int64_t LocalFileSystem::seek(FileInfo& fileInfo, uint64_t offset, int whence) const {
+    auto& localFileInfo = ku_dynamic_cast<FileInfo&, LocalFileInfo&>(fileInfo);
 #if defined(_WIN32)
     LARGE_INTEGER result;
     LARGE_INTEGER offset_;
     offset_.QuadPart = offset;
-    SetFilePointerEx((HANDLE)localFileInfo->handle, offset_, &result, whence);
+    SetFilePointerEx((HANDLE)localFileInfo.handle, offset_, &result, whence);
     return result.QuadPart;
 #else
-    return lseek(localFileInfo->fd, offset, whence);
+    return lseek(localFileInfo.fd, offset, whence);
 #endif
 }
 
-void LocalFileSystem::truncate(FileInfo* fileInfo, uint64_t size) const {
-    auto localFileInfo = ku_dynamic_cast<FileInfo*, LocalFileInfo*>(fileInfo);
+void LocalFileSystem::truncate(FileInfo& fileInfo, uint64_t size) const {
+    auto& localFileInfo = ku_dynamic_cast<FileInfo&, LocalFileInfo&>(fileInfo);
 #if defined(_WIN32)
     auto offsetHigh = (LONG)(size >> 32);
     LONG* offsetHighPtr = NULL;
     if (offsetHigh > 0)
         offsetHighPtr = &offsetHigh;
-    if (SetFilePointer((HANDLE)localFileInfo->handle, size & 0xffffffff, offsetHighPtr,
+    if (SetFilePointer((HANDLE)localFileInfo.handle, size & 0xffffffff, offsetHighPtr,
             FILE_BEGIN) == INVALID_SET_FILE_POINTER) {
         auto error = GetLastError();
-        throw Exception(stringFormat("Cannot set file pointer for file: {} handle: {} "
-                                     "new position: {}. Error {}: {}",
-            fileInfo->path, (intptr_t)localFileInfo->handle, size, error,
+        throw IOException(stringFormat("Cannot set file pointer for file: {} handle: {} "
+                                       "new position: {}. Error {}: {}",
+            fileInfo.path, (intptr_t)localFileInfo.handle, size, error,
             std::system_category().message(error)));
     }
-    if (!SetEndOfFile((HANDLE)localFileInfo->handle)) {
+    if (!SetEndOfFile((HANDLE)localFileInfo.handle)) {
         auto error = GetLastError();
-        throw Exception(stringFormat("Cannot truncate file: {} handle: {} "
-                                     "size: {}. Error {}: {}",
-            fileInfo->path, (intptr_t)localFileInfo->handle, size, error,
+        throw IOException(stringFormat("Cannot truncate file: {} handle: {} "
+                                       "size: {}. Error {}: {}",
+            fileInfo.path, (intptr_t)localFileInfo.handle, size, error,
             std::system_category().message(error)));
     }
 #else
-    if (ftruncate(localFileInfo->fd, size) < 0) {
+    if (ftruncate(localFileInfo.fd, size) < 0) {
         // LCOV_EXCL_START
-        throw Exception(
-            stringFormat("Failed to truncate file {}: {}", fileInfo->path, posixErrMessage()));
+        throw IOException(
+            stringFormat("Failed to truncate file {}: {}", fileInfo.path, posixErrMessage()));
         // LCOV_EXCL_STOP
     }
 #endif
 }
 
-uint64_t LocalFileSystem::getFileSize(kuzu::common::FileInfo* fileInfo) const {
-    auto localFileInfo = ku_dynamic_cast<FileInfo*, LocalFileInfo*>(fileInfo);
+uint64_t LocalFileSystem::getFileSize(const FileInfo& fileInfo) const {
+    auto& localFileInfo = ku_dynamic_cast<const FileInfo&, const LocalFileInfo&>(fileInfo);
 #ifdef _WIN32
     LARGE_INTEGER size;
-    if (!GetFileSizeEx((HANDLE)localFileInfo->handle, &size)) {
+    if (!GetFileSizeEx((HANDLE)localFileInfo.handle, &size)) {
         auto error = GetLastError();
-        throw Exception(stringFormat("Cannot read size of file. path: {} - Error {}: {}",
-            fileInfo->path, error, systemErrMessage(error)));
+        throw IOException(stringFormat("Cannot read size of file. path: {} - Error {}: {}",
+            fileInfo.path, error, systemErrMessage(error)));
     }
     return size.QuadPart;
 #else
     struct stat s;
-    if (fstat(localFileInfo->fd, &s) == -1) {
-        throw Exception(stringFormat("Cannot read size of file. path: {} - Error {}: {}",
-            fileInfo->path, errno, posixErrMessage()));
+    if (fstat(localFileInfo.fd, &s) == -1) {
+        throw IOException(stringFormat("Cannot read size of file. path: {} - Error {}: {}",
+            fileInfo.path, errno, posixErrMessage()));
     }
     KU_ASSERT(s.st_size >= 0);
     return s.st_size;
 #endif
 }
 
 } // namespace common
```

### sdist/kuzu-source/src/common/file_system/virtual_file_system.cpp

```diff
@@ -42,37 +42,41 @@
 }
 
 std::string VirtualFileSystem::expandPath(main::ClientContext* context,
     const std::string& path) const {
     return findFileSystem(path)->expandPath(context, path);
 }
 
-void VirtualFileSystem::readFromFile(FileInfo* /*fileInfo*/, void* /*buffer*/,
+void VirtualFileSystem::readFromFile(FileInfo& /*fileInfo*/, void* /*buffer*/,
     uint64_t /*numBytes*/, uint64_t /*position*/) const {
     KU_UNREACHABLE;
 }
 
-int64_t VirtualFileSystem::readFile(FileInfo* /*fileInfo*/, void* /*buf*/, size_t /*nbyte*/) const {
+int64_t VirtualFileSystem::readFile(FileInfo& /*fileInfo*/, void* /*buf*/, size_t /*nbyte*/) const {
     KU_UNREACHABLE;
 }
 
-void VirtualFileSystem::writeFile(FileInfo* /*fileInfo*/, const uint8_t* /*buffer*/,
+void VirtualFileSystem::writeFile(FileInfo& /*fileInfo*/, const uint8_t* /*buffer*/,
     uint64_t /*numBytes*/, uint64_t /*offset*/) const {
     KU_UNREACHABLE;
 }
 
-int64_t VirtualFileSystem::seek(FileInfo* /*fileInfo*/, uint64_t /*offset*/, int /*whence*/) const {
+void VirtualFileSystem::syncFile(const FileInfo& fileInfo) const {
+    findFileSystem(fileInfo.path)->syncFile(fileInfo);
+}
+
+int64_t VirtualFileSystem::seek(FileInfo& /*fileInfo*/, uint64_t /*offset*/, int /*whence*/) const {
     KU_UNREACHABLE;
 }
 
-void VirtualFileSystem::truncate(FileInfo* /*fileInfo*/, uint64_t /*size*/) const {
+void VirtualFileSystem::truncate(FileInfo& /*fileInfo*/, uint64_t /*size*/) const {
     KU_UNREACHABLE;
 }
 
-uint64_t VirtualFileSystem::getFileSize(kuzu::common::FileInfo* /*fileInfo*/) const {
+uint64_t VirtualFileSystem::getFileSize(const FileInfo& /*fileInfo*/) const {
     KU_UNREACHABLE;
 }
 
 FileSystem* VirtualFileSystem::findFileSystem(const std::string& path) const {
     for (auto& subSystem : subSystems) {
         if (subSystem->canHandleFile(path)) {
             return subSystem.get();
```

### sdist/kuzu-source/src/common/types/types.cpp

```diff
@@ -385,14 +385,44 @@
     case LogicalTypeID::RDF_VARIANT:
         return LogicalTypeUtils::toString(typeID);
     default:
         KU_UNREACHABLE;
     }
 }
 
+static LogicalTypeID strToLogicalTypeID(const std::string& trimmedStr);
+static std::vector<std::string> parseStructFields(const std::string& structTypeStr);
+static std::unique_ptr<LogicalType> parseListType(const std::string& trimmedStr);
+static std::unique_ptr<LogicalType> parseArrayType(const std::string& trimmedStr);
+static std::vector<StructField> parseStructTypeInfo(const std::string& structTypeStr);
+static std::unique_ptr<LogicalType> parseStructType(const std::string& trimmedStr);
+static std::unique_ptr<LogicalType> parseMapType(const std::string& trimmedStr);
+static std::unique_ptr<LogicalType> parseUnionType(const std::string& trimmedStr);
+
+LogicalType LogicalType::fromString(const std::string& str) {
+    LogicalType dataType;
+    auto trimmedStr = StringUtils::ltrim(StringUtils::rtrim(str));
+    auto upperDataTypeString = StringUtils::getUpper(trimmedStr);
+    if (upperDataTypeString.ends_with("[]")) {
+        dataType = *parseListType(trimmedStr);
+    } else if (upperDataTypeString.ends_with("]")) {
+        dataType = *parseArrayType(trimmedStr);
+    } else if (upperDataTypeString.starts_with("STRUCT")) {
+        dataType = *parseStructType(trimmedStr);
+    } else if (upperDataTypeString.starts_with("MAP")) {
+        dataType = *parseMapType(trimmedStr);
+    } else if (upperDataTypeString.starts_with("UNION")) {
+        dataType = *parseUnionType(trimmedStr);
+    } else {
+        dataType.typeID = strToLogicalTypeID(upperDataTypeString);
+    }
+    dataType.physicalType = LogicalType::getPhysicalType(dataType.typeID);
+    return dataType;
+}
+
 void LogicalType::serialize(Serializer& serializer) const {
     serializer.serializeValue(typeID);
     serializer.serializeValue(physicalType);
     switch (physicalType) {
     case PhysicalTypeID::LIST:
     case PhysicalTypeID::ARRAY:
     case PhysicalTypeID::STRUCT:
@@ -540,87 +570,66 @@
         return PhysicalTypeID::POINTER;
     } break;
     default:
         KU_UNREACHABLE;
     }
 }
 
-LogicalType LogicalTypeUtils::dataTypeFromString(const std::string& dataTypeString) {
-    LogicalType dataType;
-    auto trimmedStr = StringUtils::ltrim(StringUtils::rtrim(dataTypeString));
-    auto upperDataTypeString = StringUtils::getUpper(trimmedStr);
-    if (upperDataTypeString.ends_with("[]")) {
-        dataType = *parseListType(trimmedStr);
-    } else if (upperDataTypeString.ends_with("]")) {
-        dataType = *parseArrayType(trimmedStr);
-    } else if (upperDataTypeString.starts_with("STRUCT")) {
-        dataType = *parseStructType(trimmedStr);
-    } else if (upperDataTypeString.starts_with("MAP")) {
-        dataType = *parseMapType(trimmedStr);
-    } else if (upperDataTypeString.starts_with("UNION")) {
-        dataType = *parseUnionType(trimmedStr);
-    } else {
-        dataType.typeID = dataTypeIDFromString(upperDataTypeString);
-    }
-    dataType.physicalType = LogicalType::getPhysicalType(dataType.typeID);
-    return dataType;
-}
-
-LogicalTypeID LogicalTypeUtils::dataTypeIDFromString(const std::string& dataTypeIDString) {
-    auto upperDataTypeIDString = StringUtils::getUpper(dataTypeIDString);
-    if ("INTERNAL_ID" == upperDataTypeIDString) {
+LogicalTypeID strToLogicalTypeID(const std::string& str) {
+    auto upperStr = StringUtils::getUpper(str);
+    if ("INTERNAL_ID" == upperStr) {
         return LogicalTypeID::INTERNAL_ID;
-    } else if ("INT64" == upperDataTypeIDString) {
+    } else if ("INT64" == upperStr) {
         return LogicalTypeID::INT64;
-    } else if ("INT32" == upperDataTypeIDString || "INT" == upperDataTypeIDString) {
+    } else if ("INT32" == upperStr || "INT" == upperStr) {
         return LogicalTypeID::INT32;
-    } else if ("INT16" == upperDataTypeIDString) {
+    } else if ("INT16" == upperStr) {
         return LogicalTypeID::INT16;
-    } else if ("INT8" == upperDataTypeIDString) {
+    } else if ("INT8" == upperStr) {
         return LogicalTypeID::INT8;
-    } else if ("UINT64" == upperDataTypeIDString) {
+    } else if ("UINT64" == upperStr) {
         return LogicalTypeID::UINT64;
-    } else if ("UINT32" == upperDataTypeIDString) {
+    } else if ("UINT32" == upperStr) {
         return LogicalTypeID::UINT32;
-    } else if ("UINT16" == upperDataTypeIDString) {
+    } else if ("UINT16" == upperStr) {
         return LogicalTypeID::UINT16;
-    } else if ("UINT8" == upperDataTypeIDString) {
+    } else if ("UINT8" == upperStr) {
         return LogicalTypeID::UINT8;
-    } else if ("INT128" == upperDataTypeIDString) {
+    } else if ("INT128" == upperStr) {
         return LogicalTypeID::INT128;
-    } else if ("DOUBLE" == upperDataTypeIDString) {
+    } else if ("DOUBLE" == upperStr || "FLOAT8" == upperStr) {
         return LogicalTypeID::DOUBLE;
-    } else if ("FLOAT" == upperDataTypeIDString) {
+    } else if ("FLOAT" == upperStr || "FLOAT4" == upperStr || "REAL" == upperStr) {
         return LogicalTypeID::FLOAT;
-    } else if ("BOOLEAN" == upperDataTypeIDString || "BOOL" == upperDataTypeIDString) {
+    } else if ("BOOLEAN" == upperStr || "BOOL" == upperStr) {
         return LogicalTypeID::BOOL;
-    } else if ("BYTEA" == upperDataTypeIDString || "BLOB" == upperDataTypeIDString) {
+    } else if ("BYTEA" == upperStr || "BLOB" == upperStr) {
         return LogicalTypeID::BLOB;
-    } else if ("UUID" == upperDataTypeIDString) {
+    } else if ("UUID" == upperStr) {
         return LogicalTypeID::UUID;
-    } else if ("STRING" == upperDataTypeIDString) {
+    } else if ("STRING" == upperStr) {
         return LogicalTypeID::STRING;
-    } else if ("DATE" == upperDataTypeIDString) {
+    } else if ("DATE" == upperStr) {
         return LogicalTypeID::DATE;
-    } else if ("TIMESTAMP" == upperDataTypeIDString) {
+    } else if ("TIMESTAMP" == upperStr) {
         return LogicalTypeID::TIMESTAMP;
-    } else if ("TIMESTAMP_NS" == upperDataTypeIDString) {
+    } else if ("TIMESTAMP_NS" == upperStr) {
         return LogicalTypeID::TIMESTAMP_NS;
-    } else if ("TIMESTAMP_MS" == upperDataTypeIDString) {
+    } else if ("TIMESTAMP_MS" == upperStr) {
         return LogicalTypeID::TIMESTAMP_MS;
-    } else if ("TIMESTAMP_SEC" == upperDataTypeIDString || "TIMESTAMP_S" == upperDataTypeIDString) {
+    } else if ("TIMESTAMP_SEC" == upperStr || "TIMESTAMP_S" == upperStr) {
         return LogicalTypeID::TIMESTAMP_SEC;
-    } else if ("TIMESTAMP_TZ" == upperDataTypeIDString) {
+    } else if ("TIMESTAMP_TZ" == upperStr) {
         return LogicalTypeID::TIMESTAMP_TZ;
-    } else if ("INTERVAL" == upperDataTypeIDString) {
+    } else if ("INTERVAL" == upperStr || "DURATION" == upperStr) {
         return LogicalTypeID::INTERVAL;
-    } else if ("SERIAL" == upperDataTypeIDString) {
+    } else if ("SERIAL" == upperStr) {
         return LogicalTypeID::SERIAL;
     } else {
-        throw NotImplementedException("Cannot parse dataTypeID: " + dataTypeIDString);
+        throw NotImplementedException("Cannot parse dataTypeID: " + str);
     }
 }
 
 std::string LogicalTypeUtils::toString(LogicalTypeID dataTypeID) {
     // LCOV_EXCL_START
     switch (dataTypeID) {
     case LogicalTypeID::ANY:
@@ -818,15 +827,15 @@
         LogicalTypeID::TIMESTAMP_NS, LogicalTypeID::TIMESTAMP_MS, LogicalTypeID::TIMESTAMP_SEC,
         LogicalTypeID::TIMESTAMP_TZ, LogicalTypeID::INTERVAL, LogicalTypeID::LIST,
         LogicalTypeID::ARRAY, LogicalTypeID::MAP, LogicalTypeID::FLOAT, LogicalTypeID::SERIAL,
         LogicalTypeID::NODE, LogicalTypeID::REL, LogicalTypeID::STRUCT, LogicalTypeID::UNION,
         LogicalTypeID::RDF_VARIANT};
 }
 
-std::vector<std::string> LogicalTypeUtils::parseStructFields(const std::string& structTypeStr) {
+std::vector<std::string> parseStructFields(const std::string& structTypeStr) {
     std::vector<std::string> structFieldsStr;
     auto startPos = 0u;
     auto curPos = 0u;
     auto numOpenBrackets = 0u;
     while (curPos < structTypeStr.length()) {
         switch (structTypeStr[curPos]) {
         case '(': {
@@ -849,30 +858,30 @@
         curPos++;
     }
     structFieldsStr.push_back(
         StringUtils::ltrim(structTypeStr.substr(startPos, curPos - startPos)));
     return structFieldsStr;
 }
 
-std::unique_ptr<LogicalType> LogicalTypeUtils::parseListType(const std::string& trimmedStr) {
-    return LogicalType::LIST(dataTypeFromString(trimmedStr.substr(0, trimmedStr.size() - 2)));
+std::unique_ptr<LogicalType> parseListType(const std::string& trimmedStr) {
+    return LogicalType::LIST(LogicalType::fromString(trimmedStr.substr(0, trimmedStr.size() - 2)));
 }
 
-std::unique_ptr<LogicalType> LogicalTypeUtils::parseArrayType(const std::string& trimmedStr) {
+std::unique_ptr<LogicalType> parseArrayType(const std::string& trimmedStr) {
     auto leftBracketPos = trimmedStr.find_last_of('[');
     auto rightBracketPos = trimmedStr.find_last_of(']');
-    auto childType =
-        std::make_unique<LogicalType>(dataTypeFromString(trimmedStr.substr(0, leftBracketPos)));
+    auto childType = std::make_unique<LogicalType>(
+        LogicalType::fromString(trimmedStr.substr(0, leftBracketPos)));
     auto numElements = std::strtoll(
         trimmedStr.substr(leftBracketPos + 1, rightBracketPos - leftBracketPos - 1).c_str(),
         nullptr, 0 /* base */);
     return LogicalType::ARRAY(std::move(childType), numElements);
 }
 
-std::vector<StructField> LogicalTypeUtils::parseStructTypeInfo(const std::string& structTypeStr) {
+std::vector<StructField> parseStructTypeInfo(const std::string& structTypeStr) {
     auto leftBracketPos = structTypeStr.find('(');
     auto rightBracketPos = structTypeStr.find_last_of(')');
     if (leftBracketPos == std::string::npos || rightBracketPos == std::string::npos) {
         throw Exception("Cannot parse struct type: " + structTypeStr);
     }
     // Remove the leading and trailing brackets.
     auto structFieldsStr =
@@ -880,36 +889,36 @@
     std::vector<StructField> structFields;
     auto structFieldStrs = parseStructFields(structFieldsStr);
     for (auto& structFieldStr : structFieldStrs) {
         auto pos = structFieldStr.find(' ');
         auto fieldName = structFieldStr.substr(0, pos);
         auto fieldTypeString = structFieldStr.substr(pos + 1);
         structFields.emplace_back(fieldName,
-            std::make_unique<LogicalType>(dataTypeFromString(fieldTypeString)));
+            std::make_unique<LogicalType>(LogicalType::fromString(fieldTypeString)));
     }
     return structFields;
 }
 
-std::unique_ptr<LogicalType> LogicalTypeUtils::parseStructType(const std::string& trimmedStr) {
+std::unique_ptr<LogicalType> parseStructType(const std::string& trimmedStr) {
     return LogicalType::STRUCT(parseStructTypeInfo(trimmedStr));
 }
 
-std::unique_ptr<LogicalType> LogicalTypeUtils::parseMapType(const std::string& trimmedStr) {
+std::unique_ptr<LogicalType> parseMapType(const std::string& trimmedStr) {
     auto leftBracketPos = trimmedStr.find('(');
     auto rightBracketPos = trimmedStr.find_last_of(')');
     if (leftBracketPos == std::string::npos || rightBracketPos == std::string::npos) {
         throw Exception("Cannot parse map type: " + trimmedStr);
     }
     auto mapTypeStr = trimmedStr.substr(leftBracketPos + 1, rightBracketPos - leftBracketPos - 1);
     auto keyValueTypes = StringUtils::splitComma(mapTypeStr);
-    return LogicalType::MAP(dataTypeFromString(keyValueTypes[0]),
-        dataTypeFromString(keyValueTypes[1]));
+    return LogicalType::MAP(LogicalType::fromString(keyValueTypes[0]),
+        LogicalType::fromString(keyValueTypes[1]));
 }
 
-std::unique_ptr<LogicalType> LogicalTypeUtils::parseUnionType(const std::string& trimmedStr) {
+std::unique_ptr<LogicalType> parseUnionType(const std::string& trimmedStr) {
     auto unionFields = parseStructTypeInfo(trimmedStr);
     auto unionTagField = StructField(UnionType::TAG_FIELD_NAME,
         std::make_unique<LogicalType>(UnionType::TAG_FIELD_TYPE));
     unionFields.insert(unionFields.begin(), std::move(unionTagField));
     return LogicalType::UNION(std::move(unionFields));
 }
```

### sdist/kuzu-source/src/function/built_in_function_utils.cpp

```diff
@@ -13,40 +13,51 @@
 using namespace kuzu::catalog;
 using namespace kuzu::processor;
 
 namespace kuzu {
 namespace function {
 
 static void validateNonEmptyCandidateFunctions(std::vector<AggregateFunction*>& candidateFunctions,
-    const std::string& name, const std::vector<common::LogicalType>& inputTypes, bool isDistinct,
-    function::function_set& set);
+    const std::string& name, const std::vector<LogicalType>& inputTypes, bool isDistinct,
+    const function::function_set& set);
 static void validateNonEmptyCandidateFunctions(std::vector<Function*>& candidateFunctions,
-    const std::string& name, const std::vector<common::LogicalType>& inputTypes,
-    function::function_set& set);
+    const std::string& name, const std::vector<LogicalType>& inputTypes,
+    const function::function_set& set);
 
 void BuiltInFunctionsUtils::createFunctions(CatalogSet* catalogSet) {
     auto functions = FunctionCollection::getFunctions();
     for (auto i = 0u; functions[i].name != nullptr; ++i) {
         auto functionSet = functions[i].getFunctionSetFunc();
         catalogSet->createEntry(std::make_unique<FunctionCatalogEntry>(
             functions[i].catalogEntryType, functions[i].name, std::move(functionSet)));
     }
 }
 
+catalog::CatalogEntry* BuiltInFunctionsUtils::getFunctionCatalogEntry(const std::string& name,
+    CatalogSet* catalogSet) {
+    if (!catalogSet->containsEntry(name)) {
+        throw CatalogException(stringFormat("{} function does not exist.", name));
+    }
+    return catalogSet->getEntry(name);
+}
+
 Function* BuiltInFunctionsUtils::matchFunction(const std::string& name, CatalogSet* catalogSet) {
-    return matchFunction(name, std::vector<common::LogicalType>{}, catalogSet);
+    return matchFunction(name, std::vector<LogicalType>{}, catalogSet);
 }
 
 Function* BuiltInFunctionsUtils::matchFunction(const std::string& name,
-    const std::vector<common::LogicalType>& inputTypes, CatalogSet* catalogSet) {
-    if (!catalogSet->containsEntry(name)) {
-        throw CatalogException(stringFormat("{} function does not exist.", name));
-    }
-    auto& functionSet =
-        reinterpret_cast<FunctionCatalogEntry*>(catalogSet->getEntry(name))->getFunctionSet();
+    const std::vector<LogicalType>& inputTypes, CatalogSet* catalogSet) {
+    auto entry = getFunctionCatalogEntry(name, catalogSet);
+    return matchFunction(name, inputTypes, entry);
+}
+
+Function* BuiltInFunctionsUtils::matchFunction(const std::string& name,
+    const std::vector<LogicalType>& inputTypes, const catalog::CatalogEntry* catalogEntry) {
+    auto functionEntry = catalogEntry->constPtrCast<FunctionCatalogEntry>();
+    auto& functionSet = functionEntry->getFunctionSet();
     bool isOverload = functionSet.size() > 1;
     std::vector<Function*> candidateFunctions;
     uint32_t minCost = UINT32_MAX;
     for (auto& function : functionSet) {
         auto func = reinterpret_cast<Function*>(function.get());
         auto cost = getFunctionCost(inputTypes, func, isOverload);
         if (cost == UINT32_MAX) {
@@ -65,15 +76,15 @@
         return getBestMatch(candidateFunctions);
     }
     validateSpecialCases(candidateFunctions, name, inputTypes, functionSet);
     return candidateFunctions[0];
 }
 
 AggregateFunction* BuiltInFunctionsUtils::matchAggregateFunction(const std::string& name,
-    const std::vector<common::LogicalType>& inputTypes, bool isDistinct, CatalogSet* catalogSet) {
+    const std::vector<LogicalType>& inputTypes, bool isDistinct, CatalogSet* catalogSet) {
     auto& functionSet =
         reinterpret_cast<FunctionCatalogEntry*>(catalogSet->getEntry(name))->getFunctionSet();
     std::vector<AggregateFunction*> candidateFunctions;
     for (auto& function : functionSet) {
         auto aggregateFunction = ku_dynamic_cast<Function*, AggregateFunction*>(function.get());
         auto cost = getAggregateFunctionCost(inputTypes, isDistinct, aggregateFunction);
         if (cost == UINT32_MAX) {
@@ -457,15 +468,15 @@
         cost += castCost;
     }
     return cost;
 }
 
 void BuiltInFunctionsUtils::validateSpecialCases(std::vector<Function*>& candidateFunctions,
     const std::string& name, const std::vector<LogicalType>& inputTypes,
-    function::function_set& set) {
+    const function::function_set& set) {
     // special case for add func
     if (name == AddFunction::name) {
         auto targetType0 = candidateFunctions[0]->parameterTypeIDs[0];
         auto targetType1 = candidateFunctions[0]->parameterTypeIDs[1];
         auto inputType0 = inputTypes[0].getLogicalTypeID();
         auto inputType1 = inputTypes[1].getLogicalTypeID();
         if ((inputType0 != LogicalTypeID::STRING || inputType1 != LogicalTypeID::STRING) &&
@@ -496,15 +507,15 @@
         result += " Supported inputs are\n" + supportedInputs;
     }
     return result;
 }
 
 void validateNonEmptyCandidateFunctions(std::vector<AggregateFunction*>& candidateFunctions,
     const std::string& name, const std::vector<LogicalType>& inputTypes, bool isDistinct,
-    function::function_set& set) {
+    const function::function_set& set) {
     if (candidateFunctions.empty()) {
         std::string supportedInputsString;
         for (auto& function : set) {
             auto aggregateFunction = ku_dynamic_cast<Function*, AggregateFunction*>(function.get());
             if (aggregateFunction->isDistinct) {
                 supportedInputsString += "DISTINCT ";
             }
@@ -513,15 +524,15 @@
         throw BinderException(
             getFunctionMatchFailureMsg(name, inputTypes, supportedInputsString, isDistinct));
     }
 }
 
 void validateNonEmptyCandidateFunctions(std::vector<Function*>& candidateFunctions,
     const std::string& name, const std::vector<LogicalType>& inputTypes,
-    function::function_set& set) {
+    const function::function_set& set) {
     if (candidateFunctions.empty()) {
         std::string supportedInputsString;
         for (auto& function : set) {
             if (function->parameterTypeIDs.empty()) {
                 continue;
             }
             supportedInputsString += function->signatureToString() + "\n";
```

### sdist/kuzu-source/src/include/catalog/catalog.h

```diff
@@ -53,16 +53,18 @@
     common::table_id_t createTableSchema(const binder::BoundCreateTableInfo& info);
     void dropTableSchema(common::table_id_t tableID);
     void alterTableSchema(const binder::BoundAlterInfo& info);
 
     void setTableComment(common::table_id_t tableID, const std::string& comment);
 
     // ----------------------------- Functions ----------------------------
-    void addFunction(std::string name, function::function_set functionSet);
-    void addBuiltInFunction(std::string name, function::function_set functionSet);
+    void addFunction(CatalogEntryType entryType, std::string name,
+        function::function_set functionSet);
+    void addBuiltInFunction(CatalogEntryType entryType, std::string name,
+        function::function_set functionSet);
     CatalogSet* getFunctions(transaction::Transaction* tx) const;
     CatalogEntry* getFunctionEntry(transaction::Transaction* tx, const std::string& name);
 
     bool containsMacro(transaction::Transaction* tx, const std::string& macroName) const;
     void addScalarMacroFunction(std::string name,
         std::unique_ptr<function::ScalarMacroFunction> macro);
     // TODO(Ziyi): pass transaction pointer here.
```

### sdist/kuzu-source/src/include/catalog/catalog_content.h

```diff
@@ -49,15 +49,16 @@
 private:
     // ----------------------------- Functions ----------------------------
     void registerBuiltInFunctions();
 
     bool containMacro(const std::string& macroName) const {
         return functions->containsEntry(macroName);
     }
-    void addFunction(std::string name, function::function_set definitions);
+    void addFunction(CatalogEntryType entryType, std::string name,
+        function::function_set definitions);
 
     function::ScalarMacroFunction* getScalarMacroFunction(const std::string& name) const;
 
     // ----------------------------- Table entries ----------------------------
     uint64_t getNumTables() const { return tables->getEntries().size(); }
 
     bool containsTable(const std::string& tableName) const;
```

### sdist/kuzu-source/src/include/catalog/catalog_entry/catalog_entry.h

```diff
@@ -29,14 +29,19 @@
     // serialization & deserialization
     //===--------------------------------------------------------------------===//
     virtual void serialize(common::Serializer& serializer) const;
     static std::unique_ptr<CatalogEntry> deserialize(common::Deserializer& deserializer);
     virtual std::unique_ptr<CatalogEntry> copy() const = 0;
     virtual std::string toCypher(main::ClientContext* /*clientContext*/) const { KU_UNREACHABLE; }
 
+    template<class TARGET>
+    const TARGET* constPtrCast() const {
+        return common::ku_dynamic_cast<const CatalogEntry*, const TARGET*>(this);
+    }
+
 private:
     CatalogEntryType type;
     std::string name;
 };
 
 } // namespace catalog
 } // namespace kuzu
```

### sdist/kuzu-source/src/include/catalog/catalog_entry/catalog_entry_type.h

```diff
@@ -1,10 +1,11 @@
 #pragma once
 
 #include <cstdint>
+#include <string>
 
 namespace kuzu {
 namespace catalog {
 
 enum class CatalogEntryType : uint8_t {
     NODE_TABLE_ENTRY = 0,
     REL_TABLE_ENTRY = 1,
@@ -14,9 +15,13 @@
     AGGREGATE_FUNCTION_ENTRY = 5,
     SCALAR_FUNCTION_ENTRY = 6,
     REWRITE_FUNCTION_ENTRY = 7,
     TABLE_FUNCTION_ENTRY = 8,
     FOREIGN_TABLE_ENTRY = 9,
 };
 
+struct CatalogEntryTypeUtils {
+    static std::string toString(CatalogEntryType type);
+};
+
 } // namespace catalog
 } // namespace kuzu
```

### sdist/kuzu-source/src/include/catalog/catalog_entry/function_catalog_entry.h

```diff
@@ -14,15 +14,15 @@
     FunctionCatalogEntry() = default;
     FunctionCatalogEntry(CatalogEntryType entryType, std::string name,
         function::function_set functionSet);
 
     //===--------------------------------------------------------------------===//
     // getters & setters
     //===--------------------------------------------------------------------===//
-    function::function_set& getFunctionSet() { return functionSet; }
+    const function::function_set& getFunctionSet() const { return functionSet; }
 
     //===--------------------------------------------------------------------===//
     // serialization & deserialization
     //===--------------------------------------------------------------------===//
     // We always register functions while initializing the catalog, so we don't have to
     // serialize functions.
     void serialize(common::Serializer& /*serializer*/) const override { return; }
```

### sdist/kuzu-source/src/include/common/file_system/file_info.h

```diff
@@ -12,23 +12,24 @@
 
 struct KUZU_API FileInfo {
     FileInfo(std::string path, FileSystem* fileSystem)
         : path{std::move(path)}, fileSystem{fileSystem} {}
 
     virtual ~FileInfo() = default;
 
-    // TODO: This function should be marked as const.
-    uint64_t getFileSize();
+    uint64_t getFileSize() const;
 
     void readFromFile(void* buffer, uint64_t numBytes, uint64_t position);
 
     int64_t readFile(void* buf, size_t nbyte);
 
     void writeFile(const uint8_t* buffer, uint64_t numBytes, uint64_t offset);
 
+    void syncFile() const;
+
     int64_t seek(uint64_t offset, int whence);
 
     void truncate(uint64_t size);
 
     const std::string path;
 
     FileSystem* fileSystem;
```

### sdist/kuzu-source/src/include/common/file_system/file_system.h

```diff
@@ -41,25 +41,27 @@
 
     static std::string joinPath(const std::string& base, const std::string& part);
 
     static std::string getFileExtension(const std::filesystem::path& path);
 
     virtual bool canHandleFile(const std::string& /*path*/) const { KU_UNREACHABLE; }
 
+    virtual void syncFile(const FileInfo& fileInfo) const = 0;
+
 protected:
-    virtual void readFromFile(FileInfo* fileInfo, void* buffer, uint64_t numBytes,
+    virtual void readFromFile(FileInfo& fileInfo, void* buffer, uint64_t numBytes,
         uint64_t position) const = 0;
 
-    virtual int64_t readFile(FileInfo* fileInfo, void* buf, size_t nbyte) const = 0;
+    virtual int64_t readFile(FileInfo& fileInfo, void* buf, size_t nbyte) const = 0;
 
-    virtual void writeFile(FileInfo* fileInfo, const uint8_t* buffer, uint64_t numBytes,
+    virtual void writeFile(FileInfo& fileInfo, const uint8_t* buffer, uint64_t numBytes,
         uint64_t offset) const;
 
-    virtual int64_t seek(FileInfo* fileInfo, uint64_t offset, int whence) const = 0;
+    virtual int64_t seek(FileInfo& fileInfo, uint64_t offset, int whence) const = 0;
 
-    virtual void truncate(FileInfo* fileInfo, uint64_t size) const;
+    virtual void truncate(FileInfo& fileInfo, uint64_t size) const;
 
-    virtual uint64_t getFileSize(FileInfo* fileInfo) const = 0;
+    virtual uint64_t getFileSize(const FileInfo& fileInfo) const = 0;
 };
 
 } // namespace common
 } // namespace kuzu
```

### sdist/kuzu-source/src/include/common/file_system/local_file_system.h

```diff
@@ -42,25 +42,27 @@
 
     void removeFileIfExists(const std::string& path) const override;
 
     bool fileOrPathExists(const std::string& path) const override;
 
     std::string expandPath(main::ClientContext* context, const std::string& path) const override;
 
+    void syncFile(const FileInfo& fileInfo) const override;
+
 protected:
-    void readFromFile(FileInfo* fileInfo, void* buffer, uint64_t numBytes,
+    void readFromFile(FileInfo& fileInfo, void* buffer, uint64_t numBytes,
         uint64_t position) const override;
 
-    int64_t readFile(FileInfo* fileInfo, void* buf, size_t nbyte) const override;
+    int64_t readFile(FileInfo& fileInfo, void* buf, size_t nbyte) const override;
 
-    void writeFile(FileInfo* fileInfo, const uint8_t* buffer, uint64_t numBytes,
+    void writeFile(FileInfo& fileInfo, const uint8_t* buffer, uint64_t numBytes,
         uint64_t offset) const override;
 
-    int64_t seek(FileInfo* fileInfo, uint64_t offset, int whence) const override;
+    int64_t seek(FileInfo& fileInfo, uint64_t offset, int whence) const override;
 
-    void truncate(FileInfo* fileInfo, uint64_t size) const override;
+    void truncate(FileInfo& fileInfo, uint64_t size) const override;
 
-    uint64_t getFileSize(FileInfo* fileInfo) const override;
+    uint64_t getFileSize(const FileInfo& fileInfo) const override;
 };
 
 } // namespace common
 } // namespace kuzu
```

### sdist/kuzu-source/src/include/common/file_system/virtual_file_system.h

```diff
@@ -28,28 +28,30 @@
 
     void removeFileIfExists(const std::string& path) const override;
 
     bool fileOrPathExists(const std::string& path) const override;
 
     std::string expandPath(main::ClientContext* context, const std::string& path) const override;
 
+    void syncFile(const FileInfo& fileInfo) const override;
+
 protected:
-    void readFromFile(FileInfo* fileInfo, void* buffer, uint64_t numBytes,
+    void readFromFile(FileInfo& fileInfo, void* buffer, uint64_t numBytes,
         uint64_t position) const override;
 
-    int64_t readFile(FileInfo* fileInfo, void* buf, size_t nbyte) const override;
+    int64_t readFile(FileInfo& fileInfo, void* buf, size_t nbyte) const override;
 
-    void writeFile(FileInfo* fileInfo, const uint8_t* buffer, uint64_t numBytes,
+    void writeFile(FileInfo& fileInfo, const uint8_t* buffer, uint64_t numBytes,
         uint64_t offset) const override;
 
-    int64_t seek(FileInfo* fileInfo, uint64_t offset, int whence) const override;
+    int64_t seek(FileInfo& fileInfo, uint64_t offset, int whence) const override;
 
-    void truncate(FileInfo* fileInfo, uint64_t size) const override;
+    void truncate(FileInfo& fileInfo, uint64_t size) const override;
 
-    uint64_t getFileSize(FileInfo* fileInfo) const override;
+    uint64_t getFileSize(const FileInfo& fileInfo) const override;
 
 private:
     FileSystem* findFileSystem(const std::string& path) const;
 
 private:
     std::vector<std::unique_ptr<FileSystem>> subSystems;
     std::unique_ptr<FileSystem> defaultFS;
```

### sdist/kuzu-source/src/include/common/types/types.h

```diff
@@ -266,44 +266,41 @@
 
 private:
     std::vector<StructField> fields;
     std::unordered_map<std::string, struct_field_idx_t> fieldNameToIdxMap;
 };
 
 class LogicalType {
-    friend class LogicalTypeUtils;
+    friend struct LogicalTypeUtils;
     friend struct StructType;
     friend struct ListType;
     friend struct ArrayType;
 
 public:
     KUZU_API LogicalType() : typeID{LogicalTypeID::ANY}, extraTypeInfo{nullptr} {
         physicalType = getPhysicalType(this->typeID);
     };
     explicit KUZU_API LogicalType(LogicalTypeID typeID);
     KUZU_API LogicalType(const LogicalType& other);
     KUZU_API LogicalType(LogicalType&& other) = default;
 
     KUZU_API LogicalType& operator=(const LogicalType& other);
-
     KUZU_API bool operator==(const LogicalType& other) const;
-
     KUZU_API bool operator!=(const LogicalType& other) const;
-
     KUZU_API LogicalType& operator=(LogicalType&& other) = default;
 
     KUZU_API std::string toString() const;
+    static LogicalType fromString(const std::string& str);
 
-    KUZU_API inline LogicalTypeID getLogicalTypeID() const { return typeID; }
+    KUZU_API LogicalTypeID getLogicalTypeID() const { return typeID; }
 
-    inline PhysicalTypeID getPhysicalType() const { return physicalType; }
+    PhysicalTypeID getPhysicalType() const { return physicalType; }
     static PhysicalTypeID getPhysicalType(LogicalTypeID logicalType);
 
-    inline bool hasExtraTypeInfo() const { return extraTypeInfo != nullptr; }
-    inline void setExtraTypeInfo(std::unique_ptr<ExtraTypeInfo> typeInfo) {
+    void setExtraTypeInfo(std::unique_ptr<ExtraTypeInfo> typeInfo) {
         extraTypeInfo = std::move(typeInfo);
     }
 
     void serialize(Serializer& serializer) const;
 
     static std::unique_ptr<LogicalType> deserialize(Deserializer& deserializer);
 
@@ -438,16 +435,14 @@
 
 private:
     LogicalTypeID typeID;
     PhysicalTypeID physicalType;
     std::unique_ptr<ExtraTypeInfo> extraTypeInfo;
 };
 
-// TODO: Should remove `logical_types_t`.
-using logical_types_t = std::vector<std::unique_ptr<LogicalType>>;
 using logical_type_vec_t = std::vector<LogicalType>;
 
 struct ListType {
     static inline LogicalType* getChildType(const LogicalType* type) {
         KU_ASSERT(type->getPhysicalType() == PhysicalTypeID::LIST ||
                   type->getPhysicalType() == PhysicalTypeID::ARRAY);
         auto listTypeInfo = reinterpret_cast<ListTypeInfo*>(type->extraTypeInfo.get());
@@ -572,37 +567,25 @@
 };
 
 struct PhysicalTypeUtils {
     static std::string physicalTypeToString(PhysicalTypeID physicalType);
     static uint32_t getFixedTypeSize(PhysicalTypeID physicalType);
 };
 
-class LogicalTypeUtils {
-public:
+struct LogicalTypeUtils {
     KUZU_API static std::string toString(LogicalTypeID dataTypeID);
     KUZU_API static std::string toString(const std::vector<LogicalType>& dataTypes);
     KUZU_API static std::string toString(const std::vector<LogicalTypeID>& dataTypeIDs);
-    KUZU_API static LogicalType dataTypeFromString(const std::string& dataTypeString);
     static uint32_t getRowLayoutSize(const LogicalType& logicalType);
     static bool isNumerical(const LogicalType& dataType);
     static bool isNested(const LogicalType& dataType);
     static bool isNested(LogicalTypeID logicalTypeID);
     static std::vector<LogicalTypeID> getAllValidComparableLogicalTypes();
     static std::vector<LogicalTypeID> getNumericalLogicalTypeIDs();
     static std::vector<LogicalTypeID> getIntegerLogicalTypeIDs();
     static std::vector<LogicalTypeID> getAllValidLogicTypes();
-
-private:
-    static LogicalTypeID dataTypeIDFromString(const std::string& trimmedStr);
-    static std::vector<std::string> parseStructFields(const std::string& structTypeStr);
-    static std::unique_ptr<LogicalType> parseListType(const std::string& trimmedStr);
-    static std::unique_ptr<LogicalType> parseArrayType(const std::string& trimmedStr);
-    static std::vector<StructField> parseStructTypeInfo(const std::string& structTypeStr);
-    static std::unique_ptr<LogicalType> parseStructType(const std::string& trimmedStr);
-    static std::unique_ptr<LogicalType> parseMapType(const std::string& trimmedStr);
-    static std::unique_ptr<LogicalType> parseUnionType(const std::string& trimmedStr);
 };
 
 enum class FileVersionType : uint8_t { ORIGINAL = 0, WAL_VERSION = 1 };
 
 } // namespace common
 } // namespace kuzu
```

### sdist/kuzu-source/src/include/function/built_in_function_utils.h

```diff
@@ -2,27 +2,33 @@
 
 #include "aggregate_function.h"
 #include "function.h"
 
 namespace kuzu {
 namespace catalog {
 class CatalogSet;
+class CatalogEntry;
 } // namespace catalog
 
 namespace function {
 
 class BuiltInFunctionsUtils {
 public:
     static void createFunctions(catalog::CatalogSet* catalogSet);
 
+    static catalog::CatalogEntry* getFunctionCatalogEntry(const std::string& name,
+        catalog::CatalogSet* catalogSet);
     static Function* matchFunction(const std::string& name, catalog::CatalogSet* catalogSet);
     // TODO(Ziyi): We should have a unified interface for matching table, aggregate and scalar
     // functions.
     static Function* matchFunction(const std::string& name,
         const std::vector<common::LogicalType>& inputTypes, catalog::CatalogSet* catalogSet);
+    static Function* matchFunction(const std::string& name,
+        const std::vector<common::LogicalType>& inputTypes,
+        const catalog::CatalogEntry* catalogEntry);
 
     static AggregateFunction* matchAggregateFunction(const std::string& name,
         const std::vector<common::LogicalType>& inputTypes, bool isDistinct,
         catalog::CatalogSet* catalogSet);
 
     static uint32_t getCastCost(common::LogicalTypeID inputTypeID,
         common::LogicalTypeID targetTypeID);
@@ -74,12 +80,12 @@
     static uint32_t matchVarLengthParameters(const std::vector<common::LogicalType>& inputTypes,
         common::LogicalTypeID targetTypeID, bool isOverload);
     static uint32_t getAggregateFunctionCost(const std::vector<common::LogicalType>& inputTypes,
         bool isDistinct, AggregateFunction* function);
 
     static void validateSpecialCases(std::vector<Function*>& candidateFunctions,
         const std::string& name, const std::vector<common::LogicalType>& inputTypes,
-        function::function_set& set);
+        const function::function_set& set);
 };
 
 } // namespace function
 } // namespace kuzu
```

### sdist/kuzu-source/src/include/function/function.h

```diff
@@ -41,14 +41,19 @@
 
     virtual std::unique_ptr<Function> copy() const = 0;
 
     // TODO(Ziyi): Move to catalog entry once we have implemented the catalog entry.
     FunctionType type;
     std::string name;
     std::vector<common::LogicalTypeID> parameterTypeIDs;
+
+    template<class TARGET>
+    const TARGET* constPtrCast() const {
+        return common::ku_dynamic_cast<const Function*, const TARGET*>(this);
+    }
 };
 
 struct BaseScalarFunction : public Function {
     BaseScalarFunction(FunctionType type, std::string name,
         std::vector<common::LogicalTypeID> parameterTypeIDs, common::LogicalTypeID returnTypeID,
         scalar_bind_func bindFunc)
         : Function{type, std::move(name), std::move(parameterTypeIDs)}, returnTypeID{returnTypeID},
```

### sdist/kuzu-source/src/include/main/database.h

```diff
@@ -97,15 +97,15 @@
      * @param loggingLevel New logging level. (Supported logging levels are: "info", "debug",
      * "err").
      */
     KUZU_API static void setLoggingLevel(std::string loggingLevel);
 
     // TODO(Ziyi): Instead of exposing a dedicated API for adding a new function, we should consider
     // add function through the extension module.
-    void addBuiltInFunction(std::string name,
+    void addTableFunction(std::string name,
         std::vector<std::unique_ptr<function::Function>> functionSet);
 
     KUZU_API void registerFileSystem(std::unique_ptr<common::FileSystem> fs);
 
     KUZU_API void registerStorageExtension(std::string name,
         std::unique_ptr<storage::StorageExtension> storageExtension);
```

### sdist/kuzu-source/src/include/storage/store/column_chunk.h

```diff
@@ -113,16 +113,14 @@
     virtual bool sanityCheck();
 
 protected:
     // Initializes the data buffer. Is (and should be) only called in constructor.
     void initializeBuffer(common::offset_t capacity);
     void initializeFunction();
 
-    common::offset_t getOffsetInBuffer(common::offset_t pos) const;
-
     virtual void copyVectorToBuffer(common::ValueVector* vector, common::offset_t startPosInChunk,
         const common::SelectionVector& selVector);
 
 private:
     uint64_t getBufferSize(uint64_t capacity_) const;
 
 protected:
```

### sdist/kuzu-source/src/include/storage/store/rel_table_data.h

```diff
@@ -3,16 +3,14 @@
 #include "common/enums/rel_direction.h"
 #include "storage/store/chunked_node_group.h"
 #include "storage/store/table_data.h"
 
 namespace kuzu {
 namespace storage {
 
-using density_range_t = std::pair<double, double>;
-
 class LocalRelNG;
 struct RelDataReadState : public TableDataReadState {
     common::RelDataDirection direction;
     common::offset_t startNodeOffset;
     common::offset_t numNodes;
     common::offset_t currentNodeOffset;
     common::offset_t posInCurrentCSR;
@@ -250,18 +248,14 @@
             offsets[i] = i + startOffset;
         }
     }
 
     common::offset_t findCSROffsetInRegion(const PersistentState& persistentState,
         common::offset_t nodeOffset, common::offset_t relOffset) const;
 
-    static inline common::vector_idx_t getDataIdxFromDirection(common::RelDataDirection direction) {
-        return direction == common::RelDataDirection::FWD ? 0 : 1;
-    }
-
 private:
     PackedCSRInfo packedCSRInfo;
     CSRHeaderColumns csrHeaderColumns;
     common::RelDataDirection direction;
     common::RelMultiplicity multiplicity;
 };
```

### sdist/kuzu-source/src/main/client_context.cpp

```diff
@@ -462,15 +462,16 @@
     queryResult->querySummary->executionTime = executingTimer.getElapsedTimeMS();
     queryResult->initResultTableAndIterator(std::move(resultFT),
         preparedStatement->statementResult->getColumns());
     return queryResult;
 }
 
 void ClientContext::addScalarFunction(std::string name, function::function_set definitions) {
-    database->catalog->addFunction(std::move(name), std::move(definitions));
+    database->catalog->addFunction(CatalogEntryType::SCALAR_FUNCTION_ENTRY, std::move(name),
+        std::move(definitions));
 }
 
 bool ClientContext::startUDFAutoTrx(transaction::TransactionContext* trx) {
     if (!trx->hasActiveTransaction()) {
         auto res = query("BEGIN TRANSACTION");
         KU_ASSERT(res->isSuccess());
         return true;
```

### sdist/kuzu-source/src/main/database.cpp

```diff
@@ -103,16 +103,17 @@
     bufferManager->clearEvictionQueue();
 }
 
 void Database::setLoggingLevel(std::string loggingLevel) {
     spdlog::set_level(LoggingLevelUtils::convertStrToLevelEnum(std::move(loggingLevel)));
 }
 
-void Database::addBuiltInFunction(std::string name, function::function_set functionSet) {
-    catalog->addBuiltInFunction(std::move(name), std::move(functionSet));
+void Database::addTableFunction(std::string name, function::function_set functionSet) {
+    catalog->addBuiltInFunction(CatalogEntryType::TABLE_FUNCTION_ENTRY, std::move(name),
+        std::move(functionSet));
 }
 
 void Database::registerFileSystem(std::unique_ptr<common::FileSystem> fs) {
     vfs->registerFileSystem(std::move(fs));
 }
 
 void Database::registerStorageExtension(std::string name,
```

### sdist/kuzu-source/src/processor/operator/persistent/reader/csv/driver.cpp

```diff
@@ -90,15 +90,15 @@
 
 void SniffCSVNameAndTypeDriver::addValue(uint64_t, common::column_id_t, std::string_view value) {
     std::string columnName(value);
     LogicalType columnType(LogicalTypeID::STRING);
     auto it = value.rfind(':');
     if (it != std::string_view::npos) {
         try {
-            columnType = LogicalTypeUtils::dataTypeFromString(std::string(value.substr(it + 1)));
+            columnType = LogicalType::fromString(std::string(value.substr(it + 1)));
             columnName = std::string(value.substr(0, it));
         } catch (const Exception&) { // NOLINT(bugprone-empty-catch):
                                      // This is how we check for a suitable
                                      // datatype name.
             // Didn't parse, just use the whole name.
         }
     }
```

### sdist/kuzu-source/src/processor/operator/persistent/rel_batch_insert.cpp

```diff
@@ -67,14 +67,15 @@
             relInfo.tableEntry->getName(), std::to_string(invalid.value() + startNodeOffset),
             RelDataDirectionUtils::relDirectionToString(relInfo.direction)));
     }
     // Resize csr data column chunks.
     offset_t csrChunkCapacity =
         csrHeader.getEndCSROffset(numNodes - 1) + csrHeader.getCSRLength(numNodes - 1);
     localState.nodeGroup->resizeChunks(csrChunkCapacity);
+    localState.nodeGroup->setAllNull();
     for (auto& chunkedGroup : partition.getChunkedGroups()) {
         auto& offsetChunk = chunkedGroup->getColumnChunkUnsafe(relInfo.offsetColumnID);
         setOffsetFromCSROffsets(offsetChunk, *csrHeader.offset);
     }
     populateEndCSROffsets(csrHeader, gaps);
 }
```

### sdist/kuzu-source/src/storage/store/column.cpp

```diff
@@ -894,63 +894,53 @@
     return nullChunkCollection;
 }
 
 std::unique_ptr<Column> ColumnFactory::createColumn(std::string name, LogicalType dataType,
     const MetadataDAHInfo& metaDAHeaderInfo, BMFileHandle* dataFH, BMFileHandle* metadataFH,
     BufferManager* bufferManager, WAL* wal, transaction::Transaction* transaction,
     RWPropertyStats propertyStatistics, bool enableCompression) {
-    switch (dataType.getLogicalTypeID()) {
-    case LogicalTypeID::BOOL:
-    case LogicalTypeID::INT64:
-    case LogicalTypeID::INT32:
-    case LogicalTypeID::INT16:
-    case LogicalTypeID::INT8:
-    case LogicalTypeID::UINT64:
-    case LogicalTypeID::UINT32:
-    case LogicalTypeID::UINT16:
-    case LogicalTypeID::UINT8:
-    case LogicalTypeID::INT128:
-    case LogicalTypeID::UUID:
-    case LogicalTypeID::DOUBLE:
-    case LogicalTypeID::FLOAT:
-    case LogicalTypeID::DATE:
-    case LogicalTypeID::TIMESTAMP:
-    case LogicalTypeID::TIMESTAMP_MS:
-    case LogicalTypeID::TIMESTAMP_NS:
-    case LogicalTypeID::TIMESTAMP_SEC:
-    case LogicalTypeID::TIMESTAMP_TZ:
-    case LogicalTypeID::INTERVAL: {
-        return std::make_unique<Column>(name, std::move(dataType), metaDAHeaderInfo, dataFH,
-            metadataFH, bufferManager, wal, transaction, propertyStatistics, enableCompression);
+    switch (dataType.getPhysicalType()) {
+    case PhysicalTypeID::BOOL:
+    case PhysicalTypeID::INT64:
+    case PhysicalTypeID::INT32:
+    case PhysicalTypeID::INT16:
+    case PhysicalTypeID::INT8:
+    case PhysicalTypeID::UINT64:
+    case PhysicalTypeID::UINT32:
+    case PhysicalTypeID::UINT16:
+    case PhysicalTypeID::UINT8:
+    case PhysicalTypeID::INT128:
+    case PhysicalTypeID::DOUBLE:
+    case PhysicalTypeID::FLOAT:
+    case PhysicalTypeID::INTERVAL: {
+        if (dataType.getLogicalTypeID() == LogicalTypeID::SERIAL) {
+            return std::make_unique<SerialColumn>(name, metaDAHeaderInfo, dataFH, metadataFH,
+                bufferManager, wal, transaction);
+        } else {
+            return std::make_unique<Column>(name, std::move(dataType), metaDAHeaderInfo, dataFH,
+                metadataFH, bufferManager, wal, transaction, propertyStatistics, enableCompression);
+        }
     }
-    case LogicalTypeID::INTERNAL_ID: {
+    case PhysicalTypeID::INTERNAL_ID: {
         return std::make_unique<InternalIDColumn>(name, metaDAHeaderInfo, dataFH, metadataFH,
             bufferManager, wal, transaction, propertyStatistics, enableCompression);
     }
-    case LogicalTypeID::BLOB:
-    case LogicalTypeID::STRING: {
+    case PhysicalTypeID::STRING: {
         return std::make_unique<StringColumn>(name, std::move(dataType), metaDAHeaderInfo, dataFH,
             metadataFH, bufferManager, wal, transaction, propertyStatistics, enableCompression);
     }
-    case LogicalTypeID::ARRAY:
-    case LogicalTypeID::MAP:
-    case LogicalTypeID::LIST: {
+    case PhysicalTypeID::ARRAY:
+    case PhysicalTypeID::LIST: {
         return std::make_unique<ListColumn>(name, std::move(dataType), metaDAHeaderInfo, dataFH,
             metadataFH, bufferManager, wal, transaction, propertyStatistics, enableCompression);
     }
-    case LogicalTypeID::UNION:
-    case LogicalTypeID::STRUCT:
-    case LogicalTypeID::RDF_VARIANT: {
+    case PhysicalTypeID::STRUCT: {
         return std::make_unique<StructColumn>(name, std::move(dataType), metaDAHeaderInfo, dataFH,
             metadataFH, bufferManager, wal, transaction, propertyStatistics, enableCompression);
     }
-    case LogicalTypeID::SERIAL: {
-        return std::make_unique<SerialColumn>(name, metaDAHeaderInfo, dataFH, metadataFH,
-            bufferManager, wal, transaction);
-    }
     default: {
         KU_UNREACHABLE;
     }
     }
 }
 
 } // namespace storage
```

### sdist/kuzu-source/src/storage/store/column_chunk.cpp

```diff
@@ -1,15 +1,14 @@
 #include "storage/store/column_chunk.h"
 
 #include "common/data_chunk/sel_vector.h"
 #include "common/exception/copy.h"
 #include "common/types/internal_id_t.h"
 #include "common/types/types.h"
 #include "storage/compression/compression.h"
-#include "storage/storage_utils.h"
 #include "storage/store/list_column_chunk.h"
 #include "storage/store/string_column_chunk.h"
 #include "storage/store/struct_column_chunk.h"
 
 using namespace kuzu::common;
 
 namespace kuzu {
@@ -337,24 +336,14 @@
             std::min(DEFAULT_VECTOR_CAPACITY, numValuesToPopulate - numValuesAppended);
         defaultValueVector->state->selVector->selectedSize = numValuesToAppend;
         append(defaultValueVector, *defaultValueVector->state->selVector);
         numValuesAppended += numValuesToAppend;
     }
 }
 
-offset_t ColumnChunk::getOffsetInBuffer(offset_t pos) const {
-    auto numElementsInAPage =
-        PageUtils::getNumElementsInAPage(numBytesPerValue, false /* hasNull */);
-    auto posCursor = PageUtils::getPageCursorForPos(pos, numElementsInAPage);
-    auto offsetInBuffer = posCursor.pageIdx * BufferPoolConstants::PAGE_4KB_SIZE +
-                          posCursor.elemPosInPage * numBytesPerValue;
-    KU_ASSERT(offsetInBuffer + numBytesPerValue <= bufferSize);
-    return offsetInBuffer;
-}
-
 void ColumnChunk::copyVectorToBuffer(ValueVector* vector, offset_t startPosInChunk,
     const SelectionVector& selVector) {
     auto bufferToWrite = buffer.get() + startPosInChunk * numBytesPerValue;
     KU_ASSERT(startPosInChunk + selVector.selectedSize <= capacity);
     auto vectorDataToWriteFrom = vector->getData();
     if (selVector.isUnfiltered()) {
         memcpy(bufferToWrite, vectorDataToWriteFrom, selVector.selectedSize * numBytesPerValue);
@@ -609,15 +598,14 @@
         }
     }
 
 private:
     common::table_id_t commonTableID;
 };
 
-// TODO(Guodong): Change the input param `dataType` to PhysicalType.
 std::unique_ptr<ColumnChunk> ColumnChunkFactory::createColumnChunk(LogicalType dataType,
     bool enableCompression, uint64_t capacity, bool inMemory) {
     switch (dataType.getPhysicalType()) {
     case PhysicalTypeID::BOOL: {
         return std::make_unique<BoolColumnChunk>(capacity, enableCompression);
     }
     case PhysicalTypeID::INT64:
```

### sdist/kuzu-source/src/storage/store/string_column_chunk.cpp

```diff
@@ -80,44 +80,46 @@
 }
 
 void StringColumnChunk::write(ColumnChunk* chunk, ColumnChunk* dstOffsets,
     RelMultiplicity /*multiplicity*/) {
     KU_ASSERT(chunk->getDataType().getPhysicalType() == PhysicalTypeID::STRING &&
               dstOffsets->getDataType().getPhysicalType() == PhysicalTypeID::INTERNAL_ID &&
               chunk->getNumValues() == dstOffsets->getNumValues());
+    auto stringChunk = ku_dynamic_cast<ColumnChunk*, StringColumnChunk*>(chunk);
     for (auto i = 0u; i < chunk->getNumValues(); i++) {
         auto offsetInChunk = dstOffsets->getValue<offset_t>(i);
         if (!needFinalize && offsetInChunk < numValues) [[unlikely]] {
             needFinalize = true;
         }
-        nullChunk->setNull(offsetInChunk, chunk->getNullChunk()->isNull(i));
+        bool isNull = chunk->getNullChunk()->isNull(i);
+        nullChunk->setNull(offsetInChunk, isNull);
         if (offsetInChunk >= numValues) {
             numValues = offsetInChunk + 1;
         }
-        if (!chunk->getNullChunk()->isNull(i)) {
-            auto stringChunk = ku_dynamic_cast<ColumnChunk*, StringColumnChunk*>(chunk);
+        if (!isNull) {
             setValueFromString(stringChunk->getValue<std::string_view>(i), offsetInChunk);
         }
     }
 }
 
 void StringColumnChunk::write(ColumnChunk* srcChunk, offset_t srcOffsetInChunk,
     offset_t dstOffsetInChunk, offset_t numValuesToCopy) {
     KU_ASSERT(srcChunk->getDataType().getPhysicalType() == PhysicalTypeID::STRING);
     if ((dstOffsetInChunk + numValuesToCopy) >= numValues) {
         numValues = dstOffsetInChunk + numValuesToCopy;
     }
+    auto srcStringChunk = ku_dynamic_cast<ColumnChunk*, StringColumnChunk*>(srcChunk);
     for (auto i = 0u; i < numValuesToCopy; i++) {
         auto srcPos = srcOffsetInChunk + i;
         auto dstPos = dstOffsetInChunk + i;
-        nullChunk->setNull(dstPos, srcChunk->getNullChunk()->isNull(srcPos));
-        if (srcChunk->getNullChunk()->isNull(srcPos)) {
+        bool isNull = srcChunk->getNullChunk()->isNull(srcPos);
+        nullChunk->setNull(dstPos, isNull);
+        if (isNull) {
             continue;
         }
-        auto srcStringChunk = ku_dynamic_cast<ColumnChunk*, StringColumnChunk*>(srcChunk);
         setValueFromString(srcStringChunk->getValue<std::string_view>(srcPos), dstPos);
     }
 }
 
 void StringColumnChunk::copy(ColumnChunk* srcChunk, offset_t srcOffsetInChunk,
     offset_t dstOffsetInChunk, offset_t numValuesToCopy) {
     KU_ASSERT(srcChunk->getDataType().getPhysicalType() == PhysicalTypeID::STRING);
```

### sdist/kuzu-source/src/storage/wal/wal.cpp

```diff
@@ -1,16 +1,18 @@
 #include "storage/wal/wal.h"
 
 #include <fcntl.h>
 
+#include "common/exception/io.h"
 #include "common/file_system/file_info.h"
 #include "common/file_system/virtual_file_system.h"
 #include "common/serializer/buffered_file.h"
 #include "common/serializer/deserializer.h"
 #include "common/serializer/serializer.h"
+#include "spdlog/spdlog.h"
 #include "storage/storage_utils.h"
 
 using namespace kuzu::common;
 
 namespace kuzu {
 namespace storage {
 
@@ -27,15 +29,19 @@
         readOnly ? FileHandle::O_PERSISTENT_FILE_READ_ONLY :
                    FileHandle::O_PERSISTENT_FILE_CREATE_NOT_EXISTS,
         BMFileHandle::FileVersionedType::NON_VERSIONED_FILE, vfs);
     initialize();
 }
 
 WAL::~WAL() {
-    flushAllPages();
+    try {
+        flushAllPages();
+    } catch (IOException& e) {
+        spdlog::error("Failed to flush WAL: {}", e.what());
+    }
 }
 
 page_idx_t WAL::logPageUpdateRecord(DBFileID dbFileID, page_idx_t pageIdxInOriginalFile) {
     lock_t lck{mtx};
     auto pageIdxInWAL = shadowingFH->addNewPage();
     PageUpdateOrInsertRecord walRecord(dbFileID, pageIdxInOriginalFile, pageIdxInWAL,
         false /*isInsert*/);
@@ -132,15 +138,15 @@
     StorageUtils::removeAllWALFiles(directory);
     updatedTables.clear();
 }
 
 void WAL::flushAllPages() {
     bufferedWriter->flush();
     bufferManager.flushAllDirtyPagesInFrames(*shadowingFH);
-    // TODO: Should sync as well.
+    bufferedWriter->getFileInfo().syncFile();
 }
 
 bool WAL::isEmptyWAL() const {
     return isEmpty;
 }
 
 void WAL::initialize() {
```

### sdist/kuzu-source/tools/python_api/src_cpp/py_database.cpp

```diff
@@ -44,15 +44,15 @@
 }
 
 PyDatabase::PyDatabase(const std::string& databasePath, uint64_t bufferPoolSize,
     uint64_t maxNumThreads, bool compression, bool readOnly, uint64_t maxDBSize) {
     auto systemConfig =
         SystemConfig(bufferPoolSize, maxNumThreads, compression, readOnly, maxDBSize);
     database = std::make_unique<Database>(databasePath, systemConfig);
-    database->addBuiltInFunction(kuzu::PandasScanFunction::name,
+    database->addTableFunction(kuzu::PandasScanFunction::name,
         kuzu::PandasScanFunction::getFunctionSet());
     storageDriver = std::make_unique<kuzu::main::StorageDriver>(database.get());
     py::gil_scoped_acquire acquire;
     if (kuzu::importCache.get() == nullptr) {
         kuzu::importCache = std::make_shared<kuzu::PythonCachedImport>();
     }
 }
```

### sdist/kuzu-source/tools/python_api/src_py/query_result.py

```diff
@@ -285,15 +285,15 @@
 
                 elif column_type == Type.RECURSIVE_REL.value:
                     for node in row[i]["_nodes"]:
                         _id = node["_id"]
                         nodes[(_id["table"], _id["offset"])] = node
                         table_to_label_dict[_id["table"]] = node["_label"]
                     for rel in row[i]["_rels"]:
-                        for key in rel:
+                        for key in list(rel.keys()):
                             if rel[key] is None:
                                 del rel[key]
                         _src = rel["_src"]
                         _dst = rel["_dst"]
                         rels[(_src["table"], _src["offset"], _dst["table"], _dst["offset"])] = rel
 
         # Add nodes
```

### sdist/kuzu-source/tools/rust_api/src/database.rs

```diff
@@ -154,17 +154,16 @@
         )?;
         temp_dir.close()?;
         Ok(())
     }
 
     #[test]
     fn create_database_failure() {
-        let result: Error = Database::new("", SystemConfig::default())
-            .expect_err("An empty string should not be a valid database path!")
-            .into();
+        Database::new("", SystemConfig::default())
+            .expect_err("An empty string should not be a valid database path!");
     }
 
     #[test]
     fn test_database_read_only() -> Result<()> {
         let temp_dir = tempfile::tempdir()?;
         // Create database first so that it can be opened read-only
         {
```

### sdist/kuzu.egg-info/PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuzu
-Version: 0.3.3.dev35
+Version: 0.3.3.dev36
 Summary: An in-process property graph database management system built for query speed and scalability.
 Home-page: https://github.com/kuzudb/kuzu
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kuzu Version: 0.3.3.dev35 Summary: An in-process
+Metadata-Version: 2.1 Name: kuzu Version: 0.3.3.dev36 Summary: An in-process
 property graph database management system built for query speed and
 scalability. Home-page: https://github.com/kuzudb/kuzu License: MIT Platform:
 UNKNOWN Description-Content-Type: text/markdown License-File: LICENSE
                     [https://kuzudb.com/img/kuzu-logo.png]
 
   _[_G_i_t_h_u_b_ _A_c_t_i_o_n_s_ _B_a_d_g_e_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_i_t_h_u_b_/_k_u_z_u_d_b_/_k_u_z_u_/_b_r_a_n_c_h_/_m_a_s_t_e_r_/
               _g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_N_1_A_T_6_H_7_9_L_M_]_[_d_i_s_c_o_r_d_]_[_t_w_i_t_t_e_r_]
```

### sdist/pyproject.toml

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "kuzu"
 description = "Highly scalable, extremely fast, easy-to-use embeddable graph database"
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = ["graph", "database"]
-version = "0.3.3.dev35"
+version = "0.3.3.dev36"
 
 [project.urls]
 Homepage = "https://kuzudb.com/"
 Documentation = "https://docs.kuzudb.com/"
 Repository = "https://github.com/kuzudb/kuzu"
 Changelog = "https://github.com/kuzudb/kuzu/releases"
```

