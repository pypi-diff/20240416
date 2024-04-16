# Comparing `tmp/aioipfs-0.6.7.tar.gz` & `tmp/aioipfs-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioipfs-0.6.7.tar", last modified: Thu Apr 11 09:59:15 2024, max compression
+gzip compressed data, was "aioipfs-0.6.8.tar", last modified: Tue Apr 16 21:29:11 2024, max compression
```

## Comparing `aioipfs-0.6.7.tar` & `aioipfs-0.6.8.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:59:15.002682 aioipfs-0.6.7/
--rw-rw-rw-   0 root         (0) root         (0)     7652 2024-04-11 09:58:33.000000 aioipfs-0.6.7/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       54 2024-04-11 09:58:33.000000 aioipfs-0.6.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6714 2024-04-11 09:59:15.002682 aioipfs-0.6.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4843 2024-04-11 09:58:33.000000 aioipfs-0.6.7/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:59:14.997682 aioipfs-0.6.7/aioipfs/
--rw-rw-rw-   0 root         (0) root         (0)    10725 2024-04-11 09:58:33.000000 aioipfs-0.6.7/aioipfs/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    58824 2024-04-11 09:58:33.000000 aioipfs-0.6.7/aioipfs/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:59:14.999682 aioipfs-0.6.7/aioipfs/apis/
--rw-rw-rw-   0 root         (0) root         (0)     7998 2024-04-11 09:58:33.000000 aioipfs-0.6.7/aioipfs/apis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6764 2024-04-11 09:58:33.000000 aioipfs-0.6.7/aioipfs/apis/dag.py
--rw-rw-rw-   0 root         (0) root         (0)     2109 2024-04-11 09:58:33.000000 aioipfs-0.6.7/aioipfs/apis/multibase.py
--rw-rw-rw-   0 root         (0) root         (0)    12594 2024-04-11 09:58:33.000000 aioipfs-0.6.7/aioipfs/apis/p2p.py
--rw-rw-rw-   0 root         (0) root         (0)     7602 2024-04-11 09:58:33.000000 aioipfs-0.6.7/aioipfs/apis/pin.py
--rw-rw-rw-   0 root         (0) root         (0)     6103 2024-04-11 09:58:33.000000 aioipfs-0.6.7/aioipfs/apis/pubsub.py
--rw-rw-rw-   0 root         (0) root         (0)     4769 2024-04-11 09:58:33.000000 aioipfs-0.6.7/aioipfs/apis/swarm.py
--rw-rw-rw-   0 root         (0) root         (0)     2443 2024-04-11 09:58:33.000000 aioipfs-0.6.7/aioipfs/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     6929 2024-04-11 09:58:33.000000 aioipfs-0.6.7/aioipfs/gitignore_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     5322 2024-04-11 09:58:33.000000 aioipfs-0.6.7/aioipfs/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    10771 2024-04-11 09:58:33.000000 aioipfs-0.6.7/aioipfs/multi.py
--rw-rw-rw-   0 root         (0) root         (0)     2371 2024-04-11 09:58:33.000000 aioipfs-0.6.7/aioipfs/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:59:15.000682 aioipfs-0.6.7/aioipfs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6714 2024-04-11 09:59:14.000000 aioipfs-0.6.7/aioipfs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      513 2024-04-11 09:59:14.000000 aioipfs-0.6.7/aioipfs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 09:59:14.000000 aioipfs-0.6.7/aioipfs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      316 2024-04-11 09:59:14.000000 aioipfs-0.6.7/aioipfs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-11 09:59:14.000000 aioipfs-0.6.7/aioipfs.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1825 2024-04-11 09:58:33.000000 aioipfs-0.6.7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 09:59:15.002682 aioipfs-0.6.7/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:59:14.999682 aioipfs-0.6.7/tests/
--rwxrwxrwx   0 root         (0) root         (0)    39157 2024-04-11 09:58:33.000000 aioipfs-0.6.7/tests/test_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 21:29:11.621747 aioipfs-0.6.8/
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2024-04-16 21:28:40.000000 aioipfs-0.6.8/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       54 2024-04-16 21:28:40.000000 aioipfs-0.6.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7627 2024-04-16 21:29:11.621747 aioipfs-0.6.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5502 2024-04-16 21:28:40.000000 aioipfs-0.6.8/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 21:29:11.616747 aioipfs-0.6.8/aioipfs/
+-rw-rw-rw-   0 root         (0) root         (0)    10795 2024-04-16 21:28:40.000000 aioipfs-0.6.8/aioipfs/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    59423 2024-04-16 21:28:40.000000 aioipfs-0.6.8/aioipfs/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 21:29:11.619747 aioipfs-0.6.8/aioipfs/apis/
+-rw-rw-rw-   0 root         (0) root         (0)     8143 2024-04-16 21:28:40.000000 aioipfs-0.6.8/aioipfs/apis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6802 2024-04-16 21:28:40.000000 aioipfs-0.6.8/aioipfs/apis/dag.py
+-rw-rw-rw-   0 root         (0) root         (0)     2109 2024-04-16 21:28:40.000000 aioipfs-0.6.8/aioipfs/apis/multibase.py
+-rw-rw-rw-   0 root         (0) root         (0)    12682 2024-04-16 21:28:40.000000 aioipfs-0.6.8/aioipfs/apis/p2p.py
+-rw-rw-rw-   0 root         (0) root         (0)     7641 2024-04-16 21:28:40.000000 aioipfs-0.6.8/aioipfs/apis/pin.py
+-rw-rw-rw-   0 root         (0) root         (0)     6161 2024-04-16 21:28:40.000000 aioipfs-0.6.8/aioipfs/apis/pubsub.py
+-rw-rw-rw-   0 root         (0) root         (0)     4769 2024-04-16 21:28:40.000000 aioipfs-0.6.8/aioipfs/apis/swarm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2443 2024-04-16 21:28:40.000000 aioipfs-0.6.8/aioipfs/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5484 2024-04-16 21:28:40.000000 aioipfs-0.6.8/aioipfs/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    10807 2024-04-16 21:28:40.000000 aioipfs-0.6.8/aioipfs/multi.py
+-rw-rw-rw-   0 root         (0) root         (0)     2403 2024-04-16 21:28:40.000000 aioipfs-0.6.8/aioipfs/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 21:29:11.619747 aioipfs-0.6.8/aioipfs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7627 2024-04-16 21:29:11.000000 aioipfs-0.6.8/aioipfs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      541 2024-04-16 21:29:11.000000 aioipfs-0.6.8/aioipfs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 21:29:11.000000 aioipfs-0.6.8/aioipfs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2024-04-16 21:29:11.000000 aioipfs-0.6.8/aioipfs.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      398 2024-04-16 21:29:11.000000 aioipfs-0.6.8/aioipfs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-16 21:29:11.000000 aioipfs-0.6.8/aioipfs.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2008 2024-04-16 21:28:40.000000 aioipfs-0.6.8/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 21:29:11.622747 aioipfs-0.6.8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 21:29:11.619747 aioipfs-0.6.8/tests/
+-rwxrwxrwx   0 root         (0) root         (0)    33305 2024-04-16 21:28:40.000000 aioipfs-0.6.8/tests/test_client.py
+-rwxrwxrwx   0 root         (0) root         (0)     1193 2024-04-16 21:28:40.000000 aioipfs-0.6.8/tests/test_helpers.py
```

### Comparing `aioipfs-0.6.7/LICENSE` & `aioipfs-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.7/PKG-INFO` & `aioipfs-0.6.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioipfs
-Version: 0.6.7
+Version: 0.6.8
 Summary: Asynchronous IPFS client library
 Author-email: cipres <alkaline@gmx.co.uk>
 License: LGPLv3
 Project-URL: Homepage, https://gitlab.com/cipres/aioipfs
 Keywords: asyncio,aiohttp,ipfs
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
@@ -31,24 +31,30 @@
 Requires-Dist: py-multibase>=1.0.3
 Requires-Dist: py-multiformats-cid>=0.4.3
 Requires-Dist: setuptools>=67.7.0
 Provides-Extra: orjson
 Requires-Dist: orjson>=3.0; extra == "orjson"
 Provides-Extra: car
 Requires-Dist: ipfs-car-decoder==0.1.1; extra == "car"
-Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: pytest-asyncio; extra == "test"
-Requires-Dist: tox; extra == "test"
-Requires-Dist: flake8; extra == "test"
-Requires-Dist: wheel; extra == "test"
+Provides-Extra: dev
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-asyncio; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: tox; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: wheel; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx==5.3.0; extra == "docs"
 Requires-Dist: sphinxcontrib-asyncio; extra == "docs"
 Requires-Dist: guzzle_sphinx_theme; extra == "docs"
+Provides-Extra: bohort
+Requires-Dist: appdirs>=1.4.4; extra == "bohort"
+Requires-Dist: omegaconf==2.3.0; extra == "bohort"
+Requires-Dist: ptpython-aioipfs>=3.0.27; extra == "bohort"
 
 =======
 aioipfs
 =======
 
 :info: Asynchronous IPFS_ client library
 
@@ -57,28 +63,31 @@
 
 This library supports the
 `RPC API specifications <https://docs.ipfs.tech/reference/kubo/rpc>`_
 for kubo_ version *0.27.0*. Unit tests are run against
 most major go-ipfs releases and all kubo_
 releases, see the *CI* section below.
 
-See `the documentation here <https://aioipfs.readthedocs.io/en/latest>`_.
+See the documentation `here <https://aioipfs.readthedocs.io/en/latest>`_.
 
-.. image:: https://github.com/pinnaculum/aioipfs/workflows/aioipfs-build/badge.svg
-    :target: https://github.com/pinnaculum/aioipfs
-
-.. image:: https://gitlab.com/cipres/aioipfs/badges/master/pipeline.svg
+.. image:: https://gitlab.com/cipres/aioipfs/badges/master/coverage.svg
 
 Installation
 ============
 
 .. code-block:: shell
 
     pip install aioipfs
 
+To install the requirements for `bohort <https://aioipfs.readthedocs.io/en/latest/bohort.html>`_, a REPL tool for making RPC calls on kubo nodes:
+
+.. code-block:: shell
+
+    pip install 'aioipfs[bohort]'
+
 Support for CAR (Content-Addressable Archives) decoding (with the
 `ipfs-car-decoder package <https://github.com/kralverde/py-ipfs-car-decoder/>`_)
 can be enabled with the *car* extra:
 
 .. code-block:: shell
 
     pip install 'aioipfs[car]'
@@ -117,14 +126,23 @@
 
 .. code-block:: python
 
     client = aioipfs.AsyncIPFS(host='localhost', port=5001)
 
     client = aioipfs.AsyncIPFS(host='::1', port=5201)
 
+If the kubo server requires authentication, you can pass the RPC authentication
+credentials via the constructor's *auth* keyword argument:
+
+.. code-block:: python
+
+    client = aioipfs.AsyncIPFS(auth=aioipfs.BasicAuth('john', 'password123'))
+
+    client = aioipfs.AsyncIPFS(auth=aioipfs.BearerAuth('my-secret-token'))
+
 Get an IPFS resource
 --------------------
 
 .. code-block:: python
 
     import sys
     import asyncio
@@ -203,14 +221,20 @@
 The Gitlab CI workflow runs unit tests against the following
 go-ipfs/kubo releases (`go here <https://gitlab.com/cipres/aioipfs/-/jobs>`_
 for the CI jobs overview).
 
 - go-ipfs >=0.11.0,<=0.13.0
 - kubo >=0.14.0,<=0.27.0
 
+.. image:: https://github.com/pinnaculum/aioipfs/workflows/aioipfs-build/badge.svg
+    :target: https://github.com/pinnaculum/aioipfs/actions
+
+.. image:: https://gitlab.com/cipres/aioipfs/badges/master/pipeline.svg
+    :target: https://gitlab.com/cipres/aioipfs/-/jobs
+
 Features
 ========
 
 Async file writing on get operations
 ------------------------------------
 
 The **aiofiles** library is used to asynchronously write data retrieved from
```

### Comparing `aioipfs-0.6.7/README.rst` & `aioipfs-0.6.8/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -9,28 +9,31 @@
 
 This library supports the
 `RPC API specifications <https://docs.ipfs.tech/reference/kubo/rpc>`_
 for kubo_ version *0.27.0*. Unit tests are run against
 most major go-ipfs releases and all kubo_
 releases, see the *CI* section below.
 
-See `the documentation here <https://aioipfs.readthedocs.io/en/latest>`_.
+See the documentation `here <https://aioipfs.readthedocs.io/en/latest>`_.
 
-.. image:: https://github.com/pinnaculum/aioipfs/workflows/aioipfs-build/badge.svg
-    :target: https://github.com/pinnaculum/aioipfs
-
-.. image:: https://gitlab.com/cipres/aioipfs/badges/master/pipeline.svg
+.. image:: https://gitlab.com/cipres/aioipfs/badges/master/coverage.svg
 
 Installation
 ============
 
 .. code-block:: shell
 
     pip install aioipfs
 
+To install the requirements for `bohort <https://aioipfs.readthedocs.io/en/latest/bohort.html>`_, a REPL tool for making RPC calls on kubo nodes:
+
+.. code-block:: shell
+
+    pip install 'aioipfs[bohort]'
+
 Support for CAR (Content-Addressable Archives) decoding (with the
 `ipfs-car-decoder package <https://github.com/kralverde/py-ipfs-car-decoder/>`_)
 can be enabled with the *car* extra:
 
 .. code-block:: shell
 
     pip install 'aioipfs[car]'
@@ -69,14 +72,23 @@
 
 .. code-block:: python
 
     client = aioipfs.AsyncIPFS(host='localhost', port=5001)
 
     client = aioipfs.AsyncIPFS(host='::1', port=5201)
 
+If the kubo server requires authentication, you can pass the RPC authentication
+credentials via the constructor's *auth* keyword argument:
+
+.. code-block:: python
+
+    client = aioipfs.AsyncIPFS(auth=aioipfs.BasicAuth('john', 'password123'))
+
+    client = aioipfs.AsyncIPFS(auth=aioipfs.BearerAuth('my-secret-token'))
+
 Get an IPFS resource
 --------------------
 
 .. code-block:: python
 
     import sys
     import asyncio
@@ -155,14 +167,20 @@
 The Gitlab CI workflow runs unit tests against the following
 go-ipfs/kubo releases (`go here <https://gitlab.com/cipres/aioipfs/-/jobs>`_
 for the CI jobs overview).
 
 - go-ipfs >=0.11.0,<=0.13.0
 - kubo >=0.14.0,<=0.27.0
 
+.. image:: https://github.com/pinnaculum/aioipfs/workflows/aioipfs-build/badge.svg
+    :target: https://github.com/pinnaculum/aioipfs/actions
+
+.. image:: https://gitlab.com/cipres/aioipfs/badges/master/pipeline.svg
+    :target: https://gitlab.com/cipres/aioipfs/-/jobs
+
 Features
 ========
 
 Async file writing on get operations
 ------------------------------------
 
 The **aiofiles** library is used to asynchronously write data retrieved from
```

### Comparing `aioipfs-0.6.7/aioipfs/__init__.py` & `aioipfs-0.6.8/aioipfs/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-__version__ = '0.6.7'
+__version__ = '0.6.8'
 
 from yarl import URL
-from distutils.version import StrictVersion
+from distutils.version import StrictVersion  # type: ignore
 from typing import Union
 
 import asyncio
 import aiohttp
 import ipaddress
 import re
 import socket
 
 from aiohttp import BasicAuth
 
-from multiaddr import Multiaddr
-from multiaddr.exceptions import ParseError
-from multiaddr.exceptions import StringParseError
+from multiaddr import Multiaddr  # type: ignore
+from multiaddr.exceptions import ParseError  # type: ignore
+from multiaddr.exceptions import StringParseError  # type: ignore
 
 from aioipfs import api
 from aioipfs.exceptions import *  # noqa
 from aioipfs.apis import dag as dag_api
 from aioipfs.apis import pin as pin_api
 from aioipfs.apis import multibase as multibase_api
 from aioipfs.apis import p2p as p2p_api
@@ -66,15 +66,15 @@
     """
 
     def __init__(self,
                  host: str = 'localhost',
                  port: int = RPC_API_DEFAULT_PORT,
                  scheme: str = 'http',
                  maddr: Union[Multiaddr, str] = None,
-                 auth: Union[BasicAuth, BearerAuth] = None,
+                 auth: Union[BasicAuth, BearerAuth, None] = None,
                  loop=None,
                  conns_max: int = 0,
                  conns_max_per_host: int = 0,
                  read_timeout: int = 0,
                  api_version: str = 'v0',
                  debug: bool = False):
```

### Comparing `aioipfs-0.6.7/aioipfs/api.py` & `aioipfs-0.6.8/aioipfs/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import os.path
 import tarfile
 import tempfile
 import sys
-from typing import Union
+from typing import Union, Optional, Dict
 from pathlib import Path
 
 import asyncio
-import aiofiles
+import aiofiles  # type: ignore
 import aioipfs
 
 from aiohttp import payload
 
+from .apis import HTTP_ERROR_CODES
 from .apis import SubAPI
 from . import multi
 from .helpers import *  # noqa
 
 
 class BitswapAPI(SubAPI):
     async def ledger(self, peer):
@@ -245,23 +246,23 @@
 
         :param str key: The key of the config entry (e.g. "Addresses.API")
         :param str value: The value to set the config entry to
         :param bool boolean: Set a boolean value
         :param bool json: Parse stringified JSON
         """
 
-        params = {}
+        params: Dict = {}
 
         if value is not None:
             if boolean:
                 params[ARG_PARAM] = [key, boolarg(value)]
             else:
                 params[ARG_PARAM] = [key, value]
         else:
-            params = {ARG_PARAM: key}
+            params[ARG_PARAM] = key
 
         params['bool'] = boolarg(boolean)
         params['json'] = boolarg(json)
 
         return await self.fetch_json(
             self.url('config'),
             params=params
@@ -356,14 +357,17 @@
         }
 
         async for value in self.mjson_decode(
                 self.url('dht/provide'), params=params):
             yield value
 
     async def query(self, peerid, verbose=False):
+        """
+        DEPRECATED: This command is deprecated
+        """
         async for value in self.mjson_decode(
                 self.url('dht/query'),
                 params={ARG_PARAM: peerid, 'verbose': boolarg(verbose)}):
             yield value
 
 
 class DiagAPI(SubAPI):
@@ -384,26 +388,26 @@
         return await self.fetch_text(self.url('diag/cmds/set-time'),
                                      params={ARG_PARAM: time})
 
     async def cmds_clear(self):
         return await self.fetch_text(self.url('diag/cmds/clear'))
 
     async def profile(self,
-                      output: str = None,
-                      collectors: list = None,
-                      profile_time: str = None,
-                      mutex_profile_fraction: int = None,
-                      block_profile_rate: str = None):
+                      output: Optional[str] = None,
+                      collectors: Optional[list] = None,
+                      profile_time: Optional[str] = None,
+                      mutex_profile_fraction: Optional[int] = None,
+                      block_profile_rate: Optional[str] = None):
         """
         Collect a performance profile for debugging.
 
         TODO: support passing collectors as an array
         """
 
-        params = {}
+        params: Dict = {}
 
         if isinstance(output, str):
             params['output'] = output
 
         if isinstance(profile_time, str):
             params['profile-time'] = profile_time
 
@@ -436,32 +440,32 @@
         })
 
         return await self.fetch_text(self.url('files/cp'),
                                      params=params)
 
     async def chcid(self, path: str,
                     cidversion: int,
-                    hashfn: str = None):
+                    hashfn: Optional[str] = None):
         params = {ARG_PARAM: path, 'cid-version': str(cidversion)}
 
         if isinstance(hashfn, str):
             params['hash'] = hashfn
 
         return await self.fetch_text(self.url('files/chcid'), params=params)
 
     async def flush(self, path: str = '/'):
         """
         Flush a given path's data to disk.
         """
         params = {ARG_PARAM: path}
-        return await self.fetch_text(self.url('files/flush'),
+        return await self.fetch_json(self.url('files/flush'),
                                      params=params)
 
     async def mkdir(self, path, parents=False, cid_version=None,
-                    hashfn: str = None):
+                    hashfn: Optional[str] = None):
         params = {ARG_PARAM: path, 'parents': boolarg(parents)}
 
         if isinstance(hashfn, str):
             params['hash'] = hashfn
 
         if cid_version is not None and isinstance(cid_version, int):
             params['cid-version'] = str(cid_version)
@@ -480,16 +484,16 @@
             'l': boolarg(long),
             'U': boolarg(unsorted)
         }
         return await self.fetch_json(self.url('files/ls'),
                                      params=params)
 
     async def read(self, path,
-                   offset: int = None,
-                   count: int = None):
+                   offset: Optional[int] = None,
+                   count: Optional[int] = None):
         params = {ARG_PARAM: path}
 
         if offset is not None and isinstance(offset, int):
             params['offset'] = offset
         if count is not None and isinstance(count, int):
             params['count'] = count
 
@@ -520,15 +524,15 @@
 
         return await self.fetch_json(self.url('files/stat'),
                                      params=params)
 
     async def write(self, mfspath, data, create=False,
                     parents=False, cid_version=None,
                     raw_leaves=False,
-                    hashfn: str = None,
+                    hashfn: Optional[str] = None,
                     truncate=False, offset=-1, count=-1):
         """
         Write to a mutable file in a given filesystem.
 
         :param str mfspath: Path to write to
         :param data: Data to write, can be a filepath or bytes data
         :param int offset: Byte offset to begin writing at
@@ -599,15 +603,15 @@
         )
 
 
 class KeyAPI(SubAPI):
     async def key_import(self,
                          keypath: str,
                          name,
-                         ipns_base: str = None,
+                         ipns_base: Optional[str] = None,
                          format='libp2p-protobuf-cleartext',
                          allow_any_keytype: bool = False):
         """
         Import a key and prints imported key id
 
         :param str keypath: filepath of the key to import
         :param str name: name to associate with key in keychain
@@ -653,43 +657,44 @@
         if output:
             params['output'] = str(output)
 
         return await self.fetch_json(self.url('key/export'),
                                      params=params)
 
     async def list(self, long=False,
-                   ipns_base: str = None):
+                   ipns_base: Optional[str] = None):
         params = {'l': boolarg(long)}
 
         if isinstance(ipns_base, str):
             params['ipns-base'] = ipns_base
 
         return await self.fetch_json(self.url('key/list'),
                                      params=params)
 
     async def gen(self, name, type='rsa', size: int = 2048,
-                  ipns_base: str = None):
+                  ipns_base: Optional[str] = None):
         params = {ARG_PARAM: name, 'type': type, 'size': str(size)}
 
         if isinstance(ipns_base, str):
             params['ipns-base'] = ipns_base
 
         return await self.fetch_json(self.url('key/gen'),
                                      params=params)
 
     async def rm(self, name,
-                 ipns_base: str = None):
+                 ipns_base: Optional[str] = None):
         params = {ARG_PARAM: name}
 
         if isinstance(ipns_base, str):
             params['ipns-base'] = ipns_base
 
         return await self.fetch_json(self.url('key/rm'), params=params)
 
-    async def rename(self, src, dst, ipns_base=None, force: bool = False):
+    async def rename(self, src, dst, ipns_base: Optional[str] = None,
+                     force: bool = False):
         params = {
             ARG_PARAM: [src, dst],
             'force': boolarg(force)
         }
 
         if isinstance(ipns_base, str):
             params['ipns-base'] = ipns_base
@@ -756,15 +761,15 @@
     def __init__(self, driver):
         super().__init__(driver)
 
         self.pubsub = NamePubsubAPI(driver)
 
     async def inspect(self,
                       record: Union[str, Path],
-                      verify: str = None,
+                      verify: Optional[str] = None,
                       dump: bool = True):
         """
         Inspects an IPNS Record
 
         :param record: Path to the file containing the IPNS record
         :type record: Union[Path, str]
         :param str verify: CID of the public IPNS key to validate against
@@ -790,15 +795,15 @@
 
             return await self.post(self.url('name/inspect'),
                                    mpwriter, params=params, outformat='json')
 
     async def publish(self, path, resolve=True, lifetime='24h',
                       key='self', ttl=None,
                       quieter=False, allow_offline=False,
-                      ipns_base: str = None):
+                      ipns_base: Optional[str] = None):
         """
         Publish IPNS names
 
         :param str path: ipfs path of the object to be published
         :param bool resolve: Check if the given path can be resolved
             before publishing
         :param str lifetime: Time duration that the record will be
@@ -1015,19 +1020,19 @@
             return await self.post(self.url('object/put'), mpwriter,
                                    params=params, outformat='json')
 
 
 class RefsAPI(SubAPI):
     async def refs(self,
                    path: str,
-                   format: str = None,
+                   format: Optional[str] = None,
                    edges: bool = False,
                    unique: bool = False,
                    recursive: bool = False,
-                   max_depth: int = None):
+                   max_depth: Optional[int] = None):
         """
         List links (references) from an object.
         """
         params = {
             ARG_PARAM: path,
             'unique': boolarg(unique),
             'recursive': boolarg(recursive),
@@ -1239,23 +1244,27 @@
             params['inline'] = boolarg(inline)
             params['inline-limit'] = str(kwargs.pop('inline_limit', 32))
 
         return params
 
     def _add_post(self, data, params=None):
         return self.driver.session.post(self.url('add'), data=data,
+                                        auth=self.driver.auth,
                                         params=params if params else {})
 
     async def add_single(self, mpart, params=None):
         """
         Add a single-entry multipart (used by add_{bytes,str,json})
         """
 
         async with self._add_post(
                 mpart, params=params if params else {}) as response:
+            if response.status in HTTP_ERROR_CODES:
+                self.handle_error(response, await response.text())
+
             return await response.json()
 
     async def add_generic(self, mpart, params=None):
         """
         Add a multiple-entry multipart, and yield the JSON message for every
         entry added. We use mjson_decode with the post method.
         """
@@ -1420,17 +1429,17 @@
         """ List all available commands."""
 
         return await self.fetch_json(
             self.url('commands'),
             params={'flags': boolarg(flags)}
         )
 
-    async def id(self, peer: str = None,
-                 format: str = None,
-                 peerid_base: str = None):
+    async def id(self, peer: Optional[str] = None,
+                 format: Optional[str] = None,
+                 peerid_base: Optional[str] = None):
         """
         Show IPFS node id info.
 
         :param str peer: peer id to look up, otherwise shows local node info
         """
         params = {ARG_PARAM: peer} if peer else {}
 
@@ -1738,16 +1747,16 @@
             ARG_PARAM: name,
             'recursive': boolarg(recursive)
         }
         return await self.fetch_json(self.url('dns'), params=params)
 
     async def resolve(self, name,
                       recursive: bool = False,
-                      dht_record_count: int = None,
-                      dht_timeout: int = None):
+                      dht_record_count: Optional[int] = None,
+                      dht_timeout: Optional[int] = None):
         """
         Resolve the value of names to IPFS
 
         :param str name: The name to resolve
         :param bool recursive: Resolve until the result is an IPFS name
         :param int dht_record_count: Number of records to request
             for DHT resolution
```

### Comparing `aioipfs-0.6.7/aioipfs/apis/__init__.py` & `aioipfs-0.6.8/aioipfs/apis/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import json
 import asyncio
 import sys
 
+from typing import Union
+
 from aiohttp.web_exceptions import (HTTPInternalServerError,
                                     HTTPForbidden,
                                     HTTPNotFound,
                                     HTTPMethodNotAllowed,
                                     HTTPBadRequest)
 from aiohttp.client_exceptions import *  # noqa
 
@@ -47,15 +49,15 @@
             decoded_json = json.loads(errormsg)
             mtype = decoded_json.get('Type')
             assert mtype.lower() == 'error'
             return decoded_json['Message'], decoded_json['Code']
         except Exception:
             return None, None
 
-    def handle_error(self, response, data):
+    def handle_error(self, response, data: Union[str, None]):
         """
         When the daemon returns an HTTP status code != 200, this
         method is called to raise an API exception.
         """
 
         if response.status == HTTPNotFound.status_code:
             # 404
@@ -195,14 +197,17 @@
                 kwargs['data'] = data
 
         if isinstance(headers, dict):
             kwargs['headers'] = headers
 
         try:
             async with getattr(session, method)(url, **kwargs) as response:
+                if response.status in HTTP_ERROR_CODES:
+                    self.handle_error(response, await response.text())
+
                 async for raw_message in response.content:
                     message = decode_json(raw_message)
 
                     if message is not None:
                         if 'Message' in message and 'Code' in message:
                             self.handle_error(response, raw_message)
                         else:
@@ -218,16 +223,15 @@
         except APIError as e:
             if new_session is True:
                 await session.close()
 
             raise e
         except (ClientPayloadError,
                 ClientConnectorError,
-                ServerDisconnectedError,
-                Exception):
+                ServerDisconnectedError):
             if new_session is True:
                 await session.close()
 
             raise IPFSConnectionError('Connection/payload error')
 
         if new_session is True:
             await session.close()
```

### Comparing `aioipfs-0.6.7/aioipfs/apis/dag.py` & `aioipfs-0.6.8/aioipfs/apis/dag.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os.path
 from pathlib import Path
+from typing import Optional
 from aiohttp import payload
 
 from aioipfs.api import SubAPI
 from aioipfs.api import boolarg
 from aioipfs.api import ARG_PARAM
 from aioipfs import multi
 from aioipfs import UnknownAPIError
@@ -43,15 +44,15 @@
                                                 filename=basename)
             mpwriter.append_payload(dag_payload)
 
             return await self.post(self.url('dag/put'), mpwriter,
                                    params=params, outformat='json')
 
     async def car_export(self, cid: str, progress: bool = False,
-                         output_path: Path = None):
+                         output_path: Optional[Path] = None):
         """
         Streams the selected DAG as a .car stream and return it
         as a raw buffer or write it to a file if output_path is
         passed.
 
         :param str cid: Root CID of a DAG to recursively export
         :param bool progress: Stream progress
```

### Comparing `aioipfs-0.6.7/aioipfs/apis/multibase.py` & `aioipfs-0.6.8/aioipfs/apis/multibase.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.7/aioipfs/apis/p2p.py` & `aioipfs-0.6.8/aioipfs/apis/p2p.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os.path
+from typing import Any
 
 from yarl import URL
-from multiaddr import Multiaddr
+from multiaddr import Multiaddr  # type: ignore
 
 from aioipfs.api import SubAPI
 from aioipfs.api import ARG_PARAM
 from aioipfs.api import boolarg
 from aioipfs.exceptions import APIError
 
 from aioipfs.helpers import async_enterable
@@ -102,14 +103,16 @@
 
 
 class P2PDialerMixin:
     """
     APIs to help with dialing remote p2p services
     """
 
+    driver: Any
+
     @async_enterable
     async def dial_service(self,
                            peer: str,
                            protocol: str,
                            address=None,
                            auto=True,
                            allow_loopback=False):
@@ -237,23 +240,23 @@
 
     async def listeners_for_proto(self, protocol: str) -> list:
         return [stream for stream in await self.listeners() if
                 stream['Protocol'] == protocol]
 
     async def listeners(self) -> list:
         try:
-            resp = await self.ls(headers=True)
+            resp = await self.ls(headers=True)  # type: ignore
             assert isinstance(resp, dict)
             return resp['Listeners'] if resp['Listeners'] else []
         except (AssertionError, APIError):
             return []
 
     async def streams(self) -> list:
         try:
-            resp = await self.stream_ls(headers=True)
+            resp = await self.stream_ls(headers=True)  # type: ignore
             assert isinstance(resp, dict)
             return resp['Streams'] if resp['Streams'] else []
         except (AssertionError, APIError):
             return []
 
 
 class P2PAPI(P2PDialerMixin, SubAPI):
```

### Comparing `aioipfs-0.6.7/aioipfs/apis/pin.py` & `aioipfs-0.6.8/aioipfs/apis/pin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Optional
+
 from aioipfs.apis import SubAPI
 from aioipfs.helpers import *  # noqa
 
 
 class PinRemoteServiceAPI(SubAPI):
     async def add(self, service, endpoint, key):
         """
@@ -142,15 +144,15 @@
 class PinAPI(SubAPI):
     def __init__(self, driver):
         super().__init__(driver)
 
         self.remote = PinRemoteAPI(driver)
 
     async def add(self, path, recursive=True, progress=True,
-                  name: str = None):
+                  name: Optional[str] = None):
         """
         Pin objects to local storage.
 
         :param str path: Path to object(s) to be pinned
         :param bool recursive: Recursively pin the object linked to
             by the specified object(s)
         :param str name: An optional name for the created pin(s)
```

### Comparing `aioipfs-0.6.7/aioipfs/apis/pubsub.py` & `aioipfs-0.6.8/aioipfs/apis/pubsub.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import io
 import asyncio
 from typing import Union
 
 import base58
 import base64
-import multibase
+import multibase  # type: ignore
 
 from aiohttp import payload
 from aioipfs import multi
 from aioipfs.helpers import quote_args
 from aioipfs.api import SubAPI
 from aioipfs.api import ARG_PARAM
 from aioipfs.api import boolarg
@@ -81,14 +81,17 @@
         return await self.post(self.url('pubsub/pub'),
                                None, params=quote_args(topic, msgd))
 
     async def __pub_multibase(self, topic, data: Union[str, bytes]):
         """
         New publish wire format (post 0.11.0)
         """
+
+        part: Union[payload.StringIOPayload, payload.BytesIOPayload]
+
         params = {
             ARG_PARAM: multibase.encode('base64url', topic).decode()
         }
 
         with multi.FormDataWriter() as mpwriter:
             if isinstance(data, str):
                 part = payload.StringIOPayload(io.StringIO(data))
@@ -100,16 +103,16 @@
 
             return await self.post(self.url('pubsub/pub'), mpwriter,
                                    params=params, outformat='text')
 
     async def sub(self,
                   topic: str,
                   discover: bool = True,
-                  timeout: int = None,
-                  read_timeout: int = None):
+                  timeout: int = 0,
+                  read_timeout: int = 0):
         """
         Subscribe to messages on a given topic.
 
         This is an async generator yielding messages as they are read on the
         pubsub topic.
 
         :param str topic: topic to subscribe to
@@ -136,15 +139,15 @@
 
         async for message in self.mjson_decode(
                 self.url('pubsub/sub'),
                 method='post',
                 headers={'Connection': 'Close'},
                 new_session=True,
                 timeout=timeout if timeout else 60.0 * 60 * 24 * 8,
-                read_timeout=read_timeout if read_timeout else 0,
+                read_timeout=read_timeout,
                 params=params):
             try:
                 if api_post011:
                     converted = self._decode_message(message)
                 else:
                     converted = self._decode_message_base58(message)
             except Exception as e:
```

### Comparing `aioipfs-0.6.7/aioipfs/apis/swarm.py` & `aioipfs-0.6.8/aioipfs/apis/swarm.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.7/aioipfs/exceptions.py` & `aioipfs-0.6.8/aioipfs/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.7/aioipfs/helpers.py` & `aioipfs-0.6.8/aioipfs/helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import functools
 import json
 import re
-import sys
-from multiaddr import Multiaddr
-from distutils.version import StrictVersion
+
+from multiaddr import Multiaddr  # type: ignore
+from distutils.version import StrictVersion  # type: ignore
 from contextlib import closing
+from typing import Union
 import socket
 import os.path
 
 from urllib.parse import quote
 
 from multiformats_cid import make_cid
 from multiformats_cid import CIDv1
 from multiformats_cid import CIDv0
 
 
 try:
-    import orjson
+    import orjson  # type: ignore
 except ImportError:
     have_orjson = False
 else:
     have_orjson = True
 
 
 ARG_PARAM = 'arg'
@@ -40,15 +41,15 @@
             quoted += '&{0}={1}'.format(ARG_PARAM, quote(str(arg)))
         return quoted[1:]
 
 
 def quote_dict(data):
     quoted = ''
 
-    if not isinstance(data, dict):
+    if not isinstance(data, dict):  # pragma: no cover
         raise ValueError('quote_dict: need dictionary')
 
     for arg, value in data.items():
         if isinstance(value, list):
             for lvalue in value:
                 quoted += '&{0}={1}'.format(arg, quote(str(lvalue)))
         elif isinstance(value, str):
@@ -59,25 +60,21 @@
             quoted += '&{0}={1}'.format(arg, quote(boolarg(value)))
 
     if len(quoted) > 0:
         return quoted[1:]
 
 
 def decode_json(data: bytes):
-    try:
-        if not isinstance(data, bytes):
-            raise TypeError('decode_json: invalid value type')
+    if not isinstance(data, bytes):  # pragma: no cover
+        raise TypeError('decode_json: invalid value type')
 
-        if have_orjson:
-            return orjson.loads(data.decode())
-        else:
-            return json.loads(data.decode())
-    except Exception as exc:
-        print('Could not read JSON object:', str(exc), file=sys.stderr)
-        return None
+    if have_orjson:
+        return orjson.loads(data.decode())
+    else:
+        return json.loads(data.decode())
 
 
 def async_enterable(f):
     @functools.wraps(f)
     def wrapper(*args, **kwargs):
         class AsyncEnterableInstance:
             async def __aenter__(self):
@@ -109,102 +106,102 @@
 
 def unusedTcpPort():
     try:
         with closing(socket.socket(socket.AF_INET, socket.SOCK_STREAM)) as s:
             s.bind(('', 0))
             s.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
             return s.getsockname()[1]
-    except Exception:
+    except Exception:  # pragma: no cover
         return None
 
 
 def p2p_addr_explode(addr: str) -> tuple:
     """
     Explode a P2P service endpoint address such as :
 
     /p2p/12D3KooWD3bfmNbuuuVCYwkjnFt3ukm3qaB3hDED3peHHXawvRAi/x/videocall/room1/1.0.0
     /p2p/12D3KooWD3bfmNbuuuVCYwkjnFt3ukm3qaB3hDED3peHHXawvRAi/x/test
 
     into its components, returning a tuple in the form
 
-    (peerId, protoFull, protoVersion)
+    (peer_id, proto_full, proto_version)
 
-    protoFull can be passed to 'ipfs p2p dial'
+    proto_full can be passed to 'ipfs p2p dial'
     """
 
-    peerIdRe = re.compile(r'([\w]){46,59}$')
+    peer_id_re = re.compile(r'([\w]){46,59}$')
 
     parts = addr.lstrip(os.path.sep).split(os.path.sep)
     try:
         assert parts.pop(0) == 'p2p'
-        peerId = parts.pop(0)
+        peer_id = parts.pop(0)
         prefix = parts.pop(0)
-        assert peerIdRe.match(peerId)
+        assert peer_id_re.match(peer_id)
         assert prefix in ['x', 'y', 'z']
 
-        pVersion = None
-        protoA = [prefix]
-        protoPart = parts.pop(0)
-        protoA.append(protoPart)
+        p_version = None
+        proto_a = [prefix]
+        proto_part = parts.pop(0)
+        proto_a.append(proto_part)
 
-        while protoPart:
+        while proto_part:
             try:
-                protoPart = parts.pop(0)
+                proto_part = parts.pop(0)
             except IndexError:
                 break
 
-            protoA.append(protoPart)
+            proto_a.append(proto_part)
 
             try:
-                v = StrictVersion(protoPart)
+                v = StrictVersion(proto_part)
             except Exception:
                 # No version
                 pass
             else:
                 # Found a version, should be last element
-                pVersion = v
+                p_version = v
                 assert len(parts) == 0
                 break
 
-        return peerId, os.path.sep + os.path.join(*protoA), pVersion
-    except Exception:
-        return None
+        return peer_id, os.path.sep + os.path.join(*proto_a), p_version
+    except Exception as err:
+        raise ValueError(f'Invalid p2p endpoint addr: {err}')
 
 
-def peerid_reencode(peerId: str,
+def peerid_reencode(peer_id: str,
                     base: str = 'base36',
-                    multicodec: str = 'libp2p-key') -> str:
+                    multicodec: str = 'libp2p-key') -> Union[str, None]:
     """
     Encode a PeerId to a specific base
     """
 
-    cid = make_cid(peerId)
+    cid = make_cid(peer_id)
     if not cid:
         return None
 
     if base in ['base32', 'base36']:
         return CIDv1(multicodec, cid.multihash).encode(base).decode()
     elif base in ['base58']:
         return str(CIDv0(cid.multihash))
 
     return None
 
 
-def peerid_base32(peerId: str) -> str:
+def peerid_base32(peer_id: str) -> Union[str, None]:  # pragma: no cover
     """
     Convert any PeerId to a CIDv1 (base32)
     """
-    return peerid_reencode(peerId, base='base32')
+    return peerid_reencode(peer_id, base='base32')
 
 
-def peerid_base36(peerId: str) -> str:
+def peerid_base36(peer_id: str) -> Union[str, None]:  # pragma: no cover
     """
     Convert any PeerId to a CIDv1 (base36)
     """
-    return peerid_reencode(peerId, base='base36')
+    return peerid_reencode(peer_id, base='base36')
 
 
-def peerid_base58(peerId: str) -> str:
+def peerid_base58(peer_id: str) -> Union[str, None]:  # pragma: no cover
     """
     Convert any PeerId to a CIDv0
     """
-    return peerid_reencode(peerId, base='base58')
+    return peerid_reencode(peer_id, base='base58')
```

### Comparing `aioipfs-0.6.7/aioipfs/multi.py` & `aioipfs-0.6.8/aioipfs/multi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import os.path
 import posixpath
 import io
 import re
 
-from gitignore_parser import parse_gitignore
+from gitignore_parser import parse_gitignore  # type: ignore
 import aiohttp
 from aiohttp import payload
 
 
 class FormDataWriter(aiohttp.MultipartWriter):
     def __init__(self):
         super().__init__(subtype='form-data')
@@ -43,15 +43,15 @@
 
     file_payload.set_content_disposition('form-data',
                                          name='file',
                                          filename=basename)
     return file_payload
 
 
-def glob_compile(pat):
+def glob_compile(pat):  # pragma: no cover
     """ From ipfsapi.multipart
 
        Translate a shell glob PATTERN to a regular expression.
 
     This is almost entirely based on `fnmatch.translate` source-code from the
     python 3.5 standard-library.
     """
```

### Comparing `aioipfs-0.6.7/aioipfs/util.py` & `aioipfs-0.6.8/aioipfs/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 try:
     import ipfs_car_decoder as car_decoder
     have_car_decoder = True
 except Exception:
     have_car_decoder = False
-    car_decoder = None
+    car_decoder = None  # type: ignore
 
 
 class CARDecoderMissing(Exception):
     pass
 
 
 def car_open(car_path: Path):
@@ -47,15 +47,15 @@
 class DotJSON(dict):
     """
     Based on edict, described here:
 
     https://gist.github.com/markhu/fbbab71359af00e527d0
     """
 
-    __delattr__ = dict.__delitem__
+    __delattr__ = dict.__delitem__  # type: ignore
 
     def __init__(self, data):
         if isinstance(data, str):
             data = json.loads(data)
         else:
             data = data
```

### Comparing `aioipfs-0.6.7/aioipfs.egg-info/PKG-INFO` & `aioipfs-0.6.8/aioipfs.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioipfs
-Version: 0.6.7
+Version: 0.6.8
 Summary: Asynchronous IPFS client library
 Author-email: cipres <alkaline@gmx.co.uk>
 License: LGPLv3
 Project-URL: Homepage, https://gitlab.com/cipres/aioipfs
 Keywords: asyncio,aiohttp,ipfs
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
@@ -31,24 +31,30 @@
 Requires-Dist: py-multibase>=1.0.3
 Requires-Dist: py-multiformats-cid>=0.4.3
 Requires-Dist: setuptools>=67.7.0
 Provides-Extra: orjson
 Requires-Dist: orjson>=3.0; extra == "orjson"
 Provides-Extra: car
 Requires-Dist: ipfs-car-decoder==0.1.1; extra == "car"
-Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: pytest-asyncio; extra == "test"
-Requires-Dist: tox; extra == "test"
-Requires-Dist: flake8; extra == "test"
-Requires-Dist: wheel; extra == "test"
+Provides-Extra: dev
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-asyncio; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: tox; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: wheel; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx==5.3.0; extra == "docs"
 Requires-Dist: sphinxcontrib-asyncio; extra == "docs"
 Requires-Dist: guzzle_sphinx_theme; extra == "docs"
+Provides-Extra: bohort
+Requires-Dist: appdirs>=1.4.4; extra == "bohort"
+Requires-Dist: omegaconf==2.3.0; extra == "bohort"
+Requires-Dist: ptpython-aioipfs>=3.0.27; extra == "bohort"
 
 =======
 aioipfs
 =======
 
 :info: Asynchronous IPFS_ client library
 
@@ -57,28 +63,31 @@
 
 This library supports the
 `RPC API specifications <https://docs.ipfs.tech/reference/kubo/rpc>`_
 for kubo_ version *0.27.0*. Unit tests are run against
 most major go-ipfs releases and all kubo_
 releases, see the *CI* section below.
 
-See `the documentation here <https://aioipfs.readthedocs.io/en/latest>`_.
+See the documentation `here <https://aioipfs.readthedocs.io/en/latest>`_.
 
-.. image:: https://github.com/pinnaculum/aioipfs/workflows/aioipfs-build/badge.svg
-    :target: https://github.com/pinnaculum/aioipfs
-
-.. image:: https://gitlab.com/cipres/aioipfs/badges/master/pipeline.svg
+.. image:: https://gitlab.com/cipres/aioipfs/badges/master/coverage.svg
 
 Installation
 ============
 
 .. code-block:: shell
 
     pip install aioipfs
 
+To install the requirements for `bohort <https://aioipfs.readthedocs.io/en/latest/bohort.html>`_, a REPL tool for making RPC calls on kubo nodes:
+
+.. code-block:: shell
+
+    pip install 'aioipfs[bohort]'
+
 Support for CAR (Content-Addressable Archives) decoding (with the
 `ipfs-car-decoder package <https://github.com/kralverde/py-ipfs-car-decoder/>`_)
 can be enabled with the *car* extra:
 
 .. code-block:: shell
 
     pip install 'aioipfs[car]'
@@ -117,14 +126,23 @@
 
 .. code-block:: python
 
     client = aioipfs.AsyncIPFS(host='localhost', port=5001)
 
     client = aioipfs.AsyncIPFS(host='::1', port=5201)
 
+If the kubo server requires authentication, you can pass the RPC authentication
+credentials via the constructor's *auth* keyword argument:
+
+.. code-block:: python
+
+    client = aioipfs.AsyncIPFS(auth=aioipfs.BasicAuth('john', 'password123'))
+
+    client = aioipfs.AsyncIPFS(auth=aioipfs.BearerAuth('my-secret-token'))
+
 Get an IPFS resource
 --------------------
 
 .. code-block:: python
 
     import sys
     import asyncio
@@ -203,14 +221,20 @@
 The Gitlab CI workflow runs unit tests against the following
 go-ipfs/kubo releases (`go here <https://gitlab.com/cipres/aioipfs/-/jobs>`_
 for the CI jobs overview).
 
 - go-ipfs >=0.11.0,<=0.13.0
 - kubo >=0.14.0,<=0.27.0
 
+.. image:: https://github.com/pinnaculum/aioipfs/workflows/aioipfs-build/badge.svg
+    :target: https://github.com/pinnaculum/aioipfs/actions
+
+.. image:: https://gitlab.com/cipres/aioipfs/badges/master/pipeline.svg
+    :target: https://gitlab.com/cipres/aioipfs/-/jobs
+
 Features
 ========
 
 Async file writing on get operations
 ------------------------------------
 
 The **aiofiles** library is used to asynchronously write data retrieved from
```

### Comparing `aioipfs-0.6.7/aioipfs.egg-info/SOURCES.txt` & `aioipfs-0.6.8/aioipfs.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
 aioipfs/__init__.py
 aioipfs/api.py
 aioipfs/exceptions.py
-aioipfs/gitignore_parser.py
 aioipfs/helpers.py
 aioipfs/multi.py
 aioipfs/util.py
 aioipfs.egg-info/PKG-INFO
 aioipfs.egg-info/SOURCES.txt
 aioipfs.egg-info/dependency_links.txt
+aioipfs.egg-info/entry_points.txt
 aioipfs.egg-info/requires.txt
 aioipfs.egg-info/top_level.txt
 aioipfs/apis/__init__.py
 aioipfs/apis/dag.py
 aioipfs/apis/multibase.py
 aioipfs/apis/p2p.py
 aioipfs/apis/pin.py
 aioipfs/apis/pubsub.py
 aioipfs/apis/swarm.py
-tests/test_client.py
+tests/test_client.py
+tests/test_helpers.py
```

### Comparing `aioipfs-0.6.7/pyproject.toml` & `aioipfs-0.6.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -41,29 +41,39 @@
 [project.readme]
 file = "README.rst"
 content-type = "text/x-rst"
 
 [project.optional-dependencies]
 orjson = ["orjson>=3.0"]
 car = ["ipfs-car-decoder==0.1.1"]
-test = [
+dev = [
+    "mypy",
     "pytest",
     "pytest-asyncio",
+    "pytest-cov",
     "tox",
     "flake8",
     "wheel",
 ]
 docs = [
     "sphinx==5.3.0",
     "sphinxcontrib-asyncio",
     "guzzle_sphinx_theme"
 ]
+bohort = [
+    "appdirs>=1.4.4",
+    "omegaconf==2.3.0",
+    "ptpython-aioipfs>=3.0.27"
+]
 
 [tool.setuptools.dynamic]
 version = {attr = "aioipfs.__version__"}
 
 [tool.setuptools]
 include-package-data = false
 
 [tool.setuptools.packages.find]
 exclude = ["tests"]
 namespaces = false
+
+[project.scripts]
+bohort = "aioipfs.scripts.bohort:run_bohort"
```

### Comparing `aioipfs-0.6.7/tests/test_client.py` & `aioipfs-0.6.8/tests/test_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,273 +1,35 @@
 import base64
 import pytest
 
 import tempfile
 import random
 import string
-import time
-import subprocess
 import os
 import os.path
 import platform
 import json
-import tarfile
 import sys
 
-from distutils.version import StrictVersion
 from pathlib import Path
 from multiaddr import Multiaddr
 
 import asyncio
 import aioipfs
 
 from aioipfs import util
 from aioipfs.multi import DirectoryListing
 from aioipfs.exceptions import RPCAccessDenied
 
 
-def ipfs_config_get():
-    p = subprocess.Popen(['ipfs', 'config', 'show'],
-                         stdout=subprocess.PIPE)
-    out, err = p.communicate()
-
-    try:
-        cfg = json.loads(out.decode())
-    except Exception:
-        return None
-    else:
-        return util.DotJSON(cfg)
-
-
-def ipfs_config_replace(filep: str):
-    p = subprocess.Popen(['ipfs', 'config', 'replace', filep])
-    p.communicate()
-    return p.returncode
-
-
-def ipfs_getconfig_var(var):
-    sp_getconfig = subprocess.Popen(['ipfs', 'config',
-                                     var], stdout=subprocess.PIPE)
-    stdout, stderr = sp_getconfig.communicate()
-    return stdout.decode()
-
-
-@pytest.fixture
-def ipfs_version():
-    p = subprocess.Popen(['ipfs', 'version'],
-                         stdout=subprocess.PIPE)
-    stdout, _ = p.communicate()
-    return StrictVersion(stdout.decode().replace('ipfs version ', ''))
-
-
-@pytest.fixture
-def datafiles():
-    return Path(os.path.dirname(__file__)).joinpath('datafiles')
-
-
-@pytest.fixture
-def smalltar():
-    fd, tpath = tempfile.mkstemp()
-    tar = tarfile.open(tpath, 'w|')
-    tar.add(__file__)
-    tar.close()
-    yield tar, tpath
-
-    os.close(fd)
-    os.unlink(tpath)
-
-
-@pytest.fixture
-def testfile1(tmpdir):
-    filep = tmpdir.join('testfile1.txt')
-    filep.write('POIEKJDOOOPIDMWOPIMPOWE()=ds129084bjcy')
-    return filep
-
-
-@pytest.fixture
-def testfile2(tmpdir):
-    r = random.Random()
-    filep = tmpdir.join('testfile2.txt')
-    filep.write(''.join([str(r.randint(i, i * 2)) for i in range(0, 16)]))
-    return filep
-
-
 def random_word(length=8):
     return ''.join(
         random.choice(string.ascii_lowercase) for c in range(length))
 
 
-@pytest.fixture
-def dir_hierarchy1(tmpdir):
-    root = Path(str(tmpdir))
-    root.joinpath('a/b/.c').mkdir(parents=True)
-    root.joinpath('a/b/.c/file0').touch()
-    root.joinpath('d/.e/f').mkdir(parents=True)
-    root.joinpath('d/.e/f/.file3').touch()
-    root.joinpath('file1').touch()
-    root.joinpath('.file2').touch()
-    return str(root)
-
-
-@pytest.fixture
-def dir_hierarchy2(tmpdir):
-    root = Path(str(tmpdir))
-    root.joinpath('a/b/.c').mkdir(parents=True)
-    root.joinpath('d/.e/f').mkdir(parents=True)
-    root.joinpath('d/.e/f/.file3').touch()
-    root.joinpath('file1').touch()
-
-    readme = root.joinpath('README.txt')
-    readme.touch()
-
-    with open(readme, 'wt') as f:
-        f.write('Hello')
-
-    root.joinpath('README2.txt').touch()
-    root.joinpath('.file2').touch()
-    ign = root.joinpath('.gitignore')
-    ign.touch()
-    ign.write_text("README.txt\n.file2\na\na/**\nd/.e/*/*\nd/.e/f\n")
-    return root
-
-
-def ipfs_config(param, value):
-    os.system('ipfs config {0} "{1}"'.format(param, value))
-
-
-def ipfs_config_json(param, value):
-    os.system("ipfs config --json '{0}' '{1}'".format(
-        param, json.dumps(value)))
-
-
-apiport = 9001
-gwport = 9080
-swarmport = 9002
-
-
-@pytest.fixture(scope='module')
-def ipfsdaemon():
-    # Starts a daemon on high port and temporary directory, yield it
-    # when started and shut it down on fixture's exit
-
-    tmpdir = tempfile.mkdtemp()
-
-    # Setup IPFS_PATH and initialize the repository
-    os.putenv('IPFS_PATH', tmpdir)
-    os.system('ipfs init -e')
-
-    cfg = ipfs_config_get()
-
-    with tempfile.NamedTemporaryFile(mode='wt', delete=False) as ncfgf:
-        cfg.Addresses.API = [
-            f'/ip4/127.0.0.1/tcp/{apiport}',
-            f'/ip6/::1/tcp/{apiport}',
-        ]
-
-        cfg.Addresses.Gateway = f'/ip4/127.0.0.1/tcp/{gwport}'
-        cfg.Addresses.Swarm = [f"/ip4/127.0.0.1/tcp/{swarmport}"]
-
-        # Empty bootstrap so we're not bothered
-        cfg.Bootstrap = []
-
-        cfg.Experimental.Libp2pStreamMounting = True
-        cfg.Experimental.FilestoreEnabled = True
-
-        cfg.write(ncfgf)
-
-    ipfs_config_replace(ncfgf.name)
-
-    # Run the daemon and wait a bit
-    sp = subprocess.Popen(['ipfs', 'daemon', '--enable-pubsub-experiment'],
-                          stdout=subprocess.PIPE)
-    time.sleep(1)
-
-    yield tmpdir, sp
-
-    time.sleep(0.5)
-    # Cleanup
-    sp.terminate()
-
-
-apiport_a = 9011
-gwport_a = 9090
-swarmport_a = 9012
-
-
-@pytest.fixture(scope='module')
-def ipfsdaemon_with_auth():
-    tmpdir = tempfile.mkdtemp()
-
-    os.putenv('IPFS_PATH', tmpdir)
-    os.system('ipfs init -e')
-
-    cfg = ipfs_config_get()
-
-    with tempfile.NamedTemporaryFile(mode='wt', delete=False) as ncfgf:
-        cfg.Addresses.API = [
-            f'/ip4/127.0.0.1/tcp/{apiport_a}',
-            f'/ip6/::1/tcp/{apiport_a}',
-        ]
-
-        cfg.Addresses.Gateway = f'/ip4/127.0.0.1/tcp/{gwport_a}'
-        cfg.Addresses.Swarm = [f"/ip4/127.0.0.1/tcp/{swarmport_a}"]
-
-        # Empty bootstrap so we're not bothered
-        cfg.Bootstrap = []
-
-        cfg.Experimental.Libp2pStreamMounting = True
-        cfg.Experimental.FilestoreEnabled = True
-
-        cfg.API.Authorizations = {
-            'Alice': {
-                "AuthSecret": "basic:alice:password123",
-                "AllowedPaths": ["/api/v0/files"]
-            },
-            'John': {
-                "AuthSecret": "basic:john:12345",
-                "AllowedPaths": ["/api/v0/add"]
-            },
-            'Bear': {
-                "AuthSecret": "bearer:token123",
-                "AllowedPaths": ["/api/v0"]
-            }
-        }
-
-        cfg.write(ncfgf)
-
-    ipfs_config_replace(ncfgf.name)
-
-    sp = subprocess.Popen(['ipfs', 'daemon'], stdout=subprocess.PIPE)
-    time.sleep(1)
-
-    yield tmpdir, sp
-
-    time.sleep(0.5)
-    sp.terminate()
-
-
-@pytest.fixture
-def ipfs_peerid(ipfsdaemon):
-    return ipfs_getconfig_var('Identity.PeerID').strip()
-
-
-@pytest.fixture(autouse=True)
-async def iclient(event_loop):
-    client = aioipfs.AsyncIPFS(port=apiport, loop=event_loop)
-    yield client
-    await client.close()
-
-
-@pytest.fixture(autouse=True)
-async def iclient_with_auth(event_loop):
-    client = aioipfs.AsyncIPFS(port=apiport_a, loop=event_loop)
-    yield client
-    await client.close()
-
-
 class TestClientConstructor:
     @pytest.mark.asyncio
     async def test_invalid_constructor(self, event_loop):
         # Invalid host
         with pytest.raises(aioipfs.InvalidNodeAddressError):
             aioipfs.AsyncIPFS(host=None, loop=event_loop)
 
@@ -297,14 +59,16 @@
         # Invalid application layer protocol
         with pytest.raises(aioipfs.InvalidNodeAddressError):
             aioipfs.AsyncIPFS(maddr='/ip4/localhost/tcp/4000/invalid',
                               loop=event_loop)
 
     @pytest.mark.asyncio
     async def test_constructor_apiurl(self, event_loop, ipfsdaemon):
+        ddir, apiport, sp = ipfsdaemon
+
         # Test by passing a host and port
         client = aioipfs.AsyncIPFS(
             host='localhost', port=apiport, loop=event_loop)
 
         assert str(client.api_url) == f'http://localhost:{apiport}/api/v0/'
 
         # Test by passing a host, port and scheme
@@ -374,22 +138,20 @@
         clif.auth = None
         assert clif.auth is None
 
 
 class TestAsyncIPFS:
     @pytest.mark.asyncio
     async def test_basic(self, event_loop, ipfsdaemon, iclient):
-        tmpdir, sp = ipfsdaemon
         await iclient.id()
         await iclient.core.version()
         await iclient.commands()
 
     @pytest.mark.asyncio
     async def test_bootstrap(self, event_loop, ipfsdaemon, iclient):
-        tmpdir, sp = ipfsdaemon
         await iclient.bootstrap.list()
 
     @pytest.mark.asyncio
     async def test_swarm(self, event_loop, ipfsdaemon, iclient):
         await iclient.swarm.peers()
         await iclient.swarm.addrs()
         await iclient.swarm.addrs_local()
@@ -484,24 +246,25 @@
                         iclient_with_auth, testfile1):
         if ipfs_version < aioipfs.IpfsDaemonVersion('0.25.0'):
             # RPC Authorization was introduced in kubo v0.25.0
             pytest.skip('RPC Authorization not supported ')
 
         iclient_with_auth.auth = aioipfs.BasicAuth('alice', 'password123')
 
+        # alice doesn't have access to the 'id' RPC API
         with pytest.raises(RPCAccessDenied):
             await iclient_with_auth.core.id()
 
         # alice can use the 'files' API
         assert await iclient_with_auth.files.ls('/')
 
-        # alice doesn't have access to the 'add' API
-        cids = [added['Hash'] async for added in iclient_with_auth.add(
-            str(testfile1))]
-        assert len(cids) == 0
+        # alice doesn't have access to the 'add' RPC API
+        with pytest.raises(RPCAccessDenied):
+            cids = [added['Hash'] async for added in iclient_with_auth.add(
+                str(testfile1))]
 
         # john, however, does
         iclient_with_auth.auth = aioipfs.BasicAuth('john', '12345')
         cids = [added['Hash'] async for added in iclient_with_auth.add(
             str(testfile1))]
         assert len(cids) == 1
```

