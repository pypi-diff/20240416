# Comparing `tmp/arch_flow-0.0.1.tar.gz` & `tmp/arch_flow-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arch_flow-0.0.1.tar", last modified: Tue Apr 16 05:21:02 2024, max compression
+gzip compressed data, was "arch_flow-0.0.2.tar", last modified: Tue Apr 16 05:49:28 2024, max compression
```

## Comparing `arch_flow-0.0.1.tar` & `arch_flow-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 05:21:02.626142 arch_flow-0.0.1/
--rw-rw-rw-   0        0        0     1109 2024-04-16 05:07:31.000000 arch_flow-0.0.1/LICENCE
--rw-rw-rw-   0        0        0      403 2024-04-16 05:21:02.625142 arch_flow-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       67 2024-04-16 05:09:38.000000 arch_flow-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 05:21:02.603143 arch_flow-0.0.1/arch_flow/
--rw-rw-rw-   0        0        0     4506 2024-04-16 05:19:46.000000 arch_flow-0.0.1/arch_flow/ArchFlow.py
--rw-rw-rw-   0        0        0      877 2024-04-16 05:19:46.000000 arch_flow-0.0.1/arch_flow/DirectoryCreator.py
--rw-rw-rw-   0        0        0     3142 2024-04-16 05:19:46.000000 arch_flow-0.0.1/arch_flow/DirectoryExplorer.py
--rw-rw-rw-   0        0        0     3130 2024-04-16 05:19:46.000000 arch_flow-0.0.1/arch_flow/StringManipulator.py
--rw-rw-rw-   0        0        0       24 2024-04-16 05:06:05.000000 arch_flow-0.0.1/arch_flow/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 05:21:02.624141 arch_flow-0.0.1/arch_flow.egg-info/
--rw-rw-rw-   0        0        0      403 2024-04-16 05:21:02.000000 arch_flow-0.0.1/arch_flow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2024-04-16 05:21:02.000000 arch_flow-0.0.1/arch_flow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 05:21:02.000000 arch_flow-0.0.1/arch_flow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-16 05:21:02.000000 arch_flow-0.0.1/arch_flow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-16 05:21:02.000000 arch_flow-0.0.1/arch_flow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 05:21:02.626142 arch_flow-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      509 2024-04-16 05:17:05.000000 arch_flow-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 05:49:28.096487 arch_flow-0.0.2/
+-rw-rw-rw-   0        0        0     1109 2024-04-16 05:07:31.000000 arch_flow-0.0.2/LICENCE
+-rw-rw-rw-   0        0        0      401 2024-04-16 05:49:28.095486 arch_flow-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       67 2024-04-16 05:09:38.000000 arch_flow-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 05:49:28.081486 arch_flow-0.0.2/arch_flow/
+-rw-rw-rw-   0        0        0     4506 2024-04-16 05:19:46.000000 arch_flow-0.0.2/arch_flow/ArchFlow.py
+-rw-rw-rw-   0        0        0      877 2024-04-16 05:19:46.000000 arch_flow-0.0.2/arch_flow/DirectoryCreator.py
+-rw-rw-rw-   0        0        0     3142 2024-04-16 05:19:46.000000 arch_flow-0.0.2/arch_flow/DirectoryExplorer.py
+-rw-rw-rw-   0        0        0     3130 2024-04-16 05:19:46.000000 arch_flow-0.0.2/arch_flow/StringManipulator.py
+-rw-rw-rw-   0        0        0       25 2024-04-16 05:47:55.000000 arch_flow-0.0.2/arch_flow/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 05:49:28.094487 arch_flow-0.0.2/arch_flow.egg-info/
+-rw-rw-rw-   0        0        0      401 2024-04-16 05:49:27.000000 arch_flow-0.0.2/arch_flow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2024-04-16 05:49:27.000000 arch_flow-0.0.2/arch_flow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 05:49:27.000000 arch_flow-0.0.2/arch_flow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-16 05:49:27.000000 arch_flow-0.0.2/arch_flow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-16 05:49:27.000000 arch_flow-0.0.2/arch_flow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 05:49:28.096487 arch_flow-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      507 2024-04-16 05:49:07.000000 arch_flow-0.0.2/setup.py
```

### Comparing `arch_flow-0.0.1/LICENCE` & `arch_flow-0.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `arch_flow-0.0.1/arch_flow/ArchFlow.py` & `arch_flow-0.0.2/arch_flow/ArchFlow.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.0.1/arch_flow/DirectoryCreator.py` & `arch_flow-0.0.2/arch_flow/DirectoryCreator.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.0.1/arch_flow/DirectoryExplorer.py` & `arch_flow-0.0.2/arch_flow/DirectoryExplorer.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.0.1/arch_flow/StringManipulator.py` & `arch_flow-0.0.2/arch_flow/StringManipulator.py`

 * *Files identical despite different names*

