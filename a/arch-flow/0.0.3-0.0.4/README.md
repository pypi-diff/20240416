# Comparing `tmp/arch_flow-0.0.3.tar.gz` & `tmp/arch_flow-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arch_flow-0.0.3.tar", last modified: Tue Apr 16 06:08:22 2024, max compression
+gzip compressed data, was "arch_flow-0.0.4.tar", last modified: Tue Apr 16 06:58:54 2024, max compression
```

## Comparing `arch_flow-0.0.3.tar` & `arch_flow-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 06:08:22.575261 arch_flow-0.0.3/
--rw-rw-rw-   0        0        0     1109 2024-04-16 05:07:31.000000 arch_flow-0.0.3/LICENCE
--rw-rw-rw-   0        0        0      398 2024-04-16 06:08:22.574260 arch_flow-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       66 2024-04-16 06:04:05.000000 arch_flow-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 06:08:22.564259 arch_flow-0.0.3/arch_flow/
--rw-rw-rw-   0        0        0     4506 2024-04-16 05:19:46.000000 arch_flow-0.0.3/arch_flow/ArchFlow.py
--rw-rw-rw-   0        0        0      877 2024-04-16 05:19:46.000000 arch_flow-0.0.3/arch_flow/DirectoryCreator.py
--rw-rw-rw-   0        0        0     3142 2024-04-16 05:19:46.000000 arch_flow-0.0.3/arch_flow/DirectoryExplorer.py
--rw-rw-rw-   0        0        0     3130 2024-04-16 05:19:46.000000 arch_flow-0.0.3/arch_flow/StringManipulator.py
--rw-rw-rw-   0        0        0      135 2024-04-16 06:03:03.000000 arch_flow-0.0.3/arch_flow/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 06:08:22.573260 arch_flow-0.0.3/arch_flow.egg-info/
--rw-rw-rw-   0        0        0      398 2024-04-16 06:08:22.000000 arch_flow-0.0.3/arch_flow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2024-04-16 06:08:22.000000 arch_flow-0.0.3/arch_flow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 06:08:22.000000 arch_flow-0.0.3/arch_flow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-16 06:08:22.000000 arch_flow-0.0.3/arch_flow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-16 06:08:22.000000 arch_flow-0.0.3/arch_flow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 06:08:22.575261 arch_flow-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      507 2024-04-16 06:08:18.000000 arch_flow-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 06:58:54.056956 arch_flow-0.0.4/
+-rw-rw-rw-   0        0        0     1109 2024-04-16 05:07:31.000000 arch_flow-0.0.4/LICENCE
+-rw-rw-rw-   0        0        0      398 2024-04-16 06:58:54.055956 arch_flow-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       66 2024-04-16 06:04:05.000000 arch_flow-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 06:58:54.039956 arch_flow-0.0.4/arch_flow/
+-rw-rw-rw-   0        0        0       41 2024-04-16 06:57:54.000000 arch_flow-0.0.4/arch_flow/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 06:58:54.054956 arch_flow-0.0.4/arch_flow.egg-info/
+-rw-rw-rw-   0        0        0      398 2024-04-16 06:58:53.000000 arch_flow-0.0.4/arch_flow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2024-04-16 06:58:53.000000 arch_flow-0.0.4/arch_flow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 06:58:53.000000 arch_flow-0.0.4/arch_flow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-16 06:58:53.000000 arch_flow-0.0.4/arch_flow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-16 06:58:53.000000 arch_flow-0.0.4/arch_flow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 06:58:54.056956 arch_flow-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      507 2024-04-16 06:58:18.000000 arch_flow-0.0.4/setup.py
```

### Comparing `arch_flow-0.0.3/LICENCE` & `arch_flow-0.0.4/LICENCE`

 * *Files identical despite different names*

