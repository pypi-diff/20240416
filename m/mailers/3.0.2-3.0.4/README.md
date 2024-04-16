# Comparing `tmp/mailers-3.0.2.tar.gz` & `tmp/mailers-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mailers-3.0.2.tar", max compression
+gzip compressed data, was "mailers-3.0.4.tar", max compression
```

## Comparing `mailers-3.0.2.tar` & `mailers-3.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1073 2024-03-04 19:24:31.142441 mailers-3.0.2/LICENSE
--rw-r--r--   0        0        0     9774 2024-03-04 19:24:31.142441 mailers-3.0.2/README.md
--rw-r--r--   0        0        0      829 2024-03-04 19:24:31.142441 mailers-3.0.2/mailers/__init__.py
--rw-r--r--   0        0        0       53 2024-03-04 19:24:31.142441 mailers-3.0.2/mailers/encrypters/__init__.py
--rw-r--r--   0        0        0      220 2024-03-04 19:24:31.142441 mailers-3.0.2/mailers/encrypters/base.py
--rw-r--r--   0        0        0      454 2024-03-04 19:24:31.142441 mailers-3.0.2/mailers/exceptions.py
--rw-r--r--   0        0        0     1930 2024-03-04 19:24:31.142441 mailers-3.0.2/mailers/factories.py
--rw-r--r--   0        0        0     5475 2024-03-04 19:24:31.142441 mailers-3.0.2/mailers/mailer.py
--rw-r--r--   0        0        0    12388 2024-03-04 19:24:31.142441 mailers-3.0.2/mailers/message.py
--rw-r--r--   0        0        0      167 2024-03-04 19:24:31.142441 mailers-3.0.2/mailers/preprocessors/__init__.py
--rw-r--r--   0        0        0      690 2024-03-04 19:24:31.142441 mailers-3.0.2/mailers/preprocessors/cssliner.py
--rw-r--r--   0        0        0        0 2024-03-04 19:24:31.142441 mailers-3.0.2/mailers/py.typed
--rw-r--r--   0        0        0      236 2024-03-04 19:24:31.142441 mailers-3.0.2/mailers/pytest_plugin.py
--rw-r--r--   0        0        0       47 2024-03-04 19:24:31.142441 mailers-3.0.2/mailers/signers/__init__.py
--rw-r--r--   0        0        0      214 2024-03-04 19:24:31.142441 mailers-3.0.2/mailers/signers/base.py
--rw-r--r--   0        0        0     1870 2024-03-04 19:24:31.142441 mailers-3.0.2/mailers/signers/dkim.py
--rw-r--r--   0        0        0      406 2024-03-04 19:24:31.146441 mailers-3.0.2/mailers/transports/__init__.py
--rw-r--r--   0        0        0      250 2024-03-04 19:24:31.146441 mailers-3.0.2/mailers/transports/base.py
--rw-r--r--   0        0        0      488 2024-03-04 19:24:31.146441 mailers-3.0.2/mailers/transports/console.py
--rw-r--r--   0        0        0      709 2024-03-04 19:24:31.146441 mailers-3.0.2/mailers/transports/file.py
--rw-r--r--   0        0        0      514 2024-03-04 19:24:31.146441 mailers-3.0.2/mailers/transports/memory.py
--rw-r--r--   0        0        0      914 2024-03-04 19:24:31.146441 mailers-3.0.2/mailers/transports/multi.py
--rw-r--r--   0        0        0      216 2024-03-04 19:24:31.146441 mailers-3.0.2/mailers/transports/null.py
--rw-r--r--   0        0        0     1190 2024-03-04 19:24:31.146441 mailers-3.0.2/mailers/transports/smtp.py
--rw-r--r--   0        0        0      304 2024-03-04 19:24:31.146441 mailers-3.0.2/mailers/transports/stream.py
--rw-r--r--   0        0        0     2371 2024-03-04 19:24:31.146441 mailers-3.0.2/pyproject.toml
--rw-r--r--   0        0        0    11150 1970-01-01 00:00:00.000000 mailers-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-16 19:54:26.363280 mailers-3.0.4/LICENSE
+-rw-r--r--   0        0        0     9774 2024-04-16 19:54:26.363280 mailers-3.0.4/README.md
+-rw-r--r--   0        0        0      829 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/__init__.py
+-rw-r--r--   0        0        0       53 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/encrypters/__init__.py
+-rw-r--r--   0        0        0      220 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/encrypters/base.py
+-rw-r--r--   0        0        0      454 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/exceptions.py
+-rw-r--r--   0        0        0     1930 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/factories.py
+-rw-r--r--   0        0        0     5475 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/mailer.py
+-rw-r--r--   0        0        0    12388 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/message.py
+-rw-r--r--   0        0        0      159 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/preprocessors/__init__.py
+-rw-r--r--   0        0        0      690 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/preprocessors/cssliner.py
+-rw-r--r--   0        0        0        0 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/py.typed
+-rw-r--r--   0        0        0      236 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/pytest_plugin.py
+-rw-r--r--   0        0        0       47 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/signers/__init__.py
+-rw-r--r--   0        0        0      214 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/signers/base.py
+-rw-r--r--   0        0        0     1870 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/signers/dkim.py
+-rw-r--r--   0        0        0      406 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/transports/__init__.py
+-rw-r--r--   0        0        0      250 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/transports/base.py
+-rw-r--r--   0        0        0      488 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/transports/console.py
+-rw-r--r--   0        0        0      709 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/transports/file.py
+-rw-r--r--   0        0        0      514 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/transports/memory.py
+-rw-r--r--   0        0        0      914 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/transports/multi.py
+-rw-r--r--   0        0        0      216 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/transports/null.py
+-rw-r--r--   0        0        0     1190 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/transports/smtp.py
+-rw-r--r--   0        0        0      304 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/transports/stream.py
+-rw-r--r--   0        0        0     2379 2024-04-16 19:54:26.363280 mailers-3.0.4/pyproject.toml
+-rw-r--r--   0        0        0    11154 1970-01-01 00:00:00.000000 mailers-3.0.4/PKG-INFO
```

### Comparing `mailers-3.0.2/LICENSE` & `mailers-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mailers-3.0.2/README.md` & `mailers-3.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mailers-3.0.2/mailers/__init__.py` & `mailers-3.0.4/mailers/__init__.py`

 * *Files identical despite different names*

### Comparing `mailers-3.0.2/mailers/factories.py` & `mailers-3.0.4/mailers/factories.py`

 * *Files identical despite different names*

### Comparing `mailers-3.0.2/mailers/mailer.py` & `mailers-3.0.4/mailers/mailer.py`

 * *Files identical despite different names*

### Comparing `mailers-3.0.2/mailers/message.py` & `mailers-3.0.4/mailers/message.py`

 * *Files identical despite different names*

### Comparing `mailers-3.0.2/mailers/preprocessors/cssliner.py` & `mailers-3.0.4/mailers/preprocessors/cssliner.py`

 * *Files identical despite different names*

### Comparing `mailers-3.0.2/mailers/signers/dkim.py` & `mailers-3.0.4/mailers/signers/dkim.py`

 * *Files identical despite different names*

### Comparing `mailers-3.0.2/mailers/transports/file.py` & `mailers-3.0.4/mailers/transports/file.py`

 * *Files identical despite different names*

### Comparing `mailers-3.0.2/mailers/transports/memory.py` & `mailers-3.0.4/mailers/transports/memory.py`

 * *Files identical despite different names*

### Comparing `mailers-3.0.2/mailers/transports/multi.py` & `mailers-3.0.4/mailers/transports/multi.py`

 * *Files identical despite different names*

### Comparing `mailers-3.0.2/mailers/transports/smtp.py` & `mailers-3.0.4/mailers/transports/smtp.py`

 * *Files identical despite different names*

### Comparing `mailers-3.0.2/pyproject.toml` & `mailers-3.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mailers"
-version = "3.0.2"
+version = "3.0.4"
 description = "Email delivery for asyncio."
 authors = ["alex.oleshkevich <alex.oleshkevich@gmail.com>"]
 license = "MIT"
 readme = 'README.md'
 homepage = 'https://github.com/alex-oleshkevich/mailers'
 repository = 'https://github.com/alex-oleshkevich/mailers.git'
 documentation = "https://github.com/alex-oleshkevich/mailers"
@@ -25,15 +25,15 @@
     "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 aiosmtplib = { version = "^3.0", optional = true }
 dkimpy = { version = "^1.0", optional = true }
-anyio = "^4"
+anyio = ">=3.7.1,<5"
 jinja2 = { version = "^3.0", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 pytest-asyncio = "*"
 aiosmtpd = "^1.4"
 pytest-sugar = "*"
 pytest-cov = "*"
```

### Comparing `mailers-3.0.2/PKG-INFO` & `mailers-3.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailers
-Version: 3.0.2
+Version: 3.0.4
 Summary: Email delivery for asyncio.
 Home-page: https://github.com/alex-oleshkevich/mailers
 License: MIT
 Keywords: asyncio,email,mailer,mail
 Author: alex.oleshkevich
 Author-email: alex.oleshkevich@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Provides-Extra: dkim
 Provides-Extra: jinja2
 Provides-Extra: smtp
 Requires-Dist: aiosmtplib (>=3.0,<4.0) ; extra == "smtp"
-Requires-Dist: anyio (>=4,<5)
+Requires-Dist: anyio (>=3.7.1,<5)
 Requires-Dist: dkimpy (>=1.0,<2.0) ; extra == "dkim"
 Requires-Dist: jinja2 (>=3.0,<4.0) ; extra == "jinja2"
 Project-URL: Documentation, https://github.com/alex-oleshkevich/mailers
 Project-URL: Repository, https://github.com/alex-oleshkevich/mailers.git
 Description-Content-Type: text/markdown
 
 # Mailers for asyncio
```

