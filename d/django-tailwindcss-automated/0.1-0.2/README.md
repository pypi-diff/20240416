# Comparing `tmp/django_tailwindcss_automated-0.1.tar.gz` & `tmp/django_tailwindcss_automated-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tailwindcss_automated-0.1.tar", last modified: Tue Apr 16 17:40:12 2024, max compression
+gzip compressed data, was "django_tailwindcss_automated-0.2.tar", last modified: Tue Apr 16 17:47:48 2024, max compression
```

## Comparing `django_tailwindcss_automated-0.1.tar` & `django_tailwindcss_automated-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 mwwlean   (1000) mwwlean   (1000)        0 2024-04-16 17:40:12.564906 django_tailwindcss_automated-0.1/
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)      151 2024-04-16 17:40:12.564906 django_tailwindcss_automated-0.1/PKG-INFO
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)      772 2024-04-14 20:05:35.000000 django_tailwindcss_automated-0.1/README.md
-drwxrwxr-x   0 mwwlean   (1000) mwwlean   (1000)        0 2024-04-16 17:40:12.564906 django_tailwindcss_automated-0.1/django_tailwindcss_automated/
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)       37 2024-04-16 17:36:26.000000 django_tailwindcss_automated-0.1/django_tailwindcss_automated/__init__.py
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)     6905 2024-04-16 14:31:55.000000 django_tailwindcss_automated-0.1/django_tailwindcss_automated/main.py
-drwxrwxr-x   0 mwwlean   (1000) mwwlean   (1000)        0 2024-04-16 17:40:12.564906 django_tailwindcss_automated-0.1/django_tailwindcss_automated.egg-info/
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)      151 2024-04-16 17:40:12.000000 django_tailwindcss_automated-0.1/django_tailwindcss_automated.egg-info/PKG-INFO
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)      359 2024-04-16 17:40:12.000000 django_tailwindcss_automated-0.1/django_tailwindcss_automated.egg-info/SOURCES.txt
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)        1 2024-04-16 17:40:12.000000 django_tailwindcss_automated-0.1/django_tailwindcss_automated.egg-info/dependency_links.txt
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)       80 2024-04-16 17:40:12.000000 django_tailwindcss_automated-0.1/django_tailwindcss_automated.egg-info/entry_points.txt
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)       29 2024-04-16 17:40:12.000000 django_tailwindcss_automated-0.1/django_tailwindcss_automated.egg-info/top_level.txt
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)       38 2024-04-16 17:40:12.564906 django_tailwindcss_automated-0.1/setup.cfg
--rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)      376 2024-04-16 17:40:08.000000 django_tailwindcss_automated-0.1/setup.py
+drwxrwxr-x   0 mwwlean   (1000) mwwlean   (1000)        0 2024-04-16 17:47:48.562250 django_tailwindcss_automated-0.2/
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)      151 2024-04-16 17:47:48.562250 django_tailwindcss_automated-0.2/PKG-INFO
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)      772 2024-04-14 20:05:35.000000 django_tailwindcss_automated-0.2/README.md
+drwxrwxr-x   0 mwwlean   (1000) mwwlean   (1000)        0 2024-04-16 17:47:48.562250 django_tailwindcss_automated-0.2/django_tailwindcss_automated/
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)       37 2024-04-16 17:36:26.000000 django_tailwindcss_automated-0.2/django_tailwindcss_automated/__init__.py
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)     6909 2024-04-16 17:47:37.000000 django_tailwindcss_automated-0.2/django_tailwindcss_automated/main.py
+drwxrwxr-x   0 mwwlean   (1000) mwwlean   (1000)        0 2024-04-16 17:47:48.562250 django_tailwindcss_automated-0.2/django_tailwindcss_automated.egg-info/
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)      151 2024-04-16 17:47:48.000000 django_tailwindcss_automated-0.2/django_tailwindcss_automated.egg-info/PKG-INFO
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)      359 2024-04-16 17:47:48.000000 django_tailwindcss_automated-0.2/django_tailwindcss_automated.egg-info/SOURCES.txt
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)        1 2024-04-16 17:47:48.000000 django_tailwindcss_automated-0.2/django_tailwindcss_automated.egg-info/dependency_links.txt
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)       80 2024-04-16 17:47:48.000000 django_tailwindcss_automated-0.2/django_tailwindcss_automated.egg-info/entry_points.txt
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)       29 2024-04-16 17:47:48.000000 django_tailwindcss_automated-0.2/django_tailwindcss_automated.egg-info/top_level.txt
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)       38 2024-04-16 17:47:48.562250 django_tailwindcss_automated-0.2/setup.cfg
+-rw-rw-r--   0 mwwlean   (1000) mwwlean   (1000)      376 2024-04-16 17:45:08.000000 django_tailwindcss_automated-0.2/setup.py
```

### Comparing `django_tailwindcss_automated-0.1/README.md` & `django_tailwindcss_automated-0.2/README.md`

 * *Files identical despite different names*

### Comparing `django_tailwindcss_automated-0.1/django_tailwindcss_automated/main.py` & `django_tailwindcss_automated-0.2/django_tailwindcss_automated/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,16 +246,16 @@
     create_django_project(project_name)
     install_django_compressor()
     configure_django_settings(project_name)
     create_static_folders()
     create_views_and_templates(project_name)
 
     os.chdir(project_name)
-
+    os.chdir("..")
+    tailwind_setup(project_name)
     print(f"Django project '{project_name}' with Tailwind CSS has been created  ")
 
     
 
 if __name__ == "__main__":
     main()
-    os.chdir("..")
-    tailwind_setup(project_name)
+
```

