# Comparing `tmp/pysignalclirestapi-0.3.8.tar.gz` & `tmp/pysignalclirestapi-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pysignalclirestapi-0.3.8.tar", last modified: Sat May 16 13:47:13 2020, max compression
+gzip compressed data, was "dist/pysignalclirestapi-0.3.9.tar", last modified: Sat May 16 18:42:48 2020, max compression
```

## Comparing `pysignalclirestapi-0.3.8.tar` & `pysignalclirestapi-0.3.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr--   0 bernhard  (1000) plugdev     (46)        0 2020-05-16 13:47:13.000000 pysignalclirestapi-0.3.8/
--rwxrwxr--   0 bernhard  (1000) plugdev     (46)      606 2020-05-16 13:47:13.000000 pysignalclirestapi-0.3.8/PKG-INFO
-drwxrwxr--   0 bernhard  (1000) plugdev     (46)        0 2020-05-16 13:47:13.000000 pysignalclirestapi-0.3.8/pysignalclirestapi/
--rwxrwxr--   0 bernhard  (1000) plugdev     (46)     4695 2020-05-16 13:45:28.000000 pysignalclirestapi-0.3.8/pysignalclirestapi/api.py
--rwxrwxr--   0 bernhard  (1000) plugdev     (46)       75 2020-04-26 19:42:49.000000 pysignalclirestapi-0.3.8/pysignalclirestapi/__init__.py
-drwxrwxr--   0 bernhard  (1000) plugdev     (46)        0 2020-05-16 13:47:13.000000 pysignalclirestapi-0.3.8/pysignalclirestapi.egg-info/
--rwxrwxr--   0 bernhard  (1000) plugdev     (46)        1 2020-05-16 13:47:13.000000 pysignalclirestapi-0.3.8/pysignalclirestapi.egg-info/dependency_links.txt
--rwxrwxr--   0 bernhard  (1000) plugdev     (46)      606 2020-05-16 13:47:13.000000 pysignalclirestapi-0.3.8/pysignalclirestapi.egg-info/PKG-INFO
--rwxrwxr--   0 bernhard  (1000) plugdev     (46)      253 2020-05-16 13:47:13.000000 pysignalclirestapi-0.3.8/pysignalclirestapi.egg-info/SOURCES.txt
--rwxrwxr--   0 bernhard  (1000) plugdev     (46)       19 2020-05-16 13:47:13.000000 pysignalclirestapi-0.3.8/pysignalclirestapi.egg-info/top_level.txt
--rwxrwxr--   0 bernhard  (1000) plugdev     (46)      101 2019-11-10 18:41:32.000000 pysignalclirestapi-0.3.8/README.md
--rwxrwxr--   0 bernhard  (1000) plugdev     (46)       79 2020-05-16 13:47:13.000000 pysignalclirestapi-0.3.8/setup.cfg
--rwxrwxr--   0 bernhard  (1000) plugdev     (46)      687 2020-05-16 13:44:50.000000 pysignalclirestapi-0.3.8/setup.py
+drwxrwxr--   0 bernhard  (1000) plugdev     (46)        0 2020-05-16 18:42:48.000000 pysignalclirestapi-0.3.9/
+-rwxrwxr--   0 bernhard  (1000) plugdev     (46)      606 2020-05-16 18:42:48.000000 pysignalclirestapi-0.3.9/PKG-INFO
+drwxrwxr--   0 bernhard  (1000) plugdev     (46)        0 2020-05-16 18:42:48.000000 pysignalclirestapi-0.3.9/pysignalclirestapi/
+-rwxrwxr--   0 bernhard  (1000) plugdev     (46)     4709 2020-05-16 18:42:13.000000 pysignalclirestapi-0.3.9/pysignalclirestapi/api.py
+-rwxrwxr--   0 bernhard  (1000) plugdev     (46)       75 2020-04-26 19:42:49.000000 pysignalclirestapi-0.3.9/pysignalclirestapi/__init__.py
+drwxrwxr--   0 bernhard  (1000) plugdev     (46)        0 2020-05-16 18:42:48.000000 pysignalclirestapi-0.3.9/pysignalclirestapi.egg-info/
+-rwxrwxr--   0 bernhard  (1000) plugdev     (46)        1 2020-05-16 18:42:48.000000 pysignalclirestapi-0.3.9/pysignalclirestapi.egg-info/dependency_links.txt
+-rwxrwxr--   0 bernhard  (1000) plugdev     (46)      606 2020-05-16 18:42:48.000000 pysignalclirestapi-0.3.9/pysignalclirestapi.egg-info/PKG-INFO
+-rwxrwxr--   0 bernhard  (1000) plugdev     (46)      253 2020-05-16 18:42:48.000000 pysignalclirestapi-0.3.9/pysignalclirestapi.egg-info/SOURCES.txt
+-rwxrwxr--   0 bernhard  (1000) plugdev     (46)       19 2020-05-16 18:42:48.000000 pysignalclirestapi-0.3.9/pysignalclirestapi.egg-info/top_level.txt
+-rwxrwxr--   0 bernhard  (1000) plugdev     (46)      101 2019-11-10 18:41:32.000000 pysignalclirestapi-0.3.9/README.md
+-rwxrwxr--   0 bernhard  (1000) plugdev     (46)       79 2020-05-16 18:42:48.000000 pysignalclirestapi-0.3.9/setup.cfg
+-rwxrwxr--   0 bernhard  (1000) plugdev     (46)      687 2020-05-16 18:42:44.000000 pysignalclirestapi-0.3.9/setup.py
```

### Comparing `pysignalclirestapi-0.3.8/PKG-INFO` & `pysignalclirestapi-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysignalclirestapi
-Version: 0.3.8
+Version: 0.3.9
 Summary: Small python library for the Signal Cli REST API
 Home-page: https://github.com/bbernhard/pysignalclirestapi
 Author: Bernhard B.
 Author-email: bernhard@liftingcoder.com
 License: UNKNOWN
 Description: Small python library for the [Signal Cli REST API](https://github.com/bbernhard/signal-cli-rest-api)
```

### Comparing `pysignalclirestapi-0.3.8/pysignalclirestapi/api.py` & `pysignalclirestapi-0.3.9/pysignalclirestapi/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,20 +95,20 @@
 
         try:
             if "v2" in api_versions:
                 base64_attachments = []
                 if filenames is not None: 
                     for filename in filenames:
                         with open(filename, "rb") as ofile:
-                            base64_attachments.append(str(base64.b64encode(ofile.read()), "utf-8"))
+                            base64_attachments.append(str(base64.b64encode(ofile.read())).encode("utf-8"))
                 data["base64_attachments"] = base64_attachments
             else: # fall back to api version 1 to stay downwards compatible
                 if filenames is not None and len(filenames) == 1:
                     with open(filenames[0], "rb") as ofile:
-                        data["base64_attachment"] = str(base64.b64encode(ofile.read()), "utf-8")
+                        data["base64_attachment"] = str(base64.b64encode(ofile.read())).encode("utf-8")
             
             resp = requests.post(url, json=data)
             if resp.status_code != 201:
                 json_resp = resp.json()
                 if "error" in json_resp:
                     raise SignalCliRestApiError(json_resp["error"])
                 raise SignalCliRestApiError("Unknown error while sending signal message")
```

### Comparing `pysignalclirestapi-0.3.8/pysignalclirestapi.egg-info/PKG-INFO` & `pysignalclirestapi-0.3.9/pysignalclirestapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysignalclirestapi
-Version: 0.3.8
+Version: 0.3.9
 Summary: Small python library for the Signal Cli REST API
 Home-page: https://github.com/bbernhard/pysignalclirestapi
 Author: Bernhard B.
 Author-email: bernhard@liftingcoder.com
 License: UNKNOWN
 Description: Small python library for the [Signal Cli REST API](https://github.com/bbernhard/signal-cli-rest-api)
```

### Comparing `pysignalclirestapi-0.3.8/setup.py` & `pysignalclirestapi-0.3.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pysignalclirestapi",
-    version="0.3.8",
+    version="0.3.9",
     author="Bernhard B.",
     author_email="bernhard@liftingcoder.com",
     description="Small python library for the Signal Cli REST API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bbernhard/pysignalclirestapi",
     packages=setuptools.find_packages(),
```

