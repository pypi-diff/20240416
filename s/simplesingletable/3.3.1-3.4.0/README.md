# Comparing `tmp/simplesingletable-3.3.1.tar.gz` & `tmp/simplesingletable-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplesingletable-3.3.1.tar", last modified: Mon Mar 18 21:28:27 2024, max compression
+gzip compressed data, was "simplesingletable-3.4.0.tar", last modified: Mon Apr 15 23:32:33 2024, max compression
```

## Comparing `simplesingletable-3.3.1.tar` & `simplesingletable-3.4.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-03-18 21:28:27.769891 simplesingletable-3.3.1/
--rw-r--r--   0 msull      (501) staff       (20)     1092 2023-10-16 15:46:21.000000 simplesingletable-3.3.1/LICENSE
--rw-r--r--   0 msull      (501) staff       (20)     5813 2024-03-18 21:28:27.769005 simplesingletable-3.3.1/PKG-INFO
--rw-r--r--   0 msull      (501) staff       (20)     3278 2024-03-18 21:28:18.000000 simplesingletable-3.3.1/README.md
--rw-r--r--   0 msull      (501) staff       (20)     1924 2024-03-18 21:28:18.000000 simplesingletable-3.3.1/pyproject.toml
--rw-r--r--   0 msull      (501) staff       (20)       38 2024-03-18 21:28:27.770064 simplesingletable-3.3.1/setup.cfg
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-03-18 21:28:27.751960 simplesingletable-3.3.1/src/
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-03-18 21:28:27.755914 simplesingletable-3.3.1/src/simplesingletable/
--rw-r--r--   0 msull      (501) staff       (20)      288 2024-03-18 21:28:18.000000 simplesingletable-3.3.1/src/simplesingletable/__init__.py
--rw-r--r--   0 msull      (501) staff       (20)    27017 2024-03-05 17:53:28.000000 simplesingletable-3.3.1/src/simplesingletable/dynamodb_memory.py
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-03-18 21:28:27.761314 simplesingletable-3.3.1/src/simplesingletable/extras/
--rw-r--r--   0 msull      (501) staff       (20)        0 2024-02-12 18:26:56.000000 simplesingletable-3.3.1/src/simplesingletable/extras/__init__.py
--rw-r--r--   0 msull      (501) staff       (20)    20458 2024-03-18 19:15:13.000000 simplesingletable-3.3.1/src/simplesingletable/extras/form_data.py
--rw-r--r--   0 msull      (501) staff       (20)     1704 2024-02-12 19:18:43.000000 simplesingletable-3.3.1/src/simplesingletable/extras/singleton.py
--rw-r--r--   0 msull      (501) staff       (20)    12772 2024-03-18 18:58:28.000000 simplesingletable-3.3.1/src/simplesingletable/models.py
--rw-r--r--   0 msull      (501) staff       (20)     5351 2024-03-05 17:53:29.000000 simplesingletable-3.3.1/src/simplesingletable/utils.py
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-03-18 21:28:27.764928 simplesingletable-3.3.1/src/simplesingletable.egg-info/
--rw-r--r--   0 msull      (501) staff       (20)     5813 2024-03-18 21:28:27.000000 simplesingletable-3.3.1/src/simplesingletable.egg-info/PKG-INFO
--rw-r--r--   0 msull      (501) staff       (20)      664 2024-03-18 21:28:27.000000 simplesingletable-3.3.1/src/simplesingletable.egg-info/SOURCES.txt
--rw-r--r--   0 msull      (501) staff       (20)        1 2024-03-18 21:28:27.000000 simplesingletable-3.3.1/src/simplesingletable.egg-info/dependency_links.txt
--rw-r--r--   0 msull      (501) staff       (20)      214 2024-03-18 21:28:27.000000 simplesingletable-3.3.1/src/simplesingletable.egg-info/requires.txt
--rw-r--r--   0 msull      (501) staff       (20)       32 2024-03-18 21:28:27.000000 simplesingletable-3.3.1/src/simplesingletable.egg-info/top_level.txt
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-03-18 21:28:27.762025 simplesingletable-3.3.1/src/streamlit_app/
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-03-18 21:28:27.762721 simplesingletable-3.3.1/src/streamlit_app/pages/
--rw-r--r--   0 msull      (501) staff       (20)    13081 2024-03-18 19:07:04.000000 simplesingletable-3.3.1/src/streamlit_app/pages/Form Data demo.py
--rw-r--r--   0 msull      (501) staff       (20)     7517 2024-02-23 20:37:38.000000 simplesingletable-3.3.1/src/streamlit_app/streamlit_app.py
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-03-18 21:28:27.763972 simplesingletable-3.3.1/tests/
--rw-r--r--   0 msull      (501) staff       (20)     1091 2024-02-23 20:37:38.000000 simplesingletable-3.3.1/tests/test_nonversioned_resource.py
--rw-r--r--   0 msull      (501) staff       (20)     8675 2024-02-23 20:37:38.000000 simplesingletable-3.3.1/tests/test_simplesingletable.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-04-15 23:32:33.181650 simplesingletable-3.4.0/
+-rw-r--r--   0 msull      (501) staff       (20)     1092 2023-10-16 15:46:21.000000 simplesingletable-3.4.0/LICENSE
+-rw-r--r--   0 msull      (501) staff       (20)     5813 2024-04-15 23:32:33.181190 simplesingletable-3.4.0/PKG-INFO
+-rw-r--r--   0 msull      (501) staff       (20)     3278 2024-04-15 23:32:25.000000 simplesingletable-3.4.0/README.md
+-rw-r--r--   0 msull      (501) staff       (20)     1924 2024-04-15 23:32:25.000000 simplesingletable-3.4.0/pyproject.toml
+-rw-r--r--   0 msull      (501) staff       (20)       38 2024-04-15 23:32:33.181772 simplesingletable-3.4.0/setup.cfg
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-04-15 23:32:33.169162 simplesingletable-3.4.0/src/
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-04-15 23:32:33.173403 simplesingletable-3.4.0/src/simplesingletable/
+-rw-r--r--   0 msull      (501) staff       (20)      288 2024-04-15 23:32:25.000000 simplesingletable-3.4.0/src/simplesingletable/__init__.py
+-rw-r--r--   0 msull      (501) staff       (20)    27017 2024-04-08 19:04:26.000000 simplesingletable-3.4.0/src/simplesingletable/dynamodb_memory.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-04-15 23:32:33.176031 simplesingletable-3.4.0/src/simplesingletable/extras/
+-rw-r--r--   0 msull      (501) staff       (20)        0 2024-02-12 18:26:56.000000 simplesingletable-3.4.0/src/simplesingletable/extras/__init__.py
+-rw-r--r--   0 msull      (501) staff       (20)    21742 2024-04-15 23:25:08.000000 simplesingletable-3.4.0/src/simplesingletable/extras/form_data.py
+-rw-r--r--   0 msull      (501) staff       (20)     1704 2024-02-12 19:18:43.000000 simplesingletable-3.4.0/src/simplesingletable/extras/singleton.py
+-rw-r--r--   0 msull      (501) staff       (20)    12772 2024-03-18 18:58:28.000000 simplesingletable-3.4.0/src/simplesingletable/models.py
+-rw-r--r--   0 msull      (501) staff       (20)     5351 2024-03-05 17:53:29.000000 simplesingletable-3.4.0/src/simplesingletable/utils.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-04-15 23:32:33.178819 simplesingletable-3.4.0/src/simplesingletable.egg-info/
+-rw-r--r--   0 msull      (501) staff       (20)     5813 2024-04-15 23:32:33.000000 simplesingletable-3.4.0/src/simplesingletable.egg-info/PKG-INFO
+-rw-r--r--   0 msull      (501) staff       (20)      664 2024-04-15 23:32:33.000000 simplesingletable-3.4.0/src/simplesingletable.egg-info/SOURCES.txt
+-rw-r--r--   0 msull      (501) staff       (20)        1 2024-04-15 23:32:33.000000 simplesingletable-3.4.0/src/simplesingletable.egg-info/dependency_links.txt
+-rw-r--r--   0 msull      (501) staff       (20)      214 2024-04-15 23:32:33.000000 simplesingletable-3.4.0/src/simplesingletable.egg-info/requires.txt
+-rw-r--r--   0 msull      (501) staff       (20)       32 2024-04-15 23:32:33.000000 simplesingletable-3.4.0/src/simplesingletable.egg-info/top_level.txt
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-04-15 23:32:33.176354 simplesingletable-3.4.0/src/streamlit_app/
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-04-15 23:32:33.176763 simplesingletable-3.4.0/src/streamlit_app/pages/
+-rw-r--r--   0 msull      (501) staff       (20)    13081 2024-03-18 19:07:04.000000 simplesingletable-3.4.0/src/streamlit_app/pages/Form Data demo.py
+-rw-r--r--   0 msull      (501) staff       (20)     7517 2024-02-23 20:37:38.000000 simplesingletable-3.4.0/src/streamlit_app/streamlit_app.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-04-15 23:32:33.177885 simplesingletable-3.4.0/tests/
+-rw-r--r--   0 msull      (501) staff       (20)     1091 2024-02-23 20:37:38.000000 simplesingletable-3.4.0/tests/test_nonversioned_resource.py
+-rw-r--r--   0 msull      (501) staff       (20)     9155 2024-04-08 19:12:12.000000 simplesingletable-3.4.0/tests/test_simplesingletable.py
```

### Comparing `simplesingletable-3.3.1/LICENSE` & `simplesingletable-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simplesingletable-3.3.1/PKG-INFO` & `simplesingletable-3.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplesingletable
-Version: 3.3.1
+Version: 3.4.0
 Summary: A simple boto3/Pydantic implementation of DynamoDB Single Table Design and related utilities.
 Author-email: Sully <sully@sadburger.com>
 License: The MIT License (MIT)
         Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -42,15 +42,15 @@
 Requires-Dist: watchdog; extra == "dev"
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
 Requires-Dist: twine; extra == "build"
 
 # Simple Single Table
 
-**Latest Version:** 3.3.1
+**Latest Version:** 3.4.0
 
 **simplesingletable** is a Python library that offers an abstraction layer for AWS DynamoDB operations, particularly for
 those tables using single-table design. It uses Pydantic to define the models, and tries to be as "batteries-included"
 based on how I personally have come to use DynamoDb.
 
 I've used and written variations of this same code many times, and finally decided to try and package it all up into a
 single library I could pip install and use whenever I needed cheap, easy, fast storage with few access patterns. So far
```

### Comparing `simplesingletable-3.3.1/README.md` & `simplesingletable-3.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Simple Single Table
 
-**Latest Version:** 3.3.1
+**Latest Version:** 3.4.0
 
 **simplesingletable** is a Python library that offers an abstraction layer for AWS DynamoDB operations, particularly for
 those tables using single-table design. It uses Pydantic to define the models, and tries to be as "batteries-included"
 based on how I personally have come to use DynamoDb.
 
 I've used and written variations of this same code many times, and finally decided to try and package it all up into a
 single library I could pip install and use whenever I needed cheap, easy, fast storage with few access patterns. So far
```

### Comparing `simplesingletable-3.3.1/pyproject.toml` & `simplesingletable-3.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "simplesingletable"
-version = "3.3.1"
+version = "3.4.0"
 description = "A simple boto3/Pydantic implementation of DynamoDB Single Table Design and related utilities."
 readme = "README.md"
 authors = [{ name = "Sully", email = "sully@sadburger.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -57,15 +57,15 @@
 line-length = 120
 
 [tool.ruff]
 line-length = 120
 target-version = "py310"
 
 [tool.bumpver]
-current_version = "3.3.1"
+current_version = "3.4.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `simplesingletable-3.3.1/src/simplesingletable/dynamodb_memory.py` & `simplesingletable-3.4.0/src/simplesingletable/dynamodb_memory.py`

 * *Files identical despite different names*

### Comparing `simplesingletable-3.3.1/src/simplesingletable/extras/form_data.py` & `simplesingletable-3.4.0/src/simplesingletable/extras/form_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,14 +194,48 @@
             filter_fn=filter_fn,
             results_limit=results_limit,
             max_api_calls=max_api_calls,
             pagination_key=pagination_key,
             ascending=ascending,
         )
 
+    def db_get_gsi2pk(self) -> str | None:
+        """Utilize gsi2 to track all Form entries for a particular group / row identifier, allowing efficient retrieval
+        of a specific row's worth of data."""
+        return f"{self.get_unique_key_prefix()}#{self.resource_id}#{self.group_identifier}#{self.row_identifier}"
+
+    @classmethod
+    def retrieve_all_entries_for_row(
+        cls,
+        memory: DynamoDbMemory,
+        existing_form: Form,
+        *,
+        group_identifier: str,
+        row_identifier: str,
+        filter_fn: Optional[Callable[[AnyDbResource], bool]] = None,
+        results_limit: Optional[int] = 1000,
+        max_api_calls: int = 10,
+        pagination_key: Optional[str] = None,
+        ascending=False,
+    ) -> PaginatedList["FormEntry"]:
+        key = f"{cls.get_unique_key_prefix()}#{existing_form.resource_id}#{group_identifier}#{row_identifier}"
+
+        condition = Key("gsi2pk").eq(key)
+
+        return memory.paginated_dynamodb_query(
+            key_condition=condition,
+            index_name="gsi2",
+            resource_class=cls,
+            filter_fn=filter_fn,
+            results_limit=results_limit,
+            max_api_calls=max_api_calls,
+            pagination_key=pagination_key,
+            ascending=ascending,
+        )
+
 
 class FormDataRow(Mapping):
     def __init__(
         self,
         form: Form,
         form_manager: "FormDataManager",
         group: str,
```

### Comparing `simplesingletable-3.3.1/src/simplesingletable/extras/singleton.py` & `simplesingletable-3.4.0/src/simplesingletable/extras/singleton.py`

 * *Files identical despite different names*

### Comparing `simplesingletable-3.3.1/src/simplesingletable/models.py` & `simplesingletable-3.4.0/src/simplesingletable/models.py`

 * *Files identical despite different names*

### Comparing `simplesingletable-3.3.1/src/simplesingletable/utils.py` & `simplesingletable-3.4.0/src/simplesingletable/utils.py`

 * *Files identical despite different names*

### Comparing `simplesingletable-3.3.1/src/simplesingletable.egg-info/PKG-INFO` & `simplesingletable-3.4.0/src/simplesingletable.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplesingletable
-Version: 3.3.1
+Version: 3.4.0
 Summary: A simple boto3/Pydantic implementation of DynamoDB Single Table Design and related utilities.
 Author-email: Sully <sully@sadburger.com>
 License: The MIT License (MIT)
         Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -42,15 +42,15 @@
 Requires-Dist: watchdog; extra == "dev"
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
 Requires-Dist: twine; extra == "build"
 
 # Simple Single Table
 
-**Latest Version:** 3.3.1
+**Latest Version:** 3.4.0
 
 **simplesingletable** is a Python library that offers an abstraction layer for AWS DynamoDB operations, particularly for
 those tables using single-table design. It uses Pydantic to define the models, and tries to be as "batteries-included"
 based on how I personally have come to use DynamoDb.
 
 I've used and written variations of this same code many times, and finally decided to try and package it all up into a
 single library I could pip install and use whenever I needed cheap, easy, fast storage with few access patterns. So far
```

### Comparing `simplesingletable-3.3.1/src/simplesingletable.egg-info/SOURCES.txt` & `simplesingletable-3.4.0/src/simplesingletable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `simplesingletable-3.3.1/src/streamlit_app/pages/Form Data demo.py` & `simplesingletable-3.4.0/src/streamlit_app/pages/Form Data demo.py`

 * *Files identical despite different names*

### Comparing `simplesingletable-3.3.1/src/streamlit_app/streamlit_app.py` & `simplesingletable-3.4.0/src/streamlit_app/streamlit_app.py`

 * *Files identical despite different names*

### Comparing `simplesingletable-3.3.1/tests/test_nonversioned_resource.py` & `simplesingletable-3.4.0/tests/test_nonversioned_resource.py`

 * *Files identical despite different names*

### Comparing `simplesingletable-3.3.1/tests/test_simplesingletable.py` & `simplesingletable-3.4.0/tests/test_simplesingletable.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 from datetime import datetime, timedelta, timezone
 
 import ulid
 from boto3.dynamodb.conditions import Key
+from pydantic import BaseModel
+
 from simplesingletable import DynamoDbMemory, DynamoDbVersionedResource, DynamoDbResource
 from simplesingletable.utils import generate_date_sortable_id
 
 
 class MyNonversionedTestResource(DynamoDbResource):
     name: str
 
     def db_get_gsi1pk(self) -> str | None:
         return f"parent_id#{self.parent_id}"
 
 
+class PydanticAttributeTest(BaseModel):
+    attribute_name: str = "default_attribute_name"
+
+
 class MyVersionedTestResource(DynamoDbVersionedResource):
     some_field: str
     bool_field: bool
     list_of_things: list[str | int | bool | float]
     parent_id: str
+    inner_class: PydanticAttributeTest
 
     def db_get_gsi1pk(self) -> str | None:
         return f"parent_id#{self.parent_id}"
 
 
 def test_date_id(mocker):
     # Mock datetime.utcnow to return a specific datetime
@@ -41,14 +48,15 @@
         MyVersionedTestResource,
         {
             "parent_id": "parent1",
             "some_field": "test",
             "bool_field": True,
             # multiple types in the list
             "list_of_things": ["a", False, 1, 1.2],
+            "inner_class": PydanticAttributeTest(),
         },
     )
     assert dynamodb_memory.read_existing(resource.resource_id, MyVersionedTestResource) == resource
 
     resource_ulid = resource.resource_id_as_ulid()
     assert id_before_create.timestamp() <= resource_ulid.timestamp()
 
@@ -71,27 +79,29 @@
     new_resource_1 = dynamodb_memory.create_new(
         MyVersionedTestResource,
         {
             "parent_id": "parent1",
             "some_field": "test",
             "bool_field": True,
             "list_of_things": [],
+            "inner_class": PydanticAttributeTest(),
         },
     )
     assert dynamodb_memory.read_existing(new_resource_1.resource_id, MyVersionedTestResource) == new_resource_1
 
     # create a second resource with the same parent
     _incr_time()
     new_resource_2 = dynamodb_memory.create_new(
         MyVersionedTestResource,
         {
             "parent_id": "parent1",
             "some_field": "test",
             "bool_field": False,
             "list_of_things": ["adsf"],
+            "inner_class": PydanticAttributeTest(),
         },
     )
 
     def _q(pid, limit=10, pagination_key=None, ascending=True):
         return dynamodb_memory.paginated_dynamodb_query(
             resource_class=MyVersionedTestResource,
             index_name="gsi1",
@@ -116,14 +126,15 @@
     new_resource_3 = dynamodb_memory.create_new(
         MyVersionedTestResource,
         {
             "parent_id": "parent2",
             "some_field": "test",
             "bool_field": True,
             "list_of_things": [1, 2, 3],
+            "inner_class": PydanticAttributeTest(),
         },
     )
 
     # first parent id unchanged
     assert _q(new_resource_1.parent_id) == [new_resource_1, new_resource_2]
 
     assert _q(new_resource_3.parent_id) == [new_resource_3]
@@ -186,26 +197,28 @@
         dynamodb_memory.create_new(
             MyVersionedTestResource,
             {
                 "parent_id": "parent1",
                 "some_field": "test",
                 "bool_field": True,
                 "list_of_things": [],
+                "inner_class": PydanticAttributeTest(),
             },
         )
 
     # one false after
     _incr_time()
     match_item = dynamodb_memory.create_new(
         MyVersionedTestResource,
         {
             "parent_id": "parent1",
             "some_field": "test",
             "bool_field": False,
             "list_of_things": [],
+            "inner_class": PydanticAttributeTest(),
         },
     )
 
     # use a server side filter (rather than a dynamodb filter), which operates on
     # the decoded dynamodb object wherever the code is running
     def _filter(x: MyVersionedTestResource) -> bool:
         # find the one that after the ten
```

