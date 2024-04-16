# Comparing `tmp/libbs-1.2.6.tar.gz` & `tmp/libbs-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libbs-1.2.6.tar", last modified: Wed Apr 10 19:42:13 2024, max compression
+gzip compressed data, was "libbs-1.2.7.tar", last modified: Tue Apr 16 20:08:02 2024, max compression
```

## Comparing `libbs-1.2.6.tar` & `libbs-1.2.7.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:42:13.669052 libbs-1.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-10 19:42:09.000000 libbs-1.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-10 19:42:13.669052 libbs-1.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-10 19:42:09.000000 libbs-1.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:42:13.653052 libbs-1.2.6/libbs/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:42:13.657052 libbs-1.2.6/libbs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/api/artifact_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/api/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)    26006 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/api/decompiler_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    13342 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/api/type_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:42:13.657052 libbs-1.2.6/libbs/artifacts/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/artifacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/artifacts/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/artifacts/comment.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/artifacts/decompilation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/artifacts/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/artifacts/func.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/artifacts/global_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/artifacts/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/artifacts/stack_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/artifacts/struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:42:13.657052 libbs-1.2.6/libbs/decompiler_stubs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/decompiler_stubs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:42:13.661052 libbs-1.2.6/libbs/decompiler_stubs/angr_libbs/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/decompiler_stubs/angr_libbs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:42:13.661052 libbs-1.2.6/libbs/decompiler_stubs/binja_libbs/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/decompiler_stubs/binja_libbs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:42:13.661052 libbs-1.2.6/libbs/decompiler_stubs/ghidra_libbs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/decompiler_stubs/ghidra_libbs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_mainthread_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_shutdown.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:42:13.661052 libbs-1.2.6/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:42:13.661052 libbs-1.2.6/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    89858 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/decompiler_stubs/ida_libbs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:42:13.661052 libbs-1.2.6/libbs/decompilers/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/decompilers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:42:13.661052 libbs-1.2.6/libbs/decompilers/angr/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/decompilers/angr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/decompilers/angr/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/decompilers/angr/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    16964 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/decompilers/angr/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:42:13.665052 libbs-1.2.6/libbs/decompilers/binja/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/decompilers/binja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/decompilers/binja/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/decompilers/binja/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    20930 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/decompilers/binja/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:42:13.665052 libbs-1.2.6/libbs/decompilers/ghidra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/decompilers/ghidra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/decompilers/ghidra/artifact_lifter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:42:13.665052 libbs-1.2.6/libbs/decompilers/ghidra/compat/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/decompilers/ghidra/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/decompilers/ghidra/compat/ghidra_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/decompilers/ghidra/compat/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/decompilers/ghidra/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    32838 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/decompilers/ghidra/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:42:13.665052 libbs-1.2.6/libbs/decompilers/ida/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/decompilers/ida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/decompilers/ida/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)    30603 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/decompilers/ida/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/decompilers/ida/hooks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12593 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/decompilers/ida/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/plugin_installer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:42:13.665052 libbs-1.2.6/libbs/ui/
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/ui/qt_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/ui/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-10 19:42:09.000000 libbs-1.2.6/libbs/ui/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:42:13.669052 libbs-1.2.6/libbs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-10 19:42:13.000000 libbs-1.2.6/libbs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-10 19:42:13.000000 libbs-1.2.6/libbs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:42:13.000000 libbs-1.2.6/libbs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-10 19:42:13.000000 libbs-1.2.6/libbs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-10 19:42:13.000000 libbs-1.2.6/libbs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 19:42:13.000000 libbs-1.2.6/libbs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-10 19:42:13.669052 libbs-1.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-10 19:42:09.000000 libbs-1.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:42:13.669052 libbs-1.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-04-10 19:42:09.000000 libbs-1.2.6/tests/test_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-10 19:42:09.000000 libbs-1.2.6/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5728 2024-04-10 19:42:09.000000 libbs-1.2.6/tests/test_decompilers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.582665 libbs-1.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-16 20:07:58.000000 libbs-1.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-16 20:08:02.582665 libbs-1.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-04-16 20:07:58.000000 libbs-1.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.566666 libbs-1.2.7/libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.570665 libbs-1.2.7/libbs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/api/artifact_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/api/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26006 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/api/decompiler_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13342 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/api/type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.574665 libbs-1.2.7/libbs/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/artifacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/artifacts/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/artifacts/comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/artifacts/decompilation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/artifacts/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/artifacts/func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/artifacts/global_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/artifacts/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/artifacts/stack_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/artifacts/struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.574665 libbs-1.2.7/libbs/decompiler_stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompiler_stubs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.574665 libbs-1.2.7/libbs/decompiler_stubs/angr_libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompiler_stubs/angr_libbs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.574665 libbs-1.2.7/libbs/decompiler_stubs/binja_libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompiler_stubs/binja_libbs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.574665 libbs-1.2.7/libbs/decompiler_stubs/ghidra_libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompiler_stubs/ghidra_libbs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_mainthread_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_shutdown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.574665 libbs-1.2.7/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.574665 libbs-1.2.7/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89858 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompiler_stubs/ida_libbs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.574665 libbs-1.2.7/libbs/decompilers/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.574665 libbs-1.2.7/libbs/decompilers/angr/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/angr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/angr/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/angr/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16964 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/angr/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.578665 libbs-1.2.7/libbs/decompilers/binja/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/binja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/binja/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/binja/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20930 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/binja/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.578665 libbs-1.2.7/libbs/decompilers/ghidra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/ghidra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/ghidra/artifact_lifter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.578665 libbs-1.2.7/libbs/decompilers/ghidra/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/ghidra/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/ghidra/compat/ghidra_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/ghidra/compat/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7705 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/ghidra/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32838 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/ghidra/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.578665 libbs-1.2.7/libbs/decompilers/ida/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/ida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/ida/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30603 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/ida/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/ida/hooks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12593 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/ida/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/plugin_installer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.578665 libbs-1.2.7/libbs/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/ui/qt_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/ui/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/ui/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.582665 libbs-1.2.7/libbs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-16 20:08:02.000000 libbs-1.2.7/libbs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-16 20:08:02.000000 libbs-1.2.7/libbs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 20:08:02.000000 libbs-1.2.7/libbs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-16 20:08:02.000000 libbs-1.2.7/libbs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-16 20:08:02.000000 libbs-1.2.7/libbs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 20:08:02.000000 libbs-1.2.7/libbs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-16 20:08:02.582665 libbs-1.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-16 20:07:58.000000 libbs-1.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.582665 libbs-1.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-04-16 20:07:58.000000 libbs-1.2.7/tests/test_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-16 20:07:58.000000 libbs-1.2.7/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5728 2024-04-16 20:07:58.000000 libbs-1.2.7/tests/test_decompilers.py
```

### Comparing `libbs-1.2.6/LICENSE` & `libbs-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/PKG-INFO` & `libbs-1.2.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: libbs
-Version: 1.2.6
+Version: 1.2.7
 Summary: Your Only Decompiler API Lib - A generic API to script in and out of decompilers
 Home-page: https://github.com/binsync/libbs
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: toml
 Requires-Dist: pycparser
 Requires-Dist: setuptools
 Requires-Dist: prompt_toolkit
@@ -30,14 +30,16 @@
 for all BinSync based plugins.
 
 ## Install
 ```bash
 pip install libbs
 ```
 
+The minimum Python version is **3.8**.
+
 You can optionally also do `libbs --install` after to install generic plugins, but it's not required, since `libbs` 
 files will be installed with plugins that use it. 
 
 ## Usage
 LibBS exposes all decompiler API through the abstract class `DecompilerInterface`. The `DecompilerInterface` 
 can be used in either the default mode, which assumes a GUI, or `headless` mode. In `headless` mode, the interface will 
 start a new process using a specified decompiler.
```

### Comparing `libbs-1.2.6/README.md` & `libbs-1.2.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 for all BinSync based plugins.
 
 ## Install
 ```bash
 pip install libbs
 ```
 
+The minimum Python version is **3.8**.
+
 You can optionally also do `libbs --install` after to install generic plugins, but it's not required, since `libbs` 
 files will be installed with plugins that use it. 
 
 ## Usage
 LibBS exposes all decompiler API through the abstract class `DecompilerInterface`. The `DecompilerInterface` 
 can be used in either the default mode, which assumes a GUI, or `headless` mode. In `headless` mode, the interface will 
 start a new process using a specified decompiler.
```

### Comparing `libbs-1.2.6/libbs/__main__.py` & `libbs-1.2.7/libbs/__main__.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/libbs/api/artifact_dict.py` & `libbs-1.2.7/libbs/api/artifact_dict.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/libbs/api/artifact_lifter.py` & `libbs-1.2.7/libbs/api/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/libbs/api/decompiler_interface.py` & `libbs-1.2.7/libbs/api/decompiler_interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/libbs/api/type_parser.py` & `libbs-1.2.7/libbs/api/type_parser.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/libbs/api/utils.py` & `libbs-1.2.7/libbs/api/utils.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/libbs/artifacts/artifact.py` & `libbs-1.2.7/libbs/artifacts/artifact.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/libbs/artifacts/comment.py` & `libbs-1.2.7/libbs/artifacts/comment.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/libbs/artifacts/decompilation.py` & `libbs-1.2.7/libbs/artifacts/decompilation.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/libbs/artifacts/enum.py` & `libbs-1.2.7/libbs/artifacts/enum.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/libbs/artifacts/func.py` & `libbs-1.2.7/libbs/artifacts/func.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/libbs/artifacts/global_variable.py` & `libbs-1.2.7/libbs/artifacts/global_variable.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/libbs/artifacts/patch.py` & `libbs-1.2.7/libbs/artifacts/patch.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/libbs/artifacts/stack_variable.py` & `libbs-1.2.7/libbs/artifacts/stack_variable.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/libbs/artifacts/struct.py` & `libbs-1.2.7/libbs/artifacts/struct.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py` & `libbs-1.2.7/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py` & `libbs-1.2.7/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/libbs/decompilers/angr/artifact_lifter.py` & `libbs-1.2.7/libbs/decompilers/angr/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/libbs/decompilers/angr/compat.py` & `libbs-1.2.7/libbs/decompilers/angr/compat.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/libbs/decompilers/angr/interface.py` & `libbs-1.2.7/libbs/decompilers/angr/interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/libbs/decompilers/binja/artifact_lifter.py` & `libbs-1.2.7/libbs/decompilers/binja/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/libbs/decompilers/binja/hooks.py` & `libbs-1.2.7/libbs/decompilers/binja/hooks.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/libbs/decompilers/binja/interface.py` & `libbs-1.2.7/libbs/decompilers/binja/interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/libbs/decompilers/ghidra/artifact_lifter.py` & `libbs-1.2.7/libbs/decompilers/ghidra/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/libbs/decompilers/ghidra/compat/ghidra_api.py` & `libbs-1.2.7/libbs/decompilers/ghidra/compat/ghidra_api.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/libbs/decompilers/ghidra/hooks.py` & `libbs-1.2.7/libbs/decompilers/ghidra/hooks.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,52 +11,58 @@
     model = ghidra.import_module("ghidra.framework.model")
     class DataMonitor(model.DomainObjectListener):
         def __init__(self, interface: "GhidraDecompilerInterface"):
             self._interface = interface
             self.changeManager = ghidra.import_module_object("ghidra.program.util", "ChangeManager")
             self.programChangeRecord = ghidra.import_module_object("ghidra.program.util", "ProgramChangeRecord")
             self.db = ghidra.import_module("ghidra.program.database")
-        def domainObjectChanged(self, ev):
-            funcEvents = [
+
+            # Init event lists
+            self.funcEvents = [
                 self.changeManager.DOCR_FUNCTION_CHANGED,
                 self.changeManager.DOCR_FUNCTION_BODY_CHANGED,
                 self.changeManager.DOCR_VARIABLE_REFERENCE_ADDED,
                 self.changeManager.DOCR_VARIABLE_REFERENCE_REMOVED
             ]
 
-            symDelEvents = [self.changeManager.DOCR_SYMBOL_REMOVED]
+            self.symDelEvents = [self.changeManager.DOCR_SYMBOL_REMOVED]
 
-            symChgEvents = [
+            self.symChgEvents = [
                 self.changeManager.DOCR_SYMBOL_ADDED,
                 self.changeManager.DOCR_SYMBOL_RENAMED,
                 self.changeManager.DOCR_SYMBOL_DATA_CHANGED
             ]
 
-            typeEvents = [
+            self.typeEvents = [
                 self.changeManager.DOCR_DATA_TYPE_CHANGED,
                 self.changeManager.DOCR_DATA_TYPE_REPLACED,
                 self.changeManager.DOCR_DATA_TYPE_RENAMED,
                 self.changeManager.DOCR_DATA_TYPE_SETTING_CHANGED,
                 self.changeManager.DOCR_DATA_TYPE_MOVED,
                 self.changeManager.DOCR_DATA_TYPE_ADDED
             ]
-
+        def domainObjectChanged(self, ev):
             for record in ev:
                 # NOTE: This excludes type changes anything as they are DomainObjectChangeRecord
-
+                # print(f"Event type {record.getEventType()} caught:")
+                # print(f"\tNewValue: {record.getNewValue()}")
+                # print(f"\tOldValue: {record.getOldValue()}")
+                # print(f"\tObjectType: {type(record.getObject())}")
+                if record.getEventType() == 5:
+                    print(record)
                 if not self._interface.ghidra.isinstance(record, self.programChangeRecord):
                     continue
 
                 changeType = record.getEventType()
                 newValue = record.getNewValue()
                 obj = record.getObject()
 
-                if changeType in funcEvents:
+                if changeType in self.funcEvents:
                     pass
-                elif changeType in typeEvents:
+                elif changeType in self.typeEvents:
                     try:
                         struct = self._interface.structs[newValue.name]
                         # TODO: access old name indicate deletion
                         #self._interface.struct_changed(Struct(None, None, None), deleted=True)
                         self._interface.struct_changed(struct)
                     except KeyError:
                         pass
@@ -64,18 +70,20 @@
                     try:
                         enum = self._interface.enums[newValue.name]
                         #self._interface.enum_changed(Enum(None, None), deleted=True)
                         self._interface.enum_changed(enum)
                     except KeyError:
                         pass
 
-                elif changeType in symDelEvents:
+                elif changeType in self.symDelEvents:
                     # Currently unused and unsupported
                     pass
-                elif changeType in symChgEvents:
+                elif changeType in self.symChgEvents:
+                    #if changeType == 52:
+                        #print(f"Record:\n{record}")
                     if obj is None and newValue is not None:
                         obj = newValue
                     if self._interface.ghidra.isinstance(obj, self.db.function.VariableDB):
                         parent_namespace = obj.getParentNamespace()
                         storage = obj.getVariableStorage()
                         if (
                             (newValue is not None) and (storage is not None) and bool(storage.isStackStorage())
```

### Comparing `libbs-1.2.6/libbs/decompilers/ghidra/interface.py` & `libbs-1.2.7/libbs/decompilers/ghidra/interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/libbs/decompilers/ida/artifact_lifter.py` & `libbs-1.2.7/libbs/decompilers/ida/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/libbs/decompilers/ida/compat.py` & `libbs-1.2.7/libbs/decompilers/ida/compat.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/libbs/decompilers/ida/hooks.py` & `libbs-1.2.7/libbs/decompilers/ida/hooks.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/libbs/decompilers/ida/interface.py` & `libbs-1.2.7/libbs/decompilers/ida/interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/libbs/logger.py` & `libbs-1.2.7/libbs/logger.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/libbs/plugin_installer.py` & `libbs-1.2.7/libbs/plugin_installer.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/libbs/ui/__init__.py` & `libbs-1.2.7/libbs/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/libbs/ui/qt_objects.py` & `libbs-1.2.7/libbs/ui/qt_objects.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/libbs/ui/utils.py` & `libbs-1.2.7/libbs/ui/utils.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/libbs.egg-info/PKG-INFO` & `libbs-1.2.7/libbs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: libbs
-Version: 1.2.6
+Version: 1.2.7
 Summary: Your Only Decompiler API Lib - A generic API to script in and out of decompilers
 Home-page: https://github.com/binsync/libbs
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: toml
 Requires-Dist: pycparser
 Requires-Dist: setuptools
 Requires-Dist: prompt_toolkit
@@ -30,14 +30,16 @@
 for all BinSync based plugins.
 
 ## Install
 ```bash
 pip install libbs
 ```
 
+The minimum Python version is **3.8**.
+
 You can optionally also do `libbs --install` after to install generic plugins, but it's not required, since `libbs` 
 files will be installed with plugins that use it. 
 
 ## Usage
 LibBS exposes all decompiler API through the abstract class `DecompilerInterface`. The `DecompilerInterface` 
 can be used in either the default mode, which assumes a GUI, or `headless` mode. In `headless` mode, the interface will 
 start a new process using a specified decompiler.
```

### Comparing `libbs-1.2.6/libbs.egg-info/SOURCES.txt` & `libbs-1.2.7/libbs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/setup.cfg` & `libbs-1.2.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [metadata]
 name = libbs
 version = attr: libbs.__version__
 url = https://github.com/binsync/libbs
 classifiers = 
 	License :: OSI Approved :: BSD License
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
+	Programming Language :: Python :: 3.8
 license = BSD 2 Clause
 license_files = LICENSE
 description = Your Only Decompiler API Lib - A generic API to script in and out of decompilers
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
```

### Comparing `libbs-1.2.6/tests/test_artifacts.py` & `libbs-1.2.7/tests/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/tests/test_cli.py` & `libbs-1.2.7/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.6/tests/test_decompilers.py` & `libbs-1.2.7/tests/test_decompilers.py`

 * *Files identical despite different names*

