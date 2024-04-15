# Comparing `tmp/evm-trace-0.1.3.tar.gz` & `tmp/evm-trace-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evm-trace-0.1.3.tar", last modified: Tue Apr  9 17:42:28 2024, max compression
+gzip compressed data, was "evm-trace-0.1.4.tar", last modified: Mon Apr 15 18:39:58 2024, max compression
```

## Comparing `evm-trace-0.1.3.tar` & `evm-trace-0.1.4.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:28.680019 evm-trace-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:28.668018 evm-trace-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:28.668018 evm-trace-0.1.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-09 17:42:07.000000 evm-trace-0.1.3/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-09 17:42:07.000000 evm-trace-0.1.3/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-09 17:42:07.000000 evm-trace-0.1.3/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-09 17:42:07.000000 evm-trace-0.1.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-09 17:42:07.000000 evm-trace-0.1.3/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:28.668018 evm-trace-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-09 17:42:07.000000 evm-trace-0.1.3/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-09 17:42:07.000000 evm-trace-0.1.3/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-09 17:42:07.000000 evm-trace-0.1.3/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-09 17:42:07.000000 evm-trace-0.1.3/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-09 17:42:07.000000 evm-trace-0.1.3/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-09 17:42:07.000000 evm-trace-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-09 17:42:07.000000 evm-trace-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-09 17:42:07.000000 evm-trace-0.1.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-09 17:42:07.000000 evm-trace-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-09 17:42:28.680019 evm-trace-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-09 17:42:07.000000 evm-trace-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:28.672019 evm-trace-0.1.3/evm_trace/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-09 17:42:07.000000 evm-trace-0.1.3/evm_trace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-04-09 17:42:07.000000 evm-trace-0.1.3/evm_trace/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-09 17:42:07.000000 evm-trace-0.1.3/evm_trace/display.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-09 17:42:07.000000 evm-trace-0.1.3/evm_trace/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-09 17:42:07.000000 evm-trace-0.1.3/evm_trace/gas.py
--rw-r--r--   0 runner    (1001) docker     (127)    11888 2024-04-09 17:42:07.000000 evm-trace-0.1.3/evm_trace/geth.py
--rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-04-09 17:42:07.000000 evm-trace-0.1.3/evm_trace/parity.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:07.000000 evm-trace-0.1.3/evm_trace/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-09 17:42:28.000000 evm-trace-0.1.3/evm_trace/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-04-09 17:42:07.000000 evm-trace-0.1.3/evm_trace/vmtrace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:28.672019 evm-trace-0.1.3/evm_trace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-09 17:42:28.000000 evm-trace-0.1.3/evm_trace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-09 17:42:28.000000 evm-trace-0.1.3/evm_trace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:42:28.000000 evm-trace-0.1.3/evm_trace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:42:28.000000 evm-trace-0.1.3/evm_trace.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-09 17:42:28.000000 evm-trace-0.1.3/evm_trace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 17:42:28.000000 evm-trace-0.1.3/evm_trace.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-09 17:42:07.000000 evm-trace-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-09 17:42:28.680019 evm-trace-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-04-09 17:42:07.000000 evm-trace-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:28.672019 evm-trace-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:28.668018 evm-trace-0.1.3/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:28.672019 evm-trace-0.1.3/tests/data/evm_trace/
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/data/evm_trace/call.json
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/data/evm_trace/delegate_call.json
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/data/evm_trace/frame.json
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/data/evm_trace/mutable_call.json
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/data/evm_trace/static_call.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:28.680019 evm-trace-0.1.3/tests/data/geth/
--rw-r--r--   0 runner    (1001) docker     (127)    11527 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/data/geth/call.json
--rw-r--r--   0 runner    (1001) docker     (127)  3934899 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/data/geth/create2_structlogs.json
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/data/geth/create_call.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:28.680019 evm-trace-0.1.3/tests/data/parity/
--rw-r--r--   0 runner    (1001) docker     (127)   137258 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/data/parity/call.json
--rw-r--r--   0 runner    (1001) docker     (127)     7878 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/data/parity/create.json
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/data/parity/create2.json
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/data/parity/create_revert.json
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/data/parity/error.json
--rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/data/parity/revert.json
--rw-r--r--   0 runner    (1001) docker     (127)    10608 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/data/parity/revert_with_message.json
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/data/parity/selfdestruct.json
--rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/expected_traces.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/test_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/test_gas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6539 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/test_geth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/test_parity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:39:58.971319 evm-trace-0.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:39:58.959319 evm-trace-0.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:39:58.959319 evm-trace-0.1.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-15 18:39:39.000000 evm-trace-0.1.4/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-15 18:39:39.000000 evm-trace-0.1.4/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-15 18:39:39.000000 evm-trace-0.1.4/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-15 18:39:39.000000 evm-trace-0.1.4/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-15 18:39:39.000000 evm-trace-0.1.4/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:39:58.959319 evm-trace-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-15 18:39:39.000000 evm-trace-0.1.4/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-15 18:39:39.000000 evm-trace-0.1.4/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-15 18:39:39.000000 evm-trace-0.1.4/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-15 18:39:39.000000 evm-trace-0.1.4/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-15 18:39:39.000000 evm-trace-0.1.4/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-15 18:39:39.000000 evm-trace-0.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-15 18:39:39.000000 evm-trace-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-15 18:39:39.000000 evm-trace-0.1.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-15 18:39:39.000000 evm-trace-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-15 18:39:58.971319 evm-trace-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-15 18:39:39.000000 evm-trace-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:39:58.963319 evm-trace-0.1.4/evm_trace/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-15 18:39:39.000000 evm-trace-0.1.4/evm_trace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-04-15 18:39:39.000000 evm-trace-0.1.4/evm_trace/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-15 18:39:39.000000 evm-trace-0.1.4/evm_trace/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-15 18:39:39.000000 evm-trace-0.1.4/evm_trace/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-15 18:39:39.000000 evm-trace-0.1.4/evm_trace/gas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11888 2024-04-15 18:39:39.000000 evm-trace-0.1.4/evm_trace/geth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-04-15 18:39:39.000000 evm-trace-0.1.4/evm_trace/parity.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 18:39:39.000000 evm-trace-0.1.4/evm_trace/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-15 18:39:58.000000 evm-trace-0.1.4/evm_trace/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-04-15 18:39:39.000000 evm-trace-0.1.4/evm_trace/vmtrace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:39:58.963319 evm-trace-0.1.4/evm_trace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-15 18:39:58.000000 evm-trace-0.1.4/evm_trace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-15 18:39:58.000000 evm-trace-0.1.4/evm_trace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 18:39:58.000000 evm-trace-0.1.4/evm_trace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 18:39:58.000000 evm-trace-0.1.4/evm_trace.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-15 18:39:58.000000 evm-trace-0.1.4/evm_trace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-15 18:39:58.000000 evm-trace-0.1.4/evm_trace.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-15 18:39:39.000000 evm-trace-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-15 18:39:58.971319 evm-trace-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-04-15 18:39:39.000000 evm-trace-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:39:58.963319 evm-trace-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 18:39:39.000000 evm-trace-0.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-15 18:39:39.000000 evm-trace-0.1.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:39:58.959319 evm-trace-0.1.4/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:39:58.963319 evm-trace-0.1.4/tests/data/evm_trace/
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-15 18:39:39.000000 evm-trace-0.1.4/tests/data/evm_trace/call.json
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-15 18:39:39.000000 evm-trace-0.1.4/tests/data/evm_trace/delegate_call.json
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-15 18:39:39.000000 evm-trace-0.1.4/tests/data/evm_trace/frame.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-04-15 18:39:39.000000 evm-trace-0.1.4/tests/data/evm_trace/mutable_call.json
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-15 18:39:39.000000 evm-trace-0.1.4/tests/data/evm_trace/static_call.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:39:58.967319 evm-trace-0.1.4/tests/data/geth/
+-rw-r--r--   0 runner    (1001) docker     (127)    11527 2024-04-15 18:39:39.000000 evm-trace-0.1.4/tests/data/geth/call.json
+-rw-r--r--   0 runner    (1001) docker     (127)  3934899 2024-04-15 18:39:39.000000 evm-trace-0.1.4/tests/data/geth/create2_structlogs.json
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-15 18:39:39.000000 evm-trace-0.1.4/tests/data/geth/create_call.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:39:58.971319 evm-trace-0.1.4/tests/data/parity/
+-rw-r--r--   0 runner    (1001) docker     (127)   137258 2024-04-15 18:39:39.000000 evm-trace-0.1.4/tests/data/parity/call.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7878 2024-04-15 18:39:39.000000 evm-trace-0.1.4/tests/data/parity/create.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-15 18:39:39.000000 evm-trace-0.1.4/tests/data/parity/create2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-15 18:39:39.000000 evm-trace-0.1.4/tests/data/parity/create_revert.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-15 18:39:39.000000 evm-trace-0.1.4/tests/data/parity/error.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-04-15 18:39:39.000000 evm-trace-0.1.4/tests/data/parity/revert.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10608 2024-04-15 18:39:39.000000 evm-trace-0.1.4/tests/data/parity/revert_with_message.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-15 18:39:39.000000 evm-trace-0.1.4/tests/data/parity/selfdestruct.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-04-15 18:39:39.000000 evm-trace-0.1.4/tests/expected_traces.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-15 18:39:39.000000 evm-trace-0.1.4/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-15 18:39:39.000000 evm-trace-0.1.4/tests/test_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-15 18:39:39.000000 evm-trace-0.1.4/tests/test_gas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6539 2024-04-15 18:39:39.000000 evm-trace-0.1.4/tests/test_geth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-15 18:39:39.000000 evm-trace-0.1.4/tests/test_parity.py
```

### Comparing `evm-trace-0.1.3/.github/ISSUE_TEMPLATE/bug.md` & `evm-trace-0.1.4/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/.github/ISSUE_TEMPLATE/feature.md` & `evm-trace-0.1.4/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/.github/ISSUE_TEMPLATE/work-item.md` & `evm-trace-0.1.4/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/.github/release-drafter.yml` & `evm-trace-0.1.4/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/.github/workflows/commitlint.yaml` & `evm-trace-0.1.4/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/.github/workflows/prtitle.yaml` & `evm-trace-0.1.4/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/.github/workflows/publish.yaml` & `evm-trace-0.1.4/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/.github/workflows/test.yaml` & `evm-trace-0.1.4/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/.gitignore` & `evm-trace-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/.pre-commit-config.yaml` & `evm-trace-0.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/CONTRIBUTING.md` & `evm-trace-0.1.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/LICENSE` & `evm-trace-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/PKG-INFO` & `evm-trace-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evm-trace
-Version: 0.1.3
+Version: 0.1.4
 Summary: evm-trace: Ethereum Virtual Machine transaction tracing tool
 Home-page: https://github.com/ApeWorX/evm-trace
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `evm-trace-0.1.3/README.md` & `evm-trace-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/evm_trace/__init__.py` & `evm-trace-0.1.4/evm_trace/__init__.py`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/evm_trace/base.py` & `evm-trace-0.1.4/evm_trace/base.py`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/evm_trace/display.py` & `evm-trace-0.1.4/evm_trace/display.py`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/evm_trace/enums.py` & `evm-trace-0.1.4/evm_trace/enums.py`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/evm_trace/gas.py` & `evm-trace-0.1.4/evm_trace/gas.py`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/evm_trace/geth.py` & `evm-trace-0.1.4/evm_trace/geth.py`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/evm_trace/parity.py` & `evm-trace-0.1.4/evm_trace/parity.py`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/evm_trace/vmtrace.py` & `evm-trace-0.1.4/evm_trace/vmtrace.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,21 +129,21 @@
 
         # geth convention is to return after memory expansion, but before the operation is applied
         yield VMTraceFrame(
             address=address,
             pc=op.pc,
             op=op.op,
             depth=depth,
-            stack=[to_int(val) for _, val in stack.values],
+            stack=[to_int(val) for val in stack.values],
             memory=read_memory(0, len(memory)),
             storage=storage.copy(),
         )
 
         if op.op in ["CALL", "DELEGATECALL", "STATICCALL"]:
-            call_address = Address.__eth_pydantic_validate__(stack.values[-2][1])
+            call_address = Address.__eth_pydantic_validate__(stack.values[-2])
 
         if op.ex:
             if op.ex.mem:
                 memory.write(op.ex.mem.off, len(op.ex.mem.data), op.ex.mem.data)
 
             num_pop = POPCODES.get(op.op)
             if num_pop:
```

### Comparing `evm-trace-0.1.3/evm_trace.egg-info/PKG-INFO` & `evm-trace-0.1.4/evm_trace.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evm-trace
-Version: 0.1.3
+Version: 0.1.4
 Summary: evm-trace: Ethereum Virtual Machine transaction tracing tool
 Home-page: https://github.com/ApeWorX/evm-trace
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `evm-trace-0.1.3/evm_trace.egg-info/SOURCES.txt` & `evm-trace-0.1.4/evm_trace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/evm_trace.egg-info/requires.txt` & `evm-trace-0.1.4/evm_trace.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 pydantic<3,>=2.5.2
-py-evm<0.9,>=0.7.0a4
+py-evm<0.11,>=0.10.0b6
 eth-utils<3,>=2.3.1
 msgspec>=0.8
 eth-pydantic-types>=0.1.0a5
 
 [dev]
 pytest>=6.0
 pytest-xdist
```

### Comparing `evm-trace-0.1.3/pyproject.toml` & `evm-trace-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/setup.py` & `evm-trace-0.1.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/evm-trace",
     include_package_data=True,
     install_requires=[
         "pydantic>=2.5.2,<3",
-        "py-evm>=0.7.0a4,<0.9",  # NOTE: We support both 0.7 and 0.8.
+        "py-evm>=0.10.0b6,<0.11",
         "eth-utils>=2.3.1,<3",
         "msgspec>=0.8",
         "eth-pydantic-types>=0.1.0a5",
     ],
     python_requires=">=3.8,<4",
     extras_require=extras_require,
     py_modules=["evm_trace"],
```

### Comparing `evm-trace-0.1.3/tests/conftest.py` & `evm-trace-0.1.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/tests/data/evm_trace/call.json` & `evm-trace-0.1.4/tests/data/evm_trace/call.json`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/tests/data/evm_trace/frame.json` & `evm-trace-0.1.4/tests/data/evm_trace/frame.json`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/tests/data/evm_trace/mutable_call.json` & `evm-trace-0.1.4/tests/data/evm_trace/mutable_call.json`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/tests/data/geth/call.json` & `evm-trace-0.1.4/tests/data/geth/call.json`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/tests/data/geth/create2_structlogs.json` & `evm-trace-0.1.4/tests/data/geth/create2_structlogs.json`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/tests/data/geth/create_call.json` & `evm-trace-0.1.4/tests/data/geth/create_call.json`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/tests/data/parity/call.json` & `evm-trace-0.1.4/tests/data/parity/call.json`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/tests/data/parity/create.json` & `evm-trace-0.1.4/tests/data/parity/create.json`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/tests/data/parity/create2.json` & `evm-trace-0.1.4/tests/data/parity/create2.json`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/tests/data/parity/create_revert.json` & `evm-trace-0.1.4/tests/data/parity/create_revert.json`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/tests/data/parity/error.json` & `evm-trace-0.1.4/tests/data/parity/error.json`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/tests/data/parity/revert.json` & `evm-trace-0.1.4/tests/data/parity/revert.json`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/tests/data/parity/revert_with_message.json` & `evm-trace-0.1.4/tests/data/parity/revert_with_message.json`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/tests/data/parity/selfdestruct.json` & `evm-trace-0.1.4/tests/data/parity/selfdestruct.json`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/tests/expected_traces.py` & `evm-trace-0.1.4/tests/expected_traces.py`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/tests/test_base.py` & `evm-trace-0.1.4/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/tests/test_gas.py` & `evm-trace-0.1.4/tests/test_gas.py`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/tests/test_geth.py` & `evm-trace-0.1.4/tests/test_geth.py`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.3/tests/test_parity.py` & `evm-trace-0.1.4/tests/test_parity.py`

 * *Files identical despite different names*

