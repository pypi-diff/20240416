# Comparing `tmp/pan_ztp_patcher-0.1.2.tar.gz` & `tmp/pan_ztp_patcher-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pan_ztp_patcher-0.1.2.tar", max compression
+gzip compressed data, was "pan_ztp_patcher-0.2.0.tar", max compression
```

## Comparing `pan_ztp_patcher-0.1.2.tar` & `pan_ztp_patcher-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0     3906 2024-04-14 12:44:04.130157 pan_ztp_patcher-0.1.2/README.md
--rw-r--r--   0        0        0     3398 2024-04-15 23:00:01.382962 pan_ztp_patcher-0.1.2/pan_ztp_patcher/app.py
--rw-r--r--   0        0        0    11624 2024-04-14 15:11:26.566687 pan_ztp_patcher-0.1.2/pan_ztp_patcher/ztp_patcher.py
--rw-r--r--   0        0        0      485 2024-04-15 23:00:42.575595 pan_ztp_patcher-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4604 1970-01-01 00:00:00.000000 pan_ztp_patcher-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3906 2024-04-14 12:44:04.130157 pan_ztp_patcher-0.2.0/README.md
+-rw-r--r--   0        0        0     5130 2024-04-16 12:39:11.838310 pan_ztp_patcher-0.2.0/pan_ztp_patcher/app.py
+-rw-r--r--   0        0        0      377 2024-04-16 12:10:48.380233 pan_ztp_patcher-0.2.0/pan_ztp_patcher/constants.py
+-rw-r--r--   0        0        0     1041 2024-04-16 12:06:48.369908 pan_ztp_patcher-0.2.0/pan_ztp_patcher/utils.py
+-rw-r--r--   0        0        0    16606 2024-04-16 12:37:54.918382 pan_ztp_patcher-0.2.0/pan_ztp_patcher/ztp_patcher.py
+-rw-r--r--   0        0        0      510 2024-04-16 12:20:26.625193 pan_ztp_patcher-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4644 1970-01-01 00:00:00.000000 pan_ztp_patcher-0.2.0/PKG-INFO
```

### Comparing `pan_ztp_patcher-0.1.2/README.md` & `pan_ztp_patcher-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pan_ztp_patcher-0.1.2/PKG-INFO` & `pan_ztp_patcher-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pan-ztp-patcher
-Version: 0.1.2
+Version: 0.2.0
 Summary: Update content version on PAN-OS firewalls
 License: Apache2.0
 Author: Calvin Remsburg
 Author-email: cremsburg.dev@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: paramiko (>=3.4.0,<4.0.0)
+Requires-Dist: python-dotenv (==0.21.1)
 Description-Content-Type: text/markdown
 
 # PAN-OS ZTP Patcher
 
 The PAN-OS ZTP Patcher is a utility designed to streamline the process of updating the content version on PAN-OS firewalls during the Zero Touch Provisioning (ZTP) process. It leverages a Raspberry Pi Zero appliance to automate the content update procedure, eliminating the need for manual intervention.
 
 ## Use Case
```

