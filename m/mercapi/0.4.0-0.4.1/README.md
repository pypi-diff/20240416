# Comparing `tmp/mercapi-0.4.0.tar.gz` & `tmp/mercapi-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercapi-0.4.0.tar", max compression
+gzip compressed data, was "mercapi-0.4.1.tar", max compression
```

## Comparing `mercapi-0.4.0.tar` & `mercapi-0.4.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1065 2023-12-20 23:12:25.671068 mercapi-0.4.0/LICENSE
--rw-r--r--   0        0        0     1473 2023-12-20 23:12:25.671068 mercapi-0.4.0/README.md
--rw-r--r--   0        0        0       63 2023-12-20 23:12:25.683068 mercapi-0.4.0/mercapi/__init__.py
--rw-r--r--   0        0        0       38 2023-12-20 23:12:25.683068 mercapi-0.4.0/mercapi/mapping/__init__.py
--rw-r--r--   0        0        0    26607 2023-12-20 23:12:25.683068 mercapi-0.4.0/mercapi/mapping/definitions.py
--rw-r--r--   0        0        0     7487 2023-12-20 23:12:25.683068 mercapi-0.4.0/mercapi/mercapi.py
--rw-r--r--   0        0        0      111 2023-12-20 23:12:25.683068 mercapi-0.4.0/mercapi/models/__init__.py
--rw-r--r--   0        0        0     2380 2023-12-20 23:12:25.683068 mercapi-0.4.0/mercapi/models/base.py
--rw-r--r--   0        0        0      633 2023-12-20 23:12:25.683068 mercapi-0.4.0/mercapi/models/common.py
--rw-r--r--   0        0        0       23 2023-12-20 23:12:25.683068 mercapi-0.4.0/mercapi/models/item/__init__.py
--rw-r--r--   0        0        0     1608 2023-12-20 23:12:25.683068 mercapi-0.4.0/mercapi/models/item/data.py
--rw-r--r--   0        0        0     1602 2023-12-20 23:12:25.683068 mercapi-0.4.0/mercapi/models/item/item.py
--rw-r--r--   0        0        0       54 2023-12-20 23:12:25.683068 mercapi-0.4.0/mercapi/models/profile/__init__.py
--rw-r--r--   0        0        0      890 2023-12-20 23:12:25.683068 mercapi-0.4.0/mercapi/models/profile/items.py
--rw-r--r--   0        0        0     1091 2023-12-20 23:12:25.683068 mercapi-0.4.0/mercapi/models/profile/profile.py
--rw-r--r--   0        0        0      114 2023-12-20 23:12:25.683068 mercapi-0.4.0/mercapi/models/search/__init__.py
--rw-r--r--   0        0        0      190 2023-12-20 23:12:25.683068 mercapi-0.4.0/mercapi/models/search/meta.py
--rw-r--r--   0        0        0      696 2023-12-20 23:12:25.683068 mercapi-0.4.0/mercapi/models/search/search_result_item.py
--rw-r--r--   0        0        0     1285 2023-12-20 23:12:25.683068 mercapi-0.4.0/mercapi/models/search/search_results.py
--rw-r--r--   0        0        0       68 2023-12-20 23:12:25.683068 mercapi-0.4.0/mercapi/requests/__init__.py
--rw-r--r--   0        0        0       28 2023-12-20 23:12:25.683068 mercapi-0.4.0/mercapi/requests/base.py
--rw-r--r--   0        0        0     4016 2023-12-20 23:12:25.683068 mercapi-0.4.0/mercapi/requests/search.py
--rw-r--r--   0        0        0        0 2023-12-20 23:12:25.683068 mercapi-0.4.0/mercapi/util/__init__.py
--rw-r--r--   0        0        0      152 2023-12-20 23:12:25.683068 mercapi-0.4.0/mercapi/util/errors.py
--rw-r--r--   0        0        0      798 2023-12-20 23:12:25.683068 mercapi-0.4.0/mercapi/util/jwt.py
--rw-r--r--   0        0        0      854 2023-12-20 23:12:25.687068 mercapi-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2362 1970-01-01 00:00:00.000000 mercapi-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-16 19:14:53.195426 mercapi-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1473 2024-04-16 19:14:53.195426 mercapi-0.4.1/README.md
+-rw-r--r--   0        0        0       63 2024-04-16 19:14:53.207426 mercapi-0.4.1/mercapi/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-16 19:14:53.207426 mercapi-0.4.1/mercapi/mapping/__init__.py
+-rw-r--r--   0        0        0    26607 2024-04-16 19:14:53.207426 mercapi-0.4.1/mercapi/mapping/definitions.py
+-rw-r--r--   0        0        0     7487 2024-04-16 19:14:53.207426 mercapi-0.4.1/mercapi/mercapi.py
+-rw-r--r--   0        0        0      111 2024-04-16 19:14:53.207426 mercapi-0.4.1/mercapi/models/__init__.py
+-rw-r--r--   0        0        0     2380 2024-04-16 19:14:53.207426 mercapi-0.4.1/mercapi/models/base.py
+-rw-r--r--   0        0        0      633 2024-04-16 19:14:53.207426 mercapi-0.4.1/mercapi/models/common.py
+-rw-r--r--   0        0        0       23 2024-04-16 19:14:53.207426 mercapi-0.4.1/mercapi/models/item/__init__.py
+-rw-r--r--   0        0        0     1608 2024-04-16 19:14:53.207426 mercapi-0.4.1/mercapi/models/item/data.py
+-rw-r--r--   0        0        0     1602 2024-04-16 19:14:53.207426 mercapi-0.4.1/mercapi/models/item/item.py
+-rw-r--r--   0        0        0       54 2024-04-16 19:14:53.207426 mercapi-0.4.1/mercapi/models/profile/__init__.py
+-rw-r--r--   0        0        0      910 2024-04-16 19:14:53.207426 mercapi-0.4.1/mercapi/models/profile/items.py
+-rw-r--r--   0        0        0     1091 2024-04-16 19:14:53.207426 mercapi-0.4.1/mercapi/models/profile/profile.py
+-rw-r--r--   0        0        0      114 2024-04-16 19:14:53.207426 mercapi-0.4.1/mercapi/models/search/__init__.py
+-rw-r--r--   0        0        0      190 2024-04-16 19:14:53.207426 mercapi-0.4.1/mercapi/models/search/meta.py
+-rw-r--r--   0        0        0      696 2024-04-16 19:14:53.207426 mercapi-0.4.1/mercapi/models/search/search_result_item.py
+-rw-r--r--   0        0        0     1285 2024-04-16 19:14:53.207426 mercapi-0.4.1/mercapi/models/search/search_results.py
+-rw-r--r--   0        0        0       68 2024-04-16 19:14:53.207426 mercapi-0.4.1/mercapi/requests/__init__.py
+-rw-r--r--   0        0        0       28 2024-04-16 19:14:53.207426 mercapi-0.4.1/mercapi/requests/base.py
+-rw-r--r--   0        0        0     4020 2024-04-16 19:14:53.207426 mercapi-0.4.1/mercapi/requests/search.py
+-rw-r--r--   0        0        0        0 2024-04-16 19:14:53.207426 mercapi-0.4.1/mercapi/util/__init__.py
+-rw-r--r--   0        0        0      148 2024-04-16 19:14:53.207426 mercapi-0.4.1/mercapi/util/errors.py
+-rw-r--r--   0        0        0      798 2024-04-16 19:14:53.207426 mercapi-0.4.1/mercapi/util/jwt.py
+-rw-r--r--   0        0        0      854 2024-04-16 19:14:53.207426 mercapi-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2362 1970-01-01 00:00:00.000000 mercapi-0.4.1/PKG-INFO
```

### Comparing `mercapi-0.4.0/LICENSE` & `mercapi-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mercapi-0.4.0/README.md` & `mercapi-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `mercapi-0.4.0/mercapi/mapping/definitions.py` & `mercapi-0.4.1/mercapi/mapping/definitions.py`

 * *Files identical despite different names*

### Comparing `mercapi-0.4.0/mercapi/mercapi.py` & `mercapi-0.4.1/mercapi/mercapi.py`

 * *Files identical despite different names*

### Comparing `mercapi-0.4.0/mercapi/models/base.py` & `mercapi-0.4.1/mercapi/models/base.py`

 * *Files identical despite different names*

### Comparing `mercapi-0.4.0/mercapi/models/common.py` & `mercapi-0.4.1/mercapi/models/common.py`

 * *Files identical despite different names*

### Comparing `mercapi-0.4.0/mercapi/models/item/data.py` & `mercapi-0.4.1/mercapi/models/item/data.py`

 * *Files identical despite different names*

### Comparing `mercapi-0.4.0/mercapi/models/item/item.py` & `mercapi-0.4.1/mercapi/models/item/item.py`

 * *Files identical despite different names*

### Comparing `mercapi-0.4.0/mercapi/models/profile/items.py` & `mercapi-0.4.1/mercapi/models/profile/items.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass
 from datetime import datetime
-from typing import List
+from typing import List, Optional
 
 from mercapi.models import Item
 from mercapi.models.base import ResponseModel
 from mercapi.models.common import ItemCategorySummary
 from mercapi.models.item.data import ShippingFromArea
 
 
@@ -17,15 +17,15 @@
     price: int
     thumbnails: List[str]
     root_category_id: int
     num_likes: int
     num_comments: int
     created: datetime
     updated: datetime
-    item_category: ItemCategorySummary
+    item_category: Optional[ItemCategorySummary]
     shipping_from_area: ShippingFromArea
 
     async def full_item(self) -> Item:
         """Fetch full details of a listing (item).
 
         Equivalent of :func:`~mercapi.Mercapi.item`
         """
```

### Comparing `mercapi-0.4.0/mercapi/models/profile/profile.py` & `mercapi-0.4.1/mercapi/models/profile/profile.py`

 * *Files identical despite different names*

### Comparing `mercapi-0.4.0/mercapi/models/search/search_result_item.py` & `mercapi-0.4.1/mercapi/models/search/search_result_item.py`

 * *Files identical despite different names*

### Comparing `mercapi-0.4.0/mercapi/models/search/search_results.py` & `mercapi-0.4.1/mercapi/models/search/search_results.py`

 * *Files identical despite different names*

### Comparing `mercapi-0.4.0/mercapi/requests/search.py` & `mercapi-0.4.1/mercapi/requests/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             "searchSessionId": uuid.uuid4().hex,
             "indexRouting": "INDEX_ROUTING_UNSPECIFIED",
             "thumbnailTypes": [],
             "searchCondition": {
                 "keyword": self.search_conditions.query,
                 "sort": self.search_conditions.sort_by.name,
                 "order": self.search_conditions.sort_order.name,
-                "status": [],
+                "status": status,
                 "sizeId": self.search_conditions.sizes,
                 "categoryId": self.search_conditions.categories,
                 "brandId": self.search_conditions.brands,
                 "sellerId": [],
                 "priceMin": self.search_conditions.price_min,
                 "priceMax": self.search_conditions.price_max,
                 "itemConditionId": self.search_conditions.item_conditions,
```

### Comparing `mercapi-0.4.0/mercapi/util/jwt.py` & `mercapi-0.4.1/mercapi/util/jwt.py`

 * *Files identical despite different names*

### Comparing `mercapi-0.4.0/pyproject.toml` & `mercapi-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mercapi"
-version = "0.4.0"
+version = "0.4.1"
 description = "Python API for querying and browsing mercari.jp"
 authors = ["take-kun <109226194+take-kun@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/take-kun/mercapi/"
 keywords = ["api", "scraping"]
```

### Comparing `mercapi-0.4.0/PKG-INFO` & `mercapi-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercapi
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python API for querying and browsing mercari.jp
 Home-page: https://github.com/take-kun/mercapi/
 License: MIT
 Keywords: api,scraping
 Author: take-kun
 Author-email: 109226194+take-kun@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
```

