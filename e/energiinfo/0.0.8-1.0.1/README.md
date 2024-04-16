# Comparing `tmp/energiinfo-0.0.8.tar.gz` & `tmp/energiinfo-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energiinfo-0.0.8.tar", last modified: Mon Mar 25 21:11:32 2024, max compression
+gzip compressed data, was "energiinfo-1.0.1.tar", last modified: Tue Apr 16 13:30:59 2024, max compression
```

## Comparing `energiinfo-0.0.8.tar` & `energiinfo-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 veulsan  (2037719458) 1135428931        0 2024-03-25 21:11:32.861171 energiinfo-0.0.8/
--rw-r--r--   0 veulsan  (2037719458) 1135428931    35149 2024-03-22 12:46:44.000000 energiinfo-0.0.8/LICENSE
--rw-r--r--   0 veulsan  (2037719458) 1135428931     1917 2024-03-25 21:11:32.860809 energiinfo-0.0.8/PKG-INFO
--rw-r--r--   0 veulsan  (2037719458) 1135428931     1359 2024-03-22 22:45:09.000000 energiinfo-0.0.8/README.md
--rw-r--r--   0 veulsan  (2037719458) 1135428931       87 2024-03-22 23:05:51.000000 energiinfo-0.0.8/pyproject.toml
--rw-r--r--   0 veulsan  (2037719458) 1135428931      685 2024-03-25 21:11:32.863020 energiinfo-0.0.8/setup.cfg
-drwxr-xr-x   0 veulsan  (2037719458) 1135428931        0 2024-03-25 21:11:32.591674 energiinfo-0.0.8/src/
-drwxr-xr-x   0 veulsan  (2037719458) 1135428931        0 2024-03-25 21:11:32.756911 energiinfo-0.0.8/src/energiinfo/
--rw-r--r--   0 veulsan  (2037719458) 1135428931     1786 2024-03-25 13:36:01.000000 energiinfo-0.0.8/src/energiinfo/HttpClient.py
--rw-r--r--   0 veulsan  (2037719458) 1135428931       85 2024-03-25 15:19:52.000000 energiinfo-0.0.8/src/energiinfo/__init__.py
--rw-r--r--   0 veulsan  (2037719458) 1135428931     6565 2024-03-25 15:18:34.000000 energiinfo-0.0.8/src/energiinfo/api.py
--rw-r--r--   0 veulsan  (2037719458) 1135428931      972 2024-03-24 02:32:43.000000 energiinfo-0.0.8/src/energiinfo/const.py
-drwxr-xr-x   0 veulsan  (2037719458) 1135428931        0 2024-03-25 21:11:32.859905 energiinfo-0.0.8/src/energiinfo.egg-info/
--rw-r--r--   0 veulsan  (2037719458) 1135428931     1917 2024-03-25 21:11:32.000000 energiinfo-0.0.8/src/energiinfo.egg-info/PKG-INFO
--rw-r--r--   0 veulsan  (2037719458) 1135428931      296 2024-03-25 21:11:32.000000 energiinfo-0.0.8/src/energiinfo.egg-info/SOURCES.txt
--rw-r--r--   0 veulsan  (2037719458) 1135428931        1 2024-03-25 21:11:32.000000 energiinfo-0.0.8/src/energiinfo.egg-info/dependency_links.txt
--rw-r--r--   0 veulsan  (2037719458) 1135428931       11 2024-03-25 21:11:32.000000 energiinfo-0.0.8/src/energiinfo.egg-info/top_level.txt
+drwxr-xr-x   0 veulsan  (2037719458) 1135428931        0 2024-04-16 13:30:59.273381 energiinfo-1.0.1/
+-rw-r--r--   0 veulsan  (2037719458) 1135428931    35149 2024-04-16 12:42:03.000000 energiinfo-1.0.1/LICENSE
+-rw-r--r--   0 veulsan  (2037719458) 1135428931     1917 2024-04-16 13:30:59.272691 energiinfo-1.0.1/PKG-INFO
+-rw-r--r--   0 veulsan  (2037719458) 1135428931     1359 2024-04-16 12:42:03.000000 energiinfo-1.0.1/README.md
+-rw-r--r--   0 veulsan  (2037719458) 1135428931       87 2024-04-16 13:30:50.000000 energiinfo-1.0.1/pyproject.toml
+-rw-r--r--   0 veulsan  (2037719458) 1135428931      685 2024-04-16 13:30:59.285241 energiinfo-1.0.1/setup.cfg
+drwxr-xr-x   0 veulsan  (2037719458) 1135428931        0 2024-04-16 13:30:59.224506 energiinfo-1.0.1/src/
+drwxr-xr-x   0 veulsan  (2037719458) 1135428931        0 2024-04-16 13:30:59.245622 energiinfo-1.0.1/src/energiinfo/
+-rw-r--r--   0 veulsan  (2037719458) 1135428931       85 2024-04-16 13:26:33.000000 energiinfo-1.0.1/src/energiinfo/__init__.py
+-rw-r--r--   0 veulsan  (2037719458) 1135428931     8812 2024-04-16 13:13:32.000000 energiinfo-1.0.1/src/energiinfo/api.py
+-rw-r--r--   0 veulsan  (2037719458) 1135428931     1009 2024-04-16 13:18:42.000000 energiinfo-1.0.1/src/energiinfo/const.py
+drwxr-xr-x   0 veulsan  (2037719458) 1135428931        0 2024-04-16 13:30:59.271359 energiinfo-1.0.1/src/energiinfo.egg-info/
+-rw-r--r--   0 veulsan  (2037719458) 1135428931     1917 2024-04-16 13:30:59.000000 energiinfo-1.0.1/src/energiinfo.egg-info/PKG-INFO
+-rw-r--r--   0 veulsan  (2037719458) 1135428931      267 2024-04-16 13:30:59.000000 energiinfo-1.0.1/src/energiinfo.egg-info/SOURCES.txt
+-rw-r--r--   0 veulsan  (2037719458) 1135428931        1 2024-04-16 13:30:59.000000 energiinfo-1.0.1/src/energiinfo.egg-info/dependency_links.txt
+-rw-r--r--   0 veulsan  (2037719458) 1135428931       11 2024-04-16 13:30:59.000000 energiinfo-1.0.1/src/energiinfo.egg-info/top_level.txt
```

### Comparing `energiinfo-0.0.8/LICENSE` & `energiinfo-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `energiinfo-0.0.8/PKG-INFO` & `energiinfo-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energiinfo
-Version: 0.0.8
+Version: 1.0.1
 Summary: Energiinfo API package
 Home-page: https://gitlab.com/veulsan/energiinfo
 Author: Ulrik Sannsell
 Author-email: ulrik@sannsell.se
 Project-URL: Bug Tracker, https://gitlab.com/veulsan/energiinfo/-/issues
 Project-URL: repository, https://gitlab.com/veulsan/energiinfo
 Classifier: Programming Language :: Python :: 3
```

### Comparing `energiinfo-0.0.8/README.md` & `energiinfo-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `energiinfo-0.0.8/setup.cfg` & `energiinfo-1.0.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = energiinfo
-version = 0.0.8
+version = 1.0.1
 author = Ulrik Sannsell
 author_email = ulrik@sannsell.se
 description = Energiinfo API package
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://gitlab.com/veulsan/energiinfo
 project_urls =
```

### Comparing `energiinfo-0.0.8/src/energiinfo/api.py` & `energiinfo-1.0.1/src/energiinfo/api.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import requests
 
 from .const import (
     BASE_ENDPOINT,
     BASE_HOSTNAME,
     BASE_URL,
     CMD_LOGIN,
+    CMD_LOGIN_TOKEN,
     CMD_LOGOUT,
     CMD_PROFILE,
     CMD_METERPOINTS,
     CMD_INVOICES,
     CMD_PERIOD,
     CMD_OBJECTSETTINGS,
     CMD_TEMPERATURE,
@@ -34,26 +35,76 @@
     siteid = ""
 
     def __init__(self, apiurl: str, siteid: str, token: str = None):
          self.api_url = apiurl
          self.session = requests.Session()
          self.siteid = siteid
          if token is not None:
-            self.access_token = token
-
+             self.authenticateToken(token)
     def getStatus(self):
         return self.status
 
     def getErrorMessage(self):
         return self.error_message
 
+    def authenticateToken(self, token: str):
+        login_url = self.api_url + "/?cmd={}".format(CMD_LOGIN_TOKEN)
+
+        data = {
+            'site': self.siteid,
+            'access_token': token,
+        }
+
+        error_message = ''
+
+        try:
+            response = self.session.post(login_url, data=data)
+            # Check if the login request was successful (status code 200)
+            if response.status_code == 200:
+                # Parse the JSON response
+                self.status = response.json().get('status')
+                if self.status == 'ERR':
+                    self.error_message = response.json().get('error_message')
+                if self.status == 'OK':
+                    self.logged_in = True
+                    self.access_token = response.json().get('access_token')
+                    return self.access_token
+            elif response.status_code >= 400 and response.status_code < 500:
+                self.status = 'ERR'
+                self.error_message = f"Client Error: {response.status_code}"
+                return {'status': self.status, 'error_message': self.error_message}
+            elif response.status_code == 500:
+                self.status = 'ERR'
+                self.error_message = 'Internal server error'
+                return {'status': self.status, 'error_message': self.error_message}
+            else:
+                self.status = 'ERR'
+                self.error_message = response.json().get('error_message')
+                # print(f"Failed to execute cmd: {command}. Status code: {response.status_code}")
+                return None
+                self.error_message = str(e)
+        except requests.exceptions.RequestException as e:
+            # Handle request exceptions such as network errors
+            self.status = 'ERR'
+            self.error_message = f"Request Exception: {e}"
+            return None
+        except ValueError as e:
+            # Handle JSON parsing errors
+            self.status = 'ERR'
+            self.error_message = f"JSON Parsing Error: {e}"
+            return None
+        except Exception as e:
+            # Catch any other unexpected exceptions
+            self.status = 'ERR'
+            self.error_message = f"An unexpected error occurred: {e}"
+            return None
+
     def get_access_token(self):
         if self.access_token is not None:
-            response = self.run_command(self.api_url, CMD_PROFILE, None, None)
-            self.status = response['status']
+            self.authenticateToken(self.access_token)
             if response['status'] == 'OK':
                 self.logged_in = True
             else:
                 self.error_message = response.get('error_message')
                 self.logged_in = False
                 return None
```

### Comparing `energiinfo-0.0.8/src/energiinfo/const.py` & `energiinfo-1.0.1/src/energiinfo/const.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 BASE_HOSTNAME = "api4.energiinfo.se"
 BASE_URL = "https://" + BASE_HOSTNAME + "/"
 BASE_ENDPOINT = BASE_URL
 
 # Commands
 #cmd=login
 CMD_LOGIN="login"
+CMD_LOGIN_TOKEN="login/access_token"
 #cmd=login
 CMD_LOGOUT="logout"
 #cmd=meteringpoints
 CMD_METERPOINTS="meteringpoints"
 #cmd=invoices
 CMD_INVOICES="invoices"
 #cmd=servicesettings/get
@@ -36,8 +37,8 @@
     "Chrome/85.0.{BUILD}.{REV} Safari/537.36"
 )
 CLIENT_HEADERS = {
     "Content-Type": "application/json",
     "Accept": "application/json",
 }
 
-TOKEN_EXPRIATION = datetime.timedelta(minutes=60)
+TOKEN_EXPIRATION = datetime.timedelta(minutes=60)
```

### Comparing `energiinfo-0.0.8/src/energiinfo.egg-info/PKG-INFO` & `energiinfo-1.0.1/src/energiinfo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energiinfo
-Version: 0.0.8
+Version: 1.0.1
 Summary: Energiinfo API package
 Home-page: https://gitlab.com/veulsan/energiinfo
 Author: Ulrik Sannsell
 Author-email: ulrik@sannsell.se
 Project-URL: Bug Tracker, https://gitlab.com/veulsan/energiinfo/-/issues
 Project-URL: repository, https://gitlab.com/veulsan/energiinfo
 Classifier: Programming Language :: Python :: 3
```

