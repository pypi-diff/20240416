# Comparing `tmp/django_tailwindcss_automated-0.2.tar.gz` & `tmp/django_tailwindcss_automated-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tailwindcss_automated-0.2.tar", last modified: Tue Apr 16 17:47:48 2024, max compression
+gzip compressed data, was "django_tailwindcss_automated-0.3.tar", last modified: Tue Apr 16 18:13:18 2024, max compression
```

## Comparing `django_tailwindcss_automated-0.2.tar` & `django_tailwindcss_automated-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 mwwlean   (1000) mwwlean   (1000)        0 2024-04-16 17:47:48.562250 django_tailwindcss_automated-0.2/
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)      151 2024-04-16 17:47:48.562250 django_tailwindcss_automated-0.2/PKG-INFO
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)      772 2024-04-14 20:05:35.000000 django_tailwindcss_automated-0.2/README.md
-drwxrwxr-x   0 mwwlean   (1000) mwwlean   (1000)        0 2024-04-16 17:47:48.562250 django_tailwindcss_automated-0.2/django_tailwindcss_automated/
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)       37 2024-04-16 17:36:26.000000 django_tailwindcss_automated-0.2/django_tailwindcss_automated/__init__.py
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)     6909 2024-04-16 17:47:37.000000 django_tailwindcss_automated-0.2/django_tailwindcss_automated/main.py
-drwxrwxr-x   0 mwwlean   (1000) mwwlean   (1000)        0 2024-04-16 17:47:48.562250 django_tailwindcss_automated-0.2/django_tailwindcss_automated.egg-info/
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)      151 2024-04-16 17:47:48.000000 django_tailwindcss_automated-0.2/django_tailwindcss_automated.egg-info/PKG-INFO
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)      359 2024-04-16 17:47:48.000000 django_tailwindcss_automated-0.2/django_tailwindcss_automated.egg-info/SOURCES.txt
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)        1 2024-04-16 17:47:48.000000 django_tailwindcss_automated-0.2/django_tailwindcss_automated.egg-info/dependency_links.txt
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)       80 2024-04-16 17:47:48.000000 django_tailwindcss_automated-0.2/django_tailwindcss_automated.egg-info/entry_points.txt
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)       29 2024-04-16 17:47:48.000000 django_tailwindcss_automated-0.2/django_tailwindcss_automated.egg-info/top_level.txt
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)       38 2024-04-16 17:47:48.562250 django_tailwindcss_automated-0.2/setup.cfg
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)      376 2024-04-16 17:45:08.000000 django_tailwindcss_automated-0.2/setup.py
+drwxrwxr-x   0 mwwlean   (1000) mwwlean   (1000)        0 2024-04-16 18:13:18.670567 django_tailwindcss_automated-0.3/
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)      171 2024-04-16 18:13:18.670567 django_tailwindcss_automated-0.3/PKG-INFO
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)      772 2024-04-14 20:05:35.000000 django_tailwindcss_automated-0.3/README.md
+drwxrwxr-x   0 mwwlean   (1000) mwwlean   (1000)        0 2024-04-16 18:13:18.658567 django_tailwindcss_automated-0.3/django_tailwindcss_automated/
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)       37 2024-04-16 17:36:26.000000 django_tailwindcss_automated-0.3/django_tailwindcss_automated/__init__.py
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)     6909 2024-04-16 17:47:37.000000 django_tailwindcss_automated-0.3/django_tailwindcss_automated/main.py
+drwxrwxr-x   0 mwwlean   (1000) mwwlean   (1000)        0 2024-04-16 18:13:18.670567 django_tailwindcss_automated-0.3/django_tailwindcss_automated.egg-info/
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)      171 2024-04-16 18:13:17.000000 django_tailwindcss_automated-0.3/django_tailwindcss_automated.egg-info/PKG-INFO
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)      359 2024-04-16 18:13:17.000000 django_tailwindcss_automated-0.3/django_tailwindcss_automated.egg-info/SOURCES.txt
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)        1 2024-04-16 18:13:17.000000 django_tailwindcss_automated-0.3/django_tailwindcss_automated.egg-info/dependency_links.txt
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)       80 2024-04-16 18:13:17.000000 django_tailwindcss_automated-0.3/django_tailwindcss_automated.egg-info/entry_points.txt
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)       29 2024-04-16 18:13:17.000000 django_tailwindcss_automated-0.3/django_tailwindcss_automated.egg-info/top_level.txt
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)       38 2024-04-16 18:13:18.670567 django_tailwindcss_automated-0.3/setup.cfg
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)      404 2024-04-16 18:13:00.000000 django_tailwindcss_automated-0.3/setup.py
```

### Comparing `django_tailwindcss_automated-0.2/README.md` & `django_tailwindcss_automated-0.3/README.md`

 * *Files identical despite different names*

### Comparing `django_tailwindcss_automated-0.2/django_tailwindcss_automated/main.py` & `django_tailwindcss_automated-0.3/django_tailwindcss_automated/main.py`

 * *Files identical despite different names*

