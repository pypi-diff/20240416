# Comparing `tmp/cosmix_launcher-1.0.5.tar.gz` & `tmp/cosmix_launcher-1.0.6.tar.gz`

## Comparing `cosmix_launcher-1.0.5.tar` & `cosmix_launcher-1.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/cosmix.bat
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/license.txt
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/requirements.txt
--rwxr-xr-x   0        0        0      130 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/scripts/publish.sh
--rwxr-xr-x   0        0        0      343 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/scripts/test.sh
--rw-r--r--   0        0        0     5117 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/src/cosmix/__main__.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/src/cosmix/api/__init__.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/src/cosmix/api/config.py
--rw-r--r--   0        0        0     5516 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/src/cosmix/api/instance.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/src/cosmix/api/logger.py
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/src/cosmix/api/maven.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/src/cosmix/api/mod.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/src/cosmix/api/net.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/src/cosmix/api/paths.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/src/cosmix/api/versions.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/.gitignore
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/readme.md
--rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.6/cosmix.bat
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.6/license.txt
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.6/requirements.txt
+-rwxr-xr-x   0        0        0      130 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.6/scripts/publish.sh
+-rwxr-xr-x   0        0        0      343 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.6/scripts/test.sh
+-rw-r--r--   0        0        0     5824 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.6/src/cosmix/__main__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.6/src/cosmix/api/__init__.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.6/src/cosmix/api/config.py
+-rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.6/src/cosmix/api/instance.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.6/src/cosmix/api/logger.py
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.6/src/cosmix/api/maven.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.6/src/cosmix/api/mod.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.6/src/cosmix/api/net.py
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.6/src/cosmix/api/paths.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.6/src/cosmix/api/versions.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.6/.gitignore
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.6/readme.md
+-rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.6/PKG-INFO
```

### Comparing `cosmix_launcher-1.0.5/license.txt` & `cosmix_launcher-1.0.6/license.txt`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.5/requirements.txt` & `cosmix_launcher-1.0.6/requirements.txt`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.5/src/cosmix/__main__.py` & `cosmix_launcher-1.0.6/src/cosmix/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,34 +10,45 @@
 import click
 import os
 import send2trash
 import shutil
 
 
 @click.group()
-def cosmix():
-    pass
+@click.option("--work-dir", "-w", type=str, default=paths.WORK_DIR, help="Set a working directory for Cosmix.")
+def cosmix(work_dir: str):
+    if work_dir != paths.WORK_DIR:
+        paths.update_work_dir(os.path.abspath(work_dir))
+        # We clear config caches here just in case the config was cached before the
+        # working directory was updated
+        config._CACHED_CONFIG = None
+        logger._sanatization_mode = None
+        logger._sanatized_username = None
+        logger._colored_logs = None
+        logger.info("Set working directory to " + work_dir)
 
 
 @cosmix.command()
 def version():
     logger.info("Cosmix " + api.VERSION)
 
 
 @cosmix.command()
-def debug():
+@click.option("--no-versions", "-V", is_flag=True, default=False, help="Disables latest version checks.")
+def debug(no_versions: bool):
     logger.info("Cosmix " + api.VERSION)
     logger.info("Paths:")
     logger.info("  Local Path: " + paths.LOCAL_PATH)
     logger.info("  Work Dir:   " + paths.WORK_DIR)
     logger.info("  Instances:  " + paths.INSTANCES)
     logger.info("  Deps:       " + paths.DEPS)
-    logger.info("Latest Available Versions: (these may take a second)")
-    logger.info("  Cosmic Reach: " + versions.get_latest_of("reach"))
-    logger.info("  Cosmic Quilt: " + versions.get_latest_of("quilt"))
+    if not no_versions:
+        logger.info("Latest Available Versions: (these may take a second)")
+        logger.info("  Cosmic Reach: " + versions.get_latest_of("reach"))
+        logger.info("  Cosmic Quilt: " + versions.get_latest_of("quilt"))
 
 
 @cosmix.command()
 @click.option("--version", "-v", default="latest", type=str, help="The version of Cosmic Reach to use. Defaults to 'latest'")
 @click.option("--quilt-version", "-q", default=None, type=str, help="The Cosmic Quilt version to use.")
 @click.option("--display-name", "-n", default=None, type=str, help="An optional display name to use for the instance.")
 @click.argument("name")
```

### Comparing `cosmix_launcher-1.0.5/src/cosmix/api/config.py` & `cosmix_launcher-1.0.6/src/cosmix/api/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 def get_config() -> dict:
     global _CACHED_CONFIG
     if not os.path.exists(paths.WORK_DIR):
         os.makedirs(paths.WORK_DIR, exist_ok = True)
 
     path = os.path.join(paths.WORK_DIR, "config.hjson")
     if not os.path.isfile(path):
-        with open(path, "w") as fp:
+        with open(path, "w+") as fp:
             fp.write(DEFAULT_CONFIG)
 
     if _CACHED_CONFIG is None:
         with open(path, "r") as fp:
             _CACHED_CONFIG = hjson.load(fp)
 
     return _CACHED_CONFIG
```

### Comparing `cosmix_launcher-1.0.5/src/cosmix/api/instance.py` & `cosmix_launcher-1.0.6/src/cosmix/api/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,16 @@
         else:
             args.extend([
                 "-Dloader.gameJarPath=" + paths.path_to_cr(self.version),
                 "-classpath", self.get_classpath(),
                 "org.quiltmc.loader.impl.launch.knot.KnotClient"
             ])
         args.extend(self.args)
-        args.extend(launch_args)
+        if launch_args is not None:
+            args.extend(launch_args)
 
         logger.info(f"Launching \"{self.display_name}\" ({self.name}) with args {args} in folder {self.path}")
         os.execvp("java", args)
 
     def download(self, is_updating: bool = False):
         cr_path = paths.path_to_cr(self.version)
         if not os.path.isfile(cr_path):
```

### Comparing `cosmix_launcher-1.0.5/src/cosmix/api/maven.py` & `cosmix_launcher-1.0.6/src/cosmix/api/maven.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.5/src/cosmix/api/mod.py` & `cosmix_launcher-1.0.6/src/cosmix/api/mod.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.5/src/cosmix/api/net.py` & `cosmix_launcher-1.0.6/src/cosmix/api/net.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.5/src/cosmix/api/versions.py` & `cosmix_launcher-1.0.6/src/cosmix/api/versions.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.5/pyproject.toml` & `cosmix_launcher-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cosmix-launcher"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
     { name = "EmmaTheMartian", email="emmathemartian@gmail.com" },
 ]
 description = "A dead simple CLI-based launcher for Cosmic Reach and Cosmic Quilt"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `cosmix_launcher-1.0.5/readme.md` & `cosmix_launcher-1.0.6/readme.md`

 * *Files 4% similar despite different names*

```diff
@@ -61,14 +61,17 @@
 To install and/or upgrade all of them at once, just run:
 
 `python3 -m pip install --upgrade hjson tqdm requests crm1 Send2Trash click java-manifest`
 
 ## Usage
 
 ```
+global options:
+    --work-dir -w               specify a working directory for Cosmix to use.
+
 cosmix version
     prints the current installed cosmix version
 
 cosmix debug
     prints a lot of debug information related to cosmix
 
 cosmix add [instance]
```

### Comparing `cosmix_launcher-1.0.5/PKG-INFO` & `cosmix_launcher-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cosmix-launcher
-Version: 1.0.5
+Version: 1.0.6
 Summary: A dead simple CLI-based launcher for Cosmic Reach and Cosmic Quilt
 Project-URL: Homepage, https://codeberg.org/EmmaTheMartian/cosmix
 Project-URL: Issues, https://codeberg.org/EmmaTheMartian/cosmix/issues
 Author-email: EmmaTheMartian <emmathemartian@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
@@ -80,14 +80,17 @@
 To install and/or upgrade all of them at once, just run:
 
 `python3 -m pip install --upgrade hjson tqdm requests crm1 Send2Trash click java-manifest`
 
 ## Usage
 
 ```
+global options:
+    --work-dir -w               specify a working directory for Cosmix to use.
+
 cosmix version
     prints the current installed cosmix version
 
 cosmix debug
     prints a lot of debug information related to cosmix
 
 cosmix add [instance]
```

