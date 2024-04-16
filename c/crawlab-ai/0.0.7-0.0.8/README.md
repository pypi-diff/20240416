# Comparing `tmp/crawlab-ai-0.0.7.tar.gz` & `tmp/crawlab-ai-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlab-ai-0.0.7.tar", last modified: Tue Apr 16 13:58:25 2024, max compression
+gzip compressed data, was "crawlab-ai-0.0.8.tar", last modified: Tue Apr 16 13:59:00 2024, max compression
```

## Comparing `crawlab-ai-0.0.7.tar` & `crawlab-ai-0.0.8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:58:25.002229 crawlab-ai-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-16 13:58:05.000000 crawlab-ai-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-16 13:58:25.002229 crawlab-ai-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-16 13:58:05.000000 crawlab-ai-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:58:24.994229 crawlab-ai-0.0.7/crawlab_ai/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-16 13:58:05.000000 crawlab-ai-0.0.7/crawlab_ai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:58:24.998229 crawlab-ai-0.0.7/crawlab_ai/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-16 13:58:05.000000 crawlab-ai-0.0.7/crawlab_ai/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-16 13:58:05.000000 crawlab-ai-0.0.7/crawlab_ai/cli/codegen.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-16 13:58:05.000000 crawlab-ai-0.0.7/crawlab_ai/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-16 13:58:05.000000 crawlab-ai-0.0.7/crawlab_ai/cli/crawl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:58:24.998229 crawlab-ai-0.0.7/crawlab_ai/code/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:58:05.000000 crawlab-ai-0.0.7/crawlab_ai/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-16 13:58:05.000000 crawlab-ai-0.0.7/crawlab_ai/code/article.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-16 13:58:05.000000 crawlab-ai-0.0.7/crawlab_ai/code/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:58:24.998229 crawlab-ai-0.0.7/crawlab_ai/scrapy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:58:05.000000 crawlab-ai-0.0.7/crawlab_ai/scrapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-16 13:58:05.000000 crawlab-ai-0.0.7/crawlab_ai/scrapy/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-04-16 13:58:05.000000 crawlab-ai-0.0.7/crawlab_ai/scrapy/list_spider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:58:24.998229 crawlab-ai-0.0.7/crawlab_ai/spider/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:58:05.000000 crawlab-ai-0.0.7/crawlab_ai/spider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-04-16 13:58:05.000000 crawlab-ai-0.0.7/crawlab_ai/spider/article_spider.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-16 13:58:05.000000 crawlab-ai-0.0.7/crawlab_ai/spider/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6314 2024-04-16 13:58:05.000000 crawlab-ai-0.0.7/crawlab_ai/spider/list_spider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:58:24.998229 crawlab-ai-0.0.7/crawlab_ai/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:58:05.000000 crawlab-ai-0.0.7/crawlab_ai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-16 13:58:05.000000 crawlab-ai-0.0.7/crawlab_ai/utils/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-16 13:58:05.000000 crawlab-ai-0.0.7/crawlab_ai/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-16 13:58:05.000000 crawlab-ai-0.0.7/crawlab_ai/utils/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:58:24.998229 crawlab-ai-0.0.7/crawlab_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-16 13:58:24.000000 crawlab-ai-0.0.7/crawlab_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-16 13:58:24.000000 crawlab-ai-0.0.7/crawlab_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 13:58:24.000000 crawlab-ai-0.0.7/crawlab_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-16 13:58:24.000000 crawlab-ai-0.0.7/crawlab_ai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-16 13:58:24.000000 crawlab-ai-0.0.7/crawlab_ai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 13:58:25.002229 crawlab-ai-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-16 13:58:05.000000 crawlab-ai-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:58:24.998229 crawlab-ai-0.0.7/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:58:05.000000 crawlab-ai-0.0.7/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:58:25.002229 crawlab-ai-0.0.7/test/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:58:05.000000 crawlab-ai-0.0.7/test/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-16 13:58:05.000000 crawlab-ai-0.0.7/test/utils/test_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:59:00.107435 crawlab-ai-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-16 13:58:37.000000 crawlab-ai-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-16 13:59:00.107435 crawlab-ai-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-16 13:58:37.000000 crawlab-ai-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:59:00.103435 crawlab-ai-0.0.8/crawlab_ai/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-16 13:58:37.000000 crawlab-ai-0.0.8/crawlab_ai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:59:00.107435 crawlab-ai-0.0.8/crawlab_ai/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-16 13:58:37.000000 crawlab-ai-0.0.8/crawlab_ai/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-16 13:58:37.000000 crawlab-ai-0.0.8/crawlab_ai/cli/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-16 13:58:37.000000 crawlab-ai-0.0.8/crawlab_ai/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-16 13:58:37.000000 crawlab-ai-0.0.8/crawlab_ai/cli/crawl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:59:00.107435 crawlab-ai-0.0.8/crawlab_ai/code/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:58:37.000000 crawlab-ai-0.0.8/crawlab_ai/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-16 13:58:37.000000 crawlab-ai-0.0.8/crawlab_ai/code/article.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-16 13:58:37.000000 crawlab-ai-0.0.8/crawlab_ai/code/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:59:00.107435 crawlab-ai-0.0.8/crawlab_ai/scrapy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:58:37.000000 crawlab-ai-0.0.8/crawlab_ai/scrapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-16 13:58:37.000000 crawlab-ai-0.0.8/crawlab_ai/scrapy/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-04-16 13:58:37.000000 crawlab-ai-0.0.8/crawlab_ai/scrapy/list_spider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:59:00.107435 crawlab-ai-0.0.8/crawlab_ai/spider/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:58:37.000000 crawlab-ai-0.0.8/crawlab_ai/spider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-04-16 13:58:37.000000 crawlab-ai-0.0.8/crawlab_ai/spider/article_spider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-16 13:58:37.000000 crawlab-ai-0.0.8/crawlab_ai/spider/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6314 2024-04-16 13:58:37.000000 crawlab-ai-0.0.8/crawlab_ai/spider/list_spider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:59:00.107435 crawlab-ai-0.0.8/crawlab_ai/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:58:37.000000 crawlab-ai-0.0.8/crawlab_ai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-16 13:58:37.000000 crawlab-ai-0.0.8/crawlab_ai/utils/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-16 13:58:37.000000 crawlab-ai-0.0.8/crawlab_ai/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-16 13:58:37.000000 crawlab-ai-0.0.8/crawlab_ai/utils/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:59:00.103435 crawlab-ai-0.0.8/crawlab_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-16 13:59:00.000000 crawlab-ai-0.0.8/crawlab_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-16 13:59:00.000000 crawlab-ai-0.0.8/crawlab_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 13:59:00.000000 crawlab-ai-0.0.8/crawlab_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-16 13:59:00.000000 crawlab-ai-0.0.8/crawlab_ai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-16 13:59:00.000000 crawlab-ai-0.0.8/crawlab_ai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 13:59:00.107435 crawlab-ai-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-16 13:58:37.000000 crawlab-ai-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:59:00.107435 crawlab-ai-0.0.8/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:58:37.000000 crawlab-ai-0.0.8/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:59:00.107435 crawlab-ai-0.0.8/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:58:37.000000 crawlab-ai-0.0.8/test/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-16 13:58:37.000000 crawlab-ai-0.0.8/test/utils/test_auth.py
```

### Comparing `crawlab-ai-0.0.7/LICENSE` & `crawlab-ai-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `crawlab-ai-0.0.7/README.md` & `crawlab-ai-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `crawlab-ai-0.0.7/crawlab_ai/cli/__init__.py` & `crawlab-ai-0.0.8/crawlab_ai/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `crawlab-ai-0.0.7/crawlab_ai/cli/codegen.py` & `crawlab-ai-0.0.8/crawlab_ai/cli/codegen.py`

 * *Files identical despite different names*

### Comparing `crawlab-ai-0.0.7/crawlab_ai/cli/config.py` & `crawlab-ai-0.0.8/crawlab_ai/cli/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,9 +11,9 @@
     config_parser.set_defaults(func=config)
 
 
 def config(args):
     if args.token:
         set_token(args.token)
 
-    if args.url:
-        set_api_endpoint(args.url)
+    # if args.url:
+    #     set_api_endpoint(args.url)
```

### Comparing `crawlab-ai-0.0.7/crawlab_ai/cli/crawl.py` & `crawlab-ai-0.0.8/crawlab_ai/cli/crawl.py`

 * *Files identical despite different names*

### Comparing `crawlab-ai-0.0.7/crawlab_ai/code/article.py` & `crawlab-ai-0.0.8/crawlab_ai/code/article.py`

 * *Files identical despite different names*

### Comparing `crawlab-ai-0.0.7/crawlab_ai/code/list.py` & `crawlab-ai-0.0.8/crawlab_ai/code/list.py`

 * *Files identical despite different names*

### Comparing `crawlab-ai-0.0.7/crawlab_ai/scrapy/list_spider.py` & `crawlab-ai-0.0.8/crawlab_ai/scrapy/list_spider.py`

 * *Files identical despite different names*

### Comparing `crawlab-ai-0.0.7/crawlab_ai/spider/article_spider.py` & `crawlab-ai-0.0.8/crawlab_ai/spider/article_spider.py`

 * *Files identical despite different names*

### Comparing `crawlab-ai-0.0.7/crawlab_ai/spider/list_spider.py` & `crawlab-ai-0.0.8/crawlab_ai/spider/list_spider.py`

 * *Files identical despite different names*

### Comparing `crawlab-ai-0.0.7/crawlab_ai/utils/auth.py` & `crawlab-ai-0.0.8/crawlab_ai/utils/auth.py`

 * *Files identical despite different names*

### Comparing `crawlab-ai-0.0.7/crawlab_ai/utils/env.py` & `crawlab-ai-0.0.8/crawlab_ai/utils/env.py`

 * *Files identical despite different names*

### Comparing `crawlab-ai-0.0.7/crawlab_ai.egg-info/SOURCES.txt` & `crawlab-ai-0.0.8/crawlab_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crawlab-ai-0.0.7/test/utils/test_auth.py` & `crawlab-ai-0.0.8/test/utils/test_auth.py`

 * *Files identical despite different names*

