# Comparing `tmp/ticketsdk-2.3.0.tar.gz` & `tmp/ticketsdk-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ticketsdk-2.3.0.tar", last modified: Fri Apr 12 04:03:54 2024, max compression
+gzip compressed data, was "ticketsdk-2.3.1.tar", last modified: Mon Apr 15 09:25:41 2024, max compression
```

## Comparing `ticketsdk-2.3.0.tar` & `ticketsdk-2.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-12 04:03:54.566671 ticketsdk-2.3.0/
--rw-r--r--   0 phamchuong   (501) staff       (20)      503 2024-04-12 04:03:54.566474 ticketsdk-2.3.0/PKG-INFO
--rw-r--r--   0 phamchuong   (501) staff       (20)     1717 2024-04-11 09:47:21.000000 ticketsdk-2.3.0/README.md
--rw-r--r--   0 phamchuong   (501) staff       (20)       38 2024-04-12 04:03:54.566725 ticketsdk-2.3.0/setup.cfg
--rw-r--r--   0 phamchuong   (501) staff       (20)      851 2024-04-12 04:03:17.000000 ticketsdk-2.3.0/setup.py
-drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-12 04:03:54.563417 ticketsdk-2.3.0/ticketsdk/
--rw-r--r--   0 phamchuong   (501) staff       (20)      516 2024-04-02 03:10:03.000000 ticketsdk-2.3.0/ticketsdk/__init__.py
--rw-r--r--   0 phamchuong   (501) staff       (20)     3995 2024-03-27 09:22:59.000000 ticketsdk-2.3.0/ticketsdk/client.py
--rw-r--r--   0 phamchuong   (501) staff       (20)      354 2024-03-27 10:12:08.000000 ticketsdk-2.3.0/ticketsdk/constants.py
-drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-12 04:03:54.565642 ticketsdk-2.3.0/ticketsdk/seller/
--rw-r--r--   0 phamchuong   (501) staff       (20)     3118 2024-04-09 08:03:12.000000 ticketsdk-2.3.0/ticketsdk/seller/__init__.py
--rw-r--r--   0 phamchuong   (501) staff       (20)     3362 2024-04-12 02:58:57.000000 ticketsdk-2.3.0/ticketsdk/validators.py
-drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-12 04:03:54.566038 ticketsdk-2.3.0/ticketsdk.egg-info/
--rw-r--r--   0 phamchuong   (501) staff       (20)      503 2024-04-12 04:03:54.000000 ticketsdk-2.3.0/ticketsdk.egg-info/PKG-INFO
--rw-r--r--   0 phamchuong   (501) staff       (20)      300 2024-04-12 04:03:54.000000 ticketsdk-2.3.0/ticketsdk.egg-info/SOURCES.txt
--rw-r--r--   0 phamchuong   (501) staff       (20)       33 2024-04-12 04:03:54.000000 ticketsdk-2.3.0/ticketsdk.egg-info/dependency_links.txt
--rw-r--r--   0 phamchuong   (501) staff       (20)       55 2024-04-12 04:03:54.000000 ticketsdk-2.3.0/ticketsdk.egg-info/requires.txt
--rw-r--r--   0 phamchuong   (501) staff       (20)       10 2024-04-12 04:03:54.000000 ticketsdk-2.3.0/ticketsdk.egg-info/top_level.txt
+drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-15 09:25:41.627124 ticketsdk-2.3.1/
+-rw-r--r--   0 phamchuong   (501) staff       (20)      503 2024-04-15 09:25:41.626946 ticketsdk-2.3.1/PKG-INFO
+-rw-r--r--   0 phamchuong   (501) staff       (20)     1717 2024-04-11 09:47:21.000000 ticketsdk-2.3.1/README.md
+-rw-r--r--   0 phamchuong   (501) staff       (20)       38 2024-04-15 09:25:41.627168 ticketsdk-2.3.1/setup.cfg
+-rw-r--r--   0 phamchuong   (501) staff       (20)      851 2024-04-15 09:23:14.000000 ticketsdk-2.3.1/setup.py
+drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-15 09:25:41.625385 ticketsdk-2.3.1/ticketsdk/
+-rw-r--r--   0 phamchuong   (501) staff       (20)      516 2024-04-02 03:10:03.000000 ticketsdk-2.3.1/ticketsdk/__init__.py
+-rw-r--r--   0 phamchuong   (501) staff       (20)     3995 2024-03-27 09:22:59.000000 ticketsdk-2.3.1/ticketsdk/client.py
+-rw-r--r--   0 phamchuong   (501) staff       (20)      354 2024-03-27 10:12:08.000000 ticketsdk-2.3.1/ticketsdk/constants.py
+drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-15 09:25:41.626282 ticketsdk-2.3.1/ticketsdk/seller/
+-rw-r--r--   0 phamchuong   (501) staff       (20)     3118 2024-04-09 08:03:12.000000 ticketsdk-2.3.1/ticketsdk/seller/__init__.py
+-rw-r--r--   0 phamchuong   (501) staff       (20)     3390 2024-04-15 09:22:43.000000 ticketsdk-2.3.1/ticketsdk/validators.py
+drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-15 09:25:41.626767 ticketsdk-2.3.1/ticketsdk.egg-info/
+-rw-r--r--   0 phamchuong   (501) staff       (20)      503 2024-04-15 09:25:41.000000 ticketsdk-2.3.1/ticketsdk.egg-info/PKG-INFO
+-rw-r--r--   0 phamchuong   (501) staff       (20)      300 2024-04-15 09:25:41.000000 ticketsdk-2.3.1/ticketsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 phamchuong   (501) staff       (20)       33 2024-04-15 09:25:41.000000 ticketsdk-2.3.1/ticketsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 phamchuong   (501) staff       (20)       55 2024-04-15 09:25:41.000000 ticketsdk-2.3.1/ticketsdk.egg-info/requires.txt
+-rw-r--r--   0 phamchuong   (501) staff       (20)       10 2024-04-15 09:25:41.000000 ticketsdk-2.3.1/ticketsdk.egg-info/top_level.txt
```

### Comparing `ticketsdk-2.3.0/README.md` & `ticketsdk-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ticketsdk-2.3.0/setup.py` & `ticketsdk-2.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 PKG = "ticketsdk"
-version = "2.3.0"
+version = "2.3.1"
 long_desc = (
     """This SDK is a programatic inteface into the ticket APIs of NandH Logistics."""
 )
 
 setup(
     name=PKG,
     version=version,
```

### Comparing `ticketsdk-2.3.0/ticketsdk/__init__.py` & `ticketsdk-2.3.1/ticketsdk/__init__.py`

 * *Files identical despite different names*

### Comparing `ticketsdk-2.3.0/ticketsdk/client.py` & `ticketsdk-2.3.1/ticketsdk/client.py`

 * *Files identical despite different names*

### Comparing `ticketsdk-2.3.0/ticketsdk/seller/__init__.py` & `ticketsdk-2.3.1/ticketsdk/seller/__init__.py`

 * *Files identical despite different names*

### Comparing `ticketsdk-2.3.0/ticketsdk/validators.py` & `ticketsdk-2.3.1/ticketsdk/validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         raise ValidationError(f"lambda_type not exists")
 
 
 class NewTicketSchema(Schema):
     issue_code = fields.Str(required=True, validate=validate_issue_code)
     from_system = fields.Str(required=True, validate=validate_from_system)
     ref_code = fields.Str(required=True)
-    partner_code = fields.Str(required=True)
+    partner_code = fields.Str(required=False, allow_none=True, allow_empty=True)
     ticket_name = fields.Str(required=True)
     requested_email = fields.Str(required=True)
     ticket_description = fields.Str(required=True)
     attachments = fields.List(fields.Str(), allow_none=False, allow_empty=True)
     lambda_type = fields.Str(required=True)
     requested_by_employee_email = fields.Str(required=False)
     requested_by_employee_name = fields.Str(required=False)
@@ -66,15 +66,15 @@
     page = fields.Int(required=True)
     code = fields.Str(required=False)
     created_at_from = fields.Float(required=False)
     created_at_to = fields.Float(required=False)
     page = fields.Int(required=False)
     status = fields.Str(required=False)
     partner_code = fields.Str(required=False)
-    customer_status = fields.Str(required=False)
+    refcode = fields.Str(required=False)
 
     class Meta:
         strict = True
         unknown = RAISE
 
 
 class DetailTicketSchema(Schema):
```

