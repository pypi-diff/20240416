# Comparing `tmp/gammarer.aws-frontend-web-app-deploy-stack-1.1.5.tar.gz` & `tmp/gammarer.aws-frontend-web-app-deploy-stack-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-frontend-web-app-deploy-stack-1.1.5.tar", last modified: Tue Apr  9 19:13:22 2024, max compression
+gzip compressed data, was "gammarer.aws-frontend-web-app-deploy-stack-1.1.6.tar", last modified: Tue Apr 16 19:15:32 2024, max compression
```

## Comparing `gammarer.aws-frontend-web-app-deploy-stack-1.1.5.tar` & `gammarer.aws-frontend-web-app-deploy-stack-1.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:13:22.389634 gammarer.aws-frontend-web-app-deploy-stack-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-09 19:13:09.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-09 19:13:09.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-04-09 19:13:22.389634 gammarer.aws-frontend-web-app-deploy-stack-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-04-09 19:13:09.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-09 19:13:09.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 19:13:22.389634 gammarer.aws-frontend-web-app-deploy-stack-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-09 19:13:09.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:13:22.385634 gammarer.aws-frontend-web-app-deploy-stack-1.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:13:22.385634 gammarer.aws-frontend-web-app-deploy-stack-1.1.5/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:13:22.385634 gammarer.aws-frontend-web-app-deploy-stack-1.1.5/src/gammarer/aws_frontend_web_app_deploy_stack/
--rw-r--r--   0 runner    (1001) docker     (127)    28187 2024-04-09 19:13:09.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.5/src/gammarer/aws_frontend_web_app_deploy_stack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:13:22.385634 gammarer.aws-frontend-web-app-deploy-stack-1.1.5/src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-09 19:13:09.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.5/src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36388 2024-04-09 19:13:09.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.5/src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/aws-frontend-web-app-deploy-stack@1.1.5.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:13:09.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.5/src/gammarer/aws_frontend_web_app_deploy_stack/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:13:22.385634 gammarer.aws-frontend-web-app-deploy-stack-1.1.5/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-04-09 19:13:22.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.5/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-09 19:13:22.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.5/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:13:22.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.5/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-09 19:13:22.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.5/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 19:13:22.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.5/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:15:32.127126 gammarer.aws-frontend-web-app-deploy-stack-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-16 19:15:20.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-16 19:15:20.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-04-16 19:15:32.127126 gammarer.aws-frontend-web-app-deploy-stack-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-04-16 19:15:20.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-16 19:15:20.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 19:15:32.127126 gammarer.aws-frontend-web-app-deploy-stack-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-16 19:15:20.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:15:32.127126 gammarer.aws-frontend-web-app-deploy-stack-1.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:15:32.127126 gammarer.aws-frontend-web-app-deploy-stack-1.1.6/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:15:32.127126 gammarer.aws-frontend-web-app-deploy-stack-1.1.6/src/gammarer/aws_frontend_web_app_deploy_stack/
+-rw-r--r--   0 runner    (1001) docker     (127)    28187 2024-04-16 19:15:20.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.6/src/gammarer/aws_frontend_web_app_deploy_stack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:15:32.127126 gammarer.aws-frontend-web-app-deploy-stack-1.1.6/src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-16 19:15:20.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.6/src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36386 2024-04-16 19:15:20.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.6/src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/aws-frontend-web-app-deploy-stack@1.1.6.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:15:20.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.6/src/gammarer/aws_frontend_web_app_deploy_stack/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:15:32.127126 gammarer.aws-frontend-web-app-deploy-stack-1.1.6/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-04-16 19:15:32.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.6/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-16 19:15:32.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.6/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:15:32.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.6/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-16 19:15:32.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.6/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 19:15:32.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.6/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/top_level.txt
```

### Comparing `gammarer.aws-frontend-web-app-deploy-stack-1.1.5/LICENSE` & `gammarer.aws-frontend-web-app-deploy-stack-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-frontend-web-app-deploy-stack-1.1.5/PKG-INFO` & `gammarer.aws-frontend-web-app-deploy-stack-1.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-frontend-web-app-deploy-stack
-Version: 1.1.5
+Version: 1.1.6
 Summary: This is an AWS CDK Construct to make deploying a Frontend Web App (SPA) deploy to S3 behind CloudFront.
 Home-page: https://github.com/gammarer/aws-frontend-web-app-deploy-stack.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-frontend-web-app-deploy-stack.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-frontend-web-app-deploy-stack-1.1.5/README.md` & `gammarer.aws-frontend-web-app-deploy-stack-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-frontend-web-app-deploy-stack-1.1.5/setup.py` & `gammarer.aws-frontend-web-app-deploy-stack-1.1.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-frontend-web-app-deploy-stack",
-    "version": "1.1.5",
+    "version": "1.1.6",
     "description": "This is an AWS CDK Construct to make deploying a Frontend Web App (SPA) deploy to S3 behind CloudFront.",
     "license": "Apache-2.0",
     "url": "https://github.com/gammarer/aws-frontend-web-app-deploy-stack.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarer.aws_frontend_web_app_deploy_stack",
         "gammarer.aws_frontend_web_app_deploy_stack._jsii"
     ],
     "package_data": {
         "gammarer.aws_frontend_web_app_deploy_stack._jsii": [
-            "aws-frontend-web-app-deploy-stack@1.1.5.jsii.tgz"
+            "aws-frontend-web-app-deploy-stack@1.1.6.jsii.tgz"
         ],
         "gammarer.aws_frontend_web_app_deploy_stack": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `gammarer.aws-frontend-web-app-deploy-stack-1.1.5/src/gammarer/aws_frontend_web_app_deploy_stack/__init__.py` & `gammarer.aws-frontend-web-app-deploy-stack-1.1.6/src/gammarer/aws_frontend_web_app_deploy_stack/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-frontend-web-app-deploy-stack-1.1.5/src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/__init__.py` & `gammarer.aws-frontend-web-app-deploy-stack-1.1.6/src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 import constructs._jsii
 import gammarer.aws_secure_bucket._jsii
 import gammarer.aws_secure_cloudfront_origin_bucket._jsii
 import gammarer.aws_secure_frontend_web_app_cloudfront_distribution._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@gammarer/aws-frontend-web-app-deploy-stack",
-    "1.1.5",
+    "1.1.6",
     __name__[0:-6],
-    "aws-frontend-web-app-deploy-stack@1.1.5.jsii.tgz",
+    "aws-frontend-web-app-deploy-stack@1.1.6.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `gammarer.aws-frontend-web-app-deploy-stack-1.1.5/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/PKG-INFO` & `gammarer.aws-frontend-web-app-deploy-stack-1.1.6/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-frontend-web-app-deploy-stack
-Version: 1.1.5
+Version: 1.1.6
 Summary: This is an AWS CDK Construct to make deploying a Frontend Web App (SPA) deploy to S3 behind CloudFront.
 Home-page: https://github.com/gammarer/aws-frontend-web-app-deploy-stack.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-frontend-web-app-deploy-stack.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-frontend-web-app-deploy-stack-1.1.5/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/SOURCES.txt` & `gammarer.aws-frontend-web-app-deploy-stack-1.1.6/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/SOURCES.txt
 src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/dependency_links.txt
 src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/requires.txt
 src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/top_level.txt
 src/gammarer/aws_frontend_web_app_deploy_stack/__init__.py
 src/gammarer/aws_frontend_web_app_deploy_stack/py.typed
 src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/__init__.py
-src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/aws-frontend-web-app-deploy-stack@1.1.5.jsii.tgz
+src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/aws-frontend-web-app-deploy-stack@1.1.6.jsii.tgz
```

