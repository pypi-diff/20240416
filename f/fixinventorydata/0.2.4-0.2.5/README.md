# Comparing `tmp/fixinventorydata-0.2.4.tar.gz` & `tmp/fixinventorydata-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventorydata-0.2.4.tar", last modified: Mon Feb 26 21:46:21 2024, max compression
+gzip compressed data, was "fixinventorydata-0.2.5.tar", last modified: Tue Apr 16 13:43:30 2024, max compression
```

## Comparing `fixinventorydata-0.2.4.tar` & `fixinventorydata-0.2.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:46:21.708332 fixinventorydata-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-26 21:46:03.000000 fixinventorydata-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-02-26 21:46:21.708332 fixinventorydata-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-02-26 21:46:03.000000 fixinventorydata-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:46:21.684332 fixinventorydata-0.2.4/fixinventorydata/
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-02-26 21:46:03.000000 fixinventorydata-0.2.4/fixinventorydata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14365 2024-02-26 21:46:03.000000 fixinventorydata-0.2.4/fixinventorydata/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-02-26 21:46:03.000000 fixinventorydata-0.2.4/fixinventorydata/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-26 21:46:03.000000 fixinventorydata-0.2.4/fixinventorydata/co2.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-26 21:46:03.000000 fixinventorydata-0.2.4/fixinventorydata/colors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:46:21.708332 fixinventorydata-0.2.4/fixinventorydata/data/
--rw-r--r--   0 runner    (1001) docker     (127)    17029 2024-02-26 21:46:03.000000 fixinventorydata-0.2.4/fixinventorydata/data/ccfdataset.json
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-02-26 21:46:03.000000 fixinventorydata-0.2.4/fixinventorydata/data/colors.json
--rw-r--r--   0 runner    (1001) docker     (127) 18763286 2024-02-26 21:46:03.000000 fixinventorydata-0.2.4/fixinventorydata/data/instances.json
--rw-r--r--   0 runner    (1001) docker     (127)    13805 2024-02-26 21:46:03.000000 fixinventorydata-0.2.4/fixinventorydata/data/regions.json
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-02-26 21:46:03.000000 fixinventorydata-0.2.4/fixinventorydata/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:46:21.708332 fixinventorydata-0.2.4/fixinventorydata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-02-26 21:46:21.000000 fixinventorydata-0.2.4/fixinventorydata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-02-26 21:46:21.000000 fixinventorydata-0.2.4/fixinventorydata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 21:46:21.000000 fixinventorydata-0.2.4/fixinventorydata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-02-26 21:46:21.000000 fixinventorydata-0.2.4/fixinventorydata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 21:46:21.000000 fixinventorydata-0.2.4/fixinventorydata.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-26 21:46:21.000000 fixinventorydata-0.2.4/fixinventorydata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-26 21:46:21.000000 fixinventorydata-0.2.4/fixinventorydata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-26 21:46:21.708332 fixinventorydata-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-02-26 21:46:03.000000 fixinventorydata-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:46:21.708332 fixinventorydata-0.2.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-26 21:46:03.000000 fixinventorydata-0.2.4/test/test_args.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:43:30.668034 fixinventorydata-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-16 13:43:11.000000 fixinventorydata-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-16 13:43:30.668034 fixinventorydata-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-16 13:43:11.000000 fixinventorydata-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:43:30.644034 fixinventorydata-0.2.5/fixinventorydata/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-16 13:43:11.000000 fixinventorydata-0.2.5/fixinventorydata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14962 2024-04-16 13:43:11.000000 fixinventorydata-0.2.5/fixinventorydata/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-16 13:43:11.000000 fixinventorydata-0.2.5/fixinventorydata/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-16 13:43:11.000000 fixinventorydata-0.2.5/fixinventorydata/co2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-16 13:43:11.000000 fixinventorydata-0.2.5/fixinventorydata/colors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:43:30.668034 fixinventorydata-0.2.5/fixinventorydata/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    17029 2024-04-16 13:43:11.000000 fixinventorydata-0.2.5/fixinventorydata/data/ccfdataset.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-16 13:43:11.000000 fixinventorydata-0.2.5/fixinventorydata/data/colors.json
+-rw-r--r--   0 runner    (1001) docker     (127) 18763286 2024-04-16 13:43:11.000000 fixinventorydata-0.2.5/fixinventorydata/data/instances.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15958 2024-04-16 13:43:11.000000 fixinventorydata-0.2.5/fixinventorydata/data/regions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-16 13:43:11.000000 fixinventorydata-0.2.5/fixinventorydata/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:43:30.668034 fixinventorydata-0.2.5/fixinventorydata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-16 13:43:30.000000 fixinventorydata-0.2.5/fixinventorydata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-16 13:43:30.000000 fixinventorydata-0.2.5/fixinventorydata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 13:43:30.000000 fixinventorydata-0.2.5/fixinventorydata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-16 13:43:30.000000 fixinventorydata-0.2.5/fixinventorydata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 13:43:30.000000 fixinventorydata-0.2.5/fixinventorydata.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-16 13:43:30.000000 fixinventorydata-0.2.5/fixinventorydata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-16 13:43:30.000000 fixinventorydata-0.2.5/fixinventorydata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-16 13:43:30.668034 fixinventorydata-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-16 13:43:11.000000 fixinventorydata-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:43:30.668034 fixinventorydata-0.2.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-16 13:43:11.000000 fixinventorydata-0.2.5/test/test_args.py
```

### Comparing `fixinventorydata-0.2.4/PKG-INFO` & `fixinventorydata-0.2.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventorydata
-Version: 0.2.4
+Version: 0.2.5
 Summary: Miscellaneous Fix Inventory data.
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `fixinventorydata-0.2.4/README.md` & `fixinventorydata-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `fixinventorydata-0.2.4/fixinventorydata/__main__.py` & `fixinventorydata-0.2.5/fixinventorydata/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,15 +79,26 @@
 def gen_gcp_regions() -> dict:
     print("Processing GCP regions")
     regions = {}
     locations_url = "https://cloud.google.com/about/locations"
     r = requests.get(locations_url)
     soup = BeautifulSoup(r.text, "html.parser")
     for loc in soup.find_all("span", {"class": "zone"}):
-        long_region = loc.previous_sibling
+        long_region = loc.previous_sibling.text.strip()
+        if len(long_region) == 0:
+            previous_element = loc.previous_element
+            while previous_element:
+                if (
+                    previous_element.name == "a"
+                    and "cloud-link" in previous_element.get("class", [])
+                    and len(previous_element.text.strip()) > 2
+                ):
+                    long_region = previous_element.text.strip()
+                    break
+                previous_element = previous_element.previous_element
         short_region = loc.text
         if "(" in short_region and ")" in short_region:
             short_region = short_region[short_region.find("(") + 1 : short_region.find(")")]
         location = extract_gcp_location(short_region, long_region)
         location = lookup_location(short_region, location)
         regions[short_region] = {
             "short_name": short_region,
@@ -144,14 +155,16 @@
     "us-east4": "Ashburn, Virginia, USA",
     "us-central1": "Council Bluffs, Iowa, USA",
     "us-south1": "Dallas, Texas, USA",
     "europe-west1": "St. Ghislain, Belgium",
     "europe-west4": "Eemshaven, Netherlands",
     "europe-north1": "Hamina, Finland",
     "southamerica-west1": "Santiago, Chile",
+    "me-central1": "Doha, Qatar",
+    "me-central2": "Dammam, Saudi Arabia",
 }
 
 
 def extract_aws_location(short_region: str, long_region: str) -> str:
     if short_region in aws_override:
         return aws_override[short_region]
     if "(" in long_region and ")" in long_region:
```

### Comparing `fixinventorydata-0.2.4/fixinventorydata/cloud.py` & `fixinventorydata-0.2.5/fixinventorydata/cloud.py`

 * *Files identical despite different names*

### Comparing `fixinventorydata-0.2.4/fixinventorydata/data/ccfdataset.json` & `fixinventorydata-0.2.5/fixinventorydata/data/ccfdataset.json`

 * *Files identical despite different names*

### Comparing `fixinventorydata-0.2.4/fixinventorydata/data/colors.json` & `fixinventorydata-0.2.5/fixinventorydata/data/colors.json`

 * *Files identical despite different names*

### Comparing `fixinventorydata-0.2.4/fixinventorydata/data/instances.json` & `fixinventorydata-0.2.5/fixinventorydata/data/instances.json`

 * *Files identical despite different names*

### Comparing `fixinventorydata-0.2.4/fixinventorydata/data/regions.json` & `fixinventorydata-0.2.5/fixinventorydata/data/regions.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9275156506568146%*

 * *Differences: {"'aws'": "{'ap-east-1': {'latitude': 22.350627, 'longitude': 114.1849161}, 'ap-northeast-1': "*

 * *          "{'latitude': 35.6821936, 'longitude': 139.762221}, 'ap-northeast-3': {'latitude': "*

 * *          "34.6198813, 'longitude': 135.490357}, 'ap-south-1': {'latitude': 18.9733536, "*

 * *          "'longitude': 72.82810491917377}, 'ap-southeast-3': {'latitude': -6.175247, 'longitude': "*

 * *          "106.8270488}, 'eu-west-1': {'latitude': 53.3493795, 'longitude': -6.2605593}, "*

 * *          "'eu-west-2': {'latitude': 51 […]*

```diff
@@ -3,103 +3,139 @@
         "af-south-1": {
             "latitude": -33.928992,
             "long_name": "Africa (Cape Town)",
             "longitude": 18.417396,
             "short_name": "af-south-1"
         },
         "ap-east-1": {
-            "latitude": 22.2793278,
+            "latitude": 22.350627,
             "long_name": "Asia Pacific (Hong Kong)",
-            "longitude": 114.1628131,
+            "longitude": 114.1849161,
             "short_name": "ap-east-1"
         },
         "ap-northeast-1": {
-            "latitude": 35.6812665,
+            "latitude": 35.6821936,
             "long_name": "Asia Pacific (Tokyo)",
-            "longitude": 139.757653,
+            "longitude": 139.762221,
             "short_name": "ap-northeast-1"
         },
         "ap-northeast-2": {
             "latitude": 37.5666791,
             "long_name": "Asia Pacific (Seoul)",
             "longitude": 126.9782914,
             "short_name": "ap-northeast-2"
         },
         "ap-northeast-3": {
-            "latitude": 34.661629000000005,
+            "latitude": 34.6198813,
             "long_name": "Asia Pacific (Osaka)",
-            "longitude": 135.49992679245517,
+            "longitude": 135.490357,
             "short_name": "ap-northeast-3"
         },
         "ap-south-1": {
-            "latitude": 19.0785451,
+            "latitude": 18.9733536,
             "long_name": "Asia Pacific (Mumbai)",
-            "longitude": 72.878176,
+            "longitude": 72.82810491917377,
             "short_name": "ap-south-1"
         },
+        "ap-south-2": {
+            "latitude": 17.360589,
+            "long_name": "Asia Pacific (Hyderabad)",
+            "longitude": 78.4740613,
+            "short_name": "ap-south-2"
+        },
         "ap-southeast-1": {
             "latitude": 1.357107,
             "long_name": "Asia Pacific (Singapore)",
             "longitude": 103.8194992,
             "short_name": "ap-southeast-1"
         },
         "ap-southeast-2": {
             "latitude": -33.8698439,
             "long_name": "Asia Pacific (Sydney)",
             "longitude": 151.2082848,
             "short_name": "ap-southeast-2"
         },
         "ap-southeast-3": {
-            "latitude": -6.1753942,
+            "latitude": -6.175247,
             "long_name": "Asia Pacific (Jakarta)",
-            "longitude": 106.827183,
+            "longitude": 106.8270488,
             "short_name": "ap-southeast-3"
         },
+        "ap-southeast-4": {
+            "latitude": -37.8142454,
+            "long_name": "Asia Pacific (Melbourne)",
+            "longitude": 144.9631732,
+            "short_name": "ap-southeast-4"
+        },
         "ca-central-1": {
             "latitude": 45.5031824,
             "long_name": "Canada (Central)",
             "longitude": -73.5698065,
             "short_name": "ca-central-1"
         },
+        "ca-west-1": {
+            "latitude": 51.0456064,
+            "long_name": "Canada West (Calgary)",
+            "longitude": -114.057541,
+            "short_name": "ca-west-1"
+        },
         "eu-central-1": {
             "latitude": 50.1106444,
             "long_name": "Europe (Frankfurt)",
             "longitude": 8.6820917,
             "short_name": "eu-central-1"
         },
+        "eu-central-2": {
+            "latitude": 47.3744489,
+            "long_name": "Europe (Zurich)",
+            "longitude": 8.5410422,
+            "short_name": "eu-central-2"
+        },
         "eu-north-1": {
             "latitude": 59.3251172,
             "long_name": "Europe (Stockholm)",
             "longitude": 18.0710935,
             "short_name": "eu-north-1"
         },
         "eu-south-1": {
             "latitude": 45.4641943,
             "long_name": "Europe (Milan)",
             "longitude": 9.1896346,
             "short_name": "eu-south-1"
         },
+        "eu-south-2": {
+            "latitude": 39.3260685,
+            "long_name": "Europe (Spain)",
+            "longitude": -4.8379791,
+            "short_name": "eu-south-2"
+        },
         "eu-west-1": {
-            "latitude": 53.3498006,
+            "latitude": 53.3493795,
             "long_name": "Europe (Ireland)",
-            "longitude": -6.2602964,
+            "longitude": -6.2605593,
             "short_name": "eu-west-1"
         },
         "eu-west-2": {
-            "latitude": 51.5073359,
+            "latitude": 51.4893335,
             "long_name": "Europe (London)",
-            "longitude": -0.12765,
+            "longitude": -0.14405508452768728,
             "short_name": "eu-west-2"
         },
         "eu-west-3": {
             "latitude": 48.8588897,
             "long_name": "Europe (Paris)",
             "longitude": 2.3200410217200766,
             "short_name": "eu-west-3"
         },
+        "il-central-1": {
+            "latitude": 32.0852997,
+            "long_name": "Israel (Tel Aviv)",
+            "longitude": 34.7818064,
+            "short_name": "il-central-1"
+        },
         "me-central-1": {
             "latitude": 25.074282349999997,
             "long_name": "Middle East (UAE)",
             "longitude": 55.18853865430702,
             "short_name": "me-central-1"
         },
         "me-south-1": {
@@ -123,17 +159,17 @@
         "us-east-2": {
             "latitude": 39.9622601,
             "long_name": "US East (Ohio)",
             "longitude": -83.0007065,
             "short_name": "us-east-2"
         },
         "us-west-1": {
-            "latitude": 37.7790262,
+            "latitude": 37.7792588,
             "long_name": "US West (N. California)",
-            "longitude": -122.419906,
+            "longitude": -122.4193286,
             "short_name": "us-west-1"
         },
         "us-west-2": {
             "latitude": 45.839855,
             "long_name": "US West (Oregon)",
             "longitude": -119.700583,
             "short_name": "us-west-2"
@@ -161,17 +197,17 @@
         "fra1": {
             "latitude": 50.1106444,
             "long_name": "Frankfurt 1",
             "longitude": 8.6820917,
             "short_name": "fra1"
         },
         "lon1": {
-            "latitude": 51.5073359,
+            "latitude": 51.4893335,
             "long_name": "London 1",
-            "longitude": -0.12765,
+            "longitude": -0.14405508452768728,
             "short_name": "lon1"
         },
         "nyc1": {
             "latitude": 40.7127281,
             "long_name": "New York 1",
             "longitude": -74.0060152,
             "short_name": "nyc1"
@@ -185,29 +221,29 @@
         "nyc3": {
             "latitude": 40.7127281,
             "long_name": "New York 3",
             "longitude": -74.0060152,
             "short_name": "nyc3"
         },
         "sfo1": {
-            "latitude": 37.7790262,
+            "latitude": 37.7792588,
             "long_name": "San Francisco 1",
-            "longitude": -122.419906,
+            "longitude": -122.4193286,
             "short_name": "sfo1"
         },
         "sfo2": {
-            "latitude": 37.7790262,
+            "latitude": 37.7792588,
             "long_name": "San Francisco 2",
-            "longitude": -122.419906,
+            "longitude": -122.4193286,
             "short_name": "sfo2"
         },
         "sfo3": {
-            "latitude": 37.7790262,
+            "latitude": 37.7792588,
             "long_name": "San Francisco 3",
-            "longitude": -122.419906,
+            "longitude": -122.4193286,
             "short_name": "sfo3"
         },
         "sgp1": {
             "latitude": 1.357107,
             "long_name": "Singapore 1",
             "longitude": 103.8194992,
             "short_name": "sgp1"
@@ -222,84 +258,90 @@
             "latitude": 43.6534817,
             "long_name": "Toronto 1",
             "longitude": -79.3839347,
             "short_name": "tor1"
         }
     },
     "gcp": {
+        "africa-south1": {
+            "latitude": -26.205,
+            "long_name": "Johannesburg",
+            "longitude": 28.049722,
+            "short_name": "africa-south1"
+        },
         "asia-east1": {
-            "latitude": 23.9739374,
+            "latitude": 23.5983227,
             "long_name": "Taiwan",
-            "longitude": 120.9820179,
+            "longitude": 120.83537694479215,
             "short_name": "asia-east1"
         },
         "asia-east2": {
-            "latitude": 22.2793278,
+            "latitude": 22.350627,
             "long_name": "Hong Kong",
-            "longitude": 114.1628131,
+            "longitude": 114.1849161,
             "short_name": "asia-east2"
         },
         "asia-northeast1": {
-            "latitude": 35.6812665,
+            "latitude": 35.6821936,
             "long_name": "Tokyo",
-            "longitude": 139.757653,
+            "longitude": 139.762221,
             "short_name": "asia-northeast1"
         },
         "asia-northeast2": {
-            "latitude": 34.661629000000005,
+            "latitude": 34.6198813,
             "long_name": "Osaka",
-            "longitude": 135.49992679245517,
+            "longitude": 135.490357,
             "short_name": "asia-northeast2"
         },
         "asia-northeast3": {
             "latitude": 37.5666791,
             "long_name": "Seoul",
             "longitude": 126.9782914,
             "short_name": "asia-northeast3"
         },
         "asia-south1": {
-            "latitude": 19.0785451,
+            "latitude": 18.9733536,
             "long_name": "Mumbai",
-            "longitude": 72.878176,
+            "longitude": 72.82810491917377,
             "short_name": "asia-south1"
         },
         "asia-south2": {
-            "latitude": 28.6517178,
+            "latitude": 28.6273928,
             "long_name": "Delhi",
-            "longitude": 77.2219388,
+            "longitude": 77.1716954,
             "short_name": "asia-south2"
         },
         "asia-southeast1": {
             "latitude": 1.357107,
             "long_name": "Singapore",
             "longitude": 103.8194992,
             "short_name": "asia-southeast1"
         },
         "asia-southeast2": {
-            "latitude": -6.1753942,
+            "latitude": -6.175247,
             "long_name": "Jakarta",
-            "longitude": 106.827183,
+            "longitude": 106.8270488,
             "short_name": "asia-southeast2"
         },
         "australia-southeast1": {
             "latitude": -33.8698439,
             "long_name": "Sydney",
             "longitude": 151.2082848,
             "short_name": "australia-southeast1"
         },
         "australia-southeast2": {
-            "latitude": -37.8142176,
+            "latitude": -37.8142454,
             "long_name": "Melbourne",
-            "longitude": 144.9631608,
+            "longitude": 144.9631732,
             "short_name": "australia-southeast2"
         },
         "europe-central2": {
-            "latitude": 52.2319581,
+            "latitude": 52.2337172,
             "long_name": "Warsaw",
-            "longitude": 21.0067249,
+            "longitude": 21.071432235636493,
             "short_name": "europe-central2"
         },
         "europe-north1": {
             "latitude": 60.5688901,
             "long_name": "Finland",
             "longitude": 27.1881877,
             "short_name": "europe-north1"
@@ -312,30 +354,42 @@
         },
         "europe-west1": {
             "latitude": 50.4477484,
             "long_name": "Belgium",
             "longitude": 3.8195241,
             "short_name": "europe-west1"
         },
+        "europe-west10": {
+            "latitude": 52.5170365,
+            "long_name": "Berlin",
+            "longitude": 13.3888599,
+            "short_name": "europe-west10"
+        },
+        "europe-west12": {
+            "latitude": 45.0677551,
+            "long_name": "Turin",
+            "longitude": 7.6824892,
+            "short_name": "europe-west12"
+        },
         "europe-west2": {
-            "latitude": 51.5073359,
+            "latitude": 51.4893335,
             "long_name": "London",
-            "longitude": -0.12765,
+            "longitude": -0.14405508452768728,
             "short_name": "europe-west2"
         },
         "europe-west3": {
             "latitude": 50.1106444,
             "long_name": "Frankfurt",
             "longitude": 8.6820917,
             "short_name": "europe-west3"
         },
         "europe-west4": {
             "latitude": 53.44847365,
             "long_name": "Netherlands",
-            "longitude": 6.849962720298231,
+            "longitude": 6.849962702578557,
             "short_name": "europe-west4"
         },
         "europe-west6": {
             "latitude": 47.3744489,
             "long_name": "Zurich",
             "longitude": 8.5410422,
             "short_name": "europe-west6"
@@ -348,14 +402,26 @@
         },
         "europe-west9": {
             "latitude": 48.8588897,
             "long_name": "Paris",
             "longitude": 2.3200410217200766,
             "short_name": "europe-west9"
         },
+        "me-central1": {
+            "latitude": 25.2856329,
+            "long_name": "Doha",
+            "longitude": 51.5264162,
+            "short_name": "me-central1"
+        },
+        "me-central2": {
+            "latitude": 26.4367824,
+            "long_name": "Dammam",
+            "longitude": 50.1039991,
+            "short_name": "me-central2"
+        },
         "me-west1": {
             "latitude": 32.0852997,
             "long_name": "Tel Aviv",
             "longitude": 34.7818064,
             "short_name": "me-west1"
         },
         "northamerica-northeast1": {
```

### Comparing `fixinventorydata-0.2.4/fixinventorydata/utils.py` & `fixinventorydata-0.2.5/fixinventorydata/utils.py`

 * *Files identical despite different names*

### Comparing `fixinventorydata-0.2.4/fixinventorydata.egg-info/PKG-INFO` & `fixinventorydata-0.2.5/fixinventorydata.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventorydata
-Version: 0.2.4
+Version: 0.2.5
 Summary: Miscellaneous Fix Inventory data.
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `fixinventorydata-0.2.4/fixinventorydata.egg-info/SOURCES.txt` & `fixinventorydata-0.2.5/fixinventorydata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixinventorydata-0.2.4/setup.py` & `fixinventorydata-0.2.5/setup.py`

 * *Files identical despite different names*

