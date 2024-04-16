# Comparing `tmp/dialog_whatsapp-0.0.1.5.tar.gz` & `tmp/dialog_whatsapp-0.0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialog_whatsapp-0.0.1.5.tar", max compression
+gzip compressed data, was "dialog_whatsapp-0.0.1.6.tar", max compression
```

## Comparing `dialog_whatsapp-0.0.1.5.tar` & `dialog_whatsapp-0.0.1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      442 2024-04-09 21:44:14.527027 dialog_whatsapp-0.0.1.5/README.md
--rw-r--r--   0        0        0        0 2024-04-09 21:44:14.527225 dialog_whatsapp-0.0.1.5/dialog_whatsapp/__init__.py
--rw-r--r--   0        0        0     5292 2024-04-12 20:16:52.888594 dialog_whatsapp-0.0.1.5/dialog_whatsapp/plugin.py
--rw-r--r--   0        0        0     1931 2024-04-10 12:58:05.999480 dialog_whatsapp-0.0.1.5/dialog_whatsapp/responses.py
--rw-r--r--   0        0        0     1467 2024-04-10 13:01:25.860692 dialog_whatsapp-0.0.1.5/dialog_whatsapp/settings.py
--rw-r--r--   0        0        0      439 2024-04-12 20:19:02.932568 dialog_whatsapp-0.0.1.5/pyproject.toml
--rw-r--r--   0        0        0      859 1970-01-01 00:00:00.000000 dialog_whatsapp-0.0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      442 2024-04-09 21:44:14.527027 dialog_whatsapp-0.0.1.6/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 21:44:14.527225 dialog_whatsapp-0.0.1.6/dialog_whatsapp/__init__.py
+-rw-r--r--   0        0        0     5313 2024-04-16 00:34:20.290629 dialog_whatsapp-0.0.1.6/dialog_whatsapp/plugin.py
+-rw-r--r--   0        0        0     1952 2024-04-16 00:34:26.445457 dialog_whatsapp-0.0.1.6/dialog_whatsapp/responses.py
+-rw-r--r--   0        0        0     1467 2024-04-10 13:01:25.860692 dialog_whatsapp-0.0.1.6/dialog_whatsapp/settings.py
+-rw-r--r--   0        0        0      439 2024-04-16 00:34:36.521178 dialog_whatsapp-0.0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      859 1970-01-01 00:00:00.000000 dialog_whatsapp-0.0.1.6/PKG-INFO
```

### Comparing `dialog_whatsapp-0.0.1.5/dialog_whatsapp/plugin.py` & `dialog_whatsapp-0.0.1.6/dialog_whatsapp/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     PROJECT_CONFIG,
     DATASET,
     OPENAI_API_KEY,
     ROUTE_SUFFIX
 )
 from dialog.llm.default import DialogLLM
 
-from dialog.models.helpers import create_session
+from dialog_lib.db.utils import create_chat_session as create_session
 from uuid import uuid4
 
 client = OpenAI()
 
 router = APIRouter()
 
 logger = logging.getLogger(__name__)
```

### Comparing `dialog_whatsapp-0.0.1.5/dialog_whatsapp/responses.py` & `dialog_whatsapp-0.0.1.6/dialog_whatsapp/responses.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from dialog_whatsapp.settings import (
     WHATSAPP_VERIFY_TOKEN,
     WHATSAPP_API_TOKEN,
     WHATSAPP_ACCOUNT_NUMBER,
     PROJECT_CONFIG
 )
 
-from dialog.models.helpers import create_session
+from dialog_lib.db.utils import create_chat_session as create_session
 
 logger = logging.getLogger(__name__)
 
 
 async def whatsapp_get_response(request):
     """
     Returns the challenge response for WhatsApp if verify token matches
```

### Comparing `dialog_whatsapp-0.0.1.5/dialog_whatsapp/settings.py` & `dialog_whatsapp-0.0.1.6/dialog_whatsapp/settings.py`

 * *Files identical despite different names*

### Comparing `dialog_whatsapp-0.0.1.5/PKG-INFO` & `dialog_whatsapp-0.0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dialog-whatsapp
-Version: 0.0.1.5
+Version: 0.0.1.6
 Summary: 
 Author: Vinicius Mesel
 Author-email: 4984147+vmesel@users.noreply.github.com
 Requires-Python: >=3.11,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

