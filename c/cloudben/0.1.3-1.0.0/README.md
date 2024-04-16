# Comparing `tmp/cloudben-0.1.3.tar.gz` & `tmp/cloudben-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudben-0.1.3.tar", max compression
+gzip compressed data, was "cloudben-1.0.0.tar", max compression
```

## Comparing `cloudben-0.1.3.tar` & `cloudben-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2195 2024-04-15 01:50:36.528860 cloudben-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-04-15 01:50:36.528860 cloudben-0.1.3/cloudben/__init__.py
--rw-r--r--   0        0        0       47 2024-04-15 01:50:36.528860 cloudben-0.1.3/cloudben/__main__.py
--rw-r--r--   0        0        0     6654 2024-04-15 01:50:36.528860 cloudben-0.1.3/cloudben/main.py
--rw-r--r--   0        0        0      463 2024-04-15 01:50:36.528860 cloudben-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2642 1970-01-01 00:00:00.000000 cloudben-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     3504 2024-04-16 02:10:29.226549 cloudben-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-16 02:10:29.226549 cloudben-1.0.0/cloudben/__init__.py
+-rw-r--r--   0        0        0       47 2024-04-16 02:10:29.226549 cloudben-1.0.0/cloudben/__main__.py
+-rw-r--r--   0        0        0     9406 2024-04-16 02:10:29.226549 cloudben-1.0.0/cloudben/main.py
+-rw-r--r--   0        0        0      453 2024-04-16 02:10:29.226549 cloudben-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3941 1970-01-01 00:00:00.000000 cloudben-1.0.0/PKG-INFO
```

### Comparing `cloudben-0.1.3/cloudben/main.py` & `cloudben-1.0.0/cloudben/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,14 +23,18 @@
     content: Annotated[str, typer.Argument(help="value of the Cloudflare record (what the record will resolve to)")],
     type: Annotated[TYPE, typer.Argument(case_sensitive=True, help="type of the Cloudflare record")],
     priority: Annotated[int, typer.Option(
         help="priority of the TXT record", min=0, max=65535)] = 0,
     json: Annotated[bool, typer.Option(
         help="will output valid JSON. It can we useful when using this command in your script. Vanity logging will be disabled")] = False
 ):
+    """
+    Create a DNS records for a specific zone.
+    Example usage: cloudben create-record $zoneid "cloudben" "my-azure-alb.azure.com" CNAME
+    """
 
     token = os.getenv('CF_TOKEN')
     if not token or token == "":
         raise Exception(
             f'CF_TOKEN env variable not found or not initialized, I got: {token}')
 
     headers = {
@@ -63,20 +67,26 @@
         else:
             print(f'Record creted succesfully, {res.text}')
 
 
 @app.command()
 def get_records(
     zone_id: Annotated[str, typer.Argument(help="your zone id")],
-    query: Annotated[str, typer.Option(
-        help="Text to be contained in the record's name.")] = None,
+    name_query: Annotated[str, typer.Option(
+        help="Text to be contained in the record's name.")] = "",
+    content_query: Annotated[str, typer.Option(
+        help="Text to be contained in the record's content.")] = "",
     json: Annotated[bool, typer.Option(
         help="will output valid JSON. It can we useful when using this command in your script. Vanity logging will be disabled")] = False
 ):
-
+    """
+    Get all the DNS records for a specific zone given a query.
+    Example usage: cloudben get-records $zoneid --query "ben" --json
+    """
+    
     token = os.getenv('CF_TOKEN')
     if not token or token == "":
         raise Exception(
             f'CF_TOKEN env variable not found or not initialized, I got: {token}')
 
     headers = {
         'Authorization': f'Bearer {token}'
@@ -84,27 +94,36 @@
 
     res = requests.get(
         f'https://api.cloudflare.com/client/v4/zones/{zone_id}/dns_records', headers=headers)
 
     if res.status_code != 200:
         raise Exception(f'Request failed {res.text}')
 
-    if query == None:
+    if name_query == "" and content_query == "":
         if json:
             print(res.json()['result'])
         else:
             for r in res.json()['result']:
                 print(f'> ({r['id']}) {r['name']}: {r['content']}')
 
-        raise typer.Exit()
 
     matches = []
     for record in res.json()['result']:
-        if query in record['name']:
-            matches.append(record)
+        if name_query != "" and content_query != "":
+            if name_query in record['name'] and content_query in record['content']:
+                matches.append(record)
+                # continue
+
+        elif name_query != "":
+            if name_query in record['name']:
+                matches.append(record)
+
+        elif content_query != "":
+            if content_query in record['content']:
+                matches.append(record)
 
     if json:
         print(matches)
     else:
         for r in matches:
             print(f'> ({r['id']}) {r['name']}: {r['content']}')
 
@@ -112,15 +131,19 @@
 @app.command()
 def delete_record(
     zone_id: Annotated[str, typer.Argument(help="your zone id")],
     record_id: Annotated[str, typer.Argument(help="id of the record to delete")],
     force: Annotated[bool, typer.Option(
         '--force', help="Do not ask for confirmation when deleting.")] = False,
 ):
-
+    """
+    Delete a DNS record given a record id
+    Example usage: cloudben delete-record $zoneid "<record_id>"
+    """
+    
     token = os.getenv('CF_TOKEN')
     if not token or token == "":
         raise Exception(
             f'CF_TOKEN env variable not found or not initialized, I got: {token}')
 
     headers = {
         'Authorization': f'Bearer {token}'
@@ -146,45 +169,66 @@
             raise typer.Abort()
 
     del_res = requests.delete(url=f'https://api.cloudflare.com/client/v4/zones/{
                               zone_id}/dns_records/{record_id}', headers=headers)
 
     if del_res.status_code != 200:
         print(f'Error while deleting the record {del_res.text}')
+        raise typer.Exit(code=1)
     else:
         print(f'Record {res['name']} deleted')
 
 
 @app.command()
 def delete_records(
     zone_id: Annotated[str, typer.Argument(help="your zone id")],
-    query: Annotated[str, typer.Argument(help="Text to be contained in the record's name.")],
+    name_query: Annotated[str, typer.Option(help="Text to be contained in the record's name.")] = "",
+    content_query: Annotated[str, typer.Option(help="Text to be contained in the record's value.")] = "",
     force: Annotated[bool, typer.Option(
         '--force', help="Do not ask for confirmation when deleting.")] = False,
 ):
+    """
+    Delete all the DNS records that match the provided queries. If both --name_query and --content_query are provided the records will match both the criterias (it's an AND not an OR)\n
+    Example usage: cloudben delete-record $zoneid "<record_id>" --name_query "benny"
+    """
 
     token = os.getenv('CF_TOKEN')
     if not token or token == "":
         raise Exception(
             f'CF_TOKEN env variable not found or not initialized, I got: {token}')
 
+    if name_query == "" and content_query == "":
+        raise typer.BadParameter("At least one of --name_query and --content_query must be provided and must not be an empty string.")
+
     headers = {
         'Authorization': f'Bearer {token}'
     }
 
     res = requests.get(
         f'https://api.cloudflare.com/client/v4/zones/{zone_id}/dns_records/', headers=headers)
 
     if res.status_code != 200:
         raise Exception(f'Request failed {res}')
 
     matches = []
     for record in res.json()['result']:
-        if query in record['name']:
-            matches.append(record)
+        if name_query != "" and content_query != "":
+            if name_query in record['name'] and content_query in record['content']:
+                matches.append(record)
+                continue
+
+        elif name_query != "":
+            if name_query in record['name']:
+                matches.append(record)
+            
+            
+        elif content_query != "":
+            if content_query in record['content']:
+                matches.append(record)
+
 
     print("Matched records:")
     for m in matches:
         print(f'> {m['name']}')
 
     print("\n")
     for match in matches:
@@ -199,13 +243,38 @@
                 # raise typer.Abort()
 
         del_res = requests.delete(url=f'https://api.cloudflare.com/client/v4/zones/{
                                   zone_id}/dns_records/{match['id']}', headers=headers)
 
         if del_res.status_code != 200:
             print(f'Error while deleting the record {del_res.text}')
+            raise typer.Exit(code=1)
         else:
             print(f'Record {match['name']} deleted\n')
 
+@app.command()
+def export_records(zone_id: str):
+    """
+    Export DNS records for a specific zone.
+    Example usage: python cloudflare_cli.py export_dns_records --zone_id ZONE_ID
+    """
+    
+    token = os.getenv('CF_TOKEN')
+    if not token or token == "":
+        raise Exception(
+            f'CF_TOKEN env variable not found or not initialized, I got: {token}')
+
+    headers = {
+        'Authorization': f'Bearer {token}'
+    }
+
+    response = requests.get(f"https://api.cloudflare.com/client/v4/zones/{zone_id}/dns_records/export", headers=headers)
+    
+    if response.status_code == 200:
+        typer.echo(response.text)
+    else:
+        typer.echo(f"Error: {response.status_code} - {response.json()['errors'][0]['message']}")
+        raise typer.Exit(code=1)
+
 
 if __name__ == "__main__":
     app()
```

### Comparing `cloudben-0.1.3/PKG-INFO` & `cloudben-1.0.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: cloudben
-Version: 0.1.3
-Summary: Simple CLI tool to interact with the Cloudflare APIs.
-Author: Alberto Gallinaro
-Author-email: alberto.gallinaro@audienceview.com
-Requires-Python: >=3.12,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: typer[all] (>=0.12.3,<0.13.0)
-Description-Content-Type: text/markdown
-
 # `cloudben`
 
 **Usage**:
 
 ```console
 $ cloudben [OPTIONS] COMMAND [ARGS]...
 ```
@@ -23,21 +10,25 @@
 
 * `--install-completion`: Install completion for the current shell.
 * `--show-completion`: Show completion for the current shell, to copy it or customize the installation.
 * `--help`: Show this message and exit.
 
 **Commands**:
 
-* `create-record`
-* `delete-record`
-* `delete-records`
-* `get-records`
+* `create-record`: Create a DNS records for a specific zone.
+* `delete-record`: Delete a DNS record given a record id...
+* `delete-records`: Delete all the DNS records that match the...
+* `export-records`: Export DNS records for a specific zone.
+* `get-records`: Get all the DNS records for a specific...
 
 ## `cloudben create-record`
 
+Create a DNS records for a specific zone.
+Example usage: cloudben create-record $zoneid "cloudben" "my-azure-alb.azure.com" CNAME
+
 **Usage**:
 
 ```console
 $ cloudben create-record [OPTIONS] ZONE_ID NAME CONTENT TYPE:{A|CNAME|AAAA|TXT|MX}
 ```
 
 **Arguments**:
@@ -51,14 +42,17 @@
 
 * `--priority INTEGER RANGE`: priority of the TXT record  [default: 0; 0<=x<=65535]
 * `--json / --no-json`: will output valid JSON. It can we useful when using this command in your script. Vanity logging will be disabled  [default: no-json]
 * `--help`: Show this message and exit.
 
 ## `cloudben delete-record`
 
+Delete a DNS record given a record id
+Example usage: cloudben delete-record $zoneid "<record_id>"
+
 **Usage**:
 
 ```console
 $ cloudben delete-record [OPTIONS] ZONE_ID RECORD_ID
 ```
 
 **Arguments**:
@@ -69,41 +63,68 @@
 **Options**:
 
 * `--force`: Do not ask for confirmation when deleting.
 * `--help`: Show this message and exit.
 
 ## `cloudben delete-records`
 
+Delete all the DNS records that match the provided queries. If both --name_query and --content_query are provided the records will match both the criterias (it's an AND not an OR)
+
+Example usage: cloudben delete-record $zoneid "<record_id>" --name_query "benny"
+
 **Usage**:
 
 ```console
-$ cloudben delete-records [OPTIONS] ZONE_ID QUERY
+$ cloudben delete-records [OPTIONS] ZONE_ID
 ```
 
 **Arguments**:
 
 * `ZONE_ID`: your zone id  [required]
-* `QUERY`: Text to be contained in the record's name.  [required]
 
 **Options**:
 
+* `--name-query TEXT`: Text to be contained in the record's name.
+* `--content-query TEXT`: Text to be contained in the record's value.
 * `--force`: Do not ask for confirmation when deleting.
 * `--help`: Show this message and exit.
 
+## `cloudben export-records`
+
+Export DNS records for a specific zone.
+Example usage: python cloudflare_cli.py export_dns_records --zone_id ZONE_ID
+
+**Usage**:
+
+```console
+$ cloudben export-records [OPTIONS] ZONE_ID
+```
+
+**Arguments**:
+
+* `ZONE_ID`: [required]
+
+**Options**:
+
+* `--help`: Show this message and exit.
+
 ## `cloudben get-records`
 
+Get all the DNS records for a specific zone given a query.
+Example usage: cloudben get-records $zoneid --query "ben" --json
+
 **Usage**:
 
 ```console
 $ cloudben get-records [OPTIONS] ZONE_ID
 ```
 
 **Arguments**:
 
 * `ZONE_ID`: your zone id  [required]
 
 **Options**:
 
-* `--query TEXT`: Text to be contained in the record's name.
+* `--name-query TEXT`: Text to be contained in the record's name.
+* `--content-query TEXT`: Text to be contained in the record's content.
 * `--json / --no-json`: will output valid JSON. It can we useful when using this command in your script. Vanity logging will be disabled  [default: no-json]
 * `--help`: Show this message and exit.
-
```

