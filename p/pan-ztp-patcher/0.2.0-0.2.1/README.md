# Comparing `tmp/pan_ztp_patcher-0.2.0.tar.gz` & `tmp/pan_ztp_patcher-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pan_ztp_patcher-0.2.0.tar", max compression
+gzip compressed data, was "pan_ztp_patcher-0.2.1.tar", max compression
```

## Comparing `pan_ztp_patcher-0.2.0.tar` & `pan_ztp_patcher-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     3906 2024-04-14 12:44:04.130157 pan_ztp_patcher-0.2.0/README.md
--rw-r--r--   0        0        0     5130 2024-04-16 12:39:11.838310 pan_ztp_patcher-0.2.0/pan_ztp_patcher/app.py
--rw-r--r--   0        0        0      377 2024-04-16 12:10:48.380233 pan_ztp_patcher-0.2.0/pan_ztp_patcher/constants.py
--rw-r--r--   0        0        0     1041 2024-04-16 12:06:48.369908 pan_ztp_patcher-0.2.0/pan_ztp_patcher/utils.py
--rw-r--r--   0        0        0    16606 2024-04-16 12:37:54.918382 pan_ztp_patcher-0.2.0/pan_ztp_patcher/ztp_patcher.py
--rw-r--r--   0        0        0      510 2024-04-16 12:20:26.625193 pan_ztp_patcher-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4644 1970-01-01 00:00:00.000000 pan_ztp_patcher-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3906 2024-04-14 12:44:04.130157 pan_ztp_patcher-0.2.1/README.md
+-rw-r--r--   0        0        0     4258 2024-04-16 15:57:34.298745 pan_ztp_patcher-0.2.1/pan_ztp_patcher/app.py
+-rw-r--r--   0        0        0     1041 2024-04-16 12:06:48.369908 pan_ztp_patcher-0.2.1/pan_ztp_patcher/utils.py
+-rw-r--r--   0        0        0    17250 2024-04-16 16:00:27.694196 pan_ztp_patcher-0.2.1/pan_ztp_patcher/ztp_patcher.py
+-rw-r--r--   0        0        0      510 2024-04-16 16:25:55.295578 pan_ztp_patcher-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4644 1970-01-01 00:00:00.000000 pan_ztp_patcher-0.2.1/PKG-INFO
```

### Comparing `pan_ztp_patcher-0.2.0/README.md` & `pan_ztp_patcher-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pan_ztp_patcher-0.2.0/pan_ztp_patcher/utils.py` & `pan_ztp_patcher-0.2.1/pan_ztp_patcher/utils.py`

 * *Files identical despite different names*

### Comparing `pan_ztp_patcher-0.2.0/pan_ztp_patcher/ztp_patcher.py` & `pan_ztp_patcher-0.2.1/pan_ztp_patcher/ztp_patcher.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 import logging
 import paramiko
 import sys
 import time
 import urllib.request
 import xml.etree.ElementTree as ET
 
-from pan_ztp_patcher.constants import (
-    MONITOR_JOB_STATUS_TIMEOUT,
-    SCP_IMPORT_TIMEOUT,
-)  # noqa: E501
-
-
 logger = logging.getLogger(__name__)
 
 
 def change_firewall_password(
     pan_hostname,
     pan_username,
     pan_password,
@@ -37,31 +31,35 @@
         paramiko.SSHException: If an SSH exception occurs.
         Exception: If any other error occurs during the password change process. # noqa: E501
 
     Example:
         change_firewall_password("192.168.1.1", "admin", "pan_password_default", "pan_password")
     """
 
+    logger.info("=" * 79)
+    logger.info("Changing firewall password...")
+    logger.info("=" * 79)
+
     # Create an SSH client
     client = paramiko.SSHClient()
     client.set_missing_host_key_policy(paramiko.AutoAddPolicy())
 
     try:
         # Connect to the firewall
-        logging.debug("Connecting to {}...".format(pan_hostname))
+        logger.debug("Connecting to {}...".format(pan_hostname))
         client.connect(
             pan_hostname, username=pan_username, password=pan_password_default
         )
         logger.info("Connected to {} successfully.".format(pan_hostname))
 
         # Create an interactive shell
         shell = client.invoke_shell()
 
         # Wait for the prompt
-        logging.debug("Waiting for the prompt...")
+        logger.debug("Waiting for the prompt...")
         time.sleep(2)
         output = shell.recv(1024).decode("utf-8")
         logger.debug("Received output: {}".format(output))
 
         # Send the old password
         logger.debug(
             "Sending pan_password_default: {}".format(pan_password_default)
@@ -82,15 +80,15 @@
         logger.debug("Confirming pan_password: {}".format(pan_password))
         shell.send(pan_password + "\n")
         time.sleep(2)
         output = shell.recv(1024).decode("utf-8")
         logger.debug("Received output: {}".format(output))
 
         # Close the SSH connection
-        logging.debug("Closing the SSH connection...")
+        logger.debug("Closing the SSH connection...")
         client.close()
         logger.info("Password changed successfully.")
 
     except paramiko.AuthenticationException:
         logger.error("Authentication failed. Please check your credentials.")
     except paramiko.SSHException as ssh_exception:
         logger.error("SSH exception occurred: {}".format(str(ssh_exception)))
@@ -119,41 +117,45 @@
         xml.etree.ElementTree.ParseError: If an error occurs while parsing the XML response. # noqa: E501
         Exception: If any other error occurs during the API request.
 
     Example:
         api_key = retrieve_api_key("192.168.1.1", "admin", "password")
     """
 
+    logger.info("=" * 79)
+    logger.info("Retrieving API key...")
+    logger.info("=" * 79)
+
     try:
         # Construct the API URL
         url = "https://{}/api/?type=keygen&user={}&password={}".format(
             pan_hostname, pan_username, urllib.parse.quote(pan_password)
         )
         logger.debug("API URL: {}".format(url))
 
         # Create an HTTPS request with SSL verification disabled
-        logging.debug("Retrieving API key...")
+        logger.debug("Retrieving API key...")
         request = urllib.request.Request(url)
         response = urllib.request.urlopen(
             request, context=urllib.request.ssl._create_unverified_context()
         )
-        logging.debug("Received response: {}".format(response))
+        logger.debug("Received response: {}".format(response))
 
         # Read the response content
-        logging.debug("Reading response content...")
+        logger.debug("Reading response content...")
         response_content = response.read().decode("utf-8")
         logger.debug("Received response: {}".format(response_content))
 
         # Parse the XML response
-        logging.debug("Parsing XML response...")
+        logger.debug("Parsing XML response...")
         root = ET.fromstring(response_content)
         logger.debug("Root element: {}".format(root.tag))
 
         # Extract the API key from the response
-        logging.debug("Extracting API key...")
+        logger.debug("Extracting API key...")
         api_key_element = root.find("./result/key")
         if api_key_element is not None:
             api_key = api_key_element.text
             logger.debug("Retrieved API key: {}".format(api_key))
             logger.info("Retrieved API key: {}".format(api_key))
             return api_key
         else:
@@ -198,24 +200,30 @@
         paramiko.SSHException: If an SSH exception occurs.
         Exception: If any other error occurs during the SCP import process.
 
     Example:
         import_content_via_scp("192.168.1.1", "admin", "password", "192.168.1.2", "/var/tmp/", "content.txt") # noqa: E501
     """
 
+    logger.info("=" * 79)
+    logger.info("Importing content via SCP...")
+    logger.info("=" * 79)
+
     # Create an SSH client
     client = paramiko.SSHClient()
     client.set_missing_host_key_policy(paramiko.AutoAddPolicy())
 
     try:
         # Connect to the firewall
         logger.debug("Connecting to {}...".format(pan_hostname))
         client.connect(
-            pan_hostname, username=pan_username, password=pan_password
-        )  # noqa: E501
+            pan_hostname,
+            username=pan_username,
+            password=pan_password,
+        )
         logger.info("Connected to {} successfully.".format(pan_hostname))
 
         # Create an interactive shell
         shell = client.invoke_shell()
 
         # Wait for the prompt
         logger.debug("Waiting for the prompt...")
@@ -233,45 +241,50 @@
         logger.debug("Sending SCP command: {}".format(scp_command))
         shell.send(scp_command + "\n")
         time.sleep(2)
         output = shell.recv(1024).decode("utf-8")
         logger.debug("Received output: {}".format(output))
 
         # Check if the host authenticity prompt appears
-        logging.debug("Checking for host authenticity prompt...")
-        if "Are you sure you want to continue connecting" in output:
+        logger.debug("Checking for host authenticity prompt...")
+        if "Please type 'yes', 'no' or the fingerprint" in output:
             logger.debug("Sending 'yes' to the prompt...")
             shell.send("yes\n")
             time.sleep(2)
             output = shell.recv(1024).decode("utf-8")
             logger.debug("Received output: {}".format(output))
 
         # Send the password for pi@
-        logging.debug("Sending password for pi@{}...".format(pi_hostname))
+        logger.debug("Sending password for pi@{}...".format(pi_hostname))
+        time.sleep(2)
         shell.send(pi_password + "\n")
         time.sleep(2)
         output = shell.recv(1024).decode("utf-8")
         logger.debug("Received output: {}".format(output))
 
         # Wait for the completion prompt
         logger.debug("Waiting for the completion prompt...")
         start_time = time.time()
-        while "saved" not in output:
-            if time.time() - start_time > SCP_IMPORT_TIMEOUT:
+        while True:
+            if time.time() - start_time > 120:
                 logger.error(
                     "Timeout occurred while waiting for the completion prompt."
                 )
                 break
             output += shell.recv(1024).decode("utf-8")
             logger.debug("Received output: {}".format(output))
+            if "already exists" in output:
+                logger.info("Content file already exists on the firewall.")
+                break
+            elif "100%" in output and "ETA" not in output:
+                logger.debug("SCP import content completed successfully.")
+                logger.info("SCP import content completed successfully.")
+                break
             time.sleep(1)
 
-        logger.debug("SCP import content completed successfully.")
-        logger.info("SCP import content completed successfully.")
-
         # Close the SSH connection
         client.close()
 
     except paramiko.AuthenticationException:
         logger.error("Authentication failed. Please check your credentials.")
     except paramiko.SSHException as ssh_exception:
         logger.error("SSH exception occurred: {}".format(str(ssh_exception)))
@@ -300,14 +313,18 @@
         xml.etree.ElementTree.ParseError: If an error occurs while parsing the XML response. # noqa: E501
         Exception: If any other error occurs during the API request.
 
     Example:
         job_id = install_content_via_api("192.168.1.1", "api_key", "content.txt")
     """
 
+    logger.info("=" * 79)
+    logger.info("Installing content via API...")
+    logger.info("=" * 79)
+
     try:
         # Construct the API URL
         url = "https://{}/api/?type=op&cmd={}".format(
             pan_hostname,
             urllib.parse.quote_plus(
                 "<request><content><upgrade><install><file>{}</file></install></upgrade></content></request>".format(  # noqa: E501
                     content_file
@@ -317,27 +334,27 @@
         logger.debug("API URL: {}".format(url))
 
         # Create an HTTPS request with SSL verification disabled
         request = urllib.request.Request(url)
         request.add_header("X-PAN-KEY", api_key)
 
         # Send the API request
-        logging.debug("Sending API request...")
+        logger.debug("Sending API request...")
         response = urllib.request.urlopen(
             request, context=urllib.request.ssl._create_unverified_context()
         )
-        logging.debug("Received response: {}".format(response))
+        logger.debug("Received response: {}".format(response))
 
         # Read the response content
-        logging.debug("Reading response content...")
+        logger.debug("Reading response content...")
         response_content = response.read().decode("utf-8")
         logger.debug("Received response: {}".format(response_content))
 
         # Parse the XML response
-        logging.debug("Parsing XML response...")
+        logger.debug("Parsing XML response...")
         root = ET.fromstring(response_content)
         logger.debug("Root element: {}".format(root.tag))
 
         # Check the response status
         status = root.attrib.get("status")
         if status == "success":
             job_element = root.find("./result/job")
@@ -379,14 +396,18 @@
         xml.etree.ElementTree.ParseError: If an error occurs while parsing the XML response. # noqa: E501
         Exception: If any other error occurs during the job monitoring process.
 
     Example:
         monitor_job_status("192.168.1.1", "api_key", "job_id")
     """
 
+    logger.info("=" * 79)
+    logger.info("Monitoring job status...")
+    logger.info("=" * 79)
+
     start_time = time.time()
 
     while True:
         try:
             # Construct the API URL for job monitoring
             url = "https://{}/api/?type=op&cmd={}".format(
                 pan_hostname,
@@ -397,28 +418,28 @@
             logger.debug("Job monitoring URL: {}".format(url))
 
             # Create an HTTPS request with SSL verification disabled
             request = urllib.request.Request(url)
             request.add_header("X-PAN-KEY", api_key)
 
             # Send the API request
-            logging.debug("Sending job monitoring request...")
+            logger.debug("Sending job monitoring request...")
             response = urllib.request.urlopen(
                 request,
                 context=urllib.request.ssl._create_unverified_context(),  # noqa: E501
             )
-            logging.debug("Received response: {}".format(response))
+            logger.debug("Received response: {}".format(response))
 
             # Read the response content
-            logging.debug("Reading response content...")
+            logger.debug("Reading response content...")
             response_content = response.read().decode("utf-8")
             logger.debug("Received response: {}".format(response_content))
 
             # Parse the XML response
-            logging.debug("Parsing XML response...")
+            logger.debug("Parsing XML response...")
             root = ET.fromstring(response_content)
             logger.debug("Root element: {}".format(root.tag))
 
             # Check the job status
             job_status_element = root.find("./result/job/status")
             if job_status_element is not None:
                 job_status = job_status_element.text
@@ -426,25 +447,26 @@
                     job_result_element = root.find("./result/job/result")
                     if job_result_element is not None:
                         job_result = job_result_element.text
                         if job_result == "OK":
                             logger.info("Job completed successfully.")
                             return
                         else:
-                            logger.error("Job completed with an error.")
+                            logger.error("Job completed with an error.")  # noqa: E501
+                            logger.error(job_result)
                             sys.exit(1)
                     else:
                         logger.error("Job result not found in the response.")
                         sys.exit(1)
             else:
                 logger.error("Job status not found in the response.")
                 sys.exit(1)
 
             # Check the timeout
-            if time.time() - start_time > MONITOR_JOB_STATUS_TIMEOUT:
+            if time.time() - start_time > 120:
                 logger.error("Job monitoring timed out.")
                 sys.exit(1)
 
             # Wait for 2 seconds before the next iteration
             time.sleep(2)
 
         except urllib.error.URLError as url_error:
```

### Comparing `pan_ztp_patcher-0.2.0/PKG-INFO` & `pan_ztp_patcher-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pan-ztp-patcher
-Version: 0.2.0
+Version: 0.2.1
 Summary: Update content version on PAN-OS firewalls
 License: Apache2.0
 Author: Calvin Remsburg
 Author-email: cremsburg.dev@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

