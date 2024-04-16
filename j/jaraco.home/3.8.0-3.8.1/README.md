# Comparing `tmp/jaraco.home-3.8.0.tar.gz` & `tmp/jaraco_home-3.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.home-3.8.0.tar", last modified: Thu Apr 11 20:24:05 2024, max compression
+gzip compressed data, was "jaraco_home-3.8.1.tar", last modified: Tue Apr 16 02:05:14 2024, max compression
```

## Comparing `jaraco.home-3.8.0.tar` & `jaraco_home-3.8.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:24:05.723543 jaraco.home-3.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:24:05.715543 jaraco.home-3.8.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:24:05.715543 jaraco.home-3.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-11 20:24:05.723543 jaraco.home-3.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:24:05.715543 jaraco.home-3.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:24:05.715543 jaraco.home-3.8.0/jaraco/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:24:05.719543 jaraco.home-3.8.0/jaraco/home/
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/jaraco/home/Gather HDHomeRun Stats.plist
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/jaraco/home/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/jaraco/home/check-traps.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/jaraco/home/contact.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/jaraco/home/hdhomerun.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/jaraco/home/mock hdhomerun.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/jaraco/home/relay.py
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/jaraco/home/report-spam-call.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/jaraco/home/thermostat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:24:05.719543 jaraco.home-3.8.0/jaraco.home.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-11 20:24:05.000000 jaraco.home-3.8.0/jaraco.home.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-11 20:24:05.000000 jaraco.home-3.8.0/jaraco.home.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 20:24:05.000000 jaraco.home-3.8.0/jaraco.home.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-11 20:24:05.000000 jaraco.home-3.8.0/jaraco.home.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-11 20:24:05.000000 jaraco.home-3.8.0/jaraco.home.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-11 20:24:05.723543 jaraco.home-3.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-11 20:23:50.000000 jaraco.home-3.8.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:05:14.024095 jaraco_home-3.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:05:14.020095 jaraco_home-3.8.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:05:14.020095 jaraco_home-3.8.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-16 02:05:14.024095 jaraco_home-3.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:05:14.020095 jaraco_home-3.8.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:05:14.016095 jaraco_home-3.8.1/jaraco/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:05:14.020095 jaraco_home-3.8.1/jaraco/home/
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/jaraco/home/Gather HDHomeRun Stats.plist
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/jaraco/home/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/jaraco/home/check-traps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/jaraco/home/contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/jaraco/home/hdhomerun.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/jaraco/home/mock hdhomerun.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/jaraco/home/relay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/jaraco/home/report-spam-call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/jaraco/home/thermostat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:05:14.024095 jaraco_home-3.8.1/jaraco.home.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-16 02:05:13.000000 jaraco_home-3.8.1/jaraco.home.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-16 02:05:14.000000 jaraco_home-3.8.1/jaraco.home.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 02:05:13.000000 jaraco_home-3.8.1/jaraco.home.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-16 02:05:13.000000 jaraco_home-3.8.1/jaraco.home.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 02:05:13.000000 jaraco_home-3.8.1/jaraco.home.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-16 02:05:14.024095 jaraco_home-3.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-16 02:04:58.000000 jaraco_home-3.8.1/tox.ini
```

### Comparing `jaraco.home-3.8.0/.github/workflows/main.yml` & `jaraco_home-3.8.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.8.0/LICENSE` & `jaraco_home-3.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.8.0/NEWS.rst` & `jaraco_home-3.8.1/NEWS.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v3.8.1
+======
+
+Bugfixes
+--------
+
+- Fix check-traps to actually reflect status.
+
+
 v3.8.0
 ======
 
 Features
 --------
 
 - Add script for checking the mouse trap(s).
```

### Comparing `jaraco.home-3.8.0/PKG-INFO` & `jaraco_home-3.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.home
-Version: 3.8.0
+Version: 3.8.1
 Summary: Some functions supporting the devices in jaraco's home
 Home-page: https://github.com/jaraco/jaraco.home
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jaraco.home-3.8.0/README.rst` & `jaraco_home-3.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.8.0/conftest.py` & `jaraco_home-3.8.1/conftest.py`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.8.0/docs/conf.py` & `jaraco_home-3.8.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.8.0/jaraco/home/Gather HDHomeRun Stats.plist` & `jaraco_home-3.8.1/jaraco/home/Gather HDHomeRun Stats.plist`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.8.0/jaraco/home/check-traps.py` & `jaraco_home-3.8.1/jaraco/home/check-traps.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,10 +9,10 @@
 async def check_traps():
     username = contact.load().email
     password = keyring.get_password('https://www.victorpest.com', username)
     async with vsk.VictorAsyncClient(username, password) as client:
         api = vsk.VictorApi(client)
         traps = await api.get_traps()
         for trap in traps:
-            if trap.status:
-                print(trap.name, "has non-zero status")
+            if trap.trapstatistics.kills_present:
+                print(trap.name, "needs attention")
         return any(trap.status for trap in traps)
```

### Comparing `jaraco.home-3.8.0/jaraco/home/hdhomerun.py` & `jaraco_home-3.8.1/jaraco/home/hdhomerun.py`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.8.0/jaraco/home/relay.py` & `jaraco_home-3.8.1/jaraco/home/relay.py`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.8.0/jaraco/home/report-spam-call.py` & `jaraco_home-3.8.1/jaraco/home/report-spam-call.py`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.8.0/jaraco/home/thermostat.py` & `jaraco_home-3.8.1/jaraco/home/thermostat.py`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.8.0/jaraco.home.egg-info/PKG-INFO` & `jaraco_home-3.8.1/jaraco.home.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.home
-Version: 3.8.0
+Version: 3.8.1
 Summary: Some functions supporting the devices in jaraco's home
 Home-page: https://github.com/jaraco/jaraco.home
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jaraco.home-3.8.0/jaraco.home.egg-info/SOURCES.txt` & `jaraco_home-3.8.1/jaraco.home.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.8.0/pytest.ini` & `jaraco_home-3.8.1/pytest.ini`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.8.0/setup.cfg` & `jaraco_home-3.8.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `jaraco.home-3.8.0/tox.ini` & `jaraco_home-3.8.1/tox.ini`

 * *Files identical despite different names*

