# Comparing `tmp/pan_ztp_patcher-0.1.1.tar.gz` & `tmp/pan_ztp_patcher-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pan_ztp_patcher-0.1.1.tar", max compression
+gzip compressed data, was "pan_ztp_patcher-0.1.2.tar", max compression
```

## Comparing `pan_ztp_patcher-0.1.1.tar` & `pan_ztp_patcher-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3906 2024-04-14 12:44:04.130157 pan_ztp_patcher-0.1.1/README.md
--rw-r--r--   0        0        0     3404 2024-04-14 12:39:11.239941 pan_ztp_patcher-0.1.1/pan_ztp_patcher/app.py
--rw-r--r--   0        0        0    11624 2024-04-14 13:07:41.807950 pan_ztp_patcher-0.1.1/pan_ztp_patcher/ztp_patcher.py
--rw-r--r--   0        0        0      485 2024-04-14 13:07:58.486785 pan_ztp_patcher-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4604 1970-01-01 00:00:00.000000 pan_ztp_patcher-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3906 2024-04-14 12:44:04.130157 pan_ztp_patcher-0.1.2/README.md
+-rw-r--r--   0        0        0     3398 2024-04-15 23:00:01.382962 pan_ztp_patcher-0.1.2/pan_ztp_patcher/app.py
+-rw-r--r--   0        0        0    11624 2024-04-14 15:11:26.566687 pan_ztp_patcher-0.1.2/pan_ztp_patcher/ztp_patcher.py
+-rw-r--r--   0        0        0      485 2024-04-15 23:00:42.575595 pan_ztp_patcher-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4604 1970-01-01 00:00:00.000000 pan_ztp_patcher-0.1.2/PKG-INFO
```

### Comparing `pan_ztp_patcher-0.1.1/README.md` & `pan_ztp_patcher-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pan_ztp_patcher-0.1.1/pan_ztp_patcher/app.py` & `pan_ztp_patcher-0.1.2/pan_ztp_patcher/app.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import argparse
 import logging
 from logging.handlers import RotatingFileHandler
 from pan_ztp_patcher.ztp_patcher import (
-    change_password,
     get_api_key,
     scp_import_content,
     send_api_request,
     job_monitor,
 )
 
 
@@ -34,102 +33,97 @@
     logger.addHandler(console_handler)
 
     # Parse command-line arguments
     parser = argparse.ArgumentParser(
         description="Update content version on PAN-OS firewalls",
     )
     parser.add_argument(
-        "-H",
-        "--hostname",
+        "--pi-hostname",
         required=True,
-        help="Firewall hostname or IP address",
+        help="Raspberry Pi hostname or IP address",
     )
     parser.add_argument(
-        "-u",
-        "--username",
+        "--pi-username",
         required=True,
-        help="Firewall username",
+        help="Raspberry Pi username",
     )
     parser.add_argument(
-        "-o",
-        "--old-password",
+        "--pi-password",
         required=True,
-        help="Firewall old password",
+        help="Raspberry Pi password",
     )
     parser.add_argument(
-        "-n",
-        "--new-password",
+        "--pan-hostname",
         required=True,
-        help="Firewall new password",
+        help="PAN-OS firewall hostname or IP address",
     )
     parser.add_argument(
-        "-p",
-        "--pi-hostname",
-        default="192.168.1.2",
-        help="Raspberry Pi hostname or IP address (default: 192.168.1.2)",
+        "--pan-username",
+        required=True,
+        help="PAN-OS firewall username",
     )
     parser.add_argument(
-        "-d",
-        "--pi-content-path",
+        "--pan-password",
+        required=True,
+        help="PAN-OS firewall password",
+    )
+    parser.add_argument(
+        "--content-path",
         default="/var/tmp/",
-        help="Raspberry Pi content path (default: /var/tmp/)",
+        help="Content path on the Raspberry Pi (default: /var/tmp/)",
     )
     parser.add_argument(
-        "-f",
         "--content-file",
         default="panupv2-all-contents-8834-8684",
         help="Content file name (default: panupv2-all-contents-8834-8684)",
     )
     args = parser.parse_args()
 
     # Firewall connection details
-    hostname = args.hostname
-    username = args.username
-    old_password = args.old_password
-    new_password = args.new_password
+    pan_hostname = args.pan_hostname
+    pan_username = args.pan_username
+    pan_password = args.pan_password
 
     # Raspberry Pi connection details
     pi_hostname = args.pi_hostname
-    pi_content_path = args.pi_content_path
+    pi_username = args.pi_username
+    pi_password = args.pi_password
+    content_path = args.content_path
     content_file = args.content_file
 
     # Call the functions
-    change_password(
-        hostname,
-        username,
-        old_password,
-        new_password,
-    )
     api_key = get_api_key(
-        hostname,
-        username,
-        new_password,
+        pan_hostname,
+        pan_username,
+        pan_password,
     )
     if api_key:
         logger.info("API Key: {}".format(api_key))
     else:
         logger.error("Failed to retrieve the API key.")
         return
 
     scp_import_content(
-        hostname,
-        username,
-        new_password,
+        pan_hostname,
+        pan_username,
+        pan_password,
         pi_hostname,
-        pi_content_path,
+        pi_username,
+        pi_password,
+        content_path,
         content_file,
     )
     job_id = send_api_request(
-        hostname,
+        pan_hostname,
         api_key,
         content_file,
     )
     if job_id:
         job_monitor(
-            hostname,
+            pan_hostname,
             api_key,
             job_id,
         )
     else:
         logger.error("Failed to retrieve the job ID.")
```

### Comparing `pan_ztp_patcher-0.1.1/pan_ztp_patcher/ztp_patcher.py` & `pan_ztp_patcher-0.1.2/pan_ztp_patcher/ztp_patcher.py`

 * *Files identical despite different names*

### Comparing `pan_ztp_patcher-0.1.1/PKG-INFO` & `pan_ztp_patcher-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pan-ztp-patcher
-Version: 0.1.1
+Version: 0.1.2
 Summary: Update content version on PAN-OS firewalls
 License: Apache2.0
 Author: Calvin Remsburg
 Author-email: cremsburg.dev@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

