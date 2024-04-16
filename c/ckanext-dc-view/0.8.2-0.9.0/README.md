# Comparing `tmp/ckanext-dc_view-0.8.2.tar.gz` & `tmp/ckanext-dc_view-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-dc_view-0.8.2.tar", last modified: Thu Jan 18 13:41:19 2024, max compression
+gzip compressed data, was "ckanext-dc_view-0.9.0.tar", last modified: Tue Apr 16 10:38:00 2024, max compression
```

## Comparing `ckanext-dc_view-0.8.2.tar` & `ckanext-dc_view-0.9.0.tar`

### file list

```diff
@@ -1,39 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:41:19.550565 ckanext-dc_view-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-01-18 13:40:53.000000 ckanext-dc_view-0.8.2/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-01-18 13:40:53.000000 ckanext-dc_view-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-01-18 13:40:53.000000 ckanext-dc_view-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-01-18 13:41:19.550565 ckanext-dc_view-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-01-18 13:40:53.000000 ckanext-dc_view-0.8.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:41:19.546565 ckanext-dc_view-0.8.2/ckanext/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-01-18 13:40:53.000000 ckanext-dc_view-0.8.2/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:41:19.546565 ckanext-dc_view-0.8.2/ckanext/dc_view/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-01-18 13:40:53.000000 ckanext-dc_view-0.8.2/ckanext/dc_view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-01-18 13:40:53.000000 ckanext-dc_view-0.8.2/ckanext/dc_view/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-01-18 13:41:03.000000 ckanext-dc_view-0.8.2/ckanext/dc_view/_version_save.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:41:19.550565 ckanext-dc_view-0.8.2/ckanext/dc_view/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-01-18 13:40:53.000000 ckanext-dc_view-0.8.2/ckanext/dc_view/assets/dc_view.css
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-01-18 13:40:53.000000 ckanext-dc_view-0.8.2/ckanext/dc_view/assets/webassets.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-01-18 13:40:53.000000 ckanext-dc_view-0.8.2/ckanext/dc_view/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7468 2024-01-18 13:40:53.000000 ckanext-dc_view-0.8.2/ckanext/dc_view/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-01-18 13:40:53.000000 ckanext-dc_view-0.8.2/ckanext/dc_view/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-01-18 13:40:53.000000 ckanext-dc_view-0.8.2/ckanext/dc_view/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-01-18 13:40:53.000000 ckanext-dc_view-0.8.2/ckanext/dc_view/route_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:41:19.550565 ckanext-dc_view-0.8.2/ckanext/dc_view/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-01-18 13:40:53.000000 ckanext-dc_view-0.8.2/ckanext/dc_view/templates/dc_view.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:41:19.550565 ckanext-dc_view-0.8.2/ckanext/dc_view/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 13:40:53.000000 ckanext-dc_view-0.8.2/ckanext/dc_view/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-01-18 13:40:53.000000 ckanext-dc_view-0.8.2/ckanext/dc_view/tests/helper_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-18 13:40:53.000000 ckanext-dc_view-0.8.2/ckanext/dc_view/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-01-18 13:40:53.000000 ckanext-dc_view-0.8.2/ckanext/dc_view/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-01-18 13:40:53.000000 ckanext-dc_view-0.8.2/ckanext/dc_view/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-01-18 13:40:53.000000 ckanext-dc_view-0.8.2/ckanext/dc_view/tests/test_route.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:41:19.550565 ckanext-dc_view-0.8.2/ckanext_dc_view.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-01-18 13:41:19.000000 ckanext-dc_view-0.8.2/ckanext_dc_view.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-01-18 13:41:19.000000 ckanext-dc_view-0.8.2/ckanext_dc_view.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 13:41:19.000000 ckanext-dc_view-0.8.2/ckanext_dc_view.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-01-18 13:41:19.000000 ckanext-dc_view-0.8.2/ckanext_dc_view.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-18 13:41:19.000000 ckanext-dc_view-0.8.2/ckanext_dc_view.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-01-18 13:41:19.000000 ckanext-dc_view-0.8.2/ckanext_dc_view.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-18 13:41:19.000000 ckanext-dc_view-0.8.2/ckanext_dc_view.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 13:41:19.550565 ckanext-dc_view-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-01-18 13:40:53.000000 ckanext-dc_view-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:38:00.919777 ckanext-dc_view-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-16 10:37:26.000000 ckanext-dc_view-0.9.0/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-16 10:37:26.000000 ckanext-dc_view-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-16 10:37:26.000000 ckanext-dc_view-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-16 10:38:00.919777 ckanext-dc_view-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-16 10:37:26.000000 ckanext-dc_view-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:38:00.915778 ckanext-dc_view-0.9.0/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-16 10:37:26.000000 ckanext-dc_view-0.9.0/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:38:00.915778 ckanext-dc_view-0.9.0/ckanext/dc_view/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-16 10:37:26.000000 ckanext-dc_view-0.9.0/ckanext/dc_view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-04-16 10:37:26.000000 ckanext-dc_view-0.9.0/ckanext/dc_view/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-16 10:37:39.000000 ckanext-dc_view-0.9.0/ckanext/dc_view/_version_save.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:38:00.915778 ckanext-dc_view-0.9.0/ckanext/dc_view/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-16 10:37:26.000000 ckanext-dc_view-0.9.0/ckanext/dc_view/assets/dc_view.css
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-16 10:37:26.000000 ckanext-dc_view-0.9.0/ckanext/dc_view/assets/webassets.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-16 10:37:26.000000 ckanext-dc_view-0.9.0/ckanext/dc_view/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-16 10:37:26.000000 ckanext-dc_view-0.9.0/ckanext/dc_view/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-16 10:37:26.000000 ckanext-dc_view-0.9.0/ckanext/dc_view/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-16 10:37:26.000000 ckanext-dc_view-0.9.0/ckanext/dc_view/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-16 10:37:26.000000 ckanext-dc_view-0.9.0/ckanext/dc_view/route_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:38:00.915778 ckanext-dc_view-0.9.0/ckanext/dc_view/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-16 10:37:26.000000 ckanext-dc_view-0.9.0/ckanext/dc_view/templates/dc_view.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:38:00.919777 ckanext-dc_view-0.9.0/ckanext/dc_view/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:37:26.000000 ckanext-dc_view-0.9.0/ckanext/dc_view/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-16 10:37:26.000000 ckanext-dc_view-0.9.0/ckanext/dc_view/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-16 10:37:26.000000 ckanext-dc_view-0.9.0/ckanext/dc_view/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-16 10:37:26.000000 ckanext-dc_view-0.9.0/ckanext/dc_view/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-04-16 10:37:26.000000 ckanext-dc_view-0.9.0/ckanext/dc_view/tests/test_route.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:38:00.919777 ckanext-dc_view-0.9.0/ckanext_dc_view.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-16 10:38:00.000000 ckanext-dc_view-0.9.0/ckanext_dc_view.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-16 10:38:00.000000 ckanext-dc_view-0.9.0/ckanext_dc_view.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 10:38:00.000000 ckanext-dc_view-0.9.0/ckanext_dc_view.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-16 10:38:00.000000 ckanext-dc_view-0.9.0/ckanext_dc_view.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-16 10:38:00.000000 ckanext-dc_view-0.9.0/ckanext_dc_view.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-16 10:38:00.000000 ckanext-dc_view-0.9.0/ckanext_dc_view.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-16 10:38:00.000000 ckanext-dc_view-0.9.0/ckanext_dc_view.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 10:38:00.919777 ckanext-dc_view-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-16 10:37:26.000000 ckanext-dc_view-0.9.0/setup.py
```

### Comparing `ckanext-dc_view-0.8.2/CHANGELOG` & `ckanext-dc_view-0.9.0/CHANGELOG`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+0.9.0
+ - ref: don't create any preview files locally, upload directly to S3
+ - ref: only serve preview images from S3
+ - ref: migrate to dcor_shared 0.7.4
 0.8.2
  - maintenance release
 0.8.1
  - fix: failed to create preview images due to invalid basin data
 0.8.0
  - feat: add job that uploads preview images to S3
 0.7.1
```

### Comparing `ckanext-dc_view-0.8.2/LICENSE` & `ckanext-dc_view-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-dc_view-0.8.2/PKG-INFO` & `ckanext-dc_view-0.9.0/ckanext_dc_view.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ckanext-dc_view
-Version: 0.8.2
+Name: ckanext-dc-view
+Version: 0.9.0
 Summary: Preview DC data in DCOR 
 Home-page: https://github.com/DCOR-dev/ckanext-dc_view
 Author: Paul Müller
 Author-email: dev@craban.de
 License: AGPLv3+
 Keywords: CKAN,DCOR,RT-DC
 Platform: UNKNOWN
```

### Comparing `ckanext-dc_view-0.8.2/README.rst` & `ckanext-dc_view-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `ckanext-dc_view-0.8.2/ckanext/dc_view/_version.py` & `ckanext-dc_view-0.9.0/ckanext/dc_view/_version.py`

 * *Files identical despite different names*

### Comparing `ckanext-dc_view-0.8.2/ckanext/dc_view/cli.py` & `ckanext-dc_view-0.9.0/ckanext/dc_view/cli.py`

 * *Files identical despite different names*

### Comparing `ckanext-dc_view-0.8.2/ckanext/dc_view/jobs.py` & `ckanext-dc_view-0.9.0/ckanext/dc_view/jobs.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,90 +1,60 @@
 import atexit
 from collections import OrderedDict
 import os
+import pathlib
 import shutil
 import tempfile
 
-import ckan.plugins.toolkit as toolkit
 import dclab
-from dclab.rtdc_dataset import linker
-from dcor_shared import (
-    DC_MIME_TYPES, s3, sha256sum, get_ckan_config_option, get_resource_path,
-    wait_for_resource)
+from dcor_shared import DC_MIME_TYPES, s3cc, get_dc_instance, wait_for_resource
 import numpy as np
 
 # Create a temporary matplotlib config directory which is removed on exit
 mpldir = tempfile.mkdtemp(prefix="ckan_dcor_dc_view_")
 atexit.register(shutil.rmtree, mpldir)
 os.environ['MPLCONFIGDIR'] = mpldir
 
 from matplotlib.gridspec import GridSpec  # noqa: E402
 import matplotlib  # noqa: E402
+
 matplotlib.use('agg')
 import matplotlib.pylab as plt  # noqa: E402
 
 
 def admin_context():
     return {'ignore_auth': True, 'user': 'default'}
 
 
 def create_preview_job(resource, override=False):
     """Generate a *_preview.png file for a DC resource"""
-    path = get_resource_path(resource["id"])
-    wait_for_resource(path)
+    rid = resource["id"]
+    wait_for_resource(rid)
     mtype = resource.get('mimetype', '')
-    if mtype in DC_MIME_TYPES:
-        # only do this for rtdc data
-        jpgpath = path.with_name(path.name + "_preview.jpg")
-        if not jpgpath.exists() or override:
-            generate_preview(path, jpgpath)
-            return True
+    if (mtype in DC_MIME_TYPES
+        # Check whether the file already exists on S3
+        and (override
+             or not s3cc.artifact_exists(resource_id=rid,
+                                         artifact="preview"))):
+        # Create the preview in a temporary location
+        with tempfile.TemporaryDirectory() as ttd_name:
+            path_preview = pathlib.Path(ttd_name) / "preview.jpg"
+            with get_dc_instance(rid) as ds:
+                fig = overview_plot(rtdc_ds=ds)
+                fig.savefig(str(path_preview), dpi=80)
+                plt.close()
+            # Upload the preview to S3
+            s3cc.upload_artifact(resource_id=rid,
+                                 path_artifact=path_preview,
+                                 artifact="preview",
+                                 override=True)
+        return True
     return False
 
 
-def migrate_preview_to_s3_job(resource):
-    """Migrate a preview image to the S3 object store"""
-    path = get_resource_path(resource["id"])
-    path_prev = path.with_name(path.name + "_preview.jpg")
-    ds_dict = toolkit.get_action('package_show')(
-        admin_context(),
-        {'id': resource["package_id"]})
-    # Perform the upload
-    bucket_name = get_ckan_config_option(
-        "dcor_object_store.bucket_name").format(
-        organization_id=ds_dict["organization"]["id"])
-    rid = resource["id"]
-    sha256 = sha256sum(path_prev)
-    s3.upload_file(
-        bucket_name=bucket_name,
-        object_name=f"preview/{rid[:3]}/{rid[3:6]}/{rid[6:]}",
-        path=path_prev,
-        sha256=sha256,
-        private=ds_dict["private"])
-    # TODO: delete the local resource after successful upload?
-
-
-def generate_preview(path_rtdc, path_jpg):
-    # Check whether we have a condensed version of the dataset.
-    # If so, include that in the overview plot.
-    paths = []
-    path_condensed = path_rtdc.with_name(path_rtdc.name + "_condensed.rtdc")
-    if path_condensed.exists():
-        paths.append(path_condensed)
-    paths.append(path_rtdc)
-    # We create a linked HDF5 file which includes all paths.
-    with linker.combine_h5files(paths, external="raise") as fd:
-        # We do not enable basins, because it is time-consuming.
-        ds = dclab.rtdc_dataset.fmt_hdf5.RTDC_HDF5(fd, enable_basins=False)
-        # This is the original dataset
-        fig = overview_plot(rtdc_ds=ds)
-        fig.savefig(str(path_jpg), dpi=80)
-        plt.close()
-
-
 def overview_plot(rtdc_ds):
     """Simple overview plot adapted from the dclab examples
 
     Parameters
     ----------
     rtdc_ds: dclab.rtdc_dataset.core.RTDCBase
         Full RT-DC dataset to plot
@@ -106,15 +76,15 @@
     rtdc_ds.apply_filter()
     ds = dclab.new_dataset(rtdc_ds)
 
     # Features for scatter plot
     scatter_x = "area_um"
     scatter_y = "deform"
     # Event index to display
-    event_index = min(len(ds)-1, 47)
+    event_index = min(len(ds) - 1, 47)
 
     xlabel = dclab.dfn.get_feature_label(scatter_x, rtdc_ds=ds)
     ylabel = dclab.dfn.get_feature_label(scatter_y, rtdc_ds=ds)
 
     plots = OrderedDict()
     plots["scatter_basic"] = scatter_x in ds and scatter_y in ds
     plots["scatter_kde"] = scatter_x in ds and scatter_y in ds
@@ -133,15 +103,15 @@
     for key in plots:
         if plots[key]:
             if key in ["image", "mask"]:
                 height_ratios.append(1)
             else:
                 height_ratios.append(2)
 
-    fig = plt.figure(figsize=(4, np.sum(height_ratios)*1.5))
+    fig = plt.figure(figsize=(4, np.sum(height_ratios) * 1.5))
 
     gs = GridSpec(numplots, 1, height_ratios=height_ratios)
     ii = 0
 
     if scatter_x in ds and scatter_y in ds:
         ax1 = fig.add_subplot(gs[ii])
         ax1.set_title("Basic scatter plot")
```

### Comparing `ckanext-dc_view-0.8.2/ckanext/dc_view/meta.py` & `ckanext-dc_view-0.9.0/ckanext/dc_view/meta.py`

 * *Files identical despite different names*

### Comparing `ckanext-dc_view-0.8.2/ckanext/dc_view/plugin.py` & `ckanext-dc_view-0.9.0/ckanext/dc_view/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import ckan.plugins.toolkit as toolkit
 import ckan.plugins as plugins
 
 from dcor_shared import DC_MIME_TYPES, s3
 from rq.job import Job
 
 from .cli import get_commands
-from .jobs import create_preview_job, migrate_preview_to_s3_job
+from .jobs import create_preview_job
 from .meta import render_metadata_html
 from .route_funcs import dcpreview
 
 
 class DCViewPlugin(plugins.SingletonPlugin):
     """DC data view and route for *_preview.png"""
     plugins.implements(plugins.IBlueprint)
@@ -48,49 +48,38 @@
     # IConfigurer
     def update_config(self, config):
         plugins.toolkit.add_template_directory(config, 'templates')
         plugins.toolkit.add_resource('assets', 'dc_view')
 
     # IResourceController
     def after_resource_create(self, context, resource):
-        """Generate preview data"""
-        if resource.get('mimetype') in DC_MIME_TYPES:
+        """Generate preview image and upload to S3"""
+        # We only create the preview and upload it to S3 if the file is
+        # a DC file and if S3 is available.
+        if resource.get('mimetype') in DC_MIME_TYPES and s3.is_available():
             pkg_job_id = f"{resource['package_id']}_{resource['position']}_"
             depends_on = []
             extensions = [config.get("ckan.plugins")]
             # Are we waiting for symlinking (ckanext-dcor_depot)?
             # (This makes wait_for_resource really fast ;)
             if "dcor_depot" in extensions:
                 # Wait for the resource to be moved to the depot.
                 jid_sl = pkg_job_id + "symlink"
                 depends_on.append(jid_sl)
-            jid_preview = pkg_job_id + "preview"
+            jid_preview = pkg_job_id + "previews3"
             if not Job.exists(jid_preview, connection=ckan_redis_connect()):
                 toolkit.enqueue_job(create_preview_job,
                                     [resource],
                                     title="Create resource preview image",
                                     queue="dcor-normal",
                                     rq_kwargs={
                                         "timeout": 3600,
                                         "job_id": jid_preview,
                                         "depends_on": copy.copy(depends_on)})
 
-            # Upload the condensed dataset to S3
-            if s3.is_available():
-                jid_condensed_s3 = pkg_job_id + "previews3"
-                toolkit.enqueue_job(
-                    migrate_preview_to_s3_job,
-                    [resource],
-                    title="Migrate preview image to S3 object store",
-                    queue="dcor-normal",
-                    rq_kwargs={"timeout": 1000,
-                               "job_id": jid_condensed_s3,
-                               "depends_on": [jid_preview]}
-                    )
-
     # IResourceView
     def info(self):
         return {'name': 'dc_view',
                 'title': plugins.toolkit._('DC Info'),
                 'icon': 'microscope',
                 'iframed': False,
                 'always_available': True,
@@ -103,16 +92,17 @@
         same_domain = datapreview.on_same_domain(data_dict)
         if mtype in DC_MIME_TYPES and same_domain:
             return True
         else:
             return False
 
     def setup_template_variables(self, context, data_dict):
-        preview_url = '/dataset/{}/resource/{}/preview.jpg'.format(
-            data_dict['package']['id'], data_dict['resource']['id'])
+        ds_id = data_dict["package"]["id"]
+        rid = data_dict["resource"]["id"]
+        preview_url = f"/dataset/{ds_id}/resource/{rid}/preview.jpg"
         metadata_html = render_metadata_html(data_dict["resource"])
         return {
             'metadata_html': metadata_html,
             'preview_url': preview_url,
         }
 
     def view_template(self, context, data_dict):
```

### Comparing `ckanext-dc_view-0.8.2/ckanext/dc_view/tests/test_jobs.py` & `ckanext-dc_view-0.9.0/ckanext/dc_view/tests/test_jobs.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,51 +5,39 @@
 
 A common approach is to use the mock package to replace the
 ckan.plugins.toolkit.enqueue_job function with a mock that executes jobs
 synchronously instead of asynchronously
 """
 from unittest import mock
 import pathlib
-import time
 
 import pytest
 import requests
 
 import ckan.lib
 import ckan.tests.factories as factories
 
 import ckanext.dcor_schemas.plugin
 import dcor_shared
+from dcor_shared import s3cc
+from dcor_shared.testing import make_dataset, synchronous_enqueue_job
 
-from .helper_methods import make_dataset
 
-
-data_dir = pathlib.Path(__file__).parent / "data"
-
-
-def synchronous_enqueue_job(job_func, args=None, kwargs=None, title=None,
-                            queue=None, rq_kwargs=None):
-    """
-    Synchronous mock for ``ckan.plugins.toolkit.enqueue_job``.
-    """
-    if rq_kwargs is None:
-        rq_kwargs = {}
-    args = args or []
-    kwargs = kwargs or {}
-    job_func(*args, **kwargs)
+data_path = pathlib.Path(__file__).parent / "data"
 
 
 # We need the dcor_depot extension to make sure that the symbolic-
 # linking pipeline is used.
 @pytest.mark.ckan_config('ckan.plugins', 'dcor_depot dcor_schemas dc_view')
 @pytest.mark.usefixtures('clean_db', 'with_request_context')
 @mock.patch('ckan.plugins.toolkit.enqueue_job',
             side_effect=synchronous_enqueue_job)
-def test_create_preview_job(enqueue_job_mock, create_with_upload, monkeypatch,
-                            ckan_config, tmpdir):
+def test_create_preview_s3_job(
+        enqueue_job_mock, create_with_upload, monkeypatch, ckan_config,
+        tmpdir):
     monkeypatch.setitem(ckan_config, 'ckan.storage_path', str(tmpdir))
     monkeypatch.setattr(ckan.lib.uploader,
                         'get_storage_path',
                         lambda: str(tmpdir))
     monkeypatch.setattr(
         ckanext.dcor_schemas.plugin,
         'DISABLE_AFTER_DATASET_CREATE_FOR_CONCURRENT_JOB_TESTS',
@@ -63,43 +51,36 @@
     # Note: `call_action` bypasses authorization!
     # create 1st dataset
     create_context = {'ignore_auth': False, 'user': user['name'],
                       'api_version': 3}
     dataset = make_dataset(create_context,
                            owner_org,
                            activate=False)
-    path = data_dir / "calibration_beads_47.rtdc"
+    path = data_path / "calibration_beads_47.rtdc"
     content = path.read_bytes()
     result = create_with_upload(
         content, 'test.rtdc',
         url="upload",
         package_id=dataset["id"],
         context=create_context,
     )
     resource_path = dcor_shared.get_resource_path(result["id"])
     assert resource_path.exists()
-    preview_path = resource_path.with_name(resource_path.name + "_preview.jpg")
     # give the background job a little time to complete
-    for ii in range(100):
-        if not preview_path.exists():
-            time.sleep(0.1)
-        else:
-            assert preview_path.stat().st_size > 1000
-            break
-    else:
-        raise ValueError("Preview generation timed out after 10s!")
+    assert s3cc.artifact_exists(resource_id=result["id"],
+                                artifact="preview")
 
 
 # We need the dcor_depot extension to make sure that the symbolic-
 # linking pipeline is used.
 @pytest.mark.ckan_config('ckan.plugins', 'dcor_depot dc_view dcor_schemas')
 @pytest.mark.usefixtures('clean_db', 'with_request_context')
 @mock.patch('ckan.plugins.toolkit.enqueue_job',
             side_effect=synchronous_enqueue_job)
-def test_upload_preview_dataset_to_s3_job(
+def test_create_preview_s3_job_alternate(
         enqueue_job_mock, create_with_upload, monkeypatch, ckan_config,
         tmpdir):
     monkeypatch.setitem(ckan_config, 'ckan.storage_path', str(tmpdir))
     monkeypatch.setattr(ckan.lib.uploader,
                         'get_storage_path',
                         lambda: str(tmpdir))
     monkeypatch.setattr(
@@ -113,29 +94,24 @@
         'capacity': 'admin'
     }])
     # Note: `call_action` bypasses authorization!
     # create 1st dataset
     create_context = {'ignore_auth': False,
                       'user': user['name'],
                       'api_version': 3}
-    ds_dict, res_dict = make_dataset(create_context,
-                                     owner_org,
-                                     create_with_upload=create_with_upload,
-                                     activate=True)
+    ds_dict, res_dict = make_dataset(
+        create_context,
+        owner_org,
+        create_with_upload=create_with_upload,
+        resource_path=data_path / "calibration_beads_47.rtdc",
+        activate=True)
     bucket_name = dcor_shared.get_ckan_config_option(
         "dcor_object_store.bucket_name").format(
         organization_id=ds_dict["organization"]["id"])
     rid = res_dict["id"]
     object_name = f"preview/{rid[:3]}/{rid[3:6]}/{rid[6:]}"
     endpoint = dcor_shared.get_ckan_config_option(
         "dcor_object_store.endpoint_url")
     prev_url = f"{endpoint}/{bucket_name}/{object_name}"
     response = requests.get(prev_url)
     assert response.ok, "resource is public"
     assert response.status_code == 200
-    # Verify SHA256sum
-    path = dcor_shared.get_resource_path(res_dict["id"])
-    path_prev = path.with_name(path.name + "_preview.jpg")
-    dl_path = tmpdir / "prev_image.jpg"
-    with dl_path.open("wb") as fd:
-        fd.write(response.content)
-    assert dcor_shared.sha256sum(dl_path) == dcor_shared.sha256sum(path_prev)
```

### Comparing `ckanext-dc_view-0.8.2/ckanext_dc_view.egg-info/PKG-INFO` & `ckanext-dc_view-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ckanext-dc-view
-Version: 0.8.2
+Name: ckanext-dc_view
+Version: 0.9.0
 Summary: Preview DC data in DCOR 
 Home-page: https://github.com/DCOR-dev/ckanext-dc_view
 Author: Paul Müller
 Author-email: dev@craban.de
 License: AGPLv3+
 Keywords: CKAN,DCOR,RT-DC
 Platform: UNKNOWN
```

### Comparing `ckanext-dc_view-0.8.2/ckanext_dc_view.egg-info/SOURCES.txt` & `ckanext-dc_view-0.9.0/ckanext_dc_view.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 ckanext/dc_view/meta.py
 ckanext/dc_view/plugin.py
 ckanext/dc_view/route_funcs.py
 ckanext/dc_view/assets/dc_view.css
 ckanext/dc_view/assets/webassets.yml
 ckanext/dc_view/templates/dc_view.html
 ckanext/dc_view/tests/__init__.py
-ckanext/dc_view/tests/helper_methods.py
 ckanext/dc_view/tests/requirements.txt
 ckanext/dc_view/tests/test_jobs.py
 ckanext/dc_view/tests/test_plugin.py
 ckanext/dc_view/tests/test_route.py
 ckanext_dc_view.egg-info/PKG-INFO
 ckanext_dc_view.egg-info/SOURCES.txt
 ckanext_dc_view.egg-info/dependency_links.txt
```

### Comparing `ckanext-dc_view-0.8.2/setup.py` & `ckanext-dc_view-0.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     keywords=["CKAN", "DCOR", "RT-DC"],
     packages=find_packages(exclude=['contrib', 'docs', 'tests*']),
     package_dir={name: name},
     namespace_packages=['ckanext'],
     install_requires=[
         # the "ckan" dependency is implied
         "dclab>=0.57.0",
-        "dcor_shared>=0.5.3",
+        "dcor_shared>=0.7.4",
         "matplotlib",
         "numpy>=1.19",
         "pillow",
     ],
     include_package_data=True,
     # To provide executable scripts, use entry points in preference to the
     # "scripts" keyword. Entry points provide cross-platform support and allow
```

