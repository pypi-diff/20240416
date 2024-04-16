# Comparing `tmp/momotor-django-4.1.0.tar.gz` & `tmp/momotor_django-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "momotor-django-4.1.0.tar", last modified: Fri Jun  9 07:45:20 2023, max compression
+gzip compressed data, was "momotor_django-5.0.0.tar", last modified: Tue Apr 16 08:01:53 2024, max compression
```

## Comparing `momotor-django-4.1.0.tar` & `momotor_django-5.0.0.tar`

### file list

```diff
@@ -1,36 +1,62 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:45:20.000000 momotor-django-4.1.0/
--rw-r--r--   0 root         (0) root         (0)     1840 2023-06-09 07:45:20.000000 momotor-django-4.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      657 2022-08-22 08:11:03.000000 momotor-django-4.1.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 07:45:20.000000 momotor-django-4.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2258 2023-06-09 07:44:52.000000 momotor-django-4.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:45:20.000000 momotor-django-4.1.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:45:20.000000 momotor-django-4.1.0/src/momotor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:45:20.000000 momotor-django-4.1.0/src/momotor/django/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 07:44:52.000000 momotor-django-4.1.0/src/momotor/django/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      860 2022-08-22 08:11:03.000000 momotor-django-4.1.0/src/momotor/django/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      178 2022-08-22 08:11:03.000000 momotor-django-4.1.0/src/momotor/django/apps.py
--rw-rw-rw-   0 root         (0) root         (0)    18614 2023-06-09 07:44:52.000000 momotor-django-4.1.0/src/momotor/django/connection.py
--rw-rw-rw-   0 root         (0) root         (0)      509 2022-08-22 08:11:03.000000 momotor-django-4.1.0/src/momotor/django/defaults.py
--rw-rw-rw-   0 root         (0) root         (0)     1163 2023-06-09 07:44:52.000000 momotor-django-4.1.0/src/momotor/django/fields.py
--rw-rw-rw-   0 root         (0) root         (0)      621 2023-06-09 07:44:52.000000 momotor-django-4.1.0/src/momotor/django/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:45:20.000000 momotor-django-4.1.0/src/momotor/django/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      546 2022-08-22 08:11:03.000000 momotor-django-4.1.0/src/momotor/django/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 07:44:52.000000 momotor-django-4.1.0/src/momotor/django/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      229 2022-08-22 08:11:03.000000 momotor-django-4.1.0/src/momotor/django/models.py
--rw-rw-rw-   0 root         (0) root         (0)       60 2022-08-22 08:11:03.000000 momotor-django-4.1.0/src/momotor/django/tests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:45:20.000000 momotor-django-4.1.0/src/momotor/django/token_store/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 07:44:52.000000 momotor-django-4.1.0/src/momotor/django/token_store/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2562 2023-06-09 07:44:52.000000 momotor-django-4.1.0/src/momotor/django/token_store/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1349 2022-08-22 08:11:03.000000 momotor-django-4.1.0/src/momotor/django/token_store/cache.py
--rw-rw-rw-   0 root         (0) root         (0)      338 2022-08-22 08:11:03.000000 momotor-django-4.1.0/src/momotor/django/token_store/dummy.py
--rw-rw-rw-   0 root         (0) root         (0)      532 2022-08-22 08:11:03.000000 momotor-django-4.1.0/src/momotor/django/token_store/memory.py
--rw-rw-rw-   0 root         (0) root         (0)     1738 2022-08-22 08:11:03.000000 momotor-django-4.1.0/src/momotor/django/token_store/model.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-09 07:44:31.000000 momotor-django-4.1.0/src/momotor/django/version.py
--rw-rw-rw-   0 root         (0) root         (0)       63 2022-08-22 08:11:03.000000 momotor-django-4.1.0/src/momotor/django/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 07:45:20.000000 momotor-django-4.1.0/src/momotor_django.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1840 2023-06-09 07:45:19.000000 momotor-django-4.1.0/src/momotor_django.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      921 2023-06-09 07:45:19.000000 momotor-django-4.1.0/src/momotor_django.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 07:45:19.000000 momotor-django-4.1.0/src/momotor_django.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 07:45:19.000000 momotor-django-4.1.0/src/momotor_django.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      135 2023-06-09 07:45:19.000000 momotor-django-4.1.0/src/momotor_django.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-09 07:45:19.000000 momotor-django-4.1.0/src/momotor_django.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:01:53.000000 momotor_django-5.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     3228 2024-04-16 08:01:09.000000 momotor_django-5.0.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     3220 2024-04-16 08:01:09.000000 momotor_django-5.0.0/.gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:01:53.000000 momotor_django-5.0.0/.idea/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:01:53.000000 momotor_django-5.0.0/.idea/inspectionProfiles/
+-rw-rw-rw-   0 root         (0) root         (0)      174 2024-04-16 08:01:09.000000 momotor_django-5.0.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-rw-   0 root         (0) root         (0)      280 2024-04-16 08:01:09.000000 momotor_django-5.0.0/.idea/modules.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1340 2024-04-16 08:01:09.000000 momotor_django-5.0.0/.idea/momotor.lib.django.iml
+-rw-rw-rw-   0 root         (0) root         (0)    20105 2024-04-16 08:01:49.000000 momotor_django-5.0.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     2643 2024-04-16 08:01:53.000000 momotor_django-5.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      657 2024-04-16 08:01:09.000000 momotor_django-5.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:01:53.000000 momotor_django-5.0.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      638 2024-04-16 08:01:09.000000 momotor_django-5.0.0/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      764 2024-04-16 08:01:09.000000 momotor_django-5.0.0/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:01:53.000000 momotor_django-5.0.0/docs/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:01:53.000000 momotor_django-5.0.0/docs/source/_ext/
+-rw-rw-rw-   0 root         (0) root         (0)      258 2024-04-16 08:01:09.000000 momotor_django-5.0.0/docs/source/_ext/djangoroles.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:01:53.000000 momotor_django-5.0.0/docs/source/_static/
+-rw-rw-rw-   0 root         (0) root         (0)     6988 2024-04-16 08:01:09.000000 momotor_django-5.0.0/docs/source/_static/logo-text-negative.png
+-rw-rw-rw-   0 root         (0) root         (0)     6887 2024-04-16 08:01:09.000000 momotor_django-5.0.0/docs/source/_static/logo-text.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:01:53.000000 momotor_django-5.0.0/docs/source/_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      672 2024-04-16 08:01:09.000000 momotor_django-5.0.0/docs/source/_templates/projectlinks.html
+-rw-rw-rw-   0 root         (0) root         (0)     4754 2024-04-16 08:01:09.000000 momotor_django-5.0.0/docs/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-04-16 08:01:09.000000 momotor_django-5.0.0/docs/source/connection.rst
+-rw-rw-rw-   0 root         (0) root         (0)      402 2024-04-16 08:01:09.000000 momotor_django-5.0.0/docs/source/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3535 2024-04-16 08:01:09.000000 momotor_django-5.0.0/docs/source/settings.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2023 2024-04-16 08:01:09.000000 momotor_django-5.0.0/docs/source/tokenstore.rst
+-rw-rw-rw-   0 root         (0) root         (0)      436 2024-04-16 08:01:09.000000 momotor_django-5.0.0/publish-docs.sh
+-rw-rw-rw-   0 root         (0) root         (0)     2588 2024-04-16 08:01:09.000000 momotor_django-5.0.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      413 2024-04-16 08:01:09.000000 momotor_django-5.0.0/semver.sh
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 08:01:53.000000 momotor_django-5.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-16 08:01:09.000000 momotor_django-5.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:01:53.000000 momotor_django-5.0.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:01:53.000000 momotor_django-5.0.0/src/momotor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:01:53.000000 momotor_django-5.0.0/src/momotor/django/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 08:01:09.000000 momotor_django-5.0.0/src/momotor/django/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      860 2024-04-16 08:01:09.000000 momotor_django-5.0.0/src/momotor/django/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      178 2024-04-16 08:01:09.000000 momotor_django-5.0.0/src/momotor/django/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)    18750 2024-04-16 08:01:09.000000 momotor_django-5.0.0/src/momotor/django/connection.py
+-rw-rw-rw-   0 root         (0) root         (0)      509 2024-04-16 08:01:09.000000 momotor_django-5.0.0/src/momotor/django/defaults.py
+-rw-rw-rw-   0 root         (0) root         (0)     1163 2024-04-16 08:01:09.000000 momotor_django-5.0.0/src/momotor/django/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      621 2024-04-16 08:01:09.000000 momotor_django-5.0.0/src/momotor/django/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:01:53.000000 momotor_django-5.0.0/src/momotor/django/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      546 2024-04-16 08:01:09.000000 momotor_django-5.0.0/src/momotor/django/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 08:01:09.000000 momotor_django-5.0.0/src/momotor/django/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      229 2024-04-16 08:01:09.000000 momotor_django-5.0.0/src/momotor/django/models.py
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-04-16 08:01:09.000000 momotor_django-5.0.0/src/momotor/django/tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:01:53.000000 momotor_django-5.0.0/src/momotor/django/token_store/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 08:01:09.000000 momotor_django-5.0.0/src/momotor/django/token_store/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2606 2024-04-16 08:01:09.000000 momotor_django-5.0.0/src/momotor/django/token_store/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1361 2024-04-16 08:01:09.000000 momotor_django-5.0.0/src/momotor/django/token_store/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)      349 2024-04-16 08:01:09.000000 momotor_django-5.0.0/src/momotor/django/token_store/dummy.py
+-rw-rw-rw-   0 root         (0) root         (0)      543 2024-04-16 08:01:09.000000 momotor_django-5.0.0/src/momotor/django/token_store/memory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1750 2024-04-16 08:01:09.000000 momotor_django-5.0.0/src/momotor/django/token_store/model.py
+-rw-rw-rw-   0 root         (0) root         (0)       63 2024-04-16 08:01:09.000000 momotor_django-5.0.0/src/momotor/django/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:01:53.000000 momotor_django-5.0.0/src/momotor_django.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2643 2024-04-16 08:01:53.000000 momotor_django-5.0.0/src/momotor_django.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1336 2024-04-16 08:01:53.000000 momotor_django-5.0.0/src/momotor_django.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 08:01:53.000000 momotor_django-5.0.0/src/momotor_django.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      348 2024-04-16 08:01:53.000000 momotor_django-5.0.0/src/momotor_django.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-16 08:01:53.000000 momotor_django-5.0.0/src/momotor_django.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       37 2024-04-16 08:01:49.000000 momotor_django-5.0.0/version.toml
```

### Comparing `momotor-django-4.1.0/README.md` & `momotor_django-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `momotor-django-4.1.0/src/momotor/django/admin.py` & `momotor_django-5.0.0/src/momotor/django/admin.py`

 * *Files identical despite different names*

### Comparing `momotor-django-4.1.0/src/momotor/django/connection.py` & `momotor_django-5.0.0/src/momotor/django/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 import asyncio
-import sys
-import warnings
-from contextlib import asynccontextmanager
+import collections.abc
+import importlib.metadata
 import logging
-import time
 import typing
+import warnings
+from contextlib import asynccontextmanager
+from functools import lru_cache
 from importlib import import_module
 
 import backoff
+import sys
+import time
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
 from google.protobuf.empty_pb2 import Empty
 from google.protobuf.message import Message
 from grpclib.exceptions import StreamTerminatedError, GRPCError
-from momotor.rpc.proto.job_pb2 import JobStatusStream
 
 from momotor.django.defaults import *
 from momotor.rpc.asset.exceptions import UnexpectedEndOfStream
 from momotor.rpc.auth.client import get_authenticated_channel
 from momotor.rpc.exception import raise_message_exception, RPCException, AuthException
 from momotor.rpc.proto.auth_pb2 import ServerInfoResponse
 from momotor.rpc.proto.client_grpc import ClientStub
+from momotor.rpc.proto.job_pb2 import JobStatusStream
 from momotor.rpc.utils import format_msg
-from momotor.rpc.version import __VERSION__ as PROTO_VERSION
 from momotor.shared.doc import annotate_docstring
 from momotor.shared.log import AsyncLogWrapper
 
 try:
     import ssl
 except ImportError:
     ssl = None
 
 if typing.TYPE_CHECKING:
-    import concurrent.futures.Executor
+    from concurrent.futures import Executor
 
 logger = logging.getLogger(__package__)
 async_logger = AsyncLogWrapper(logger)
 
 retry_exceptions = (ConnectionError, StreamTerminatedError, UnexpectedEndOfStream, GRPCError)
 if ssl:
     retry_exceptions += (ssl.SSLError, ssl.CertificateError, ssl.SSLEOFError)
@@ -44,41 +46,46 @@
 retry_connection = backoff.on_exception(
     backoff.expo,
     retry_exceptions,
     max_value=10,
     logger=logger
 )
 
-retry_connection.__doc__ = """
+retry_connection.__doc__ = f"""
     A decorator to retry a function when a transient connection error occurs.
     
     Catches the exception and retries the function several times whenever one of the following exceptions is raised:
     
     * :py:class:`ConnectionError`
     * :py:class:`grpclib.exceptions.GRPCError`
     * :py:class:`grpclib.exceptions.StreamTerminatedError`
     * :py:class:`momotor.rpc.asset.exceptions.UnexpectedEndOfStream`
     * :py:class:`ssl.CertificateError`
     * :py:class:`ssl.SSLEOFError`
     * :py:class:`ssl.SSLError`
     
     Produces log messages on the ``{logger.name}`` logger.
-""".format(logger=logger)
+"""
 
 
 def consume_task_result(task: asyncio.Task):
     try:
         task.result()
     except:
         pass
 
 
+@lru_cache(maxsize=1)
+def get_protocol_version():
+    return importlib.metadata.version('momotor-engine-proto')
+
+
 async def version_check(server_info: "ServerInfoResponse"):
-    if server_info.protoVersion != PROTO_VERSION:
-        msg = f"protocol version mismatch: client has {PROTO_VERSION}, broker has {server_info.protoVersion}"
+    if (local_version := get_protocol_version()) != (remote_version := server_info.protoVersion):
+        msg = f"protocol version mismatch: client has {local_version}, broker has {remote_version}"
         await async_logger.warning(msg)
 
 
 @retry_connection
 async def _retry_message(method, request, timeout=None):
     try:
         await async_logger.debug(f"RPC call {method.name} {format_msg(request)}")
@@ -138,15 +145,15 @@
     Produces log messages on the ``{logger.name}`` logger.
 
     :param loop: The :std:doc:`asyncio loop <python:library/asyncio-eventloop>` to use the `executor` with.
                  If `None`, uses the current active event loop. (Deprecated on Python 3.8)
     :param executor: An executor to run I/O blocking tasks on. If `None`, uses the current loop's default executor.
     :param token_pool_kwargs: Any additional keyword arguments are passed on to the :ref:`token store <token_store>`
     """
-    def __init__(self, *, loop=None, executor: "concurrent.futures.Executor" = None, **token_pool_kwargs):
+    def __init__(self, *, loop=None, executor: "Executor" = None, **token_pool_kwargs):
         if loop is not None and sys.version_info >= (3, 8):
             warnings.warn("The loop argument is deprecated since Python 3.8+", DeprecationWarning)
 
         self.loop = loop
 
         broker_settings = getattr(settings, 'MOMOTOR_BROKER')
         assert broker_settings is not None, 'MOMOTOR_BROKER missing from settings'
@@ -393,15 +400,15 @@
         asyncio.ensure_future(self.send_message(method_name, request, private_channel=private_channel, timeout=timeout))\
             .add_done_callback(consume_task_result)
 
     async def multi_job_status_stream(self, *,
                                       private_channel: bool = False,
                                       connect_timeout: float = None,
                                       status_timeout: float = None) \
-            -> typing.AsyncIterable[JobStatusStream]:
+            -> collections.abc.AsyncIterable[JobStatusStream]:
 
         """ Async generator that connects to the
         :py:func:`~momotor.rpc.proto.client_grpc.ClientBase.multiJobStatusStream` client endpoint and yields the
         :py:class:`~momotor.rpc.proto.job_pb2.JobStatusStream` status messages
 
         :param private_channel: `True` to use a private channel
         :param connect_timeout: timeout (in seconds) to wait until connected. `None` for no timeout
@@ -421,15 +428,15 @@
                 else:
                     connected = True
 
                 while connected and stub == self._client_stub:
                     try:
                         try:
                             message = typing.cast(
-                                typing.Optional[JobStatusStream],
+                                JobStatusStream | None,
                                 await asyncio.wait_for(stream.recv_message(), timeout=status_timeout)
                             )
 
                         except asyncio.TimeoutError:
                             await async_logger.debug(f"RPC call multiJobStatusStream recv timeout")
                             connected = False
```

### Comparing `momotor-django-4.1.0/src/momotor/django/fields.py` & `momotor_django-5.0.0/src/momotor/django/fields.py`

 * *Files identical despite different names*

### Comparing `momotor-django-4.1.0/src/momotor/django/forms.py` & `momotor_django-5.0.0/src/momotor/django/forms.py`

 * *Files identical despite different names*

### Comparing `momotor-django-4.1.0/src/momotor/django/migrations/0001_initial.py` & `momotor_django-5.0.0/src/momotor/django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `momotor-django-4.1.0/src/momotor/django/token_store/base.py` & `momotor_django-5.0.0/src/momotor/django/token_store/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+from __future__ import annotations
+
 import asyncio
+import collections.abc
 import typing
 from abc import ABC
 from functools import partial
 
 if typing.TYPE_CHECKING:
-    import concurrent.futures.Executor
+    from concurrent.futures import Executor
 
 
 class BaseTokenStore(ABC):
     """ Abstract base class for token stores. The store is provided with the :setting:`MOMOTOR_BROKER` settings
     and an :std:doc:`asyncio loop <python:library/asyncio-eventloop>` and
     :py:class:`executor <python:concurrent.futures.Executor>`.
 
@@ -20,31 +23,31 @@
     :param loop: The :std:doc:`asyncio loop <python:library/asyncio-eventloop>` to use the `executor` with.
                  If `None`, uses the current active event loop.
     :param executor: An executor to run I/O blocking tasks on. If `None`, uses the current loop's default executor.
     :param kwargs: The additional token store arguments passed to
                    :py:class:`~momotor.django.connection.BrokerConnection`
     """
 
-    def __init__(self, settings: dict, *, loop=None, executor: "concurrent.futures.Executor" = None, **kwargs):
+    def __init__(self, settings: dict, *, loop=None, executor: "Executor" = None, **kwargs):
         self.loop = loop or asyncio.get_running_loop()  #: The `loop` argument as provided to the constructor
         self.executor = executor  #: The `executor` argument as provided to the constructor
         self.settings = settings  #: The `settings` argument as provided to the constructor
 
-    def _run_in_executor(self, func: typing.Callable, *args, **kwargs):
+    def _run_in_executor(self, func: collections.abc.Callable, *args, **kwargs):
         """ Run a function in the executor provided to __init__
 
         :param func: function to run
         :param args: arguments to the function
         :param kwargs: keyword arguments to the function
         :return: return value of the function
         """
         callback = partial(func, *args, **kwargs)
         return self.loop.run_in_executor(self.executor, callback)
 
-    async def get(self) -> typing.Optional[str]:
+    async def get(self) -> str | None:
         """ Get the current token from the store
 
         :return: The token. Or `None` if not currently authorized
         """
         raise NotImplementedError
 
     async def set(self, token: str):
```

### Comparing `momotor-django-4.1.0/src/momotor/django/token_store/cache.py` & `momotor_django-5.0.0/src/momotor/django/token_store/cache.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from __future__ import annotations
+
 import asyncio
-import typing
 
 from django.core.cache import caches
 from django.utils.encoding import smart_str
 
 from momotor.django.defaults import DEFAULT_CACHE_KEY
 from momotor.django.token_store.memory import InMemoryTokenStore
 
@@ -13,15 +14,15 @@
     """
     def __init__(self, settings, *, loop=None, executor=None):
         super().__init__(settings, loop=loop, executor=executor)
         self.key = settings.get('TOKEN_KEY', DEFAULT_CACHE_KEY).format(settings)
         self.cache = caches[settings.get('TOKEN_CACHE_NAME', 'default')]
         self.lock = asyncio.Lock()
 
-    async def get(self) -> typing.Optional[str]:
+    async def get(self) -> str | None:
         async with self.lock:
             token = await super().get()
             if token is None:
                 token = await self._run_in_executor(self.cache.get, self.key)
                 if token:
                     await super().set(token)
```

### Comparing `momotor-django-4.1.0/src/momotor/django/token_store/memory.py` & `momotor_django-5.0.0/src/momotor/django/token_store/memory.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import typing
+from __future__ import annotations
 
 from momotor.django.token_store.base import BaseTokenStore
 
 
 class InMemoryTokenStore(BaseTokenStore):
     """ Token store that saves tokens in memory
     """
     def __init__(self, settings, *, loop=None, executor=None):
         super().__init__(settings, loop=loop, executor=executor)
         self.__token = None
 
-    async def get(self) -> typing.Optional[str]:
+    async def get(self) -> str | None:
         return self.__token
 
     async def set(self, token: str):
         self.__token = token
 
     async def delete(self):
         self.__token = None
```

### Comparing `momotor-django-4.1.0/src/momotor/django/token_store/model.py` & `momotor_django-5.0.0/src/momotor/django/token_store/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from __future__ import annotations
+
 import asyncio
-import typing
 
 from django.core.exceptions import ObjectDoesNotExist
 
 from momotor.django.models import MomotorToken
 from momotor.django.token_store.memory import InMemoryTokenStore
 
 
@@ -15,15 +16,15 @@
 
         db = token_model.objects
         db_name = settings.get('TOKEN_DATABASE_NAME')
         self.db = db.using(db_name) if db_name else db
         self.api_key = settings['API_KEY']
         self.lock = asyncio.Lock()
 
-    async def get(self) -> typing.Optional[str]:
+    async def get(self) -> str | None:
         async with self.lock:
             token = await super().get()
             if token is None:
                 try:
                     obj = await self._run_in_executor(self.db.get, api_key=self.api_key)
                 except ObjectDoesNotExist:
                     pass
```

### Comparing `momotor-django-4.1.0/src/momotor_django.egg-info/SOURCES.txt` & `momotor_django-5.0.0/src/momotor_django.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,46 @@
+.gitignore
+.gitlab-ci.yml
+CHANGELOG.md
 README.md
+publish-docs.sh
+pyproject.toml
+semver.sh
 setup.py
+version.toml
+.idea/modules.xml
+.idea/momotor.lib.django.iml
+.idea/inspectionProfiles/profiles_settings.xml
+docs/Makefile
+docs/make.bat
+docs/source/conf.py
+docs/source/connection.rst
+docs/source/index.rst
+docs/source/settings.rst
+docs/source/tokenstore.rst
+docs/source/_ext/djangoroles.py
+docs/source/_static/logo-text-negative.png
+docs/source/_static/logo-text.png
+docs/source/_templates/projectlinks.html
 src/momotor/django/__init__.py
 src/momotor/django/admin.py
 src/momotor/django/apps.py
 src/momotor/django/connection.py
 src/momotor/django/defaults.py
 src/momotor/django/fields.py
 src/momotor/django/forms.py
 src/momotor/django/models.py
 src/momotor/django/tests.py
-src/momotor/django/version.py
 src/momotor/django/views.py
 src/momotor/django/migrations/0001_initial.py
 src/momotor/django/migrations/__init__.py
 src/momotor/django/token_store/__init__.py
 src/momotor/django/token_store/base.py
 src/momotor/django/token_store/cache.py
 src/momotor/django/token_store/dummy.py
 src/momotor/django/token_store/memory.py
 src/momotor/django/token_store/model.py
 src/momotor_django.egg-info/PKG-INFO
 src/momotor_django.egg-info/SOURCES.txt
 src/momotor_django.egg-info/dependency_links.txt
-src/momotor_django.egg-info/not-zip-safe
 src/momotor_django.egg-info/requires.txt
 src/momotor_django.egg-info/top_level.txt
```

