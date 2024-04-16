# Comparing `tmp/get_bibtex-1.0.1.tar.gz` & `tmp/get_bibtex-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "get_bibtex-1.0.1.tar", last modified: Sun Apr 14 12:04:37 2024, max compression
+gzip compressed data, was "get_bibtex-1.1.0.tar", last modified: Tue Apr 16 13:31:38 2024, max compression
```

## Comparing `get_bibtex-1.0.1.tar` & `get_bibtex-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:04:37.359810 get_bibtex-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-14 12:04:37.359810 get_bibtex-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-14 12:04:29.000000 get_bibtex-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:04:37.359810 get_bibtex-1.0.1/apiModels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 12:04:29.000000 get_bibtex-1.0.1/apiModels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-04-14 12:04:29.000000 get_bibtex-1.0.1/apiModels/get_bibtex_from_crossref.py
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-14 12:04:29.000000 get_bibtex-1.0.1/apiModels/get_bibtex_from_google_scholar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:04:37.359810 get_bibtex-1.0.1/get_bibtex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-14 12:04:37.000000 get_bibtex-1.0.1/get_bibtex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-14 12:04:37.000000 get_bibtex-1.0.1/get_bibtex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 12:04:37.000000 get_bibtex-1.0.1/get_bibtex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-14 12:04:37.000000 get_bibtex-1.0.1/get_bibtex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 12:04:37.359810 get_bibtex-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-14 12:04:29.000000 get_bibtex-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:04:37.359810 get_bibtex-1.0.1/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 12:04:29.000000 get_bibtex-1.0.1/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-14 12:04:29.000000 get_bibtex-1.0.1/utils/get_bibtex_from_link.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-14 12:04:29.000000 get_bibtex-1.0.1/utils/verify.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:31:38.614428 get_bibtex-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-16 13:31:38.614428 get_bibtex-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-16 13:31:30.000000 get_bibtex-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:31:38.610427 get_bibtex-1.1.0/apiModels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:31:30.000000 get_bibtex-1.1.0/apiModels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-16 13:31:30.000000 get_bibtex-1.1.0/apiModels/get_bibtex_from_crossref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-16 13:31:30.000000 get_bibtex-1.1.0/apiModels/get_bibtex_from_dblp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-04-16 13:31:30.000000 get_bibtex-1.1.0/apiModels/get_bibtex_from_google_scholar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-16 13:31:30.000000 get_bibtex-1.1.0/apiModels/meta_class.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:31:38.610427 get_bibtex-1.1.0/apiModels/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:31:30.000000 get_bibtex-1.1.0/apiModels/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-16 13:31:30.000000 get_bibtex-1.1.0/apiModels/utils/verify.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:31:38.614428 get_bibtex-1.1.0/apiModels/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:31:30.000000 get_bibtex-1.1.0/apiModels/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-04-16 13:31:30.000000 get_bibtex-1.1.0/apiModels/workflow/crossref2dblp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-16 13:31:30.000000 get_bibtex-1.1.0/apiModels/workflow/make_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:31:38.614428 get_bibtex-1.1.0/get_bibtex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-16 13:31:38.000000 get_bibtex-1.1.0/get_bibtex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-16 13:31:38.000000 get_bibtex-1.1.0/get_bibtex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 13:31:38.000000 get_bibtex-1.1.0/get_bibtex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 13:31:38.000000 get_bibtex-1.1.0/get_bibtex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 13:31:38.614428 get_bibtex-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-16 13:31:30.000000 get_bibtex-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:31:38.614428 get_bibtex-1.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-16 13:31:30.000000 get_bibtex-1.1.0/test/test_api_models.py
```

### Comparing `get_bibtex-1.0.1/PKG-INFO` & `get_bibtex-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: get_bibtex
-Version: 1.0.1
+Version: 1.1.0
 Summary: This is a project to get bibtex from CrossRef and Google Scholar
 Author: Yaowen Liu
 Author-email: 153672925@qq.com
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -12,15 +12,15 @@
 Classifier: Intended Audience :: Education
 Classifier: Natural Language :: English
 Classifier: Natural Language :: Chinese (Simplified)
 Description-Content-Type: text/markdown
 
 
 # get bibtex from crossref and google scholar
-
+Switch to [Chinese](README_CN.md)
 ## Introduction
 This is a simple python script to get bibtex from crossref and google scholar. It is useful when you want to get bibtex for a list of DOIs or titles.
 
 ## Depend
 - requests // for http request
 - re // for regular expression
 - serpapi // for google scholar
```

### Comparing `get_bibtex-1.0.1/README.md` & `get_bibtex-1.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 # get bibtex from crossref and google scholar
-
+Switch to [Chinese](README_CN.md)
 ## Introduction
 This is a simple python script to get bibtex from crossref and google scholar. It is useful when you want to get bibtex for a list of DOIs or titles.
 
 ## Depend
 - requests // for http request
 - re // for regular expression
 - serpapi // for google scholar
```

### Comparing `get_bibtex-1.0.1/apiModels/get_bibtex_from_crossref.py` & `get_bibtex-1.1.0/apiModels/get_bibtex_from_crossref.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import requests
 from requests.adapters import HTTPAdapter
 from tqdm import tqdm
 
+from apiModels.meta_class import AbstractGetBibTex
 
-class GetBibTex:
+
+class GetBibTex(AbstractGetBibTex):
     """
     Get BibTex from citation strings using the Google Scholar API
     Done by: liuyaowen
     Since: 2024-4-10
     """
     def __init__(self, email, max_retries=5, rows=4):
         """
@@ -57,21 +59,23 @@
         """
         :param citations:  a list of citation strings
         :return:  a list of BibTex strings
         """
         assert isinstance(citations, list)
         bibtexs = []
         failed_citations = []
-        for citation in tqdm(citations):
+        for citation in tqdm(citations, desc="Getting BibTex from CrossRef"):
             bibtex = self.get_bibtex(citation)
-            if bibtex:
+            if bibtex is not False:
                 bibtexs.append(bibtex)
             else:
                 failed_citations.append(citation)
         return bibtexs, failed_citations
 
-
-
-
-
-if __name__ == '__main__':
-    var = list["https://doi.org/10.1016/j.joi.2021.102579"]
+    def isready(self):
+        """
+        :return:  True if the API is available
+        """
+        try:
+            self.session.get(self.api_url, headers=self.headers, params=self.params)
+        except Exception as e:
+            raise ConnectionError("Crossref API not available")
```

### Comparing `get_bibtex-1.0.1/apiModels/get_bibtex_from_google_scholar.py` & `get_bibtex-1.1.0/apiModels/get_bibtex_from_google_scholar.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+from typing import Tuple, List
+
 import requests
 from serpapi import GoogleSearch
 from tqdm import tqdm
-from typing import Tuple, List, Any, Union
+
+from apiModels.meta_class import AbstractGetBibTex
 
 
-class GetBibTexFromGoogleScholar:
+class GetBibTexFromGoogleScholar(AbstractGetBibTex):
     """
     Get BibTex from citation strings using the Google Scholar API
     Done by: liuyaowen
     Since: 2024-4-10
     """
     # citation style
     MPA = 0
@@ -61,17 +64,17 @@
         """
         :param citations: a list of citation strings
         :return:    if flag is True, return bibtexs else return snippets
                     and if link request failed, return snippets
         """
         bibtexs = []
         snippets = []
-        for citation in tqdm(citations):
+        for citation in tqdm(citations, desc="Getting BibTex from Google Scholar"):
             bibtex = self.get_bibtex(citation)
-            if bibtex:
+            if bibtex is not False:
                 bibtexs.append(bibtex)
             else:
                 snippets.append(citation)
         return bibtexs, snippets
 
     def __get_result_id(self, query):
         """
@@ -92,8 +95,17 @@
                 result_ = result_[:-1]
                 print(result_)
             query_ = query.replace(" ", "").lower()
             # verify the result is the paper we want to find,beacuse the result may not be the word in the citation,
             # so we need sure the paper's length is more than 10 so that decrease the probability of wrong result
             if result_ in query_ and len(result_) > 10:
                 return result["result_id"]
-            return False
+            return False
+
+    def isready(self):
+        """
+        :return: True if the API is available
+        """
+        try:
+            self.__get_result_id("test")
+        except Exception as e:
+            raise ConnectionError("Google Scholar API not available")
```

### Comparing `get_bibtex-1.0.1/get_bibtex.egg-info/PKG-INFO` & `get_bibtex-1.1.0/get_bibtex.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: get_bibtex
-Version: 1.0.1
+Version: 1.1.0
 Summary: This is a project to get bibtex from CrossRef and Google Scholar
 Author: Yaowen Liu
 Author-email: 153672925@qq.com
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -12,15 +12,15 @@
 Classifier: Intended Audience :: Education
 Classifier: Natural Language :: English
 Classifier: Natural Language :: Chinese (Simplified)
 Description-Content-Type: text/markdown
 
 
 # get bibtex from crossref and google scholar
-
+Switch to [Chinese](README_CN.md)
 ## Introduction
 This is a simple python script to get bibtex from crossref and google scholar. It is useful when you want to get bibtex for a list of DOIs or titles.
 
 ## Depend
 - requests // for http request
 - re // for regular expression
 - serpapi // for google scholar
```

### Comparing `get_bibtex-1.0.1/setup.py` & `get_bibtex-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         "Natural Language :: English",
         "Natural Language :: Chinese (Simplified)",
 
     ],
 
     # 如果上传时出现ERROR：The user '' isn't allowed to upload to project ''，换个名字，长一点无所谓，不能跟别人重复
     name="get_bibtex",
-    version="1.0.1",
+    version="1.1.0",
     author="Yaowen Liu",
     author_email="153672925@qq.com",
     description="This is a project to get bibtex from CrossRef and Google Scholar",
     long_description=my_long_description,
 
     # 存放源码的地址，填入gitee的源码网址即可
     # url="https://gitee.com/UnderTurrets/",
```

