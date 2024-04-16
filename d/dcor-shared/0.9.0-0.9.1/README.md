# Comparing `tmp/dcor_shared-0.9.0.tar.gz` & `tmp/dcor_shared-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcor_shared-0.9.0.tar", last modified: Wed Mar  6 17:08:36 2024, max compression
+gzip compressed data, was "dcor_shared-0.9.1.tar", last modified: Thu Mar  7 08:48:15 2024, max compression
```

## Comparing `dcor_shared-0.9.0.tar` & `dcor_shared-0.9.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:08:36.253926 dcor_shared-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-03-06 17:08:10.000000 dcor_shared-0.9.0/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-06 17:08:10.000000 dcor_shared-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-06 17:08:10.000000 dcor_shared-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-03-06 17:08:36.253926 dcor_shared-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-03-06 17:08:10.000000 dcor_shared-0.9.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:08:36.253926 dcor_shared-0.9.0/dcor_shared/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-06 17:08:10.000000 dcor_shared-0.9.0/dcor_shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-03-06 17:08:10.000000 dcor_shared-0.9.0/dcor_shared/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-06 17:08:23.000000 dcor_shared-0.9.0/dcor_shared/_version_save.py
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-03-06 17:08:10.000000 dcor_shared-0.9.0/dcor_shared/ckan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-03-06 17:08:10.000000 dcor_shared-0.9.0/dcor_shared/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-06 17:08:10.000000 dcor_shared-0.9.0/dcor_shared/dcinst.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-06 17:08:10.000000 dcor_shared-0.9.0/dcor_shared/mime.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-03-06 17:08:10.000000 dcor_shared-0.9.0/dcor_shared/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-06 17:08:10.000000 dcor_shared-0.9.0/dcor_shared/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)    15002 2024-03-06 17:08:10.000000 dcor_shared-0.9.0/dcor_shared/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     9102 2024-03-06 17:08:10.000000 dcor_shared-0.9.0/dcor_shared/s3cc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9986 2024-03-06 17:08:10.000000 dcor_shared-0.9.0/dcor_shared/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:08:36.253926 dcor_shared-0.9.0/dcor_shared.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-03-06 17:08:36.000000 dcor_shared-0.9.0/dcor_shared.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-03-06 17:08:36.000000 dcor_shared-0.9.0/dcor_shared.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 17:08:36.000000 dcor_shared-0.9.0/dcor_shared.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-06 17:08:36.000000 dcor_shared-0.9.0/dcor_shared.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-06 17:08:36.000000 dcor_shared-0.9.0/dcor_shared.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-06 17:08:36.253926 dcor_shared-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-03-06 17:08:10.000000 dcor_shared-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:08:36.253926 dcor_shared-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-06 17:08:10.000000 dcor_shared-0.9.0/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-03-06 17:08:10.000000 dcor_shared-0.9.0/tests/test_ckan.py
--rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-03-06 17:08:10.000000 dcor_shared-0.9.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    16215 2024-03-06 17:08:10.000000 dcor_shared-0.9.0/tests/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     9706 2024-03-06 17:08:10.000000 dcor_shared-0.9.0/tests/test_s3cc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-03-06 17:08:10.000000 dcor_shared-0.9.0/tests/test_testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 08:48:15.399390 dcor_shared-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-03-07 08:47:49.000000 dcor_shared-0.9.1/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-07 08:47:49.000000 dcor_shared-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-07 08:47:49.000000 dcor_shared-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-03-07 08:48:15.399390 dcor_shared-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-03-07 08:47:49.000000 dcor_shared-0.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 08:48:15.399390 dcor_shared-0.9.1/dcor_shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-07 08:47:49.000000 dcor_shared-0.9.1/dcor_shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-03-07 08:47:49.000000 dcor_shared-0.9.1/dcor_shared/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-07 08:48:01.000000 dcor_shared-0.9.1/dcor_shared/_version_save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-03-07 08:47:49.000000 dcor_shared-0.9.1/dcor_shared/ckan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-03-07 08:47:49.000000 dcor_shared-0.9.1/dcor_shared/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-07 08:47:49.000000 dcor_shared-0.9.1/dcor_shared/dcinst.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-07 08:47:49.000000 dcor_shared-0.9.1/dcor_shared/mime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-03-07 08:47:49.000000 dcor_shared-0.9.1/dcor_shared/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-07 08:47:49.000000 dcor_shared-0.9.1/dcor_shared/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15002 2024-03-07 08:47:49.000000 dcor_shared-0.9.1/dcor_shared/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12262 2024-03-07 08:47:49.000000 dcor_shared-0.9.1/dcor_shared/s3cc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9986 2024-03-07 08:47:49.000000 dcor_shared-0.9.1/dcor_shared/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 08:48:15.399390 dcor_shared-0.9.1/dcor_shared.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-03-07 08:48:15.000000 dcor_shared-0.9.1/dcor_shared.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-03-07 08:48:15.000000 dcor_shared-0.9.1/dcor_shared.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 08:48:15.000000 dcor_shared-0.9.1/dcor_shared.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-07 08:48:15.000000 dcor_shared-0.9.1/dcor_shared.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-07 08:48:15.000000 dcor_shared-0.9.1/dcor_shared.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-07 08:48:15.399390 dcor_shared-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-03-07 08:47:49.000000 dcor_shared-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 08:48:15.399390 dcor_shared-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-07 08:47:49.000000 dcor_shared-0.9.1/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-03-07 08:47:49.000000 dcor_shared-0.9.1/tests/test_ckan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-03-07 08:47:49.000000 dcor_shared-0.9.1/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16215 2024-03-07 08:47:49.000000 dcor_shared-0.9.1/tests/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-03-07 08:47:49.000000 dcor_shared-0.9.1/tests/test_s3cc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-03-07 08:47:49.000000 dcor_shared-0.9.1/tests/test_testing.py
```

### Comparing `dcor_shared-0.9.0/CHANGELOG` & `dcor_shared-0.9.1/CHANGELOG`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+0.9.1
+ - feat: add convenience method `get_s3_attributes_for_artifact`
 0.9.0
  - feat: introduce `testing.make_dataset_via_s3` and
    `testing.make_resource_via_s3` which uploads resources via S3
  - enh: make sha256 optional in `s3.upload_file`
 0.8.0
  - feat: introduce `get_resource_dc_config`, `get_resource_info`, and
    `s3cc.get_s3_dc_handle_basin_based`
```

### Comparing `dcor_shared-0.9.0/LICENSE` & `dcor_shared-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dcor_shared-0.9.0/PKG-INFO` & `dcor_shared-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcor_shared
-Version: 0.9.0
+Version: 0.9.1
 Summary: Functionalities shared by the DCOR CKAN extensions
 Home-page: https://github.com/DCOR-dev/dcor_shared
 Author: Paul Müller
 Author-email: dev@craban.de
 License: AGPLv3+
 Keywords: DCOR
 Platform: ALL
```

### Comparing `dcor_shared-0.9.0/README.rst` & `dcor_shared-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `dcor_shared-0.9.0/dcor_shared/_version.py` & `dcor_shared-0.9.1/dcor_shared/_version.py`

 * *Files identical despite different names*

### Comparing `dcor_shared-0.9.0/dcor_shared/ckan.py` & `dcor_shared-0.9.1/dcor_shared/ckan.py`

 * *Files identical despite different names*

### Comparing `dcor_shared-0.9.0/dcor_shared/data.py` & `dcor_shared-0.9.1/dcor_shared/data.py`

 * *Files identical despite different names*

### Comparing `dcor_shared-0.9.0/dcor_shared/dcinst.py` & `dcor_shared-0.9.1/dcor_shared/dcinst.py`

 * *Files identical despite different names*

### Comparing `dcor_shared-0.9.0/dcor_shared/parse.py` & `dcor_shared-0.9.1/dcor_shared/parse.py`

 * *Files identical despite different names*

### Comparing `dcor_shared-0.9.0/dcor_shared/paths.py` & `dcor_shared-0.9.1/dcor_shared/paths.py`

 * *Files identical despite different names*

### Comparing `dcor_shared-0.9.0/dcor_shared/s3.py` & `dcor_shared-0.9.1/dcor_shared/s3.py`

 * *Files identical despite different names*

### Comparing `dcor_shared-0.9.0/dcor_shared/s3cc.py` & `dcor_shared-0.9.1/dcor_shared/s3cc.py`

 * *Files 24% similar despite different names*

```diff
@@ -57,14 +57,89 @@
         resource_id=resource_id, artifact=artifact)
     return s3.create_presigned_url(bucket_name=bucket_name,
                                    object_name=object_name,
                                    expiration=expiration,
                                    filename=filename)
 
 
+def get_s3_attributes_for_artifact(
+        resource_id: str,
+        artifact: Literal["condensed", "preview", "resource"] = "resource"):
+    """Return all attribute for an artifact in the S3 object store
+
+    Returns
+    -------
+    meta: dict
+        Metadata dictionary with the keys "etag", "server", "size",
+        and "success".
+    """
+    bucket_name, object_name = get_s3_bucket_object_for_artifact(
+        resource_id=resource_id, artifact=artifact)
+    s3_client, _, _ = s3.get_s3()
+    attr_info = s3_client.head_object(Bucket=bucket_name, Key=object_name)
+    # Example output from MinIO::
+    #
+    #     {'AcceptRanges': 'bytes',
+    #      'ContentLength': 904729,
+    #      'ContentType': 'application/octet-stream',
+    #      'ETag': '"108d47e80f3e5f35110493b1fdcd30d5"',
+    #      'LastModified': datetime.datetime(2024, 3, 7, 8, 15,
+    #                                        tzinfo=tzutc()),
+    #      'Metadata': {},
+    #      'ResponseMetadata': {
+    #         'HTTPHeaders': {
+    #             'accept-ranges': 'bytes',
+    #             'content-length': '904729',
+    #             'content-type': 'application/octet-stream',
+    #             'date': 'Thu, 07 Mar 2024 08:15:02 GMT',
+    #             'etag': '"108d47e80f3e5f35110493b1fdcd30d5"',
+    #             'last-modified': 'Thu, 07 Mar 2024 '
+    #                              '08:15:00 GMT',
+    #             'server': 'MinIO',
+    #             'strict-transport-security': 'max-age=31536000; '
+    #                                          'includeSubDomains',
+    #             'vary': 'Origin, Accept-Encoding',
+    #             'x-amz-id-2': 'dd9025bab4ad464b049177c95eb6e...',
+    #             'x-amz-request-id': '17BA6D680CB67A2C',
+    #             'x-amz-tagging-count': '1',
+    #             'x-content-type-options': 'nosniff',
+    #             'x-xss-protection': '1; mode=block'},
+    #         'HTTPStatusCode': 200,
+    #         'HostId': 'dd9025bab4ad464b049177c95eb6ebf3...',
+    #         'RequestId': '17BA6D680CB67A2C',
+    #         'RetryAttempts': 0}
+    #      }
+    meta = {}
+    for key, funcs in [
+        ("etag", [lambda m: m.get("ETag"),
+                  lambda m: m.get("ResponseMetadata",
+                                  {}).get("HTTPHeaders",
+                                          {}).get("etag"),
+                  ]),
+        ("server", [lambda m: m.get("ResponseMetadata",
+                                    {}).get("HTTPHeaders",
+                                            {}).get("server", "unknown")
+                    ]),
+        ("size", [lambda m: m.get("ContentLength"),
+                  lambda m: m.get("ResponseMetadata",
+                                  {}).get("HTTPHeaders",
+                                          {}).get("content-length"),
+                  ]),
+        ("success", [lambda m: m.get("ResponseMetadata",
+                                     {}).get("HTTPStatusCode", 404) == 200
+                     ]),
+    ]:
+        for fn in funcs:
+            val = fn(attr_info)
+            if val is not None:
+                meta[key] = val
+                break
+    return meta
+
+
 def get_s3_bucket_object_for_artifact(
         resource_id: str,
         artifact: Literal["condensed", "preview", "resource"] = "resource"):
     """Return `bucket_name` and `object_name` for an artifact of a resource
 
     The value of artifact can be either "condensed", "preview", or "resource"
     (those are the keys under which the individual objects are stored in S3).
```

### Comparing `dcor_shared-0.9.0/dcor_shared/testing.py` & `dcor_shared-0.9.1/dcor_shared/testing.py`

 * *Files identical despite different names*

### Comparing `dcor_shared-0.9.0/dcor_shared.egg-info/PKG-INFO` & `dcor_shared-0.9.1/dcor_shared.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcor-shared
-Version: 0.9.0
+Version: 0.9.1
 Summary: Functionalities shared by the DCOR CKAN extensions
 Home-page: https://github.com/DCOR-dev/dcor_shared
 Author: Paul Müller
 Author-email: dev@craban.de
 License: AGPLv3+
 Keywords: DCOR
 Platform: ALL
```

### Comparing `dcor_shared-0.9.0/dcor_shared.egg-info/SOURCES.txt` & `dcor_shared-0.9.1/dcor_shared.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcor_shared-0.9.0/setup.py` & `dcor_shared-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `dcor_shared-0.9.0/tests/test_ckan.py` & `dcor_shared-0.9.1/tests/test_ckan.py`

 * *Files identical despite different names*

### Comparing `dcor_shared-0.9.0/tests/test_data.py` & `dcor_shared-0.9.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `dcor_shared-0.9.0/tests/test_s3.py` & `dcor_shared-0.9.1/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `dcor_shared-0.9.0/tests/test_s3cc.py` & `dcor_shared-0.9.1/tests/test_s3cc.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,33 @@
         "490efdf5d9bb4cd4b2a6bcf2fe54d4dc201c38530140bcb168980bf8bf846c73"
 
 
 @pytest.mark.ckan_config('ckan.plugins', 'dcor_schemas')
 @pytest.mark.usefixtures('clean_db', 'with_request_context')
 @mock.patch('ckan.plugins.toolkit.enqueue_job',
             side_effect=synchronous_enqueue_job)
+def test_get_s3_attributes_for_artifact(enqueue_job_mock):
+    rid, _, _, org_dict = setup_s3_resource_on_ckan()
+
+    # Make sure the resource exists
+    res_dict = helpers.call_action("resource_show", id=rid)
+    assert res_dict["id"] == rid, "sanity check"
+
+    # get the size
+    meta = s3cc.get_s3_attributes_for_artifact(rid)
+    assert meta["size"] == 904729
+    assert meta["success"]
+    assert meta["etag"]
+    assert meta["server"]
+
+
+@pytest.mark.ckan_config('ckan.plugins', 'dcor_schemas')
+@pytest.mark.usefixtures('clean_db', 'with_request_context')
+@mock.patch('ckan.plugins.toolkit.enqueue_job',
+            side_effect=synchronous_enqueue_job)
 def test_get_s3_bucket_object_for_artifact(enqueue_job_mock):
     rid, _, _, org_dict = setup_s3_resource_on_ckan()
 
     # Make sure the resource exists
     res_dict = helpers.call_action("resource_show", id=rid)
     assert res_dict["id"] == rid, "sanity check"
```

### Comparing `dcor_shared-0.9.0/tests/test_testing.py` & `dcor_shared-0.9.1/tests/test_testing.py`

 * *Files identical despite different names*

