# Comparing `tmp/py-allspice-2.4.0.tar.gz` & `tmp/py_allspice-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-allspice-2.4.0.tar", last modified: Fri Oct 27 21:22:48 2023, max compression
+gzip compressed data, was "py_allspice-2.5.0.tar", last modified: Tue Apr 16 15:33:26 2024, max compression
```

## Comparing `py-allspice-2.4.0.tar` & `py_allspice-2.5.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:22:48.206292 py-allspice-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2023-10-27 21:22:38.000000 py-allspice-2.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2023-10-27 21:22:48.206292 py-allspice-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2023-10-27 21:22:38.000000 py-allspice-2.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:22:48.202292 py-allspice-2.4.0/allspice/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2023-10-27 21:22:38.000000 py-allspice-2.4.0/allspice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16723 2023-10-27 21:22:38.000000 py-allspice-2.4.0/allspice/allspice.py
--rw-r--r--   0 runner    (1001) docker     (127)    59578 2023-10-27 21:22:38.000000 py-allspice-2.4.0/allspice/apiobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     4815 2023-10-27 21:22:38.000000 py-allspice-2.4.0/allspice/baseapiobject.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2023-10-27 21:22:38.000000 py-allspice-2.4.0/allspice/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2023-10-27 21:22:38.000000 py-allspice-2.4.0/allspice/ratelimiter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:22:48.202292 py-allspice-2.4.0/allspice/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 21:22:38.000000 py-allspice-2.4.0/allspice/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12259 2023-10-27 21:22:38.000000 py-allspice-2.4.0/allspice/utils/bom_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2023-10-27 21:22:38.000000 py-allspice-2.4.0/allspice/utils/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2023-10-27 21:22:38.000000 py-allspice-2.4.0/allspice/utils/netlist_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:22:48.202292 py-allspice-2.4.0/py_allspice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2023-10-27 21:22:48.000000 py-allspice-2.4.0/py_allspice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      569 2023-10-27 21:22:48.000000 py-allspice-2.4.0/py_allspice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-27 21:22:48.000000 py-allspice-2.4.0/py_allspice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-10-27 21:22:48.000000 py-allspice-2.4.0/py_allspice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-10-27 21:22:48.000000 py-allspice-2.4.0/py_allspice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      288 2023-10-27 21:22:38.000000 py-allspice-2.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-27 21:22:48.206292 py-allspice-2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      872 2023-10-27 21:22:40.000000 py-allspice-2.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:22:48.206292 py-allspice-2.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    26615 2023-10-27 21:22:38.000000 py-allspice-2.4.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2023-10-27 21:22:38.000000 py-allspice-2.4.0/tests/test_api_longtests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2023-10-27 21:22:38.000000 py-allspice-2.4.0/tests/test_api_ratelimiting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2023-10-27 21:22:38.000000 py-allspice-2.4.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:33:26.335110 py_allspice-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-16 15:33:19.000000 py_allspice-2.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-04-16 15:33:26.335110 py_allspice-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-04-16 15:33:19.000000 py_allspice-2.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:33:26.331110 py_allspice-2.5.0/allspice/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-16 15:33:19.000000 py_allspice-2.5.0/allspice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16521 2024-04-16 15:33:19.000000 py_allspice-2.5.0/allspice/allspice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75142 2024-04-16 15:33:19.000000 py_allspice-2.5.0/allspice/apiobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-04-16 15:33:19.000000 py_allspice-2.5.0/allspice/baseapiobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-16 15:33:19.000000 py_allspice-2.5.0/allspice/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-16 15:33:19.000000 py_allspice-2.5.0/allspice/ratelimiter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:33:26.331110 py_allspice-2.5.0/allspice/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:33:19.000000 py_allspice-2.5.0/allspice/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11888 2024-04-16 15:33:19.000000 py_allspice-2.5.0/allspice/utils/bom_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-16 15:33:19.000000 py_allspice-2.5.0/allspice/utils/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-04-16 15:33:19.000000 py_allspice-2.5.0/allspice/utils/netlist_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:33:26.335110 py_allspice-2.5.0/py_allspice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-04-16 15:33:26.000000 py_allspice-2.5.0/py_allspice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-16 15:33:26.000000 py_allspice-2.5.0/py_allspice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:33:26.000000 py_allspice-2.5.0/py_allspice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-16 15:33:26.000000 py_allspice-2.5.0/py_allspice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 15:33:26.000000 py_allspice-2.5.0/py_allspice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-16 15:33:19.000000 py_allspice-2.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 15:33:26.335110 py_allspice-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-16 15:33:19.000000 py_allspice-2.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:33:26.335110 py_allspice-2.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    32675 2024-04-16 15:33:19.000000 py_allspice-2.5.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-04-16 15:33:19.000000 py_allspice-2.5.0/tests/test_api_longtests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-16 15:33:19.000000 py_allspice-2.5.0/tests/test_api_ratelimiting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-04-16 15:33:19.000000 py_allspice-2.5.0/tests/test_utils.py
```

### Comparing `py-allspice-2.4.0/LICENSE` & `py_allspice-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-allspice-2.4.0/PKG-INFO` & `py_allspice-2.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,24 @@
-Metadata-Version: 2.1
-Name: py-allspice
-Version: 2.4.0
-Summary: A python wrapper for the AllSpice Hub API
-Home-page: https://github.com/AllSpiceIO/py-allspice
-Download-URL: https://github.com/AllSpiceIO/py-allspice
-Author: AllSpice, Inc.
-Author-email: maintainers@allspice.io
-License: MIT
-Keywords: AllSpice,AllSpice Hub,api,wrapper
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: frozendict
-Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
-
 # py-allspice
 
 A very simple API client for AllSpice Hub
 
 Note that not the full Swagger-API is accessible. The whole implementation is focused
 on making access and working with Organizations, Teams, Repositories and Users as pain
 free as possible.
 
 Forked from https://github.com/Langenfeld/py-gitea.
 
 ## Usage
 
 ### Examples
 
-Check the [examples directory](./examples/) for full, working example scripts
-that you can adapt or refer to for your own needs.
+Check the [examples directory](https://github.com/AllSpiceIO/py-allspice/tree/main/examples)
+for full, working example scripts that you can adapt or refer to for your own
+needs.
 
 ### Quickstart
 
 First get an `allspice_client` object wrapping access and authentication (via an api token) for your instance of AllSpice Hub.
 
 ```python
 from allspice import *
@@ -49,15 +33,15 @@
 Operations like requesting the AllSpice version or authentication user can be requested directly from the `allspice_client` object:
 
 ```python
 print("AllSpice Version: " + allspice_client.get_version())
 print("API-Token belongs to user: " + allspice_client.get_user().username)
 ```
 
-Adding entities like Users, Organizations, ...  also is done via the allspice_client object.
+Adding entities like Users, Organizations, ... also is done via the allspice_client object.
 
 ```python
 user = allspice_client.create_user("Test Testson", "test@test.test", "password")
 ```
 
 All operations on entities in allspice are then accomplished via the according wrapper objects for those entities.
 Each of those objects has a `.request` method that creates an entity according to your allspice_client instance.
@@ -65,52 +49,52 @@
 ```python
 other_user = User.request(allspice_client, "OtherUserName")
 print(other_user.username)
 ```
 
 Note that the fields of the User, Organization,... classes are dynamically created at runtime, and thus not visible during divelopment. Refer to the AllSpice API documentation for the fields names.
 
-
 Fields that can not be altered via allspice-api, are read only. After altering a field, the `.commit` method of the according object must be called to synchronize the changed fields with your allspice_client instance.
 
 ```python
 org = Organization.request(allspice_client, test_org)
 org.description = "some new description"
 org.location = "some new location"
 org.commit()
 ```
 
 An entity in allspice can be deleted by calling delete.
+
 ```python
 org.delete()
 ```
 
 All entity objects do have methods to execute some of the requests possible though the AllSpice api:
+
 ```python
 org = Organization.request(allspice_client, ORGNAME)
 teams = org.get_teams()
 for team in teams:
 	repos = team.get_repos()
 	for repo in repos:
 		print(repo.name)
 ```
 
-
 ## Installation
 
-Use ``pip install py-allspice`` to install.
+Use `pip install py-allspice` to install.
 
 ## A Note on Versioning
 
 This repository does not follow the same versioning policy as py-gitea. After v1.17.x,
 py-allspice switched to Semantic Versioning with v2.0.0. In general, versions of
 py-allspice do NOT conform to versions of AllSpice Hub, and the latest version of
 py-allspice should be compatible with the current version of AllSpice Hub.
 
 ## Tests
 
 Tests can be run with:
 
-```python3 -m pytest test_api.py```
+`python3 -m pytest test_api.py`
 
 Make sure to have an instance of AllSpice Hub running on `http://localhost:3000`, and an admin-user token at `.token`.
-The admin user must be named ``test``, with email ``secondarytest@test.org``.
+The admin user must be named `test`, with email `secondarytest@test.org`.
```

### Comparing `py-allspice-2.4.0/README.md` & `py_allspice-2.5.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,41 @@
+Metadata-Version: 2.1
+Name: py-allspice
+Version: 2.5.0
+Summary: A python wrapper for the AllSpice Hub API
+Home-page: https://github.com/AllSpiceIO/py-allspice
+Download-URL: https://github.com/AllSpiceIO/py-allspice
+Author: AllSpice, Inc.
+Author-email: maintainers@allspice.io
+License: MIT
+Keywords: AllSpice,AllSpice Hub,api,wrapper
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: frozendict
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+
 # py-allspice
 
 A very simple API client for AllSpice Hub
 
 Note that not the full Swagger-API is accessible. The whole implementation is focused
 on making access and working with Organizations, Teams, Repositories and Users as pain
 free as possible.
 
 Forked from https://github.com/Langenfeld/py-gitea.
 
 ## Usage
 
 ### Examples
 
-Check the [examples directory](./examples/) for full, working example scripts
-that you can adapt or refer to for your own needs.
+Check the [examples directory](https://github.com/AllSpiceIO/py-allspice/tree/main/examples)
+for full, working example scripts that you can adapt or refer to for your own
+needs.
 
 ### Quickstart
 
 First get an `allspice_client` object wrapping access and authentication (via an api token) for your instance of AllSpice Hub.
 
 ```python
 from allspice import *
@@ -32,15 +50,15 @@
 Operations like requesting the AllSpice version or authentication user can be requested directly from the `allspice_client` object:
 
 ```python
 print("AllSpice Version: " + allspice_client.get_version())
 print("API-Token belongs to user: " + allspice_client.get_user().username)
 ```
 
-Adding entities like Users, Organizations, ...  also is done via the allspice_client object.
+Adding entities like Users, Organizations, ... also is done via the allspice_client object.
 
 ```python
 user = allspice_client.create_user("Test Testson", "test@test.test", "password")
 ```
 
 All operations on entities in allspice are then accomplished via the according wrapper objects for those entities.
 Each of those objects has a `.request` method that creates an entity according to your allspice_client instance.
@@ -48,52 +66,52 @@
 ```python
 other_user = User.request(allspice_client, "OtherUserName")
 print(other_user.username)
 ```
 
 Note that the fields of the User, Organization,... classes are dynamically created at runtime, and thus not visible during divelopment. Refer to the AllSpice API documentation for the fields names.
 
-
 Fields that can not be altered via allspice-api, are read only. After altering a field, the `.commit` method of the according object must be called to synchronize the changed fields with your allspice_client instance.
 
 ```python
 org = Organization.request(allspice_client, test_org)
 org.description = "some new description"
 org.location = "some new location"
 org.commit()
 ```
 
 An entity in allspice can be deleted by calling delete.
+
 ```python
 org.delete()
 ```
 
 All entity objects do have methods to execute some of the requests possible though the AllSpice api:
+
 ```python
 org = Organization.request(allspice_client, ORGNAME)
 teams = org.get_teams()
 for team in teams:
 	repos = team.get_repos()
 	for repo in repos:
 		print(repo.name)
 ```
 
-
 ## Installation
 
-Use ``pip install py-allspice`` to install.
+Use `pip install py-allspice` to install.
 
 ## A Note on Versioning
 
 This repository does not follow the same versioning policy as py-gitea. After v1.17.x,
 py-allspice switched to Semantic Versioning with v2.0.0. In general, versions of
 py-allspice do NOT conform to versions of AllSpice Hub, and the latest version of
 py-allspice should be compatible with the current version of AllSpice Hub.
 
 ## Tests
 
 Tests can be run with:
 
-```python3 -m pytest test_api.py```
+`python3 -m pytest test_api.py`
 
 Make sure to have an instance of AllSpice Hub running on `http://localhost:3000`, and an admin-user token at `.token`.
-The admin user must be named ``test``, with email ``secondarytest@test.org``.
+The admin user must be named `test`, with email `secondarytest@test.org`.
```

### Comparing `py-allspice-2.4.0/allspice/allspice.py` & `py_allspice-2.5.0/allspice/allspice.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,20 @@
 from typing import List, Dict, Union, Optional
 
 from frozendict import frozendict
 import requests
 import urllib3
 
 from .apiobject import User, Organization, Repository, Team
-from .exceptions import NotFoundException, ConflictException, AlreadyExistsException, NotYetGeneratedException
+from .exceptions import (
+    NotFoundException,
+    ConflictException,
+    AlreadyExistsException,
+    NotYetGeneratedException,
+)
 from .ratelimiter import RateLimitedSession
 
 
 class AllSpice:
     """Object to establish a session with AllSpice Hub."""
 
     ADMIN_CREATE_USER = """/admin/users"""
@@ -69,15 +74,16 @@
         # Manage authentification
         if not token_text and not auth:
             raise ValueError("Please provide auth or token_text, but not both")
         if token_text:
             self.headers["Authorization"] = "token " + token_text
         if auth:
             self.logger.warning(
-                "Using basic auth is not recommended. Prefer using a token instead.")
+                "Using basic auth is not recommended. Prefer using a token instead."
+            )
             self.requests.auth = auth
 
         # Manage SSL certification verification
         self.requests.verify = verify
         if not verify:
             urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
@@ -90,25 +96,26 @@
         request = self.requests.get(self.__get_url(endpoint), headers=self.headers, params=params)
         if request.status_code not in [200, 201]:
             message = f"Received status code: {request.status_code} ({request.url})"
             if request.status_code in [404]:
                 raise NotFoundException(message)
             if request.status_code in [403]:
                 raise Exception(
-                    f"Unauthorized: {request.url} - Check your permissions and try again! ({message})")
+                    f"Unauthorized: {request.url} - Check your permissions and try again! ({message})"
+                )
             if request.status_code in [409]:
                 raise ConflictException(message)
             if request.status_code in [503]:
                 raise NotYetGeneratedException(message)
             raise Exception(message)
         return request
 
     @staticmethod
     def parse_result(result) -> Dict:
-        """ Parses the result-JSON to a dict. """
+        """Parses the result-JSON to a dict."""
         if result.text and len(result.text) > 3:
             return json.loads(result.text)
         return {}
 
     def requests_get(self, endpoint: str, params=frozendict(), sudo=None):
         combined_params = {}
         combined_params.update(params)
@@ -156,35 +163,37 @@
                 aggregated_result.extend(result)
 
             page += 1
 
     def requests_put(self, endpoint: str, data: Optional[dict] = None):
         if not data:
             data = {}
-        request = self.requests.put(self.__get_url(
-            endpoint), headers=self.headers, data=json.dumps(data))
+        request = self.requests.put(
+            self.__get_url(endpoint), headers=self.headers, data=json.dumps(data)
+        )
         if request.status_code not in [200, 204]:
             message = f"Received status code: {request.status_code} ({request.url}) {request.text}"
             self.logger.error(message)
             raise Exception(message)
 
     def requests_delete(self, endpoint: str, data: Optional[dict] = None):
-        request = self.requests.delete(self.__get_url(
-            endpoint), headers=self.headers, data=json.dumps(data))
+        request = self.requests.delete(
+            self.__get_url(endpoint), headers=self.headers, data=json.dumps(data)
+        )
         if request.status_code not in [200, 204]:
             message = f"Received status code: {request.status_code} ({request.url})"
             self.logger.error(message)
             raise Exception(message)
 
     def requests_post(
-            self,
-            endpoint: str,
-            data: Optional[dict] = None,
-            params: Optional[dict] = None,
-            files: Optional[dict] = None,
+        self,
+        endpoint: str,
+        data: Optional[dict] = None,
+        params: Optional[dict] = None,
+        files: Optional[dict] = None,
     ):
         """
         Make a POST call to the endpoint.
 
         :param endpoint: The path to the endpoint
         :param data: A dictionary for JSON data
         :param params: A dictionary of query params
@@ -203,27 +212,29 @@
         if files is not None:
             args["headers"].pop("Content-type")
             args["files"] = files
 
         request = self.requests.post(self.__get_url(endpoint), **args)
 
         if request.status_code not in [200, 201, 202]:
-            if ("already exists" in request.text or "e-mail already in use" in request.text):
+            if "already exists" in request.text or "e-mail already in use" in request.text:
                 self.logger.warning(request.text)
                 raise AlreadyExistsException()
             self.logger.error(f"Received status code: {request.status_code} ({request.url})")
             self.logger.error(f"With info: {data} ({self.headers})")
             self.logger.error(f"Answer: {request.text}")
             raise Exception(
-                f"Received status code: {request.status_code} ({request.url}), {request.text}")
+                f"Received status code: {request.status_code} ({request.url}), {request.text}"
+            )
         return self.parse_result(request)
 
     def requests_patch(self, endpoint: str, data: dict):
-        request = self.requests.patch(self.__get_url(
-            endpoint), headers=self.headers, data=json.dumps(data))
+        request = self.requests.patch(
+            self.__get_url(endpoint), headers=self.headers, data=json.dumps(data)
+        )
         if request.status_code not in [200, 201]:
             error_message = f"Received status code: {request.status_code} ({request.url}) {data}"
             self.logger.error(error_message)
             raise Exception(error_message)
         return self.parse_result(request)
 
     def get_orgs_public_members_all(self, orgname):
@@ -263,25 +274,25 @@
 
     def get_repository(self, owner: str, name: str) -> Repository:
         path = self.GET_REPOSITORY.format(owner=owner, name=name)
         result = self.requests_get(path)
         return Repository.parse_response(self, result)
 
     def create_user(
-            self,
-            user_name: str,
-            email: str,
-            password: str,
-            full_name: Optional[str] = None,
-            login_name: Optional[str] = None,
-            change_pw=True,
-            send_notify=True,
-            source_id=0,
+        self,
+        user_name: str,
+        email: str,
+        password: str,
+        full_name: Optional[str] = None,
+        login_name: Optional[str] = None,
+        change_pw=True,
+        send_notify=True,
+        source_id=0,
     ):
-        """ Create User.
+        """Create User.
         Throws:
             AlreadyExistsException, if the User exists already
             Exception, if something else went wrong.
         """
         if not login_name:
             login_name = user_name
         if not full_name:
@@ -310,27 +321,27 @@
         else:
             self.logger.error(result["message"])
             raise Exception("User not created... (gitea: %s)" % result["message"])
         user = User.parse_response(self, result)
         return user
 
     def create_repo(
-            self,
-            repoOwner: Union[User, Organization],
-            repoName: str,
-            description: str = "",
-            private: bool = False,
-            autoInit=True,
-            gitignores: Optional[str] = None,
-            license: Optional[str] = None,
-            readme: str = "Default",
-            issue_labels: Optional[str] = None,
-            default_branch="master",
+        self,
+        repoOwner: Union[User, Organization],
+        repoName: str,
+        description: str = "",
+        private: bool = False,
+        autoInit=True,
+        gitignores: Optional[str] = None,
+        license: Optional[str] = None,
+        readme: str = "Default",
+        issue_labels: Optional[str] = None,
+        default_branch="master",
     ):
-        """ Create a Repository as the administrator
+        """Create a Repository as the administrator
 
         Throws:
             AlreadyExistsException: If the Repository exists already.
             Exception: If something else went wrong.
 
         Note:
             Non-admin users can not use this method. Please use instead
@@ -357,67 +368,61 @@
             self.logger.info("Successfully created Repository %s " % result["name"])
         else:
             self.logger.error(result["message"])
             raise Exception("Repository not created... (gitea: %s)" % result["message"])
         return Repository.parse_response(self, result)
 
     def create_org(
-            self,
-            owner: User,
-            orgName: str,
-            description: str,
-            location="",
-            website="",
-            full_name="",
+        self,
+        owner: User,
+        orgName: str,
+        description: str,
+        location="",
+        website="",
+        full_name="",
     ):
         assert isinstance(owner, User)
         result = self.requests_post(
             AllSpice.CREATE_ORG % owner.username,
             data={
                 "username": orgName,
                 "description": description,
                 "location": location,
                 "website": website,
                 "full_name": full_name,
             },
         )
         if "id" in result:
-            self.logger.info(
-                "Successfully created Organization %s" % result["username"]
-            )
+            self.logger.info("Successfully created Organization %s" % result["username"])
         else:
-            self.logger.error(
-                "Organization not created... (gitea: %s)" % result["message"]
-            )
+            self.logger.error("Organization not created... (gitea: %s)" % result["message"])
             self.logger.error(result["message"])
-            raise Exception(
-                "Organization not created... (gitea: %s)" % result["message"]
-            )
+            raise Exception("Organization not created... (gitea: %s)" % result["message"])
         return Organization.parse_response(self, result)
 
     def create_team(
-            self,
-            org: Organization,
-            name: str,
-            description: str = "",
-            permission: str = "read",
-            can_create_org_repo: bool = False,
-            includes_all_repositories: bool = False,
-            units=(
-                "repo.code",
-                "repo.issues",
-                "repo.ext_issues",
-                "repo.wiki",
-                "repo.pulls",
-                "repo.releases",
-                "repo.ext_wiki",
-            ),
-            units_map={},
+        self,
+        org: Organization,
+        name: str,
+        description: str = "",
+        permission: str = "read",
+        can_create_org_repo: bool = False,
+        includes_all_repositories: bool = False,
+        units=(
+            "repo.code",
+            "repo.issues",
+            "repo.ext_issues",
+            "repo.wiki",
+            "repo.pulls",
+            "repo.releases",
+            "repo.ext_wiki",
+        ),
+        units_map={},
     ):
-        """ Creates a Team.
+        """Creates a Team.
 
         Args:
             org (Organization): Organization the Team will be part of.
             name (str): The Name of the Team to be created.
             description (str): Optional, None, short description of the new Team.
             permission (str): Optional, 'read', What permissions the members
             units_map (dict): Optional, {}, a mapping of units to their
```

### Comparing `py-allspice-2.4.0/allspice/apiobject.py` & `py_allspice-2.5.0/allspice/apiobject.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,24 @@
 from __future__ import annotations
 
 import logging
 from functools import cached_property
-from typing import ClassVar, List, Tuple, Dict, Sequence, Optional, Union, Set, IO, Literal
+import re
+from typing import (
+    ClassVar,
+    List,
+    Tuple,
+    Dict,
+    Sequence,
+    Optional,
+    Union,
+    Set,
+    IO,
+    Literal,
+)
 from datetime import datetime, timezone
 from enum import Enum
 
 from .baseapiobject import ReadonlyApiObject, ApiObject
 from .exceptions import NotFoundException, ConflictException
 
 
@@ -29,19 +41,19 @@
             return False
         return self.allspice_client == other.allspice_client and self.name == other.name
 
     def __hash__(self):
         return hash(self.allspice_client) ^ hash(self.name)
 
     @classmethod
-    def request(cls, allspice_client, name: str) -> 'Organization':
+    def request(cls, allspice_client, name: str) -> "Organization":
         return cls._request(allspice_client, {"name": name})
 
     @classmethod
-    def parse_response(cls, allspice_client, result) -> 'Organization':
+    def parse_response(cls, allspice_client, result) -> "Organization":
         api_object = super().parse_response(allspice_client, result)
         # add "name" field to make this behave similar to users for gitea < 1.18
         # also necessary for repository-owner when org is repo owner
         if not hasattr(api_object, "name"):
             Organization._add_read_property("name", result["username"], api_object)
         return api_object
 
@@ -54,24 +66,24 @@
     }
 
     def commit(self):
         args = {"name": self.name}
         self._commit(args)
 
     def create_repo(
-            self,
-            repoName: str,
-            description: str = "",
-            private: bool = False,
-            autoInit=True,
-            gitignores: Optional[str] = None,
-            license: Optional[str] = None,
-            readme: str = "Default",
-            issue_labels: Optional[str] = None,
-            default_branch="master",
+        self,
+        repoName: str,
+        description: str = "",
+        private: bool = False,
+        autoInit=True,
+        gitignores: Optional[str] = None,
+        license: Optional[str] = None,
+        readme: str = "Default",
+        issue_labels: Optional[str] = None,
+        default_branch="master",
     ):
         """Create an organization Repository
 
         Throws:
             AlreadyExistsException: If the Repository exists already.
             Exception: If something else went wrong.
         """
@@ -106,47 +118,45 @@
         repos = self.get_repositories()
         for repo in repos:
             if repo.name == name:
                 return repo
         raise NotFoundException("Repository %s not existent in organization." % name)
 
     def get_teams(self) -> List["Team"]:
-        results = self.allspice_client.requests_get(
-            Organization.ORG_TEAMS_REQUEST % self.username
-        )
+        results = self.allspice_client.requests_get(Organization.ORG_TEAMS_REQUEST % self.username)
         teams = [Team.parse_response(self.allspice_client, result) for result in results]
         # organisation seems to be missing using this request, so we add org manually
         for t in teams:
             setattr(t, "_organization", self)
         return teams
 
     def get_team(self, name) -> "Team":
         teams = self.get_teams()
         for team in teams:
             if team.name == name:
                 return team
         raise NotFoundException("Team not existent in organization.")
 
     def create_team(
-            self,
-            name: str,
-            description: str = "",
-            permission: str = "read",
-            can_create_org_repo: bool = False,
-            includes_all_repositories: bool = False,
-            units=(
-                "repo.code",
-                "repo.issues",
-                "repo.ext_issues",
-                "repo.wiki",
-                "repo.pulls",
-                "repo.releases",
-                "repo.ext_wiki",
-            ),
-            units_map={},
+        self,
+        name: str,
+        description: str = "",
+        permission: str = "read",
+        can_create_org_repo: bool = False,
+        includes_all_repositories: bool = False,
+        units=(
+            "repo.code",
+            "repo.issues",
+            "repo.ext_issues",
+            "repo.wiki",
+            "repo.pulls",
+            "repo.releases",
+            "repo.ext_wiki",
+        ),
+        units_map={},
     ) -> "Team":
         """Alias for AllSpice#create_team"""
         # TODO: Move AllSpice#create_team to Organization#create_team and
         #       deprecate AllSpice#create_team.
         return self.allspice_client.create_team(
             org=self,
             name=name,
@@ -175,15 +185,15 @@
             return False
 
     def remove_member(self, user: "User"):
         path = f"/orgs/{self.username}/members/{user.username}"
         self.allspice_client.requests_delete(path)
 
     def delete(self):
-        """ Delete this Organization. Invalidates this Objects data. Also deletes all Repositories owned by the User"""
+        """Delete this Organization. Invalidates this Objects data. Also deletes all Repositories owned by the User"""
         for repo in self.get_repositories():
             repo.delete()
         self.allspice_client.requests_delete(Organization.API_OBJECT.format(name=self.username))
         self.deleted = True
 
     def get_heatmap(self) -> List[Tuple[datetime, int]]:
         results = self.allspice_client.requests_get(User.USER_HEATMAP % self.username)
@@ -254,24 +264,24 @@
             {"login_name": login_name, "source_id": source_id}
         )
         args = {"username": self.username}
         self.allspice_client.requests_patch(User.ADMIN_EDIT_USER.format(**args), data=values)
         self._dirty_fields = {}
 
     def create_repo(
-            self,
-            repoName: str,
-            description: str = "",
-            private: bool = False,
-            autoInit=True,
-            gitignores: Optional[str] = None,
-            license: Optional[str] = None,
-            readme: str = "Default",
-            issue_labels: Optional[str] = None,
-            default_branch="master",
+        self,
+        repoName: str,
+        description: str = "",
+        private: bool = False,
+        autoInit=True,
+        gitignores: Optional[str] = None,
+        license: Optional[str] = None,
+        readme: str = "Default",
+        issue_labels: Optional[str] = None,
+        default_branch="master",
     ):
         """Create a user Repository
 
         Throws:
             AlreadyExistsException: If the Repository exists already.
             Exception: If something else went wrong.
         """
@@ -293,45 +303,45 @@
             self.allspice_client.logger.info("Successfully created Repository %s " % result["name"])
         else:
             self.allspice_client.logger.error(result["message"])
             raise Exception("Repository not created... (gitea: %s)" % result["message"])
         return Repository.parse_response(self, result)
 
     def get_repositories(self) -> List["Repository"]:
-        """ Get all Repositories owned by this User."""
+        """Get all Repositories owned by this User."""
         url = f"/users/{self.username}/repos"
         results = self.allspice_client.requests_get_paginated(url)
         return [Repository.parse_response(self.allspice_client, result) for result in results]
 
     def get_orgs(self) -> List[Organization]:
-        """ Get all Organizations this user is a member of."""
+        """Get all Organizations this user is a member of."""
         url = f"/users/{self.username}/orgs"
         results = self.allspice_client.requests_get_paginated(url)
         return [Organization.parse_response(self.allspice_client, result) for result in results]
 
-    def get_teams(self) -> List['Team']:
+    def get_teams(self) -> List["Team"]:
         url = "/user/teams"
         results = self.allspice_client.requests_get_paginated(url, sudo=self)
         return [Team.parse_response(self.allspice_client, result) for result in results]
 
-    def get_accessible_repos(self) -> List['Repository']:
-        """ Get all Repositories accessible by the logged in User."""
+    def get_accessible_repos(self) -> List["Repository"]:
+        """Get all Repositories accessible by the logged in User."""
         results = self.allspice_client.requests_get("/user/repos", sudo=self)
         return [Repository.parse_response(self, result) for result in results]
 
     def __request_emails(self):
         result = self.allspice_client.requests_get(User.USER_MAIL % self.login)
         # report if the adress changed by this
         for mail in result:
             self._emails.append(mail["email"])
             if mail["primary"]:
                 self._email = mail["email"]
 
     def delete(self):
-        """ Deletes this User. Also deletes all Repositories he owns."""
+        """Deletes this User. Also deletes all Repositories he owns."""
         self.allspice_client.requests_delete(User.ADMIN_DELETE_USER % self.username)
         self.deleted = True
 
     def get_heatmap(self) -> List[Tuple[datetime, int]]:
         results = self.allspice_client.requests_get(User.USER_HEATMAP % self.username)
         results = [
             (datetime.fromtimestamp(result["timestamp"]), result["contributions"])
@@ -379,47 +389,65 @@
     REPO_TRANSFER = "/repos/{owner}/{repo}/transfer"
     REPO_MILESTONES = """/repos/{owner}/{repo}/milestones"""
     REPO_GET_ARCHIVE = "/repos/{owner}/{repo}/archive/{ref}.{format}"
     REPO_GET_ALLSPICE_JSON = "/repos/{owner}/{repo}/allspice_generated/json/{content}"
     REPO_GET_ALLSPICE_SVG = "/repos/{owner}/{repo}/allspice_generated/svg/{content}"
     REPO_GET_TOPICS = "/repos/{owner}/{repo}/topics"
     REPO_ADD_TOPIC = "/repos/{owner}/{repo}/topics/{topic}"
+    REPO_GET_RELEASES = "/repos/{owner}/{repo}/releases"
+    REPO_GET_LATEST_RELEASE = "/repos/{owner}/{repo}/releases/latest"
+    REPO_GET_RELEASE_BY_TAG = "/repos/{owner}/{repo}/releases/tags/{tag}"
+    REPO_GET_COMMIT_STATUS = "/repos/{owner}/{repo}/statuses/{sha}"
 
     class ArchiveFormat(Enum):
         """
         Archive formats for Repository.get_archive
         """
 
         TAR = "tar.gz"
         ZIP = "zip"
 
+    class CommitStatusSort(Enum):
+        """
+        Sort order for Repository.get_commit_status
+        """
+
+        OLDEST = "oldest"
+        RECENT_UPDATE = "recentupdate"
+        LEAST_UPDATE = "leastupdate"
+        LEAST_INDEX = "leastindex"
+        HIGHEST_INDEX = "highestindex"
+
     def __init__(self, allspice_client):
         super().__init__(allspice_client)
 
     def __eq__(self, other):
         if not isinstance(other, Repository):
             return False
         return self.owner == other.owner and self.name == other.name
 
     def __hash__(self):
         return hash(self.owner) ^ hash(self.name)
 
     _fields_to_parsers: ClassVar[dict] = {
         # dont know how to tell apart user and org as owner except form email being empty.
-        "owner": lambda allspice_client, r: Organization.parse_response(allspice_client, r)
-        if r["email"] == "" else User.parse_response(allspice_client, r),
+        "owner": lambda allspice_client, r: (
+            Organization.parse_response(allspice_client, r)
+            if r["email"] == ""
+            else User.parse_response(allspice_client, r)
+        ),
         "updated_at": lambda allspice_client, t: Util.convert_time(t),
     }
 
     @classmethod
     def request(
-            cls,
-            allspice_client,
-            owner: str,
-            name: str,
+        cls,
+        allspice_client,
+        owner: str,
+        name: str,
     ) -> Repository:
         return cls._request(allspice_client, {"owner": owner, "name": name})
 
     @classmethod
     def search(
         cls,
         allspice_client,
@@ -458,16 +486,15 @@
         if user is not None:
             params["user"] = user.id
         if owner_to_prioritize is not None:
             params["owner_to_prioritize"] = owner_to_prioritize.id
 
         responses = allspice_client.requests_get_paginated(cls.REPO_SEARCH, params=params)
 
-        return [Repository.parse_response(allspice_client, response)
-                for response in responses]
+        return [Repository.parse_response(allspice_client, response) for response in responses]
 
     _patchable_fields: ClassVar[set[str]] = {
         "allow_manual_merge",
         "allow_merge_commits",
         "allow_rebase",
         "allow_rebase_explicit",
         "allow_rebase_update",
@@ -494,47 +521,53 @@
         "website",
     }
 
     def commit(self):
         args = {"owner": self.owner.username, "name": self.name}
         self._commit(args)
 
-    def get_branches(self) -> List['Branch']:
+    def get_branches(self) -> List["Branch"]:
         """Get all the Branches of this Repository."""
 
         results = self.allspice_client.requests_get_paginated(
             Repository.REPO_BRANCHES % (self.owner.username, self.name)
         )
         return [Branch.parse_response(self.allspice_client, result) for result in results]
 
-    def get_branch(self, name: str) -> 'Branch':
+    def get_branch(self, name: str) -> "Branch":
         """Get a specific Branch of this Repository."""
         result = self.allspice_client.requests_get(
             Repository.REPO_BRANCH.format(owner=self.owner.username, repo=self.name, branch=name)
         )
         return Branch.parse_response(self.allspice_client, result)
 
-    def add_branch(self, create_from: Branch, newname: str) -> "Branch":
+    def add_branch(self, create_from: Ref, newname: str) -> "Branch":
         """Add a branch to the repository"""
         # Note: will only work with gitea 1.13 or higher!
-        data = {"new_branch_name": newname, "old_branch_name": create_from.name}
+
+        ref_name = Util.data_params_for_ref(create_from)
+        if "ref" not in ref_name:
+            raise ValueError("create_from must be a Branch, Commit or string")
+        ref_name = ref_name["ref"]
+
+        data = {"new_branch_name": newname, "old_ref_name": ref_name}
         result = self.allspice_client.requests_post(
             Repository.REPO_BRANCHES % (self.owner.username, self.name), data=data
         )
         return Branch.parse_response(self.allspice_client, result)
 
     def get_issues(
-            self,
-            state: Union[Literal["open"], Literal["closed"], Literal["all"]] = "all",
-            search_query: Optional[str] = None,
-            labels: Optional[List[str]] = None,
-            milestones: Optional[List[Union[Milestone, str]]] = None,
-            assignee: Optional[Union[User, str]] = None,
-            since: Optional[datetime] = None,
-            before: Optional[datetime] = None,
+        self,
+        state: Union[Literal["open"], Literal["closed"], Literal["all"]] = "all",
+        search_query: Optional[str] = None,
+        labels: Optional[List[str]] = None,
+        milestones: Optional[List[Union[Milestone, str]]] = None,
+        assignee: Optional[Union[User, str]] = None,
+        since: Optional[datetime] = None,
+        before: Optional[datetime] = None,
     ) -> List["Issue"]:
         """
         Get all Issues of this Repository (open and closed)
 
         https://hub.allspice.io/api/swagger#/repository/repoListIssues
 
         All params of this method are optional filters. If you don't specify a filter, it
@@ -556,16 +589,18 @@
         }
         if search_query:
             data["q"] = search_query
         if labels:
             data["labels"] = ",".join(labels)
         if milestones:
             data["milestone"] = ",".join(
-                [milestone.name if isinstance(milestone, Milestone) else milestone for
-                 milestone in milestones]
+                [
+                    milestone.name if isinstance(milestone, Milestone) else milestone
+                    for milestone in milestones
+                ]
             )
         if assignee:
             if isinstance(assignee, User):
                 data["assignee"] = assignee.username
             else:
                 data["assignee"] = assignee
         if since:
@@ -586,18 +621,18 @@
             Issue._add_read_property("repo", self, issue)
             Issue._add_read_property("owner", self.owner, issue)
             issues.append(issue)
 
         return issues
 
     def get_design_reviews(
-            self,
-            state: Union[Literal["open"], Literal["closed"], Literal["all"]] = "all",
-            milestone: Optional[Union[Milestone, str]] = None,
-            labels: Optional[List[str]] = None,
+        self,
+        state: Union[Literal["open"], Literal["closed"], Literal["all"]] = "all",
+        milestone: Optional[Union[Milestone, str]] = None,
+        labels: Optional[List[str]] = None,
     ) -> List["DesignReview"]:
         """
         Get all Design Reviews of this Repository.
 
         https://hub.allspice.io/api/swagger#/repository/repoListPullRequests
 
         :param state: The state of the Design Reviews to get. If None, all Design Reviews
@@ -615,26 +650,24 @@
                 params["milestone"] = milestone.name
             else:
                 params["milestone"] = milestone
         if labels:
             params["labels"] = ",".join(labels)
 
         results = self.allspice_client.requests_get_paginated(
-            self.REPO_DESIGN_REVIEWS.format(owner=self.owner.username,
-                                            repo=self.name),
+            self.REPO_DESIGN_REVIEWS.format(owner=self.owner.username, repo=self.name),
             params=params,
         )
-        return [DesignReview.parse_response(self.allspice_client, result)
-                for result in results]
+        return [DesignReview.parse_response(self.allspice_client, result) for result in results]
 
     def get_commits(
-            self,
-            sha: Optional[str] = None,
-            path: Optional[str] = None,
-            stat: bool = True,
+        self,
+        sha: Optional[str] = None,
+        path: Optional[str] = None,
+        stat: bool = True,
     ) -> List["Commit"]:
         """
         Get all the Commits of this Repository.
 
         https://hub.allspice.io/api/swagger#/repository/repoGetAllCommits
 
         :param sha: The SHA of the commit to start listing commits from.
@@ -655,32 +688,31 @@
         try:
             results = self.allspice_client.requests_get_paginated(
                 Repository.REPO_COMMITS % (self.owner.username, self.name),
                 params=data,
             )
         except ConflictException as err:
             logging.warning(err)
-            logging.warning(
-                "Repository %s/%s is Empty" % (self.owner.username, self.name)
-            )
+            logging.warning("Repository %s/%s is Empty" % (self.owner.username, self.name))
             results = []
         return [Commit.parse_response(self.allspice_client, result) for result in results]
 
     def get_issues_state(self, state) -> List["Issue"]:
         """
         DEPRECATED: Use get_issues() instead.
 
         Get issues of state Issue.open or Issue.closed of a repository.
         """
 
         assert state in [Issue.OPENED, Issue.CLOSED]
         issues = []
         data = {"state": state}
         results = self.allspice_client.requests_get_paginated(
-            Repository.REPO_ISSUES.format(owner=self.owner.username, repo=self.name), params=data
+            Repository.REPO_ISSUES.format(owner=self.owner.username, repo=self.name),
+            params=data,
         )
         for result in results:
             issue = Issue.parse_response(self.allspice_client, result)
             # adding data not contained in the issue answer
             Issue._add_read_property("repo", self, issue)
             Issue._add_read_property("owner", self.owner, issue)
             issues.append(issue)
@@ -708,28 +740,29 @@
         data = {
             "assignees": assignees,
             "body": description,
             "closed": False,
             "title": title,
         }
         result = self.allspice_client.requests_post(
-            Repository.REPO_ISSUES.format(owner=self.owner.username, repo=self.name), data=data
+            Repository.REPO_ISSUES.format(owner=self.owner.username, repo=self.name),
+            data=data,
         )
         return Issue.parse_response(self.allspice_client, result)
 
     def create_design_review(
-            self,
-            title: str,
-            head: Union[Branch, str],
-            base: Union[Branch, str],
-            assignees: Optional[Set[Union[User, str]]] = None,
-            body: Optional[str] = None,
-            due_date: Optional[datetime] = None,
-            milestone: Optional['Milestone'] = None,
-    ) -> 'DesignReview':
+        self,
+        title: str,
+        head: Union[Branch, str],
+        base: Union[Branch, str],
+        assignees: Optional[Set[Union[User, str]]] = None,
+        body: Optional[str] = None,
+        due_date: Optional[datetime] = None,
+        milestone: Optional["Milestone"] = None,
+    ) -> "DesignReview":
         """
         Create a new Design Review.
 
         See https://hub.allspice.io/api/swagger#/repository/repoCreatePullRequest
 
         :param title: Title of the Design Review
         :param head: Branch or name of the branch to merge into the base branch
@@ -751,31 +784,36 @@
         else:
             data["head"] = head
         if isinstance(base, Branch):
             data["base"] = base.name
         else:
             data["base"] = base
         if assignees:
-            data["assignees"] = [a.username if isinstance(a, User) else a for a in
-                                 assignees]
+            data["assignees"] = [a.username if isinstance(a, User) else a for a in assignees]
         if body:
             data["body"] = body
         if due_date:
             data["due_date"] = Util.format_time(due_date)
         if milestone:
             data["milestone"] = milestone.id
 
         result = self.allspice_client.requests_post(
             self.REPO_DESIGN_REVIEWS.format(owner=self.owner.username, repo=self.name),
-            data=data
+            data=data,
         )
 
         return DesignReview.parse_response(self.allspice_client, result)
 
-    def create_milestone(self, title: str, description: str, due_date: Optional[str] = None, state: str = "open") -> "Milestone":
+    def create_milestone(
+        self,
+        title: str,
+        description: str,
+        due_date: Optional[str] = None,
+        state: str = "open",
+    ) -> "Milestone":
         url = Repository.REPO_MILESTONES.format(owner=self.owner.username, repo=self.name)
         data = {"title": title, "description": description, "state": state}
         if due_date:
             data["due_date"] = due_date
         result = self.allspice_client.requests_post(url, data=data)
         return Milestone.parse_response(self.allspice_client, result)
 
@@ -799,16 +837,15 @@
 
     def is_collaborator(self, username) -> bool:
         if isinstance(username, User):
             username = username.username
         try:
             # returns 204 if its ok, 404 if its not
             self.allspice_client.requests_get(
-                Repository.REPO_IS_COLLABORATOR
-                % (self.owner.username, self.name, username)
+                Repository.REPO_IS_COLLABORATOR % (self.owner.username, self.name, username)
             )
             return True
         except Exception:
             return False
 
     def get_users_with_access(self) -> Sequence[User]:
         url = f"/repos/{self.owner.username}/{self.name}/collaborators"
@@ -825,63 +862,92 @@
                     collabs += team.get_members()
             return collabs
 
     def remove_collaborator(self, user_name: str):
         url = f"/repos/{self.owner.username}/{self.name}/collaborators/{user_name}"
         self.allspice_client.requests_delete(url)
 
-    def transfer_ownership(self, new_owner: Union["User", "Organization"], new_teams: Set["Team"] = frozenset()):
+    def transfer_ownership(
+        self,
+        new_owner: Union["User", "Organization"],
+        new_teams: Set["Team"] = frozenset(),
+    ):
         url = Repository.REPO_TRANSFER.format(owner=self.owner.username, repo=self.name)
         data = {"new_owner": new_owner.username}
         if isinstance(new_owner, Organization):
             new_team_ids = [team.id for team in new_teams if team in new_owner.get_teams()]
             data["team_ids"] = new_team_ids
         self.allspice_client.requests_post(url, data=data)
         # TODO: make sure this instance is either updated or discarded
 
     def get_git_content(
-            self: Optional[str] = None,
-            ref: Optional["Ref"] = None,
-            commit: "Optional[Commit]" = None
+        self: Optional[str] = None,
+        ref: Optional["Ref"] = None,
+        commit: "Optional[Commit]" = None,
     ) -> List["Content"]:
         """
         Get a list of all files in the repository.
 
         https://hub.allspice.io/api/swagger#/repository/repoGetContentsList
 
         :param ref: branch or commit to get content from
         :param commit: commit to get content from (deprecated)
         """
         url = f"/repos/{self.owner.username}/{self.name}/contents"
         data = Util.data_params_for_ref(ref or commit)
 
-        result = [Content.parse_response(self.allspice_client, f)
-                  for f in self.allspice_client.requests_get(url, data)]
+        result = [
+            Content.parse_response(self.allspice_client, f)
+            for f in self.allspice_client.requests_get(url, data)
+        ]
         return result
 
     def get_file_content(
-            self,
-            content: Content,
-            ref: Optional[Ref] = None,
-            commit: Optional[Commit] = None,
+        self,
+        content: Content,
+        ref: Optional[Ref] = None,
+        commit: Optional[Commit] = None,
     ) -> Union[str, List["Content"]]:
         """https://hub.allspice.io/api/swagger#/repository/repoGetContents"""
         url = f"/repos/{self.owner.username}/{self.name}/contents/{content.path}"
         data = Util.data_params_for_ref(ref or commit)
 
         if content.type == Content.FILE:
             return self.allspice_client.requests_get(url, data)["content"]
         else:
-            return [Content.parse_response(self.allspice_client, f) for f in self.allspice_client.requests_get(url, data)]
+            return [
+                Content.parse_response(self.allspice_client, f)
+                for f in self.allspice_client.requests_get(url, data)
+            ]
+
+    def get_raw_file(
+        self,
+        file_path: str,
+        ref: Optional[Ref] = None,
+    ) -> bytes:
+        """
+        Get the raw, binary data of a single file.
+
+        Note: if the file you are requesting is a text file, you might want to
+        use .decode() on the result to get a string. For example:
+
+            content = repo.get_raw_file("file.txt").decode("utf-8")
 
-    def get_generated_json(
-            self,
-            content: Union[Content, str],
-            ref: Optional[Ref] = None
-    ) -> dict:
+        See https://hub.allspice.io/api/swagger#/repository/repoGetRawFile
+
+        :param file_path: The path to the file to get.
+        :param ref: The branch or commit to get the file from.  If not provided,
+            the default branch is used.
+        """
+
+        url = f"/repos/{self.owner.username}/{self.name}/raw/{file_path}"
+        params = Util.data_params_for_ref(ref)
+        return self.allspice_client.requests_get_raw(url, params=params)
+
+    def get_generated_json(self, content: Union[Content, str], ref: Optional[Ref] = None) -> dict:
         """
         Get the json blob for a cad file if it exists, otherwise enqueue
         a new job and return a 503 status.
 
         WARNING: This is still experimental and not recommended for critical
         applications. The structure and content of the returned dictionary can
         change at any time.
@@ -896,19 +962,15 @@
             owner=self.owner.username,
             repo=self.name,
             content=content,
         )
         data = Util.data_params_for_ref(ref)
         return self.allspice_client.requests_get(url, data)
 
-    def get_generated_svg(
-            self,
-            content: Union[Content, str],
-            ref: Optional[Ref] = None
-    ) -> bytes:
+    def get_generated_svg(self, content: Union[Content, str], ref: Optional[Ref] = None) -> bytes:
         """
         Get the svg blob for a cad file if it exists, otherwise enqueue
         a new job and return a 503 status.
 
         WARNING: This is still experimental and not yet recommended for
         critical applications. The content of the returned svg can change
         at any time.
@@ -948,17 +1010,17 @@
         if not data:
             data = {}
         url = f"/repos/{self.owner.username}/{self.name}/contents/{file_path}"
         data.update({"sha": file_sha})
         return self.allspice_client.requests_delete(url, data)
 
     def get_archive(
-            self,
-            ref: Ref = "main",
-            archive_format: ArchiveFormat = ArchiveFormat.ZIP,
+        self,
+        ref: Ref = "main",
+        archive_format: ArchiveFormat = ArchiveFormat.ZIP,
     ) -> bytes:
         """
         Download all the files in a specific ref of a repository as a zip or tarball
         archive.
 
         https://hub.allspice.io/api/swagger#/repository/repoGetArchive
 
@@ -995,21 +1057,157 @@
         See https://hub.allspice.io/api/swagger#/repository/repoAddTopic
 
         :param topic: The topic to add. Topic names must consist only of
             lowercase letters, numnbers and dashes (-), and cannot start with
             dashes. Topic names also must be under 35 characters long.
         """
 
-        url = self.REPO_ADD_TOPIC.format(
-            owner=self.owner.username,
-            repo=self.name,
-            topic=topic
-        )
+        url = self.REPO_ADD_TOPIC.format(owner=self.owner.username, repo=self.name, topic=topic)
         self.allspice_client.requests_put(url)
 
+    def create_release(
+        self,
+        tag_name: str,
+        name: Optional[str] = None,
+        body: Optional[str] = None,
+        draft: bool = False,
+    ):
+        """
+        Create a release for this repository. The release will be created for
+        the tag with the given name. If there is no tag with this name, create
+        the tag first.
+
+        See https://hub.allspice.io/api/swagger#/repository/repoCreateRelease
+        """
+
+        url = self.REPO_GET_RELEASES.format(owner=self.owner.username, repo=self.name)
+        data = {
+            "tag_name": tag_name,
+            "draft": draft,
+        }
+        if name is not None:
+            data["name"] = name
+        if body is not None:
+            data["body"] = body
+        response = self.allspice_client.requests_post(url, data)
+        return Release.parse_response(self.allspice_client, response, self)
+
+    def get_releases(
+        self, draft: Optional[bool] = None, pre_release: Optional[bool] = None
+    ) -> List[Release]:
+        """
+        Get the list of releases for this repository.
+
+        See https://hub.allspice.io/api/swagger#/repository/repoListReleases
+        """
+
+        data = {}
+
+        if draft is not None:
+            data["draft"] = draft
+        if pre_release is not None:
+            data["pre-release"] = pre_release
+
+        url = self.REPO_GET_RELEASES.format(owner=self.owner.username, repo=self.name)
+        responses = self.allspice_client.requests_get_paginated(url, params=data)
+
+        return [
+            Release.parse_response(self.allspice_client, response, self) for response in responses
+        ]
+
+    def get_latest_release(self) -> Release:
+        """
+        Get the latest release for this repository.
+
+        See https://hub.allspice.io/api/swagger#/repository/repoGetLatestRelease
+        """
+
+        url = self.REPO_GET_LATEST_RELEASE.format(owner=self.owner.username, repo=self.name)
+        response = self.allspice_client.requests_get(url)
+        release = Release.parse_response(self.allspice_client, response, self)
+        return release
+
+    def get_release_by_tag(self, tag: str) -> Release:
+        """
+        Get a release by its tag.
+
+        See https://hub.allspice.io/api/swagger#/repository/repoGetReleaseByTag
+        """
+
+        url = self.REPO_GET_RELEASE_BY_TAG.format(
+            owner=self.owner.username, repo=self.name, tag=tag
+        )
+        response = self.allspice_client.requests_get(url)
+        release = Release.parse_response(self.allspice_client, response, self)
+        return release
+
+    def get_commit_statuses(
+        self,
+        commit: Union[str, Commit],
+        sort: Optional[CommitStatusSort] = None,
+        state: Optional[CommitStatusState] = None,
+    ) -> List[CommitStatus]:
+        """
+        Get a list of statuses for a commit.
+
+        This is roughly equivalent to the Commit.get_statuses method, but this
+        method allows you to sort and filter commits and is more convenient if
+        you have a commit SHA and don't need to get the commit itself.
+
+        See https://hub.allspice.io/api/swagger#/repository/repoListStatuses
+        """
+
+        if isinstance(commit, Commit):
+            commit = commit.sha
+
+        params = {}
+        if sort is not None:
+            params["sort"] = sort.value
+        if state is not None:
+            params["state"] = state.value
+
+        url = self.REPO_GET_COMMIT_STATUS.format(
+            owner=self.owner.username, repo=self.name, sha=commit
+        )
+        response = self.allspice_client.requests_get_paginated(url, params=params)
+        return [CommitStatus.parse_response(self.allspice_client, status) for status in response]
+
+    def create_commit_status(
+        self,
+        commit: Union[str, Commit],
+        context: Optional[str] = None,
+        description: Optional[str] = None,
+        state: Optional[CommitStatusState] = None,
+        target_url: Optional[str] = None,
+    ) -> CommitStatus:
+        """
+        Create a status on a commit.
+
+        See https://hub.allspice.io/api/swagger#/repository/repoCreateStatus
+        """
+
+        if isinstance(commit, Commit):
+            commit = commit.sha
+
+        data = {}
+        if context is not None:
+            data["context"] = context
+        if description is not None:
+            data["description"] = description
+        if state is not None:
+            data["state"] = state.value
+        if target_url is not None:
+            data["target_url"] = target_url
+
+        url = self.REPO_GET_COMMIT_STATUS.format(
+            owner=self.owner.username, repo=self.name, sha=commit
+        )
+        response = self.allspice_client.requests_post(url, data=data)
+        return CommitStatus.parse_response(self.allspice_client, response)
+
     def delete(self):
         self.allspice_client.requests_delete(
             Repository.REPO_DELETE % (self.owner.username, self.name)
         )
         self.deleted = True
 
 
@@ -1088,32 +1286,24 @@
             return False
         return self.repo == other.repo and self.id == other.id
 
     def __hash__(self):
         return hash(self.repo) ^ hash(self.id)
 
     @classmethod
-    def request(
-            cls,
-            allspice_client,
-            owner: str,
-            repo: str,
-            id: str
-    ) -> 'Comment':
+    def request(cls, allspice_client, owner: str, repo: str, id: str) -> "Comment":
         return cls._request(allspice_client, {"owner": owner, "repo": repo, "id": id})
 
     _fields_to_parsers: ClassVar[dict] = {
         "user": lambda allspice_client, r: User.parse_response(allspice_client, r),
         "created_at": lambda _, t: Util.convert_time(t),
         "updated_at": lambda _, t: Util.convert_time(t),
     }
 
-    _patchable_fields: ClassVar[set[str]] = {
-        "body"
-    }
+    _patchable_fields: ClassVar[set[str]] = {"body"}
 
     @property
     def parent_url(self) -> str:
         """URL of the parent of this comment (the issue or the pull request)"""
 
         if self.issue_url is not None:
             return self.issue_url
@@ -1134,32 +1324,29 @@
             "id": self.id,
         }
 
     def commit(self):
         self._commit(self.__fields_for_path())
 
     def delete(self):
-        self.allspice_client.requests_delete(
-            self.API_OBJECT.format(**self.__fields_for_path())
-        )
+        self.allspice_client.requests_delete(self.API_OBJECT.format(**self.__fields_for_path()))
         self.deleted = True
 
     def get_attachments(self) -> List[Attachment]:
         """
         Get all attachments on this comment. This returns Attachment objects, which
         contain a link to download the attachment.
 
         https://hub.allspice.io/api/swagger#/issue/issueListIssueCommentAttachments
         """
 
         results = self.allspice_client.requests_get(
             self.GET_ATTACHMENTS_PATH.format(**self.__fields_for_path())
         )
-        return [Attachment.parse_response(self.allspice_client, result) for result in
-                results]
+        return [Attachment.parse_response(self.allspice_client, result) for result in results]
 
     def create_attachment(self, file: IO, name: Optional[str] = None) -> Attachment:
         """
         Create an attachment on this comment.
 
         https://hub.allspice.io/api/swagger#/issue/issueCreateIssueCommentAttachment
 
@@ -1211,40 +1398,154 @@
             "attachment_id": attachment.id,
         }
         self.allspice_client.requests_delete(self.ATTACHMENT_PATH.format(**args))
         attachment.deleted = True
 
 
 class Commit(ReadonlyApiObject):
+    API_OBJECT = """/repos/{owner}/{repo}/commits/{sha}"""
+    COMMIT_GET_STATUS = """/repos/{owner}/{repo}/commits/{sha}/status"""
+    COMMIT_GET_STATUSES = """/repos/{owner}/{repo}/commits/{sha}/statuses"""
+
+    # Regex to extract owner and repo names from the url property
+    URL_REGEXP = re.compile(r"/repos/([^/]+)/([^/]+)/git/commits")
 
     def __init__(self, allspice_client):
         super().__init__(allspice_client)
 
     _fields_to_parsers: ClassVar[dict] = {
         # NOTE: api may return None for commiters that are no allspice users
-        "author": lambda allspice_client, u: User.parse_response(allspice_client, u) if u else None
+        "author": lambda allspice_client, u: (
+            User.parse_response(allspice_client, u) if u else None
+        )
     }
 
     def __eq__(self, other):
         if not isinstance(other, Commit):
             return False
         return self.sha == other.sha
 
     def __hash__(self):
         return hash(self.sha)
 
     @classmethod
-    def parse_response(cls, allspice_client, result) -> 'Commit':
+    def parse_response(cls, allspice_client, result) -> "Commit":
         commit_cache = result["commit"]
         api_object = cls(allspice_client)
         cls._initialize(allspice_client, api_object, result)
         # inner_commit for legacy reasons
         Commit._add_read_property("inner_commit", commit_cache, api_object)
         return api_object
 
+    def get_status(self) -> CommitCombinedStatus:
+        """
+        Get a combined status consisting of all statues on this commit.
+
+        Note that the returned object is a CommitCombinedStatus object, which
+        also contains a list of all statuses on the commit.
+
+        https://hub.allspice.io/api/swagger#/repository/repoGetCommitStatus
+        """
+
+        result = self.allspice_client.requests_get(
+            self.COMMIT_GET_STATUS.format(**self._fields_for_path)
+        )
+        return CommitCombinedStatus.parse_response(self.allspice_client, result)
+
+    def get_statuses(self) -> List[CommitStatus]:
+        """
+        Get a list of all statuses on this commit.
+
+        https://hub.allspice.io/api/swagger#/repository/repoListCommitStatuses
+        """
+
+        results = self.allspice_client.requests_get(
+            self.COMMIT_GET_STATUSES.format(**self._fields_for_path)
+        )
+        return [CommitStatus.parse_response(self.allspice_client, result) for result in results]
+
+    @cached_property
+    def _fields_for_path(self) -> dict[str, str]:
+        matches = self.URL_REGEXP.search(self.url)
+        return {
+            "owner": matches.group(1),
+            "repo": matches.group(2),
+            "sha": self.sha,
+        }
+
+
+class CommitStatusState(Enum):
+    PENDING = "pending"
+    SUCCESS = "success"
+    ERROR = "error"
+    FAILURE = "failure"
+    WARNING = "warning"
+
+    @classmethod
+    def try_init(cls, value: str) -> Union[CommitStatusState, str]:
+        """
+        Try converting a string to the enum, and if that fails, return the
+        string itself.
+        """
+
+        try:
+            return cls(value)
+        except ValueError:
+            value
+
+
+class CommitStatus(ReadonlyApiObject):
+    def __init__(self, allspice_client):
+        super().__init__(allspice_client)
+
+    _fields_to_parsers: ClassVar[dict] = {
+        # Gitea/ASH doesn't actually validate that the status is a "valid"
+        # status, so we can expect empty or unknown strings in the status field.
+        "status": lambda _, s: CommitStatusState.try_init(s),
+        "creator": lambda allspice_client, u: (
+            User.parse_response(allspice_client, u) if u else None
+        ),
+    }
+
+    def __eq__(self, other):
+        if not isinstance(other, CommitStatus):
+            return False
+        return self.id == other.id
+
+    def __hash__(self):
+        return hash(self.id)
+
+
+class CommitCombinedStatus(ReadonlyApiObject):
+    def __init__(self, allspice_client):
+        super().__init__(allspice_client)
+
+    _fields_to_parsers: ClassVar[dict] = {
+        # See CommitStatus
+        "state": lambda _, s: CommitStatusState.try_init(s),
+        "statuses": lambda allspice_client, statuses: [
+            CommitStatus.parse_response(allspice_client, status) for status in statuses
+        ],
+        "repository": lambda allspice_client, r: Repository.parse_response(allspice_client, r),
+    }
+
+    def __eq__(self, other):
+        if not isinstance(other, CommitCombinedStatus):
+            return False
+        return self.sha == other.sha
+
+    def __hash__(self):
+        return hash(self.sha)
+
+    @classmethod
+    def parse_response(cls, allspice_client, result) -> "CommitCombinedStatus":
+        api_object = cls(allspice_client)
+        cls._initialize(allspice_client, api_object, result)
+        return api_object
+
 
 class Issue(ApiObject):
     API_OBJECT = """/repos/{owner}/{repo}/issues/{index}"""  # <owner, repo, index>
     GET_TIME = """/repos/%s/%s/issues/%s/times"""  # <owner, repo, index>
     GET_COMMENTS = """/repos/{owner}/{repo}/issues/{index}/comments"""
     CREATE_ISSUE = """/repos/{owner}/{repo}/issues"""
 
@@ -1262,18 +1563,22 @@
     def __hash__(self):
         return hash(self.repo) ^ hash(self.id)
 
     _fields_to_parsers: ClassVar[dict] = {
         "milestone": lambda allspice_client, m: Milestone.parse_response(allspice_client, m),
         "user": lambda allspice_client, u: User.parse_response(allspice_client, u),
         "assignee": lambda allspice_client, u: User.parse_response(allspice_client, u),
-        "assignees": lambda allspice_client, us: [User.parse_response(allspice_client, u) for u in us],
-        "state": lambda allspice_client, s: Issue.CLOSED if s == "closed" else Issue.OPENED,
+        "assignees": lambda allspice_client, us: [
+            User.parse_response(allspice_client, u) for u in us
+        ],
+        "state": lambda allspice_client, s: (Issue.CLOSED if s == "closed" else Issue.OPENED),
         # Repository in this request is just a "RepositoryMeta" record, thus request whole object
-        "repository": lambda allspice_client, r: Repository.request(allspice_client, r["owner"], r["name"])
+        "repository": lambda allspice_client, r: Repository.request(
+            allspice_client, r["owner"], r["name"]
+        ),
     }
 
     _parsers_to_fields: ClassVar[dict] = {
         "milestone": lambda m: m.id,
     }
 
     _patchable_fields: ClassVar[set[str]] = {
@@ -1306,19 +1611,15 @@
         result = allspice_client.requests_post(Issue.CREATE_ISSUE.format(**args), data=data)
         return Issue.parse_response(allspice_client, result)
 
     def get_time_sum(self, user: User) -> int:
         results = self.allspice_client.requests_get(
             Issue.GET_TIME % (self.owner.username, self.repo.name, self.number)
         )
-        return sum(
-            result["time"]
-            for result in results
-            if result and result["user_id"] == user.id
-        )
+        return sum(result["time"] for result in results if result and result["user_id"] == user.id)
 
     def get_times(self) -> Optional[Dict]:
         return self.allspice_client.requests_get(
             Issue.GET_TIME % (self.owner.username, self.repository.name, self.number)
         )
 
     def delete_time(self, time_id: str):
@@ -1332,31 +1633,25 @@
         )
 
     def get_comments(self) -> List[Comment]:
         """https://hub.allspice.io/api/swagger#/issue/issueGetComments"""
 
         results = self.allspice_client.requests_get(
             self.GET_COMMENTS.format(
-                owner=self.owner.username,
-                repo=self.repo.name,
-                index=self.number
+                owner=self.owner.username, repo=self.repo.name, index=self.number
             )
         )
 
-        return [
-            Comment.parse_response(self.allspice_client, result) for result in results
-        ]
+        return [Comment.parse_response(self.allspice_client, result) for result in results]
 
     def create_comment(self, body: str) -> Comment:
         """https://hub.allspice.io/api/swagger#/issue/issueCreateComment"""
 
         path = self.GET_COMMENTS.format(
-            owner=self.owner.username,
-            repo=self.repo.name,
-            index=self.number
+            owner=self.owner.username, repo=self.repo.name, index=self.number
         )
 
         response = self.allspice_client.requests_post(path, data={"body": body})
         return Comment.parse_response(self.allspice_client, response)
 
 
 class DesignReview(ApiObject):
@@ -1393,40 +1688,38 @@
             return False
         return self.repo == other.repo and self.id == other.id
 
     def __hash__(self):
         return hash(self.repo) ^ hash(self.id)
 
     @classmethod
-    def parse_response(cls, allspice_client, result) -> 'DesignReview':
+    def parse_response(cls, allspice_client, result) -> "DesignReview":
         api_object = super().parse_response(allspice_client, result)
         cls._add_read_property(
             "repository",
-            Repository.parse_response(allspice_client,
-                                      result["base"]["repo"]),
-            api_object
+            Repository.parse_response(allspice_client, result["base"]["repo"]),
+            api_object,
         )
 
         return api_object
 
     @classmethod
     def request(cls, allspice_client, owner: str, repo: str, number: str):
         """See https://hub.allspice.io/api/swagger#/repository/repoGetPullRequest"""
-        return cls._request(allspice_client,
-                            {"owner": owner, "repo": repo, "index": number})
+        return cls._request(allspice_client, {"owner": owner, "repo": repo, "index": number})
 
     _fields_to_parsers: ClassVar[dict] = {
         "assignee": lambda allspice_client, u: User.parse_response(allspice_client, u),
-        "assignees": lambda allspice_client, us: [User.parse_response(allspice_client, u)
-                                                  for u in us],
-        "base": lambda allspice_client, b: b["ref"],
-        "head": lambda allspice_client, h: h["ref"],
+        "assignees": lambda allspice_client, us: [
+            User.parse_response(allspice_client, u) for u in us
+        ],
+        "base": lambda _, b: b["ref"],
+        "head": lambda _, h: h["ref"],
         "merged_by": lambda allspice_client, u: User.parse_response(allspice_client, u),
-        "milestone": lambda allspice_client, m: Milestone.parse_response(allspice_client,
-                                                                         m),
+        "milestone": lambda allspice_client, m: Milestone.parse_response(allspice_client, m),
         "user": lambda allspice_client, u: User.parse_response(allspice_client, u),
     }
 
     _patchable_fields: ClassVar[set[str]] = {
         "allow_maintainer_edits",
         "assignee",
         "assignees",
@@ -1449,30 +1742,32 @@
         data = self.get_dirty_fields()
         if "due_date" in data and data["due_date"] is None:
             data["unset_due_date"] = True
 
         args = {
             "owner": self.repository.owner.username,
             "repo": self.repository.name,
-            "index": self.number
+            "index": self.number,
         }
         self._commit(args, data)
 
     def merge(self, merge_type: MergeType):
         """
         Merge the pull request. See
         https://hub.allspice.io/api/swagger#/repository/repoMergePullRequest
 
         :param merge_type: The type of merge to perform. See the MergeType enum.
         """
 
         self.allspice_client.requests_put(
-            self.MERGE_DESIGN_REVIEW.format(owner=self.repository.owner.username,
-                                            repo=self.repository.name,
-                                            index=self.number),
+            self.MERGE_DESIGN_REVIEW.format(
+                owner=self.repository.owner.username,
+                repo=self.repository.name,
+                index=self.number,
+            ),
             data={"Do": merge_type.value},
         )
 
     def get_comments(self) -> List[Comment]:
         """
         Get the comments on this pull request, but not specifically on a review.
 
@@ -1481,20 +1776,18 @@
         :return: A list of comments on this pull request.
         """
 
         results = self.allspice_client.requests_get(
             self.GET_COMMENTS.format(
                 owner=self.repository.owner.username,
                 repo=self.repository.name,
-                index=self.number
+                index=self.number,
             )
         )
-        return [
-            Comment.parse_response(self.allspice_client, result) for result in results
-        ]
+        return [Comment.parse_response(self.allspice_client, result) for result in results]
 
     def create_comment(self, body: str):
         """
         Create a comment on this pull request. This uses the same endpoint as the
         comments on issues, and will not be associated with any reviews.
 
         https://hub.allspice.io/api/swagger#/issue/issueCreateComment
@@ -1503,17 +1796,17 @@
         :return: The comment that was created.
         """
 
         result = self.allspice_client.requests_post(
             self.GET_COMMENTS.format(
                 owner=self.repository.owner.username,
                 repo=self.repository.name,
-                index=self.number
+                index=self.number,
             ),
-            data={"body": body}
+            data={"body": body},
         )
         return Comment.parse_response(self.allspice_client, result)
 
 
 class Team(ApiObject):
     API_OBJECT = """/teams/{id}"""  # <id>
     ADD_REPO = """/teams/%s/repos/%s/%s"""  # <id, org, repo>
@@ -1563,34 +1856,230 @@
         if isinstance(repo, Repository):
             repo_name = repo.name
         else:
             repo_name = repo
         self.allspice_client.requests_put(Team.ADD_REPO % (self.id, org.username, repo_name))
 
     def get_members(self):
-        """ Get all users assigned to the team. """
+        """Get all users assigned to the team."""
         results = self.allspice_client.requests_get_paginated(
             Team.GET_MEMBERS % self.id,
         )
         return [User.parse_response(self.allspice_client, result) for result in results]
 
     def get_repos(self):
-        """ Get all repos of this Team."""
+        """Get all repos of this Team."""
         results = self.allspice_client.requests_get(Team.GET_REPOS % self.id)
         return [Repository.parse_response(self.allspice_client, result) for result in results]
 
     def delete(self):
         self.allspice_client.requests_delete(Team.TEAM_DELETE % self.id)
         self.deleted = True
 
     def remove_team_member(self, user_name: str):
         url = f"/teams/{self.id}/members/{user_name}"
         self.allspice_client.requests_delete(url)
 
 
+class Release(ApiObject):
+    """
+    A release on a repo.
+    """
+
+    API_OBJECT = "/repos/{owner}/{repo}/releases/{id}"
+    RELEASE_CREATE_ASSET = "/repos/{owner}/{repo}/releases/{id}/assets"
+    # Note that we don't strictly need the get_assets route, as the release
+    # object already contains the assets.
+
+    def __init__(self, allspice_client):
+        super().__init__(allspice_client)
+
+    def __eq__(self, other):
+        if not isinstance(other, Release):
+            return False
+        return self.repo == other.repo and self.id == other.id
+
+    def __hash__(self):
+        return hash(self.repo) ^ hash(self.id)
+
+    _fields_to_parsers: ClassVar[dict] = {
+        "author": lambda allspice_client, author: User.parse_response(allspice_client, author),
+    }
+    _patchable_fields: ClassVar[set[str]] = {
+        "body",
+        "draft",
+        "name",
+        "prerelease",
+        "tag_name",
+        "target_commitish",
+    }
+
+    @classmethod
+    def parse_response(cls, allspice_client, result, repo) -> Release:
+        release = super().parse_response(allspice_client, result)
+        Release._add_read_property("repo", repo, release)
+        setattr(
+            release,
+            "_assets",
+            [
+                ReleaseAsset.parse_response(allspice_client, asset, release)
+                for asset in result["assets"]
+            ],
+        )
+        return release
+
+    @classmethod
+    def request(
+        cls,
+        allspice_client,
+        owner: str,
+        repo: str,
+        id: Optional[int] = None,
+    ) -> Release:
+        args = {"owner": owner, "repo": repo, "id": id}
+        release_response = cls._get_gitea_api_object(allspice_client, args)
+        repo = Repository.request(allspice_client, owner, repo)
+        release = cls.parse_response(allspice_client, release_response, repo)
+        return release
+
+    def commit(self):
+        args = {"owner": self.repo.owner.name, "repo": self.repo.name, "id": self.id}
+        self._commit(args)
+
+    def create_asset(self, file: IO, name: Optional[str] = None) -> ReleaseAsset:
+        """
+        Create an asset for this release.
+
+        https://hub.allspice.io/api/swagger#/repository/repoCreateReleaseAsset
+
+        :param file: The file to upload. This should be a file-like object.
+        :param name: The name of the file.
+        :return: The created asset.
+        """
+
+        args = {"files": {"attachment": file}}
+        if name is not None:
+            args["params"] = {"name": name}
+
+        result = self.allspice_client.requests_post(
+            self.RELEASE_CREATE_ASSET.format(
+                owner=self.repo.owner.username,
+                repo=self.repo.name,
+                id=self.id,
+            ),
+            **args,
+        )
+        return ReleaseAsset.parse_response(self.allspice_client, result, self)
+
+    def delete(self):
+        args = {"owner": self.repo.owner.name, "repo": self.repo.name, "id": self.id}
+        self.allspice_client.requests_delete(self.API_OBJECT.format(**args))
+        self.deleted = True
+
+
+class ReleaseAsset(ApiObject):
+    API_OBJECT = "/repos/{owner}/{repo}/releases/{release_id}/assets/{id}"
+
+    def __init__(self, allspice_client):
+        super().__init__(allspice_client)
+
+    def __eq__(self, other):
+        if not isinstance(other, ReleaseAsset):
+            return False
+        return self.release == other.release and self.id == other.id
+
+    def __hash__(self):
+        return hash(self.release) ^ hash(self.id)
+
+    _fields_to_parsers: ClassVar[dict] = {}
+    _patchable_fields: ClassVar[set[str]] = {
+        "name",
+    }
+
+    @classmethod
+    def parse_response(cls, allspice_client, result, release) -> ReleaseAsset:
+        asset = super().parse_response(allspice_client, result)
+        ReleaseAsset._add_read_property("release", release, asset)
+        return asset
+
+    @classmethod
+    def request(
+        cls,
+        allspice_client,
+        owner: str,
+        repo: str,
+        release_id: int,
+        id: int,
+    ) -> ReleaseAsset:
+        args = {"owner": owner, "repo": repo, "release_id": release_id, "id": id}
+        asset_response = cls._get_gitea_api_object(allspice_client, args)
+        release = Release.request(allspice_client, owner, repo, release_id)
+        asset = cls.parse_response(allspice_client, asset_response, release)
+        return asset
+
+    def commit(self):
+        args = {
+            "owner": self.release.repo.owner,
+            "repo": self.release.repo.name,
+            "release_id": self.release.id,
+            "id": self.id,
+        }
+        self._commit(args)
+
+    def download(self) -> bytes:
+        """
+        Download the raw, binary data of this asset.
+
+        Note 1: if the file you are requesting is a text file, you might want to
+        use .decode() on the result to get a string. For example:
+
+            asset.download().decode("utf-8")
+
+        Note 2: this method will store the entire file in memory. If you are
+        downloading a large file, you might want to use download_to_file instead.
+        """
+
+        return self.allspice_client.requests.get(
+            self.browser_download_url,
+            headers=self.allspice_client.headers,
+        ).content
+
+    def download_to_file(self, io: IO):
+        """
+        Download the raw, binary data of this asset to a file-like object.
+
+        Example:
+
+            with open("my_file.zip", "wb") as f:
+                asset.download_to_file(f)
+
+        :param io: The file-like object to write the data to.
+        """
+
+        response = self.allspice_client.requests.get(
+            self.browser_download_url,
+            headers=self.allspice_client.headers,
+            stream=True,
+        )
+        # 4kb chunks
+        for chunk in response.iter_content(chunk_size=4096):
+            if chunk:
+                io.write(chunk)
+
+    def delete(self):
+        args = {
+            "owner": self.release.repo.owner.name,
+            "repo": self.release.repo.name,
+            "release_id": self.release.id,
+            "id": self.id,
+        }
+        self.allspice_client.requests_delete(self.API_OBJECT.format(**args))
+        self.deleted = True
+
+
 class Content(ReadonlyApiObject):
     FILE = "file"
 
     def __init__(self, allspice_client):
         super().__init__(allspice_client)
 
     def __eq__(self, other):
@@ -1604,15 +2093,15 @@
 
 Ref = Union[Branch, Commit, str]
 
 
 class Util:
     @staticmethod
     def convert_time(time: str) -> datetime:
-        """ Parsing of strange Gitea time format ("%Y-%m-%dT%H:%M:%S:%z" but with ":" in time zone notation)"""
+        """Parsing of strange Gitea time format ("%Y-%m-%dT%H:%M:%S:%z" but with ":" in time zone notation)"""
         try:
             return datetime.strptime(time[:-3] + "00", "%Y-%m-%dT%H:%M:%S%z")
         except ValueError:
             return datetime.strptime(time[:-3] + "00", "%Y-%m-%dT%H:%M:%S")
 
     @staticmethod
     def format_time(time: datetime) -> str:
```

### Comparing `py-allspice-2.4.0/allspice/baseapiobject.py` & `py_allspice-2.5.0/allspice/baseapiobject.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import ClassVar, Optional
 
 from .exceptions import ObjectIsInvalid, MissingEqualityImplementation, RawRequestEndpointMissing
 
 
 class ReadonlyApiObject:
-
     def __init__(self, allspice_client):
         self.allspice_client = allspice_client
         self.deleted = False  # set if .delete was called, so that an exception is risen
 
     def __str__(self):
         return "AllSpiceObject (%s):" % (type(self))
 
@@ -33,15 +32,15 @@
     def _request(cls, allspice_client, args):
         result = cls._get_gitea_api_object(allspice_client, args)
         api_object = cls.parse_response(allspice_client, result)
         return api_object
 
     @classmethod
     def _get_gitea_api_object(cls, allspice_client, args):
-        """Retrieving an object always as GET_API_OBJECT """
+        """Retrieving an object always as GET_API_OBJECT"""
         return allspice_client.requests_get(cls.API_OBJECT.format(**args))
 
     @classmethod
     def parse_response(cls, allspice_client, result) -> "ReadonlyApiObject":
         # allspice_client.logger.debug("Found api object of type %s (id: %s)" % (type(cls), id))
         api_object = cls(allspice_client)
         cls._initialize(allspice_client, api_object, result)
@@ -59,16 +58,15 @@
             if not hasattr(api_object, name):
                 cls._add_read_property(name, None, api_object)
 
     @classmethod
     def _add_read_property(cls, name, value, api_object):
         if not hasattr(api_object, name):
             setattr(api_object, "_" + name, value)
-            prop = property(
-                (lambda n: lambda self: self._get_var(n))(name))
+            prop = property((lambda n: lambda self: self._get_var(n))(name))
             setattr(cls, name, prop)
         else:
             raise AttributeError(f"Attribute {name} already exists on api object.")
 
     def _get_var(self, name):
         if self.deleted:
             raise ObjectIsInvalid()
@@ -120,15 +118,16 @@
 
     @classmethod
     def _add_write_property(cls, name, value, api_object):
         if not hasattr(api_object, "_" + name):
             setattr(api_object, "_" + name, value)
         prop = property(
             (lambda n: lambda self: self._get_var(n))(name),
-            (lambda n: lambda self, v: self.__set_var(n, v))(name))
+            (lambda n: lambda self, v: self.__set_var(n, v))(name),
+        )
         setattr(cls, name, prop)
 
     def __set_var(self, name, i):
         if self.deleted:
             raise ObjectIsInvalid()
         self._dirty_fields.add(name)
         setattr(self, "_" + name, i)
```

### Comparing `py-allspice-2.4.0/allspice/exceptions.py` & `py_allspice-2.5.0/allspice/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,22 +17,25 @@
 class NotYetGeneratedException(Exception):
     """
     For AllSpice generated objects, this exception is raised when the
     object has not yet been generated.
 
     Usually, retrying after a while will be successful.
     """
+
     pass
 
 
 class RawRequestEndpointMissing(Exception):
     """This ApiObject can only be obtained through other api objects and does not have
     diret .request method."""
+
     pass
 
 
 class MissingEqualityImplementation(Exception):
     """
     Each Object obtained from the AllSpice Hub api must be able to check itself for equality in relation to its
     fields obtained from gitea. Risen if an api object is lacking the proper implementation.
     """
+
     pass
```

### Comparing `py-allspice-2.4.0/allspice/ratelimiter.py` & `py_allspice-2.5.0/allspice/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `py-allspice-2.4.0/allspice/utils/bom_generation.py` & `py_allspice-2.5.0/allspice/utils/bom_generation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from __future__ import annotations
-import base64
 
 from dataclasses import dataclass
 import re
 import time
 from typing import Optional, Union
 
 from allspice.utils.core import get_all_pcb_components
 
 from ..allspice import AllSpice
 from ..apiobject import Content, Ref, Repository
 from ..exceptions import NotYetGeneratedException
 
+PRJPCB_SCHDOC_REGEX = re.compile(r"DocumentPath=(.*?SchDoc)(\r\n|\n\r|\n)")
+
 
 @dataclass
 class SchematicComponent:
     description: str
     manufacturer: str
     part_number: str
     designator: str
@@ -80,14 +81,15 @@
         return AttributesMapping(
             description=dictionary["description"],
             manufacturer=dictionary["manufacturer"],
             part_number=dictionary["part_number"],
             designator=dictionary["designator"],
         )
 
+
 # TODO: We should make this generic for all PCBs and change all `pcbdoc` references to `pcb`
 # TODO: We should default to generating a BOM using only the project file + schematics.
 #   Using PCB to generate the BOM should be an option flag, but we shouldn't be combining
 #   PCB and schematic BOMs.
 
 
 def generate_bom_for_altium(
@@ -118,15 +120,15 @@
     """
 
     allspice_client.logger.info(
         f"Generating BOM for {repository.name=} on {ref=} using {attributes_mapping=}"
     )
     allspice_client.logger.info(f"Fetching {prjpcb_file=} and {pcbdoc_file=}")
 
-    prjpcb_file = _get_file_content(repository, prjpcb_file, ref)
+    prjpcb_file = repository.get_raw_file(prjpcb_file, ref=ref).decode("utf-8")
     schdoc_files_in_proj = {x for x in _extract_schdoc_list_from_prjpcb(prjpcb_file)}
 
     allspice_client.logger.info("Found %d SchDoc files", len(schdoc_files_in_proj))
 
     schdoc_components = _extract_all_schdoc_components(
         repository,
         ref,
@@ -158,37 +160,22 @@
     for alternative in alternatives:
         if alternative in attributes:
             return attributes[alternative]["text"]
 
     return None
 
 
-def _get_file_content(repo, file_path, ref) -> str:
-    """
-    Get the content of a file in a repo on a branch.
-    """
-
-    files_in_repo = repo.get_git_content(ref=ref)
-    file = next((x for x in files_in_repo if x.path == file_path), None)
-    if not file:
-        raise ValueError(
-            f"File {file_path} not found in repo {repo.name} at ref {ref.name}"
-        )
-
-    content = repo.get_file_content(file, ref=ref)
-    return base64.b64decode(content).decode("utf-8")
-
-
 def _extract_schdoc_list_from_prjpcb(prjpcb_file_content) -> list[str]:
     """
     Get a list of SchDoc files from a PrjPcb file.
     """
 
-    pattern = re.compile(r"DocumentPath=(.*?SchDoc)\r\n")
-    return [match.group(1) for match in pattern.finditer(prjpcb_file_content)]
+    # Sometimes the SchDoc file can use \n\r instead of CRLF line endings.
+    # Unfortunately, it looks like $ even with re.M doesn't(?) match \n\r.
+    return [match.group(1) for match in PRJPCB_SCHDOC_REGEX.finditer(prjpcb_file_content)]
 
 
 def _schdoc_component_from_attributes(
     attributes: dict,
     mapper: AttributesMapping,
 ) -> SchematicComponent:
     """
@@ -325,17 +312,15 @@
     orphan_pcb_components = []
 
     for pcbdoc_component in pcbdoc_components:
         if pcbdoc_component.schematic_link in schdoc_components_by_designator:
             schdoc_designator = pcbdoc_component.schematic_link
             pcb_designator = pcbdoc_component.designator
 
-            pcb_designators_for_schdoc_designators[schdoc_designator].append(
-                pcb_designator
-            )
+            pcb_designators_for_schdoc_designators[schdoc_designator].append(pcb_designator)
         else:
             orphan_pcb_components.append(pcbdoc_component)
 
     bom = []
     for (
         schdoc_designator,
         pcb_designators,
@@ -377,12 +362,10 @@
         if bom_entry.part_number != "":
             if bom_entry.part_number not in bom_entries_by_part_number:
                 bom_entries_by_part_number[bom_entry.part_number] = bom_entry
             else:
                 bom_entries_by_part_number[bom_entry.part_number].designators.extend(
                     bom_entry.designators
                 )
-                bom_entries_by_part_number[
-                    bom_entry.part_number
-                ].quantity += bom_entry.quantity
+                bom_entries_by_part_number[bom_entry.part_number].quantity += bom_entry.quantity
 
     return list(bom_entries_by_part_number.values())
```

### Comparing `py-allspice-2.4.0/allspice/utils/core.py` & `py_allspice-2.5.0/allspice/utils/core.py`

 * *Files identical despite different names*

### Comparing `py-allspice-2.4.0/allspice/utils/netlist_generation.py` & `py_allspice-2.5.0/allspice/utils/netlist_generation.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,17 +46,15 @@
         object returned by the AllSpice API, or a string containing the path to
         the file in the repo.
     :param ref: The ref, i.e. branch, commit or git ref from which to take the
         project files. Defaults to "main".
     :return: A list of netlist entries.
     """
 
-    allspice_client.logger.info(
-        f"Generating netlist for {repository.name=} on {ref=}"
-    )
+    allspice_client.logger.info(f"Generating netlist for {repository.name=} on {ref=}")
     allspice_client.logger.info(f"Fetching {pcb_file=}")
 
     pcb_components = _extract_all_pcb_components(allspice_client.logger, repository, ref, pcb_file)
 
     return _group_netlist_entries(pcb_components)
 
 
@@ -76,33 +74,28 @@
     for component in component_instances.values():
         pins = []
         for pin in component["pads"].values():
             try:
                 designator = pin["designator"]
             except KeyError:
                 logger.warn(
-                    f"No pad designator: pad in component {component['designator']} has no defined designator.")
+                    f"No pad designator: pad in component {component['designator']} has no defined designator."
+                )
                 continue
 
             try:
                 net = pin["net_name"]
             except KeyError:
                 logger.warning(
-                    f"Unconnected pad: {designator} in component {component['designator']}.")
+                    f"Unconnected pad: {designator} in component {component['designator']}."
+                )
                 continue
 
-            pins.append(ComponentPin(
-                designator=designator,
-                net=net
-            ))
-        components.append(
-            PcbComponent(
-                designator=component["designator"],
-                pins=pins)
-        )
+            pins.append(ComponentPin(designator=designator, net=net))
+        components.append(PcbComponent(designator=component["designator"], pins=pins))
 
     return components
 
 
 def _group_netlist_entries(components: list[PcbComponent]) -> dict[NetlistEntry]:
     """
     Group connected pins by the net
@@ -110,9 +103,10 @@
 
     netlist_entries_by_net = {}
 
     for component in components:
         for pin in component.pins:
             if pin.net:
                 netlist_entries_by_net.setdefault(pin.net, []).append(
-                    component.designator + "." + str(pin.designator))
+                    component.designator + "." + str(pin.designator)
+                )
     return netlist_entries_by_net
```

### Comparing `py-allspice-2.4.0/py_allspice.egg-info/PKG-INFO` & `py_allspice-2.5.0/py_allspice.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-allspice
-Version: 2.4.0
+Version: 2.5.0
 Summary: A python wrapper for the AllSpice Hub API
 Home-page: https://github.com/AllSpiceIO/py-allspice
 Download-URL: https://github.com/AllSpiceIO/py-allspice
 Author: AllSpice, Inc.
 Author-email: maintainers@allspice.io
 License: MIT
 Keywords: AllSpice,AllSpice Hub,api,wrapper
@@ -25,16 +25,17 @@
 
 Forked from https://github.com/Langenfeld/py-gitea.
 
 ## Usage
 
 ### Examples
 
-Check the [examples directory](./examples/) for full, working example scripts
-that you can adapt or refer to for your own needs.
+Check the [examples directory](https://github.com/AllSpiceIO/py-allspice/tree/main/examples)
+for full, working example scripts that you can adapt or refer to for your own
+needs.
 
 ### Quickstart
 
 First get an `allspice_client` object wrapping access and authentication (via an api token) for your instance of AllSpice Hub.
 
 ```python
 from allspice import *
@@ -49,15 +50,15 @@
 Operations like requesting the AllSpice version or authentication user can be requested directly from the `allspice_client` object:
 
 ```python
 print("AllSpice Version: " + allspice_client.get_version())
 print("API-Token belongs to user: " + allspice_client.get_user().username)
 ```
 
-Adding entities like Users, Organizations, ...  also is done via the allspice_client object.
+Adding entities like Users, Organizations, ... also is done via the allspice_client object.
 
 ```python
 user = allspice_client.create_user("Test Testson", "test@test.test", "password")
 ```
 
 All operations on entities in allspice are then accomplished via the according wrapper objects for those entities.
 Each of those objects has a `.request` method that creates an entity according to your allspice_client instance.
@@ -65,52 +66,52 @@
 ```python
 other_user = User.request(allspice_client, "OtherUserName")
 print(other_user.username)
 ```
 
 Note that the fields of the User, Organization,... classes are dynamically created at runtime, and thus not visible during divelopment. Refer to the AllSpice API documentation for the fields names.
 
-
 Fields that can not be altered via allspice-api, are read only. After altering a field, the `.commit` method of the according object must be called to synchronize the changed fields with your allspice_client instance.
 
 ```python
 org = Organization.request(allspice_client, test_org)
 org.description = "some new description"
 org.location = "some new location"
 org.commit()
 ```
 
 An entity in allspice can be deleted by calling delete.
+
 ```python
 org.delete()
 ```
 
 All entity objects do have methods to execute some of the requests possible though the AllSpice api:
+
 ```python
 org = Organization.request(allspice_client, ORGNAME)
 teams = org.get_teams()
 for team in teams:
 	repos = team.get_repos()
 	for repo in repos:
 		print(repo.name)
 ```
 
-
 ## Installation
 
-Use ``pip install py-allspice`` to install.
+Use `pip install py-allspice` to install.
 
 ## A Note on Versioning
 
 This repository does not follow the same versioning policy as py-gitea. After v1.17.x,
 py-allspice switched to Semantic Versioning with v2.0.0. In general, versions of
 py-allspice do NOT conform to versions of AllSpice Hub, and the latest version of
 py-allspice should be compatible with the current version of AllSpice Hub.
 
 ## Tests
 
 Tests can be run with:
 
-```python3 -m pytest test_api.py```
+`python3 -m pytest test_api.py`
 
 Make sure to have an instance of AllSpice Hub running on `http://localhost:3000`, and an admin-user token at `.token`.
-The admin user must be named ``test``, with email ``secondarytest@test.org``.
+The admin user must be named `test`, with email `secondarytest@test.org`.
```

### Comparing `py-allspice-2.4.0/py_allspice.egg-info/SOURCES.txt` & `py_allspice-2.5.0/py_allspice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-allspice-2.4.0/setup.py` & `py_allspice-2.5.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,29 @@
 from setuptools import setup, find_packages
 
-with open('README.md') as readme_file:
+with open("README.md") as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
-    name='py-allspice',
-    version='2.4.0',
-    description='A python wrapper for the AllSpice Hub API',
+    name="py-allspice",
+    version="2.5.0",
+    description="A python wrapper for the AllSpice Hub API",
     long_description_content_type="text/markdown",
     long_description=README,
-    license='MIT',
+    license="MIT",
     packages=find_packages(),
-    author='AllSpice, Inc.',
-    author_email='maintainers@allspice.io',
-    keywords=['AllSpice', 'AllSpice Hub', 'api', 'wrapper'],
-    url='https://github.com/AllSpiceIO/py-allspice',
-    download_url='https://github.com/AllSpiceIO/py-allspice'
+    author="AllSpice, Inc.",
+    author_email="maintainers@allspice.io",
+    keywords=["AllSpice", "AllSpice Hub", "api", "wrapper"],
+    url="https://github.com/AllSpiceIO/py-allspice",
+    download_url="https://github.com/AllSpiceIO/py-allspice",
 )
 
 install_requires = [
-    'requests',
-    'frozendict',
+    "requests",
+    "frozendict",
 ]
 
-extras_require = {
-    'test': ['pytest']
-}
+extras_require = {"test": ["pytest"]}
 
-if __name__ == '__main__':
-    setup(
-        **setup_args,
-        install_requires=install_requires,
-        extras_require=extras_require
-    )
+if __name__ == "__main__":
+    setup(**setup_args, install_requires=install_requires, extras_require=extras_require)
```

### Comparing `py-allspice-2.4.0/tests/test_api.py` & `py_allspice-2.5.0/tests/test_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,52 @@
 import base64
 import datetime
 import time
 
 import pytest
 import uuid
 
-from allspice import AllSpice, User, Organization, Team, Repository, Issue, Milestone, \
-    DesignReview, Branch, Comment
+from allspice import (
+    AllSpice,
+    User,
+    Organization,
+    Team,
+    Repository,
+    Issue,
+    Milestone,
+    DesignReview,
+    Branch,
+    Comment,
+)
 from allspice import NotFoundException
-from allspice.apiobject import Util
+from allspice.apiobject import CommitStatusState, Util
 from allspice.exceptions import NotYetGeneratedException
 
 # put a ".token" file into your directory containg only the token for AllSpice Hub
 
 
 @pytest.fixture(scope="session")
 def port(pytestconfig):
-    '''Load --port command-line arg if set'''
+    """Load --port command-line arg if set"""
     return pytestconfig.getoption("port")
 
 
 @pytest.fixture
 def instance(port, scope="module"):
     try:
-        g = AllSpice(f"http://localhost:{port}", open(".token",
-                     "r").read().strip(), ratelimiting=None)
+        g = AllSpice(
+            f"http://localhost:{port}",
+            open(".token", "r").read().strip(),
+            ratelimiting=None,
+        )
         print("AllSpice Hub Version: " + g.get_version())
         print("API-Token belongs to user: " + g.get_user().username)
         return g
     except Exception:
-        assert (
-            False
-        ), f"AllSpice Hub could not load. \
+        assert False, f"AllSpice Hub could not load. \
                 - Instance running at http://localhost:{port} \
                 - Token at .token   \
                     ?"
 
 
 # make up some fresh names for the tests run
 test_org = "org_" + uuid.uuid4().hex[:8]
@@ -86,15 +97,15 @@
 def test_change_user(instance):
     user = instance.get_user_by_name(test_user)
     location = "a house"
     user.location = location
     new_fullname = "Other Test Full Name"
     user.full_name = new_fullname
     user.commit(user.username, 0)
-    del (user)
+    del user
     user = instance.get_user_by_name(test_user)
     assert user.full_name == new_fullname
     assert user.location == location
 
 
 def test_create_org(instance):
     user = instance.get_user()
@@ -155,15 +166,18 @@
 
 def test_add_content_to_repo(instance):
     repo = Repository.request(instance, test_org, test_repo)
     file_content = open("tests/data/test.pcbdoc", "rb").read()
     file_content = base64.b64encode(file_content).decode("utf-8")
     repo.create_file("test.pcbdoc", file_content)
     assert len(repo.get_commits()) == 2
-    assert [content.name for content in repo.get_git_content()] == ["README.md", "test.pcbdoc"]
+    assert [content.name for content in repo.get_git_content()] == [
+        "README.md",
+        "test.pcbdoc",
+    ]
 
 
 def test_get_json_before_generated(instance):
     repo = Repository.request(instance, test_org, test_repo)
     with pytest.raises(NotYetGeneratedException):
         repo.get_generated_json("test.pcbdoc")
 
@@ -282,41 +296,47 @@
     readmes = [c for c in content if c.name == "README.md"]
     assert len(readmes) > 0
     readme_content = repo.get_file_content(readmes[0])
     assert len(readme_content) > 0
     assert "descr" in str(base64.b64decode(readme_content))
 
 
+def test_get_raw_file(instance):
+    org = Organization.request(instance, test_org)
+    repo = org.get_repository(test_repo)
+    readme_content = repo.get_raw_file("README.md")
+    assert len(readme_content) > 0
+    assert "descr" in str(readme_content)
+
+
 def test_create_file(instance):
     TESTFILE_CONENTE = "TestStringFileContent"
-    TESTFILE_CONENTE_B64 = base64.b64encode(bytes(TESTFILE_CONENTE, 'utf-8'))
+    TESTFILE_CONENTE_B64 = base64.b64encode(bytes(TESTFILE_CONENTE, "utf-8"))
     org = Organization.request(instance, test_org)
     repo = org.get_repository(test_repo)
-    repo.create_file("testfile.md",
-                     content=TESTFILE_CONENTE_B64.decode("ascii"))
+    repo.create_file("testfile.md", content=TESTFILE_CONENTE_B64.decode("ascii"))
     # test if putting was successful
     content = repo.get_git_content()
     readmes = [c for c in content if c.name == "testfile.md"]
     assert len(readmes) > 0
     readme_content = repo.get_file_content(readmes[0])
     assert len(readme_content) > 0
     assert TESTFILE_CONENTE in str(base64.b64decode(readme_content))
 
 
 def test_change_file(instance):
     TESTFILE_CONENTE = "TestStringFileContent with changed content now"
-    TESTFILE_CONENTE_B64 = base64.b64encode(bytes(TESTFILE_CONENTE, 'utf-8'))
+    TESTFILE_CONENTE_B64 = base64.b64encode(bytes(TESTFILE_CONENTE, "utf-8"))
     org = Organization.request(instance, test_org)
     repo = org.get_repository(test_repo)
     # figure out the sha of the file to change
     content = repo.get_git_content()
     readmes = [c for c in content if c.name == "testfile.md"]
     # change
-    repo.change_file("testfile.md", readmes[0].sha,
-                     content=TESTFILE_CONENTE_B64.decode("ascii"))
+    repo.change_file("testfile.md", readmes[0].sha, content=TESTFILE_CONENTE_B64.decode("ascii"))
     # test if putting was successful
     content = repo.get_git_content()
     readmes = [c for c in content if c.name == "testfile.md"]
     assert len(readmes) > 0
     readme_content = repo.get_file_content(readmes[0])
     assert len(readme_content) > 0
     assert TESTFILE_CONENTE in str(base64.b64decode(readme_content))
@@ -337,19 +357,29 @@
 
 
 def test_create_branch(instance):
     org = Organization.request(instance, test_org)
     repo = org.get_repository(test_repo)
     branches = repo.get_branches()
     master = [b for b in branches if b.name == "master"]
-    number_of_branches = len(branches)
     assert len(master) > 0
-    repo.add_branch(master[0], "test_branch")
-    branches = repo.get_branches()
-    assert len(branches) == number_of_branches + 1
+    branch = repo.add_branch(master[0], "test_branch")
+    assert branch.name == "test_branch"
+    branch = repo.get_branch("test_branch")
+    assert branch.name == "test_branch"
+
+
+def test_create_branch_from_str_ref(instance):
+    org = Organization.request(instance, test_org)
+    repo = org.get_repository(test_repo)
+    new_branch_name = "branch-" + uuid.uuid4().hex[:8]
+    branch = repo.add_branch("master", new_branch_name)
+    assert branch.name == new_branch_name
+    branch = repo.get_branch(new_branch_name)
+    assert branch.name == new_branch_name
 
 
 def test_create_team(instance):
     org = Organization.request(instance, test_org)
     team = instance.create_team(org, test_team, "descr")
     assert team.name == test_team
     assert team.description == "descr"
@@ -383,15 +413,15 @@
 
 def test_create_team_with_units_map(instance):
     org = Organization.request(instance, test_org)
     team = instance.create_team(
         org,
         test_team + "2",
         "descr",
-        units_map={"repo.code": "write", "repo.wiki": "admin"}
+        units_map={"repo.code": "write", "repo.wiki": "admin"},
     )
     assert set(team.units) == set(["repo.code", "repo.wiki"])
     assert team.units_map == {"repo.code": "write", "repo.wiki": "admin"}
 
 
 def test_patch_team(instance):
     fields = {
@@ -489,16 +519,24 @@
     issue2.milestone = milestone
     issue2.commit()
     del issue2
     issue3 = Issue.request(instance, org.username, repo.name, number)
     assert issue3.milestone is not None
     assert issue3.milestone.description == "this is only a teststone2"
     issues = repo.get_issues()
-    assert len([issue for issue in issues
-                if issue.milestone is not None and issue.milestone.title == ms_title]) > 0
+    assert (
+        len(
+            [
+                issue
+                for issue in issues
+                if issue.milestone is not None and issue.milestone.title == ms_title
+            ]
+        )
+        > 0
+    )
 
 
 def test_create_issue_comment(instance):
     org = Organization.request(instance, test_org)
     repo = Repository.request(instance, org.username, test_repo)
     issue = repo.get_issues()[0]
     comment = issue.create_comment("this is a comment")
@@ -550,16 +588,15 @@
 
 
 def test_create_issue_attachment_with_name(instance):
     org = Organization.request(instance, test_org)
     repo = Repository.request(instance, org.username, test_repo)
     issue = repo.get_issues()[0]
     comment = issue.create_comment("this is a comment that will have an attachment")
-    attachment = comment.create_attachment(open("requirements.txt", "rb"),
-                                           "something else.txt")
+    attachment = comment.create_attachment(open("requirements.txt", "rb"), "something else.txt")
     assert attachment.name == "something else.txt"
     assert attachment.download_count == 0
 
 
 def test_get_issue_attachments(instance):
     org = Organization.request(instance, test_org)
     repo = Repository.request(instance, org.username, test_repo)
@@ -660,14 +697,159 @@
     repo = Repository.request(instance, org.username, test_repo)
     dr = repo.get_design_reviews()[0]
     comments = dr.get_comments()
     assert len(comments) > 0
     assert comments[0].body == "This is a test comment"
 
 
+def test_repo_create_release(instance):
+    org = Organization.request(instance, test_org)
+    repo = Repository.request(instance, org.username, test_repo)
+    # Just a tag should be enough.
+    release = repo.create_release("v0.0.1")
+    assert release.tag_name == "v0.0.1"
+    release = repo.create_release("v0.1.0", "v0.1.0 release", "release with new tag")
+    assert release.tag_name == "v0.1.0"
+    assert release.name == "v0.1.0 release"
+    assert release.body == "release with new tag"
+
+
+def test_get_repo_releases(instance):
+    org = Organization.request(instance, test_org)
+    repo = Repository.request(instance, org.username, test_repo)
+    releases = repo.get_releases()
+    assert len(releases) > 0
+    assert releases[0].name == "v0.1.0 release"
+
+
+def test_get_repo_latest_release(instance):
+    org = Organization.request(instance, test_org)
+    repo = Repository.request(instance, org.username, test_repo)
+    release = repo.get_latest_release()
+    assert release is not None
+    assert release.name == "v0.1.0 release"
+
+
+def test_get_release_by_tag(instance):
+    org = Organization.request(instance, test_org)
+    repo = Repository.request(instance, org.username, test_repo)
+    release = repo.get_release_by_tag("v0.1.0")
+    assert release is not None
+    assert release.name == "v0.1.0 release"
+
+
+def test_edit_release(instance):
+    org = Organization.request(instance, test_org)
+    repo = Repository.request(instance, org.username, test_repo)
+    release = repo.get_latest_release()
+    # Note that the tag hasn't changed
+    release.name = "v0.1.1 release"
+    release.body = "release with changed name"
+    release.commit()
+    del release
+    release = repo.get_latest_release()
+    assert release.name == "v0.1.1 release"
+    assert release.body == "release with changed name"
+
+
+def test_create_release_asset(instance):
+    org = Organization.request(instance, test_org)
+    repo = Repository.request(instance, org.username, test_repo)
+    release = repo.get_latest_release()
+    asset = release.create_asset(open("requirements.txt", "rb"))
+    assert asset.name == "requirements.txt"
+    assert asset.download_count == 0
+
+
+def test_create_release_asset_with_name(instance):
+    org = Organization.request(instance, test_org)
+    repo = Repository.request(instance, org.username, test_repo)
+    release = repo.get_latest_release()
+    asset = release.create_asset(open("requirements.txt", "rb"), "something else.txt")
+    assert asset.name == "something else.txt"
+    assert asset.download_count == 0
+
+
+def test_get_release_assets(instance):
+    org = Organization.request(instance, test_org)
+    repo = Repository.request(instance, org.username, test_repo)
+    release = repo.get_latest_release()
+    assert len(release.assets) > 0
+    assert release.assets[0].name == "requirements.txt"
+
+
+def test_download_release_asset(instance):
+    org = Organization.request(instance, test_org)
+    repo = Repository.request(instance, org.username, test_repo)
+    release = repo.get_latest_release()
+    asset = release.assets[0]
+    data = asset.download()
+    assert data == open("requirements.txt", "rb").read()
+
+
+def test_delete_release_asset(instance):
+    org = Organization.request(instance, test_org)
+    repo = Repository.request(instance, org.username, test_repo)
+    release = repo.get_latest_release()
+    asset = release.assets[0]
+    asset.delete()
+    assert len(release.assets) == (len(repo.get_latest_release().assets) + 1)
+
+
+def test_delete_release(instance):
+    org = Organization.request(instance, test_org)
+    repo = Repository.request(instance, org.username, test_repo)
+    release = repo.get_latest_release()
+    old_releases = repo.get_releases()
+    release.delete()
+    assert len(repo.get_releases()) == len(old_releases) - 1
+
+
+def test_create_commit_status(instance):
+    org = Organization.request(instance, test_org)
+    repo = Repository.request(instance, org.username, test_repo)
+    commit = repo.get_commits()[0]
+    status = repo.create_commit_status(
+        commit,
+        state=CommitStatusState.ERROR,
+        context="This is a test status",
+    )
+    assert status.status == CommitStatusState.ERROR
+    assert status.context == "This is a test status"
+    assert status.description == ""
+
+
+def test_get_commit_statuses(instance):
+    org = Organization.request(instance, test_org)
+    repo = Repository.request(instance, org.username, test_repo)
+    commit = repo.get_commits()[0]
+    statuses = commit.get_statuses()
+    assert len(statuses) > 0
+    assert statuses[0].context == "This is a test status"
+
+
+def test_get_commit_combined_status(instance):
+    org = Organization.request(instance, test_org)
+    repo = Repository.request(instance, org.username, test_repo)
+    commit = repo.get_commits()[0]
+    status = commit.get_status()
+    assert status is not None
+    assert status.state == CommitStatusState.FAILURE
+
+
+def test_get_commit_status_from(instance):
+    org = Organization.request(instance, test_org)
+    repo = Repository.request(instance, org.username, test_repo)
+    commit = repo.get_commits()[0]
+    statuses = repo.get_commit_statuses(commit, state=CommitStatusState.SUCCESS)
+    assert len(statuses) == 0
+    statuses = repo.get_commit_statuses(commit, state=CommitStatusState.ERROR)
+    assert len(statuses) == 1
+
+
 def test_get_repo_archive(instance):
     # This requires a repo with actual files in it, so we use the test repo
     repo = Repository.request(instance, test_org, test_repo)
     branch = repo.get_branches()[0]
     archive = repo.get_archive(branch)
     assert archive is not None
 
@@ -700,27 +882,29 @@
     with pytest.raises(NotFoundException):
         Repository.request(instance, test_user, test_repo)
 
 
 def test_change_repo_ownership_org(instance):
     old_org = Organization.request(instance, test_org)
     user = User.request(instance, test_user)
-    new_org = instance.create_org(user, test_org+"_repomove", "Org for testing moving repositories")
+    new_org = instance.create_org(
+        user, test_org + "_repomove", "Org for testing moving repositories"
+    )
     new_team = instance.create_team(new_org, test_team + "_repomove", "descr")
-    repo_name = test_repo+"_repomove"
+    repo_name = test_repo + "_repomove"
     repo = instance.create_repo(old_org, repo_name, "descr")
     repo.transfer_ownership(new_org, set([new_team]))
     assert repo_name not in [repo.name for repo in old_org.get_repositories()]
     assert repo_name in [repo.name for repo in new_org.get_repositories()]
 
 
 def test_change_repo_ownership_user(instance):
     old_org = Organization.request(instance, test_org)
     user = User.request(instance, test_user)
-    repo_name = test_repo+"_repomove"
+    repo_name = test_repo + "_repomove"
     repo = instance.create_repo(old_org, repo_name, "descr")
     repo.transfer_ownership(user)
     assert repo_name not in [repo.name for repo in old_org.get_repositories()]
     assert repo_name in [repo.name for repo in user.get_repositories()]
     for repo in user.get_repositories():
         repo.transfer_ownership(old_org)
         assert repo_name in [repo.name for repo in old_org.get_repositories()]
```

### Comparing `py-allspice-2.4.0/tests/test_api_longtests.py` & `py_allspice-2.5.0/tests/test_api_longtests.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,47 +4,49 @@
 from allspice import AllSpice, Issue
 
 # put a ".token" file into your directory containg only the token for AllSpice Hub
 
 
 @pytest.fixture(scope="session")
 def port(pytestconfig):
-    '''Load --port command-line arg if set'''
+    """Load --port command-line arg if set"""
     return pytestconfig.getoption("port")
 
 
 @pytest.fixture
 def instance(port, scope="module"):
     try:
-        g = AllSpice(f"http://localhost:{port}", open(".token",
-                     "r").read().strip(), ratelimiting=None)
+        g = AllSpice(
+            f"http://localhost:{port}", open(".token", "r").read().strip(), ratelimiting=None
+        )
         print("AllSpice Hub Version: " + g.get_version())
         print("API-Token belongs to user: " + g.get_user().username)
         return g
     except Exception:
-        assert (
-            False
-        ), f"AllSpice Hub could not load. \
+        assert False, f"AllSpice Hub could not load. \
                 - Instance running at http://localhost:{port} \
                 - Token at .token   \
                     ?"
 
 
 # make up some fresh names for the tests run
 test_org = "org_" + uuid.uuid4().hex[:8]
 test_user = "user_" + uuid.uuid4().hex[:8]
 test_team = "team_" + uuid.uuid4().hex[:8]  # team names seem to have a rather low max length
 test_repo = "repo_" + uuid.uuid4().hex[:8]
 
 
 def _create_test_org(instance, test_name):
     test_user_unique = "-".join([test_user, test_name])
-    user = instance.create_user(test_user_unique, test_user_unique + "@example.org",
-                                "abcdefg1.23AB", send_notify=False)
-    return instance.create_org(user, "-".join([test_org, test_name]), "some Description for longtests")
+    user = instance.create_user(
+        test_user_unique, test_user_unique + "@example.org", "abcdefg1.23AB", send_notify=False
+    )
+    return instance.create_org(
+        user, "-".join([test_org, test_name]), "some Description for longtests"
+    )
 
 
 def test_list_repos(request, instance):
     org = _create_test_org(instance, request.node.name)
     repos = org.get_repositories()
     assert len(repos) == 0
     # test a number of repository listings larger than the pagination number (default 50)
@@ -53,18 +55,20 @@
     repos = org.get_repositories()
     assert len(repos) >= 53
 
 
 def test_list_issue(request, instance):
     org = _create_test_org(instance, request.node.name)
     repo = instance.create_repo(
-        org, test_repo, "Testing a huge number of Issues and how they are listed")
+        org, test_repo, "Testing a huge number of Issues and how they are listed"
+    )
     for x in range(0, 100):
-        Issue.create_issue(instance, repo, "TestIssue" + str(x),
-                           "We will be too many to be listed on one page")
+        Issue.create_issue(
+            instance, repo, "TestIssue" + str(x), "We will be too many to be listed on one page"
+        )
     issues = repo.get_issues()
     assert len(issues) > 98
 
 
 def test_list_team_members(request, instance):
     org = _create_test_org(instance, request.node.name)
 
@@ -72,13 +76,13 @@
     users = []
     for i in range(100):
         users.append(
             instance.create_user(
                 test_user + str(i),
                 test_user + str(i) + "@example.org",
                 "abcdefg1.23AB",
-                send_notify=False
+                send_notify=False,
             ),
         )
     for user in users:
         team.add_user(user)
     assert len(team.get_members()) == len(users)
```

### Comparing `py-allspice-2.4.0/tests/test_api_ratelimiting.py` & `py_allspice-2.5.0/tests/test_api_ratelimiting.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 import time
 
 from allspice import AllSpice
 
 
 @pytest.fixture(scope="session")
 def port(pytestconfig):
-    '''Load --port command-line arg if set'''
+    """Load --port command-line arg if set"""
     return pytestconfig.getoption("port")
 
+
 # put a ".token" file into your directory containg only the token for AllSpice Hub
 
 
 @pytest.fixture
 def instance(port, scope="module"):
     try:
         g = AllSpice(
@@ -20,17 +21,15 @@
             token_text=open(".token", "r").read().strip(),
             ratelimiting=(10, 1),
         )
         print("AllSpice Hub Version: " + g.get_version())
         print("API-Token belongs to user: " + g.get_user().username)
         return g
     except Exception:
-        assert (
-            False
-        ), f"AllSpice Hub could not load. \
+        assert False, f"AllSpice Hub could not load. \
                 - Instance running at http://localhost:{port} \
                 - Token at .token   \
                     ?"
 
 
 def test_access_is_ratelimited(instance):
     start_time = time.time()
```

### Comparing `py-allspice-2.4.0/tests/test_utils.py` & `py_allspice-2.5.0/tests/test_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,28 @@
+import base64
 import csv
 import dataclasses
 import uuid
 
 import pytest
 
 from allspice import AllSpice
-from allspice.utils.bom_generation import AttributesMapping, generate_bom_for_altium
+from allspice.utils.bom_generation import (
+    AttributesMapping,
+    generate_bom_for_altium,
+)
 from allspice.utils.netlist_generation import generate_netlist
 
 test_repo = "repo_" + uuid.uuid4().hex[:8]
+test_branch = "branch_" + uuid.uuid4().hex[:8]
 
 
 @pytest.fixture(scope="session")
 def port(pytestconfig):
-    '''Load --port command-line arg if set'''
+    """Load --port command-line arg if set"""
     return pytestconfig.getoption("port")
 
 
 @pytest.fixture
 def instance(port):
     try:
         g = AllSpice(
@@ -26,17 +31,15 @@
             ratelimiting=None,
         )
         print("AllSpice Hub Version: " + g.get_version())
         print("API-Token belongs to user: " + g.get_user().username)
 
         return g
     except Exception:
-        assert (
-            False
-        ), f"AllSpice Hub could not load. Is there: \
+        assert False, f"AllSpice Hub could not load. Is there: \
                 - an Instance running at http://localhost:{port} \
                 - a Token at .token \
                     ?"
 
 
 def _setup_for_generation(instance, test_name):
     # TODO: we should commit a smaller set of files in this repo so we don't depend on external data
@@ -49,16 +52,17 @@
             "service": "git",
         },
     )
 
 
 def test_bom_generation(request, instance):
     _setup_for_generation(instance, request.node.name)
-    repo = instance.get_repository(instance.get_user().username,
-                                   "-".join([test_repo, request.node.name]))
+    repo = instance.get_repository(
+        instance.get_user().username, "-".join([test_repo, request.node.name])
+    )
     attributes_mapping = AttributesMapping(
         description=["PART DESCRIPTION"],
         designator=["Designator"],
         manufacturer=["Manufacturer", "MANUFACTURER"],
         part_number=["PART", "MANUFACTURER #"],
     )
     bom = generate_bom_for_altium(
@@ -72,28 +76,87 @@
     )
     assert len(bom) == 107
 
     bom_as_dicts = []
     # We have to do this manually because of how csv.DictWriter works.
     for item in bom:
         entry_as_dict = {}
-        for (key, value) in dataclasses.asdict(item).items():
+        for key, value in dataclasses.asdict(item).items():
+            entry_as_dict[key] = str(value) if value is not None else ""
+        bom_as_dicts.append(entry_as_dict)
+
+    with open("tests/data/archimajor_bom_expected.csv", "r") as f:
+        reader = csv.DictReader(f)
+        for row, expected_row in zip(reader, bom_as_dicts):
+            assert row == expected_row
+
+
+def test_bom_generation_with_odd_line_endings(request, instance):
+    _setup_for_generation(instance, request.node.name)
+    repo = instance.get_repository(
+        instance.get_user().username, "-".join([test_repo, request.node.name])
+    )
+    # We hard-code a ref so that this test is reproducible.
+    ref = "95719adde8107958bf40467ee092c45b6ddaba00"
+    attributes_mapping = AttributesMapping(
+        description=["PART DESCRIPTION"],
+        designator=["Designator"],
+        manufacturer=["Manufacturer", "MANUFACTURER"],
+        part_number=["PART", "MANUFACTURER #"],
+    )
+
+    new_branch_name = "-".join([test_branch, request.node.name])
+    repo.add_branch(ref, new_branch_name)
+    ref = new_branch_name
+
+    files_in_repo = repo.get_git_content(ref=ref)
+    prjpcb_file = next((x for x in files_in_repo if x.path == "Archimajor.PrjPcb"), None)
+    assert prjpcb_file is not None
+
+    original_prjpcb_sha = prjpcb_file.sha
+    prjpcb_content = repo.get_raw_file(prjpcb_file.path, ref=ref).decode("utf-8")
+    new_prjpcb_content = prjpcb_content.replace("\r\n", "\n\r")
+    new_content_econded = base64.b64encode(new_prjpcb_content.encode("utf-8")).decode("utf-8")
+    repo.change_file("Archimajor.PrjPcb", original_prjpcb_sha, new_content_econded, {"branch": ref})
+
+    # Sanity check that the file was changed.
+    prjpcb_content_now = repo.get_raw_file("Archimajor.PrjPcb", ref=ref).decode("utf-8")
+    assert prjpcb_content_now != prjpcb_content
+
+    bom = generate_bom_for_altium(
+        instance,
+        repo,
+        "Archimajor.PrjPcb",
+        "Archimajor.PcbDoc",
+        attributes_mapping,
+        # Note that ref here is the branch, not a commit sha as in the previous
+        # test.
+        ref=ref,
+    )
+    assert len(bom) == 107
+
+    bom_as_dicts = []
+    # We have to do this manually because of how csv.DictWriter works.
+    for item in bom:
+        entry_as_dict = {}
+        for key, value in dataclasses.asdict(item).items():
             entry_as_dict[key] = str(value) if value is not None else ""
         bom_as_dicts.append(entry_as_dict)
 
     with open("tests/data/archimajor_bom_expected.csv", "r") as f:
         reader = csv.DictReader(f)
         for row, expected_row in zip(reader, bom_as_dicts):
             assert row == expected_row
 
 
 def test_netlist_generation(request, instance):
     _setup_for_generation(instance, request.node.name)
-    repo = instance.get_repository(instance.get_user().username,
-                                   "-".join([test_repo, request.node.name]))
+    repo = instance.get_repository(
+        instance.get_user().username, "-".join([test_repo, request.node.name])
+    )
     netlist = generate_netlist(
         instance,
         repo,
         "Archimajor.PcbDoc",
         # We hard-code a ref so that this test is reproducible.
         ref="95719adde8107958bf40467ee092c45b6ddaba00",
     )
```

