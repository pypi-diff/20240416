# Comparing `tmp/arch_flow-0.0.7.tar.gz` & `tmp/arch_flow-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arch_flow-0.0.7.tar", last modified: Tue Apr 16 07:29:56 2024, max compression
+gzip compressed data, was "arch_flow-0.0.8.tar", last modified: Tue Apr 16 07:34:38 2024, max compression
```

## Comparing `arch_flow-0.0.7.tar` & `arch_flow-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 07:29:56.340036 arch_flow-0.0.7/
--rw-rw-rw-   0        0        0     1109 2024-04-16 05:07:31.000000 arch_flow-0.0.7/LICENCE
--rw-rw-rw-   0        0        0      398 2024-04-16 07:29:56.339036 arch_flow-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       66 2024-04-16 06:04:05.000000 arch_flow-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 07:29:56.338037 arch_flow-0.0.7/arch_flow.egg-info/
--rw-rw-rw-   0        0        0      398 2024-04-16 07:29:56.000000 arch_flow-0.0.7/arch_flow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-04-16 07:29:56.000000 arch_flow-0.0.7/arch_flow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 07:29:56.000000 arch_flow-0.0.7/arch_flow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-16 07:29:56.000000 arch_flow-0.0.7/arch_flow.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-16 07:29:56.000000 arch_flow-0.0.7/arch_flow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 07:29:56.340036 arch_flow-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      502 2024-04-16 07:27:38.000000 arch_flow-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 07:34:38.193292 arch_flow-0.0.8/
+-rw-rw-rw-   0        0        0     1109 2024-04-16 05:07:31.000000 arch_flow-0.0.8/LICENCE
+-rw-rw-rw-   0        0        0      398 2024-04-16 07:34:38.192291 arch_flow-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       66 2024-04-16 06:04:05.000000 arch_flow-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 07:34:38.176292 arch_flow-0.0.8/arch_flow/
+-rw-rw-rw-   0        0        0     4506 2024-04-16 07:34:12.000000 arch_flow-0.0.8/arch_flow/ArchFlow.py
+-rw-rw-rw-   0        0        0      877 2024-04-16 07:34:12.000000 arch_flow-0.0.8/arch_flow/DirectoryCreator.py
+-rw-rw-rw-   0        0        0     3142 2024-04-16 07:34:12.000000 arch_flow-0.0.8/arch_flow/DirectoryExplorer.py
+-rw-rw-rw-   0        0        0     3130 2024-04-16 07:34:12.000000 arch_flow-0.0.8/arch_flow/StringManipulator.py
+-rw-rw-rw-   0        0        0       32 2024-04-16 07:33:26.000000 arch_flow-0.0.8/arch_flow/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 07:34:38.191292 arch_flow-0.0.8/arch_flow.egg-info/
+-rw-rw-rw-   0        0        0      398 2024-04-16 07:34:38.000000 arch_flow-0.0.8/arch_flow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2024-04-16 07:34:38.000000 arch_flow-0.0.8/arch_flow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 07:34:38.000000 arch_flow-0.0.8/arch_flow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-16 07:34:38.000000 arch_flow-0.0.8/arch_flow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-16 07:34:38.000000 arch_flow-0.0.8/arch_flow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 07:34:38.193292 arch_flow-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      507 2024-04-16 07:34:33.000000 arch_flow-0.0.8/setup.py
```

### Comparing `arch_flow-0.0.7/LICENCE` & `arch_flow-0.0.8/LICENCE`

 * *Files identical despite different names*

