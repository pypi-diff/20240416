# Comparing `tmp/vectara-cli-0.1.9.tar.gz` & `tmp/vectara-cli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectara-cli-0.1.9.tar", last modified: Sun Apr  7 15:46:34 2024, max compression
+gzip compressed data, was "vectara-cli-0.2.0.tar", last modified: Tue Apr 16 20:48:45 2024, max compression
```

## Comparing `vectara-cli-0.1.9.tar` & `vectara-cli-0.2.0.tar`

### file list

```diff
@@ -1,45 +1,68 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 15:46:34.808295 vectara-cli-0.1.9/
--rw-rw-rw-   0        0        0    33954 2024-04-06 18:07:05.000000 vectara-cli-0.1.9/LICENSE.md
--rw-rw-rw-   0        0        0    22546 2024-04-07 15:46:34.806212 vectara-cli-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0    21380 2024-04-07 08:11:24.000000 vectara-cli-0.1.9/README.md
--rw-rw-rw-   0        0        0       42 2024-04-07 15:46:34.808792 vectara-cli-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1428 2024-04-07 15:46:32.000000 vectara-cli-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 15:46:34.770661 vectara-cli-0.1.9/vectara_cli/
--rw-rw-rw-   0        0        0        0 2024-04-05 09:13:47.000000 vectara-cli-0.1.9/vectara_cli/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 15:46:34.780173 vectara-cli-0.1.9/vectara_cli/advanced/
--rw-rw-rw-   0        0        0        0 2024-04-06 18:07:05.000000 vectara-cli-0.1.9/vectara_cli/advanced/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 15:46:34.781673 vectara-cli-0.1.9/vectara_cli/advanced/commercial/
--rw-rw-rw-   0        0        0        0 2024-04-06 18:07:05.000000 vectara-cli-0.1.9/vectara_cli/advanced/commercial/__init__.py
--rw-rw-rw-   0        0        0     7672 2024-04-06 19:42:54.000000 vectara-cli-0.1.9/vectara_cli/advanced/commercial/enterprise.py
-drwxrwxrwx   0        0        0        0 2024-04-07 15:46:34.785188 vectara-cli-0.1.9/vectara_cli/advanced/noncommercial/
--rw-rw-rw-   0        0        0        0 2024-04-05 09:13:47.000000 vectara-cli-0.1.9/vectara_cli/advanced/noncommercial/__init__.py
--rw-rw-rw-   0        0        0     6223 2024-04-06 19:29:01.000000 vectara-cli-0.1.9/vectara_cli/advanced/noncommercial/nerdspan.py
--rw-rw-rw-   0        0        0     9808 2024-04-06 21:57:37.000000 vectara-cli-0.1.9/vectara_cli/advanced/noncommercial/rebel.py
-drwxrwxrwx   0        0        0        0 2024-04-07 15:46:34.801780 vectara-cli-0.1.9/vectara_cli/commands/
--rw-rw-rw-   0        0        0        0 2024-04-06 18:07:05.000000 vectara-cli-0.1.9/vectara_cli/commands/__init__.py
--rw-rw-rw-   0        0        0     4109 2024-04-07 15:24:00.000000 vectara-cli-0.1.9/vectara_cli/commands/create_corpus.py
--rw-rw-rw-   0        0        0      704 2024-04-06 21:50:16.000000 vectara-cli-0.1.9/vectara_cli/commands/delete_corpus.py
--rw-rw-rw-   0        0        0     1575 2024-04-07 14:14:09.000000 vectara-cli-0.1.9/vectara_cli/commands/index_document.py
--rw-rw-rw-   0        0        0      944 2024-04-07 12:31:13.000000 vectara-cli-0.1.9/vectara_cli/commands/index_text.py
--rw-rw-rw-   0        0        0     1131 2024-04-06 21:50:16.000000 vectara-cli-0.1.9/vectara_cli/commands/nerdspan_upsert_folder.py
--rw-rw-rw-   0        0        0      643 2024-04-06 21:50:16.000000 vectara-cli-0.1.9/vectara_cli/commands/query.py
--rw-rw-rw-   0        0        0     1345 2024-04-06 21:50:16.000000 vectara-cli-0.1.9/vectara_cli/commands/rebel_upsert_folder.py
--rw-rw-rw-   0        0        0     1189 2024-04-06 21:50:16.000000 vectara-cli-0.1.9/vectara_cli/commands/span_enhance_folder.py
--rw-rw-rw-   0        0        0      822 2024-04-06 21:50:16.000000 vectara-cli-0.1.9/vectara_cli/commands/span_text.py
--rw-rw-rw-   0        0        0      900 2024-04-06 21:50:16.000000 vectara-cli-0.1.9/vectara_cli/commands/upload_document.py
--rw-rw-rw-   0        0        0      978 2024-04-06 21:50:16.000000 vectara-cli-0.1.9/vectara_cli/commands/upload_enriched_text.py
--rw-rw-rw-   0        0        0      893 2024-04-06 21:50:16.000000 vectara-cli-0.1.9/vectara_cli/config_manager.py
--rw-rw-rw-   0        0        0    17818 2024-04-07 14:24:08.000000 vectara-cli-0.1.9/vectara_cli/core.py
--rw-rw-rw-   0        0        0     1675 2024-04-07 14:22:48.000000 vectara-cli-0.1.9/vectara_cli/corpus_data.py
--rw-rw-rw-   0        0        0      528 2024-04-07 11:57:54.000000 vectara-cli-0.1.9/vectara_cli/custom_dimension.py
--rw-rw-rw-   0        0        0      937 2024-04-07 09:41:11.000000 vectara-cli-0.1.9/vectara_cli/defaults.py
--rw-rw-rw-   0        0        0      506 2024-04-07 11:49:57.000000 vectara-cli-0.1.9/vectara_cli/filter_attribute.py
--rw-rw-rw-   0        0        0     2885 2024-04-07 15:00:09.000000 vectara-cli-0.1.9/vectara_cli/main.py
--rw-rw-rw-   0        0        0      405 2024-04-07 14:58:40.000000 vectara-cli-0.1.9/vectara_cli/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-07 15:46:34.803715 vectara-cli-0.1.9/vectara_cli.egg-info/
--rw-rw-rw-   0        0        0    22546 2024-04-07 15:46:34.000000 vectara-cli-0.1.9/vectara_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1199 2024-04-07 15:46:34.000000 vectara-cli-0.1.9/vectara_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 15:46:34.000000 vectara-cli-0.1.9/vectara_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-04-07 15:46:34.000000 vectara-cli-0.1.9/vectara_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       83 2024-04-07 15:46:34.000000 vectara-cli-0.1.9/vectara_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-07 15:46:34.000000 vectara-cli-0.1.9/vectara_cli.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 20:48:45.224866 vectara-cli-0.2.0/
+-rw-rw-rw-   0        0        0    33954 2024-04-06 18:07:05.000000 vectara-cli-0.2.0/LICENSE.md
+-rw-rw-rw-   0        0        0    32823 2024-04-16 20:48:45.223366 vectara-cli-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    31620 2024-04-16 20:44:42.000000 vectara-cli-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-16 20:48:45.225367 vectara-cli-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1450 2024-04-16 20:43:01.000000 vectara-cli-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 20:48:45.157240 vectara-cli-0.2.0/tests/
+-rw-rw-rw-   0        0        0      344 2024-04-16 20:43:01.000000 vectara-cli-0.2.0/tests/test_LocalVectaraClient.py
+-rw-rw-rw-   0        0        0     2282 2024-04-16 20:43:01.000000 vectara-cli-0.2.0/tests/test_advanced_query.py
+-rw-rw-rw-   0        0        0      738 2024-04-16 20:43:01.000000 vectara-cli-0.2.0/tests/test_command_mapping.py
+-rw-rw-rw-   0        0        0     1000 2024-04-16 20:43:01.000000 vectara-cli-0.2.0/tests/test_config_manager.py
+-rw-rw-rw-   0        0        0     3018 2024-04-16 20:43:01.000000 vectara-cli-0.2.0/tests/test_create_corpus.py
+-rw-rw-rw-   0        0        0     2778 2024-04-16 20:43:01.000000 vectara-cli-0.2.0/tests/test_delete_corpus.py
+-rw-rw-rw-   0        0        0     2971 2024-04-16 20:43:01.000000 vectara-cli-0.2.0/tests/test_index_document.py
+-rw-rw-rw-   0        0        0     1675 2024-04-16 20:43:01.000000 vectara-cli-0.2.0/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2024-04-16 20:48:45.161757 vectara-cli-0.2.0/vectara_cli/
+-rw-rw-rw-   0        0        0        0 2024-04-05 09:13:47.000000 vectara-cli-0.2.0/vectara_cli/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 20:48:45.190822 vectara-cli-0.2.0/vectara_cli/commands/
+-rw-rw-rw-   0        0        0        0 2024-04-06 18:07:05.000000 vectara-cli-0.2.0/vectara_cli/commands/__init__.py
+-rw-rw-rw-   0        0        0     1119 2024-04-16 20:43:01.000000 vectara-cli-0.2.0/vectara_cli/commands/advanced_query.py
+-rw-rw-rw-   0        0        0     2393 2024-04-16 20:43:01.000000 vectara-cli-0.2.0/vectara_cli/commands/create_corpus.py
+-rw-rw-rw-   0        0        0      753 2024-04-16 20:43:01.000000 vectara-cli-0.2.0/vectara_cli/commands/delete_corpus.py
+-rw-rw-rw-   0        0        0      905 2024-04-16 20:43:01.000000 vectara-cli-0.2.0/vectara_cli/commands/index_document.py
+-rw-rw-rw-   0        0        0     1944 2024-04-16 20:43:01.000000 vectara-cli-0.2.0/vectara_cli/commands/index_text.py
+-rw-rw-rw-   0        0        0     1372 2024-04-16 20:43:01.000000 vectara-cli-0.2.0/vectara_cli/commands/nerdspan_upsert_folder.py
+-rw-rw-rw-   0        0        0      806 2024-04-16 20:43:01.000000 vectara-cli-0.2.0/vectara_cli/commands/query.py
+-rw-rw-rw-   0        0        0     1116 2024-04-16 20:43:01.000000 vectara-cli-0.2.0/vectara_cli/commands/rebel_upsert_folder.py
+-rw-rw-rw-   0        0        0     1197 2024-04-16 20:43:01.000000 vectara-cli-0.2.0/vectara_cli/commands/span_enhance_folder.py
+-rw-rw-rw-   0        0        0     1446 2024-04-16 20:43:01.000000 vectara-cli-0.2.0/vectara_cli/commands/span_text.py
+-rw-rw-rw-   0        0        0     3310 2024-04-16 20:43:01.000000 vectara-cli-0.2.0/vectara_cli/commands/specialized_query.py
+-rw-rw-rw-   0        0        0      877 2024-04-16 20:43:01.000000 vectara-cli-0.2.0/vectara_cli/commands/upload_document.py
+-rw-rw-rw-   0        0        0      986 2024-04-16 20:43:01.000000 vectara-cli-0.2.0/vectara_cli/commands/upload_enriched_text.py
+-rw-rw-rw-   0        0        0     1124 2024-04-16 20:43:01.000000 vectara-cli-0.2.0/vectara_cli/commands/upload_folder.py
+-rw-rw-rw-   0        0        0    21061 2024-04-16 20:43:01.000000 vectara-cli-0.2.0/vectara_cli/core.py
+drwxrwxrwx   0        0        0        0 2024-04-16 20:48:45.202855 vectara-cli-0.2.0/vectara_cli/data/
+-rw-rw-rw-   0        0        0        0 2024-04-05 09:13:47.000000 vectara-cli-0.2.0/vectara_cli/data/__init__.py
+-rw-rw-rw-   0        0        0     1889 2024-04-16 20:43:01.000000 vectara-cli-0.2.0/vectara_cli/data/corpus_data.py
+-rw-rw-rw-   0        0        0      771 2024-04-08 12:01:39.000000 vectara-cli-0.2.0/vectara_cli/data/custom_dimension.py
+-rw-rw-rw-   0        0        0     1206 2024-04-08 12:02:19.000000 vectara-cli-0.2.0/vectara_cli/data/defaults.py
+-rw-rw-rw-   0        0        0      506 2024-04-07 11:49:57.000000 vectara-cli-0.2.0/vectara_cli/data/filter_attribute.py
+-rw-rw-rw-   0        0        0      789 2024-04-08 12:29:53.000000 vectara-cli-0.2.0/vectara_cli/data/metadata_handler.py
+-rw-rw-rw-   0        0        0     6362 2024-04-16 20:43:01.000000 vectara-cli-0.2.0/vectara_cli/data/query_request.py
+-rw-rw-rw-   0        0        0     2328 2024-04-16 20:43:01.000000 vectara-cli-0.2.0/vectara_cli/data/query_response.py
+drwxrwxrwx   0        0        0        0 2024-04-16 20:48:45.205852 vectara-cli-0.2.0/vectara_cli/helptexts/
+-rw-rw-rw-   0        0        0        0 2024-04-05 09:13:47.000000 vectara-cli-0.2.0/vectara_cli/helptexts/__init__.py
+-rw-rw-rw-   0        0        0    15202 2024-04-16 20:43:01.000000 vectara-cli-0.2.0/vectara_cli/helptexts/help_text.py
+-rw-rw-rw-   0        0        0     3042 2024-04-16 20:43:01.000000 vectara-cli-0.2.0/vectara_cli/main.py
+drwxrwxrwx   0        0        0        0 2024-04-16 20:48:45.206855 vectara-cli-0.2.0/vectara_cli/rebel_span/
+-rw-rw-rw-   0        0        0        0 2024-04-16 20:43:01.000000 vectara-cli-0.2.0/vectara_cli/rebel_span/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 20:48:45.208860 vectara-cli-0.2.0/vectara_cli/rebel_span/commercial/
+-rw-rw-rw-   0        0        0        0 2024-04-16 20:43:01.000000 vectara-cli-0.2.0/vectara_cli/rebel_span/commercial/__init__.py
+-rw-rw-rw-   0        0        0     6975 2024-04-16 20:43:01.000000 vectara-cli-0.2.0/vectara_cli/rebel_span/commercial/enterprise.py
+drwxrwxrwx   0        0        0        0 2024-04-16 20:48:45.212873 vectara-cli-0.2.0/vectara_cli/rebel_span/noncommercial/
+-rw-rw-rw-   0        0        0       70 2024-04-16 20:43:01.000000 vectara-cli-0.2.0/vectara_cli/rebel_span/noncommercial/__init__.py
+-rw-rw-rw-   0        0        0     7157 2024-04-16 20:43:01.000000 vectara-cli-0.2.0/vectara_cli/rebel_span/noncommercial/nerdspan.py
+-rw-rw-rw-   0        0        0     9808 2024-04-16 20:43:01.000000 vectara-cli-0.2.0/vectara_cli/rebel_span/noncommercial/rebel.py
+drwxrwxrwx   0        0        0        0 2024-04-16 20:48:45.218366 vectara-cli-0.2.0/vectara_cli/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-05 09:13:47.000000 vectara-cli-0.2.0/vectara_cli/utils/__init__.py
+-rw-rw-rw-   0        0        0     1902 2024-04-16 20:43:01.000000 vectara-cli-0.2.0/vectara_cli/utils/config_manager.py
+-rw-rw-rw-   0        0        0      374 2024-04-13 09:44:40.000000 vectara-cli-0.2.0/vectara_cli/utils/create_ui.py
+-rw-rw-rw-   0        0        0      727 2024-04-16 20:43:01.000000 vectara-cli-0.2.0/vectara_cli/utils/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-16 20:48:45.219872 vectara-cli-0.2.0/vectara_cli.egg-info/
+-rw-rw-rw-   0        0        0    32823 2024-04-16 20:48:44.000000 vectara-cli-0.2.0/vectara_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1852 2024-04-16 20:48:45.000000 vectara-cli-0.2.0/vectara_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 20:48:44.000000 vectara-cli-0.2.0/vectara_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-16 20:48:44.000000 vectara-cli-0.2.0/vectara_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       94 2024-04-16 20:48:44.000000 vectara-cli-0.2.0/vectara_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-16 20:48:44.000000 vectara-cli-0.2.0/vectara_cli.egg-info/top_level.txt
```

### Comparing `vectara-cli-0.1.9/LICENSE.md` & `vectara-cli-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.9/PKG-INFO` & `vectara-cli-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectara-cli
-Version: 0.1.9
+Version: 0.2.0
 Summary: A CLI tool for interacting with the Vectara platform, including advanced text processing and indexing features.
 Home-page: https://git.tonic-ai.com/releases/vectara-cli
 Author: Tonic-AI
 Author-email: team@tonic-ai.com
 License: MIT
 Keywords: vectara search-engine document-indexing text-analysis information-retrieval natural-language-processing cli-tool data-science machine-learning text-processing
 Classifier: Programming Language :: Python :: 3
@@ -13,68 +13,252 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: requests
-Provides-Extra: advanced
-Requires-Dist: accelerate; extra == "advanced"
-Requires-Dist: torch>=1.8.0; extra == "advanced"
-Requires-Dist: transformers>=4.5.0; extra == "advanced"
-Requires-Dist: span_marker; extra == "advanced"
-Requires-Dist: spacy; extra == "advanced"
+Requires-Dist: argparse
+Provides-Extra: rebel-span
+Requires-Dist: accelerate; extra == "rebel-span"
+Requires-Dist: torch>=1.8.0; extra == "rebel-span"
+Requires-Dist: transformers>=4.5.0; extra == "rebel-span"
+Requires-Dist: span_marker; extra == "rebel-span"
+Requires-Dist: spacy; extra == "rebel-span"
 
 # vectara-cli
 
 `vectara-cli` is a Python package designed to interact with the Vectara platform, providing a command-line interface (CLI) and a set of APIs for indexing and querying documents, managing corpora, and performing advanced text analysis and processing tasks. This package is particularly useful for developers and data scientists working on search and information retrieval applications.
 
-## Features
+
+#### Features
 
 - Indexing text and documents into Vectara corpora.
 - Querying indexed documents.
 - Creating and deleting corpora.
-- Advanced text processing and analysis using pre-trained models (optional advanced package).
-
-## QuickStart
-
-get started with the [example_notebooks here](https://git.tonic-ai.com/releases/vectara-cli/examples/examples.ipynb) by downloading them and running them locally on any laptop.
+- Advanced text processing and analysis using pre-trained models (optional advanced package(s)).
 
-## Installation
 
 ### Basic Installation
 
 The basic installation includes the core functionality for interacting with the Vectara platform.
 
 ```bash
 pip install vectara-cli
 ```
 
-### Advanced Installation
+#### Advanced Installation
 
 The advanced installation includes additional dependencies for advanced text processing and analysis features. This requires PyTorch, Transformers, and Accelerate, which can be substantial in size.
 
 ```bash
-pip install vectara-cli[advanced]
+pip install vectara-cli[rebel_span]
 ```
 
 Ensure you have an appropriate PyTorch version installed for your system, especially if you're installing on a machine with GPU support. Refer to the [official PyTorch installation guide](https://pytorch.org/get-started/locally/) for more details.
 
-## Command Line Interface (CLI) Usage
+#### Command Line Interface (CLI) Usage
+
+The `vectara-cli` provides a powerful command line interface for interacting with the Vectara platform, enabling tasks such as document indexing, querying, corpus management, and advanced text processing directly from your terminal.
+
+Before your start always set your api keys with :
+
+```bash
+vectara set-api-keys <user_id> <api_key>
+```
+
+#### Deploy Your App
+
+- [x] **`vectara create-ui`:** This command will create a new UI for your app.
+
+**Note:** that this script assumes you have [Node.js and NPM installed](https://nodejs.org/en/download) on your system, as required by the npx command.
+
+<details>
+<summary> Table of Contents </summary>
 
-The `vectara-cli` provides a powerful command line interface for interacting with the Vectara platform, enabling tasks such as document indexing, querying, corpus management, and advanced text processing directly from your terminal. This section will guide you through the basics of using the `vectara-cli`.
+- **[Get started with the example_notebooks here](https://git.tonic-ai.com/releases/vectara-cli/examples/examples.ipynb)**
+- **[More About Configuration](https://git.tonic-ai.com/releases/vectara-cli/-/blob/devbranch/docs/configuration.md)**
+- **[Basic Usage CLI](https://git.tonic-ai.com/releases/vectara-cli/-/blob/devbranch/docs/basic_useage_cli.md?ref_type=heads)**
+- **[Programmatic Usage](https://git.tonic-ai.com/releases/vectara-cli/-/blob/devbranch/docs/basic_usage.md?ref_type=heads)**
+- **[Advanced Usage](https://git.tonic-ai.com/releases/vectara-cli/-/blob/devbranch/docs/advanced_usage.md?ref_type=heads)**
+- **[CONTRIBUTE](https://git.tonic-ai.com/releases/vectara-cli/-/blob/devbranch/CONTRIBUTE.md?ref_type=heads)**
+- **[Testing](https://git.tonic-ai.com/releases/vectara-cli/-/blob/devbranch/tests)**
 
-### Installation
+</details>
 
-Before using the CLI, ensure you have the package installed. You can install it directly from PyPi using pip:
+<details>
+<summary> Get Started </summary>
+
+#### Command Line Interface (CLI) Usage
+
+The `vectara-cli` provides a powerful command line interface for interacting with the Vectara platform, enabling tasks such as document indexing, querying, corpus management, and advanced text processing directly from your terminal.
+
+Before your start always set your api keys with :
 
 ```bash
-pip install vectara-cli
+vectara set-api-keys <user_id> <api_key>
+```
+
+## Basic Usage of Vectara CLI
+
+The Vectara CLI provides a simple and efficient way to interact with the Vectara platform, allowing users to create corpora, index documents, and perform various other operations directly from the command line. This section covers the basic usage of the Vectara CLI for common tasks such as creating a corpus and indexing documents.
+
+### Creating a Corpus
+
+To create a new corpus, you can use the `create-corpus` command. A corpus represents a collection of documents and serves as the primary organizational unit within Vectara.
+
+### Basic Corpus Creation
+
+```bash
+vectara create-corpus <corpus_id> <name> <description>
+```
+
+- `<corpus_id>`: The unique identifier for the corpus. Must be an integer.
+- `<name>`: The name of the corpus. This should be a unique name that describes the corpus.
+- `<description>`: A brief description of what the corpus is about.
+
+#### Example
+
+```bash
+vectara create-corpus 123 "My Corpus" "A corpus containing documents on topic XYZ"
+```
+
+This command creates a basic corpus with the specified ID, name, and description.
+
+### Indexing a Document
+
+To index a document into a corpus, you can use the `index-document` command. This command allows you to add a text document to the specified corpus, making it searchable within the Vectara platform.
+
+### Indexing Text
+
+```bash
+vectara index-text <corpus_id> <document_id> <text> <context> <metadata_json>
+```
+
+- `<corpus_id>`: The unique identifier for the corpus where the document will be indexed.
+- `<document_id>`: A unique identifier for the document being indexed.
+- `<text>`: The actual text content of the document that you want to index.
+- `<context>`: Additional context or information about the document.
+- `<metadata_json>`: A JSON string containing metadata about the document.
+
+#### Example
+
+```bash
+vectara index-text 12345 67890 "This is the text of the document." "Summary of the document" '{"author":"John Doe", "publishDate":"2024-01-01"}'
+```
+
+This command indexes a document with the provided text, context, and metadata into the specified corpus.
+
+### Advanced Corpus Creation
+
+For more advanced scenarios, you might want to specify additional options such as custom dimensions, filter attributes, or privacy settings for your corpus. The `create-corpus-advanced` command allows for these additional configurations.
+
+### Advanced Creation with Options
+
+```bash
+vectara create-corpus-advanced <name> <description> [options]
+```
+
+Options include setting custom dimensions, filter attributes, public/private status, and more.
+
+#### Example
+
+```bash
+vectara create-corpus-advanced "Research Papers" "Corpus for academic research papers" --custom_dimensions '{"dimension1": "value1", "dimension2": "value2"}' --filter_attributes '{"author": "John Doe"}'
+```
+
+This command creates a corpus with custom dimensions and filter attributes specified, allowing for more detailed organization and retrieval capabilities.
+
+### Deleting a Corpus
+
+To remove an existing corpus from the Vectara platform, you can use the `delete-corpus` command. Deleting a corpus will permanently remove the corpus and all documents contained within it. This action cannot be undone, so ensure that you really want to delete the corpus before proceeding.
+
+#### Basic Corpus Deletion
+
+```bash
+vectara delete-corpus <corpus_id>
+```
+
+- `<corpus_id>`: The unique identifier for the corpus you wish to delete. This must be an integer.
+
+#### Example
+
+```bash
+vectara delete-corpus 12345
+```
+
+This command deletes the corpus with the specified ID from the Vectara platform. Upon successful deletion, you will receive a confirmation message. If the corpus cannot be found or if there is an error during the deletion process, an error message will be displayed instead.
+
+### Uploading a Document
+
+To upload a document to a specific corpus in the Vectara platform, you can use the `upload-document` command. This allows you to add various types of documents, such as PDFs, Word documents, and plain text files, making them searchable within your corpus.
+
+#### Basic Document Upload
+
+```bash
+vectara upload-document <corpus_id> <file_path> [document_id]
+```
+
+- `<corpus_id>`: The unique identifier for the corpus where the document will be uploaded. This must be an integer.
+- `<file_path>`: The path to the document file that you want to upload.
+- `[document_id]`: An optional parameter that specifies the document ID. If not provided, Vectara will generate a unique ID for the document.
+
+#### Example
+
+```bash
+vectara upload-document 12345 "/path/to/document.pdf"
+```
+
+This command uploads a document from the specified file path to the corpus with the given ID. If the upload is successful, you will receive a confirmation message along with any relevant details provided by the Vectara platform.
+
+#### Uploading with a Specific Document ID
+
+If you wish to specify a document ID during the upload process, you can include it as an additional argument:
+
+```bash
+vectara upload-document 12345 "/path/to/document.pdf" "custom-document-id-123"
+```
+
+This allows you to assign a custom identifier to the document, which can be useful for tracking or referencing the document within your application or database.
+
+#### Supported Document Formats
+
+Vectara supports a variety of document formats for upload, including but not limited to:
+
+- PDF (.pdf)
+- Microsoft Word (.docx)
+- PowerPoint (.pptx)
+- Plain Text (.txt)
+
+Ensure that your documents are in one of the supported formats before attempting to upload them to the Vectara platform.
+
+#### Metadata and Context
+
+While the basic upload command does not include options for metadata and context, it's important to note that Vectara allows for the association of metadata with documents. This can be accomplished through advanced usage of the Vectara CLI or API, enabling you to provide additional information about the documents you upload, such as author, publication date, tags, and more.
+
+For detailed instructions on advanced document upload options, including how to include metadata and context, please refer to the Vectara documentation or the advanced usage section of the Vectara CLI help.
+
+
+#### Querying
+
+To perform a query in a specific corpus:
+
+```bash
+vectara query "<query_text>" <num_results> <corpus_id>
 ```
 
+- `<query_text>`: The text of the query.
+- `<num_results>`: The maximum number of results to return.
+- `<corpus_id>`: The ID of the corpus to query against.
+
+</details>
+
+<details>
+<summary>  Configuration </summary>
+
 ### Optional: Conda Virtual Environment Setup
 
 Conda is an open-source package management system and environment management system that runs on Windows, macOS, and Linux. It allows you to install, run, and update packages and their dependencies. To set up this project using Conda, follow the steps below:
 
 #### Prerequisites
 
 - Ensure that you have Conda installed on your system. If you do not have Conda installed, you can download it from the [official Conda website](https://www.anaconda.com/products/distribution).
@@ -85,25 +269,23 @@
 2. Navigate to the project directory where the `environment.yml` file is located.
 3. Create a new Conda environment by running the following command:
 
    ```bash
    conda env create -f environment.yml
    ```
 
-   This will create a new environment with the name specified in the `environment.yml` file and install all the required packages.
 
 #### Activating the Environment
 
 Once the environment is created, you can activate it using the following command:
 
 ```bash
-conda activate <env_name>
+conda activate vectara
 ```
 
-Replace `<env_name>` with the name of your Conda environment.
 
 #### Deactivating the Environment
 
 When you are done working on the project, you can deactivate the Conda environment by running:
 
 ```bash
 conda deactivate
@@ -120,19 +302,17 @@
 This will update the environment with any new dependencies specified in the `environment.yml` file.
 
 #### Removing the Environment
 
 If you wish to remove the Conda environment, you can do so with the following command:
 
 ```bash
-conda env remove -n <env_name>
+conda env remove -n vectara
 ```
 
-Again, replace `<env_name>` with the name of your Conda environment.
-
 By following these steps, you can manage your project's dependencies in an isolated environment using Conda.
 
 ### Configuration
 
 #### Setting Credentials via CLI Commands
 
 The `vectara-cli` tool now supports a convenient feature for setting your Vectara customer ID and API key directly through the command line. This method utilizes a command specifically designed for securely storing your credentials, making it easier to manage your Vectara configuration without manually setting environment variables or directly embedding your credentials in your scripts.
@@ -140,23 +320,23 @@
 #### Using the `set-api-keys` Command
 
 To set your Vectara customer ID and API key using the `vectara-cli`, you can use the `set-api-keys` command. This command stores your credentials securely, allowing `vectara-cli` to automatically use them for authentication in future operations.
 
 - **Syntax:** The command follows this simple syntax:
 
 ```bash
-vectara-cli set-api-keys <customer_id> <api_key>
+vectara set-api-keys <customer_id> <api_key>
 ```
 
 Replace `<customer_id>` with your Vectara customer ID and `<api_key>` with your Vectara API key.
 
 - **Example:**
 
 ```bash
-vectara-cli set-api-keys 123456789 abcdefghijklmnopqrstuvwxyz
+vectara set-api-keys 123456789 abcdefghijklmnopqrstuvwxyz
 ```
 
 After executing this command, you will see a confirmation message indicating that your API keys have been set successfully.
 
 #### Windows
 
 For Windows users, you can also set environment variables through the Command Prompt or PowerShell, or via the System Properties window.
@@ -177,67 +357,19 @@
 
 Note that changes made through the command line will only take effect in new instances of the terminal or command prompt.
 
 #### Using Credentials in `vectara-cli`
 
 Once you have set up your environment variables, `vectara-cli` will automatically use these credentials for authentication. There's no need to manually input your customer ID and API key each time you execute a command.
 
-### Basic Commands
-
+</details>
 
-#### Indexing a Document
+<details>
+<summary> Programmatic Usage </summary>
 
-To index a document into a specific corpus:
-
-```bash
-vectara-cli index-document <corpus_id> <document_id> "<title>" '<metadata_json>' "<section_text>"
-```
-
-- `<corpus_id>`: The ID of the corpus where the document will be indexed.
-- `<document_id>`: A unique identifier for the document.
-- `<title>`: The title of the document.
-- `<metadata_json>`: A JSON string containing document metadata.
-- `<section_text>`: The text content of the document.
-
-#### Querying
-
-To perform a query in a specific corpus:
-
-```bash
-vectara-cli query "<query_text>" <num_results> <corpus_id>
-```
-
-- `<query_text>`: The text of the query.
-- `<num_results>`: The maximum number of results to return.
-- `<corpus_id>`: The ID of the corpus to query against.
-
-#### Creating a Corpus
-
-To create a new corpus:
-
-```bash
-vectara-cli create-corpus <corpus_id> "<name>"
-```
-
-- `<corpus_id>`: The ID for the new corpus.
-- `<name>`: The name of the new corpus.
-
-#### Deleting a Corpus
-
-To delete an existing corpus:
-
-```bash
-vectara-cli delete-corpus <corpus_id>
-```
-
-- `<corpus_id>`: The ID of the corpus to delete.
-
-### Advanced Commands
-
-### Basic Usage
 
 #### Setting Up a Vectara Client
 
 First, initialize the Vectara client with your customer ID and API key. This client will be used for all subsequent operations.
 
 ```python
 from vectara_cli.core import VectaraClient
@@ -286,41 +418,14 @@
 num_results = 10  # Number of results to return
 corpus_id = 'your_corpus_id'
 
 results = vectara_client.query(query_text, num_results, corpus_id)
 print(results)
 ```
 
-#### Creating a Corpus
-
-You can create a new corpus by specifying its ID, name, description, and other settings.
-
-```python
-create_corpus_response = vectara_client.create_corpus(
-    corpus_id=123456789,
-    name="Example Corpus",
-    description="This is an example corpus.",
-    dtProvision=1234567890,
-    enabled=True,
-    swapQenc=False,
-    swapIenc=False,
-    textless=False,
-    encrypted=False,
-    encoderId="default",
-    metadataMaxBytes=10000,
-    customDimensions=[
-        {"name": "dimension1", "description": "First custom dimension", "servingDefault": 1.0, "indexingDefault": 1.0}
-    ],
-    filterAttributes=[
-        {"name": "filter1", "description": "First filter attribute", "indexed": True, "type": "FILTER_ATTRIBUTE_TYPE__UNDEFINED", "level": "FILTER_ATTRIBUTE_LEVEL__UNDEFINED"}
-    ]
-)
-print(create_corpus_response)
-```
-
 #### Deleting a Corpus
 
 To delete a corpus, you only need to provide its ID.
 
 ```python
 corpus_id = 'your_corpus_id'
 response, success = vectara_client.delete_corpus(corpus_id)
@@ -344,41 +449,47 @@
 try:
     response, status = vectara_client.upload_document(corpus_id, file_path, document_id, metadata)
     print("Upload successful:", response)
 except Exception as e:
     print("Upload failed:", str(e))
 ```
 
+</details>
+
+<details>
+<summary> Advanced Usage </summary>
+
+
 ### Advanced Usage
 
 
 To leverage the advanced text processing capabilities, ensure you have completed the advanced installation of `vectara-cli`. This includes the necessary dependencies for text analysis:
 
 ```bash
-pip install vectara-cli[advanced]
+pip install vectara-cli[rebel_span]
 ```
 
 #### Span Text Processing
 
 To process text using the Span model:
 
 ```bash
-vectara-cli span-text "<text>" "<model_name>" "<model_type>"
+vectara span-text "<text>" "<model_name>" "<model_type>"
 ```
 
 - `<text>`: The text to process.
 - `<model_name>`: The name of the Span model to use.
 - `<model_type>`: The type of the Span model.
 
 #### Enhanced Batch Processing with NerdSpan
 
 To process and upload documents from a folder:
 
 ```bash
-vectara-cli nerdspan-upsert-folder "<folder_path>" "<model_name>" "<model_type>"
+vectara nerdspan-upsert-folder "<folder_path>" "<model_name>" "<model_type>"
 ```
 
 - `<folder_path>`: The path to the folder containing documents to process and upload.
 - `<model_name>`: The name of the model to use for processing.
 - `<model_type>`: The type of the model.
 
 For more advanced processing and upsert operations, including using the Rebel model for complex document analysis and upload, refer to the specific command documentation provided with the CLI.
@@ -396,28 +507,28 @@
 >> **- supported models:** `science` and `keyphrase`
 
 - **Upload Enriched Text**
 
   To upload text that has been enriched with additional metadata:
 
   ```bash
-  vectara-cli upload-enriched-text <corpus_id> <document_id> <model_name> "<text>"
+  vectara upload-enriched-text <corpus_id> <document_id> <model_name> "<text>"
   ```
 
   - `<corpus_id>`: The ID of the corpus where the document will be uploaded.
   - `<document_id>`: A unique identifier for the document.
   - `<model_name>`: The name of the model used for text enrichment. `science` or `keyphrase`
   - `<text>`: The text content to be enriched and uploaded.
 
 - **Span Enhance Folder**
 
   To process and upload all documents within a folder, enhancing them using a specified model:
 
   ```bash
-  vectara-cli span-enhance-folder <corpus_id_1> <corpus_id_2> <model_name> "<folder_path>"
+  vectara span-enhance-folder <corpus_id_1> <corpus_id_2> <model_name> "<folder_path>"
   ```
 
   - `<corpus_id_1>`: The ID for the corpus to upload plain text documents.
   - `<corpus_id_2>`: The ID for the corpus to upload enhanced text documents.
   - `<model_name>`: The name of the model used for document enhancement. **supported models :** `science` and `keyphrase`
   - `<folder_path>`: The path to the folder containing the documents to be processed.
 
@@ -457,15 +568,15 @@
 This example showcases how to enrich text with additional metadata using the `EnterpriseSpan` class and upload it to a specified corpus in Vectara. By leveraging advanced models for text processing, users can significantly enhance the quality and relevance of their search and retrieval operations on the Vectara platform.
 
 ### Non-Commercial Advanced Usage
 
 The advanced features allow you to enrich your indexes with additional information automatically. This should produce better results for retrieval.
 
 
-![The mRebel pre-trained model is able to extract triplets for up to 400 relation types from Wikidata](https://git.tonic-ai.com/releases/vectara-cli/res/images/image.png?ref_type=heads)
+![Span Models for Named Entity Recognition](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/image.png?ref_type=heads)
 
 ### Non-Commercial Advanced Usage Using Span Models
 
 The `vectara-cli` package extends its functionality through the advanced usage of Span Models, enabling users to perform sophisticated text analysis and entity recognition tasks. This feature is particularly beneficial for non-commercial applications that require deep understanding and processing of textual data.
 
 The `Span` class supports processing and indexing documents from a folder, enabling batch operations for efficiency. This feature allows for the automatic extraction of entities from multiple documents, which are then indexed into specified corpora with enriched metadata.
 
@@ -517,16 +628,17 @@
     vectara_client.index_text(corpus_id, document_id, text, metadata_json=metadata_json)
     ```
 
 **Reference:** Aarsen, T. (2023). SpanMarker for Named Entity Recognition. Radboud University. Supervised by Prof. Dr. Fermin Moscoso del Prado Martin (fermin.moscoso-del-prado@ru.nl) and Dr. Daniel Vila Suero (daniel@argilla.io). Second assessor: Dr. Harrie Oosterhuis (harrie.oosterhuis@ru.nl).
 
 #### Non-Commercial Advanced Rag Using Rebel
 
-![mRebel](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/Screenshot_2024-04-05_112158.png?ref_type=heads)
-![Span Models for Named Entity Recognition](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/Screenshot_2024-04-05_112142.png?ref_type=heads)
+![mRebel](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/Screenshot_2024-04-05_112158.png)
+
+![The mRebel pre-trained model is able to extract triplets for up to 400 relation types from Wikidata](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/Screenshot_2024-04-05_112142.png)
 
 The mRebel pre-trained model is able to extract triplets for up to 400 relation types from Wikidata.
 
 
 Use the use the `Rebel Class` for advanced indexing. This will automatically extract `named entities`, `key phrases`, and other relevant information from your documents : 
 
 
@@ -554,23 +666,148 @@
     print(f"Document ID: {result['documentIndex']}, Score: {result['score']}, Text: {result['text'][:100]}...")
 
 print("\n=== Enhanced Results ===")
 for result in enhanced_results:
     print(f"Document ID: {result['documentIndex']}, Score: {result['score']}, Text: {result['text'][:100]}...")
 ```
 
-## Contributing
+</details>
+
+<details>
+<summary> Contributing </summary>
+
+# Contributing Guidelines for vectara-cli
+
+Thank you for your interest in contributing to `vectara-cli`! As an open-source project, we welcome contributions from developers of all skill levels. This guide will provide you with information on how to contribute effectively and make a valuable impact on the project.
+
+## Prerequisites
+
+Before you begin, ensure you have the following installed:
+
+- Python (preferably the latest Python 3 version)
+- Conda (for managing environments)
+- Git (for version control)
 
-Contributions to `vectara-cli` are welcome! Please refer to the contributing guidelines in the repository for more information on how to contribute.
+## Identify An Issue
 
+Browse the [Issues](https://git.tonic-ai.com/contribute/vectara/vectara-cli/issues) to find tasks to work on. You can start with issues labeled as "good first issue".
+- If you have an idea or a bug fix that is not listed, feel free to open a new issue to discuss it with other contributors.
 
-### Contributing to Advanced Features
+## Setting Up for Contribution
+
+1. **Fork the Repository**: Visit [vectara-cli on GitLab](https://git.tonic-ai.com/contribute/vectara/vectara-cli/) and fork the project to your account.
+
+2. **Create a New Branch**: Before you start making changes, switch to the `devbranch` and create a new branch for your feature or fix. We encourage naming your branch in a way that reflects the issue or feature you're working on.
+
+    ```bash
+    git checkout devbranch
+    git checkout -b feature/your-feature-name
+    ```
+    Or, if you're working on a specific issue:
+
+    ```bash
+    git checkout devbranch
+    git checkout -b issue/ISSUE_NUMBER-short-description
+    ```
 
-We welcome contributions to improve and expand the advanced features of `vectara-cli`. Whether it's adding new models, enhancing existing functionalities, or fixing bugs, your contributions are valuable to us. Please refer to our contributing guidelines for more information on how to contribute.
+    This naming convention (`feature/your-feature-name` or `issue/ISSUE_NUMBER-short-description`) helps in identifying branches with their purposes, making collaboration and review processes more efficient.
+
+- the easiest way to make a correctly named branch is to use the gitlab gui directly inside the issue that you are responding to.
+
+![easily use the GUI to make a branch](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/contributingimage.png)
+
+
+3. **Create and Activate Conda Environment**:
+
+   ```bash
+   conda env create -f environment.yml
+   conda activate vectara-cli
+   ```
+
+4. **Install the Project in Editable Mode**:
+
+   ```bash
+   pip install --editable .
+   ```
 
-## License
+## Develop
 
-`vectara-cli` is MIT licensed. See the [LICENSE](LICENSE.md) file for more details.
+- **Add Functionality**: Write your code and add it to the appropriate directory:
+  - For new functionalities, add your code in `./vectara_cli/commands`.
+  - Add command line functionality in `main.py`.
+  - Create or modify data objects in `./vectara_cli/data`.
 
----
+- **Add Help Text**: Update help texts in `./vectara_cli/help_texts/help_text.py` to reflect your changes or new commands.
 
-This README provides a comprehensive guide for installing and using the `vectara-cli` package. For further information or assistance, please refer to the [Vectara documentation](https://docs.vectara.com) or submit an issue on the [GitLab repository](https://git.tonic-ai.com/releases/vectara-cli/).
+## Write Tests
+
+- Add tests for your new functionalities in the `tests/` directory.
+- Ensure all tests pass by running them locally.
+
+## Document Your Changes
+
+Update any documentation relevant to your changes, including inline comments and README if necessary.
+
+## Submitting Your Contributions
+
+1. **Commit Your Changes**: After making your changes, commit them to your branch. Use descriptive commit messages that explain the "why" and "what" of your changes. This practice helps reviewers understand your reasoning and the context of your contributions.
+
+    ```bash
+    git add .
+    git commit -m "A descriptive message explaining the change"
+    ```
+
+2. **Push Your Changes**: Once you're ready, push your changes to your forked repository on GitLab.
+
+    ```bash
+    git push origin feature/your-feature-name
+    ```
+    
+    Or, if you're working on an issue:
+
+    ```bash
+    git push origin issue/ISSUE_NUMBER-short-description
+    ```
+
+### 3. Create a Merge Request
+- Go to the [Merge Requests](https://git.tonic-ai.com/contribute/vectara/vectara-cli/-/merge_requests) page.
+- Create a new merge request, compare your feature branch to the main repository's `devbranch`.
+- Fill in a detailed description of your changes and link to any relevant issues.
+
+## Review Process
+Once your merge request is submitted:
+- The project maintainers will review your code and may request changes.
+- Collaborate on modifications and push updates to your branch accordingly.
+- Once approved, a maintainer will merge your changes into the main codebase.
+
+## Post-merge
+After your changes have been merged:
+- Sync your fork with the original repository.
+- Consider deleting your branch to keep your fork clean:
+  ```bash
+  git branch -d your-feature-branch
+  git push origin --delete your-feature-branch
+  ```
+
+Thank you for contributing to `vectara-cli`! For any questions or further discussions, please reach out on the issues page or [on discord](https://discord.gg/7H4SKQekKe).
+
+- **[CONTRIBUTE](https://git.tonic-ai.com/releases/vectara-cli/-/blob/devbranch/CONTRIBUTE.md?ref_type=heads)**
+- **[Testing](https://git.tonic-ai.com/releases/vectara-cli/-/blob/devbranch/tests)**
+
+</details>
+
+<details><summary>License</summary>
+
+`vectara-cli` is MIT licensed. See the [LICENSE](https://git.tonic-ai.com/releases/vectara-cli/-/blob/devbranch/LICENSE.md?ref_type=heads) file for more details.
+
+</details>
+
+```
+@misc{Vectara Cli,
+  author = { isayahc , Josephrp, p3nGu1nZz},
+  title = {Vectara Cli is a Python package for Vectara platform interaction, ideal for search and information retrieval tasks.},
+  year = {2024},
+  publisher = {TeamTonic},
+  journal = {Tonic-AI repository},
+  howpublished = {\url{https://git.tonic-ai.com/releases/vectara-cli}}
+}
+```
```

### Comparing `vectara-cli-0.1.9/README.md` & `vectara-cli-0.2.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,54 +1,237 @@
 # vectara-cli
 
 `vectara-cli` is a Python package designed to interact with the Vectara platform, providing a command-line interface (CLI) and a set of APIs for indexing and querying documents, managing corpora, and performing advanced text analysis and processing tasks. This package is particularly useful for developers and data scientists working on search and information retrieval applications.
 
-## Features
+
+#### Features
 
 - Indexing text and documents into Vectara corpora.
 - Querying indexed documents.
 - Creating and deleting corpora.
-- Advanced text processing and analysis using pre-trained models (optional advanced package).
-
-## QuickStart
-
-get started with the [example_notebooks here](https://git.tonic-ai.com/releases/vectara-cli/examples/examples.ipynb) by downloading them and running them locally on any laptop.
+- Advanced text processing and analysis using pre-trained models (optional advanced package(s)).
 
-## Installation
 
 ### Basic Installation
 
 The basic installation includes the core functionality for interacting with the Vectara platform.
 
 ```bash
 pip install vectara-cli
 ```
 
-### Advanced Installation
+#### Advanced Installation
 
 The advanced installation includes additional dependencies for advanced text processing and analysis features. This requires PyTorch, Transformers, and Accelerate, which can be substantial in size.
 
 ```bash
-pip install vectara-cli[advanced]
+pip install vectara-cli[rebel_span]
 ```
 
 Ensure you have an appropriate PyTorch version installed for your system, especially if you're installing on a machine with GPU support. Refer to the [official PyTorch installation guide](https://pytorch.org/get-started/locally/) for more details.
 
-## Command Line Interface (CLI) Usage
+#### Command Line Interface (CLI) Usage
+
+The `vectara-cli` provides a powerful command line interface for interacting with the Vectara platform, enabling tasks such as document indexing, querying, corpus management, and advanced text processing directly from your terminal.
+
+Before your start always set your api keys with :
+
+```bash
+vectara set-api-keys <user_id> <api_key>
+```
+
+#### Deploy Your App
+
+- [x] **`vectara create-ui`:** This command will create a new UI for your app.
+
+**Note:** that this script assumes you have [Node.js and NPM installed](https://nodejs.org/en/download) on your system, as required by the npx command.
+
+<details>
+<summary> Table of Contents </summary>
 
-The `vectara-cli` provides a powerful command line interface for interacting with the Vectara platform, enabling tasks such as document indexing, querying, corpus management, and advanced text processing directly from your terminal. This section will guide you through the basics of using the `vectara-cli`.
+- **[Get started with the example_notebooks here](https://git.tonic-ai.com/releases/vectara-cli/examples/examples.ipynb)**
+- **[More About Configuration](https://git.tonic-ai.com/releases/vectara-cli/-/blob/devbranch/docs/configuration.md)**
+- **[Basic Usage CLI](https://git.tonic-ai.com/releases/vectara-cli/-/blob/devbranch/docs/basic_useage_cli.md?ref_type=heads)**
+- **[Programmatic Usage](https://git.tonic-ai.com/releases/vectara-cli/-/blob/devbranch/docs/basic_usage.md?ref_type=heads)**
+- **[Advanced Usage](https://git.tonic-ai.com/releases/vectara-cli/-/blob/devbranch/docs/advanced_usage.md?ref_type=heads)**
+- **[CONTRIBUTE](https://git.tonic-ai.com/releases/vectara-cli/-/blob/devbranch/CONTRIBUTE.md?ref_type=heads)**
+- **[Testing](https://git.tonic-ai.com/releases/vectara-cli/-/blob/devbranch/tests)**
 
-### Installation
+</details>
 
-Before using the CLI, ensure you have the package installed. You can install it directly from PyPi using pip:
+<details>
+<summary> Get Started </summary>
+
+#### Command Line Interface (CLI) Usage
+
+The `vectara-cli` provides a powerful command line interface for interacting with the Vectara platform, enabling tasks such as document indexing, querying, corpus management, and advanced text processing directly from your terminal.
+
+Before your start always set your api keys with :
 
 ```bash
-pip install vectara-cli
+vectara set-api-keys <user_id> <api_key>
+```
+
+## Basic Usage of Vectara CLI
+
+The Vectara CLI provides a simple and efficient way to interact with the Vectara platform, allowing users to create corpora, index documents, and perform various other operations directly from the command line. This section covers the basic usage of the Vectara CLI for common tasks such as creating a corpus and indexing documents.
+
+### Creating a Corpus
+
+To create a new corpus, you can use the `create-corpus` command. A corpus represents a collection of documents and serves as the primary organizational unit within Vectara.
+
+### Basic Corpus Creation
+
+```bash
+vectara create-corpus <corpus_id> <name> <description>
+```
+
+- `<corpus_id>`: The unique identifier for the corpus. Must be an integer.
+- `<name>`: The name of the corpus. This should be a unique name that describes the corpus.
+- `<description>`: A brief description of what the corpus is about.
+
+#### Example
+
+```bash
+vectara create-corpus 123 "My Corpus" "A corpus containing documents on topic XYZ"
+```
+
+This command creates a basic corpus with the specified ID, name, and description.
+
+### Indexing a Document
+
+To index a document into a corpus, you can use the `index-document` command. This command allows you to add a text document to the specified corpus, making it searchable within the Vectara platform.
+
+### Indexing Text
+
+```bash
+vectara index-text <corpus_id> <document_id> <text> <context> <metadata_json>
+```
+
+- `<corpus_id>`: The unique identifier for the corpus where the document will be indexed.
+- `<document_id>`: A unique identifier for the document being indexed.
+- `<text>`: The actual text content of the document that you want to index.
+- `<context>`: Additional context or information about the document.
+- `<metadata_json>`: A JSON string containing metadata about the document.
+
+#### Example
+
+```bash
+vectara index-text 12345 67890 "This is the text of the document." "Summary of the document" '{"author":"John Doe", "publishDate":"2024-01-01"}'
+```
+
+This command indexes a document with the provided text, context, and metadata into the specified corpus.
+
+### Advanced Corpus Creation
+
+For more advanced scenarios, you might want to specify additional options such as custom dimensions, filter attributes, or privacy settings for your corpus. The `create-corpus-advanced` command allows for these additional configurations.
+
+### Advanced Creation with Options
+
+```bash
+vectara create-corpus-advanced <name> <description> [options]
 ```
 
+Options include setting custom dimensions, filter attributes, public/private status, and more.
+
+#### Example
+
+```bash
+vectara create-corpus-advanced "Research Papers" "Corpus for academic research papers" --custom_dimensions '{"dimension1": "value1", "dimension2": "value2"}' --filter_attributes '{"author": "John Doe"}'
+```
+
+This command creates a corpus with custom dimensions and filter attributes specified, allowing for more detailed organization and retrieval capabilities.
+
+### Deleting a Corpus
+
+To remove an existing corpus from the Vectara platform, you can use the `delete-corpus` command. Deleting a corpus will permanently remove the corpus and all documents contained within it. This action cannot be undone, so ensure that you really want to delete the corpus before proceeding.
+
+#### Basic Corpus Deletion
+
+```bash
+vectara delete-corpus <corpus_id>
+```
+
+- `<corpus_id>`: The unique identifier for the corpus you wish to delete. This must be an integer.
+
+#### Example
+
+```bash
+vectara delete-corpus 12345
+```
+
+This command deletes the corpus with the specified ID from the Vectara platform. Upon successful deletion, you will receive a confirmation message. If the corpus cannot be found or if there is an error during the deletion process, an error message will be displayed instead.
+
+### Uploading a Document
+
+To upload a document to a specific corpus in the Vectara platform, you can use the `upload-document` command. This allows you to add various types of documents, such as PDFs, Word documents, and plain text files, making them searchable within your corpus.
+
+#### Basic Document Upload
+
+```bash
+vectara upload-document <corpus_id> <file_path> [document_id]
+```
+
+- `<corpus_id>`: The unique identifier for the corpus where the document will be uploaded. This must be an integer.
+- `<file_path>`: The path to the document file that you want to upload.
+- `[document_id]`: An optional parameter that specifies the document ID. If not provided, Vectara will generate a unique ID for the document.
+
+#### Example
+
+```bash
+vectara upload-document 12345 "/path/to/document.pdf"
+```
+
+This command uploads a document from the specified file path to the corpus with the given ID. If the upload is successful, you will receive a confirmation message along with any relevant details provided by the Vectara platform.
+
+#### Uploading with a Specific Document ID
+
+If you wish to specify a document ID during the upload process, you can include it as an additional argument:
+
+```bash
+vectara upload-document 12345 "/path/to/document.pdf" "custom-document-id-123"
+```
+
+This allows you to assign a custom identifier to the document, which can be useful for tracking or referencing the document within your application or database.
+
+#### Supported Document Formats
+
+Vectara supports a variety of document formats for upload, including but not limited to:
+
+- PDF (.pdf)
+- Microsoft Word (.docx)
+- PowerPoint (.pptx)
+- Plain Text (.txt)
+
+Ensure that your documents are in one of the supported formats before attempting to upload them to the Vectara platform.
+
+#### Metadata and Context
+
+While the basic upload command does not include options for metadata and context, it's important to note that Vectara allows for the association of metadata with documents. This can be accomplished through advanced usage of the Vectara CLI or API, enabling you to provide additional information about the documents you upload, such as author, publication date, tags, and more.
+
+For detailed instructions on advanced document upload options, including how to include metadata and context, please refer to the Vectara documentation or the advanced usage section of the Vectara CLI help.
+
+
+#### Querying
+
+To perform a query in a specific corpus:
+
+```bash
+vectara query "<query_text>" <num_results> <corpus_id>
+```
+
+- `<query_text>`: The text of the query.
+- `<num_results>`: The maximum number of results to return.
+- `<corpus_id>`: The ID of the corpus to query against.
+
+</details>
+
+<details>
+<summary>  Configuration </summary>
+
 ### Optional: Conda Virtual Environment Setup
 
 Conda is an open-source package management system and environment management system that runs on Windows, macOS, and Linux. It allows you to install, run, and update packages and their dependencies. To set up this project using Conda, follow the steps below:
 
 #### Prerequisites
 
 - Ensure that you have Conda installed on your system. If you do not have Conda installed, you can download it from the [official Conda website](https://www.anaconda.com/products/distribution).
@@ -59,25 +242,23 @@
 2. Navigate to the project directory where the `environment.yml` file is located.
 3. Create a new Conda environment by running the following command:
 
    ```bash
    conda env create -f environment.yml
    ```
 
-   This will create a new environment with the name specified in the `environment.yml` file and install all the required packages.
 
 #### Activating the Environment
 
 Once the environment is created, you can activate it using the following command:
 
 ```bash
-conda activate <env_name>
+conda activate vectara
 ```
 
-Replace `<env_name>` with the name of your Conda environment.
 
 #### Deactivating the Environment
 
 When you are done working on the project, you can deactivate the Conda environment by running:
 
 ```bash
 conda deactivate
@@ -94,19 +275,17 @@
 This will update the environment with any new dependencies specified in the `environment.yml` file.
 
 #### Removing the Environment
 
 If you wish to remove the Conda environment, you can do so with the following command:
 
 ```bash
-conda env remove -n <env_name>
+conda env remove -n vectara
 ```
 
-Again, replace `<env_name>` with the name of your Conda environment.
-
 By following these steps, you can manage your project's dependencies in an isolated environment using Conda.
 
 ### Configuration
 
 #### Setting Credentials via CLI Commands
 
 The `vectara-cli` tool now supports a convenient feature for setting your Vectara customer ID and API key directly through the command line. This method utilizes a command specifically designed for securely storing your credentials, making it easier to manage your Vectara configuration without manually setting environment variables or directly embedding your credentials in your scripts.
@@ -114,23 +293,23 @@
 #### Using the `set-api-keys` Command
 
 To set your Vectara customer ID and API key using the `vectara-cli`, you can use the `set-api-keys` command. This command stores your credentials securely, allowing `vectara-cli` to automatically use them for authentication in future operations.
 
 - **Syntax:** The command follows this simple syntax:
 
 ```bash
-vectara-cli set-api-keys <customer_id> <api_key>
+vectara set-api-keys <customer_id> <api_key>
 ```
 
 Replace `<customer_id>` with your Vectara customer ID and `<api_key>` with your Vectara API key.
 
 - **Example:**
 
 ```bash
-vectara-cli set-api-keys 123456789 abcdefghijklmnopqrstuvwxyz
+vectara set-api-keys 123456789 abcdefghijklmnopqrstuvwxyz
 ```
 
 After executing this command, you will see a confirmation message indicating that your API keys have been set successfully.
 
 #### Windows
 
 For Windows users, you can also set environment variables through the Command Prompt or PowerShell, or via the System Properties window.
@@ -151,67 +330,19 @@
 
 Note that changes made through the command line will only take effect in new instances of the terminal or command prompt.
 
 #### Using Credentials in `vectara-cli`
 
 Once you have set up your environment variables, `vectara-cli` will automatically use these credentials for authentication. There's no need to manually input your customer ID and API key each time you execute a command.
 
-### Basic Commands
-
+</details>
 
-#### Indexing a Document
+<details>
+<summary> Programmatic Usage </summary>
 
-To index a document into a specific corpus:
-
-```bash
-vectara-cli index-document <corpus_id> <document_id> "<title>" '<metadata_json>' "<section_text>"
-```
-
-- `<corpus_id>`: The ID of the corpus where the document will be indexed.
-- `<document_id>`: A unique identifier for the document.
-- `<title>`: The title of the document.
-- `<metadata_json>`: A JSON string containing document metadata.
-- `<section_text>`: The text content of the document.
-
-#### Querying
-
-To perform a query in a specific corpus:
-
-```bash
-vectara-cli query "<query_text>" <num_results> <corpus_id>
-```
-
-- `<query_text>`: The text of the query.
-- `<num_results>`: The maximum number of results to return.
-- `<corpus_id>`: The ID of the corpus to query against.
-
-#### Creating a Corpus
-
-To create a new corpus:
-
-```bash
-vectara-cli create-corpus <corpus_id> "<name>"
-```
-
-- `<corpus_id>`: The ID for the new corpus.
-- `<name>`: The name of the new corpus.
-
-#### Deleting a Corpus
-
-To delete an existing corpus:
-
-```bash
-vectara-cli delete-corpus <corpus_id>
-```
-
-- `<corpus_id>`: The ID of the corpus to delete.
-
-### Advanced Commands
-
-### Basic Usage
 
 #### Setting Up a Vectara Client
 
 First, initialize the Vectara client with your customer ID and API key. This client will be used for all subsequent operations.
 
 ```python
 from vectara_cli.core import VectaraClient
@@ -260,41 +391,14 @@
 num_results = 10  # Number of results to return
 corpus_id = 'your_corpus_id'
 
 results = vectara_client.query(query_text, num_results, corpus_id)
 print(results)
 ```
 
-#### Creating a Corpus
-
-You can create a new corpus by specifying its ID, name, description, and other settings.
-
-```python
-create_corpus_response = vectara_client.create_corpus(
-    corpus_id=123456789,
-    name="Example Corpus",
-    description="This is an example corpus.",
-    dtProvision=1234567890,
-    enabled=True,
-    swapQenc=False,
-    swapIenc=False,
-    textless=False,
-    encrypted=False,
-    encoderId="default",
-    metadataMaxBytes=10000,
-    customDimensions=[
-        {"name": "dimension1", "description": "First custom dimension", "servingDefault": 1.0, "indexingDefault": 1.0}
-    ],
-    filterAttributes=[
-        {"name": "filter1", "description": "First filter attribute", "indexed": True, "type": "FILTER_ATTRIBUTE_TYPE__UNDEFINED", "level": "FILTER_ATTRIBUTE_LEVEL__UNDEFINED"}
-    ]
-)
-print(create_corpus_response)
-```
-
 #### Deleting a Corpus
 
 To delete a corpus, you only need to provide its ID.
 
 ```python
 corpus_id = 'your_corpus_id'
 response, success = vectara_client.delete_corpus(corpus_id)
@@ -318,41 +422,47 @@
 try:
     response, status = vectara_client.upload_document(corpus_id, file_path, document_id, metadata)
     print("Upload successful:", response)
 except Exception as e:
     print("Upload failed:", str(e))
 ```
 
+</details>
+
+<details>
+<summary> Advanced Usage </summary>
+
+
 ### Advanced Usage
 
 
 To leverage the advanced text processing capabilities, ensure you have completed the advanced installation of `vectara-cli`. This includes the necessary dependencies for text analysis:
 
 ```bash
-pip install vectara-cli[advanced]
+pip install vectara-cli[rebel_span]
 ```
 
 #### Span Text Processing
 
 To process text using the Span model:
 
 ```bash
-vectara-cli span-text "<text>" "<model_name>" "<model_type>"
+vectara span-text "<text>" "<model_name>" "<model_type>"
 ```
 
 - `<text>`: The text to process.
 - `<model_name>`: The name of the Span model to use.
 - `<model_type>`: The type of the Span model.
 
 #### Enhanced Batch Processing with NerdSpan
 
 To process and upload documents from a folder:
 
 ```bash
-vectara-cli nerdspan-upsert-folder "<folder_path>" "<model_name>" "<model_type>"
+vectara nerdspan-upsert-folder "<folder_path>" "<model_name>" "<model_type>"
 ```
 
 - `<folder_path>`: The path to the folder containing documents to process and upload.
 - `<model_name>`: The name of the model to use for processing.
 - `<model_type>`: The type of the model.
 
 For more advanced processing and upsert operations, including using the Rebel model for complex document analysis and upload, refer to the specific command documentation provided with the CLI.
@@ -370,28 +480,28 @@
 >> **- supported models:** `science` and `keyphrase`
 
 - **Upload Enriched Text**
 
   To upload text that has been enriched with additional metadata:
 
   ```bash
-  vectara-cli upload-enriched-text <corpus_id> <document_id> <model_name> "<text>"
+  vectara upload-enriched-text <corpus_id> <document_id> <model_name> "<text>"
   ```
 
   - `<corpus_id>`: The ID of the corpus where the document will be uploaded.
   - `<document_id>`: A unique identifier for the document.
   - `<model_name>`: The name of the model used for text enrichment. `science` or `keyphrase`
   - `<text>`: The text content to be enriched and uploaded.
 
 - **Span Enhance Folder**
 
   To process and upload all documents within a folder, enhancing them using a specified model:
 
   ```bash
-  vectara-cli span-enhance-folder <corpus_id_1> <corpus_id_2> <model_name> "<folder_path>"
+  vectara span-enhance-folder <corpus_id_1> <corpus_id_2> <model_name> "<folder_path>"
   ```
 
   - `<corpus_id_1>`: The ID for the corpus to upload plain text documents.
   - `<corpus_id_2>`: The ID for the corpus to upload enhanced text documents.
   - `<model_name>`: The name of the model used for document enhancement. **supported models :** `science` and `keyphrase`
   - `<folder_path>`: The path to the folder containing the documents to be processed.
 
@@ -431,15 +541,15 @@
 This example showcases how to enrich text with additional metadata using the `EnterpriseSpan` class and upload it to a specified corpus in Vectara. By leveraging advanced models for text processing, users can significantly enhance the quality and relevance of their search and retrieval operations on the Vectara platform.
 
 ### Non-Commercial Advanced Usage
 
 The advanced features allow you to enrich your indexes with additional information automatically. This should produce better results for retrieval.
 
 
-![The mRebel pre-trained model is able to extract triplets for up to 400 relation types from Wikidata](https://git.tonic-ai.com/releases/vectara-cli/res/images/image.png?ref_type=heads)
+![Span Models for Named Entity Recognition](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/image.png?ref_type=heads)
 
 ### Non-Commercial Advanced Usage Using Span Models
 
 The `vectara-cli` package extends its functionality through the advanced usage of Span Models, enabling users to perform sophisticated text analysis and entity recognition tasks. This feature is particularly beneficial for non-commercial applications that require deep understanding and processing of textual data.
 
 The `Span` class supports processing and indexing documents from a folder, enabling batch operations for efficiency. This feature allows for the automatic extraction of entities from multiple documents, which are then indexed into specified corpora with enriched metadata.
 
@@ -491,16 +601,17 @@
     vectara_client.index_text(corpus_id, document_id, text, metadata_json=metadata_json)
     ```
 
 **Reference:** Aarsen, T. (2023). SpanMarker for Named Entity Recognition. Radboud University. Supervised by Prof. Dr. Fermin Moscoso del Prado Martin (fermin.moscoso-del-prado@ru.nl) and Dr. Daniel Vila Suero (daniel@argilla.io). Second assessor: Dr. Harrie Oosterhuis (harrie.oosterhuis@ru.nl).
 
 #### Non-Commercial Advanced Rag Using Rebel
 
-![mRebel](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/Screenshot_2024-04-05_112158.png?ref_type=heads)
-![Span Models for Named Entity Recognition](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/Screenshot_2024-04-05_112142.png?ref_type=heads)
+![mRebel](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/Screenshot_2024-04-05_112158.png)
+
+![The mRebel pre-trained model is able to extract triplets for up to 400 relation types from Wikidata](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/Screenshot_2024-04-05_112142.png)
 
 The mRebel pre-trained model is able to extract triplets for up to 400 relation types from Wikidata.
 
 
 Use the use the `Rebel Class` for advanced indexing. This will automatically extract `named entities`, `key phrases`, and other relevant information from your documents : 
 
 
@@ -528,23 +639,148 @@
     print(f"Document ID: {result['documentIndex']}, Score: {result['score']}, Text: {result['text'][:100]}...")
 
 print("\n=== Enhanced Results ===")
 for result in enhanced_results:
     print(f"Document ID: {result['documentIndex']}, Score: {result['score']}, Text: {result['text'][:100]}...")
 ```
 
-## Contributing
+</details>
+
+<details>
+<summary> Contributing </summary>
+
+# Contributing Guidelines for vectara-cli
+
+Thank you for your interest in contributing to `vectara-cli`! As an open-source project, we welcome contributions from developers of all skill levels. This guide will provide you with information on how to contribute effectively and make a valuable impact on the project.
+
+## Prerequisites
+
+Before you begin, ensure you have the following installed:
+
+- Python (preferably the latest Python 3 version)
+- Conda (for managing environments)
+- Git (for version control)
+
+## Identify An Issue
+
+Browse the [Issues](https://git.tonic-ai.com/contribute/vectara/vectara-cli/issues) to find tasks to work on. You can start with issues labeled as "good first issue".
+- If you have an idea or a bug fix that is not listed, feel free to open a new issue to discuss it with other contributors.
+
+## Setting Up for Contribution
+
+1. **Fork the Repository**: Visit [vectara-cli on GitLab](https://git.tonic-ai.com/contribute/vectara/vectara-cli/) and fork the project to your account.
+
+2. **Create a New Branch**: Before you start making changes, switch to the `devbranch` and create a new branch for your feature or fix. We encourage naming your branch in a way that reflects the issue or feature you're working on.
+
+    ```bash
+    git checkout devbranch
+    git checkout -b feature/your-feature-name
+    ```
+    Or, if you're working on a specific issue:
+
+    ```bash
+    git checkout devbranch
+    git checkout -b issue/ISSUE_NUMBER-short-description
+    ```
+
+    This naming convention (`feature/your-feature-name` or `issue/ISSUE_NUMBER-short-description`) helps in identifying branches with their purposes, making collaboration and review processes more efficient.
+
+- the easiest way to make a correctly named branch is to use the gitlab gui directly inside the issue that you are responding to.
+
+![easily use the GUI to make a branch](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/contributingimage.png)
+
+
+3. **Create and Activate Conda Environment**:
+
+   ```bash
+   conda env create -f environment.yml
+   conda activate vectara-cli
+   ```
+
+4. **Install the Project in Editable Mode**:
+
+   ```bash
+   pip install --editable .
+   ```
+
+## Develop
+
+- **Add Functionality**: Write your code and add it to the appropriate directory:
+  - For new functionalities, add your code in `./vectara_cli/commands`.
+  - Add command line functionality in `main.py`.
+  - Create or modify data objects in `./vectara_cli/data`.
+
+- **Add Help Text**: Update help texts in `./vectara_cli/help_texts/help_text.py` to reflect your changes or new commands.
+
+## Write Tests
+
+- Add tests for your new functionalities in the `tests/` directory.
+- Ensure all tests pass by running them locally.
+
+## Document Your Changes
+
+Update any documentation relevant to your changes, including inline comments and README if necessary.
 
-Contributions to `vectara-cli` are welcome! Please refer to the contributing guidelines in the repository for more information on how to contribute.
+## Submitting Your Contributions
 
+1. **Commit Your Changes**: After making your changes, commit them to your branch. Use descriptive commit messages that explain the "why" and "what" of your changes. This practice helps reviewers understand your reasoning and the context of your contributions.
 
-### Contributing to Advanced Features
+    ```bash
+    git add .
+    git commit -m "A descriptive message explaining the change"
+    ```
+
+2. **Push Your Changes**: Once you're ready, push your changes to your forked repository on GitLab.
+
+    ```bash
+    git push origin feature/your-feature-name
+    ```
+    
+    Or, if you're working on an issue:
+
+    ```bash
+    git push origin issue/ISSUE_NUMBER-short-description
+    ```
 
-We welcome contributions to improve and expand the advanced features of `vectara-cli`. Whether it's adding new models, enhancing existing functionalities, or fixing bugs, your contributions are valuable to us. Please refer to our contributing guidelines for more information on how to contribute.
+### 3. Create a Merge Request
+- Go to the [Merge Requests](https://git.tonic-ai.com/contribute/vectara/vectara-cli/-/merge_requests) page.
+- Create a new merge request, compare your feature branch to the main repository's `devbranch`.
+- Fill in a detailed description of your changes and link to any relevant issues.
+
+## Review Process
+Once your merge request is submitted:
+- The project maintainers will review your code and may request changes.
+- Collaborate on modifications and push updates to your branch accordingly.
+- Once approved, a maintainer will merge your changes into the main codebase.
+
+## Post-merge
+After your changes have been merged:
+- Sync your fork with the original repository.
+- Consider deleting your branch to keep your fork clean:
+  ```bash
+  git branch -d your-feature-branch
+  git push origin --delete your-feature-branch
+  ```
+
+Thank you for contributing to `vectara-cli`! For any questions or further discussions, please reach out on the issues page or [on discord](https://discord.gg/7H4SKQekKe).
 
-## License
+- **[CONTRIBUTE](https://git.tonic-ai.com/releases/vectara-cli/-/blob/devbranch/CONTRIBUTE.md?ref_type=heads)**
+- **[Testing](https://git.tonic-ai.com/releases/vectara-cli/-/blob/devbranch/tests)**
 
-`vectara-cli` is MIT licensed. See the [LICENSE](LICENSE.md) file for more details.
+</details>
 
----
+<details><summary>License</summary>
 
-This README provides a comprehensive guide for installing and using the `vectara-cli` package. For further information or assistance, please refer to the [Vectara documentation](https://docs.vectara.com) or submit an issue on the [GitLab repository](https://git.tonic-ai.com/releases/vectara-cli/).
+`vectara-cli` is MIT licensed. See the [LICENSE](https://git.tonic-ai.com/releases/vectara-cli/-/blob/devbranch/LICENSE.md?ref_type=heads) file for more details.
+
+</details>
+
+```
+@misc{Vectara Cli,
+  author = { isayahc , Josephrp, p3nGu1nZz},
+  title = {Vectara Cli is a Python package for Vectara platform interaction, ideal for search and information retrieval tasks.},
+  year = {2024},
+  publisher = {TeamTonic},
+  journal = {Tonic-AI repository},
+  howpublished = {\url{https://git.tonic-ai.com/releases/vectara-cli}}
+}
+```
```

### Comparing `vectara-cli-0.1.9/setup.py` & `vectara-cli-0.2.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # ./setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name="vectara-cli",
-    version="0.1.9",
+    version="0.2.0",
     author="Tonic-AI",
     author_email="team@tonic-ai.com",
     description="A CLI tool for interacting with the Vectara platform, including advanced text processing and indexing features.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://git.tonic-ai.com/releases/vectara-cli",
     packages=find_packages(),
     install_requires=[
         "requests",
+        "argparse", 
     ],
     extras_require={
-        "advanced": [
+        "rebel_span": [
             "accelerate",
             "torch>=1.8.0",
             "transformers>=4.5.0",
             "span_marker",
             "spacy",
         ],
     },
@@ -36,8 +37,8 @@
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Utilities",
     ],
     python_requires=">=3.9",
     license="MIT",
     keywords="vectara search-engine document-indexing text-analysis information-retrieval natural-language-processing cli-tool data-science machine-learning text-processing",
-)
+)
```

### Comparing `vectara-cli-0.1.9/vectara_cli/advanced/commercial/enterprise.py` & `vectara-cli-0.2.0/vectara_cli/rebel_span/commercial/enterprise.py`

 * *Files 4% similar despite different names*

```diff
@@ -176,23 +176,7 @@
             if not success or not extracted_text:
                 continue
             text_chunks = self.text_chunk(extracted_text)
 
             for chunk in text_chunks:
                 predictions = self.predict(chunk)
                 self.upload_enriched_text(corpus_id_2, document_id, chunk, predictions)
-
-
-# # Example usage
-# if __name__ == "__main__":
-#     logging.basicConfig(level=logging.INFO)
-#     enterprise_model = EnterpriseSpan("keyphrase")
-#     text = "Example text for processing."
-#     try:
-#         entities = enterprise_model.predict(text)
-#         formatted_predictions = enterprise_model.format_predictions(entities)
-#         print("Predictions:\n", formatted_predictions)
-#         # Prepend formatted predictions to the original text
-#         complete_text = f"Extracted Information:\n{formatted_predictions}\n\nOriginal Text:\n{text}"
-#         print("\nComplete Text:\n", complete_text)
-#     except Exception as e:
-#         print(f"An error occurred: {e}")
```

### Comparing `vectara-cli-0.1.9/vectara_cli/advanced/noncommercial/rebel.py` & `vectara-cli-0.2.0/vectara_cli/rebel_span/noncommercial/rebel.py`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.9/vectara_cli/commands/delete_corpus.py` & `vectara-cli-0.2.0/vectara_cli/commands/query.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-# ./commands/delete_corpus.py
+# query.py
 
 from vectara_cli.core import VectaraClient
-from vectara_cli.config_manager import ConfigManager
+from vectara_cli.utils.config_manager import ConfigManager
+from vectara_cli.data.query_response import QueryResponse
 
-
-def main(args, vectara_client):
-    if len(args) < 2:
-        print("Usage: vectara-cli delete-corpus corpus_id")
+def main(vectara_client, args):
+    if len(args) < 3:
+        print("Usage: vectara-cli query query_text num_results corpus_id")
         return
-
-    corpus_id = args[1]
+    query_text = args[0]
+    num_results = int(args[1])
+    corpus_id = args[2]
 
     try:
-        customer_id, api_key = ConfigManager.get_api_keys()
-        response, success = vectara_client.delete_corpus(corpus_id)
-
-        if success:
-            print("Corpus deleted successfully.")
-        else:
-            print("Failed to delete corpus:", response)
+        # customer_id, api_key = ConfigManager.get_api_keys()
+        response = vectara_client.query(query_text, num_results, corpus_id)
+        parsed_response = QueryResponse.parse_response(response)
+        for item in parsed_response:
+            print(item)
     except ValueError as e:
         print(e)
 
-
 if __name__ == "__main__":
     import sys
 
-    main(sys.argv[1:])
+    main(sys.argv)
```

### Comparing `vectara-cli-0.1.9/vectara_cli/commands/rebel_upsert_folder.py` & `vectara-cli-0.2.0/vectara_cli/commands/rebel_upsert_folder.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 # ./commands/rebel_upsert_folder.py
 
 import os
 from vectara_cli.core import VectaraClient
-from vectara_cli.config_manager import ConfigManager
-from vectara_cli.advanced.noncommercial.rebel import Rebel
+from vectara_cli.utils.config_manager import ConfigManager
+from vectara_cli.rebel_span.noncommercial.rebel import Rebel
 
 
-def main(args, vectara_client):
+def main(vectara_client, args):
     if len(args) < 4:
         print(
             "Usage: vectara-cli advanced-upsert-folder folder_path corpus_id_1 corpus_id_2"
         )
-        print(
-            "Usage: vectara-cli advanced-upsert-folder folder_path corpus_id_1 corpus_id_2"
-        )
         return
 
     folder_path = args[1]
     corpus_id_1 = args[2]
     corpus_id_2 = args[3]
 
     try:
@@ -27,17 +24,14 @@
             print(f"The specified folder path does not exist: {folder_path}")
             return
 
         rebel = Rebel()
         rebel.advanced_upsert_folder(
             vectara_client, corpus_id_1, corpus_id_2, folder_path
         )
-        rebel.advanced_upsert_folder(
-            vectara_client, corpus_id_1, corpus_id_2, folder_path
-        )
         print(f"Advanced processing and upsert completed for folder: {folder_path}")
     except Exception as e:
         print("An error occurred during the upsert process:", str(e))
 
 
 if __name__ == "__main__":
     import sys
```

### Comparing `vectara-cli-0.1.9/vectara_cli/commands/span_enhance_folder.py` & `vectara-cli-0.2.0/vectara_cli/commands/span_enhance_folder.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # ./commands/span_enhance_folder.py
 
 import os
-from vectara_cli.config_manager import ConfigManager
-from vectara_cli.advanced.commercial.enterprise import EnterpriseSpan
+from vectara_cli.utils.config_manager import ConfigManager
+from vectara_cli.rebel_span.commercial.enterprise import EnterpriseSpan
 
 
-def main(args, vectara_client):
-    if len(args) < 5:
+def main(vectara_client, args):
+    if len(args) < 4:
         print(
             "Usage: vectara-cli span-enhance-folder corpus_id_1 corpus_id_2 model_name folder_path"
         )
         return
 
-    corpus_id_1 = args[1]
-    corpus_id_2 = args[2]
-    model_name = args[3]
-    folder_path = args[4]
+    corpus_id_1 = args[0]
+    corpus_id_2 = args[1]
+    model_name = args[2]
+    folder_path = args[3]
 
     try:
         customer_id, api_key = ConfigManager.get_api_keys()
         if not os.path.isdir(folder_path):
             print(f"The specified folder path does not exist: {folder_path}")
             return
```

### Comparing `vectara-cli-0.1.9/vectara_cli/commands/span_text.py` & `vectara-cli-0.2.0/vectara_cli/commands/nerdspan_upsert_folder.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,45 @@
-# ./commands/span_text.py
+# ./commands/nerdspan_upsert_folder.py
 
-from vectara_cli.advanced.noncommercial.nerdspan import Span
-from vectara_cli.config_manager import ConfigManager
 
+import sys
+import os
+from vectara_cli.rebel_span.noncommercial.nerdspan import Span
+from vectara_cli.utils.config_manager import ConfigManager
+from vectara_cli.core import VectaraClient
+from vectara_cli.data.corpus_data import CorpusData
 
-def main(args, vectara_client):
-    if len(args) < 5:
-        print("Usage: vectara-cli process-text text model_name model_type")
+
+def main(vectara_client:VectaraClient, args):
+    if len(args) < 3:
+        print("Usage: vectara process-and-upload folder_path model_name model_type")
         return
 
-    text = args[1]
-    model_name = args[2]
-    model_type = args[3]
+    folder_path = args[0]
+    model_name = args[1]
+    model_type = args[2]
 
     try:
-        customer_id, api_key = ConfigManager.get_api_keys()
-        span = Span(text, customer_id, api_key)
-        span.load_model(model_name, model_type)
-        output_str, key_value_pairs = span.analyze_text(model_name)
-        print(output_str)
-        print(key_value_pairs)
+        # customer_id, api_key = ConfigManager.get_api_keys()
+        if not os.path.isdir(folder_path):
+            print(f"The specified folder path does not exist: {folder_path}")
+            return
+        span = Span(
+            vectara_client=vectara_client, 
+            text="", 
+            model_name=model_name, 
+            model_type=model_type
+        )
+        corpus_id_1, corpus_id_2 = span.process_and_upload(
+            folder_path, model_name, model_type
+        )
+        print(
+            f"Documents processed and uploaded. Raw uploads in Corpus ID: {corpus_id_1}, Processed uploads in Corpus ID: {corpus_id_2}"
+        )
     except Exception as e:
-        print("Error processing text:", str(e))
+        print("An error occurred during processing:", str(e))
 
 
 if __name__ == "__main__":
-    import sys
+    
 
-    main(sys.argv[1:])
+    main(sys.argv)
```

### Comparing `vectara-cli-0.1.9/vectara_cli/commands/upload_document.py` & `vectara-cli-0.2.0/vectara_cli/commands/upload_document.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # ./commands/upload_document.py
 
-from vectara_cli.core import VectaraClient
-from vectara_cli.config_manager import ConfigManager
+from vectara_cli.utils.config_manager import ConfigManager
+from vectara_cli.helptexts.help_text import print_upload_document_help
 
-
-def main(args, vectara_client):
-    if len(args) < 4:
-        print("Usage: vectara-cli upload-document corpus_id file_path [document_id]")
+def main(vectara_client, args):
+    if len(args) < 3:
+        print_upload_document_help()
         return
 
-    corpus_id = args[1]
-    file_path = args[2]
-    document_id = args[3] if len(args) > 3 else None
+    corpus_id = args[0]
+    file_path = args[1]
+    document_id = args[2] if len(args) > 3 else None
     metadata = {}
 
     try:
         customer_id, api_key = ConfigManager.get_api_keys()
         response, status = vectara_client.upload_document(
             corpus_id, file_path, document_id, metadata
         )
@@ -26,9 +25,8 @@
             print("Upload failed:", response)
     except Exception as e:
         print("Upload failed:", str(e))
 
 
 if __name__ == "__main__":
     import sys
-
-    main(sys.argv[1:])
+    main(sys.argv)
```

### Comparing `vectara-cli-0.1.9/vectara_cli/commands/upload_enriched_text.py` & `vectara-cli-0.2.0/vectara_cli/commands/upload_enriched_text.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ./commands/upload_enriched_text.py
 
-from vectara_cli.config_manager import ConfigManager
-from vectara_cli.advanced.commercial.enterprise import EnterpriseSpan
+from vectara_cli.utils.config_manager import ConfigManager
+from vectara_cli.rebel_span.commercial.enterprise import EnterpriseSpan
 
 
-def main(args, vectara_client):
+def main(vectara_client, args):
     if len(args) < 6:
         print(
             "Usage: vectara-cli upload-enriched-text corpus_id document_id model_name text"
         )
         return
 
     corpus_id = args[1]
```

### Comparing `vectara-cli-0.1.9/vectara_cli/core.py` & `vectara-cli-0.2.0/vectara_cli/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 # ./vectara-cli/core.py
 
 import requests
 import json
 import os
 import logging
-from .corpus_data import CorpusData
-from .defaults import CorpusDefaults
+from typing import List, Tuple
+from .data.corpus_data import CorpusData
+from .data.defaults import CorpusDefaults
+from .data.query_request import (
+    QueryRequest, CorpusKey, ContextConfig, SummaryConfig, 
+    ChatRequest , ScaleRequest , SpecialRequest, GrowthRequest
+)
+from .data.query_response import QueryResponse
 
 class VectaraClient:
     def __init__(self, customer_id, api_key):
         self.base_url = "https://api.vectara.io"
         self.customer_id = str(customer_id)
         self.api_key = api_key
         self.headers = {
@@ -21,64 +27,52 @@
 
     def index_text(
         self,
         corpus_id,
         document_id,
         text,
         context="",
-        metadata_json="",
+        metadata_json="{}",
         custom_dims=None,
+        timeout=30
     ):
         if custom_dims is None:
             custom_dims = []
-        if not isinstance(metadata_json, str):
-            metadata_json = json.dumps(metadata_json)
+        try:
+            metadata_json_obj = json.loads(metadata_json)
+        except json.JSONDecodeError:
+            raise ValueError("metadata_json must be a valid JSON string.")
+        
         corpus_id = str(corpus_id)
         url = f"{self.base_url}/v1/core/index"
         payload = {
-            "customerId": int(self.customer_id),
-            "corpusId": int(corpus_id), 
+            "customerId": self.customer_id,
+            "corpusId": corpus_id,
             "document": {
                 "documentId": document_id,
-                "metadataJson": metadata_json.replace('"', '\\"'),
+                "metadataJson": json.dumps(metadata_json_obj),
                 "parts": [
                     {
                         "text": text,
                         "context": context,
-#                       "metadataJson": json.dumps(metadata_json),
-                        "metadataJson": metadata_json,
+                        "metadataJson": json.dumps(metadata_json_obj),
                         "customDims": custom_dims,
                     }
                 ],
                 "defaultPartContext": context,
                 "customDims": custom_dims,
             },
         }
-
-        response = requests.post(url, headers=self.headers, data=json.dumps(payload))
-
-        if response.status_code == 200:
-            response_data = response.json()
-            if "status" in response_data and response_data["status"]["code"] == "OK":
-                print("Indexing successful.")
-                return response_data
-            else:
-                print(
-                    "Indexing completed with status:", response_data["status"]["code"]
-                )
-                return response_data
-        else:
-            try:
-                error_response = response.json()
-                print(
-                    f"Error indexing text: {error_response.get('message', 'Unknown error')}"
-                )
-            except json.JSONDecodeError:
-                print(f"Non-JSON error response from server: {response.text}")
-            return None
+        try:
+            response = requests.post(f"{self.base_url}/v1/core/index", headers=self.headers, json=payload, timeout=timeout)
+            response.raise_for_status()
+            return response.json()
+        except requests.exceptions.RequestException as e:
+            logging.error(f"Request failed: {e}")
+            raise
 
     def query(self, query_text, num_results=10, corpus_id=None):
         url = f"{self.base_url}/v1/query"
         data_dict = {
             "query": [
                 {
                     "query": query_text,
@@ -88,41 +82,65 @@
                             "customer_id": self.headers["customer-id"],
                             "corpus_id": corpus_id,
                         }
                     ],
                 }
             ]
         }
-
         response = requests.post(url, headers=self.headers, data=json.dumps(data_dict))
         if response.status_code != 200:
             print(f"Query failed with status code: {response.status_code}")
             return None
-
         try:
+            print("a")
             response_data = response.json()
+            print("response_data: ", response_data)
         except json.JSONDecodeError:
             print("Failed to parse JSON response from query.")
             return None
 
         return self._parse_query_response(response_data)
 
+    def advanced_query(self, query_text, num_results,  corpus_id, context_config, summary_config):
+        url = f"{self.base_url}/v1/query"
+        data = {
+            "query": [{
+                "query": query_text,
+                "start": 0,
+                "numResults": num_results,
+                "contextConfig": context_config,
+                "corpusKey": [{
+                    #"customerId": self.customer_id,
+                    "corpusId": corpus_id
+                }],
+                "summary": [summary_config]
+            }]
+        }
+
+        print("Sending request to:", url)
+        print("Request data:", json.dumps(data, indent=4)) 
+        response = requests.post(url, headers=self.headers, json=data)
+        print(f"Response Status Code: {response.status_code}")
+        print(f"Response content: {response.text}")
+        print(f"Response Status Code: {response.status_code}")
+        if response.status_code == 200:
+            return response.json()
+        else:
+            return {"error": f"Failed to fetch data: {response.text}"}
+    
     def _parse_query_response(self, response_data):
+        print("Parsing query response data...")
+        responses = []
         if "responseSet" in response_data:
             for response_set in response_data["responseSet"]:
-                if "response" in response_set:
-                    # Extracting and returning the first response for simplicity. Adjust as needed.
-                    responses = response_set["response"]
-                    return [
-                        self._extract_response_info(response) for response in responses
-                    ]
-        else:
-            print("No response set found in the data")
-        return []
-
+                if 'response' in response_set:
+                    processed_responses = QueryResponse.parse_response(response_set['response'])
+                    responses.extend(processed_responses)
+        return responses    
+    
     @staticmethod
     def _extract_response_info(response):
         return {
             "text": response.get("text", ""),
             "score": response.get("score", 0),
             "metadata": response.get("metadata", []),
             "documentIndex": response.get("documentIndex"),
@@ -146,19 +164,43 @@
             "customer_id": self.customer_id,
             "corpus_id": corpus_id,
             "document": document,
         }
 
         return json.dumps(request)
 
-    def create_corpus(self, corpus_data: CorpusData):
-        url = f"{self.base_url}/v1/create-corpus"
-        payload = corpus_data.to_dict()
+    def post_query(self, data):
+        url = f"{self.base_url}/v1/query"
+        response = requests.post(url, headers=self.headers, json=data)
+        return response.json()
+
+    def make_specialized_request(self, request):
+        if isinstance(request, SpecialRequest):
+            query_data = {
+                "query": [{
+                    "query": request.query,
+                    "start": request.start,
+                    "numResults": request.num_results,
+                    "contextConfig": request.context_config.to_dict(),
+                    "corpusKey": [key.to_dict() for key in request.corpus_config],
+                    "summary": [request.summary_config.to_dict()]
+                }]
+            }
+
+            if isinstance(request, ScaleRequest) and hasattr(request, 'lexical_config'):
+                query_data['query'][0]['lexicalInterpolationConfig'] = request.lexical_config.to_dict()
+
+            if isinstance(request, ChatRequest) and hasattr(request, 'chat_config'):
+                query_data['query'][0]['chat'] = request.chat_config.to_dict()
+
+            return self.post_query(query_data)
 
-        response = requests.post(url, headers=self.headers, data=json.dumps(payload))
+    def create_corpus(self, corpus_data: dict):
+        url = f"{self.base_url}/v1/create-corpus"
+        response = requests.post(url, headers=self.headers, data=json.dumps({"corpus": corpus_data}))
         return self._parse_response(response)
 
     def _parse_response(self, response):
         if response.status_code == 200:
             try:
                 response_data = response.json()
                 return {"success": True, "data": response_data}
@@ -248,15 +290,15 @@
         except ValueError as e:
             logging.error("Invalid response received from Vectara API: %s", e)
             return {"code": "INVALID_RESPONSE", "message": "The response from Vectara API could not be decoded."}, False
 
 
     def index_documents_from_folder(
         self, corpus_id, folder_path, return_extracted_document=False
-    ):
+    ) -> Tuple[str,bool,requests.request]:
         """Indexes all documents in a specified folder.
 
         Args:
             corpus_id: The ID of the corpus to which the documents will be indexed.
             folder_path: The path to the folder containing the documents.
 
         Returns:
@@ -267,32 +309,77 @@
             file_path = os.path.join(folder_path, file_name)
             document_id = os.path.splitext(file_name)[0]
 
             try:
                 response, status = self.upload_document(
                     corpus_id,
                     file_path,
-                    document_id=document_id,
+                    # document_id=document_id,
                     return_extracted_document=return_extracted_document,
                 )
-                extracted_text = (
-                    response.get("extractedText", "")
-                    if return_extracted_document
-                    else None
-                )
-                results.append((document_id, status == "Success", extracted_text))
+                extracted_chunks:List[str]=[ i['text'] for i in response['document']['section'] ]
+                joined_chunks:str = ''.join(extracted_chunks)
+                
+                # extracted_text = (
+                #     response.get("extractedText", "")
+                #     if return_extracted_document
+                #     else None
+                # )
+                results.append((document_id, status == "Success", joined_chunks))
                 if status != "Success":
                     logging.error(f"Failed to index document {document_id}: {response}")
                 else:
                     logging.info(f"Successfully indexed document {document_id}")
             except Exception as e:
                 logging.error(f"Error uploading or indexing file {file_name}: {e}")
                 results.append((document_id, False, None))
 
         return results
+    
+    def alt_index_documents_from_folder(
+        self, corpus_id, folder_path, return_extracted_document=False
+    # ) -> Tuple[str,requests,requests.request]:
+    ) -> Tuple[str,dict,str]:
+        """Indexes all documents in a specified folder.
+
+        Args:
+            corpus_id: The ID of the corpus to which the documents will be indexed.
+            folder_path: The path to the folder containing the documents.
+
+        Returns:
+            A list of tuples, each containing the document ID and a boolean indicating success or failure.
+        """
+        results = []
+        for file_name in os.listdir(folder_path):
+            file_path = os.path.join(folder_path, file_name)
+            document_id = os.path.splitext(file_name)[0]
+
+            try:
+                response, status = self.upload_document(
+                    corpus_id,
+                    file_path,
+                    # document_id=document_id,
+                    return_extracted_document=return_extracted_document,
+                )
+                extracted_chunks:List[str]=[ i['text'] for i in response['document']['section'] ]
+                joined_chunks:str = ''.join(extracted_chunks)
+                
+
+                results.append((document_id, response , joined_chunks))
+                
+                
+                if status != "Success":
+                    logging.error(f"Failed to index document {document_id}: {response}")
+                else:
+                    logging.info(f"Successfully indexed document {document_id}")
+            except Exception as e:
+                logging.error(f"Error uploading or indexing file {file_name}: {e}")
+                results.append((document_id, response, ""))
+
+        return results
 
     def delete_corpus(self, corpus_id):
         """Deletes a specified corpus.
 
         Args:
             corpus_id: The ID of the corpus to be deleted.
 
@@ -326,15 +413,15 @@
             logging.error("Request failed: %s", e)
             return {"error": str(e)}, False
 
     def upload_document(
         self,
         corpus_id,
         file_path,
-        document_id=None,
+        # document_id=None,
         metadata=None,
         return_extracted_document=False,
     ):
         """
         Uploads and indexes a document into a corpus.
 
         Args:
@@ -373,108 +460,65 @@
                 error_message = "Failed to parse error response."
 
             raise Exception(
                 f"Failed to upload document: HTTP {response.status_code} - {error_message}"
             )
 
 
-# # Example usage
-# CUSTOMER_ID = "your_customer_id"
-# API_KEY = "your_api_key"
-# CORPUS_ID = "your_corpus_id"
-# FILE_PATH = "/path/to/your/document.pdf"
-# DOCUMENT_ID = "unique_document_id"  # Optional
-# METADATA = {"author": "Author Name", "title": "Document Title"}  # Optional
-
-# vectara_client = VectaraClient(CUSTOMER_ID, API_KEY)
-# try:
-#     response = vectara_client.upload_document(CORPUS_ID, FILE_PATH, DOCUMENT_ID, METADATA)
-#     print("Upload successful:", response)
-# except Exception as e:
-#     print("Upload failed:", str(e))
-
-# # Example usage:
-# CUSTOMER_ID = "your_customer_id"
-# API_KEY = "your_api_key"
-# CORPUS_ID = 1  # Example corpus ID, replace with actual corpus ID to delete
-
-# vectara_client = VectaraClient(CUSTOMER_ID, API_KEY)
-# response, success = vectara_client.delete_corpus(CORPUS_ID)
-
-# if success:
-#     print("Corpus deleted successfully.")
-# else:
-#     print("Failed to delete corpus:", response)
-# # Example usage:
-# CUSTOMER_ID = "your_customer_id"
-# API_KEY = "your_api_key"
-# CORPUS_ID = "your_corpus_id"
-
-# vectara_client = VectaraClient(CUSTOMER_ID, API_KEY)
-
-# # Indexing a document
-# metadata = {
-#     "book-name": "Another example title",
-#     "collection": "Mathematics",
-#     "author": "Example Author",
-# }
-# section_text = "The answer to the ultimate question of life, the universe, and everything is 42."
-# document_id = "doc-id-2"
-# title = "Another Example Title"
-
-# response, success = vectara_client.index_document(CORPUS_ID, document_id, title, metadata, section_text)
-# if success:
-#     print("Document indexed successfully.")
-# else:
-#     print("Document indexing failed.", response)
-
-# # Example usage:
-# CUSTOMER_ID = "your_customer_id"
-# API_KEY = "your_api_key"
-
-# vectara_client = VectaraClient(CUSTOMER_ID, API_KEY)
-
-# # Creating a corpus
-# create_corpus_response = vectara_client.create_corpus(
-#     corpus_id=123456789,
-#     name="Example Corpus",
-#     description="This is an example corpus.",
-#     dtProvision=1234567890,
-#     enabled=True,
-#     swapQenc=False,
-#     swapIenc=False,
-#     textless=False,
-#     encrypted=False,
-#     encoderId="default",
-#     metadataMaxBytes=10000,
-#     customDimensions=[
-#         {"name": "dimension1", "description": "First custom dimension", "servingDefault": 1.0, "indexingDefault": 1.0}
-#     ],
-#     filterAttributes=[
-#         {"name": "filter1", "description": "First filter attribute", "indexed": True, "type": "FILTER_ATTRIBUTE_TYPE__UNDEFINED", "level": "FILTER_ATTRIBUTE_LEVEL__UNDEFINED"}
-#     ]
-# )
-# print(create_corpus_response)
-# # Example usage:
-# CUSTOMER_ID = "your_customer_id"
-# API_KEY = "your_api_key"
-# CORPUS_ID = "your_corpus_id"
-
-# vectara_client = VectaraClient(CUSTOMER_ID, API_KEY)
-
-# # Indexing a document
-# index_response = vectara_client.index_document(
-#     corpus_id=CORPUS_ID,
-#     document_id="unique_document_id",
-#     text="This is the document text.",
-#     context="Document context",
-#     metadata_json='{"author": "John Doe"}'
-# )
-# print(index_response)
-
-# # Querying
-# query_response = vectara_client.query(
-#     query_text="What is the meaning of life?",
-#     num_results=10,
-#     corpus_id=CORPUS_ID
-# )
-# print(query_response)
+class LocalVectaraClient(VectaraClient):
+    """
+    A client for interacting with the Vectara API using local environment variables
+    for authentication.
+
+    Inherits from VectaraClient.
+
+    Attributes:
+        base_url (str): The base URL of the Vectara API.
+        customer_id (str): The customer ID used for authentication.
+        api_key (str): The API key used for authentication.
+        headers (dict): The headers to be included in API requests.
+
+    Methods:
+        __init__(self, *args, **kwargs): Initializes the client with authentication
+            credentials retrieved from environment variables.
+        index_text(self, corpus_id, document_id, text, context="", metadata_json="{}",
+            custom_dims=None, timeout=30): Indexes text data into the specified corpus.
+        query(self, query_text, num_results=10, corpus_id=None): Performs a simple
+            text-based query.
+        advanced_query(self, query_text, num_results=10, corpus_id=None, context_config=None,
+            summary_config=None): Performs an advanced query with optional configuration
+            for context and summary.
+        create_corpus(self, corpus_data: CorpusData): Creates a new corpus with the
+            provided metadata.
+        index_document(self, corpus_id, document_id, title, metadata, section_text):
+            Indexes a single document into the specified corpus.
+        index_documents_from_folder(self, corpus_id, folder_path, return_extracted_document=False):
+            Indexes all documents in a specified folder into the specified corpus.
+        delete_corpus(self, corpus_id): Deletes the specified corpus.
+        upload_document(self, corpus_id, file_path, document_id=None, metadata=None,
+            return_extracted_document=False): Uploads and indexes a single document into
+            the specified corpus.
+
+    """
+
+    def __init__(self, *args, **kwargs):
+        """
+        Initializes the LocalVectaraClient instance with authentication credentials
+        retrieved from environment variables.
+
+        Args:
+            *args: Variable length argument list.
+            **kwargs: Arbitrary keyword arguments.
+
+        """
+        self.base_url = "https://api.vectara.io"
+        self.customer_id = os.getenv("VECTARA_CUSTOMER_ID")
+        self.api_key = os.getenv("VECTARA_API_KEY")
+        self.headers = {
+            "Content-Type": "application/json",
+            "Accept": "application/json",
+            "customer-id": str(self.customer_id),
+            "x-api-key": self.api_key,
+        }
+
+        
+
```

### Comparing `vectara-cli-0.1.9/vectara_cli/corpus_data.py` & `vectara-cli-0.2.0/vectara_cli/data/corpus_data.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,49 @@
 # ./corpus_data.py
 
 from .filter_attribute import FilterAttribute
 from .custom_dimension import CustomDimension
 
 class CorpusData:
-    def __init__(self, corpus_id, name, description, dtProvision, enabled, swapQenc, swapIenc, textless, encrypted, encoderId, metadataMaxBytes, customDimensions, filterAttributes):
+    def __init__(
+        self, 
+        name:str, 
+        description:str, 
+        dtProvision=None, 
+        corpus_id=None, 
+        enabled:bool=True, 
+        swapQenc:bool=True, 
+        swapIenc:bool=False, 
+        textless:bool=False, 
+        encrypted:bool=False, 
+        encoderId:int=1,
+        metadataMaxBytes:int=1000, 
+        customDimensions:list=[], 
+        filterAttributes:list=[],
+    ):
         self.corpus_id = corpus_id
         self.name = name
         self.description = description
-        self.dtProvision = int(dtProvision) if encoderId.isdigit() else None
+        self.dtProvision = dtProvision if dtProvision is not None else None
         self.enabled = enabled
         self.swapQenc = swapQenc
         self.swapIenc = swapIenc
         self.textless = textless
         self.encrypted = encrypted
-        self.encoderId = int(encoderId) if encoderId.isdigit() else 1
+        self.encoderId = encoderId if encoderId is not None else 1
         self.metadataMaxBytes = metadataMaxBytes
         self.customDimensions = [CustomDimension(**dim) for dim in customDimensions]
         self.filterAttributes = [FilterAttribute(**attr) for attr in filterAttributes]
 
     def to_dict(self):
         return {
             "id": self.corpus_id,
             "name": self.name,
             "description": self.description,
-            "dtProvision": self.dtProvision, # ommit if there's an issue ?
+            "dtProvision": self.dtProvision,
             "enabled": self.enabled,
             "swapQenc": self.swapQenc,
             "swapIenc": self.swapIenc,
             "textless": self.textless,
             "encrypted": self.encrypted,
             "encoderId": self.encoderId,
             "metadataMaxBytes": self.metadataMaxBytes,
```

### Comparing `vectara-cli-0.1.9/vectara_cli/custom_dimension.py` & `vectara-cli-0.2.0/vectara_cli/data/custom_dimension.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,7 +10,18 @@
     def to_dict(self):
         return {
             "name": self.name,
             "description": self.description,
             "servingDefault": self.servingDefault,
             "indexingDefault": self.indexingDefault,
         }
+
+class TextCustomDimensions:
+    def __init__(self, name, value):
+        self.name = name
+        self.value = value
+
+    def to_dict(self):
+        return {
+            "name": self.name,
+            "value": self.value
+        }
```

### Comparing `vectara-cli-0.1.9/vectara_cli/main.py` & `vectara-cli-0.2.0/vectara_cli/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,78 +1,106 @@
- # ./main.py
-import sys 
+# ./main.py
+
+import sys
 from vectara_cli.commands import (
+    create_corpus,
     nerdspan_upsert_folder,
     index_text,
     index_document,
-    query,
-    create_corpus,
+    advanced_query,
     delete_corpus,
     span_enhance_folder,
     upload_document,
     upload_enriched_text,
     span_text,
     rebel_upsert_folder,
+    upload_folder,
+    query,
+    specialized_query,
+)
+from vectara_cli.utils.create_ui import create_ui
+from vectara_cli.utils.config_manager import ConfigManager
+from vectara_cli.utils.utils import (
+    get_vectara_client,
+    set_api_keys as set_api_keys_main,
+    get_api_keys as get_api_keys_main,
 )
-from vectara_cli.config_manager import ConfigManager
-# from vectara_cli.commands.set_api_keys import main as set_api_keys_main
-from vectara_cli.utils import get_vectara_client , set_api_keys as set_api_keys_main
-
-def print_help():
-    help_text = """
-    Usage: vectara-cli <command> [arguments]
-
-    Commands:
-    set-api-keys <customer_id> <api_key> - Set the API keys for Vectara client.
-    index-document <args> - Index a document in the Vectara platform.
-    query <args> - Query the Vectara platform.
-    create-corpus <args> - Create a new corpus in the Vectara platform.
-    delete-corpus <args> - Delete a corpus from the Vectara platform.
-    span-text <args> - Process text using the span model.
-    span-enhance-folder <args> - Enhance documents in a folder using the span model.
-    upload-document <args> - Upload a document to the Vectara platform.
-    upload-enriched-text <args> - Upload enriched text to the Vectara platform.
-    nerdspan-upsert-folder <args> - Process and upload documents in a folder using the nerdspan model.
-    rebel-upsert-folder <args> - Perform advanced upsert for a folder using the rebel model.
+from vectara_cli.helptexts.help_text import main_help_text
+from typing import Callable, Dict
 
-    Use 'vectara-cli help' to display this help message.
+def get_command_mapping() -> Dict[str,Callable]:
+    command_mapping = {
+        "index-document": index_document.main,
+        "query": query.main,
+        "create-corpus": create_corpus.main,
+        "delete-corpus": delete_corpus.main,
+        "span-text": span_text.main,
+        "span-enhance-folder": span_enhance_folder.main,
+        "upload-document": upload_document.main,
+        "upload-folder": upload_folder.main,
+        "upload-enriched-text": upload_enriched_text.main,
+        "nerdspan-upsert-folder": nerdspan_upsert_folder.main,
+        "rebel-upsert-folder": rebel_upsert_folder.main,
+        "index-text": index_text.main,
+        "create-ui": create_ui,
+        "advanced-query": advanced_query.main,
+        "specialized-query": specialized_query,
+    }
+    return command_mapping
+
+
+def handle_api_keys(args):
+    if len(args) != 2:
+        print(
+            "Error: set-api-keys requires exactly 2 arguments: customer_id and api_key."
+        )
+    else:
+        set_api_keys_main(*args)
+    sys.exit(1)
+
+
+def display_api_keys():
     """
-    print(help_text)
+    Prints the customer ID and API key to the console.
+    """
+    customer_id, api_key = get_api_keys_main()
+    print(f"Customer ID: {customer_id}")
+    print(f"API Key: {api_key}")
 
-def main():
+
+def handle_command(command, args):
+    vectara_client = get_vectara_client()
+    command_mapping = get_command_mapping()
+    if command in command_mapping:
+        if command == "create-ui":
+            command_mapping[command]()
+        else:
+            command_func = command_mapping[command]
+            if callable(command_func):
+                command_func(vectara_client, args)
+            else:
+                print(
+                    f"vectara: '{command}' is not a vectara command. See 'vectara --help'."
+                )
+            sys.exit(1)
+
+
+def handle_help():
     if len(sys.argv) < 2 or sys.argv[1] in ("help", "--help", "-h"):
-        print_help()
-        return
+        main_help_text()
+        sys.exit(0)
 
-    command = sys.argv[1]
-    args = sys.argv[1:] 
 
+def main():
+    handle_help()
+    command = sys.argv[1]
+    args = sys.argv[2:]
     if command == "set-api-keys":
-        set_api_keys_main(args)
+        handle_api_keys(args)
+    elif command == "get-api-keys":
+        display_api_keys()
     else:
-        try:
-            vectara_client = get_vectara_client()
-            command_mapping = {
-                "index-document": index_document.main,
-                "query": query.main,
-                "create-corpus": create_corpus.main,
-                "delete-corpus": delete_corpus.main,
-                "span-text": span_text.main,
-                "span-enhance-folder": span_enhance_folder.main,
-                "upload-document": upload_document.main,
-                "upload-enriched-text": upload_enriched_text.main,
-                "nerdspan-upsert-folder": nerdspan_upsert_folder.main,
-                "rebel-upsert-folder": rebel_upsert_folder.main,
-                "index-text": index_text.main,
-            }
+        handle_command(command, args)
 
-            if command in command_mapping:
-                command_mapping[command](args, vectara_client)
-            else:
-                print(f"Unknown command: {command}")
-                print_help()
-        except ValueError as e:
-            print(e)
-            sys.exit(1)
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `vectara-cli-0.1.9/vectara_cli.egg-info/PKG-INFO` & `vectara-cli-0.2.0/vectara_cli.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectara-cli
-Version: 0.1.9
+Version: 0.2.0
 Summary: A CLI tool for interacting with the Vectara platform, including advanced text processing and indexing features.
 Home-page: https://git.tonic-ai.com/releases/vectara-cli
 Author: Tonic-AI
 Author-email: team@tonic-ai.com
 License: MIT
 Keywords: vectara search-engine document-indexing text-analysis information-retrieval natural-language-processing cli-tool data-science machine-learning text-processing
 Classifier: Programming Language :: Python :: 3
@@ -13,68 +13,252 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: requests
-Provides-Extra: advanced
-Requires-Dist: accelerate; extra == "advanced"
-Requires-Dist: torch>=1.8.0; extra == "advanced"
-Requires-Dist: transformers>=4.5.0; extra == "advanced"
-Requires-Dist: span_marker; extra == "advanced"
-Requires-Dist: spacy; extra == "advanced"
+Requires-Dist: argparse
+Provides-Extra: rebel-span
+Requires-Dist: accelerate; extra == "rebel-span"
+Requires-Dist: torch>=1.8.0; extra == "rebel-span"
+Requires-Dist: transformers>=4.5.0; extra == "rebel-span"
+Requires-Dist: span_marker; extra == "rebel-span"
+Requires-Dist: spacy; extra == "rebel-span"
 
 # vectara-cli
 
 `vectara-cli` is a Python package designed to interact with the Vectara platform, providing a command-line interface (CLI) and a set of APIs for indexing and querying documents, managing corpora, and performing advanced text analysis and processing tasks. This package is particularly useful for developers and data scientists working on search and information retrieval applications.
 
-## Features
+
+#### Features
 
 - Indexing text and documents into Vectara corpora.
 - Querying indexed documents.
 - Creating and deleting corpora.
-- Advanced text processing and analysis using pre-trained models (optional advanced package).
-
-## QuickStart
-
-get started with the [example_notebooks here](https://git.tonic-ai.com/releases/vectara-cli/examples/examples.ipynb) by downloading them and running them locally on any laptop.
+- Advanced text processing and analysis using pre-trained models (optional advanced package(s)).
 
-## Installation
 
 ### Basic Installation
 
 The basic installation includes the core functionality for interacting with the Vectara platform.
 
 ```bash
 pip install vectara-cli
 ```
 
-### Advanced Installation
+#### Advanced Installation
 
 The advanced installation includes additional dependencies for advanced text processing and analysis features. This requires PyTorch, Transformers, and Accelerate, which can be substantial in size.
 
 ```bash
-pip install vectara-cli[advanced]
+pip install vectara-cli[rebel_span]
 ```
 
 Ensure you have an appropriate PyTorch version installed for your system, especially if you're installing on a machine with GPU support. Refer to the [official PyTorch installation guide](https://pytorch.org/get-started/locally/) for more details.
 
-## Command Line Interface (CLI) Usage
+#### Command Line Interface (CLI) Usage
+
+The `vectara-cli` provides a powerful command line interface for interacting with the Vectara platform, enabling tasks such as document indexing, querying, corpus management, and advanced text processing directly from your terminal.
+
+Before your start always set your api keys with :
+
+```bash
+vectara set-api-keys <user_id> <api_key>
+```
+
+#### Deploy Your App
+
+- [x] **`vectara create-ui`:** This command will create a new UI for your app.
+
+**Note:** that this script assumes you have [Node.js and NPM installed](https://nodejs.org/en/download) on your system, as required by the npx command.
+
+<details>
+<summary> Table of Contents </summary>
 
-The `vectara-cli` provides a powerful command line interface for interacting with the Vectara platform, enabling tasks such as document indexing, querying, corpus management, and advanced text processing directly from your terminal. This section will guide you through the basics of using the `vectara-cli`.
+- **[Get started with the example_notebooks here](https://git.tonic-ai.com/releases/vectara-cli/examples/examples.ipynb)**
+- **[More About Configuration](https://git.tonic-ai.com/releases/vectara-cli/-/blob/devbranch/docs/configuration.md)**
+- **[Basic Usage CLI](https://git.tonic-ai.com/releases/vectara-cli/-/blob/devbranch/docs/basic_useage_cli.md?ref_type=heads)**
+- **[Programmatic Usage](https://git.tonic-ai.com/releases/vectara-cli/-/blob/devbranch/docs/basic_usage.md?ref_type=heads)**
+- **[Advanced Usage](https://git.tonic-ai.com/releases/vectara-cli/-/blob/devbranch/docs/advanced_usage.md?ref_type=heads)**
+- **[CONTRIBUTE](https://git.tonic-ai.com/releases/vectara-cli/-/blob/devbranch/CONTRIBUTE.md?ref_type=heads)**
+- **[Testing](https://git.tonic-ai.com/releases/vectara-cli/-/blob/devbranch/tests)**
 
-### Installation
+</details>
 
-Before using the CLI, ensure you have the package installed. You can install it directly from PyPi using pip:
+<details>
+<summary> Get Started </summary>
+
+#### Command Line Interface (CLI) Usage
+
+The `vectara-cli` provides a powerful command line interface for interacting with the Vectara platform, enabling tasks such as document indexing, querying, corpus management, and advanced text processing directly from your terminal.
+
+Before your start always set your api keys with :
 
 ```bash
-pip install vectara-cli
+vectara set-api-keys <user_id> <api_key>
+```
+
+## Basic Usage of Vectara CLI
+
+The Vectara CLI provides a simple and efficient way to interact with the Vectara platform, allowing users to create corpora, index documents, and perform various other operations directly from the command line. This section covers the basic usage of the Vectara CLI for common tasks such as creating a corpus and indexing documents.
+
+### Creating a Corpus
+
+To create a new corpus, you can use the `create-corpus` command. A corpus represents a collection of documents and serves as the primary organizational unit within Vectara.
+
+### Basic Corpus Creation
+
+```bash
+vectara create-corpus <corpus_id> <name> <description>
+```
+
+- `<corpus_id>`: The unique identifier for the corpus. Must be an integer.
+- `<name>`: The name of the corpus. This should be a unique name that describes the corpus.
+- `<description>`: A brief description of what the corpus is about.
+
+#### Example
+
+```bash
+vectara create-corpus 123 "My Corpus" "A corpus containing documents on topic XYZ"
+```
+
+This command creates a basic corpus with the specified ID, name, and description.
+
+### Indexing a Document
+
+To index a document into a corpus, you can use the `index-document` command. This command allows you to add a text document to the specified corpus, making it searchable within the Vectara platform.
+
+### Indexing Text
+
+```bash
+vectara index-text <corpus_id> <document_id> <text> <context> <metadata_json>
+```
+
+- `<corpus_id>`: The unique identifier for the corpus where the document will be indexed.
+- `<document_id>`: A unique identifier for the document being indexed.
+- `<text>`: The actual text content of the document that you want to index.
+- `<context>`: Additional context or information about the document.
+- `<metadata_json>`: A JSON string containing metadata about the document.
+
+#### Example
+
+```bash
+vectara index-text 12345 67890 "This is the text of the document." "Summary of the document" '{"author":"John Doe", "publishDate":"2024-01-01"}'
+```
+
+This command indexes a document with the provided text, context, and metadata into the specified corpus.
+
+### Advanced Corpus Creation
+
+For more advanced scenarios, you might want to specify additional options such as custom dimensions, filter attributes, or privacy settings for your corpus. The `create-corpus-advanced` command allows for these additional configurations.
+
+### Advanced Creation with Options
+
+```bash
+vectara create-corpus-advanced <name> <description> [options]
+```
+
+Options include setting custom dimensions, filter attributes, public/private status, and more.
+
+#### Example
+
+```bash
+vectara create-corpus-advanced "Research Papers" "Corpus for academic research papers" --custom_dimensions '{"dimension1": "value1", "dimension2": "value2"}' --filter_attributes '{"author": "John Doe"}'
+```
+
+This command creates a corpus with custom dimensions and filter attributes specified, allowing for more detailed organization and retrieval capabilities.
+
+### Deleting a Corpus
+
+To remove an existing corpus from the Vectara platform, you can use the `delete-corpus` command. Deleting a corpus will permanently remove the corpus and all documents contained within it. This action cannot be undone, so ensure that you really want to delete the corpus before proceeding.
+
+#### Basic Corpus Deletion
+
+```bash
+vectara delete-corpus <corpus_id>
+```
+
+- `<corpus_id>`: The unique identifier for the corpus you wish to delete. This must be an integer.
+
+#### Example
+
+```bash
+vectara delete-corpus 12345
+```
+
+This command deletes the corpus with the specified ID from the Vectara platform. Upon successful deletion, you will receive a confirmation message. If the corpus cannot be found or if there is an error during the deletion process, an error message will be displayed instead.
+
+### Uploading a Document
+
+To upload a document to a specific corpus in the Vectara platform, you can use the `upload-document` command. This allows you to add various types of documents, such as PDFs, Word documents, and plain text files, making them searchable within your corpus.
+
+#### Basic Document Upload
+
+```bash
+vectara upload-document <corpus_id> <file_path> [document_id]
+```
+
+- `<corpus_id>`: The unique identifier for the corpus where the document will be uploaded. This must be an integer.
+- `<file_path>`: The path to the document file that you want to upload.
+- `[document_id]`: An optional parameter that specifies the document ID. If not provided, Vectara will generate a unique ID for the document.
+
+#### Example
+
+```bash
+vectara upload-document 12345 "/path/to/document.pdf"
+```
+
+This command uploads a document from the specified file path to the corpus with the given ID. If the upload is successful, you will receive a confirmation message along with any relevant details provided by the Vectara platform.
+
+#### Uploading with a Specific Document ID
+
+If you wish to specify a document ID during the upload process, you can include it as an additional argument:
+
+```bash
+vectara upload-document 12345 "/path/to/document.pdf" "custom-document-id-123"
+```
+
+This allows you to assign a custom identifier to the document, which can be useful for tracking or referencing the document within your application or database.
+
+#### Supported Document Formats
+
+Vectara supports a variety of document formats for upload, including but not limited to:
+
+- PDF (.pdf)
+- Microsoft Word (.docx)
+- PowerPoint (.pptx)
+- Plain Text (.txt)
+
+Ensure that your documents are in one of the supported formats before attempting to upload them to the Vectara platform.
+
+#### Metadata and Context
+
+While the basic upload command does not include options for metadata and context, it's important to note that Vectara allows for the association of metadata with documents. This can be accomplished through advanced usage of the Vectara CLI or API, enabling you to provide additional information about the documents you upload, such as author, publication date, tags, and more.
+
+For detailed instructions on advanced document upload options, including how to include metadata and context, please refer to the Vectara documentation or the advanced usage section of the Vectara CLI help.
+
+
+#### Querying
+
+To perform a query in a specific corpus:
+
+```bash
+vectara query "<query_text>" <num_results> <corpus_id>
 ```
 
+- `<query_text>`: The text of the query.
+- `<num_results>`: The maximum number of results to return.
+- `<corpus_id>`: The ID of the corpus to query against.
+
+</details>
+
+<details>
+<summary>  Configuration </summary>
+
 ### Optional: Conda Virtual Environment Setup
 
 Conda is an open-source package management system and environment management system that runs on Windows, macOS, and Linux. It allows you to install, run, and update packages and their dependencies. To set up this project using Conda, follow the steps below:
 
 #### Prerequisites
 
 - Ensure that you have Conda installed on your system. If you do not have Conda installed, you can download it from the [official Conda website](https://www.anaconda.com/products/distribution).
@@ -85,25 +269,23 @@
 2. Navigate to the project directory where the `environment.yml` file is located.
 3. Create a new Conda environment by running the following command:
 
    ```bash
    conda env create -f environment.yml
    ```
 
-   This will create a new environment with the name specified in the `environment.yml` file and install all the required packages.
 
 #### Activating the Environment
 
 Once the environment is created, you can activate it using the following command:
 
 ```bash
-conda activate <env_name>
+conda activate vectara
 ```
 
-Replace `<env_name>` with the name of your Conda environment.
 
 #### Deactivating the Environment
 
 When you are done working on the project, you can deactivate the Conda environment by running:
 
 ```bash
 conda deactivate
@@ -120,19 +302,17 @@
 This will update the environment with any new dependencies specified in the `environment.yml` file.
 
 #### Removing the Environment
 
 If you wish to remove the Conda environment, you can do so with the following command:
 
 ```bash
-conda env remove -n <env_name>
+conda env remove -n vectara
 ```
 
-Again, replace `<env_name>` with the name of your Conda environment.
-
 By following these steps, you can manage your project's dependencies in an isolated environment using Conda.
 
 ### Configuration
 
 #### Setting Credentials via CLI Commands
 
 The `vectara-cli` tool now supports a convenient feature for setting your Vectara customer ID and API key directly through the command line. This method utilizes a command specifically designed for securely storing your credentials, making it easier to manage your Vectara configuration without manually setting environment variables or directly embedding your credentials in your scripts.
@@ -140,23 +320,23 @@
 #### Using the `set-api-keys` Command
 
 To set your Vectara customer ID and API key using the `vectara-cli`, you can use the `set-api-keys` command. This command stores your credentials securely, allowing `vectara-cli` to automatically use them for authentication in future operations.
 
 - **Syntax:** The command follows this simple syntax:
 
 ```bash
-vectara-cli set-api-keys <customer_id> <api_key>
+vectara set-api-keys <customer_id> <api_key>
 ```
 
 Replace `<customer_id>` with your Vectara customer ID and `<api_key>` with your Vectara API key.
 
 - **Example:**
 
 ```bash
-vectara-cli set-api-keys 123456789 abcdefghijklmnopqrstuvwxyz
+vectara set-api-keys 123456789 abcdefghijklmnopqrstuvwxyz
 ```
 
 After executing this command, you will see a confirmation message indicating that your API keys have been set successfully.
 
 #### Windows
 
 For Windows users, you can also set environment variables through the Command Prompt or PowerShell, or via the System Properties window.
@@ -177,67 +357,19 @@
 
 Note that changes made through the command line will only take effect in new instances of the terminal or command prompt.
 
 #### Using Credentials in `vectara-cli`
 
 Once you have set up your environment variables, `vectara-cli` will automatically use these credentials for authentication. There's no need to manually input your customer ID and API key each time you execute a command.
 
-### Basic Commands
-
+</details>
 
-#### Indexing a Document
+<details>
+<summary> Programmatic Usage </summary>
 
-To index a document into a specific corpus:
-
-```bash
-vectara-cli index-document <corpus_id> <document_id> "<title>" '<metadata_json>' "<section_text>"
-```
-
-- `<corpus_id>`: The ID of the corpus where the document will be indexed.
-- `<document_id>`: A unique identifier for the document.
-- `<title>`: The title of the document.
-- `<metadata_json>`: A JSON string containing document metadata.
-- `<section_text>`: The text content of the document.
-
-#### Querying
-
-To perform a query in a specific corpus:
-
-```bash
-vectara-cli query "<query_text>" <num_results> <corpus_id>
-```
-
-- `<query_text>`: The text of the query.
-- `<num_results>`: The maximum number of results to return.
-- `<corpus_id>`: The ID of the corpus to query against.
-
-#### Creating a Corpus
-
-To create a new corpus:
-
-```bash
-vectara-cli create-corpus <corpus_id> "<name>"
-```
-
-- `<corpus_id>`: The ID for the new corpus.
-- `<name>`: The name of the new corpus.
-
-#### Deleting a Corpus
-
-To delete an existing corpus:
-
-```bash
-vectara-cli delete-corpus <corpus_id>
-```
-
-- `<corpus_id>`: The ID of the corpus to delete.
-
-### Advanced Commands
-
-### Basic Usage
 
 #### Setting Up a Vectara Client
 
 First, initialize the Vectara client with your customer ID and API key. This client will be used for all subsequent operations.
 
 ```python
 from vectara_cli.core import VectaraClient
@@ -286,41 +418,14 @@
 num_results = 10  # Number of results to return
 corpus_id = 'your_corpus_id'
 
 results = vectara_client.query(query_text, num_results, corpus_id)
 print(results)
 ```
 
-#### Creating a Corpus
-
-You can create a new corpus by specifying its ID, name, description, and other settings.
-
-```python
-create_corpus_response = vectara_client.create_corpus(
-    corpus_id=123456789,
-    name="Example Corpus",
-    description="This is an example corpus.",
-    dtProvision=1234567890,
-    enabled=True,
-    swapQenc=False,
-    swapIenc=False,
-    textless=False,
-    encrypted=False,
-    encoderId="default",
-    metadataMaxBytes=10000,
-    customDimensions=[
-        {"name": "dimension1", "description": "First custom dimension", "servingDefault": 1.0, "indexingDefault": 1.0}
-    ],
-    filterAttributes=[
-        {"name": "filter1", "description": "First filter attribute", "indexed": True, "type": "FILTER_ATTRIBUTE_TYPE__UNDEFINED", "level": "FILTER_ATTRIBUTE_LEVEL__UNDEFINED"}
-    ]
-)
-print(create_corpus_response)
-```
-
 #### Deleting a Corpus
 
 To delete a corpus, you only need to provide its ID.
 
 ```python
 corpus_id = 'your_corpus_id'
 response, success = vectara_client.delete_corpus(corpus_id)
@@ -344,41 +449,47 @@
 try:
     response, status = vectara_client.upload_document(corpus_id, file_path, document_id, metadata)
     print("Upload successful:", response)
 except Exception as e:
     print("Upload failed:", str(e))
 ```
 
+</details>
+
+<details>
+<summary> Advanced Usage </summary>
+
+
 ### Advanced Usage
 
 
 To leverage the advanced text processing capabilities, ensure you have completed the advanced installation of `vectara-cli`. This includes the necessary dependencies for text analysis:
 
 ```bash
-pip install vectara-cli[advanced]
+pip install vectara-cli[rebel_span]
 ```
 
 #### Span Text Processing
 
 To process text using the Span model:
 
 ```bash
-vectara-cli span-text "<text>" "<model_name>" "<model_type>"
+vectara span-text "<text>" "<model_name>" "<model_type>"
 ```
 
 - `<text>`: The text to process.
 - `<model_name>`: The name of the Span model to use.
 - `<model_type>`: The type of the Span model.
 
 #### Enhanced Batch Processing with NerdSpan
 
 To process and upload documents from a folder:
 
 ```bash
-vectara-cli nerdspan-upsert-folder "<folder_path>" "<model_name>" "<model_type>"
+vectara nerdspan-upsert-folder "<folder_path>" "<model_name>" "<model_type>"
 ```
 
 - `<folder_path>`: The path to the folder containing documents to process and upload.
 - `<model_name>`: The name of the model to use for processing.
 - `<model_type>`: The type of the model.
 
 For more advanced processing and upsert operations, including using the Rebel model for complex document analysis and upload, refer to the specific command documentation provided with the CLI.
@@ -396,28 +507,28 @@
 >> **- supported models:** `science` and `keyphrase`
 
 - **Upload Enriched Text**
 
   To upload text that has been enriched with additional metadata:
 
   ```bash
-  vectara-cli upload-enriched-text <corpus_id> <document_id> <model_name> "<text>"
+  vectara upload-enriched-text <corpus_id> <document_id> <model_name> "<text>"
   ```
 
   - `<corpus_id>`: The ID of the corpus where the document will be uploaded.
   - `<document_id>`: A unique identifier for the document.
   - `<model_name>`: The name of the model used for text enrichment. `science` or `keyphrase`
   - `<text>`: The text content to be enriched and uploaded.
 
 - **Span Enhance Folder**
 
   To process and upload all documents within a folder, enhancing them using a specified model:
 
   ```bash
-  vectara-cli span-enhance-folder <corpus_id_1> <corpus_id_2> <model_name> "<folder_path>"
+  vectara span-enhance-folder <corpus_id_1> <corpus_id_2> <model_name> "<folder_path>"
   ```
 
   - `<corpus_id_1>`: The ID for the corpus to upload plain text documents.
   - `<corpus_id_2>`: The ID for the corpus to upload enhanced text documents.
   - `<model_name>`: The name of the model used for document enhancement. **supported models :** `science` and `keyphrase`
   - `<folder_path>`: The path to the folder containing the documents to be processed.
 
@@ -457,15 +568,15 @@
 This example showcases how to enrich text with additional metadata using the `EnterpriseSpan` class and upload it to a specified corpus in Vectara. By leveraging advanced models for text processing, users can significantly enhance the quality and relevance of their search and retrieval operations on the Vectara platform.
 
 ### Non-Commercial Advanced Usage
 
 The advanced features allow you to enrich your indexes with additional information automatically. This should produce better results for retrieval.
 
 
-![The mRebel pre-trained model is able to extract triplets for up to 400 relation types from Wikidata](https://git.tonic-ai.com/releases/vectara-cli/res/images/image.png?ref_type=heads)
+![Span Models for Named Entity Recognition](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/image.png?ref_type=heads)
 
 ### Non-Commercial Advanced Usage Using Span Models
 
 The `vectara-cli` package extends its functionality through the advanced usage of Span Models, enabling users to perform sophisticated text analysis and entity recognition tasks. This feature is particularly beneficial for non-commercial applications that require deep understanding and processing of textual data.
 
 The `Span` class supports processing and indexing documents from a folder, enabling batch operations for efficiency. This feature allows for the automatic extraction of entities from multiple documents, which are then indexed into specified corpora with enriched metadata.
 
@@ -517,16 +628,17 @@
     vectara_client.index_text(corpus_id, document_id, text, metadata_json=metadata_json)
     ```
 
 **Reference:** Aarsen, T. (2023). SpanMarker for Named Entity Recognition. Radboud University. Supervised by Prof. Dr. Fermin Moscoso del Prado Martin (fermin.moscoso-del-prado@ru.nl) and Dr. Daniel Vila Suero (daniel@argilla.io). Second assessor: Dr. Harrie Oosterhuis (harrie.oosterhuis@ru.nl).
 
 #### Non-Commercial Advanced Rag Using Rebel
 
-![mRebel](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/Screenshot_2024-04-05_112158.png?ref_type=heads)
-![Span Models for Named Entity Recognition](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/Screenshot_2024-04-05_112142.png?ref_type=heads)
+![mRebel](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/Screenshot_2024-04-05_112158.png)
+
+![The mRebel pre-trained model is able to extract triplets for up to 400 relation types from Wikidata](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/Screenshot_2024-04-05_112142.png)
 
 The mRebel pre-trained model is able to extract triplets for up to 400 relation types from Wikidata.
 
 
 Use the use the `Rebel Class` for advanced indexing. This will automatically extract `named entities`, `key phrases`, and other relevant information from your documents : 
 
 
@@ -554,23 +666,148 @@
     print(f"Document ID: {result['documentIndex']}, Score: {result['score']}, Text: {result['text'][:100]}...")
 
 print("\n=== Enhanced Results ===")
 for result in enhanced_results:
     print(f"Document ID: {result['documentIndex']}, Score: {result['score']}, Text: {result['text'][:100]}...")
 ```
 
-## Contributing
+</details>
+
+<details>
+<summary> Contributing </summary>
+
+# Contributing Guidelines for vectara-cli
+
+Thank you for your interest in contributing to `vectara-cli`! As an open-source project, we welcome contributions from developers of all skill levels. This guide will provide you with information on how to contribute effectively and make a valuable impact on the project.
+
+## Prerequisites
+
+Before you begin, ensure you have the following installed:
+
+- Python (preferably the latest Python 3 version)
+- Conda (for managing environments)
+- Git (for version control)
 
-Contributions to `vectara-cli` are welcome! Please refer to the contributing guidelines in the repository for more information on how to contribute.
+## Identify An Issue
 
+Browse the [Issues](https://git.tonic-ai.com/contribute/vectara/vectara-cli/issues) to find tasks to work on. You can start with issues labeled as "good first issue".
+- If you have an idea or a bug fix that is not listed, feel free to open a new issue to discuss it with other contributors.
 
-### Contributing to Advanced Features
+## Setting Up for Contribution
+
+1. **Fork the Repository**: Visit [vectara-cli on GitLab](https://git.tonic-ai.com/contribute/vectara/vectara-cli/) and fork the project to your account.
+
+2. **Create a New Branch**: Before you start making changes, switch to the `devbranch` and create a new branch for your feature or fix. We encourage naming your branch in a way that reflects the issue or feature you're working on.
+
+    ```bash
+    git checkout devbranch
+    git checkout -b feature/your-feature-name
+    ```
+    Or, if you're working on a specific issue:
+
+    ```bash
+    git checkout devbranch
+    git checkout -b issue/ISSUE_NUMBER-short-description
+    ```
 
-We welcome contributions to improve and expand the advanced features of `vectara-cli`. Whether it's adding new models, enhancing existing functionalities, or fixing bugs, your contributions are valuable to us. Please refer to our contributing guidelines for more information on how to contribute.
+    This naming convention (`feature/your-feature-name` or `issue/ISSUE_NUMBER-short-description`) helps in identifying branches with their purposes, making collaboration and review processes more efficient.
+
+- the easiest way to make a correctly named branch is to use the gitlab gui directly inside the issue that you are responding to.
+
+![easily use the GUI to make a branch](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/contributingimage.png)
+
+
+3. **Create and Activate Conda Environment**:
+
+   ```bash
+   conda env create -f environment.yml
+   conda activate vectara-cli
+   ```
+
+4. **Install the Project in Editable Mode**:
+
+   ```bash
+   pip install --editable .
+   ```
 
-## License
+## Develop
 
-`vectara-cli` is MIT licensed. See the [LICENSE](LICENSE.md) file for more details.
+- **Add Functionality**: Write your code and add it to the appropriate directory:
+  - For new functionalities, add your code in `./vectara_cli/commands`.
+  - Add command line functionality in `main.py`.
+  - Create or modify data objects in `./vectara_cli/data`.
 
----
+- **Add Help Text**: Update help texts in `./vectara_cli/help_texts/help_text.py` to reflect your changes or new commands.
 
-This README provides a comprehensive guide for installing and using the `vectara-cli` package. For further information or assistance, please refer to the [Vectara documentation](https://docs.vectara.com) or submit an issue on the [GitLab repository](https://git.tonic-ai.com/releases/vectara-cli/).
+## Write Tests
+
+- Add tests for your new functionalities in the `tests/` directory.
+- Ensure all tests pass by running them locally.
+
+## Document Your Changes
+
+Update any documentation relevant to your changes, including inline comments and README if necessary.
+
+## Submitting Your Contributions
+
+1. **Commit Your Changes**: After making your changes, commit them to your branch. Use descriptive commit messages that explain the "why" and "what" of your changes. This practice helps reviewers understand your reasoning and the context of your contributions.
+
+    ```bash
+    git add .
+    git commit -m "A descriptive message explaining the change"
+    ```
+
+2. **Push Your Changes**: Once you're ready, push your changes to your forked repository on GitLab.
+
+    ```bash
+    git push origin feature/your-feature-name
+    ```
+    
+    Or, if you're working on an issue:
+
+    ```bash
+    git push origin issue/ISSUE_NUMBER-short-description
+    ```
+
+### 3. Create a Merge Request
+- Go to the [Merge Requests](https://git.tonic-ai.com/contribute/vectara/vectara-cli/-/merge_requests) page.
+- Create a new merge request, compare your feature branch to the main repository's `devbranch`.
+- Fill in a detailed description of your changes and link to any relevant issues.
+
+## Review Process
+Once your merge request is submitted:
+- The project maintainers will review your code and may request changes.
+- Collaborate on modifications and push updates to your branch accordingly.
+- Once approved, a maintainer will merge your changes into the main codebase.
+
+## Post-merge
+After your changes have been merged:
+- Sync your fork with the original repository.
+- Consider deleting your branch to keep your fork clean:
+  ```bash
+  git branch -d your-feature-branch
+  git push origin --delete your-feature-branch
+  ```
+
+Thank you for contributing to `vectara-cli`! For any questions or further discussions, please reach out on the issues page or [on discord](https://discord.gg/7H4SKQekKe).
+
+- **[CONTRIBUTE](https://git.tonic-ai.com/releases/vectara-cli/-/blob/devbranch/CONTRIBUTE.md?ref_type=heads)**
+- **[Testing](https://git.tonic-ai.com/releases/vectara-cli/-/blob/devbranch/tests)**
+
+</details>
+
+<details><summary>License</summary>
+
+`vectara-cli` is MIT licensed. See the [LICENSE](https://git.tonic-ai.com/releases/vectara-cli/-/blob/devbranch/LICENSE.md?ref_type=heads) file for more details.
+
+</details>
+
+```
+@misc{Vectara Cli,
+  author = { isayahc , Josephrp, p3nGu1nZz},
+  title = {Vectara Cli is a Python package for Vectara platform interaction, ideal for search and information retrieval tasks.},
+  year = {2024},
+  publisher = {TeamTonic},
+  journal = {Tonic-AI repository},
+  howpublished = {\url{https://git.tonic-ai.com/releases/vectara-cli}}
+}
+```
```

### Comparing `vectara-cli-0.1.9/vectara_cli.egg-info/SOURCES.txt` & `vectara-cli-0.2.0/vectara_cli.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,55 @@
 LICENSE.md
 README.md
 setup.py
+tests/test_LocalVectaraClient.py
+tests/test_advanced_query.py
+tests/test_command_mapping.py
+tests/test_config_manager.py
+tests/test_create_corpus.py
+tests/test_delete_corpus.py
+tests/test_index_document.py
+tests/test_main.py
 vectara_cli/__init__.py
-vectara_cli/config_manager.py
 vectara_cli/core.py
-vectara_cli/corpus_data.py
-vectara_cli/custom_dimension.py
-vectara_cli/defaults.py
-vectara_cli/filter_attribute.py
 vectara_cli/main.py
-vectara_cli/utils.py
 vectara_cli.egg-info/PKG-INFO
 vectara_cli.egg-info/SOURCES.txt
 vectara_cli.egg-info/dependency_links.txt
 vectara_cli.egg-info/entry_points.txt
 vectara_cli.egg-info/requires.txt
 vectara_cli.egg-info/top_level.txt
-vectara_cli/advanced/__init__.py
-vectara_cli/advanced/commercial/__init__.py
-vectara_cli/advanced/commercial/enterprise.py
-vectara_cli/advanced/noncommercial/__init__.py
-vectara_cli/advanced/noncommercial/nerdspan.py
-vectara_cli/advanced/noncommercial/rebel.py
 vectara_cli/commands/__init__.py
+vectara_cli/commands/advanced_query.py
 vectara_cli/commands/create_corpus.py
 vectara_cli/commands/delete_corpus.py
 vectara_cli/commands/index_document.py
 vectara_cli/commands/index_text.py
 vectara_cli/commands/nerdspan_upsert_folder.py
 vectara_cli/commands/query.py
 vectara_cli/commands/rebel_upsert_folder.py
 vectara_cli/commands/span_enhance_folder.py
 vectara_cli/commands/span_text.py
+vectara_cli/commands/specialized_query.py
 vectara_cli/commands/upload_document.py
-vectara_cli/commands/upload_enriched_text.py
+vectara_cli/commands/upload_enriched_text.py
+vectara_cli/commands/upload_folder.py
+vectara_cli/data/__init__.py
+vectara_cli/data/corpus_data.py
+vectara_cli/data/custom_dimension.py
+vectara_cli/data/defaults.py
+vectara_cli/data/filter_attribute.py
+vectara_cli/data/metadata_handler.py
+vectara_cli/data/query_request.py
+vectara_cli/data/query_response.py
+vectara_cli/helptexts/__init__.py
+vectara_cli/helptexts/help_text.py
+vectara_cli/rebel_span/__init__.py
+vectara_cli/rebel_span/commercial/__init__.py
+vectara_cli/rebel_span/commercial/enterprise.py
+vectara_cli/rebel_span/noncommercial/__init__.py
+vectara_cli/rebel_span/noncommercial/nerdspan.py
+vectara_cli/rebel_span/noncommercial/rebel.py
+vectara_cli/utils/__init__.py
+vectara_cli/utils/config_manager.py
+vectara_cli/utils/create_ui.py
+vectara_cli/utils/utils.py
```

