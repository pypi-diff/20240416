# Comparing `tmp/aina-gradio-theme-2.2.tar.gz` & `tmp/aina_gradio_theme-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aina-gradio-theme-2.2.tar", last modified: Mon Mar 11 15:43:33 2024, max compression
+gzip compressed data, was "aina_gradio_theme-2.3.tar", last modified: Tue Apr 16 08:17:46 2024, max compression
```

## Comparing `aina-gradio-theme-2.2.tar` & `aina_gradio_theme-2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:43:33.874794 aina-gradio-theme-2.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:43:33.870794 aina-gradio-theme-2.2/AinaTheme/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-11 15:43:28.000000 aina-gradio-theme-2.2/AinaTheme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-03-11 15:43:28.000000 aina-gradio-theme-2.2/AinaTheme/aina_class.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:43:33.874794 aina-gradio-theme-2.2/AinaTheme/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 15:43:28.000000 aina-gradio-theme-2.2/AinaTheme/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-03-11 15:43:28.000000 aina-gradio-theme-2.2/AinaTheme/utils/custom_colors.py
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-11 15:43:28.000000 aina-gradio-theme-2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-03-11 15:43:33.874794 aina-gradio-theme-2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-03-11 15:43:28.000000 aina-gradio-theme-2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:43:33.874794 aina-gradio-theme-2.2/aina_gradio_theme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-03-11 15:43:33.000000 aina-gradio-theme-2.2/aina_gradio_theme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-11 15:43:33.000000 aina-gradio-theme-2.2/aina_gradio_theme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 15:43:33.000000 aina-gradio-theme-2.2/aina_gradio_theme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-11 15:43:33.000000 aina-gradio-theme-2.2/aina_gradio_theme.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 15:43:33.874794 aina-gradio-theme-2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-11 15:43:28.000000 aina-gradio-theme-2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:17:46.826264 aina_gradio_theme-2.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:17:46.822264 aina_gradio_theme-2.3/AinaTheme/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-16 08:17:41.000000 aina_gradio_theme-2.3/AinaTheme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-16 08:17:41.000000 aina_gradio_theme-2.3/AinaTheme/aina_class.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:17:46.822264 aina_gradio_theme-2.3/AinaTheme/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:17:41.000000 aina_gradio_theme-2.3/AinaTheme/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-16 08:17:41.000000 aina_gradio_theme-2.3/AinaTheme/utils/custom_colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 08:17:41.000000 aina_gradio_theme-2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-16 08:17:46.826264 aina_gradio_theme-2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-16 08:17:41.000000 aina_gradio_theme-2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:17:46.826264 aina_gradio_theme-2.3/aina_gradio_theme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-16 08:17:46.000000 aina_gradio_theme-2.3/aina_gradio_theme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-16 08:17:46.000000 aina_gradio_theme-2.3/aina_gradio_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 08:17:46.000000 aina_gradio_theme-2.3/aina_gradio_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 08:17:46.000000 aina_gradio_theme-2.3/aina_gradio_theme.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 08:17:46.826264 aina_gradio_theme-2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-16 08:17:41.000000 aina_gradio_theme-2.3/setup.py
```

### Comparing `aina-gradio-theme-2.2/AinaTheme/aina_class.py` & `aina_gradio_theme-2.3/AinaTheme/aina_class.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,13 +39,15 @@
             font=font,
             font_mono=font_mono,
         )
         self.name = "aina"
         super().set(
             block_title_text_color="black",
             block_label_text_color="black",
-            block_label_text_weight=400,
-            block_title_text_weight=400,
+            block_label_text_weight=600,
+            block_title_text_weight=600,
             block_title_background_fill="transparent",
             block_label_background_fill="transparent",
+            input_shadow="rgba(0, 0, 0, 0.02) 0px 1px 3px 0px, rgba(27, 31, 35, 0.15) 0px 0px 0px 1px",
+            input_shadow_focus="rgba(0, 0, 0, 0.02) 0px 1px 3px 0px, rgba(27, 31, 35, 0.15) 0px 0px 0px 2px",
         )
```

### Comparing `aina-gradio-theme-2.2/AinaTheme/utils/custom_colors.py` & `aina_gradio_theme-2.3/AinaTheme/utils/custom_colors.py`

 * *Files identical despite different names*

### Comparing `aina-gradio-theme-2.2/LICENSE` & `aina_gradio_theme-2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aina-gradio-theme-2.2/PKG-INFO` & `aina_gradio_theme-2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aina-gradio-theme
-Version: 2.2
+Version: 2.3
 Summary: Aina Theme is a custom Gradio theme inspired by the visual style of Storj theme. Feel free to use this theme to create Gradio apps that have a visual connection to the world of cloud technology.
 Home-page: https://github.com/projecte-aina/aina-gradio-theme
 Author: Projecte Aina
 Author-email: aina@bsc.es
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aina-gradio-theme-2.2/README.md` & `aina_gradio_theme-2.3/README.md`

 * *Files identical despite different names*

### Comparing `aina-gradio-theme-2.2/aina_gradio_theme.egg-info/PKG-INFO` & `aina_gradio_theme-2.3/aina_gradio_theme.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aina-gradio-theme
-Version: 2.2
+Version: 2.3
 Summary: Aina Theme is a custom Gradio theme inspired by the visual style of Storj theme. Feel free to use this theme to create Gradio apps that have a visual connection to the world of cloud technology.
 Home-page: https://github.com/projecte-aina/aina-gradio-theme
 Author: Projecte Aina
 Author-email: aina@bsc.es
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aina-gradio-theme-2.2/setup.py` & `aina_gradio_theme-2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="aina-gradio-theme",
-    version="2.2",
+    version="2.3",
     description="Aina Theme is a custom Gradio theme inspired by the visual style of Storj theme. Feel free to use this theme to create Gradio apps that have a visual connection to the world of cloud technology.",
     long_description=open("README.md", 'r').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/projecte-aina/aina-gradio-theme",
     author="Projecte Aina",
     author_email="aina@bsc.es",
     license="Apache License 2.0",
```

