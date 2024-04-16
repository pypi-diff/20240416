# Comparing `tmp/ssht-0.9.1.tar.gz` & `tmp/ssht-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ssht-0.9.1.tar", last modified: Tue Jun 18 12:57:35 2019, max compression
+gzip compressed data, was "ssht-1.0.0.tar", max compression
```

## Comparing `ssht-0.9.1.tar` & `ssht-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,7 @@
-drwxr-xr-x   0 henk       (501) staff       (20)        0 2019-06-18 12:57:35.000000 ssht-0.9.1/
--rw-r--r--   0 henk       (501) staff       (20)      683 2019-06-18 12:57:35.000000 ssht-0.9.1/PKG-INFO
-drwxr-xr-x   0 henk       (501) staff       (20)        0 2019-06-18 12:57:35.000000 ssht-0.9.1/ssht.egg-info/
--rw-r--r--   0 henk       (501) staff       (20)      683 2019-06-18 12:57:35.000000 ssht-0.9.1/ssht.egg-info/PKG-INFO
--rw-r--r--   0 henk       (501) staff       (20)        1 2017-11-03 09:57:05.000000 ssht-0.9.1/ssht.egg-info/not-zip-safe
--rw-r--r--   0 henk       (501) staff       (20)      271 2019-06-18 12:57:35.000000 ssht-0.9.1/ssht.egg-info/SOURCES.txt
--rw-r--r--   0 henk       (501) staff       (20)       41 2019-06-18 12:57:35.000000 ssht-0.9.1/ssht.egg-info/entry_points.txt
--rw-r--r--   0 henk       (501) staff       (20)       32 2019-06-18 12:57:35.000000 ssht-0.9.1/ssht.egg-info/requires.txt
--rw-r--r--   0 henk       (501) staff       (20)        5 2019-06-18 12:57:35.000000 ssht-0.9.1/ssht.egg-info/top_level.txt
--rw-r--r--   0 henk       (501) staff       (20)        1 2019-06-18 12:57:35.000000 ssht-0.9.1/ssht.egg-info/dependency_links.txt
--rw-r--r--   0 henk       (501) staff       (20)     2364 2019-06-18 12:52:36.000000 ssht-0.9.1/README.md
--rw-r--r--   0 henk       (501) staff       (20)     1143 2019-06-18 12:55:33.000000 ssht-0.9.1/setup.py
--rw-r--r--   0 henk       (501) staff       (20)       95 2019-06-18 12:57:35.000000 ssht-0.9.1/setup.cfg
-drwxr-xr-x   0 henk       (501) staff       (20)        0 2019-06-18 12:57:35.000000 ssht-0.9.1/ssht/
--rw-r--r--   0 henk       (501) staff       (20)     3018 2019-06-18 12:52:36.000000 ssht-0.9.1/ssht/ssht.py
--rw-r--r--   0 henk       (501) staff       (20)     5038 2019-06-18 12:52:36.000000 ssht-0.9.1/ssht/plugins.py
--rw-r--r--   0 henk       (501) staff       (20)        0 2017-11-03 08:56:26.000000 ssht-0.9.1/ssht/__init__.py
+-rw-r--r--   0        0        0     1067 2017-11-03 08:56:26.000000 ssht-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2712 2024-04-16 11:04:18.341698 ssht-1.0.0/README.md
+-rw-r--r--   0        0        0     1140 2024-04-16 10:04:36.843952 ssht-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2017-11-03 08:56:26.000000 ssht-1.0.0/ssht/__init__.py
+-rw-r--r--   0        0        0     4953 2022-11-10 09:53:16.380116 ssht-1.0.0/ssht/plugins.py
+-rw-r--r--   0        0        0     3927 2022-11-10 09:53:16.380370 ssht-1.0.0/ssht/ssht.py
+-rw-r--r--   0        0        0     3599 1970-01-01 00:00:00.000000 ssht-1.0.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ssht-0.9.1/README.md` & `ssht-1.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,55 @@
 # ssht
 SSH client wrapper for easily connecting to hosts
 
-[![Build Status](https://travis-ci.org/hkraal/ssht.svg?branch=master)](https://travis-ci.org/hkraal/ssht)
 [![Coverage Status](https://coveralls.io/repos/github/hkraal/ssht/badge.svg?branch=master)](https://coveralls.io/github/hkraal/ssht?branch=master)
-[![Requirements Status](https://requires.io/github/hkraal/ssht/requirements.svg?branch=master)](https://requires.io/github/hkraal/ssht/requirements/?branch=master)
 ![](https://img.shields.io/pypi/pyversions/ssht.svg?style=flat)
 
 This wrapper for the well known `ssh` client makes it possible to connect to the right server with just typing a part of the host name. The external sources are queried using the search term and those matching the string will be presented as an option.
 
 Current supported sources:
 
 * JSON file
 * MySQL database
 * JSON API endpoint
+* Custom parser class
 
-# Installation
+### Installation
 
 Install ssht using pip:
 
-    pip install ssht
+    pip3 install ssht
 
 or if you want the latest version:
 
-    pip install https://github.com/hkraal/ssht/archive/master.zip
+    pip3 install https://github.com/hkraal/ssht/archive/master.zip
+
+
+### Usage
+
+    ssht [-h] name [-4] [-6] 
+    
+    positional arguments:
+      name        name of the host to connect to
+    
+    optional arguments:
+      -h, --help  show this help message and exit
+      -4          connect using ipv4 (skip dns if ipv4 address is defined)
+      -6          connect using ipv6 (skip dns of ipv6 address is defined)
+
+Example of a connection
+
+    $ ssht host01
+    1) root@host01.exmaple.com
+    2) host01.exmaple.com
+    Connect to: 1
+    Connecting to "host01.example.com"
+    root@host01:~$
+
+### Configuration
 
 Create ssht folder in home directory
 
     mkdir ~/.ssht
 
 Configure sources in ~/.ssht:
 
@@ -67,28 +90,37 @@
 			"url": "http://ssht-api.dev",
 			"headers": {
 				"Authentication": "bla:huk"
 			}
 		}
 	}
 
-# Usage
+**Define custom class**:
 
-    ssht [-h] name [-4] [-6] 
-    
-    positional arguments:
-      name        name of the host to connect to
-    
-    optional arguments:
-      -h, --help  show this help message and exit
-      -4          connect using ipv4 (skip dns if ipv4 address is defined)
-      -6          connect using ipv6 (skip dns of ipv6 address is defined)
+1) Create a Python package containing your class
 
-Example of a connection
+```
+from ssht.plugins import Parser, Host
 
-    $ ssht host01
-    1) root@host01.exmaple.com
-    2) host01.exmaple.com
-    Connect to: 1
-    Connecting to "host01.example.com"
-    root@host01:~$
 
+class ExampleParser(Parser):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._files = self.get_files('.custom')
+
+    def search(self, needle):
+        return [
+            Host(hostname='host01.example.com', ipv4='192.168.0.2'),
+        ]
+```
+
+2) Enable your class in `~/.ssht/config.json`
+
+```
+{
+    "parsers":
+    [
+        "ssht.plugins.JsonParser",
+        "ssht_provider.ExampleParser"
+    ]
+}
+```
```

### Comparing `ssht-0.9.1/setup.py` & `ssht-1.0.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,41 @@
-from setuptools import setup
+[tool.poetry]
+name = "ssht"
+version = "1.0.0"
+description = "SSH client wrapper for easily connecting to hosts"
+authors = ["Henk Kraal <hkraal@users.noreply.github.com>"]
+classifiers = [
+        'Development Status :: 4 - Beta',
+        'Environment :: Console',
+        'Intended Audience :: System Administrators',
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
+        'Topic :: System :: Shells',
+        'Topic :: Utilities',
+]
 
-setup(name='ssht',
-      version='0.9.1',
-      description='SSH client wrapper for easily connecting to hosts',
-      long_description='',
-      classifiers=[
-          'Development Status :: 4 - Beta',
-          'Intended Audience :: System Administrators',
-          'License :: OSI Approved :: MIT License',
-          'Programming Language :: Python :: 2.7',
-          'Programming Language :: Python :: 3.4',
-          'Programming Language :: Python :: 3.5',
-          'Programming Language :: Python :: 3.6',
-          'Topic :: System :: Shells',
-          'Topic :: Utilities',
-      ],
-      url='http://github.com/hkraal/ssht',
-      author='Henk Kraal',
-      author_email='hkraal@users.noreply.github.com',
-      license='MIT',
-      packages=['ssht'],
-      package_dir={'ssht': 'ssht'},
-      install_requires=[
-          'mysql-connector>=2.1.4',
-          'requests',
-      ],
-      include_package_data=True,
-      zip_safe=False,
-      entry_points={
-          'console_scripts': ['ssht=ssht.ssht:main'],
-      },
-      setup_requires=['pytest-runner'],
-      tests_require=['pytest'],
-      )
+readme = "README.md"
+packages = [
+    {include = "ssht"}
+]
+
+[tool.poetry.scripts]
+ssht = "ssht.ssht:main"
+
+[tool.poetry.dependencies]
+python = "~3.8|~3.9|~3.10|~3.11|~3.12"
+mysql-connector = "^2.2.9"
+requests = "^2.31.0"
+
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.4.3"
+pytest-mock = "^3.12.0"
+pytest-cov = "^4.1.0"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `ssht-0.9.1/ssht/plugins.py` & `ssht-1.0.0/ssht/plugins.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,22 +4,15 @@
 import os
 
 import mysql.connector
 import requests
 
 
 class Host(object):
-
-    def __init__(
-            self,
-            hostname,
-            port=None,
-            ipv4=None,
-            ipv6=None,
-            user=None):
+    def __init__(self, hostname, port=None, ipv4=None, ipv6=None, user=None):
         self.hostname = hostname
         self.port = port if port else None
         self.ipv4 = ipv4 if ipv4 else None
         self.ipv6 = ipv6 if ipv6 else None
         self.user = user if user else None
 
     @staticmethod
@@ -36,27 +29,26 @@
             return '{0}@{1}'.format(self.user, self.hostname)
         return self.hostname
 
     def match(self, needle):
         for search_field in ['hostname', 'ipv4', 'ipv6']:
             value = getattr(self, search_field, None)
             if value is not None and (
-                    fnmatch.fnmatch(value, needle) or needle in value):
+                fnmatch.fnmatch(value, needle) or needle in value
+            ):
                 return True
         return False
 
     def __repr__(self):
         if self.ipv4 is not None:
-            return '<Host: hostname={0}, ipv4={1}>'.format(
-                self.hostname, self.ipv4)
+            return '<Host: hostname={0}, ipv4={1}>'.format(self.hostname, self.ipv4)
         return '<Host: hostname={0}>'.format(self.hostname)
 
 
 class Parser(object):
-
     def __init__(self, path):
         '''
 
         :param path:
         '''
         self._path = path
         self._hosts = []
@@ -78,15 +70,14 @@
         content = ''
         with open(path, 'r') as fh:
             content = fh.read()
         return content
 
 
 class JsonParser(Parser):
-
     def __init__(self, *args, **kwargs):
         super(JsonParser, self).__init__(*args, **kwargs)
         self._files = self.get_files(ext='.json')
         self._load_data()
 
     def _load_data(self):
         '''
@@ -95,23 +86,23 @@
         for file_ in self._files:
             path = os.path.join(self._path, file_)
             logging.debug('Parsing "{0}"'.format(path))
 
             try:
                 d = json.loads(self._get_file_content(path))
                 logging.debug('Got: {0}'.format(d))
+                if not 'hosts' in d:
+                    return
                 for host in d['hosts']:
                     self._hosts.append(Host.factory(host))
-            except ValueError as ex:    # pragma: nocover
-                print('Invalid JSON file: {0}'.format(path))
-                logging.error(ex)
+            except ValueError as ex:  # pragma: nocover
+                logging.info(f'Config file {path} contains invalid JSON')
 
 
 class MySQLParser(Parser):  # pragma: nocover
-
     def __init__(self, *args, **kwargs):
         super(MySQLParser, self).__init__(*args, **kwargs)
         self._files = self.get_files(ext='.mysql')
         self._load_data()
 
     def _load_data(self):
         '''
@@ -145,17 +136,15 @@
                 try:
                     d = json.loads(fh.read())
                 except ValueError as ex:
                     print('Invalid JSON file: {0}'.format(path))
                     logging.error(ex)
                 if 'headers' not in d['config']:
                     d['config']['headers'] = {}
-                req = requests.get(
-                    d['config']['url'],
-                    headers=d['config']['headers'])
+                req = requests.get(d['config']['url'], headers=d['config']['headers'])
                 try:
                     res = req.json()
                 except ValueError as ex:
                     print('Invalid JSON response for: {0}'.format(path))
                     logging.error(ex)
                 if 'hosts' not in res:
                     print('No hosts in JSON response for: {0}'.format(path))
```

