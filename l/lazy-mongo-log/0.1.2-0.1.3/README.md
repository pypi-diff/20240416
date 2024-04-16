# Comparing `tmp/lazy_mongo_log-0.1.2.tar.gz` & `tmp/lazy_mongo_log-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_mongo_log-0.1.2.tar", max compression
+gzip compressed data, was "lazy_mongo_log-0.1.3.tar", max compression
```

## Comparing `lazy_mongo_log-0.1.2.tar` & `lazy_mongo_log-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-04-05 03:06:13.339284 lazy_mongo_log-0.1.2/README.md
--rw-r--r--   0        0        0       41 2024-04-05 04:53:06.661714 lazy_mongo_log-0.1.2/lazy_mongo_log/__init__.py
--rw-r--r--   0        0        0     4455 2024-04-05 05:22:01.113043 lazy_mongo_log-0.1.2/lazy_mongo_log/lazy_mongo_log.py
--rw-r--r--   0        0        0      199 2024-04-05 03:29:29.197277 lazy_mongo_log-0.1.2/lazy_mongo_log/schemas.py
--rw-r--r--   0        0        0      323 2024-04-05 05:22:39.577990 lazy_mongo_log-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 lazy_mongo_log-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3109 2024-04-16 01:31:03.429959 lazy_mongo_log-0.1.3/README.md
+-rw-r--r--   0        0        0       41 2024-04-05 04:53:06.661714 lazy_mongo_log-0.1.3/lazy_mongo_log/__init__.py
+-rw-r--r--   0        0        0     4455 2024-04-05 05:22:01.113043 lazy_mongo_log-0.1.3/lazy_mongo_log/lazy_mongo_log.py
+-rw-r--r--   0        0        0      203 2024-04-16 07:06:33.271199 lazy_mongo_log-0.1.3/lazy_mongo_log/schemas.py
+-rw-r--r--   0        0        0      323 2024-04-16 07:08:43.370358 lazy_mongo_log-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3695 1970-01-01 00:00:00.000000 lazy_mongo_log-0.1.3/PKG-INFO
```

### Comparing `lazy_mongo_log-0.1.2/lazy_mongo_log/lazy_mongo_log.py` & `lazy_mongo_log-0.1.3/lazy_mongo_log/lazy_mongo_log.py`

 * *Files identical despite different names*

