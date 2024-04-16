# Comparing `tmp/dictrule-0.2.0.tar.gz` & `tmp/dictrule-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dictrule-0.2.0.tar", last modified: Tue Apr 16 04:56:09 2024, max compression
+gzip compressed data, was "dictrule-0.3.0.tar", last modified: Tue Apr 16 05:35:10 2024, max compression
```

## Comparing `dictrule-0.2.0.tar` & `dictrule-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:56:09.506765 dictrule-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 04:56:02.000000 dictrule-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12367 2024-04-16 04:56:09.506765 dictrule-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11059 2024-04-16 04:56:02.000000 dictrule-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-16 04:56:02.000000 dictrule-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 04:56:09.506765 dictrule-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-16 04:56:02.000000 dictrule-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:56:09.502766 dictrule-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:56:09.506765 dictrule-0.2.0/src/dictrule/
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-16 04:56:02.000000 dictrule-0.2.0/src/dictrule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-16 04:56:02.000000 dictrule-0.2.0/src/dictrule/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-16 04:56:02.000000 dictrule-0.2.0/src/dictrule/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-16 04:56:02.000000 dictrule-0.2.0/src/dictrule/dr_property.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-16 04:56:02.000000 dictrule-0.2.0/src/dictrule/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-16 04:56:02.000000 dictrule-0.2.0/src/dictrule/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-16 04:56:02.000000 dictrule-0.2.0/src/dictrule/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:56:09.506765 dictrule-0.2.0/src/dictrule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12367 2024-04-16 04:56:09.000000 dictrule-0.2.0/src/dictrule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-16 04:56:09.000000 dictrule-0.2.0/src/dictrule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 04:56:09.000000 dictrule-0.2.0/src/dictrule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 04:56:09.000000 dictrule-0.2.0/src/dictrule.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 04:56:09.000000 dictrule-0.2.0/src/dictrule.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:35:10.101965 dictrule-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-16 05:35:06.000000 dictrule-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12356 2024-04-16 05:35:10.101965 dictrule-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11059 2024-04-16 05:35:06.000000 dictrule-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-16 05:35:06.000000 dictrule-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 05:35:10.101965 dictrule-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-04-16 05:35:06.000000 dictrule-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:35:10.097965 dictrule-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:35:10.101965 dictrule-0.3.0/src/dictrule/
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-16 05:35:06.000000 dictrule-0.3.0/src/dictrule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-16 05:35:06.000000 dictrule-0.3.0/src/dictrule/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-16 05:35:06.000000 dictrule-0.3.0/src/dictrule/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-16 05:35:06.000000 dictrule-0.3.0/src/dictrule/dr_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-16 05:35:06.000000 dictrule-0.3.0/src/dictrule/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-16 05:35:06.000000 dictrule-0.3.0/src/dictrule/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-16 05:35:06.000000 dictrule-0.3.0/src/dictrule/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:35:10.101965 dictrule-0.3.0/src/dictrule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12356 2024-04-16 05:35:10.000000 dictrule-0.3.0/src/dictrule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-16 05:35:10.000000 dictrule-0.3.0/src/dictrule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 05:35:10.000000 dictrule-0.3.0/src/dictrule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 05:35:09.000000 dictrule-0.3.0/src/dictrule.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 05:35:10.000000 dictrule-0.3.0/src/dictrule.egg-info/top_level.txt
```

### Comparing `dictrule-0.2.0/PKG-INFO` & `dictrule-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: dictrule
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python rules defined by a dict and a text generator from the rules
 Home-page: https://github.com/elhoangvu/dictrule
 Author: Zooxy Le
 Author-email: elhoangvu@gmail.com
-License: Apache-2.0
+License: MIT License
 Project-URL: Documentation, https://github.com/elhoangvu/dictrule
 Project-URL: Source, https://github.com/elhoangvu/dictrule
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `dictrule-0.2.0/README.md` & `dictrule-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `dictrule-0.2.0/setup.py` & `dictrule-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         include_package_data=True,
         python_requires=">=3.7",
         license=about["__license__"],
         zip_safe=False,
         classifiers=[
             "Development Status :: 5 - Production/Stable",
             "Intended Audience :: Developers",
-            "License :: OSI Approved :: Apache Software License",
+            "License :: OSI Approved :: MIT License",
             "Operating System :: OS Independent",
             "Programming Language :: Python",
             "Programming Language :: Python :: 3",
             "Programming Language :: Python :: 3.7",
             "Programming Language :: Python :: 3.8",
             "Programming Language :: Python :: 3.9",
             "Programming Language :: Python :: 3.10",
```

### Comparing `dictrule-0.2.0/src/dictrule/__init__.py` & `dictrule-0.3.0/src/dictrule/__init__.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.2.0/src/dictrule/__version__.py` & `dictrule-0.3.0/src/dictrule/__version__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,12 +6,12 @@
 \__,_/_/\___/\__/_/   \__,_/_/\___/    |___/\___/_/  /____/_/\____/_/ /_/ 
                                                                           
 """
 
 __title__ = "dictrule"
 __description__ = "Python rules defined by a dict and a text generator from the rules"
 __url__ = "https://github.com/elhoangvu/dictrule"
-__version__ = "0.2.0"
+__version__ = "0.3.0"
 __author__ = "Zooxy Le"
 __author_email__ = "elhoangvu@gmail.com"
-__license__ = "Apache-2.0"
+__license__ = "MIT License"
 __copyright__ = "Copyright Zooxy Le"
```

### Comparing `dictrule-0.2.0/src/dictrule/context.py` & `dictrule-0.3.0/src/dictrule/context.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.2.0/src/dictrule/dr_property.py` & `dictrule-0.3.0/src/dictrule/dr_property.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.2.0/src/dictrule/generator.py` & `dictrule-0.3.0/src/dictrule/generator.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.2.0/src/dictrule/rule.py` & `dictrule-0.3.0/src/dictrule/rule.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.2.0/src/dictrule.egg-info/PKG-INFO` & `dictrule-0.3.0/src/dictrule.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: dictrule
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python rules defined by a dict and a text generator from the rules
 Home-page: https://github.com/elhoangvu/dictrule
 Author: Zooxy Le
 Author-email: elhoangvu@gmail.com
-License: Apache-2.0
+License: MIT License
 Project-URL: Documentation, https://github.com/elhoangvu/dictrule
 Project-URL: Source, https://github.com/elhoangvu/dictrule
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

