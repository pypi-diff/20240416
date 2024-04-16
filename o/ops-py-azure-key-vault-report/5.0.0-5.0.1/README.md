# Comparing `tmp/ops_py_azure_key_vault_report-5.0.0.tar.gz` & `tmp/ops_py_azure_key_vault_report-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ops_py_azure_key_vault_report-5.0.0.tar", last modified: Tue Apr 16 10:42:19 2024, max compression
+gzip compressed data, was "ops_py_azure_key_vault_report-5.0.1.tar", last modified: Tue Apr 16 12:51:50 2024, max compression
```

## Comparing `ops_py_azure_key_vault_report-5.0.0.tar` & `ops_py_azure_key_vault_report-5.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:42:19.601046 ops_py_azure_key_vault_report-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-16 10:42:17.000000 ops_py_azure_key_vault_report-5.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11193 2024-04-16 10:42:19.601046 ops_py_azure_key_vault_report-5.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:42:19.601046 ops_py_azure_key_vault_report-5.0.0/azure_key_vault_report/
--rwxr-xr-x   0 runner    (1001) docker     (127)      120 2024-04-16 10:42:14.000000 ops_py_azure_key_vault_report-5.0.0/azure_key_vault_report/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2848 2024-04-16 10:42:14.000000 ops_py_azure_key_vault_report-5.0.0/azure_key_vault_report/az_cmd.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18781 2024-04-16 10:42:14.000000 ops_py_azure_key_vault_report-5.0.0/azure_key_vault_report/azure_key_vault_report.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      929 2024-04-16 10:42:14.000000 ops_py_azure_key_vault_report-5.0.0/azure_key_vault_report/config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1346 2024-04-16 10:42:14.000000 ops_py_azure_key_vault_report-5.0.0/azure_key_vault_report/html_table.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1218 2024-04-16 10:42:14.000000 ops_py_azure_key_vault_report-5.0.0/azure_key_vault_report/markdown.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3185 2024-04-16 10:42:14.000000 ops_py_azure_key_vault_report-5.0.0/azure_key_vault_report/ms_teams_json.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      949 2024-04-16 10:42:14.000000 ops_py_azure_key_vault_report-5.0.0/azure_key_vault_report/set_timestamp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4149 2024-04-16 10:42:14.000000 ops_py_azure_key_vault_report-5.0.0/azure_key_vault_report/slack_payloads.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:42:19.601046 ops_py_azure_key_vault_report-5.0.0/ops_py_azure_key_vault_report.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11193 2024-04-16 10:42:19.000000 ops_py_azure_key_vault_report-5.0.0/ops_py_azure_key_vault_report.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-16 10:42:19.000000 ops_py_azure_key_vault_report-5.0.0/ops_py_azure_key_vault_report.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 10:42:19.000000 ops_py_azure_key_vault_report-5.0.0/ops_py_azure_key_vault_report.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-16 10:42:19.000000 ops_py_azure_key_vault_report-5.0.0/ops_py_azure_key_vault_report.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-16 10:42:17.000000 ops_py_azure_key_vault_report-5.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     9772 2024-04-16 10:42:17.000000 ops_py_azure_key_vault_report-5.0.0/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 10:42:19.601046 ops_py_azure_key_vault_report-5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-16 10:42:17.000000 ops_py_azure_key_vault_report-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:51:50.200017 ops_py_azure_key_vault_report-5.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-16 12:51:48.000000 ops_py_azure_key_vault_report-5.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11193 2024-04-16 12:51:50.196017 ops_py_azure_key_vault_report-5.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:51:50.196017 ops_py_azure_key_vault_report-5.0.1/azure_key_vault_report/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      120 2024-04-16 12:51:44.000000 ops_py_azure_key_vault_report-5.0.1/azure_key_vault_report/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2848 2024-04-16 12:51:44.000000 ops_py_azure_key_vault_report-5.0.1/azure_key_vault_report/az_cmd.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19628 2024-04-16 12:51:44.000000 ops_py_azure_key_vault_report-5.0.1/azure_key_vault_report/azure_key_vault_report.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      929 2024-04-16 12:51:44.000000 ops_py_azure_key_vault_report-5.0.1/azure_key_vault_report/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1346 2024-04-16 12:51:44.000000 ops_py_azure_key_vault_report-5.0.1/azure_key_vault_report/html_table.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1218 2024-04-16 12:51:44.000000 ops_py_azure_key_vault_report-5.0.1/azure_key_vault_report/markdown.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3185 2024-04-16 12:51:44.000000 ops_py_azure_key_vault_report-5.0.1/azure_key_vault_report/ms_teams_json.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      949 2024-04-16 12:51:44.000000 ops_py_azure_key_vault_report-5.0.1/azure_key_vault_report/set_timestamp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4149 2024-04-16 12:51:44.000000 ops_py_azure_key_vault_report-5.0.1/azure_key_vault_report/slack_payloads.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:51:50.196017 ops_py_azure_key_vault_report-5.0.1/ops_py_azure_key_vault_report.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11193 2024-04-16 12:51:50.000000 ops_py_azure_key_vault_report-5.0.1/ops_py_azure_key_vault_report.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-16 12:51:50.000000 ops_py_azure_key_vault_report-5.0.1/ops_py_azure_key_vault_report.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 12:51:50.000000 ops_py_azure_key_vault_report-5.0.1/ops_py_azure_key_vault_report.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-16 12:51:50.000000 ops_py_azure_key_vault_report-5.0.1/ops_py_azure_key_vault_report.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-16 12:51:48.000000 ops_py_azure_key_vault_report-5.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     9772 2024-04-16 12:51:48.000000 ops_py_azure_key_vault_report-5.0.1/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 12:51:50.200017 ops_py_azure_key_vault_report-5.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-16 12:51:48.000000 ops_py_azure_key_vault_report-5.0.1/setup.py
```

### Comparing `ops_py_azure_key_vault_report-5.0.0/LICENSE` & `ops_py_azure_key_vault_report-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_report-5.0.0/PKG-INFO` & `ops_py_azure_key_vault_report-5.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-py-azure-key-vault-report
-Version: 5.0.0
+Version: 5.0.1
 Summary: Output a Key Vault Secrets report
 License: MIT License
         
         Copyright (c) 2024 Equinor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `ops_py_azure_key_vault_report-5.0.0/azure_key_vault_report/az_cmd.py` & `ops_py_azure_key_vault_report-5.0.1/azure_key_vault_report/az_cmd.py`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_report-5.0.0/azure_key_vault_report/azure_key_vault_report.py` & `ops_py_azure_key_vault_report-5.0.1/azure_key_vault_report/azure_key_vault_report.py`

 * *Files 8% similar despite different names*

```diff
@@ -386,20 +386,48 @@
 
             # Create json of the report
             self.report = self.create_kv_rows(rows)
 
         logging.info("report generated.")
 
     def get_slack_md(self, row):
-        payload = {"text": ""}
-        for i, x in enumerate(self.report_values["heading"]):
-            payload["text"] += f"*{row[i]}:* {x}\n"
+        if not row:
+            return
 
-        if payload.get("text"):
-            return payload
+        payload = {
+                "blocks": [
+                    {
+                        "type": "header",
+                        "text": {
+                            "type": "plain_text",
+                            "text": f"{row[0]}"
+                        }
+                    },
+                    {
+                        "type": "section",
+                        "text": {
+                            "type": "mrkdwn",
+                            "text": f"*{row[-1]}*"
+                        }
+                    },
+                    {
+                        "type": "section",
+                        "fields": []
+                    }
+                ]
+            }
+
+        blocks = payload.get("blocks")
+        for i in range(1, len(row)-1):
+            x = {"type": "mrkdwn",
+                 "text": f"*{self.report_values['heading'][i]}:*\n{row[i]}"
+                 }
+            blocks[-1]["fields"].append(x)
+        blocks.append({"type": "divider"})
+        return payload
 
     def create_kv_rows(self, rows):
         kv_rows = []
         for i, r in enumerate(rows):
             if i > 0:
                 j = {}
                 for n, v in enumerate(self.report_values.get("heading")):
```

### Comparing `ops_py_azure_key_vault_report-5.0.0/azure_key_vault_report/config.py` & `ops_py_azure_key_vault_report-5.0.1/azure_key_vault_report/config.py`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_report-5.0.0/azure_key_vault_report/html_table.py` & `ops_py_azure_key_vault_report-5.0.1/azure_key_vault_report/html_table.py`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_report-5.0.0/azure_key_vault_report/markdown.py` & `ops_py_azure_key_vault_report-5.0.1/azure_key_vault_report/markdown.py`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_report-5.0.0/azure_key_vault_report/ms_teams_json.py` & `ops_py_azure_key_vault_report-5.0.1/azure_key_vault_report/ms_teams_json.py`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_report-5.0.0/azure_key_vault_report/set_timestamp.py` & `ops_py_azure_key_vault_report-5.0.1/azure_key_vault_report/set_timestamp.py`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_report-5.0.0/azure_key_vault_report/slack_payloads.py` & `ops_py_azure_key_vault_report-5.0.1/azure_key_vault_report/slack_payloads.py`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_report-5.0.0/ops_py_azure_key_vault_report.egg-info/PKG-INFO` & `ops_py_azure_key_vault_report-5.0.1/ops_py_azure_key_vault_report.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-py-azure-key-vault-report
-Version: 5.0.0
+Version: 5.0.1
 Summary: Output a Key Vault Secrets report
 License: MIT License
         
         Copyright (c) 2024 Equinor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `ops_py_azure_key_vault_report-5.0.0/ops_py_azure_key_vault_report.egg-info/SOURCES.txt` & `ops_py_azure_key_vault_report-5.0.1/ops_py_azure_key_vault_report.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_report-5.0.0/readme.md` & `ops_py_azure_key_vault_report-5.0.1/readme.md`

 * *Files identical despite different names*

