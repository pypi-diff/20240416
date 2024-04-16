# Comparing `tmp/ckanext-dc_log_view-0.3.3.tar.gz` & `tmp/ckanext-dc_log_view-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-dc_log_view-0.3.3.tar", last modified: Thu Jan 18 13:32:42 2024, max compression
+gzip compressed data, was "ckanext-dc_log_view-0.4.0.tar", last modified: Tue Apr 16 10:28:59 2024, max compression
```

## Comparing `ckanext-dc_log_view-0.3.3.tar` & `ckanext-dc_log_view-0.4.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:32:42.297543 ckanext-dc_log_view-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-01-18 13:32:19.000000 ckanext-dc_log_view-0.3.3/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-01-18 13:32:19.000000 ckanext-dc_log_view-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-01-18 13:32:19.000000 ckanext-dc_log_view-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-01-18 13:32:42.297543 ckanext-dc_log_view-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-01-18 13:32:19.000000 ckanext-dc_log_view-0.3.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:32:42.297543 ckanext-dc_log_view-0.3.3/ckanext/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-01-18 13:32:19.000000 ckanext-dc_log_view-0.3.3/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:32:42.297543 ckanext-dc_log_view-0.3.3/ckanext/dc_log_view/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-01-18 13:32:19.000000 ckanext-dc_log_view-0.3.3/ckanext/dc_log_view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-01-18 13:32:19.000000 ckanext-dc_log_view-0.3.3/ckanext/dc_log_view/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-01-18 13:32:29.000000 ckanext-dc_log_view-0.3.3/ckanext/dc_log_view/_version_save.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:32:42.297543 ckanext-dc_log_view-0.3.3/ckanext/dc_log_view/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-01-18 13:32:19.000000 ckanext-dc_log_view-0.3.3/ckanext/dc_log_view/assets/dc_log_view.css
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-18 13:32:19.000000 ckanext-dc_log_view-0.3.3/ckanext/dc_log_view/assets/webassets.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-01-18 13:32:19.000000 ckanext-dc_log_view-0.3.3/ckanext/dc_log_view/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:32:42.297543 ckanext-dc_log_view-0.3.3/ckanext/dc_log_view/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-01-18 13:32:19.000000 ckanext-dc_log_view-0.3.3/ckanext/dc_log_view/templates/dc_view_log.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:32:42.297543 ckanext-dc_log_view-0.3.3/ckanext/dc_log_view/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 13:32:19.000000 ckanext-dc_log_view-0.3.3/ckanext/dc_log_view/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-18 13:32:19.000000 ckanext-dc_log_view-0.3.3/ckanext/dc_log_view/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-01-18 13:32:19.000000 ckanext-dc_log_view-0.3.3/ckanext/dc_log_view/tests/test_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:32:42.297543 ckanext-dc_log_view-0.3.3/ckanext_dc_log_view.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-01-18 13:32:42.000000 ckanext-dc_log_view-0.3.3/ckanext_dc_log_view.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-01-18 13:32:42.000000 ckanext-dc_log_view-0.3.3/ckanext_dc_log_view.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 13:32:42.000000 ckanext-dc_log_view-0.3.3/ckanext_dc_log_view.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-01-18 13:32:42.000000 ckanext-dc_log_view-0.3.3/ckanext_dc_log_view.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-18 13:32:42.000000 ckanext-dc_log_view-0.3.3/ckanext_dc_log_view.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-18 13:32:42.000000 ckanext-dc_log_view-0.3.3/ckanext_dc_log_view.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-18 13:32:42.000000 ckanext-dc_log_view-0.3.3/ckanext_dc_log_view.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 13:32:42.297543 ckanext-dc_log_view-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-01-18 13:32:19.000000 ckanext-dc_log_view-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:28:59.481544 ckanext-dc_log_view-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-16 10:28:34.000000 ckanext-dc_log_view-0.4.0/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-16 10:28:34.000000 ckanext-dc_log_view-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-16 10:28:34.000000 ckanext-dc_log_view-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-16 10:28:59.477543 ckanext-dc_log_view-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-16 10:28:34.000000 ckanext-dc_log_view-0.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:28:59.477543 ckanext-dc_log_view-0.4.0/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-16 10:28:34.000000 ckanext-dc_log_view-0.4.0/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:28:59.477543 ckanext-dc_log_view-0.4.0/ckanext/dc_log_view/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-16 10:28:34.000000 ckanext-dc_log_view-0.4.0/ckanext/dc_log_view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-04-16 10:28:34.000000 ckanext-dc_log_view-0.4.0/ckanext/dc_log_view/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-16 10:28:45.000000 ckanext-dc_log_view-0.4.0/ckanext/dc_log_view/_version_save.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:28:59.477543 ckanext-dc_log_view-0.4.0/ckanext/dc_log_view/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-16 10:28:34.000000 ckanext-dc_log_view-0.4.0/ckanext/dc_log_view/assets/dc_log_view.css
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-16 10:28:34.000000 ckanext-dc_log_view-0.4.0/ckanext/dc_log_view/assets/webassets.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-16 10:28:34.000000 ckanext-dc_log_view-0.4.0/ckanext/dc_log_view/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:28:59.477543 ckanext-dc_log_view-0.4.0/ckanext/dc_log_view/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-16 10:28:34.000000 ckanext-dc_log_view-0.4.0/ckanext/dc_log_view/templates/dc_view_log.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:28:59.477543 ckanext-dc_log_view-0.4.0/ckanext/dc_log_view/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:28:34.000000 ckanext-dc_log_view-0.4.0/ckanext/dc_log_view/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-16 10:28:34.000000 ckanext-dc_log_view-0.4.0/ckanext/dc_log_view/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-04-16 10:28:34.000000 ckanext-dc_log_view-0.4.0/ckanext/dc_log_view/tests/test_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:28:59.477543 ckanext-dc_log_view-0.4.0/ckanext_dc_log_view.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-16 10:28:59.000000 ckanext-dc_log_view-0.4.0/ckanext_dc_log_view.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-16 10:28:59.000000 ckanext-dc_log_view-0.4.0/ckanext_dc_log_view.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 10:28:59.000000 ckanext-dc_log_view-0.4.0/ckanext_dc_log_view.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-16 10:28:59.000000 ckanext-dc_log_view-0.4.0/ckanext_dc_log_view.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-16 10:28:59.000000 ckanext-dc_log_view-0.4.0/ckanext_dc_log_view.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-16 10:28:59.000000 ckanext-dc_log_view-0.4.0/ckanext_dc_log_view.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-16 10:28:59.000000 ckanext-dc_log_view-0.4.0/ckanext_dc_log_view.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 10:28:59.481544 ckanext-dc_log_view-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-16 10:28:34.000000 ckanext-dc_log_view-0.4.0/setup.py
```

### Comparing `ckanext-dc_log_view-0.3.3/CHANGELOG` & `ckanext-dc_log_view-0.4.0/CHANGELOG`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+0.4.0
+ - ref: migrate to dcor_shared 0.7.3
+ - tests: add tests
 0.3.3
  - maintenance release
 0.3.2
  - maintenance release
 0.3.1
  - docs: update gitignore
  - ci: use standarad ckan.ini
```

### Comparing `ckanext-dc_log_view-0.3.3/LICENSE` & `ckanext-dc_log_view-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-dc_log_view-0.3.3/PKG-INFO` & `ckanext-dc_log_view-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-dc_log_view
-Version: 0.3.3
+Version: 0.4.0
 Summary: View DC data logs on DCOR
 Home-page: https://github.com/DCOR-dev/ckanext-dc_log_view
 Author: Paul Müller
 Author-email: dev@craban.de
 License: AGPLv3+
 Keywords: CKAN,DCOR,RT-DC
 Platform: UNKNOWN
```

### Comparing `ckanext-dc_log_view-0.3.3/README.rst` & `ckanext-dc_log_view-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `ckanext-dc_log_view-0.3.3/ckanext/dc_log_view/_version.py` & `ckanext-dc_log_view-0.4.0/ckanext/dc_log_view/_version.py`

 * *Files identical despite different names*

### Comparing `ckanext-dc_log_view-0.3.3/ckanext/dc_log_view/assets/dc_log_view.css` & `ckanext-dc_log_view-0.4.0/ckanext/dc_log_view/assets/dc_log_view.css`

 * *Files identical despite different names*

### Comparing `ckanext-dc_log_view-0.3.3/ckanext/dc_log_view/plugin.py` & `ckanext-dc_log_view-0.4.0/ckanext/dc_log_view/plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-import dclab
-
 import ckan.lib.datapreview as datapreview
 import ckan.plugins as p
 
-from dcor_shared import DC_MIME_TYPES, get_resource_path
+from dcor_shared import DC_MIME_TYPES, get_dc_instance
 
 
 class DCLogViewPlugin(p.SingletonPlugin):
     """This plugin makes log views of DC data"""
     p.implements(p.IConfigurer, inherit=True)
     p.implements(p.IResourceView, inherit=True)
 
@@ -33,18 +31,17 @@
         if mtype in DC_MIME_TYPES and same_domain:
             return True
         else:
             return False
 
     def setup_template_variables(self, context, data_dict):
         # get the local resource location
-        resource = data_dict['resource']
-        path = get_resource_path(resource["id"])
+        res_dict = data_dict['resource']
         # extract the logs
         logs = {}
-        with dclab.new_dataset(path) as ds:
+        with get_dc_instance(res_dict["id"]) as ds:
             for key in ds.logs:
                 logs[key] = ds.logs[key]
         return {"logs": logs}
 
     def view_template(self, context, data_dict):
         return 'dc_view_log.html'
```

### Comparing `ckanext-dc_log_view-0.3.3/ckanext/dc_log_view/templates/dc_view_log.html` & `ckanext-dc_log_view-0.4.0/ckanext/dc_log_view/templates/dc_view_log.html`

 * *Files identical despite different names*

### Comparing `ckanext-dc_log_view-0.3.3/ckanext_dc_log_view.egg-info/PKG-INFO` & `ckanext-dc_log_view-0.4.0/ckanext_dc_log_view.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-dc-log-view
-Version: 0.3.3
+Version: 0.4.0
 Summary: View DC data logs on DCOR
 Home-page: https://github.com/DCOR-dev/ckanext-dc_log_view
 Author: Paul Müller
 Author-email: dev@craban.de
 License: AGPLv3+
 Keywords: CKAN,DCOR,RT-DC
 Platform: UNKNOWN
```

### Comparing `ckanext-dc_log_view-0.3.3/ckanext_dc_log_view.egg-info/SOURCES.txt` & `ckanext-dc_log_view-0.4.0/ckanext_dc_log_view.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-dc_log_view-0.3.3/setup.py` & `ckanext-dc_log_view-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     keywords=["CKAN", "DCOR", "RT-DC"],
     packages=find_packages(exclude=['contrib', 'docs', 'tests*']),
     package_dir={name: name},
     namespace_packages=['ckanext'],
     install_requires=[
         # the "ckan" dependency is implied
         "dclab>=0.52.0",
-        "dcor_shared>0.3.1",
+        "dcor_shared>=0.7.3",
     ],
     include_package_data=True,
     # To provide executable scripts, use entry points in preference to the
     # "scripts" keyword. Entry points provide cross-platform support and allow
     # pip to create the appropriate form of executable for the target platform.
     entry_points='''
         [ckan.plugins]
```

