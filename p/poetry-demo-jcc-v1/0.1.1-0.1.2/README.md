# Comparing `tmp/poetry_demo_jcc_v1-0.1.1.tar.gz` & `tmp/poetry_demo_jcc_v1-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_demo_jcc_v1-0.1.1.tar", max compression
+gzip compressed data, was "poetry_demo_jcc_v1-0.1.2.tar", max compression
```

## Comparing `poetry_demo_jcc_v1-0.1.1.tar` & `poetry_demo_jcc_v1-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       55 2024-04-11 02:04:36.447321 poetry_demo_jcc_v1-0.1.1/poetry_demo/__init__.py
--rw-r--r--   0        0        0      400 2024-04-11 01:59:58.796787 poetry_demo_jcc_v1-0.1.1/poetry_demo/poetry_demo.py
--rw-r--r--   0        0        0      557 2024-04-11 21:26:18.436143 poetry_demo_jcc_v1-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      366 2024-04-11 21:18:57.484819 poetry_demo_jcc_v1-0.1.1/README.rst
--rw-r--r--   0        0        0      753 1970-01-01 00:00:00.000000 poetry_demo_jcc_v1-0.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0      366 2024-04-11 21:18:57.484819 poetry_demo_jcc_v1-0.1.2/README.rst
+-rwxr-xr-x   0        0        0       55 2024-04-11 02:04:36.447321 poetry_demo_jcc_v1-0.1.2/poetry_demo/__init__.py
+-rwxr-xr-x   0        0        0      400 2024-04-11 01:59:58.796787 poetry_demo_jcc_v1-0.1.2/poetry_demo/poetry_demo.py
+-rwxr-xr-x   0        0        0      556 2024-04-16 19:10:23.585629 poetry_demo_jcc_v1-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      904 1970-01-01 00:00:00.000000 poetry_demo_jcc_v1-0.1.2/PKG-INFO
```

### Comparing `poetry_demo_jcc_v1-0.1.1/pyproject.toml` & `poetry_demo_jcc_v1-0.1.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "poetry-demo-jcc-v1"
-version = "0.1.1"
+version = "0.1.2"
 description = "J'son's first Poetry attempt! Just the How Long process wrapper."
 authors = ["Jason Cannelos <jasonc@esagegroup.com>"]
 readme = "README.rst"
 packages= [
     { include="poetry_demo", from="." }
 ]
 
 [tool.poetry.dependencies]
-python = "^3.12"
+python = "^3.9"
 pendulum = "^3.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^7.0.0"
 black = "^24.3.0"
 pytest = "^8.1.1"
```

