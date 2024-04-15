# Comparing `tmp/mkdocs_rtd-0.0.8.tar.gz` & `tmp/mkdocs_rtd-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_rtd-0.0.8.tar", max compression
+gzip compressed data, was "mkdocs_rtd-0.0.9.tar", max compression
```

## Comparing `mkdocs_rtd-0.0.8.tar` & `mkdocs_rtd-0.0.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1007 2023-09-30 06:38:00.169861 mkdocs_rtd-0.0.8/README.md
--rw-r--r--   0        0        0      467 2023-09-30 06:38:00.169861 mkdocs_rtd-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      170 2023-09-30 06:38:00.169861 mkdocs_rtd-0.0.8/rtd/404.html
--rw-r--r--   0        0        0        0 2023-09-30 06:38:00.169861 mkdocs_rtd-0.0.8/rtd/__init__.py
--rw-r--r--   0        0        0     7909 2023-09-30 06:38:00.169861 mkdocs_rtd-0.0.8/rtd/base.html
--rw-r--r--   0        0        0     2487 2023-09-30 06:38:00.169861 mkdocs_rtd-0.0.8/rtd/breadcrumbs.html
--rw-r--r--   0        0        0    87624 2023-09-30 06:38:00.169861 mkdocs_rtd-0.0.8/rtd/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0        0        0    67312 2023-09-30 06:38:00.169861 mkdocs_rtd-0.0.8/rtd/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0        0        0    86288 2023-09-30 06:38:00.169861 mkdocs_rtd-0.0.8/rtd/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0        0        0    66444 2023-09-30 06:38:00.169861 mkdocs_rtd-0.0.8/rtd/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0        0        0   165742 2023-09-30 06:38:00.173861 mkdocs_rtd-0.0.8/rtd/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   444379 2023-09-30 06:38:00.173861 mkdocs_rtd-0.0.8/rtd/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2023-09-30 06:38:00.177861 mkdocs_rtd-0.0.8/rtd/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2023-09-30 06:38:00.177861 mkdocs_rtd-0.0.8/rtd/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2023-09-30 06:38:00.177861 mkdocs_rtd-0.0.8/rtd/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0   323344 2023-09-30 06:38:00.177861 mkdocs_rtd-0.0.8/rtd/css/fonts/lato-bold-italic.woff
--rw-r--r--   0        0        0   193308 2023-09-30 06:38:00.177861 mkdocs_rtd-0.0.8/rtd/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0        0        0   309728 2023-09-30 06:38:00.181861 mkdocs_rtd-0.0.8/rtd/css/fonts/lato-bold.woff
--rw-r--r--   0        0        0   184912 2023-09-30 06:38:00.181861 mkdocs_rtd-0.0.8/rtd/css/fonts/lato-bold.woff2
--rw-r--r--   0        0        0   328412 2023-09-30 06:38:00.181861 mkdocs_rtd-0.0.8/rtd/css/fonts/lato-normal-italic.woff
--rw-r--r--   0        0        0   195704 2023-09-30 06:38:00.181861 mkdocs_rtd-0.0.8/rtd/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0        0        0   309192 2023-09-30 06:38:00.185861 mkdocs_rtd-0.0.8/rtd/css/fonts/lato-normal.woff
--rw-r--r--   0        0        0   182708 2023-09-30 06:38:00.185861 mkdocs_rtd-0.0.8/rtd/css/fonts/lato-normal.woff2
--rw-r--r--   0        0        0   135539 2023-09-30 06:38:00.185861 mkdocs_rtd-0.0.8/rtd/css/theme.css
--rw-r--r--   0        0        0     9466 2023-09-30 06:38:00.185861 mkdocs_rtd-0.0.8/rtd/css/theme_extra.css
--rw-r--r--   0        0        0     1327 2023-09-30 06:38:00.185861 mkdocs_rtd-0.0.8/rtd/footer.html
--rw-r--r--   0        0        0      599 2023-09-30 06:38:00.185861 mkdocs_rtd-0.0.8/rtd/github_icon.png
--rw-r--r--   0        0        0     1150 2023-09-30 06:38:00.185861 mkdocs_rtd-0.0.8/rtd/img/favicon.ico
--rw-r--r--   0        0        0     2731 2023-09-30 06:38:00.185861 mkdocs_rtd-0.0.8/rtd/js/html5shiv.min.js
--rw-r--r--   0        0        0    89501 2023-09-30 06:38:00.185861 mkdocs_rtd-0.0.8/rtd/js/jquery-3.6.0.min.js
--rw-r--r--   0        0        0     9487 2023-09-30 06:38:00.185861 mkdocs_rtd-0.0.8/rtd/js/theme.js
--rw-r--r--   0        0        0      990 2023-09-30 06:38:00.189861 mkdocs_rtd-0.0.8/rtd/js/theme_extra.js
--rw-r--r--   0        0        0     3005 2023-09-30 06:38:00.189861 mkdocs_rtd-0.0.8/rtd/locales/de/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     3050 2023-09-30 06:38:00.189861 mkdocs_rtd-0.0.8/rtd/locales/es/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     3139 2023-09-30 06:38:00.189861 mkdocs_rtd-0.0.8/rtd/locales/fa/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     3022 2023-09-30 06:38:00.189861 mkdocs_rtd-0.0.8/rtd/locales/fr/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     3011 2023-09-30 06:38:00.189861 mkdocs_rtd-0.0.8/rtd/locales/id/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     3031 2023-09-30 06:38:00.189861 mkdocs_rtd-0.0.8/rtd/locales/it/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     3132 2023-09-30 06:38:00.189861 mkdocs_rtd-0.0.8/rtd/locales/ja/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     3068 2023-09-30 06:38:00.189861 mkdocs_rtd-0.0.8/rtd/locales/pt_BR/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     3311 2023-09-30 06:38:00.189861 mkdocs_rtd-0.0.8/rtd/locales/ru/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     2998 2023-09-30 06:38:00.189861 mkdocs_rtd-0.0.8/rtd/locales/tr/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     3307 2023-09-30 06:38:00.189861 mkdocs_rtd-0.0.8/rtd/locales/uk/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     3009 2023-09-30 06:38:00.189861 mkdocs_rtd-0.0.8/rtd/locales/zh_CN/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     3003 2023-09-30 06:38:00.189861 mkdocs_rtd-0.0.8/rtd/locales/zh_TW/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0      384 2023-09-30 06:38:00.189861 mkdocs_rtd-0.0.8/rtd/main.html
--rw-r--r--   0        0        0      411 2023-09-30 06:38:00.189861 mkdocs_rtd-0.0.8/rtd/mkdocs_theme.yml
--rw-r--r--   0        0        0     1127 2023-09-30 06:38:00.189861 mkdocs_rtd-0.0.8/rtd/nav.html
--rw-r--r--   0        0        0      757 2023-09-30 06:38:00.189861 mkdocs_rtd-0.0.8/rtd/search.html
--rw-r--r--   0        0        0      326 2023-09-30 06:38:00.189861 mkdocs_rtd-0.0.8/rtd/searchbox.html
--rw-r--r--   0        0        0      486 2023-09-30 06:38:00.189861 mkdocs_rtd-0.0.8/rtd/toc.html
--rw-r--r--   0        0        0     1070 2023-09-30 06:38:00.189861 mkdocs_rtd-0.0.8/rtd/versions.html
--rw-r--r--   0        0        0     2244 1970-01-01 00:00:00.000000 mkdocs_rtd-0.0.8/setup.py
--rw-r--r--   0        0        0     1613 1970-01-01 00:00:00.000000 mkdocs_rtd-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1007 2023-10-16 18:56:57.697965 mkdocs_rtd-0.0.9/README.md
+-rw-r--r--   0        0        0      467 2023-10-16 18:56:57.697965 mkdocs_rtd-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      170 2023-10-16 18:56:57.697965 mkdocs_rtd-0.0.9/rtd/404.html
+-rw-r--r--   0        0        0        0 2023-10-16 18:56:57.697965 mkdocs_rtd-0.0.9/rtd/__init__.py
+-rw-r--r--   0        0        0     7909 2023-10-16 18:56:57.697965 mkdocs_rtd-0.0.9/rtd/base.html
+-rw-r--r--   0        0        0     2487 2023-10-16 18:56:57.697965 mkdocs_rtd-0.0.9/rtd/breadcrumbs.html
+-rw-r--r--   0        0        0    87624 2023-10-16 18:56:57.697965 mkdocs_rtd-0.0.9/rtd/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0        0        0    67312 2023-10-16 18:56:57.697965 mkdocs_rtd-0.0.9/rtd/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0        0        0    86288 2023-10-16 18:56:57.697965 mkdocs_rtd-0.0.9/rtd/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0        0        0    66444 2023-10-16 18:56:57.697965 mkdocs_rtd-0.0.9/rtd/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0        0        0   165742 2023-10-16 18:56:57.697965 mkdocs_rtd-0.0.9/rtd/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   444379 2023-10-16 18:56:57.701964 mkdocs_rtd-0.0.9/rtd/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   165548 2023-10-16 18:56:57.701964 mkdocs_rtd-0.0.9/rtd/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    98024 2023-10-16 18:56:57.701964 mkdocs_rtd-0.0.9/rtd/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    77160 2023-10-16 18:56:57.701964 mkdocs_rtd-0.0.9/rtd/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0   323344 2023-10-16 18:56:57.705965 mkdocs_rtd-0.0.9/rtd/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0        0        0   193308 2023-10-16 18:56:57.705965 mkdocs_rtd-0.0.9/rtd/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0        0        0   309728 2023-10-16 18:56:57.705965 mkdocs_rtd-0.0.9/rtd/css/fonts/lato-bold.woff
+-rw-r--r--   0        0        0   184912 2023-10-16 18:56:57.705965 mkdocs_rtd-0.0.9/rtd/css/fonts/lato-bold.woff2
+-rw-r--r--   0        0        0   328412 2023-10-16 18:56:57.709965 mkdocs_rtd-0.0.9/rtd/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0        0        0   195704 2023-10-16 18:56:57.709965 mkdocs_rtd-0.0.9/rtd/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0        0        0   309192 2023-10-16 18:56:57.709965 mkdocs_rtd-0.0.9/rtd/css/fonts/lato-normal.woff
+-rw-r--r--   0        0        0   182708 2023-10-16 18:56:57.709965 mkdocs_rtd-0.0.9/rtd/css/fonts/lato-normal.woff2
+-rw-r--r--   0        0        0   135539 2023-10-16 18:56:57.713965 mkdocs_rtd-0.0.9/rtd/css/theme.css
+-rw-r--r--   0        0        0     9466 2023-10-16 18:56:57.713965 mkdocs_rtd-0.0.9/rtd/css/theme_extra.css
+-rw-r--r--   0        0        0     1327 2023-10-16 18:56:57.713965 mkdocs_rtd-0.0.9/rtd/footer.html
+-rw-r--r--   0        0        0      599 2023-10-16 18:56:57.713965 mkdocs_rtd-0.0.9/rtd/github_icon.png
+-rw-r--r--   0        0        0     1150 2023-10-16 18:56:57.713965 mkdocs_rtd-0.0.9/rtd/img/favicon.ico
+-rw-r--r--   0        0        0     2731 2023-10-16 18:56:57.713965 mkdocs_rtd-0.0.9/rtd/js/html5shiv.min.js
+-rw-r--r--   0        0        0    89501 2023-10-16 18:56:57.713965 mkdocs_rtd-0.0.9/rtd/js/jquery-3.6.0.min.js
+-rw-r--r--   0        0        0     9519 2023-10-16 18:56:57.713965 mkdocs_rtd-0.0.9/rtd/js/theme.js
+-rw-r--r--   0        0        0      990 2023-10-16 18:56:57.713965 mkdocs_rtd-0.0.9/rtd/js/theme_extra.js
+-rw-r--r--   0        0        0     3005 2023-10-16 18:56:57.713965 mkdocs_rtd-0.0.9/rtd/locales/de/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     3050 2023-10-16 18:56:57.713965 mkdocs_rtd-0.0.9/rtd/locales/es/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     3139 2023-10-16 18:56:57.713965 mkdocs_rtd-0.0.9/rtd/locales/fa/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     3022 2023-10-16 18:56:57.713965 mkdocs_rtd-0.0.9/rtd/locales/fr/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     3011 2023-10-16 18:56:57.713965 mkdocs_rtd-0.0.9/rtd/locales/id/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     3031 2023-10-16 18:56:57.713965 mkdocs_rtd-0.0.9/rtd/locales/it/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     3132 2023-10-16 18:56:57.713965 mkdocs_rtd-0.0.9/rtd/locales/ja/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     3068 2023-10-16 18:56:57.713965 mkdocs_rtd-0.0.9/rtd/locales/pt_BR/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     3311 2023-10-16 18:56:57.713965 mkdocs_rtd-0.0.9/rtd/locales/ru/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     2998 2023-10-16 18:56:57.713965 mkdocs_rtd-0.0.9/rtd/locales/tr/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     3307 2023-10-16 18:56:57.713965 mkdocs_rtd-0.0.9/rtd/locales/uk/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     3009 2023-10-16 18:56:57.713965 mkdocs_rtd-0.0.9/rtd/locales/zh_CN/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     3003 2023-10-16 18:56:57.713965 mkdocs_rtd-0.0.9/rtd/locales/zh_TW/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      384 2023-10-16 18:56:57.713965 mkdocs_rtd-0.0.9/rtd/main.html
+-rw-r--r--   0        0        0      411 2023-10-16 18:56:57.713965 mkdocs_rtd-0.0.9/rtd/mkdocs_theme.yml
+-rw-r--r--   0        0        0     1127 2023-10-16 18:56:57.713965 mkdocs_rtd-0.0.9/rtd/nav.html
+-rw-r--r--   0        0        0      757 2023-10-16 18:56:57.713965 mkdocs_rtd-0.0.9/rtd/search.html
+-rw-r--r--   0        0        0      326 2023-10-16 18:56:57.713965 mkdocs_rtd-0.0.9/rtd/searchbox.html
+-rw-r--r--   0        0        0      486 2023-10-16 18:56:57.713965 mkdocs_rtd-0.0.9/rtd/toc.html
+-rw-r--r--   0        0        0     1070 2023-10-16 18:56:57.713965 mkdocs_rtd-0.0.9/rtd/versions.html
+-rw-r--r--   0        0        0     2244 1970-01-01 00:00:00.000000 mkdocs_rtd-0.0.9/setup.py
+-rw-r--r--   0        0        0     1613 1970-01-01 00:00:00.000000 mkdocs_rtd-0.0.9/PKG-INFO
```

### Comparing `mkdocs_rtd-0.0.8/README.md` & `mkdocs_rtd-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/base.html` & `mkdocs_rtd-0.0.9/rtd/base.html`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/breadcrumbs.html` & `mkdocs_rtd-0.0.9/rtd/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/css/fonts/Roboto-Slab-Bold.woff` & `mkdocs_rtd-0.0.9/rtd/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/css/fonts/Roboto-Slab-Bold.woff2` & `mkdocs_rtd-0.0.9/rtd/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/css/fonts/Roboto-Slab-Regular.woff` & `mkdocs_rtd-0.0.9/rtd/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/css/fonts/Roboto-Slab-Regular.woff2` & `mkdocs_rtd-0.0.9/rtd/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/css/fonts/fontawesome-webfont.eot` & `mkdocs_rtd-0.0.9/rtd/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/css/fonts/fontawesome-webfont.svg` & `mkdocs_rtd-0.0.9/rtd/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/css/fonts/fontawesome-webfont.ttf` & `mkdocs_rtd-0.0.9/rtd/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/css/fonts/fontawesome-webfont.woff` & `mkdocs_rtd-0.0.9/rtd/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/css/fonts/fontawesome-webfont.woff2` & `mkdocs_rtd-0.0.9/rtd/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/css/fonts/lato-bold-italic.woff` & `mkdocs_rtd-0.0.9/rtd/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/css/fonts/lato-bold-italic.woff2` & `mkdocs_rtd-0.0.9/rtd/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/css/fonts/lato-bold.woff` & `mkdocs_rtd-0.0.9/rtd/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/css/fonts/lato-bold.woff2` & `mkdocs_rtd-0.0.9/rtd/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/css/fonts/lato-normal-italic.woff` & `mkdocs_rtd-0.0.9/rtd/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/css/fonts/lato-normal-italic.woff2` & `mkdocs_rtd-0.0.9/rtd/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/css/fonts/lato-normal.woff` & `mkdocs_rtd-0.0.9/rtd/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/css/fonts/lato-normal.woff2` & `mkdocs_rtd-0.0.9/rtd/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/css/theme.css` & `mkdocs_rtd-0.0.9/rtd/css/theme.css`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/css/theme_extra.css` & `mkdocs_rtd-0.0.9/rtd/css/theme_extra.css`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/footer.html` & `mkdocs_rtd-0.0.9/rtd/footer.html`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/github_icon.png` & `mkdocs_rtd-0.0.9/rtd/github_icon.png`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/img/favicon.ico` & `mkdocs_rtd-0.0.9/rtd/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/js/html5shiv.min.js` & `mkdocs_rtd-0.0.9/rtd/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/js/jquery-3.6.0.min.js` & `mkdocs_rtd-0.0.9/rtd/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/js/theme.js` & `mkdocs_rtd-0.0.9/rtd/js/theme.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -159,15 +159,15 @@
                     //     }
                     // } catch (n) {
                     //     console.log("Error expanding nav for anchor", n)
                     // }
                 },
                 onScroll: function() {
                     this.winScroll = !1;
-                    if (this.navBar.is(":hover")) {
+                    if (this.navBar.is(":hover") || this.currentItem.length == 0) {
                         return;
                     }
                     var n = this.win.scrollTop(),
                         e = n + this.winHeight,
                         t = Math.min(
                             this.navBar.scrollTop() + (n - this.winPosition),
                             this.navBar.scrollTop() + this.currentItem.position().top - this.searchBarHeight
```

### Comparing `mkdocs_rtd-0.0.8/rtd/js/theme_extra.js` & `mkdocs_rtd-0.0.9/rtd/js/theme_extra.js`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/locales/de/LC_MESSAGES/messages.po` & `mkdocs_rtd-0.0.9/rtd/locales/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/locales/es/LC_MESSAGES/messages.po` & `mkdocs_rtd-0.0.9/rtd/locales/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/locales/fa/LC_MESSAGES/messages.po` & `mkdocs_rtd-0.0.9/rtd/locales/fa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/locales/fr/LC_MESSAGES/messages.po` & `mkdocs_rtd-0.0.9/rtd/locales/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/locales/id/LC_MESSAGES/messages.po` & `mkdocs_rtd-0.0.9/rtd/locales/id/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/locales/it/LC_MESSAGES/messages.po` & `mkdocs_rtd-0.0.9/rtd/locales/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/locales/ja/LC_MESSAGES/messages.po` & `mkdocs_rtd-0.0.9/rtd/locales/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/locales/pt_BR/LC_MESSAGES/messages.po` & `mkdocs_rtd-0.0.9/rtd/locales/pt_BR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/locales/ru/LC_MESSAGES/messages.po` & `mkdocs_rtd-0.0.9/rtd/locales/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/locales/tr/LC_MESSAGES/messages.po` & `mkdocs_rtd-0.0.9/rtd/locales/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/locales/uk/LC_MESSAGES/messages.po` & `mkdocs_rtd-0.0.9/rtd/locales/uk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/locales/zh_CN/LC_MESSAGES/messages.po` & `mkdocs_rtd-0.0.9/rtd/locales/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/locales/zh_TW/LC_MESSAGES/messages.po` & `mkdocs_rtd-0.0.9/rtd/locales/zh_TW/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/nav.html` & `mkdocs_rtd-0.0.9/rtd/nav.html`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/search.html` & `mkdocs_rtd-0.0.9/rtd/search.html`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/rtd/versions.html` & `mkdocs_rtd-0.0.9/rtd/versions.html`

 * *Files identical despite different names*

### Comparing `mkdocs_rtd-0.0.8/setup.py` & `mkdocs_rtd-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
          'locales/zh_TW/LC_MESSAGES/*']}
 
 entry_points = \
 {'mkdocs.themes': ['rtd = rtd']}
 
 setup_kwargs = {
     'name': 'mkdocs-rtd',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'A fork of mkdocs readthedocs theme to make it work with mkapi',
     'long_description': "# mkdocs-rtd\n\nA fork of mkdocs readthedocs theme to make it work better, especially with mkapi.\n\nWhy just use `extra_css` and `extra_javascript`?\n\n- The javascript written in `theme.js` shipped with the original theme has problems expanding the sidebar items and it's not easy to fix it only using `extra_javascript`.\n\n## Installation\n\n```bash\npip install -U mkdocs-rtd\n```\n\n## Usage\n\n```yaml\ntheme:\n  name: rtd\n```\n\nAll options are the same when using the original theme (`readthedocs`). See also:\n<https://www.mkdocs.org/user-guide/choosing-your-theme/#readthedocs>\n\n## Modifications\n\n- Add social icons (only Github supported now) to the top right corner of the page.\n- Adjust some styles\n- Open external links in new tab by default\n- Do not reset side nav items when url hash is `#` or empty\n- Make search box sticky\n- Add css support for `pymdownx.blocks.tab` (must use `alternate_style: true`)\n- Set `ignoreUnescapedHTML` to `true` for `hljs`\n- Keep current sidebar item always in view when scrolling\n",
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mkdocs_rtd-0.0.8/PKG-INFO` & `mkdocs_rtd-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-rtd
-Version: 0.0.8
+Version: 0.0.9
 Summary: A fork of mkdocs readthedocs theme to make it work with mkapi
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

