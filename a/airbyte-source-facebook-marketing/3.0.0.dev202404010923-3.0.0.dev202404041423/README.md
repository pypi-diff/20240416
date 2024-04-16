# Comparing `tmp/airbyte_source_facebook_marketing-3.0.0.dev202404010923.tar.gz` & `tmp/airbyte_source_facebook_marketing-3.0.0.dev202404041423.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_facebook_marketing-3.0.0.dev202404010923.tar", max compression
+gzip compressed data, was "airbyte_source_facebook_marketing-3.0.0.dev202404041423.tar", max compression
```

## Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404010923.tar` & `airbyte_source_facebook_marketing-3.0.0.dev202404041423.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     4712 2024-04-01 09:20:45.074363 airbyte_source_facebook_marketing-3.0.0.dev202404010923/README.md
--rw-r--r--   0        0        0      904 2024-04-01 09:23:13.630343 airbyte_source_facebook_marketing-3.0.0.dev202404010923/pyproject.toml
--rw-r--r--   0        0        0     4784 2024-04-01 09:20:45.074363 airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/README.md
--rw-r--r--   0        0        0      455 2024-04-01 09:20:45.074363 airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/__init__.py
--rw-r--r--   0        0        0     8030 2024-04-01 09:20:45.074363 airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/api.py
--rw-r--r--   0        0        0     5157 2024-04-01 09:20:45.074363 airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/config_migrations.py
--rw-r--r--   0        0        0      469 2024-04-01 09:20:45.074363 airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/run.py
--rw-r--r--   0        0        0      885 2024-04-01 09:20:45.074363 airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/schemas/activities.json
--rw-r--r--   0        0        0     5948 2024-04-01 09:20:45.074363 airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/schemas/ad_account.json
--rw-r--r--   0        0        0    42732 2024-04-01 09:20:45.078363 airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/schemas/ad_creatives.json
--rw-r--r--   0        0        0     2660 2024-04-01 09:20:45.078363 airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/schemas/ad_sets.json
--rw-r--r--   0        0        0    11058 2024-04-01 09:20:45.078363 airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/schemas/ads.json
--rw-r--r--   0        0        0     7681 2024-04-01 09:20:45.078363 airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/schemas/ads_insights.json
--rw-r--r--   0        0        0      609 2024-04-01 09:20:45.078363 airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/schemas/ads_insights_action_breakdowns.json
--rw-r--r--   0        0        0     2586 2024-04-01 09:20:45.078363 airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/schemas/ads_insights_breakdowns.json
--rw-r--r--   0        0        0     2606 2024-04-01 09:20:45.078363 airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/schemas/campaigns.json
--rw-r--r--   0        0        0     3587 2024-04-01 09:20:45.078363 airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/schemas/custom_audiences.json
--rw-r--r--   0        0        0     1458 2024-04-01 09:20:45.078363 airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/schemas/custom_conversions.json
--rw-r--r--   0        0        0     1195 2024-04-01 09:20:45.078363 airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/schemas/images.json
--rw-r--r--   0        0        0      764 2024-04-01 09:20:45.078363 airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/schemas/shared/ads_action_stats.json
--rw-r--r--   0        0        0      302 2024-04-01 09:20:45.078363 airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/schemas/shared/ads_histogram_stats.json
--rw-r--r--   0        0        0     1341 2024-04-01 09:20:45.078363 airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/schemas/shared/ads_image_crops.json
--rw-r--r--   0        0        0     3152 2024-04-01 09:20:45.078363 airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/schemas/shared/geo_locations.json
--rw-r--r--   0        0        0     7241 2024-04-01 09:20:45.078363 airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/schemas/shared/targeting.json
--rw-r--r--   0        0        0     2403 2024-04-01 09:20:45.078363 airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/schemas/videos.json
--rw-r--r--   0        0        0    13493 2024-04-01 09:20:45.078363 airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/source.py
--rw-r--r--   0        0        0    10791 2024-04-01 09:20:45.078363 airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/spec.py
--rw-r--r--   0        0        0     1728 2024-04-01 09:20:45.078363 airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/streams/__init__.py
--rw-r--r--   0        0        0    13938 2024-04-01 09:20:45.078363 airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/streams/async_job.py
--rw-r--r--   0        0        0     6544 2024-04-01 09:20:45.078363 airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/streams/async_job_manager.py
--rw-r--r--   0        0        0    16290 2024-04-01 09:20:45.078363 airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/streams/base_insight_streams.py
--rw-r--r--   0        0        0    15508 2024-04-01 09:20:45.078363 airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/streams/base_streams.py
--rw-r--r--   0        0        0     6949 2024-04-01 09:20:45.078363 airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/streams/common.py
--rw-r--r--   0        0        0     2484 2024-04-01 09:20:45.078363 airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/streams/patches.py
--rw-r--r--   0        0        0    13957 2024-04-01 09:20:45.078363 airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/streams/streams.py
--rw-r--r--   0        0        0     2551 2024-04-01 09:20:45.078363 airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/utils.py
--rw-r--r--   0        0        0     5550 1970-01-01 00:00:00.000000 airbyte_source_facebook_marketing-3.0.0.dev202404010923/PKG-INFO
+-rw-r--r--   0        0        0     4712 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/README.md
+-rw-r--r--   0        0        0      904 2024-04-04 14:23:19.230402 airbyte_source_facebook_marketing-3.0.0.dev202404041423/pyproject.toml
+-rw-r--r--   0        0        0     4784 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/README.md
+-rw-r--r--   0        0        0      455 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/__init__.py
+-rw-r--r--   0        0        0     8030 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/api.py
+-rw-r--r--   0        0        0     5157 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/config_migrations.py
+-rw-r--r--   0        0        0      469 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/run.py
+-rw-r--r--   0        0        0      885 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/activities.json
+-rw-r--r--   0        0        0     5948 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/ad_account.json
+-rw-r--r--   0        0        0    42732 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/ad_creatives.json
+-rw-r--r--   0        0        0     2660 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/ad_sets.json
+-rw-r--r--   0        0        0    11058 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/ads.json
+-rw-r--r--   0        0        0     7681 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/ads_insights.json
+-rw-r--r--   0        0        0      609 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/ads_insights_action_breakdowns.json
+-rw-r--r--   0        0        0     2981 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/ads_insights_breakdowns.json
+-rw-r--r--   0        0        0     2606 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/campaigns.json
+-rw-r--r--   0        0        0     3587 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/custom_audiences.json
+-rw-r--r--   0        0        0     1458 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/custom_conversions.json
+-rw-r--r--   0        0        0     1195 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/images.json
+-rw-r--r--   0        0        0      764 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/shared/ads_action_stats.json
+-rw-r--r--   0        0        0      302 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/shared/ads_histogram_stats.json
+-rw-r--r--   0        0        0     1341 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/shared/ads_image_crops.json
+-rw-r--r--   0        0        0     3152 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/shared/geo_locations.json
+-rw-r--r--   0        0        0     7241 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/shared/targeting.json
+-rw-r--r--   0        0        0     2403 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/videos.json
+-rw-r--r--   0        0        0    13493 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/source.py
+-rw-r--r--   0        0        0    10791 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/spec.py
+-rw-r--r--   0        0        0     1728 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/streams/__init__.py
+-rw-r--r--   0        0        0    13938 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/streams/async_job.py
+-rw-r--r--   0        0        0     6544 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/streams/async_job_manager.py
+-rw-r--r--   0        0        0    17218 2024-04-04 14:20:01.544351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/streams/base_insight_streams.py
+-rw-r--r--   0        0        0    15508 2024-04-04 14:20:01.544351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/streams/base_streams.py
+-rw-r--r--   0        0        0     6949 2024-04-04 14:20:01.544351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/streams/common.py
+-rw-r--r--   0        0        0     2484 2024-04-04 14:20:01.544351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/streams/patches.py
+-rw-r--r--   0        0        0    13957 2024-04-04 14:20:01.544351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/streams/streams.py
+-rw-r--r--   0        0        0     2551 2024-04-04 14:20:01.544351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/utils.py
+-rw-r--r--   0        0        0     5550 1970-01-01 00:00:00.000000 airbyte_source_facebook_marketing-3.0.0.dev202404041423/PKG-INFO
```

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404010923/README.md` & `airbyte_source_facebook_marketing-3.0.0.dev202404041423/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404010923/pyproject.toml` & `airbyte_source_facebook_marketing-3.0.0.dev202404041423/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "3.0.0.dev202404010923"
+version = "3.0.0.dev202404041423"
 name = "airbyte-source-facebook-marketing"
 description = "Source implementation for Facebook Marketing."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "ELv2"
 readme = "README.md"
```

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/README.md` & `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/api.py` & `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/api.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/config_migrations.py` & `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/config_migrations.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/schemas/activities.json` & `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/activities.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/schemas/ad_account.json` & `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/ad_account.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/schemas/ad_creatives.json` & `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/ad_creatives.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/schemas/ad_sets.json` & `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/ad_sets.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/schemas/ads.json` & `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/ads.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/schemas/ads_insights.json` & `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/ads_insights.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/schemas/ads_insights_action_breakdowns.json` & `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/ads_insights_action_breakdowns.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/schemas/ads_insights_breakdowns.json` & `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/ads_insights_breakdowns.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8870967741935484%*

 * *Differences: {"'properties'": "{'body_asset_id': OrderedDict([('type', ['null', 'string'])]), "*

 * *                 "'call_to_action_asset_id': OrderedDict([('type', ['null', 'string'])]), "*

 * *                 "'description_asset_id': OrderedDict([('type', ['null', 'string'])]), "*

 * *                 "'image_asset_id': OrderedDict([('type', ['null', 'string'])]), "*

 * *                 "'link_url_asset_id': OrderedDict([('type', ['null', 'string'])]), "*

 * *                 "'title_asset_id': OrderedDict([('type', ['null', 'string'])]) […]*

```diff
@@ -34,14 +34,20 @@
                 }
             },
             "type": [
                 "null",
                 "object"
             ]
         },
+        "body_asset_id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "call_to_action_asset": {
             "properties": {
                 "id": {
                     "type": [
                         "null",
                         "string"
                     ]
@@ -54,14 +60,20 @@
                 }
             },
             "type": [
                 "null",
                 "object"
             ]
         },
+        "call_to_action_asset_id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "country": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "description_asset": {
@@ -80,14 +92,20 @@
                 }
             },
             "type": [
                 "null",
                 "object"
             ]
         },
+        "description_asset_id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "device_platform": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "dma": {
@@ -142,14 +160,20 @@
                 }
             },
             "type": [
                 "null",
                 "object"
             ]
         },
+        "image_asset_id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "impression_device": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "link_url_asset": {
@@ -168,14 +192,20 @@
                 }
             },
             "type": [
                 "null",
                 "object"
             ]
         },
+        "link_url_asset_id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "place_page_id": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "platform_position": {
@@ -224,14 +254,20 @@
                 }
             },
             "type": [
                 "null",
                 "object"
             ]
         },
+        "title_asset_id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "video_asset": {
             "properties": {
                 "id": {
                     "type": [
                         "null",
                         "string"
                     ]
@@ -261,10 +297,16 @@
                     ]
                 }
             },
             "type": [
                 "null",
                 "object"
             ]
+        },
+        "video_asset_id": {
+            "type": [
+                "null",
+                "string"
+            ]
         }
     }
 }
```

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/schemas/campaigns.json` & `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/campaigns.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/schemas/custom_audiences.json` & `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/custom_audiences.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/schemas/custom_conversions.json` & `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/custom_conversions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/schemas/images.json` & `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/images.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/schemas/shared/ads_action_stats.json` & `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/shared/ads_action_stats.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/schemas/shared/ads_image_crops.json` & `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/shared/ads_image_crops.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/schemas/shared/geo_locations.json` & `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/shared/geo_locations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/schemas/shared/targeting.json` & `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/shared/targeting.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/schemas/videos.json` & `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/videos.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/source.py` & `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/spec.py` & `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/spec.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/streams/__init__.py` & `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/streams/async_job.py` & `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/streams/async_job.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/streams/async_job_manager.py` & `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/streams/async_job_manager.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/streams/base_insight_streams.py` & `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/streams/base_insight_streams.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,24 @@
     breakdowns = []
     action_breakdowns = [
         "action_type",
         "action_target_id",
         "action_destination",
     ]
 
+    object_breakdowns = {
+        "body_asset": "body_asset_id",
+        "call_to_action_asset": "call_to_action_asset_id",
+        "description_asset": "description_asset_id",
+        "image_asset": "image_asset_id",
+        "link_url_asset": "link_url_asset_id",
+        "title_asset": "title_asset_id",
+        "video_asset": "video_asset_id",
+    }
+
     # Facebook store metrics maximum of 37 months old. Any time range that
     # older than 37 months from current date would result in 400 Bad request HTTP response.
     # https://developers.facebook.com/docs/marketing-api/reference/ad-account/insights/#overview
     INSIGHTS_RETENTION_PERIOD = pendulum.duration(months=37)
 
     action_attribution_windows = ALL_ACTION_ATTRIBUTION_WINDOWS
     time_increment = 1
@@ -93,15 +103,24 @@
         """We override stream name to let the user change it via configuration."""
         name = self._new_class_name or self.__class__.__name__
         return casing.camel_to_snake(name)
 
     @property
     def primary_key(self) -> Optional[Union[str, List[str], List[List[str]]]]:
         """Build complex PK based on slices and breakdowns"""
-        return ["date_start", "account_id", "ad_id"] + self.breakdowns
+
+        breakdowns_pks = []
+
+        for breakdown in self.breakdowns:
+            if breakdown in self.object_breakdowns.keys():
+                breakdowns_pks.append(self.object_breakdowns[breakdown])
+            else:
+                breakdowns_pks.append(breakdown)
+
+        return ["date_start", "account_id", "ad_id"] + breakdowns_pks
 
     @property
     def insights_lookback_period(self):
         """
         Facebook freezes insight data 28 days after it was generated, which means that all data
         from the past 28 days may have changed since we last emitted it, so we retrieve it again.
         But in some cases users my have define their own lookback window, that's
@@ -109,14 +128,20 @@
         """
         return pendulum.duration(days=self._insights_lookback_window)
 
     @property
     def insights_job_timeout(self):
         return pendulum.duration(minutes=self._insights_job_timeout)
 
+    def _transform_breakdown(self, record: Mapping[str, Any]) -> Mapping[str, Any]:
+        for breakdown in self.object_breakdowns:
+            if breakdown in record:
+                record[self.object_breakdowns[breakdown]] = record[breakdown]["id"]
+        return record
+
     def list_objects(self, params: Mapping[str, Any]) -> Iterable:
         """Because insights has very different read_records we don't need this method anymore"""
 
     def read_records(
         self,
         sync_mode: SyncMode,
         cursor_field: List[str] = None,
@@ -127,15 +152,15 @@
         job = stream_slice["insight_job"]
         account_id = stream_slice["account_id"]
 
         try:
             for obj in job.get_result():
                 data = obj.export_all_data()
                 if self._response_data_is_valid(data):
-                    yield data
+                    yield self._transform_breakdown(data)
         except FacebookBadObjectError as e:
             raise AirbyteTracedException(
                 message=f"API error occurs on Facebook side during job: {job}, wrong (empty) response received with errors: {e} "
                 f"Please try again later",
                 failure_type=FailureType.system_error,
             ) from e
         except FacebookRequestError as exc:
```

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/streams/base_streams.py` & `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/streams/base_streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/streams/common.py` & `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/streams/common.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/streams/patches.py` & `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/streams/patches.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/streams/streams.py` & `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/streams/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404010923/source_facebook_marketing/utils.py` & `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404010923/PKG-INFO` & `airbyte_source_facebook_marketing-3.0.0.dev202404041423/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-facebook-marketing
-Version: 3.0.0.dev202404010923
+Version: 3.0.0.dev202404041423
 Summary: Source implementation for Facebook Marketing.
 Home-page: https://airbyte.com
 License: ELv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
```

