# Comparing `tmp/rubin.citsci-0.3.1.tar.gz` & `tmp/rubin_citsci-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubin.citsci-0.3.1.tar", last modified: Thu Mar 21 18:05:03 2024, max compression
+gzip compressed data, was "rubin_citsci-0.3.2.tar", last modified: Tue Apr 16 16:51:58 2024, max compression
```

## Comparing `rubin.citsci-0.3.1.tar` & `rubin_citsci-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:05:03.468864 rubin.citsci-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    16157 2024-03-21 18:04:58.000000 rubin.citsci-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-21 18:05:03.468864 rubin.citsci-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-21 18:04:58.000000 rubin.citsci-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-21 18:04:58.000000 rubin.citsci-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 18:05:03.468864 rubin.citsci-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:05:03.464864 rubin.citsci-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:05:03.464864 rubin.citsci-0.3.1/src/rubin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:05:03.468864 rubin.citsci-0.3.1/src/rubin/citsci/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 18:04:58.000000 rubin.citsci-0.3.1/src/rubin/citsci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21120 2024-03-21 18:04:58.000000 rubin.citsci-0.3.1/src/rubin/citsci/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:05:03.468864 rubin.citsci-0.3.1/src/rubin.citsci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-21 18:05:03.000000 rubin.citsci-0.3.1/src/rubin.citsci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-21 18:05:03.000000 rubin.citsci-0.3.1/src/rubin.citsci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 18:05:03.000000 rubin.citsci-0.3.1/src/rubin.citsci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-21 18:05:03.000000 rubin.citsci-0.3.1/src/rubin.citsci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-21 18:05:03.000000 rubin.citsci-0.3.1/src/rubin.citsci.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:51:58.066398 rubin_citsci-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    16157 2024-04-16 16:51:54.000000 rubin_citsci-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-16 16:51:58.066398 rubin_citsci-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-16 16:51:54.000000 rubin_citsci-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-16 16:51:54.000000 rubin_citsci-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 16:51:58.066398 rubin_citsci-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:51:58.066398 rubin_citsci-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:51:58.066398 rubin_citsci-0.3.2/src/rubin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:51:58.066398 rubin_citsci-0.3.2/src/rubin/citsci/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 16:51:54.000000 rubin_citsci-0.3.2/src/rubin/citsci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21281 2024-04-16 16:51:54.000000 rubin_citsci-0.3.2/src/rubin/citsci/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:51:58.066398 rubin_citsci-0.3.2/src/rubin.citsci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-16 16:51:58.000000 rubin_citsci-0.3.2/src/rubin.citsci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-16 16:51:58.000000 rubin_citsci-0.3.2/src/rubin.citsci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 16:51:58.000000 rubin_citsci-0.3.2/src/rubin.citsci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-16 16:51:58.000000 rubin_citsci-0.3.2/src/rubin.citsci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 16:51:58.000000 rubin_citsci-0.3.2/src/rubin.citsci.egg-info/top_level.txt
```

### Comparing `rubin.citsci-0.3.1/LICENSE` & `rubin_citsci-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rubin.citsci-0.3.1/src/rubin/citsci/pipeline.py` & `rubin_citsci-0.3.2/src/rubin/citsci/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,15 +270,15 @@
         storage_client = storage.Client()
         bucket = storage_client.bucket(bucket_name)
         blob = bucket.blob(self.guid + "/manifest.csv")
 
         blob.upload_from_filename(manifest_path)
         return
 
-    def send_image_data(self, subject_set_name, zip_path):
+    def send_image_data(self, subject_set_name, zip_path, **options):
         """
             Sends the new data batch to the Rubin EPO Data Center for public hosting
             so that the data can be added to the target Zooniverse project.
 
             Several events need to have occurred for this function to complete
             successfully:
             
@@ -309,15 +309,17 @@
         self.step = 0
         self.log_step("Checking batch status")
         if self.__has_active_batch() == True:
             raise CitizenSciencePipelineError("INCOMPLETE SUBJECT SET EXISTS! You cannot send another batch of data while a subject set is still active (not yet retired) on the Zooniverse platform - you can only send a new batch of data if all subject sets associated to a project have been completed.")
         self.__upload_cutouts(zip_path)
         self.__create_new_subject_set(subject_set_name)
 
-        self.edc_response = self.__alert_edc_of_new_citsci_data()
+        contains_flipbook = options.get("flipbook") if "flipbook" in options else False
+
+        self.edc_response = self.__alert_edc_of_new_citsci_data(flipbook=contains_flipbook)
         
         self.__process_edc_response()
         return
     
     def __get_gcp_location(self):
         return base64.b64decode("L29wdC9sc3N0L3NvZnR3YXJlL2p1cHl0ZXJsYWIvc2VjcmV0cy9idXRsZXItZ2NzLWlkZi1jcmVkcy5qc29u").decode("ascii")
             
@@ -379,26 +381,26 @@
         storage_client = storage.Client()
         bucket = storage_client.bucket(bucket_name)
         blob = bucket.blob(destination_blob_name)
 
         blob.upload_from_filename(source_file_name)
         return
 
-    def __alert_edc_of_new_citsci_data(self, tabular = False):
+    def __alert_edc_of_new_citsci_data(self, flipbook=False, tabular = False):
         """
             This function is called as part of the send_image_data()  workflow and should
             not be accessed publicly as unexpected results will occur.
         """
 
         project_id_str = str(self.project_id)
         self.log_step("Notifying the Rubin EPO Data Center of the new data, which will finish processing of the data and notify Zooniverse")
 
         try:
             resource = "citizen-science-image-ingest" if tabular == False else "citizen-science-tabular-ingest"
-            edc_endpoint = f"https://rsp-data-exporter{self.dev_mode_url}-dot-skyviewer.uw.r.appspot.com/{resource}?email={self.email}&vendor_project_id={project_id_str}&guid={self.guid}&vendor_batch_id={str(self.vendor_batch_id)}&debug=True"
+            edc_endpoint = f"https://rsp-data-exporter{self.dev_mode_url}-dot-skyviewer.uw.r.appspot.com/{resource}?email={self.email}&vendor_project_id={project_id_str}&guid={self.guid}&vendor_batch_id={str(self.vendor_batch_id)}&flipbook={flipbook}&debug=True"
             # print(edc_endpoint)
             response = urllib.request.urlopen(edc_endpoint, timeout=3600).read()
             str(response)
             manifestUrl = response.decode('UTF-8')
             return manifestUrl
         except Exception as e:
             self.clean_up_unused_subject_set()
@@ -464,8 +466,8 @@
 
     # Constructor or Initializer
     def __init__(self, value):
         self.value = value
 
     # __str__ is to print() the value
     def __str__(self):
-        return(repr(self.value))
+        return(repr(self.value))
```

