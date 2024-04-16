# Comparing `tmp/escriptorium-fetcher-0.1.0.tar.gz` & `tmp/escriptorium-fetcher-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "escriptorium-fetcher-0.1.0.tar", max compression
+gzip compressed data, was "escriptorium-fetcher-0.1.1.tar", max compression
```

## Comparing `escriptorium-fetcher-0.1.0.tar` & `escriptorium-fetcher-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1441 2024-02-22 13:50:02.275794 escriptorium-fetcher-0.1.0/README.md
--rw-r--r--   0        0        0       22 2024-02-22 13:23:19.472690 escriptorium-fetcher-0.1.0/escriptorium_fetcher/__init__.py
--rw-r--r--   0        0        0        0 2024-02-22 17:43:34.082810 escriptorium-fetcher-0.1.0/escriptorium_fetcher/__main__.py
--rw-r--r--   0        0        0     7259 2024-02-22 16:45:16.840727 escriptorium-fetcher-0.1.0/escriptorium_fetcher/main.py
--rw-r--r--   0        0        0      507 2024-02-22 14:01:30.104862 escriptorium-fetcher-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2294 2024-02-22 17:50:11.116767 escriptorium-fetcher-0.1.0/setup.py
--rw-r--r--   0        0        0     1909 2024-02-22 17:50:11.116943 escriptorium-fetcher-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1441 2024-04-15 15:34:02.011395 escriptorium-fetcher-0.1.1/README.md
+-rw-r--r--   0        0        0       22 2024-04-15 15:34:02.011395 escriptorium-fetcher-0.1.1/escriptorium_fetcher/__init__.py
+-rw-r--r--   0        0        0     7517 2024-04-16 14:05:26.305437 escriptorium-fetcher-0.1.1/escriptorium_fetcher/main.py
+-rw-r--r--   0        0        0      507 2024-04-16 14:34:11.364801 escriptorium-fetcher-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2294 2024-04-16 14:34:17.869262 escriptorium-fetcher-0.1.1/setup.py
+-rw-r--r--   0        0        0     1909 2024-04-16 14:34:17.869426 escriptorium-fetcher-0.1.1/PKG-INFO
```

### Comparing `escriptorium-fetcher-0.1.0/README.md` & `escriptorium-fetcher-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `escriptorium-fetcher-0.1.0/escriptorium_fetcher/main.py` & `escriptorium-fetcher-0.1.1/escriptorium_fetcher/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import io
 import os 
 import typer
 import srsly
 import getpass
+import requests 
 
 from escriptorium_connector import EscriptoriumConnector
 from pathlib import Path
 from rich import print
 from rich.progress import track
 from typing_extensions import Annotated
 from zipfile import ZipFile
@@ -72,32 +73,35 @@
     # connect to escriptorium
     E = EscriptoriumConnector(
         os.environ.get("ESCRIPTORIUM_URL"),
         os.environ.get("ESCRIPTORIUM_USERNAME"),
         os.environ.get("ESCRIPTORIUM_PASSWORD")
     )
     # get list of projects
-    projects = E.get_projects()
-    project_names = [p.name for p in projects.results]
-    for i, name in enumerate(project_names):
-        print(
-            f"[bold green_yellow]{i}[/bold green_yellow] [bold white]{name}[/bold white]"
-        )
-    project_name = typer.prompt("🐾 Select a project to fetch")
-    # if the user enters a number, use that to select the document
-    if project_name.isdigit():
-        project_pk = projects.results[int(project_name)].id
-        project_slug = projects.results[int(project_name)].slug
-        E.set_connector_project_by_pk(project_pk)
-        print(
-            f"[bold green_yellow] 🦴 Fetching {E.project_name}...[/bold green_yellow]"
-        )
-    else:
-        project_slug = None
-
+    projects = requests.get(f"{os.environ.get('ESCRIPTORIUM_URL')}/api/projects", headers=E.http.headers )
+    if projects.status_code == 200:
+        projects = projects.json()
+        project_results = projects['results']
+        project_names = [p['name'] for p in project_results]
+        for i, name in enumerate(project_names):
+            print(
+                f"[bold green_yellow]{i}[/bold green_yellow] [bold white]{name}[/bold white]"
+            )
+        project_name = typer.prompt("🐾 Select a project to fetch")
+        # if the user enters a number, use that to select the document
+        if project_name.isdigit():
+            proj_name = project_results[int(project_name)]['name']
+            project_slug = project_results[int(project_name)]['slug']
+           
+            print(
+            f"[bold green_yellow] 🦴 Fetching {project_slug}...[/bold green_yellow]"
+            )
+        else:
+            project_slug = None
+    
     # get each document in the project
     documents = E.get_documents()
     documents = [d for d in documents.results if d.project == project_slug]
     # get document parts, images, and transcriptions
     if not no_transcriptions:
         transcriptions = E.get_document_transcriptions(documents[0].pk)
         transcription_names = [t.name for t in transcriptions]
@@ -107,15 +111,15 @@
             )
         selection = typer.prompt("Please select a transcription to fetch")
         # if the user enters a number, use that to select the document
         if selection.isdigit():
             transcription_pk = transcriptions[int(selection)].pk
             transcription_name = transcriptions[int(selection)].name
             print(
-                f"[bold green_yellow] 🐶 Using text from {transcription_name}...[/bold green_yellow]"
+                f"[bold green_yellow] 🐶 Fetching text from {transcription_name}...[/bold green_yellow]"
             )
         else:
             print("Please enter the number of the transcription to fetch 🐩")
 
     for document in documents:
         parts = E.get_document_parts(document.pk)
         for part in track(parts.results, description=f"Downloading {document.name} 🐕‍🦺"):
@@ -157,18 +161,18 @@
                                 ).mkdir(parents=True, exist_ok=True)
                             Path(
                                 str(
                                     os.environ.get("TRANSCRIPTION_PATH")
                                     + "/"
                                     + document.name
                                     + "/"
-                                    + part.name
+                                    + part.filename.split(".")[0]
                                     + ".xml"
                                 )
                             ).write_bytes(transcription)
             except Exception as e:
-                print(f"[bold red]Error[/bold red] {part.name}: {e}")
+                print(f"[bold red]Error[/bold red] {part.title}: {e}")
     print("🦮 All Done 🦮")
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `escriptorium-fetcher-0.1.0/setup.py` & `escriptorium-fetcher-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'typer[all]>=0.9.0,<0.10.0']
 
 entry_points = \
 {'console_scripts': ['fetcher = escriptorium_fetcher.main:app']}
 
 setup_kwargs = {
     'name': 'escriptorium-fetcher',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
     'long_description': '# 🐕 escriptorium-fetcher 🐕\nA CLI for downloading data from an eScriptorium server.\n\n\n### Installation\n```bash\npip install escriptorium-fetcher\n```\n\n### Usage\n```bash\n$ fetcher\n```\nYou will be prompted to select a project to fetch. Enter the number next to the project that you would like to fetch and press enter. For example, if you would like to fetch the first project, enter the following and press enter:\n```bash\n0 initial_batch-2024-02-21\n1 another_project-2024-02-21\n🐾 Select a project to fetch: 0\n```\nBy default, fetcher downloads images and transcriptions. You need to select which transcription you want to download. Enter the number next to the transcription that you would like to fetch and press enter. For example, if you would like to fetch the first transcription, enter the following and press enter:\n```bash\n0 vision\n1 manual\nPlease select a transcription to fetch: 0\n```\n\nThe first time that you run the script you will be prompted to enter:\n- the url of the eScriptorium server\n- your username for the eScriptorium server\n- your password for the eScriptorium server\n- a local path to save the image files\n- a local path to save the transcription files (ALTO xml)\n\nTo clear  your settings and start over, run:\n```bash\n$ fetcher --clear-secrets\n```\nIf you do not want to download images or transcriptions, you can use the `--no-images` or `--no-transcriptions` flags. For example:\n```bash\n$ fetcher --no-images\n```',
     'author': 'apjanco',
     'author_email': 'apjanco@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `escriptorium-fetcher-0.1.0/PKG-INFO` & `escriptorium-fetcher-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: escriptorium-fetcher
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: apjanco
 Author-email: apjanco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: escriptorium-connector (>=0.2.6,<0.3.0)
```

