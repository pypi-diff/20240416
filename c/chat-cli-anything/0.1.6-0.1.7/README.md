# Comparing `tmp/chat_cli_anything-0.1.6.tar.gz` & `tmp/chat_cli_anything-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat_cli_anything-0.1.6.tar", max compression
+gzip compressed data, was "chat_cli_anything-0.1.7.tar", max compression
```

## Comparing `chat_cli_anything-0.1.6.tar` & `chat_cli_anything-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2024-03-13 16:33:27.236056 chat_cli_anything-0.1.6/LICENSE
--rw-r--r--   0        0        0     7930 2024-04-07 09:17:05.654963 chat_cli_anything-0.1.6/README.md
--rw-r--r--   0        0        0        0 2024-03-20 12:50:07.078680 chat_cli_anything-0.1.6/chat_cli_anything/__init__.py
--rw-r--r--   0        0        0    30203 2024-04-07 11:22:53.916737 chat_cli_anything-0.1.6/chat_cli_anything/ask.py
--rw-r--r--   0        0        0     7015 2024-04-07 11:13:51.883055 chat_cli_anything-0.1.6/chat_cli_anything/config.py
--rw-r--r--   0        0        0     7876 2024-04-03 09:16:53.301015 chat_cli_anything-0.1.6/chat_cli_anything/db.py
--rw-r--r--   0        0        0     1621 2024-04-03 09:17:55.507727 chat_cli_anything-0.1.6/chat_cli_anything/embedding.py
--rw-r--r--   0        0        0     2798 2024-04-03 06:48:40.337190 chat_cli_anything-0.1.6/chat_cli_anything/loader.py
--rw-r--r--   0        0        0     2695 2024-04-07 11:06:03.928644 chat_cli_anything-0.1.6/chat_cli_anything/request.py
--rw-r--r--   0        0        0      729 2024-03-31 17:35:50.217211 chat_cli_anything-0.1.6/chat_cli_anything/rerank.py
--rw-r--r--   0        0        0     1868 2024-04-01 08:49:00.737620 chat_cli_anything-0.1.6/chat_cli_anything/service.py
--rw-r--r--   0        0        0     1050 2024-04-07 11:16:54.254791 chat_cli_anything-0.1.6/chat_cli_anything/util.py
--rw-r--r--   0        0        0     1466 2024-04-07 11:23:38.398822 chat_cli_anything-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     9464 1970-01-01 00:00:00.000000 chat_cli_anything-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-13 16:33:27.236056 chat_cli_anything-0.1.7/LICENSE
+-rw-r--r--   0        0        0     7930 2024-04-07 09:17:05.654963 chat_cli_anything-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2024-03-20 12:50:07.078680 chat_cli_anything-0.1.7/chat_cli_anything/__init__.py
+-rw-r--r--   0        0        0    32639 2024-04-15 11:33:17.045968 chat_cli_anything-0.1.7/chat_cli_anything/ask.py
+-rw-r--r--   0        0        0     9641 2024-04-16 14:34:55.649939 chat_cli_anything-0.1.7/chat_cli_anything/config.py
+-rw-r--r--   0        0        0     8305 2024-04-15 11:24:08.954963 chat_cli_anything-0.1.7/chat_cli_anything/db.py
+-rw-r--r--   0        0        0     1583 2024-04-15 09:35:00.631353 chat_cli_anything-0.1.7/chat_cli_anything/embedding.py
+-rw-r--r--   0        0        0     2798 2024-04-03 06:48:40.337190 chat_cli_anything-0.1.7/chat_cli_anything/loader.py
+-rw-r--r--   0        0        0     2695 2024-04-07 11:06:03.928644 chat_cli_anything-0.1.7/chat_cli_anything/request.py
+-rw-r--r--   0        0        0      900 2024-04-15 02:15:43.665432 chat_cli_anything-0.1.7/chat_cli_anything/rerank.py
+-rw-r--r--   0        0        0     1868 2024-04-01 08:49:00.737620 chat_cli_anything-0.1.7/chat_cli_anything/service.py
+-rw-r--r--   0        0        0     1067 2024-04-09 05:24:26.253738 chat_cli_anything-0.1.7/chat_cli_anything/util.py
+-rw-r--r--   0        0        0     1437 2024-04-16 14:37:03.981815 chat_cli_anything-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     9464 1970-01-01 00:00:00.000000 chat_cli_anything-0.1.7/PKG-INFO
```

### Comparing `chat_cli_anything-0.1.6/LICENSE` & `chat_cli_anything-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `chat_cli_anything-0.1.6/README.md` & `chat_cli_anything-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `chat_cli_anything-0.1.6/chat_cli_anything/ask.py` & `chat_cli_anything-0.1.7/chat_cli_anything/ask.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 import socket
 import requests
 import os
 import json
 import psutil
 from chat_cli_anything.config import Config
 from chat_cli_anything.request import build_client, stream_predict, predict
-from typing import Dict, Any, Union, Optional, List, TypeVar, Sequence
+from typing import Dict, Any, Union, Optional, List, TypeVar, Sequence, Tuple
 from copy import deepcopy
 from chat_cli_anything.util import parse_markdown_codeblock, cache_path
+from chat_cli_anything.service import SERVICE_NAME
 from rich.console import Console
 from rich.markdown import Markdown
 from rich.live import Live
 import sys
 
 FAISS = TypeVar("FAISS")
 
@@ -433,75 +434,82 @@
 @click.group(name='cc-db')
 def db():
     """Manage document database."""
     pass
 
 @click.group(name='cc-service')
 def service():
-    """Manage service"""
+    """Manage local embedding and rerank services."""
     pass
 
 
 filename = click.argument('filename', required=False, default='')
 object_name = click.option('-o', '--object-name', required=False, default='')
 continue_generate = click.option('-c', '--continue-generate', is_flag=True)
+config_type = click.option('-t', '--config-type', type=str, default='llm', help='Config type, "llm" or "embedding"')
 
 
 @config.command()
 @click.argument('name', default=None)
 @click.argument('base-url', default=None)
 @click.option('--model', default='Empty')
 @click.option('--api-key', default='Empty', envvar="OPENAI_API_KEY")
 @click.option('--max-tokens', default=4096)
-@click.option('--proxy')
+@click.option('--proxy', default='')
+@config_type
 def add(name: Union[str, None], base_url: Union[str, None],
-        api_key: str, model: str, max_tokens: int, proxy: Optional[str] = None):
+        api_key: str, model: str, max_tokens: int, proxy: Optional[str], config_type: str):
     """Add a new configuration."""
     if name is None:
         name = click.prompt('Enter base name')
     if base_url is None:
         base_url = click.prompt('Enter the url')
 
     config = Config()
-    config.add(name, base_url, api_key, model, max_tokens, proxy)
+    config.add(name, base_url, api_key, model, max_tokens, proxy, config_type)
     click.echo(f"Configuration '{name}' added successfully.")
 
 
+
 @config.command()
 @click.argument('name')
 @click.option('-a', '--all', is_flag=True, help='Remove all providers')
-def remove(name: str, all: bool):
+@config_type
+def remove(name: str, all: bool, config_type: str):
     """Remove a configuration."""
     config = Config()
-    config.remove(name, all)
+    config.remove(name, all, config_type)
 
 
 @config.command()
 @click.argument('name', required=False, default='')
 @click.option('-s', '--show-api-key', is_flag=True)
-def list(name: str, show_api_key: bool):
+@click.option('-t', '--config-type', type=str, default='all', help='Config type.')
+def list(name: str, show_api_key: bool, config_type: str):
     """List configurations. The active provider will be marked with '*'."""
     config = Config()
-    config.list(name, api_key=show_api_key)  # Set api_key to True or False based on your preference
+    config.list(name, api_key=show_api_key, config_type=config_type)  # Set api_key to True or False based on your preference
 
 
 @config.command()
 @click.argument('name', required=True)
-def switch(name: str):
+@config_type
+def switch(name: str, config_type: str):
     """Switch to a different configuration and save the change."""
     config = Config()
-    config.switch(name)
+    config.switch(name, config_type)
 
 
 @config.command()
 @click.argument('name', required=True)
-def ping(name: str):
+@config_type
+def ping(name: str, config_type: str):
     """Ping provider."""
     config = Config()
-    config.ping(name)
+    config.ping(name, config_type)
 
 
 @config.command()
 @click.argument('path', required=True)
 @click.option('-o', '--override', is_flag=True, help='Whether override existing file.')
 def dump(path: str, override: bool):
     """Export current configurations."""
@@ -529,15 +537,17 @@
     interface.check_active_config_exists()
 
     if db is not None:
         from chat_cli_anything.db import load_vectorstore
         _db = db
         status, db = load_vectorstore(db)
         if status:
-            check_and_start_service()
+            if not _service_is_running():
+                click.secho(f'{SERVICE_NAME} is not running. Add using `cc-config` or start local embedding service using `cc-db`.', fg='red')
+                return
         else:
             click.secho(f"The '{_db}' does not exist.", fg='red')
             return
     interface.ask(query, 'chat', filename, db, rerank, show_chunks, advance=advance)
 
 
 @cli.command(name='cc-chat')
@@ -558,15 +568,17 @@
     interface.check_active_config_exists()
 
     if db is not None:
         from chat_cli_anything.db import load_vectorstore
         _db = db
         status, db = load_vectorstore(db)
         if status:
-            check_and_start_service()
+            if not _service_is_running():
+                click.secho(f'{SERVICE_NAME} is not running. Add using `cc-config` or start local embedding service using `cc-db`.', fg='red')
+                return
         else:
             click.secho(f"The {_db} is not exists.", fg='red')
             return
     if show_history:
         interface.show_chat_history()
     elif clear:
         interface.clear_chat_history()
@@ -668,15 +680,17 @@
 @click.option('-n', '--name', help='The name of the knowledge base.')
 @click.option('-m', '--comment', default='', help='Add comment to info')
 def ingest(files: str, name: str, comment: str):
     """Read documents and convert it searchable database."""
     from chat_cli_anything.loader import parse_files
     from chat_cli_anything.db import create_vectorstore, _generate_name
 
-    check_and_start_service()
+    if not _service_is_running():
+        click.secho(f'{SERVICE_NAME} is not accessible.', fg='red')
+        return
 
     click.echo('Collecting documents')
     docs, hash_files_processed = [], {}
     for f in files:
         res = parse_files(f)
         if res:
             _docs, _files_processed = res
@@ -729,55 +743,80 @@
 @click.option('-k', '--topk', type=int, default=5, help='Number of top results to return.')
 def search(db: str, query: str, topk: int):
     """Search in database."""
     from chat_cli_anything.db import load_vectorstore
     _db = db
     status, db = load_vectorstore(db)
     if status:
-        check_and_start_service()
+        if not _service_is_running():
+            click.secho(f'{SERVICE_NAME} is not running. Add using `cc-config` or start local embedding service using `cc-db`.', fg='red')
+            return
     else:
         click.secho(f"The '{_db}' does not exist.", fg='red')
     search_result = db.similarity_search(query, k=topk)
     for i, result in enumerate(search_result):
         click.echo(f"{i+1}. \n {result.page_content}")
 
-def _check_port_is_accessible(port: int):
+def _check_port_is_accessible(url: str, port: int):
     with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
         try:
             s.connect(('localhost', port))
             return True
         except ConnectionRefusedError:
             return False
 
-def _is_excepted_service_type(port: int, service_name: str):
+def _is_excepted_service_type(url: str, port: int, service_name: str):
     try:
-        response = requests.get(f'http://localhost:{port}/ping', timeout=1)
+        response = requests.get(f'{url}:{port}/ping', timeout=2)
         if response.json()['service_name'] == service_name:
             return True
         return False
     except Exception as ex:
         print(ex)
         return False
 
-def check_and_start_service():
-    """
-    """
+
+def _split_url(url: str) -> Tuple[str, int]:
+    """"""
+    items = url.strip('/').split(':')
+    return ':'.join(items[:-1]), int(items[-1])
+
+
+def _service_is_running():
+    """"""
     from chat_cli_anything.service import SERVICE_NAME
     config = Config()
-    port = config.config.get('local_service_port', Config.DEFAULT_PORT)
+    active_embedding = config.get('active_embedding', None)
+
+    if not active_embedding:
+        click.secho(f'{SERVICE_NAME} is not configured.', fg='red')
+
+    base_url = config.get('embeddings')[active_embedding]['base_url']
+    url, port = _split_url(base_url)
+
+    if _is_excepted_service_type(url, port, SERVICE_NAME):
+        return True
+
+    port = config.get('local_service_port', Config.DEFAULT_PORT) 
+    if _is_excepted_service_type('http://localhost', port, SERVICE_NAME):
+        return True
+    return False
+
 
+def _start_local_service():
+    """"""
+    port = Config().get('local_service_port', Config.DEFAULT_PORT)
 
     need_created = True
-    if _check_port_is_accessible(port):
-        if _is_excepted_service_type(port, SERVICE_NAME):
-            click.secho(f'{SERVICE_NAME} is already running background.')
-            need_created = False
-        else:
-            click.secho(f'{port} has been used .')
-            port += port
+    if _service_is_running():
+        click.secho(f'{SERVICE_NAME} is already running.')
+        need_created = False
+
+    while _check_port_is_accessible('http://localhost', port):
+        port += 1
 
     if need_created:
         # start service in backend with detach from current host
         import shlex
         import subprocess
         cmds = "{} -m chat_cli_anything.service {}".format(sys.executable, port)
         # cmds = "{} -m cli-chat.chat_cli_anything.service {}".format(sys.executable, port)
@@ -787,58 +826,83 @@
         config.save()
         click.secho(f'{SERVICE_NAME} is running background.')
 
 
 def show_service():
     from chat_cli_anything.service import SERVICE_NAME
     config = Config()
-    port = config.config.get('local_service_port', Config.DEFAULT_PORT)
-    if _check_port_is_accessible(port) and _is_excepted_service_type(port, SERVICE_NAME):
-        click.secho(f'Service is running on local port ' + click.style(f'{port}', fg='green') + f', check http://localhost:{port}/docs for more inforamtion.')
+    active_embedding = config.get('active_embedding', None)
+
+    if not active_embedding:
+        click.secho(f'{SERVICE_NAME} is not configured.', fg='red')
+
+    base_url = config.get('embeddings')[active_embedding]['base_url']
+    url, port = _split_url(base_url)
+
+    if _is_excepted_service_type(url, port, SERVICE_NAME):
+        click.secho(f'Service is running on {url}' + click.style(f'{port}', fg='green') + f', check {url}:{port}/docs for more inforamtion.')
     else:
-        click.echo(f'Service is not running on local machine.')
+        click.echo(f'Service is not running on {url}:{port}.')
 
 
 def stop_service():
     from chat_cli_anything.service import SERVICE_NAME
-    config = Config()
-    port = config.config.get('local_service_port', Config.DEFAULT_PORT)
+    port = Config().get('local_server_port', Config.DEFAULT_PORT)
+    url = 'http://localhost'
+
 
-    if _check_port_is_accessible(port) and _is_excepted_service_type(port, SERVICE_NAME):
+    if (_check_port_is_accessible(url, port) and 
+        _is_excepted_service_type(url, port, SERVICE_NAME)):
         # get pid of process listened on given port
         import psutil
         import signal
 
-        def get_pid_listening_port(port):
+        def get_pid_listening_port(port) -> List[int]:
             pid_list = []
             for proc in psutil.process_iter(['pid', 'name', 'connections']):
                 conns = proc.info.get('connections', []) or []
                 for conn in conns:
                     if conn.status == psutil.CONN_LISTEN and conn.laddr.port == port:
                         pid_list.append(proc.info['pid'])
             return pid_list
-        
+
         pid = get_pid_listening_port(port)[0]
         os.kill(pid, signal.SIGTERM)
-        click.secho('Process is killed')
+        click.secho('Local service stopped.')
     else:
-        click.secho('Service is not running.')
+        click.secho('Not local service is running.')
+
 
 @service.command(name='start')
 def start():
-    check_and_start_service()
+    input = 'y'
+
+    if _service_is_running():
+        config = Config()
+        active_embedding = config.get('active_embedding', None)
+        base_url = config.get('embeddings')[active_embedding]['base_url']
+        click.secho(f'{SERVICE_NAME} is already running on {base_url}.')
+        input = click.prompt('Do you want to start a service locally?[y/n]', type=str)
+
+    if input == 'y':
+        _start_local_service()
+        click.secho(f"Service is starting backend. It may take while, use cc-db status check status.")
+
 
 @service.command(name='stop')
 def stop():
+    """Stop local embedding service."""
     stop_service()
 
+
 @service.command(name='status')
 def status():
     show_service()
 
+
 @cli.command(name='cc-info')
 def info():
     # list db path
     from chat_cli_anything.db import DB_PATH
     click.secho('db path: {}'.format(DB_PATH))
     # list config path
     click.secho('config path: {}'.format(Config.CONFIG_PATH))
```

### Comparing `chat_cli_anything-0.1.6/chat_cli_anything/db.py` & `chat_cli_anything-0.1.7/chat_cli_anything/db.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from pathlib import Path
 from hashlib import md5
 from typing import List, Dict, Any, Sequence, Optional, Tuple
 import json
 from copy import deepcopy
 from chat_cli_anything.util import cache_path, calculate_hash
 from chat_cli_anything.config import Config
+from chat_cli_anything.service import SERVICE_NAME
 from pydantic import BaseModel
 from langchain_community.vectorstores import FAISS
 from langchain.docstore.document import Document
 from datetime import datetime
 from tabulate import tabulate
 from sqlalchemy import create_engine, Column, Integer, String, ForeignKey
 from sqlalchemy.ext.declarative import declarative_base
@@ -169,23 +170,30 @@
 ):
     """
     docs:
     files_processed:
     """
     Session = sessionmaker(bind=engine)
     session = Session()
-    embedding_model = LocalEmbeddings(Config().get('local_server_port', Config.DEFAULT_PORT))
+    config = Config()
+    active_embedding = config.get('active_embedding', None)
+
+    if not active_embedding:
+        return False, 'No embedding is configured.'
+
+    base_url = config.get('embeddings')[active_embedding]['base_url']
+    embedding_model = LocalEmbeddings(base_url)
 
     inspector = Inspector.from_engine(engine)
     if 'document_set' in inspector.get_table_names():
         # check name not exists
         current_set_with_given_name = session.query(DocumentSetDB).filter(DocumentSetDB.name == name).first()
         print(name)
         if current_set_with_given_name:
-            return False, 'Name Already Exists.'
+            return False, 'Name already exists.'
 
     # from documents
     document_set = DocumentSetDB(name=name,
                                comment=comment,
                                created_time=datetime.now().strftime('%Y-%m-%d %H:%M:%S'))
     session.add(document_set)
 
@@ -216,15 +224,22 @@
     return True, 'Successfully created.'
 
 
 def load_vectorstore(name: str) -> Tuple[bool, Any]:
     """
     name: hash or store name
     """
-    embedding_model = LocalEmbeddings(Config().get('local_server_port', Config.DEFAULT_PORT))
+    config = Config()
+    active_embedding = config.get('active_embedding', None)
+
+    if not active_embedding:
+        return False, 'No embedding is configured.'
+
+    base_url = config.get('embeddings')[active_embedding]['base_url']
+    embedding_model = LocalEmbeddings(base_url)
     Session = sessionmaker(bind=engine)
     with Session() as session:
         # query from Document Set data base
         res = session.query(DocumentSetDB, SetOfDocumentDB, DocumentInfoDB).filter(DocumentSetDB.name == name, DocumentSetDB.name == SetOfDocumentDB.name, SetOfDocumentDB.hash == DocumentInfoDB.hash).all()
         if not res:
             return False, 'Document set not found.'
         else:
```

### Comparing `chat_cli_anything-0.1.6/chat_cli_anything/embedding.py` & `chat_cli_anything-0.1.7/chat_cli_anything/embedding.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,47 +10,47 @@
 
 
 def build_embedding_model():
     import torch
     from langchain_community.embeddings import HuggingFaceBgeEmbeddings
     """"""
     logger.info('Loading embedding model')
-    # model_name = "BAAI/bge-small-zh-v1.5"
-    model_name = "infgrad/stella-base-zh-v3-1792d"
+    model_name = "BAAI/bge-small-zh-v1.5"
+    # model_name = "infgrad/stella-base-zh-v3-1792d"
 
     if torch.cuda.is_available():
         device = "cuda"
     else:
         device = "cpu"
 
     model_kwargs = {"device": device}
     encode_kwargs = {"normalize_embeddings": True}
 
     embedding_model = HuggingFaceBgeEmbeddings(
         model_name=model_name,
         model_kwargs=model_kwargs,
-        encode_kwargs=encode_kwargs
+        encode_kwargs=encode_kwargs,
     )
     logger.info('Loading complete.')
     return embedding_model
 
 
 class LocalEmbeddings(Embeddings):
-    def __init__(self, port: int) -> None:
-        self.port = port
+    def __init__(self, url: str) -> None:
+        self.url = url
         super().__init__()
 
     def embed_documents(self, texts: List[str]) -> List[List[float]]:
         response = requests.post(
-            f'http://localhost:{self.port}/embed_documents',
+            f'{self.url}/embed_documents',
             timeout=10 * len(texts) + 10,
             json=[{'text': text} for text in texts]
         )
         return [r['embedding'] for r in response.json()]
 
     def embed_query(self, text: str) -> List[float]:
         response = requests.post(
-            f'http://localhost:{self.port}/embedding',
+            f'{self.url}/embedding',
             timeout=10,
             json={'text': text}
         )
         return response.json()['embedding']
```

### Comparing `chat_cli_anything-0.1.6/chat_cli_anything/loader.py` & `chat_cli_anything-0.1.7/chat_cli_anything/loader.py`

 * *Files identical despite different names*

### Comparing `chat_cli_anything-0.1.6/chat_cli_anything/request.py` & `chat_cli_anything-0.1.7/chat_cli_anything/request.py`

 * *Files identical despite different names*

### Comparing `chat_cli_anything-0.1.6/chat_cli_anything/service.py` & `chat_cli_anything-0.1.7/chat_cli_anything/service.py`

 * *Files identical despite different names*

### Comparing `chat_cli_anything-0.1.6/chat_cli_anything/util.py` & `chat_cli_anything-0.1.7/chat_cli_anything/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 LANGUAGES = [
     'python', 'javascript', 'typescript', 'cpp',
     'c', 'java', 'php', 'ruby', 'go', 'rust',
     'swift', 'kotlin', 'scala', 'dart', 'rust',
     'lua', 'perl', 'groovy', 'haskell', 'pascal',
-    'basic', 'cobol', 'fortran', 'lisp'
+    'basic', 'cobol', 'fortran', 'lisp', 'shell', 'bash'
 ]
 
 def parse_markdown_codeblock(text: str) -> List[str]:
     """"""
     matched_str = re.findall('```(.*?)```', text, re.DOTALL)
     code_str: List[str] = []
     for s in matched_str:
```

### Comparing `chat_cli_anything-0.1.6/pyproject.toml` & `chat_cli_anything-0.1.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chat-cli-anything"
-version = "0.1.6"
+version = "0.1.7"
 description = "Chat with anything on cli."
 authors = ["liuping <liuping@shukun.net>"]
 license = "Apache"
 readme = "README.md"
 keywords = ["chatgpt", "cli", "chat"]
 packages = [{ include = "chat_cli_anything" }]
 
@@ -16,18 +16,18 @@
 pypdf = "^4.1.0"
 fastapi = "^0.110.0"
 click = "^8.1.7"
 requests = "^2.31.0"
 psutil = "^5.9.8"
 tabulate = "^0.9.0"
 rich = "^13.7.1"
+langchain = "^0.1.13"
 langchain-core = "^0.1.36"
 uvicorn = "^0.29.0"
 langchain-community = {version = "^0.0.29", optional = true}
-langchain = {version = "^0.1.13", optional = true}
 flagembedding = {version = "^1.2.8", optional = true}
 torch = {version = ">=2.1.0", optional = true}
 langchain-openai = {version = "^0.1.1", optional = true}
 langchain-text-splitters = {version = "^0.0.1", optional = true}
 tiktoken = "^0.6.0"
 tqdm = "^4.66.2"
```

### Comparing `chat_cli_anything-0.1.6/PKG-INFO` & `chat_cli_anything-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-cli-anything
-Version: 0.1.6
+Version: 0.1.7
 Summary: Chat with anything on cli.
 License: Apache
 Keywords: chatgpt,cli,chat
 Author: liuping
 Author-email: liuping@shukun.net
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

