# Comparing `tmp/templatise-2.2.4.tar.gz` & `tmp/templatise-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templatise-2.2.4.tar", max compression
+gzip compressed data, was "templatise-2.2.5.tar", max compression
```

## Comparing `templatise-2.2.4.tar` & `templatise-2.2.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1211 2024-03-31 11:50:49.898565 templatise-2.2.4/LICENSE
--rw-r--r--   0        0        0     1942 2024-03-31 11:50:49.898565 templatise-2.2.4/README.md
--rw-r--r--   0        0        0     1860 2024-03-31 11:50:49.898565 templatise-2.2.4/pyproject.toml
--rw-r--r--   0        0        0       19 2024-03-31 11:50:49.906565 templatise-2.2.4/templatise/__init__.py
--rw-r--r--   0        0        0     3813 2024-03-31 11:50:49.906565 templatise-2.2.4/templatise/actions.py
--rw-r--r--   0        0        0     2647 2024-03-31 11:50:49.906565 templatise-2.2.4/templatise/configuration.py
--rw-r--r--   0        0        0      999 2024-03-31 11:50:49.906565 templatise-2.2.4/templatise/git.py
--rw-r--r--   0        0        0     3546 2024-03-31 11:50:49.906565 templatise-2.2.4/templatise/initialise.py
--rw-r--r--   0        0        0     1140 2024-03-31 11:50:49.906565 templatise-2.2.4/templatise/licence.py
--rw-r--r--   0        0        0   251608 2024-03-31 11:50:49.910565 templatise-2.2.4/templatise/licenses.json
--rw-r--r--   0        0        0      994 2024-03-31 11:50:49.910565 templatise-2.2.4/templatise/project_name.py
--rw-r--r--   0        0        0     3423 1970-01-01 00:00:00.000000 templatise-2.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-16 07:50:18.953802 templatise-2.2.5/LICENSE
+-rw-r--r--   0        0        0     1942 2024-04-16 07:50:18.953802 templatise-2.2.5/README.md
+-rw-r--r--   0        0        0     1860 2024-04-16 07:50:18.953802 templatise-2.2.5/pyproject.toml
+-rw-r--r--   0        0        0       19 2024-04-16 07:50:18.961803 templatise-2.2.5/templatise/__init__.py
+-rw-r--r--   0        0        0     3813 2024-04-16 07:50:18.961803 templatise-2.2.5/templatise/actions.py
+-rw-r--r--   0        0        0     2647 2024-04-16 07:50:18.961803 templatise-2.2.5/templatise/configuration.py
+-rw-r--r--   0        0        0      999 2024-04-16 07:50:18.961803 templatise-2.2.5/templatise/git.py
+-rw-r--r--   0        0        0     3546 2024-04-16 07:50:18.961803 templatise-2.2.5/templatise/initialise.py
+-rw-r--r--   0        0        0     1140 2024-04-16 07:50:18.961803 templatise-2.2.5/templatise/licence.py
+-rw-r--r--   0        0        0   251608 2024-04-16 07:50:18.961803 templatise-2.2.5/templatise/licenses.json
+-rw-r--r--   0        0        0      994 2024-04-16 07:50:18.961803 templatise-2.2.5/templatise/project_name.py
+-rw-r--r--   0        0        0     3423 1970-01-01 00:00:00.000000 templatise-2.2.5/PKG-INFO
```

### Comparing `templatise-2.2.4/LICENSE` & `templatise-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `templatise-2.2.4/README.md` & `templatise-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `templatise-2.2.4/pyproject.toml` & `templatise-2.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 description = "You can use template.py to create a new GitHub repository."
 include = ["templatise/licenses.json"]
 keywords = ["python", "template", "vscode", "devcontainers"]
 license = "unlicense"
 name = "templatise"
 readme = "README.md"
 repository = "https://github.com/alunduil/template.py"
-version = "2.2.4"
+version = "2.2.5"
 
 [tool.poetry.dependencies]
 click = "^8.1.3"
 click-log = "^0.4.0"
 python = "^3.9"
 requests = "^2.28.1"
 retry = "^0.9.2"
```

### Comparing `templatise-2.2.4/templatise/actions.py` & `templatise-2.2.5/templatise/actions.py`

 * *Files identical despite different names*

### Comparing `templatise-2.2.4/templatise/configuration.py` & `templatise-2.2.5/templatise/configuration.py`

 * *Files identical despite different names*

### Comparing `templatise-2.2.4/templatise/git.py` & `templatise-2.2.5/templatise/git.py`

 * *Files identical despite different names*

### Comparing `templatise-2.2.4/templatise/initialise.py` & `templatise-2.2.5/templatise/initialise.py`

 * *Files identical despite different names*

### Comparing `templatise-2.2.4/templatise/licence.py` & `templatise-2.2.5/templatise/licence.py`

 * *Files identical despite different names*

### Comparing `templatise-2.2.4/templatise/licenses.json` & `templatise-2.2.5/templatise/licenses.json`

 * *Files identical despite different names*

### Comparing `templatise-2.2.4/templatise/project_name.py` & `templatise-2.2.5/templatise/project_name.py`

 * *Files identical despite different names*

### Comparing `templatise-2.2.4/PKG-INFO` & `templatise-2.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templatise
-Version: 2.2.4
+Version: 2.2.5
 Summary: You can use template.py to create a new GitHub repository.
 Home-page: https://github.com/alunduil/template.py
 License: Unlicense
 Keywords: python,template,vscode,devcontainers
 Author: Alex Brandt
 Author-email: alunduil@gmail.com
 Requires-Python: >=3.9,<4.0
```

