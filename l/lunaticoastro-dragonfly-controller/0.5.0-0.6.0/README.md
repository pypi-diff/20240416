# Comparing `tmp/lunaticoastro_dragonfly_controller-0.5.0.tar.gz` & `tmp/lunaticoastro_dragonfly_controller-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lunaticoastro_dragonfly_controller-0.5.0.tar", max compression
+gzip compressed data, was "lunaticoastro_dragonfly_controller-0.6.0.tar", max compression
```

## Comparing `lunaticoastro_dragonfly_controller-0.5.0.tar` & `lunaticoastro_dragonfly_controller-0.6.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11357 2024-04-16 00:28:53.804105 lunaticoastro_dragonfly_controller-0.5.0/LICENSE
--rw-r--r--   0        0        0     2831 2024-04-16 00:28:53.804105 lunaticoastro_dragonfly_controller-0.5.0/README.md
--rw-r--r--   0        0        0     8644 2024-04-16 00:28:53.804105 lunaticoastro_dragonfly_controller-0.5.0/dragonfly_dome/controller.py
--rw-r--r--   0        0        0     1349 2024-04-16 00:28:53.804105 lunaticoastro_dragonfly_controller-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3429 1970-01-01 00:00:00.000000 lunaticoastro_dragonfly_controller-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-16 12:06:52.276927 lunaticoastro_dragonfly_controller-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2832 2024-04-16 12:06:52.276927 lunaticoastro_dragonfly_controller-0.6.0/README.md
+-rw-r--r--   0        0        0     8644 2024-04-16 12:06:52.276927 lunaticoastro_dragonfly_controller-0.6.0/dragonfly_dome/controller.py
+-rw-r--r--   0        0        0     1377 2024-04-16 12:06:52.276927 lunaticoastro_dragonfly_controller-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3430 1970-01-01 00:00:00.000000 lunaticoastro_dragonfly_controller-0.6.0/PKG-INFO
```

### Comparing `lunaticoastro_dragonfly_controller-0.5.0/LICENSE` & `lunaticoastro_dragonfly_controller-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lunaticoastro_dragonfly_controller-0.5.0/README.md` & `lunaticoastro_dragonfly_controller-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# lunaticoastro-dragonfly-controller
+# Lunaticoastro Dragonfly Controller
 Python code serves as a client that controls and queries a dome (DragonFly Dome) controller over a network, allowing it to send commands, and fetch relay and sensor data remotely.
 
 Once the Container is running you can open the API at http://<container_ip>:8080/api/ui/
 
 # DragonFly Dome Controller  
 This Docker container provides an isolated environment for running a server that interfaces with the DragonFly Dome controller, allowing remote command sending and data retrieval.  
 
@@ -78,7 +78,8 @@
 
 Acknowledgments
 ---------------
 
 *   Miguel Angel García Grande
 *   Jaime Alemany
 *   [lunaticoastro.com](lunaticoastro.com)
+
```

### Comparing `lunaticoastro_dragonfly_controller-0.5.0/dragonfly_dome/controller.py` & `lunaticoastro_dragonfly_controller-0.6.0/dragonfly_dome/controller.py`

 * *Files identical despite different names*

### Comparing `lunaticoastro_dragonfly_controller-0.5.0/pyproject.toml` & `lunaticoastro_dragonfly_controller-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lunaticoastro-dragonfly-controller"
-version = "0.5.0"
+version = "0.6.0"
 description = "Python Lib to control lunaticoastro dragonfly"
 readme = "README.md"
 authors = ["Robert Bradley <robbrad182@gmail.com>"]
 packages = [
     { include = "dragonfly_dome", from = "." },
 ]
 
@@ -41,9 +41,10 @@
 
 [tool.commitizen]
 major_version_zero = true
 version_provider = "poetry"
 version_scheme = "semver"
 version_files = [
     "home-assistant/custom_components/lunaticoastro-dragonfly-controller/manifest.json:version",
-    "home-assistant/custom_components/lunaticoastro-dragonfly-controller/manifest.json:requirements"
+    "home-assistant/custom_components/lunaticoastro-dragonfly-controller/manifest.json:requirements",
+    "swagger.yaml:version"
 ]
```

### Comparing `lunaticoastro_dragonfly_controller-0.5.0/PKG-INFO` & `lunaticoastro_dragonfly_controller-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: lunaticoastro-dragonfly-controller
-Version: 0.5.0
+Version: 0.6.0
 Summary: Python Lib to control lunaticoastro dragonfly
 Author: Robert Bradley
 Author-email: robbrad182@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: connexion[swagger-ui] (>=3.0.6,<4.0.0)
 Requires-Dist: uvicorn (>=0.29.0,<0.30.0)
 Project-URL: issues, https://github.com/robbrad/lunaticoastro-dragonfly-controller/issues
 Description-Content-Type: text/markdown
 
-# lunaticoastro-dragonfly-controller
+# Lunaticoastro Dragonfly Controller
 Python code serves as a client that controls and queries a dome (DragonFly Dome) controller over a network, allowing it to send commands, and fetch relay and sensor data remotely.
 
 Once the Container is running you can open the API at http://<container_ip>:8080/api/ui/
 
 # DragonFly Dome Controller  
 This Docker container provides an isolated environment for running a server that interfaces with the DragonFly Dome controller, allowing remote command sending and data retrieval.  
 
@@ -94,7 +94,8 @@
 Acknowledgments
 ---------------
 
 *   Miguel Angel García Grande
 *   Jaime Alemany
 *   [lunaticoastro.com](lunaticoastro.com)
 
+
```

