# Comparing `tmp/climb-onyx-client-4.1.1.tar.gz` & `tmp/climb_onyx_client-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climb-onyx-client-4.1.1.tar", last modified: Tue Apr  9 12:00:51 2024, max compression
+gzip compressed data, was "climb_onyx_client-4.2.0.tar", last modified: Tue Apr 16 11:16:14 2024, max compression
```

## Comparing `climb-onyx-client-4.1.1.tar` & `climb_onyx_client-4.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:00:51.169333 climb-onyx-client-4.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-09 12:00:40.000000 climb-onyx-client-4.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-09 12:00:51.169333 climb-onyx-client-4.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-04-09 12:00:40.000000 climb-onyx-client-4.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:00:51.169333 climb-onyx-client-4.1.1/climb_onyx_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-09 12:00:51.000000 climb-onyx-client-4.1.1/climb_onyx_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-09 12:00:51.000000 climb-onyx-client-4.1.1/climb_onyx_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 12:00:51.000000 climb-onyx-client-4.1.1/climb_onyx_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-09 12:00:51.000000 climb-onyx-client-4.1.1/climb_onyx_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-09 12:00:51.000000 climb-onyx-client-4.1.1/climb_onyx_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-09 12:00:51.000000 climb-onyx-client-4.1.1/climb_onyx_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:00:51.169333 climb-onyx-client-4.1.1/onyx/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-09 12:00:40.000000 climb-onyx-client-4.1.1/onyx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    68249 2024-04-09 12:00:40.000000 climb-onyx-client-4.1.1/onyx/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    28064 2024-04-09 12:00:40.000000 climb-onyx-client-4.1.1/onyx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-09 12:00:40.000000 climb-onyx-client-4.1.1/onyx/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-09 12:00:40.000000 climb-onyx-client-4.1.1/onyx/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-04-09 12:00:40.000000 climb-onyx-client-4.1.1/onyx/field.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 12:00:40.000000 climb-onyx-client-4.1.1/onyx/version.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 12:00:51.169333 climb-onyx-client-4.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-09 12:00:40.000000 climb-onyx-client-4.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:00:51.169333 climb-onyx-client-4.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    43940 2024-04-09 12:00:40.000000 climb-onyx-client-4.1.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-09 12:00:40.000000 climb-onyx-client-4.1.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-04-09 12:00:40.000000 climb-onyx-client-4.1.1/tests/test_field.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:16:14.711441 climb_onyx_client-4.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-16 11:16:10.000000 climb_onyx_client-4.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-16 11:16:14.711441 climb_onyx_client-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-04-16 11:16:10.000000 climb_onyx_client-4.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:16:14.707441 climb_onyx_client-4.2.0/climb_onyx_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-16 11:16:14.000000 climb_onyx_client-4.2.0/climb_onyx_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-16 11:16:14.000000 climb_onyx_client-4.2.0/climb_onyx_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 11:16:14.000000 climb_onyx_client-4.2.0/climb_onyx_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-16 11:16:14.000000 climb_onyx_client-4.2.0/climb_onyx_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-16 11:16:14.000000 climb_onyx_client-4.2.0/climb_onyx_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-16 11:16:14.000000 climb_onyx_client-4.2.0/climb_onyx_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:16:14.707441 climb_onyx_client-4.2.0/onyx/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-16 11:16:10.000000 climb_onyx_client-4.2.0/onyx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76127 2024-04-16 11:16:10.000000 climb_onyx_client-4.2.0/onyx/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32218 2024-04-16 11:16:10.000000 climb_onyx_client-4.2.0/onyx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-16 11:16:10.000000 climb_onyx_client-4.2.0/onyx/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-16 11:16:10.000000 climb_onyx_client-4.2.0/onyx/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-04-16 11:16:10.000000 climb_onyx_client-4.2.0/onyx/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 11:16:10.000000 climb_onyx_client-4.2.0/onyx/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 11:16:14.711441 climb_onyx_client-4.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-16 11:16:10.000000 climb_onyx_client-4.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:16:14.707441 climb_onyx_client-4.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    50429 2024-04-16 11:16:10.000000 climb_onyx_client-4.2.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-16 11:16:10.000000 climb_onyx_client-4.2.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-04-16 11:16:10.000000 climb_onyx_client-4.2.0/tests/test_field.py
```

### Comparing `climb-onyx-client-4.1.1/LICENSE` & `climb_onyx_client-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `climb-onyx-client-4.1.1/PKG-INFO` & `climb_onyx_client-4.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climb-onyx-client
-Version: 4.1.1
+Version: 4.2.0
 Summary: Client program for interacting with Onyx.
 Home-page: https://github.com/CLIMB-TRE/onyx-client
 Author: Thomas Brier
 Author-email: t.brier@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `climb-onyx-client-4.1.1/README.md` & `climb_onyx_client-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `climb-onyx-client-4.1.1/climb_onyx_client.egg-info/PKG-INFO` & `climb_onyx_client-4.2.0/climb_onyx_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climb-onyx-client
-Version: 4.1.1
+Version: 4.2.0
 Summary: Client program for interacting with Onyx.
 Home-page: https://github.com/CLIMB-TRE/onyx-client
 Author: Thomas Brier
 Author-email: t.brier@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `climb-onyx-client-4.1.1/onyx/api.py` & `climb_onyx_client-4.2.0/onyx/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,28 @@
         "projects": lambda domain: OnyxClient._handle_endpoint(
             lambda: os.path.join(
                 str(domain),
                 "projects/",
             ),
             domain=domain,
         ),
+        "types": lambda domain: OnyxClient._handle_endpoint(
+            lambda: os.path.join(
+                str(domain),
+                "projects/types/",
+            ),
+            domain=domain,
+        ),
+        "lookups": lambda domain: OnyxClient._handle_endpoint(
+            lambda: os.path.join(
+                str(domain),
+                "projects/lookups/",
+            ),
+            domain=domain,
+        ),
         "fields": lambda domain, project: OnyxClient._handle_endpoint(
             lambda: os.path.join(
                 str(domain),
                 "projects",
                 str(project),
                 "fields/",
             ),
@@ -75,14 +89,27 @@
                 "projects",
                 str(project),
                 "query/",
             ),
             domain=domain,
             project=project,
         ),
+        "history": lambda domain, project, climb_id: OnyxClient._handle_endpoint(
+            lambda: os.path.join(
+                str(domain),
+                "projects",
+                str(project),
+                "history",
+                str(climb_id),
+                "",
+            ),
+            domain=domain,
+            project=project,
+            climb_id=climb_id,
+        ),
         "identify": lambda domain, project, field: OnyxClient._handle_endpoint(
             lambda: os.path.join(
                 str(domain),
                 "projects",
                 str(project),
                 "identify",
                 str(field),
@@ -243,19 +270,30 @@
             if name != "domain":
                 for char in "/?":
                     if char in val:
                         raise OnyxClientError(
                             f"Argument '{name}' contains invalid character: '{char}'."
                         )
 
-                # Crude but effective
-                # Prevents calling other endpoints from the get() function with a climb_id equal to the endpoint name
+                # Crude but effective prevention of unexpectedly calling other endpoints
                 # Its not the end of the world if that did happen, but to the user it would be quite confusing
-                if name == "climb_id":
-                    for clash in ["test", "query", "fields", "lookups", "choices"]:
+                clashes = {
+                    "project": ["types", "lookups"],
+                    "climb_id": [
+                        "test",
+                        "query",
+                        "fields",
+                        "choices",
+                        "history",
+                        "identify",
+                    ],
+                }
+
+                if name in clashes:
+                    for clash in clashes[name]:
                         if val == clash:
                             raise OnyxClientError(
                                 f"Argument '{name}' cannot have value '{val}'. This creates a URL that resolves to a different endpoint."
                             )
 
         return endpoint()
 
@@ -385,14 +423,28 @@
     def projects(self) -> requests.Response:
         response = self._request(
             method="get",
             url=OnyxClient.ENDPOINTS["projects"](self.config.domain),
         )
         return response
 
+    def types(self) -> requests.Response:
+        response = self._request(
+            method="get",
+            url=OnyxClient.ENDPOINTS["types"](self.config.domain),
+        )
+        return response
+
+    def lookups(self) -> requests.Response:
+        response = self._request(
+            method="get",
+            url=OnyxClient.ENDPOINTS["lookups"](self.config.domain),
+        )
+        return response
+
     def fields(self, project: str) -> requests.Response:
         response = self._request(
             method="get",
             url=OnyxClient.ENDPOINTS["fields"](self.config.domain, project),
         )
         return response
 
@@ -521,14 +573,25 @@
 
             # Write data
             writer.writeheader()
             writer.writerow(row)
             for row in data_iterator:
                 writer.writerow(row)
 
+    def history(
+        self,
+        project: str,
+        climb_id: str,
+    ) -> requests.Response:
+        response = self._request(
+            method="get",
+            url=OnyxClient.ENDPOINTS["history"](self.config.domain, project, climb_id),
+        )
+        return response
+
     def identify(
         self,
         project: str,
         field: str,
         value: str,
         site: Optional[str] = None,
     ) -> requests.Response:
@@ -895,14 +958,137 @@
         """
 
         response = super().projects()
         response.raise_for_status()
         return response.json()["data"]
 
     @onyx_errors
+    def types(self) -> List[Dict[str, Any]]:
+        """
+        View available field types.
+
+        Returns:
+            List of field types.
+
+        Examples:
+            ```python
+            import os
+            from onyx import OnyxConfig, OnyxEnv, OnyxClient
+
+            config = OnyxConfig(
+                domain=os.environ[OnyxEnv.DOMAIN],
+                token=os.environ[OnyxEnv.TOKEN],
+            )
+
+            with OnyxClient(config) as client:
+                field_types = client.types()
+            ```
+            ```python
+            >>> field_types
+            [
+                {
+                    "type": "text",
+                    "description": "A string of characters.",
+                    "lookups": [
+                        "exact",
+                        "ne",
+                        "in",
+                        "notin",
+                        "contains",
+                        "startswith",
+                        "endswith",
+                        "iexact",
+                        "icontains",
+                        "istartswith",
+                        "iendswith",
+                        "length",
+                        "length__in",
+                        "length__range",
+                        "isnull",
+                    ],
+                },
+                {
+                    "type": "choice",
+                    "description": "A restricted set of options.",
+                    "lookups": [
+                        "exact",
+                        "ne",
+                        "in",
+                        "notin",
+                        "isnull",
+                    ],
+                },
+            ]
+            ```
+        """
+
+        response = super().types()
+        response.raise_for_status()
+        return response.json()["data"]
+
+    @onyx_errors
+    def lookups(self) -> List[Dict[str, Any]]:
+        """
+        View available lookups.
+
+        Returns:
+            List of lookups.
+
+        Examples:
+            ```python
+            import os
+
+            from onyx import OnyxConfig, OnyxEnv, OnyxClient
+
+            config = OnyxConfig(
+                domain=os.environ[OnyxEnv.DOMAIN],
+                token=os.environ[OnyxEnv.TOKEN],
+            )
+
+            with OnyxClient(config) as client:
+                lookups = client.lookups()
+            ```
+            ```python
+            >>> lookups
+            [
+                {
+                    "lookup": "exact",
+                    "description": "The field's value must be equal to the query value.",
+                    "types": [
+                        "text",
+                        "choice",
+                        "integer",
+                        "decimal",
+                        "date",
+                        "datetime",
+                        "bool",
+                    ],
+                },
+                {
+                    "lookup": "ne",
+                    "description": "The field's value must not be equal to the query value.",
+                    "types": [
+                        "text",
+                        "choice",
+                        "integer",
+                        "decimal",
+                        "date",
+                        "datetime",
+                        "bool",
+                    ],
+                },
+            ]
+            ```
+        """
+
+        response = super().lookups()
+        response.raise_for_status()
+        return response.json()["data"]
+
+    @onyx_errors
     def fields(self, project: str) -> Dict[str, Any]:
         """
         View fields for a project.
 
         Args:
             project: Name of the project.
 
@@ -1440,14 +1626,92 @@
         super().to_csv(
             csv_file=csv_file,
             data=data,
             delimiter=delimiter,
         )
 
     @onyx_errors
+    def history(
+        self,
+        project: str,
+        climb_id: str,
+    ) -> Dict[str, Any]:
+        """
+        View the history of a record in a project.
+
+        Args:
+            project: Name of the project.
+            climb_id: Unique identifier for the record in the project.
+
+        Returns:
+            Dict containing the history of the record.
+
+        Examples:
+            ```python
+            import os
+            from onyx import OnyxConfig, OnyxEnv, OnyxClient
+
+            config = OnyxConfig(
+                domain=os.environ[OnyxEnv.DOMAIN],
+                token=os.environ[OnyxEnv.TOKEN],
+            )
+
+            with OnyxClient(config) as client:
+                history = client.history("project", "C-1234567890")
+            ```
+            ```python
+            >>> history
+            {
+                "climb_id": "C-1234567890",
+                "history": [
+                    {
+                        "username": "user",
+                        "timestamp": "2023-01-01T00:00:00Z",
+                        "action": "add",
+                    },
+                    {
+                        "username": "user",
+                        "timestamp": "2023-01-02T00:00:00Z",
+                        "action": "change",
+                        "changes": [
+                            {
+                                "field": "field_1",
+                                "type": "text",
+                                "from": "value1",
+                                "to": "value2",
+                            },
+                            {
+                                "field": "field_2",
+                                "type": "integer",
+                                "from": 3,
+                                "to": 4,
+                            },
+                            {
+                                "field": "nested_field",
+                                "type": "relation",
+                                "action": "add",
+                                "count" : 3,
+                            },
+                            {
+                                "field": "nested_field",
+                                "type": "relation",
+                                "action": "change",
+                                "count" : 10,
+                            },
+                        ],
+                    },
+                ],
+            }
+            ```
+        """
+        response = super().history(project, climb_id)
+        response.raise_for_status()
+        return response.json()["data"]
+
+    @onyx_errors
     def identify(
         self,
         project: str,
         field: str,
         value: str,
         site: Optional[str] = None,
     ) -> Dict[str, str]:
```

### Comparing `climb-onyx-client-4.1.1/onyx/cli.py` & `climb_onyx_client-4.2.0/onyx/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -319,28 +319,110 @@
             )
 
             for column in columns:
                 table.add_column(column)
 
             for project in projects:
                 table.add_row(
-                    project.get("project"),
-                    project.get("scope"),
+                    project.get("project", ""),
+                    project.get("scope", ""),
                     " | ".join(
                         [format_action(action) for action in project.get("actions", [])]
                     ),
                 )
 
             console.print(table)
         else:
             typer.echo(json_dump_pretty(projects))
     except Exception as e:
         handle_error(e)
 
 
+@app.command()
+def types(
+    context: typer.Context,
+    format: Optional[InfoFormats] = typer.Option(
+        InfoFormats.TABLE.value,
+        "-F",
+        "--format",
+        help=HelpText.FORMAT.value,
+    ),
+):
+    """
+    View available field types.
+    """
+
+    try:
+        api = setup_onyx_api(context.obj)
+        types = api.client.types()
+
+        if format == InfoFormats.TABLE:
+            columns = ["Type", "Description", "Lookups"]
+            table = Table(
+                show_lines=True,
+            )
+
+            for column in columns:
+                table.add_column(column)
+
+            for t in types:
+                table.add_row(
+                    t.get("type", ""),
+                    t.get("description", ""),
+                    " | ".join(t.get("lookups", [])),
+                )
+
+            console.print(table)
+        else:
+            typer.echo(json_dump_pretty(types))
+    except Exception as e:
+        handle_error(e)
+
+
+@app.command()
+def lookups(
+    context: typer.Context,
+    format: Optional[InfoFormats] = typer.Option(
+        InfoFormats.TABLE.value,
+        "-F",
+        "--format",
+        help=HelpText.FORMAT.value,
+    ),
+):
+    """
+    View available lookups.
+    """
+
+    try:
+        api = setup_onyx_api(context.obj)
+        lookups = api.client.lookups()
+
+        if format == InfoFormats.TABLE:
+            columns = ["Lookup", "Description", "Types"]
+            table = Table(
+                show_lines=True,
+            )
+
+            for column in columns:
+                table.add_column(column)
+
+            for lookup in lookups:
+                table.add_row(
+                    lookup.get("lookup", ""),
+                    lookup.get("description", ""),
+                    " | ".join(lookup.get("types", [])),
+                )
+
+            console.print(table)
+        else:
+            typer.echo(json_dump_pretty(projects))
+    except Exception as e:
+        handle_error(e)
+
+
 def add_fields_table(
     table: Table, data: Dict[str, Any], prefix: Optional[str] = None
 ) -> None:
     """
     Add fields from the field specification data to the input table.
 
     Works recursively for nested fields.
@@ -356,19 +438,24 @@
         if field_spec.get("default") is not None:
             restrictions.append(f"• Default: {field_spec['default']}")
         if field_spec.get("restrictions"):
             restrictions.extend(
                 f"• {restriction}" for restriction in field_spec["restrictions"]
             )
         if field_spec.get("values"):
-            restrictions.append("• Choices: " + ", ".join(field_spec["values"]))
+            if len(field_spec["values"]) > 20:
+                restrictions.append(
+                    "• Choices: " + ", ".join(field_spec["values"][:20]) + ", ..."
+                )
+            else:
+                restrictions.append("• Choices: " + ", ".join(field_spec["values"]))
 
         table.add_row(
             # Field
-            f"[dim]{prefix}.{field}[/dim]" if prefix else field,
+            ("-" * (prefix.count(".") + 1) + f" {prefix}.{field}" if prefix else field),
             # Status
             (
                 Status.REQUIRED.value
                 if field_spec["required"]
                 else Status.OPTIONAL.value
             ),
             # Type
@@ -524,15 +611,15 @@
         InfoFormats.TABLE.value,
         "-F",
         "--format",
         help=HelpText.FORMAT.value,
     ),
 ):
     """
-    View options for a choice field.
+    View options for a choice field in a project.
     """
 
     try:
         api = setup_onyx_api(context.obj)
         field = parse_extra_option([field])[0]
         choices = api.client.choices(project, field)
 
@@ -723,14 +810,77 @@
                 for record in records:
                     writer.writerow(record)
     except Exception as e:
         handle_error(e)
 
 
 @app.command()
+def history(
+    context: typer.Context,
+    project: str = typer.Argument(...),
+    climb_id: str = typer.Argument(...),
+    format: Optional[InfoFormats] = typer.Option(
+        InfoFormats.TABLE.value,
+        "-F",
+        "--format",
+        help=HelpText.FORMAT.value,
+    ),
+):
+    """
+    View the history of a record in a project.
+    """
+
+    try:
+        api = setup_onyx_api(context.obj)
+        history = api.client.history(project, climb_id)
+
+        if format == InfoFormats.TABLE:
+            columns = ["Username", "Timestamp", "Action", "Changes"]
+
+            table = Table(show_lines=True)
+            for column in columns:
+                table.add_column(column)
+
+            actions = {
+                "add": "added",
+                "change": "changed",
+                "delete": "deleted",
+            }
+
+            for h in history["history"]:
+                changes = []
+                for change in h.get("changes", []):
+                    if change.get("type") == "relation":
+                        action = actions.get(change.get("action", ""), "")
+                        count = change.get("count", "")
+
+                        if count:
+                            count = f"{count} record{'s' if count != 1 else ''}"
+
+                        changes.append(f"• {change['field']}: {action} {count}")
+                    else:
+                        changes.append(
+                            f"• {change['field']}: {change.get('from', '')} → {change.get('to', '')}"
+                        )
+
+                table.add_row(
+                    h.get("username", ""),
+                    h.get("timestamp", ""),
+                    format_action(h.get("action", "")),
+                    "\n".join(changes),
+                )
+
+            console.print(table)
+        else:
+            typer.echo(json_dump_pretty(history))
+    except Exception as e:
+        handle_error(e)
+
+
+@app.command()
 def identify(
     context: typer.Context,
     project: str = typer.Argument(...),
     field: str = typer.Argument(...),
     value: str = typer.Argument(...),
     site: Optional[str] = typer.Option(
         None,
```

### Comparing `climb-onyx-client-4.1.1/onyx/config.py` & `climb_onyx_client-4.2.0/onyx/config.py`

 * *Files identical despite different names*

### Comparing `climb-onyx-client-4.1.1/onyx/exceptions.py` & `climb_onyx_client-4.2.0/onyx/exceptions.py`

 * *Files identical despite different names*

### Comparing `climb-onyx-client-4.1.1/onyx/field.py` & `climb_onyx_client-4.2.0/onyx/field.py`

 * *Files identical despite different names*

### Comparing `climb-onyx-client-4.1.1/setup.py` & `climb_onyx_client-4.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `climb-onyx-client-4.1.1/tests/test_api.py` & `climb_onyx_client-4.2.0/tests/test_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -35,14 +35,64 @@
         {
             "project": PROJECT,
             "action": "view",
             "scope": "base",
         }
     ],
 }
+TYPES_DATA = {
+    "status": "success",
+    "code": 200,
+    "data": [
+        {
+            "type": "text",
+            "description": "A text field.",
+            "lookups": [
+                "exact",
+                "iexact",
+                "contains",
+                "icontains",
+                "startswith",
+                "istartswith",
+                "endswith",
+                "iendswith",
+            ],
+        },
+        {
+            "type": "choice",
+            "description": "A choice field.",
+            "lookups": [
+                "exact",
+                "iexact",
+            ],
+        },
+    ],
+}
+LOOKUPS_DATA = {
+    "status": "success",
+    "code": 200,
+    "data": [
+        {
+            "lookup": "exact",
+            "description": "Exact match.",
+            "types": [
+                "text",
+                "choice",
+            ],
+        },
+        {
+            "lookup": "iexact",
+            "description": "Case-insensitive exact match.",
+            "types": [
+                "text",
+                "choice",
+            ],
+        },
+    ],
+}
 FIELDS_DATA = {
     "status": "success",
     "code": 200,
     "data": {
         "version": "0.1.0",
         "fields": {
             "climb_id": {
@@ -265,14 +315,34 @@
             "published_date": "2023-09-18",
             "sample_id": "sample-123",
             "run_name": "run-456",
         },
     ],
 }
 QUERY_SPECIFIC_BODY = {"&": [{"sample_id": SAMPLE_ID}, {"run_name": RUN_NAME}]}
+HISTORY_DATA = {
+    "status": "success",
+    "code": 200,
+    "data": {
+        "climb_id": CLIMB_ID,
+        "history": [
+            {
+                "username": USERNAME,
+                "timestamp": "2024-01-01T12:00:00Z",
+                "action": "add",
+            },
+            {
+                "username": USERNAME,
+                "timestamp": "2024-01-01T12:00:01Z",
+                "action": "change",
+                "changes": [],
+            },
+        ],
+    },
+}
 IDENTIFY_FIELD = "sample_id"
 IDENTIFY_VALUE = "sample-123"
 IDENTIFY_FIELDS = {"value": IDENTIFY_VALUE}
 IDENTIFY_DATA = {
     "status": "success",
     "code": 200,
     "data": {
@@ -465,15 +535,23 @@
     "data": {
         "username": OTHER_USERNAME,
         "is_approved": True,
     },
 }
 INVALID_DOMAIN_ARGUMENTS = ["", " ", None]
 INVALID_ARGUMENTS = INVALID_DOMAIN_ARGUMENTS + ["/", "?", "/?"]
-CLIMB_ID_ENDPOINT_CLASHES = ["test", "query", "fields", "lookups", "choices"]
+PROJECT_ENDPOINT_CLASHES = ["types", "lookups"]
+CLIMB_ID_ENDPOINT_CLASHES = [
+    "test",
+    "query",
+    "fields",
+    "choices",
+    "history",
+    "identify",
+]
 
 
 class MockResponse:
     def __init__(self, data):
         self.data = data
         self.status_code = data["code"]
         if self.status_code < 400:
@@ -564,14 +642,20 @@
             elif json == IDENTIFY_OTHER_SITE_FIELDS:
                 return MockResponse(IDENTIFY_OTHER_SITE_DATA)
 
     elif method == "get":
         if url == OnyxClient.ENDPOINTS["projects"](DOMAIN):
             return MockResponse(PROJECT_DATA)
 
+        elif url == OnyxClient.ENDPOINTS["types"](DOMAIN):
+            return MockResponse(TYPES_DATA)
+
+        elif url == OnyxClient.ENDPOINTS["lookups"](DOMAIN):
+            return MockResponse(LOOKUPS_DATA)
+
         elif url == OnyxClient.ENDPOINTS["fields"](DOMAIN, PROJECT):
             return MockResponse(FIELDS_DATA)
 
         elif url == OnyxClient.ENDPOINTS["fields"](DOMAIN, NOT_PROJECT):
             return MockResponse(FIELDS_NOT_PROJECT_DATA)
 
         elif url == OnyxClient.ENDPOINTS["fields"](DOMAIN, ERROR_CAUSING_PROJECT):
@@ -601,14 +685,17 @@
 
         elif url == OnyxClient.ENDPOINTS["filter"](DOMAIN, ERROR_CAUSING_PROJECT):
             return MockResponse(FILTER_ERROR_CAUSING_PROJECT_DATA)
 
         elif url == FILTER_PAGE_2_URL:
             return MockResponse(FILTER_PAGE_2_DATA)
 
+        elif url == OnyxClient.ENDPOINTS["history"](DOMAIN, PROJECT, CLIMB_ID):
+            return MockResponse(HISTORY_DATA)
+
         elif url == OnyxClient.ENDPOINTS["profile"](DOMAIN):
             return MockResponse(PROFILE_DATA)
 
         elif url == OnyxClient.ENDPOINTS["waiting"](DOMAIN):
             return MockResponse(WAITING_DATA)
 
         elif url == OnyxClient.ENDPOINTS["siteusers"](DOMAIN):
@@ -671,94 +758,144 @@
             username=USERNAME,
             password=PASSWORD,
         )
         self.client = OnyxClient(self.config)
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_context_manager(self, mock_request):
+        """
+        Test that the OnyxClient can be used as a context manager.
+        """
+
         with OnyxClient(self.config) as client:
             self.assertIsInstance(client._session, requests.Session)
             self.assertEqual(
                 client._request_handler, client._session.request  #  type: ignore
             )
 
         self.assertEqual(client._request_handler, requests.request)
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_connection_error(self, mock_request):
+        """
+        Test that the OnyxClient raises an OnyxConnectionError when a connection error occurs.
+        """
+
         self.config.domain = BAD_DOMAIN
 
         # Non-generator connection error
         with pytest.raises(exceptions.OnyxConnectionError):
             self.client.projects()
 
         # Generator connection error
         with pytest.raises(exceptions.OnyxConnectionError):
             [x for x in self.client.filter(PROJECT)]
 
         self.assertEqual(self.config.token, None)
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_request_error(self, mock_request):
+        """
+        Test that the OnyxClient raises an OnyxRequestError when a request error occurs.
+        """
+
         # Non-generator request error
         with pytest.raises(exceptions.OnyxRequestError) as e:
             self.client.fields(NOT_PROJECT)
         self.assertEqual(e.value.response.json(), FIELDS_NOT_PROJECT_DATA)
 
         # Generator request error
         with pytest.raises(exceptions.OnyxRequestError) as e:
             [x for x in self.client.filter(PROJECT, fields={UNKNOWN_FIELD: "haha"})]
         self.assertEqual(e.value.response.json(), FILTER_UNKNOWN_FIELD_DATA)
 
         self.assertEqual(self.config.token, TOKEN)
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_server_error(self, mock_request):
+        """
+        Test that the OnyxClient raises an OnyxServerError when a server error occurs.
+        """
+
         # Non-generator server error
         with pytest.raises(exceptions.OnyxServerError) as e:
             self.client.fields(ERROR_CAUSING_PROJECT)
         self.assertEqual(e.value.response.json(), FIELDS_ERROR_CAUSING_PROJECT_DATA)
 
         # Generator server error
         with pytest.raises(exceptions.OnyxServerError) as e:
             [x for x in self.client.filter(ERROR_CAUSING_PROJECT)]
         self.assertEqual(e.value.response.json(), FILTER_ERROR_CAUSING_PROJECT_DATA)
 
         self.assertEqual(self.config.token, TOKEN)
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_projects(self, mock_request):
+        """
+        Test that the OnyxClient can retrieve a list of projects.
+        """
+
         self.assertEqual(self.client.projects(), PROJECT_DATA["data"])
         self.assertEqual(self.config.token, TOKEN)
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
+    def test_types(self, mock_request):
+        """
+        Test that the OnyxClient can retrieve a list of field types.
+        """
+
+        self.assertEqual(self.client.types(), TYPES_DATA["data"])
+        self.assertEqual(self.config.token, TOKEN)
+
+    @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
+    def test_lookups(self, mock_request):
+        """
+        Test that the OnyxClient can retrieve a list of lookups.
+        """
+
+        self.assertEqual(self.client.lookups(), LOOKUPS_DATA["data"])
+        self.assertEqual(self.config.token, TOKEN)
+
+    @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_fields(self, mock_request):
+        """
+        Test that the OnyxClient can retrieve the field specification of a project.
+        """
+
         self.assertEqual(self.client.fields(PROJECT), FIELDS_DATA["data"])
         self.assertEqual(self.config.token, TOKEN)
 
         for invalid in INVALID_ARGUMENTS:
             with pytest.raises(exceptions.OnyxClientError):
                 self.client.fields(invalid)
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_choices(self, mock_request):
+        """
+        Test that the OnyxClient can retrieve the choices of a choice field.
+        """
+
         self.assertEqual(
             self.client.choices(PROJECT, CHOICE_FIELD), CHOICES_DATA["data"]
         )
         self.assertEqual(self.config.token, TOKEN)
 
         for invalid in INVALID_ARGUMENTS:
             with pytest.raises(exceptions.OnyxClientError):
                 self.client.choices(invalid, CHOICE_FIELD)
 
             with pytest.raises(exceptions.OnyxClientError):
                 self.client.choices(PROJECT, invalid)
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_get(self, mock_request):
+        """
+        Test that the OnyxClient can retrieve a record from a project.
+        """
+
         self.assertEqual(self.client.get(PROJECT, CLIMB_ID), GET_DATA["data"])
         self.assertEqual(
             self.client.get(
                 PROJECT, fields={"sample_id": SAMPLE_ID, "run_name": RUN_NAME}
             ),
             FILTER_SPECIFIC_DATA["data"][0],
         )
@@ -801,20 +938,28 @@
         for invalid in INVALID_ARGUMENTS:
             with pytest.raises(exceptions.OnyxClientError):
                 self.client.get(invalid, CLIMB_ID)
 
             with pytest.raises(exceptions.OnyxClientError):
                 self.client.get(PROJECT, invalid)
 
+        for clash in PROJECT_ENDPOINT_CLASHES:
+            with pytest.raises(exceptions.OnyxClientError):
+                self.client.get(clash, CLIMB_ID)
+
         for clash in CLIMB_ID_ENDPOINT_CLASHES:
             with pytest.raises(exceptions.OnyxClientError):
                 self.client.get(PROJECT, clash)
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_filter(self, mock_request):
+        """
+        Test that the OnyxClient can filter records from a project.
+        """
+
         self.assertEqual(
             [x for x in self.client.filter(PROJECT)],
             FILTER_PAGE_1_DATA["data"] + FILTER_PAGE_2_DATA["data"],
         )
         self.assertEqual(
             [
                 x
@@ -850,14 +995,18 @@
 
         for invalid in INVALID_ARGUMENTS:
             with pytest.raises(exceptions.OnyxClientError):
                 [x for x in self.client.filter(invalid)]
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_query(self, mock_request):
+        """
+        Test that the OnyxClient can query records from a project.
+        """
+
         self.assertEqual(
             [x for x in self.client.query(PROJECT)],
             QUERY_PAGE_1_DATA["data"] + QUERY_PAGE_2_DATA["data"],
         )
         self.assertEqual(
             [
                 x
@@ -902,18 +1051,50 @@
 
         for invalid in INVALID_ARGUMENTS:
             with pytest.raises(exceptions.OnyxClientError):
                 [x for x in self.client.query(invalid)]
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_to_csv(self, mock_request):
+        """
+        Test that the OnyxClient can convert records to CSV.
+        """
+
         pass  # TODO Test to_csv
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
+    def test_history(self, mock_request):
+        """
+        Test that the OnyxClient can retrieve the history of a record.
+        """
+
+        self.assertEqual(self.client.history(PROJECT, CLIMB_ID), HISTORY_DATA["data"])
+        self.assertEqual(self.config.token, TOKEN)
+
+        for invalid in INVALID_ARGUMENTS:
+            with pytest.raises(exceptions.OnyxClientError):
+                self.client.history(invalid, CLIMB_ID)
+
+            with pytest.raises(exceptions.OnyxClientError):
+                self.client.history(PROJECT, invalid)
+
+        for clash in PROJECT_ENDPOINT_CLASHES:
+            with pytest.raises(exceptions.OnyxClientError):
+                self.client.get(clash, CLIMB_ID)
+
+        for clash in CLIMB_ID_ENDPOINT_CLASHES:
+            with pytest.raises(exceptions.OnyxClientError):
+                self.client.history(PROJECT, clash)
+
+    @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_identify(self, mock_request):
+        """
+        Test that the OnyxClient can identify an anonymised value on a field.
+        """
+
         self.assertEqual(
             self.client.identify(PROJECT, IDENTIFY_FIELD, IDENTIFY_VALUE),
             IDENTIFY_DATA["data"],
         )
         self.assertEqual(
             self.client.identify(
                 PROJECT, IDENTIFY_FIELD, IDENTIFY_VALUE, site=OTHER_SITE
@@ -935,14 +1116,18 @@
                 self.client.identify(PROJECT, invalid, IDENTIFY_VALUE)
 
             with pytest.raises(exceptions.OnyxClientError):
                 self.client.identify(PROJECT, invalid, IDENTIFY_VALUE, site=OTHER_SITE)
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_create(self, mock_request):
+        """
+        Test that the OnyxClient can create a record in a project.
+        """
+
         self.assertEqual(
             self.client.create(PROJECT, CREATE_FIELDS), CREATE_DATA["data"]
         )
         self.assertEqual(
             self.client.create(PROJECT, CREATE_FIELDS, test=True),
             TESTCREATE_DATA["data"],
         )
@@ -953,14 +1138,18 @@
                 self.client.create(invalid, CREATE_FIELDS)
 
             with pytest.raises(exceptions.OnyxClientError):
                 self.client.create(invalid, CREATE_FIELDS, test=True)
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_update(self, mock_request):
+        """
+        Test that the OnyxClient can update a record in a project.
+        """
+
         self.assertEqual(
             self.client.update(PROJECT, CLIMB_ID, UPDATE_FIELDS), UPDATE_DATA["data"]
         )
         self.assertEqual(
             self.client.update(PROJECT, CLIMB_ID, UPDATE_FIELDS, test=True),
             TESTUPDATE_DATA["data"],
         )
@@ -975,32 +1164,44 @@
 
             with pytest.raises(exceptions.OnyxClientError):
                 self.client.update(PROJECT, invalid, UPDATE_FIELDS)
 
             with pytest.raises(exceptions.OnyxClientError):
                 self.client.update(PROJECT, invalid, UPDATE_FIELDS, test=True)
 
+        for clash in PROJECT_ENDPOINT_CLASHES:
+            with pytest.raises(exceptions.OnyxClientError):
+                self.client.get(clash, CLIMB_ID, UPDATE_FIELDS)
+
         for clash in CLIMB_ID_ENDPOINT_CLASHES:
             with pytest.raises(exceptions.OnyxClientError):
                 self.client.update(PROJECT, clash, UPDATE_FIELDS)
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_delete(self, mock_request):
+        """
+        Test that the OnyxClient can delete a record from a project.
+        """
+
         self.assertEqual(self.client.delete(PROJECT, CLIMB_ID), DELETE_DATA["data"])
         self.assertEqual(self.config.token, TOKEN)
 
         for invalid in INVALID_ARGUMENTS:
             with pytest.raises(exceptions.OnyxClientError):
                 self.client.delete(invalid, CLIMB_ID)
 
             with pytest.raises(exceptions.OnyxClientError):
                 self.client.delete(PROJECT, invalid)
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_csv_create(self, mock_request):
+        """
+        Test that the OnyxClient can create records from a CSV file.
+        """
+
         for data, test in [
             (CREATE_DATA["data"], False),
             (TESTCREATE_DATA["data"], True),
         ]:
             self.assertEqual(
                 self.client.csv_create(
                     PROJECT,
@@ -1103,14 +1304,18 @@
                 PROJECT,
                 io.StringIO(TSV_CREATE_MULTI_FILE),
                 delimiter="\t",
             )
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_csv_update(self, mock_request):
+        """
+        Test that the OnyxClient can update records from a CSV file.
+        """
+
         for data, test in [
             (UPDATE_DATA["data"], False),
             (TESTUPDATE_DATA["data"], True),
         ]:
             self.assertEqual(
                 self.client.csv_update(
                     PROJECT,
@@ -1242,14 +1447,18 @@
                 io.StringIO(TSV_UPDATE_MULTI_MISSING_FILE),
                 delimiter="\t",
                 multiline=True,
             )
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_csv_delete(self, mock_request):
+        """
+        Test that the OnyxClient can delete records from a CSV file.
+        """
+
         self.assertEqual(
             self.client.csv_delete(
                 PROJECT,
                 io.StringIO(CSV_DELETE_SINGLE_FILE),
             ),
             DELETE_DATA["data"],
         )
@@ -1304,14 +1513,18 @@
                 PROJECT,
                 io.StringIO(TSV_DELETE_MULTI_FILE),
                 delimiter="\t",
             )
 
     @mock.patch("requests.post", side_effect=mock_register_post)
     def test_register(self, mock_request):
+        """
+        Test that the OnyxClient can register a new user.
+        """
+
         self.assertEqual(
             OnyxClient.register(
                 domain=DOMAIN,
                 first_name=FIRST_NAME,
                 last_name=LAST_NAME,
                 email=EMAIL,
                 site=SITE,
@@ -1329,48 +1542,80 @@
                     email=EMAIL,
                     site=SITE,
                     password=PASSWORD,
                 )
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_login(self, mock_request):
+        """
+        Test that the OnyxClient can login.
+        """
+
         self.assertEqual(self.client.login(), LOGIN_DATA["data"])
         self.assertEqual(self.config.token, TOKEN)
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_logout(self, mock_request):
+        """
+        Test that the OnyxClient can logout.
+        """
+
         self.assertEqual(self.client.logout(), LOGOUT_DATA["data"])
         self.assertEqual(self.config.token, None)
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_logoutall(self, mock_request):
+        """
+        Test that the OnyxClient can logout from all devices.
+        """
+
         self.assertEqual(self.client.logoutall(), LOGOUTALL_DATA["data"])
         self.assertEqual(self.config.token, None)
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_profile(self, mock_request):
+        """
+        Test that the OnyxClient can retrieve the user profile.
+        """
+
         self.assertEqual(self.client.profile(), PROFILE_DATA["data"])
         self.assertEqual(self.config.token, TOKEN)
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_approve(self, mock_request):
+        """
+        Test that the OnyxClient can approve a user.
+        """
+
         self.assertEqual(self.client.approve(OTHER_USERNAME), APPROVE_DATA["data"])
         self.assertEqual(self.config.token, TOKEN)
 
         for invalid in INVALID_ARGUMENTS:
             with pytest.raises(exceptions.OnyxClientError):
                 self.client.approve(invalid)
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_waiting(self, mock_request):
+        """
+        Test that the OnyxClient can retrieve a list of users waiting to be approved.
+        """
+
         self.assertEqual(self.client.waiting(), WAITING_DATA["data"])
         self.assertEqual(self.config.token, TOKEN)
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_site_users(self, mock_request):
+        """
+        Test that the OnyxClient can retrieve a list of users on the site.
+        """
+
         self.assertEqual(self.client.site_users(), SITE_USERS_DATA["data"])
         self.assertEqual(self.config.token, TOKEN)
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_all_users(self, mock_request):
+        """
+        Test that the OnyxClient can retrieve a list of all users.
+        """
+
         self.assertEqual(self.client.all_users(), ALL_USERS_DATA["data"])
         self.assertEqual(self.config.token, TOKEN)
```

### Comparing `climb-onyx-client-4.1.1/tests/test_config.py` & `climb_onyx_client-4.2.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `climb-onyx-client-4.1.1/tests/test_field.py` & `climb_onyx_client-4.2.0/tests/test_field.py`

 * *Files identical despite different names*

