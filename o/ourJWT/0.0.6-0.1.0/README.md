# Comparing `tmp/ourJWT-0.0.6.tar.gz` & `tmp/ourJWT-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourJWT-0.0.6.tar", last modified: Tue Apr 16 13:26:00 2024, max compression
+gzip compressed data, was "ourJWT-0.1.0.tar", last modified: Tue Apr 16 13:53:24 2024, max compression
```

## Comparing `ourJWT-0.0.6.tar` & `ourJWT-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 gd-harco (102195) 2022_lyon  (4222)        0 2024-04-16 13:26:00.086230 ourJWT-0.0.6/
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      258 2024-04-16 13:26:00.086230 ourJWT-0.0.6/PKG-INFO
-drwxr-xr-x   0 gd-harco (102195) 2022_lyon  (4222)        0 2024-04-16 13:26:00.086230 ourJWT-0.0.6/ourJWT/
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)     3319 2024-04-16 13:25:57.000000 ourJWT-0.0.6/ourJWT/OUR_class.py
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      374 2024-04-16 08:08:01.000000 ourJWT-0.0.6/ourJWT/OUR_exception.py
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      153 2024-04-16 08:08:01.000000 ourJWT-0.0.6/ourJWT/__init__.py
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      850 2024-04-16 13:24:45.000000 ourJWT-0.0.6/ourJWT/decorators.py
-drwxr-xr-x   0 gd-harco (102195) 2022_lyon  (4222)        0 2024-04-16 13:26:00.086230 ourJWT-0.0.6/ourJWT.egg-info/
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      258 2024-04-16 13:26:00.000000 ourJWT-0.0.6/ourJWT.egg-info/PKG-INFO
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      241 2024-04-16 13:26:00.000000 ourJWT-0.0.6/ourJWT.egg-info/SOURCES.txt
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)        1 2024-04-16 13:26:00.000000 ourJWT-0.0.6/ourJWT.egg-info/dependency_links.txt
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      134 2024-04-16 13:26:00.000000 ourJWT-0.0.6/ourJWT.egg-info/requires.txt
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)        7 2024-04-16 13:26:00.000000 ourJWT-0.0.6/ourJWT.egg-info/top_level.txt
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)       38 2024-04-16 13:26:00.086230 ourJWT-0.0.6/setup.cfg
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      599 2024-04-16 12:59:14.000000 ourJWT-0.0.6/setup.py
+drwxr-xr-x   0 gd-harco (102195) 2022_lyon  (4222)        0 2024-04-16 13:53:24.094298 ourJWT-0.1.0/
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      258 2024-04-16 13:53:24.094298 ourJWT-0.1.0/PKG-INFO
+drwxr-xr-x   0 gd-harco (102195) 2022_lyon  (4222)        0 2024-04-16 13:53:24.094298 ourJWT-0.1.0/ourJWT/
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)     3327 2024-04-16 13:50:18.000000 ourJWT-0.1.0/ourJWT/OUR_class.py
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      374 2024-04-16 08:08:01.000000 ourJWT-0.1.0/ourJWT/OUR_exception.py
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      153 2024-04-16 08:08:01.000000 ourJWT-0.1.0/ourJWT/__init__.py
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      850 2024-04-16 13:50:22.000000 ourJWT-0.1.0/ourJWT/decorators.py
+drwxr-xr-x   0 gd-harco (102195) 2022_lyon  (4222)        0 2024-04-16 13:53:24.094298 ourJWT-0.1.0/ourJWT.egg-info/
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      258 2024-04-16 13:53:24.000000 ourJWT-0.1.0/ourJWT.egg-info/PKG-INFO
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      241 2024-04-16 13:53:24.000000 ourJWT-0.1.0/ourJWT.egg-info/SOURCES.txt
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)        1 2024-04-16 13:53:24.000000 ourJWT-0.1.0/ourJWT.egg-info/dependency_links.txt
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      134 2024-04-16 13:53:24.000000 ourJWT-0.1.0/ourJWT.egg-info/requires.txt
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)        7 2024-04-16 13:53:24.000000 ourJWT-0.1.0/ourJWT.egg-info/top_level.txt
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)       38 2024-04-16 13:53:24.094298 ourJWT-0.1.0/setup.cfg
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      599 2024-04-16 13:53:19.000000 ourJWT-0.1.0/setup.py
```

### Comparing `ourJWT-0.0.6/ourJWT/OUR_class.py` & `ourJWT-0.1.0/ourJWT/OUR_class.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 
 class Decoder:
     pub_key: str
 
     def __init__(self, pub_key):
         if pub_key is None:
              raise OUR_exception.NoKey
-        self.pub_key = pub_key
+        Decoder.pub_key = pub_key
 
 
-
-    def decode(self, to_decode, check_date: bool=True):
+    @staticmethod
+    def decode(to_decode, check_date: bool=True):
         """
         decode the given JWT into a dict.
 
         Args:
             to_decode (str): The JWT to be decoded.
 
         Raises:
@@ -29,36 +29,36 @@
             OUR_exception.ExpiredToken: if the token is expired
 
         Returns:
             dict: The decoded JWT.
         """
         try:
             token = jwt.decode(jwt=to_decode,
-                                key=self.pub_key,
+                                key=Decoder.pub_key,
                                 algorithms=["RS256"],
                                 issuer=good_iss,
                                 options={"verify_exp": check_date})
         except(jwt.DecodeError,
                 jwt.InvalidIssuerError,
                 jwt.InvalidSignatureError):
             raise OUR_exception.RefusedToken()
         except jwt.ExpiredSignatureError:
             raise OUR_exception.ExpiredToken()
         if token["sub"] != "auth" and token["sub"] != "refresh":
             raise OUR_exception.BadSubject
         return token
-    
-    def check_auth(function):
+
+    def check_auth():
         def decorator(function):
             def wrapper(request: HttpRequest):
                 auth: str = request.COOKIES.get("auth_token", None)
                 if auth is None:
                     return response.HttpResponseBadRequest(reason="No auth cookie sent")
                 try:
-                    auth_decoded = self.decode(auth)
+                    auth_decoded = Decoder.decode(auth)
                 except (OUR_exception.BadSubject,
                         OUR_exception.RefusedToken,
                         OUR_exception.ExpiredToken):
                     return HttpResponseUnauthorized(reason="Bad auth token")
                 return function(request, token=auth_decoded)
             return wrapper
         return decorator
```

### Comparing `ourJWT-0.0.6/ourJWT/decorators.py` & `ourJWT-0.1.0/ourJWT/decorators.py`

 * *Files identical despite different names*

### Comparing `ourJWT-0.0.6/setup.py` & `ourJWT-0.1.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     include_package_data=True,
     name='ourJWT',
-    version='0.0.6',
+    version='0.1.0',
     description='repackaging of pyJWT package, adding fonction required for our_transcendence',
     author="gd-harco",
     author_email="gd-harco@student.42lyon.fr",
     py_modules=['ourJWT'],
     packages=find_packages(),
     install_requires=[
         'asgiref==3.8.1',
```

