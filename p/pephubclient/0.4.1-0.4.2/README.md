# Comparing `tmp/pephubclient-0.4.1.tar.gz` & `tmp/pephubclient-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pephubclient-0.4.1.tar", last modified: Thu Mar  7 21:59:02 2024, max compression
+gzip compressed data, was "pephubclient-0.4.2.tar", last modified: Tue Apr 16 18:35:40 2024, max compression
```

## Comparing `pephubclient-0.4.1.tar` & `pephubclient-0.4.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 21:59:02.792609 pephubclient-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-03-07 21:58:54.000000 pephubclient-0.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-07 21:58:54.000000 pephubclient-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11390 2024-03-07 21:59:02.792609 pephubclient-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10411 2024-03-07 21:58:54.000000 pephubclient-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 21:59:02.788609 pephubclient-0.4.1/pephubclient/
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-07 21:58:54.000000 pephubclient-0.4.1/pephubclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-07 21:58:54.000000 pephubclient-0.4.1/pephubclient/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-03-07 21:58:54.000000 pephubclient-0.4.1/pephubclient/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-03-07 21:58:54.000000 pephubclient-0.4.1/pephubclient/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-03-07 21:58:54.000000 pephubclient-0.4.1/pephubclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-03-07 21:58:54.000000 pephubclient-0.4.1/pephubclient/files_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-03-07 21:58:54.000000 pephubclient-0.4.1/pephubclient/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-03-07 21:58:54.000000 pephubclient-0.4.1/pephubclient/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 21:59:02.788609 pephubclient-0.4.1/pephubclient/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 21:58:54.000000 pephubclient-0.4.1/pephubclient/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-03-07 21:58:54.000000 pephubclient-0.4.1/pephubclient/modules/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     8916 2024-03-07 21:58:54.000000 pephubclient-0.4.1/pephubclient/modules/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 21:59:02.788609 pephubclient-0.4.1/pephubclient/pephub_oauth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 21:58:54.000000 pephubclient-0.4.1/pephubclient/pephub_oauth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-07 21:58:54.000000 pephubclient-0.4.1/pephubclient/pephub_oauth/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-07 21:58:54.000000 pephubclient-0.4.1/pephubclient/pephub_oauth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-07 21:58:54.000000 pephubclient-0.4.1/pephubclient/pephub_oauth/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-03-07 21:58:54.000000 pephubclient-0.4.1/pephubclient/pephub_oauth/pephub_oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)    12455 2024-03-07 21:58:54.000000 pephubclient-0.4.1/pephubclient/pephubclient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 21:59:02.788609 pephubclient-0.4.1/pephubclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11390 2024-03-07 21:59:02.000000 pephubclient-0.4.1/pephubclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-03-07 21:59:02.000000 pephubclient-0.4.1/pephubclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 21:59:02.000000 pephubclient-0.4.1/pephubclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-07 21:59:02.000000 pephubclient-0.4.1/pephubclient.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-07 21:59:02.000000 pephubclient-0.4.1/pephubclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-07 21:59:02.000000 pephubclient-0.4.1/pephubclient.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 21:59:02.788609 pephubclient-0.4.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-07 21:58:54.000000 pephubclient-0.4.1/requirements/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-07 21:58:54.000000 pephubclient-0.4.1/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 21:59:02.792609 pephubclient-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-03-07 21:58:54.000000 pephubclient-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 21:59:02.788609 pephubclient-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-03-07 21:58:54.000000 pephubclient-0.4.1/tests/test_manual.py
--rw-r--r--   0 runner    (1001) docker     (127)    17534 2024-03-07 21:58:54.000000 pephubclient-0.4.1/tests/test_pephubclient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:35:40.460804 pephubclient-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-16 18:35:26.000000 pephubclient-0.4.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-16 18:35:26.000000 pephubclient-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11390 2024-04-16 18:35:40.456804 pephubclient-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10411 2024-04-16 18:35:26.000000 pephubclient-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:35:40.452804 pephubclient-0.4.2/pephubclient/
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-16 18:35:26.000000 pephubclient-0.4.2/pephubclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-16 18:35:26.000000 pephubclient-0.4.2/pephubclient/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-16 18:35:26.000000 pephubclient-0.4.2/pephubclient/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-16 18:35:26.000000 pephubclient-0.4.2/pephubclient/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-16 18:35:26.000000 pephubclient-0.4.2/pephubclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-16 18:35:26.000000 pephubclient-0.4.2/pephubclient/files_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10186 2024-04-16 18:35:26.000000 pephubclient-0.4.2/pephubclient/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-16 18:35:26.000000 pephubclient-0.4.2/pephubclient/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:35:40.456804 pephubclient-0.4.2/pephubclient/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:35:26.000000 pephubclient-0.4.2/pephubclient/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-04-16 18:35:26.000000 pephubclient-0.4.2/pephubclient/modules/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-04-16 18:35:26.000000 pephubclient-0.4.2/pephubclient/modules/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:35:40.456804 pephubclient-0.4.2/pephubclient/pephub_oauth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:35:26.000000 pephubclient-0.4.2/pephubclient/pephub_oauth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-16 18:35:26.000000 pephubclient-0.4.2/pephubclient/pephub_oauth/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-16 18:35:26.000000 pephubclient-0.4.2/pephubclient/pephub_oauth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-16 18:35:26.000000 pephubclient-0.4.2/pephubclient/pephub_oauth/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-04-16 18:35:26.000000 pephubclient-0.4.2/pephubclient/pephub_oauth/pephub_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12455 2024-04-16 18:35:26.000000 pephubclient-0.4.2/pephubclient/pephubclient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:35:40.456804 pephubclient-0.4.2/pephubclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11390 2024-04-16 18:35:40.000000 pephubclient-0.4.2/pephubclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-16 18:35:40.000000 pephubclient-0.4.2/pephubclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 18:35:40.000000 pephubclient-0.4.2/pephubclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-16 18:35:40.000000 pephubclient-0.4.2/pephubclient.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-16 18:35:40.000000 pephubclient-0.4.2/pephubclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-16 18:35:40.000000 pephubclient-0.4.2/pephubclient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:35:40.456804 pephubclient-0.4.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-16 18:35:26.000000 pephubclient-0.4.2/requirements/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-16 18:35:26.000000 pephubclient-0.4.2/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 18:35:40.460804 pephubclient-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-16 18:35:26.000000 pephubclient-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:35:40.456804 pephubclient-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-16 18:35:26.000000 pephubclient-0.4.2/tests/test_manual.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17534 2024-04-16 18:35:26.000000 pephubclient-0.4.2/tests/test_pephubclient.py
```

### Comparing `pephubclient-0.4.1/LICENSE.txt` & `pephubclient-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pephubclient-0.4.1/PKG-INFO` & `pephubclient-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pephubclient
-Version: 0.4.1
+Version: 0.4.2
 Summary: PEPhub command line interface.
 Home-page: https://github.com/databio/pephubclient/
 Author: Oleksandr Khoroshevskyi, Rafal Stepien
 Author-email: khorosh@virginia.edu
 License: BSD2
 Keywords: project,bioinformatics,metadata
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pephubclient Version: 0.4.1 Summary: PEPhub command
+Metadata-Version: 2.1 Name: pephubclient Version: 0.4.2 Summary: PEPhub command
 line interface. Home-page: https://github.com/databio/pephubclient/ Author:
 Oleksandr Khoroshevskyi, Rafal Stepien Author-email: khorosh@virginia.edu
 License: BSD2 Keywords: project,bioinformatics,metadata Classifier: Development
 Status :: 3 - Alpha Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
```

### Comparing `pephubclient-0.4.1/README.md` & `pephubclient-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pephubclient-0.4.1/pephubclient/__init__.py` & `pephubclient-0.4.2/pephubclient/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pephubclient.pephubclient import PEPHubClient
 from pephubclient.helpers import is_registry_path, save_pep
 import logging
 import coloredlogs
 
 __app_name__ = "pephubclient"
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 __author__ = "Oleksandr Khoroshevskyi, Rafal Stepien"
 
 
 __all__ = [
     "PEPHubClient",
     __app_name__,
     __author__,
```

### Comparing `pephubclient-0.4.1/pephubclient/cli.py` & `pephubclient-0.4.2/pephubclient/cli.py`

 * *Files identical despite different names*

### Comparing `pephubclient-0.4.1/pephubclient/constants.py` & `pephubclient-0.4.2/pephubclient/constants.py`

 * *Files identical despite different names*

### Comparing `pephubclient-0.4.1/pephubclient/exceptions.py` & `pephubclient-0.4.2/pephubclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `pephubclient-0.4.1/pephubclient/files_manager.py` & `pephubclient-0.4.2/pephubclient/files_manager.py`

 * *Files identical despite different names*

### Comparing `pephubclient-0.4.1/pephubclient/helpers.py` & `pephubclient-0.4.2/pephubclient/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     @staticmethod
     def send_request(
         method: str,
         url: str,
         headers: Optional[dict] = None,
         cookies: Optional[dict] = None,
         params: Optional[dict] = None,
-        json: Optional[dict] = None,
+        json: Optional[Union[dict, list]] = None,
     ) -> requests.Response:
         request_return = requests.request(
             method=method,
             url=url,
             verify=False,
             cookies=cookies,
             headers=headers,
```

### Comparing `pephubclient-0.4.1/pephubclient/models.py` & `pephubclient-0.4.2/pephubclient/models.py`

 * *Files identical despite different names*

### Comparing `pephubclient-0.4.1/pephubclient/modules/sample.py` & `pephubclient-0.4.2/pephubclient/modules/sample.py`

 * *Files identical despite different names*

### Comparing `pephubclient-0.4.1/pephubclient/modules/view.py` & `pephubclient-0.4.2/pephubclient/modules/view.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,35 +67,44 @@
 
     def create(
         self,
         namespace: str,
         name: str,
         tag: str,
         view_name: str,
+        description: str = None,
         sample_list: list = None,
+        no_fail: bool = False,
     ):
         """
         Create view in project in PEPhub.
 
         :param namespace: namespace of project
         :param name: name of project
         :param tag: tag of project
+        :param description: description of the view
         :param view_name: name of the view
         :param sample_list: list of sample names
+        :param no_fail: whether to raise an error if view was not added to the project
         """
+
+        if not sample_list or not isinstance(sample_list, list):
+            raise ValueError("Sample list must be a list of sample names.")
+
         url = self._build_view_request_url(
             namespace=namespace, name=name, view_name=view_name
         )
 
         url = url + self.parse_query_param(pep_variables={"tag": tag})
 
         response = self.send_request(
             method="POST",
             url=url,
             headers=self.parse_header(self.__jwt_data),
+            params={"description": description, "no_fail": no_fail},
             json=sample_list,
         )
         if response.status_code == ResponseStatusCodes.ACCEPTED:
             _LOGGER.info(
                 f"View '{view_name}' created in project '{namespace}/{name}:{tag}' successfully."
             )
             return None
```

### Comparing `pephubclient-0.4.1/pephubclient/pephub_oauth/exceptions.py` & `pephubclient-0.4.2/pephubclient/pephub_oauth/exceptions.py`

 * *Files identical despite different names*

### Comparing `pephubclient-0.4.1/pephubclient/pephub_oauth/pephub_oauth.py` & `pephubclient-0.4.2/pephubclient/pephub_oauth/pephub_oauth.py`

 * *Files identical despite different names*

### Comparing `pephubclient-0.4.1/pephubclient/pephubclient.py` & `pephubclient-0.4.2/pephubclient/pephubclient.py`

 * *Files identical despite different names*

### Comparing `pephubclient-0.4.1/pephubclient.egg-info/PKG-INFO` & `pephubclient-0.4.2/pephubclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pephubclient
-Version: 0.4.1
+Version: 0.4.2
 Summary: PEPhub command line interface.
 Home-page: https://github.com/databio/pephubclient/
 Author: Oleksandr Khoroshevskyi, Rafal Stepien
 Author-email: khorosh@virginia.edu
 License: BSD2
 Keywords: project,bioinformatics,metadata
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pephubclient Version: 0.4.1 Summary: PEPhub command
+Metadata-Version: 2.1 Name: pephubclient Version: 0.4.2 Summary: PEPhub command
 line interface. Home-page: https://github.com/databio/pephubclient/ Author:
 Oleksandr Khoroshevskyi, Rafal Stepien Author-email: khorosh@virginia.edu
 License: BSD2 Keywords: project,bioinformatics,metadata Classifier: Development
 Status :: 3 - Alpha Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
```

### Comparing `pephubclient-0.4.1/pephubclient.egg-info/SOURCES.txt` & `pephubclient-0.4.2/pephubclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pephubclient-0.4.1/setup.py` & `pephubclient-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `pephubclient-0.4.1/tests/test_manual.py` & `pephubclient-0.4.2/tests/test_manual.py`

 * *Files identical despite different names*

### Comparing `pephubclient-0.4.1/tests/test_pephubclient.py` & `pephubclient-0.4.2/tests/test_pephubclient.py`

 * *Files identical despite different names*

