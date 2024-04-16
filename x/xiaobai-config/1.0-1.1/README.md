# Comparing `tmp/xiaobai_config-1.0.tar.gz` & `tmp/xiaobai_config-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaobai_config-1.0.tar", last modified: Sat Mar 12 05:56:10 2022, max compression
+gzip compressed data, was "xiaobai_config-1.1.tar", last modified: Tue Apr 16 05:27:11 2024, max compression
```

## Comparing `xiaobai_config-1.0.tar` & `xiaobai_config-1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 zrx        (501) staff       (20)        0 2022-03-12 05:56:10.721828 xiaobai_config-1.0/
--rw-r--r--   0 zrx        (501) staff       (20)     1074 2022-03-12 05:33:03.000000 xiaobai_config-1.0/LICENSE
--rw-r--r--   0 zrx        (501) staff       (20)      458 2022-03-12 05:56:10.721445 xiaobai_config-1.0/PKG-INFO
--rw-r--r--   0 zrx        (501) staff       (20)      100 2022-03-12 05:43:36.000000 xiaobai_config-1.0/README.md
--rw-r--r--   0 zrx        (501) staff       (20)       38 2022-03-12 05:56:10.721953 xiaobai_config-1.0/setup.cfg
--rw-r--r--   0 zrx        (501) staff       (20)      573 2022-03-12 05:56:01.000000 xiaobai_config-1.0/setup.py
-drwxr-xr-x   0 zrx        (501) staff       (20)        0 2022-03-12 05:56:10.716856 xiaobai_config-1.0/simple_config/
--rw-r--r--   0 zrx        (501) staff       (20)      932 2022-03-12 05:55:46.000000 xiaobai_config-1.0/simple_config/__init__.py
--rw-r--r--   0 zrx        (501) staff       (20)     4309 2022-03-12 05:24:31.000000 xiaobai_config-1.0/simple_config/converter.py
--rw-r--r--   0 zrx        (501) staff       (20)     7279 2022-03-12 05:24:31.000000 xiaobai_config-1.0/simple_config/core.py
--rw-r--r--   0 zrx        (501) staff       (20)      257 2022-03-12 05:24:31.000000 xiaobai_config-1.0/simple_config/exceptions.py
-drwxr-xr-x   0 zrx        (501) staff       (20)        0 2022-03-12 05:56:10.718313 xiaobai_config-1.0/test/
--rw-r--r--   0 zrx        (501) staff       (20)     2167 2022-03-12 05:24:31.000000 xiaobai_config-1.0/test/test_config.py
--rw-r--r--   0 zrx        (501) staff       (20)      713 2022-03-12 05:24:31.000000 xiaobai_config-1.0/test/test_const.py
-drwxr-xr-x   0 zrx        (501) staff       (20)        0 2022-03-12 05:56:10.720786 xiaobai_config-1.0/xiaobai_config.egg-info/
--rw-r--r--   0 zrx        (501) staff       (20)      458 2022-03-12 05:56:10.000000 xiaobai_config-1.0/xiaobai_config.egg-info/PKG-INFO
--rw-r--r--   0 zrx        (501) staff       (20)      320 2022-03-12 05:56:10.000000 xiaobai_config-1.0/xiaobai_config.egg-info/SOURCES.txt
--rw-r--r--   0 zrx        (501) staff       (20)        1 2022-03-12 05:56:10.000000 xiaobai_config-1.0/xiaobai_config.egg-info/dependency_links.txt
--rw-r--r--   0 zrx        (501) staff       (20)       14 2022-03-12 05:56:10.000000 xiaobai_config-1.0/xiaobai_config.egg-info/top_level.txt
+drwxr-xr-x   0 zrx        (501) staff       (20)        0 2024-04-16 05:27:11.094785 xiaobai_config-1.1/
+-rw-r--r--   0 zrx        (501) staff       (20)     1074 2022-03-12 05:33:03.000000 xiaobai_config-1.1/LICENSE
+-rw-r--r--   0 zrx        (501) staff       (20)      422 2024-04-16 05:27:11.094589 xiaobai_config-1.1/PKG-INFO
+-rw-r--r--   0 zrx        (501) staff       (20)      101 2024-04-16 05:22:22.000000 xiaobai_config-1.1/README.md
+-rw-r--r--   0 zrx        (501) staff       (20)       38 2024-04-16 05:27:11.094828 xiaobai_config-1.1/setup.cfg
+-rw-r--r--   0 zrx        (501) staff       (20)      575 2024-04-16 05:22:22.000000 xiaobai_config-1.1/setup.py
+drwxr-xr-x   0 zrx        (501) staff       (20)        0 2024-04-16 05:27:11.093147 xiaobai_config-1.1/test/
+-rw-r--r--   0 zrx        (501) staff       (20)     2169 2024-04-16 05:27:02.000000 xiaobai_config-1.1/test/test_config.py
+-rw-r--r--   0 zrx        (501) staff       (20)      713 2022-03-12 05:24:31.000000 xiaobai_config-1.1/test/test_const.py
+drwxr-xr-x   0 zrx        (501) staff       (20)        0 2024-04-16 05:27:11.093938 xiaobai_config-1.1/xiaobai_config/
+-rw-r--r--   0 zrx        (501) staff       (20)      932 2024-04-16 05:27:02.000000 xiaobai_config-1.1/xiaobai_config/__init__.py
+-rw-r--r--   0 zrx        (501) staff       (20)     4309 2022-03-12 05:24:31.000000 xiaobai_config-1.1/xiaobai_config/converter.py
+-rw-r--r--   0 zrx        (501) staff       (20)     7279 2022-03-12 05:24:31.000000 xiaobai_config-1.1/xiaobai_config/core.py
+-rw-r--r--   0 zrx        (501) staff       (20)      257 2022-03-12 05:24:31.000000 xiaobai_config-1.1/xiaobai_config/exceptions.py
+drwxr-xr-x   0 zrx        (501) staff       (20)        0 2024-04-16 05:27:11.094371 xiaobai_config-1.1/xiaobai_config.egg-info/
+-rw-r--r--   0 zrx        (501) staff       (20)      422 2024-04-16 05:27:11.000000 xiaobai_config-1.1/xiaobai_config.egg-info/PKG-INFO
+-rw-r--r--   0 zrx        (501) staff       (20)      324 2024-04-16 05:27:11.000000 xiaobai_config-1.1/xiaobai_config.egg-info/SOURCES.txt
+-rw-r--r--   0 zrx        (501) staff       (20)        1 2024-04-16 05:27:11.000000 xiaobai_config-1.1/xiaobai_config.egg-info/dependency_links.txt
+-rw-r--r--   0 zrx        (501) staff       (20)       15 2024-04-16 05:27:11.000000 xiaobai_config-1.1/xiaobai_config.egg-info/top_level.txt
```

### Comparing `xiaobai_config-1.0/LICENSE` & `xiaobai_config-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaobai_config-1.0/setup.py` & `xiaobai_config-1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import setuptools
-import simple_config
+import xiaobai_config
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="xiaobai_config",
-    version=simple_config.__version__,
+    version=xiaobai_config.__version__,
     author="xiaobai",
     author_email="xiaobaizrx@gmail.com",
     description="A small tool to parse and store project config",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `xiaobai_config-1.0/simple_config/__init__.py` & `xiaobai_config-1.1/xiaobai_config/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,9 +27,9 @@
             if not key.isupper():
                 continue
             setattr(_const, key, getattr(current_module, key))
         return _const
 
 
 __name__ = "xiaobai_config"
-__all__ = ('Config', 'ConfigAttribute', 'const')
-__version__ = '1.0'
+__all__ = ('Config', 'ConfigAttribute', 'Const')
+__version__ = '1.1'
```

### Comparing `xiaobai_config-1.0/simple_config/converter.py` & `xiaobai_config-1.1/xiaobai_config/converter.py`

 * *Files identical despite different names*

### Comparing `xiaobai_config-1.0/simple_config/core.py` & `xiaobai_config-1.1/xiaobai_config/core.py`

 * *Files identical despite different names*

### Comparing `xiaobai_config-1.0/test/test_config.py` & `xiaobai_config-1.1/test/test_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 
-from simple_config import Config, ConfigAttribute, converter
-from simple_config import exceptions
+from xiaobai_config import Config, ConfigAttribute, converter
+from xiaobai_config import exceptions
 
 file_dir = os.path.dirname(os.path.abspath(__file__))
 
 
 class ProjectConfig(Config):
     ETCD_HOST = ConfigAttribute('ETCD_HOST')
     ETCD_PORT = ConfigAttribute('ETCD_PORT', get_converter=int)
```

### Comparing `xiaobai_config-1.0/test/test_const.py` & `xiaobai_config-1.1/test/test_const.py`

 * *Files identical despite different names*

