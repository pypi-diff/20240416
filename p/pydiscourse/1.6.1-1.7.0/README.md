# Comparing `tmp/pydiscourse-1.6.1.tar.gz` & `tmp/pydiscourse-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydiscourse-1.6.1.tar", last modified: Fri Sep  1 14:39:13 2023, max compression
+gzip compressed data, was "pydiscourse-1.7.0.tar", last modified: Tue Apr 16 20:37:09 2024, max compression
```

## Comparing `pydiscourse-1.6.1.tar` & `pydiscourse-1.7.0.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 14:39:13.196979 pydiscourse-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (999)      325 2023-09-01 14:38:59.000000 pydiscourse-1.6.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (999)     2582 2023-09-01 14:38:59.000000 pydiscourse-1.6.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (999)     1072 2023-09-01 14:38:59.000000 pydiscourse-1.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)      122 2023-09-01 14:38:59.000000 pydiscourse-1.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (999)     5227 2023-09-01 14:39:13.196979 pydiscourse-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     2328 2023-09-01 14:38:59.000000 pydiscourse-1.6.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (999)      939 2023-09-01 14:38:59.000000 pydiscourse-1.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)     1111 2023-09-01 14:39:13.196979 pydiscourse-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)       83 2023-09-01 14:38:59.000000 pydiscourse-1.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 14:39:13.192978 pydiscourse-1.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 14:39:13.196979 pydiscourse-1.6.1/src/pydiscourse/
--rw-r--r--   0 runner    (1001) docker     (999)      146 2023-09-01 14:38:59.000000 pydiscourse-1.6.1/src/pydiscourse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    42728 2023-09-01 14:38:59.000000 pydiscourse-1.6.1/src/pydiscourse/client.py
--rw-r--r--   0 runner    (1001) docker     (999)      511 2023-09-01 14:38:59.000000 pydiscourse-1.6.1/src/pydiscourse/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (999)     2648 2023-09-01 14:38:59.000000 pydiscourse-1.6.1/src/pydiscourse/main.py
--rw-r--r--   0 runner    (1001) docker     (999)     3268 2023-09-01 14:38:59.000000 pydiscourse-1.6.1/src/pydiscourse/sso.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 14:39:13.196979 pydiscourse-1.6.1/src/pydiscourse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     5227 2023-09-01 14:39:13.000000 pydiscourse-1.6.1/src/pydiscourse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      489 2023-09-01 14:39:13.000000 pydiscourse-1.6.1/src/pydiscourse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-01 14:39:13.000000 pydiscourse-1.6.1/src/pydiscourse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       57 2023-09-01 14:39:13.000000 pydiscourse-1.6.1/src/pydiscourse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-01 14:39:13.000000 pydiscourse-1.6.1/src/pydiscourse.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (999)       16 2023-09-01 14:39:13.000000 pydiscourse-1.6.1/src/pydiscourse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       12 2023-09-01 14:39:13.000000 pydiscourse-1.6.1/src/pydiscourse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:37:09.879937 pydiscourse-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-16 20:37:01.000000 pydiscourse-1.7.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-16 20:37:01.000000 pydiscourse-1.7.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-16 20:37:01.000000 pydiscourse-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-16 20:37:01.000000 pydiscourse-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-04-16 20:37:09.879937 pydiscourse-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-16 20:37:01.000000 pydiscourse-1.7.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-16 20:37:01.000000 pydiscourse-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-16 20:37:09.879937 pydiscourse-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-16 20:37:01.000000 pydiscourse-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:37:09.871937 pydiscourse-1.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:37:09.875937 pydiscourse-1.7.0/src/pydiscourse/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-16 20:37:01.000000 pydiscourse-1.7.0/src/pydiscourse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43019 2024-04-16 20:37:01.000000 pydiscourse-1.7.0/src/pydiscourse/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-16 20:37:01.000000 pydiscourse-1.7.0/src/pydiscourse/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-16 20:37:01.000000 pydiscourse-1.7.0/src/pydiscourse/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-16 20:37:01.000000 pydiscourse-1.7.0/src/pydiscourse/sso.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:37:09.879937 pydiscourse-1.7.0/src/pydiscourse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-04-16 20:37:09.000000 pydiscourse-1.7.0/src/pydiscourse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-16 20:37:09.000000 pydiscourse-1.7.0/src/pydiscourse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 20:37:09.000000 pydiscourse-1.7.0/src/pydiscourse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-16 20:37:09.000000 pydiscourse-1.7.0/src/pydiscourse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 20:37:09.000000 pydiscourse-1.7.0/src/pydiscourse.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-16 20:37:09.000000 pydiscourse-1.7.0/src/pydiscourse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 20:37:09.000000 pydiscourse-1.7.0/src/pydiscourse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:37:09.875937 pydiscourse-1.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-04-16 20:37:01.000000 pydiscourse-1.7.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-16 20:37:01.000000 pydiscourse-1.7.0/tests/test_sso.py
```

### Comparing `pydiscourse-1.6.1/HISTORY.rst` & `pydiscourse-1.7.0/HISTORY.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 .. :changelog:
 
 Release history
 ===============
 
+
+1.7.0
+-----
+
+- Possible breaking change: Change `search()` term paramater from `term` to `q`,
+  fixes search. Thanks @weber-s
+- Add support for Python 3.12
+
 1.6.1
 -----
 
 - Adds `posts_by_number` endpoint from @Dettorer
 
 1.6.0
 -----
```

### Comparing `pydiscourse-1.6.1/LICENSE` & `pydiscourse-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydiscourse-1.6.1/PKG-INFO` & `pydiscourse-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: pydiscourse
-Version: 1.6.1
+Version: 1.7.0
 Summary: "A Python library for the Discourse API"
 Home-page: https://github.com/bennylope/pydiscourse
 Author: "Marc Sibson and contributors"
 Author-email: "ben@benlopatin.com"
 License: "MIT"
 Platform: OS Independent
 License-File: LICENSE
 License-File: AUTHORS
+Requires-Dist: requests>=2.4.2
 
 ===========
 pydiscourse
 ===========
 
 .. image:: https://github.com/bennylope/pydiscourse/workflows/Tests/badge.svg
     :alt: Build Status
@@ -90,14 +91,22 @@
     pydiscoursecli --host-http://yourhost --api-user-system user eviltrout
 
 .. :changelog:
 
 Release history
 ===============
 
+
+1.7.0
+-----
+
+- Possible breaking change: Change `search()` term paramater from `term` to `q`,
+  fixes search. Thanks @weber-s
+- Add support for Python 3.12
+
 1.6.1
 -----
 
 - Adds `posts_by_number` endpoint from @Dettorer
 
 1.6.0
 -----
```

### Comparing `pydiscourse-1.6.1/README.rst` & `pydiscourse-1.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `pydiscourse-1.6.1/pyproject.toml` & `pydiscourse-1.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydiscourse-1.6.1/setup.cfg` & `pydiscourse-1.7.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	pydiscoursecli = pydiscourse.main:main
```

### Comparing `pydiscourse-1.6.1/src/pydiscourse/client.py` & `pydiscourse-1.7.0/src/pydiscourse/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,14 +226,25 @@
             level:
 
         Returns:
 
         """
         return self._put(f"/admin/users/{userid}/trust_level", level=level)
 
+    def anonymize(self, userid):
+        """
+
+        Args:
+            userid: the Discourse user ID
+
+        Returns:
+
+        """
+        return self._put(f"/admin/users/{userid}/anonymize")
+
     def suspend(self, userid, duration, reason):
         """
         Suspend a user's account
 
         Args:
             userid: the Discourse user ID
             duration: the length of time in days for which a user's account
@@ -840,25 +851,25 @@
 
         Returns:
 
         """
         kwargs = {"email": user_email, "topic_id": topic_id}
         return self._post(f"/t/{topic_id}/invite.json", **kwargs)
 
-    def search(self, term, **kwargs):
+    def search(self, q, **kwargs):
         """
 
         Args:
-            term:
+            q:
             **kwargs:
 
         Returns:
 
         """
-        kwargs["term"] = term
+        kwargs["q"] = q
         return self._get("/search.json", **kwargs)
 
     def badges(self, **kwargs):
         """
 
         Args:
             **kwargs:
@@ -1496,14 +1507,20 @@
             category_id
             **kwargs:
                 notification_level=(int)
 
         """
         return self._post(f"/category/{category_id}/notifications", **kwargs)
 
+    def about(self):
+        """
+        Get site info
+        """
+        return self._get("/about.json")
+
     def _get(self, path, override_request_kwargs=None, **kwargs):
         """
 
         Args:
             path:
             **kwargs:
```

### Comparing `pydiscourse-1.6.1/src/pydiscourse/main.py` & `pydiscourse-1.7.0/src/pydiscourse/main.py`

 * *Files identical despite different names*

### Comparing `pydiscourse-1.6.1/src/pydiscourse/sso.py` & `pydiscourse-1.7.0/src/pydiscourse/sso.py`

 * *Files identical despite different names*

### Comparing `pydiscourse-1.6.1/src/pydiscourse.egg-info/PKG-INFO` & `pydiscourse-1.7.0/src/pydiscourse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: pydiscourse
-Version: 1.6.1
+Version: 1.7.0
 Summary: "A Python library for the Discourse API"
 Home-page: https://github.com/bennylope/pydiscourse
 Author: "Marc Sibson and contributors"
 Author-email: "ben@benlopatin.com"
 License: "MIT"
 Platform: OS Independent
 License-File: LICENSE
 License-File: AUTHORS
+Requires-Dist: requests>=2.4.2
 
 ===========
 pydiscourse
 ===========
 
 .. image:: https://github.com/bennylope/pydiscourse/workflows/Tests/badge.svg
     :alt: Build Status
@@ -90,14 +91,22 @@
     pydiscoursecli --host-http://yourhost --api-user-system user eviltrout
 
 .. :changelog:
 
 Release history
 ===============
 
+
+1.7.0
+-----
+
+- Possible breaking change: Change `search()` term paramater from `term` to `q`,
+  fixes search. Thanks @weber-s
+- Add support for Python 3.12
+
 1.6.1
 -----
 
 - Adds `posts_by_number` endpoint from @Dettorer
 
 1.6.0
 -----
```

