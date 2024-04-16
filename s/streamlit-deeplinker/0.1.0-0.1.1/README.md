# Comparing `tmp/streamlit_deeplinker-0.1.0.tar.gz` & `tmp/streamlit_deeplinker-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_deeplinker-0.1.0.tar", max compression
+gzip compressed data, was "streamlit_deeplinker-0.1.1.tar", max compression
```

## Comparing `streamlit_deeplinker-0.1.0.tar` & `streamlit_deeplinker-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11358 2024-04-16 06:32:08.295244 streamlit_deeplinker-0.1.0/LICENCE
--rw-r--r--   0        0        0     2738 2024-04-16 06:32:08.295244 streamlit_deeplinker-0.1.0/README.md
--rw-r--r--   0        0        0      500 2024-04-16 06:32:08.299244 streamlit_deeplinker-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      189 2024-04-16 06:32:08.299244 streamlit_deeplinker-0.1.0/streamlit_deeplinker/__init__.py
--rw-r--r--   0        0        0     6438 2024-04-16 06:32:08.299244 streamlit_deeplinker-0.1.0/streamlit_deeplinker/router.py
--rw-r--r--   0        0        0     3302 1970-01-01 00:00:00.000000 streamlit_deeplinker-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-04-16 06:36:44.812632 streamlit_deeplinker-0.1.1/LICENCE
+-rw-r--r--   0        0        0     2953 2024-04-16 06:36:44.812632 streamlit_deeplinker-0.1.1/README.md
+-rw-r--r--   0        0        0      500 2024-04-16 06:36:44.812632 streamlit_deeplinker-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      189 2024-04-16 06:36:44.812632 streamlit_deeplinker-0.1.1/streamlit_deeplinker/__init__.py
+-rw-r--r--   0        0        0     6438 2024-04-16 06:36:44.812632 streamlit_deeplinker-0.1.1/streamlit_deeplinker/router.py
+-rw-r--r--   0        0        0     3517 1970-01-01 00:00:00.000000 streamlit_deeplinker-0.1.1/PKG-INFO
```

### Comparing `streamlit_deeplinker-0.1.0/LICENCE` & `streamlit_deeplinker-0.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `streamlit_deeplinker-0.1.0/README.md` & `streamlit_deeplinker-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,34 @@
-# Streamlit Deeplink
+# Streamlit Deeplinker
 
 Set state deep in an application with ease. 
 
 Make them navigatable through your broswer history, and shareable with other people through an URL.
 
+## Install
+Install with your favorite package manager
+
+**Poetry**: `poetry add streamlit-deeplinker`
+
+**Pip**: `pip install streamlit-deeplinker`
+
+And then you can start creating deeplink applications like the following:
+
 ```python
 from streamlit_deeplinker import deeplinks, set_deeplink
 from pydantic import BaseModel
 
 class StateA(BaseModel):
     name: str
 
-def page_a(state: StateA):
+async def page_a(state: StateA):
     ...
 
 @deeplinks(
-    deeplinks={ # type: ignore
+    deeplinks={
         StateA: page_a,
     }
 )
 def app():
     st.title("Deeplink Example")
 
     st.write("This is the landing page. You can navigate to other pages using the sidebar.")
```

### Comparing `streamlit_deeplinker-0.1.0/streamlit_deeplinker/router.py` & `streamlit_deeplinker-0.1.1/streamlit_deeplinker/router.py`

 * *Files identical despite different names*

### Comparing `streamlit_deeplinker-0.1.0/PKG-INFO` & `streamlit_deeplinker-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,49 @@
 Metadata-Version: 2.1
 Name: streamlit-deeplinker
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package that makes it possible to add deeplinks in a streamlit application
 Author: Mats E. Mollestad
 Author-email: mats@mollestad.no
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pydantic (>=2.7.0,<3.0.0)
 Requires-Dist: streamlit (>=1.33.0,<2.0.0)
 Description-Content-Type: text/markdown
 
-# Streamlit Deeplink
+# Streamlit Deeplinker
 
 Set state deep in an application with ease. 
 
 Make them navigatable through your broswer history, and shareable with other people through an URL.
 
+## Install
+Install with your favorite package manager
+
+**Poetry**: `poetry add streamlit-deeplinker`
+
+**Pip**: `pip install streamlit-deeplinker`
+
+And then you can start creating deeplink applications like the following:
+
 ```python
 from streamlit_deeplinker import deeplinks, set_deeplink
 from pydantic import BaseModel
 
 class StateA(BaseModel):
     name: str
 
-def page_a(state: StateA):
+async def page_a(state: StateA):
     ...
 
 @deeplinks(
-    deeplinks={ # type: ignore
+    deeplinks={
         StateA: page_a,
     }
 )
 def app():
     st.title("Deeplink Example")
 
     st.write("This is the landing page. You can navigate to other pages using the sidebar.")
```

