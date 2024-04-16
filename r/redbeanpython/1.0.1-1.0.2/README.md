# Comparing `tmp/redbeanpython-1.0.1.tar.gz` & `tmp/redbeanpython-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redbeanpython-1.0.1.tar", max compression
+gzip compressed data, was "redbeanpython-1.0.2.tar", max compression
```

## Comparing `redbeanpython-1.0.1.tar` & `redbeanpython-1.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1065 2024-02-01 12:27:07.435522 redbeanpython-1.0.1/LICENSE
--rw-r--r--   0        0        0    11477 2024-02-04 20:21:45.279258 redbeanpython-1.0.1/README.md
--rw-r--r--   0        0        0     2693 2024-02-04 20:22:30.741018 redbeanpython-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      508 2024-02-02 15:06:25.674315 redbeanpython-1.0.1/redbeanpython/__init__.py
--rw-r--r--   0        0        0        0 2024-01-31 23:27:15.096238 redbeanpython-1.0.1/redbeanpython/bean/__init__.py
--rw-r--r--   0        0        0     3930 2024-02-04 17:51:50.908736 redbeanpython-1.0.1/redbeanpython/bean/bean.py
--rw-r--r--   0        0        0     1527 2024-02-04 17:54:58.792441 redbeanpython-1.0.1/redbeanpython/bean/beans.py
--rw-r--r--   0        0        0      372 2024-02-04 17:49:35.755057 redbeanpython-1.0.1/redbeanpython/bean/id.py
--rw-r--r--   0        0        0     1625 2024-02-02 15:21:32.708590 redbeanpython-1.0.1/redbeanpython/bean/validator.py
--rw-r--r--   0        0        0        0 2024-01-31 23:40:52.736122 redbeanpython-1.0.1/redbeanpython/cli/__init__.py
--rw-r--r--   0        0        0     3507 2024-02-04 13:09:50.643846 redbeanpython-1.0.1/redbeanpython/cli/cli.py
--rw-r--r--   0        0        0     2660 2024-02-04 17:15:14.462475 redbeanpython-1.0.1/redbeanpython/config.py
--rw-r--r--   0        0        0      656 2024-02-04 13:51:25.154745 redbeanpython-1.0.1/redbeanpython/const.py
--rw-r--r--   0        0        0      428 2024-01-31 23:49:26.767509 redbeanpython-1.0.1/redbeanpython/errors.py
--rw-r--r--   0        0        0    15788 2024-02-04 20:04:37.341392 redbeanpython-1.0.1/redbeanpython/facade.py
--rw-r--r--   0        0        0        0 2024-01-31 23:51:19.887722 redbeanpython-1.0.1/redbeanpython/model/__init__.py
--rw-r--r--   0        0        0      113 2024-02-02 15:18:16.549252 redbeanpython-1.0.1/redbeanpython/model/model.py
--rw-r--r--   0        0        0     1623 2024-02-04 17:07:31.886737 redbeanpython-1.0.1/redbeanpython/model/models_creator.py
--rw-r--r--   0        0        0        0 2024-01-19 19:33:07.069304 redbeanpython-1.0.1/redbeanpython/py.typed
--rw-r--r--   0        0        0    17055 2024-02-04 18:20:35.597555 redbeanpython-1.0.1/redbeanpython/redbean.py
--rw-r--r--   0        0        0        0 2024-01-31 23:27:15.096238 redbeanpython-1.0.1/redbeanpython/structure/__init__.py
--rw-r--r--   0        0        0      834 2024-02-04 17:35:46.746510 redbeanpython-1.0.1/redbeanpython/structure/column_type.py
--rw-r--r--   0        0        0     6323 2024-02-04 20:15:27.436456 redbeanpython-1.0.1/redbeanpython/structure/db_structure.py
--rw-r--r--   0        0        0     2119 2024-02-03 20:59:17.301717 redbeanpython-1.0.1/redbeanpython/structure/supported_types.py
--rw-r--r--   0        0        0     2308 2024-02-04 20:15:27.436456 redbeanpython-1.0.1/redbeanpython/structure/table.py
--rw-r--r--   0        0        0      881 2024-02-03 20:59:17.305717 redbeanpython-1.0.1/redbeanpython/structure/type.py
--rw-r--r--   0        0        0      966 2024-01-29 09:40:02.208631 redbeanpython-1.0.1/redbeanpython/templates/alembic.ini.mako
--rw-r--r--   0        0        0     1445 2024-01-31 23:51:22.943835 redbeanpython-1.0.1/redbeanpython/templates/env.py.template
--rw-r--r--   0        0        0     1540 2024-02-01 00:05:56.380476 redbeanpython-1.0.1/redbeanpython/templates/env.sqlite.py.template
--rw-r--r--   0        0        0      826 2024-02-03 19:55:06.295240 redbeanpython-1.0.1/redbeanpython/templates/model.py.mako
--rw-r--r--   0        0        0      749 2024-01-31 23:11:18.764581 redbeanpython-1.0.1/redbeanpython/templates/script.py.mako.template
--rw-r--r--   0        0        0    12418 1970-01-01 00:00:00.000000 redbeanpython-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-02-01 12:27:07.435522 redbeanpython-1.0.2/LICENSE
+-rw-r--r--   0        0        0    11477 2024-04-16 20:49:38.246707 redbeanpython-1.0.2/README.md
+-rw-r--r--   0        0        0     2695 2024-04-16 20:58:10.847079 redbeanpython-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      508 2024-02-02 15:06:25.674315 redbeanpython-1.0.2/redbeanpython/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-31 23:27:15.096238 redbeanpython-1.0.2/redbeanpython/bean/__init__.py
+-rw-r--r--   0        0        0     3930 2024-02-04 17:51:50.908736 redbeanpython-1.0.2/redbeanpython/bean/bean.py
+-rw-r--r--   0        0        0     1527 2024-02-04 17:54:58.792441 redbeanpython-1.0.2/redbeanpython/bean/beans.py
+-rw-r--r--   0        0        0      372 2024-02-04 17:49:35.755057 redbeanpython-1.0.2/redbeanpython/bean/id.py
+-rw-r--r--   0        0        0     1625 2024-02-02 15:21:32.708590 redbeanpython-1.0.2/redbeanpython/bean/validator.py
+-rw-r--r--   0        0        0        0 2024-01-31 23:40:52.736122 redbeanpython-1.0.2/redbeanpython/cli/__init__.py
+-rw-r--r--   0        0        0     3507 2024-02-04 13:09:50.643846 redbeanpython-1.0.2/redbeanpython/cli/cli.py
+-rw-r--r--   0        0        0     2660 2024-04-16 20:48:43.140448 redbeanpython-1.0.2/redbeanpython/config.py
+-rw-r--r--   0        0        0      656 2024-04-16 20:48:43.140448 redbeanpython-1.0.2/redbeanpython/const.py
+-rw-r--r--   0        0        0      428 2024-01-31 23:49:26.767509 redbeanpython-1.0.2/redbeanpython/errors.py
+-rw-r--r--   0        0        0    15788 2024-04-16 20:48:43.140448 redbeanpython-1.0.2/redbeanpython/facade.py
+-rw-r--r--   0        0        0        0 2024-01-31 23:51:19.887722 redbeanpython-1.0.2/redbeanpython/model/__init__.py
+-rw-r--r--   0        0        0      113 2024-02-02 15:18:16.549252 redbeanpython-1.0.2/redbeanpython/model/model.py
+-rw-r--r--   0        0        0     1623 2024-02-04 17:07:31.886737 redbeanpython-1.0.2/redbeanpython/model/models_creator.py
+-rw-r--r--   0        0        0        0 2024-01-19 19:33:07.069304 redbeanpython-1.0.2/redbeanpython/py.typed
+-rw-r--r--   0        0        0    17055 2024-02-04 18:20:35.597555 redbeanpython-1.0.2/redbeanpython/redbean.py
+-rw-r--r--   0        0        0        0 2024-01-31 23:27:15.096238 redbeanpython-1.0.2/redbeanpython/structure/__init__.py
+-rw-r--r--   0        0        0      834 2024-02-04 17:35:46.746510 redbeanpython-1.0.2/redbeanpython/structure/column_type.py
+-rw-r--r--   0        0        0     6323 2024-04-16 20:48:43.140448 redbeanpython-1.0.2/redbeanpython/structure/db_structure.py
+-rw-r--r--   0        0        0     2119 2024-02-03 20:59:17.301717 redbeanpython-1.0.2/redbeanpython/structure/supported_types.py
+-rw-r--r--   0        0        0     2308 2024-02-04 20:15:27.436456 redbeanpython-1.0.2/redbeanpython/structure/table.py
+-rw-r--r--   0        0        0      881 2024-02-03 20:59:17.305717 redbeanpython-1.0.2/redbeanpython/structure/type.py
+-rw-r--r--   0        0        0      966 2024-01-29 09:40:02.208631 redbeanpython-1.0.2/redbeanpython/templates/alembic.ini.mako
+-rw-r--r--   0        0        0     1445 2024-01-31 23:51:22.943835 redbeanpython-1.0.2/redbeanpython/templates/env.py.template
+-rw-r--r--   0        0        0     1540 2024-02-01 00:05:56.380476 redbeanpython-1.0.2/redbeanpython/templates/env.sqlite.py.template
+-rw-r--r--   0        0        0      826 2024-02-03 19:55:06.295240 redbeanpython-1.0.2/redbeanpython/templates/model.py.mako
+-rw-r--r--   0        0        0      749 2024-01-31 23:11:18.764581 redbeanpython-1.0.2/redbeanpython/templates/script.py.mako.template
+-rw-r--r--   0        0        0    12418 1970-01-01 00:00:00.000000 redbeanpython-1.0.2/PKG-INFO
```

### Comparing `redbeanpython-1.0.1/LICENSE` & `redbeanpython-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `redbeanpython-1.0.1/README.md` & `redbeanpython-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 - alembic 1.7 or newer.
 
 
 ## Database requirements
 
 For **PostgreSQL** support RedBeanPython requires:
 
-- psycopg2 2.9.9 or newer.
+- psycopg 3.0.18 or newer.
 
 For **MySQL/MariaDB** support RedBeanPython requires:
 
 - PyMySQL 1.0.2 or newer.
 
 
 # How it works? Let's see an example of a usual project lifecycle.
```

### Comparing `redbeanpython-1.0.1/pyproject.toml` & `redbeanpython-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "redbeanpython"
-version = "1.0.1"
+version = "1.0.2"
 description = "RedBeanPython ORM"
 authors = ["Adam Puza <adampuza@redbeanpython.org>"]
 readme = "README.md"
 license = "MIT"
 packages = [
     { include = "redbeanpython" },
 ]
@@ -34,15 +34,15 @@
 
 [tool.poetry.dependencies]
 python = ">= 3.11"
 SQLAlchemy = ">= 2.0.0"
 alembic = ">= 1.8.0"
 
 [tool.poetry.group.postgres.dependencies]
-psycopg2 = "^2.9.9"
+psycopg = ">= 3.0.18"
 
 [tool.poetry.group.mysql.dependencies]
 PyMySQL = ">= 1.0.2"
 
 [tool.poetry.group.dev.dependencies]
 poethepoet = "^0.24.4"
 black = "^24.1.1"
```

### Comparing `redbeanpython-1.0.1/redbeanpython/bean/bean.py` & `redbeanpython-1.0.2/redbeanpython/bean/bean.py`

 * *Files identical despite different names*

### Comparing `redbeanpython-1.0.1/redbeanpython/bean/beans.py` & `redbeanpython-1.0.2/redbeanpython/bean/beans.py`

 * *Files identical despite different names*

### Comparing `redbeanpython-1.0.1/redbeanpython/bean/validator.py` & `redbeanpython-1.0.2/redbeanpython/bean/validator.py`

 * *Files identical despite different names*

### Comparing `redbeanpython-1.0.1/redbeanpython/cli/cli.py` & `redbeanpython-1.0.2/redbeanpython/cli/cli.py`

 * *Files identical despite different names*

### Comparing `redbeanpython-1.0.1/redbeanpython/config.py` & `redbeanpython-1.0.2/redbeanpython/config.py`

 * *Files identical despite different names*

### Comparing `redbeanpython-1.0.1/redbeanpython/const.py` & `redbeanpython-1.0.2/redbeanpython/const.py`

 * *Files identical despite different names*

### Comparing `redbeanpython-1.0.1/redbeanpython/facade.py` & `redbeanpython-1.0.2/redbeanpython/facade.py`

 * *Files identical despite different names*

### Comparing `redbeanpython-1.0.1/redbeanpython/model/models_creator.py` & `redbeanpython-1.0.2/redbeanpython/model/models_creator.py`

 * *Files identical despite different names*

### Comparing `redbeanpython-1.0.1/redbeanpython/redbean.py` & `redbeanpython-1.0.2/redbeanpython/redbean.py`

 * *Files identical despite different names*

### Comparing `redbeanpython-1.0.1/redbeanpython/structure/column_type.py` & `redbeanpython-1.0.2/redbeanpython/structure/column_type.py`

 * *Files identical despite different names*

### Comparing `redbeanpython-1.0.1/redbeanpython/structure/db_structure.py` & `redbeanpython-1.0.2/redbeanpython/structure/db_structure.py`

 * *Files identical despite different names*

### Comparing `redbeanpython-1.0.1/redbeanpython/structure/supported_types.py` & `redbeanpython-1.0.2/redbeanpython/structure/supported_types.py`

 * *Files identical despite different names*

### Comparing `redbeanpython-1.0.1/redbeanpython/structure/table.py` & `redbeanpython-1.0.2/redbeanpython/structure/table.py`

 * *Files identical despite different names*

### Comparing `redbeanpython-1.0.1/redbeanpython/structure/type.py` & `redbeanpython-1.0.2/redbeanpython/structure/type.py`

 * *Files identical despite different names*

### Comparing `redbeanpython-1.0.1/redbeanpython/templates/alembic.ini.mako` & `redbeanpython-1.0.2/redbeanpython/templates/alembic.ini.mako`

 * *Files identical despite different names*

### Comparing `redbeanpython-1.0.1/redbeanpython/templates/env.py.template` & `redbeanpython-1.0.2/redbeanpython/templates/env.py.template`

 * *Files identical despite different names*

### Comparing `redbeanpython-1.0.1/redbeanpython/templates/env.sqlite.py.template` & `redbeanpython-1.0.2/redbeanpython/templates/env.sqlite.py.template`

 * *Files identical despite different names*

### Comparing `redbeanpython-1.0.1/redbeanpython/templates/model.py.mako` & `redbeanpython-1.0.2/redbeanpython/templates/model.py.mako`

 * *Files identical despite different names*

### Comparing `redbeanpython-1.0.1/redbeanpython/templates/script.py.mako.template` & `redbeanpython-1.0.2/redbeanpython/templates/script.py.mako.template`

 * *Files identical despite different names*

### Comparing `redbeanpython-1.0.1/PKG-INFO` & `redbeanpython-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redbeanpython
-Version: 1.0.1
+Version: 1.0.2
 Summary: RedBeanPython ORM
 License: MIT
 Author: Adam Puza
 Author-email: adampuza@redbeanpython.org
 Requires-Python: >=3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -65,15 +65,15 @@
 - alembic 1.7 or newer.
 
 
 ## Database requirements
 
 For **PostgreSQL** support RedBeanPython requires:
 
-- psycopg2 2.9.9 or newer.
+- psycopg 3.0.18 or newer.
 
 For **MySQL/MariaDB** support RedBeanPython requires:
 
 - PyMySQL 1.0.2 or newer.
 
 
 # How it works? Let's see an example of a usual project lifecycle.
```

