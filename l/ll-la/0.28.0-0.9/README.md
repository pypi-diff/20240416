# Comparing `tmp/ll-la-0.28.0.tar.gz` & `tmp/ll-la-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ll-la-0.28.0.tar", last modified: Tue Apr 16 15:05:59 2024, max compression
+gzip compressed data, was "dist/ll-la-0.9.tar", last modified: Wed Jun 26 14:36:04 2019, max compression
```

## Comparing `ll-la-0.28.0.tar` & `ll-la-0.9.tar`

### file list

```diff
@@ -1,53 +1,20 @@
-drwxr-xr-x   0 walter     (501) staff       (20)        0 2024-04-16 15:05:59.477665 ll-la-0.28.0/
--rw-r--r--   0 walter     (501) staff       (20)     1140 2020-02-18 11:28:58.000000 ll-la-0.28.0/LICENSE.txt
--rw-r--r--   0 walter     (501) staff       (20)     1333 2024-04-16 15:05:59.477756 ll-la-0.28.0/PKG-INFO
--rw-r--r--   0 walter     (501) staff       (20)      514 2021-12-08 12:05:50.000000 ll-la-0.28.0/README.rst
--rw-r--r--   0 walter     (501) staff       (20)       92 2024-04-16 15:05:59.478057 ll-la-0.28.0/setup.cfg
--rw-r--r--   0 walter     (501) staff       (20)     2512 2024-04-16 15:03:04.000000 ll-la-0.28.0/setup.py
-drwxr-xr-x   0 walter     (501) staff       (20)        0 2024-04-16 15:05:59.469539 ll-la-0.28.0/src/
-drwxr-xr-x   0 walter     (501) staff       (20)        0 2024-04-16 15:05:59.469459 ll-la-0.28.0/src/ll/
-drwxr-xr-x   0 walter     (501) staff       (20)        0 2024-04-16 15:05:59.470881 ll-la-0.28.0/src/ll/la/
--rw-r--r--   0 walter     (501) staff       (20)   274433 2024-04-16 15:03:04.000000 ll-la-0.28.0/src/ll/la/__init__.py
--rw-r--r--   0 walter     (501) staff       (20)    63659 2024-04-16 15:03:04.000000 ll-la-0.28.0/src/ll/la/handlers.py
--rw-r--r--   0 walter     (501) staff       (20)   129600 2024-01-09 13:51:03.000000 ll-la-0.28.0/src/ll/la/vsql.py
-drwxr-xr-x   0 walter     (501) staff       (20)        0 2024-04-16 15:05:59.471788 ll-la-0.28.0/src/ll_la.egg-info/
--rw-r--r--   0 walter     (501) staff       (20)     1333 2024-04-16 15:05:59.000000 ll-la-0.28.0/src/ll_la.egg-info/PKG-INFO
--rw-r--r--   0 walter     (501) staff       (20)     1215 2024-04-16 15:05:59.000000 ll-la-0.28.0/src/ll_la.egg-info/SOURCES.txt
--rw-r--r--   0 walter     (501) staff       (20)        1 2024-04-16 15:05:59.000000 ll-la-0.28.0/src/ll_la.egg-info/dependency_links.txt
--rw-r--r--   0 walter     (501) staff       (20)        1 2019-06-26 14:24:03.000000 ll-la-0.28.0/src/ll_la.egg-info/not-zip-safe
--rw-r--r--   0 walter     (501) staff       (20)      125 2024-04-16 15:05:59.000000 ll-la-0.28.0/src/ll_la.egg-info/requires.txt
--rw-r--r--   0 walter     (501) staff       (20)        3 2024-04-16 15:05:59.000000 ll-la-0.28.0/src/ll_la.egg-info/top_level.txt
-drwxr-xr-x   0 walter     (501) staff       (20)        0 2024-04-16 15:05:59.477549 ll-la-0.28.0/test/
--rw-r--r--   0 walter     (501) staff       (20)    98350 2024-04-16 15:03:04.000000 ll-la-0.28.0/test/test_livingapi.py
--rw-r--r--   0 walter     (501) staff       (20)    18584 2023-12-07 15:50:09.000000 ll-la-0.28.0/test/test_vsql.py
--rw-r--r--   0 walter     (501) staff       (20)     3098 2023-12-07 15:50:09.000000 ll-la-0.28.0/test/test_vsql_attr.py
--rw-r--r--   0 walter     (501) staff       (20)     6771 2023-12-07 15:50:09.000000 ll-la-0.28.0/test/test_vsql_binop_add.py
--rw-r--r--   0 walter     (501) staff       (20)     5019 2023-12-07 15:50:09.000000 ll-la-0.28.0/test/test_vsql_binop_and.py
--rw-r--r--   0 walter     (501) staff       (20)     2524 2023-12-07 15:50:09.000000 ll-la-0.28.0/test/test_vsql_binop_bitand.py
--rw-r--r--   0 walter     (501) staff       (20)     2548 2023-12-07 15:50:09.000000 ll-la-0.28.0/test/test_vsql_binop_bitor.py
--rw-r--r--   0 walter     (501) staff       (20)      865 2023-12-07 15:50:09.000000 ll-la-0.28.0/test/test_vsql_binop_bitxor.py
--rw-r--r--   0 walter     (501) staff       (20)     5917 2023-12-07 15:50:09.000000 ll-la-0.28.0/test/test_vsql_binop_contains.py
--rw-r--r--   0 walter     (501) staff       (20)     2106 2023-12-07 15:50:09.000000 ll-la-0.28.0/test/test_vsql_binop_floordiv.py
--rw-r--r--   0 walter     (501) staff       (20)     5447 2023-12-07 15:50:09.000000 ll-la-0.28.0/test/test_vsql_binop_is.py
--rw-r--r--   0 walter     (501) staff       (20)     5603 2023-12-07 15:50:09.000000 ll-la-0.28.0/test/test_vsql_binop_isnot.py
--rw-r--r--   0 walter     (501) staff       (20)     1935 2023-12-07 15:50:09.000000 ll-la-0.28.0/test/test_vsql_binop_item.py
--rw-r--r--   0 walter     (501) staff       (20)     1912 2023-12-07 15:50:09.000000 ll-la-0.28.0/test/test_vsql_binop_mod.py
--rw-r--r--   0 walter     (501) staff       (20)     7513 2023-12-07 15:50:09.000000 ll-la-0.28.0/test/test_vsql_binop_mul.py
--rw-r--r--   0 walter     (501) staff       (20)     6128 2023-12-07 15:50:09.000000 ll-la-0.28.0/test/test_vsql_binop_notcontains.py
--rw-r--r--   0 walter     (501) staff       (20)     5191 2023-12-07 15:50:09.000000 ll-la-0.28.0/test/test_vsql_binop_or.py
--rw-r--r--   0 walter     (501) staff       (20)      774 2023-12-07 15:50:09.000000 ll-la-0.28.0/test/test_vsql_binop_shiftleft.py
--rw-r--r--   0 walter     (501) staff       (20)      875 2023-12-07 15:50:09.000000 ll-la-0.28.0/test/test_vsql_binop_shiftright.py
--rw-r--r--   0 walter     (501) staff       (20)     2675 2023-12-07 15:50:09.000000 ll-la-0.28.0/test/test_vsql_binop_sub.py
--rw-r--r--   0 walter     (501) staff       (20)     1731 2023-12-07 15:50:09.000000 ll-la-0.28.0/test/test_vsql_binop_truediv.py
--rw-r--r--   0 walter     (501) staff       (20)    20436 2023-12-07 15:50:09.000000 ll-la-0.28.0/test/test_vsql_cmp_eq.py
--rw-r--r--   0 walter     (501) staff       (20)    17052 2023-12-07 15:50:09.000000 ll-la-0.28.0/test/test_vsql_cmp_ge.py
--rw-r--r--   0 walter     (501) staff       (20)    16805 2023-12-07 15:50:09.000000 ll-la-0.28.0/test/test_vsql_cmp_gt.py
--rw-r--r--   0 walter     (501) staff       (20)    17013 2023-12-07 15:50:09.000000 ll-la-0.28.0/test/test_vsql_cmp_le.py
--rw-r--r--   0 walter     (501) staff       (20)    16765 2023-12-07 15:50:09.000000 ll-la-0.28.0/test/test_vsql_cmp_lt.py
--rw-r--r--   0 walter     (501) staff       (20)    19894 2023-12-07 15:50:09.000000 ll-la-0.28.0/test/test_vsql_cmp_ne.py
--rw-r--r--   0 walter     (501) staff       (20)    20706 2023-12-07 15:50:09.000000 ll-la-0.28.0/test/test_vsql_func.py
--rw-r--r--   0 walter     (501) staff       (20)     3258 2023-12-07 15:50:09.000000 ll-la-0.28.0/test/test_vsql_meth.py
--rw-r--r--   0 walter     (501) staff       (20)     9501 2023-12-07 15:50:09.000000 ll-la-0.28.0/test/test_vsql_slice.py
--rw-r--r--   0 walter     (501) staff       (20)      679 2023-12-07 15:50:09.000000 ll-la-0.28.0/test/test_vsql_unop_bitnot.py
--rw-r--r--   0 walter     (501) staff       (20)     1580 2023-12-07 15:50:09.000000 ll-la-0.28.0/test/test_vsql_unop_neg.py
--rw-r--r--   0 walter     (501) staff       (20)     2520 2023-12-07 15:50:09.000000 ll-la-0.28.0/test/test_vsql_unop_not.py
+drwxr-xr-x   0 walter     (501) staff       (20)        0 2019-06-26 14:36:04.000000 ll-la-0.9/
+-rw-r--r--   0 walter     (501) staff       (20)     1503 2019-06-26 14:36:04.000000 ll-la-0.9/PKG-INFO
+-rw-r--r--   0 walter     (501) staff       (20)      486 2019-04-12 07:49:50.000000 ll-la-0.9/README.rst
+-rw-r--r--   0 walter     (501) staff       (20)       92 2019-06-26 14:36:04.000000 ll-la-0.9/setup.cfg
+-rw-r--r--   0 walter     (501) staff       (20)     2369 2019-06-26 14:35:02.000000 ll-la-0.9/setup.py
+drwxr-xr-x   0 walter     (501) staff       (20)        0 2019-06-26 14:36:04.000000 ll-la-0.9/src/
+drwxr-xr-x   0 walter     (501) staff       (20)        0 2019-06-26 14:36:04.000000 ll-la-0.9/src/ll/
+drwxr-xr-x   0 walter     (501) staff       (20)        0 2019-06-26 14:36:04.000000 ll-la-0.9/src/ll/la/
+-rw-r--r--   0 walter     (501) staff       (20)    74679 2019-06-26 14:35:02.000000 ll-la-0.9/src/ll/la/__init__.py
+-rw-r--r--   0 walter     (501) staff       (20)    36984 2019-04-12 07:51:19.000000 ll-la-0.9/src/ll/la/handlers.py
+-rw-r--r--   0 walter     (501) staff       (20)    24664 2019-04-12 07:49:50.000000 ll-la-0.9/src/ll/la/vsql.py
+drwxr-xr-x   0 walter     (501) staff       (20)        0 2019-06-26 14:36:04.000000 ll-la-0.9/src/ll_la.egg-info/
+-rw-r--r--   0 walter     (501) staff       (20)     1503 2019-06-26 14:36:04.000000 ll-la-0.9/src/ll_la.egg-info/PKG-INFO
+-rw-r--r--   0 walter     (501) staff       (20)      310 2019-06-26 14:36:04.000000 ll-la-0.9/src/ll_la.egg-info/SOURCES.txt
+-rw-r--r--   0 walter     (501) staff       (20)        1 2019-06-26 14:36:04.000000 ll-la-0.9/src/ll_la.egg-info/dependency_links.txt
+-rw-r--r--   0 walter     (501) staff       (20)        1 2019-06-26 14:24:03.000000 ll-la-0.9/src/ll_la.egg-info/not-zip-safe
+-rw-r--r--   0 walter     (501) staff       (20)       48 2019-06-26 14:36:04.000000 ll-la-0.9/src/ll_la.egg-info/requires.txt
+-rw-r--r--   0 walter     (501) staff       (20)        3 2019-06-26 14:36:04.000000 ll-la-0.9/src/ll_la.egg-info/top_level.txt
+drwxr-xr-x   0 walter     (501) staff       (20)        0 2019-06-26 14:36:04.000000 ll-la-0.9/test/
+-rw-r--r--   0 walter     (501) staff       (20)    44330 2019-04-12 07:51:19.000000 ll-la-0.9/test/test_livingapi.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `ll-la-0.28.0/PKG-INFO` & `ll-la-0.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,41 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: ll-la
-Version: 0.28.0
+Version: 0.9
 Summary: Python API for LivingApps
 Home-page: http://github.com/LivingLogic/LivingApps.Python.LivingAPI
 Author: Walter Doerwald
 Author-email: walter@livinglogic.de
 License: MIT
+Description: ``ll.la`` provides a Python API for the LivingApps system
+        (see http://www.living-apps.de/ or http://www.living-apps.com/ for more info).
+        
+        ``ll.la`` allows you to fetch the configured data sources from a template,
+        create new records, and update and delete existing records all from your Python
+        prompt (or script).
+        
+        For more info about LivingApps and this Python SDK, see
+        https://my.living-apps.de/docs/PythonSDK.html (in german).
+        
+        
+        0.9 (2019-06-26)
+        ----------------
+        
+        * Fixed shortcut attributes for the ``Globals`` object.
+        
+        * First Cheeseshop release.
+        
+        
+        
 Keywords: LivingApps
-Classifier: Development Status :: 5 - Production/Stable
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
-Provides-Extra: db
-License-File: LICENSE.txt
-
-``ll.la`` provides a Python API for the LivingApps system
-(see http://www.living-apps.de/ or http://www.living-apps.com/ for more info).
-
-``ll.la`` allows you to fetch the configured data sources from a template,
-create new records, and update and delete existing records all from your Python
-prompt (or script).
-
-For more info about LivingApps and this Python SDK, see
-https://my.living-apps.de/docs/PythonSDK.html (in german).
-
-
-0.28.0 (2024-04-16)
--------------------
-
-* Add method ``User.change()``.
-
-
+Requires-Python: >=3.6
```

### Comparing `ll-la-0.28.0/setup.py` & `ll-la-0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 prompt (or script).
 
 For more info about LivingApps and this Python SDK, see
 https://my.living-apps.de/docs/PythonSDK.html (in german).
 """
 
 CLASSIFIERS = """
-Development Status :: 5 - Production/Stable
+Development Status :: 3 - Alpha
 Intended Audience :: Developers
 License :: OSI Approved :: MIT License
 Operating System :: OS Independent
 Programming Language :: Python
 Programming Language :: Python :: 3 :: Only
 Programming Language :: Python :: 3
-Programming Language :: Python :: 3.8
+Programming Language :: Python :: 3.6
 Topic :: Software Development :: Libraries :: Python Modules
 Topic :: Internet :: WWW/HTTP
 """
 
 KEYWORDS = """
 LivingApps
 """
@@ -50,34 +50,29 @@
 description = re.subn(":[a-z]+:`~?([-a-zA-Z0-9_./]+)`", "``\\1``", description)[0]
 
 # Expand tabs (so they won't show up as 8 spaces in the Windows installer)
 description = description.expandtabs(2)
 
 args = dict(
 	name="ll-la",
-	version="0.28.0",
+	version="0.9",
 	description="Python API for LivingApps",
 	long_description=description,
 	author="Walter Doerwald",
 	author_email="walter@livinglogic.de",
 	url="http://github.com/LivingLogic/LivingApps.Python.LivingAPI",
 	license="MIT",
-	python_requires=">=3.8",
+	python_requires=">=3.6",
 	classifiers=sorted({c for c in CLASSIFIERS.strip().splitlines() if c.strip() and not c.strip().startswith("#")}),
 	keywords=", ".join(sorted({k.strip() for k in KEYWORDS.strip().splitlines() if k.strip() and not k.strip().startswith("#")})),
 	package_dir={"": "src"},
 	packages=["ll.la"],
 	install_requires=[
-		"ll-xist >= 5.75",
+		"ll-xist >= 5.45",
 		"requests >= 2.21.0",
-		"geocoder >= 1.30.1",
-		"Pillow >= 6.1.0",
-		"validators >= 0.18.2",
+		"geocoder >= 1.30.1"
 	],
-	extras_require={
-		"db": ["cx_Oracle >= 8.0", "psycopg[binary] >= 3.0.5"],
-	},
 	zip_safe=False,
 )
 
 if __name__ == "__main__":
 	setuptools.setup(**args)
```

### Comparing `ll-la-0.28.0/src/ll/la/handlers.py` & `ll-la-0.9/src/ll/la/handlers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # cython: language_level=3, always_allow_keywords=True
 
-## Copyright 2016-2024 by LivingLogic AG, Bayreuth/Germany
+## Copyright 2016-2019 by LivingLogic AG, Bayreuth/Germany
 ##
 ## All Rights Reserved
 
 """
 :mod:`handlers` provides various handler classes for talking to LivingApps.
 
 :class:`Handler` is the base class of all handler classes. Subclasses are:
@@ -26,58 +26,39 @@
 :class:`FileHandler`
 	This is used to store LivingApps meta data in the local file system.
 
 	This makes it possible to import and export internal and view templates
 	and their configuration into and out of LivingApps.
 """
 
-import os, datetime, pathlib, itertools, json, mimetypes, operator, warnings, random
+import os, io, datetime, pathlib, itertools, json, mimetypes, operator, warnings
 
 import requests, requests.exceptions # This requires :mod:`request`, which you can install with ``pip install requests``
 
 from ll import url, ul4c, ul4on # This requires the :mod:`ll` package, which you can install with ``pip install ll-xist``
 
 try:
 	from ll import orasql
 except ImportError:
 	orasql = None
 
-orasql_required_message = "ll.orasql required (install via `pip install ll-xist`)"
-
-try:
-	import psycopg
-except ImportError:
-	psycopg = None
-
-try:
-	from psycopg import rows
-except ImportError:
-	rows = None
-
-psycopg_required_message = "psycopg required (install via `pip install 'psycopg[binary]'`)"
-
 from ll import la
 
 from ll.la import vsql
 
 
 __docformat__ = "reStructuredText"
 
 __all__ = ["Handler", "HTTPHandler", "DBHandler", "FileHandler"]
 
 
 ###
 ### Utility functions and classes
 ###
 
-def uuid():
-	now = datetime.datetime.now()
-	return f"{int(now.timestamp()):08x}{now.microsecond & 0xffff:04x}{random.randint(0, (1<<(12*4))-1):012x}"
-
-
 def raise_403(response):
 	"""
 	Raise an HTTP exception with the status code 403 (i.e. "Forbidden").
 
 	(This is used if the HTTP interface would redirect us to a different page,
 	which we don't want).
 	"""
@@ -92,112 +73,92 @@
 class Handler:
 	"""
 	A :class:`Handler` object handles communication with a LivingApps system.
 	"""
 
 	def __init__(self):
 		self.globals = None
-		registry = {
-			"de.livinglogic.livingapi.globals": self._loadglobals,
-		}
-		self.ul4on_decoder = ul4on.Decoder(registry)
-
-	def reset(self):
-		"""
-		Reset the handler to the initial state.
-
-		This reset the UL4ON decoder.
-		"""
-		self.ul4on_decoder.reset()
-
-	def commit(self):
-		pass
-
-	def rollback(self):
-		pass
-
-	def __enter__(self):
-		return self
-
-	def __exit__(self, exc_type, exc_value, traceback):
-		self.reset()
-		if exc_type is not None:
-			self.rollback()
-		else:
-			self.commit()
 
 	def get(self, *path, **params):
 		warnings.warn("The method get() is deprecated, please use viewtemplate_data() instead.")
 		return self.viewtemplate_data(*path, **params)
 
 	def viewtemplate_data(self, *path, **params):
 		raise NotImplementedError
 
-	def loadinternaltemplates(self, tpl_uuid):
+	def meta_data(self, *appids):
 		raise NotImplementedError
 
-	def viewtemplate_params_incremental_data(self, globals, id):
-		return None
-
-	def emailtemplate_params_incremental_data(self, globals, id):
-		return None
-
-	def app_params_incremental_data(self, app):
-		return None
-
-	def view_layout_controls_incremental_data(self, view):
-		return None
-
-	def app_child_controls_incremental_data(self, app):
-		return None
-
-	def app_menus_incremental_data(self, app):
-		return None
-
-	def app_panels_incremental_data(self, app):
-		return None
-
-	def record_attachments_incremental_data(self, id):
-		return None
+	def file(self, source):
+		"""
+		Create a :class:`~ll.la.File` object from :obj:`source`.
 
-	def meta_data(self, *appids, records=False):
-		raise NotImplementedError
+		:obj:`source` can be :class:`pathlib.Path` or :class:`os.PathLike` object,
+		an :class:`~ll.url.URL` object or a stream (i.e. an object with a
+		:meth:`read` method and a :attr:`name` attribute.
+		"""
+		path = None
+		stream = None
+		mimetype = None
+		if isinstance(source, pathlib.Path):
+			content = source.read_bytes()
+			filename = source.name
+			path = str(source.resolve())
+		elif isinstance(source, str):
+			with open(source, "rb") as f:
+				content = f.read()
+			filename = os.path.basename(source)
+			path = source
+		elif isinstance(source, os.PathLike):
+			path = source.__fspath__()
+			with open(path, "rb") as f:
+				content = f.read()
+			filename = os.path.basename(path)
+		elif isinstance(source, url.URL):
+			filename = source.file
+			with source.openread() as r:
+				content = r.read()
+				stream = io.BytesIO(content)
+		else:
+			content = source.read()
+			if source.name:
+				filename = os.path.basename(source.name)
+			else:
+				filename = "Dummy"
+			stream = source
+		if mimetype is None:
+			mimetype = mimetypes.guess_type(filename, strict=False)[0]
+		file = la.File(filename=filename, mimetype=mimetype)
+		if file.mimetype.startswith("image/"):
+			from PIL import Image # This requires :mod:`Pillow`, which you can install with ``pip install pillow``
+			if stream:
+				stream.seek(0)
+			with Image.open(path or stream) as img:
+				file.width = img.size[0]
+				file.height = img.size[1]
+		file._content = content
+		file.handler = self
+		return file
 
-	def _geofrominfo(self, info:str) -> la.Geo:
+	def _geofrominfo(self, info):
 		import geocoder # This requires the :mod:`geocoder` module, install with ``pip install geocoder``
-		provider = geocoder.osm
-		result = provider(info, language="de")
-		if not result.error and result.lat and result.lng and result.address:
-			return la.Geo(result.lat, result.lng, result.address)
+		for provider in (geocoder.google, geocoder.osm):
+			result = provider(info, language="de")
+			if not result.error and result.lat and result.lng and result.address:
+				return la.Geo(result.lat, result.lng, result.address)
 		return None
 
-	def _geofromlatlong(self, lat:float, long:float) -> la.Geo:
+	def _geofromlatlong(self, lat, long):
 		import geocoder # This requires the :mod:`geocoder` module, install with ``pip install geocoder``
-		provider = geocoder.osm
-		result = provider([lat, long], method="reverse", language="de")
-		if not result.error and result.lat and result.lng and result.address:
-			return la.Geo(result.lat, result.lng, result.address)
+		for provider in (geocoder.google, geocoder.osm):
+			result = provider([lat, long], method="reverse", language="de")
+			if not result.error and result.lat and result.lng and result.address:
+				return la.Geo(result.lat, result.lng, result.address)
 		return None
 
-	def _geofromstring(self, s:str) -> la.Geo:
-		parts = s.split(",", 2)
-		if len(parts) < 2:
-			return self._geofrominfo(s)
-		else:
-			try:
-				lat = float(parts[0])
-				long = float(parts[1])
-			except ValueError:
-				return self._geofrominfo(s)
-			else:
-				if len(parts) == 2:
-					return self._geofromlatlong(lat, long)
-				else:
-					return la.Geo(lat, long, parts[2].strip())
-
 	def geo(self, lat=None, long=None, info=None):
 		"""
 		Create a :class:`~ll.la.Geo` object from :obj:`lat`/:obj`long` or :obj:`info`.
 
 		Example::
 
 			>>> from ll import la
@@ -215,392 +176,170 @@
 			return self._geofrominfo(lat)
 		# Get description from coordinates
 		elif lat is not None and long is not None and info is None:
 			return self._geofromlatlong(lat, long)
 		else:
 			raise TypeError("geo() requires either (lat, long) arguments or a (info) argument")
 
-	def seq(self):
-		raise NotImplementedError
-
-	def appseq(self, app):
-		raise NotImplementedError
-
 	def save_record(self, record):
 		raise NotImplementedError
 
 	def delete_record(self, record):
 		raise NotImplementedError
 
 	def _executeaction(self, record, actionidentifier):
 		raise NotImplementedError
 
 	def file_content(self, file):
 		raise NotImplementedError
 
-	def save_app(self, app, recursive=True):
-		raise NotImplementedError
-
 	def save_file(self, file):
 		raise NotImplementedError
 
-	def save_parameter(self, parameter, recursive=True):
-		raise NotImplementedError
-
 	def save_internaltemplate(self, internaltemplate, recursive=True):
 		raise NotImplementedError
 
 	def save_viewtemplate(self, viewtemplate, recursive=True):
 		raise NotImplementedError
 
-	def delete_viewtemplate(self, viewtemplate):
-		raise NotImplementedError
-
-	def delete_internaltemplate(self, internaltemplate):
-		raise NotImplementedError
-
-	def save_datasourceconfig(self, datasource, recursive=True):
+	def save_datasource(self, datasource, recursive=True):
 		raise NotImplementedError
 
 	def save_datasourcechildren(self, datasourcechildren, recursive=True):
 		raise NotImplementedError
 
-	def change_user(self, lang, oldpassword, newpassword, newemail):
-		raise NotImplementedError
-
-	def fetch_templates(self, app):
-		return la.attrdict()
-
-	def fetch_librarytemplates(self):
-		return la.attrdict()
-
-	def fetch_libraryparams(self):
-		return la.attrdict()
-
-	def fetch_viewtemplate_params(self, globals):
-		return la.attrdict()
+	def _loadfile(self):
+		file = la.File()
+		file.handler = self
+		return file
 
-	def fetch_emailtemplate_params(self, globals):
-		return la.attrdict()
-
-	def _loadglobals(self, id=None):
-		globals = la.Globals(id=id)
+	def _loadglobals(self):
+		globals = la.Globals()
 		globals.handler = self
 		return globals
 
 	def _loaddump(self, dump):
-		dump = self.ul4on_decoder.loads(dump)
-		if isinstance(dump, dict):
-			dump = la.attrdict(dump)
-			if "datasources" in dump:
-				dump.datasources = la.attrdict(dump.datasources)
+		registry = {
+			"de.livingapps.appdd.file": self._loadfile,
+			"de.livinglogic.livingapi.file": self._loadfile,
+			"de.livingapps.appdd.globals": self._loadglobals,
+			"de.livinglogic.livingapi.globals": self._loadglobals,
+		}
+		dump = ul4on.loads(dump, registry)
+		dump = la.attrdict(dump)
+		if "datasources" in dump:
+			dump.datasources = la.attrdict(dump.datasources)
 		return dump
 
 
 class DBHandler(Handler):
-	def __init__(self, *, connection=None, connectstring=None, connection_postgres=None, connectstring_postgres=None, uploaddir=None, ide_account=None, ide_id=None):
-		"""
-		Create a new :class:`DBHandler`.
-
-		For the database connection pass either ``connection`` with an
-		:mod:`~ll.orasql` connection or ``connectstring`` with a connecstring.
-
-		For a connection to the Postgres database pass either
-		``connection_postgres`` with a :mod:`psycopg` connection or
-		``connectstring_postgres`` with a connecstring. If you pass neither,
-		functionality that requires the Postgres database (like template libraries)
-		will not be available and will fail if used.
-
-		``uploaddir`` must be an ``ssh`` URL specifying the upload directory
-		on the web server. If no uploads will be made, it can also be :const:`None`.
-
-		To use a user account either specify ``ide_account`` which must be the
-		account name (i.e. the email address) of the user or ``ide_id`` which
-		must be the users database id. If neither is given only public view
-		templates can be fetched.
-		"""
-
+	def __init__(self, connectstring, uploaddirectory, account):
 		super().__init__()
-
-		now = datetime.datetime.now()
-		self.requestid = uuid()
-		if connection is not None:
-			if connectstring is not None:
-				raise ValueError("Specify connectstring or connection, but not both")
-			self._db = connection
-		elif connectstring is not None:
-			self._db = connectstring
-		else:
-			self._db = None
-
-		if connection_postgres is not None:
-			if connectstring_postgres is not None:
-				raise ValueError("Specify connectstring_postgres or connection_postgres, but not both")
-			self._db_pg = connection_postgres
-		elif connectstring_postgres is not None:
-			self._db_pg = connectstring_postgres
-		else:
-			self._db_pg = None
-
-		if uploaddir is not None:
-			uploaddir = url.URL(uploaddir)
-		self.uploaddir = uploaddir
-
-		self._varchars = None
+		if orasql is None:
+			raise ImportError("ll.orasql required")
+		self.db = orasql.connect(connectstring, readlobs=True)
+		self.uploaddirectory = url.URL(uploaddirectory)
+		self.varchars = self.db.gettype("LL.VARCHARS")
 		self.urlcontext = None
 
 		# Procedures
 		self.proc_data_insert = orasql.Procedure("LIVINGAPI_PKG.DATA_INSERT")
 		self.proc_data_update = orasql.Procedure("LIVINGAPI_PKG.DATA_UPDATE")
 		self.proc_data_delete = orasql.Procedure("LIVINGAPI_PKG.DATA_DELETE")
-		self.proc_appparameter_save = orasql.Procedure("APPPARAMETER_PKG.APPPARAMETER_SAVE_LA")
-		self.proc_appparameter_delete = orasql.Procedure("APPPARAMETER_PKG.APPPARAMETER_DELETE")
 		self.proc_dataaction_execute = orasql.Procedure("LIVINGAPI_PKG.DATAACTION_EXECUTE")
-		self.proc_upload_upr_insert = orasql.Procedure("UPLOAD_PKG.UPLOAD_UPR_INSERT")
-		self.proc_appparameter_import_waf = orasql.Procedure("APPPARAMETER_PKG.APPPARAMETER_IMPORT")
-		self.proc_identity_change = orasql.Procedure("LIVINGAPI_PKG.IDENTITY_CHANGE")
+		self.proc_upload_insert = orasql.Procedure("UPLOAD_PKG.UPLOAD_INSERT")
+		self.proc_internaltemplate_import = orasql.Procedure("INTERNALTEMPLATE_PKG.INTERNALTEMPLATE_IMPORT")
 		self.proc_viewtemplate_import = orasql.Procedure("VIEWTEMPLATE_PKG.VIEWTEMPLATE_IMPORT")
-		self.proc_viewtemplate_delete = orasql.Procedure("VIEWTEMPLATE_PKG.VIEWTEMPLATE_DELETE")
 		self.proc_datasource_import = orasql.Procedure("DATASOURCE_PKG.DATASOURCE_IMPORT")
 		self.proc_datasourcechildren_import = orasql.Procedure("DATASOURCE_PKG.DATASOURCECHILDREN_IMPORT")
 		self.proc_dataorder_import = orasql.Procedure("DATASOURCE_PKG.DATAORDER_IMPORT")
 		self.proc_dataorder_delete = orasql.Procedure("DATASOURCE_PKG.DATAORDER_DELETE")
 		self.proc_vsqlsource_insert = orasql.Procedure("VSQL_PKG.VSQLSOURCE_INSERT")
 		self.proc_vsql_insert = orasql.Procedure("VSQL_PKG.VSQL_INSERT")
-		self.proc_init = orasql.Procedure("LIVINGAPI_PKG.INIT")
-		self.proc_clear_all = orasql.Procedure("LIVINGAPI_PKG.CLEAR_ALL")
-		self.func_seq = orasql.Function("LIVINGAPI_PKG.SEQ")
-		self.func_template_seq = orasql.Function("LIVINGAPI_PKG.TEMPLATE_SEQ_BY_TPL_UUID")
-
-		self.custom_procs = {} # For the insert/update/delete procedures of system templates
-		self.internaltemplates = {} # Maps ``tpl_uuid`` to template dictionary
-		self.viewtemplate_params = {} # Maps ``vt_id`` to parameter dictionary
-		self.emailtemplate_params = {} # Maps ``et_id`` to parameter dictionary
-		self.librarytemplates = None # Maps ``lt_id`` to templates
-		self.libraryparams = None # Maps ``lp_id`` to :class:`AppParameter`
-
-		if ide_id is not None:
-			if ide_account is not None:
-				raise ValueError("Specify ide_id or ide_account, but not both")
-			self.ide_id = ide_id
-		elif ide_account is not None:
+
+		self.custom_procs = {}
+
+		if account is None:
+			self.ide_id = None
+		else:
 			c = self.cursor()
-			c.execute("select ide_id from identity where ide_account = :ide_account", ide_account=ide_account)
+			c.execute("select ide_id from identity where ide_account = :account", account=account)
 			r = c.fetchone()
 			if r is None:
-				raise ValueError(f"no user {ide_account!r}")
+				raise ValueError(f"no user {account!r}")
 			self.ide_id = r.ide_id
-		else:
-			self.ide_id = None
 
 	def __repr__(self):
-		return f"<{self.__class__.__module__}.{self.__class__.__qualname__} connectstring={self.db.connectstring()!r} ide_id={self.ide_id!r} at {id(self):#x}>"
-
-	@property
-	def db(self):
-		if self._db is None:
-			raise ValueError("No Oracle database connection available")
-		elif isinstance(self._db, str):
-			if orasql is None:
-				raise ImportError(orasql_required_message)
-			self._db = orasql.connect(self._db, readlobs=True)
-		return self._db
-
-	@property
-	def db_pg(self):
-		if self._db_pg is None:
-			raise ValueError("No Postgres database connection available")
-		elif isinstance(self._db_pg, str):
-			if psycopg is None:
-				raise ImportError(psycopg_required_message)
-			self._db_pg = psycopg.connect(self._db_pg)
-		return self._db_pg
-
-	@property
-	def varchars(self):
-		if self._varchars is None:
-			self._varchars = self.db.gettype("LL.VARCHARS")
-		return self._varchars
+		return f"<{self.__class__.__module__}.{self.__class__.__qualname__} connectstring={self.db.connectstring()!r} at {id(self):#x}>"
 
 	def cursor(self):
-		return self.db.cursor(readlobs=True)
-
-	def cursor_pg(self, row_factory=None):
-		if row_factory is None:
-			if rows is None:
-				raise ImportError(psycopg_required_message)
-			row_factory = rows.tuple_row
-		return self.db_pg.cursor(row_factory=row_factory)
+		return self.db.cursor()
 
 	def commit(self):
-		if self._db is not None:
-			self.db.commit()
-		if self._db_pg is not None:
-			self.db_pg.commit()
-
-	def rollback(self):
-		if self.db is not None:
-			self.db.rollback()
-		if self.db_pg is not None:
-			self.db_pg.rollback()
-
-	def reset(self):
-		super().reset()
-		self.proc_clear_all(self.cursor())
-
-	def seq(self):
-		c = self.cursor()
-		(value, r) = self.func_seq(c)
-		return int(value)
-
-	def appseq(self, app):
-		c = self.cursor()
-		(value, r) = self.func_template_seq(c, app.id)
-		return int(value)
+		self.db.commit()
 
 	def save_app(self, app, recursive=True):
 		# FIXME: Save the app itself
 		if recursive:
 			if app.internaltemplates is not None:
 				for internaltemplate in app.internaltemplates.values():
 					self.save_internaltemplate(internaltemplate, recursive=recursive)
 			if app.viewtemplates is not None:
 				for viewtemplate in app.viewtemplates.values():
 					self.save_viewtemplate(viewtemplate, recursive=recursive)
-			if app._ownparams is not None:
-				for param in app._ownparams.values():
-					self.save_parameter(param)
 
 	def save_file(self, file):
-		if file.internal_id is None:
+		if file.internalid is None:
 			if file._content is None:
 				raise ValueError(f"Can't save {file!r} without content!")
 			c = self.cursor()
-			r = self.proc_upload_upr_insert(
+			r = self.proc_upload_insert(
 				c,
 				c_user=self.ide_id,
 				p_upl_orgname=file.filename,
 				p_upl_size=len(file._content),
 				p_upl_mimetype=file.mimetype,
 				p_upl_width=file.width,
 				p_upl_height=file.height,
 			)
 			if self.urlcontext is None:
 				self.urlcontext = url.Context()
-			with (self.uploaddir/r.p_upl_name).open("wb", context=self.urlcontext) as f:
+			with (self.uploaddirectory/r.p_upl_name).open("wb", context=self.urlcontext) as f:
 				f.write(file._content)
-			file.context_id = r.p_context_id
-			file.id = f"{r.p_upr_path}/{r.p_upl_id}"
-			file.internal_id = r.p_upl_id
+			file.internalid = r.p_upl_id
 
 	def file_content(self, file):
+		upr_id = file.url.rsplit("/")[-1]
+		c = self.cursor()
+		c.execute(
+			"select u.upl_name from upload u, uploadref ur where u.upl_id=ur.upl_id and ur.upr_id = :upr_id",
+			upr_id=upr_id,
+		)
+		r = c.fetchone()
+		if r is None:
+			raise ValueError(f"no such file {file.url!r}")
 		with url.Context():
-			u = self.uploaddir/file.storagefilename
+			u = self.uploaddirectory/r.upl_name
 			return u.openread().read()
 
-	def _save_vsql_ast(self, vsqlexpr, required_datatype=None, cursor=None, vs_id_super=None, vs_order=None, vss_id=None, pos=None):
-		"""
-		Save the vSQL expression :obj:`vsqlexpr`.
-
-		``cursor``, ``vs_id_super``, ``vs_order``, ``vss_id`` and ``pos`` are used
-		internally for recursive calls and should not be passed by the user.
-		"""
-		if cursor is None:
-			cursor = self.cursor()
-		source = vsqlexpr.source()
-		sourcelen = len(source)
-		if pos is None:
-			pos = 0
-		finalpos = pos + sourcelen
-
-		datatype = vsqlexpr.datatype
-		error = vsqlexpr.error
-		if vss_id is None:
-			# Validate target datatype (if the tree is valid so far)
-			if datatype is not None:
-				error = vsql.DataType.compatible_to(datatype, required_datatype)
-				if error is not None:
-					datatype = None
-
-			r = self.proc_vsqlsource_insert(
-				cursor,
-				c_user=self.ide_id,
-				p_vss_source=source,
-			)
-			vss_id = r.p_vss_id
-		r = self.proc_vsql_insert(
-			cursor,
-			c_user=self.ide_id,
-			p_vs_id_super=vs_id_super,
-			p_vs_order=vs_order,
-			p_vs_nodetype=vsqlexpr.nodetype.value,
-			p_vs_value=vsqlexpr.nodevalue,
-			p_vs_datatype=datatype.value if datatype is not None else None,
-			p_vs_erroridentifier=error.value if error is not None else None,
-			p_vss_id=vss_id,
-			p_vs_start=pos,
-			p_vs_stop=finalpos,
-		)
-		vs_id = r.p_vs_id
-		# FieldRefAST has children in the implementation, but in the database it has not
-		if not isinstance(vsqlexpr, vsql.FieldRefAST):
-			order = 10
-			for child in vsqlexpr.content:
-				if isinstance(child, str):
-					pos += len(child)
-				else:
-					(_, pos) = self._save_vsql_ast(child, None, cursor, vs_id, order, vss_id, pos)
-					order += 10
-		return (vs_id, finalpos)
-
-	def save_vsql_ast(self, vsqlexpr, datatype=None, cursor=None):
-		return self._save_vsql_ast(vsqlexpr, datatype, cursor)[0]
-
-	def save_vsql_source(self, cursor, source, function, datatype=None, **queryargs):
-		if not source:
-			return None
-
-		if cursor is None:
-			cursor = self.cursor()
-
-		args = ", ".join(f"{a}=>:{a}" for a in queryargs)
-		query = f"select {function}({args}) from dual"
-		cursor.execute(query, **queryargs)
-		dump = cursor.fetchone()[0]
-		dump = dump.decode("utf-8")
-		vars = ul4on.loads(dump)
-		vsqlexpr = vsql.AST.fromsource(source, **vars)
-		return self.save_vsql_ast(vsqlexpr, datatype, cursor)
+	def save_vsql(self, cursor, source, function, datatype=None, **queryargs):
+		return vsql.compile_and_save(self, cursor, source, datatype, function, **queryargs)
 
 	def save_internaltemplate(self, internaltemplate, recursive=True):
 		template = ul4c.Template(internaltemplate.source, name=internaltemplate.identifier)
-		cursor = self.cursor_pg()
-
-		cursor.execute(
-			"""
-			call internaltemplate.internaltemplate_import(
-				c_user => %s,
-				p_it_id => null,
-				p_app_id => %s,
-				p_it_identifier => %s,
-				p_utv_source => %s,
-				p_utv_signature => %s,
-				p_utv_whitespace => %s,
-				p_utv_doc => %s
-			)
-			""",
-			[
-				self.ide_id,
-				internaltemplate.app.id,
-				template.name,
-				template.source,
-				ul4c._str(template.signature) if template.signature is not None else None,
-				template.whitespace,
-				template.doc,
-			]
+		cursor = self.cursor()
+		self.proc_internaltemplate_import(
+			cursor,
+			c_user=self.ide_id,
+			p_tpl_uuid=internaltemplate.app.id,
+			p_it_identifier=template.name,
+			p_utv_source=template.source,
+			p_utv_signature=ul4c._str(template.signature) if template.signature is not None else None,
+			p_utv_whitespace=template.whitespace,
+			p_utv_doc=template.doc,
 		)
 
 	def save_viewtemplate(self, viewtemplate, recursive=True):
 		template = ul4c.Template(viewtemplate.source, name=viewtemplate.identifier)
 		cursor = self.cursor()
 		r = self.proc_viewtemplate_import(
 			cursor,
@@ -609,68 +348,53 @@
 			p_vt_type=viewtemplate.type.value,
 			p_vt_identifier=template.name,
 			p_vt_mimetype=viewtemplate.mimetype,
 			p_utv_signature=ul4c._str(template.signature) if template.signature is not None else None,
 			p_utv_whitespace=template.whitespace,
 			p_utv_doc=template.doc,
 			p_utv_source=template.source,
+			p_vt_defaultlist=int(viewtemplate.type is la.ViewTemplate.Type.LISTDEFAULT) if viewtemplate.type in {la.ViewTemplate.Type.LIST, la.ViewTemplate.Type.LISTDEFAULT} else None,
+			p_vt_resultpage=int(viewtemplate.type is la.ViewTemplate.Type.DETAILRESULT) if viewtemplate.type is {la.ViewTemplate.Type.DETAIL, la.ViewTemplate.Type.DETAILRESULT} else None,
 			p_vt_permission_level=viewtemplate.permission.value
 		)
 		viewtemplate.id = r.p_vt_id
 		if recursive:
 			for datasource in viewtemplate.datasources.values():
-				self.save_datasourceconfig(datasource, recursive=recursive)
-
-	def delete_viewtemplate(self, viewtemplate):
-		cursor = self.cursor()
-		self.proc_viewtemplate_delete(
-			cursor,
-			c_user=self.ide_id,
-			p_vt_id=viewtemplate.id,
-		)
-		viewtemplate._deleted = True
-
-	def delete_internaltemplate(self, internaltemplate):
-		cursor = self.cursor()
-		self.proc_internaltemplate_delete(
-			cursor,
-			c_user=self.ide_id,
-			p_it_id=internaltemplate.id,
-		)
-		internaltemplate._deleted = True
+				self.save_datasource(datasource, recursive=recursive)
 
-	def save_datasourceconfig(self, datasource, recursive=True):
+	def save_datasource(self, datasource, recursive=True):
 		cursor = self.cursor()
 
 		# Compile and save the app filter
-		vs_id_appfilter = self.save_vsql_source(
+		vs_id_appfilter = self.save_vsql(
 			cursor,
 			datasource.appfilter,
-			la.DataSourceConfig.appfilter.function,
+			la.DataSource.appfilter.function,
 			p_vt_id=datasource.parent.id,
 			p_tpl_uuid_a=None,
 		)
 
 		# Compile and save the record filter
-		vs_id_recordfilter = self.save_vsql_source(
+		vs_id_recordfilter = self.save_vsql(
 			cursor,
 			datasource.recordfilter,
-			la.DataSourceConfig.recordfilter.function,
+			la.DataSource.recordfilter.function,
 			p_vt_id=datasource.parent.id,
 			p_tpl_uuid_r=datasource.app.id if datasource.app is not None else None,
 		)
 
 		# FIXME: Support for system apps?
 		r = self.proc_datasource_import(
 			cursor,
 			c_user=self.ide_id,
 			p_vt_id=datasource.parent.id,
 			p_tpl_uuid=datasource.app.id if datasource.app is not None else None,
 			p_dmv_id=None,
 			p_tpl_uuid_systemplate=None,
+			p_ds_includetemplates=int(datasource.includetemplates),
 			p_ds_includerecords=int(datasource.includerecords),
 			p_ds_includecontrols=int(datasource.includecontrols),
 			p_ds_includecount=int(datasource.includecount),
 			p_ds_includecloned=int(datasource.includecloned),
 			p_ds_identifier=datasource.identifier,
 			p_ds_includepermissions=int(datasource.includepermissions),
 			p_ds_includeattachments=int(datasource.includeattachments),
@@ -713,15 +437,15 @@
 			query,
 			tpl_uuid=datasourcechildren.control.app.id,
 			ctl_identifier=datasourcechildren.control.identifier,
 		)
 		ctl_id = cursor.fetchone()[0]
 
 		# Compile and save the record filter
-		vs_id_filter = self.save_vsql_source(
+		vs_id_filter = self.save_vsql(
 			cursor,
 			datasourcechildren.filter,
 			la.DataSourceChildren.filter.function,
 			p_ds_id=datasourcechildren.datasource.id,
 			p_ctl_id=ctl_id,
 		)
 
@@ -755,15 +479,15 @@
 		for (old_record, dataorder) in itertools.zip_longest(old_records, orders):
 			if old_record is not None:
 				(do_id, do_order) = old_record
 			else:
 				(do_id, do_order) = (None, last_order + 10)
 			if dataorder is not None:
 				# Compile and save the order expression
-				vs_id_expression = self.save_vsql_source(
+				vs_id_expression = self.save_vsql(
 					cursor,
 					dataorder.expression,
 					function,
 					**procargs,
 				)
 
 				# Import the ``dataorder`` record
@@ -777,226 +501,28 @@
 					**procargs,
 				)
 				dataorder.id = r.p_do_id
 				last_order = do_order
 			else:
 				self.proc_dataorder_delete(cursor, c_user=self.ide_id, p_do_id=do_id)
 
-	def _reinitialize_livingapi_db(self, cursor, globals):
-		"""
-		Reinitialize the server side state of the UL4ON codec machinery.
-
-		We do this by calling ``livingapi_pkg.init()`` passing the local
-		information about the current view/email template and detail record.
-
-		We also need to pass the state of the local UL4ON backref registry to
-		the server so that existing object won't have to be loaded again.
-
-		(This is mostly a performance optimization, but for email templates it
-		is essential that the detail record won't be loaded again, as we want
-		to use the state of the record as it was recorded in
-		``emailqueue.eq_data``).
-		"""
-		backrefs = []
-
-		# The backref registry might contain objects for which we can't sync
-		# backreferences to the database. This can happen when the dump hasn't
-		# been created by the database (for example when the template gateway
-		# puts an UL4ON dump into the session). But since the database doesn't
-		# know how to create those backreferences, we can be sure that it doesn't
-		# create then, so we can put any object into that backreference slot
-		# (But we **do** have to put something in that slot, otherwise all
-		# following backreference indexes would be off by one.
-		# For those fake backreferences we use the special type ``ignore``
-		# which is handled specifically by ``livingapi_pkg.init_ul4on()``
-		for obj in self.ul4on_decoder._objects:
-			ul4onname = "ignore"
-			ul4onid = None
-			if isinstance(obj, str):
-				# We tell the database to ignore long string, since it can't
-				# create backreferences to those.
-				if len(obj) < 296:
-					ul4onname = "str"
-					ul4onid = obj
-				# Else:
-			elif hasattr(obj, "ul4onname"):
-				# Ignore backreferences to ``Geo`` objects
-				if not isinstance(obj, la.Geo):
-					if obj.ul4onid is None:
-						raise TypeError(f"Can't sync backreference to non-persistent object of type {type(obj)!r}")
-					else:
-						ul4onname = obj.ul4onname
-						ul4onid = obj.ul4onid
-			# For everthing else we have a back reference that couldn't have been
-			# produced by the database, so we ignore it too.
-			backrefs.append(ul4onname)
-			backrefs.append(ul4onid)
-
-		args = dict(
-			c_user=self.ide_id,
-			p_ul4onbackrefs=self.varchars(backrefs),
-		)
-		if globals.emailtemplate_id is not None:
-			args["p_et_id"] = globals.emailtemplate_id
-		elif globals.viewtemplate_id is not None:
-			args["p_vt_id"] = globals.viewtemplate_id
-		elif globals.view_id is not None:
-			args["p_vw_id"] = globals.view_id
-		elif globals.app is not None:
-			args["p_tpl_uuid"] = globals.app.id
-		if globals.record is not None:
-			args["p_dat_id"] = globals.record.id
-		self.proc_init(cursor, **args)
-
-	def _execute_incremental_ul4on_query(self, cursor, globals, query, **args):
-		"""
-		Returns the deserialized UL4ON data from executing a database function
-		that returns an "incremental" dump. ("incremental" means that it might
-		have backreferences to a previous dump). The data from this dump
-		will be merged into the exiting data.
-
-		When such a database function (e.g. ``livingapi_pkg.app_params_inc_ful4on()``)
-		detects that the UL4ON codec machinery in ``ul4onblobbuffer_pkg`` and
-		``livingapi_pkg`` hasn't been initialized yet, it returns ``null``.
-
-		This can happen in email templates where the UL4ON dump will not be loaded
-		via calls to ``livingapi_pkg.data_ful4on()`` (but from
-		``emailqueue.eq_data``) or when executing a data action results in an
-		email, so that an UL4ON dump for the email queue will be generated, which
-		results in the UL4ON codec machinery being reset.
-
-		In this case we have to reinitialize the UL4ON codec machinery (by calling
-		:meth:`_reinitialize_livingapi_db`) and try calling the database function
-		again.
-		"""
-		cursor.execute(query, **args)
-		dump = cursor.fetchone()[0]
-		if dump is None:
-			self._reinitialize_livingapi_db(cursor, globals)
-			cursor.execute(query, **args)
-			dump = cursor.fetchone()[0]
-		dump = dump.decode("utf-8")
-		dump = self._loaddump(dump)
-		return dump
-
-	def meta_data(self, *appids, records=False):
+	def meta_data(self, *appids):
 		cursor = self.cursor()
+
 		tpl_uuids = self.varchars(appids)
 		cursor.execute(
-			"select livingapi_pkg.metadata_ful4on(c_user=>:ide_id, p_tpl_uuids=>:tpl_uuids, p_records=>:records) from dual",
+			"select livingapi_pkg.metadata_ful4on(:ide_id, :tpl_uuids) from dual",
 			ide_id=self.ide_id,
 			tpl_uuids=tpl_uuids,
-			records=int(bool(records))
 		)
-		dump = cursor.fetchone()[0]
-		dump = dump.decode("utf-8")
-		dump = self._loaddump(dump)
-		return dump
-
-	def record_sync_data(self, dat_id, force=False):
-		if not force:
-			result = self.ul4on_decoder.persistent_object(la.Record.ul4onname, dat_id)
-			if result is not None:
-				return result
-		c = self.cursor()
-		c.execute(
-			"select livingapi_pkg.record_sync_ful4on(p_dat_id=>:dat_id, p_force=>:force) from dual",
-			dat_id=dat_id,
-			force=int(force),
-		)
-		r = c.fetchone()
-		dump = r[0].decode("utf-8")
-		record = self._loaddump(dump)
-		return record
-
-	def records_sync_data(self, dat_ids, force=False):
-		if force:
-			missing = set(dat_ids)
-		else:
-			missing = set()
-			for dat_id in dat_ids:
-				record = self.ul4on_decoder.persistent_object(la.Record.ul4onname, dat_id)
-				if record is None:
-					missing.add(dat_id)
-				else:
-					found[dat_id] = record
-		c = self.cursor()
-		c.execute(
-			"select livingapi_pkg.records_sync_ful4on(p_dat_ids=>:dat_ids, p_force=>:force) from dual",
-			dat_ids=self.varchars(missing),
-			force=int(force),
-		)
-		r = c.fetchone()
-		dump = r[0].decode("utf-8")
-		records = self._loaddump(dump)
-		return records
-
-	def _data(self, vt_id=None, et_id=None, vw_id=None, tpl_uuid=None, dat_id=None, dat_ids=None, ctl_identifier=None, searchtext=None, reqparams=None, mode=None, sync=False, exportmeta=False, funcname="data_ful4on"):
-		paramslist = []
-		if reqparams:
-			for (key, value) in reqparams.items():
-				if value is not None:
-					if isinstance(value, str):
-						paramslist.append(key)
-						paramslist.append(value)
-					elif isinstance(value, list):
-						for subvalue in value:
-							paramslist.append(key)
-							paramslist.append(subvalue)
-		paramslist = self.varchars(paramslist)
-
-		c = self.cursor()
-
-		# Reset the UL4ON decoder before loading
-		# (since the server will reset its UL4ON codec state too)
-		self.reset()
-
-		c.execute(
-			"""
-				select
-					livingapi_pkg.data_ful4on(
-						c_user => :c_user,
-						p_requestid => :p_requestid,
-						p_vt_id => :p_vt_id,
-						p_et_id => :p_et_id,
-						p_vw_id => :p_vw_id,
-						p_tpl_uuid => :p_tpl_uuid,
-						p_dat_id => :p_dat_id,
-						p_dat_ids => :p_dat_ids,
-						p_ctl_identifier => :p_ctl_identifier,
-						p_searchtext => :p_searchtext,
-						p_reqparams => :p_reqparams,
-						p_mode => :p_mode,
-						p_sync => :p_sync,
-						p_exportmeta => :p_exportmeta,
-						p_funcname => :p_funcname
-					)
-				from dual
-			""",
-			c_user=self.ide_id,
-			p_requestid=self.requestid,
-			p_vt_id=vt_id,
-			p_et_id=et_id,
-			p_vw_id=vw_id,
-			p_tpl_uuid=tpl_uuid,
-			p_dat_id=dat_id,
-			p_dat_ids=self.varchars(dat_ids or []),
-			p_ctl_identifier=ctl_identifier,
-			p_searchtext=searchtext,
-			p_reqparams=paramslist,
-			p_mode=mode,
-			p_sync=int(sync),
-			p_exportmeta=int(exportmeta),
-			p_funcname=funcname,
-		)
-
-		r = c.fetchone()
+		r = cursor.fetchone()
 		dump = r[0].decode("utf-8")
+		with open("gurk.ul4on", "w", encoding="utf-8") as f:
+			f.write(dump)
 		dump = self._loaddump(dump)
-		# Since the database didn't reset its backref registry, we don't either
 		return dump
 
 	def viewtemplate_data(self, *path, **params):
 		if not 1 <= len(path) <= 2:
 			raise ValueError(f"need one or two path components, got {len(path)}")
 
 		appid = path[0]
@@ -1008,353 +534,112 @@
 		r = c.fetchone()
 		if r is None:
 			raise ValueError(f"no app {appid!r}")
 		tpl_id = r.tpl_id
 		if "template" in params:
 			template = params.pop("template")
 			c.execute(
-				"select vt_id from viewtemplate where tpl_id = :tpl_id and vt_identifier = :identifier",
+				"select vt_id from viewtemplate where tpl_id = :tpl_id and vt_identifier = : identifier",
 				tpl_id=tpl_id,
 				identifier=template,
 			)
 		else:
 			template = None
 			c.execute(
-				"select vt_id from viewtemplate where tpl_id = :tpl_id and vt_type = 'listdefault'",
+				"select vt_id from viewtemplate where tpl_id = :tpl_id and vt_defaultlist != 0",
 				tpl_id=tpl_id,
 			)
 		r = c.fetchone()
 		if r is None:
 			if template is None:
 				raise ValueError(f"no default template for app {appid!r}")
 			else:
 				raise ValueError(f"no template named {template!r} for app {appid!r}")
 		vt_id = r.vt_id
-
-		return self._data(vt_id=r.vt_id, dat_id=datid, reqparams=params, funcname="viewtemplatedata_ful4on")
-
-	def viewtemplate_params_incremental_data(self, globals, id):
-		return self._execute_incremental_ul4on_query(
-			self.cursor(),
-			globals,
-			"select livingapi_pkg.viewtemplate_params_inc_ful4on(:p_vt_id) from dual",
-			p_vt_id=id,
-		)
-
-	def emailtemplate_params_incremental_data(self, globals, id):
-		return self._execute_incremental_ul4on_query(
-			self.cursor(),
-			globals,
-			"select livingapi_pkg.emailtemplate_params_inc_ful4on(:p_et_id) from dual",
-			p_et_id=id,
-		)
-
-	def app_params_incremental_data(self, app):
-		return self._execute_incremental_ul4on_query(
-			self.cursor(),
-			app.globals,
-			"select livingapi_pkg.app_params_inc_ful4on(:p_tpl_uuid) from dual",
-			p_tpl_uuid=app.id,
-		)
-
-	def app_views_incremental_data(self, app):
-		return self._execute_incremental_ul4on_query(
-			self.cursor(),
-			app.globals,
-			"select livingapi_pkg.app_views_inc_ful4on(:p_tpl_uuid) from dual",
-			p_tpl_uuid=app.id,
-		)
-
-	def record_attachments_incremental_data(self, record):
-		return self._execute_incremental_ul4on_query(
-			self.cursor(),
-			record.app.globals,
-			"select livingapi_pkg.record_attachments_inc_ful4on(:p_dat_id) from dual",
-			p_dat_id=record.id,
-		)
-
-	def view_layout_controls_incremental_data(self, view):
-		return self._execute_incremental_ul4on_query(
-			self.cursor(),
-			view.app.globals,
-			"select livingapi_pkg.view_layoutcontrols_inc_ful4on(:p_vw_id) from dual",
-			p_vw_id=view.id,
-		)
-
-	def app_child_controls_incremental_data(self, app):
-		return self._execute_incremental_ul4on_query(
-			self.cursor(),
-			app.globals,
-			"select livingapi_pkg.app_childcontrols_inc_ful4on(:p_tpl_uuid) from dual",
-			p_tpl_uuid=app.id,
-		)
-
-	def app_menus_incremental_data(self, app):
-		return self._execute_incremental_ul4on_query(
-			self.cursor(),
-			app.globals,
-			"select livingapi_pkg.app_links_inc_ful4on(:c_user, :p_tpl_uuid, 'menuitem') from dual",
-			c_user=self.ide_id,
-			p_tpl_uuid=app.id,
-		)
-
-	def app_panels_incremental_data(self, app):
-		return self._execute_incremental_ul4on_query(
-			self.cursor(),
-			app.globals,
-			"select livingapi_pkg.app_links_inc_ful4on(:c_user, :p_tpl_uuid, 'panel') from dual",
-			c_user=self.ide_id,
-			p_tpl_uuid=app.id,
+		reqparams = []
+		for (key, value) in params.items():
+			if value is not None:
+				if isinstance(value, str):
+					reqparams.append(key)
+					reqparams.append(value)
+				elif isinstance(value, list):
+					for subvalue in value:
+						reqparams.append(key)
+						reqparams.append(subvalue)
+		reqparams = self.varchars(reqparams)
+		c.execute(
+			"select livingapi_pkg.viewtemplatedata_ful4on(:ide_id, :vt_id, :dat_id, :reqparams) from dual",
+			ide_id=self.ide_id,
+			vt_id=vt_id,
+			dat_id=datid,
+			reqparams=reqparams,
 		)
+		r = c.fetchone()
+		dump = r[0].decode("utf-8")
+		dump = self._loaddump(dump)
+		return dump
 
 	def save_record(self, record, recursive=True):
-		record.clear_errors()
 		app = record.app
 		real = app.basetable in {"data_select", "data"}
 		if real:
 			proc = self.proc_data_insert if record.id is None else self.proc_data_update
 			pk = "dat_id"
 		else:
 			proc = self._getproc(app.insertprocedure if record.id is None else app.updateprocedure)
 			pk = app.primarykey
 
 		args = {
 			"c_user": self.ide_id,
 		}
-		if real:
-			if record.id is None:
-				args["p_tpl_uuid"] = app.id
-			mode = record.app.globals.mode
-			args["p_mode"] = mode.value if mode is not None else None
+		if real and record.id is None:
+			args["p_tpl_uuid"] = app.id
 		if record.id is not None:
 			args[f"p_{pk}"] = record.id
 		for field in record.fields.values():
 			if record.id is None or field._dirty:
-				args[f"p_{field.control.fieldname}"] = field._asdbarg(self)
+				args[f"p_{field.control.field}"] = field.control._asdbarg(field.value)
 				if record.id is not None:
-					args[f"p_{field.control.fieldname}_changed"] = 1
+					args[f"p_{field.control.field}_changed"] = 1
 		c = self.cursor()
-		try:
-			result = proc(c, **args)
-		except orasql.DatabaseError as exc:
-			error = exc.args[0]
-			if error.code == 20010:
-				parts = error.message.split("\x01")[1:-1]
-				if parts:
-					# An error message with the usual formatting from ``errmsg_pkg``.
-					controls_by_field = {c.field: c for c in record.app.controls.values()} # Maps the field name to the control
-					field = None
-					for (i, part) in enumerate(parts):
-						if i % 2:
-							if field:
-								if field not in controls_by_field:
-									record.add_error(f"{field}: {part}")
-								else:
-									control = controls_by_field[field]
-									identifier = control.identifier
-									if app.active_view is not None and identifier not in app.active_view.controls:
-										record.add_error(f"{identifier}: {part}")
-									else:
-										record.fields[identifier].add_error(part)
-							else:
-								record.add_error(part)
-						else:
-							field = part
-				else:
-					# An error message with strange formatting, use this as is.
-					record.add_error(error.message)
-				return False
-			else:
-				# Some other database exception
-				raise
+		result = proc(c, **args)
 
 		if result.p_errormessage:
-			record.add_error(result.p_errormessage)
-			saved = False
-		else:
-			saved = True
+			raise ValueError(result.p_errormessage)
 
-			if record.id is None:
-				record.id = result[f"p_{pk}"]
-				record.createdat = datetime.datetime.now()
-				record.createdby = app.globals.user
-				record.updatecount = 0
-			else:
-				record.updatedat = datetime.datetime.now()
-				record.updatedby = app.globals.user
-				record.updatecount += 1
-			for field in record.fields.values():
-				field._dirty = False
-
-		return saved
+		if record.id is None:
+			record.id = result[f"p_{pk}"]
+			record.createdat = datetime.datetime.now()
+			record.createdby = app.globals.user
+			record.updatecount = 0
+		else:
+			record.updatedat = datetime.datetime.now()
+			record.updatedby = app.globals.user
+			record.updatecount += 1
+		for field in record.fields.values():
+			field._dirty = False
+			field.errors = []
+		record.errors = []
 
 	def delete_record(self, record):
 		app = record.app
-		args = {
-			"c_user": self.ide_id,
-			"p_dat_id": record.id,
-		}
 		if app.basetable in {"data_select", "data"}:
 			proc = self.proc_data_delete
-			mode = record.app.globals.mode
-			args["p_mode"] = mode.value if mode is not None else None
 		else:
 			proc = self._getproc(app.deleteprocedure)
 
-			mode = record.app.globals.mode
-
 		c = self.cursor()
-		r = proc(c, **args)
-		record._deleted = True
-
-		if r.p_errormessage:
-			raise ValueError(r.p_errormessage)
-
-	def save_parameter(self, parameter, recursive=True):
-		c = self.cursor()
-		app = parameter.owner
-
-		p_ap_value_bool = None
-		p_ap_value_date = None
-		p_ap_value_datetime = None
-		p_ap_value_str = None
-		p_ap_value_html = None
-		p_ap_value_other = None
-		p_upl_id = None
-		p_tpl_uuid_value = None
-		p_ctl_id = None
-
-		if parameter.value is not None:
-			if parameter.type is parameter.Type.BOOL:
-				p_ap_value_bool = int(parameter.value)
-			elif parameter.type is parameter.Type.INT:
-				p_ap_value_other = str(parameter.value)
-			elif parameter.type is parameter.Type.NUMBER:
-				p_ap_value_other = str(parameter.value)
-			elif parameter.type is parameter.Type.STR:
-				p_ap_value_str = parameter.value
-			elif parameter.type is parameter.Type.HTML:
-				p_ap_value_html = parameter.value
-			elif parameter.type is parameter.Type.COLOR:
-				p_ap_value_other = f"#{parameter.value.r():02x}{parameter.value.g():02x}{parameter.value.b():02x}{parameter.value.a():02x}"
-			elif parameter.type is parameter.Type.DATE:
-				p_ap_value_date = parameter.value
-			elif parameter.type is parameter.Type.DATETIME:
-				p_ap_value_datetime = parameter.value
-			elif parameter.type is parameter.Type.DATEDELTA:
-				p_ap_value_other = str(parameter.value.days)
-			elif parameter.type is parameter.Type.DATETIMEDELTA:
-				seconds = parameter.value.seconds
-				(minutes, seconds) = divmod(seconds, 60)
-				(hours, minutes) = divmod(minutes, 60)
-				p_ap_value_other = f"{parameter.value.days} days, {hours:02}:{minutes:02}:{seconds:02}"
-			elif parameter.type is parameter.Type.MONTHDELTA:
-				p_ap_value_other = str(parameter.value.months())
-			elif parameter.type is parameter.Type.UPLOAD:
-				if parameter.value.internal_id is None:
-					raise la.ValueError(error_object_unsaved(parameter.value))
-				p_upl_id = parameter.value.internal_id
-			elif parameter.type is parameter.Type.APP:
-				p_tpl_uuid_value = parameter.value.id
-			elif parameter.type is parameter.Type.CONTROL:
-				p_ctl_id = parameter.value.id
-
-		try:
-			result = self.proc_appparameter_save(
-				c,
-				c_user=self.ide_id,
-				c_lang="de", # FIXME
-				p_requestid=self.requestid,
-				p_ap_id=parameter.id,
-				p_tpl_uuid=app.id,
-				p_vt_id=None,
-				p_et_id=None,
-				p_ap_id_super=parameter.parent.id if parameter.parent is not None else None,
-				p_ap_order=parameter.order,
-				p_ap_identifier=parameter.identifier,
-				p_ap_type=parameter.type.value,
-				p_ap_description=parameter.description,
-				p_ap_value_bool=p_ap_value_bool,
-				p_ap_value_date=p_ap_value_date,
-				p_ap_value_datetime=p_ap_value_datetime,
-				p_ap_value_str=p_ap_value_str,
-				p_ap_value_html=p_ap_value_html,
-				p_ap_value_other=p_ap_value_other,
-				p_upl_id=p_upl_id,
-				p_tpl_uuid_value=p_tpl_uuid_value,
-				p_ctl_id=p_ctl_id,
-			)
-		except orasql.DatabaseError as exc:
-			error = exc.args[0]
-			if error.code == 20010:
-				parts = error.message.split("\x01")[1:-1]
-				if parts:
-					# An error message with the usual formatting from ``errmsg_pkg``.
-					raise ValueError("\n".join(parts[1::2])) from None
-				else:
-					# An error message with strange formatting, use it as it is.
-					raise ValueError(error.message) from None
-			else:
-				# Some other database exception
-				raise
-
-		if parameter.id is None:
-			parameter.id = result.p_ap_id
-			parameter.createdat = datetime.datetime.now()
-			parameter.createdby = app.globals.user
-		else:
-			parameter.updatedat = datetime.datetime.now()
-			parameter.updatedby = app.globals.user
-		parameter._dirty = False
-		if recursive:
-			if parameter.type is parameter.Type.LIST:
-				for child in parameter.value:
-					self.save_parameter(child, True)
-			elif parameter.type is parameter.Type.DICT:
-				for child in parameter.value.values():
-					self.save_parameter(child, True)
-
-	def delete_parameter(self, parameter):
-		if not parameter._deleted:
-			c = self.cursor()
-			r = self.proc_appparameter_delete(
-				c,
-				c_user=self.ide_id,
-				p_ap_id=parameter.id,
-			)
-			if parameter.parent is not None:
-				if parameter.type is parameter.Type.DICT:
-					parameter.parent.value.pop(parameter.identifier)
-				elif parameter.type is parameter.Type.LIST:
-					parameter.parent.value.remove(parameter)
-			parameter._deleted = True
-
-	def parameter_sync_data(self, ap_id):
-		c = self.cursor()
-		c.execute(
-			"select livingapi_pkg.appparam_sync_ful4on(p_ap_id=>:ap_id) from dual",
-			ap_id=ap_id,
-		)
-		r = c.fetchone()
-		dump = r[0].decode("utf-8")
-		parameter = self._loaddump(dump)
-		return parameter
-	
-	def change_user(self, lang, oldpassword, newpassword, newemail):
-		c = self.cursor()
-		r = self.proc_identity_change(
+		r = proc(
 			c,
 			c_user=self.ide_id,
-			c_lang=lang,
-			p_oldpassword=oldpassword,
-			p_newpassword=newpassword,
-			p_newemail=newemail,
+			p_dat_id=record.id,
 		)
-		return r.p_errormessage
 
+		if r.p_errormessage:
+			raise ValueError(r.p_errormessage)
 
 	def _executeaction(self, record, actionidentifier):
 		c = self.cursor()
 		r = self.proc_dataaction_execute(
 			c,
 			c_user=self.ide_id,
 			p_dat_id=record.id,
@@ -1364,186 +649,66 @@
 		if r.p_errormessage:
 			raise ValueError(r.p_errormessage)
 
 	def _getproc(self, procname):
 		try:
 			return self.custom_procs[procname]
 		except KeyError:
-			proc = self.db.object_named(procname)
+			proc = self.db.getobject(procname)
 			if not isinstance(proc, orasql.Procedure):
 				raise ValueError(f"no procedure {procname}")
 			self.custom_procs[procname] = proc
 			return proc
 
-	def loadinternaltemplates(self, tpl_uuid):
-		if tpl_uuid in self.internaltemplates:
-			return self.internaltemplates[tpl_uuid]
-		c = self.cursor_pg()
-		c.execute("""
-			select
-				it_identifier,
-				tmt_key,
-				utv_source
-			from
-				internaltemplate.internaltemplate_select
-			where
-				app_id=%s
-		""", [tpl_uuid])
-		templates = la.attrdict()
-		for r in c:
-			(identifier, type, source) = r
-			namespace = f"app_{tpl_uuid}.internaltemplates.{type}" if type else f"app_{tpl_uuid}.internaltemplates"
-			template = ul4c.Template(source, name=identifier, namespace=namespace)
-			if type not in templates:
-				templates[type] = la.attrdict()
-			templates[type][template.name] = template
-		self.internaltemplates[tpl_uuid] = templates
-		return templates
-
-	def fetch_templates(self, app):
-		if app.superid is None:
-			return self.loadinternaltemplates(app.id)
-		else:
-			return {
-				**self.loadinternaltemplates(app.superid),
-				**self.loadinternaltemplates(app.id),
-			}
-
-	def fetch_viewtemplate_params(self, globals):
-		id = globals.viewtemplate_id
-		if id not in self.viewtemplate_params:
-			self.viewtemplate_params[id] = self.viewtemplate_params_incremental_data(globals, id)
-		return self.viewtemplate_params[id]
-
-	def fetch_emailtemplate_params(self, globals):
-		id = globals.emailtemplate_id
-		if id not in self.emailtemplate_params:
-			self.emailtemplate_params[id] = self.emailtemplate_params_incremental_data(globals, id)
-		return self.emailtemplate_params[id]
-
-	def fetch_librarytemplates(self):
-		if self.librarytemplates is None:
-			c = self.cursor_pg(row_factory=rows.tuple_row)
-			c.execute("""
-				select
-					lt_identifier,
-					tmt_key,
-					utv_source
-				from
-					templatelibrary.librarytemplate_select
-			""")
-			templates = la.attrdict()
-			for r in c:
-				(identifier, type, source) = r
-				namespace = f"templatelibrary.{type}" if type else f"templatelibrary"
-				template = ul4c.Template(source, name=identifier, namespace=namespace)
-				if type not in templates:
-					templates[type] = la.attrdict()
-				templates[type][template.name] = template
-			self.librarytemplates = templates
-		return self.librarytemplates
-
-	def fetch_libraryparams(self):
-		if self.libraryparams is None:
-			c = self.cursor_pg(row_factory=rows.tuple_row)
-			c.execute("select templatelibrary.libraryparameters_ful4on()")
-			r = c.fetchone()
-			dump = r[0]
-			# Don't reuse the decoder for the dumps from Oracle, this is an independent one
-			# Note that we ignore the problem of persistent objects, since none of the
-			# persistent objects in this dump are in the other dump
-			dump = ul4on.loads(dump)
-			if isinstance(dump, dict):
-				dump = la.attrdict(dump)
-			self.libraryparams = la.attrdict(dump)
-		return self.libraryparams
-
 
 class HTTPHandler(Handler):
-	def __init__(self, url, username=None, password=None, auth_token=None):
+	def __init__(self, url, username=None, password=None):
 		super().__init__()
 		if not url.endswith("/"):
 			url += "/"
-		url += "gateway/"
 		self.url = url
 		self.username = username
-		self.password = password
-		self.session = None
-		self.auth_token = auth_token
+
+		self.session = requests.Session()
+
+		self.auth_token = None
+
+		# If :obj:`username` or :obj:`password` are not given, we don't log in
+		# This means we can only fetch data for public templates, i.e. those that are marked as "for all users"
+		if username is not None and password is not None:
+			# Login to the LivingApps installation and store the auth token we get
+			r = self.session.post(
+				f"{self.url}gateway/login",
+				data=json.dumps({"username": username, "password": password}),
+				headers={"Content-Type": "application/json"},
+			)
+			result = r.json()
+			if result.get("status") == "success":
+				self.auth_token = result["auth_token"]
+			else:
+				raise_403(r)
 
 	def __repr__(self):
 		return f"<{self.__class__.__module__}.{self.__class__.__qualname__} url={self.url!r} username={self.username!r} at {id(self):#x}>"
 
-	def _login(self):
-		if self.session is None:
-			self.session = requests.Session()
-			if self.auth_token is None:
-				# If :obj:`username` or :obj:`password` are not given, we don't log in
-				# This means we can only fetch data for public templates, i.e. those that are marked as "for all users"
-				if self.username is not None and self.password is not None:
-					# Login to the LivingApps installation and store the auth token we get
-					r = self.session.post(
-						f"{self.url}login",
-						data=json.dumps({"username": self.username, "password": self.password}),
-						headers={"Content-Type": "application/json"},
-					)
-					result = r.json()
-					if result.get("status") == "success":
-						self.auth_token = result["auth_token"]
-					else:
-						raise_403(r)
-
 	def _add_auth_token(self, kwargs):
-		self._login()
 		if self.auth_token:
 			if "headers" not in kwargs:
 				kwargs["headers"] = {}
 			kwargs["headers"]["X-La-Auth-Token"] = self.auth_token
 
-	def save_file(self, file):
-		if file.internal_id is None:
-			if file._content is None:
-				raise ValueError(f"Can't save {file!r} without content!")
-			kwargs = {
-				"files": {
-					"files[]": (file.filename, file._content, file.mimetype),
-				},
-			}
-			self._add_auth_token(kwargs)
-			r = self.session.post(
-				f"{self.url}upload/tempfiles",
-				**kwargs,
-			)
-			r.raise_for_status()
-			result = r.json()[0]
-			print(result)
-			file.name = result["orgname"]
-			file.context_id = result["url"].split("/")[2]
-			file.id = result["upr_id"] + "/" + result["upl_id"]
-			file.width = result["width"]
-			file.height = result["height"]
-			file.size = result["size"]
-			file.mimetype = result["mimetype"]
-			file.internal_id = result["upl_id"]
-
 	def file_content(self, file):
 		kwargs = {}
 		self._add_auth_token(kwargs)
 		r = self.session.get(
 			self.url.rstrip("/") + file.url,
 			**kwargs,
 		)
-		r.raise_for_status()
 		return r.content
 
-	def records_sync_data(self, dat_ids, force=False):
-		if not dat_ids:
-			return {}
-		raise NotImplementedError("Can't sync records via {self!r}")
-
 	def viewtemplate_data(self, *path, **params):
 		if not 1 <= len(path) <= 2:
 			raise ValueError(f"need one or two path components, got {len(path)}")
 		kwargs = {
 			"headers": {
 				"Accept": "application/la-ul4on",
 			},
@@ -1551,108 +716,89 @@
 				key + "[]" if isinstance(value, list) else key: value
 				for (key, value) in params.items()
 			},
 		}
 		path = "/".join(path)
 		self._add_auth_token(kwargs)
 		r = self.session.get(
-			f"{self.url}apps/{path}",
+			f"{self.url}gateway/apps/{path}",
 			**kwargs,
 		)
 		r.raise_for_status()
 		# Workaround: If we're not logged in, but request a protected template,
 		# we get redirected to the login page
 		# -> raise a 403 error instead
 		if self.auth_token is None and r.history:
 			raise_403(r)
 		dump = r.content.decode("utf-8")
 		dump = self._loaddump(dump)
 		return dump
 
 	def save_record(self, record, recursive=True):
-		record.clear_errors()
-		fields = {field.control.identifier: field._asjson(self) for field in record.fields.values() if record.id is None or field.is_dirty()}
+		fields = {field.control.identifier: field.control._asjson(field.value) for field in record.fields.values() if record.id is None or field.is_dirty()}
 		app = record.app
 		recorddata = {"fields": fields}
 		if record.id is not None:
 			recorddata["id"] = record.id
 		data = dict(id=app.id, data=[recorddata])
 		kwargs = {
 			"data": json.dumps({"appdd": data}),
 			"headers": {
 				"Content-Type": "application/json",
 			},
 		}
 		self._add_auth_token(kwargs)
 		r = self.session.post(
-			f"{self.url}v1/appdd/{app.id}.json",
+			f"{self.url}gateway/v1/appdd/{app.id}.json",
 			**kwargs,
 		)
-		if r.status_code >= 300 and r.status_code != 422:
-			r.raise_for_status()
+		r.raise_for_status()
 		result = json.loads(r.text)
 		status = result["status"]
 		if status != "ok":
-			errors_added = False
-			if "globalerrors" in result:
-				for error in result["globalerrors"]:
-					record.add_error(error)
-					errors_added = True
-			if "fielderrors" in result:
-				for (identifier, errors) in result["fielderrors"].items():
-					record.fields[identifier].add_error(*errors)
-					errors_added = True
-			if not errors_added:
-				record.add_error(f"Response status {status!r}")
-			return False
-		else:
-			if record.id is None:
-				record.id = result["id"]
-				record.createdat = datetime.datetime.now()
-				record.createdby = app.globals.user
-				record.updatecount = 0
-			else:
-				record.updatedat = datetime.datetime.now()
-				record.updatedby = app.globals.user
-				record.updatecount += 1
-			for field in record.fields.values():
-				field._dirty = False
-			return True
+			raise TypeError(f"Response status {status!r}")
+		if record.id is None:
+			record.id = result["id"]
+			record.createdat = datetime.datetime.now()
+			record.createdby = app.globals.user
+			record.updatecount = 0
+		else:
+			record.updatedat = datetime.datetime.now()
+			record.updatedby = app.globals.user
+			record.updatecount += 1
+		for field in record.fields.values():
+			field._dirty = False
+			field.errors = []
+		record.errors = []
 
 	def delete_record(self, record):
 		kwargs = {}
 		self._add_auth_token(kwargs)
 
 		r = self.session.delete(
-			f"{self.url}v1/appdd/{record.app.id}/{record.id}.json",
+			f"{self.url}gateway/v1/appdd/{record.app.id}/{record.id}.json",
 			**kwargs,
 		)
 		r.raise_for_status()
 		if r.text != '"Successfully deleted dataset"':
 			raise TypeError(f"Unexpected response {r.text!r}")
 		record._deleted = True
 
 	def _executeaction(self, record, actionidentifier):
 		kwargs = {
 			"data": {"recid": record.id},
 		}
 		self._add_auth_token(kwargs)
 
 		r = self.session.post(
-			f"{self.url}api/v1/apps/{record.app.id}/actions/{actionidentifier}",
+			f"{self.url}gateway/api/v1/apps/{record.app.id}/actions/{actionidentifier}",
 			**kwargs,
 		)
 		r.raise_for_status()
 
-	def record_sync_data(self, dat_id, force=False):
-		result = self.ul4on_decoder.persistent_object(la.Record.ul4onname, dat_id)
-		if result is not None and not force:
-			return result
-		raise NotImplementedError
-
 
 class FileHandler(Handler):
 	controltypes = {}
 	for c in la.Control.__subclasses__():
 		if hasattr(c, "fulltype"):
 			controltypes[c.fulltype] = c
 		for c2 in c.__subclasses__():
@@ -1662,35 +808,35 @@
 		del c
 
 	def __init__(self, basepath=None):
 		if basepath is None:
 			basepath = pathlib.Path()
 		self.basepath = pathlib.Path(basepath)
 
-	def meta_data(self, *appids, records=False):
+	def meta_data(self, *appids):
 		apps = {}
 		for childpath in self.basepath.iterdir():
 			if childpath.is_dir() and childpath.name.endswith(")") and " (" in childpath.name:
 				pos = childpath.name.rfind(" (")
 				id = childpath.name[pos+2:-1]
 				name = childpath.name[:pos]
 				app = la.App(name=name)
 				app.id = id
 				self._loadcontrols(app)
-				self.loadinternaltemplates(app)
+				self._loadinternaltemplates(app)
 				apps[app.id] = app
-		return attrdict(apps)
+		return apps
 
 	def _loadcontrols(self, app):
 		path = self.basepath/f"{app.name} ({app.id})/index.json"
 		if path.exists():
 			dump = json.loads(path.read_text(encoding="utf-8"))
 
 
-	def loadinternaltemplates(self, app):
+	def _loadinternaltemplates(self, app):
 		dir = self.basepath/f"{app.name} ({app.id})/internaltemplates"
 		if dir.exists():
 			for filepath in dir.iterdir():
 				identifier = filepath.with_suffix("").name
 				source = filepath.read_text(encoding="utf-8")
 				template = ul4c.Template(source, name=identifier)
 				internaltemplate = la.InternalTemplate(
```

### Comparing `ll-la-0.28.0/src/ll_la.egg-info/PKG-INFO` & `ll-la-0.9/src/ll_la.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,41 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: ll-la
-Version: 0.28.0
+Version: 0.9
 Summary: Python API for LivingApps
 Home-page: http://github.com/LivingLogic/LivingApps.Python.LivingAPI
 Author: Walter Doerwald
 Author-email: walter@livinglogic.de
 License: MIT
+Description: ``ll.la`` provides a Python API for the LivingApps system
+        (see http://www.living-apps.de/ or http://www.living-apps.com/ for more info).
+        
+        ``ll.la`` allows you to fetch the configured data sources from a template,
+        create new records, and update and delete existing records all from your Python
+        prompt (or script).
+        
+        For more info about LivingApps and this Python SDK, see
+        https://my.living-apps.de/docs/PythonSDK.html (in german).
+        
+        
+        0.9 (2019-06-26)
+        ----------------
+        
+        * Fixed shortcut attributes for the ``Globals`` object.
+        
+        * First Cheeseshop release.
+        
+        
+        
 Keywords: LivingApps
-Classifier: Development Status :: 5 - Production/Stable
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
-Provides-Extra: db
-License-File: LICENSE.txt
-
-``ll.la`` provides a Python API for the LivingApps system
-(see http://www.living-apps.de/ or http://www.living-apps.com/ for more info).
-
-``ll.la`` allows you to fetch the configured data sources from a template,
-create new records, and update and delete existing records all from your Python
-prompt (or script).
-
-For more info about LivingApps and this Python SDK, see
-https://my.living-apps.de/docs/PythonSDK.html (in german).
-
-
-0.28.0 (2024-04-16)
--------------------
-
-* Add method ``User.change()``.
-
-
+Requires-Python: >=3.6
```

