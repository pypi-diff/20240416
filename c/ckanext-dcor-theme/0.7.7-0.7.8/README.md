# Comparing `tmp/ckanext-dcor_theme-0.7.7.tar.gz` & `tmp/ckanext-dcor_theme-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-dcor_theme-0.7.7.tar", last modified: Thu Jan 18 13:39:05 2024, max compression
+gzip compressed data, was "ckanext-dcor_theme-0.7.8.tar", last modified: Tue Apr 16 10:40:20 2024, max compression
```

## Comparing `ckanext-dcor_theme-0.7.7.tar` & `ckanext-dcor_theme-0.7.8.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:39:05.951528 ckanext-dcor_theme-0.7.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-01-18 13:39:05.951528 ckanext-dcor_theme-0.7.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:39:05.927528 ckanext-dcor_theme-0.7.7/ckanext/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:39:05.931528 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-01-18 13:39:03.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/_version_save.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:39:05.931528 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/assets/hide_action_buttons.css
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/assets/webassets.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:39:05.931528 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/assets_theme/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/assets_theme/webassets.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:39:05.931528 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/cli/i18n_branding.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/cli/main_css_branding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:39:05.931528 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/css/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/css/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/css/dcor_theme.css
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/css/lato_fonts.css
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/css/make_dcor_main_css.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:39:05.927528 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:39:05.927528 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/base/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:39:05.931528 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/base/images/
--rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/base/images/background-tile.png
--rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/base/images/ckan-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/base/images/placeholder-group.png
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/base/images/placeholder-organization.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:39:05.943528 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   256056 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/fonts/Lato-Bold.eot
--rw-r--r--   0 runner    (1001) docker     (127)   600856 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/fonts/Lato-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   309728 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/fonts/Lato-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (127)   184912 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/fonts/Lato-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   266158 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/fonts/Lato-BoldItalic.eot
--rw-r--r--   0 runner    (1001) docker     (127)   622572 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/fonts/Lato-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   323344 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/fonts/Lato-BoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (127)   193308 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/fonts/Lato-BoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   268604 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/fonts/Lato-Italic.eot
--rw-r--r--   0 runner    (1001) docker     (127)   639388 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/fonts/Lato-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   328412 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/fonts/Lato-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (127)   195704 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/fonts/Lato-Italic.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   253461 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/fonts/Lato-Regular.eot
--rw-r--r--   0 runner    (1001) docker     (127)   607720 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/fonts/Lato-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   309192 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/fonts/Lato-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)   182708 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/fonts/Lato-Regular.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)     4494 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/fonts/OFL.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:39:05.947528 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/images/
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/images/dcor-076.png
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/images/dcor-096.png
--rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/images/dcor-152.png
--rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/images/dcor-180.png
--rw-r--r--   0 runner    (1001) docker     (127)  3398816 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/images/dcor_tiles.png
--rw-r--r--   0 runner    (1001) docker     (127)    42274 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/images/dcor_tiles_420.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:39:05.947528 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/templates/contact.html
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/templates/footer.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:39:05.927528 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/templates/group/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:39:05.947528 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/templates/group/snippets/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/templates/group/snippets/helper.html
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/templates/header.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:39:05.927528 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/templates/home/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:39:05.947528 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/templates/home/snippets/
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/templates/home/snippets/promoted.html
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/templates/imprint.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:39:05.927528 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/templates/organization/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:39:05.947528 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/templates/organization/snippets/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/templates/organization/snippets/helper.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:39:05.947528 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/templates/package/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/templates/package/read_base.html
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/templates/package/resource_read.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:39:05.951528 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/templates/package/snippets/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/templates/package/snippets/resource_view.html
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/templates/privacy.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:39:05.951528 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/templates/snippets/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/templates/snippets/social.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:39:05.951528 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/tests/test_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:39:05.951528 ckanext-dcor_theme-0.7.7/ckanext_dcor_theme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-01-18 13:39:05.000000 ckanext-dcor_theme-0.7.7/ckanext_dcor_theme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-01-18 13:39:05.000000 ckanext-dcor_theme-0.7.7/ckanext_dcor_theme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 13:39:05.000000 ckanext-dcor_theme-0.7.7/ckanext_dcor_theme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-01-18 13:39:05.000000 ckanext-dcor_theme-0.7.7/ckanext_dcor_theme.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-18 13:39:05.000000 ckanext-dcor_theme-0.7.7/ckanext_dcor_theme.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-18 13:39:05.000000 ckanext-dcor_theme-0.7.7/ckanext_dcor_theme.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-18 13:39:05.000000 ckanext-dcor_theme-0.7.7/ckanext_dcor_theme.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 13:39:05.951528 ckanext-dcor_theme-0.7.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-01-18 13:38:54.000000 ckanext-dcor_theme-0.7.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:20.319919 ckanext-dcor_theme-0.7.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-16 10:40:08.000000 ckanext-dcor_theme-0.7.8/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-16 10:40:08.000000 ckanext-dcor_theme-0.7.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-16 10:40:08.000000 ckanext-dcor_theme-0.7.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-16 10:40:20.315919 ckanext-dcor_theme-0.7.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-16 10:40:08.000000 ckanext-dcor_theme-0.7.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:20.295919 ckanext-dcor_theme-0.7.8/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-16 10:40:08.000000 ckanext-dcor_theme-0.7.8/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:20.295919 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-16 10:40:08.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-04-16 10:40:08.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-16 10:40:18.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/_version_save.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:20.295919 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-16 10:40:08.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/assets/hide_action_buttons.css
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-16 10:40:08.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/assets/webassets.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:20.295919 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/assets_theme/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-16 10:40:08.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/assets_theme/webassets.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:20.295919 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-16 10:40:08.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-16 10:40:08.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/cli/i18n_branding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-16 10:40:08.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/cli/main_css_branding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-16 10:40:08.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:20.299919 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/css/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-16 10:40:08.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/css/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-16 10:40:08.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/css/dcor_theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-16 10:40:08.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/css/lato_fonts.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-16 10:40:08.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/css/make_dcor_main_css.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-16 10:40:08.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:20.295919 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:20.295919 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/base/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:20.299919 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/base/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-04-16 10:40:08.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/base/images/background-tile.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-04-16 10:40:08.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/base/images/ckan-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-16 10:40:08.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/base/images/placeholder-group.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-16 10:40:08.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/base/images/placeholder-organization.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:20.307919 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   256056 2024-04-16 10:40:08.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/fonts/Lato-Bold.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   600856 2024-04-16 10:40:08.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/fonts/Lato-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   309728 2024-04-16 10:40:08.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/fonts/Lato-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   184912 2024-04-16 10:40:08.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/fonts/Lato-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   266158 2024-04-16 10:40:08.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/fonts/Lato-BoldItalic.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   622572 2024-04-16 10:40:08.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/fonts/Lato-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   323344 2024-04-16 10:40:09.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/fonts/Lato-BoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   193308 2024-04-16 10:40:09.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/fonts/Lato-BoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   268604 2024-04-16 10:40:09.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/fonts/Lato-Italic.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   639388 2024-04-16 10:40:09.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/fonts/Lato-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   328412 2024-04-16 10:40:09.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/fonts/Lato-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   195704 2024-04-16 10:40:09.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/fonts/Lato-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   253461 2024-04-16 10:40:09.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/fonts/Lato-Regular.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   607720 2024-04-16 10:40:09.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/fonts/Lato-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   309192 2024-04-16 10:40:09.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/fonts/Lato-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   182708 2024-04-16 10:40:09.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/fonts/Lato-Regular.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4494 2024-04-16 10:40:09.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/fonts/OFL.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:20.315919 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-04-16 10:40:09.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/images/dcor-076.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-16 10:40:09.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/images/dcor-096.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-04-16 10:40:09.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/images/dcor-152.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-04-16 10:40:09.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/images/dcor-180.png
+-rw-r--r--   0 runner    (1001) docker     (127)  3398816 2024-04-16 10:40:09.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/images/dcor_tiles.png
+-rw-r--r--   0 runner    (1001) docker     (127)    42274 2024-04-16 10:40:09.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/images/dcor_tiles_420.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:20.315919 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-16 10:40:09.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-16 10:40:09.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/templates/contact.html
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-16 10:40:09.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/templates/footer.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:20.295919 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/templates/group/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:20.315919 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/templates/group/snippets/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-16 10:40:09.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/templates/group/snippets/helper.html
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-16 10:40:09.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/templates/header.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:20.295919 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/templates/home/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:20.315919 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/templates/home/snippets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-16 10:40:09.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/templates/home/snippets/promoted.html
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-16 10:40:09.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/templates/imprint.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:20.295919 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/templates/organization/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:20.315919 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/templates/organization/snippets/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-16 10:40:09.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/templates/organization/snippets/helper.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:20.315919 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/templates/package/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-16 10:40:09.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/templates/package/read_base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-16 10:40:09.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/templates/package/resource_read.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:20.315919 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/templates/package/snippets/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-16 10:40:09.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/templates/package/snippets/resource_view.html
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-16 10:40:09.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/templates/privacy.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:20.315919 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/templates/snippets/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-16 10:40:09.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/templates/snippets/social.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:20.315919 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:09.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-16 10:40:09.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-16 10:40:09.000000 ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/tests/test_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:20.315919 ckanext-dcor_theme-0.7.8/ckanext_dcor_theme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-16 10:40:20.000000 ckanext-dcor_theme-0.7.8/ckanext_dcor_theme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-16 10:40:20.000000 ckanext-dcor_theme-0.7.8/ckanext_dcor_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 10:40:20.000000 ckanext-dcor_theme-0.7.8/ckanext_dcor_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-16 10:40:20.000000 ckanext-dcor_theme-0.7.8/ckanext_dcor_theme.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-16 10:40:20.000000 ckanext-dcor_theme-0.7.8/ckanext_dcor_theme.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-16 10:40:20.000000 ckanext-dcor_theme-0.7.8/ckanext_dcor_theme.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-16 10:40:20.000000 ckanext-dcor_theme-0.7.8/ckanext_dcor_theme.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 10:40:20.319919 ckanext-dcor_theme-0.7.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-16 10:40:09.000000 ckanext-dcor_theme-0.7.8/setup.py
```

### Comparing `ckanext-dcor_theme-0.7.7/CHANGELOG` & `ckanext-dcor_theme-0.7.8/CHANGELOG`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+0.7.8
+ - maintenance release
 0.7.7
  - maintenance release
 0.7.6
  - maintenance release
 0.7.5
  - enh: update color replacement
 0.7.4
```

### Comparing `ckanext-dcor_theme-0.7.7/LICENSE` & `ckanext-dcor_theme-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/PKG-INFO` & `ckanext-dcor_theme-0.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-dcor_theme
-Version: 0.7.7
+Version: 0.7.8
 Summary: The DCOR CKAN theme
 Home-page: https://github.com/DCOR-dev/ckanext-dcor_theme
 Author: Paul Müller
 Author-email: dev@craban.de
 License: AGPLv3+
 Keywords: CKAN,DCOR,RT-DC
 Platform: UNKNOWN
```

### Comparing `ckanext-dcor_theme-0.7.7/README.rst` & `ckanext-dcor_theme-0.7.8/README.rst`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/_version.py` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/_version.py`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/cli/i18n_branding.py` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/cli/i18n_branding.py`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/cli.py` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/cli.py`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/css/dcor_theme.css` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/css/dcor_theme.css`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/css/lato_fonts.css` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/css/lato_fonts.css`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/css/make_dcor_main_css.py` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/css/make_dcor_main_css.py`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/plugin.py` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/base/images/background-tile.png` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/base/images/background-tile.png`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/base/images/ckan-logo.png` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/base/images/ckan-logo.png`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/base/images/placeholder-group.png` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/base/images/placeholder-group.png`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/base/images/placeholder-organization.png` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/base/images/placeholder-organization.png`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/fonts/Lato-Bold.eot` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/fonts/Lato-Bold.eot`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/fonts/Lato-Bold.ttf` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/fonts/Lato-Bold.ttf`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/fonts/Lato-Bold.woff` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/fonts/Lato-Bold.woff`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/fonts/Lato-Bold.woff2` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/fonts/Lato-Bold.woff2`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/fonts/Lato-BoldItalic.eot` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/fonts/Lato-BoldItalic.eot`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/fonts/Lato-BoldItalic.ttf` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/fonts/Lato-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/fonts/Lato-BoldItalic.woff` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/fonts/Lato-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/fonts/Lato-BoldItalic.woff2` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/fonts/Lato-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/fonts/Lato-Italic.eot` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/fonts/Lato-Italic.eot`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/fonts/Lato-Italic.ttf` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/fonts/Lato-Italic.ttf`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/fonts/Lato-Italic.woff` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/fonts/Lato-Italic.woff`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/fonts/Lato-Italic.woff2` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/fonts/Lato-Italic.woff2`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/fonts/Lato-Regular.eot` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/fonts/Lato-Regular.eot`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/fonts/Lato-Regular.ttf` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/fonts/Lato-Regular.woff` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/fonts/Lato-Regular.woff`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/fonts/Lato-Regular.woff2` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/fonts/Lato-Regular.woff2`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/fonts/OFL.txt` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/fonts/OFL.txt`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/images/dcor-076.png` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/images/dcor-076.png`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/images/dcor-096.png` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/images/dcor-096.png`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/images/dcor-152.png` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/images/dcor-152.png`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/images/dcor-180.png` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/images/dcor-180.png`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/images/dcor_tiles.png` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/images/dcor_tiles.png`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/public/images/dcor_tiles_420.jpg` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/public/images/dcor_tiles_420.jpg`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/templates/base.html` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/templates/base.html`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/templates/footer.html` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/templates/footer.html`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/templates/group/snippets/helper.html` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/templates/group/snippets/helper.html`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/templates/header.html` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/templates/header.html`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/templates/home/snippets/promoted.html` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/templates/home/snippets/promoted.html`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/templates/organization/snippets/helper.html` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/templates/organization/snippets/helper.html`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext/dcor_theme/templates/package/resource_read.html` & `ckanext-dcor_theme-0.7.8/ckanext/dcor_theme/templates/package/resource_read.html`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/ckanext_dcor_theme.egg-info/PKG-INFO` & `ckanext-dcor_theme-0.7.8/ckanext_dcor_theme.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-dcor-theme
-Version: 0.7.7
+Version: 0.7.8
 Summary: The DCOR CKAN theme
 Home-page: https://github.com/DCOR-dev/ckanext-dcor_theme
 Author: Paul Müller
 Author-email: dev@craban.de
 License: AGPLv3+
 Keywords: CKAN,DCOR,RT-DC
 Platform: UNKNOWN
```

### Comparing `ckanext-dcor_theme-0.7.7/ckanext_dcor_theme.egg-info/SOURCES.txt` & `ckanext-dcor_theme-0.7.8/ckanext_dcor_theme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_theme-0.7.7/setup.py` & `ckanext-dcor_theme-0.7.8/setup.py`

 * *Files identical despite different names*

