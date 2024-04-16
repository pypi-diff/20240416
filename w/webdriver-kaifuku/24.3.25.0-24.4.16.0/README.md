# Comparing `tmp/webdriver_kaifuku-24.3.25.0.tar.gz` & `tmp/webdriver_kaifuku-24.4.16.0.tar.gz`

## Comparing `webdriver_kaifuku-24.3.25.0.tar` & `webdriver_kaifuku-24.4.16.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     8831 2020-02-02 00:00:00.000000 webdriver_kaifuku-24.3.25.0/src/webdriver_kaifuku/__init__.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 webdriver_kaifuku-24.3.25.0/src/webdriver_kaifuku/tries.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 webdriver_kaifuku-24.3.25.0/.gitignore
--rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 webdriver_kaifuku-24.3.25.0/LICENSE
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 webdriver_kaifuku-24.3.25.0/README.md
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 webdriver_kaifuku-24.3.25.0/pyproject.toml
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 webdriver_kaifuku-24.3.25.0/PKG-INFO
+-rw-r--r--   0        0        0     8831 2020-02-02 00:00:00.000000 webdriver_kaifuku-24.4.16.0/src/webdriver_kaifuku/__init__.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 webdriver_kaifuku-24.4.16.0/src/webdriver_kaifuku/tries.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 webdriver_kaifuku-24.4.16.0/.gitignore
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 webdriver_kaifuku-24.4.16.0/LICENSE
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 webdriver_kaifuku-24.4.16.0/README.md
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 webdriver_kaifuku-24.4.16.0/pyproject.toml
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 webdriver_kaifuku-24.4.16.0/PKG-INFO
```

### Comparing `webdriver_kaifuku-24.3.25.0/src/webdriver_kaifuku/__init__.py` & `webdriver_kaifuku-24.4.16.0/src/webdriver_kaifuku/__init__.py`

 * *Files identical despite different names*

### Comparing `webdriver_kaifuku-24.3.25.0/src/webdriver_kaifuku/tries.py` & `webdriver_kaifuku-24.4.16.0/src/webdriver_kaifuku/tries.py`

 * *Files identical despite different names*

### Comparing `webdriver_kaifuku-24.3.25.0/.gitignore` & `webdriver_kaifuku-24.4.16.0/.gitignore`

 * *Files identical despite different names*

### Comparing `webdriver_kaifuku-24.3.25.0/LICENSE` & `webdriver_kaifuku-24.4.16.0/LICENSE`

 * *Files identical despite different names*

### Comparing `webdriver_kaifuku-24.3.25.0/README.md` & `webdriver_kaifuku-24.4.16.0/README.md`

 * *Files identical despite different names*

### Comparing `webdriver_kaifuku-24.3.25.0/pyproject.toml` & `webdriver_kaifuku-24.4.16.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,45 @@
 [project]
 classifiers = [
   "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Topic :: Software Development :: Quality Assurance",
   "Topic :: Software Development :: Testing",
 ]
 description = "Restartable webdriver instances"
 dynamic = ["version"]
 keywords = ["selenium"]
 license_file = "LICENSE"
 name = "webdriver_kaifuku"
 readme = "README.md"
 requires-python = ">=3.8"
+maintainers = [
+  {name="Ronny Pfannschmidt", email="rpfannsc@redhat.com"},
+  {name="Nikhil Dhandre", email="ndhandre@redhat.com"},
+]
 
 dependencies = [
   "attrs",
   "requests",
   "selenium>=4.0.0",
 ]
 
 [project.optional-dependencies]
 test = [
   "pytest",
   "wait_for",
 ]
 
 [project.urls]
-repository = "https://github.com/RonnyPfannschmidt/webdriver_kaifuku"
+repository = "https://github.com/RedHatQE/webdriver_kaifuku"
 
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling", "hatch-vcs"]
 
 [tool.hatch.build.targets.sdist]
 include = ["/src"]
```

### Comparing `webdriver_kaifuku-24.3.25.0/PKG-INFO` & `webdriver_kaifuku-24.4.16.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.3
 Name: webdriver_kaifuku
-Version: 24.3.25.0
+Version: 24.4.16.0
 Summary: Restartable webdriver instances
-Project-URL: repository, https://github.com/RonnyPfannschmidt/webdriver_kaifuku
+Project-URL: repository, https://github.com/RedHatQE/webdriver_kaifuku
+Maintainer-email: Ronny Pfannschmidt <rpfannsc@redhat.com>, Nikhil Dhandre <ndhandre@redhat.com>
 License-File: LICENSE
 Keywords: selenium
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.8
 Requires-Dist: attrs
 Requires-Dist: requests
 Requires-Dist: selenium>=4.0.0
 Provides-Extra: test
```

#### html2text {}

```diff
@@ -1,14 +1,17 @@
-Metadata-Version: 2.3 Name: webdriver_kaifuku Version: 24.3.25.0 Summary:
+Metadata-Version: 2.3 Name: webdriver_kaifuku Version: 24.4.16.0 Summary:
 Restartable webdriver instances Project-URL: repository, https://github.com/
-RonnyPfannschmidt/webdriver_kaifuku License-File: LICENSE Keywords: selenium
-Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Topic ::
+RedHatQE/webdriver_kaifuku Maintainer-email: Ronny Pfannschmidt
+redhat.com>, Nikhil Dhandre
+redhat.com> License-File: LICENSE Keywords: selenium Classifier: License :: OSI
+Approved :: Mozilla Public License 2.0 (MPL 2.0) Classifier: Programming
+Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
+3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12 Classifier: Topic ::
 Software Development :: Quality Assurance Classifier: Topic :: Software
 Development :: Testing Requires-Python: >=3.8 Requires-Dist: attrs Requires-
 Dist: requests Requires-Dist: selenium>=4.0.0 Provides-Extra: test Requires-
 Dist: pytest; extra == 'test' Requires-Dist: wait-for; extra == 'test'
 Description-Content-Type: text/markdown
                         ************ wweebbddrriivveerr__kkaaiiffuukkuu ************
                    ******** RReessttaarrttaabbllee wweebbddrriivveerr iinnssttaanncceess ********
```

