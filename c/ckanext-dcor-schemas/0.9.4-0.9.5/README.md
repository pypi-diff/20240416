# Comparing `tmp/ckanext-dcor_schemas-0.9.4.tar.gz` & `tmp/ckanext-dcor_schemas-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ckanext-dcor_schemas-0.9.4.tar", last modified: Mon Sep 21 13:36:40 2020, max compression
+gzip compressed data, was "dist/ckanext-dcor_schemas-0.9.5.tar", last modified: Mon Sep 21 15:00:55 2020, max compression
```

## Comparing `ckanext-dcor_schemas-0.9.4.tar` & `ckanext-dcor_schemas-0.9.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-21 13:36:40.520228 ckanext-dcor_schemas-0.9.4/
--rw-rw-r--   0 travis    (2000) travis    (2000)      342 2020-09-21 13:36:20.000000 ckanext-dcor_schemas-0.9.4/CHANGELOG
--rw-rw-r--   0 travis    (2000) travis    (2000)    34523 2020-09-21 13:36:20.000000 ckanext-dcor_schemas-0.9.4/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      166 2020-09-21 13:36:20.000000 ckanext-dcor_schemas-0.9.4/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     4633 2020-09-21 13:36:40.520228 ckanext-dcor_schemas-0.9.4/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3393 2020-09-21 13:36:20.000000 ckanext-dcor_schemas-0.9.4/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-21 13:36:40.516230 ckanext-dcor_schemas-0.9.4/ckanext/
--rw-rw-r--   0 travis    (2000) travis    (2000)      200 2020-09-21 13:36:20.000000 ckanext-dcor_schemas-0.9.4/ckanext/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-21 13:36:40.516230 ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/
--rw-rw-r--   0 travis    (2000) travis    (2000)       59 2020-09-21 13:36:20.000000 ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7095 2020-09-21 13:36:20.000000 ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/_version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       82 2020-09-21 13:36:23.000000 ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/_version_save.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-21 13:36:40.520228 ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/assets/
--rw-rw-r--   0 travis    (2000) travis    (2000)      319 2020-09-21 13:36:20.000000 ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/assets/hide_unused_elements.css
--rw-rw-r--   0 travis    (2000) travis    (2000)       65 2020-09-21 13:36:20.000000 ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/assets/webassets.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)     8141 2020-09-21 13:36:20.000000 ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/auth.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1924 2020-09-21 13:36:20.000000 ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2822 2020-09-21 13:36:20.000000 ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/jobs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1873 2020-09-21 13:36:20.000000 ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/licenses.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    10940 2020-09-21 13:36:20.000000 ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/plugin.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-21 13:36:40.520228 ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/templates/
--rw-rw-r--   0 travis    (2000) travis    (2000)      120 2020-09-21 13:36:20.000000 ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/templates/base.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-21 13:36:40.520228 ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/templates/organization/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3208 2020-09-21 13:36:20.000000 ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/templates/organization/bulk_process.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-21 13:36:40.520228 ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/templates/package/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1568 2020-09-21 13:36:20.000000 ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/templates/package/resource_read.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      122 2020-09-21 13:36:20.000000 ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/templates/package/resources.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-21 13:36:40.520228 ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/templates/package/snippets/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1869 2020-09-21 13:36:20.000000 ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/templates/package/snippets/additional_info.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     2792 2020-09-21 13:36:20.000000 ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/templates/package/snippets/package_basic_fields.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      396 2020-09-21 13:36:20.000000 ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/templates/package/snippets/package_metadata_fields.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      205 2020-09-21 13:36:20.000000 ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/templates/package/snippets/resource_edit_form.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      253 2020-09-21 13:36:20.000000 ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/templates/package/snippets/resource_form.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-21 13:36:40.520228 ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-09-21 13:36:20.000000 ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      116 2020-09-21 13:36:20.000000 ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/tests/test_plugin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7753 2020-09-21 13:36:20.000000 ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/validate.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-21 13:36:40.520228 ckanext-dcor_schemas-0.9.4/ckanext_dcor_schemas.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4633 2020-09-21 13:36:40.000000 ckanext-dcor_schemas-0.9.4/ckanext_dcor_schemas.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1405 2020-09-21 13:36:40.000000 ckanext-dcor_schemas-0.9.4/ckanext_dcor_schemas.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-09-21 13:36:40.000000 ckanext-dcor_schemas-0.9.4/ckanext_dcor_schemas.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       99 2020-09-21 13:36:40.000000 ckanext-dcor_schemas-0.9.4/ckanext_dcor_schemas.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2020-09-21 13:36:40.000000 ckanext-dcor_schemas-0.9.4/ckanext_dcor_schemas.egg-info/namespace_packages.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2020-09-21 13:36:40.000000 ckanext-dcor_schemas-0.9.4/ckanext_dcor_schemas.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       49 2020-09-21 13:36:20.000000 ckanext-dcor_schemas-0.9.4/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-09-21 13:36:40.520228 ckanext-dcor_schemas-0.9.4/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2300 2020-09-21 13:36:20.000000 ckanext-dcor_schemas-0.9.4/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-21 15:00:55.479249 ckanext-dcor_schemas-0.9.5/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      403 2020-09-21 15:00:34.000000 ckanext-dcor_schemas-0.9.5/CHANGELOG
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34523 2020-09-21 15:00:34.000000 ckanext-dcor_schemas-0.9.5/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      166 2020-09-21 15:00:34.000000 ckanext-dcor_schemas-0.9.5/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4633 2020-09-21 15:00:55.479249 ckanext-dcor_schemas-0.9.5/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3393 2020-09-21 15:00:34.000000 ckanext-dcor_schemas-0.9.5/README.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-21 15:00:55.471253 ckanext-dcor_schemas-0.9.5/ckanext/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      200 2020-09-21 15:00:34.000000 ckanext-dcor_schemas-0.9.5/ckanext/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-21 15:00:55.475252 ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       59 2020-09-21 15:00:34.000000 ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7095 2020-09-21 15:00:34.000000 ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/_version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       82 2020-09-21 15:00:37.000000 ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/_version_save.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-21 15:00:55.475252 ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/assets/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      319 2020-09-21 15:00:34.000000 ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/assets/hide_unused_elements.css
+-rw-rw-r--   0 travis    (2000) travis    (2000)       65 2020-09-21 15:00:34.000000 ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/assets/webassets.yml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8141 2020-09-21 15:00:34.000000 ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/auth.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1924 2020-09-21 15:00:34.000000 ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2822 2020-09-21 15:00:34.000000 ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/jobs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1873 2020-09-21 15:00:34.000000 ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/licenses.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11047 2020-09-21 15:00:34.000000 ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/plugin.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-21 15:00:55.475252 ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/templates/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      120 2020-09-21 15:00:34.000000 ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/templates/base.html
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-21 15:00:55.475252 ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/templates/organization/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3208 2020-09-21 15:00:34.000000 ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/templates/organization/bulk_process.html
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-21 15:00:55.475252 ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/templates/package/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1568 2020-09-21 15:00:34.000000 ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/templates/package/resource_read.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      122 2020-09-21 15:00:34.000000 ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/templates/package/resources.html
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-21 15:00:55.475252 ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/templates/package/snippets/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1869 2020-09-21 15:00:34.000000 ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/templates/package/snippets/additional_info.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2792 2020-09-21 15:00:34.000000 ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/templates/package/snippets/package_basic_fields.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      396 2020-09-21 15:00:34.000000 ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/templates/package/snippets/package_metadata_fields.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      205 2020-09-21 15:00:34.000000 ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/templates/package/snippets/resource_edit_form.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      253 2020-09-21 15:00:34.000000 ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/templates/package/snippets/resource_form.html
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-21 15:00:55.475252 ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-09-21 15:00:34.000000 ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      116 2020-09-21 15:00:34.000000 ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/tests/test_plugin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7753 2020-09-21 15:00:34.000000 ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/validate.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-21 15:00:55.475252 ckanext-dcor_schemas-0.9.5/ckanext_dcor_schemas.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4633 2020-09-21 15:00:55.000000 ckanext-dcor_schemas-0.9.5/ckanext_dcor_schemas.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1405 2020-09-21 15:00:55.000000 ckanext-dcor_schemas-0.9.5/ckanext_dcor_schemas.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-09-21 15:00:55.000000 ckanext-dcor_schemas-0.9.5/ckanext_dcor_schemas.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       99 2020-09-21 15:00:55.000000 ckanext-dcor_schemas-0.9.5/ckanext_dcor_schemas.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2020-09-21 15:00:55.000000 ckanext-dcor_schemas-0.9.5/ckanext_dcor_schemas.egg-info/namespace_packages.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2020-09-21 15:00:55.000000 ckanext-dcor_schemas-0.9.5/ckanext_dcor_schemas.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       49 2020-09-21 15:00:34.000000 ckanext-dcor_schemas-0.9.5/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-09-21 15:00:55.479249 ckanext-dcor_schemas-0.9.5/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2300 2020-09-21 15:00:34.000000 ckanext-dcor_schemas-0.9.5/setup.py
```

### Comparing `ckanext-dcor_schemas-0.9.4/LICENSE` & `ckanext-dcor_schemas-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_schemas-0.9.4/PKG-INFO` & `ckanext-dcor_schemas-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ckanext-dcor_schemas
-Version: 0.9.4
+Version: 0.9.5
 Summary: Introduces or lifts restrictions (authorization) for managing data and metadata on DCOR
 Home-page: https://github.com/DCOR-dev/ckanext-dcor_schemas
 Author: Paul Müller
 Author-email: dev@craban.de
 License: AGPLv3+
 Description: ckanext-dcor_schemas
         ====================
```

### Comparing `ckanext-dcor_schemas-0.9.4/README.rst` & `ckanext-dcor_schemas-0.9.5/README.rst`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/_version.py` & `ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/_version.py`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/auth.py` & `ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/auth.py`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/helpers.py` & `ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/jobs.py` & `ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/jobs.py`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/licenses.json` & `ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/licenses.json`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/plugin.py` & `ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,37 +233,40 @@
             grps = logic.get_action("group_list_authz")(
                 {u'user': user_obj.id}, {})
             labels.extend(u'group-%s' % o['id'] for o in grps)
         return labels
 
     # IResourceController
     def after_create(self, context, resource):
-        """Generate sha256 hash"""
-        jidm = "-".join([resource["id"], resource["name"], "mimetype"])
-        toolkit.enqueue_job(jobs.set_format_job,
-                            [resource],
-                            title="Set mimetype for resource",
-                            queue="dcor-short",
-                            rq_kwargs={"timeout": 60,
-                                       "job_id": jidm})
-        jidp = "-".join([resource["id"], resource["name"], "dcparms"])
-        toolkit.enqueue_job(jobs.set_dc_config_job,
-                            [resource],
-                            title="Set DC parameters for resource",
-                            queue="dcor-normal",
-                            rq_kwargs={"timeout": 60,
-                                       "job_id": jidp})
+        """Add custom jobs"""
         jids = "-".join([resource["id"], resource["name"], "sha256"])
         toolkit.enqueue_job(jobs.set_sha256_job,
                             [resource],
                             title="Set SHA256 hash for resource",
                             queue="dcor-normal",
                             rq_kwargs={"timeout": 500,
                                        "job_id": jids})
 
+        if resource.get('mimetype') in DC_MIME_TYPES:
+            jidm = "-".join([resource["id"], resource["name"], "mimetype"])
+            toolkit.enqueue_job(jobs.set_format_job,
+                                [resource],
+                                title="Set mimetype for resource",
+                                queue="dcor-short",
+                                rq_kwargs={"timeout": 60,
+                                           "job_id": jidm})
+
+            jidp = "-".join([resource["id"], resource["name"], "dcparms"])
+            toolkit.enqueue_job(jobs.set_dc_config_job,
+                                [resource],
+                                title="Set DC parameters for resource",
+                                queue="dcor-normal",
+                                rq_kwargs={"timeout": 60,
+                                           "job_id": jidp})
+
     def before_create(self, context, resource):
         # set the filename
         if "upload" in resource:
             upload = resource["upload"]
             if hasattr(upload, "filename"):
                 filename = upload.filename
             elif hasattr(upload, "name"):
```

### Comparing `ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/templates/organization/bulk_process.html` & `ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/templates/organization/bulk_process.html`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/templates/package/resource_read.html` & `ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/templates/package/resource_read.html`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/templates/package/snippets/additional_info.html` & `ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/templates/package/snippets/additional_info.html`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/templates/package/snippets/package_basic_fields.html` & `ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/templates/package/snippets/package_basic_fields.html`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_schemas-0.9.4/ckanext/dcor_schemas/validate.py` & `ckanext-dcor_schemas-0.9.5/ckanext/dcor_schemas/validate.py`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_schemas-0.9.4/ckanext_dcor_schemas.egg-info/PKG-INFO` & `ckanext-dcor_schemas-0.9.5/ckanext_dcor_schemas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ckanext-dcor-schemas
-Version: 0.9.4
+Version: 0.9.5
 Summary: Introduces or lifts restrictions (authorization) for managing data and metadata on DCOR
 Home-page: https://github.com/DCOR-dev/ckanext-dcor_schemas
 Author: Paul Müller
 Author-email: dev@craban.de
 License: AGPLv3+
 Description: ckanext-dcor_schemas
         ====================
```

### Comparing `ckanext-dcor_schemas-0.9.4/ckanext_dcor_schemas.egg-info/SOURCES.txt` & `ckanext-dcor_schemas-0.9.5/ckanext_dcor_schemas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_schemas-0.9.4/setup.py` & `ckanext-dcor_schemas-0.9.5/setup.py`

 * *Files identical despite different names*

