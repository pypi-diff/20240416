# Comparing `tmp/vt-py-0.8.0.tar.gz` & `tmp/vt-py-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vt-py-0.8.0.tar", last modified: Tue Nov  9 07:53:15 2021, max compression
+gzip compressed data, was "vt-py-0.9.0.tar", last modified: Tue Nov 30 13:57:02 2021, max compression
```

## Comparing `vt-py-0.8.0.tar` & `vt-py-0.9.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-09 07:53:15.772691 vt-py-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-11-09 07:53:06.000000 vt-py-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1552 2021-11-09 07:53:15.772691 vt-py-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1092 2021-11-09 07:53:06.000000 vt-py-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       63 2021-11-09 07:53:15.776691 vt-py-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1608 2021-11-09 07:53:06.000000 vt-py-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-09 07:53:15.772691 vt-py-0.8.0/vt/
--rw-r--r--   0 runner    (1001) docker     (121)      771 2021-11-09 07:53:06.000000 vt-py-0.8.0/vt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24972 2021-11-09 07:53:06.000000 vt-py-0.8.0/vt/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      900 2021-11-09 07:53:06.000000 vt-py-0.8.0/vt/error.py
--rw-r--r--   0 runner    (1001) docker     (121)     5350 2021-11-09 07:53:06.000000 vt-py-0.8.0/vt/feed.py
--rw-r--r--   0 runner    (1001) docker     (121)     5364 2021-11-09 07:53:06.000000 vt-py-0.8.0/vt/iterator.py
--rw-r--r--   0 runner    (1001) docker     (121)     6346 2021-11-09 07:53:06.000000 vt-py-0.8.0/vt/object.py
--rw-r--r--   0 runner    (1001) docker     (121)      966 2021-11-09 07:53:06.000000 vt-py-0.8.0/vt/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-11-09 07:53:06.000000 vt-py-0.8.0/vt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-09 07:53:15.772691 vt-py-0.8.0/vt_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1552 2021-11-09 07:53:15.000000 vt-py-0.8.0/vt_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      285 2021-11-09 07:53:15.000000 vt-py-0.8.0/vt_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-09 07:53:15.000000 vt-py-0.8.0/vt_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       56 2021-11-09 07:53:15.000000 vt-py-0.8.0/vt_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        3 2021-11-09 07:53:15.000000 vt-py-0.8.0/vt_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 13:57:02.717573 vt-py-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-11-30 13:56:47.000000 vt-py-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1552 2021-11-30 13:57:02.717573 vt-py-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1092 2021-11-30 13:56:47.000000 vt-py-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2021-11-30 13:57:02.717573 vt-py-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1608 2021-11-30 13:56:47.000000 vt-py-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 13:57:02.717573 vt-py-0.9.0/vt/
+-rw-r--r--   0 runner    (1001) docker     (121)      771 2021-11-30 13:56:47.000000 vt-py-0.9.0/vt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28212 2021-11-30 13:56:47.000000 vt-py-0.9.0/vt/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      900 2021-11-30 13:56:47.000000 vt-py-0.9.0/vt/error.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5350 2021-11-30 13:56:47.000000 vt-py-0.9.0/vt/feed.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5364 2021-11-30 13:56:47.000000 vt-py-0.9.0/vt/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6604 2021-11-30 13:56:47.000000 vt-py-0.9.0/vt/object.py
+-rw-r--r--   0 runner    (1001) docker     (121)      966 2021-11-30 13:56:47.000000 vt-py-0.9.0/vt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2021-11-30 13:56:47.000000 vt-py-0.9.0/vt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 13:57:02.717573 vt-py-0.9.0/vt_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1552 2021-11-30 13:57:02.000000 vt-py-0.9.0/vt_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2021-11-30 13:57:02.000000 vt-py-0.9.0/vt_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-30 13:57:02.000000 vt-py-0.9.0/vt_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2021-11-30 13:57:02.000000 vt-py-0.9.0/vt_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2021-11-30 13:57:02.000000 vt-py-0.9.0/vt_py.egg-info/top_level.txt
```

### Comparing `vt-py-0.8.0/LICENSE` & `vt-py-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vt-py-0.8.0/PKG-INFO` & `vt-py-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vt-py
-Version: 0.8.0
+Version: 0.9.0
 Summary: The official Python client library for VirusTotal
 Home-page: https://github.com/VirusTotal/vt-py
 License: Apache 2
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `vt-py-0.8.0/README.md` & `vt-py-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `vt-py-0.8.0/setup.py` & `vt-py-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `vt-py-0.8.0/vt/__init__.py` & `vt-py-0.9.0/vt/__init__.py`

 * *Files identical despite different names*

### Comparing `vt-py-0.8.0/vt/client.py` & `vt-py-0.9.0/vt/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -660,7 +660,104 @@
   async def _wait_for_analysis_completion(self, analysis):
     while True:
       analysis = await self.get_object_async('/analyses/{}', analysis.id)
       if analysis.status == 'completed':
         break
       await asyncio.sleep(20)
     return analysis
+
+  def create_collection_from_raw_text(self, name, raw_text, **kwargs):
+    """Creates a collection in VirusTotal from raw text.
+
+    The collection's IoCs will be extracted from the given raw text.
+
+    Args:
+      name: Name of the collection.
+      raw: Raw text.
+      **kwargs: Other attributes that can be added to the collection,
+        like for example, the description.
+
+    Returns:
+      The new collection.
+
+    Raises:
+      ValueError: If the name is empty.
+      vt.error.APIError: If there are no IoCs in the raw text.
+    """
+    return make_sync(self.create_collection_from_raw_text_async(
+        name, raw_text, **kwargs))
+
+  async def create_collection_from_raw_text_async(
+      self, name, raw_text, **kwargs):
+    """Like :func:`create_collection_from_raw_text` but returns a coroutine."""
+    if not name:
+      raise ValueError('No name provided')
+    attributes = {'name': name}
+    attributes.update(kwargs)
+    payload = {
+        'attributes': attributes,
+        'type': 'collection',
+        'meta': {'raw': raw_text},
+        'id': '',
+    }
+    collection_obj = Object.from_dict(payload)
+    response = await self.post_object_async('/collections', obj=collection_obj)
+    return response
+
+  def create_collection_from_iocs(
+      self, name, files=None, urls=None, domains=None, ip_addresses=None,
+      **kwargs):
+    """Creates a collection in VirusTotal from lists of IoCs.
+
+    Args:
+      name: Name of the collection.
+      files: List of file hashes.
+      urls: List of URLs.
+      domains: List of domains.
+      ip_addresses: List of IP addresses.
+      **kwargs: Other attributes that can be added to the collection,
+        like for example, the description.
+
+    Returns:
+      The new collection.
+
+    Raises:
+      ValueError: If the name is empty or there are no IoCs to add to the
+        collection.
+      vt.error.APIError: If any of the IoCs provided are not valid.
+    """
+    return make_sync(self.create_collection_from_iocs_async(
+        name, files, urls, domains, ip_addresses, **kwargs))
+
+  async def create_collection_from_iocs_async(
+      self, name, files=None, urls=None, domains=None, ip_addresses=None,
+      **kwargs):
+    """Like :func:`create_collection_from_iocs` but returns a coroutine."""
+    if not name:
+      raise ValueError('No name provided')
+    attributes = {'name': name}
+    attributes.update(kwargs)
+    relationships = {}
+    if files:
+      relationships['files'] = {
+          'data': [{'type': 'file', 'id': h} for h in files]}
+    if urls:
+      relationships['urls'] = {
+          'data': [{'type': 'url', 'url': u} for u in urls]}
+    if domains:
+      relationships['domains'] = {
+          'data': [{'type': 'domain', 'id': d} for d in domains]}
+    if ip_addresses:
+      relationships['ip_addresses'] = {
+          'data': [{'type': 'ip_address', 'id': i} for i in ip_addresses]}
+    if not relationships:
+      raise ValueError('No IoCs provided')
+
+    payload = {
+        'attributes': attributes,
+        'type': 'collection',
+        'relationships': relationships,
+        'id': '',
+    }
+    collection_obj = Object.from_dict(payload)
+    response = await self.post_object_async('/collections', obj=collection_obj)
+    return response
```

### Comparing `vt-py-0.8.0/vt/error.py` & `vt-py-0.9.0/vt/error.py`

 * *Files identical despite different names*

### Comparing `vt-py-0.8.0/vt/feed.py` & `vt-py-0.9.0/vt/feed.py`

 * *Files identical despite different names*

### Comparing `vt-py-0.8.0/vt/iterator.py` & `vt-py-0.9.0/vt/iterator.py`

 * *Files identical despite different names*

### Comparing `vt-py-0.8.0/vt/object.py` & `vt-py-0.9.0/vt/object.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,17 @@
         "type": <object type>,
         "id": <object id>,
         "links": {
           "self": "https://www.virustotal.com/api/v3/<collection name>/<object id>"
         },
         "attributes": {
           ...
+        },
+        "meta": {
+          ...
         }
       }
 
     At least `type` and `id` are required to be present in the dictionary, if
     not, an exception is raised.
     """
     if not isinstance(obj_dict, dict):
@@ -101,14 +104,17 @@
 
     if 'context_attributes' in obj_dict:
       obj._context_attributes = obj_dict['context_attributes']
 
     if 'relationships' in obj_dict:
       obj._relationships = obj_dict['relationships']
 
+    if 'meta' in obj_dict:
+      obj._meta = obj_dict['meta']
+
     return obj
 
   def __init__(self, obj_type, obj_id=None, obj_attributes=None):
     """Initializes a VirusTotal API object."""
 
     if not isinstance(obj_attributes, (dict, type(None))):
       raise ValueError('Object attributes must be a dictionary')
@@ -169,14 +175,20 @@
 
   @property
   def relationships(self):
     if hasattr(self, '_relationships'):
       return self._relationships
     return {}
 
+  @property
+  def meta(self):
+    if hasattr(self, '_meta'):
+      return self._meta
+    return {}
+
   def get(self, attr_name, default=None):
     """Returns an attribute by name.
 
     If the attribute is not present in the object, it returns None
     or the value specified in the "default" argument.
 
     :param attr_name: Name of the attribute.
@@ -203,8 +215,11 @@
 
     if self.relationships:
       result['relationships'] = self.relationships
 
     if self.context_attributes:
       result['context_attributes'] = self.context_attributes
 
+    if self.meta:
+      result['meta'] = self.meta
+
     return result
```

### Comparing `vt-py-0.8.0/vt/utils.py` & `vt-py-0.9.0/vt/utils.py`

 * *Files identical despite different names*

### Comparing `vt-py-0.8.0/vt_py.egg-info/PKG-INFO` & `vt-py-0.9.0/vt_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vt-py
-Version: 0.8.0
+Version: 0.9.0
 Summary: The official Python client library for VirusTotal
 Home-page: https://github.com/VirusTotal/vt-py
 License: Apache 2
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

