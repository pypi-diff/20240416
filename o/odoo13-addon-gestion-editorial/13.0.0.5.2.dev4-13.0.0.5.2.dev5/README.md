# Comparing `tmp/odoo13-addon-gestion_editorial-13.0.0.5.2.dev4.tar.gz` & `tmp/odoo13-addon-gestion_editorial-13.0.0.5.2.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo13-addon-gestion_editorial-13.0.0.5.2.dev4.tar", last modified: Tue Mar 26 19:13:27 2024, max compression
+gzip compressed data, was "odoo13-addon-gestion_editorial-13.0.0.5.2.dev5.tar", last modified: Tue Apr 16 13:11:12 2024, max compression
```

## Comparing `odoo13-addon-gestion_editorial-13.0.0.5.2.dev4.tar` & `odoo13-addon-gestion_editorial-13.0.0.5.2.dev5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:13:27.979366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/
--rw-r--r--   0 root         (0) root         (0)      526 2024-03-26 19:13:27.979366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-03-26 19:13:27.975366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1770 2024-03-26 19:13:27.975366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/__manifest__.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-03-26 19:13:27.975366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:13:27.975366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/data/
--rw-rw-rw-   0 root         (0) root         (0)     1009 2024-03-26 19:13:27.975366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/data/deposito_compra_data.xml
--rw-rw-rw-   0 root         (0) root         (0)      491 2024-03-26 19:13:27.975366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/data/product_categories_ddaa_data.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:13:27.975366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/i18n_extra/
--rwxrwxrwx   0 root         (0) root         (0)      790 2024-03-26 19:13:27.975366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/i18n_extra/es.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:13:27.975366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/models/
--rw-rw-rw-   0 root         (0) root         (0)      372 2024-03-26 19:13:27.975366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19855 2024-03-26 19:13:27.975366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/models/liquidacion_descontrol.py
--rw-rw-rw-   0 root         (0) root         (0)    13148 2024-03-26 19:13:27.975366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/models/product_descontrol.py
--rw-rw-rw-   0 root         (0) root         (0)      304 2024-03-26 19:13:27.975366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/models/product_pricelist_descontrol.py
--rw-rw-rw-   0 root         (0) root         (0)     3280 2024-03-26 19:13:27.975366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/models/purchase_order_descontrol.py
--rw-rw-rw-   0 root         (0) root         (0)     2557 2024-03-26 19:13:27.975366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/models/res_company_descontrol.py
--rw-rw-rw-   0 root         (0) root         (0)      867 2024-03-26 19:13:27.975366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/models/res_config_settings_descontrol.py
--rw-rw-rw-   0 root         (0) root         (0)     1372 2024-03-26 19:13:27.975366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/models/res_partner_descontrol.py
--rw-rw-rw-   0 root         (0) root         (0)     1301 2024-03-26 19:13:27.975366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/models/sale_order_descontrol.py
--rw-rw-rw-   0 root         (0) root         (0)     8421 2024-03-26 19:13:27.975366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/models/stock_picking_descontrol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:13:27.975366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:13:27.975366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/static/description/
--rw-rw-rw-   0 root         (0) root         (0)    19361 2024-03-26 19:13:27.975366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/static/description/icon.png
--rw-rw-rw-   0 root         (0) root         (0)     2595 2024-03-26 19:13:27.975366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/static/description/logo-devcontrol.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:13:27.979366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/views/
--rw-rw-rw-   0 root         (0) root         (0)    11654 2024-03-26 19:13:27.979366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/views/liquidacion_descontrol_view.xml
--rw-rw-rw-   0 root         (0) root         (0)    19929 2024-03-26 19:13:27.979366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/views/product_descontrol_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      634 2024-03-26 19:13:27.979366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/views/product_pricelist_descontrol_view.xml
--rw-rw-rw-   0 root         (0) root         (0)     1961 2024-03-26 19:13:27.979366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/views/purchase_order_descontrol_view.xml
--rw-rw-rw-   0 root         (0) root         (0)     2406 2024-03-26 19:13:27.979366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/views/report_invoice_document_descontrol_view.xml
--rw-rw-rw-   0 root         (0) root         (0)     4646 2024-03-26 19:13:27.979366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/views/report_saleorder_document_descontrol_view.xml
--rw-rw-rw-   0 root         (0) root         (0)     3605 2024-03-26 19:13:27.979366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/views/res_config_settings_descontrol_view.xml
--rw-rw-rw-   0 root         (0) root         (0)     1633 2024-03-26 19:13:27.979366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/views/res_partner_descontrol_view.xml
--rw-rw-rw-   0 root         (0) root         (0)     1088 2024-03-26 19:13:27.979366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/views/sale_order_descontrol_view.xml
--rw-rw-rw-   0 root         (0) root         (0)     1577 2024-03-26 19:13:27.979366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/views/stock_picking_descontrol_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      446 2024-03-26 19:13:27.979366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/views/stock_quant_descontrol_view.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:13:27.979366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/wizards/
--rw-rw-rw-   0 root         (0) root         (0)       44 2024-03-26 19:13:27.979366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/wizards/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 19:13:27.979366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/wizards/liquidacion_lineas_pendientes/
--rw-rw-rw-   0 root         (0) root         (0)       44 2024-03-26 19:13:27.979366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/wizards/liquidacion_lineas_pendientes/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10172 2024-03-26 19:13:27.979366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/wizards/liquidacion_lineas_pendientes/liquidacion_lineas_pendientes.py
--rw-rw-rw-   0 root         (0) root         (0)     4767 2024-03-26 19:13:27.979366 odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/wizards/liquidacion_lineas_pendientes/liquidacion_lineas_pendientes.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:11:12.166043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/
+-rw-r--r--   0 root         (0) root         (0)      526 2024-04-16 13:11:12.166043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-04-16 13:11:12.162043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1876 2024-04-16 13:11:12.162043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/__manifest__.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-16 13:11:12.162043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:11:12.162043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/data/
+-rw-rw-rw-   0 root         (0) root         (0)     1009 2024-04-16 13:11:12.162043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/data/deposito_compra_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)      491 2024-04-16 13:11:12.162043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/data/product_categories_ddaa_data.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:11:12.162043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/i18n_extra/
+-rwxrwxrwx   0 root         (0) root         (0)      790 2024-04-16 13:11:12.162043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/i18n_extra/es.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:11:12.162043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/models/
+-rw-rw-rw-   0 root         (0) root         (0)      372 2024-04-16 13:11:12.162043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19855 2024-04-16 13:11:12.162043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/models/liquidacion_descontrol.py
+-rw-rw-rw-   0 root         (0) root         (0)    13148 2024-04-16 13:11:12.162043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/models/product_descontrol.py
+-rw-rw-rw-   0 root         (0) root         (0)      304 2024-04-16 13:11:12.162043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/models/product_pricelist_descontrol.py
+-rw-rw-rw-   0 root         (0) root         (0)     3280 2024-04-16 13:11:12.162043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/models/purchase_order_descontrol.py
+-rw-rw-rw-   0 root         (0) root         (0)     2557 2024-04-16 13:11:12.162043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/models/res_company_descontrol.py
+-rw-rw-rw-   0 root         (0) root         (0)      867 2024-04-16 13:11:12.162043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/models/res_config_settings_descontrol.py
+-rw-rw-rw-   0 root         (0) root         (0)     1372 2024-04-16 13:11:12.162043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/models/res_partner_descontrol.py
+-rw-rw-rw-   0 root         (0) root         (0)     1301 2024-04-16 13:11:12.162043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/models/sale_order_descontrol.py
+-rw-rw-rw-   0 root         (0) root         (0)     8421 2024-04-16 13:11:12.162043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/models/stock_picking_descontrol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:11:12.162043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:11:12.162043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/static/description/
+-rw-rw-rw-   0 root         (0) root         (0)    19361 2024-04-16 13:11:12.162043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/static/description/icon.png
+-rw-rw-rw-   0 root         (0) root         (0)     2595 2024-04-16 13:11:12.162043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/static/description/logo-devcontrol.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:11:12.166043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/views/
+-rw-rw-rw-   0 root         (0) root         (0)    11654 2024-04-16 13:11:12.166043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/views/liquidacion_descontrol_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)    19929 2024-04-16 13:11:12.166043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/views/product_descontrol_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      634 2024-04-16 13:11:12.166043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/views/product_pricelist_descontrol_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1961 2024-04-16 13:11:12.166043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/views/purchase_order_descontrol_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2406 2024-04-16 13:11:12.166043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/views/report_invoice_document_descontrol_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     4646 2024-04-16 13:11:12.166043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/views/report_saleorder_document_descontrol_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     3605 2024-04-16 13:11:12.166043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/views/res_config_settings_descontrol_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1633 2024-04-16 13:11:12.166043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/views/res_partner_descontrol_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2024-04-16 13:11:12.166043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/views/sale_order_descontrol_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1577 2024-04-16 13:11:12.166043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/views/stock_picking_descontrol_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      446 2024-04-16 13:11:12.166043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/views/stock_quant_descontrol_view.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:11:12.166043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/wizards/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2024-04-16 13:11:12.166043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/wizards/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 13:11:12.166043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/wizards/liquidacion_lineas_pendientes/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2024-04-16 13:11:12.166043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/wizards/liquidacion_lineas_pendientes/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10172 2024-04-16 13:11:12.166043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/wizards/liquidacion_lineas_pendientes/liquidacion_lineas_pendientes.py
+-rw-rw-rw-   0 root         (0) root         (0)     4767 2024-04-16 13:11:12.166043 odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/wizards/liquidacion_lineas_pendientes/liquidacion_lineas_pendientes.xml
```

### Comparing `odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/PKG-INFO` & `odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo13-addon-gestion_editorial
-Version: 13.0.0.5.2.dev4
+Version: 13.0.0.5.2.dev5
 Requires-Python: >=3.5
 Requires-Dist: odoo13-addon-account_invoice_pricelist
 Requires-Dist: odoo>=13.0a,<13.1dev
 Summary: =?utf-8?q?M=C3=B3dulo_para_gesti=C3=B3n_de_la_editorial_Descontrol=2E?=
 Home-page: https://framagit.org/devcontrol
 License: OPL-1
 Author: Colectivo DEVCONTROL
```

### Comparing `odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/__manifest__.py` & `odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/__manifest__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,25 @@
     'description': 'Módulo para gestión de la editorial Descontrol.',
     'category': 'Industries',
     'author': 'Colectivo DEVCONTROL',
     'author_email': 'devcontrol@zici.fr',
     'maintainer': 'Colectivo DEVCONTROL',
     'company': 'Colectivo DEVCONTROL',
     'website': 'https://framagit.org/devcontrol',
-    'depends': ['product', 'account', 'sale_stock', 'base', 'account_invoice_pricelist', 'sale_purchase', 'stock'],
+    'depends': [
+        'account',
+        'account_invoice_pricelist',
+        'base',
+        'product',
+        'sale',
+        'sale_management',
+        'sale_purchase',
+        'sale_stock',
+        'stock',
+    ],
     'data': [
         'data/product_categories_ddaa_data.xml',
         'data/deposito_compra_data.xml',
         'wizards/liquidacion_lineas_pendientes/liquidacion_lineas_pendientes.xml',
         'views/product_descontrol_view.xml',
         'views/res_partner_descontrol_view.xml',
         'views/liquidacion_descontrol_view.xml',
```

### Comparing `odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/data/deposito_compra_data.xml` & `odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/data/deposito_compra_data.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/i18n_extra/es.po` & `odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/i18n_extra/es.po`

 * *Files identical despite different names*

### Comparing `odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/models/liquidacion_descontrol.py` & `odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/models/liquidacion_descontrol.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/models/product_descontrol.py` & `odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/models/product_descontrol.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/models/purchase_order_descontrol.py` & `odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/models/purchase_order_descontrol.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/models/res_company_descontrol.py` & `odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/models/res_company_descontrol.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/models/res_config_settings_descontrol.py` & `odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/models/res_config_settings_descontrol.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/models/res_partner_descontrol.py` & `odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/models/res_partner_descontrol.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/models/sale_order_descontrol.py` & `odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/models/sale_order_descontrol.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/models/stock_picking_descontrol.py` & `odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/models/stock_picking_descontrol.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/static/description/icon.png` & `odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/static/description/icon.png`

 * *Files identical despite different names*

### Comparing `odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/static/description/logo-devcontrol.png` & `odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/static/description/logo-devcontrol.png`

 * *Files identical despite different names*

### Comparing `odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/views/liquidacion_descontrol_view.xml` & `odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/views/liquidacion_descontrol_view.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/views/product_descontrol_view.xml` & `odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/views/product_descontrol_view.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/views/product_pricelist_descontrol_view.xml` & `odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/views/product_pricelist_descontrol_view.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/views/purchase_order_descontrol_view.xml` & `odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/views/purchase_order_descontrol_view.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/views/report_invoice_document_descontrol_view.xml` & `odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/views/report_invoice_document_descontrol_view.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/views/report_saleorder_document_descontrol_view.xml` & `odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/views/report_saleorder_document_descontrol_view.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/views/res_config_settings_descontrol_view.xml` & `odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/views/res_config_settings_descontrol_view.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/views/res_partner_descontrol_view.xml` & `odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/views/res_partner_descontrol_view.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/views/sale_order_descontrol_view.xml` & `odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/views/sale_order_descontrol_view.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/views/stock_picking_descontrol_view.xml` & `odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/views/stock_picking_descontrol_view.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/wizards/liquidacion_lineas_pendientes/liquidacion_lineas_pendientes.py` & `odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/wizards/liquidacion_lineas_pendientes/liquidacion_lineas_pendientes.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-gestion_editorial-13.0.0.5.2.dev4/wizards/liquidacion_lineas_pendientes/liquidacion_lineas_pendientes.xml` & `odoo13-addon-gestion_editorial-13.0.0.5.2.dev5/wizards/liquidacion_lineas_pendientes/liquidacion_lineas_pendientes.xml`

 * *Files identical despite different names*

