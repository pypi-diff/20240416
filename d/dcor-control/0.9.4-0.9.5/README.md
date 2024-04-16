# Comparing `tmp/dcor_control-0.9.4.tar.gz` & `tmp/dcor_control-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcor_control-0.9.4.tar", last modified: Thu Jan 18 13:26:09 2024, max compression
+gzip compressed data, was "dcor_control-0.9.5.tar", last modified: Thu Jan 18 13:57:45 2024, max compression
```

## Comparing `dcor_control-0.9.4.tar` & `dcor_control-0.9.5.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:26:09.032665 dcor_control-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-01-18 13:25:27.000000 dcor_control-0.9.4/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-01-18 13:25:27.000000 dcor_control-0.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-01-18 13:25:27.000000 dcor_control-0.9.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9288 2024-01-18 13:26:09.032665 dcor_control-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-01-18 13:25:27.000000 dcor_control-0.9.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:26:09.024665 dcor_control-0.9.4/dcor_control/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-01-18 13:25:48.000000 dcor_control-0.9.4/dcor_control/_version_save.py
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/backup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:26:09.024665 dcor_control-0.9.4/dcor_control/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/cli/backup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/cli/develop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/cli/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/cli/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/cli/reset.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/cli/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:26:09.028665 dcor_control-0.9.4/dcor_control/inspect/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/inspect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/inspect/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     9470 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/inspect/config_ckan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/inspect/config_nginx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/inspect/config_supervisord.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/inspect/config_uwsgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/inspect/data_ckan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:26:09.028665 dcor_control-0.9.4/dcor_control/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:26:09.028665 dcor_control-0.9.4/dcor_control/resources/branding/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/resources/branding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/resources/branding/licenses_medical.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:26:09.028665 dcor_control-0.9.4/dcor_control/resources/branding/public_dcor/
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/resources/branding/public_dcor/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:26:09.028665 dcor_control-0.9.4/dcor_control/resources/branding/public_medical/
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/resources/branding/public_medical/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:26:09.028665 dcor_control-0.9.4/dcor_control/resources/branding/public_medical/images/
--rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/resources/branding/public_medical/images/dcor-076.png
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/resources/branding/public_medical/images/dcor-096.png
--rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/resources/branding/public_medical/images/dcor-152.png
--rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/resources/branding/public_medical/images/dcor-180.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:26:09.028665 dcor_control-0.9.4/dcor_control/resources/branding/public_testing/
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/resources/branding/public_testing/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:26:09.028665 dcor_control-0.9.4/dcor_control/resources/branding/public_testing/images/
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/resources/branding/public_testing/images/dcor-076.png
--rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/resources/branding/public_testing/images/dcor-096.png
--rw-r--r--   0 runner    (1001) docker     (127)    10048 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/resources/branding/public_testing/images/dcor-152.png
--rw-r--r--   0 runner    (1001) docker     (127)    10048 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/resources/branding/public_testing/images/dcor-180.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:26:09.028665 dcor_control-0.9.4/dcor_control/resources/branding/resource_schema_medical/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/resources/branding/resource_schema_medical/supplement1_medical.json
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/resources/branding/resource_schema_medical/supplement2_chip.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:26:09.028665 dcor_control-0.9.4/dcor_control/resources/branding/templates_dcor/
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/resources/branding/templates_dcor/contact.html
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/resources/branding/templates_dcor/imprint.html
--rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/resources/branding/templates_dcor/privacy.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:26:09.024665 dcor_control-0.9.4/dcor_control/resources/branding/templates_medical/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:26:09.024665 dcor_control-0.9.4/dcor_control/resources/branding/templates_medical/home/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:26:09.028665 dcor_control-0.9.4/dcor_control/resources/branding/templates_medical/home/snippets/
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/resources/branding/templates_medical/home/snippets/promoted.html
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/resources/compatible_versions.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/resources/dcor_options.ini
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/resources/server_options.json
--rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/update.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-01-18 13:25:27.000000 dcor_control-0.9.4/dcor_control/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:26:09.024665 dcor_control-0.9.4/dcor_control.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9288 2024-01-18 13:26:08.000000 dcor_control-0.9.4/dcor_control.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-01-18 13:26:08.000000 dcor_control-0.9.4/dcor_control.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 13:26:08.000000 dcor_control-0.9.4/dcor_control.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-18 13:26:08.000000 dcor_control-0.9.4/dcor_control.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-01-18 13:26:08.000000 dcor_control-0.9.4/dcor_control.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-18 13:26:08.000000 dcor_control-0.9.4/dcor_control.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 13:26:09.032665 dcor_control-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-01-18 13:25:27.000000 dcor_control-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:57:45.104915 dcor_control-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-01-18 13:57:17.000000 dcor_control-0.9.5/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-01-18 13:57:17.000000 dcor_control-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-01-18 13:57:17.000000 dcor_control-0.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9288 2024-01-18 13:57:45.104915 dcor_control-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-01-18 13:57:17.000000 dcor_control-0.9.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:57:45.096915 dcor_control-0.9.5/dcor_control/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-01-18 13:57:26.000000 dcor_control-0.9.5/dcor_control/_version_save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/backup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:57:45.100915 dcor_control-0.9.5/dcor_control/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/cli/backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/cli/develop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/cli/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/cli/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/cli/reset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/cli/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:57:45.100915 dcor_control-0.9.5/dcor_control/inspect/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/inspect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/inspect/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9470 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/inspect/config_ckan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/inspect/config_nginx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/inspect/config_supervisord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/inspect/config_uwsgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/inspect/data_ckan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:57:45.100915 dcor_control-0.9.5/dcor_control/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:57:45.100915 dcor_control-0.9.5/dcor_control/resources/branding/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/resources/branding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/resources/branding/licenses_medical.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:57:45.100915 dcor_control-0.9.5/dcor_control/resources/branding/public_dcor/
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/resources/branding/public_dcor/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:57:45.104915 dcor_control-0.9.5/dcor_control/resources/branding/public_medical/
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/resources/branding/public_medical/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:57:45.104915 dcor_control-0.9.5/dcor_control/resources/branding/public_medical/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/resources/branding/public_medical/images/dcor-076.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/resources/branding/public_medical/images/dcor-096.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/resources/branding/public_medical/images/dcor-152.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/resources/branding/public_medical/images/dcor-180.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:57:45.104915 dcor_control-0.9.5/dcor_control/resources/branding/public_testing/
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/resources/branding/public_testing/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:57:45.104915 dcor_control-0.9.5/dcor_control/resources/branding/public_testing/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/resources/branding/public_testing/images/dcor-076.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/resources/branding/public_testing/images/dcor-096.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10048 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/resources/branding/public_testing/images/dcor-152.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10048 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/resources/branding/public_testing/images/dcor-180.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:57:45.104915 dcor_control-0.9.5/dcor_control/resources/branding/resource_schema_medical/
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/resources/branding/resource_schema_medical/supplement1_medical.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/resources/branding/resource_schema_medical/supplement2_chip.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:57:45.104915 dcor_control-0.9.5/dcor_control/resources/branding/templates_dcor/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/resources/branding/templates_dcor/contact.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/resources/branding/templates_dcor/imprint.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/resources/branding/templates_dcor/privacy.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:57:45.096915 dcor_control-0.9.5/dcor_control/resources/branding/templates_medical/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:57:45.096915 dcor_control-0.9.5/dcor_control/resources/branding/templates_medical/home/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:57:45.104915 dcor_control-0.9.5/dcor_control/resources/branding/templates_medical/home/snippets/
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/resources/branding/templates_medical/home/snippets/promoted.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/resources/compatible_versions.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/resources/dcor_options.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/resources/server_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-01-18 13:57:17.000000 dcor_control-0.9.5/dcor_control/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:57:45.100915 dcor_control-0.9.5/dcor_control.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9288 2024-01-18 13:57:45.000000 dcor_control-0.9.5/dcor_control.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-01-18 13:57:45.000000 dcor_control-0.9.5/dcor_control.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 13:57:45.000000 dcor_control-0.9.5/dcor_control.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-18 13:57:45.000000 dcor_control-0.9.5/dcor_control.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-01-18 13:57:45.000000 dcor_control-0.9.5/dcor_control.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-18 13:57:45.000000 dcor_control-0.9.5/dcor_control.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 13:57:45.104915 dcor_control-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-01-18 13:57:17.000000 dcor_control-0.9.5/setup.py
```

### Comparing `dcor_control-0.9.4/CHANGELOG` & `dcor_control-0.9.5/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+0.9.5
+ - enh: properly check for nginx status before attempting to reload
 0.9.4
  - maintenance release
 0.9.3
  - enh: add dcor_control to compatible version list
  - cleanup
 0.9.2
  - fix: fix compatible versions header
```

### Comparing `dcor_control-0.9.4/LICENSE` & `dcor_control-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dcor_control-0.9.4/PKG-INFO` & `dcor_control-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcor_control
-Version: 0.9.4
+Version: 0.9.5
 Summary: CLI for maintaining DCOR installations
 Home-page: https://github.com/DCOR-dev/dcor_control/
 Author: Paul Müller
 Author-email: dev@craban.de
 License: GPLv3+
 Keywords: RT-DC,DCOR
 Platform: UNKNOWN
```

### Comparing `dcor_control-0.9.4/README.rst` & `dcor_control-0.9.5/README.rst`

 * *Files identical despite different names*

### Comparing `dcor_control-0.9.4/dcor_control/_version.py` & `dcor_control-0.9.5/dcor_control/_version.py`

 * *Files identical despite different names*

### Comparing `dcor_control-0.9.4/dcor_control/backup.py` & `dcor_control-0.9.5/dcor_control/backup.py`

 * *Files identical despite different names*

### Comparing `dcor_control-0.9.4/dcor_control/cli/backup.py` & `dcor_control-0.9.5/dcor_control/cli/backup.py`

 * *Files identical despite different names*

### Comparing `dcor_control-0.9.4/dcor_control/cli/develop.py` & `dcor_control-0.9.5/dcor_control/cli/develop.py`

 * *Files identical despite different names*

### Comparing `dcor_control-0.9.4/dcor_control/cli/info.py` & `dcor_control-0.9.5/dcor_control/cli/info.py`

 * *Files identical despite different names*

### Comparing `dcor_control-0.9.4/dcor_control/cli/inspect.py` & `dcor_control-0.9.5/dcor_control/cli/inspect.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import subprocess as sp
-
 import click
 from dcor_shared import paths
 
 from .. import inspect as inspect_mod
 
 
 @click.command()
@@ -55,15 +53,14 @@
         autocorrect=assume_yes)
 
     click.secho("Checking uwsgi configuration...", bold=True)
     inspect_mod.check_uwsgi(harakiri=7200, autocorrect=assume_yes)
 
     inspect_mod.reload_supervisord()
 
-    click.secho("Reloading nginx...", bold=True)
-    sp.check_output("systemctl reload nginx", shell=True)
+    inspect_mod.reload_nginx()
 
     # ask the user whether to search for orphaned files
     if assume_yes or click.confirm('Perform search for orphaned files?'):
         inspect_mod.check_orphaned_files(assume_yes=assume_yes)
 
     click.secho('DONE', fg=u'green', bold=True)
```

### Comparing `dcor_control-0.9.4/dcor_control/cli/reset.py` & `dcor_control-0.9.5/dcor_control/cli/reset.py`

 * *Files identical despite different names*

### Comparing `dcor_control-0.9.4/dcor_control/cli/update.py` & `dcor_control-0.9.5/dcor_control/cli/update.py`

 * *Files identical despite different names*

### Comparing `dcor_control-0.9.4/dcor_control/inspect/common.py` & `dcor_control-0.9.5/dcor_control/inspect/common.py`

 * *Files identical despite different names*

### Comparing `dcor_control-0.9.4/dcor_control/inspect/config_ckan.py` & `dcor_control-0.9.5/dcor_control/inspect/config_ckan.py`

 * *Files identical despite different names*

### Comparing `dcor_control-0.9.4/dcor_control/inspect/config_nginx.py` & `dcor_control-0.9.5/dcor_control/inspect/config_nginx.py`

 * *Files identical despite different names*

### Comparing `dcor_control-0.9.4/dcor_control/inspect/config_supervisord.py` & `dcor_control-0.9.5/dcor_control/inspect/config_supervisord.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,24 +24,43 @@
                     "[program:ckan-ckan-worker-dcor-{}]".format(worker))
                 data = data.replace(
                     "/ckan.ini jobs worker",
                     "/ckan.ini jobs worker dcor-{}".format(worker))
                 wpath.write_text(data)
 
 
+def is_nginx_running():
+    """Simple check for whether supervisord is running"""
+    try:
+        sp.check_output("sudo systemctl status nginx", shell=True)
+    except sp.CalledProcessError:
+        return False
+    else:
+        return True
+
+
 def is_supervisord_running():
     """Simple check for whether supervisord is running"""
     try:
         sp.check_output("sudo supervisorctl status", shell=True)
     except sp.CalledProcessError:
         return False
     else:
         return True
 
 
+def reload_nginx():
+    if is_nginx_running():
+        click.secho("Reloading nginx...", bold=True)
+        sp.check_output("sudo systemctl reload nginx", shell=True)
+    else:
+        click.secho("Not reloading nginx (not running)...",
+                    bold=True, fg="red")
+
+
 def reload_supervisord():
     if is_supervisord_running():
         click.secho("Reloading CKAN...", bold=True)
         sp.check_output("sudo supervisorctl reload", shell=True)
     else:
         click.secho("Not reloading CKAN (supervisord not running)...",
                     bold=True, fg="red")
```

### Comparing `dcor_control-0.9.4/dcor_control/inspect/config_uwsgi.py` & `dcor_control-0.9.5/dcor_control/inspect/config_uwsgi.py`

 * *Files identical despite different names*

### Comparing `dcor_control-0.9.4/dcor_control/inspect/data_ckan.py` & `dcor_control-0.9.5/dcor_control/inspect/data_ckan.py`

 * *Files identical despite different names*

### Comparing `dcor_control-0.9.4/dcor_control/resources/branding/licenses_medical.json` & `dcor_control-0.9.5/dcor_control/resources/branding/licenses_medical.json`

 * *Files identical despite different names*

### Comparing `dcor_control-0.9.4/dcor_control/resources/branding/public_dcor/favicon.ico` & `dcor_control-0.9.5/dcor_control/resources/branding/public_dcor/favicon.ico`

 * *Files identical despite different names*

### Comparing `dcor_control-0.9.4/dcor_control/resources/branding/public_medical/favicon.ico` & `dcor_control-0.9.5/dcor_control/resources/branding/public_medical/favicon.ico`

 * *Files identical despite different names*

### Comparing `dcor_control-0.9.4/dcor_control/resources/branding/public_medical/images/dcor-076.png` & `dcor_control-0.9.5/dcor_control/resources/branding/public_medical/images/dcor-076.png`

 * *Files identical despite different names*

### Comparing `dcor_control-0.9.4/dcor_control/resources/branding/public_medical/images/dcor-096.png` & `dcor_control-0.9.5/dcor_control/resources/branding/public_medical/images/dcor-096.png`

 * *Files identical despite different names*

### Comparing `dcor_control-0.9.4/dcor_control/resources/branding/public_medical/images/dcor-152.png` & `dcor_control-0.9.5/dcor_control/resources/branding/public_medical/images/dcor-152.png`

 * *Files identical despite different names*

### Comparing `dcor_control-0.9.4/dcor_control/resources/branding/public_medical/images/dcor-180.png` & `dcor_control-0.9.5/dcor_control/resources/branding/public_medical/images/dcor-180.png`

 * *Files identical despite different names*

### Comparing `dcor_control-0.9.4/dcor_control/resources/branding/public_testing/favicon.ico` & `dcor_control-0.9.5/dcor_control/resources/branding/public_testing/favicon.ico`

 * *Files identical despite different names*

### Comparing `dcor_control-0.9.4/dcor_control/resources/branding/public_testing/images/dcor-076.png` & `dcor_control-0.9.5/dcor_control/resources/branding/public_testing/images/dcor-076.png`

 * *Files identical despite different names*

### Comparing `dcor_control-0.9.4/dcor_control/resources/branding/public_testing/images/dcor-096.png` & `dcor_control-0.9.5/dcor_control/resources/branding/public_testing/images/dcor-096.png`

 * *Files identical despite different names*

### Comparing `dcor_control-0.9.4/dcor_control/resources/branding/public_testing/images/dcor-152.png` & `dcor_control-0.9.5/dcor_control/resources/branding/public_testing/images/dcor-152.png`

 * *Files identical despite different names*

### Comparing `dcor_control-0.9.4/dcor_control/resources/branding/public_testing/images/dcor-180.png` & `dcor_control-0.9.5/dcor_control/resources/branding/public_testing/images/dcor-180.png`

 * *Files identical despite different names*

### Comparing `dcor_control-0.9.4/dcor_control/resources/branding/resource_schema_medical/supplement1_medical.json` & `dcor_control-0.9.5/dcor_control/resources/branding/resource_schema_medical/supplement1_medical.json`

 * *Files identical despite different names*

### Comparing `dcor_control-0.9.4/dcor_control/resources/branding/resource_schema_medical/supplement2_chip.json` & `dcor_control-0.9.5/dcor_control/resources/branding/resource_schema_medical/supplement2_chip.json`

 * *Files identical despite different names*

### Comparing `dcor_control-0.9.4/dcor_control/resources/branding/templates_dcor/imprint.html` & `dcor_control-0.9.5/dcor_control/resources/branding/templates_dcor/imprint.html`

 * *Files identical despite different names*

### Comparing `dcor_control-0.9.4/dcor_control/resources/branding/templates_dcor/privacy.html` & `dcor_control-0.9.5/dcor_control/resources/branding/templates_dcor/privacy.html`

 * *Files identical despite different names*

### Comparing `dcor_control-0.9.4/dcor_control/resources/branding/templates_medical/home/snippets/promoted.html` & `dcor_control-0.9.5/dcor_control/resources/branding/templates_medical/home/snippets/promoted.html`

 * *Files identical despite different names*

### Comparing `dcor_control-0.9.4/dcor_control/resources/compatible_versions.txt` & `dcor_control-0.9.5/dcor_control/resources/compatible_versions.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 ckan      ckanext-dc_log_view  ckanext-dc_serve  ckanext-dc_view  ckanext-dcor_depot  ckanext-dcor_schemas  ckanext-dcor_theme  dcor_control  dcor_shared
+2.10.3    0.3.3                0.14.1            0.8.2            0.13.8              0.18.11               0.7.7               0.9.4         0.5.6
 2.10.3    0.3.2                0.14.0            0.8.1            0.13.7              0.18.10               0.7.6               0.9.3         0.5.5
 2.10.1    0.3.2                0.14.0            0.8.1            0.13.7              0.18.9                0.7.6               0.9.3         0.5.5
 2.10.1    0.3.2                0.13.11           0.8.0            0.13.6              0.18.9                0.7.6               0.9.3         0.5.4
 2.10.1    0.3.1                0.13.2            0.7.1            0.13.4              0.18.7                0.7.5               0.9.3         0.5.2
 2.10.1    0.3.1                0.13.0            0.7.1            0.13.3              0.18.6                0.7.5               0.9.3         0.5.2
 2.10.1    0.3.1                0.12.2            0.7.1            0.13.0              0.18.6                0.7.4               0.9.3         0.4.4
 2.10.1    0.3.1                0.12.2            0.7.1            0.12.1              0.18.4                0.7.4               0.9.3         0.4.3
```

### Comparing `dcor_control-0.9.4/dcor_control/resources/dcor_options.ini` & `dcor_control-0.9.5/dcor_control/resources/dcor_options.ini`

 * *Files identical despite different names*

### Comparing `dcor_control-0.9.4/dcor_control/resources/server_options.json` & `dcor_control-0.9.5/dcor_control/resources/server_options.json`

 * *Files identical despite different names*

### Comparing `dcor_control-0.9.4/dcor_control/update.py` & `dcor_control-0.9.5/dcor_control/update.py`

 * *Files identical despite different names*

### Comparing `dcor_control-0.9.4/dcor_control/util.py` & `dcor_control-0.9.5/dcor_control/util.py`

 * *Files identical despite different names*

### Comparing `dcor_control-0.9.4/dcor_control.egg-info/PKG-INFO` & `dcor_control-0.9.5/dcor_control.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcor-control
-Version: 0.9.4
+Version: 0.9.5
 Summary: CLI for maintaining DCOR installations
 Home-page: https://github.com/DCOR-dev/dcor_control/
 Author: Paul Müller
 Author-email: dev@craban.de
 License: GPLv3+
 Keywords: RT-DC,DCOR
 Platform: UNKNOWN
```

### Comparing `dcor_control-0.9.4/dcor_control.egg-info/SOURCES.txt` & `dcor_control-0.9.5/dcor_control.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcor_control-0.9.4/setup.py` & `dcor_control-0.9.5/setup.py`

 * *Files identical despite different names*

