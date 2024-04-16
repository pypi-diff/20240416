# Comparing `tmp/arch_flow-0.0.6.tar.gz` & `tmp/arch_flow-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arch_flow-0.0.6.tar", last modified: Tue Apr 16 07:03:48 2024, max compression
+gzip compressed data, was "arch_flow-0.0.7.tar", last modified: Tue Apr 16 07:29:56 2024, max compression
```

## Comparing `arch_flow-0.0.6.tar` & `arch_flow-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 07:03:48.090591 arch_flow-0.0.6/
--rw-rw-rw-   0        0        0     1109 2024-04-16 05:07:31.000000 arch_flow-0.0.6/LICENCE
--rw-rw-rw-   0        0        0      398 2024-04-16 07:03:48.089591 arch_flow-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       66 2024-04-16 06:04:05.000000 arch_flow-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 07:03:48.076591 arch_flow-0.0.6/arch_flow/
--rw-rw-rw-   0        0        0       32 2024-04-16 07:03:32.000000 arch_flow-0.0.6/arch_flow/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 07:03:48.088588 arch_flow-0.0.6/arch_flow.egg-info/
--rw-rw-rw-   0        0        0      398 2024-04-16 07:03:48.000000 arch_flow-0.0.6/arch_flow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2024-04-16 07:03:48.000000 arch_flow-0.0.6/arch_flow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 07:03:48.000000 arch_flow-0.0.6/arch_flow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-16 07:03:48.000000 arch_flow-0.0.6/arch_flow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-16 07:03:48.000000 arch_flow-0.0.6/arch_flow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 07:03:48.090591 arch_flow-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      507 2024-04-16 07:03:39.000000 arch_flow-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 07:29:56.340036 arch_flow-0.0.7/
+-rw-rw-rw-   0        0        0     1109 2024-04-16 05:07:31.000000 arch_flow-0.0.7/LICENCE
+-rw-rw-rw-   0        0        0      398 2024-04-16 07:29:56.339036 arch_flow-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       66 2024-04-16 06:04:05.000000 arch_flow-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 07:29:56.338037 arch_flow-0.0.7/arch_flow.egg-info/
+-rw-rw-rw-   0        0        0      398 2024-04-16 07:29:56.000000 arch_flow-0.0.7/arch_flow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-04-16 07:29:56.000000 arch_flow-0.0.7/arch_flow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 07:29:56.000000 arch_flow-0.0.7/arch_flow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-16 07:29:56.000000 arch_flow-0.0.7/arch_flow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-16 07:29:56.000000 arch_flow-0.0.7/arch_flow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 07:29:56.340036 arch_flow-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      502 2024-04-16 07:27:38.000000 arch_flow-0.0.7/setup.py
```

### Comparing `arch_flow-0.0.6/LICENCE` & `arch_flow-0.0.7/LICENCE`

 * *Files identical despite different names*

