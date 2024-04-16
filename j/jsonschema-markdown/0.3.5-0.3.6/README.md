# Comparing `tmp/jsonschema_markdown-0.3.5.tar.gz` & `tmp/jsonschema_markdown-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonschema_markdown-0.3.5.tar", max compression
+gzip compressed data, was "jsonschema_markdown-0.3.6.tar", max compression
```

## Comparing `jsonschema_markdown-0.3.5.tar` & `jsonschema_markdown-0.3.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1073 2024-04-11 15:45:33.615499 jsonschema_markdown-0.3.5/LICENSE
--rw-r--r--   0        0        0     2846 2024-04-11 15:45:33.615499 jsonschema_markdown-0.3.5/README.md
--rw-r--r--   0        0        0       81 2024-04-11 15:45:33.615499 jsonschema_markdown-0.3.5/jsonschema_markdown/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 15:45:33.615499 jsonschema_markdown-0.3.5/jsonschema_markdown/converter/__init__.py
--rw-r--r--   0        0        0    13815 2024-04-11 15:45:33.615499 jsonschema_markdown-0.3.5/jsonschema_markdown/converter/markdown.py
--rw-r--r--   0        0        0     1321 2024-04-11 15:45:33.615499 jsonschema_markdown-0.3.5/jsonschema_markdown/main.py
--rw-r--r--   0        0        0     1103 2024-04-11 15:45:33.615499 jsonschema_markdown-0.3.5/jsonschema_markdown/utils.py
--rw-r--r--   0        0        0     1340 2024-04-11 15:45:33.615499 jsonschema_markdown-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     4097 1970-01-01 00:00:00.000000 jsonschema_markdown-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-16 00:37:34.794862 jsonschema_markdown-0.3.6/LICENSE
+-rw-r--r--   0        0        0     3152 2024-04-16 00:37:34.794862 jsonschema_markdown-0.3.6/README.md
+-rw-r--r--   0        0        0       81 2024-04-16 00:37:34.794862 jsonschema_markdown-0.3.6/jsonschema_markdown/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:37:34.794862 jsonschema_markdown-0.3.6/jsonschema_markdown/converter/__init__.py
+-rw-r--r--   0        0        0    15937 2024-04-16 00:37:34.794862 jsonschema_markdown-0.3.6/jsonschema_markdown/converter/markdown.py
+-rw-r--r--   0        0        0     1606 2024-04-16 00:37:34.794862 jsonschema_markdown-0.3.6/jsonschema_markdown/main.py
+-rw-r--r--   0        0        0     1103 2024-04-16 00:37:34.794862 jsonschema_markdown-0.3.6/jsonschema_markdown/utils.py
+-rw-r--r--   0        0        0     1340 2024-04-16 00:37:34.794862 jsonschema_markdown-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     4403 1970-01-01 00:00:00.000000 jsonschema_markdown-0.3.6/PKG-INFO
```

### Comparing `jsonschema_markdown-0.3.5/LICENSE` & `jsonschema_markdown-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonschema_markdown-0.3.5/README.md` & `jsonschema_markdown-0.3.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -21,23 +21,27 @@
 Usage: jsonschema-markdown [OPTIONS] FILENAME
 
   Load FILENAME and output a markdown version.
 
   Use '-' as FILENAME to read from stdin.
 
 Options:
-  -t, --title TEXT          Do not use the title from the schema, use this
-                            title instead.
-  --footer / --no-footer    Add a footer with a link to the project.
-                            [default: footer]
-  --resolve / --no-resolve  [Experimental] Resolve $ref pointers.  [default:
-                            no-resolve]
-  --debug / --no-debug      Enable debug output.  [default: no-debug]
-  --version                 Show the version and exit.
-  --help                    Show this message and exit.
+  -t, --title TEXT                Do not use the title from the schema, use
+                                  this title instead.
+  --footer / --no-footer          Add a footer with a link to the project.
+                                  [default: footer]
+  --empty-columns / --no-empty-columns
+                                  Remove empty columns from the output, useful
+                                  when deprecated or examples are not used.
+                                  [default: empty-columns]
+  --resolve / --no-resolve        [Experimental] Resolve $ref pointers.
+                                  [default: no-resolve]
+  --debug / --no-debug            Enable debug output.  [default: no-debug]
+  --version                       Show the version and exit.
+  --help                          Show this message and exit.
 
 # Example
 $ jsonschema-markdown schema.json > schema.md
 ```
 
 ## Usage with Docker
 The `jsonschema-markdown` command is also available as a Docker image. To use it, you can mount the schema file as a volume.
```

### Comparing `jsonschema_markdown-0.3.5/jsonschema_markdown/converter/markdown.py` & `jsonschema_markdown-0.3.6/jsonschema_markdown/converter/markdown.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,30 +8,68 @@
 from jsonschema_markdown.utils import (
     create_const_markdown,
     create_enum_markdown,
     sort_properties,
 )
 
 
+def _should_include_column(column_values):
+    """
+    Check if any item has a non-falsy (non-empty) value for this column.
+    """
+    return any(value for value in column_values)
+
+
+def _get_schema_header(
+    schema: dict, title_fallback: str, description_fallback: str, nested: bool = False
+) -> str:
+    """
+    Get the title and description of the schema.
+
+    If nested, all headings are increased by one level.
+    """
+
+    prefix = "" if not nested else "#"
+
+    md = ""
+    # Add the title and description of the schema
+    md += f"{prefix}# {schema.get('title', title_fallback)}\n\n"
+    description = schema.get("description", description_fallback).strip(" \n")
+    md += description if description else description_fallback
+    md += "\n\n"
+
+    # Add examples if present
+    examples = schema.get("examples", [])
+    if examples:
+        md += f"{prefix}### Examples\n\n"
+        for example in examples:
+            md += f"```\n{example}\n```\n\n"
+
+    md += f"{prefix}### Type: `{schema.get('type', 'object(?)').strip()}`\n\n"
+
+    return md
+
+
 def generate(
     schema: dict,
     title: str = "jsonschema-markdown",
     footer: bool = True,
     replace_refs: bool = False,
     debug: bool = False,
+    hide_empty_columns: bool = False,
 ) -> str:
     """
     Generate a markdown string from a given JSON schema.
 
-    Parameters:
-        schema (dict): The JSON schema to generate markdown from.
-        title (str, optional): The title of the markdown document. Defaults to "jsonschema-markdown".
-        footer (bool, optional): Whether to include a footer section in the markdown with the current date and time. Defaults to True.
-        replace_refs (bool, optional): This feature is experimental. Whether to replace JSON references with their resolved values. Defaults to False.
-        debug (bool, optional): Whether to print debug messages. Defaults to False.
+    Args:
+        schema: The JSON schema to generate markdown from.
+        title: The title of the markdown document.
+        footer: Whether to include a footer section in the markdown with the current date and time.
+        replace_refs: This feature is experimental. Whether to replace JSON references with their resolved values.
+        debug: Whether to print debug messages.
 
     Returns:
         str: The generated markdown string.
     """
     # Set the log level
     if debug:
         logger.remove()
@@ -45,70 +83,58 @@
 
         _schema: dict = jsonref.replace_refs(schema)  # type: ignore
     else:
         _schema = schema
     markdown = ""
 
     # Add the title and description of the schema
-    markdown += f"# {_schema.get('title', title)}\n\n"
-    description = _schema.get("description", "").strip(" \n")
-    markdown += (
-        f"{description}\n\n"
-        if description
-        else "JSON Schema missing a description, provide it using the `description` key in the root of the JSON document.\n\n"
+    markdown += _get_schema_header(
+        _schema,
+        title,
+        "JSON Schema missing a description, provide it using the `description` key in the root of the JSON document.",
     )
 
-    # Add examples if present
-    examples = _schema.get("examples", [])
-    if examples:
-        markdown += "## Schema Examples\n\n"
-        for example in examples:
-            markdown += f"```\n{example}\n```\n\n"
-
     defs = _schema.get("definitions", _schema.get("$defs", {}))
-    markdown += _create_definition_table(_schema, defs)
+    markdown += _create_definition_table(
+        _schema, defs, hide_empty_columns=hide_empty_columns
+    )
 
     if defs:
         markdown += "\n\n---\n\n# Definitions\n\n"
-
         for key, definition in defs.items():
-            examples = definition.get("examples", [])
-            description = definition.get(
-                "description", "No description provided for this model."
-            ).strip(" \n")
-            markdown += f"\n\n## {definition.get('title', key)}\n\n"
-            markdown += f"{description}\n\n"
-            if examples:
-                markdown += "### Examples\n\n"
-                for example in examples:
-                    markdown += f"```\n{example}\n```\n\n"
-            markdown += f"### Type: `{definition.get('type', 'object(?)').strip()}`\n\n"
-            markdown += _create_definition_table(definition, defs)
+            markdown += _get_schema_header(
+                definition, key, "No description provided for this model.", nested=True
+            )
+            markdown += _create_definition_table(
+                definition, defs, hide_empty_columns=hide_empty_columns
+            )
 
     if footer:
         # Add timestamp and a link to the project
         markdown += "\n\n---\n\nMarkdown generated with [jsonschema-markdown](https://github.com/elisiariocouto/jsonschema-markdown)."
 
     res = markdown.strip(" \n")
     res += "\n"
 
     return res
 
 
-def _create_definition_table(schema: dict, defs: dict) -> str:
+def _create_definition_table(schema: dict, defs: dict, hide_empty_columns: bool) -> str:
     """
     Create a table of the properties in the schema.
-    Outputs a markdown table with the following columns:
+
+    Returns: Markdown table with the following columns
     - Property name
     - Type
     - Required
     - Possible Values / Definition Subschema
     - Deprecated
     - Default value
     - Description
+    - Examples
 
     Search for deprecated string in the description or a deprecated key set to true in the property
     """
 
     logger.debug(f"Creating definition table for schema: {schema}")
 
     if schema.get("enum"):
@@ -126,16 +152,15 @@
         markdown += "> ⚠️ Additional properties are not allowed.\n\n"
 
     if not schema.get("properties"):
         return markdown
 
     schema["properties"] = sort_properties(schema)
 
-    markdown += "| Property | Type | Required | Possible Values | Deprecated | Default | Description | Examples\n"
-    markdown += "| -------- | ---- | -------- | --------------- | ---------- | ------- | ----------- | --------\n"
+    table_items = []
 
     for property_name, property_details in schema["properties"].items():
         property_type = property_details.get("type")
 
         logger.debug(f"Processing {property_name} of type {property_type}")
         logger.debug(f"Property details: {property_details}")
 
@@ -154,33 +179,93 @@
         examples = ", ".join(
             [
                 f"```{str(example)}```"
                 for example in property_details.get("examples", [])
             ]
         )
 
+        item = {
+            "property": property_name,
+            "type": f"`{property_type}`",
+            "required": "✅" if property_name in schema.get("required", []) else "",
+            "possible_values": possible_values,
+            "deprecated": (
+                "⛔️"
+                if "[deprecated]"
+                in str(property_details.get("description", "")).lower()
+                or property_details.get("deprecated")
+                else ""
+            ),
+            "default": "`" + json.dumps(default) + "`" if default else "",
+            "description": description,
+            "examples": examples,
+        }
+        table_items.append(item)
+
+    # This should not happen, but just in case
+    if not table_items:
+        markdown += "No items to display."
+        return markdown
+
+    if hide_empty_columns:
+        always_include_columns = ["property", "type", "required", "description"]
+        # Determine which columns should be included
+        columns = list(table_items[0].keys())
+        include_column = {
+            column: _should_include_column([item[column] for item in table_items])
+            for column in columns
+        }
+
+        # Include the columns that should always be included
+        for column in always_include_columns:
+            include_column[column] = True
+
+        # Generate the header row
+        capitalized_columns = [
+            col.replace("_", " ").capitalize() for col in columns if include_column[col]
+        ]
+        markdown += "| " + " | ".join(capitalized_columns) + " |\n"
+        # Generate the separator row
+        markdown += (
+            "| "
+            + " | ".join(["-" * len(col) for col in columns if include_column[col]])
+            + " |\n"
+        )
+
+        # Generate the item rows
+        for item in table_items:
+            markdown += (
+                "| "
+                + " | ".join([str(item[col]) for col in columns if include_column[col]])
+                + " |\n"
+            )
+    else:
+        # Generate the header row
+        capitalized_columns = [
+            col.replace("_", " ").capitalize() for col in table_items[0]
+        ]
+        markdown += "| " + " | ".join(capitalized_columns) + " |\n"
+
+        # Generate the separator row
         markdown += (
-            f"| {property_name} | "
-            f"`{property_type}` | "
-            f"{'✅' if property_name in schema.get('required', []) else ''} | "
-            f"{possible_values}| "
-            f"{'⛔️' if '[deprecated]' in str(property_details.get('description','')).lower() or property_details.get('deprecated') else ''} | "
-            f"{'`'+json.dumps(default)+'`' if default else ''} | "
-            f"{description} |"
-            f"{examples} |\n"
+            "| " + " | ".join(["-" * len(col) for col in table_items[0]]) + " |\n"
         )
+        # Generate the item rows
+
+        for item in table_items:
+            markdown += "| " + " | ".join(item.values()) + " |\n"
 
     return markdown
 
 
 def _get_property_ref(ref, defs):
     ref = ref.split("/")[-1]
     if ref in defs:
         return (
-            defs[ref].get("type", "object(?)"),
+            defs[ref].get("type", "Missing type"),
             f"[{ref}](#{ref.replace(' ', '-').lower()})",
         )
     else:
         return "Missing type", "Missing definition"
 
 
 def get_property_if_ref(property_details: dict, defs) -> tuple:
```

### Comparing `jsonschema_markdown-0.3.5/jsonschema_markdown/main.py` & `jsonschema_markdown-0.3.6/jsonschema_markdown/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,21 @@
     "--footer/--no-footer",
     is_flag=True,
     default=True,
     show_default=True,
     help="Add a footer with a link to the project.",
 )
 @click.option(
+    "--empty-columns/--no-empty-columns",
+    is_flag=True,
+    default=True,
+    show_default=True,
+    help="Remove empty columns from the output, useful when deprecated or examples are not used.",
+)
+@click.option(
     "--resolve/--no-resolve",
     is_flag=True,
     default=False,
     show_default=True,
     help="[Experimental] Resolve $ref pointers.",
 )
 @click.option(
@@ -35,14 +42,15 @@
     help="Enable debug output.",
 )
 @click.version_option(package_name="jsonschema_markdown")
 def cli(
     filename,
     title,
     footer,
+    empty_columns,
     resolve,
     debug,
 ):
     """
     Load FILENAME and output a markdown version.
 
     Use '-' as FILENAME to read from stdin.
@@ -50,14 +58,15 @@
 
     file_contents = json.loads(filename.read())
 
     kwargs = {
         "footer": footer,
         "replace_refs": resolve,
         "debug": debug,
+        "hide_empty_columns": not empty_columns,
     }
 
     if title:
         kwargs["title"] = title
 
     # Convert the file contents to markdown
     markdown = jsonschema_markdown.generate(file_contents, **kwargs)
```

### Comparing `jsonschema_markdown-0.3.5/jsonschema_markdown/utils.py` & `jsonschema_markdown-0.3.6/jsonschema_markdown/utils.py`

 * *Files identical despite different names*

### Comparing `jsonschema_markdown-0.3.5/pyproject.toml` & `jsonschema_markdown-0.3.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "jsonschema-markdown"
 license = "MIT"
-version = "0.3.5"
+version = "0.3.6"
 description = "Export a JSON Schema document to Markdown documentation."
 authors = ["Elisiário Couto <elisiario@couto.io>"]
 repository = "https://github.com/elisiariocouto/jsonschema-markdown"
 readme = "README.md"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Environment :: Console",
```

### Comparing `jsonschema_markdown-0.3.5/PKG-INFO` & `jsonschema_markdown-0.3.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonschema-markdown
-Version: 0.3.5
+Version: 0.3.6
 Summary: Export a JSON Schema document to Markdown documentation.
 Home-page: https://github.com/elisiariocouto/jsonschema-markdown
 License: MIT
 Keywords: jsonschema,markdown,documentation,docs,json
 Author: Elisiário Couto
 Author-email: elisiario@couto.io
 Requires-Python: >=3.9,<4.0
@@ -51,23 +51,27 @@
 Usage: jsonschema-markdown [OPTIONS] FILENAME
 
   Load FILENAME and output a markdown version.
 
   Use '-' as FILENAME to read from stdin.
 
 Options:
-  -t, --title TEXT          Do not use the title from the schema, use this
-                            title instead.
-  --footer / --no-footer    Add a footer with a link to the project.
-                            [default: footer]
-  --resolve / --no-resolve  [Experimental] Resolve $ref pointers.  [default:
-                            no-resolve]
-  --debug / --no-debug      Enable debug output.  [default: no-debug]
-  --version                 Show the version and exit.
-  --help                    Show this message and exit.
+  -t, --title TEXT                Do not use the title from the schema, use
+                                  this title instead.
+  --footer / --no-footer          Add a footer with a link to the project.
+                                  [default: footer]
+  --empty-columns / --no-empty-columns
+                                  Remove empty columns from the output, useful
+                                  when deprecated or examples are not used.
+                                  [default: empty-columns]
+  --resolve / --no-resolve        [Experimental] Resolve $ref pointers.
+                                  [default: no-resolve]
+  --debug / --no-debug            Enable debug output.  [default: no-debug]
+  --version                       Show the version and exit.
+  --help                          Show this message and exit.
 
 # Example
 $ jsonschema-markdown schema.json > schema.md
 ```
 
 ## Usage with Docker
 The `jsonschema-markdown` command is also available as a Docker image. To use it, you can mount the schema file as a volume.
```

