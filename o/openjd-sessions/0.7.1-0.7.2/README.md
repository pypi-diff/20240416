# Comparing `tmp/openjd_sessions-0.7.1.tar.gz` & `tmp/openjd_sessions-0.7.2.tar.gz`

## Comparing `openjd_sessions-0.7.1.tar` & `openjd_sessions-0.7.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 openjd_sessions-0.7.1/openjd/sessions/__init__.py
--rw-r--r--   0        0        0    12908 2020-02-02 00:00:00.000000 openjd_sessions-0.7.1/openjd/sessions/_action_filter.py
--rw-r--r--   0        0        0     9183 2020-02-02 00:00:00.000000 openjd_sessions-0.7.1/openjd/sessions/_embedded_files.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 openjd_sessions-0.7.1/openjd/sessions/_logging.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 openjd_sessions-0.7.1/openjd/sessions/_os_checker.py
--rw-r--r--   0        0        0     4311 2020-02-02 00:00:00.000000 openjd_sessions-0.7.1/openjd/sessions/_path_mapping.py
--rw-r--r--   0        0        0    23365 2020-02-02 00:00:00.000000 openjd_sessions-0.7.1/openjd/sessions/_runner_base.py
--rw-r--r--   0        0        0     8518 2020-02-02 00:00:00.000000 openjd_sessions-0.7.1/openjd/sessions/_runner_env_script.py
--rw-r--r--   0        0        0     6298 2020-02-02 00:00:00.000000 openjd_sessions-0.7.1/openjd/sessions/_runner_step_script.py
--rw-r--r--   0        0        0    46897 2020-02-02 00:00:00.000000 openjd_sessions-0.7.1/openjd/sessions/_session.py
--rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 openjd_sessions-0.7.1/openjd/sessions/_session_user.py
--rw-r--r--   0        0        0    15807 2020-02-02 00:00:00.000000 openjd_sessions-0.7.1/openjd/sessions/_subprocess.py
--rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 openjd_sessions-0.7.1/openjd/sessions/_tempdir.py
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 openjd_sessions-0.7.1/openjd/sessions/_types.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 openjd_sessions-0.7.1/openjd/sessions/_version.py
--rw-r--r--   0        0        0     4199 2020-02-02 00:00:00.000000 openjd_sessions-0.7.1/openjd/sessions/_windows_permission_helper.py
--rw-r--r--   0        0        0     4255 2020-02-02 00:00:00.000000 openjd_sessions-0.7.1/openjd/sessions/_windows_process_killer.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 openjd_sessions-0.7.1/openjd/sessions/py.typed
--rwxr-xr-x   0        0        0     2195 2020-02-02 00:00:00.000000 openjd_sessions-0.7.1/openjd/sessions/_scripts/_posix/_signal_subprocess.sh
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 openjd_sessions-0.7.1/openjd/sessions/_scripts/_windows/_signal_win_subprocess.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 openjd_sessions-0.7.1/openjd/sessions/_win32/__init__.py
--rw-r--r--   0        0        0    17836 2020-02-02 00:00:00.000000 openjd_sessions-0.7.1/openjd/sessions/_win32/_api.py
--rw-r--r--   0        0        0     5612 2020-02-02 00:00:00.000000 openjd_sessions-0.7.1/openjd/sessions/_win32/_helpers.py
--rw-r--r--   0        0        0     5623 2020-02-02 00:00:00.000000 openjd_sessions-0.7.1/openjd/sessions/_win32/_locate_executable.py
--rw-r--r--   0        0        0     9904 2020-02-02 00:00:00.000000 openjd_sessions-0.7.1/openjd/sessions/_win32/_popen_as_user.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 openjd_sessions-0.7.1/.gitignore
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 openjd_sessions-0.7.1/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 openjd_sessions-0.7.1/NOTICE
--rw-r--r--   0        0        0    15168 2020-02-02 00:00:00.000000 openjd_sessions-0.7.1/README.md
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 openjd_sessions-0.7.1/hatch.toml
--rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 openjd_sessions-0.7.1/pyproject.toml
--rw-r--r--   0        0        0    16487 2020-02-02 00:00:00.000000 openjd_sessions-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 openjd_sessions-0.7.2/openjd/sessions/__init__.py
+-rw-r--r--   0        0        0    12908 2020-02-02 00:00:00.000000 openjd_sessions-0.7.2/openjd/sessions/_action_filter.py
+-rw-r--r--   0        0        0     9183 2020-02-02 00:00:00.000000 openjd_sessions-0.7.2/openjd/sessions/_embedded_files.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 openjd_sessions-0.7.2/openjd/sessions/_logging.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 openjd_sessions-0.7.2/openjd/sessions/_os_checker.py
+-rw-r--r--   0        0        0     4311 2020-02-02 00:00:00.000000 openjd_sessions-0.7.2/openjd/sessions/_path_mapping.py
+-rw-r--r--   0        0        0    23365 2020-02-02 00:00:00.000000 openjd_sessions-0.7.2/openjd/sessions/_runner_base.py
+-rw-r--r--   0        0        0     8518 2020-02-02 00:00:00.000000 openjd_sessions-0.7.2/openjd/sessions/_runner_env_script.py
+-rw-r--r--   0        0        0     6298 2020-02-02 00:00:00.000000 openjd_sessions-0.7.2/openjd/sessions/_runner_step_script.py
+-rw-r--r--   0        0        0    46897 2020-02-02 00:00:00.000000 openjd_sessions-0.7.2/openjd/sessions/_session.py
+-rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 openjd_sessions-0.7.2/openjd/sessions/_session_user.py
+-rw-r--r--   0        0        0    15807 2020-02-02 00:00:00.000000 openjd_sessions-0.7.2/openjd/sessions/_subprocess.py
+-rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 openjd_sessions-0.7.2/openjd/sessions/_tempdir.py
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 openjd_sessions-0.7.2/openjd/sessions/_types.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 openjd_sessions-0.7.2/openjd/sessions/_version.py
+-rw-r--r--   0        0        0     4199 2020-02-02 00:00:00.000000 openjd_sessions-0.7.2/openjd/sessions/_windows_permission_helper.py
+-rw-r--r--   0        0        0     4255 2020-02-02 00:00:00.000000 openjd_sessions-0.7.2/openjd/sessions/_windows_process_killer.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 openjd_sessions-0.7.2/openjd/sessions/py.typed
+-rwxr-xr-x   0        0        0     2195 2020-02-02 00:00:00.000000 openjd_sessions-0.7.2/openjd/sessions/_scripts/_posix/_signal_subprocess.sh
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 openjd_sessions-0.7.2/openjd/sessions/_scripts/_windows/_signal_win_subprocess.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 openjd_sessions-0.7.2/openjd/sessions/_win32/__init__.py
+-rw-r--r--   0        0        0    17836 2020-02-02 00:00:00.000000 openjd_sessions-0.7.2/openjd/sessions/_win32/_api.py
+-rw-r--r--   0        0        0     5612 2020-02-02 00:00:00.000000 openjd_sessions-0.7.2/openjd/sessions/_win32/_helpers.py
+-rw-r--r--   0        0        0     5623 2020-02-02 00:00:00.000000 openjd_sessions-0.7.2/openjd/sessions/_win32/_locate_executable.py
+-rw-r--r--   0        0        0     9904 2020-02-02 00:00:00.000000 openjd_sessions-0.7.2/openjd/sessions/_win32/_popen_as_user.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 openjd_sessions-0.7.2/.gitignore
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 openjd_sessions-0.7.2/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 openjd_sessions-0.7.2/NOTICE
+-rw-r--r--   0        0        0    15025 2020-02-02 00:00:00.000000 openjd_sessions-0.7.2/README.md
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 openjd_sessions-0.7.2/hatch.toml
+-rw-r--r--   0        0        0     5213 2020-02-02 00:00:00.000000 openjd_sessions-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0    16372 2020-02-02 00:00:00.000000 openjd_sessions-0.7.2/PKG-INFO
```

### Comparing `openjd_sessions-0.7.1/openjd/sessions/__init__.py` & `openjd_sessions-0.7.2/openjd/sessions/__init__.py`

 * *Files identical despite different names*

### Comparing `openjd_sessions-0.7.1/openjd/sessions/_action_filter.py` & `openjd_sessions-0.7.2/openjd/sessions/_action_filter.py`

 * *Files identical despite different names*

### Comparing `openjd_sessions-0.7.1/openjd/sessions/_embedded_files.py` & `openjd_sessions-0.7.2/openjd/sessions/_embedded_files.py`

 * *Files identical despite different names*

### Comparing `openjd_sessions-0.7.1/openjd/sessions/_logging.py` & `openjd_sessions-0.7.2/openjd/sessions/_logging.py`

 * *Files identical despite different names*

### Comparing `openjd_sessions-0.7.1/openjd/sessions/_path_mapping.py` & `openjd_sessions-0.7.2/openjd/sessions/_path_mapping.py`

 * *Files identical despite different names*

### Comparing `openjd_sessions-0.7.1/openjd/sessions/_runner_base.py` & `openjd_sessions-0.7.2/openjd/sessions/_runner_base.py`

 * *Files identical despite different names*

### Comparing `openjd_sessions-0.7.1/openjd/sessions/_runner_env_script.py` & `openjd_sessions-0.7.2/openjd/sessions/_runner_env_script.py`

 * *Files identical despite different names*

### Comparing `openjd_sessions-0.7.1/openjd/sessions/_runner_step_script.py` & `openjd_sessions-0.7.2/openjd/sessions/_runner_step_script.py`

 * *Files identical despite different names*

### Comparing `openjd_sessions-0.7.1/openjd/sessions/_session.py` & `openjd_sessions-0.7.2/openjd/sessions/_session.py`

 * *Files identical despite different names*

### Comparing `openjd_sessions-0.7.1/openjd/sessions/_session_user.py` & `openjd_sessions-0.7.2/openjd/sessions/_session_user.py`

 * *Files identical despite different names*

### Comparing `openjd_sessions-0.7.1/openjd/sessions/_subprocess.py` & `openjd_sessions-0.7.2/openjd/sessions/_subprocess.py`

 * *Files identical despite different names*

### Comparing `openjd_sessions-0.7.1/openjd/sessions/_tempdir.py` & `openjd_sessions-0.7.2/openjd/sessions/_tempdir.py`

 * *Files identical despite different names*

### Comparing `openjd_sessions-0.7.1/openjd/sessions/_types.py` & `openjd_sessions-0.7.2/openjd/sessions/_types.py`

 * *Files identical despite different names*

### Comparing `openjd_sessions-0.7.1/openjd/sessions/_windows_permission_helper.py` & `openjd_sessions-0.7.2/openjd/sessions/_windows_permission_helper.py`

 * *Files identical despite different names*

### Comparing `openjd_sessions-0.7.1/openjd/sessions/_windows_process_killer.py` & `openjd_sessions-0.7.2/openjd/sessions/_windows_process_killer.py`

 * *Files identical despite different names*

### Comparing `openjd_sessions-0.7.1/openjd/sessions/_scripts/_posix/_signal_subprocess.sh` & `openjd_sessions-0.7.2/openjd/sessions/_scripts/_posix/_signal_subprocess.sh`

 * *Files identical despite different names*

### Comparing `openjd_sessions-0.7.1/openjd/sessions/_scripts/_windows/_signal_win_subprocess.py` & `openjd_sessions-0.7.2/openjd/sessions/_scripts/_windows/_signal_win_subprocess.py`

 * *Files identical despite different names*

### Comparing `openjd_sessions-0.7.1/openjd/sessions/_win32/_api.py` & `openjd_sessions-0.7.2/openjd/sessions/_win32/_api.py`

 * *Files identical despite different names*

### Comparing `openjd_sessions-0.7.1/openjd/sessions/_win32/_helpers.py` & `openjd_sessions-0.7.2/openjd/sessions/_win32/_helpers.py`

 * *Files identical despite different names*

### Comparing `openjd_sessions-0.7.1/openjd/sessions/_win32/_locate_executable.py` & `openjd_sessions-0.7.2/openjd/sessions/_win32/_locate_executable.py`

 * *Files identical despite different names*

### Comparing `openjd_sessions-0.7.1/openjd/sessions/_win32/_popen_as_user.py` & `openjd_sessions-0.7.2/openjd/sessions/_win32/_popen_as_user.py`

 * *Files identical despite different names*

### Comparing `openjd_sessions-0.7.1/LICENSE` & `openjd_sessions-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openjd_sessions-0.7.1/README.md` & `openjd_sessions-0.7.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # Open Job Description - Sessions for Python
 
 [![pypi](https://img.shields.io/pypi/v/openjd-sessions.svg)](https://pypi.python.org/pypi/openjd-sessions)
+[![python](https://img.shields.io/pypi/pyversions/openjd-sessions.svg?style=flat)](https://pypi.python.org/pypi/openjd-sessions)
+[![license](https://img.shields.io/pypi/l/openjd-sessions.svg?style=flat)](https://github.com/OpenJobDescription/openjd-sessions/blob/mainline/LICENSE)
 
 Open Job Description is a flexible open specification for defining render jobs which are portable
 between studios and render solutions. This package provides a library that can be used to build
 a runtime that is able to run Jobs in a
 [Session](https://github.com/OpenJobDescription/openjd-specifications/wiki/How-Jobs-Are-Run#sessions)
 as defined by Open Job Description.
 
@@ -17,20 +19,14 @@
 
 1. Python 3.9 or higher;
 2. Linux, MacOS, or Windows operating system;
 3. On Linux/MacOS:
     * `sudo`
 4. On Windows:
     * CPython implementation of Python
-    * PowerShell 5.x
-
-**EXPERIMENTAL** Note that compatibility with the Windows operating system is currently in active development
-and should be considered to be experimental. We recommend that this library not be used in Windows-based
-production environments at this time. We will remove this notice when Windows compatibility is considered
-sufficiently stable and secure for use in Windows-based production environments.
 
 ## Versioning
 
 This package's version follows [Semantic Versioning 2.0](https://semver.org/), but is still considered to be in its 
 initial development, thus backwards incompatible versions are denoted by minor version bumps. To help illustrate how
 versions will increment during this initial development stage, they are described below:
```

### Comparing `openjd_sessions-0.7.1/hatch.toml` & `openjd_sessions-0.7.2/hatch.toml`

 * *Files identical despite different names*

### Comparing `openjd_sessions-0.7.1/pyproject.toml` & `openjd_sessions-0.7.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 [build-system]
 requires = ["hatchling", "hatch-vcs"]
 build-backend = "hatchling.build"
 
 [project]
 name = "openjd-sessions"
+authors = [
+  {name = "Amazon Web Services"},
+]
 dynamic = ["version"]
 readme = "README.md"
 license = "Apache-2.0"
 requires-python = ">=3.9"
 description = "Provides a library that can be used to build a runtime that is able to run Jobs in a Session as defined by Open Job Description."
 # https://pypi.org/classifiers/
 classifiers = [
```

### Comparing `openjd_sessions-0.7.1/PKG-INFO` & `openjd_sessions-0.7.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.3
 Name: openjd-sessions
-Version: 0.7.1
+Version: 0.7.2
 Summary: Provides a library that can be used to build a runtime that is able to run Jobs in a Session as defined by Open Job Description.
 Project-URL: Homepage, https://github.com/OpenJobDescription/openjd-sessions-for-python
 Project-URL: Source, https://github.com/OpenJobDescription/openjd-sessions-for-python
+Author: Amazon Web Services
 License-Expression: Apache-2.0
 License-File: LICENSE
 License-File: NOTICE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
@@ -25,14 +26,16 @@
 Requires-Dist: psutil==5.9.*; platform_system == 'Windows'
 Requires-Dist: pywin32==306; platform_system == 'Windows'
 Description-Content-Type: text/markdown
 
 # Open Job Description - Sessions for Python
 
 [![pypi](https://img.shields.io/pypi/v/openjd-sessions.svg)](https://pypi.python.org/pypi/openjd-sessions)
+[![python](https://img.shields.io/pypi/pyversions/openjd-sessions.svg?style=flat)](https://pypi.python.org/pypi/openjd-sessions)
+[![license](https://img.shields.io/pypi/l/openjd-sessions.svg?style=flat)](https://github.com/OpenJobDescription/openjd-sessions/blob/mainline/LICENSE)
 
 Open Job Description is a flexible open specification for defining render jobs which are portable
 between studios and render solutions. This package provides a library that can be used to build
 a runtime that is able to run Jobs in a
 [Session](https://github.com/OpenJobDescription/openjd-specifications/wiki/How-Jobs-Are-Run#sessions)
 as defined by Open Job Description.
 
@@ -45,20 +48,14 @@
 
 1. Python 3.9 or higher;
 2. Linux, MacOS, or Windows operating system;
 3. On Linux/MacOS:
     * `sudo`
 4. On Windows:
     * CPython implementation of Python
-    * PowerShell 5.x
-
-**EXPERIMENTAL** Note that compatibility with the Windows operating system is currently in active development
-and should be considered to be experimental. We recommend that this library not be used in Windows-based
-production environments at this time. We will remove this notice when Windows compatibility is considered
-sufficiently stable and secure for use in Windows-based production environments.
 
 ## Versioning
 
 This package's version follows [Semantic Versioning 2.0](https://semver.org/), but is still considered to be in its 
 initial development, thus backwards incompatible versions are denoted by minor version bumps. To help illustrate how
 versions will increment during this initial development stage, they are described below:
```

