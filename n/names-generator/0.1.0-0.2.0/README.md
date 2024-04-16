# Comparing `tmp/names_generator-0.1.0.tar.gz` & `tmp/names_generator-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/names_generator-0.1.0.tar", last modified: Fri Dec 11 16:31:28 2020, max compression
+gzip compressed data, was "names_generator-0.2.0.tar", last modified: Tue Apr 16 03:38:35 2024, max compression
```

## Comparing `names_generator-0.1.0.tar` & `names_generator-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2020-12-11 16:31:28.926318 names_generator-0.1.0/
--rw-r--r--   0 geoffrey   (501) staff       (20)     3402 2020-12-11 16:31:28.925850 names_generator-0.1.0/PKG-INFO
--rw-r--r--   0 geoffrey   (501) staff       (20)     1925 2020-12-03 15:21:57.000000 names_generator-0.1.0/README.rst
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2020-12-11 16:31:28.915363 names_generator-0.1.0/names_generator/
--rw-r--r--   0 geoffrey   (501) staff       (20)     3646 2020-12-11 16:30:45.000000 names_generator-0.1.0/names_generator/__init__.py
--rw-r--r--   0 geoffrey   (501) staff       (20)      807 2020-12-11 16:31:02.000000 names_generator-0.1.0/names_generator/__meta__.py
--rw-r--r--   0 geoffrey   (501) staff       (20)    50743 2020-12-03 01:43:54.000000 names_generator-0.1.0/names_generator/names.py
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2020-12-11 16:31:28.925161 names_generator-0.1.0/names_generator.egg-info/
--rw-r--r--   0 geoffrey   (501) staff       (20)     3402 2020-12-11 16:31:28.000000 names_generator-0.1.0/names_generator.egg-info/PKG-INFO
--rw-r--r--   0 geoffrey   (501) staff       (20)      336 2020-12-11 16:31:28.000000 names_generator-0.1.0/names_generator.egg-info/SOURCES.txt
--rw-r--r--   0 geoffrey   (501) staff       (20)        1 2020-12-11 16:31:28.000000 names_generator-0.1.0/names_generator.egg-info/dependency_links.txt
--rw-r--r--   0 geoffrey   (501) staff       (20)       56 2020-12-11 16:31:28.000000 names_generator-0.1.0/names_generator.egg-info/entry_points.txt
--rw-r--r--   0 geoffrey   (501) staff       (20)       14 2020-12-11 16:31:28.000000 names_generator-0.1.0/names_generator.egg-info/requires.txt
--rw-r--r--   0 geoffrey   (501) staff       (20)       16 2020-12-11 16:31:28.000000 names_generator-0.1.0/names_generator.egg-info/top_level.txt
--rw-r--r--   0 geoffrey   (501) staff       (20)       38 2020-12-11 16:31:28.926483 names_generator-0.1.0/setup.cfg
--rw-r--r--   0 geoffrey   (501) staff       (20)     2254 2020-12-03 02:18:56.000000 names_generator-0.1.0/setup.py
+drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2024-04-16 03:38:35.538097 names_generator-0.2.0/
+-rw-r--r--   0 geoffrey   (501) staff       (20)    11357 2020-12-03 00:30:31.000000 names_generator-0.2.0/LICENSE
+-rw-r--r--   0 geoffrey   (501) staff       (20)     2874 2024-04-16 03:38:35.537914 names_generator-0.2.0/PKG-INFO
+-rw-r--r--   0 geoffrey   (501) staff       (20)     1925 2020-12-03 15:21:57.000000 names_generator-0.2.0/README.rst
+drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2024-04-16 03:38:35.536648 names_generator-0.2.0/names_generator/
+-rw-r--r--   0 geoffrey   (501) staff       (20)     3686 2024-04-16 03:34:54.000000 names_generator-0.2.0/names_generator/__init__.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)      807 2024-04-16 03:35:59.000000 names_generator-0.2.0/names_generator/__meta__.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)    50743 2020-12-03 01:43:54.000000 names_generator-0.2.0/names_generator/names.py
+drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2024-04-16 03:38:35.537737 names_generator-0.2.0/names_generator.egg-info/
+-rw-r--r--   0 geoffrey   (501) staff       (20)     2874 2024-04-16 03:38:35.000000 names_generator-0.2.0/names_generator.egg-info/PKG-INFO
+-rw-r--r--   0 geoffrey   (501) staff       (20)      368 2024-04-16 03:38:35.000000 names_generator-0.2.0/names_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 geoffrey   (501) staff       (20)        1 2024-04-16 03:38:35.000000 names_generator-0.2.0/names_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 geoffrey   (501) staff       (20)       55 2024-04-16 03:38:35.000000 names_generator-0.2.0/names_generator.egg-info/entry_points.txt
+-rw-r--r--   0 geoffrey   (501) staff       (20)       14 2024-04-16 03:38:35.000000 names_generator-0.2.0/names_generator.egg-info/requires.txt
+-rw-r--r--   0 geoffrey   (501) staff       (20)       16 2024-04-16 03:38:35.000000 names_generator-0.2.0/names_generator.egg-info/top_level.txt
+-rw-r--r--   0 geoffrey   (501) staff       (20)       38 2024-04-16 03:38:35.538134 names_generator-0.2.0/setup.cfg
+-rw-r--r--   0 geoffrey   (501) staff       (20)     2518 2024-04-16 03:34:54.000000 names_generator-0.2.0/setup.py
+drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2024-04-16 03:38:35.537585 names_generator-0.2.0/tests/
+-rw-r--r--   0 geoffrey   (501) staff       (20)     1779 2024-04-16 03:34:54.000000 names_generator-0.2.0/tests/test_generator.py
```

### Comparing `names_generator-0.1.0/README.rst` & `names_generator-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `names_generator-0.1.0/names_generator/__init__.py` & `names_generator-0.2.0/names_generator/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 # standard libs
 import sys
 import random
 import logging
 
 # internal libs
-from .__meta__ import __version__, __description__, __authors__, __contact__
-from . import names
+from names_generator.__meta__ import __version__, __description__, __authors__, __contact__
+from names_generator import names
 
 # external libs
 from cmdkit.app import Application
 from cmdkit.cli import Interface
 
 
 # In the interest of keeping with the original implementation :)
@@ -78,30 +78,31 @@
         random.seed(seed)
     return format_names(random_names(), style=style)
 
 
 # Command-line interface implementation
 PROGRAM = 'generate_name'
 USAGE = f"""\
-usage: {PROGRAM} [-h] [-v] [--style NAME]
-Generate random name pairing.\
+Usage: 
+  {PROGRAM} [-h] [-v] [--style NAME]
+  Generate random name pairing.\
 """
 
 EPILOG = f"""\
 Documentation and issue tracking at:
 https://github.com/glentner/names_generator\
 """
 
 HELP = f"""\
 {USAGE}
 
-options:
--s, --style    NAME    Formatting (default: underscore).
--h, --help             Show this message and exit.
--v, --version          Show the version and exit.
+Options:
+  -s, --style    NAME    Formatting (default: underscore).
+  -h, --help             Show this message and exit.
+  -v, --version          Show the version and exit.
 
 {EPILOG}\
 """
 
 
 class NamesGeneratorApp(Application):
     """Top-level application class for `generate_name` console application."""
```

### Comparing `names_generator-0.1.0/names_generator/__meta__.py` & `names_generator-0.2.0/names_generator/__meta__.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,12 +7,12 @@
 #
 # You should have received a copy of the Apache License along with this program.
 # If not, see <https://www.apache.org/licenses/LICENSE-2.0>.
 
 """Metadata for names_generator package."""
 
 
-__version__   = '0.1.0'
+__version__   = '0.2.0'
 __authors__   = 'Geoffrey Lentner'
 __contact__   = 'glentner@purdue.edu'
 __license__   = 'Apache License'
 __description__ = 'Clone of the Moby/Docker random name generator as a Python package.'
```

### Comparing `names_generator-0.1.0/names_generator/names.py` & `names_generator-0.2.0/names_generator/names.py`

 * *Files identical despite different names*

### Comparing `names_generator-0.1.0/setup.py` & `names_generator-0.2.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -41,11 +41,15 @@
     long_description = long_description,
     long_description_content_type = 'text/x-rst',
     classifiers      = ['Development Status :: 5 - Production/Stable',
                         'Topic :: Software Development :: Libraries :: Application Frameworks',
                         'License :: OSI Approved :: Apache Software License',
                         'Programming Language :: Python :: 3.7',
                         'Programming Language :: Python :: 3.8',
-                        'Programming Language :: Python :: 3.9'],
+                        'Programming Language :: Python :: 3.9',
+                        'Programming Language :: Python :: 3.10',
+                        'Programming Language :: Python :: 3.11',
+                        'Programming Language :: Python :: 3.12',
+                        'Programming Language :: Python :: 3.13'],
     entry_points     = {'console_scripts': [f'generate_name=names_generator:main']},
-    install_requires = ['cmdkit>=2.1.2', ]
+    install_requires = ['cmdkit>=2.7.4', ]
 )
```

