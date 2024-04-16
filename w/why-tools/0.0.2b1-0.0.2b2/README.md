# Comparing `tmp/why-tools-0.0.2b1.tar.gz` & `tmp/why-tools-0.0.2b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "why-tools-0.0.2b1.tar", last modified: Mon Apr 15 15:07:58 2024, max compression
+gzip compressed data, was "why-tools-0.0.2b2.tar", last modified: Tue Apr 16 13:33:25 2024, max compression
```

## Comparing `why-tools-0.0.2b1.tar` & `why-tools-0.0.2b2.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxr-x   0 yintian   (1000) yintian   (1000)        0 2024-04-15 15:07:58.005360 why-tools-0.0.2b1/
--rw-rw-r--   0 yintian   (1000) yintian   (1000)      598 2024-04-15 15:07:58.005360 why-tools-0.0.2b1/PKG-INFO
--rw-rw-r--   0 yintian   (1000) yintian   (1000)        8 2024-04-15 11:18:57.000000 why-tools-0.0.2b1/README.md
--rw-rw-r--   0 yintian   (1000) yintian   (1000)       38 2024-04-15 15:07:58.005360 why-tools-0.0.2b1/setup.cfg
--rw-rw-r--   0 yintian   (1000) yintian   (1000)     4089 2024-04-15 15:06:47.000000 why-tools-0.0.2b1/setup.py
-drwxrwxr-x   0 yintian   (1000) yintian   (1000)        0 2024-04-15 15:07:58.005360 why-tools-0.0.2b1/why_tools.egg-info/
--rw-rw-r--   0 yintian   (1000) yintian   (1000)      598 2024-04-15 15:07:57.000000 why-tools-0.0.2b1/why_tools.egg-info/PKG-INFO
--rw-rw-r--   0 yintian   (1000) yintian   (1000)      230 2024-04-15 15:07:57.000000 why-tools-0.0.2b1/why_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 yintian   (1000) yintian   (1000)        1 2024-04-15 15:07:57.000000 why-tools-0.0.2b1/why_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 yintian   (1000) yintian   (1000)       33 2024-04-15 15:07:57.000000 why-tools-0.0.2b1/why_tools.egg-info/requires.txt
--rw-rw-r--   0 yintian   (1000) yintian   (1000)        7 2024-04-15 15:07:57.000000 why-tools-0.0.2b1/why_tools.egg-info/top_level.txt
-drwxrwxr-x   0 yintian   (1000) yintian   (1000)        0 2024-04-15 15:07:58.005360 why-tools-0.0.2b1/ytools/
--rw-rw-r--   0 yintian   (1000) yintian   (1000)      187 2024-04-15 15:07:57.000000 why-tools-0.0.2b1/ytools/__init__.py
--rw-rw-r--   0 yintian   (1000) yintian   (1000)      566 2024-04-15 11:36:15.000000 why-tools-0.0.2b1/ytools/file.py
--rw-rw-r--   0 yintian   (1000) yintian   (1000)      194 2024-04-15 12:01:24.000000 why-tools-0.0.2b1/ytools/log.py
+drwxrwxr-x   0 yintian   (1000) yintian   (1000)        0 2024-04-16 13:33:25.258742 why-tools-0.0.2b2/
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)      701 2024-04-16 13:33:25.258742 why-tools-0.0.2b2/PKG-INFO
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)      111 2024-04-15 15:11:28.000000 why-tools-0.0.2b2/README.md
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)       38 2024-04-16 13:33:25.258742 why-tools-0.0.2b2/setup.cfg
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)     4188 2024-04-16 13:33:24.000000 why-tools-0.0.2b2/setup.py
+drwxrwxr-x   0 yintian   (1000) yintian   (1000)        0 2024-04-16 13:33:25.258742 why-tools-0.0.2b2/why_tools.egg-info/
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)      701 2024-04-16 13:33:25.000000 why-tools-0.0.2b2/why_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)      261 2024-04-16 13:33:25.000000 why-tools-0.0.2b2/why_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)        1 2024-04-16 13:33:25.000000 why-tools-0.0.2b2/why_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)       14 2024-04-16 13:33:25.000000 why-tools-0.0.2b2/why_tools.egg-info/requires.txt
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)        7 2024-04-16 13:33:25.000000 why-tools-0.0.2b2/why_tools.egg-info/top_level.txt
+drwxrwxr-x   0 yintian   (1000) yintian   (1000)        0 2024-04-16 13:33:25.258742 why-tools-0.0.2b2/ytools/
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)      187 2024-04-16 13:33:24.000000 why-tools-0.0.2b2/ytools/__init__.py
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)     1578 2024-04-16 13:31:34.000000 why-tools-0.0.2b2/ytools/date.py
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)      566 2024-04-15 11:36:15.000000 why-tools-0.0.2b2/ytools/file.py
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)      194 2024-04-15 12:01:24.000000 why-tools-0.0.2b2/ytools/log.py
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)     1752 2024-04-16 12:19:04.000000 why-tools-0.0.2b2/ytools/utils.py
```

### Comparing `why-tools-0.0.2b1/PKG-INFO` & `why-tools-0.0.2b2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: why-tools
-Version: 0.0.2b1
+Version: 0.0.2b2
 Summary: 为什么还要使用别的工具呢？
 Home-page: https://github.com/yintian710/whytools
 Author: yintian
 Author-email: yintian710@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -14,7 +14,11 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 
 
 # YTools
 
+提供一个普通的工具，旨在用的顺手，让大部分工具都不需要多次实例化
+
+## 
+
```

### Comparing `why-tools-0.0.2b1/setup.py` & `why-tools-0.0.2b2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -93,16 +93,18 @@
         os.system(f'{sys.executable} setup.py sdist build')
 
         self.status('Uploading the package to PyPI via Twine…')
         os.system('twine upload dist/*')
 
         self.status('Pushing git tags…')
         os.system('git tag v{0}'.format(about['__version__']))
+        os.system('git commit -a v{0}'.format(about['__version__']))
         # os.system()
         os.system('git push --tags')
+        os.system('git push')
 
         sys.exit()
 
 
 # Where the magic happens:
 setup(
     name=NAME,
```

### Comparing `why-tools-0.0.2b1/why_tools.egg-info/PKG-INFO` & `why-tools-0.0.2b2/why_tools.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: why-tools
-Version: 0.0.2b1
+Version: 0.0.2b2
 Summary: 为什么还要使用别的工具呢？
 Home-page: https://github.com/yintian710/whytools
 Author: yintian
 Author-email: yintian710@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -14,7 +14,11 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 
 
 # YTools
 
+提供一个普通的工具，旨在用的顺手，让大部分工具都不需要多次实例化
+
+## 
+
```

### Comparing `why-tools-0.0.2b1/ytools/file.py` & `why-tools-0.0.2b2/ytools/file.py`

 * *Files identical despite different names*

