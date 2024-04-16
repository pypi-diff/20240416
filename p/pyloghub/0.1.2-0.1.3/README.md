# Comparing `tmp/pyloghub-0.1.2.tar.gz` & `tmp/pyloghub-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyloghub-0.1.2.tar", last modified: Wed Jan 10 18:55:25 2024, max compression
+gzip compressed data, was "pyloghub-0.1.3.tar", last modified: Tue Apr 16 13:05:35 2024, max compression
```

## Comparing `pyloghub-0.1.2.tar` & `pyloghub-0.1.3.tar`

### file list

```diff
@@ -1,45 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-01-10 18:55:25.273892 pyloghub-0.1.2/
--rw-rw-rw-   0        0        0     2985 2024-01-10 17:25:17.000000 pyloghub-0.1.2/CHANGELOG.md
--rw-rw-rw-   0        0        0     1071 2023-12-14 13:48:24.000000 pyloghub-0.1.2/LICENSE
--rw-rw-rw-   0        0        0       39 2023-12-14 14:12:08.000000 pyloghub-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0    12148 2024-01-10 18:55:25.271890 pyloghub-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0    11086 2024-01-10 17:44:06.000000 pyloghub-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-01-10 18:55:25.103154 pyloghub-0.1.2/pyloghub/
--rw-rw-rw-   0        0        0       22 2024-01-10 16:39:44.000000 pyloghub-0.1.2/pyloghub/__init__.py
--rw-rw-rw-   0        0        0     9166 2023-12-14 07:43:59.000000 pyloghub-0.1.2/pyloghub/center_of_gravity.py
--rw-rw-rw-   0        0        0     9956 2023-12-14 08:02:14.000000 pyloghub-0.1.2/pyloghub/center_of_gravity_plus.py
--rw-rw-rw-   0        0        0    11682 2024-01-10 16:52:22.000000 pyloghub-0.1.2/pyloghub/dataset.py
--rw-rw-rw-   0        0        0    10958 2023-12-14 07:53:55.000000 pyloghub-0.1.2/pyloghub/distance_calculation.py
--rw-rw-rw-   0        0        0    11484 2023-12-14 09:02:38.000000 pyloghub-0.1.2/pyloghub/fixed_center_of_gravity.py
--rw-rw-rw-   0        0        0     9649 2023-12-13 13:47:45.000000 pyloghub-0.1.2/pyloghub/geocoding.py
--rw-rw-rw-   0        0        0    18989 2023-12-14 09:51:21.000000 pyloghub-0.1.2/pyloghub/milkrun_optimization_plus.py
-drwxrwxrwx   0        0        0        0 2024-01-10 18:55:25.264459 pyloghub-0.1.2/pyloghub/sample_data/
--rw-rw-rw-   0        0        0    15659 2023-12-14 16:26:34.000000 pyloghub-0.1.2/pyloghub/sample_data/COGPlusSampleDataAddresses.xlsx
--rw-rw-rw-   0        0        0    15903 2023-12-14 16:26:46.000000 pyloghub-0.1.2/pyloghub/sample_data/COGPlusSampleDataReverse.xlsx
--rw-rw-rw-   0        0        0    16985 2023-12-14 16:26:57.000000 pyloghub-0.1.2/pyloghub/sample_data/COGSampleDataAddresses.xlsx
--rw-rw-rw-   0        0        0    16665 2023-12-14 16:27:09.000000 pyloghub-0.1.2/pyloghub/sample_data/COGSampleDataReverse.xlsx
--rw-rw-rw-   0        0        0    13101 2023-12-14 16:27:20.000000 pyloghub-0.1.2/pyloghub/sample_data/DistanceCalcSampleDataAddresses.xlsx
--rw-rw-rw-   0        0        0    12986 2023-12-14 16:27:30.000000 pyloghub-0.1.2/pyloghub/sample_data/DistanceCalcSampleDataReverse.xlsx
--rw-rw-rw-   0        0        0    36539 2023-12-14 16:27:40.000000 pyloghub-0.1.2/pyloghub/sample_data/FixedCOGSampleDataAddresses.xlsx
--rw-rw-rw-   0        0        0    33868 2023-12-14 16:27:52.000000 pyloghub-0.1.2/pyloghub/sample_data/FixedCOGSampleDataReverse.xlsx
--rw-rw-rw-   0        0        0    14535 2023-12-14 16:28:03.000000 pyloghub-0.1.2/pyloghub/sample_data/GeocodingSampleDataAddresses.xlsx
--rw-rw-rw-   0        0        0    13881 2023-12-14 16:28:13.000000 pyloghub-0.1.2/pyloghub/sample_data/GeocodingSampleDataReverse.xlsx
--rw-rw-rw-   0        0        0    33828 2023-12-14 16:28:24.000000 pyloghub-0.1.2/pyloghub/sample_data/MilkrunPlusSampleDataAddresses.xlsx
--rw-rw-rw-   0        0        0    26624 2023-12-14 16:28:36.000000 pyloghub-0.1.2/pyloghub/sample_data/MilkrunPlusSampleDataReverse.xlsx
--rw-rw-rw-   0        0        0    54710 2023-12-14 16:28:50.000000 pyloghub-0.1.2/pyloghub/sample_data/shipmentAnalyzerAddresses.xlsx
--rw-rw-rw-   0        0        0    47612 2023-12-14 16:29:02.000000 pyloghub-0.1.2/pyloghub/sample_data/shipmentAnalyzerReverse.xlsx
--rw-rw-rw-   0        0        0    22689 2023-12-14 16:29:13.000000 pyloghub-0.1.2/pyloghub/sample_data/transportPlusAddresses.xlsx
--rw-rw-rw-   0        0        0    22883 2023-12-14 16:29:24.000000 pyloghub-0.1.2/pyloghub/sample_data/transportPlusReverse.xlsx
--rw-rw-rw-   0        0        0    16230 2023-12-13 13:08:53.000000 pyloghub-0.1.2/pyloghub/shipment_analyzer.py
--rw-rw-rw-   0        0        0    18398 2023-12-14 10:03:54.000000 pyloghub-0.1.2/pyloghub/transport_optimization_plus.py
-drwxrwxrwx   0        0        0        0 2024-01-10 18:55:25.269898 pyloghub-0.1.2/pyloghub.egg-info/
--rw-rw-rw-   0        0        0    12148 2024-01-10 18:55:24.000000 pyloghub-0.1.2/pyloghub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1395 2024-01-10 18:55:25.000000 pyloghub-0.1.2/pyloghub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-10 18:55:24.000000 pyloghub-0.1.2/pyloghub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-01-10 18:55:24.000000 pyloghub-0.1.2/pyloghub.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-01-10 18:55:24.000000 pyloghub-0.1.2/pyloghub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-10 18:55:25.273892 pyloghub-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      957 2024-01-10 15:57:23.000000 pyloghub-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-10 18:55:25.268895 pyloghub-0.1.2/tests/
--rw-rw-rw-   0        0        0        0 2023-12-08 11:11:58.000000 pyloghub-0.1.2/tests/__init__.py
--rw-rw-rw-   0        0        0     2655 2023-12-14 17:18:16.000000 pyloghub-0.1.2/tests/test_geocoding.py
+drwxrwxrwx   0        0        0        0 2024-04-16 13:05:35.354483 pyloghub-0.1.3/
+-rw-rw-rw-   0        0        0     4854 2024-04-16 11:49:30.000000 pyloghub-0.1.3/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1071 2023-12-14 13:48:24.000000 pyloghub-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0       39 2023-12-14 14:12:08.000000 pyloghub-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    14087 2024-04-16 13:05:35.352484 pyloghub-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0    12949 2024-04-16 12:59:46.000000 pyloghub-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 13:05:35.246447 pyloghub-0.1.3/pyloghub/
+-rw-rw-rw-   0        0        0       22 2024-01-10 16:39:44.000000 pyloghub-0.1.3/pyloghub/__init__.py
+-rw-rw-rw-   0        0        0     9466 2024-04-16 09:20:24.000000 pyloghub-0.1.3/pyloghub/center_of_gravity.py
+-rw-rw-rw-   0        0        0    10256 2024-04-16 09:22:34.000000 pyloghub-0.1.3/pyloghub/center_of_gravity_plus.py
+-rw-rw-rw-   0        0        0    11825 2024-04-16 09:36:09.000000 pyloghub-0.1.3/pyloghub/dataset.py
+-rw-rw-rw-   0        0        0    11256 2024-04-16 09:43:20.000000 pyloghub-0.1.3/pyloghub/distance_calculation.py
+-rw-rw-rw-   0        0        0    11784 2024-04-16 09:24:54.000000 pyloghub-0.1.3/pyloghub/fixed_center_of_gravity.py
+-rw-rw-rw-   0        0        0    11306 2024-04-16 10:01:35.000000 pyloghub-0.1.3/pyloghub/freight_matrix.py
+-rw-rw-rw-   0        0        0     9884 2024-04-16 09:14:38.000000 pyloghub-0.1.3/pyloghub/geocoding.py
+-rw-rw-rw-   0        0        0    19287 2024-04-16 09:27:21.000000 pyloghub-0.1.3/pyloghub/milkrun_optimization_plus.py
+drwxrwxrwx   0        0        0        0 2024-04-16 13:05:35.339417 pyloghub-0.1.3/pyloghub/sample_data/
+-rw-rw-rw-   0        0        0    15659 2023-12-14 16:26:34.000000 pyloghub-0.1.3/pyloghub/sample_data/COGPlusSampleDataAddresses.xlsx
+-rw-rw-rw-   0        0        0    15903 2023-12-14 16:26:46.000000 pyloghub-0.1.3/pyloghub/sample_data/COGPlusSampleDataReverse.xlsx
+-rw-rw-rw-   0        0        0    16985 2023-12-14 16:26:57.000000 pyloghub-0.1.3/pyloghub/sample_data/COGSampleDataAddresses.xlsx
+-rw-rw-rw-   0        0        0    16665 2023-12-14 16:27:09.000000 pyloghub-0.1.3/pyloghub/sample_data/COGSampleDataReverse.xlsx
+-rw-rw-rw-   0        0        0    13101 2023-12-14 16:27:20.000000 pyloghub-0.1.3/pyloghub/sample_data/DistanceCalcSampleDataAddresses.xlsx
+-rw-rw-rw-   0        0        0    12986 2023-12-14 16:27:30.000000 pyloghub-0.1.3/pyloghub/sample_data/DistanceCalcSampleDataReverse.xlsx
+-rw-rw-rw-   0        0        0    36539 2023-12-14 16:27:40.000000 pyloghub-0.1.3/pyloghub/sample_data/FixedCOGSampleDataAddresses.xlsx
+-rw-rw-rw-   0        0        0    33868 2023-12-14 16:27:52.000000 pyloghub-0.1.3/pyloghub/sample_data/FixedCOGSampleDataReverse.xlsx
+-rw-rw-rw-   0        0        0    14535 2023-12-14 16:28:03.000000 pyloghub-0.1.3/pyloghub/sample_data/GeocodingSampleDataAddresses.xlsx
+-rw-rw-rw-   0        0        0    13881 2023-12-14 16:28:13.000000 pyloghub-0.1.3/pyloghub/sample_data/GeocodingSampleDataReverse.xlsx
+-rw-rw-rw-   0        0        0    33828 2023-12-14 16:28:24.000000 pyloghub-0.1.3/pyloghub/sample_data/MilkrunPlusSampleDataAddresses.xlsx
+-rw-rw-rw-   0        0        0    26624 2023-12-14 16:28:36.000000 pyloghub-0.1.3/pyloghub/sample_data/MilkrunPlusSampleDataReverse.xlsx
+-rw-rw-rw-   0        0        0    61039 2024-02-22 09:09:10.000000 pyloghub-0.1.3/pyloghub/sample_data/freightMatrixAddresses.xlsx
+-rw-rw-rw-   0        0        0    58815 2024-02-22 09:19:34.000000 pyloghub-0.1.3/pyloghub/sample_data/freightMatrixReverse.xlsx
+-rw-rw-rw-   0        0        0    54710 2023-12-14 16:28:50.000000 pyloghub-0.1.3/pyloghub/sample_data/shipmentAnalyzerAddresses.xlsx
+-rw-rw-rw-   0        0        0    47612 2023-12-14 16:29:02.000000 pyloghub-0.1.3/pyloghub/sample_data/shipmentAnalyzerReverse.xlsx
+-rw-rw-rw-   0        0        0    22689 2023-12-14 16:29:13.000000 pyloghub-0.1.3/pyloghub/sample_data/transportPlusAddresses.xlsx
+-rw-rw-rw-   0        0        0    22883 2023-12-14 16:29:24.000000 pyloghub-0.1.3/pyloghub/sample_data/transportPlusReverse.xlsx
+-rw-rw-rw-   0        0        0    16492 2024-04-16 09:32:36.000000 pyloghub-0.1.3/pyloghub/shipment_analyzer.py
+-rw-rw-rw-   0        0        0    18698 2024-04-16 09:29:52.000000 pyloghub-0.1.3/pyloghub/transport_optimization_plus.py
+drwxrwxrwx   0        0        0        0 2024-04-16 13:05:35.349455 pyloghub-0.1.3/pyloghub.egg-info/
+-rw-rw-rw-   0        0        0    14087 2024-04-16 13:05:35.000000 pyloghub-0.1.3/pyloghub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1518 2024-04-16 13:05:35.000000 pyloghub-0.1.3/pyloghub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 13:05:35.000000 pyloghub-0.1.3/pyloghub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-04-16 13:05:35.000000 pyloghub-0.1.3/pyloghub.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-16 13:05:35.000000 pyloghub-0.1.3/pyloghub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 13:05:35.355486 pyloghub-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      957 2024-04-16 13:00:52.000000 pyloghub-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 13:05:35.346941 pyloghub-0.1.3/tests/
+-rw-rw-rw-   0        0        0        0 2023-12-08 11:11:58.000000 pyloghub-0.1.3/tests/__init__.py
+-rw-rw-rw-   0        0        0     2655 2023-12-14 17:18:16.000000 pyloghub-0.1.3/tests/test_geocoding.py
```

### Comparing `pyloghub-0.1.2/LICENSE` & `pyloghub-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyloghub-0.1.2/PKG-INFO` & `pyloghub-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pyloghub
-Version: 0.1.2
+Version: 0.1.3
 Summary: The `pyloghub` package provides convinient access to various Log-hub API services for Supply Chain Visualization, Network Design Optimization, and Transport Optimization as well as access to the Log-hub platform data.
 Home-page: https://github.com/log-hub/log-hub-python
 Author: Log-hub AG
 Author-email: support@log-hub.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
+Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: openpyxl
 Requires-Dist: python-dotenv
 
 <p align="center">
   <img src="assets/log-hub-github-header.png" alt="Header Image" width="980"/>
 </p>
@@ -133,15 +134,18 @@
 
 ## Available Functionalities
 
 ### Overview
 
 `pyloghub` offers a suite of functionalities to enhance your supply chain management processes. Below is a quick guide to the available features and sample usage for each.
 
-### Geocoding
+<p align="left">
+  <img src="examples\assets\geocoding.png" alt="Header Image"  width="980"/>
+</p>
+
 #### Forward Geocoding
 Convert addresses to geographic coordinates.
 
 ```python
 from pyloghub.geocoding import forward_geocoding, forward_geocoding_sample_data
 
 sample_data = forward_geocoding_sample_data()
@@ -156,15 +160,18 @@
 from pyloghub.geocoding import reverse_geocoding, reverse_geocoding_sample_data
 
 sample_data = reverse_geocoding_sample_data()
 geocodes_df = sample_data['geocodes']
 reverse_geocoding_result_df = reverse_geocoding(geocodes_df, api_key)
 ```
 
-### Distance Calculation
+<p align="left">
+  <img src="examples\assets\distance_calculation.png" alt="Header Image"  width="980"/>
+</p>
+
 #### Forward Distance Calculation
 Calculate distances based on address data.
 
 ```python
 from pyloghub.distance_calculation import forward_distance_calculation, forward_distance_calculation_sample_data
 
 sample_data = forward_distance_calculation_sample_data()
@@ -181,15 +188,18 @@
 
 sample_data = reverse_distance_calculation_sample_data()
 geocode_data_df = sample_data['geocode_data']
 parameters = sample_data['parameters']
 reverse_center_of_gravity_result_df = reverse_distance_calculation(geocode_data_df, parameters, api_key)
 ```
 
-### Center of Gravity
+<p align="left">
+  <img src="examples\assets\center_of_gravity.png" alt="Header Image"  width="980"/>
+</p>
+
 #### Forward Center of Gravity
 Determine optimal facility locations based on addresses.
 
 ```python
 from pyloghub.center_of_gravity import forward_center_of_gravity, forward_center_of_gravity_sample_data
 
 sample_data = forward_center_of_gravity_sample_data()
@@ -206,15 +216,18 @@
 
 sample_data = reverse_center_of_gravity_sample_data()
 coordinates_df = sample_data['coordinates']
 parameters = sample_data['parameters']
 assigned_geocodes_df, centers_df = reverse_center_of_gravity(coordinates_df, parameters, api_key)
 ```
 
-### Transport Optimization
+<p align="left">
+  <img src="examples\assets\milkrun_optimization.png" alt="Header Image"  width="980"/>
+</p>
+
 #### Milkrun Optimization Plus
 Optimize delivery routes with multiple stops.
 
 ```python
 from pyloghub.milkrun_optimization_plus import forward_milkrun_optimization_plus, forward_milkrun_optimization_plus_sample_data
 
 sample_data = forward_milkrun_optimization_plus_sample_data()
@@ -224,14 +237,18 @@
 timeWindowProfiles_df = sample_data['timeWindowProfiles']
 breaks_df = sample_data['breaks']
 parameters = sample_data['parameters']
 
 route_overview_df, route_details_df, external_orders_df  = forward_milkrun_optimization_plus(depots_df, vehicles_df, jobs_df, timeWindowProfiles_df, breaks_df, parameters, api_key)
 ```
 
+<p align="left">
+  <img src="examples\assets\transport_optimization.png" alt="Header Image"  width="980"/>
+</p>
+
 #### Transport Optimization Plus
 Optimize transport routes for shipments.
 
 ```python
 from pyloghub.transport_optimization_plus import forward_transport_optimization_plus, forward_transport_optimization_plus_sample_data
 
 sample_data = forward_transport_optimization_plus_sample_data()
@@ -240,14 +257,18 @@
 timeWindowProfiles_df = sample_data['timeWindowProfiles']
 breaks_df = sample_data['breaks']
 parameters = sample_data['parameters']
 
 route_overview_df, route_details_df, external_orders_df = forward_transport_optimization_plus(vehicles_df, shipments_df, timeWindowProfiles_df, breaks_df, parameters, api_key)
 ```
 
+<p align="left">
+  <img src="examples\assets\shipment_analyzer.png" alt="Header Image"  width="980"/>
+</p>
+
 #### Shipment Analyzer
 Analyze and optimize shipment costs and operations.
 
 ```python
 from pyloghub.shipment_analyzer import forward_shipment_analyzer, forward_shipment_analyzer_sample_data
 
 sample_data = forward_shipment_analyzer_sample_data()
@@ -258,14 +279,48 @@
 parameters = sample_data['parameters']
 
 shipments_analysis_df, transports_analysis_df = forward_shipment_analyzer(shipments_df, transport_costs_adjustments_df, consolidation_df, surcharges_df, parameters, api_key)
 ```
 
 For the Milkrun Optimization, Transport Optimization as well as the Shipment Analyzer service there is also the reverse version available.
 
+<p align="left">
+  <img src="examples\assets\freight_matrix.png" alt="Header Image"  width="980"/>
+</p>
+
+#### Freight Matrix
+Evaluate shipments with costs based on your own freight cost matrices. The following matrix types are supported:
+
+* Absolute weight distance matrix
+* Relative weight distance matrix
+* Absolute weight zone matrix
+* Relative weight zone matrix
+* Zone zone matrix
+* Absolute weight zone distance matrix
+* Relative weight zone distance matrix
+
+```python
+from pyloghub.freight_matrix import forward_freight_matrix, forward_freight_matrix_sample_data
+
+sample_data = forward_freight_matrix_sample_data()
+shipments_df = sample_data['shipments']
+matrix_id = "Your freight matrix id"
+
+evaluated_shipments_df = forward_freight_matrix(shipments_df, matrix_id, api_key)
+evaluated_shipments_df
+```
+You can create a freight matrix on the Log-hub Platform. Therefore, please create a workspace and click within the workspace on "Create Freight Matrix". There you can provide the matrix a name, select the matrix type and define all other parameters. 
+To get the matrix id, please click on the "gear" icon. There you can copy & paste the matrix id that is needed in your API request.
+
+
+<p align="left">
+  <img src="examples\assets\log_hub_tables.png" alt="Header Image"  width="980"/>
+</p>
+
+
 ### Working with Log-hub Tables
 
 To read or update a table, you need a table link from a table in the Log-hub platform. Therefore, please navigate in a workspace with an existing dataset and go to the table you would like to read or update. Click on the "three dots" and click on "Table Link". Then copy the corresponding table link. If no table exists create a dataset and a new table via the GUI.
 
 #### Reading Data from a Table
 The read_table function simplifies the process of fetching and formatting data from a specific table on the Log-hub platform into a pandas DataFrame. This function ensures that the data types in the DataFrame match those in the Log-hub table, leveraging metadata from the table for precise formatting.
```

### Comparing `pyloghub-0.1.2/README.md` & `pyloghub-0.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -115,15 +115,18 @@
 
 ## Available Functionalities
 
 ### Overview
 
 `pyloghub` offers a suite of functionalities to enhance your supply chain management processes. Below is a quick guide to the available features and sample usage for each.
 
-### Geocoding
+<p align="left">
+  <img src="examples\assets\geocoding.png" alt="Header Image"  width="980"/>
+</p>
+
 #### Forward Geocoding
 Convert addresses to geographic coordinates.
 
 ```python
 from pyloghub.geocoding import forward_geocoding, forward_geocoding_sample_data
 
 sample_data = forward_geocoding_sample_data()
@@ -138,15 +141,18 @@
 from pyloghub.geocoding import reverse_geocoding, reverse_geocoding_sample_data
 
 sample_data = reverse_geocoding_sample_data()
 geocodes_df = sample_data['geocodes']
 reverse_geocoding_result_df = reverse_geocoding(geocodes_df, api_key)
 ```
 
-### Distance Calculation
+<p align="left">
+  <img src="examples\assets\distance_calculation.png" alt="Header Image"  width="980"/>
+</p>
+
 #### Forward Distance Calculation
 Calculate distances based on address data.
 
 ```python
 from pyloghub.distance_calculation import forward_distance_calculation, forward_distance_calculation_sample_data
 
 sample_data = forward_distance_calculation_sample_data()
@@ -163,15 +169,18 @@
 
 sample_data = reverse_distance_calculation_sample_data()
 geocode_data_df = sample_data['geocode_data']
 parameters = sample_data['parameters']
 reverse_center_of_gravity_result_df = reverse_distance_calculation(geocode_data_df, parameters, api_key)
 ```
 
-### Center of Gravity
+<p align="left">
+  <img src="examples\assets\center_of_gravity.png" alt="Header Image"  width="980"/>
+</p>
+
 #### Forward Center of Gravity
 Determine optimal facility locations based on addresses.
 
 ```python
 from pyloghub.center_of_gravity import forward_center_of_gravity, forward_center_of_gravity_sample_data
 
 sample_data = forward_center_of_gravity_sample_data()
@@ -188,15 +197,18 @@
 
 sample_data = reverse_center_of_gravity_sample_data()
 coordinates_df = sample_data['coordinates']
 parameters = sample_data['parameters']
 assigned_geocodes_df, centers_df = reverse_center_of_gravity(coordinates_df, parameters, api_key)
 ```
 
-### Transport Optimization
+<p align="left">
+  <img src="examples\assets\milkrun_optimization.png" alt="Header Image"  width="980"/>
+</p>
+
 #### Milkrun Optimization Plus
 Optimize delivery routes with multiple stops.
 
 ```python
 from pyloghub.milkrun_optimization_plus import forward_milkrun_optimization_plus, forward_milkrun_optimization_plus_sample_data
 
 sample_data = forward_milkrun_optimization_plus_sample_data()
@@ -206,14 +218,18 @@
 timeWindowProfiles_df = sample_data['timeWindowProfiles']
 breaks_df = sample_data['breaks']
 parameters = sample_data['parameters']
 
 route_overview_df, route_details_df, external_orders_df  = forward_milkrun_optimization_plus(depots_df, vehicles_df, jobs_df, timeWindowProfiles_df, breaks_df, parameters, api_key)
 ```
 
+<p align="left">
+  <img src="examples\assets\transport_optimization.png" alt="Header Image"  width="980"/>
+</p>
+
 #### Transport Optimization Plus
 Optimize transport routes for shipments.
 
 ```python
 from pyloghub.transport_optimization_plus import forward_transport_optimization_plus, forward_transport_optimization_plus_sample_data
 
 sample_data = forward_transport_optimization_plus_sample_data()
@@ -222,14 +238,18 @@
 timeWindowProfiles_df = sample_data['timeWindowProfiles']
 breaks_df = sample_data['breaks']
 parameters = sample_data['parameters']
 
 route_overview_df, route_details_df, external_orders_df = forward_transport_optimization_plus(vehicles_df, shipments_df, timeWindowProfiles_df, breaks_df, parameters, api_key)
 ```
 
+<p align="left">
+  <img src="examples\assets\shipment_analyzer.png" alt="Header Image"  width="980"/>
+</p>
+
 #### Shipment Analyzer
 Analyze and optimize shipment costs and operations.
 
 ```python
 from pyloghub.shipment_analyzer import forward_shipment_analyzer, forward_shipment_analyzer_sample_data
 
 sample_data = forward_shipment_analyzer_sample_data()
@@ -240,14 +260,48 @@
 parameters = sample_data['parameters']
 
 shipments_analysis_df, transports_analysis_df = forward_shipment_analyzer(shipments_df, transport_costs_adjustments_df, consolidation_df, surcharges_df, parameters, api_key)
 ```
 
 For the Milkrun Optimization, Transport Optimization as well as the Shipment Analyzer service there is also the reverse version available.
 
+<p align="left">
+  <img src="examples\assets\freight_matrix.png" alt="Header Image"  width="980"/>
+</p>
+
+#### Freight Matrix
+Evaluate shipments with costs based on your own freight cost matrices. The following matrix types are supported:
+
+* Absolute weight distance matrix
+* Relative weight distance matrix
+* Absolute weight zone matrix
+* Relative weight zone matrix
+* Zone zone matrix
+* Absolute weight zone distance matrix
+* Relative weight zone distance matrix
+
+```python
+from pyloghub.freight_matrix import forward_freight_matrix, forward_freight_matrix_sample_data
+
+sample_data = forward_freight_matrix_sample_data()
+shipments_df = sample_data['shipments']
+matrix_id = "Your freight matrix id"
+
+evaluated_shipments_df = forward_freight_matrix(shipments_df, matrix_id, api_key)
+evaluated_shipments_df
+```
+You can create a freight matrix on the Log-hub Platform. Therefore, please create a workspace and click within the workspace on "Create Freight Matrix". There you can provide the matrix a name, select the matrix type and define all other parameters. 
+To get the matrix id, please click on the "gear" icon. There you can copy & paste the matrix id that is needed in your API request.
+
+
+<p align="left">
+  <img src="examples\assets\log_hub_tables.png" alt="Header Image"  width="980"/>
+</p>
+
+
 ### Working with Log-hub Tables
 
 To read or update a table, you need a table link from a table in the Log-hub platform. Therefore, please navigate in a workspace with an existing dataset and go to the table you would like to read or update. Click on the "three dots" and click on "Table Link". Then copy the corresponding table link. If no table exists create a dataset and a new table via the GUI.
 
 #### Reading Data from a Table
 The read_table function simplifies the process of fetching and formatting data from a specific table on the Log-hub platform into a pandas DataFrame. This function ensures that the data types in the DataFrame match those in the Log-hub table, leveraging metadata from the table for precise formatting.
```

### Comparing `pyloghub-0.1.2/pyloghub/center_of_gravity.py` & `pyloghub-0.1.3/pyloghub/center_of_gravity.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,15 +59,18 @@
         return df
 
     # Validate and convert data types
     addresses = validate_and_convert_data_types(addresses)
     if addresses is None:
         return None
     
-    url = "https://production.supply-chain-apps.log-hub.com/api/applications/v1/centerofgravity"
+    DEFAULT_LOG_HUB_API_SERVER = "https://production.supply-chain-apps.log-hub.com"
+    LOG_HUB_API_SERVER = os.getenv('LOG_HUB_API_SERVER', DEFAULT_LOG_HUB_API_SERVER)
+    url = f"{LOG_HUB_API_SERVER}/api/applications/v1/centerofgravity"
+    
     headers = {
         "accept": "application/json",
         "authorization": f"apikey {api_key}",
         "content-type": "application/json"
     }
     payload = {
         "addresses": addresses.to_dict(orient='records'),
@@ -160,15 +163,18 @@
         return df
 
     # Validate and convert data types
     coordinates = validate_and_convert_data_types(coordinates)
     if coordinates is None:
         return None
 
-    url = "https://production.supply-chain-apps.log-hub.com/api/applications/v1/reversecenterofgravity"
+    DEFAULT_LOG_HUB_API_SERVER = "https://production.supply-chain-apps.log-hub.com"
+    LOG_HUB_API_SERVER = os.getenv('LOG_HUB_API_SERVER', DEFAULT_LOG_HUB_API_SERVER)
+    url = f"{LOG_HUB_API_SERVER}/api/applications/v1/reversecenterofgravity"
+    
     headers = {
         "accept": "application/json",
         "authorization": f"apikey {api_key}",
         "content-type": "application/json"
     }
     payload = {
         "coordinates": coordinates.to_dict(orient='records'),
```

### Comparing `pyloghub-0.1.2/pyloghub/center_of_gravity_plus.py` & `pyloghub-0.1.3/pyloghub/center_of_gravity_plus.py`

 * *Files 14% similar despite different names*

```diff
@@ -61,15 +61,18 @@
         return df
 
     # Validate and convert data types
     addresses = validate_and_convert_data_types(addresses)
     if addresses is None:
         return None
 
-    url = "https://production.supply-chain-apps.log-hub.com/api/applications/v1/centerofgravityplus"
+    DEFAULT_LOG_HUB_API_SERVER = "https://production.supply-chain-apps.log-hub.com"
+    LOG_HUB_API_SERVER = os.getenv('LOG_HUB_API_SERVER', DEFAULT_LOG_HUB_API_SERVER)
+    url = f"{LOG_HUB_API_SERVER}/api/applications/v1/centerofgravityplus"
+    
     headers = {
         "accept": "application/json",
         "authorization": f"apikey {api_key}",
         "content-type": "application/json"
     }
     payload = {
         "addresses": addresses.to_dict(orient='records'),
@@ -169,15 +172,18 @@
         return df
 
     # Validate and convert data types
     coordinates = validate_and_convert_data_types(coordinates)
     if coordinates is None:
         return None
 
-    url = "https://production.supply-chain-apps.log-hub.com/api/applications/v1/reversecenterofgravityplus"
+    DEFAULT_LOG_HUB_API_SERVER = "https://production.supply-chain-apps.log-hub.com"
+    LOG_HUB_API_SERVER = os.getenv('LOG_HUB_API_SERVER', DEFAULT_LOG_HUB_API_SERVER)
+    url = f"{LOG_HUB_API_SERVER}/api/applications/v1/reversecenterofgravityplus"
+    
     headers = {
         "accept": "application/json",
         "authorization": f"apikey {api_key}",
         "content-type": "application/json"
     }
     payload = {
         "coordinates": coordinates.to_dict(orient='records'),
```

### Comparing `pyloghub-0.1.2/pyloghub/dataset.py` & `pyloghub-0.1.3/pyloghub/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,15 +254,17 @@
     # Prepare data for update including the table name and columns metadata
     update_data = {
         "name": table_name,
         "columns": metadata['columns'],
         "rows": dataframe.to_dict(orient='records')
     }
 
-    url = f"https://production.supply-chain-apps.log-hub.com/api/v1/datasets/{dataset_id}/tables/{table_id}"
+    DEFAULT_LOG_HUB_API_SERVER = "https://production.supply-chain-apps.log-hub.com"
+    LOG_HUB_API_SERVER = os.getenv('LOG_HUB_API_SERVER', DEFAULT_LOG_HUB_API_SERVER)
+    url = f"{LOG_HUB_API_SERVER}/api/v1/datasets/{dataset_id}/tables/{table_id}"
 
     try:
         # Send PATCH request
         response = requests.patch(url, headers=headers, data=json.dumps(update_data))
 
         # Check if the request was successful
         if response.status_code == 200:
```

### Comparing `pyloghub-0.1.2/pyloghub/distance_calculation.py` & `pyloghub-0.1.3/pyloghub/distance_calculation.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,18 @@
         return df
 
     # Validate and convert data types
     address_pairs = validate_and_convert_data_types(address_pairs)
     if address_pairs is None:
         return None
 
-    url = "https://production.supply-chain-apps.log-hub.com/api/applications/v1/distancecalculation"
+    DEFAULT_LOG_HUB_API_SERVER = "https://production.supply-chain-apps.log-hub.com"
+    LOG_HUB_API_SERVER = os.getenv('LOG_HUB_API_SERVER', DEFAULT_LOG_HUB_API_SERVER)
+    url = f"{LOG_HUB_API_SERVER}/api/applications/v1/distancecalculation"
+    
     headers = {
         "accept": "application/json",
         "authorization": f"apikey {api_key}",
         "content-type": "application/json"
     }
     batch_size = 5000
     max_retries = 3
@@ -187,16 +190,18 @@
         return df
 
     # Validate and convert data types
     geocodes = validate_and_convert_data_types(geocodes)
     if geocodes is None:
         return None
 
-
-    url = "https://production.supply-chain-apps.log-hub.com/api/applications/v1/reversedistancecalculation"
+    DEFAULT_LOG_HUB_API_SERVER = "https://production.supply-chain-apps.log-hub.com"
+    LOG_HUB_API_SERVER = os.getenv('LOG_HUB_API_SERVER', DEFAULT_LOG_HUB_API_SERVER)
+    url = f"{LOG_HUB_API_SERVER}/api/applications/v1/reversedistancecalculation"
+    
     headers = {
         "accept": "application/json",
         "authorization": f"apikey {api_key}",
         "content-type": "application/json"
     }
     batch_size = 5000
     max_retries = 3
```

### Comparing `pyloghub-0.1.2/pyloghub/fixed_center_of_gravity.py` & `pyloghub-0.1.3/pyloghub/fixed_center_of_gravity.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,15 +76,18 @@
 
     # Validate and convert data types for customers and fixed centers
     customers = validate_and_convert_data_types(customers, customer_columns)
     fixed_centers = validate_and_convert_data_types(fixed_centers, fixed_center_columns) if not fixed_centers.empty else fixed_centers
     if customers is None or (not fixed_centers.empty and fixed_centers is None):
         return None
     
-    url = "https://production.supply-chain-apps.log-hub.com/api/applications/v1/fixedcenterofgravity"
+    DEFAULT_LOG_HUB_API_SERVER = "https://production.supply-chain-apps.log-hub.com"
+    LOG_HUB_API_SERVER = os.getenv('LOG_HUB_API_SERVER', DEFAULT_LOG_HUB_API_SERVER)
+    url = f"{LOG_HUB_API_SERVER}/api/applications/v1/fixedcenterofgravity"
+    
     headers = {
         "accept": "application/json",
         "authorization": f"apikey {api_key}",
         "content-type": "application/json"
     }
 
     payload = {
@@ -192,15 +195,18 @@
 
     # Validate and convert data types for customers and fixed centers
     customers = validate_and_convert_data_types(customers, customer_columns)
     fixed_centers = validate_and_convert_data_types(fixed_centers, fixed_center_columns) if not fixed_centers.empty else fixed_centers
     if customers is None or (not fixed_centers.empty and fixed_centers is None):
         return None
 
-    url = "https://production.supply-chain-apps.log-hub.com/api/applications/v1/reversefixedcenterofgravity"
+    DEFAULT_LOG_HUB_API_SERVER = "https://production.supply-chain-apps.log-hub.com"
+    LOG_HUB_API_SERVER = os.getenv('LOG_HUB_API_SERVER', DEFAULT_LOG_HUB_API_SERVER)
+    url = f"{LOG_HUB_API_SERVER}/api/applications/v1/reversefixedcenterofgravity"
+    
     headers = {
         "accept": "application/json",
         "authorization": f"apikey {api_key}",
         "content-type": "application/json"
     }
 
     payload = {
```

### Comparing `pyloghub-0.1.2/pyloghub/geocoding.py` & `pyloghub-0.1.3/pyloghub/geocoding.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,18 @@
     # Validate and convert data types
     addresses = validate_and_convert_data_types(addresses)
     if addresses is None:
         return None
 
     addresses = addresses.fillna("")
     
-    url = "https://production.supply-chain-apps.log-hub.com/api/applications/v1/geocoding"
+    DEFAULT_LOG_HUB_API_SERVER = "https://production.supply-chain-apps.log-hub.com"
+    LOG_HUB_API_SERVER = os.getenv('LOG_HUB_API_SERVER', DEFAULT_LOG_HUB_API_SERVER)
+    url = f"{LOG_HUB_API_SERVER}/api/applications/v1/geocoding"
+    
     headers = {
         "accept": "application/json",
         "authorization": f"apikey {api_key}",
         "content-type": "application/json"
     }
     batch_size = 5000
     max_retries = 3
@@ -170,17 +173,19 @@
     
     # Convert the list of lists to a list of dictionaries
     geocodes = [{"latitude": lat, "longitude": lon} for lat, lon in geocodes]
     
     # Convert the list of dictionaries to a pandas DataFrame
     geocodes = pd.DataFrame(geocodes)
     
-    # Convert the latitude and longitude columns to float64
     
-    url = "https://production.supply-chain-apps.log-hub.com/api/applications/v1/reversegeocoding"
+    DEFAULT_LOG_HUB_API_SERVER = "https://production.supply-chain-apps.log-hub.com"
+    LOG_HUB_API_SERVER = os.getenv('LOG_HUB_API_SERVER', DEFAULT_LOG_HUB_API_SERVER)
+    url = f"{LOG_HUB_API_SERVER}/api/applications/v1/reversegeocoding"
+
     headers = {
         "accept": "application/json",
         "authorization": f"apikey {api_key}",
         "content-type": "application/json"
     }
     batch_size = 5000
     max_retries = 3
```

### Comparing `pyloghub-0.1.2/pyloghub/milkrun_optimization_plus.py` & `pyloghub-0.1.3/pyloghub/milkrun_optimization_plus.py`

 * *Files 5% similar despite different names*

```diff
@@ -143,16 +143,18 @@
     timeWindowProfiles = validate_and_convert_data_types(timeWindowProfiles, timeWindowProfile_columns)
     breaks = validate_and_convert_data_types(breaks, break_columns)
 
     # Exit if any DataFrame validation failed
     if any(df is None for df in [depots, vehicles, jobs, timeWindowProfiles, breaks]):
         return None
 
-
-    url = "https://production.supply-chain-apps.log-hub.com/api/applications/v1/milkrunoptimizationplus"
+    DEFAULT_LOG_HUB_API_SERVER = "https://production.supply-chain-apps.log-hub.com"
+    LOG_HUB_API_SERVER = os.getenv('LOG_HUB_API_SERVER', DEFAULT_LOG_HUB_API_SERVER)
+    url = f"{LOG_HUB_API_SERVER}/api/applications/v1/milkrunoptimizationplus"
+    
     headers = {
         "accept": "application/json",
         "authorization": f"apikey {api_key}",
         "content-type": "application/json"
     }
 
     payload = {
@@ -329,15 +331,18 @@
     timeWindowProfiles = validate_and_convert_data_types(timeWindowProfiles, timeWindowProfile_columns)
     breaks = validate_and_convert_data_types(breaks, break_columns)
 
     # Exit if any DataFrame validation failed
     if any(df is None for df in [depots, vehicles, jobs, timeWindowProfiles, breaks]):
         return None
 
-    url = "https://production.supply-chain-apps.log-hub.com/api/applications/v1/reversemilkrunoptimizationplus"
+    DEFAULT_LOG_HUB_API_SERVER = "https://production.supply-chain-apps.log-hub.com"
+    LOG_HUB_API_SERVER = os.getenv('LOG_HUB_API_SERVER', DEFAULT_LOG_HUB_API_SERVER)
+    url = f"{LOG_HUB_API_SERVER}/api/applications/v1/reversemilkrunoptimizationplus"
+    
     headers = {
         "accept": "application/json",
         "authorization": f"apikey {api_key}",
         "content-type": "application/json"
     }
 
     payload = {
```

### Comparing `pyloghub-0.1.2/pyloghub/sample_data/COGPlusSampleDataAddresses.xlsx` & `pyloghub-0.1.3/pyloghub/sample_data/COGPlusSampleDataAddresses.xlsx`

 * *Files identical despite different names*

### Comparing `pyloghub-0.1.2/pyloghub/sample_data/COGPlusSampleDataReverse.xlsx` & `pyloghub-0.1.3/pyloghub/sample_data/COGPlusSampleDataReverse.xlsx`

 * *Files identical despite different names*

### Comparing `pyloghub-0.1.2/pyloghub/sample_data/COGSampleDataAddresses.xlsx` & `pyloghub-0.1.3/pyloghub/sample_data/COGSampleDataAddresses.xlsx`

 * *Files identical despite different names*

### Comparing `pyloghub-0.1.2/pyloghub/sample_data/COGSampleDataReverse.xlsx` & `pyloghub-0.1.3/pyloghub/sample_data/COGSampleDataReverse.xlsx`

 * *Files identical despite different names*

### Comparing `pyloghub-0.1.2/pyloghub/sample_data/DistanceCalcSampleDataAddresses.xlsx` & `pyloghub-0.1.3/pyloghub/sample_data/DistanceCalcSampleDataAddresses.xlsx`

 * *Files identical despite different names*

### Comparing `pyloghub-0.1.2/pyloghub/sample_data/DistanceCalcSampleDataReverse.xlsx` & `pyloghub-0.1.3/pyloghub/sample_data/DistanceCalcSampleDataReverse.xlsx`

 * *Files identical despite different names*

### Comparing `pyloghub-0.1.2/pyloghub/sample_data/FixedCOGSampleDataAddresses.xlsx` & `pyloghub-0.1.3/pyloghub/sample_data/FixedCOGSampleDataAddresses.xlsx`

 * *Files identical despite different names*

### Comparing `pyloghub-0.1.2/pyloghub/sample_data/FixedCOGSampleDataReverse.xlsx` & `pyloghub-0.1.3/pyloghub/sample_data/FixedCOGSampleDataReverse.xlsx`

 * *Files identical despite different names*

### Comparing `pyloghub-0.1.2/pyloghub/sample_data/GeocodingSampleDataAddresses.xlsx` & `pyloghub-0.1.3/pyloghub/sample_data/GeocodingSampleDataAddresses.xlsx`

 * *Files identical despite different names*

### Comparing `pyloghub-0.1.2/pyloghub/sample_data/GeocodingSampleDataReverse.xlsx` & `pyloghub-0.1.3/pyloghub/sample_data/GeocodingSampleDataReverse.xlsx`

 * *Files identical despite different names*

### Comparing `pyloghub-0.1.2/pyloghub/sample_data/MilkrunPlusSampleDataAddresses.xlsx` & `pyloghub-0.1.3/pyloghub/sample_data/MilkrunPlusSampleDataAddresses.xlsx`

 * *Files identical despite different names*

### Comparing `pyloghub-0.1.2/pyloghub/sample_data/MilkrunPlusSampleDataReverse.xlsx` & `pyloghub-0.1.3/pyloghub/sample_data/MilkrunPlusSampleDataReverse.xlsx`

 * *Files identical despite different names*

### Comparing `pyloghub-0.1.2/pyloghub/sample_data/shipmentAnalyzerAddresses.xlsx` & `pyloghub-0.1.3/pyloghub/sample_data/shipmentAnalyzerAddresses.xlsx`

 * *Files identical despite different names*

### Comparing `pyloghub-0.1.2/pyloghub/sample_data/shipmentAnalyzerReverse.xlsx` & `pyloghub-0.1.3/pyloghub/sample_data/shipmentAnalyzerReverse.xlsx`

 * *Files identical despite different names*

### Comparing `pyloghub-0.1.2/pyloghub/sample_data/transportPlusAddresses.xlsx` & `pyloghub-0.1.3/pyloghub/sample_data/transportPlusAddresses.xlsx`

 * *Files identical despite different names*

### Comparing `pyloghub-0.1.2/pyloghub/sample_data/transportPlusReverse.xlsx` & `pyloghub-0.1.3/pyloghub/sample_data/transportPlusReverse.xlsx`

 * *Files identical despite different names*

### Comparing `pyloghub-0.1.2/pyloghub/shipment_analyzer.py` & `pyloghub-0.1.3/pyloghub/shipment_analyzer.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,15 +109,18 @@
     surcharges = convert_to_float(surcharges, ['flatOnTop'])
 
     # Validate boolean parameter
     if 'consolidation' in parameters and not validate_boolean(parameters['consolidation']):
         logging.error("Invalid type for 'consolidation' in parameters. It should be boolean.")
         return None
 
-    url = "https://production.supply-chain-apps.log-hub.com/api/applications/v1/shipmentanalyzerplus"
+    DEFAULT_LOG_HUB_API_SERVER = "https://production.supply-chain-apps.log-hub.com"
+    LOG_HUB_API_SERVER = os.getenv('LOG_HUB_API_SERVER', DEFAULT_LOG_HUB_API_SERVER)
+    url = f"{LOG_HUB_API_SERVER}/api/applications/v1/shipmentanalyzerplus"
+    
     headers = {
         "accept": "application/json",
         "authorization": f"apikey {api_key}",
         "content-type": "application/json"
     }
 
     payload = {
@@ -252,16 +255,18 @@
     # Convert and validate other dataframes as in forward_shipment_analyzer...
 
     # Validate boolean parameter
     if 'consolidation' in parameters and not validate_boolean(parameters['consolidation']):
         logging.error("Invalid type for 'consolidation' in parameters. It should be boolean.")
         return None
 
-    # API call with the modified URL
-    url = "https://production.supply-chain-apps.log-hub.com/api/applications/v1/reverseshipmentanalyzerplus"
+    DEFAULT_LOG_HUB_API_SERVER = "https://production.supply-chain-apps.log-hub.com"
+    LOG_HUB_API_SERVER = os.getenv('LOG_HUB_API_SERVER', DEFAULT_LOG_HUB_API_SERVER)
+    url = f"{LOG_HUB_API_SERVER}/api/applications/v1/reverseshipmentanalyzerplus"
+    
     headers = {
         "accept": "application/json",
         "authorization": f"apikey {api_key}",
         "content-type": "application/json"
     }
 
     payload = {
```

### Comparing `pyloghub-0.1.2/pyloghub/transport_optimization_plus.py` & `pyloghub-0.1.3/pyloghub/transport_optimization_plus.py`

 * *Files 6% similar despite different names*

```diff
@@ -131,15 +131,18 @@
     timeWindowProfiles = validate_and_convert_data_types(timeWindowProfiles, timeWindowProfile_columns)
     breaks = validate_and_convert_data_types(breaks, break_columns)
 
     # Exit if any DataFrame validation failed
     if any(df is None for df in [vehicles, jobs, timeWindowProfiles, breaks]):
         return None
 
-    url = "https://production.supply-chain-apps.log-hub.com/api/applications/v1/transportoptimizationplus"
+    DEFAULT_LOG_HUB_API_SERVER = "https://production.supply-chain-apps.log-hub.com"
+    LOG_HUB_API_SERVER = os.getenv('LOG_HUB_API_SERVER', DEFAULT_LOG_HUB_API_SERVER)
+    url = f"{LOG_HUB_API_SERVER}/api/applications/v1/transportoptimizationplus"
+    
     headers = {
         "accept": "application/json",
         "authorization": f"apikey {api_key}",
         "content-type": "application/json"
     }
 
     payload = {
@@ -306,15 +309,18 @@
     timeWindowProfiles = validate_and_convert_data_types(timeWindowProfiles, timeWindowProfile_columns)
     breaks = validate_and_convert_data_types(breaks, break_columns)
 
     # Exit if any DataFrame validation failed
     if any(df is None for df in [vehicles, jobs, timeWindowProfiles, breaks]):
         return None
 
-    url = "https://production.supply-chain-apps.log-hub.com/api/applications/v1/reversetransportoptimizationplus"
+    DEFAULT_LOG_HUB_API_SERVER = "https://production.supply-chain-apps.log-hub.com"
+    LOG_HUB_API_SERVER = os.getenv('LOG_HUB_API_SERVER', DEFAULT_LOG_HUB_API_SERVER)
+    url = f"{LOG_HUB_API_SERVER}/api/applications/v1/reversetransportoptimizationplus"
+    
     headers = {
         "accept": "application/json",
         "authorization": f"apikey {api_key}",
         "content-type": "application/json"
     }
 
     payload = {
```

### Comparing `pyloghub-0.1.2/pyloghub.egg-info/PKG-INFO` & `pyloghub-0.1.3/pyloghub.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pyloghub
-Version: 0.1.2
+Version: 0.1.3
 Summary: The `pyloghub` package provides convinient access to various Log-hub API services for Supply Chain Visualization, Network Design Optimization, and Transport Optimization as well as access to the Log-hub platform data.
 Home-page: https://github.com/log-hub/log-hub-python
 Author: Log-hub AG
 Author-email: support@log-hub.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
+Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: openpyxl
 Requires-Dist: python-dotenv
 
 <p align="center">
   <img src="assets/log-hub-github-header.png" alt="Header Image" width="980"/>
 </p>
@@ -133,15 +134,18 @@
 
 ## Available Functionalities
 
 ### Overview
 
 `pyloghub` offers a suite of functionalities to enhance your supply chain management processes. Below is a quick guide to the available features and sample usage for each.
 
-### Geocoding
+<p align="left">
+  <img src="examples\assets\geocoding.png" alt="Header Image"  width="980"/>
+</p>
+
 #### Forward Geocoding
 Convert addresses to geographic coordinates.
 
 ```python
 from pyloghub.geocoding import forward_geocoding, forward_geocoding_sample_data
 
 sample_data = forward_geocoding_sample_data()
@@ -156,15 +160,18 @@
 from pyloghub.geocoding import reverse_geocoding, reverse_geocoding_sample_data
 
 sample_data = reverse_geocoding_sample_data()
 geocodes_df = sample_data['geocodes']
 reverse_geocoding_result_df = reverse_geocoding(geocodes_df, api_key)
 ```
 
-### Distance Calculation
+<p align="left">
+  <img src="examples\assets\distance_calculation.png" alt="Header Image"  width="980"/>
+</p>
+
 #### Forward Distance Calculation
 Calculate distances based on address data.
 
 ```python
 from pyloghub.distance_calculation import forward_distance_calculation, forward_distance_calculation_sample_data
 
 sample_data = forward_distance_calculation_sample_data()
@@ -181,15 +188,18 @@
 
 sample_data = reverse_distance_calculation_sample_data()
 geocode_data_df = sample_data['geocode_data']
 parameters = sample_data['parameters']
 reverse_center_of_gravity_result_df = reverse_distance_calculation(geocode_data_df, parameters, api_key)
 ```
 
-### Center of Gravity
+<p align="left">
+  <img src="examples\assets\center_of_gravity.png" alt="Header Image"  width="980"/>
+</p>
+
 #### Forward Center of Gravity
 Determine optimal facility locations based on addresses.
 
 ```python
 from pyloghub.center_of_gravity import forward_center_of_gravity, forward_center_of_gravity_sample_data
 
 sample_data = forward_center_of_gravity_sample_data()
@@ -206,15 +216,18 @@
 
 sample_data = reverse_center_of_gravity_sample_data()
 coordinates_df = sample_data['coordinates']
 parameters = sample_data['parameters']
 assigned_geocodes_df, centers_df = reverse_center_of_gravity(coordinates_df, parameters, api_key)
 ```
 
-### Transport Optimization
+<p align="left">
+  <img src="examples\assets\milkrun_optimization.png" alt="Header Image"  width="980"/>
+</p>
+
 #### Milkrun Optimization Plus
 Optimize delivery routes with multiple stops.
 
 ```python
 from pyloghub.milkrun_optimization_plus import forward_milkrun_optimization_plus, forward_milkrun_optimization_plus_sample_data
 
 sample_data = forward_milkrun_optimization_plus_sample_data()
@@ -224,14 +237,18 @@
 timeWindowProfiles_df = sample_data['timeWindowProfiles']
 breaks_df = sample_data['breaks']
 parameters = sample_data['parameters']
 
 route_overview_df, route_details_df, external_orders_df  = forward_milkrun_optimization_plus(depots_df, vehicles_df, jobs_df, timeWindowProfiles_df, breaks_df, parameters, api_key)
 ```
 
+<p align="left">
+  <img src="examples\assets\transport_optimization.png" alt="Header Image"  width="980"/>
+</p>
+
 #### Transport Optimization Plus
 Optimize transport routes for shipments.
 
 ```python
 from pyloghub.transport_optimization_plus import forward_transport_optimization_plus, forward_transport_optimization_plus_sample_data
 
 sample_data = forward_transport_optimization_plus_sample_data()
@@ -240,14 +257,18 @@
 timeWindowProfiles_df = sample_data['timeWindowProfiles']
 breaks_df = sample_data['breaks']
 parameters = sample_data['parameters']
 
 route_overview_df, route_details_df, external_orders_df = forward_transport_optimization_plus(vehicles_df, shipments_df, timeWindowProfiles_df, breaks_df, parameters, api_key)
 ```
 
+<p align="left">
+  <img src="examples\assets\shipment_analyzer.png" alt="Header Image"  width="980"/>
+</p>
+
 #### Shipment Analyzer
 Analyze and optimize shipment costs and operations.
 
 ```python
 from pyloghub.shipment_analyzer import forward_shipment_analyzer, forward_shipment_analyzer_sample_data
 
 sample_data = forward_shipment_analyzer_sample_data()
@@ -258,14 +279,48 @@
 parameters = sample_data['parameters']
 
 shipments_analysis_df, transports_analysis_df = forward_shipment_analyzer(shipments_df, transport_costs_adjustments_df, consolidation_df, surcharges_df, parameters, api_key)
 ```
 
 For the Milkrun Optimization, Transport Optimization as well as the Shipment Analyzer service there is also the reverse version available.
 
+<p align="left">
+  <img src="examples\assets\freight_matrix.png" alt="Header Image"  width="980"/>
+</p>
+
+#### Freight Matrix
+Evaluate shipments with costs based on your own freight cost matrices. The following matrix types are supported:
+
+* Absolute weight distance matrix
+* Relative weight distance matrix
+* Absolute weight zone matrix
+* Relative weight zone matrix
+* Zone zone matrix
+* Absolute weight zone distance matrix
+* Relative weight zone distance matrix
+
+```python
+from pyloghub.freight_matrix import forward_freight_matrix, forward_freight_matrix_sample_data
+
+sample_data = forward_freight_matrix_sample_data()
+shipments_df = sample_data['shipments']
+matrix_id = "Your freight matrix id"
+
+evaluated_shipments_df = forward_freight_matrix(shipments_df, matrix_id, api_key)
+evaluated_shipments_df
+```
+You can create a freight matrix on the Log-hub Platform. Therefore, please create a workspace and click within the workspace on "Create Freight Matrix". There you can provide the matrix a name, select the matrix type and define all other parameters. 
+To get the matrix id, please click on the "gear" icon. There you can copy & paste the matrix id that is needed in your API request.
+
+
+<p align="left">
+  <img src="examples\assets\log_hub_tables.png" alt="Header Image"  width="980"/>
+</p>
+
+
 ### Working with Log-hub Tables
 
 To read or update a table, you need a table link from a table in the Log-hub platform. Therefore, please navigate in a workspace with an existing dataset and go to the table you would like to read or update. Click on the "three dots" and click on "Table Link". Then copy the corresponding table link. If no table exists create a dataset and a new table via the GUI.
 
 #### Reading Data from a Table
 The read_table function simplifies the process of fetching and formatting data from a specific table on the Log-hub platform into a pandas DataFrame. This function ensures that the data types in the DataFrame match those in the Log-hub table, leveraging metadata from the table for precise formatting.
```

### Comparing `pyloghub-0.1.2/pyloghub.egg-info/SOURCES.txt` & `pyloghub-0.1.3/pyloghub.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 setup.py
 pyloghub/__init__.py
 pyloghub/center_of_gravity.py
 pyloghub/center_of_gravity_plus.py
 pyloghub/dataset.py
 pyloghub/distance_calculation.py
 pyloghub/fixed_center_of_gravity.py
+pyloghub/freight_matrix.py
 pyloghub/geocoding.py
 pyloghub/milkrun_optimization_plus.py
 pyloghub/shipment_analyzer.py
 pyloghub/transport_optimization_plus.py
 pyloghub.egg-info/PKG-INFO
 pyloghub.egg-info/SOURCES.txt
 pyloghub.egg-info/dependency_links.txt
@@ -26,13 +27,15 @@
 pyloghub/sample_data/DistanceCalcSampleDataReverse.xlsx
 pyloghub/sample_data/FixedCOGSampleDataAddresses.xlsx
 pyloghub/sample_data/FixedCOGSampleDataReverse.xlsx
 pyloghub/sample_data/GeocodingSampleDataAddresses.xlsx
 pyloghub/sample_data/GeocodingSampleDataReverse.xlsx
 pyloghub/sample_data/MilkrunPlusSampleDataAddresses.xlsx
 pyloghub/sample_data/MilkrunPlusSampleDataReverse.xlsx
+pyloghub/sample_data/freightMatrixAddresses.xlsx
+pyloghub/sample_data/freightMatrixReverse.xlsx
 pyloghub/sample_data/shipmentAnalyzerAddresses.xlsx
 pyloghub/sample_data/shipmentAnalyzerReverse.xlsx
 pyloghub/sample_data/transportPlusAddresses.xlsx
 pyloghub/sample_data/transportPlusReverse.xlsx
 tests/__init__.py
 tests/test_geocoding.py
```

### Comparing `pyloghub-0.1.2/setup.py` & `pyloghub-0.1.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='pyloghub',
-    version='0.1.2',
+    version='0.1.3',
     packages=find_packages(),
     description='The `pyloghub` package provides convinient access to various Log-hub API services for Supply Chain Visualization, Network Design Optimization, and Transport Optimization as well as access to the Log-hub platform data.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/log-hub/log-hub-python',
     author='Log-hub AG',
     author_email='support@log-hub.com',
```

### Comparing `pyloghub-0.1.2/tests/test_geocoding.py` & `pyloghub-0.1.3/tests/test_geocoding.py`

 * *Files identical despite different names*

