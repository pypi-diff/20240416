# Comparing `tmp/wikidot-3.0.1.tar.gz` & `tmp/wikidot-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikidot-3.0.1.tar", last modified: Mon Apr 15 08:08:01 2024, max compression
+gzip compressed data, was "wikidot-3.0.2.tar", last modified: Tue Apr 16 06:45:24 2024, max compression
```

## Comparing `wikidot-3.0.1.tar` & `wikidot-3.0.2.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-15 08:08:01.400372 wikidot-3.0.1/
--rw-r--r--   0 ukwhatn    (501) staff       (20)     1070 2024-04-11 05:41:21.000000 wikidot-3.0.1/LICENSE
--rw-r--r--   0 ukwhatn    (501) staff       (20)     3121 2024-04-15 08:08:01.400184 wikidot-3.0.1/PKG-INFO
--rw-r--r--   0 ukwhatn    (501) staff       (20)     2339 2024-04-15 07:24:27.000000 wikidot-3.0.1/README.md
--rw-r--r--   0 ukwhatn    (501) staff       (20)      732 2024-04-15 08:07:05.000000 wikidot-3.0.1/pyproject.toml
--rw-r--r--   0 ukwhatn    (501) staff       (20)       38 2024-04-15 08:08:01.400410 wikidot-3.0.1/setup.cfg
-drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-15 08:08:01.393803 wikidot-3.0.1/wikidot/
--rw-r--r--   0 ukwhatn    (501) staff       (20)       34 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/__init__.py
-drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-15 08:08:01.395635 wikidot-3.0.1/wikidot/common/
--rw-r--r--   0 ukwhatn    (501) staff       (20)       40 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/common/__init__.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)      998 2024-04-15 07:24:27.000000 wikidot-3.0.1/wikidot/common/decorators.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     2517 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/common/exceptions.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)      450 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/common/logger.py
-drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-15 08:08:01.396209 wikidot-3.0.1/wikidot/connector/
--rw-r--r--   0 ukwhatn    (501) staff       (20)        0 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/connector/__init__.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)    10788 2024-04-15 07:24:27.000000 wikidot-3.0.1/wikidot/connector/ajax.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)      261 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/connector/api.py
-drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-15 08:08:01.398148 wikidot-3.0.1/wikidot/module/
--rw-r--r--   0 ukwhatn    (501) staff       (20)        0 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/module/__init__.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     2091 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/module/auth.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     6407 2024-04-15 07:24:27.000000 wikidot-3.0.1/wikidot/module/client.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)    11798 2024-04-15 07:45:35.000000 wikidot-3.0.1/wikidot/module/page.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)      194 2024-04-15 07:34:32.000000 wikidot-3.0.1/wikidot/module/page_source.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     8521 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/module/private_message.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     6742 2024-04-15 07:24:27.000000 wikidot-3.0.1/wikidot/module/site.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     3053 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/module/site_application.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     7728 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/module/user.py
-drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-15 08:08:01.398804 wikidot-3.0.1/wikidot/util/
--rw-r--r--   0 ukwhatn    (501) staff       (20)        0 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/util/__init__.py
-drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-15 08:08:01.399245 wikidot-3.0.1/wikidot/util/parser/
--rw-r--r--   0 ukwhatn    (501) staff       (20)       77 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/util/parser/__init__.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)      752 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/util/parser/odate.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     2038 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/util/parser/user.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     2635 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/util/quick_module.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     1869 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/util/requestutil.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     1477 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/util/stringutil.py
-drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-15 08:08:01.399499 wikidot-3.0.1/wikidot/util/table/
--rw-r--r--   0 ukwhatn    (501) staff       (20)        0 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/util/table/__init__.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     7128 2024-04-11 05:41:21.000000 wikidot-3.0.1/wikidot/util/table/char_table.py
-drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-15 08:08:01.399803 wikidot-3.0.1/wikidot.egg-info/
--rw-r--r--   0 ukwhatn    (501) staff       (20)     3121 2024-04-15 08:08:01.000000 wikidot-3.0.1/wikidot.egg-info/PKG-INFO
--rw-r--r--   0 ukwhatn    (501) staff       (20)      902 2024-04-15 08:08:01.000000 wikidot-3.0.1/wikidot.egg-info/SOURCES.txt
--rw-r--r--   0 ukwhatn    (501) staff       (20)        1 2024-04-15 08:08:01.000000 wikidot-3.0.1/wikidot.egg-info/dependency_links.txt
--rw-r--r--   0 ukwhatn    (501) staff       (20)       68 2024-04-15 08:08:01.000000 wikidot-3.0.1/wikidot.egg-info/requires.txt
--rw-r--r--   0 ukwhatn    (501) staff       (20)        8 2024-04-15 08:08:01.000000 wikidot-3.0.1/wikidot.egg-info/top_level.txt
+drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-16 06:45:24.984228 wikidot-3.0.2/
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     1070 2024-04-11 05:41:21.000000 wikidot-3.0.2/LICENSE
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     3121 2024-04-16 06:45:24.984022 wikidot-3.0.2/PKG-INFO
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     2339 2024-04-15 07:24:27.000000 wikidot-3.0.2/README.md
+-rw-r--r--   0 ukwhatn    (501) staff       (20)      732 2024-04-16 06:43:38.000000 wikidot-3.0.2/pyproject.toml
+-rw-r--r--   0 ukwhatn    (501) staff       (20)       38 2024-04-16 06:45:24.984273 wikidot-3.0.2/setup.cfg
+drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-16 06:45:24.976945 wikidot-3.0.2/wikidot/
+-rw-r--r--   0 ukwhatn    (501) staff       (20)       34 2024-04-11 05:41:21.000000 wikidot-3.0.2/wikidot/__init__.py
+drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-16 06:45:24.978947 wikidot-3.0.2/wikidot/common/
+-rw-r--r--   0 ukwhatn    (501) staff       (20)       40 2024-04-11 05:41:21.000000 wikidot-3.0.2/wikidot/common/__init__.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)      998 2024-04-15 07:24:27.000000 wikidot-3.0.2/wikidot/common/decorators.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     2517 2024-04-11 05:41:21.000000 wikidot-3.0.2/wikidot/common/exceptions.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)      450 2024-04-11 05:41:21.000000 wikidot-3.0.2/wikidot/common/logger.py
+drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-16 06:45:24.979544 wikidot-3.0.2/wikidot/connector/
+-rw-r--r--   0 ukwhatn    (501) staff       (20)        0 2024-04-11 05:41:21.000000 wikidot-3.0.2/wikidot/connector/__init__.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)    10788 2024-04-15 07:24:27.000000 wikidot-3.0.2/wikidot/connector/ajax.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)      261 2024-04-11 05:41:21.000000 wikidot-3.0.2/wikidot/connector/api.py
+drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-16 06:45:24.981846 wikidot-3.0.2/wikidot/module/
+-rw-r--r--   0 ukwhatn    (501) staff       (20)        0 2024-04-11 05:41:21.000000 wikidot-3.0.2/wikidot/module/__init__.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     2091 2024-04-11 05:41:21.000000 wikidot-3.0.2/wikidot/module/auth.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     6407 2024-04-15 07:24:27.000000 wikidot-3.0.2/wikidot/module/client.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)    14671 2024-04-16 06:41:50.000000 wikidot-3.0.2/wikidot/module/page.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     3602 2024-04-16 06:41:50.000000 wikidot-3.0.2/wikidot/module/page_revision.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)      194 2024-04-15 07:34:32.000000 wikidot-3.0.2/wikidot/module/page_source.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     8665 2024-04-16 06:41:50.000000 wikidot-3.0.2/wikidot/module/private_message.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     6742 2024-04-16 06:21:58.000000 wikidot-3.0.2/wikidot/module/site.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     3053 2024-04-11 05:41:21.000000 wikidot-3.0.2/wikidot/module/site_application.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     7868 2024-04-16 06:41:50.000000 wikidot-3.0.2/wikidot/module/user.py
+drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-16 06:45:24.982522 wikidot-3.0.2/wikidot/util/
+-rw-r--r--   0 ukwhatn    (501) staff       (20)        0 2024-04-11 05:41:21.000000 wikidot-3.0.2/wikidot/util/__init__.py
+drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-16 06:45:24.982987 wikidot-3.0.2/wikidot/util/parser/
+-rw-r--r--   0 ukwhatn    (501) staff       (20)       77 2024-04-11 05:41:21.000000 wikidot-3.0.2/wikidot/util/parser/__init__.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)      752 2024-04-11 05:41:21.000000 wikidot-3.0.2/wikidot/util/parser/odate.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     2038 2024-04-11 05:41:21.000000 wikidot-3.0.2/wikidot/util/parser/user.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     2635 2024-04-11 05:41:21.000000 wikidot-3.0.2/wikidot/util/quick_module.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     1869 2024-04-11 05:41:21.000000 wikidot-3.0.2/wikidot/util/requestutil.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     1477 2024-04-11 05:41:21.000000 wikidot-3.0.2/wikidot/util/stringutil.py
+drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-16 06:45:24.983248 wikidot-3.0.2/wikidot/util/table/
+-rw-r--r--   0 ukwhatn    (501) staff       (20)        0 2024-04-11 05:41:21.000000 wikidot-3.0.2/wikidot/util/table/__init__.py
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     7128 2024-04-11 05:41:21.000000 wikidot-3.0.2/wikidot/util/table/char_table.py
+drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-16 06:45:24.983619 wikidot-3.0.2/wikidot.egg-info/
+-rw-r--r--   0 ukwhatn    (501) staff       (20)     3121 2024-04-16 06:45:24.000000 wikidot-3.0.2/wikidot.egg-info/PKG-INFO
+-rw-r--r--   0 ukwhatn    (501) staff       (20)      934 2024-04-16 06:45:24.000000 wikidot-3.0.2/wikidot.egg-info/SOURCES.txt
+-rw-r--r--   0 ukwhatn    (501) staff       (20)        1 2024-04-16 06:45:24.000000 wikidot-3.0.2/wikidot.egg-info/dependency_links.txt
+-rw-r--r--   0 ukwhatn    (501) staff       (20)       68 2024-04-16 06:45:24.000000 wikidot-3.0.2/wikidot.egg-info/requires.txt
+-rw-r--r--   0 ukwhatn    (501) staff       (20)        8 2024-04-16 06:45:24.000000 wikidot-3.0.2/wikidot.egg-info/top_level.txt
```

### Comparing `wikidot-3.0.1/LICENSE` & `wikidot-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.1/PKG-INFO` & `wikidot-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikidot
-Version: 3.0.1
+Version: 3.0.2
 Summary: Wikidot Utility Library
 Author-email: ukwhatn <ukwhatn@gmail.com>
 Project-URL: Homepage, https://github.com/ukwhatn/wikidot.py
 Project-URL: Bug Tracker, https://github.com/ukwhatn/wikidot.py/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `wikidot-3.0.1/README.md` & `wikidot-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.1/pyproject.toml` & `wikidot-3.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "wikidot"
-version = "3.0.1"
+version = "3.0.2"
 authors = [{ name = "ukwhatn", email = "ukwhatn@gmail.com" }]
 description = "Wikidot Utility Library"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3.10",
```

### Comparing `wikidot-3.0.1/wikidot/common/decorators.py` & `wikidot-3.0.2/wikidot/common/decorators.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.1/wikidot/common/exceptions.py` & `wikidot-3.0.2/wikidot/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.1/wikidot/connector/ajax.py` & `wikidot-3.0.2/wikidot/connector/ajax.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.1/wikidot/module/auth.py` & `wikidot-3.0.2/wikidot/module/auth.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.1/wikidot/module/client.py` & `wikidot-3.0.2/wikidot/module/client.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.1/wikidot/module/page.py` & `wikidot-3.0.2/wikidot/module/page.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import re
+from collections.abc import Iterator
 from dataclasses import dataclass, asdict
 from datetime import datetime
 from typing import TYPE_CHECKING, Optional, Union, Any
 
 from bs4 import BeautifulSoup
 
 from wikidot.common import exceptions
+from wikidot.module.page_revision import PageRevision, PageRevisionCollection
 from wikidot.module.page_source import PageSource
 from wikidot.util.parser import user as user_parser, odate as odate_parser
 from wikidot.util.requestutil import RequestUtil
 
 if TYPE_CHECKING:
     from wikidot.module.site import Site
     from wikidot.module.user import User
@@ -69,18 +71,29 @@
     def as_dict(self) -> dict[str, Any]:
         res = {k: v for k, v in asdict(self).items() if v is not None}
         if "tags" in res and isinstance(res["tags"], list):
             res["tags"] = " ".join(res["tags"])
         return res
 
 
-class PageCollection(list):
+class PageCollection(list['Page']):
+    def __init__(self, site: 'Site' = None, pages: list['Page'] = None):
+        super().__init__(pages or [])
+
+        if site is not None:
+            self.site = site
+        else:
+            self.site = self[0].site
+
+    def __iter__(self) -> Iterator['Page']:
+        return super().__iter__()
+
     @staticmethod
     def _parse(site: 'Site', html_body: BeautifulSoup):
-        pages = PageCollection()
+        pages = []
 
         for page_element in html_body.select("span.page"):
             page_params = {}
 
             # レーティング方式を判定
             is_5star_rating = page_element.select_one("span.rating span.page-rate-list-pages-start") is not None
 
@@ -126,15 +139,15 @@
 
                 else:
                     value = value_element.text.strip()
 
                 # keyを変換
                 if "_linked" in key:
                     key = key.replace("_linked", "")
-                elif key in ["comments", "children"]:
+                elif key in ["comments", "children", "revisions"]:
                     key = f"{key}_count"
                 elif key in ["rating_votes"]:
                     key = "votes"
 
                 page_params[key] = value
 
             # タグのリストを統合
@@ -144,15 +157,15 @@
 
             page_params["tags"] = page_params["tags"] + page_params["_tags"]
             del page_params["_tags"]
 
             # ページオブジェクトを作成
             pages.append(Page(site, **page_params))
 
-        return pages
+        return PageCollection(site, pages)
 
     @staticmethod
     def search_pages(
             site: 'Site',
             query: SearchPagesQuery = SearchPagesQuery()
     ):
         # 初回実行
@@ -192,34 +205,35 @@
                 _query_dict = query_dict.copy()
                 _query_dict["offset"] = i * query.perPage
                 request_bodies.append(_query_dict)
 
             responses = site.amc_request(request_bodies)
             html_bodies.extend([BeautifulSoup(response.json()["body"], "lxml") for response in responses])
 
-        pages = PageCollection()
+        pages = []
         for html_body in html_bodies:
             pages.extend(PageCollection._parse(site, html_body))
 
-        return pages
+        return PageCollection(site, pages)
 
     @staticmethod
     def _acquire_page_ids(
+            site: 'Site',
             pages: list['Page']
     ):
         # pagesからidが設定されていないものを抽出
         target_pages = [page for page in pages if not page.is_id_acquired()]
 
         # なければ終了
         if len(target_pages) == 0:
             return pages
 
         # norender, noredirectでアクセス
         responses = RequestUtil.request(
-            target_pages[0].site.client,
+            site.client,
             "GET",
             [f"{page.get_url()}/norender/true/noredirect/true" for page in target_pages]
         )
 
         # "WIKIREQUEST.info.pageId = xxx;"の値をidに設定
         for index, response in enumerate(responses):
             source = response.text
@@ -228,35 +242,80 @@
             if id_match is None:
                 raise exceptions.UnexpectedException(f'Cannot find page id: {target_pages[index].fullname}')
             target_pages[index].id = int(id_match.group(1))
 
         return pages
 
     def get_page_ids(self):
-        return PageCollection._acquire_page_ids(self)
+        return PageCollection._acquire_page_ids(self.site, self)
 
     @staticmethod
     def _acquire_page_sources(
+            site: 'Site',
             pages: list['Page']
     ):
         if len(pages) == 0:
-            return []
-        response = pages[0].site.amc_request([{
+            return pages
+
+        responses = site.amc_request([{
             "moduleName": "viewsource/ViewSourceModule",
             "page_id": page.id
         } for page in pages])
 
-        for page, response in zip(pages, response):
-            body = response.json()["body"]
+        for page, responses in zip(pages, responses):
+            body = responses.json()["body"]
             source = BeautifulSoup(body, "lxml").select_one("div.page-source").text.strip().removeprefix("\t")
             page.source = PageSource(page, source)
         return pages
 
     def get_page_sources(self):
-        return PageCollection._acquire_page_sources(self)
+        return PageCollection._acquire_page_sources(self.site, self)
+
+    @staticmethod
+    def _acquire_page_revisions(
+            site: 'Site',
+            pages: list['Page']
+    ):
+        if len(pages) == 0:
+            return pages
+
+        responses = site.amc_request([{
+            "moduleName": "history/PageRevisionListModule",
+            "page_id": page.id,
+            "options": {"all": True},
+            "perpage": 100000000  # pagerを使わずに全て取得
+        } for page in pages])
+
+        for page, response in zip(pages, responses):
+            body = response.json()["body"]
+            revs = []
+            body_html = BeautifulSoup(body, "lxml")
+            for rev_element in body_html.select('table.page-history > tr[id^=revision-row-]'):
+                rev_id = int(rev_element["id"].removeprefix("revision-row-"))
+
+                tds = rev_element.select("td")
+                rev_no = int(tds[0].text.strip().removesuffix("."))
+                created_by = user_parser(page.site.client, tds[4].select_one("span.printuser"))
+                created_at = odate_parser(tds[5].select_one("span.odate"))
+                comment = tds[6].text.strip()
+
+                revs.append(PageRevision(
+                    page=page,
+                    id=rev_id,
+                    rev_no=rev_no,
+                    created_by=created_by,
+                    created_at=created_at,
+                    comment=comment
+                ))
+            page.revisions = revs
+
+        return pages
+
+    def get_page_revisions(self):
+        return PageCollection._acquire_page_revisions(self.site, self)
 
 
 @dataclass
 class Page:
     """ページオブジェクト
 
     Attributes
@@ -279,15 +338,15 @@
         サイズ
     rating: int | float
         レーティング +/-ならint、5つ星ならfloat
     votes: int
         vote数
     rating_percent: float
         5つ星レーティングにおけるパーセンテージ
-    revisions: int
+    revisions_count: int
         リビジョン数
     parent_fullname: str | None
         親ページのフルネーム 存在しない場合はNone
     tags: list[str]
         タグのリスト
     created_by: User
         作成者
@@ -311,59 +370,79 @@
     title: str
     children_count: int
     comments_count: int
     size: int
     rating: int | float
     votes: int
     rating_percent: float
-    revisions: int
+    revisions_count: int
     parent_fullname: str | None
     tags: list[str]
     created_by: 'User'
     created_at: datetime
     updated_by: 'User'
     updated_at: datetime
     commented_by: Optional['User']
     commented_at: datetime
     _id: int = None
     _source: Optional[PageSource] = None
+    _revisions: list['PageRevision'] = None
 
     def get_url(self) -> str:
         return f"{self.site.get_url()}/{self.fullname}"
 
     @property
     def id(self) -> int:
         """ページID（必要であれば取得）
 
         Returns
         -------
         int
             ページID
         """
         if self._id is None:
-            PageCollection([self]).get_page_ids()
+            PageCollection(self.site, [self]).get_page_ids()
         return self._id
 
     @id.setter
     def id(self, value: int):
         self._id = value
 
     def is_id_acquired(self) -> bool:
         return self._id is not None
 
     @property
     def source(self) -> PageSource:
         if self._source is None:
-            PageCollection([self]).get_page_sources()
+            PageCollection(self.site, [self]).get_page_sources()
         return self._source
 
     @source.setter
     def source(self, value: PageSource):
         self._source = value
 
+    @property
+    def revisions(self) -> PageRevisionCollection['PageRevision']:
+        if self._revisions is None:
+            PageCollection(self.site, [self]).get_page_revisions()
+        return PageRevisionCollection(self, self._revisions)
+
+    @revisions.setter
+    def revisions(self, value: list['PageRevision'] | PageRevisionCollection['PageRevision']):
+        self._revisions = value
+
+    @property
+    def latest_revision(self) -> PageRevision:
+        # revision_countとrev_noが一致するものを取得
+        for revision in self.revisions:
+            if revision.rev_no == self.revisions_count:
+                return revision
+
+        raise exceptions.NotFoundException("Cannot find latest revision")
+
     def destroy(self):
         self.site.client.login_check()
         self.site.amc_request([{
             "action": "WikiPageAction",
             "event": "deletePage",
             "page_id": self.id,
             "moduleName": "Empty"
```

### Comparing `wikidot-3.0.1/wikidot/module/private_message.py` & `wikidot-3.0.2/wikidot/module/private_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 from dataclasses import dataclass
 from datetime import datetime
 from typing import TYPE_CHECKING
+from collections.abc import Iterator
 
 import httpx
 from bs4 import BeautifulSoup, Tag, ResultSet
 
 from wikidot.common import exceptions
 from wikidot.common.decorators import login_required
 from wikidot.util.parser import odate as odate_parser, user as user_parser
 
 if TYPE_CHECKING:
     from wikidot.module.user import AbstractUser, User
     from wikidot.module.client import Client
 
 
-class PrivateMessageCollection(list):
+class PrivateMessageCollection(list['PrivateMessage']):
     def __str__(self):
         return f'{self.__class__.__name__}({len(self)} messages)'
 
+    def __iter__(self) -> Iterator['PrivateMessage']:
+        return super().__iter__()
+
     @staticmethod
     @login_required
     def from_ids(
             client: 'Client',
             message_ids: list[int]
     ) -> 'PrivateMessageCollection':
         """メッセージIDのリストからメッセージオブジェクトのリストを取得する
```

### Comparing `wikidot-3.0.1/wikidot/module/site.py` & `wikidot-3.0.2/wikidot/module/site.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.1/wikidot/module/site_application.py` & `wikidot-3.0.2/wikidot/module/site_application.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.1/wikidot/module/user.py` & `wikidot-3.0.2/wikidot/module/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,27 @@
+from collections.abc import Iterator
 from dataclasses import dataclass
 from typing import TYPE_CHECKING
 
 from bs4 import BeautifulSoup
 
 from wikidot.common.exceptions import NotFoundException
 from wikidot.util.requestutil import RequestUtil
 from wikidot.util.stringutil import StringUtil
 
 if TYPE_CHECKING:
     from wikidot.module.client import Client
 
 
-class UserCollection(list):
+class UserCollection(list['AbstractUser']):
     """ユーザーオブジェクトのリスト"""
 
+    def __iter__(self) -> Iterator['AbstractUser']:
+        return super().__iter__()
+
     @staticmethod
     def from_names(
             client: 'Client',
             names: list[str],
             raise_when_not_found: bool = False
     ) -> 'UserCollection':
         """ユーザー名のリストからユーザーオブジェクトのリストを取得する
```

### Comparing `wikidot-3.0.1/wikidot/util/parser/odate.py` & `wikidot-3.0.2/wikidot/util/parser/odate.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.1/wikidot/util/parser/user.py` & `wikidot-3.0.2/wikidot/util/parser/user.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.1/wikidot/util/quick_module.py` & `wikidot-3.0.2/wikidot/util/quick_module.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.1/wikidot/util/requestutil.py` & `wikidot-3.0.2/wikidot/util/requestutil.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.1/wikidot/util/stringutil.py` & `wikidot-3.0.2/wikidot/util/stringutil.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.1/wikidot/util/table/char_table.py` & `wikidot-3.0.2/wikidot/util/table/char_table.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.1/wikidot.egg-info/PKG-INFO` & `wikidot-3.0.2/wikidot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikidot
-Version: 3.0.1
+Version: 3.0.2
 Summary: Wikidot Utility Library
 Author-email: ukwhatn <ukwhatn@gmail.com>
 Project-URL: Homepage, https://github.com/ukwhatn/wikidot.py
 Project-URL: Bug Tracker, https://github.com/ukwhatn/wikidot.py/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `wikidot-3.0.1/wikidot.egg-info/SOURCES.txt` & `wikidot-3.0.2/wikidot.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 wikidot/connector/__init__.py
 wikidot/connector/ajax.py
 wikidot/connector/api.py
 wikidot/module/__init__.py
 wikidot/module/auth.py
 wikidot/module/client.py
 wikidot/module/page.py
+wikidot/module/page_revision.py
 wikidot/module/page_source.py
 wikidot/module/private_message.py
 wikidot/module/site.py
 wikidot/module/site_application.py
 wikidot/module/user.py
 wikidot/util/__init__.py
 wikidot/util/quick_module.py
```

