# Comparing `tmp/hazwaz-0.0.2.tar.gz` & `tmp/hazwaz-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hazwaz-0.0.2.tar", last modified: Thu Aug  4 06:35:30 2022, max compression
+gzip compressed data, was "hazwaz-0.0.3.tar", last modified: Tue Apr 16 07:36:47 2024, max compression
```

## Comparing `hazwaz-0.0.2.tar` & `hazwaz-0.0.3.tar`

### file list

```diff
@@ -1,39 +1,42 @@
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2022-08-04 06:35:30.045893 hazwaz-0.0.2/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      340 2022-08-04 06:34:14.000000 hazwaz-0.0.2/CHANGELOG.rst
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)       61 2022-08-01 13:06:15.000000 hazwaz-0.0.2/MANIFEST.in
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     2131 2022-08-04 06:35:30.045893 hazwaz-0.0.2/PKG-INFO
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1101 2022-08-01 13:06:15.000000 hazwaz-0.0.2/README.rst
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)    34523 2022-02-22 15:01:29.000000 hazwaz-0.0.2/agpl.txt
--rwxr-xr-x   0 valhalla  (1023) valhalla  (1023)      828 2022-08-01 13:06:15.000000 hazwaz-0.0.2/check
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2022-08-04 06:35:30.033892 hazwaz-0.0.2/docs/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      638 2022-02-22 19:02:16.000000 hazwaz-0.0.2/docs/Makefile
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      804 2022-02-22 19:02:16.000000 hazwaz-0.0.2/docs/make.bat
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2022-08-04 06:35:30.041893 hazwaz-0.0.2/docs/source/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     2004 2022-08-04 06:32:55.000000 hazwaz-0.0.2/docs/source/conf.py
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2022-08-04 06:35:30.041893 hazwaz-0.0.2/docs/source/examples/
--rwxr-xr-x   0 valhalla  (1023) valhalla  (1023)     1266 2022-08-02 07:47:45.000000 hazwaz-0.0.2/docs/source/examples/greeter.py
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1281 2022-08-04 06:27:38.000000 hazwaz-0.0.2/docs/source/index.rst
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2022-08-04 06:35:30.041893 hazwaz-0.0.2/docs/source/reference/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      130 2022-02-22 19:25:00.000000 hazwaz-0.0.2/docs/source/reference/hazwaz.command.rst
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      127 2022-08-01 13:06:15.000000 hazwaz-0.0.2/docs/source/reference/hazwaz.mixins.rst
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      216 2022-08-01 13:06:15.000000 hazwaz-0.0.2/docs/source/reference/hazwaz.rst
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      133 2022-08-01 13:06:15.000000 hazwaz-0.0.2/docs/source/reference/hazwaz.unittest.rst
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)       55 2022-08-01 13:06:15.000000 hazwaz-0.0.2/docs/source/reference/modules.rst
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1874 2022-08-02 07:01:03.000000 hazwaz-0.0.2/docs/source/testing.rst
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     2809 2022-08-01 13:45:40.000000 hazwaz-0.0.2/docs/source/tutorial.rst
--rwxr-xr-x   0 valhalla  (1023) valhalla  (1023)      351 2022-08-01 13:06:15.000000 hazwaz-0.0.2/docs/update_reference.sh
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2022-08-04 06:35:30.041893 hazwaz-0.0.2/hazwaz/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)       91 2022-03-14 18:48:26.000000 hazwaz-0.0.2/hazwaz/__init__.py
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     4741 2022-08-02 07:44:55.000000 hazwaz-0.0.2/hazwaz/command.py
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1527 2022-08-02 07:20:03.000000 hazwaz-0.0.2/hazwaz/mixins.py
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1510 2022-08-01 14:50:38.000000 hazwaz-0.0.2/hazwaz/unittest.py
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2022-08-04 06:35:30.045893 hazwaz-0.0.2/hazwaz.egg-info/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     2131 2022-08-04 06:35:29.000000 hazwaz-0.0.2/hazwaz.egg-info/PKG-INFO
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      662 2022-08-04 06:35:29.000000 hazwaz-0.0.2/hazwaz.egg-info/SOURCES.txt
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)        1 2022-08-04 06:35:29.000000 hazwaz-0.0.2/hazwaz.egg-info/dependency_links.txt
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)        7 2022-08-04 06:35:29.000000 hazwaz-0.0.2/hazwaz.egg-info/top_level.txt
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)       38 2022-08-04 06:35:30.045893 hazwaz-0.0.2/setup.cfg
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1489 2022-08-04 06:33:02.000000 hazwaz-0.0.2/setup.py
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2022-08-04 06:35:30.045893 hazwaz-0.0.2/tests/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     6649 2022-08-02 07:57:28.000000 hazwaz-0.0.2/tests/test_command.py
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     2000 2022-08-02 07:57:44.000000 hazwaz-0.0.2/tests/test_mixins.py
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2024-04-16 07:36:47.407174 hazwaz-0.0.3/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      452 2024-04-16 07:35:52.000000 hazwaz-0.0.3/CHANGELOG.rst
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)       61 2022-07-16 19:03:22.000000 hazwaz-0.0.3/MANIFEST.in
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     2332 2024-04-16 07:36:47.407174 hazwaz-0.0.3/PKG-INFO
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1101 2022-07-16 16:11:31.000000 hazwaz-0.0.3/README.rst
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)    34523 2022-07-16 13:34:41.000000 hazwaz-0.0.3/agpl.txt
+-rwxr-xr-x   0 valhalla  (1023) valhalla  (1023)      785 2024-04-16 07:19:17.000000 hazwaz-0.0.3/check
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2024-04-16 07:36:47.403174 hazwaz-0.0.3/docs/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      638 2022-07-16 13:34:41.000000 hazwaz-0.0.3/docs/Makefile
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      804 2022-07-16 13:34:41.000000 hazwaz-0.0.3/docs/make.bat
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2024-04-16 07:36:47.403174 hazwaz-0.0.3/docs/source/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     2004 2022-08-04 14:20:20.000000 hazwaz-0.0.3/docs/source/conf.py
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2024-04-16 07:36:47.403174 hazwaz-0.0.3/docs/source/examples/
+-rwxr-xr-x   0 valhalla  (1023) valhalla  (1023)     1266 2024-04-03 12:02:21.000000 hazwaz-0.0.3/docs/source/examples/greeter.py
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1281 2022-08-04 14:20:20.000000 hazwaz-0.0.3/docs/source/index.rst
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2024-04-16 07:36:47.403174 hazwaz-0.0.3/docs/source/reference/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      130 2022-07-16 13:34:41.000000 hazwaz-0.0.3/docs/source/reference/hazwaz.command.rst
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      127 2022-07-17 12:03:40.000000 hazwaz-0.0.3/docs/source/reference/hazwaz.mixins.rst
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      216 2022-07-17 12:21:02.000000 hazwaz-0.0.3/docs/source/reference/hazwaz.rst
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      133 2022-07-17 12:03:40.000000 hazwaz-0.0.3/docs/source/reference/hazwaz.unittest.rst
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)       55 2022-07-17 12:03:40.000000 hazwaz-0.0.3/docs/source/reference/modules.rst
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1874 2022-08-04 14:20:20.000000 hazwaz-0.0.3/docs/source/testing.rst
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     2809 2022-07-16 13:34:41.000000 hazwaz-0.0.3/docs/source/tutorial.rst
+-rwxr-xr-x   0 valhalla  (1023) valhalla  (1023)      351 2022-07-17 12:09:45.000000 hazwaz-0.0.3/docs/update_reference.sh
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2024-04-16 07:36:47.407174 hazwaz-0.0.3/hazwaz/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)       91 2022-07-16 13:34:41.000000 hazwaz-0.0.3/hazwaz/__init__.py
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      411 2024-04-16 07:36:47.000000 hazwaz-0.0.3/hazwaz/_version.py
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     4741 2022-08-04 15:33:59.000000 hazwaz-0.0.3/hazwaz/command.py
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1525 2022-08-04 18:49:59.000000 hazwaz-0.0.3/hazwaz/mixins.py
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)        0 2024-02-03 20:38:15.000000 hazwaz-0.0.3/hazwaz/py.typed
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1510 2022-08-04 14:20:20.000000 hazwaz-0.0.3/hazwaz/unittest.py
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2024-04-16 07:36:47.407174 hazwaz-0.0.3/hazwaz.egg-info/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     2332 2024-04-16 07:36:47.000000 hazwaz-0.0.3/hazwaz.egg-info/PKG-INFO
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      712 2024-04-16 07:36:47.000000 hazwaz-0.0.3/hazwaz.egg-info/SOURCES.txt
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)        1 2024-04-16 07:36:47.000000 hazwaz-0.0.3/hazwaz.egg-info/dependency_links.txt
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)        7 2024-04-16 07:36:47.000000 hazwaz-0.0.3/hazwaz.egg-info/top_level.txt
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1390 2024-04-16 07:26:48.000000 hazwaz-0.0.3/pyproject.toml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)       38 2024-04-16 07:36:47.407174 hazwaz-0.0.3/setup.cfg
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)       39 2024-04-16 07:28:50.000000 hazwaz-0.0.3/setup.py
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2024-04-16 07:36:47.407174 hazwaz-0.0.3/tests/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     6649 2022-08-04 14:20:20.000000 hazwaz-0.0.3/tests/test_command.py
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     2000 2022-08-04 14:20:20.000000 hazwaz-0.0.3/tests/test_mixins.py
```

### Comparing `hazwaz-0.0.2/PKG-INFO` & `hazwaz-0.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: hazwaz
-Version: 0.0.2
-Summary: write command line scripts
-Home-page: https://hazwaz.trueelena.org/
-Author: Elena ``of Valhalla'' Grandi
-Author-email: valhalla@trueelena.org
+Version: 0.0.3
+Summary: A command line scripts framework
+Author-email: Elena ``of Valhalla'' Grandi <valhalla@trueelena.org>
 License: AGPLv3+
-Project-URL: Source, https://git.sr.ht/~valhalla/hazwaz
+Project-URL: Homepage, https://hazwaz.trueelena.org/
 Project-URL: Documentation, https://hazwaz.trueelena.org/
+Project-URL: Repository, https://git.sr.ht/~valhalla/hazwaz
+Project-URL: Source, https://git.sr.ht/~valhalla/hazwaz
+Project-URL: Issues, https://todo.sr.ht/~valhalla/hazwaz
 Project-URL: Tracker, https://todo.sr.ht/~valhalla/hazwaz
+Project-URL: Changelog, https://git.sr.ht/~valhalla/hazwaz/tree/master/item/CHANGELOG.rst
 Keywords: cli
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
-Requires-Python: >=3
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 
 ===============================
  hazwaz - command line library
 ===============================
 
 hazwaz is a python3 library to write command line scripts.
@@ -52,9 +53,7 @@
 This program is distributed in the hope that it will be useful, but
 WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU Affero
 General Public License for more details.
 
 You should have received a copy of the GNU Affero General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-
```

### Comparing `hazwaz-0.0.2/README.rst` & `hazwaz-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `hazwaz-0.0.2/agpl.txt` & `hazwaz-0.0.3/agpl.txt`

 * *Files identical despite different names*

### Comparing `hazwaz-0.0.2/check` & `hazwaz-0.0.3/check`

 * *Files 19% similar despite different names*

```diff
@@ -6,33 +6,29 @@
 then
     $0 coverage
     $0 typecheck
     $0 qa
     exit 0
 fi
 
-if which nose2-3 > /dev/null
-then
-    NOSE2=nose2-3
-else
-    NOSE2=nose2
-fi
+PYTHON="${PYTHON:-python3}"
+COVERAGE="${COVERAGE:-python3-coverage}"
 
 export PYTHONDEVMODE=1
 
 SUBCMD=$1
 shift 1
 
 case $SUBCMD in
     "tests")
-        $NOSE2 $COVER_OPT --log-level=ERROR -B --log-capture $*
+        $PYTHON -m unittest discover -s tests
         ;;
     "coverage")
-        $NOSE2 --with-coverage --coverage-report=term-missing \
-            --log-level=ERROR -B --log-capture $*
+        $COVERAGE run --source=hazwaz -m unittest discover -s tests
+        $COVERAGE report -m
         ;;
     "qa")
         flake8 --select=E,F,W,C90,E123 --ignore=W503 .
         isort --check-only --diff .
         if which doc8
         then
             doc8 .
```

### Comparing `hazwaz-0.0.2/docs/Makefile` & `hazwaz-0.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hazwaz-0.0.2/docs/make.bat` & `hazwaz-0.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hazwaz-0.0.2/docs/source/conf.py` & `hazwaz-0.0.3/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'hazwaz'
 copyright = '2022, Elena Grandi'
 author = 'Elena “of Valhalla” Grandi'
 
 # The full version, including alpha/beta/rc tags
-release = '0.0.2'
+release = '0.0.3'
 # The major project version
 version = '0.0'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
```

### Comparing `hazwaz-0.0.2/docs/source/examples/greeter.py` & `hazwaz-0.0.3/docs/source/examples/greeter.py`

 * *Files identical despite different names*

### Comparing `hazwaz-0.0.2/docs/source/index.rst` & `hazwaz-0.0.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `hazwaz-0.0.2/docs/source/testing.rst` & `hazwaz-0.0.3/docs/source/testing.rst`

 * *Files identical despite different names*

### Comparing `hazwaz-0.0.2/docs/source/tutorial.rst` & `hazwaz-0.0.3/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `hazwaz-0.0.2/hazwaz/command.py` & `hazwaz-0.0.3/hazwaz/command.py`

 * *Files identical despite different names*

### Comparing `hazwaz-0.0.2/hazwaz/mixins.py` & `hazwaz-0.0.3/hazwaz/mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     #: Defaults to the value of ``$EDITOR``, followed by
     #: ``sensible-editor``, followed by ``vi`` as a last resort.
     #:
     #: Each editor should be a tuple ``(<executable>, <name>)``, where
     #: ``<name>`` is printed in case of errors.
     #:
     #: To write unittests that use this mixin, you can override this
-    #: attribute with ``[("true"), ("true")]``.
+    #: attribute with ``[("true", "true")]``.
     editors = [
         (os.environ.get("EDITOR"), "$EDITOR (set to {editor})"),
         ("sensible-editor", "sensible-editor"),
         ("vi", "vi"),
     ]
 
     def edit_file_in_external_editor(self, filepath: str) -> bool:
```

### Comparing `hazwaz-0.0.2/hazwaz/unittest.py` & `hazwaz-0.0.3/hazwaz/unittest.py`

 * *Files identical despite different names*

### Comparing `hazwaz-0.0.2/hazwaz.egg-info/PKG-INFO` & `hazwaz-0.0.3/hazwaz.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: hazwaz
-Version: 0.0.2
-Summary: write command line scripts
-Home-page: https://hazwaz.trueelena.org/
-Author: Elena ``of Valhalla'' Grandi
-Author-email: valhalla@trueelena.org
+Version: 0.0.3
+Summary: A command line scripts framework
+Author-email: Elena ``of Valhalla'' Grandi <valhalla@trueelena.org>
 License: AGPLv3+
-Project-URL: Source, https://git.sr.ht/~valhalla/hazwaz
+Project-URL: Homepage, https://hazwaz.trueelena.org/
 Project-URL: Documentation, https://hazwaz.trueelena.org/
+Project-URL: Repository, https://git.sr.ht/~valhalla/hazwaz
+Project-URL: Source, https://git.sr.ht/~valhalla/hazwaz
+Project-URL: Issues, https://todo.sr.ht/~valhalla/hazwaz
 Project-URL: Tracker, https://todo.sr.ht/~valhalla/hazwaz
+Project-URL: Changelog, https://git.sr.ht/~valhalla/hazwaz/tree/master/item/CHANGELOG.rst
 Keywords: cli
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
-Requires-Python: >=3
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 
 ===============================
  hazwaz - command line library
 ===============================
 
 hazwaz is a python3 library to write command line scripts.
@@ -52,9 +53,7 @@
 This program is distributed in the hope that it will be useful, but
 WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU Affero
 General Public License for more details.
 
 You should have received a copy of the GNU Affero General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-
```

### Comparing `hazwaz-0.0.2/hazwaz.egg-info/SOURCES.txt` & `hazwaz-0.0.3/hazwaz.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 CHANGELOG.rst
 MANIFEST.in
 README.rst
 agpl.txt
 check
+pyproject.toml
 setup.py
 docs/Makefile
 docs/make.bat
 docs/update_reference.sh
 docs/source/conf.py
 docs/source/index.rst
 docs/source/testing.rst
@@ -14,16 +15,18 @@
 docs/source/examples/greeter.py
 docs/source/reference/hazwaz.command.rst
 docs/source/reference/hazwaz.mixins.rst
 docs/source/reference/hazwaz.rst
 docs/source/reference/hazwaz.unittest.rst
 docs/source/reference/modules.rst
 hazwaz/__init__.py
+hazwaz/_version.py
 hazwaz/command.py
 hazwaz/mixins.py
+hazwaz/py.typed
 hazwaz/unittest.py
 hazwaz.egg-info/PKG-INFO
 hazwaz.egg-info/SOURCES.txt
 hazwaz.egg-info/dependency_links.txt
 hazwaz.egg-info/top_level.txt
 tests/test_command.py
 tests/test_mixins.py
```

### Comparing `hazwaz-0.0.2/tests/test_command.py` & `hazwaz-0.0.3/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `hazwaz-0.0.2/tests/test_mixins.py` & `hazwaz-0.0.3/tests/test_mixins.py`

 * *Files identical despite different names*

