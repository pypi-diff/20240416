# Comparing `tmp/quip-cli-1.8.8.tar.gz` & `tmp/quip-cli-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quip-cli-1.8.8.tar", last modified: Fri Apr 14 18:34:55 2023, max compression
+gzip compressed data, was "quip-cli-1.9.0.tar", last modified: Mon Apr 15 22:08:12 2024, max compression
```

## Comparing `quip-cli-1.8.8.tar` & `quip-cli-1.9.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2023-04-14 18:34:55.375705 quip-cli-1.8.8/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    27790 2023-04-14 18:34:55.375370 quip-cli-1.8.8/PKG-INFO
--rwxrw-r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    27390 2022-11-10 22:02:44.000000 quip-cli-1.8.8/README.md
--rwxrw-r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       89 2023-02-23 14:36:14.000000 quip-cli-1.8.8/pyproject.toml
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2023-04-14 18:34:55.372090 quip-cli-1.8.8/quip/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2276 2023-04-14 17:57:00.000000 quip-cli-1.8.8/quip/__init__.py
--rwxrwxr--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    20123 2023-04-14 18:15:41.000000 quip-cli-1.8.8/quip/external.py
--rwxrwxr--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    19670 2022-11-10 22:25:14.000000 quip-cli-1.8.8/quip/field_builder.py
--rwxrwxr--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    73416 2023-04-14 18:24:04.000000 quip-cli-1.8.8/quip/quip.py
--rwxrwxr--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     7104 2022-12-05 17:10:38.000000 quip-cli-1.8.8/quip/version_builder.py
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2023-04-14 18:34:55.374920 quip-cli-1.8.8/quip_cli.egg-info/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    27790 2023-04-14 18:34:55.000000 quip-cli-1.8.8/quip_cli.egg-info/PKG-INFO
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      320 2023-04-14 18:34:55.000000 quip-cli-1.8.8/quip_cli.egg-info/SOURCES.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        1 2023-04-14 18:34:55.000000 quip-cli-1.8.8/quip_cli.egg-info/dependency_links.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       39 2023-04-14 18:34:55.000000 quip-cli-1.8.8/quip_cli.egg-info/entry_points.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      101 2023-04-14 18:34:55.000000 quip-cli-1.8.8/quip_cli.egg-info/requires.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        5 2023-04-14 18:34:55.000000 quip-cli-1.8.8/quip_cli.egg-info/top_level.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       38 2023-04-14 18:34:55.375766 quip-cli-1.8.8/setup.cfg
--rwxrw-r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1281 2022-10-06 20:00:12.000000 quip-cli-1.8.8/setup.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-15 22:08:12.881988 quip-cli-1.9.0/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    27949 2024-04-15 22:08:12.881753 quip-cli-1.9.0/PKG-INFO
+-rwxrw-r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    27549 2023-08-18 17:30:20.000000 quip-cli-1.9.0/README.md
+-rwxrw-r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       89 2023-02-23 14:36:14.000000 quip-cli-1.9.0/pyproject.toml
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-15 22:08:12.878738 quip-cli-1.9.0/quip/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2277 2024-04-15 21:16:21.000000 quip-cli-1.9.0/quip/__init__.py
+-rwxrwxr--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    20123 2023-04-14 18:15:41.000000 quip-cli-1.9.0/quip/external.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5307 2023-08-21 16:56:55.000000 quip-cli-1.9.0/quip/fact.py
+-rwxrwxr--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    22972 2024-04-15 21:45:23.000000 quip-cli-1.9.0/quip/field_builder.py
+-rwxrwxr--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    74251 2023-08-21 18:36:06.000000 quip-cli-1.9.0/quip/quip.py
+-rwxrwxr--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     7104 2022-12-05 17:10:38.000000 quip-cli-1.9.0/quip/version_builder.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-15 22:08:12.881311 quip-cli-1.9.0/quip_cli.egg-info/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    27949 2024-04-15 22:08:12.000000 quip-cli-1.9.0/quip_cli.egg-info/PKG-INFO
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      333 2024-04-15 22:08:12.000000 quip-cli-1.9.0/quip_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        1 2024-04-15 22:08:12.000000 quip-cli-1.9.0/quip_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       39 2024-04-15 22:08:12.000000 quip-cli-1.9.0/quip_cli.egg-info/entry_points.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      101 2024-04-15 22:08:12.000000 quip-cli-1.9.0/quip_cli.egg-info/requires.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        5 2024-04-15 22:08:12.000000 quip-cli-1.9.0/quip_cli.egg-info/top_level.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       38 2024-04-15 22:08:12.882028 quip-cli-1.9.0/setup.cfg
+-rwxrw-r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1281 2022-10-06 20:00:12.000000 quip-cli-1.9.0/setup.py
```

### Comparing `quip-cli-1.8.8/PKG-INFO` & `quip-cli-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quip-cli
-Version: 1.8.8
+Version: 1.9.0
 Summary: Tool for creating/updating new universal integrations
 Author: Stonebranch
 Author-email: huseyin.gomleksizoglu@stonebranch.com
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -542,28 +542,34 @@
   items: []
   dependencies:
   - end_point
   - region
   - credentials
   show_if:
     action: start-batch,sync-start-batch
+    required: true
 
 - application_id: Text
   start: true
   restriction: Output Only
   field_mapping: Text Field 1
   show_if:
     action: start-batch,sync-start-batch
 
 - parameters: Array
   start: true
   name_title: Parameter Name
   value_title: Parameter Value
   field_mapping: Array Field 1
   span: 2
+  values:
+  - task_name
+  - template: Value
+  - variable_1: Value 1
+  - variable_2: Value 2
 
 ```
 
 Format of the child elements are like this.
 
 * First value will be the name of the field and the value of that element will be the type of the field.
 * Field Types can be one of these items
@@ -587,14 +593,15 @@
     * span: If you want the field to fill the row set value to 2. Default: 1
     * text_type: If the text field has YAML or JSON content, set value to YAML or JSON. Default: Plain
     * dynamic: If the field is a dynamic choice field, set the value to true. Default: false
     * restriction: If the field has restrictions like output only, set the value to "Output Only". Default: No Restriction
     * name_title: This field is only for Array types. This field is the label of the first field.
     * value_title: This field is only for Array types. This field is the label of the second field.
     * titles: (alias: headers) This field is another representation of the name_title and value_title fields. You can set the name and value field title in a comma seperated string. For example: `titles: Field Name, Field Value`
+    * values: Default values of an Array field.
     * allow_multiple: This field is only for Choice types. To allow selecting multiple values, set value to true. Default: false
     * allow_empty: This field is only for Choice types. To allow not selecting any value, set value to true. Default: false
     * length: Sets the max lenght of the field.
     * max: Sets the maximum allowed number for that field.
     * min: Set the minimum allowed number for that field.
     
     ### items
```

### Comparing `quip-cli-1.8.8/README.md` & `quip-cli-1.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -530,28 +530,34 @@
   items: []
   dependencies:
   - end_point
   - region
   - credentials
   show_if:
     action: start-batch,sync-start-batch
+    required: true
 
 - application_id: Text
   start: true
   restriction: Output Only
   field_mapping: Text Field 1
   show_if:
     action: start-batch,sync-start-batch
 
 - parameters: Array
   start: true
   name_title: Parameter Name
   value_title: Parameter Value
   field_mapping: Array Field 1
   span: 2
+  values:
+  - task_name
+  - template: Value
+  - variable_1: Value 1
+  - variable_2: Value 2
 
 ```
 
 Format of the child elements are like this.
 
 * First value will be the name of the field and the value of that element will be the type of the field.
 * Field Types can be one of these items
@@ -575,14 +581,15 @@
     * span: If you want the field to fill the row set value to 2. Default: 1
     * text_type: If the text field has YAML or JSON content, set value to YAML or JSON. Default: Plain
     * dynamic: If the field is a dynamic choice field, set the value to true. Default: false
     * restriction: If the field has restrictions like output only, set the value to "Output Only". Default: No Restriction
     * name_title: This field is only for Array types. This field is the label of the first field.
     * value_title: This field is only for Array types. This field is the label of the second field.
     * titles: (alias: headers) This field is another representation of the name_title and value_title fields. You can set the name and value field title in a comma seperated string. For example: `titles: Field Name, Field Value`
+    * values: Default values of an Array field.
     * allow_multiple: This field is only for Choice types. To allow selecting multiple values, set value to true. Default: false
     * allow_empty: This field is only for Choice types. To allow not selecting any value, set value to true. Default: false
     * length: Sets the max lenght of the field.
     * max: Sets the maximum allowed number for that field.
     * min: Set the minimum allowed number for that field.
     
     ### items
```

### Comparing `quip-cli-1.8.8/quip/__init__.py` & `quip-cli-1.9.0/quip/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from colorama import Fore, Style, init
+
 init()
 
-__version__ = "1.8.8"
+__version__ = "1.9.0"
 
 def cprint(text, color, end='\n', style='Normal'):
     if len(str(text).strip()) == 0: return
     fore = getattr(Fore, color.upper())
     style = getattr(Style, style.upper())
     print('{0}{1}{2}{3}'.format(fore, style, text, Style.RESET_ALL), end=end)
```

### Comparing `quip-cli-1.8.8/quip/external.py` & `quip-cli-1.9.0/quip/external.py`

 * *Files identical despite different names*

### Comparing `quip-cli-1.8.8/quip/field_builder.py` & `quip-cli-1.9.0/quip/field_builder.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 
 def prepare_fields(fields, code):
     numbers = {}
     available_fields = { 
         "Text": list(range(1, 21)),
         "Large Text": list(range(1, 5)),
         "Integer": list(range(1, 11)),
-        "Boolean": list(range(1, 11)),
+        "Boolean": list(range(1, 16)),
         "Choice": list(range(1, 16)),
         "Credential": list(range(1, 7)),
-        "Script": list(range(1, 3)),
+        "Script": list(range(1, 5)),
         "Array": list(range(1, 5)),
-        "Float": list(range(1, 5))
+        "Float": list(range(1, 5)),
+        "Sap Connection": list(range(1, 2)),
+        "Database Connection": list(range(1, 2))
     }
 
     field_mapping = {}
     fields_dict = []
     for field in fields: # Check the ones having field_mapping
         name = list(field.keys())[0]
         type = list(field.values())[0]
@@ -49,17 +51,21 @@
         type = list(field.values())[0]
         type = get_type_name(type)
         if not code: 
             print(f"{name}:{type}:{field_mapping[name]}")
         
         sequence = len(fields_dict)
         if type in ["Text", "Large Text"]:
-            _dict = create_text_field(name, field_mapping[name], sequence)
+            regex = field.get("regex", None)
+            _dict = create_text_field(name, field_mapping[name], sequence, regex)
         elif type == "Credential":
-            _dict = create_credential_field(name, field_mapping[name], sequence)
+            allow_var = field.get("allow_variable", False)
+            if allow_var:
+                field["span"] = 2
+            _dict = create_credential_field(name, field_mapping[name], sequence, allow_var)
         elif type == "Script":
             _dict = create_script_field(name, field_mapping[name], sequence)
         elif type == "Boolean":
             _dict = create_boolean_field(name, field_mapping[name], sequence)
         elif type == "Choice":
             if code:
                 if field.get("dynamic", False):
@@ -71,15 +77,15 @@
             elif "headers" in field:
                 name_title, value_title = field["headers"].split(",")
             else:
                 name_title = field["name_title"]
                 value_title = field["value_title"]
             name_title = name_title.strip(" ")
             value_title = value_title.strip(" ")
-            _dict = create_array_field(name, field_mapping[name], sequence, name_title, value_title)
+            _dict = create_array_field(name, field_mapping[name], sequence, name_title, value_title, field.get("values", []))
         else:
             _dict = copy.copy(FIELD_TEMPLATE)
             _dict["name"] = name
             _dict["label"] = labelize(name)
             _dict["fieldType"] = type
             _dict["sequence"] = sequence
             _dict["fieldMapping"] = field_mapping[name]
@@ -99,14 +105,27 @@
     set_if_not_equal(result, "agentType", conf.get("agent_type", None), None)
     set_if_not_equal(result, "description", conf.get("description", None), None)
     set_if_not_equal(result, "extension", conf.get("extension", None), None)
     set_if_not_equal(result, "minReleaseLevel", conf.get("min_release", None), None)
     set_if_not_equal(result, "variablePrefix", conf.get("var_prefix", None), None)
     set_if_not_equal(result, "sysId", conf.get("sys_id", None), None)
     set_if_not_equal(result, "scriptTypeWindows", conf.get("script_ext_windows", None), None)
+    set_if_not_equal(result, "useCommonScript", conf.get("common_script", None), None)
+    set_if_not_equal(result, "alwaysCancelOnFinish", conf.get("always_cancel", None), None)
+    set_if_not_equal(result, "sendEnvironment", conf.get("send_environment", "Launch"), "Launch")
+    if str(result["sendEnvironment"]).lower() in ["all", "yes", "true"]:
+        result["sendEnvironment"] = "Launch, Dynamic Choice, Dynamic Command"
+    elif str(result["sendEnvironment"]).lower() in ["", "no", "false"]:
+        result["sendEnvironment"] = "Launch"
+    set_if_not_equal(result, "sendVariables", conf.get("send_variables", None), None)
+    if str(result.get("sendVariables", "")).lower() in ["local", "yes", "true"]:
+        result["sendVariables"] = "Local"
+    elif str(result.get("sendVariables", "")).lower() in ["", "no", "false"]:
+        result["sendVariables"] = None
+
     return result
 
 
 def get_type_name(type):
     type = type.title()
     if type.lower() in ["large", "largetext", "textarea", "text area"]:
         type = "Large Text"
@@ -117,31 +136,33 @@
     elif type.lower() in ["creds", "cred", "credentials"]:
         type = "Credential"
     elif type.lower() in ["bool", "check", "checkbox", "check box"]:
         type = "Boolean"
     return type
 
 
-def create_text_field(name, _mapping, sequence):
+def create_text_field(name, _mapping, sequence, regex=None):
     field_dict = copy.copy(FIELD_TEMPLATE)
     field_dict["name"] = name
     field_dict["label"] = labelize(name)
     field_dict["fieldType"] = "Text"
     field_dict["sequence"] = sequence
     field_dict["fieldMapping"] = _mapping
+    field_dict["fieldRegex"] = regex
     field_dict["sysId"] = new_uuid()
     return field_dict
 
-def create_credential_field(name, _mapping, sequence):
+def create_credential_field(name, _mapping, sequence, allow_variable=True):
     field_dict = dict(copy.copy(FIELD_TEMPLATE))
     field_dict["name"] = name
     field_dict["label"] = labelize(name)
     field_dict["fieldType"] = "Credential"
     field_dict["sequence"] = sequence
     field_dict["fieldMapping"] = _mapping
+    field_dict["allowVariable"] = allow_variable
     field_dict["sysId"] = new_uuid()
     return field_dict
 
 def create_choice_field(name, _mapping, sequence, options):
     field_dict = copy.copy(FIELD_TEMPLATE)
     field_dict["name"] = name
     field_dict["label"] = labelize(name)
@@ -156,14 +177,16 @@
             _choice_dict["fieldValue"] = option
             _choice_dict["fieldValueLabel"] = labelize(option)
         elif isinstance(option, dict):
             option_name = list(option.keys())[0]
             option_label = list(option.values())[0]
             _choice_dict["fieldValue"] = option_name
             _choice_dict["fieldValueLabel"] = option_label
+        if _choice_dict["fieldValue"] == _choice_dict["fieldValueLabel"]:
+            _choice_dict["useFieldValueForLabel"] = True
         _choice_dict["sysId"] = new_uuid()
         _choice_dict["sequence"] = len(field_dict["choices"])
         field_dict["choices"].append(_choice_dict)
     return field_dict
 
 def create_script_field(name, _mapping, sequence):
     field_dict = dict(copy.copy(FIELD_TEMPLATE))
@@ -181,29 +204,39 @@
     field_dict["label"] = labelize(name)
     field_dict["fieldType"] = "Boolean"
     field_dict["sequence"] = sequence
     field_dict["fieldMapping"] = _mapping
     field_dict["sysId"] = new_uuid()
     return field_dict
 
-def create_array_field(name, _mapping, sequence, name_title, value_title):
+def create_array_field(name, _mapping, sequence, name_title, value_title, items):
     field_dict = dict(copy.copy(FIELD_TEMPLATE))
     field_dict["name"] = name
     field_dict["label"] = labelize(name)
     field_dict["fieldType"] = "Array"
     field_dict["sequence"] = sequence
     field_dict["fieldMapping"] = _mapping
     field_dict["arrayNameTitle"] = name_title
     field_dict["arrayValueTitle"] = value_title
     field_dict["sysId"] = new_uuid()
+    for item in items:
+        _choice_dict = copy.copy(ARRAY_FIELD_TEMPLATE)
+        if isinstance(item, str):
+            _choice_dict["name"] = item
+        elif isinstance(item, dict):
+            option_name = list(item.keys())[0]
+            option_label = list(item.values())[0]
+            _choice_dict["name"] = option_name
+            _choice_dict["value"] = option_label
+        field_dict["arrayFieldValue"].append(_choice_dict)
     return field_dict
 
 def process_raw_update(field_details, dict, field_mapping):
     dict["required"] = field_details.get("required", False)
-    dict["hint"] = field_details.get("hint", None)
+    dict["hint"] = safe_strip(field_details.get("hint", None))
     dict["formColumnSpan"] = field_details.get("span", 1)
     dict["formStartRow"] = field_details.get("start", False)
     dict["formEndRow"] = field_details.get("end", False)
     dict["textType"] = field_details.get("text_type", "Plain")
     dict["fieldValue"] = field_details.get("default", None)
     dict["fieldRestriction"] = field_details.get("restriction", "No Restriction")
     dict["choiceAllowMultiple"] = field_details.get("allow_multiple", False)
@@ -275,20 +308,36 @@
         set_if_not_equal(field, "name_title", field_json["arrayNameTitle"], None)
         set_if_not_equal(field, "value_title", field_json["arrayValueTitle"], None)
         set_if_not_equal(field, "allow_multiple", field_json["choiceAllowMultiple"], False)
         set_if_not_equal(field, "allow_empty", field_json["choiceAllowEmpty"], False)
         set_if_not_equal(field, "length", field_json["fieldLength"], None)
         set_if_not_equal(field, "max", field_json["intFieldMax"], None)
         set_if_not_equal(field, "min", field_json["intFieldMin"], None)
+
+        if field_json["fieldType"] == "Text":
+            set_if_not_equal(field, "regex", field_json["fieldRegex"], None)
+
+        if field_json["fieldType"] == "Credential":
+            set_if_not_equal(field, "allow_variable", field_json["allowVariable"], False)
+
+        if field_json["fieldType"] == "Array":
+            field["values"] = []
+            for choice in field_json["arrayFieldValue"]:
+                if len(choice.get('value')) > 0:
+                    field["values"].append({f"{choice.get('name')}": f"{choice.get('value')}"})
+                else:
+                    field["values"].append(choice.get('name'))
         
         if field_json["fieldType"] == "Choice":
             field["items"] = []
             for choice in field_json["choices"]:
                 if choice.get('fieldValueLabel') != labelize(choice.get('fieldValue')) and choice.get("useFieldValueForLabel") == False:
-                    field["items"].append({f"{choice.get('fieldValue')}": f"{choice.get('fieldValueLabel')}"})
+                    field["items"].append({f"{choice.get('fieldValue')}": f"{choice.get('fieldValueLabel')}"})     
+                elif choice.get("useFieldValueForLabel"):
+                    field["items"].append({f"{choice.get('fieldValue')}": f"{choice.get('fieldValue')}"})
                 else:
                     field["items"].append(choice.get('fieldValue'))
 
             if len(field_json["choiceFields"]) > 0:
                 field["dependencies"] = []
                 for choice_field in field_json["choiceFields"]:
                     if choice_field is None:
@@ -328,14 +377,18 @@
     set_if_not_equal(result, "template_type", _json["templateType"], None)
     set_if_not_equal(result, "agent_type", _json["agentType"], None)
     set_if_not_equal(result, "extension", _json["extension"], None)
     set_if_not_equal(result, "min_release", _json["minReleaseLevel"], None)
     set_if_not_equal(result, "var_prefix", _json["variablePrefix"], None)
     set_if_not_equal(result, "sys_id", _json["sysId"], None)
     set_if_not_equal(result, "script_ext_windows", _json["scriptTypeWindows"], None)
+    set_if_not_equal(result, "common_script", _json["useCommonScript"], None)
+    set_if_not_equal(result, "always_cancel", _json["alwaysCancelOnFinish"], None)
+    set_if_not_equal(result, "send_environment", _json["sendEnvironment"], None)
+    set_if_not_equal(result, "send_variables", _json["sendVariables"], None)
     result["description"] = "" if _json["description"] is None else _json["description"]  # always show description
     return result
 
 def dump_events(events_json):
     events = []
     if events_json is None:
         return events
@@ -388,14 +441,23 @@
         name = name.replace("-", " ")
         return name.title()
 
 def set_if_not_equal(_var, _field, value, default):
     if value != default:
         _var[_field] = value
 
+def safe_strip(value):
+    if value is None:
+        return value 
+    
+    try:
+        return value.strip()
+    except:
+        return value
+
 def print_code_samples(code_type, name, type=None):
     if code_type == "field":
         if type == "Credential":
             line = ('self.{name} = {{ "user": fields.get("{name}.user", None), "password": fields.get("{name}.password", None) }}'.format(name=name))
         elif type == "Choice":
             line = ("""self.{name} = fields.get("{name}", [None])[0]""".format(name=name))
         elif type == "Boolean":
@@ -410,14 +472,15 @@
         print("""    return ExtensionResult(
     rc = 0,
     message = "Available Fields: '{}'".format(_fields),
     values = _fields
     )""")
 
 FIELD_TEMPLATE = {
+            "arrayFieldValue" : [ ],
             "arrayNameTitle" : None,
             "arrayValueTitle" : None,
             "booleanNoValue" : None,
             "booleanValueType" : "true/false",
             "booleanYesValue" : None,
             "choiceAllowEmpty" : False,
             "choiceAllowMultiple" : False,
@@ -456,7 +519,12 @@
 CHOICE_TEMPLATE = {
                     "fieldValue" : "",
                     "fieldValueLabel" : "",
                     "sequence" : 0,
                     "sysId" : "",
                     "useFieldValueForLabel" : False
                 }
+
+ARRAY_FIELD_TEMPLATE = {
+                    "name" : "",
+                    "value" : ""
+                    }
```

### Comparing `quip-cli-1.8.8/quip/quip.py` & `quip-cli-1.9.0/quip/quip.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 import requests
 from shutil import make_archive, unpack_archive, move
 import tempfile
 from datetime import datetime
 import quip.field_builder as fb
 import quip.version_builder as vb
 import quip.external as external
+from quip.fact import print_greeting
 from argparse import RawTextHelpFormatter
 from quip import __version__, yes_or_no, cprint, choose_one, color_text
 import keyring
 import platform
 
 version = __version__
 UPDATE_ACTION = ["update", "u", "up"]
@@ -46,14 +47,15 @@
 class Quip:
     def __init__(self, log_level=logging.INFO) -> None:
         cprint(f"======= QUIP (v.{version}-BETA) =======", color="cyan")
         logging.basicConfig(level=log_level)
         self.in_project_folder = False
         self.args = self.parse_arguments()
         self.set_global_configs(self.args.name, self.args.config)
+        self.start_time = datetime.now()
 
     def parse_arguments(self):
         parser = argparse.ArgumentParser(description='Wrapper for UIP command.', formatter_class=RawTextHelpFormatter)
         parser.add_argument('--version', action='version', version=f'quip {version}-BETA')
         subparsers = parser.add_subparsers(dest='action')
         parser.add_argument('--config', '-c', default=None,
                              help='path of the global config. Default is ~/.uip_config.yml')
@@ -123,14 +125,17 @@
         parser_clean.add_argument('name', nargs="?", help='name of the project')
         parser_clean.add_argument('--macfilesonly', '-m', action='store_true',
                              help='Delete only MacOS Hidden files like ._* or .DS_Store')
 
         parser_setup = subparsers.add_parser('setup', help='Setup External Systems')
         parser_setup.add_argument('name', nargs="?", help='name of the project')
 
+        parser_setup = subparsers.add_parser('launch', help='Launch Task')
+        parser_setup.add_argument('task_name', help='name of the task')
+
         parser_version = subparsers.add_parser('version', help='shows the version of the template/extension')
         parser_version.add_argument('version_method', nargs="?", choices=["minor", "major", "release", "beta", "rc"], help='update the version of the project. Options: beta,minor,major,release,rc.')
         parser_version.add_argument('--force', dest="forced_version", help='Force to change the version in all possible files')
 
         parser_config = subparsers.add_parser('config', help='show the configuration')
 
         args = parser.parse_args()
@@ -138,15 +143,15 @@
         if args.debug:
             logging.getLogger().setLevel(logging.DEBUG)
 
         if args.action is None:
             parser.print_help()
             sys.exit(0)
         
-        if args.action in ["config", "version"]:
+        if args.action in ["config", "version", "launch"]:
             # give a fake name because name is mandatory
             args.name = ""
         
         if args.action in (["clean"] + CLEAN_ACTION):
             # Ignore project name to clean macfiles
             if args.macfilesonly:
                 args.name = ""
@@ -254,14 +259,16 @@
                     self.rename_build_package(self.curr_version[0])
         elif action == "config":
             if not self.uip_global_config.get("new", False):
                 QuipGlobalConfig().check_config(self.uip_global_config)
             sys.exit(0)
         elif action == "setup":
             self.create_external_systems()
+        elif action == "launch":
+            self.launch_task()
         elif action in CLEAN_ACTION:
             if self.args.macfilesonly:
                 self.delete_macos_hidden_files(".")
             else:
                 self.clean_project()
             sys.exit(0)
         elif action == "version":
@@ -336,15 +343,15 @@
     def update_project(self, update_uuid=False, update_new_uuid=False, new_project=True):
         logging.info(f"Updating extension {self.template_name}")
         if not self.args.template:
             self.update_extension_yaml(self.extension_name, new_project=new_project)
             self.update_uip_config(self.project_name, new_project=new_project)
         else:
             self.update_script_config(self.project_folder_name)
-        self.update_template_json(self.project_name, update_uuid, update_new_uuid)
+        self.update_template_json(self.project_name, update_uuid, update_new_uuid, new_project=new_project)
 
     def update_rename_scripts(self):
         for _script in ["script", "scriptUnix", "scriptWindows"]:
             script_path = self.join_path("src", "templates", _script)
             if os.path.exists(script_path):
                 os.rename(script_path, script_path + ".py")
                 cprint(f"Script renamed: {script_path} => {script_path}.py", "yellow")
@@ -379,14 +386,16 @@
             logging.info(f"Nothing to convert. Put an image file under templates folder and make sure the file name is not 'template_icon.png'")
 
     def create_icon_safe(self, message=None):
         try:
             self.create_icon(message=message)
         except Exception as ex:
             logging.error(f"WARNING: Couldn't create a new ICON")
+            font_name = self._global_conf_defaults.get("icon_font", "cour.ttf")
+            logging.error(f"WARNING: Check the icon_font in the quip config. You may need to install a TrueTypeFont to your system. Current value is {font_name}")
             logging.error(f"Error: {ex}")
             return
 
     def create_icon(self, message=None):
         try:
             from PIL import Image, ImageDraw, ImageFont
         except Exception as ex:
@@ -478,14 +487,16 @@
                     if os.path.exists(original_file_path):
                         os.remove(os.path.join(dir_path, filename))
                     else:
                         logging.info(f"Skipping {filename} (corresponding original file not found)")
             elif os.path.isdir(os.path.join(dir_path, filename)):
                 self.delete_macos_hidden_files(os.path.join(dir_path, filename))
 
+    def launch_task(self):
+        self.run_uip("launch", self.args.task_name)
 
     def clean_project(self, full=True):
         if full:
             folders = ["build", "dist", "temp", "downloads"]
         else:
             folders = ["build", "dist"]
         
@@ -1063,15 +1074,15 @@
         command = subprocess.run(command, shell=True, stderr=subprocess.PIPE, stdout=subprocess.PIPE)
         if command.returncode != 0:
             logging.error("UIP Init command failed.")
             logging.error(f"ERROR: Command is {command}")
             logging.error(f"ERROR: Return code is {command.returncode}")
             sys.exit(command.returncode)
     
-    def run_uip(self, action):
+    def run_uip(self, action, value=None):
         need_pass = False
         uac_url = self._global_conf_uip["url"]
         uac_user = self._global_conf_uip["userid"]
         if action in ["push_all", "push"]:
             additional_params = "-a" if action == "push_all" else ""
             command = f'''uip push {additional_params} -i {uac_url} -u {uac_user}'''
             need_pass = True
@@ -1080,58 +1091,61 @@
             command = f'''uip pull -i {uac_url} -u {uac_user}'''
         elif action == "build":
             need_pass = False
             command = f'''uip build -a'''
         elif action == "clean":
             need_pass = False
             command = f'''uip clean'''
+        elif action == "launch":
+            need_pass = True
+            command = f'''uip task launch "{value}" -i {uac_url} -u {uac_user}'''
 
         if need_pass:
             uac_pass = self.ask_password(uac_url, uac_user)
             os.environ["UIP_PASSWORD"] = uac_pass
         
         logging.info(f"Initializing the extension with command {command}")
         cprint(command, color="yellow")
         result = subprocess.run(command, shell=True, stderr=subprocess.PIPE, stdout=subprocess.PIPE, universal_newlines=True)
         if result.returncode != 0:
             logging.error("UIP command failed.")
             logging.error(f"ERROR: Command is {command}")
             logging.error(f"ERROR: Return code is {command.returncode}")
             sys.exit(command.returncode)
         else:
-            cprint(f"======= UIP Output =======", color="yellow")
+            cprint(f" UIP Output ".center(30, "="), color="yellow")
             for line in result.stdout.splitlines():
                 if line.lower().startswith("success"):
                     cprint(line, color="green")
                 elif line.lower().find("error") > 0:
                     cprint(line, color="red")
                 else:
                     print(line)
-            cprint(f"==============", color="yellow")
+            cprint(f"=" * 30, color="yellow")
     
     def run_git(self, command):
         command = "git " + command
         cprint(command, color="yellow")
         result = subprocess.run(command, shell=True, stderr=subprocess.PIPE, stdout=subprocess.PIPE, universal_newlines=True)
         if result.returncode != 0:
             logging.error("GIT command failed.")
             logging.error(f"ERROR: Command is {command}")
             logging.error(f"ERROR: Return code is {command.returncode}")
             sys.exit(command.returncode)
         else:
             if len(result.stdout) > 0:
-                cprint(f"======= GIT Output =======", color="yellow")
+                cprint(f" GIT Output ".center(30, "="), color="yellow")
                 for line in result.stdout.splitlines():
                     if line.lower().startswith("success"):
                         cprint(line, color="green")
                     elif line.lower().find("error") > 0:
                         cprint(line, color="red")
                     else:
                         print(line)
-                cprint(f"==============", color="yellow")
+                cprint(f"=" * 30, color="yellow")
             
     def rename_build_package(self, version):
         package_folder = self.join_path("dist", "package_build")
         for filename in os.listdir(package_folder):
             if filename.endswith("universal_template.zip"):
                 base_filename = "unv-tmplt-" + os.path.basename(filename).replace("_universal_template.zip", f"-{version}.zip").replace("_", " ")
                 new_filename = os.path.join(os.path.dirname(filename),  base_filename)
@@ -1220,28 +1234,28 @@
                 if update_uuid:
                     logging.info("Updating SysIds in template.json")
                     template_content = self.update_all_sysid_values(template_content)
                 if update_new_uuid:
                     logging.info("Updating new_uuid with a valid SysIds in template.json")
                     template_content = self.update_new_uuid_values(template_content)
             
-            if new_project:
-                with open(template, "w") as f:
-                    _json = json.loads(template_content)
+            with open(template, "w") as f:
+                _json = json.loads(template_content)
+                if new_project:
                     if "extension" in _json and _json["extension"] is not None:
                         _json["extension"] = self.extension_name
                     _json["name"] = self.template_name
                     if "variablePrefix" in _json:
                         if self.args.template:
                             _json["variablePrefix"] = "var"
                         else:
                             _json["variablePrefix"] = self.extension_name.replace("-", "_")
                             if len(_json["variablePrefix"]) > 20:
                                 _json["variablePrefix"] = "ext"
-                    f.write(self.format_json(_json))
+                f.write(self.format_json(_json))
             logging.debug("template.json file is updated")
         else:
             logging.error(f"ERROR: template.json file is missing! Path= {template}")
             sys.exit(1)
     
     def merge_template_scripts(self, project_name):
         logging.info("Merging scripts to template.json file")
@@ -1516,11 +1530,13 @@
 
         if len(self.indents) == 2:
             super().write_line_break()
 
 def run():
     _quip = Quip(log_level=logging.INFO)
     _quip.main()
+    print_greeting(_quip)
 
 if __name__ == '__main__':
     _quip = Quip(log_level=logging.INFO)
     _quip.main()
+    print_greeting(_quip)
```

### Comparing `quip-cli-1.8.8/quip/version_builder.py` & `quip-cli-1.9.0/quip/version_builder.py`

 * *Files identical despite different names*

### Comparing `quip-cli-1.8.8/quip_cli.egg-info/PKG-INFO` & `quip-cli-1.9.0/quip_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quip-cli
-Version: 1.8.8
+Version: 1.9.0
 Summary: Tool for creating/updating new universal integrations
 Author: Stonebranch
 Author-email: huseyin.gomleksizoglu@stonebranch.com
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -542,28 +542,34 @@
   items: []
   dependencies:
   - end_point
   - region
   - credentials
   show_if:
     action: start-batch,sync-start-batch
+    required: true
 
 - application_id: Text
   start: true
   restriction: Output Only
   field_mapping: Text Field 1
   show_if:
     action: start-batch,sync-start-batch
 
 - parameters: Array
   start: true
   name_title: Parameter Name
   value_title: Parameter Value
   field_mapping: Array Field 1
   span: 2
+  values:
+  - task_name
+  - template: Value
+  - variable_1: Value 1
+  - variable_2: Value 2
 
 ```
 
 Format of the child elements are like this.
 
 * First value will be the name of the field and the value of that element will be the type of the field.
 * Field Types can be one of these items
@@ -587,14 +593,15 @@
     * span: If you want the field to fill the row set value to 2. Default: 1
     * text_type: If the text field has YAML or JSON content, set value to YAML or JSON. Default: Plain
     * dynamic: If the field is a dynamic choice field, set the value to true. Default: false
     * restriction: If the field has restrictions like output only, set the value to "Output Only". Default: No Restriction
     * name_title: This field is only for Array types. This field is the label of the first field.
     * value_title: This field is only for Array types. This field is the label of the second field.
     * titles: (alias: headers) This field is another representation of the name_title and value_title fields. You can set the name and value field title in a comma seperated string. For example: `titles: Field Name, Field Value`
+    * values: Default values of an Array field.
     * allow_multiple: This field is only for Choice types. To allow selecting multiple values, set value to true. Default: false
     * allow_empty: This field is only for Choice types. To allow not selecting any value, set value to true. Default: false
     * length: Sets the max lenght of the field.
     * max: Sets the maximum allowed number for that field.
     * min: Set the minimum allowed number for that field.
     
     ### items
```

### Comparing `quip-cli-1.8.8/setup.py` & `quip-cli-1.9.0/setup.py`

 * *Files identical despite different names*

