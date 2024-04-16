# Comparing `tmp/PALs-0.3.5.tar.gz` & `tmp/PALs-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PALs-0.3.5.tar", last modified: Thu Jun 29 12:20:46 2023, max compression
+gzip compressed data, was "PALs-0.4.0.tar", last modified: Tue Apr 16 13:05:33 2024, max compression
```

## Comparing `PALs-0.3.5.tar` & `PALs-0.4.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-06-29 12:20:46.583046 PALs-0.3.5/
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-06-29 12:20:46.575046 PALs-0.3.5/.ci/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      104 2021-02-01 16:04:04.000000 PALs-0.3.5/.ci/pytest.ini
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-06-29 12:20:46.575046 PALs-0.3.5/.circleci/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1094 2023-01-06 19:39:01.000000 PALs-0.3.5/.circleci/config.yml
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      313 2021-02-01 16:04:04.000000 PALs-0.3.5/.coveragerc
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      204 2023-01-06 19:39:01.000000 PALs-0.3.5/MANIFEST.in
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-06-29 12:20:46.575046 PALs-0.3.5/PALs.egg-info/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     9839 2023-06-29 12:20:45.000000 PALs-0.3.5/PALs.egg-info/PKG-INFO
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      449 2023-06-29 12:20:46.000000 PALs-0.3.5/PALs.egg-info/SOURCES.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2023-06-29 12:20:45.000000 PALs-0.3.5/PALs.egg-info/dependency_links.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2021-02-01 16:06:26.000000 PALs-0.3.5/PALs.egg-info/not-zip-safe
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       54 2023-06-29 12:20:46.000000 PALs-0.3.5/PALs.egg-info/requires.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        5 2023-06-29 12:20:46.000000 PALs-0.3.5/PALs.egg-info/top_level.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     9839 2023-06-29 12:20:46.583046 PALs-0.3.5/PKG-INFO
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4201 2023-06-29 12:20:25.000000 PALs-0.3.5/changelog.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      256 2023-01-06 19:39:01.000000 PALs-0.3.5/docker-compose.yaml
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1549 2021-02-01 16:04:04.000000 PALs-0.3.5/license.txt
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-06-29 12:20:46.575046 PALs-0.3.5/pals/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       32 2021-02-01 16:04:04.000000 PALs-0.3.5/pals/__init__.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     6459 2023-06-29 12:18:47.000000 PALs-0.3.5/pals/core.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-06-29 12:20:46.575046 PALs-0.3.5/pals/tests/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     7437 2023-06-29 12:18:47.000000 PALs-0.3.5/pals/tests/test_core.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       18 2023-06-29 12:19:04.000000 PALs-0.3.5/pals/version.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       24 2021-02-01 16:04:04.000000 PALs-0.3.5/pyp.ini
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4883 2023-01-06 19:39:01.000000 PALs-0.3.5/readme.rst
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-06-29 12:20:46.575046 PALs-0.3.5/scripts/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      941 2021-02-01 16:04:04.000000 PALs-0.3.5/scripts/hang.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      410 2023-01-06 19:39:01.000000 PALs-0.3.5/scripts/setup-codecov
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      172 2023-06-29 12:20:46.583046 PALs-0.3.5/setup.cfg
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1469 2023-01-06 19:39:01.000000 PALs-0.3.5/setup.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      219 2023-01-06 19:39:01.000000 PALs-0.3.5/stable-requirements.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1151 2023-03-06 17:23:08.000000 PALs-0.3.5/tox.ini
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2024-04-16 13:05:33.634095 PALs-0.4.0/
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2024-04-16 13:05:33.634095 PALs-0.4.0/.ci/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      104 2021-02-01 16:04:04.000000 PALs-0.4.0/.ci/pytest.ini
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2024-04-16 13:05:33.634095 PALs-0.4.0/.circleci/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1024 2023-06-29 12:35:31.000000 PALs-0.4.0/.circleci/config.yml
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      313 2021-02-01 16:04:04.000000 PALs-0.4.0/.coveragerc
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      204 2023-01-06 19:39:01.000000 PALs-0.4.0/MANIFEST.in
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2024-04-16 13:05:33.634095 PALs-0.4.0/PALs.egg-info/
+-rw-r--r--   0 mlewellyn  (1000) mlewellyn  (1000)    10176 2024-04-16 13:05:32.000000 PALs-0.4.0/PALs.egg-info/PKG-INFO
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      449 2024-04-16 13:05:33.000000 PALs-0.4.0/PALs.egg-info/SOURCES.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2024-04-16 13:05:32.000000 PALs-0.4.0/PALs.egg-info/dependency_links.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2021-02-01 16:06:26.000000 PALs-0.4.0/PALs.egg-info/not-zip-safe
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       54 2024-04-16 13:05:33.000000 PALs-0.4.0/PALs.egg-info/requires.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        5 2024-04-16 13:05:33.000000 PALs-0.4.0/PALs.egg-info/top_level.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    10176 2024-04-16 13:05:33.634095 PALs-0.4.0/PKG-INFO
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4538 2024-04-16 13:05:17.000000 PALs-0.4.0/changelog.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      256 2024-04-16 12:49:13.000000 PALs-0.4.0/docker-compose.yaml
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1549 2021-02-01 16:04:04.000000 PALs-0.4.0/license.txt
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2024-04-16 13:05:33.634095 PALs-0.4.0/pals/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       32 2021-02-01 16:04:04.000000 PALs-0.4.0/pals/__init__.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     6490 2024-04-16 13:03:53.000000 PALs-0.4.0/pals/core.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2024-04-16 13:05:33.634095 PALs-0.4.0/pals/tests/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     7575 2024-04-16 13:03:53.000000 PALs-0.4.0/pals/tests/test_core.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       18 2024-04-16 13:04:07.000000 PALs-0.4.0/pals/version.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       24 2021-02-01 16:04:04.000000 PALs-0.4.0/pyp.ini
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4883 2023-01-06 19:39:01.000000 PALs-0.4.0/readme.rst
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2024-04-16 13:05:33.634095 PALs-0.4.0/scripts/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      941 2021-02-01 16:04:04.000000 PALs-0.4.0/scripts/hang.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      410 2023-01-06 19:39:01.000000 PALs-0.4.0/scripts/setup-codecov
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      172 2024-04-16 13:05:33.634095 PALs-0.4.0/setup.cfg
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1469 2024-04-16 13:03:53.000000 PALs-0.4.0/setup.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      219 2023-01-06 19:39:01.000000 PALs-0.4.0/stable-requirements.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1257 2024-04-16 13:03:53.000000 PALs-0.4.0/tox.ini
```

### Comparing `PALs-0.3.5/PALs.egg-info/PKG-INFO` & `PALs-0.4.0/PALs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PALs
-Version: 0.3.5
+Version: 0.4.0
 Summary: Easy distributed locking using PostgreSQL Advisory Locks.
 Home-page: https://github.com/level12/pals
 Author: Randy Syring
 Author-email: randy.syring@level12.io
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -176,14 +176,24 @@
 * https://github.com/Xof/django-pglocks
 
 
 
 Changelog
 =========
 
+0.4.0 released 2024-04-16
+-------------------------
+
+- support psycopg3, backwards compatible with psycopg2 (thanks to @petr.prikryl) (0139bea_)
+- remove python 3.7 and 3.8 from CI, resolve flake8 issue (24bff1f_)
+
+.. _0139bea: https://github.com/level12/pals/commit/0139bea
+.. _24bff1f: https://github.com/level12/pals/commit/24bff1f
+
+
 0.3.5 released 2023-06-29
 -------------------------
 
 - fix cursor usage after connection close (thanks to @moser) (ded88e7_)
 
 .. _ded88e7: https://github.com/level12/pals/commit/ded88e7
```

### Comparing `PALs-0.3.5/PKG-INFO` & `PALs-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PALs
-Version: 0.3.5
+Version: 0.4.0
 Summary: Easy distributed locking using PostgreSQL Advisory Locks.
 Home-page: https://github.com/level12/pals
 Author: Randy Syring
 Author-email: randy.syring@level12.io
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -176,14 +176,24 @@
 * https://github.com/Xof/django-pglocks
 
 
 
 Changelog
 =========
 
+0.4.0 released 2024-04-16
+-------------------------
+
+- support psycopg3, backwards compatible with psycopg2 (thanks to @petr.prikryl) (0139bea_)
+- remove python 3.7 and 3.8 from CI, resolve flake8 issue (24bff1f_)
+
+.. _0139bea: https://github.com/level12/pals/commit/0139bea
+.. _24bff1f: https://github.com/level12/pals/commit/24bff1f
+
+
 0.3.5 released 2023-06-29
 -------------------------
 
 - fix cursor usage after connection close (thanks to @moser) (ded88e7_)
 
 .. _ded88e7: https://github.com/level12/pals/commit/ded88e7
```

### Comparing `PALs-0.3.5/changelog.rst` & `PALs-0.4.0/changelog.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Changelog
 =========
 
+0.4.0 released 2024-04-16
+-------------------------
+
+- support psycopg3, backwards compatible with psycopg2 (thanks to @petr.prikryl) (0139bea_)
+- remove python 3.7 and 3.8 from CI, resolve flake8 issue (24bff1f_)
+
+.. _0139bea: https://github.com/level12/pals/commit/0139bea
+.. _24bff1f: https://github.com/level12/pals/commit/24bff1f
+
+
 0.3.5 released 2023-06-29
 -------------------------
 
 - fix cursor usage after connection close (thanks to @moser) (ded88e7_)
 
 .. _ded88e7: https://github.com/level12/pals/commit/ded88e7
```

### Comparing `PALs-0.3.5/license.txt` & `PALs-0.4.0/license.txt`

 * *Files identical despite different names*

### Comparing `PALs-0.3.5/pals/core.py` & `PALs-0.4.0/pals/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         blocking = blocking if blocking is not None else self.blocking
         acquire_timeout = acquire_timeout or self.acquire_timeout
 
         if self.conn is None:
             self.conn = self.engine.connect()
 
         if blocking:
-            timeout_sql = sa.text('set lock_timeout = :timeout')
+            timeout_sql = sa.text("select set_config('lock_timeout', :timeout :: text, false)")
             with self.conn.begin():
                 self.conn.execute(timeout_sql, {'timeout': acquire_timeout})
 
             lock_sql = sa.text(f'select pg_advisory_lock{self.shared_suffix}(:lock_num)')
         else:
             lock_sql = sa.text(f'select pg_try_advisory_lock{self.shared_suffix}(:lock_num)')
```

### Comparing `PALs-0.3.5/pals/tests/test_core.py` & `PALs-0.4.0/pals/tests/test_core.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,27 @@
 import threading
 import time
 
 import pytest
 
 import pals
 
+try:
+    import psycopg  # noqa: F401
+
+    db_driver = 'postgresql+psycopg'
+except ImportError:
+    db_driver = 'postgresql'
+
+
 # Default URL will work for CI tests
-db_url = os.environ.get('PALS_DB_URL', 'postgresql://postgres:password@localhost/postgres')
+db_url = os.environ.get(
+    'PALS_DB_URL',
+    f'{db_driver}://postgres:password@localhost/postgres'
+)
 
 
 def random_str(length):
     return ''.join(random.choice(string.printable) for _ in range(25))
 
 
 class TestLocker:
@@ -218,8 +229,7 @@
 
         for thread in threads:
             thread.start()
         for thread in threads:
             thread.join()
 
         assert [r for r in results if isinstance(r, Exception)] == []
-
```

### Comparing `PALs-0.3.5/readme.rst` & `PALs-0.4.0/readme.rst`

 * *Files identical despite different names*

### Comparing `PALs-0.3.5/scripts/hang.py` & `PALs-0.4.0/scripts/hang.py`

 * *Files identical despite different names*

### Comparing `PALs-0.3.5/setup.py` & `PALs-0.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,11 +37,11 @@
     install_requires=[
         'sqlalchemy',
     ],
     extras_require={
         'tests': [
             'pytest',
             'pytest-cov',
-            'psycopg2-binary',
+            'psycopg[binary]',
         ],
     }
 )
```

### Comparing `PALs-0.3.5/tox.ini` & `PALs-0.4.0/tox.ini`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [tox]
 envlist =
-    py37
-    py{38,39,310}-{base,stable}
-    py37-{lowest}
-    py310-{lowest}
+    py{39,310,311}-{base,stable}
+    py311-{lowest}
     project
 
 [testenv]
 # Ignore all "not installed in testenv" warnings.
 whitelist_externals = *
 passenv = PALS_DB_URL
 
 skip_install = true
 
 recreate = true
 deps =
     -e .[tests]
     stable: -r stable-requirements.txt
     lowest: sqlalchemy<2
+    lowest: psycopg2-binary
 commands =
+    lowest: pip uninstall -y psycopg psycopg-binary
+    stable: pip uninstall -y psycopg psycopg-binary
     pip --version
     # Output installed versions to compare with previous test runs in case a dependency's change
     # breaks things for our build.
     pip freeze
     py.test \
         # feed a blank file so that a user's default pytest.ini doesn't get used
         -c .ci/pytest.ini \
@@ -34,15 +35,15 @@
         --cov-report xml \
         --no-cov-on-fail \
         --junit-xml={toxinidir}/.ci/test-reports/{envname}.pytests.xml \
     pals/tests
 
 
 [testenv:project]
-basepython = python3.10
+basepython = python3.11
 skip_install = true
 usedevelop = false
 deps =
     check-manifest
     flake8
     twine
 commands =
```

