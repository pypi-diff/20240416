# Comparing `tmp/imas_tools-0.1.3.tar.gz` & `tmp/imas_tools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imas_tools-0.1.3.tar", max compression
+gzip compressed data, was "imas_tools-0.2.0.tar", max compression
```

## Comparing `imas_tools-0.1.3.tar` & `imas_tools-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,8 @@
--rw-r--r--   0        0        0        0 2024-04-13 09:02:36.035606 imas_tools-0.1.3/imas_tools/__init__.py
--rw-r--r--   0        0        0     4126 2024-04-13 12:27:59.670781 imas_tools-0.1.3/imas_tools/recochoku.py
--rw-r--r--   0        0        0      416 2024-04-13 12:24:36.397548 imas_tools-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-13 09:02:36.044152 imas_tools-0.1.3/README.md
--rw-r--r--   0        0        0      598 1970-01-01 00:00:00.000000 imas_tools-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-13 09:02:36.035606 imas_tools-0.2.0/imas_tools/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 13:36:34.820658 imas_tools-0.2.0/imas_tools/portal/__init__.py
+-rw-r--r--   0        0        0     4499 2024-04-16 16:33:35.339011 imas_tools-0.2.0/imas_tools/portal/calendar.py
+-rw-r--r--   0        0        0     1787 2024-04-16 16:32:38.339304 imas_tools-0.2.0/imas_tools/portal/interfaces.py
+-rw-r--r--   0        0        0     4126 2024-04-13 12:27:59.670781 imas_tools-0.2.0/imas_tools/recochoku.py
+-rw-r--r--   0        0        0      465 2024-04-16 16:46:12.955123 imas_tools-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-13 09:02:36.044152 imas_tools-0.2.0/README.md
+-rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 imas_tools-0.2.0/PKG-INFO
```

### Comparing `imas_tools-0.1.3/imas_tools/recochoku.py` & `imas_tools-0.2.0/imas_tools/recochoku.py`

 * *Files identical despite different names*

### Comparing `imas_tools-0.1.3/PKG-INFO` & `imas_tools-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: imas-tools
-Version: 0.1.3
+Version: 0.2.0
 Summary: 
 Author: darwintree
 Author-email: 17946284+darwintree@users.noreply.github.com
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
+Requires-Dist: pytz (>=2024.1,<2025.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: typing-extensions (>=4.11.0,<5.0.0)
 Description-Content-Type: text/markdown
```

