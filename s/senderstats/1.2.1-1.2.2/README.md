# Comparing `tmp/senderstats-1.2.1.tar.gz` & `tmp/senderstats-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "senderstats-1.2.1.tar", last modified: Fri Mar 29 20:53:46 2024, max compression
+gzip compressed data, was "senderstats-1.2.2.tar", last modified: Tue Apr 16 19:07:49 2024, max compression
```

## Comparing `senderstats-1.2.1.tar` & `senderstats-1.2.2.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:53:46.432299 senderstats-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-29 20:53:41.000000 senderstats-1.2.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:53:46.428299 senderstats-1.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:53:46.428299 senderstats-1.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-03-29 20:53:41.000000 senderstats-1.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-03-29 20:53:41.000000 senderstats-1.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     7813 2024-03-29 20:53:46.432299 senderstats-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7489 2024-03-29 20:53:41.000000 senderstats-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-29 20:53:41.000000 senderstats-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 20:53:46.432299 senderstats-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:53:46.428299 senderstats-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:53:46.428299 senderstats-1.2.1/src/senderstats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 20:53:41.000000 senderstats-1.2.1/src/senderstats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10387 2024-03-29 20:53:41.000000 senderstats-1.2.1/src/senderstats/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:53:46.432299 senderstats-1.2.1/src/senderstats/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 20:53:41.000000 senderstats-1.2.1/src/senderstats/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-03-29 20:53:41.000000 senderstats-1.2.1/src/senderstats/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6760 2024-03-29 20:53:41.000000 senderstats-1.2.1/src/senderstats/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-03-29 20:53:41.000000 senderstats-1.2.1/src/senderstats/common/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-03-29 20:53:41.000000 senderstats-1.2.1/src/senderstats/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:53:46.432299 senderstats-1.2.1/src/senderstats/lib/
--rw-r--r--   0 runner    (1001) docker     (127)    14405 2024-03-29 20:53:41.000000 senderstats-1.2.1/src/senderstats/lib/MessageDataProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)    11388 2024-03-29 20:53:41.000000 senderstats-1.2.1/src/senderstats/lib/MessageDataReport.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 20:53:41.000000 senderstats-1.2.1/src/senderstats/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:53:46.432299 senderstats-1.2.1/src/senderstats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7813 2024-03-29 20:53:46.000000 senderstats-1.2.1/src/senderstats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-03-29 20:53:46.000000 senderstats-1.2.1/src/senderstats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 20:53:46.000000 senderstats-1.2.1/src/senderstats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-29 20:53:46.000000 senderstats-1.2.1/src/senderstats.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-29 20:53:46.000000 senderstats-1.2.1/src/senderstats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-29 20:53:46.000000 senderstats-1.2.1/src/senderstats.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:07:49.400999 senderstats-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-16 19:07:43.000000 senderstats-1.2.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:07:49.393000 senderstats-1.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:07:49.396999 senderstats-1.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-16 19:07:43.000000 senderstats-1.2.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-16 19:07:43.000000 senderstats-1.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     8213 2024-04-16 19:07:49.396999 senderstats-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7889 2024-04-16 19:07:43.000000 senderstats-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-16 19:07:43.000000 senderstats-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 19:07:49.400999 senderstats-1.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:07:49.393000 senderstats-1.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:07:49.396999 senderstats-1.2.2/src/senderstats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 19:07:43.000000 senderstats-1.2.2/src/senderstats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11065 2024-04-16 19:07:43.000000 senderstats-1.2.2/src/senderstats/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:07:49.396999 senderstats-1.2.2/src/senderstats/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 19:07:43.000000 senderstats-1.2.2/src/senderstats/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-16 19:07:43.000000 senderstats-1.2.2/src/senderstats/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6760 2024-04-16 19:07:43.000000 senderstats-1.2.2/src/senderstats/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-16 19:07:43.000000 senderstats-1.2.2/src/senderstats/common/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:07:49.396999 senderstats-1.2.2/src/senderstats/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)    16594 2024-04-16 19:07:43.000000 senderstats-1.2.2/src/senderstats/lib/MessageDataProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12438 2024-04-16 19:07:43.000000 senderstats-1.2.2/src/senderstats/lib/MessageDataReport.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 19:07:43.000000 senderstats-1.2.2/src/senderstats/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:07:49.396999 senderstats-1.2.2/src/senderstats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8213 2024-04-16 19:07:49.000000 senderstats-1.2.2/src/senderstats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-16 19:07:49.000000 senderstats-1.2.2/src/senderstats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:07:49.000000 senderstats-1.2.2/src/senderstats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-16 19:07:49.000000 senderstats-1.2.2/src/senderstats.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 19:07:49.000000 senderstats-1.2.2/src/senderstats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 19:07:49.000000 senderstats-1.2.2/src/senderstats.egg-info/top_level.txt
```

### Comparing `senderstats-1.2.1/.github/workflows/python-publish.yml` & `senderstats-1.2.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `senderstats-1.2.1/.gitignore` & `senderstats-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `senderstats-1.2.1/PKG-INFO` & `senderstats-1.2.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: senderstats
-Version: 1.2.1
+Version: 1.2.2
 Summary: Tool to Process Smart Search Results and Identify Top Senders
 License: MIT
 Project-URL: repository, https://github.com/pfptcommunity/senderstats
 Requires-Python: >3.9
 Description-Content-Type: text/markdown
 Requires-Dist: xlsxwriter
 Requires-Dist: tldextract
@@ -26,49 +26,58 @@
 ```
 
 or can install the tool using pip.
 
 ```
 pip install senderstats
 ```
+
 ### Use Cases:
+
 **Outbound message volumes and data transferred by:**
-  * Envelope sender
-  * Header From:
-  * Return-Path:
-  * Envelope header: From:, MessageID Host, MessageID Domain (helpful to identify original sender)
-  * Envelope sender and header From: for SPF alignment purposes
+
+* Envelope sender
+* Header From:
+* Return-Path:
+* Envelope header: From:, MessageID Host, MessageID Domain (helpful to identify original sender)
+* Envelope sender and header From: for SPF alignment purposes
+* Random subject line sampling to help understand the type of traffic
 
 **Summarize message volume information:**
-  * Estimated application email traffic based on sender volume threshold:
-    * Estimated application data 
-    * Estimated application messages 
-    * Estimated application average size 
+
+* Estimated application email traffic based on sender volume threshold:
+    * Estimated application data
+    * Estimated application messages
+    * Estimated application average size
     * Estimated application peak hourly volume
-  * Total outbound data
-    * Total outbound data 
-    * Total outbound messages 
+* Total outbound data
+    * Total outbound data
+    * Total outbound messages
     * Total outbound average size
     * Total outbound peak hourly volume
 
 ### Usage Options:
+
 ```
-usage: senderstats [-h] -i <file> [<file> ...] -o <xlsx> [--mfrom MFrom] [--hfrom HFrom] [--rpath RPath] [--msgid MsgID] [--size MsgSz] [--date Date] [--gen-hfrom] [--gen-rpath] [--gen-alignment] [--gen-msgid] [-t THRESHOLD] [--no-display-name] [--remove-prvs] [--decode-srs] [--no-empty-hfrom] [--excluded-domains <domain> [<domain> ...]] [--restrict-domains <domain> [<domain> ...]] [--excluded-senders <sender> [<sender> ...]] [--date-format DateFmt] [--show-skip-detail]
+usage: senderstats [-h] -i <file> [<file> ...] -o <xlsx> [--mfrom MFrom] [--hfrom HFrom] [--rpath RPath] [--msgid MsgID] [--subject Subject] [--size MsgSz] [--date Date] [--gen-hfrom] [--gen-rpath] [--gen-alignment] [--gen-msgid]
+                   [-t N] [--no-display-name] [--remove-prvs] [--decode-srs] [--no-empty-hfrom] [--sample-subject] [--excluded-domains <domain> [<domain> ...]] [--restrict-domains <domain> [<domain> ...]]
+                   [--excluded-senders <sender> [<sender> ...]] [--date-format DateFmt] [--show-skip-detail]
 
 This tool helps identify the top senders based on smart search outbound message exports.
 
 Required arguments (optional):
   -i <file> [<file> ...], --input <file> [<file> ...]  Smart search files to read.
   -o <xlsx>, --output <xlsx>                           Output file
 
 Field mapping arguments (optional):
   --mfrom MFrom                                        CSV field of the envelope sender address. (default=Sender)
   --hfrom HFrom                                        CSV field of the header From: address. (default=Header_From)
   --rpath RPath                                        CSV field of the Return-Path: address. (default=Header_Return-Path)
   --msgid MsgID                                        CSV field of the message ID. (default=Message_ID)
+  --subject Subject                                    CSV field of the Subject, only used if --sample-subject is specified. (default=Subject)
   --size MsgSz                                         CSV field of message size. (default=Message_Size)
   --date Date                                          CSV field of message date/time. (default=Date)
 
 Reporting control arguments (optional):
   --gen-hfrom                                          Generate report showing the header From: data for messages being sent.
   --gen-rpath                                          Generate report showing return path for messages being sent.
   --gen-alignment                                      Generate report showing envelope sender and header From: alignment
@@ -76,41 +85,44 @@
   -t N, --threshold N                                  Adjust summary report threshold for messages per day to be considered application traffic. (default=100)
 
 Parsing behavior arguments (optional):
   --no-display-name                                    Remove display and use address only. Converts 'Display Name <user@domain.com>' to 'user@domain.com'
   --remove-prvs                                        Remove return path verification strings e.g. prvs=tag=sender@domain.com
   --decode-srs                                         Convert sender rewrite scheme, forwardmailbox+srs=hash=tt=domain.com=user to user@domain.com
   --no-empty-hfrom                                     If the header From: is empty the envelope sender address is used
+  --sample-subject                                     Enable probabilistic random sampling of subject lines found during processing
   --excluded-domains <domain> [<domain> ...]           Exclude domains from processing.
   --restrict-domains <domain> [<domain> ...]           Constrain domains for processing.
   --excluded-senders <sender> [<sender> ...]           Exclude senders from processing.
   --date-format DateFmt                                Date format used to parse the timestamps. (default=%Y-%m-%dT%H:%M:%S.%f%z)
 
 Extended processing controls (optional):
   --show-skip-detail                                   Show skipped details
 
 Usage:
   -h, --help                                           Show this help message and exit
 ```
 
 ### Using the Tool with Proofpoint Smart Search
 
-Export all outbound message traffic as a smart search CSV. You may need to export multiple CSVs if the data per time window exceeds 1M records. The tool can ingest multiple CSVs files at once.
+Export all outbound message traffic as a smart search CSV. You may need to export multiple CSVs if the data per time
+window exceeds 1M records. The tool can ingest multiple CSVs files at once.
 
 ![smart_search_outbound](https://github.com/pfptcommunity/senderstats/assets/83429267/83693152-922e-489a-b06d-a0765ecaf3e8)
 
-Once the files are downlaoded to a target folder, you can run the following command with the path to the files you downloaded and specify a wildard.
+Once the files are downlaoded to a target folder, you can run the following command with the path to the files you
+downloaded and specify a wildard.
 
 ```
 senderstats -i C:\path\to\downloaded\files\smart_search_results_custer_hosted_2024_03_04_*.csv -o C:\path\to\output\file\my_cluster_hosted.xlsx
 ```
 
 ### Sample Output
 
-The execution results should look similar to the following depending the options you select. 
+The execution results should look similar to the following depending the options you select.
 
 ```
 Files to be processed:
 C:\Users\ljerabek\Downloads\smart_search_results_cluster_hosted_2024_03_04_173552.csv
 C:\Users\ljerabek\Downloads\smart_search_results_cluster_hosted_2024_03_04_173855.csv
 C:\Users\ljerabek\Downloads\smart_search_results_cluster_hosted_2024_03_04_173656.csv
 C:\Users\ljerabek\Downloads\smart_search_results_cluster_hosted_2024_03_04_173754.csv
```

### Comparing `senderstats-1.2.1/README.md` & `senderstats-1.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -15,49 +15,58 @@
 ```
 
 or can install the tool using pip.
 
 ```
 pip install senderstats
 ```
+
 ### Use Cases:
+
 **Outbound message volumes and data transferred by:**
-  * Envelope sender
-  * Header From:
-  * Return-Path:
-  * Envelope header: From:, MessageID Host, MessageID Domain (helpful to identify original sender)
-  * Envelope sender and header From: for SPF alignment purposes
+
+* Envelope sender
+* Header From:
+* Return-Path:
+* Envelope header: From:, MessageID Host, MessageID Domain (helpful to identify original sender)
+* Envelope sender and header From: for SPF alignment purposes
+* Random subject line sampling to help understand the type of traffic
 
 **Summarize message volume information:**
-  * Estimated application email traffic based on sender volume threshold:
-    * Estimated application data 
-    * Estimated application messages 
-    * Estimated application average size 
+
+* Estimated application email traffic based on sender volume threshold:
+    * Estimated application data
+    * Estimated application messages
+    * Estimated application average size
     * Estimated application peak hourly volume
-  * Total outbound data
-    * Total outbound data 
-    * Total outbound messages 
+* Total outbound data
+    * Total outbound data
+    * Total outbound messages
     * Total outbound average size
     * Total outbound peak hourly volume
 
 ### Usage Options:
+
 ```
-usage: senderstats [-h] -i <file> [<file> ...] -o <xlsx> [--mfrom MFrom] [--hfrom HFrom] [--rpath RPath] [--msgid MsgID] [--size MsgSz] [--date Date] [--gen-hfrom] [--gen-rpath] [--gen-alignment] [--gen-msgid] [-t THRESHOLD] [--no-display-name] [--remove-prvs] [--decode-srs] [--no-empty-hfrom] [--excluded-domains <domain> [<domain> ...]] [--restrict-domains <domain> [<domain> ...]] [--excluded-senders <sender> [<sender> ...]] [--date-format DateFmt] [--show-skip-detail]
+usage: senderstats [-h] -i <file> [<file> ...] -o <xlsx> [--mfrom MFrom] [--hfrom HFrom] [--rpath RPath] [--msgid MsgID] [--subject Subject] [--size MsgSz] [--date Date] [--gen-hfrom] [--gen-rpath] [--gen-alignment] [--gen-msgid]
+                   [-t N] [--no-display-name] [--remove-prvs] [--decode-srs] [--no-empty-hfrom] [--sample-subject] [--excluded-domains <domain> [<domain> ...]] [--restrict-domains <domain> [<domain> ...]]
+                   [--excluded-senders <sender> [<sender> ...]] [--date-format DateFmt] [--show-skip-detail]
 
 This tool helps identify the top senders based on smart search outbound message exports.
 
 Required arguments (optional):
   -i <file> [<file> ...], --input <file> [<file> ...]  Smart search files to read.
   -o <xlsx>, --output <xlsx>                           Output file
 
 Field mapping arguments (optional):
   --mfrom MFrom                                        CSV field of the envelope sender address. (default=Sender)
   --hfrom HFrom                                        CSV field of the header From: address. (default=Header_From)
   --rpath RPath                                        CSV field of the Return-Path: address. (default=Header_Return-Path)
   --msgid MsgID                                        CSV field of the message ID. (default=Message_ID)
+  --subject Subject                                    CSV field of the Subject, only used if --sample-subject is specified. (default=Subject)
   --size MsgSz                                         CSV field of message size. (default=Message_Size)
   --date Date                                          CSV field of message date/time. (default=Date)
 
 Reporting control arguments (optional):
   --gen-hfrom                                          Generate report showing the header From: data for messages being sent.
   --gen-rpath                                          Generate report showing return path for messages being sent.
   --gen-alignment                                      Generate report showing envelope sender and header From: alignment
@@ -65,41 +74,44 @@
   -t N, --threshold N                                  Adjust summary report threshold for messages per day to be considered application traffic. (default=100)
 
 Parsing behavior arguments (optional):
   --no-display-name                                    Remove display and use address only. Converts 'Display Name <user@domain.com>' to 'user@domain.com'
   --remove-prvs                                        Remove return path verification strings e.g. prvs=tag=sender@domain.com
   --decode-srs                                         Convert sender rewrite scheme, forwardmailbox+srs=hash=tt=domain.com=user to user@domain.com
   --no-empty-hfrom                                     If the header From: is empty the envelope sender address is used
+  --sample-subject                                     Enable probabilistic random sampling of subject lines found during processing
   --excluded-domains <domain> [<domain> ...]           Exclude domains from processing.
   --restrict-domains <domain> [<domain> ...]           Constrain domains for processing.
   --excluded-senders <sender> [<sender> ...]           Exclude senders from processing.
   --date-format DateFmt                                Date format used to parse the timestamps. (default=%Y-%m-%dT%H:%M:%S.%f%z)
 
 Extended processing controls (optional):
   --show-skip-detail                                   Show skipped details
 
 Usage:
   -h, --help                                           Show this help message and exit
 ```
 
 ### Using the Tool with Proofpoint Smart Search
 
-Export all outbound message traffic as a smart search CSV. You may need to export multiple CSVs if the data per time window exceeds 1M records. The tool can ingest multiple CSVs files at once.
+Export all outbound message traffic as a smart search CSV. You may need to export multiple CSVs if the data per time
+window exceeds 1M records. The tool can ingest multiple CSVs files at once.
 
 ![smart_search_outbound](https://github.com/pfptcommunity/senderstats/assets/83429267/83693152-922e-489a-b06d-a0765ecaf3e8)
 
-Once the files are downlaoded to a target folder, you can run the following command with the path to the files you downloaded and specify a wildard.
+Once the files are downlaoded to a target folder, you can run the following command with the path to the files you
+downloaded and specify a wildard.
 
 ```
 senderstats -i C:\path\to\downloaded\files\smart_search_results_custer_hosted_2024_03_04_*.csv -o C:\path\to\output\file\my_cluster_hosted.xlsx
 ```
 
 ### Sample Output
 
-The execution results should look similar to the following depending the options you select. 
+The execution results should look similar to the following depending the options you select.
 
 ```
 Files to be processed:
 C:\Users\ljerabek\Downloads\smart_search_results_cluster_hosted_2024_03_04_173552.csv
 C:\Users\ljerabek\Downloads\smart_search_results_cluster_hosted_2024_03_04_173855.csv
 C:\Users\ljerabek\Downloads\smart_search_results_cluster_hosted_2024_03_04_173656.csv
 C:\Users\ljerabek\Downloads\smart_search_results_cluster_hosted_2024_03_04_173754.csv
```

### Comparing `senderstats-1.2.1/pyproject.toml` & `senderstats-1.2.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tools.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "senderstats"
-version = "1.2.1"
+version = "1.2.2"
 readme = "README.md"
 description = "Tool to Process Smart Search Results and Identify Top Senders"
 license = { text = "MIT" }
 requires-python = ">3.9"
 dependencies = [
     'xlsxwriter',
     'tldextract'
```

### Comparing `senderstats-1.2.1/src/senderstats/cli.py` & `senderstats-1.2.2/src/senderstats/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import sys
 from glob import glob
+
 from senderstats.common.constants import DEFAULT_THRESHOLD, DEFAULT_DOMAIN_EXCLUSIONS
 from senderstats.common.utils import *
 from senderstats.common.validators import *
 from senderstats.lib.MessageDataProcessor import *
 from senderstats.lib.MessageDataReport import MessageDataReport
 
 
@@ -43,14 +44,18 @@
                              type=str, required=False,
                              help=f'CSV field of the Return-Path: address. (default={DEFAULT_RPATH_FIELD})')
 
     field_group.add_argument('--msgid', metavar='MsgID', dest="msgid_field",
                              type=str, required=False,
                              help=f'CSV field of the message ID. (default={DEFAULT_MSGID_FIELD})')
 
+    field_group.add_argument('--subject', metavar='Subject', dest="subject_field",
+                             type=str, required=False,
+                             help=f'CSV field of the Subject, only used if --sample-subject is specified. (default={DEFAULT_SUBJECT_FIELD})')
+
     field_group.add_argument('--size', metavar='MsgSz', dest="msgsz_field",
                              type=str, required=False,
                              help=f'CSV field of message size. (default={DEFAULT_MSGSZ_FIELD})')
 
     field_group.add_argument('--date', metavar='Date', dest="date_field",
                              type=str, required=False,
                              help=f'CSV field of message date/time. (default={DEFAULT_DATE_FIELD})')
@@ -79,14 +84,17 @@
 
     parser_group.add_argument('--decode-srs', action='store_true', dest="decode_srs",
                               help='Convert sender rewrite scheme, forwardmailbox+srs=hash=tt=domain.com=user to user@domain.com')
 
     parser_group.add_argument('--no-empty-hfrom', action='store_true', dest="no_empty_hfrom",
                               help='If the header From: is empty the envelope sender address is used')
 
+    parser_group.add_argument('--sample-subject', action='store_true', dest="sample_subject",
+                              help='Enable probabilistic random sampling of subject lines found during processing')
+
     parser_group.add_argument('--excluded-domains', default=[], metavar='<domain>', dest="excluded_domains",
                               nargs='+', type=is_valid_domain_syntax, help='Exclude domains from processing.')
 
     parser_group.add_argument('--restrict-domains', default=[], metavar='<domain>', dest="restricted_domains",
                               nargs='+', type=is_valid_domain_syntax, help='Constrain domains for processing.')
 
     parser_group.add_argument('--excluded-senders', default=[], metavar='<sender>', dest="excluded_senders",
@@ -150,14 +158,17 @@
 
     if args.msgid_field:
         data_processor.set_msgid_field(args.msgid_field)
 
     if args.msgsz_field:
         data_processor.set_msgsz_field(args.msgsz_field)
 
+    if args.subject_field:
+        data_processor.set_subject_field(args.subject_field)
+
     if args.date_field:
         data_processor.set_date_field(args.date_field)
 
     if args.date_format:
         data_processor.set_date_format = args.date_format
 
     # Set processing flags
@@ -166,14 +177,17 @@
 
     if args.decode_srs:
         data_processor.set_opt_decode_srs(args.decode_srs)
 
     if args.no_empty_hfrom:
         data_processor.set_opt_empty_from(args.no_empty_hfrom)
 
+    if args.sample_subject:
+        data_processor.set_opt_sample_subject(args.sample_subject)
+
     if args.no_display:
         data_processor.set_opt_no_display(args.no_display)
 
     if args.gen_hfrom:
         data_processor.set_opt_gen_hfrom(args.gen_hfrom)
 
     if args.gen_rpath:
```

### Comparing `senderstats-1.2.1/src/senderstats/common/constants.py` & `senderstats-1.2.2/src/senderstats/common/constants.py`

 * *Files identical despite different names*

### Comparing `senderstats-1.2.1/src/senderstats/common/utils.py` & `senderstats-1.2.2/src/senderstats/common/utils.py`

 * *Files identical despite different names*

### Comparing `senderstats-1.2.1/src/senderstats/common/validators.py` & `senderstats-1.2.2/src/senderstats/common/validators.py`

 * *Files identical despite different names*

### Comparing `senderstats-1.2.1/src/senderstats/lib/MessageDataProcessor.py` & `senderstats-1.2.2/src/senderstats/lib/MessageDataProcessor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,60 @@
 import csv
 import datetime
 import re
 from collections import defaultdict
+from random import random
 from typing import DefaultDict, Any, Dict, Set, List, Optional
 
 from tldextract import tldextract
 
 from senderstats.common.utils import (convert_srs, remove_prvs, compile_domains_pattern, find_ip_in_text,
                                       parse_email_details)
 
 # Constants for the class
 DEFAULT_MFROM_FIELD = 'Sender'
 DEFAULT_HFROM_FIELD = 'Header_From'
 DEFAULT_RPATH_FIELD = 'Header_Return-Path'
 DEFAULT_MSGID_FIELD = 'Message_ID'
 DEFAULT_MSGSZ_FIELD = 'Message_Size'
+DEFAULT_SUBJECT_FIELD = 'Subject'
 DEFAULT_DATE_FIELD = 'Date'
 DEFAULT_DATE_FORMAT = '%Y-%m-%dT%H:%M:%S.%f%z'
 
 
 class MessageDataProcessor:
     # Data processing information
-    __mfrom_data: Dict[str, List[Any]]
-    __hfrom_data: Dict[str, List[Any]]
-    __rpath_data: Dict[str, List[Any]]
-    __mfrom_hfrom_data: Dict[tuple, List[Any]]
-    __msgid_data: Dict[tuple, List[Any]]
+    __mfrom_data: Dict[str, Dict]
+    __hfrom_data: Dict[str, Dict]
+    __rpath_data: Dict[str, Dict]
+    __mfrom_hfrom_data: Dict[tuple, Dict]
+    __msgid_data: Dict[tuple, Dict]
+    __subject_data: Dict[Any, Dict]
     # Counters
     __date_counter: DefaultDict[str, int]
     __total_processed_count: int
     __empty_sender_count: int
     __excluded_sender_count: DefaultDict[str, int]
     __excluded_domain_count: DefaultDict[str, int]
     __restricted_domains_count: DefaultDict[str, int]
     # Define CSV Fields
     __mfrom_field: str
     __hfrom_field: str
     __rpath_field: str
     __msgid_field: str
     __msgsz_field: str
+    __subject_field: str
     __date_field: str
     __date_format: str
     # Processing Option Flags
     __opt_no_display: bool
     __opt_decode_srs: bool
     __opt_remove_prvs: bool
     __opt_empty_from: bool
+    __opt_sample_subject: bool
     # Report generation options
     __opt_gen_hfrom: bool
     __opt_gen_alignment: bool
     __opt_gen_rpath: bool
     __opt_gen_msgid: bool
     # Restrictions
     __excluded_senders: Set[str]
@@ -59,28 +64,30 @@
     def __init__(self, excluded_senders: List[str], excluded_domains: List[str], restricted_domains: List[str]):
         # Default field mappings based on smart search output
         self.__mfrom_field = DEFAULT_MFROM_FIELD
         self.__hfrom_field = DEFAULT_HFROM_FIELD
         self.__rpath_field = DEFAULT_RPATH_FIELD
         self.__msgid_field = DEFAULT_MSGID_FIELD
         self.__msgsz_field = DEFAULT_MSGSZ_FIELD
+        self.__subject_field = DEFAULT_SUBJECT_FIELD
         self.__date_field = DEFAULT_DATE_FIELD
         self.__date_format = DEFAULT_DATE_FORMAT
         # Initialize counters
         self.__date_counter = defaultdict(int)
         self.__total_processed_count = 0
         self.__empty_sender_count = 0
         self.__excluded_sender_count = defaultdict(int)
         self.__excluded_domain_count = defaultdict(int)
         self.__restricted_domains_count = defaultdict(int)
         # Initialize processing flags
         self.__opt_no_display = False
         self.__opt_decode_srs = False
         self.__opt_remove_prvs = False
         self.__opt_empty_from = False
+        self.__opt_sample_subject = False
         # Reports we want to generate
         self.__opt_gen_hfrom = False
         self.__opt_gen_alignment = False
         self.__opt_gen_rpath = False
         self.__opt_gen_msgid = False
         # Used to match the patterns
         self.__excluded_senders = set(excluded_senders)
@@ -149,20 +156,21 @@
             rpath = remove_prvs(rpath)
 
         if self.__opt_decode_srs:
             rpath = convert_srs(rpath)
 
         return rpath
 
-    def __process_alignment_data(self, hfrom: str, mfrom: str, message_size: int):
+    def __process_alignment_data(self, hfrom: str, mfrom: str, message_size: int, subject: Optional):
         # Fat index for binding commonality
         sender_header_index = (mfrom, hfrom)
-        self.__mfrom_hfrom_data.setdefault(sender_header_index, []).append(message_size)
+        self.__mfrom_hfrom_data.setdefault(sender_header_index, {})
+        self.__update_message_size_and_subjects(self.__mfrom_hfrom_data[sender_header_index], message_size, subject)
 
-    def __process_msgid_data(self, msgid: str, mfrom: str, message_size: int) -> str:
+    def __process_msgid_data(self, msgid: str, mfrom: str, message_size: int, subject: str) -> str:
         # Message ID is unique but often the sending host behind the @ symbol is unique to the application
         msgid_parts = parse_email_details(msgid)
         msgid_domain = ''
         msgid_host = ''
 
         if msgid_parts['email_address'] or '@' in msgid:
             # Use the extracted domain if available; otherwise, split the msgid
@@ -178,21 +186,41 @@
                 # Adjust msgid_host and msgid_domain based on the presence of subdomain
                 if not msgid_host and not extracted.suffix:
                     msgid_host = msgid_domain
                     msgid_domain = ''
 
         # Fat index for binding commonality
         mid_host_domain_index = (mfrom, msgid_host, msgid_domain)
-
-        self.__msgid_data.setdefault(mid_host_domain_index, []).append(message_size)
+        self.__msgid_data.setdefault(mid_host_domain_index, {})
+        self.__update_message_size_and_subjects(self.__msgid_data[mid_host_domain_index], message_size, subject)
 
         return msgid
 
+    def __update_message_size_and_subjects(self, data: Dict, message_size: int, subject: str):
+        # Ensure the message_size list exists and append the new message size
+        data.setdefault("message_size", []).append(message_size)
+
+        if not self.__opt_sample_subject:
+            return
+
+        data.setdefault("subjects", [])
+
+        # Avoid storing empty subject lines
+        if not subject:
+            return
+
+        # Calculate probability based on the number of processed records
+        probability = 1 / len(data['message_size'])
+
+        # Ensure at least one subject is added if subjects array is empty
+        if not data['subjects'] or random() < probability:
+            data['subjects'].append(subject)
+
     def process_file(self, input_file):
-        with open(input_file, 'r', encoding='utf-8-sig') as input_file:
+        with (open(input_file, 'r', encoding='utf-8-sig') as input_file):
             reader = csv.DictReader(input_file)
             for csv_line in reader:
                 self.__total_processed_count += 1
 
                 # Make sure cast to int is valid, else 0 (size is required)
                 message_size = csv_line[self.__msgsz_field]
                 if message_size.isdigit():
@@ -202,40 +230,47 @@
 
                 mfrom = self.__process_mfrom_data(csv_line[self.__mfrom_field].casefold().strip())
 
                 # mfrom will be None, unless the filtering criteria applied properly
                 if not mfrom:
                     continue
 
+                subject = ''
+                if self.__opt_sample_subject:
+                    subject = csv_line[self.__subject_field].strip()
+
                 # Track the cleaned, filtered mfrom data for our report
-                self.__mfrom_data.setdefault(mfrom, []).append(message_size)
+                self.__mfrom_data.setdefault(mfrom, {})
+                self.__update_message_size_and_subjects(self.__mfrom_data[mfrom], message_size, subject)
 
                 # Alignment will require that we have hfrom
                 if self.__opt_gen_hfrom or self.__opt_gen_alignment:
                     hfrom = self.__process_hfrom_data(csv_line[self.__hfrom_field].casefold().strip(), mfrom)
 
                     # Generate data for HFrom
                     if self.__opt_gen_hfrom:
-                        self.__hfrom_data.setdefault(hfrom, []).append(message_size)
+                        self.__hfrom_data.setdefault(hfrom, {})
+                        self.__update_message_size_and_subjects(self.__hfrom_data[hfrom], message_size, subject)
 
                     # Generate data for HFrom and MFrom Alignment
                     if self.__opt_gen_alignment:
-                        self.__process_alignment_data(hfrom, mfrom, message_size)
+                        self.__process_alignment_data(hfrom, mfrom, message_size, subject)
 
                 # Generate data for return path
                 if self.__opt_gen_rpath:
                     rpath = self.__process_rpath_data(csv_line[self.__rpath_field].casefold().strip())
                     if self.__opt_gen_rpath:
-                        self.__rpath_data.setdefault(rpath, []).append(message_size)
+                        self.__rpath_data.setdefault(rpath, {})
+                        self.__update_message_size_and_subjects(self.__rpath_data[rpath], message_size, subject)
 
                 # Generate data for parsed message ID
                 if self.__opt_gen_msgid:
                     # Generate data for Message ID information
                     self.__process_msgid_data(csv_line[self.__msgid_field].casefold().strip('<>[] '), mfrom,
-                                              message_size)
+                                              message_size, subject)
 
                 # Determine distinct dates of data, and count number of messages on that day
                 date = datetime.datetime.strptime(csv_line[self.__date_field], self.__date_format)
                 str_date = date.strftime('%Y-%m-%d')
                 self.__date_counter[str_date] += 1
 
     # Getter for total_processed_count
@@ -334,14 +369,25 @@
     # Setter for opt_gen_msgid
     def set_opt_gen_msgid(self, value):
         if isinstance(value, bool):
             self.__opt_gen_msgid = value
         else:
             raise ValueError("opt_gen_msgid must be a boolean")
 
+    # Setter for opt_sample_subject
+    def set_opt_sample_subject(self, value):
+        if isinstance(value, bool):
+            self.__opt_sample_subject = value
+        else:
+            raise ValueError("opt_sample_subject must be a boolean")
+
+    # Getter for opt_sample_subject
+    def get_opt_sample_subject(self) -> bool:
+        return self.__opt_sample_subject
+
     # Setter for mfrom_field
     def set_mfrom_field(self, value: str) -> None:
         if isinstance(value, str):
             self.__mfrom_field = value
         else:
             raise ValueError("mfrom_field must be a string.")
 
@@ -369,14 +415,20 @@
     # Setter for msgsz_field
     def set_msgsz_field(self, value: str) -> None:
         if isinstance(value, str):
             self.__msgsz_field = value
         else:
             raise ValueError("msgsz_field must be a string.")
 
+    def set_subject_field(self, value: str) -> None:
+        if isinstance(value, str):
+            self.__subject_field = value
+        else:
+            raise ValueError("subject_field must be a string.")
+
     # Setter for date_field
     def set_date_field(self, value: str) -> None:
         if isinstance(value, str):
             self.__date_field = value
         else:
             raise ValueError("date_field must be a string.")
```

### Comparing `senderstats-1.2.1/src/senderstats/lib/MessageDataReport.py` & `senderstats-1.2.2/src/senderstats/lib/MessageDataReport.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,32 +9,38 @@
 class MessageDataReport:
     __threshold: int
     __data_processor: MessageDataProcessor
     __workbook: Workbook
     __header_format: Format
     __summary_format: Format
     __summary_values_format: Format
+    __subject_format: Format
+    __data_cell_format: Format
     __days: int
 
     def __init__(self, output_file: str, data_processor: MessageDataProcessor, threshold: int):
         self.__data_processor = data_processor
         self.__days = len(data_processor.get_date_counter())
         self.__threshold = threshold
 
         self.__workbook = Workbook(output_file)
         self.__summary_format = self.__workbook.add_format()
         self.__summary_format.set_bold()
         self.__summary_format.set_align('right')
 
         self.__summary_values_format = self.__workbook.add_format()
-        self.__summary_values_format.set_align("right")
+        self.__summary_values_format.set_align('right')
 
         self.__header_format = self.__workbook.add_format()
         self.__header_format.set_bold()
 
+        self.__data_cell_format = self.__workbook.add_format({'valign': 'top'})
+
+        self.__subject_format = self.__workbook.add_format({'text_wrap': True})
+
     def close(self):
         self.__workbook.close()
 
     def __write_headers(self, worksheet: Worksheet, headers: list):
         """
         Writes data to an Excel worksheet with given headers and applies formatting.
 
@@ -57,32 +63,35 @@
         row = 1
         for k, v in data.items():
             col = 0
             # If it contains a fat index
             if isinstance(k, tuple):
                 # Write the fat index to columns
                 for data in k:
-                    worksheet.write_string(row, col, data)
+                    worksheet.write_string(row, col, data, self.__data_cell_format)
                     col += 1
             else:
-                worksheet.write_string(row, col, k)
+                worksheet.write_string(row, col, k, self.__data_cell_format)
                 col += 1
 
-            messages_per_sender = len(v)
-            total_bytes = sum(v)
-            average_message_size = average(v)
+            messages_per_sender = len(v['message_size'])
+            total_bytes = sum(v['message_size'])
+            average_message_size = average(v['message_size'])
             messages_per_sender_per_day = messages_per_sender / self.__days
 
-            worksheet.write_number(row, col, messages_per_sender)
+            worksheet.write_number(row, col, messages_per_sender, self.__data_cell_format)
             col += 1
-            worksheet.write_number(row, col, average_message_size)
+            worksheet.write_number(row, col, average_message_size, self.__data_cell_format)
             col += 1
-            worksheet.write_number(row, col, messages_per_sender_per_day)
+            worksheet.write_number(row, col, messages_per_sender_per_day, self.__data_cell_format)
             col += 1
-            worksheet.write_number(row, col, total_bytes)
+            worksheet.write_number(row, col, total_bytes, self.__data_cell_format)
+            if 'subjects' in v:
+                col += 1
+                worksheet.write_string(row, col, '\n'.join(v['subjects']), self.__subject_format)
             row += 1
 
     def create_sizing_summary(self):
         summary = self.__workbook.add_worksheet("Summary")
         summary.write(0, 0, "Estimated App Data ({} days)".format(self.__days), self.__summary_format)
         summary.write(1, 0, "Estimated App Messages ({} days)".format(self.__days), self.__summary_format)
         summary.write(2, 0, "Estimated App Average Message Size ({} days)".format(self.__days), self.__summary_format)
@@ -146,45 +155,66 @@
                                   days=self.__days,
                                   threshold=self.__threshold),
                               self.__summary_values_format)
         summary.autofit()
 
     def create_mfrom_summary(self):
         sender_sheet = self.__workbook.add_worksheet("Envelope Senders")
-        self.__write_headers(sender_sheet,
-                             ['MFrom', 'Messages', 'Size', 'Messages Per Day', 'Total Bytes'])
+        headers = ['MFrom', 'Messages', 'Size', 'Messages Per Day', 'Total Bytes']
+
+        if self.__data_processor.get_opt_sample_subject():
+            headers.append('Subjects')
+
+        self.__write_headers(sender_sheet, headers)
         self.__write_data(sender_sheet, self.__data_processor.get_mfrom_data())
         sender_sheet.autofit()
 
     def create_hfrom_summary(self):
         from_sheet = self.__workbook.add_worksheet("Header From")
-        self.__write_headers(from_sheet,
-                             ['HFrom', 'Messages', 'Size', 'Messages Per Day', 'Total Bytes'])
+        headers = ['HFrom', 'Messages', 'Size', 'Messages Per Day', 'Total Bytes']
+
+        if self.__data_processor.get_opt_sample_subject():
+            headers.append('Subjects')
+
+        self.__write_headers(from_sheet, headers)
         self.__write_data(from_sheet, self.__data_processor.get_hfrom_data())
         from_sheet.autofit()
 
     def create_rpath_summary(self):
         return_sheet = self.__workbook.add_worksheet("Return Path")
-        self.__write_headers(return_sheet,
-                             ['RPath', 'Messages', 'Size', 'Messages Per Day', 'Total Bytes'])
+
+        headers = ['RPath', 'Messages', 'Size', 'Messages Per Day', 'Total Bytes']
+
+        if self.__data_processor.get_opt_sample_subject():
+            headers.append('Subjects')
+
+        self.__write_headers(return_sheet, headers)
         self.__write_data(return_sheet, self.__data_processor.get_rpath_data())
         return_sheet.autofit()
 
     def create_msgid_summary(self):
         mid_sheet = self.__workbook.add_worksheet("MFrom + Message ID")
-        self.__write_headers(mid_sheet,
-                             ['MFrom', 'Message ID Host', 'Message ID Domain', 'Messages', 'Size',
-                              'Messages Per Day', 'Total Bytes'])
+        headers = ['MFrom', 'Message ID Host', 'Message ID Domain', 'Messages', 'Size', 'Messages Per Day',
+                   'Total Bytes']
+
+        if self.__data_processor.get_opt_sample_subject():
+            headers.append('Subjects')
+
+        self.__write_headers(mid_sheet, headers)
         self.__write_data(mid_sheet, self.__data_processor.get_msgid_data())
         mid_sheet.autofit()
 
     def create_mfrom_hfrom_summary(self):
         sender_from_sheet = self.__workbook.add_worksheet("MFrom + HFrom (Alignment)")
-        self.__write_headers(sender_from_sheet,
-                             ['MFrom', 'HFrom', 'Messages', 'Size', 'Messages Per Day', 'Total Bytes'])
+        headers = ['MFrom', 'HFrom', 'Messages', 'Size', 'Messages Per Day', 'Total Bytes']
+
+        if self.__data_processor.get_opt_sample_subject():
+            headers.append('Subjects')
+
+        self.__write_headers(sender_from_sheet, headers)
         self.__write_data(sender_from_sheet, self.__data_processor.get_mfrom_hfrom_data())
         sender_from_sheet.autofit()
 
     def generate_report(self):
         self.create_sizing_summary()
         # Only create a worksheet for data that exists
         if self.__data_processor.get_mfrom_data():
```

### Comparing `senderstats-1.2.1/src/senderstats.egg-info/PKG-INFO` & `senderstats-1.2.2/src/senderstats.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: senderstats
-Version: 1.2.1
+Version: 1.2.2
 Summary: Tool to Process Smart Search Results and Identify Top Senders
 License: MIT
 Project-URL: repository, https://github.com/pfptcommunity/senderstats
 Requires-Python: >3.9
 Description-Content-Type: text/markdown
 Requires-Dist: xlsxwriter
 Requires-Dist: tldextract
@@ -26,49 +26,58 @@
 ```
 
 or can install the tool using pip.
 
 ```
 pip install senderstats
 ```
+
 ### Use Cases:
+
 **Outbound message volumes and data transferred by:**
-  * Envelope sender
-  * Header From:
-  * Return-Path:
-  * Envelope header: From:, MessageID Host, MessageID Domain (helpful to identify original sender)
-  * Envelope sender and header From: for SPF alignment purposes
+
+* Envelope sender
+* Header From:
+* Return-Path:
+* Envelope header: From:, MessageID Host, MessageID Domain (helpful to identify original sender)
+* Envelope sender and header From: for SPF alignment purposes
+* Random subject line sampling to help understand the type of traffic
 
 **Summarize message volume information:**
-  * Estimated application email traffic based on sender volume threshold:
-    * Estimated application data 
-    * Estimated application messages 
-    * Estimated application average size 
+
+* Estimated application email traffic based on sender volume threshold:
+    * Estimated application data
+    * Estimated application messages
+    * Estimated application average size
     * Estimated application peak hourly volume
-  * Total outbound data
-    * Total outbound data 
-    * Total outbound messages 
+* Total outbound data
+    * Total outbound data
+    * Total outbound messages
     * Total outbound average size
     * Total outbound peak hourly volume
 
 ### Usage Options:
+
 ```
-usage: senderstats [-h] -i <file> [<file> ...] -o <xlsx> [--mfrom MFrom] [--hfrom HFrom] [--rpath RPath] [--msgid MsgID] [--size MsgSz] [--date Date] [--gen-hfrom] [--gen-rpath] [--gen-alignment] [--gen-msgid] [-t THRESHOLD] [--no-display-name] [--remove-prvs] [--decode-srs] [--no-empty-hfrom] [--excluded-domains <domain> [<domain> ...]] [--restrict-domains <domain> [<domain> ...]] [--excluded-senders <sender> [<sender> ...]] [--date-format DateFmt] [--show-skip-detail]
+usage: senderstats [-h] -i <file> [<file> ...] -o <xlsx> [--mfrom MFrom] [--hfrom HFrom] [--rpath RPath] [--msgid MsgID] [--subject Subject] [--size MsgSz] [--date Date] [--gen-hfrom] [--gen-rpath] [--gen-alignment] [--gen-msgid]
+                   [-t N] [--no-display-name] [--remove-prvs] [--decode-srs] [--no-empty-hfrom] [--sample-subject] [--excluded-domains <domain> [<domain> ...]] [--restrict-domains <domain> [<domain> ...]]
+                   [--excluded-senders <sender> [<sender> ...]] [--date-format DateFmt] [--show-skip-detail]
 
 This tool helps identify the top senders based on smart search outbound message exports.
 
 Required arguments (optional):
   -i <file> [<file> ...], --input <file> [<file> ...]  Smart search files to read.
   -o <xlsx>, --output <xlsx>                           Output file
 
 Field mapping arguments (optional):
   --mfrom MFrom                                        CSV field of the envelope sender address. (default=Sender)
   --hfrom HFrom                                        CSV field of the header From: address. (default=Header_From)
   --rpath RPath                                        CSV field of the Return-Path: address. (default=Header_Return-Path)
   --msgid MsgID                                        CSV field of the message ID. (default=Message_ID)
+  --subject Subject                                    CSV field of the Subject, only used if --sample-subject is specified. (default=Subject)
   --size MsgSz                                         CSV field of message size. (default=Message_Size)
   --date Date                                          CSV field of message date/time. (default=Date)
 
 Reporting control arguments (optional):
   --gen-hfrom                                          Generate report showing the header From: data for messages being sent.
   --gen-rpath                                          Generate report showing return path for messages being sent.
   --gen-alignment                                      Generate report showing envelope sender and header From: alignment
@@ -76,41 +85,44 @@
   -t N, --threshold N                                  Adjust summary report threshold for messages per day to be considered application traffic. (default=100)
 
 Parsing behavior arguments (optional):
   --no-display-name                                    Remove display and use address only. Converts 'Display Name <user@domain.com>' to 'user@domain.com'
   --remove-prvs                                        Remove return path verification strings e.g. prvs=tag=sender@domain.com
   --decode-srs                                         Convert sender rewrite scheme, forwardmailbox+srs=hash=tt=domain.com=user to user@domain.com
   --no-empty-hfrom                                     If the header From: is empty the envelope sender address is used
+  --sample-subject                                     Enable probabilistic random sampling of subject lines found during processing
   --excluded-domains <domain> [<domain> ...]           Exclude domains from processing.
   --restrict-domains <domain> [<domain> ...]           Constrain domains for processing.
   --excluded-senders <sender> [<sender> ...]           Exclude senders from processing.
   --date-format DateFmt                                Date format used to parse the timestamps. (default=%Y-%m-%dT%H:%M:%S.%f%z)
 
 Extended processing controls (optional):
   --show-skip-detail                                   Show skipped details
 
 Usage:
   -h, --help                                           Show this help message and exit
 ```
 
 ### Using the Tool with Proofpoint Smart Search
 
-Export all outbound message traffic as a smart search CSV. You may need to export multiple CSVs if the data per time window exceeds 1M records. The tool can ingest multiple CSVs files at once.
+Export all outbound message traffic as a smart search CSV. You may need to export multiple CSVs if the data per time
+window exceeds 1M records. The tool can ingest multiple CSVs files at once.
 
 ![smart_search_outbound](https://github.com/pfptcommunity/senderstats/assets/83429267/83693152-922e-489a-b06d-a0765ecaf3e8)
 
-Once the files are downlaoded to a target folder, you can run the following command with the path to the files you downloaded and specify a wildard.
+Once the files are downlaoded to a target folder, you can run the following command with the path to the files you
+downloaded and specify a wildard.
 
 ```
 senderstats -i C:\path\to\downloaded\files\smart_search_results_custer_hosted_2024_03_04_*.csv -o C:\path\to\output\file\my_cluster_hosted.xlsx
 ```
 
 ### Sample Output
 
-The execution results should look similar to the following depending the options you select. 
+The execution results should look similar to the following depending the options you select.
 
 ```
 Files to be processed:
 C:\Users\ljerabek\Downloads\smart_search_results_cluster_hosted_2024_03_04_173552.csv
 C:\Users\ljerabek\Downloads\smart_search_results_cluster_hosted_2024_03_04_173855.csv
 C:\Users\ljerabek\Downloads\smart_search_results_cluster_hosted_2024_03_04_173656.csv
 C:\Users\ljerabek\Downloads\smart_search_results_cluster_hosted_2024_03_04_173754.csv
```

### Comparing `senderstats-1.2.1/src/senderstats.egg-info/SOURCES.txt` & `senderstats-1.2.2/src/senderstats.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 .gitattributes
 .gitignore
 README.md
 pyproject.toml
 .github/workflows/python-publish.yml
 src/senderstats/__init__.py
 src/senderstats/cli.py
-src/senderstats/gui.py
 src/senderstats.egg-info/PKG-INFO
 src/senderstats.egg-info/SOURCES.txt
 src/senderstats.egg-info/dependency_links.txt
 src/senderstats.egg-info/entry_points.txt
 src/senderstats.egg-info/requires.txt
 src/senderstats.egg-info/top_level.txt
 src/senderstats/common/__init__.py
```

