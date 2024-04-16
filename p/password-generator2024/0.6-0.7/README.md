# Comparing `tmp/password_generator2024-0.6.tar.gz` & `tmp/password_generator2024-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "password_generator2024-0.6.tar", last modified: Sat Feb 10 17:24:27 2024, max compression
+gzip compressed data, was "dist/password_generator2024-0.7.tar", last modified: Tue Apr 16 09:08:17 2024, max compression
```

## Comparing `password_generator2024-0.6.tar` & `password_generator2024-0.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 PI        (1000) PI        (1000)        0 2024-02-10 17:24:27.587163 password_generator2024-0.6/
--rw-r--r--   0 PI        (1000) PI        (1000)      966 2024-02-10 17:24:27.583163 password_generator2024-0.6/PKG-INFO
--rw-r--r--   0 PI        (1000) PI        (1000)      246 2024-01-18 09:21:46.000000 password_generator2024-0.6/README.md
-drwxr-xr-x   0 PI        (1000) PI        (1000)        0 2024-02-10 17:24:27.583163 password_generator2024-0.6/password_generator2024.egg-info/
--rw-r--r--   0 PI        (1000) PI        (1000)      966 2024-02-10 17:24:27.000000 password_generator2024-0.6/password_generator2024.egg-info/PKG-INFO
--rw-r--r--   0 PI        (1000) PI        (1000)      202 2024-02-10 17:24:27.000000 password_generator2024-0.6/password_generator2024.egg-info/SOURCES.txt
--rw-r--r--   0 PI        (1000) PI        (1000)        1 2024-02-10 17:24:27.000000 password_generator2024-0.6/password_generator2024.egg-info/dependency_links.txt
--rw-r--r--   0 PI        (1000) PI        (1000)        1 2024-02-10 17:24:27.000000 password_generator2024-0.6/password_generator2024.egg-info/top_level.txt
--rw-r--r--   0 PI        (1000) PI        (1000)       38 2024-02-10 17:24:27.587163 password_generator2024-0.6/setup.cfg
--rw-r--r--   0 PI        (1000) PI        (1000)     1132 2024-02-10 17:24:11.000000 password_generator2024-0.6/setup.py
+drwxr-xr-x   0 PI        (1000) PI        (1000)        0 2024-04-16 09:08:17.738348 password_generator2024-0.7/
+-rw-r--r--   0 PI        (1000) PI        (1000)     1140 2024-04-16 09:08:17.738348 password_generator2024-0.7/PKG-INFO
+-rw-r--r--   0 PI        (1000) PI        (1000)      260 2024-04-16 08:03:53.000000 password_generator2024-0.7/README.md
+drwxr-xr-x   0 PI        (1000) PI        (1000)        0 2024-04-16 09:08:17.738348 password_generator2024-0.7/password_generator2024.egg-info/
+-rw-r--r--   0 PI        (1000) PI        (1000)     1140 2024-04-16 09:08:17.000000 password_generator2024-0.7/password_generator2024.egg-info/PKG-INFO
+-rw-r--r--   0 PI        (1000) PI        (1000)      202 2024-04-16 09:08:17.000000 password_generator2024-0.7/password_generator2024.egg-info/SOURCES.txt
+-rw-r--r--   0 PI        (1000) PI        (1000)        1 2024-04-16 09:08:17.000000 password_generator2024-0.7/password_generator2024.egg-info/dependency_links.txt
+-rw-r--r--   0 PI        (1000) PI        (1000)        1 2024-04-16 09:08:17.000000 password_generator2024-0.7/password_generator2024.egg-info/top_level.txt
+-rw-r--r--   0 PI        (1000) PI        (1000)       38 2024-04-16 09:08:17.738348 password_generator2024-0.7/setup.cfg
+-rw-r--r--   0 PI        (1000) PI        (1000)     1131 2024-04-16 09:07:54.000000 password_generator2024-0.7/setup.py
```

### Comparing `password_generator2024-0.6/PKG-INFO` & `password_generator2024-0.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: password_generator2024
-Version: 0.6
+Version: 0.7
 Summary: Simple Python Password Generator
 Home-page: https://github.com/PierreGode/password_generator
 Author: Pierre
 Author-email: pierre@gode.one
+License: UNKNOWN
+Description: # Python Password Generator
+        
+        This is a simple Python script to generate random passwords.
+        
+        ## Installation
+        
+        Describe how to install your package here.
+        
+        ## Usage
+        
+        Run the script to generate a random password:
+        
+        ```bash
+        python password_generator.py
+        version test11
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-
-# Python Password Generator
-
-This is a simple Python script to generate random passwords.
-
-## Installation
-
-Describe how to install your package here.
-
-## Usage
-
-Run the script to generate a random password:
-
-```bash
-python password_generator.py
```

### Comparing `password_generator2024-0.6/password_generator2024.egg-info/PKG-INFO` & `password_generator2024-0.7/password_generator2024.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: password-generator2024
-Version: 0.6
+Version: 0.7
 Summary: Simple Python Password Generator
 Home-page: https://github.com/PierreGode/password_generator
 Author: Pierre
 Author-email: pierre@gode.one
+License: UNKNOWN
+Description: # Python Password Generator
+        
+        This is a simple Python script to generate random passwords.
+        
+        ## Installation
+        
+        Describe how to install your package here.
+        
+        ## Usage
+        
+        Run the script to generate a random password:
+        
+        ```bash
+        python password_generator.py
+        version test11
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-
-# Python Password Generator
-
-This is a simple Python script to generate random passwords.
-
-## Installation
-
-Describe how to install your package here.
-
-## Usage
-
-Run the script to generate a random password:
-
-```bash
-python password_generator.py
```

### Comparing `password_generator2024-0.6/setup.py` & `password_generator2024-0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Read the contents of your README file
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='password_generator2024',  # This can stay with 
     
-    version='0.6',  # Increment the version
+    version='0.7',  # Increment the version
     packages=find_packages(),
     description='Simple Python Password Generator',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Pierre',
     author_email='pierre@gode.one',
     url='https://github.com/PierreGode/password_generator',
@@ -25,8 +25,8 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
     # Add other arguments to setup() as needed
-)
+)
```

