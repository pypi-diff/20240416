# Comparing `tmp/drivelinepy-1.6.1.tar.gz` & `tmp/drivelinepy-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drivelinepy-1.6.1.tar", last modified: Tue Apr  2 18:15:06 2024, max compression
+gzip compressed data, was "drivelinepy-1.7.1.tar", last modified: Mon Apr 15 23:10:04 2024, max compression
```

## Comparing `drivelinepy-1.6.1.tar` & `drivelinepy-1.7.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:06.283155 drivelinepy-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-02 18:14:50.000000 drivelinepy-1.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-02 18:15:06.283155 drivelinepy-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-02 18:14:50.000000 drivelinepy-1.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:06.283155 drivelinepy-1.6.1/drivelinepy/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-02 18:14:50.000000 drivelinepy-1.6.1/drivelinepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7335 2024-04-02 18:14:50.000000 drivelinepy-1.6.1/drivelinepy/base_api_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7806 2024-04-02 18:14:50.000000 drivelinepy-1.6.1/drivelinepy/brightpearl_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:06.283155 drivelinepy-1.6.1/drivelinepy/brightpearl_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:14:50.000000 drivelinepy-1.6.1/drivelinepy/brightpearl_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-02 18:14:50.000000 drivelinepy-1.6.1/drivelinepy/brightpearl_utils/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-02 18:14:50.000000 drivelinepy-1.6.1/drivelinepy/slack_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10787 2024-04-02 18:14:50.000000 drivelinepy-1.6.1/drivelinepy/traq_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-04-02 18:14:50.000000 drivelinepy-1.6.1/drivelinepy/virtuagym_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    17384 2024-04-02 18:14:50.000000 drivelinepy-1.6.1/drivelinepy/zoho_billing_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10899 2024-04-02 18:14:50.000000 drivelinepy-1.6.1/drivelinepy/zoho_crm_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:06.283155 drivelinepy-1.6.1/drivelinepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-02 18:15:06.000000 drivelinepy-1.6.1/drivelinepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-02 18:15:06.000000 drivelinepy-1.6.1/drivelinepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 18:15:06.000000 drivelinepy-1.6.1/drivelinepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-02 18:15:06.000000 drivelinepy-1.6.1/drivelinepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 18:15:06.000000 drivelinepy-1.6.1/drivelinepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 18:15:06.283155 drivelinepy-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-02 18:14:50.000000 drivelinepy-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:10:04.737076 drivelinepy-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-15 23:09:56.000000 drivelinepy-1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-15 23:10:04.737076 drivelinepy-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-15 23:09:56.000000 drivelinepy-1.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:10:04.737076 drivelinepy-1.7.1/drivelinepy/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-15 23:09:56.000000 drivelinepy-1.7.1/drivelinepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7335 2024-04-15 23:09:56.000000 drivelinepy-1.7.1/drivelinepy/base_api_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7806 2024-04-15 23:09:56.000000 drivelinepy-1.7.1/drivelinepy/brightpearl_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:10:04.737076 drivelinepy-1.7.1/drivelinepy/brightpearl_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 23:09:56.000000 drivelinepy-1.7.1/drivelinepy/brightpearl_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-15 23:09:56.000000 drivelinepy-1.7.1/drivelinepy/brightpearl_utils/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-15 23:09:56.000000 drivelinepy-1.7.1/drivelinepy/slack_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10787 2024-04-15 23:09:56.000000 drivelinepy-1.7.1/drivelinepy/traq_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-04-15 23:09:56.000000 drivelinepy-1.7.1/drivelinepy/virtuagym_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17384 2024-04-15 23:09:56.000000 drivelinepy-1.7.1/drivelinepy/zoho_billing_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11910 2024-04-15 23:09:56.000000 drivelinepy-1.7.1/drivelinepy/zoho_crm_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:10:04.737076 drivelinepy-1.7.1/drivelinepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-15 23:10:04.000000 drivelinepy-1.7.1/drivelinepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-15 23:10:04.000000 drivelinepy-1.7.1/drivelinepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 23:10:04.000000 drivelinepy-1.7.1/drivelinepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-15 23:10:04.000000 drivelinepy-1.7.1/drivelinepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-15 23:10:04.000000 drivelinepy-1.7.1/drivelinepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 23:10:04.737076 drivelinepy-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-15 23:09:56.000000 drivelinepy-1.7.1/setup.py
```

### Comparing `drivelinepy-1.6.1/LICENSE` & `drivelinepy-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `drivelinepy-1.6.1/PKG-INFO` & `drivelinepy-1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drivelinepy
-Version: 1.6.1
+Version: 1.7.1
 Summary: A Python package for Driveline Baseball API interactions
 Home-page: https://github.com/drivelineresearch/drivelinepy
 Author: Garrett York
 Author-email: garrett@drivelinebaseball.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `drivelinepy-1.6.1/drivelinepy/base_api_wrapper.py` & `drivelinepy-1.7.1/drivelinepy/base_api_wrapper.py`

 * *Files identical despite different names*

### Comparing `drivelinepy-1.6.1/drivelinepy/brightpearl_api.py` & `drivelinepy-1.7.1/drivelinepy/brightpearl_api.py`

 * *Files identical despite different names*

### Comparing `drivelinepy-1.6.1/drivelinepy/brightpearl_utils/helper_functions.py` & `drivelinepy-1.7.1/drivelinepy/brightpearl_utils/helper_functions.py`

 * *Files identical despite different names*

### Comparing `drivelinepy-1.6.1/drivelinepy/slack_api.py` & `drivelinepy-1.7.1/drivelinepy/slack_api.py`

 * *Files identical despite different names*

### Comparing `drivelinepy-1.6.1/drivelinepy/traq_api.py` & `drivelinepy-1.7.1/drivelinepy/traq_api.py`

 * *Files identical despite different names*

### Comparing `drivelinepy-1.6.1/drivelinepy/virtuagym_api.py` & `drivelinepy-1.7.1/drivelinepy/virtuagym_api.py`

 * *Files identical despite different names*

### Comparing `drivelinepy-1.6.1/drivelinepy/zoho_billing_api.py` & `drivelinepy-1.7.1/drivelinepy/zoho_billing_api.py`

 * *Files identical despite different names*

### Comparing `drivelinepy-1.6.1/drivelinepy/zoho_crm_api.py` & `drivelinepy-1.7.1/drivelinepy/zoho_crm_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,14 +235,43 @@
 
         all_records = self._fetch_data(endpoint, initial_params=params, data_key=data_key, page=page)
         
         self.logger.info(f"Exiting get_customer_records() with total {len(all_records)} records fetched")
         return all_records
     
     #-----------------------------------------------------------------
+    # Method - Get Deals
+    #-----------------------------------------------------------------
+
+    def get_deals(self, deal_id=None, page=1):
+        """
+        Fetches deal records from the Zoho CRM API based on the specified criteria.
+        :param deal_id: The ID of the deal to fetch.
+        :param page: The page number to fetch.
+        """
+        self.logger.info("Entering get_deals()")
+
+        endpoint = "Deals"
+        params = {}
+        data_key = "data"
+
+        if deal_id:
+            try:
+                deal_id = int(deal_id)
+            except:
+                self.logger.error("Invalid deal_id provided.")
+                return None
+            endpoint += f"/{deal_id}"
+        
+        all_deals = self._fetch_data(endpoint, initial_params=params, data_key=data_key, page=page)
+        
+        self.logger.info(f"Exiting get_deals() with total {len(all_deals)} deals fetched")
+        return all_deals
+    
+    #-----------------------------------------------------------------
     # Method - Get Supported Modules
     #-----------------------------------------------------------------
 
     def get_supported_modules(self):
         return self.SUPPORTED_MODULES
     
     def check_if_module_is_supported(self, module, ):
```

### Comparing `drivelinepy-1.6.1/drivelinepy.egg-info/PKG-INFO` & `drivelinepy-1.7.1/drivelinepy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drivelinepy
-Version: 1.6.1
+Version: 1.7.1
 Summary: A Python package for Driveline Baseball API interactions
 Home-page: https://github.com/drivelineresearch/drivelinepy
 Author: Garrett York
 Author-email: garrett@drivelinebaseball.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `drivelinepy-1.6.1/drivelinepy.egg-info/SOURCES.txt` & `drivelinepy-1.7.1/drivelinepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drivelinepy-1.6.1/setup.py` & `drivelinepy-1.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your README file
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='drivelinepy',
-    version='1.6.1',
+    version='1.7.1',
     author='Garrett York',
     author_email='garrett@drivelinebaseball.com',
     description='A Python package for Driveline Baseball API interactions',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/drivelineresearch/drivelinepy',
     packages=find_packages(),
```

