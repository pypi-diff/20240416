# Comparing `tmp/findly_unified_reporting_sdk-0.6.2.tar.gz` & `tmp/findly_unified_reporting_sdk-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findly_unified_reporting_sdk-0.6.2.tar", max compression
+gzip compressed data, was "findly_unified_reporting_sdk-0.6.5.tar", max compression
```

## Comparing `findly_unified_reporting_sdk-0.6.2.tar` & `findly_unified_reporting_sdk-0.6.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    35149 2024-03-05 17:34:31.649998 findly_unified_reporting_sdk-0.6.2/LICENSE
--rw-r--r--   0        0        0     2182 2024-03-14 18:26:39.724288 findly_unified_reporting_sdk-0.6.2/README.md
--rw-r--r--   0        0        0        0 2024-03-22 11:31:41.156543 findly_unified_reporting_sdk-0.6.2/findly/__init__.py
--rw-r--r--   0        0        0      332 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/common/__init__.py
--rw-r--r--   0        0        0     7897 2024-03-22 17:41:32.233479 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/common/common_parser.py
--rw-r--r--   0        0        0      971 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/common/date_range_helper.py
--rw-r--r--   0        0        0     3886 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/common/reports_client.py
--rw-r--r--   0        0        0     5727 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/common/where_string_comparison.py
--rw-r--r--   0        0        0        0 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/fb_ads/__init__.py
--rw-r--r--   0        0        0    20681 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/fb_ads/fb_ads_client.py
--rw-r--r--   0        0        0    31158 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/fb_ads/fb_ads_query_args_parser.py
--rw-r--r--   0        0        0     1492 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/action_breakdowns.csv
--rw-r--r--   0        0        0     5778 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/breakdowns.csv
--rw-r--r--   0        0        0    16489 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/dimensions.jsonl
--rw-r--r--   0        0        0    17708 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/fields.csv
--rw-r--r--   0        0        0    20146 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/metrics.jsonl
--rw-r--r--   0        0        0        0 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/ga4/__init__.py
--rw-r--r--   0        0        0    33529 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/ga4/ga4_client.py
--rw-r--r--   0        0        0    30004 2024-04-01 16:01:21.633515 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/ga4/ga4_query_args_parser.py
--rw-r--r--   0        0        0    33511 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/ga4/metadata/dimensions.jsonl
--rw-r--r--   0        0        0        0 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/gsc/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/gsc/gsc_client.py
--rw-r--r--   0        0        0     1038 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/gsc/gsc_service.py
--rw-r--r--   0        0        0       27 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/protos/.gitignore
--rw-r--r--   0        0        0      137 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/protos/__init__.py
--rw-r--r--   0        0        0     6569 2024-03-22 11:32:22.277139 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/protos/findly_semantic_layer_pb2.py
--rw-r--r--   0        0        0    29515 2024-03-22 11:32:22.277139 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/protos/findly_semantic_layer_pb2.pyi
--rw-r--r--   0        0        0     2993 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/urs.py
--rw-r--r--   0        0        0        0 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/util/__init__.py
--rw-r--r--   0        0        0      451 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/util/create_numeric_string_series.py
--rw-r--r--   0        0        0     1237 2024-04-01 16:01:45.173544 findly_unified_reporting_sdk-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     3108 1970-01-01 00:00:00.000000 findly_unified_reporting_sdk-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-03-05 17:34:31.649998 findly_unified_reporting_sdk-0.6.5/LICENSE
+-rw-r--r--   0        0        0     2182 2024-03-14 18:26:39.724288 findly_unified_reporting_sdk-0.6.5/README.md
+-rw-r--r--   0        0        0        0 2024-03-22 11:31:41.156543 findly_unified_reporting_sdk-0.6.5/findly/__init__.py
+-rw-r--r--   0        0        0      332 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/data_sources/common/__init__.py
+-rw-r--r--   0        0        0     7897 2024-03-22 17:41:32.233479 findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/data_sources/common/common_parser.py
+-rw-r--r--   0        0        0      971 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/data_sources/common/date_range_helper.py
+-rw-r--r--   0        0        0     3886 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/data_sources/common/reports_client.py
+-rw-r--r--   0        0        0     5727 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/data_sources/common/where_string_comparison.py
+-rw-r--r--   0        0        0        0 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/data_sources/fb_ads/__init__.py
+-rw-r--r--   0        0        0    20681 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/data_sources/fb_ads/fb_ads_client.py
+-rw-r--r--   0        0        0    31246 2024-04-16 17:38:32.855858 findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/data_sources/fb_ads/fb_ads_query_args_parser.py
+-rw-r--r--   0        0        0     1492 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/action_breakdowns.csv
+-rw-r--r--   0        0        0     5778 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/breakdowns.csv
+-rw-r--r--   0        0        0    16489 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/dimensions.jsonl
+-rw-r--r--   0        0        0    17708 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/fields.csv
+-rw-r--r--   0        0        0    20146 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/metrics.jsonl
+-rw-r--r--   0        0        0        0 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/data_sources/ga4/__init__.py
+-rw-r--r--   0        0        0    38299 2024-04-16 17:38:32.855858 findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/data_sources/ga4/ga4_client.py
+-rw-r--r--   0        0        0    30004 2024-04-01 17:15:45.015611 findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/data_sources/ga4/ga4_query_args_parser.py
+-rw-r--r--   0        0        0    33511 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/data_sources/ga4/metadata/dimensions.jsonl
+-rw-r--r--   0        0        0        0 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/data_sources/gsc/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/data_sources/gsc/gsc_client.py
+-rw-r--r--   0        0        0     1038 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/data_sources/gsc/gsc_service.py
+-rw-r--r--   0        0        0       27 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/protos/.gitignore
+-rw-r--r--   0        0        0      137 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/protos/__init__.py
+-rw-r--r--   0        0        0     6569 2024-03-22 11:32:22.277139 findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/protos/findly_semantic_layer_pb2.py
+-rw-r--r--   0        0        0    29515 2024-03-22 11:32:22.277139 findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/protos/findly_semantic_layer_pb2.pyi
+-rw-r--r--   0        0        0     2993 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/urs.py
+-rw-r--r--   0        0        0        0 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/util/__init__.py
+-rw-r--r--   0        0        0      451 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/util/create_numeric_string_series.py
+-rw-r--r--   0        0        0     1237 2024-04-16 17:38:56.571121 findly_unified_reporting_sdk-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0     3108 1970-01-01 00:00:00.000000 findly_unified_reporting_sdk-0.6.5/PKG-INFO
```

### Comparing `findly_unified_reporting_sdk-0.6.2/LICENSE` & `findly_unified_reporting_sdk-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.2/README.md` & `findly_unified_reporting_sdk-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/common/common_parser.py` & `findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/data_sources/common/common_parser.py`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/common/date_range_helper.py` & `findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/data_sources/common/date_range_helper.py`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/common/reports_client.py` & `findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/data_sources/common/reports_client.py`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/common/where_string_comparison.py` & `findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/data_sources/common/where_string_comparison.py`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/fb_ads/fb_ads_client.py` & `findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/data_sources/fb_ads/fb_ads_client.py`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/fb_ads/fb_ads_query_args_parser.py` & `findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/data_sources/fb_ads/fb_ads_query_args_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -630,15 +630,16 @@
         allowed_order_by_candidates = [
             candidate
             for candidate in order_by_candidates
             if candidate not in [DATE, YEARMONTH]
         ]
 
         for order_by_item in order_by_list:
-            if order_by_item.lstrip("-") in allowed_order_by_candidates:
+            # We should take into account the action type in the order by
+            if order_by_item.lstrip("-").split(":")[0] in allowed_order_by_candidates:
                 direction = (
                     FB_ADS_ORDER_DESC
                     if order_by_item.startswith("-")
                     else FB_ADS_ORDER_ASC
                 )
                 return [order_by_item.lstrip("-") + direction]
```

### Comparing `findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/action_breakdowns.csv` & `findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/action_breakdowns.csv`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/breakdowns.csv` & `findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/breakdowns.csv`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/dimensions.jsonl` & `findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/dimensions.jsonl`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/fields.csv` & `findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/fields.csv`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/metrics.jsonl` & `findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/metrics.jsonl`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/ga4/ga4_client.py` & `findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/data_sources/ga4/ga4_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -50,14 +50,18 @@
 )
 from findly.unified_reporting_sdk.data_sources.ga4.ga4_query_args_parser import (
     GA4QueryArgsParser,
 )
 
 COHORT_CATEGORY = "cohort"
 
+# default ga4 dimensions values
+EMPTY_STRING = ""
+NOT_SET_VALUE = "(not set)"
+
 SESSIONS_METRIC = Metric(name="sessions")
 
 ORDER_BY_SESSIONS = OrderBy(
     metric=OrderBy.MetricOrderBy(metric_name="sessions"),
     desc=True,
 )
 
@@ -924,14 +928,156 @@
         return filtered_metrics_list
 
     async def list_metrics(
         self, property_id: str, **kwargs: str
     ) -> Optional[List[MetricProto]]:
         return await self._decorated_list_metrics(property_id=property_id, **kwargs)
 
+    @cached(
+        ttl=3600, cache=Cache.MEMORY, skip_cache_func=lambda x: x is None
+    )  # Cache results for 1 hour
+    async def _decorated_get_used_metrics(
+        self, property_id: str, **kwargs: str
+    ) -> Optional[List[str]]:
+        """
+        Asynchronously retrieves a list of used metrics from a Google Analytics 4 property.
+
+        Args:
+            property_id (str): The Google Analytics 4 property identifier.
+
+        Returns:
+            Optional[List[str]]: A list of used metrics api names any exist, None otherwise.
+        """
+        LOGGER.info(
+            {
+                "msg": "getting_used_metrics",
+                "property_id": property_id,
+            }
+        )
+        metrics_list: Optional[List[MetricProto]] = await self.list_metrics(
+            property_id=property_id, **kwargs
+        )
+        if metrics_list is None:
+            LOGGER.info(
+                {
+                    "msg": "no_metrics_metadata_found",
+                    "property_id": property_id,
+                }
+            )
+            return None
+
+        tasks = [
+            self.is_metric_empty(
+                metric=Metric(name=metric.name),
+                property_id=property_id,
+                **kwargs,
+            )
+            for metric in metrics_list
+        ]
+
+        responses = await asyncio.gather(*tasks)
+
+        filtered_metrics_list = []
+
+        for index, response in enumerate(responses):
+            if not response:
+                LOGGER.info(
+                    {
+                        "msg": "metrics_values_found",
+                        "property_id": property_id,
+                        "metric_name": metrics_list[index].name,
+                    }
+                )
+                filtered_metrics_list.append(metrics_list[index].name)
+
+        return filtered_metrics_list
+
+    async def get_used_metrics(
+        self, property_id: str, **kwargs: str
+    ) -> Optional[List[str]]:
+        return await self._decorated_get_used_metrics(property_id=property_id, **kwargs)
+
+    @cached(
+        ttl=3600, cache=Cache.MEMORY, skip_cache_func=lambda x: x is None
+    )  # Cache results for 1 hour
+    async def _decorated_get_used_dimensions(
+        self, property_id: str, **kwargs: str
+    ) -> Optional[List[str]]:
+        """
+        Asynchronously retrieves a list of used dimensions from a Google Analytics 4 property.
+
+        Args:
+            property_id (str): The Google Analytics 4 property identifier.
+
+        Returns:
+            Optional[List[str]]: A list of used dimensions' display names if any exist, None otherwise.
+        """
+        LOGGER.info(
+            {
+                "msg": "getting_used_dimensions",
+                "property_id": property_id,
+            }
+        )
+        all_dimension_list = await self.list_dimensions(
+            property_id=property_id, **kwargs
+        )
+        if all_dimension_list is None:
+            LOGGER.info(
+                {
+                    "msg": "no_dimensions_metadata_found",
+                    "property_id": property_id,
+                }
+            )
+            return None
+
+        tasks = [
+            self.get_dimension_values(
+                dimension=dimension, top_n=5, property_id=property_id, **kwargs
+            )
+            for dimension in all_dimension_list
+        ]
+
+        dimensions_top_n = await asyncio.gather(*tasks)
+
+        filtered_dimension_list = []
+        for index, dimension_top_n in enumerate(dimensions_top_n):
+            if dimension_top_n is None:
+                continue
+            if EMPTY_STRING in dimension_top_n:
+                dimension_top_n.remove(EMPTY_STRING)
+            if NOT_SET_VALUE in dimension_top_n:
+                dimension_top_n.remove(NOT_SET_VALUE)
+            if len(dimension_top_n) > 0:
+                LOGGER.info(
+                    {
+                        "msg": "dimensions_values_found",
+                        "property_id": property_id,
+                        "dimension_name": all_dimension_list[index].name,
+                    }
+                )
+                filtered_dimension_list.append(all_dimension_list[index].name)
+
+        if len(filtered_dimension_list) == 0:
+            LOGGER.info(
+                {
+                    "msg": "no_dimensions_with_top_n_found",
+                    "property_id": property_id,
+                }
+            )
+            return None
+
+        return filtered_dimension_list
+
+    async def get_used_dimensions(
+        self, property_id: str, **kwargs: str
+    ) -> Optional[List[str]]:
+        return await self._decorated_get_used_dimensions(
+            property_id=property_id, **kwargs
+        )
+
     @backoff.on_exception(
         backoff.expo, Exception, max_time=60, max_tries=3, giveup=give_up
     )
     @cached(
         ttl=300, cache=Cache.MEMORY, skip_cache_func=lambda x: x is None
     )  # Cache results for 5 minutes
     async def _decorated_check_compatibility(
```

### Comparing `findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/ga4/ga4_query_args_parser.py` & `findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/data_sources/ga4/ga4_query_args_parser.py`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/ga4/metadata/dimensions.jsonl` & `findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/data_sources/ga4/metadata/dimensions.jsonl`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/gsc/gsc_service.py` & `findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/data_sources/gsc/gsc_service.py`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/protos/findly_semantic_layer_pb2.py` & `findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/protos/findly_semantic_layer_pb2.py`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/protos/findly_semantic_layer_pb2.pyi` & `findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/protos/findly_semantic_layer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/urs.py` & `findly_unified_reporting_sdk-0.6.5/findly/unified_reporting_sdk/urs.py`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.2/pyproject.toml` & `findly_unified_reporting_sdk-0.6.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findly.unified-reporting-sdk"
-version = "0.6.2"
+version = "0.6.5"
 license = "GPL-3.0-only"
 description = ""
 authors = []
 readme = "README.md"
 packages = [
     { include = "findly" },
 ]
```

### Comparing `findly_unified_reporting_sdk-0.6.2/PKG-INFO` & `findly_unified_reporting_sdk-0.6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findly-unified-reporting-sdk
-Version: 0.6.2
+Version: 0.6.5
 Summary: 
 License: GPL-3.0-only
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

