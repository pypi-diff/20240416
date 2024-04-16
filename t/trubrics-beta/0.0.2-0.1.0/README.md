# Comparing `tmp/trubrics-beta-0.0.2.tar.gz` & `tmp/trubrics_beta-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trubrics-beta-0.0.2.tar", last modified: Tue Apr  9 17:09:45 2024, max compression
+gzip compressed data, was "trubrics_beta-0.1.0.tar", last modified: Tue Apr 16 13:05:19 2024, max compression
```

## Comparing `trubrics-beta-0.0.2.tar` & `trubrics_beta-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 jeffkayne   (501) staff       (20)        0 2024-04-09 17:09:45.836982 trubrics-beta-0.0.2/
--rw-r--r--   0 jeffkayne   (501) staff       (20)      640 2024-04-09 17:09:45.836788 trubrics-beta-0.0.2/PKG-INFO
--rw-r--r--   0 jeffkayne   (501) staff       (20)      324 2024-04-09 16:04:58.000000 trubrics-beta-0.0.2/README.md
--rw-r--r--   0 jeffkayne   (501) staff       (20)      417 2024-04-09 17:09:26.000000 trubrics-beta-0.0.2/pyproject.toml
--rw-r--r--   0 jeffkayne   (501) staff       (20)        8 2024-04-09 15:57:45.000000 trubrics-beta-0.0.2/requirements.txt
--rw-r--r--   0 jeffkayne   (501) staff       (20)       38 2024-04-09 17:09:45.837031 trubrics-beta-0.0.2/setup.cfg
-drwxr-xr-x   0 jeffkayne   (501) staff       (20)        0 2024-04-09 17:09:45.835752 trubrics-beta-0.0.2/trubrics/
--rw-r--r--   0 jeffkayne   (501) staff       (20)      137 2024-04-09 17:00:05.000000 trubrics-beta-0.0.2/trubrics/__init__.py
--rw-r--r--   0 jeffkayne   (501) staff       (20)     2821 2024-04-09 17:09:03.000000 trubrics-beta-0.0.2/trubrics/sdk.py
-drwxr-xr-x   0 jeffkayne   (501) staff       (20)        0 2024-04-09 17:09:45.836576 trubrics-beta-0.0.2/trubrics_beta.egg-info/
--rw-r--r--   0 jeffkayne   (501) staff       (20)      640 2024-04-09 17:09:45.000000 trubrics-beta-0.0.2/trubrics_beta.egg-info/PKG-INFO
--rw-r--r--   0 jeffkayne   (501) staff       (20)      226 2024-04-09 17:09:45.000000 trubrics-beta-0.0.2/trubrics_beta.egg-info/SOURCES.txt
--rw-r--r--   0 jeffkayne   (501) staff       (20)        1 2024-04-09 17:09:45.000000 trubrics-beta-0.0.2/trubrics_beta.egg-info/dependency_links.txt
--rw-r--r--   0 jeffkayne   (501) staff       (20)        9 2024-04-09 17:09:45.000000 trubrics-beta-0.0.2/trubrics_beta.egg-info/top_level.txt
+drwxr-xr-x   0 jeffkayne   (501) staff       (20)        0 2024-04-16 13:05:19.122871 trubrics_beta-0.1.0/
+-rw-r--r--   0 jeffkayne   (501) staff       (20)      627 2024-04-16 13:05:19.122631 trubrics_beta-0.1.0/PKG-INFO
+-rw-r--r--   0 jeffkayne   (501) staff       (20)      311 2024-04-16 12:55:47.000000 trubrics_beta-0.1.0/README.md
+-rw-r--r--   0 jeffkayne   (501) staff       (20)      417 2024-04-16 13:04:20.000000 trubrics_beta-0.1.0/pyproject.toml
+-rw-r--r--   0 jeffkayne   (501) staff       (20)       38 2024-04-16 13:05:19.122922 trubrics_beta-0.1.0/setup.cfg
+drwxr-xr-x   0 jeffkayne   (501) staff       (20)        0 2024-04-16 13:05:19.121003 trubrics_beta-0.1.0/trubrics_beta/
+-rw-r--r--   0 jeffkayne   (501) staff       (20)      142 2024-04-16 13:00:41.000000 trubrics_beta-0.1.0/trubrics_beta/__init__.py
+-rw-r--r--   0 jeffkayne   (501) staff       (20)     2433 2024-04-16 12:46:24.000000 trubrics_beta-0.1.0/trubrics_beta/sdk.py
+drwxr-xr-x   0 jeffkayne   (501) staff       (20)        0 2024-04-16 13:05:19.122386 trubrics_beta-0.1.0/trubrics_beta.egg-info/
+-rw-r--r--   0 jeffkayne   (501) staff       (20)      627 2024-04-16 13:05:19.000000 trubrics_beta-0.1.0/trubrics_beta.egg-info/PKG-INFO
+-rw-r--r--   0 jeffkayne   (501) staff       (20)      219 2024-04-16 13:05:19.000000 trubrics_beta-0.1.0/trubrics_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffkayne   (501) staff       (20)        1 2024-04-16 13:05:19.000000 trubrics_beta-0.1.0/trubrics_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffkayne   (501) staff       (20)       14 2024-04-16 13:05:19.000000 trubrics_beta-0.1.0/trubrics_beta.egg-info/top_level.txt
```

