# Comparing `tmp/certbot_nginx_unit-1.0.8.tar.gz` & `tmp/certbot_nginx_unit-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certbot_nginx_unit-1.0.8.tar", last modified: Sun Apr 14 15:43:04 2024, max compression
+gzip compressed data, was "certbot_nginx_unit-1.0.9.tar", last modified: Tue Apr 16 07:12:53 2024, max compression
```

## Comparing `certbot_nginx_unit-1.0.8.tar` & `certbot_nginx_unit-1.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:43:04.451506 certbot_nginx_unit-1.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:43:04.447506 certbot_nginx_unit-1.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:43:04.451506 certbot_nginx_unit-1.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-14 15:43:00.000000 certbot_nginx_unit-1.0.8/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-14 15:43:00.000000 certbot_nginx_unit-1.0.8/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-14 15:43:00.000000 certbot_nginx_unit-1.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    21568 2024-04-14 15:43:00.000000 certbot_nginx_unit-1.0.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-14 15:43:00.000000 certbot_nginx_unit-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-14 15:43:04.451506 certbot_nginx_unit-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-04-14 15:43:00.000000 certbot_nginx_unit-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:43:04.451506 certbot_nginx_unit-1.0.8/certbot_nginx_unit/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-14 15:43:00.000000 certbot_nginx_unit-1.0.8/certbot_nginx_unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16926 2024-04-14 15:43:00.000000 certbot_nginx_unit-1.0.8/certbot_nginx_unit/configurator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:43:04.451506 certbot_nginx_unit-1.0.8/certbot_nginx_unit/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-14 15:43:00.000000 certbot_nginx_unit-1.0.8/certbot_nginx_unit/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-04-14 15:43:00.000000 certbot_nginx_unit-1.0.8/certbot_nginx_unit/tests/configurator_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-04-14 15:43:00.000000 certbot_nginx_unit-1.0.8/certbot_nginx_unit/unitc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:43:04.451506 certbot_nginx_unit-1.0.8/certbot_nginx_unit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-14 15:43:04.000000 certbot_nginx_unit-1.0.8/certbot_nginx_unit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-14 15:43:04.000000 certbot_nginx_unit-1.0.8/certbot_nginx_unit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 15:43:04.000000 certbot_nginx_unit-1.0.8/certbot_nginx_unit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-14 15:43:04.000000 certbot_nginx_unit-1.0.8/certbot_nginx_unit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-14 15:43:04.000000 certbot_nginx_unit-1.0.8/certbot_nginx_unit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-14 15:43:04.000000 certbot_nginx_unit-1.0.8/certbot_nginx_unit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-14 15:43:00.000000 certbot_nginx_unit-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 15:43:04.451506 certbot_nginx_unit-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-14 15:43:00.000000 certbot_nginx_unit-1.0.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-14 15:43:00.000000 certbot_nginx_unit-1.0.8/snapcraft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-14 15:43:00.000000 certbot_nginx_unit-1.0.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:12:53.124900 certbot_nginx_unit-1.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:12:53.120900 certbot_nginx_unit-1.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:12:53.124900 certbot_nginx_unit-1.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-16 07:12:48.000000 certbot_nginx_unit-1.0.9/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-16 07:12:48.000000 certbot_nginx_unit-1.0.9/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-16 07:12:48.000000 certbot_nginx_unit-1.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    21568 2024-04-16 07:12:48.000000 certbot_nginx_unit-1.0.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-16 07:12:48.000000 certbot_nginx_unit-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-04-16 07:12:53.124900 certbot_nginx_unit-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-16 07:12:48.000000 certbot_nginx_unit-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:12:53.124900 certbot_nginx_unit-1.0.9/certbot_nginx_unit/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-16 07:12:48.000000 certbot_nginx_unit-1.0.9/certbot_nginx_unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17807 2024-04-16 07:12:48.000000 certbot_nginx_unit-1.0.9/certbot_nginx_unit/configurator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:12:53.124900 certbot_nginx_unit-1.0.9/certbot_nginx_unit/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-16 07:12:48.000000 certbot_nginx_unit-1.0.9/certbot_nginx_unit/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-04-16 07:12:48.000000 certbot_nginx_unit-1.0.9/certbot_nginx_unit/tests/configurator_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-04-16 07:12:48.000000 certbot_nginx_unit-1.0.9/certbot_nginx_unit/unitc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:12:53.124900 certbot_nginx_unit-1.0.9/certbot_nginx_unit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-04-16 07:12:53.000000 certbot_nginx_unit-1.0.9/certbot_nginx_unit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-16 07:12:53.000000 certbot_nginx_unit-1.0.9/certbot_nginx_unit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 07:12:53.000000 certbot_nginx_unit-1.0.9/certbot_nginx_unit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-16 07:12:53.000000 certbot_nginx_unit-1.0.9/certbot_nginx_unit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 07:12:53.000000 certbot_nginx_unit-1.0.9/certbot_nginx_unit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-16 07:12:53.000000 certbot_nginx_unit-1.0.9/certbot_nginx_unit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-16 07:12:48.000000 certbot_nginx_unit-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 07:12:53.124900 certbot_nginx_unit-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-16 07:12:48.000000 certbot_nginx_unit-1.0.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-16 07:12:48.000000 certbot_nginx_unit-1.0.9/snapcraft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-16 07:12:48.000000 certbot_nginx_unit-1.0.9/tox.ini
```

### Comparing `certbot_nginx_unit-1.0.8/.github/workflows/publish-to-pypi.yml` & `certbot_nginx_unit-1.0.9/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `certbot_nginx_unit-1.0.8/.pylintrc` & `certbot_nginx_unit-1.0.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `certbot_nginx_unit-1.0.8/LICENSE` & `certbot_nginx_unit-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `certbot_nginx_unit-1.0.8/PKG-INFO` & `certbot_nginx_unit-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-nginx-unit
-Version: 1.0.8
+Version: 1.0.9
 Summary: Nginx Unit plugin for Certbot
 Author-email: Manuel Baldassarri <m.baldassarri@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Manuel Baldassarri
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -71,15 +71,15 @@
     sudo snap install certbot-nginx-unit 
     sudo snap set certbot trust-plugin-with-root=ok
     sudo snap connect certbot:plugin certbot-nginx-unit
     ```
 
 * Via Pip
     ```
-    pip install certbot-nginx-unit
+    pip install certbot certbot-nginx-unit
     ```
 
 * Via Pip virtual env
 
     Create a virtual environment, to avoid conflicts
     ```
     python3 -m venv /some/path
```

### Comparing `certbot_nginx_unit-1.0.8/README.md` & `certbot_nginx_unit-1.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     sudo snap install certbot-nginx-unit 
     sudo snap set certbot trust-plugin-with-root=ok
     sudo snap connect certbot:plugin certbot-nginx-unit
     ```
 
 * Via Pip
     ```
-    pip install certbot-nginx-unit
+    pip install certbot certbot-nginx-unit
     ```
 
 * Via Pip virtual env
 
     Create a virtual environment, to avoid conflicts
     ```
     python3 -m venv /some/path
```

### Comparing `certbot_nginx_unit-1.0.8/certbot_nginx_unit/configurator.py` & `certbot_nginx_unit-1.0.9/certbot_nginx_unit/configurator.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from .unitc import Unitc
 
 CONFIG_TLS_CERTIFICATE_PATH = "/listeners/*:443/tls/certificate"
 
 logger = logging.getLogger(__name__)
 
 
-class Configurator(common.Installer, interfaces.Authenticator):
+class Configurator(common.Installer, interfaces.Authenticator, interfaces.RenewDeployer):
     """Nginx Unit certificate authenticator and installer plugin for Certbot"""
 
     description = """\
     Nginx Unit certificate installer plugin for Certbot: \
     saves the necessary validation files to a .well-known/acme-challenge/ directory within the \
     nominated webroot path. Nginx Unit server must be running. \
     HTTP challenge only (wildcards not supported)."""
@@ -377,7 +377,29 @@
                 os.rmdir(path)
             except OSError as exc:
                 not_removed.insert(0, path)
                 logger.info("Challenge directory %s was not empty, didn't remove", path)
                 logger.debug("Error was: %s", exc)
         self._created_dirs = not_removed
         logger.debug("All challenges cleaned up")
+
+    def renew_deploy(self, lineage: interfaces.RenewableCert, *args: Any, **kwargs: Any) -> None:
+        """Perform updates defined by installer when a certificate has been renewed
+
+        If an installer is a subclass of the class containing this method, this
+        function will always be called when a certificate has been renewed by
+        running "certbot renew". For example if a plugin needs to copy a
+        certificate over, or change configuration based on the new certificate.
+
+        This method is called once for each lineage renewed
+
+        :param lineage: Certificate lineage object
+        :type lineage: RenewableCert
+
+        """
+        self.deploy_cert(
+            lineage.lineagename,
+            lineage.cert_path,
+            lineage.key_path,
+            lineage.chain_path,
+            lineage.fullchain_path
+        )
```

### Comparing `certbot_nginx_unit-1.0.8/certbot_nginx_unit/tests/configurator_test.py` & `certbot_nginx_unit-1.0.9/certbot_nginx_unit/tests/configurator_test.py`

 * *Files identical despite different names*

### Comparing `certbot_nginx_unit-1.0.8/certbot_nginx_unit/unitc.py` & `certbot_nginx_unit-1.0.9/certbot_nginx_unit/unitc.py`

 * *Files identical despite different names*

### Comparing `certbot_nginx_unit-1.0.8/certbot_nginx_unit.egg-info/PKG-INFO` & `certbot_nginx_unit-1.0.9/certbot_nginx_unit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-nginx-unit
-Version: 1.0.8
+Version: 1.0.9
 Summary: Nginx Unit plugin for Certbot
 Author-email: Manuel Baldassarri <m.baldassarri@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Manuel Baldassarri
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -71,15 +71,15 @@
     sudo snap install certbot-nginx-unit 
     sudo snap set certbot trust-plugin-with-root=ok
     sudo snap connect certbot:plugin certbot-nginx-unit
     ```
 
 * Via Pip
     ```
-    pip install certbot-nginx-unit
+    pip install certbot certbot-nginx-unit
     ```
 
 * Via Pip virtual env
 
     Create a virtual environment, to avoid conflicts
     ```
     python3 -m venv /some/path
```

### Comparing `certbot_nginx_unit-1.0.8/certbot_nginx_unit.egg-info/SOURCES.txt` & `certbot_nginx_unit-1.0.9/certbot_nginx_unit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `certbot_nginx_unit-1.0.8/pyproject.toml` & `certbot_nginx_unit-1.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `certbot_nginx_unit-1.0.8/snapcraft.yaml` & `certbot_nginx_unit-1.0.9/snapcraft.yaml`

 * *Files identical despite different names*

### Comparing `certbot_nginx_unit-1.0.8/tox.ini` & `certbot_nginx_unit-1.0.9/tox.ini`

 * *Files identical despite different names*

