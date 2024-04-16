# Comparing `tmp/ops-py-azure-key-vault-report-4.0.1.tar.gz` & `tmp/ops_py_azure_key_vault_report-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ops-py-azure-key-vault-report-4.0.1.tar", last modified: Fri Apr 12 13:14:34 2024, max compression
+gzip compressed data, was "ops_py_azure_key_vault_report-5.0.0.tar", last modified: Tue Apr 16 10:42:19 2024, max compression
```

## Comparing `ops-py-azure-key-vault-report-4.0.1.tar` & `ops_py_azure_key_vault_report-5.0.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:14:34.949968 ops-py-azure-key-vault-report-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-12 13:14:33.000000 ops-py-azure-key-vault-report-4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11193 2024-04-12 13:14:34.949968 ops-py-azure-key-vault-report-4.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:14:34.949968 ops-py-azure-key-vault-report-4.0.1/azure_key_vault_report/
--rwxr-xr-x   0 runner    (1001) docker     (127)      120 2024-04-12 13:14:30.000000 ops-py-azure-key-vault-report-4.0.1/azure_key_vault_report/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2848 2024-04-12 13:14:30.000000 ops-py-azure-key-vault-report-4.0.1/azure_key_vault_report/az_cmd.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17634 2024-04-12 13:14:30.000000 ops-py-azure-key-vault-report-4.0.1/azure_key_vault_report/azure_key_vault_report.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      929 2024-04-12 13:14:30.000000 ops-py-azure-key-vault-report-4.0.1/azure_key_vault_report/config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1346 2024-04-12 13:14:30.000000 ops-py-azure-key-vault-report-4.0.1/azure_key_vault_report/html_table.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1219 2024-04-12 13:14:30.000000 ops-py-azure-key-vault-report-4.0.1/azure_key_vault_report/markdown.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3185 2024-04-12 13:14:30.000000 ops-py-azure-key-vault-report-4.0.1/azure_key_vault_report/ms_teams_json.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      949 2024-04-12 13:14:30.000000 ops-py-azure-key-vault-report-4.0.1/azure_key_vault_report/set_timestamp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:14:34.949968 ops-py-azure-key-vault-report-4.0.1/ops_py_azure_key_vault_report.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11193 2024-04-12 13:14:34.000000 ops-py-azure-key-vault-report-4.0.1/ops_py_azure_key_vault_report.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-12 13:14:34.000000 ops-py-azure-key-vault-report-4.0.1/ops_py_azure_key_vault_report.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 13:14:34.000000 ops-py-azure-key-vault-report-4.0.1/ops_py_azure_key_vault_report.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-12 13:14:34.000000 ops-py-azure-key-vault-report-4.0.1/ops_py_azure_key_vault_report.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-12 13:14:33.000000 ops-py-azure-key-vault-report-4.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     9772 2024-04-12 13:14:33.000000 ops-py-azure-key-vault-report-4.0.1/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 13:14:34.949968 ops-py-azure-key-vault-report-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-12 13:14:33.000000 ops-py-azure-key-vault-report-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:42:19.601046 ops_py_azure_key_vault_report-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-16 10:42:17.000000 ops_py_azure_key_vault_report-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11193 2024-04-16 10:42:19.601046 ops_py_azure_key_vault_report-5.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:42:19.601046 ops_py_azure_key_vault_report-5.0.0/azure_key_vault_report/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      120 2024-04-16 10:42:14.000000 ops_py_azure_key_vault_report-5.0.0/azure_key_vault_report/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2848 2024-04-16 10:42:14.000000 ops_py_azure_key_vault_report-5.0.0/azure_key_vault_report/az_cmd.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18781 2024-04-16 10:42:14.000000 ops_py_azure_key_vault_report-5.0.0/azure_key_vault_report/azure_key_vault_report.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      929 2024-04-16 10:42:14.000000 ops_py_azure_key_vault_report-5.0.0/azure_key_vault_report/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1346 2024-04-16 10:42:14.000000 ops_py_azure_key_vault_report-5.0.0/azure_key_vault_report/html_table.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1218 2024-04-16 10:42:14.000000 ops_py_azure_key_vault_report-5.0.0/azure_key_vault_report/markdown.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3185 2024-04-16 10:42:14.000000 ops_py_azure_key_vault_report-5.0.0/azure_key_vault_report/ms_teams_json.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      949 2024-04-16 10:42:14.000000 ops_py_azure_key_vault_report-5.0.0/azure_key_vault_report/set_timestamp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4149 2024-04-16 10:42:14.000000 ops_py_azure_key_vault_report-5.0.0/azure_key_vault_report/slack_payloads.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:42:19.601046 ops_py_azure_key_vault_report-5.0.0/ops_py_azure_key_vault_report.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11193 2024-04-16 10:42:19.000000 ops_py_azure_key_vault_report-5.0.0/ops_py_azure_key_vault_report.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-16 10:42:19.000000 ops_py_azure_key_vault_report-5.0.0/ops_py_azure_key_vault_report.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 10:42:19.000000 ops_py_azure_key_vault_report-5.0.0/ops_py_azure_key_vault_report.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-16 10:42:19.000000 ops_py_azure_key_vault_report-5.0.0/ops_py_azure_key_vault_report.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-16 10:42:17.000000 ops_py_azure_key_vault_report-5.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     9772 2024-04-16 10:42:17.000000 ops_py_azure_key_vault_report-5.0.0/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 10:42:19.601046 ops_py_azure_key_vault_report-5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-16 10:42:17.000000 ops_py_azure_key_vault_report-5.0.0/setup.py
```

### Comparing `ops-py-azure-key-vault-report-4.0.1/LICENSE` & `ops_py_azure_key_vault_report-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ops-py-azure-key-vault-report-4.0.1/PKG-INFO` & `ops_py_azure_key_vault_report-5.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-py-azure-key-vault-report
-Version: 4.0.1
+Version: 5.0.0
 Summary: Output a Key Vault Secrets report
 License: MIT License
         
         Copyright (c) 2024 Equinor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `ops-py-azure-key-vault-report-4.0.1/azure_key_vault_report/az_cmd.py` & `ops_py_azure_key_vault_report-5.0.0/azure_key_vault_report/az_cmd.py`

 * *Files identical despite different names*

### Comparing `ops-py-azure-key-vault-report-4.0.1/azure_key_vault_report/azure_key_vault_report.py` & `ops_py_azure_key_vault_report-5.0.0/azure_key_vault_report/azure_key_vault_report.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import logging
 import datetime
 from .html_table import HTMLTable
 from .ms_teams_json import MSTeamsPayload
 from .set_timestamp import set_timestamp, now
 from .markdown import Markdown
 from .config import *
+from .slack_payloads import SlackPayloads
 
 
 ########################################################################################################################
 
 
 class AzureKeyVaultReport(object):
     """generates a report from the results of 'az keyvault' commands
@@ -92,14 +93,16 @@
         self.items = []
         self.vaults = []        # The unique list of vaults processed
         self.html_table = None  # HTML table object. Used for MS Teams
         self.report_md = ""
         self.report = []
         self.summary = {}
         self.summary_md = ""
+        self.report_summary_md = ""
+        self.slack_rows_md = []
         self.summary_values = config.get("summary")
         self.report_values = config.get("report")
         self.report_full = {
             "created_at": datetime.datetime.utcnow().isoformat(),
             "summary": {},
             "report": {}
         }
@@ -353,14 +356,19 @@
                         # Only skipped if 'include_all' is not specified.
                         if not include_all:
                             continue
 
             # Then finally add the row to the rows (The ones that will be reported)
             rows.append(row)
 
+            # Get Slack Markdown Payload of current row and add it is to list of Slack Markdown payloads
+            slack_md_payload = self.get_slack_md(row)
+            if slack_md_payload:
+                self.slack_rows_md.append(slack_md_payload)
+
             # If a html_table is created, then also add the row to the html table. Used in MS Teams payload
             if self.html_table:
                 self.html_table.add_html_row(*row)
 
         self.report_full["report"]["rows"] = self.create_kv_rows(rows_all)
 
         if include_all:
@@ -377,14 +385,22 @@
             self.report_md = md.get_output()
 
             # Create json of the report
             self.report = self.create_kv_rows(rows)
 
         logging.info("report generated.")
 
+    def get_slack_md(self, row):
+        payload = {"text": ""}
+        for i, x in enumerate(self.report_values["heading"]):
+            payload["text"] += f"*{row[i]}:* {x}\n"
+
+        if payload.get("text"):
+            return payload
+
     def create_kv_rows(self, rows):
         kv_rows = []
         for i, r in enumerate(rows):
             if i > 0:
                 j = {}
                 for n, v in enumerate(self.report_values.get("heading")):
                     j[v] = r[n]
@@ -407,17 +423,19 @@
     def get_report_markdown(self):
         """return the Markdown report"""
         return self.report_md
 
     def get_report_summary_markdown(self):
         """return the plain text report"""
         if self.report_md:
-            return f"{self.summary_md}\n\n{self.report_md}"
+            self.report_summary_md = f"{self.summary_md}\n\n{self.report_md}"
+        else:
+            self.report_summary_md = self.summary_md
 
-        return self.summary_md
+        return self.report_summary_md
 
     def get_teams_payload(self, title, text=""):
         """build and return the MS Teams payload"""
         if not isinstance(self.results, list):
             return
 
         if len(self.items) == 0:
@@ -430,7 +448,22 @@
         ms_teams_payload.set_json_facts()
         return ms_teams_payload.get_json_output()
 
     def get_html_table(self):
         """return the html table"""
         if self.html_table:
             return self.html_table.get_table()
+
+    def get_slack_payloads(self, title, max_chars=3500, app=True, md=True):
+
+        if md:
+            return self.slack_rows_md
+
+        self.get_summary_markdown()
+        self.get_report_summary_markdown()
+        self.get_report_markdown()
+
+        p = SlackPayloads(title, self.summary_md, self.report_md, self.report_summary_md, max_chars=max_chars)
+        if app:
+            return p.get_app_payloads()
+
+        return p.get_workflow_posts()
```

### Comparing `ops-py-azure-key-vault-report-4.0.1/azure_key_vault_report/config.py` & `ops_py_azure_key_vault_report-5.0.0/azure_key_vault_report/config.py`

 * *Files identical despite different names*

### Comparing `ops-py-azure-key-vault-report-4.0.1/azure_key_vault_report/html_table.py` & `ops_py_azure_key_vault_report-5.0.0/azure_key_vault_report/html_table.py`

 * *Files identical despite different names*

### Comparing `ops-py-azure-key-vault-report-4.0.1/azure_key_vault_report/markdown.py` & `ops_py_azure_key_vault_report-5.0.0/azure_key_vault_report/markdown.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,8 +36,7 @@
             output += "|\n"
 
             if header_line:
                 output += f"{header_line}|\n"
                 header_line = ""
 
         return output
-
```

### Comparing `ops-py-azure-key-vault-report-4.0.1/azure_key_vault_report/ms_teams_json.py` & `ops_py_azure_key_vault_report-5.0.0/azure_key_vault_report/ms_teams_json.py`

 * *Files identical despite different names*

### Comparing `ops-py-azure-key-vault-report-4.0.1/azure_key_vault_report/set_timestamp.py` & `ops_py_azure_key_vault_report-5.0.0/azure_key_vault_report/set_timestamp.py`

 * *Files identical despite different names*

### Comparing `ops-py-azure-key-vault-report-4.0.1/ops_py_azure_key_vault_report.egg-info/PKG-INFO` & `ops_py_azure_key_vault_report-5.0.0/ops_py_azure_key_vault_report.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-py-azure-key-vault-report
-Version: 4.0.1
+Version: 5.0.0
 Summary: Output a Key Vault Secrets report
 License: MIT License
         
         Copyright (c) 2024 Equinor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `ops-py-azure-key-vault-report-4.0.1/ops_py_azure_key_vault_report.egg-info/SOURCES.txt` & `ops_py_azure_key_vault_report-5.0.0/ops_py_azure_key_vault_report.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -6,11 +6,12 @@
 azure_key_vault_report/az_cmd.py
 azure_key_vault_report/azure_key_vault_report.py
 azure_key_vault_report/config.py
 azure_key_vault_report/html_table.py
 azure_key_vault_report/markdown.py
 azure_key_vault_report/ms_teams_json.py
 azure_key_vault_report/set_timestamp.py
+azure_key_vault_report/slack_payloads.py
 ops_py_azure_key_vault_report.egg-info/PKG-INFO
 ops_py_azure_key_vault_report.egg-info/SOURCES.txt
 ops_py_azure_key_vault_report.egg-info/dependency_links.txt
 ops_py_azure_key_vault_report.egg-info/top_level.txt
```

### Comparing `ops-py-azure-key-vault-report-4.0.1/readme.md` & `ops_py_azure_key_vault_report-5.0.0/readme.md`

 * *Files identical despite different names*

