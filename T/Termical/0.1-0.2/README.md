# Comparing `tmp/Termical-0.1.tar.gz` & `tmp/Termical-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Termical-0.1.tar", last modified: Mon Apr 15 18:08:10 2024, max compression
+gzip compressed data, was "Termical-0.2.tar", last modified: Tue Apr 16 21:03:57 2024, max compression
```

## Comparing `Termical-0.1.tar` & `Termical-0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2024-04-15 18:08:10.661427 Termical-0.1/
--rw-rw-r--   0 marek     (1000) marek     (1000)      210 2024-04-15 18:08:10.661427 Termical-0.1/PKG-INFO
-drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2024-04-15 18:08:10.661427 Termical-0.1/Termical.egg-info/
--rw-rw-r--   0 marek     (1000) marek     (1000)      210 2024-04-15 18:08:10.000000 Termical-0.1/Termical.egg-info/PKG-INFO
--rw-rw-r--   0 marek     (1000) marek     (1000)      167 2024-04-15 18:08:10.000000 Termical-0.1/Termical.egg-info/SOURCES.txt
--rw-rw-r--   0 marek     (1000) marek     (1000)        1 2024-04-15 18:08:10.000000 Termical-0.1/Termical.egg-info/dependency_links.txt
--rw-rw-r--   0 marek     (1000) marek     (1000)       71 2024-04-15 18:08:10.000000 Termical-0.1/Termical.egg-info/requires.txt
--rw-rw-r--   0 marek     (1000) marek     (1000)        1 2024-04-15 18:08:10.000000 Termical-0.1/Termical.egg-info/top_level.txt
--rw-rw-r--   0 marek     (1000) marek     (1000)       38 2024-04-15 18:08:10.661427 Termical-0.1/setup.cfg
--rw-rw-r--   0 marek     (1000) marek     (1000)      386 2024-04-15 18:03:31.000000 Termical-0.1/setup.py
+drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2024-04-16 21:03:57.549563 Termical-0.2/
+-rw-rw-r--   0 marek     (1000) marek     (1000)      210 2024-04-16 21:03:57.549563 Termical-0.2/PKG-INFO
+drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2024-04-16 21:03:57.549563 Termical-0.2/Termical.egg-info/
+-rw-rw-r--   0 marek     (1000) marek     (1000)      210 2024-04-16 21:03:57.000000 Termical-0.2/Termical.egg-info/PKG-INFO
+-rw-rw-r--   0 marek     (1000) marek     (1000)      167 2024-04-16 21:03:57.000000 Termical-0.2/Termical.egg-info/SOURCES.txt
+-rw-rw-r--   0 marek     (1000) marek     (1000)        1 2024-04-16 21:03:57.000000 Termical-0.2/Termical.egg-info/dependency_links.txt
+-rw-rw-r--   0 marek     (1000) marek     (1000)       71 2024-04-16 21:03:57.000000 Termical-0.2/Termical.egg-info/requires.txt
+-rw-rw-r--   0 marek     (1000) marek     (1000)        1 2024-04-16 21:03:57.000000 Termical-0.2/Termical.egg-info/top_level.txt
+-rw-rw-r--   0 marek     (1000) marek     (1000)       38 2024-04-16 21:03:57.549563 Termical-0.2/setup.cfg
+-rw-rw-r--   0 marek     (1000) marek     (1000)      386 2024-04-16 21:03:53.000000 Termical-0.2/setup.py
```

