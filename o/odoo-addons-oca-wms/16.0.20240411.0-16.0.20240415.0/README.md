# Comparing `tmp/odoo_addons_oca_wms-16.0.20240411.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_wms-16.0.20240415.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1594 bytes, number of entries: 4
--rw-r--r--  2.0 unx     2711 b- defN 24-Apr-12 06:36 odoo_addons_oca_wms-16.0.20240411.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-12 06:36 odoo_addons_oca_wms-16.0.20240411.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-12 06:36 odoo_addons_oca_wms-16.0.20240411.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      385 b- defN 24-Apr-12 06:36 odoo_addons_oca_wms-16.0.20240411.0.dist-info/RECORD
-4 files, 3189 bytes uncompressed, 836 bytes compressed:  73.8%
+Zip file size: 1604 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     2805 b- defN 24-Apr-16 08:26 odoo_addons_oca_wms-16.0.20240415.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-16 08:26 odoo_addons_oca_wms-16.0.20240415.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-16 08:26 odoo_addons_oca_wms-16.0.20240415.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      385 b- defN 24-Apr-16 08:26 odoo_addons_oca_wms-16.0.20240415.0.dist-info/RECORD
+4 files, 3283 bytes uncompressed, 846 bytes compressed:  74.2%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_wms-16.0.20240411.0.dist-info/METADATA
+Filename: odoo_addons_oca_wms-16.0.20240415.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_wms-16.0.20240411.0.dist-info/WHEEL
+Filename: odoo_addons_oca_wms-16.0.20240415.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_wms-16.0.20240411.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_wms-16.0.20240415.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_wms-16.0.20240411.0.dist-info/RECORD
+Filename: odoo_addons_oca_wms-16.0.20240415.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_wms-16.0.20240411.0.dist-info/METADATA` & `odoo_addons_oca_wms-16.0.20240415.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-wms
-Version: 16.0.20240411.0
+Version: 16.0.20240415.0
 Summary: Meta package for oca-wms Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
@@ -28,14 +28,15 @@
 Requires-Dist: odoo-addon-stock-release-channel-partner-public-holidays <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-release-channel-plan <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-release-channel-plan-process-end-time <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-release-channel-process-end-time <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-release-channel-propagate-channel-picking <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-release-channel-shipment-advice <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-release-channel-shipment-advice-process-end-time <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-stock-release-channel-shipment-advice-toursolver <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-release-channel-shipment-lead-time <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-release-channel-show-volume <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-release-channel-show-weight <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-storage-type <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-storage-type-putaway-abc <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-warehouse-flow <16.1dev,>=16.0dev
```

