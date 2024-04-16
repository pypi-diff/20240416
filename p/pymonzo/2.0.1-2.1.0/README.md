# Comparing `tmp/pymonzo-2.0.1.tar.gz` & `tmp/pymonzo-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymonzo-2.0.1.tar", last modified: Sat Apr 13 15:36:41 2024, max compression
+gzip compressed data, was "pymonzo-2.1.0.tar", last modified: Tue Apr 16 16:51:12 2024, max compression
```

## Comparing `pymonzo-2.0.1.tar` & `pymonzo-2.1.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    16725 2024-04-13 15:36:41.000000 pymonzo-2.0.1/LICENSE
--rw-r--r--   0        0        0     2669 2024-04-13 15:36:41.000000 pymonzo-2.0.1/README.md
--rw-r--r--   0        0        0     3677 2024-04-13 15:36:41.000000 pymonzo-2.0.1/pyproject.toml
--rw-r--r--   0        0        0      700 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/__init__.py
--rw-r--r--   0        0        0      271 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/accounts/__init__.py
--rw-r--r--   0        0        0      523 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/accounts/enums.py
--rw-r--r--   0        0        0     2216 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/accounts/resources.py
--rw-r--r--   0        0        0     3038 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/accounts/schemas.py
--rw-r--r--   0        0        0      223 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/attachments/__init__.py
--rw-r--r--   0        0        0     3037 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/attachments/resources.py
--rw-r--r--   0        0        0     1144 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/attachments/schemas.py
--rw-r--r--   0        0        0      183 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/balance/__init__.py
--rw-r--r--   0        0        0     1199 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/balance/resources.py
--rw-r--r--   0        0        0     2422 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/balance/schemas.py
--rw-r--r--   0        0        0     7970 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/client.py
--rw-r--r--   0        0        0      514 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/exceptions.py
--rw-r--r--   0        0        0      186 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/feed/__init__.py
--rw-r--r--   0        0        0     1700 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/feed/resources.py
--rw-r--r--   0        0        0     1144 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/feed/schemas.py
--rw-r--r--   0        0        0      170 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/pots/__init__.py
--rw-r--r--   0        0        0     6685 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/pots/resources.py
--rw-r--r--   0        0        0     1786 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/pots/schemas.py
--rw-r--r--   0        0        0        0 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/py.typed
--rw-r--r--   0        0        0     1852 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/resources.py
--rw-r--r--   0        0        0     1594 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/settings.py
--rw-r--r--   0        0        0      361 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/transactions/__init__.py
--rw-r--r--   0        0        0     1324 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/transactions/enums.py
--rw-r--r--   0        0        0     3954 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/transactions/resources.py
--rw-r--r--   0        0        0     7358 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/transactions/schemas.py
--rw-r--r--   0        0        0     2697 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/utils.py
--rw-r--r--   0        0        0      252 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/webhooks/__init__.py
--rw-r--r--   0        0        0     2744 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/webhooks/resources.py
--rw-r--r--   0        0        0     2346 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/webhooks/schemas.py
--rw-r--r--   0        0        0      196 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/whoami/__init__.py
--rw-r--r--   0        0        0      733 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/whoami/resources.py
--rw-r--r--   0        0        0     1028 2024-04-13 15:36:41.000000 pymonzo-2.0.1/src/pymonzo/whoami/schemas.py
--rw-r--r--   0        0        0     5093 1970-01-01 00:00:00.000000 pymonzo-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0    16725 2024-04-16 16:51:12.000000 pymonzo-2.1.0/LICENSE
+-rw-r--r--   0        0        0     2669 2024-04-16 16:51:12.000000 pymonzo-2.1.0/README.md
+-rw-r--r--   0        0        0     3677 2024-04-16 16:51:12.000000 pymonzo-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      700 2024-04-16 16:51:12.000000 pymonzo-2.1.0/src/pymonzo/__init__.py
+-rw-r--r--   0        0        0      271 2024-04-16 16:51:12.000000 pymonzo-2.1.0/src/pymonzo/accounts/__init__.py
+-rw-r--r--   0        0        0      523 2024-04-16 16:51:12.000000 pymonzo-2.1.0/src/pymonzo/accounts/enums.py
+-rw-r--r--   0        0        0     2216 2024-04-16 16:51:12.000000 pymonzo-2.1.0/src/pymonzo/accounts/resources.py
+-rw-r--r--   0        0        0     3032 2024-04-16 16:51:12.000000 pymonzo-2.1.0/src/pymonzo/accounts/schemas.py
+-rw-r--r--   0        0        0      223 2024-04-16 16:51:12.000000 pymonzo-2.1.0/src/pymonzo/attachments/__init__.py
+-rw-r--r--   0        0        0     3037 2024-04-16 16:51:12.000000 pymonzo-2.1.0/src/pymonzo/attachments/resources.py
+-rw-r--r--   0        0        0     1144 2024-04-16 16:51:12.000000 pymonzo-2.1.0/src/pymonzo/attachments/schemas.py
+-rw-r--r--   0        0        0      183 2024-04-16 16:51:12.000000 pymonzo-2.1.0/src/pymonzo/balance/__init__.py
+-rw-r--r--   0        0        0     1199 2024-04-16 16:51:12.000000 pymonzo-2.1.0/src/pymonzo/balance/resources.py
+-rw-r--r--   0        0        0     2422 2024-04-16 16:51:12.000000 pymonzo-2.1.0/src/pymonzo/balance/schemas.py
+-rw-r--r--   0        0        0     7970 2024-04-16 16:51:12.000000 pymonzo-2.1.0/src/pymonzo/client.py
+-rw-r--r--   0        0        0      514 2024-04-16 16:51:12.000000 pymonzo-2.1.0/src/pymonzo/exceptions.py
+-rw-r--r--   0        0        0      186 2024-04-16 16:51:12.000000 pymonzo-2.1.0/src/pymonzo/feed/__init__.py
+-rw-r--r--   0        0        0     1700 2024-04-16 16:51:12.000000 pymonzo-2.1.0/src/pymonzo/feed/resources.py
+-rw-r--r--   0        0        0     1144 2024-04-16 16:51:12.000000 pymonzo-2.1.0/src/pymonzo/feed/schemas.py
+-rw-r--r--   0        0        0      170 2024-04-16 16:51:12.000000 pymonzo-2.1.0/src/pymonzo/pots/__init__.py
+-rw-r--r--   0        0        0     6685 2024-04-16 16:51:12.000000 pymonzo-2.1.0/src/pymonzo/pots/resources.py
+-rw-r--r--   0        0        0     3592 2024-04-16 16:51:12.000000 pymonzo-2.1.0/src/pymonzo/pots/schemas.py
+-rw-r--r--   0        0        0        0 2024-04-16 16:51:12.000000 pymonzo-2.1.0/src/pymonzo/py.typed
+-rw-r--r--   0        0        0     1852 2024-04-16 16:51:12.000000 pymonzo-2.1.0/src/pymonzo/resources.py
+-rw-r--r--   0        0        0     1594 2024-04-16 16:51:12.000000 pymonzo-2.1.0/src/pymonzo/settings.py
+-rw-r--r--   0        0        0      361 2024-04-16 16:51:12.000000 pymonzo-2.1.0/src/pymonzo/transactions/__init__.py
+-rw-r--r--   0        0        0     1324 2024-04-16 16:51:12.000000 pymonzo-2.1.0/src/pymonzo/transactions/enums.py
+-rw-r--r--   0        0        0     3954 2024-04-16 16:51:12.000000 pymonzo-2.1.0/src/pymonzo/transactions/resources.py
+-rw-r--r--   0        0        0     7475 2024-04-16 16:51:12.000000 pymonzo-2.1.0/src/pymonzo/transactions/schemas.py
+-rw-r--r--   0        0        0     2697 2024-04-16 16:51:12.000000 pymonzo-2.1.0/src/pymonzo/utils.py
+-rw-r--r--   0        0        0      252 2024-04-16 16:51:12.000000 pymonzo-2.1.0/src/pymonzo/webhooks/__init__.py
+-rw-r--r--   0        0        0     2744 2024-04-16 16:51:12.000000 pymonzo-2.1.0/src/pymonzo/webhooks/resources.py
+-rw-r--r--   0        0        0     2346 2024-04-16 16:51:12.000000 pymonzo-2.1.0/src/pymonzo/webhooks/schemas.py
+-rw-r--r--   0        0        0      196 2024-04-16 16:51:12.000000 pymonzo-2.1.0/src/pymonzo/whoami/__init__.py
+-rw-r--r--   0        0        0      733 2024-04-16 16:51:12.000000 pymonzo-2.1.0/src/pymonzo/whoami/resources.py
+-rw-r--r--   0        0        0     1028 2024-04-16 16:51:12.000000 pymonzo-2.1.0/src/pymonzo/whoami/schemas.py
+-rw-r--r--   0        0        0     5093 1970-01-01 00:00:00.000000 pymonzo-2.1.0/PKG-INFO
```

### Comparing `pymonzo-2.0.1/LICENSE` & `pymonzo-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.1/README.md` & `pymonzo-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.1/pyproject.toml` & `pymonzo-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.1/src/pymonzo/__init__.py` & `pymonzo-2.1.0/src/pymonzo/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 [pydantic]: https://github.com/pydantic/pydantic
 """
 
 from pymonzo.client import MonzoAPI  # noqa
 
 __title__ = "pymonzo"
 __description__ = "Modern Python API client for Monzo public API."
-__version__ = "2.0.1"
+__version__ = "2.1.0"
 __url__ = "https://github.com/pawelad/pymonzo"
 __author__ = "Paweł Adamczak"
 __email__ = "pawel.ad@gmail.com"
 __license__ = "MPL-2.0"
```

### Comparing `pymonzo-2.0.1/src/pymonzo/accounts/enums.py` & `pymonzo-2.1.0/src/pymonzo/accounts/enums.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.1/src/pymonzo/accounts/resources.py` & `pymonzo-2.1.0/src/pymonzo/accounts/resources.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.1/src/pymonzo/accounts/schemas.py` & `pymonzo-2.1.0/src/pymonzo/accounts/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
             grid = Table.grid(padding=(0, 5))
             grid.title = f"Account '{self.id}' ({self.country_code})"
             grid.title_style = "bold green"
             grid.add_column(style="bold cyan")
             grid.add_column(style="" if not self.closed else "dim")
             grid.add_row("ID:", self.id)
             grid.add_row("Description:", self.description)
-            grid.add_row("Currency:", f"{self.currency} ")
+            grid.add_row("Currency:", self.currency)
             if self.account_number:
                 grid.add_row("Account Number:", self.account_number)
             if self.sort_code:
                 grid.add_row("Sort Code:", "-".join(wrap(self.sort_code, 2)))
             grid.add_row("Type:", self.type)
             grid.add_row("Closed:", "Yes" if self.closed else "No")
             grid.add_row("Created:", format_datetime(self.created))
```

### Comparing `pymonzo-2.0.1/src/pymonzo/attachments/resources.py` & `pymonzo-2.1.0/src/pymonzo/attachments/resources.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.1/src/pymonzo/attachments/schemas.py` & `pymonzo-2.1.0/src/pymonzo/attachments/schemas.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.1/src/pymonzo/balance/resources.py` & `pymonzo-2.1.0/src/pymonzo/balance/resources.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.1/src/pymonzo/balance/schemas.py` & `pymonzo-2.1.0/src/pymonzo/balance/schemas.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.1/src/pymonzo/client.py` & `pymonzo-2.1.0/src/pymonzo/client.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.1/src/pymonzo/exceptions.py` & `pymonzo-2.1.0/src/pymonzo/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.1/src/pymonzo/feed/resources.py` & `pymonzo-2.1.0/src/pymonzo/feed/resources.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.1/src/pymonzo/feed/schemas.py` & `pymonzo-2.1.0/src/pymonzo/feed/schemas.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.1/src/pymonzo/pots/resources.py` & `pymonzo-2.1.0/src/pymonzo/pots/resources.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.1/src/pymonzo/resources.py` & `pymonzo-2.1.0/src/pymonzo/resources.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.1/src/pymonzo/settings.py` & `pymonzo-2.1.0/src/pymonzo/settings.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.1/src/pymonzo/transactions/enums.py` & `pymonzo-2.1.0/src/pymonzo/transactions/enums.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.1/src/pymonzo/transactions/resources.py` & `pymonzo-2.1.0/src/pymonzo/transactions/resources.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.1/src/pymonzo/transactions/schemas.py` & `pymonzo-2.1.0/src/pymonzo/transactions/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,19 +176,22 @@
         return empty_str_to_none(v)
 
     if RICH_AVAILABLE:
 
         def __rich__(self) -> Table:
             """Pretty printing support for `rich`."""
             amount = format_currency(self.amount / 100, self.currency)
+            amount_color = "green" if self.amount > 0 else "red"
 
             grid = Table.grid(padding=(0, 5))
             grid.title = f"{amount} | {self.description}"
             grid.title_style = (
-                "bold green" if not self.decline_reason else "bold green dim"
+                f"bold {amount_color}"
+                if not self.decline_reason
+                else f"bold {amount_color} dim"
             )
             grid.add_column(style="bold cyan")
             grid.add_column(
                 style="" if not self.decline_reason else "dim",
                 max_width=50,
             )
             grid.add_row("ID:", self.id)
```

### Comparing `pymonzo-2.0.1/src/pymonzo/utils.py` & `pymonzo-2.1.0/src/pymonzo/utils.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.1/src/pymonzo/webhooks/resources.py` & `pymonzo-2.1.0/src/pymonzo/webhooks/resources.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.1/src/pymonzo/webhooks/schemas.py` & `pymonzo-2.1.0/src/pymonzo/webhooks/schemas.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.1/src/pymonzo/whoami/resources.py` & `pymonzo-2.1.0/src/pymonzo/whoami/resources.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.1/src/pymonzo/whoami/schemas.py` & `pymonzo-2.1.0/src/pymonzo/whoami/schemas.py`

 * *Files identical despite different names*

### Comparing `pymonzo-2.0.1/PKG-INFO` & `pymonzo-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonzo
-Version: 2.0.1
+Version: 2.1.0
 Summary: Modern Python API client for Monzo public API.
 Keywords: monzo,api
 Author-email: Paweł Adamczak <pawel.ad@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

