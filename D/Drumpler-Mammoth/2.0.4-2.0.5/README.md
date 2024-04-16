# Comparing `tmp/drumpler_mammoth-2.0.4.tar.gz` & `tmp/drumpler_mammoth-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drumpler_mammoth-2.0.4.tar", last modified: Tue Apr 16 20:44:15 2024, max compression
+gzip compressed data, was "drumpler_mammoth-2.0.5.tar", last modified: Tue Apr 16 20:51:39 2024, max compression
```

## Comparing `drumpler_mammoth-2.0.4.tar` & `drumpler_mammoth-2.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 20:44:15.418168 drumpler_mammoth-2.0.4/
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 20:44:15.416887 drumpler_mammoth-2.0.4/Drumpler_Mammoth.egg-info/
--rw-r--r--   0 Karel      (503) staff       (20)     4054 2024-04-16 20:44:15.000000 drumpler_mammoth-2.0.4/Drumpler_Mammoth.egg-info/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)      342 2024-04-16 20:44:15.000000 drumpler_mammoth-2.0.4/Drumpler_Mammoth.egg-info/SOURCES.txt
--rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-16 20:44:15.000000 drumpler_mammoth-2.0.4/Drumpler_Mammoth.egg-info/dependency_links.txt
--rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-16 20:44:15.000000 drumpler_mammoth-2.0.4/Drumpler_Mammoth.egg-info/requires.txt
--rw-r--r--   0 Karel      (503) staff       (20)       17 2024-04-16 20:44:15.000000 drumpler_mammoth-2.0.4/Drumpler_Mammoth.egg-info/top_level.txt
--rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 drumpler_mammoth-2.0.4/LICENSE
--rw-r--r--   0 Karel      (503) staff       (20)     4054 2024-04-16 20:44:15.417477 drumpler_mammoth-2.0.4/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 drumpler_mammoth-2.0.4/README.md
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 20:44:15.416234 drumpler_mammoth-2.0.4/drumpler-mammoth/
--rw-r--r--   0 Karel      (503) staff       (20)       30 2024-04-16 20:09:55.000000 drumpler_mammoth-2.0.4/drumpler-mammoth/__init__.py
--rw-r--r--   0 Karel      (503) staff       (20)      301 2024-04-16 20:08:33.000000 drumpler_mammoth-2.0.4/drumpler-mammoth/config.py
--rw-r--r--   0 Karel      (503) staff       (20)     3147 2024-04-16 18:54:35.000000 drumpler_mammoth-2.0.4/drumpler-mammoth/http_request.py
--rw-r--r--   0 Karel      (503) staff       (20)     3427 2024-04-16 20:09:39.000000 drumpler_mammoth-2.0.4/drumpler-mammoth/mammoth.py
--rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-16 20:44:15.418360 drumpler_mammoth-2.0.4/setup.cfg
--rw-r--r--   0 Karel      (503) staff       (20)      700 2024-04-16 20:43:29.000000 drumpler_mammoth-2.0.4/setup.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 20:51:39.979610 drumpler_mammoth-2.0.5/
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 20:51:39.978076 drumpler_mammoth-2.0.5/Drumpler_Mammoth.egg-info/
+-rw-r--r--   0 Karel      (503) staff       (20)     4054 2024-04-16 20:51:39.000000 drumpler_mammoth-2.0.5/Drumpler_Mammoth.egg-info/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)      342 2024-04-16 20:51:39.000000 drumpler_mammoth-2.0.5/Drumpler_Mammoth.egg-info/SOURCES.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-16 20:51:39.000000 drumpler_mammoth-2.0.5/Drumpler_Mammoth.egg-info/dependency_links.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-16 20:51:39.000000 drumpler_mammoth-2.0.5/Drumpler_Mammoth.egg-info/requires.txt
+-rw-r--r--   0 Karel      (503) staff       (20)       17 2024-04-16 20:51:39.000000 drumpler_mammoth-2.0.5/Drumpler_Mammoth.egg-info/top_level.txt
+-rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 drumpler_mammoth-2.0.5/LICENSE
+-rw-r--r--   0 Karel      (503) staff       (20)     4054 2024-04-16 20:51:39.978672 drumpler_mammoth-2.0.5/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 drumpler_mammoth-2.0.5/README.md
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-16 20:51:39.977405 drumpler_mammoth-2.0.5/drumpler-mammoth/
+-rw-r--r--   0 Karel      (503) staff       (20)       30 2024-04-16 20:09:55.000000 drumpler_mammoth-2.0.5/drumpler-mammoth/__init__.py
+-rw-r--r--   0 Karel      (503) staff       (20)      301 2024-04-16 20:08:33.000000 drumpler_mammoth-2.0.5/drumpler-mammoth/config.py
+-rw-r--r--   0 Karel      (503) staff       (20)     3133 2024-04-16 20:51:21.000000 drumpler_mammoth-2.0.5/drumpler-mammoth/http_request.py
+-rw-r--r--   0 Karel      (503) staff       (20)     3427 2024-04-16 20:09:39.000000 drumpler_mammoth-2.0.5/drumpler-mammoth/mammoth.py
+-rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-16 20:51:39.979751 drumpler_mammoth-2.0.5/setup.cfg
+-rw-r--r--   0 Karel      (503) staff       (20)      700 2024-04-16 20:51:26.000000 drumpler_mammoth-2.0.5/setup.py
```

### Comparing `drumpler_mammoth-2.0.4/Drumpler_Mammoth.egg-info/PKG-INFO` & `drumpler_mammoth-2.0.5/Drumpler_Mammoth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler_Mammoth
-Version: 2.0.4
+Version: 2.0.5
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler-Mammoth
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `drumpler_mammoth-2.0.4/LICENSE` & `drumpler_mammoth-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `drumpler_mammoth-2.0.4/PKG-INFO` & `drumpler_mammoth-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler_Mammoth
-Version: 2.0.4
+Version: 2.0.5
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler-Mammoth
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `drumpler_mammoth-2.0.4/README.md` & `drumpler_mammoth-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `drumpler_mammoth-2.0.4/drumpler-mammoth/http_request.py` & `drumpler_mammoth-2.0.5/drumpler-mammoth/http_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import requests
 import json
-from .constants import DRUMPLER_URL, AUTHORIZATION_KEY
+from .config import Config
 
 class HttpRequest:
     def __init__(self, id, timestamp, source_ip, user_agent, method, request_url, request_raw, custom_value, is_handled):
         self._id = id
         self._timestamp = timestamp
         self._source_ip = source_ip
         self._user_agent = user_agent
@@ -13,23 +13,23 @@
         self._request_raw = request_raw
         self._request_json = json.loads(request_raw)
         self.custom_value = custom_value
         self._is_handled = is_handled
 
     def mark_as_handled(self):
         headers = {
-            'Authorization': f'Bearer {AUTHORIZATION_KEY}',
+            'Authorization': f'Bearer {Config.AUTHORIZATION_KEY}',
             'Content-Type': 'application/json'  # Indicate JSON payload
         }
         payload = {
             'is_handled': 1  # Assuming setting `is_handled` to 1 marks it as handled
         }
 
         try:
-            response = requests.put(f"{DRUMPLER_URL}/request/{self.id}", json=payload, headers=headers)
+            response = requests.put(f"{Config.DRUMPLER_URL}/request/{self.id}", json=payload, headers=headers)
             if response.status_code == 200:
                 return f"Request {self.id} marked as handled successfully."
             else:
                 # Attempt to extract and print a more descriptive error message
                 try:
                     error_message = response.json().get('message', 'No error message provided.')
                 except ValueError:  # If response is not in JSON format
```

### Comparing `drumpler_mammoth-2.0.4/drumpler-mammoth/mammoth.py` & `drumpler_mammoth-2.0.5/drumpler-mammoth/mammoth.py`

 * *Files identical despite different names*

### Comparing `drumpler_mammoth-2.0.4/setup.py` & `drumpler_mammoth-2.0.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Drumpler_Mammoth',
-    version='2.0.4',
+    version='2.0.5',
     author='Karel Tutsu',
     author_email='karel.tutsu@gmail.com',
     description='Framework for rapidly developing a restful API that requires post processing',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/KarelOmab/Drumpler-Mammoth',
     packages=find_packages(),
```

