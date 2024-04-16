# Comparing `tmp/password-library-0.4.0.tar.gz` & `tmp/password_library-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "password-library-0.4.0.tar", last modified: Tue Dec 19 13:58:36 2023, max compression
+gzip compressed data, was "password_library-0.4.1.tar", last modified: Tue Apr 16 10:52:05 2024, max compression
```

## Comparing `password-library-0.4.0.tar` & `password_library-0.4.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2023-12-19 13:58:36.483194 password-library-0.4.0/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1065 2023-09-07 08:06:48.000000 password-library-0.4.0/LICENSE
--rw-r--r--   0 playerg9  (1000) playerg9  (1000)     5297 2023-12-19 13:58:36.483194 password-library-0.4.0/PKG-INFO
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     4061 2023-12-19 13:58:21.000000 password-library-0.4.0/README.md
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       87 2023-09-07 08:34:27.000000 password-library-0.4.0/pyproject.toml
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       38 2023-12-19 13:58:36.483194 password-library-0.4.0/setup.cfg
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1727 2023-09-17 09:51:32.000000 password-library-0.4.0/setup.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2023-12-19 13:58:36.479194 password-library-0.4.0/src/
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2023-12-19 13:58:36.483194 password-library-0.4.0/src/password_library.egg-info/
--rw-r--r--   0 playerg9  (1000) playerg9  (1000)     5297 2023-12-19 13:58:36.000000 password-library-0.4.0/src/password_library.egg-info/PKG-INFO
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      806 2023-12-19 13:58:36.000000 password-library-0.4.0/src/password_library.egg-info/SOURCES.txt
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)        1 2023-12-19 13:58:36.000000 password-library-0.4.0/src/password_library.egg-info/dependency_links.txt
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       12 2023-12-19 13:58:36.000000 password-library-0.4.0/src/password_library.egg-info/top_level.txt
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2023-12-19 13:58:36.479194 password-library-0.4.0/src/passwordlib/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1581 2023-12-19 13:58:21.000000 password-library-0.4.0/src/passwordlib/__init__.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2023-12-19 13:58:36.483194 password-library-0.4.0/src/passwordlib/analyzer/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      132 2023-09-10 10:20:59.000000 password-library-0.4.0/src/passwordlib/analyzer/__init__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     3866 2023-09-08 17:47:43.000000 password-library-0.4.0/src/passwordlib/analyzer/analyzer.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2023-12-19 13:58:36.483194 password-library-0.4.0/src/passwordlib/attr/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      165 2023-09-10 10:20:59.000000 password-library-0.4.0/src/passwordlib/attr/__init__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2154 2023-09-09 21:24:38.000000 password-library-0.4.0/src/passwordlib/attr/attribute_class.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2023-12-19 13:58:36.483194 password-library-0.4.0/src/passwordlib/commonly_used/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      263 2023-09-07 13:15:14.000000 password-library-0.4.0/src/passwordlib/commonly_used/__init__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)   781879 2023-09-07 13:08:57.000000 password-library-0.4.0/src/passwordlib/commonly_used/password-list.txt
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      687 2023-09-08 17:37:38.000000 password-library-0.4.0/src/passwordlib/commonly_used/verifier.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      135 2023-09-07 12:15:10.000000 password-library-0.4.0/src/passwordlib/config.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2023-12-19 13:58:36.483194 password-library-0.4.0/src/passwordlib/util/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      428 2023-09-10 10:20:59.000000 password-library-0.4.0/src/passwordlib/util/__init__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     5086 2023-12-19 13:40:47.000000 password-library-0.4.0/src/passwordlib/util/dumping.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1649 2023-12-19 13:58:21.000000 password-library-0.4.0/src/passwordlib/util/functions.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     3014 2023-12-19 13:58:20.000000 password-library-0.4.0/src/passwordlib/util/hashing.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2023-12-19 13:58:36.483194 password-library-0.4.0/tests/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2236 2023-09-07 15:24:30.000000 password-library-0.4.0/tests/test_analyzer.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      790 2023-09-07 13:21:04.000000 password-library-0.4.0/tests/test_attribute.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      604 2023-09-07 13:41:30.000000 password-library-0.4.0/tests/test_commonly_used_passwords.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      218 2023-09-07 09:00:23.000000 password-library-0.4.0/tests/test_import.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2847 2023-09-07 13:21:04.000000 password-library-0.4.0/tests/test_util.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-16 10:52:05.320460 password_library-0.4.1/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1065 2024-04-16 10:43:16.000000 password_library-0.4.1/LICENSE
+-rw-r--r--   0 playerg9  (1000) playerg9  (1000)     5297 2024-04-16 10:52:05.320460 password_library-0.4.1/PKG-INFO
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     4061 2024-04-16 10:43:16.000000 password_library-0.4.1/README.md
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       87 2024-04-16 10:43:16.000000 password_library-0.4.1/pyproject.toml
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       38 2024-04-16 10:52:05.320460 password_library-0.4.1/setup.cfg
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1727 2024-04-16 10:43:16.000000 password_library-0.4.1/setup.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-16 10:52:05.308457 password_library-0.4.1/src/
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-16 10:52:05.320460 password_library-0.4.1/src/password_library.egg-info/
+-rw-r--r--   0 playerg9  (1000) playerg9  (1000)     5297 2024-04-16 10:52:05.000000 password_library-0.4.1/src/password_library.egg-info/PKG-INFO
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      806 2024-04-16 10:52:05.000000 password_library-0.4.1/src/password_library.egg-info/SOURCES.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)        1 2024-04-16 10:52:05.000000 password_library-0.4.1/src/password_library.egg-info/dependency_links.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       12 2024-04-16 10:52:05.000000 password_library-0.4.1/src/password_library.egg-info/top_level.txt
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-16 10:52:05.312458 password_library-0.4.1/src/passwordlib/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1581 2024-04-16 10:51:00.000000 password_library-0.4.1/src/passwordlib/__init__.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-16 10:52:05.312458 password_library-0.4.1/src/passwordlib/analyzer/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      132 2024-04-16 10:43:16.000000 password_library-0.4.1/src/passwordlib/analyzer/__init__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     3866 2024-04-16 10:43:16.000000 password_library-0.4.1/src/passwordlib/analyzer/analyzer.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-16 10:52:05.312458 password_library-0.4.1/src/passwordlib/attr/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      165 2024-04-16 10:43:16.000000 password_library-0.4.1/src/passwordlib/attr/__init__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2154 2024-04-16 10:43:16.000000 password_library-0.4.1/src/passwordlib/attr/attribute_class.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-16 10:52:05.316459 password_library-0.4.1/src/passwordlib/commonly_used/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      263 2024-04-16 10:43:16.000000 password_library-0.4.1/src/passwordlib/commonly_used/__init__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)   781879 2024-04-16 10:43:16.000000 password_library-0.4.1/src/passwordlib/commonly_used/password-list.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      687 2024-04-16 10:43:16.000000 password_library-0.4.1/src/passwordlib/commonly_used/verifier.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      135 2024-04-16 10:43:16.000000 password_library-0.4.1/src/passwordlib/config.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-16 10:52:05.316459 password_library-0.4.1/src/passwordlib/util/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      428 2024-04-16 10:43:16.000000 password_library-0.4.1/src/passwordlib/util/__init__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     5086 2024-04-16 10:43:16.000000 password_library-0.4.1/src/passwordlib/util/dumping.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1649 2024-04-16 10:43:16.000000 password_library-0.4.1/src/passwordlib/util/functions.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     3215 2024-04-16 10:49:06.000000 password_library-0.4.1/src/passwordlib/util/hashing.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-16 10:52:05.320460 password_library-0.4.1/tests/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2236 2024-04-16 10:43:16.000000 password_library-0.4.1/tests/test_analyzer.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      979 2024-04-16 10:43:16.000000 password_library-0.4.1/tests/test_attribute.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      604 2024-04-16 10:43:16.000000 password_library-0.4.1/tests/test_commonly_used_passwords.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      218 2024-04-16 10:43:16.000000 password_library-0.4.1/tests/test_import.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2847 2024-04-16 10:43:16.000000 password_library-0.4.1/tests/test_util.py
```

### Comparing `password-library-0.4.0/LICENSE` & `password_library-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `password-library-0.4.0/PKG-INFO` & `password_library-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: password-library
-Version: 0.4.0
+Version: 0.4.1
 Summary: utility library to verify, hash, compare and more for passwords
 Home-page: https://github.com/PlayerG9/passwordlib-py/
 Author: PlayerG9
 License: MIT
 Project-URL: Author Github, https://github.com/PlayerG9
 Project-URL: Homepage, https://github.com/PlayerG9/passwordlib-py/
 Project-URL: Bug Tracker, https://github.com/PlayerG9/passwordlib-py/issues
```

### Comparing `password-library-0.4.0/README.md` & `password_library-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `password-library-0.4.0/setup.py` & `password_library-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `password-library-0.4.0/src/password_library.egg-info/PKG-INFO` & `password_library-0.4.1/src/password_library.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: password-library
-Version: 0.4.0
+Version: 0.4.1
 Summary: utility library to verify, hash, compare and more for passwords
 Home-page: https://github.com/PlayerG9/passwordlib-py/
 Author: PlayerG9
 License: MIT
 Project-URL: Author Github, https://github.com/PlayerG9
 Project-URL: Homepage, https://github.com/PlayerG9/passwordlib-py/
 Project-URL: Bug Tracker, https://github.com/PlayerG9/passwordlib-py/issues
```

### Comparing `password-library-0.4.0/src/password_library.egg-info/SOURCES.txt` & `password_library-0.4.1/src/password_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `password-library-0.4.0/src/passwordlib/__init__.py` & `password_library-0.4.1/src/passwordlib/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,13 +27,13 @@
 __copyright__ = "Copyright 2023, PlayerG9"
 __credits__ = ["PlayerG9"]
 __license__ = "MIT"
 __maintainer__ = "PlayerG9"
 __email__ = None
 __status__ = "Prototype"  # Prototype, Development, Production
 __description__ = "utility library to verify, hash, compare and more for passwords"
-__version_info__ = (0, 4, 0)
+__version_info__ = (0, 4, 1)
 __version__ = '.'.join(str(_) for _ in __version_info__)
 
 from . import config
 from . import util
 from .util import hash_password, compare_password
```

### Comparing `password-library-0.4.0/src/passwordlib/analyzer/analyzer.py` & `password_library-0.4.1/src/passwordlib/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `password-library-0.4.0/src/passwordlib/attr/attribute_class.py` & `password_library-0.4.1/src/passwordlib/attr/attribute_class.py`

 * *Files identical despite different names*

### Comparing `password-library-0.4.0/src/passwordlib/commonly_used/password-list.txt` & `password_library-0.4.1/src/passwordlib/commonly_used/password-list.txt`

 * *Files identical despite different names*

### Comparing `password-library-0.4.0/src/passwordlib/commonly_used/verifier.py` & `password_library-0.4.1/src/passwordlib/commonly_used/verifier.py`

 * *Files identical despite different names*

### Comparing `password-library-0.4.0/src/passwordlib/util/dumping.py` & `password_library-0.4.1/src/passwordlib/util/dumping.py`

 * *Files identical despite different names*

### Comparing `password-library-0.4.0/src/passwordlib/util/functions.py` & `password_library-0.4.1/src/passwordlib/util/functions.py`

 * *Files identical despite different names*

### Comparing `password-library-0.4.0/src/passwordlib/util/hashing.py` & `password_library-0.4.1/src/passwordlib/util/hashing.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,18 +24,23 @@
     :return: the hashed password
     """
     password = fn.get_password_bytes(password)
     algorithm = fn.get_algorithm(algorithm)
     iterations = fn.get_iterations(iterations)
     salt = fn.get_salt(salt)
     if algorithm == "scrypt":
+        n = iterations
+        # todo: make r & p configurable
+        r = 8  # maybe 16 better?
+        p = 1  # only one thread
         return hashlib.scrypt(
             password=password,
             salt=salt,
-            n=iterations,
+            n=n, r=r, p=p, maxmem=128 * n * r * p,
+            dklen=64,  # 64 bytes => 512 bits
         )
     else:
         return hashlib.pbkdf2_hmac(
             hash_name=algorithm,
             password=password,
             salt=salt,
             iterations=iterations,
```

### Comparing `password-library-0.4.0/tests/test_analyzer.py` & `password_library-0.4.1/tests/test_analyzer.py`

 * *Files identical despite different names*

### Comparing `password-library-0.4.0/tests/test_attribute.py` & `password_library-0.4.1/tests/test_attribute.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,31 +7,34 @@
 
 
 class TestAttribute(unittest.TestCase):
     def test_import(self):
         import passwordlib.attr # noqa
 
     def test_set(self):
+        from passwordlib.util import compare_password
         from passwordlib.attr import PasswordAttribute
 
         class User:
             name: str
             password = PasswordAttribute()
 
         user = User()
         self.assertEquals(user.password, None)
 
         user.password = "secret"
         self.assertNotEquals(user.password, "secret")
+        self.assertTrue(compare_password("secret", user.password))
 
         user.password = None
         self.assertEquals(user.password, None)
 
         user.password = "secret2"
         self.assertNotEquals(user.password, "secret2")
+        self.assertTrue(compare_password("secret2", user.password))
 
         del user.password
         self.assertEquals(user.password, None)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `password-library-0.4.0/tests/test_commonly_used_passwords.py` & `password_library-0.4.1/tests/test_commonly_used_passwords.py`

 * *Files identical despite different names*

### Comparing `password-library-0.4.0/tests/test_util.py` & `password_library-0.4.1/tests/test_util.py`

 * *Files identical despite different names*

