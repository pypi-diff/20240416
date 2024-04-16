# Comparing `tmp/python-fmrest-1.7.2.tar.gz` & `tmp/python-fmrest-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-fmrest-1.7.2.tar", last modified: Fri Mar 15 23:10:24 2024, max compression
+gzip compressed data, was "python-fmrest-1.7.3.tar", last modified: Tue Apr 16 16:37:53 2024, max compression
```

## Comparing `python-fmrest-1.7.2.tar` & `python-fmrest-1.7.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 dh         (501) staff       (20)        0 2024-03-15 23:10:24.247000 python-fmrest-1.7.2/
--rw-r--r--   0 dh         (501) staff       (20)     1069 2017-10-17 10:46:48.000000 python-fmrest-1.7.2/LICENSE
--rw-r--r--   0 dh         (501) staff       (20)     4143 2024-03-15 23:10:24.246890 python-fmrest-1.7.2/PKG-INFO
--rw-r--r--   0 dh         (501) staff       (20)     3611 2022-07-11 09:44:42.000000 python-fmrest-1.7.2/README.md
-drwxr-xr-x   0 dh         (501) staff       (20)        0 2024-03-15 23:10:24.245917 python-fmrest-1.7.2/fmrest/
--rw-r--r--   0 dh         (501) staff       (20)      158 2020-12-08 23:30:08.000000 python-fmrest-1.7.2/fmrest/__init__.py
--rw-r--r--   0 dh         (501) staff       (20)     7480 2022-06-14 09:58:52.000000 python-fmrest-1.7.2/fmrest/cloudserver.py
--rw-r--r--   0 dh         (501) staff       (20)     1304 2024-01-18 14:57:44.000000 python-fmrest-1.7.2/fmrest/const.py
--rw-r--r--   0 dh         (501) staff       (20)     2215 2024-03-15 22:35:08.000000 python-fmrest-1.7.2/fmrest/exceptions.py
--rw-r--r--   0 dh         (501) staff       (20)     3281 2020-10-06 16:49:35.000000 python-fmrest-1.7.2/fmrest/foundset.py
--rw-r--r--   0 dh         (501) staff       (20)     6603 2020-10-06 16:49:35.000000 python-fmrest-1.7.2/fmrest/record.py
--rw-r--r--   0 dh         (501) staff       (20)    44232 2024-03-15 23:08:44.000000 python-fmrest-1.7.2/fmrest/server.py
--rw-r--r--   0 dh         (501) staff       (20)     5937 2022-04-15 12:37:37.000000 python-fmrest-1.7.2/fmrest/utils.py
-drwxr-xr-x   0 dh         (501) staff       (20)        0 2024-03-15 23:10:24.246708 python-fmrest-1.7.2/python_fmrest.egg-info/
--rw-r--r--   0 dh         (501) staff       (20)     4143 2024-03-15 23:10:24.000000 python-fmrest-1.7.2/python_fmrest.egg-info/PKG-INFO
--rw-r--r--   0 dh         (501) staff       (20)      357 2024-03-15 23:10:24.000000 python-fmrest-1.7.2/python_fmrest.egg-info/SOURCES.txt
--rw-r--r--   0 dh         (501) staff       (20)        1 2024-03-15 23:10:24.000000 python-fmrest-1.7.2/python_fmrest.egg-info/dependency_links.txt
--rw-r--r--   0 dh         (501) staff       (20)       38 2024-03-15 23:10:24.000000 python-fmrest-1.7.2/python_fmrest.egg-info/requires.txt
--rw-r--r--   0 dh         (501) staff       (20)        7 2024-03-15 23:10:24.000000 python-fmrest-1.7.2/python_fmrest.egg-info/top_level.txt
--rw-r--r--   0 dh         (501) staff       (20)       38 2024-03-15 23:10:24.247046 python-fmrest-1.7.2/setup.cfg
--rw-r--r--   0 dh         (501) staff       (20)      860 2024-03-15 23:07:46.000000 python-fmrest-1.7.2/setup.py
+drwxr-xr-x   0 dh         (501) staff       (20)        0 2024-04-16 16:37:53.166517 python-fmrest-1.7.3/
+-rw-r--r--   0 dh         (501) staff       (20)     1069 2017-10-17 10:46:48.000000 python-fmrest-1.7.3/LICENSE
+-rw-r--r--   0 dh         (501) staff       (20)     4143 2024-04-16 16:37:53.166407 python-fmrest-1.7.3/PKG-INFO
+-rw-r--r--   0 dh         (501) staff       (20)     3611 2022-07-11 09:44:42.000000 python-fmrest-1.7.3/README.md
+drwxr-xr-x   0 dh         (501) staff       (20)        0 2024-04-16 16:37:53.165619 python-fmrest-1.7.3/fmrest/
+-rw-r--r--   0 dh         (501) staff       (20)      158 2020-12-08 23:30:08.000000 python-fmrest-1.7.3/fmrest/__init__.py
+-rw-r--r--   0 dh         (501) staff       (20)     7480 2022-06-14 09:58:52.000000 python-fmrest-1.7.3/fmrest/cloudserver.py
+-rw-r--r--   0 dh         (501) staff       (20)     1304 2024-01-18 14:57:44.000000 python-fmrest-1.7.3/fmrest/const.py
+-rw-r--r--   0 dh         (501) staff       (20)     2215 2024-03-15 22:35:08.000000 python-fmrest-1.7.3/fmrest/exceptions.py
+-rw-r--r--   0 dh         (501) staff       (20)     3281 2020-10-06 16:49:35.000000 python-fmrest-1.7.3/fmrest/foundset.py
+-rw-r--r--   0 dh         (501) staff       (20)     6603 2020-10-06 16:49:35.000000 python-fmrest-1.7.3/fmrest/record.py
+-rw-r--r--   0 dh         (501) staff       (20)    44627 2024-04-16 16:33:07.000000 python-fmrest-1.7.3/fmrest/server.py
+-rw-r--r--   0 dh         (501) staff       (20)     5982 2024-04-16 16:32:27.000000 python-fmrest-1.7.3/fmrest/utils.py
+drwxr-xr-x   0 dh         (501) staff       (20)        0 2024-04-16 16:37:53.166215 python-fmrest-1.7.3/python_fmrest.egg-info/
+-rw-r--r--   0 dh         (501) staff       (20)     4143 2024-04-16 16:37:53.000000 python-fmrest-1.7.3/python_fmrest.egg-info/PKG-INFO
+-rw-r--r--   0 dh         (501) staff       (20)      357 2024-04-16 16:37:53.000000 python-fmrest-1.7.3/python_fmrest.egg-info/SOURCES.txt
+-rw-r--r--   0 dh         (501) staff       (20)        1 2024-04-16 16:37:53.000000 python-fmrest-1.7.3/python_fmrest.egg-info/dependency_links.txt
+-rw-r--r--   0 dh         (501) staff       (20)       38 2024-04-16 16:37:53.000000 python-fmrest-1.7.3/python_fmrest.egg-info/requires.txt
+-rw-r--r--   0 dh         (501) staff       (20)        7 2024-04-16 16:37:53.000000 python-fmrest-1.7.3/python_fmrest.egg-info/top_level.txt
+-rw-r--r--   0 dh         (501) staff       (20)       38 2024-04-16 16:37:53.166571 python-fmrest-1.7.3/setup.cfg
+-rw-r--r--   0 dh         (501) staff       (20)      860 2024-04-16 16:33:33.000000 python-fmrest-1.7.3/setup.py
```

### Comparing `python-fmrest-1.7.2/LICENSE` & `python-fmrest-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python-fmrest-1.7.2/PKG-INFO` & `python-fmrest-1.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-fmrest
-Version: 1.7.2
+Version: 1.7.3
 Summary: python-fmrest is a wrapper around the FileMaker Data API.
 Home-page: https://github.com/davidhamann/python-fmrest
 Author: David Hamann
 Author-email: dh@davidhamann.de
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `python-fmrest-1.7.2/README.md` & `python-fmrest-1.7.3/README.md`

 * *Files identical despite different names*

### Comparing `python-fmrest-1.7.2/fmrest/cloudserver.py` & `python-fmrest-1.7.3/fmrest/cloudserver.py`

 * *Files identical despite different names*

### Comparing `python-fmrest-1.7.2/fmrest/const.py` & `python-fmrest-1.7.3/fmrest/const.py`

 * *Files identical despite different names*

### Comparing `python-fmrest-1.7.2/fmrest/exceptions.py` & `python-fmrest-1.7.3/fmrest/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-fmrest-1.7.2/fmrest/foundset.py` & `python-fmrest-1.7.3/fmrest/foundset.py`

 * *Files identical despite different names*

### Comparing `python-fmrest-1.7.2/fmrest/record.py` & `python-fmrest-1.7.3/fmrest/record.py`

 * *Files identical despite different names*

### Comparing `python-fmrest-1.7.2/fmrest/server.py` & `python-fmrest-1.7.3/fmrest/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 import importlib.util
 import warnings
 from typing import List, Dict, Optional, Any, IO, Tuple, Union, Iterator
 from functools import wraps
 import requests
 from .utils import (request, build_portal_params, build_script_params,
                     filename_from_url, PlaceholderDict)
-from .const import (PORTAL_PREFIX, FMSErrorCode, API_VERSIONS, API_DATE_FORMATS, API_PATH_PREFIX,
-                    API_PATH)
+from .const import (PORTAL_PREFIX, FMSErrorCode, API_VERSIONS,
+                    API_DATE_FORMATS, API_PATH_PREFIX,
+                    API_PATH, TIMEOUT)
 from .exceptions import BadJSON, FileMakerError, RecordError, BadGatewayError
 from .record import Record
 from .foundset import Foundset
 
 
 class Server(object):
     """The server class provides easy access to the FileMaker Data API
@@ -41,15 +42,16 @@
     def __init__(self, url: str, user: str,
                  password: str, database: str, layout: str,
                  data_sources: Optional[List[Dict]] = None,
                  verify_ssl: Union[bool, str] = True,
                  type_conversion: bool = False,
                  auto_relogin: bool = False,
                  proxies: Optional[Dict] = None,
-                 api_version: Optional[str] = None) -> None:
+                 api_version: Optional[str] = None,
+                 timeout: int = TIMEOUT) -> None:
         """Initialize the Server class.
 
         Parameters
         ----------
         url : str
             Address of the FileMaker Server, e.g. https://my-server.com or https://127.0.0.1
             Note: Data API must use https.
@@ -89,25 +91,30 @@
         proxies : dict, optional
             Pass requests through a proxy, configure like so:
             { 'https': 'http://127.0.0.1:8080' }
         api_version : str, optional
             Configure which version of the data API should be queried (e.g. v1)
             It is recommended to set the version explicitly to prevent
             potential future breaking changes.
+        timeout : int
+            Duration in seconds to wait for FMS to respond (HTTP timeout).
+            This takes priority over the legacy environment variable
+            "fmrest_timeout".
         """
 
         self.url = url
         self.user = user
         self.password = password
         self.database = database
         self.layout = layout
         self.data_sources = [] if data_sources is None else data_sources
         self.verify_ssl = verify_ssl
         self.auto_relogin = auto_relogin
         self.proxies = proxies
+        self.timeout = timeout
 
         if not api_version:
             warnings.warn('No api_version given. Defaulting to v1.')
             self.api_version = 'v1'
         elif api_version not in API_VERSIONS:
             raise ValueError(f'Invalid API version. Choose one of {API_VERSIONS}')
         else:
@@ -697,14 +704,15 @@
             calling response.close().
         """
         name = filename_from_url(file_url)
         response = request(method='get',
                            url=file_url,
                            verify=self.verify_ssl,
                            stream=stream,
+                           timeout=self.timeout,
                            proxies=self.proxies)
 
         return (name,
                 response.headers.get('Content-Type'),
                 response.headers.get('Content-Length'),
                 response)
 
@@ -916,14 +924,15 @@
         response = request(method=method,
                            headers=self._headers,
                            url=url,
                            data=request_data,
                            verify=self.verify_ssl,
                            params=params,
                            proxies=self.proxies,
+                           timeout=self.timeout,
                            **kwargs)
 
         if response.status_code == 502:
             raise BadGatewayError('Web server responded with a Bad Gateway '
                                   'error. Check if the Data API is enabled '
                                   'and responding.')
         try:
```

### Comparing `python-fmrest-1.7.2/fmrest/utils.py` & `python-fmrest-1.7.3/fmrest/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 import requests
 from .exceptions import RequestException
 from .const import TIMEOUT
 
 
 def request(*args, **kwargs) -> requests.Response:
     """Wrapper around requests library request call"""
+    timeout = kwargs.pop("timeout", TIMEOUT)
     try:
-        return requests.request(*args, timeout=TIMEOUT, **kwargs)
+        return requests.request(*args, timeout=timeout, **kwargs)
     except Exception as ex:
         raise RequestException(ex, args, kwargs) from None
 
 def build_portal_params(portals: List[Dict], names_as_string: bool = False) -> Dict[str, Any]:
     """Takes a list of dicts and returns a dict in a format as FMServer expects it.
 
     FMS expects portals and their options to be specified in the following format:
```

### Comparing `python-fmrest-1.7.2/python_fmrest.egg-info/PKG-INFO` & `python-fmrest-1.7.3/python_fmrest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-fmrest
-Version: 1.7.2
+Version: 1.7.3
 Summary: python-fmrest is a wrapper around the FileMaker Data API.
 Home-page: https://github.com/davidhamann/python-fmrest
 Author: David Hamann
 Author-email: dh@davidhamann.de
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `python-fmrest-1.7.2/setup.py` & `python-fmrest-1.7.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as ld:
     long_description = ld.read()
 
 setup(
     name='python-fmrest',
-    version='1.7.2',
+    version='1.7.3',
     python_requires='>=3.6',
     author='David Hamann',
     author_email='dh@davidhamann.de',
     description='python-fmrest is a wrapper around the FileMaker Data API.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/davidhamann/python-fmrest',
```

