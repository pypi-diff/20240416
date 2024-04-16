# Comparing `tmp/pymonday-2.1.1.tar.gz` & `tmp/pymonday-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymonday-2.1.1.tar", last modified: Mon Feb 26 12:59:20 2024, max compression
+gzip compressed data, was "pymonday-2.1.2.tar", last modified: Tue Apr 16 14:58:52 2024, max compression
```

## Comparing `pymonday-2.1.1.tar` & `pymonday-2.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-02-26 12:59:20.184617 pymonday-2.1.1/
--rw-rw-rw-   0        0        0    35823 2024-02-26 11:34:44.000000 pymonday-2.1.1/LICENSE
--rw-rw-rw-   0        0        0      344 2024-02-26 12:59:20.183617 pymonday-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      112 2024-02-26 12:54:28.000000 pymonday-2.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-02-26 12:59:20.173112 pymonday-2.1.1/pymonday/
--rw-rw-rw-   0        0        0       56 2024-02-26 11:40:39.000000 pymonday-2.1.1/pymonday/__init__.py
--rw-rw-rw-   0        0        0     1259 2024-02-26 11:40:48.000000 pymonday-2.1.1/pymonday/columns.py
--rw-rw-rw-   0        0        0    47342 2024-02-26 11:54:59.000000 pymonday-2.1.1/pymonday/monday_api_client.py
-drwxrwxrwx   0        0        0        0 2024-02-26 12:59:20.182117 pymonday-2.1.1/pymonday.egg-info/
--rw-rw-rw-   0        0        0      344 2024-02-26 12:59:20.000000 pymonday-2.1.1/pymonday.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2024-02-26 12:59:20.000000 pymonday-2.1.1/pymonday.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-26 12:59:20.000000 pymonday-2.1.1/pymonday.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-02-26 12:59:20.000000 pymonday-2.1.1/pymonday.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-02-26 12:59:20.000000 pymonday-2.1.1/pymonday.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-26 12:59:20.184617 pymonday-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0      451 2024-02-26 12:59:12.000000 pymonday-2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 14:58:52.128334 pymonday-2.1.2/
+-rw-rw-rw-   0        0        0    35823 2024-02-26 11:34:44.000000 pymonday-2.1.2/LICENSE
+-rw-rw-rw-   0        0        0      344 2024-04-16 14:58:52.127334 pymonday-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      112 2024-02-26 12:54:28.000000 pymonday-2.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 14:58:52.115832 pymonday-2.1.2/pymonday/
+-rw-rw-rw-   0        0        0       56 2024-02-26 11:40:39.000000 pymonday-2.1.2/pymonday/__init__.py
+-rw-rw-rw-   0        0        0     1259 2024-02-26 11:40:48.000000 pymonday-2.1.2/pymonday/columns.py
+-rw-rw-rw-   0        0        0    48791 2024-04-16 14:54:25.000000 pymonday-2.1.2/pymonday/monday_api_client.py
+drwxrwxrwx   0        0        0        0 2024-04-16 14:58:52.125834 pymonday-2.1.2/pymonday.egg-info/
+-rw-rw-rw-   0        0        0      344 2024-04-16 14:58:52.000000 pymonday-2.1.2/pymonday.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2024-04-16 14:58:52.000000 pymonday-2.1.2/pymonday.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 14:58:52.000000 pymonday-2.1.2/pymonday.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-04-16 14:58:52.000000 pymonday-2.1.2/pymonday.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-16 14:58:52.000000 pymonday-2.1.2/pymonday.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 14:58:52.128834 pymonday-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      451 2024-04-16 14:56:38.000000 pymonday-2.1.2/setup.py
```

### Comparing `pymonday-2.1.1/LICENSE` & `pymonday-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymonday-2.1.1/pymonday/columns.py` & `pymonday-2.1.2/pymonday/columns.py`

 * *Files identical despite different names*

### Comparing `pymonday-2.1.1/pymonday/monday_api_client.py` & `pymonday-2.1.2/pymonday/monday_api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -726,14 +726,41 @@
         cursor = response['data']['boards'][0]['groups'][0]['items_page']['cursor']
         if cursor is None:
             return items
         all_items = self.__get_next_page(cursor, items, item_attributes)
         return all_items
 
     ####################################################################################################################
+    def get_items_with_status(self, board_id, group_id, columns, column_id, index_value):
+        column_string = ""
+        for column in columns:
+            column_string = column_string + f"\"{column}\", "
+        column_string = column_string[:-2]
+        column_string = f"[{column_string}]"
+        item_attributes = f'''name id parent_item{{id name }} column_values(ids: {column_string}) {{text value
+        column{{id title}}
+        ... on BoardRelationValue {{display_value linked_items {{id}}}}
+        ... on MirrorValue {{display_value}}}}'''
+
+        initial_query = f'''{{boards(ids: {board_id}) {{groups(ids: "{group_id}") {{items_page(limit: 100 
+        query_params: {{rules: {{column_id: "{column_id}", compare_value: [{index_value}]}}}}) {{
+        cursor
+        items {{{item_attributes}}}}}}}}}}}'''
+        data = {'query': initial_query}
+        response = self.__send_post_request(data)
+        if not response:
+            return None
+        items = [item for item in response['data']['boards'][0]['groups'][0]['items_page']['items']]
+        cursor = response['data']['boards'][0]['groups'][0]['items_page']['cursor']
+        if cursor is None:
+            return items
+        all_items = self.__get_next_page(cursor, items, item_attributes)
+        return all_items
+
+    ####################################################################################################################
     def get_item_ids_between_dates(self, board_id, group_id, column_id, start_date, end_date):
         """
         Get Item IDs between a specified date range. Supports Timeline columns and start dates.
         :param board_id: UUID of the board the items are on.
         :param group_id: UUID of the group the items are in.
         :param column_id: UUID of the timeline column to filter on.
         :param start_date: Start of date range.
```

