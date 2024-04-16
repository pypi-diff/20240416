# Comparing `tmp/mure-0.6.1.tar.gz` & `tmp/mure-1.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mure-0.6.1.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `mure-0.6.1.tar` & `mure-1.0.0a0.tar`

### file list

```diff
@@ -1,9 +1,16 @@
--rw-r--r--   0        0        0    11345 2023-02-23 15:28:17.093066 mure-0.6.1/LICENSE
--rw-r--r--   0        0        0     5323 2023-02-23 15:28:17.093066 mure-0.6.1/README.md
--rw-r--r--   0        0        0     5979 2023-02-23 15:28:17.093066 mure-0.6.1/mure/__init__.py
--rw-r--r--   0        0        0     3831 2023-02-23 15:28:17.093066 mure-0.6.1/mure/dtos.py
--rw-r--r--   0        0        0     5344 2023-02-23 15:28:17.093066 mure-0.6.1/mure/iterator.py
--rw-r--r--   0        0        0     4064 2023-02-23 15:28:17.093066 mure-0.6.1/mure/logging.py
--rw-r--r--   0        0        0      811 2023-02-23 15:28:17.097066 mure-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     6326 1970-01-01 00:00:00.000000 mure-0.6.1/setup.py
--rw-r--r--   0        0        0     5942 1970-01-01 00:00:00.000000 mure-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 mure-1.0.0a0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 mure-1.0.0a0/requirements-dev.lock
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 mure-1.0.0a0/requirements.lock
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 mure-1.0.0a0/.github/workflows/main.yml
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 mure-1.0.0a0/examples/example.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 mure-1.0.0a0/mure/__init__.py
+-rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 mure-1.0.0a0/mure/core.py
+-rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 mure-1.0.0a0/mure/dtos.py
+-rw-r--r--   0        0        0     8559 2020-02-02 00:00:00.000000 mure-1.0.0a0/mure/iterator.py
+-rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 mure-1.0.0a0/mure/logging.py
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 mure-1.0.0a0/tests/test_mure.py
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 mure-1.0.0a0/.gitignore
+-rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 mure-1.0.0a0/LICENSE
+-rw-r--r--   0        0        0     6526 2020-02-02 00:00:00.000000 mure-1.0.0a0/README.md
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 mure-1.0.0a0/pyproject.toml
+-rw-r--r--   0        0        0     6902 2020-02-02 00:00:00.000000 mure-1.0.0a0/PKG-INFO
```

### Comparing `mure-0.6.1/LICENSE` & `mure-1.0.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `mure-0.6.1/README.md` & `mure-1.0.0a0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -18,56 +18,58 @@
 
 ```
 pip install mure
 ```
 
 ## Usage
 
-Pass an iterable of dictionaries (a typed dictionary `Resource`, to be precise) with at least a value for `url` and get a `ResponseIterator` with the corresponding responses:
+Pass a list of dictionaries with at least a value for `url` and get a `ResponseIterator` with the corresponding responses. The first request is fired as soon as you access the first response:
 
 ```python
 >>> import mure
 >>> from mure.dtos import Resource
 >>> resources: list[Resource] = [
 ...     {"url": "https://httpbin.org/get"},
 ...     {"url": "https://httpbin.org/get", "params": {"foo": "bar"}},
 ...     {"url": "invalid"},
 ... ]
 >>> responses = mure.get(resources, batch_size=2)
 >>> responses
-<ResponseIterator: 3 pending>
+<ResponseIterator: 3/3 pending>
 >>> for resource, response in zip(resources, responses):
 ...     print(resource, "status code:", response.status)
 ...
 {'url': 'https://httpbin.org/get'} status code: 200
 {'url': 'https://httpbin.org/get', 'params': {'foo': 'bar'}} status code: 200
 {'url': 'invalid'} status code: 0
 >>> responses
-<ResponseIterator: 0 pending>
+<ResponseIterator: 0/3 pending>
 ```
 
-The keyword argument `batch_size` defines the number of requests to perform in parallel (don't be too greedy). The resources are requested batch-wise, i. e. only one batch of responses is kept in memory (depends of course also on how you use the `ResponseIterator`).
+The keyword argument `batch_size` defines the number of requests to perform in parallel (don't be too greedy). The resources are requested batch-wise, i. e. only one batch of responses is kept in memory (depends of course also on how you use the `ResponseIterator`). Once you start accessing the first response of a batch, the next batch of resources is requested already in the background. So while you are doing something with a batch of responses (e.g. some CPU-heavy operation like parsing HTML), the next batch is already requested in the background.
 
-For example, if you set `batch_size` to `2`, have four resources and execute:
+For example, if you have four resources, set `batch_size` to `2` and execute:
 
 ```python
 >>> next(responses)
 ```
 
-the first two resources are requested in parallel and blocks until both of the responses are available (i.e. if resource 1 takes 1 second and resource 2 takes 10 seconds, it blocks 10 seconds although resource 1 is already available after 1 second). The response of resource 1 is yielded.
+the first two resources are requested in parallel and blocks until both of the responses are available (i.e. if resource 1 takes 1 second and resource 2 takes 10 seconds, it blocks 10 seconds although resource 1 is already available after 1 second). Before the response of resource 1 is yielded, the next batch of resources (i.e. 3 and 4) is already requested in the background.
 
 Executing `next()` a second time:
 
 ```python
->>> next(response)
+>>> next(responses)
 ```
 
-will be super fast, because the response of resource 2 is already available. Executing `next()` a third time will be "slow" again, because the next batch of resources is requested.
+will be super fast, because the response of resource 2 is already available (1 and 2 were in the same batch). If you are lucky, executing `next()` a third time will be fast as well, because the next batch of resources was already requested when you executed `next(responses)` the first time.
+
+### HTTP Methods
 
-However, there is also a convenience function for POST requests:
+There are convenience functions for GET, POST, HEAD, PUT, PATCH and DELETE requests, for example:
 
 ```python
 >>> resources = [
 ...     {"url": "https://httpbin.org/post"},
 ...     {"url": "https://httpbin.org/post", "json": {"foo": "bar"}},
 ...     {"url": "invalid"},
 ... ]
@@ -83,14 +85,20 @@
 ...     {"method": "POST", "url": "https://httpbin.org/post"},
 ...     {"method": "POST", "url": "https://httpbin.org/post", "json": {"foo": "bar"}},
 ...     {"method": "GET", "url": "invalid"},
 ... ]
 >>> responses = mure.request(resources)
 ```
 
+## Tips
+
+- Set timeouts (e.g. 10 seconds) to avoid waiting for too long.
+- It might be a good idea to order the URLs to be requested by domain names so that DNS resolution is done once per domain. Once a domain's IP has been resolved, subsequent requests to the same domain can benefit from cached DNS resolutions. Also when using protocols like HTTP/1.1, connections to the same domain can be reused. Batching requests by domain can allow for connection reuse.
+- Shuffling URLs randomly might be an alternative if you do not request the same domain multiple times. This helps in distributing potential slow URLs across different batches.
+
 ### Verbosity
 
 Control verbosity with the `log_errors` argument:
 
 ```python
 >>> import mure
 >>> next(mure.get([{"url": "invalid"}], log_errors=True))
```

### Comparing `mure-0.6.1/mure/__init__.py` & `mure-1.0.0a0/mure/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,201 +1,218 @@
-from typing import Iterable
-
-from mure.dtos import HTTPMethod, HTTPResource, Resource
+from mure.dtos import DELETE, GET, HEAD, PATCH, POST, PUT, HTTPMethod, HTTPResource, Resource
 from mure.iterator import ResponseIterator
 
 
 def request(
-    resources: Iterable[HTTPResource], *, batch_size: int = 5, log_errors: bool = True
+    resources: list[HTTPResource],
+    *,
+    batch_size: int = 5,
+    log_errors: bool = True,
 ) -> ResponseIterator:
     """Perform HTTP request for each resource in the given batch.
 
     Parameters
     ----------
-    resources : Iterable[HTTPResource]
+    resources : list[HTTPResource]
         Resources to request.
     batch_size : int
         Number of resources to request in parallel, by default 5.
     log_errors : bool, optional
         True if Python errors should be logged, by default True.
 
     Returns
     -------
     ResponseIterator
         The server's responses for each resource.
     """
+    if not isinstance(resources, list):
+        raise TypeError(f"Expected list of resources, got {type(resources)}")
+
+    if any("method" not in resource for resource in resources):
+        raise KeyError("Missing HTTP method in resource")
+
+    if any("url" not in resource for resource in resources):
+        raise KeyError("Missing URL in resource")
+
     return ResponseIterator(resources, batch_size=batch_size, log_errors=log_errors)
 
 
 def get(
-    resources: Iterable[Resource], *, batch_size: int = 5, log_errors: bool = True
+    resources: list[Resource],
+    *,
+    batch_size: int = 5,
+    log_errors: bool = True,
 ) -> ResponseIterator:
-    """Perform GET HTTP request for each resource in the given batch.
+    """Perform a GET request for each resource.
 
     Parameters
     ----------
-    resources : Iterable[Resource]
+    resources : list[Resource]
         Resources to request.
     batch_size : int
         Number of resources to request in parallel, by default 5.
     log_errors : bool, optional
         True if Python errors should be logged, by default True.
 
     Returns
     -------
     ResponseIterator
         The server's responses for each resource.
     """
-    return _request("GET", resources, batch_size=batch_size, log_errors=log_errors)
+    return _request(GET, resources, batch_size=batch_size, log_errors=log_errors)
 
 
 def post(
-    resources: Iterable[Resource], *, batch_size: int = 5, log_errors: bool = True
+    resources: list[Resource],
+    *,
+    batch_size: int = 5,
+    log_errors: bool = True,
 ) -> ResponseIterator:
-    """Perform GET HTTP request for each resource in the given batch.
+    """Perform a POST request for each resource.
 
     Parameters
     ----------
-    resources : Iterable[Resource]
+    resources : list[Resource]
         Resources to request.
     batch_size : int
         Number of items to request per batch in parallel, by default 5.
     log_errors : bool, optional
         True if Python errors should be logged, by default True.
 
     Returns
     -------
     ResponseIterator
         The server's responses for each resource.
     """
-    return _request("POST", resources, batch_size=batch_size, log_errors=log_errors)
+    return _request(POST, resources, batch_size=batch_size, log_errors=log_errors)
 
 
 def put(
-    resources: Iterable[Resource], *, batch_size: int = 5, log_errors: bool = True
+    resources: list[Resource],
+    *,
+    batch_size: int = 5,
+    log_errors: bool = True,
 ) -> ResponseIterator:
-    """Perform PUT HTTP request for each resource in the given batch.
+    """Perform a PUT request for each resource.
 
     Parameters
     ----------
-    resources : Iterable[Resource]
+    resources : list[Resource]
         Resources to request.
     batch_size : int
         Number of items to request per batch in parallel, by default 5.
     log_errors : bool, optional
         True if Python errors should be logged, by default True.
 
     Returns
     -------
     ResponseIterator
         The server's responses for each resource.
     """
-    return _request("PUT", resources, batch_size=batch_size, log_errors=log_errors)
+    return _request(PUT, resources, batch_size=batch_size, log_errors=log_errors)
 
 
 def patch(
-    resources: Iterable[Resource], *, batch_size: int = 5, log_errors: bool = True
+    resources: list[Resource],
+    *,
+    batch_size: int = 5,
+    log_errors: bool = True,
 ) -> ResponseIterator:
-    """Perform PATCH HTTP request for each resource in the given batch.
+    """Perform a PATCH request for each resource.
 
     Parameters
     ----------
-    resources : Iterable[Resource]
+    resources : list[Resource]
         Resources to request.
     batch_size : int
         Number of items to request per batch in parallel, by default 5.
     log_errors : bool, optional
         True if Python errors should be logged, by default True.
 
     Returns
     -------
     ResponseIterator
         The server's responses for each resource.
     """
-    return _request("PATCH", resources, batch_size=batch_size, log_errors=log_errors)
+    return _request(PATCH, resources, batch_size=batch_size, log_errors=log_errors)
 
 
 def delete(
-    resources: Iterable[Resource], *, batch_size: int = 5, log_errors: bool = True
+    resources: list[Resource],
+    *,
+    batch_size: int = 5,
+    log_errors: bool = True,
 ) -> ResponseIterator:
-    """Perform DELETE HTTP request for each resource in the given batch.
+    """Perform a DELETE request for each resource.
 
     Parameters
     ----------
-    resources : Iterable[Resource]
+    resources : list[Resource]
         Resources to request.
     batch_size : int
         Number of items to request per batch in parallel, by default 5.
     log_errors : bool, optional
         True if Python errors should be logged, by default True.
 
     Returns
     -------
     ResponseIterator
         The server's responses for each resource.
     """
-    return _request("DELETE", resources, batch_size=batch_size, log_errors=log_errors)
+    return _request(DELETE, resources, batch_size=batch_size, log_errors=log_errors)
 
 
 def head(
-    resources: Iterable[Resource], *, batch_size: int = 5, log_errors: bool = True
+    resources: list[Resource],
+    *,
+    batch_size: int = 5,
+    log_errors: bool = True,
 ) -> ResponseIterator:
-    """Perform HEAD HTTP request for each resource in the given batch.
+    """Perform a HEAD request for each resource.
 
     Parameters
     ----------
-    resources : Iterable[Resource]
+    resources : list[Resource]
         Resources to request.
     batch_size : int
         Number of items to request per batch in parallel, by default 5.
     log_errors : bool, optional
         True if Python errors should be logged, by default True.
 
     Returns
     -------
     ResponseIterator
         The server's responses for each resource.
     """
-    return _request("HEAD", resources, batch_size=batch_size, log_errors=log_errors)
+    return _request(HEAD, resources, batch_size=batch_size, log_errors=log_errors)
 
 
 def _request(
     method: HTTPMethod,
-    resources: Iterable[Resource],
+    resources: list[Resource],
     *,
     batch_size: int = 5,
-    log_errors: bool = True
+    log_errors: bool = True,
 ) -> ResponseIterator:
-    """Perform HTTP request using the specified method for each resource in the given batch.
-
-    Note
-    ----
-    Only for internal use; preserves the type of the iterable (i.e. generator stays a generator).
+    """Perform a HTTP request using the specified method for each resource.
 
     Parameters
     ----------
     method : HTTPMethod
         HTTP method to use.
-    resources : Iterable[HTTPResource]
+    resources : list[HTTPResource]
         Resources to request.
     batch_size : int
         Number of resources to request in parallel, by default 5.
     log_errors : bool, optional
         True if Python errors should be logged, by default True.
 
     Returns
     -------
     ResponseIterator
         The server's responses for each resource.
     """
-    if isinstance(resources, list):
-        return request(
-            [{**resource, "method": method} for resource in resources],
-            batch_size=batch_size,
-            log_errors=log_errors,
-        )
-    else:
-        return request(
-            ({**resource, "method": method} for resource in resources),
-            batch_size=batch_size,
-            log_errors=log_errors,
-        )
+    return request(
+        [{**resource, "method": method} for resource in resources],
+        batch_size=batch_size,
+        log_errors=log_errors,
+    )
```

### Comparing `mure-0.6.1/mure/dtos.py` & `mure-1.0.0a0/mure/dtos.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,26 @@
+import json
+from collections.abc import Iterable, Mapping
 from dataclasses import dataclass
 from ssl import SSLContext
 from types import SimpleNamespace
-from typing import Any, Iterable, Literal, Mapping, TypedDict
+from typing import Any, Literal, NotRequired, TypedDict
 from urllib.parse import urlparse
 
-import orjson
 from aiohttp import BasicAuth, ClientTimeout, Fingerprint
 from aiohttp.typedefs import LooseCookies, LooseHeaders, StrOrURL
 
-try:
-    from typing import NotRequired
-except ImportError:
-    from typing_extensions import NotRequired
-
-
 # allowed http methods
+GET = "GET"
+POST = "POST"
+HEAD = "HEAD"
+PUT = "PUT"
+PATCH = "PATCH"
+DELETE = "DELETE"
+
 HTTPMethod = Literal["GET", "POST", "HEAD", "PUT", "PATCH", "DELETE"]
 
 
 class Resource(TypedDict):
     """Resource with at least a URL specified."""
 
     url: str
@@ -107,15 +109,15 @@
         """Deserialize JSON to Python objects.
 
         Returns
         -------
         Any
             Parsed Python objects.
         """
-        return orjson.loads(self.text)
+        return json.loads(self.text)
 
     def __getitem__(self, attr: str) -> int | str | bool:
         """Get the specified attribute.
 
         Parameters
         ----------
         attr : str
@@ -125,15 +127,15 @@
         -------
         int | str | bool
             Attribute value.
         """
         return getattr(self, attr)
 
     def is_same_netloc(self, url: str) -> bool:
-        """True if the given URL has the same netloc as the response URL.
+        """Return True if the given URL has the same netloc as the response URL.
 
         Parameters
         ----------
         url : str
             URL to check.
 
         Returns
```

### Comparing `mure-0.6.1/mure/logging.py` & `mure-1.0.0a0/mure/logging.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,44 @@
-import logging
 import sys
-from logging import StreamHandler
+from logging import Formatter, StreamHandler, getLogger
+from logging import Logger as _Logger
 
 DEBUG = 10
 INFO = 20
 WARNING = 30
 ERROR = 40
 LEVELS = {"DEBUG": DEBUG, "INFO": INFO, "WARNING": WARNING, "ERROR": ERROR}
 
 
 class Logger:
-    def __init__(self, name: str):
-        """Basic logger.
+    """Basic logger."""
 
-        Parameters
-        ----------
-        name : str
-            Name of the logger.
-        """
+    def __init__(self, name: str):
         self.name = name
 
         # return a logger with the specified name, creating it if necessary
-        self._logger = logging.getLogger(name)
+        self._logger = getLogger(name)
+        self._formatter = Formatter("[%(asctime)s] [%(levelname)s] %(message)s")
 
         # stream handler to stdout
         self._stream_handler = StreamHandler(sys.stdout)
+        self._stream_handler.setFormatter(self._formatter)
         self._logger.addHandler(self._stream_handler)
 
         # set level of both the logger and the handler to INFO by default
         self.set_level("INFO")
 
     def set_level(self, level: str | int):
+        """Set log level.
+
+        Parameters
+        ----------
+        level : str | int
+            Level to set.
+        """
         # translate string to integer
         if isinstance(level, str):
             level = LEVELS[level.upper()]
 
         # set the logger's level
         self._logger.setLevel(level)
 
@@ -50,15 +54,15 @@
         message : str
             Message to log.
         """
         if self._logger.isEnabledFor(DEBUG):
             self._logger._log(DEBUG, message, ())
 
     def info(self, message: str):
-        """Info log message
+        """Info log message.
 
         Parameters
         ----------
         message : str
             Message to log
         """
         if self._logger.isEnabledFor(INFO):
@@ -109,60 +113,61 @@
         -------
         int
             Log level.
         """
         return self._logger.level
 
     def __repr__(self):
+        """Representation of the logger."""
         return f"<Logger: {self.name} ({self.level})>"
 
 
-def get_logger(name: str) -> logging.Logger:
-    """Gets the specified logger object.
+def get_logger(name: str) -> _Logger:
+    """Get the specified logger object.
 
     Parameters
     ----------
     name : str
         Name of the module to get the logger for.
 
     Returns
     -------
-    logging.Logger
+    _Logger
         Logger of the specified module.
     """
-    return logging.getLogger(name)
+    return getLogger(name)
 
 
 def logger_exists(name: str) -> bool:
-    """Checks if a logger exists for the specified module.
+    """Check if a logger exists for the specified module.
 
     Parameters
     ----------
     name : str
         Name of the module to check the logger for.
 
     Returns
     -------
     bool
         True if logger exists, False otherwise.
     """
-    return logging.getLogger(name).hasHandlers()
+    return getLogger(name).hasHandlers()
 
 
 def set_level(name: str, level: int | str):
-    """Sets log level for the specified logger.
+    """Set log level for the specified logger.
 
     Parameters
     ----------
     name : str
         Name of the module.
     level : int | str
         Level to set.
     """
-    logger = logging.getLogger(name)
+    logger = getLogger(name)
 
     # translate string to integer
     if isinstance(level, str):
         level = LEVELS[level.upper()]
 
     # set the logger's level
     logger.setLevel(level)
```

### Comparing `mure-0.6.1/setup.py` & `mure-1.0.0a0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,134 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['mure']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['aiohttp[speedups]>=3.8.3,<4.0.0', 'orjson>=3.8.5,<4.0.0']
-
-extras_require = \
-{':python_version < "3.11"': ['typing-extensions>=4.5.0,<5.0.0']}
-
-setup_kwargs = {
-    'name': 'mure',
-    'version': '0.6.1',
-    'description': 'Perform multiple HTTP requests in parallel – without writing boilerplate code or worrying about async functions.',
-    'long_description': '# mure\n\n[![downloads](https://static.pepy.tech/personalized-badge/mure?period=total&units=international_system&left_color=black&right_color=black&left_text=downloads)](https://pepy.tech/project/mure)\n[![downloads/month](https://static.pepy.tech/personalized-badge/mure?period=month&units=abbreviation&left_color=black&right_color=black&left_text=downloads/month)](https://pepy.tech/project/mure)\n[![downloads/week](https://static.pepy.tech/personalized-badge/mure?period=week&units=abbreviation&left_color=black&right_color=black&left_text=downloads/week)](https://pepy.tech/project/mure)\n\nThis is a thin layer on top of [`aiohttp`](https://docs.aiohttp.org/en/stable/) to perform multiple HTTP requests in parallel – without writing boilerplate code or worrying about `async` functions.\n\n`mure` means **mu**ltiple **re**quests, but is also the German term for a form of mass wasting involving fast-moving flow of debris and dirt that has become liquified by the addition of water.\n\n![Göscheneralp. Kolorierung des Dias durch Margrit Wehrli-Frey](https://upload.wikimedia.org/wikipedia/commons/thumb/6/6b/ETH-BIB-Muhrgang_zur_Kehlen-Reuss_vom_Rotfirn-Dia_247-13368.tif/lossy-page1-1280px-ETH-BIB-Muhrgang_zur_Kehlen-Reuss_vom_Rotfirn-Dia_247-13368.tif.jpg)\n\n(The photo was taken by [Leo Wehrli](https://de.wikipedia.org/wiki/Leo_Wehrli) and is licensed under CC BY-SA 4.0)\n\n## Installation\n\nInstall the latest stable version from [PyPI](https://pypi.org/project/mure):\n\n```\npip install mure\n```\n\n## Usage\n\nPass an iterable of dictionaries (a typed dictionary `Resource`, to be precise) with at least a value for `url` and get a `ResponseIterator` with the corresponding responses:\n\n```python\n>>> import mure\n>>> from mure.dtos import Resource\n>>> resources: list[Resource] = [\n...     {"url": "https://httpbin.org/get"},\n...     {"url": "https://httpbin.org/get", "params": {"foo": "bar"}},\n...     {"url": "invalid"},\n... ]\n>>> responses = mure.get(resources, batch_size=2)\n>>> responses\n<ResponseIterator: 3 pending>\n>>> for resource, response in zip(resources, responses):\n...     print(resource, "status code:", response.status)\n...\n{\'url\': \'https://httpbin.org/get\'} status code: 200\n{\'url\': \'https://httpbin.org/get\', \'params\': {\'foo\': \'bar\'}} status code: 200\n{\'url\': \'invalid\'} status code: 0\n>>> responses\n<ResponseIterator: 0 pending>\n```\n\nThe keyword argument `batch_size` defines the number of requests to perform in parallel (don\'t be too greedy). The resources are requested batch-wise, i. e. only one batch of responses is kept in memory (depends of course also on how you use the `ResponseIterator`).\n\nFor example, if you set `batch_size` to `2`, have four resources and execute:\n\n```python\n>>> next(responses)\n```\n\nthe first two resources are requested in parallel and blocks until both of the responses are available (i.e. if resource 1 takes 1 second and resource 2 takes 10 seconds, it blocks 10 seconds although resource 1 is already available after 1 second). The response of resource 1 is yielded.\n\nExecuting `next()` a second time:\n\n```python\n>>> next(response)\n```\n\nwill be super fast, because the response of resource 2 is already available. Executing `next()` a third time will be "slow" again, because the next batch of resources is requested.\n\nHowever, there is also a convenience function for POST requests:\n\n```python\n>>> resources = [\n...     {"url": "https://httpbin.org/post"},\n...     {"url": "https://httpbin.org/post", "json": {"foo": "bar"}},\n...     {"url": "invalid"},\n... ]\n>>> responses = mure.post(resources)\n```\n\nYou can even mix HTTP methods in the list of resources (but have to specify the method for each resource):\n\n```python\n>>> resources = [\n...     {"method": "GET", "url": "https://httpbin.org/get"},\n...     {"method": "GET", "url": "https://httpbin.org/get", "params": {"foo": "bar"}},\n...     {"method": "POST", "url": "https://httpbin.org/post"},\n...     {"method": "POST", "url": "https://httpbin.org/post", "json": {"foo": "bar"}},\n...     {"method": "GET", "url": "invalid"},\n... ]\n>>> responses = mure.request(resources)\n```\n\n### Verbosity\n\nControl verbosity with the `log_errors` argument:\n\n```python\n>>> import mure\n>>> next(mure.get([{"url": "invalid"}], log_errors=True))\ninvalid\nTraceback (most recent call last):\n  File "/home/severin/git/mure/mure/iterator.py", line 131, in _process\n    async with session.request(resource["method"], resource["url"], **kwargs) as response:\n  File "/home/severin/git/mure/.env/lib/python3.11/site-packages/aiohttp/client.py", line 1141, in __aenter__\n    self._resp = await self._coro\n                 ^^^^^^^^^^^^^^^^\n  File "/home/severin/git/mure/.env/lib/python3.11/site-packages/aiohttp/client.py", line 508, in _request\n    req = self._request_class(\n          ^^^^^^^^^^^^^^^^^^^^\n  File "/home/severin/git/mure/.env/lib/python3.11/site-packages/aiohttp/client_reqrep.py", line 305, in __init__\n    self.update_host(url)\n  File "/home/severin/git/mure/.env/lib/python3.11/site-packages/aiohttp/client_reqrep.py", line 364, in update_host\n    raise InvalidURL(url)\naiohttp.client_exceptions.InvalidURL: invalid\nResponse(status=0, reason=\'<InvalidURL invalid>\', ok=False, text=\'\')\n>>> next(mure.get([{"url": "invalid"}], log_errors=False))\nResponse(status=0, reason=\'<InvalidURL invalid>\', ok=False, text=\'\')\n```\n',
-    'author': 'Severin Simmler',
-    'author_email': 's.simmler@snapaddy.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.10,<4.0',
-}
-
-
-setup(**setup_kwargs)
+Metadata-Version: 2.3
+Name: mure
+Version: 1.0.0a0
+Summary: Perform multiple HTTP requests in parallel – without writing boilerplate code or worrying about async functions.
+Author-email: Severin Simmler <s.simmler@snapaddy.com>
+License-File: LICENSE
+Requires-Python: >=3.11
+Requires-Dist: aiohttp>=3.9.3
+Requires-Dist: chardet>=5.2.0
+Description-Content-Type: text/markdown
+
+# mure
+
+[![downloads](https://static.pepy.tech/personalized-badge/mure?period=total&units=international_system&left_color=black&right_color=black&left_text=downloads)](https://pepy.tech/project/mure)
+[![downloads/month](https://static.pepy.tech/personalized-badge/mure?period=month&units=abbreviation&left_color=black&right_color=black&left_text=downloads/month)](https://pepy.tech/project/mure)
+[![downloads/week](https://static.pepy.tech/personalized-badge/mure?period=week&units=abbreviation&left_color=black&right_color=black&left_text=downloads/week)](https://pepy.tech/project/mure)
+
+This is a thin layer on top of [`aiohttp`](https://docs.aiohttp.org/en/stable/) to perform multiple HTTP requests in parallel – without writing boilerplate code or worrying about `async` functions.
+
+`mure` means **mu**ltiple **re**quests, but is also the German term for a form of mass wasting involving fast-moving flow of debris and dirt that has become liquified by the addition of water.
+
+![Göscheneralp. Kolorierung des Dias durch Margrit Wehrli-Frey](https://upload.wikimedia.org/wikipedia/commons/thumb/6/6b/ETH-BIB-Muhrgang_zur_Kehlen-Reuss_vom_Rotfirn-Dia_247-13368.tif/lossy-page1-1280px-ETH-BIB-Muhrgang_zur_Kehlen-Reuss_vom_Rotfirn-Dia_247-13368.tif.jpg)
+
+(The photo was taken by [Leo Wehrli](https://de.wikipedia.org/wiki/Leo_Wehrli) and is licensed under CC BY-SA 4.0)
+
+## Installation
+
+Install the latest stable version from [PyPI](https://pypi.org/project/mure):
+
+```
+pip install mure
+```
+
+## Usage
+
+Pass a list of dictionaries with at least a value for `url` and get a `ResponseIterator` with the corresponding responses. The first request is fired as soon as you access the first response:
+
+```python
+>>> import mure
+>>> from mure.dtos import Resource
+>>> resources: list[Resource] = [
+...     {"url": "https://httpbin.org/get"},
+...     {"url": "https://httpbin.org/get", "params": {"foo": "bar"}},
+...     {"url": "invalid"},
+... ]
+>>> responses = mure.get(resources, batch_size=2)
+>>> responses
+<ResponseIterator: 3/3 pending>
+>>> for resource, response in zip(resources, responses):
+...     print(resource, "status code:", response.status)
+...
+{'url': 'https://httpbin.org/get'} status code: 200
+{'url': 'https://httpbin.org/get', 'params': {'foo': 'bar'}} status code: 200
+{'url': 'invalid'} status code: 0
+>>> responses
+<ResponseIterator: 0/3 pending>
+```
+
+The keyword argument `batch_size` defines the number of requests to perform in parallel (don't be too greedy). The resources are requested batch-wise, i. e. only one batch of responses is kept in memory (depends of course also on how you use the `ResponseIterator`). Once you start accessing the first response of a batch, the next batch of resources is requested already in the background. So while you are doing something with a batch of responses (e.g. some CPU-heavy operation like parsing HTML), the next batch is already requested in the background.
+
+For example, if you have four resources, set `batch_size` to `2` and execute:
+
+```python
+>>> next(responses)
+```
+
+the first two resources are requested in parallel and blocks until both of the responses are available (i.e. if resource 1 takes 1 second and resource 2 takes 10 seconds, it blocks 10 seconds although resource 1 is already available after 1 second). Before the response of resource 1 is yielded, the next batch of resources (i.e. 3 and 4) is already requested in the background.
+
+Executing `next()` a second time:
+
+```python
+>>> next(responses)
+```
+
+will be super fast, because the response of resource 2 is already available (1 and 2 were in the same batch). If you are lucky, executing `next()` a third time will be fast as well, because the next batch of resources was already requested when you executed `next(responses)` the first time.
+
+### HTTP Methods
+
+There are convenience functions for GET, POST, HEAD, PUT, PATCH and DELETE requests, for example:
+
+```python
+>>> resources = [
+...     {"url": "https://httpbin.org/post"},
+...     {"url": "https://httpbin.org/post", "json": {"foo": "bar"}},
+...     {"url": "invalid"},
+... ]
+>>> responses = mure.post(resources)
+```
+
+You can even mix HTTP methods in the list of resources (but have to specify the method for each resource):
+
+```python
+>>> resources = [
+...     {"method": "GET", "url": "https://httpbin.org/get"},
+...     {"method": "GET", "url": "https://httpbin.org/get", "params": {"foo": "bar"}},
+...     {"method": "POST", "url": "https://httpbin.org/post"},
+...     {"method": "POST", "url": "https://httpbin.org/post", "json": {"foo": "bar"}},
+...     {"method": "GET", "url": "invalid"},
+... ]
+>>> responses = mure.request(resources)
+```
+
+## Tips
+
+- Set timeouts (e.g. 10 seconds) to avoid waiting for too long.
+- It might be a good idea to order the URLs to be requested by domain names so that DNS resolution is done once per domain. Once a domain's IP has been resolved, subsequent requests to the same domain can benefit from cached DNS resolutions. Also when using protocols like HTTP/1.1, connections to the same domain can be reused. Batching requests by domain can allow for connection reuse.
+- Shuffling URLs randomly might be an alternative if you do not request the same domain multiple times. This helps in distributing potential slow URLs across different batches.
+
+### Verbosity
+
+Control verbosity with the `log_errors` argument:
+
+```python
+>>> import mure
+>>> next(mure.get([{"url": "invalid"}], log_errors=True))
+invalid
+Traceback (most recent call last):
+  File "/home/severin/git/mure/mure/iterator.py", line 131, in _process
+    async with session.request(resource["method"], resource["url"], **kwargs) as response:
+  File "/home/severin/git/mure/.env/lib/python3.11/site-packages/aiohttp/client.py", line 1141, in __aenter__
+    self._resp = await self._coro
+                 ^^^^^^^^^^^^^^^^
+  File "/home/severin/git/mure/.env/lib/python3.11/site-packages/aiohttp/client.py", line 508, in _request
+    req = self._request_class(
+          ^^^^^^^^^^^^^^^^^^^^
+  File "/home/severin/git/mure/.env/lib/python3.11/site-packages/aiohttp/client_reqrep.py", line 305, in __init__
+    self.update_host(url)
+  File "/home/severin/git/mure/.env/lib/python3.11/site-packages/aiohttp/client_reqrep.py", line 364, in update_host
+    raise InvalidURL(url)
+aiohttp.client_exceptions.InvalidURL: invalid
+Response(status=0, reason='<InvalidURL invalid>', ok=False, text='')
+>>> next(mure.get([{"url": "invalid"}], log_errors=False))
+Response(status=0, reason='<InvalidURL invalid>', ok=False, text='')
+```
```

