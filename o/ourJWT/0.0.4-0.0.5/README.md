# Comparing `tmp/ourJWT-0.0.4.tar.gz` & `tmp/ourJWT-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourJWT-0.0.4.tar", last modified: Sat Apr 13 09:37:12 2024, max compression
+gzip compressed data, was "ourJWT-0.0.5.tar", last modified: Tue Apr 16 08:55:41 2024, max compression
```

## Comparing `ourJWT-0.0.4.tar` & `ourJWT-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 gd-harco  (1000) gd-harco  (1000)        0 2024-04-13 09:37:12.390422 ourJWT-0.0.4/
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      448 2024-04-13 09:37:12.390422 ourJWT-0.0.4/PKG-INFO
-drwxrwxr-x   0 gd-harco  (1000) gd-harco  (1000)        0 2024-04-13 09:37:12.386422 ourJWT-0.0.4/ourJWT/
--rw-rw-r--   0 gd-harco  (1000) gd-harco  (1000)     2462 2024-04-13 07:58:22.000000 ourJWT-0.0.4/ourJWT/OUR_class.py
--rw-rw-r--   0 gd-harco  (1000) gd-harco  (1000)      374 2024-04-13 07:58:22.000000 ourJWT-0.0.4/ourJWT/OUR_exception.py
--rw-rw-r--   0 gd-harco  (1000) gd-harco  (1000)      153 2024-04-13 07:58:22.000000 ourJWT-0.0.4/ourJWT/__init__.py
--rw-rw-r--   0 gd-harco  (1000) gd-harco  (1000)     1195 2024-04-13 07:58:22.000000 ourJWT-0.0.4/ourJWT/decorators.py
-drwxrwxr-x   0 gd-harco  (1000) gd-harco  (1000)        0 2024-04-13 09:37:12.386422 ourJWT-0.0.4/ourJWT.egg-info/
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      448 2024-04-13 09:37:12.000000 ourJWT-0.0.4/ourJWT.egg-info/PKG-INFO
--rw-rw-r--   0 gd-harco  (1000) gd-harco  (1000)      241 2024-04-13 09:37:12.000000 ourJWT-0.0.4/ourJWT.egg-info/SOURCES.txt
--rw-rw-r--   0 gd-harco  (1000) gd-harco  (1000)        1 2024-04-13 09:37:12.000000 ourJWT-0.0.4/ourJWT.egg-info/dependency_links.txt
--rw-rw-r--   0 gd-harco  (1000) gd-harco  (1000)      134 2024-04-13 09:37:12.000000 ourJWT-0.0.4/ourJWT.egg-info/requires.txt
--rw-rw-r--   0 gd-harco  (1000) gd-harco  (1000)        7 2024-04-13 09:37:12.000000 ourJWT-0.0.4/ourJWT.egg-info/top_level.txt
--rw-rw-r--   0 gd-harco  (1000) gd-harco  (1000)       38 2024-04-13 09:37:12.390422 ourJWT-0.0.4/setup.cfg
--rw-rw-r--   0 gd-harco  (1000) gd-harco  (1000)      599 2024-04-13 09:36:58.000000 ourJWT-0.0.4/setup.py
+drwxr-xr-x   0 gd-harco (102195) 2022_lyon  (4222)        0 2024-04-16 08:55:41.426687 ourJWT-0.0.5/
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      258 2024-04-16 08:55:41.426687 ourJWT-0.0.5/PKG-INFO
+drwxr-xr-x   0 gd-harco (102195) 2022_lyon  (4222)        0 2024-04-16 08:55:41.422687 ourJWT-0.0.5/ourJWT/
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)     2456 2024-04-16 08:55:38.000000 ourJWT-0.0.5/ourJWT/OUR_class.py
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      374 2024-04-16 08:08:01.000000 ourJWT-0.0.5/ourJWT/OUR_exception.py
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      153 2024-04-16 08:08:01.000000 ourJWT-0.0.5/ourJWT/__init__.py
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)     1195 2024-04-16 08:08:01.000000 ourJWT-0.0.5/ourJWT/decorators.py
+drwxr-xr-x   0 gd-harco (102195) 2022_lyon  (4222)        0 2024-04-16 08:55:41.422687 ourJWT-0.0.5/ourJWT.egg-info/
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      258 2024-04-16 08:55:41.000000 ourJWT-0.0.5/ourJWT.egg-info/PKG-INFO
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      241 2024-04-16 08:55:41.000000 ourJWT-0.0.5/ourJWT.egg-info/SOURCES.txt
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)        1 2024-04-16 08:55:41.000000 ourJWT-0.0.5/ourJWT.egg-info/dependency_links.txt
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      134 2024-04-16 08:55:41.000000 ourJWT-0.0.5/ourJWT.egg-info/requires.txt
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)        7 2024-04-16 08:55:41.000000 ourJWT-0.0.5/ourJWT.egg-info/top_level.txt
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)       38 2024-04-16 08:55:41.426687 ourJWT-0.0.5/setup.cfg
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      599 2024-04-16 08:55:07.000000 ourJWT-0.0.5/setup.py
```

### Comparing `ourJWT-0.0.4/ourJWT/OUR_class.py` & `ourJWT-0.0.5/ourJWT/OUR_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,17 +69,17 @@
             TypeError: If the payload is not a dictionary.
 
         Returns:
             str: The encoded JWT.
         """
         if type != "refresh" and type != "auth":
             raise OUR_exception.BadSubject()
-        if Encoder.private_key is None:
+        if self.private_key is None:
             raise OUR_exception.NoKey()
         if not isinstance(to_encode, dict):
             raise TypeError("Payload not a dict")
         to_encode["iss"] = good_iss
         to_encode["sub"] = type
         encoded = jwt.encode(payload=to_encode,
-                             key=Encoder.private_key,
+                             key=self.private_key,
                              algorithm="RS256")
         return encoded
```

### Comparing `ourJWT-0.0.4/ourJWT/decorators.py` & `ourJWT-0.0.5/ourJWT/decorators.py`

 * *Files identical despite different names*

### Comparing `ourJWT-0.0.4/setup.py` & `ourJWT-0.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     include_package_data=True,
     name='ourJWT',
-    version='0.0.4',
+    version='0.0.5',
     description='repackaging of pyJWT package, adding fonction required for our_transcendence',
     author="gd-harco",
     author_email="gd-harco@student.42lyon.fr",
     py_modules=['ourJWT'],
     packages=find_packages(),
     install_requires=[
         'asgiref==3.8.1',
```

