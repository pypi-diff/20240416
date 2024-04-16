# Comparing `tmp/mcqq_tool-1.1.7.tar.gz` & `tmp/mcqq_tool-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcqq_tool-1.1.7.tar", max compression
+gzip compressed data, was "mcqq_tool-1.1.8.tar", max compression
```

## Comparing `mcqq_tool-1.1.7.tar` & `mcqq_tool-1.1.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1065 2024-03-28 14:47:17.191008 mcqq_tool-1.1.7/LICENSE
--rw-r--r--   0        0        0       79 2024-03-28 14:47:17.191008 mcqq_tool-1.1.7/README.md
--rw-r--r--   0        0        0       19 2024-03-28 14:47:17.191008 mcqq_tool-1.1.7/mcqq_tool/__init__.py
--rw-r--r--   0        0        0     2116 2024-03-28 14:47:17.191008 mcqq_tool-1.1.7/mcqq_tool/config.py
--rw-r--r--   0        0        0      266 2024-03-28 14:47:17.191008 mcqq_tool-1.1.7/mcqq_tool/model.py
--rw-r--r--   0        0        0    14787 2024-03-28 14:47:17.191008 mcqq_tool-1.1.7/mcqq_tool/parse_qq_msg.py
--rw-r--r--   0        0        0     4915 2024-03-28 14:47:17.191008 mcqq_tool-1.1.7/mcqq_tool/rule.py
--rw-r--r--   0        0        0    10587 2024-03-28 14:47:17.191008 mcqq_tool-1.1.7/mcqq_tool/send_to_mc.py
--rw-r--r--   0        0        0     2243 2024-03-28 14:47:17.191008 mcqq_tool-1.1.7/mcqq_tool/send_to_qq.py
--rw-r--r--   0        0        0      523 2024-03-28 14:47:17.191008 mcqq_tool-1.1.7/pyproject.toml
--rw-r--r--   0        0        0      869 1970-01-01 00:00:00.000000 mcqq_tool-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-16 04:17:59.359463 mcqq_tool-1.1.8/LICENSE
+-rw-r--r--   0        0        0       79 2024-04-16 04:17:59.359463 mcqq_tool-1.1.8/README.md
+-rw-r--r--   0        0        0       19 2024-04-16 04:17:59.359463 mcqq_tool-1.1.8/mcqq_tool/__init__.py
+-rw-r--r--   0        0        0     2116 2024-04-16 04:17:59.359463 mcqq_tool-1.1.8/mcqq_tool/config.py
+-rw-r--r--   0        0        0      266 2024-04-16 04:17:59.359463 mcqq_tool-1.1.8/mcqq_tool/model.py
+-rw-r--r--   0        0        0    14787 2024-04-16 04:17:59.359463 mcqq_tool-1.1.8/mcqq_tool/parse_qq_msg.py
+-rw-r--r--   0        0        0     4915 2024-04-16 04:17:59.359463 mcqq_tool-1.1.8/mcqq_tool/rule.py
+-rw-r--r--   0        0        0    10587 2024-04-16 04:17:59.359463 mcqq_tool-1.1.8/mcqq_tool/send_to_mc.py
+-rw-r--r--   0        0        0     2243 2024-04-16 04:17:59.359463 mcqq_tool-1.1.8/mcqq_tool/send_to_qq.py
+-rw-r--r--   0        0        0      516 2024-04-16 04:17:59.359463 mcqq_tool-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0      863 1970-01-01 00:00:00.000000 mcqq_tool-1.1.8/PKG-INFO
```

### Comparing `mcqq_tool-1.1.7/LICENSE` & `mcqq_tool-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mcqq_tool-1.1.7/mcqq_tool/config.py` & `mcqq_tool-1.1.8/mcqq_tool/config.py`

 * *Files identical despite different names*

### Comparing `mcqq_tool-1.1.7/mcqq_tool/parse_qq_msg.py` & `mcqq_tool-1.1.8/mcqq_tool/parse_qq_msg.py`

 * *Files identical despite different names*

### Comparing `mcqq_tool-1.1.7/mcqq_tool/rule.py` & `mcqq_tool-1.1.8/mcqq_tool/rule.py`

 * *Files identical despite different names*

### Comparing `mcqq_tool-1.1.7/mcqq_tool/send_to_mc.py` & `mcqq_tool-1.1.8/mcqq_tool/send_to_mc.py`

 * *Files identical despite different names*

### Comparing `mcqq_tool-1.1.7/mcqq_tool/send_to_qq.py` & `mcqq_tool-1.1.8/mcqq_tool/send_to_qq.py`

 * *Files identical despite different names*

### Comparing `mcqq_tool-1.1.7/pyproject.toml` & `mcqq_tool-1.1.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "mcqq-tool"
-version = "1.1.7"
+version = "1.1.8"
 description = "MC_QQ工具包"
 authors = ["17TheWord <17theword@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 nonebot2 = "^2.2.1"
 nonebot-adapter-qq = "^1.4.2"
 nonebot-adapter-onebot = "^2.4.1"
-nonebot-adapter-minecraft = "~=1.0.8.post3"
+nonebot-adapter-minecraft = "^1.1.2"
 nonebot-plugin-guild-patch-remix = "^0.2.4"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 
 [build-system]
```

### Comparing `mcqq_tool-1.1.7/PKG-INFO` & `mcqq_tool-1.1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: mcqq-tool
-Version: 1.1.7
+Version: 1.1.8
 Summary: MC_QQ工具包
 License: MIT
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: nonebot-adapter-minecraft (>=1.0.8.post3,<1.1.0)
+Requires-Dist: nonebot-adapter-minecraft (>=1.1.2,<2.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.4.1,<3.0.0)
 Requires-Dist: nonebot-adapter-qq (>=1.4.2,<2.0.0)
 Requires-Dist: nonebot-plugin-guild-patch-remix (>=0.2.4,<0.3.0)
 Requires-Dist: nonebot2 (>=2.2.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # MC_QQ_Tool
```

