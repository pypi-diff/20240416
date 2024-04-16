# Comparing `tmp/asyncio_payok-0.0.2.tar.gz` & `tmp/asyncio_payok-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncio_payok-0.0.2.tar", last modified: Tue Apr 16 11:53:01 2024, max compression
+gzip compressed data, was "asyncio_payok-0.0.3.tar", last modified: Tue Apr 16 12:03:18 2024, max compression
```

## Comparing `asyncio_payok-0.0.2.tar` & `asyncio_payok-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 11:53:01.642196 asyncio_payok-0.0.2/
--rw-rw-rw-   0        0        0     2250 2024-04-16 11:53:01.641194 asyncio_payok-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1920 2024-04-16 10:22:24.000000 asyncio_payok-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 11:53:01.613196 asyncio_payok-0.0.2/asyncio_payok/
--rw-rw-rw-   0        0        0       24 2024-04-09 06:26:31.000000 asyncio_payok-0.0.2/asyncio_payok/__init__.py
--rw-rw-rw-   0        0        0     5750 2024-04-16 10:23:54.000000 asyncio_payok-0.0.2/asyncio_payok/api.py
-drwxrwxrwx   0        0        0        0 2024-04-16 11:53:01.638192 asyncio_payok-0.0.2/asyncio_payok/const/
--rw-rw-rw-   0        0        0       40 2024-04-09 06:25:25.000000 asyncio_payok-0.0.2/asyncio_payok/const/__init__.py
--rw-rw-rw-   0        0        0      356 2024-04-08 11:04:10.000000 asyncio_payok-0.0.2/asyncio_payok/const/en.py
--rw-rw-rw-   0        0        0     1228 2024-04-09 06:25:25.000000 asyncio_payok-0.0.2/asyncio_payok/const/models.py
--rw-rw-rw-   0        0        0     1550 2024-04-15 12:48:38.000000 asyncio_payok-0.0.2/asyncio_payok/payok_base.py
-drwxrwxrwx   0        0        0        0 2024-04-16 11:53:01.640195 asyncio_payok-0.0.2/asyncio_payok.egg-info/
--rw-rw-rw-   0        0        0     2250 2024-04-16 11:53:01.000000 asyncio_payok-0.0.2/asyncio_payok.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      365 2024-04-16 11:53:01.000000 asyncio_payok-0.0.2/asyncio_payok.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 11:53:01.000000 asyncio_payok-0.0.2/asyncio_payok.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-16 11:53:01.000000 asyncio_payok-0.0.2/asyncio_payok.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-16 11:53:01.000000 asyncio_payok-0.0.2/asyncio_payok.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 11:53:01.642196 asyncio_payok-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      469 2024-04-16 11:52:51.000000 asyncio_payok-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 12:03:18.692370 asyncio_payok-0.0.3/
+-rw-rw-rw-   0        0        0     2250 2024-04-16 12:03:18.691374 asyncio_payok-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1920 2024-04-16 10:22:24.000000 asyncio_payok-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 12:03:18.674375 asyncio_payok-0.0.3/asyncio_payok/
+-rw-rw-rw-   0        0        0       24 2024-04-09 06:26:31.000000 asyncio_payok-0.0.3/asyncio_payok/__init__.py
+-rw-rw-rw-   0        0        0     5814 2024-04-16 12:03:14.000000 asyncio_payok-0.0.3/asyncio_payok/api.py
+drwxrwxrwx   0        0        0        0 2024-04-16 12:03:18.689375 asyncio_payok-0.0.3/asyncio_payok/const/
+-rw-rw-rw-   0        0        0       40 2024-04-09 06:25:25.000000 asyncio_payok-0.0.3/asyncio_payok/const/__init__.py
+-rw-rw-rw-   0        0        0      356 2024-04-08 11:04:10.000000 asyncio_payok-0.0.3/asyncio_payok/const/en.py
+-rw-rw-rw-   0        0        0     1228 2024-04-09 06:25:25.000000 asyncio_payok-0.0.3/asyncio_payok/const/models.py
+-rw-rw-rw-   0        0        0     1550 2024-04-15 12:48:38.000000 asyncio_payok-0.0.3/asyncio_payok/payok_base.py
+drwxrwxrwx   0        0        0        0 2024-04-16 12:03:18.691374 asyncio_payok-0.0.3/asyncio_payok.egg-info/
+-rw-rw-rw-   0        0        0     2250 2024-04-16 12:03:18.000000 asyncio_payok-0.0.3/asyncio_payok.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      365 2024-04-16 12:03:18.000000 asyncio_payok-0.0.3/asyncio_payok.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 12:03:18.000000 asyncio_payok-0.0.3/asyncio_payok.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-16 12:03:18.000000 asyncio_payok-0.0.3/asyncio_payok.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-16 12:03:18.000000 asyncio_payok-0.0.3/asyncio_payok.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 12:03:18.692370 asyncio_payok-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      469 2024-04-16 12:03:14.000000 asyncio_payok-0.0.3/setup.py
```

### Comparing `asyncio_payok-0.0.2/PKG-INFO` & `asyncio_payok-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncio_payok
-Version: 0.0.2
+Version: 0.0.3
 Summary: Asyncio client for PayOk API
 Home-page: https://github.com/slimeless/asycncio-payok
 Author: Abracadabra
 Author-email: stopcrybby@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
```

### Comparing `asyncio_payok-0.0.2/README.md` & `asyncio_payok-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `asyncio_payok-0.0.2/asyncio_payok/api.py` & `asyncio_payok-0.0.3/asyncio_payok/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 		Async function to retrieve transactions based on payment ID and offset.
 
 		:param payment_id: Optional[int] - The payment ID to filter transactions by.
 		:param offset: Optional[int] - The offset for paginating through transactions.
 		:return: Union[Transaction, list[Transaction]] - A single transaction or a list of transactions.
 		"""
 		method = Method.POST
+		if shop is None:
+			raise ValueError('Shop ID is required')
 		data = {
 			'API_ID': self.__api_id,
 			'API_KEY': self.__api_key,
 			'shop': self.__shop,
 		}
 		if payment_id:
 			data['payment_id'] = payment_id
```

### Comparing `asyncio_payok-0.0.2/asyncio_payok/const/models.py` & `asyncio_payok-0.0.3/asyncio_payok/const/models.py`

 * *Files identical despite different names*

### Comparing `asyncio_payok-0.0.2/asyncio_payok/payok_base.py` & `asyncio_payok-0.0.3/asyncio_payok/payok_base.py`

 * *Files identical despite different names*

### Comparing `asyncio_payok-0.0.2/asyncio_payok.egg-info/PKG-INFO` & `asyncio_payok-0.0.3/asyncio_payok.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncio_payok
-Version: 0.0.2
+Version: 0.0.3
 Summary: Asyncio client for PayOk API
 Home-page: https://github.com/slimeless/asycncio-payok
 Author: Abracadabra
 Author-email: stopcrybby@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
```

