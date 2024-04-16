# Comparing `tmp/odoo_addons_oca_stock_logistics_workflow-16.0.20240411.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_stock_logistics_workflow-16.0.20240415.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 2185 bytes, number of entries: 4
--rw-r--r--  2.0 unx     5641 b- defN 24-Apr-12 06:16 odoo_addons_oca_stock_logistics_workflow-16.0.20240411.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-12 06:16 odoo_addons_oca_stock_logistics_workflow-16.0.20240411.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-12 06:16 odoo_addons_oca_stock_logistics_workflow-16.0.20240411.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      469 b- defN 24-Apr-12 06:16 odoo_addons_oca_stock_logistics_workflow-16.0.20240411.0.dist-info/RECORD
-4 files, 6203 bytes uncompressed, 1259 bytes compressed:  79.7%
+Zip file size: 2211 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     5805 b- defN 24-Apr-16 07:54 odoo_addons_oca_stock_logistics_workflow-16.0.20240415.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-16 07:54 odoo_addons_oca_stock_logistics_workflow-16.0.20240415.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-16 07:54 odoo_addons_oca_stock_logistics_workflow-16.0.20240415.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      469 b- defN 24-Apr-16 07:54 odoo_addons_oca_stock_logistics_workflow-16.0.20240415.1.dist-info/RECORD
+4 files, 6367 bytes uncompressed, 1285 bytes compressed:  79.8%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_stock_logistics_workflow-16.0.20240411.0.dist-info/METADATA
+Filename: odoo_addons_oca_stock_logistics_workflow-16.0.20240415.1.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_stock_logistics_workflow-16.0.20240411.0.dist-info/WHEEL
+Filename: odoo_addons_oca_stock_logistics_workflow-16.0.20240415.1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_stock_logistics_workflow-16.0.20240411.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_stock_logistics_workflow-16.0.20240415.1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_stock_logistics_workflow-16.0.20240411.0.dist-info/RECORD
+Filename: odoo_addons_oca_stock_logistics_workflow-16.0.20240415.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_stock_logistics_workflow-16.0.20240411.0.dist-info/METADATA` & `odoo_addons_oca_stock_logistics_workflow-16.0.20240415.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-stock-logistics-workflow
-Version: 16.0.20240411.0
+Version: 16.0.20240415.1
 Summary: Meta package for oca-stock-logistics-workflow Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
 Requires-Dist: odoo-addon-delivery-procurement-group-carrier <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-delivery-total-weight-from-packaging <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-purchase-stock-picking-invoice-link <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-line-returned-qty <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-order-global-stock-route <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-sale-stock-restocking-fee-invoicing <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-account-product-run-fifo-hook <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-auto-move <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-customer-deposit <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-delivery-note <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-grn <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-landed-costs-currency <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-landed-costs-purchase-auto <16.1dev,>=16.0dev
@@ -57,14 +58,15 @@
 Requires-Dist: odoo-addon-stock-picking-line-sequence <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-picking-mass-action <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-picking-partner-note <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-picking-product-link <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-picking-progress <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-picking-purchase-order-link <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-picking-quick <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-stock-picking-restrict-cancel-printed <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-picking-sale-order-link <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-picking-send-by-mail <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-picking-show-backorder <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-picking-show-return <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-picking-start <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-picking-supplier-ref <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-picking-to-batch-group-fields <16.1dev,>=16.0dev
```

