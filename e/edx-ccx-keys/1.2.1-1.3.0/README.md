# Comparing `tmp/edx-ccx-keys-1.2.1.tar.gz` & `tmp/edx-ccx-keys-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-ccx-keys-1.2.1.tar", last modified: Fri May 28 14:36:27 2021, max compression
+gzip compressed data, was "edx-ccx-keys-1.3.0.tar", last modified: Tue Apr 16 18:30:12 2024, max compression
```

## Comparing `edx-ccx-keys-1.2.1.tar` & `edx-ccx-keys-1.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-05-28 14:36:27.397282 edx-ccx-keys-1.2.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)       32 2021-05-28 14:35:29.000000 edx-ccx-keys-1.2.1/AUTHORS
--rw-rw-r--   0 travis    (2000) travis    (2000)    34500 2021-05-28 14:35:29.000000 edx-ccx-keys-1.2.1/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      140 2021-05-28 14:35:29.000000 edx-ccx-keys-1.2.1/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      681 2021-05-28 14:36:27.397282 edx-ccx-keys-1.2.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      879 2021-05-28 14:35:29.000000 edx-ccx-keys-1.2.1/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-05-28 14:36:27.393284 edx-ccx-keys-1.2.1/ccx_keys/
--rw-rw-r--   0 travis    (2000) travis    (2000)       10 2021-05-28 14:35:29.000000 edx-ccx-keys-1.2.1/ccx_keys/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      279 2021-05-28 14:35:29.000000 edx-ccx-keys-1.2.1/ccx_keys/key.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6046 2021-05-28 14:35:29.000000 edx-ccx-keys-1.2.1/ccx_keys/locator.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-05-28 14:36:27.397282 edx-ccx-keys-1.2.1/ccx_keys/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)       10 2021-05-28 14:35:29.000000 edx-ccx-keys-1.2.1/ccx_keys/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16062 2021-05-28 14:35:29.000000 edx-ccx-keys-1.2.1/ccx_keys/tests/test_ccx_keys.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-05-28 14:36:27.397282 edx-ccx-keys-1.2.1/edx_ccx_keys.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      681 2021-05-28 14:36:27.000000 edx-ccx-keys-1.2.1/edx_ccx_keys.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      402 2021-05-28 14:36:27.000000 edx-ccx-keys-1.2.1/edx_ccx_keys.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-05-28 14:36:27.000000 edx-ccx-keys-1.2.1/edx_ccx_keys.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      118 2021-05-28 14:36:27.000000 edx-ccx-keys-1.2.1/edx_ccx_keys.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       35 2021-05-28 14:36:27.000000 edx-ccx-keys-1.2.1/edx_ccx_keys.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2021-05-28 14:36:27.000000 edx-ccx-keys-1.2.1/edx_ccx_keys.egg-info/top_level.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-05-28 14:36:27.397282 edx-ccx-keys-1.2.1/requirements/
--rw-rw-r--   0 travis    (2000) travis    (2000)      102 2021-05-28 14:35:29.000000 edx-ccx-keys-1.2.1/requirements/base.in
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-05-28 14:36:27.397282 edx-ccx-keys-1.2.1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1822 2021-05-28 14:35:29.000000 edx-ccx-keys-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:30:12.130379 edx-ccx-keys-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-16 18:30:09.000000 edx-ccx-keys-1.3.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    34500 2024-04-16 18:30:09.000000 edx-ccx-keys-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-16 18:30:09.000000 edx-ccx-keys-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-16 18:30:12.130379 edx-ccx-keys-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-16 18:30:09.000000 edx-ccx-keys-1.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:30:12.130379 edx-ccx-keys-1.3.0/ccx_keys/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-16 18:30:09.000000 edx-ccx-keys-1.3.0/ccx_keys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-16 18:30:09.000000 edx-ccx-keys-1.3.0/ccx_keys/key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-04-16 18:30:09.000000 edx-ccx-keys-1.3.0/ccx_keys/locator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:30:12.130379 edx-ccx-keys-1.3.0/ccx_keys/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 18:30:09.000000 edx-ccx-keys-1.3.0/ccx_keys/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16022 2024-04-16 18:30:09.000000 edx-ccx-keys-1.3.0/ccx_keys/tests/test_ccx_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:30:12.130379 edx-ccx-keys-1.3.0/edx_ccx_keys.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-16 18:30:12.000000 edx-ccx-keys-1.3.0/edx_ccx_keys.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-16 18:30:12.000000 edx-ccx-keys-1.3.0/edx_ccx_keys.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 18:30:12.000000 edx-ccx-keys-1.3.0/edx_ccx_keys.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-16 18:30:12.000000 edx-ccx-keys-1.3.0/edx_ccx_keys.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-16 18:30:12.000000 edx-ccx-keys-1.3.0/edx_ccx_keys.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 18:30:12.000000 edx-ccx-keys-1.3.0/edx_ccx_keys.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:30:12.130379 edx-ccx-keys-1.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-16 18:30:09.000000 edx-ccx-keys-1.3.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 18:30:12.130379 edx-ccx-keys-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-16 18:30:09.000000 edx-ccx-keys-1.3.0/setup.py
```

### Comparing `edx-ccx-keys-1.2.1/LICENSE` & `edx-ccx-keys-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-ccx-keys-1.2.1/PKG-INFO` & `edx-ccx-keys-1.3.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,19 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: edx-ccx-keys
-Version: 1.2.1
+Version: 1.3.0
 Summary: Opaque key support custom courses on edX
-Home-page: https://github.com/edx/ccx-keys
+Home-page: https://github.com/openedx/ccx-keys
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL
+Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
-License-File: LICENSE
-License-File: AUTHORS
-
-UNKNOWN
-
+Classifier: Programming Language :: Python :: 3.11
```

### Comparing `edx-ccx-keys-1.2.1/ccx_keys/locator.py` & `edx-ccx-keys-1.3.0/ccx_keys/locator.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,32 +70,29 @@
         )
         return new_obj
 
     def to_course_locator(self):
         """
         Returns a CourseLocator representing this location.
         """
-        # pylint: disable=no-member
         return CourseLocator(
             org=self.org,
             course=self.course,
             run=self.run,
             branch=self.branch,
             version_guid=self.version_guid
         )
 
     def _to_string(self):
         """
         Return a string representing this location.
         """
         string = super()._to_string()
         # append the identifier for the ccx to the existing course string
-        string += "+{prefix}@{ccx}".format(
-            prefix=self.CCX_PREFIX, ccx=self.ccx
-        )
+        string += f"+{self.CCX_PREFIX}@{self.ccx}"
         return string
 
     def _to_deprecated_string(self):
         """ CCXLocators are never deprecated. """
         raise NotImplementedError
 
     @classmethod
@@ -144,15 +141,15 @@
     @classmethod
     def _from_string(cls, serialized):
         """
         Requests CCXLocator to deserialize its part and then adds the local
         deserialization of block
         """
         # Allow access to _from_string protected method
-        course_key = CCXLocator._from_string(serialized)  # pylint: disable=protected-access
+        course_key = CCXLocator._from_string(serialized)
         parsed_parts = cls.parse_url(serialized)
         block_id = parsed_parts.get('block_id', None)
         if block_id is None:
             raise InvalidKeyError(cls, serialized)
         return cls(course_key, parsed_parts.get('block_type'), block_id)
 
     @property
```

### Comparing `edx-ccx-keys-1.2.1/ccx_keys/tests/test_ccx_keys.py` & `edx-ccx-keys-1.3.0/ccx_keys/tests/test_ccx_keys.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """ Tests for the ccx_keys package. """
-import ddt
-import itertools  # pylint: disable=wrong-import-order
+import itertools
+
+import ddt  # pylint: disable=import-error
 from bson.objectid import ObjectId
 from opaque_keys import InvalidKeyError
 from opaque_keys.edx.keys import CourseKey, UsageKey
 from opaque_keys.edx.locator import CourseLocator
 from opaque_keys.edx.tests import LocatorBaseTest, TestDeprecated
 
 from ccx_keys.locator import CCXBlockUsageLocator, CCXLocator
@@ -304,15 +305,15 @@
             UsageKey.from_string(url)
 
     @ddt.data(
         ('org', 'course', 'run', '1', 'category', 'name', None),
         ('org', 'course', 'run', '1', 'category', 'name:more_name', None),
     )
     @ddt.unpack
-    def test_valid_locations(self, org, course, run, ccx, category, name, revision):  # pylint: disable=unused-argument
+    def test_valid_locations(self, org, course, run, ccx, category, name, revision):
         course_key = CCXLocator(org=org, course=course, run=run, branch=revision, ccx=ccx)
         locator = CCXBlockUsageLocator(course_key, block_type=category, block_id=name, )
         self.assertEqual(org, locator.org)
         self.assertEqual(course, locator.course)
         self.assertEqual(run, locator.run)
         self.assertEqual(ccx, locator.ccx)
         self.assertEqual(category, locator.block_type)
```

### Comparing `edx-ccx-keys-1.2.1/edx_ccx_keys.egg-info/PKG-INFO` & `edx-ccx-keys-1.3.0/edx_ccx_keys.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,19 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: edx-ccx-keys
-Version: 1.2.1
+Version: 1.3.0
 Summary: Opaque key support custom courses on edX
-Home-page: https://github.com/edx/ccx-keys
+Home-page: https://github.com/openedx/ccx-keys
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL
+Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
-License-File: LICENSE
-License-File: AUTHORS
-
-UNKNOWN
-
+Classifier: Programming Language :: Python :: 3.11
```

