# Comparing `tmp/ministryofjustice_data_platform_catalogue-0.8.1.tar.gz` & `tmp/ministryofjustice_data_platform_catalogue-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ministryofjustice_data_platform_catalogue-0.8.1.tar", max compression
+gzip compressed data, was "ministryofjustice_data_platform_catalogue-0.9.0.tar", max compression
```

## Comparing `ministryofjustice_data_platform_catalogue-0.8.1.tar` & `ministryofjustice_data_platform_catalogue-0.9.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     3500 2024-01-30 14:26:50.292644 ministryofjustice_data_platform_catalogue-0.8.1/README.md
--rw-r--r--   0        0        0      213 2024-01-30 14:26:50.292644 ministryofjustice_data_platform_catalogue-0.8.1/data_platform_catalogue/__init__.py
--rw-r--r--   0        0        0      155 2024-01-30 14:26:50.292644 ministryofjustice_data_platform_catalogue-0.8.1/data_platform_catalogue/client/__init__.py
--rw-r--r--   0        0        0     2266 2024-01-30 14:26:50.292644 ministryofjustice_data_platform_catalogue-0.8.1/data_platform_catalogue/client/base.py
--rw-r--r--   0        0        0       65 2024-01-30 14:26:50.292644 ministryofjustice_data_platform_catalogue-0.8.1/data_platform_catalogue/client/datahub/__init__.py
--rw-r--r--   0        0        0    12945 2024-01-30 14:26:50.292644 ministryofjustice_data_platform_catalogue-0.8.1/data_platform_catalogue/client/datahub/datahub_client.py
--rw-r--r--   0        0        0        0 2024-01-30 14:26:50.292644 ministryofjustice_data_platform_catalogue-0.8.1/data_platform_catalogue/client/datahub/graphql/__init__.py
--rw-r--r--   0        0        0      694 2024-01-30 14:26:50.292644 ministryofjustice_data_platform_catalogue-0.8.1/data_platform_catalogue/client/datahub/graphql/facets.graphql
--rw-r--r--   0        0        0     3806 2024-01-30 14:26:50.292644 ministryofjustice_data_platform_catalogue-0.8.1/data_platform_catalogue/client/datahub/graphql/search.graphql
--rw-r--r--   0        0        0     9074 2024-01-30 14:26:50.292644 ministryofjustice_data_platform_catalogue-0.8.1/data_platform_catalogue/client/datahub/search.py
--rw-r--r--   0        0        0     8548 2024-01-30 14:26:50.292644 ministryofjustice_data_platform_catalogue-0.8.1/data_platform_catalogue/client/openmetadata.py
--rw-r--r--   0        0        0     2817 2024-01-30 14:26:50.292644 ministryofjustice_data_platform_catalogue-0.8.1/data_platform_catalogue/entities.py
--rw-r--r--   0        0        0     1899 2024-01-30 14:26:50.292644 ministryofjustice_data_platform_catalogue-0.8.1/data_platform_catalogue/search_types.py
--rw-r--r--   0        0        0      701 2024-01-30 14:26:50.296644 ministryofjustice_data_platform_catalogue-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     4298 1970-01-01 00:00:00.000000 ministryofjustice_data_platform_catalogue-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     3563 2024-01-31 14:30:25.336914 ministryofjustice_data_platform_catalogue-0.9.0/README.md
+-rw-r--r--   0        0        0      213 2024-01-31 14:30:25.336914 ministryofjustice_data_platform_catalogue-0.9.0/data_platform_catalogue/__init__.py
+-rw-r--r--   0        0        0      155 2024-01-31 14:30:25.336914 ministryofjustice_data_platform_catalogue-0.9.0/data_platform_catalogue/client/__init__.py
+-rw-r--r--   0        0        0     2343 2024-01-31 14:30:25.336914 ministryofjustice_data_platform_catalogue-0.9.0/data_platform_catalogue/client/base.py
+-rw-r--r--   0        0        0       65 2024-01-31 14:30:25.336914 ministryofjustice_data_platform_catalogue-0.9.0/data_platform_catalogue/client/datahub/__init__.py
+-rw-r--r--   0        0        0    13045 2024-01-31 14:30:25.336914 ministryofjustice_data_platform_catalogue-0.9.0/data_platform_catalogue/client/datahub/datahub_client.py
+-rw-r--r--   0        0        0        0 2024-01-31 14:30:25.336914 ministryofjustice_data_platform_catalogue-0.9.0/data_platform_catalogue/client/datahub/graphql/__init__.py
+-rw-r--r--   0        0        0      694 2024-01-31 14:30:25.336914 ministryofjustice_data_platform_catalogue-0.9.0/data_platform_catalogue/client/datahub/graphql/facets.graphql
+-rw-r--r--   0        0        0     3854 2024-01-31 14:30:25.336914 ministryofjustice_data_platform_catalogue-0.9.0/data_platform_catalogue/client/datahub/graphql/search.graphql
+-rw-r--r--   0        0        0     9202 2024-01-31 14:30:25.336914 ministryofjustice_data_platform_catalogue-0.9.0/data_platform_catalogue/client/datahub/search.py
+-rw-r--r--   0        0        0     8548 2024-01-31 14:30:25.336914 ministryofjustice_data_platform_catalogue-0.9.0/data_platform_catalogue/client/openmetadata.py
+-rw-r--r--   0        0        0     2817 2024-01-31 14:30:25.336914 ministryofjustice_data_platform_catalogue-0.9.0/data_platform_catalogue/entities.py
+-rw-r--r--   0        0        0     2224 2024-01-31 14:30:25.336914 ministryofjustice_data_platform_catalogue-0.9.0/data_platform_catalogue/search_types.py
+-rw-r--r--   0        0        0      701 2024-01-31 14:30:25.336914 ministryofjustice_data_platform_catalogue-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4361 1970-01-01 00:00:00.000000 ministryofjustice_data_platform_catalogue-0.9.0/PKG-INFO
```

### Comparing `ministryofjustice_data_platform_catalogue-0.8.1/README.md` & `ministryofjustice_data_platform_catalogue-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -84,16 +84,19 @@
 
 # Iterate over facet options
 for option in response.facets.options('domains'):
   print(option.label)
   print(option.value)
   print(option.count)
 
-# Include a filter
-client.search(filters=[MultiSelectFilter("domains", [response.facets['domains'][0].value])])
+# Include a filter and sort
+client.search(
+  filters=[MultiSelectFilter("domains", [response.facets['domains'][0].value])],
+  sort=SortOption(field="name", ascending=False)
+)
 ```
 
 ## Search filters
 
 ### Datahub
 
 Basic filters:
```

### Comparing `ministryofjustice_data_platform_catalogue-0.8.1/data_platform_catalogue/client/base.py` & `ministryofjustice_data_platform_catalogue-0.9.0/data_platform_catalogue/client/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,21 @@
 
 from ..entities import (
     CatalogueMetadata,
     DataLocation,
     DataProductMetadata,
     TableMetadata,
 )
-from ..search_types import MultiSelectFilter, ResultType, SearchFacets, SearchResponse
+from ..search_types import (
+    MultiSelectFilter,
+    ResultType,
+    SearchFacets,
+    SearchResponse,
+    SortOption,
+)
 
 logger = logging.getLogger(__name__)
 
 
 class CatalogueError(Exception):
     """
     Base class for all errors.
@@ -62,14 +68,15 @@
         count: int = 20,
         page: str | None = None,
         result_types: Sequence[ResultType] = (
             ResultType.DATA_PRODUCT,
             ResultType.TABLE,
         ),
         filters: Sequence[MultiSelectFilter] = (),
+        sort: SortOption | None = None,
     ) -> SearchResponse:
         """
         Wraps the catalogue's search function.
         """
         raise NotImplementedError
 
     def search_facets(
```

### Comparing `ministryofjustice_data_platform_catalogue-0.8.1/data_platform_catalogue/client/datahub/datahub_client.py` & `ministryofjustice_data_platform_catalogue-0.9.0/data_platform_catalogue/client/datahub/datahub_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,21 @@
 
 from ...entities import (
     CatalogueMetadata,
     DataLocation,
     DataProductMetadata,
     TableMetadata,
 )
-from ...search_types import MultiSelectFilter, ResultType, SearchFacets, SearchResponse
+from ...search_types import (
+    MultiSelectFilter,
+    ResultType,
+    SearchFacets,
+    SearchResponse,
+    SortOption,
+)
 from ..base import BaseCatalogueClient, CatalogueError, ReferencedEntityMissing, logger
 from .search import SearchClient
 
 DATAHUB_DATA_TYPE_MAPPING = {
     "boolean": schema_classes.BooleanTypeClass(),
     "tinyint": schema_classes.NumberTypeClass(),
     "smallint": schema_classes.NumberTypeClass(),
@@ -317,24 +323,26 @@
         count: int = 20,
         page: str | None = None,
         result_types: Sequence[ResultType] = (
             ResultType.DATA_PRODUCT,
             ResultType.TABLE,
         ),
         filters: Sequence[MultiSelectFilter] = (),
+        sort: SortOption | None = None,
     ) -> SearchResponse:
         """
         Wraps the catalogue's search function.
         """
         return self.search_client.search(
             query=query,
             count=count,
             page=page,
             result_types=result_types,
             filters=filters,
+            sort=sort,
         )
 
     def search_facets(
         self,
         query: str = "*",
         result_types: Sequence[ResultType] = (
             ResultType.DATA_PRODUCT,
```

### Comparing `ministryofjustice_data_platform_catalogue-0.8.1/data_platform_catalogue/client/datahub/graphql/facets.graphql` & `ministryofjustice_data_platform_catalogue-0.9.0/data_platform_catalogue/client/datahub/graphql/facets.graphql`

 * *Files identical despite different names*

### Comparing `ministryofjustice_data_platform_catalogue-0.8.1/data_platform_catalogue/client/datahub/graphql/search.graphql` & `ministryofjustice_data_platform_catalogue-0.9.0/data_platform_catalogue/client/datahub/graphql/search.graphql`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 query Search(
   $query: String!
   $count: Int!
   $start: Int!
   $types: [EntityType!]
   $filters: [FacetFilterInput!]
+  $sort: SearchSortInput
 ) {
   searchAcrossEntities(
     input: {
       types: $types
       query: $query
       start: $start
       count: $count
       orFilters: [{ and: $filters }]
+      sortInput: $sort
     }
   ) {
     start
     count
     total
     facets {
       field
```

### Comparing `ministryofjustice_data_platform_catalogue-0.8.1/data_platform_catalogue/client/datahub/search.py` & `ministryofjustice_data_platform_catalogue-0.9.0/data_platform_catalogue/client/datahub/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from ...search_types import (
     FacetOption,
     MultiSelectFilter,
     ResultType,
     SearchFacets,
     SearchResponse,
     SearchResult,
+    SortOption,
 )
 
 logger = logging.getLogger(__name__)
 
 
 class SearchClient:
     def __init__(self, graph: DataHubGraph):
@@ -39,14 +40,15 @@
         count: int = 20,
         page: str | None = None,
         result_types: Sequence[ResultType] = (
             ResultType.DATA_PRODUCT,
             ResultType.TABLE,
         ),
         filters: Sequence[MultiSelectFilter] = (),
+        sort: SortOption | None = None,
     ) -> SearchResponse:
         """
         Wraps the catalogue's search function.
         """
         if page is None:
             start = 0
         else:
@@ -59,14 +61,17 @@
             "count": count,
             "query": query,
             "start": start,
             "types": types,
             "filters": formatted_filters,
         }
 
+        if sort:
+            variables.update({"sort": sort.format()})
+
         try:
             response = self.graph.execute_graphql(self.search_query, variables)
         except GraphError as e:
             raise Exception("Unable to execute search query") from e
 
         page_results = []
         response = response["searchAcrossEntities"]
```

### Comparing `ministryofjustice_data_platform_catalogue-0.8.1/data_platform_catalogue/client/openmetadata.py` & `ministryofjustice_data_platform_catalogue-0.9.0/data_platform_catalogue/client/openmetadata.py`

 * *Files identical despite different names*

### Comparing `ministryofjustice_data_platform_catalogue-0.8.1/data_platform_catalogue/entities.py` & `ministryofjustice_data_platform_catalogue-0.9.0/data_platform_catalogue/entities.py`

 * *Files identical despite different names*

### Comparing `ministryofjustice_data_platform_catalogue-0.8.1/data_platform_catalogue/search_types.py` & `ministryofjustice_data_platform_catalogue-0.9.0/data_platform_catalogue/search_types.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,30 @@
     """
 
     filter_name: str
     included_values: list[Any]
 
 
 @dataclass
+class SortOption:
+    """Set the search result sorting."""
+
+    field: str
+    ascending: bool = True
+
+    def format(self):
+        return {
+            "sortCriterion": {
+                "field": self.field,
+                "sortOrder": "ASCENDING" if self.ascending else "DESCENDING",
+            }
+        }
+
+
+@dataclass
 class FacetOption:
     """
     A specific value that may be used to filter the search
     """
 
     value: str
     label: str
```

### Comparing `ministryofjustice_data_platform_catalogue-0.8.1/pyproject.toml` & `ministryofjustice_data_platform_catalogue-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ministryofjustice-data-platform-catalogue"
-version = "0.8.1"
+version = "0.9.0"
 description = "Library to integrate the MoJ data platform with the catalogue component."
 authors = ["MoJ Data Platform Team <data-platform-tech@digital.justice.gov.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "data_platform_catalogue" }]
 
 [tool.poetry.dependencies]
```

### Comparing `ministryofjustice_data_platform_catalogue-0.8.1/PKG-INFO` & `ministryofjustice_data_platform_catalogue-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ministryofjustice-data-platform-catalogue
-Version: 0.8.1
+Version: 0.9.0
 Summary: Library to integrate the MoJ data platform with the catalogue component.
 License: MIT
 Author: MoJ Data Platform Team
 Author-email: data-platform-tech@digital.justice.gov.uk
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -103,16 +103,19 @@
 
 # Iterate over facet options
 for option in response.facets.options('domains'):
   print(option.label)
   print(option.value)
   print(option.count)
 
-# Include a filter
-client.search(filters=[MultiSelectFilter("domains", [response.facets['domains'][0].value])])
+# Include a filter and sort
+client.search(
+  filters=[MultiSelectFilter("domains", [response.facets['domains'][0].value])],
+  sort=SortOption(field="name", ascending=False)
+)
 ```
 
 ## Search filters
 
 ### Datahub
 
 Basic filters:
```

