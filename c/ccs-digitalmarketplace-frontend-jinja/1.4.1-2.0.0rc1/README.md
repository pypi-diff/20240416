# Comparing `tmp/ccs-digitalmarketplace-frontend-jinja-1.4.1.tar.gz` & `tmp/ccs-digitalmarketplace-frontend-jinja-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccs-digitalmarketplace-frontend-jinja-1.4.1.tar", last modified: Tue Apr  9 14:01:14 2024, max compression
+gzip compressed data, was "ccs-digitalmarketplace-frontend-jinja-2.0.0rc1.tar", last modified: Tue Apr 16 12:38:03 2024, max compression
```

## Comparing `ccs-digitalmarketplace-frontend-jinja-1.4.1.tar` & `ccs-digitalmarketplace-frontend-jinja-2.0.0rc1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:01:14.596011 ccs-digitalmarketplace-frontend-jinja-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-09 14:01:06.000000 ccs-digitalmarketplace-frontend-jinja-1.4.1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-09 14:01:14.592011 ccs-digitalmarketplace-frontend-jinja-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6420 2024-04-09 14:01:06.000000 ccs-digitalmarketplace-frontend-jinja-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:01:14.592011 ccs-digitalmarketplace-frontend-jinja-1.4.1/app/
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-09 14:01:06.000000 ccs-digitalmarketplace-frontend-jinja-1.4.1/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:01:14.592011 ccs-digitalmarketplace-frontend-jinja-1.4.1/ccs_digitalmarketplace_frontend_jinja.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-09 14:01:14.000000 ccs-digitalmarketplace-frontend-jinja-1.4.1/ccs_digitalmarketplace_frontend_jinja.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-09 14:01:14.000000 ccs-digitalmarketplace-frontend-jinja-1.4.1/ccs_digitalmarketplace_frontend_jinja.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:01:14.000000 ccs-digitalmarketplace-frontend-jinja-1.4.1/ccs_digitalmarketplace_frontend_jinja.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-09 14:01:14.000000 ccs-digitalmarketplace-frontend-jinja-1.4.1/ccs_digitalmarketplace_frontend_jinja.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 14:01:14.000000 ccs-digitalmarketplace-frontend-jinja-1.4.1/ccs_digitalmarketplace_frontend_jinja.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:01:14.592011 ccs-digitalmarketplace-frontend-jinja-1.4.1/digitalmarketplace_frontend_jinja/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 14:01:06.000000 ccs-digitalmarketplace-frontend-jinja-1.4.1/digitalmarketplace_frontend_jinja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 14:01:14.596011 ccs-digitalmarketplace-frontend-jinja-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-09 14:01:06.000000 ccs-digitalmarketplace-frontend-jinja-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:38:03.972291 ccs-digitalmarketplace-frontend-jinja-2.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-16 12:37:54.000000 ccs-digitalmarketplace-frontend-jinja-2.0.0rc1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-16 12:38:03.972291 ccs-digitalmarketplace-frontend-jinja-2.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6643 2024-04-16 12:37:54.000000 ccs-digitalmarketplace-frontend-jinja-2.0.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:38:03.968291 ccs-digitalmarketplace-frontend-jinja-2.0.0rc1/app/
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-16 12:37:54.000000 ccs-digitalmarketplace-frontend-jinja-2.0.0rc1/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:38:03.972291 ccs-digitalmarketplace-frontend-jinja-2.0.0rc1/ccs_digitalmarketplace_frontend_jinja.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-16 12:38:03.000000 ccs-digitalmarketplace-frontend-jinja-2.0.0rc1/ccs_digitalmarketplace_frontend_jinja.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-16 12:38:03.000000 ccs-digitalmarketplace-frontend-jinja-2.0.0rc1/ccs_digitalmarketplace_frontend_jinja.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 12:38:03.000000 ccs-digitalmarketplace-frontend-jinja-2.0.0rc1/ccs_digitalmarketplace_frontend_jinja.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-16 12:38:03.000000 ccs-digitalmarketplace-frontend-jinja-2.0.0rc1/ccs_digitalmarketplace_frontend_jinja.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 12:38:03.000000 ccs-digitalmarketplace-frontend-jinja-2.0.0rc1/ccs_digitalmarketplace_frontend_jinja.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:38:03.972291 ccs-digitalmarketplace-frontend-jinja-2.0.0rc1/digitalmarketplace_frontend_jinja/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-16 12:37:54.000000 ccs-digitalmarketplace-frontend-jinja-2.0.0rc1/digitalmarketplace_frontend_jinja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 12:38:03.972291 ccs-digitalmarketplace-frontend-jinja-2.0.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-16 12:37:54.000000 ccs-digitalmarketplace-frontend-jinja-2.0.0rc1/setup.py
```

### Comparing `ccs-digitalmarketplace-frontend-jinja-1.4.1/LICENCE` & `ccs-digitalmarketplace-frontend-jinja-2.0.0rc1/LICENCE`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-1.4.1/README.md` & `ccs-digitalmarketplace-frontend-jinja-2.0.0rc1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 ## Compatibility
 
 The following table shows the version of Digital Marketplace Frontend Jinja that you should use for your targeted version of CCS Digital Marketplace GOV.UK Frontend:
 
 | Digital Marketplace Frontend Jinja Version | Target CCS Digital Marketplace GOV.UK Frontend Version |
 | ----------------------------- | ------------------------------ |
+| [2.0.0rc1](https://github.com/tim-s-ccs/ccs-digitalmarketplace-frontend-jinja/releases/tag/2.0.0rc1) | [6.0.0rc2](https://github.com/Crown-Commercial-Service/ccs-digitalmarketplace-govuk-frontend/releases/tag/6.0.0rc2) |
 | [1.4.1](https://github.com/tim-s-ccs/ccs-digitalmarketplace-frontend-jinja/releases/tag/1.4.1) | [5.5.0](https://github.com/Crown-Commercial-Service/ccs-digitalmarketplace-govuk-frontend/releases/tag/5.5.0) |
 | [1.4.0](https://github.com/tim-s-ccs/ccs-digitalmarketplace-frontend-jinja/releases/tag/1.4.0) | [5.5.0](https://github.com/Crown-Commercial-Service/ccs-digitalmarketplace-govuk-frontend/releases/tag/5.5.0) |
 | [1.3.3](https://github.com/tim-s-ccs/ccs-digitalmarketplace-frontend-jinja/releases/tag/1.3.3) | [5.4.3](https://github.com/Crown-Commercial-Service/ccs-digitalmarketplace-govuk-frontend/releases/tag/5.4.3) |
 | [1.3.2](https://github.com/tim-s-ccs/ccs-digitalmarketplace-frontend-jinja/releases/tag/1.3.2) | [5.4.2](https://github.com/Crown-Commercial-Service/ccs-digitalmarketplace-govuk-frontend/releases/tag/5.4.2) |
 | [1.3.1](https://github.com/tim-s-ccs/ccs-digitalmarketplace-frontend-jinja/releases/tag/1.3.1) | [5.4.1](https://github.com/Crown-Commercial-Service/ccs-digitalmarketplace-govuk-frontend/releases/tag/5.4.1) |
 | [1.3.0](https://github.com/tim-s-ccs/ccs-digitalmarketplace-frontend-jinja/releases/tag/1.3.0) | [5.4.0](https://github.com/Crown-Commercial-Service/ccs-digitalmarketplace-govuk-frontend/releases/tag/5.4.0) |
 | [1.2.0](https://github.com/tim-s-ccs/ccs-digitalmarketplace-frontend-jinja/releases/tag/1.2.0) | [5.2.0](https://github.com/Crown-Commercial-Service/ccs-digitalmarketplace-govuk-frontend/releases/tag/5.2.0) |
```

### Comparing `ccs-digitalmarketplace-frontend-jinja-1.4.1/app/__init__.py` & `ccs-digitalmarketplace-frontend-jinja-2.0.0rc1/app/__init__.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-1.4.1/setup.py` & `ccs-digitalmarketplace-frontend-jinja-2.0.0rc1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,12 +27,12 @@
     description='Jinja templates for Digital Marketplace apps.',
     long_description=__doc__,
     packages=find_packages(),
     package_data={'digitalmarketplace_frontend_jinja': components},
     include_package_data=True,
     install_requires=[
         'jinja2>3',
-        'govuk-frontend-jinja>=2.8.0,<3',
+        'govuk-frontend-jinja>=3,<4',
         'ccs-digitalmarketplace-utils>=65.0.0',
     ],
     python_requires=">=3.9,<3.12",
 )
```

