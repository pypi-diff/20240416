# Comparing `tmp/climsight-0.0.1.tar.gz` & `tmp/climsight-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climsight-0.0.1.tar", last modified: Wed Apr 10 13:48:47 2024, max compression
+gzip compressed data, was "climsight-0.2.0.tar", last modified: Tue Apr 16 12:56:38 2024, max compression
```

## Comparing `climsight-0.0.1.tar` & `climsight-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 mayiva    (1000) mayiva    (1000)        0 2024-04-10 13:48:47.157647 climsight-0.0.1/
--rw-rw-r--   0 mayiva    (1000) mayiva    (1000)     1503 2024-04-10 12:37:29.000000 climsight-0.0.1/LICENSE
--rw-r--r--   0 mayiva    (1000) mayiva    (1000)      451 2024-04-10 13:48:47.157647 climsight-0.0.1/PKG-INFO
--rw-rw-r--   0 mayiva    (1000) mayiva    (1000)     3338 2024-04-10 12:37:29.000000 climsight-0.0.1/README.md
--rw-rw-r--   0 mayiva    (1000) mayiva    (1000)      562 2024-04-10 13:28:49.000000 climsight-0.0.1/pyproject.toml
--rw-rw-r--   0 mayiva    (1000) mayiva    (1000)       38 2024-04-10 13:48:47.157647 climsight-0.0.1/setup.cfg
-drwxrwxr-x   0 mayiva    (1000) mayiva    (1000)        0 2024-04-10 13:48:47.153647 climsight-0.0.1/src/
-drwxrwxr-x   0 mayiva    (1000) mayiva    (1000)        0 2024-04-10 13:48:47.157647 climsight-0.0.1/src/climsight/
--rw-rw-r--   0 mayiva    (1000) mayiva    (1000)     4145 2024-04-10 12:38:55.000000 climsight-0.0.1/src/climsight/climate_functions.py
--rw-rw-r--   0 mayiva    (1000) mayiva    (1000)    13973 2024-04-10 12:38:55.000000 climsight-0.0.1/src/climsight/climsight.py
--rw-rw-r--   0 mayiva    (1000) mayiva    (1000)     8191 2024-04-10 12:38:55.000000 climsight-0.0.1/src/climsight/economic_functions.py
--rw-rw-r--   0 mayiva    (1000) mayiva    (1000)     4419 2024-04-10 12:38:55.000000 climsight-0.0.1/src/climsight/environmental_functions.py
--rw-rw-r--   0 mayiva    (1000) mayiva    (1000)    10546 2024-04-10 12:38:55.000000 climsight-0.0.1/src/climsight/geo_functions.py
--rw-rw-r--   0 mayiva    (1000) mayiva    (1000)      103 2024-04-10 13:28:04.000000 climsight-0.0.1/src/climsight/launch.py
-drwxrwxr-x   0 mayiva    (1000) mayiva    (1000)        0 2024-04-10 13:48:47.157647 climsight-0.0.1/src/climsight.egg-info/
--rw-r--r--   0 mayiva    (1000) mayiva    (1000)      451 2024-04-10 13:48:47.000000 climsight-0.0.1/src/climsight.egg-info/PKG-INFO
--rw-rw-r--   0 mayiva    (1000) mayiva    (1000)      450 2024-04-10 13:48:47.000000 climsight-0.0.1/src/climsight.egg-info/SOURCES.txt
--rw-rw-r--   0 mayiva    (1000) mayiva    (1000)        1 2024-04-10 13:48:47.000000 climsight-0.0.1/src/climsight.egg-info/dependency_links.txt
--rw-rw-r--   0 mayiva    (1000) mayiva    (1000)       64 2024-04-10 13:48:47.000000 climsight-0.0.1/src/climsight.egg-info/entry_points.txt
--rw-rw-r--   0 mayiva    (1000) mayiva    (1000)      136 2024-04-10 13:48:47.000000 climsight-0.0.1/src/climsight.egg-info/requires.txt
--rw-rw-r--   0 mayiva    (1000) mayiva    (1000)       10 2024-04-10 13:48:47.000000 climsight-0.0.1/src/climsight.egg-info/top_level.txt
+drwxrwxr-x   0 mayiva    (1000) mayiva    (1000)        0 2024-04-16 12:56:38.341546 climsight-0.2.0/
+-rw-rw-r--   0 mayiva    (1000) mayiva    (1000)     1503 2024-04-08 08:27:15.000000 climsight-0.2.0/LICENSE
+-rw-r--r--   0 mayiva    (1000) mayiva    (1000)     4273 2024-04-16 12:56:38.341546 climsight-0.2.0/PKG-INFO
+-rw-rw-r--   0 mayiva    (1000) mayiva    (1000)     3800 2024-04-16 12:48:02.000000 climsight-0.2.0/README.md
+-rw-rw-r--   0 mayiva    (1000) mayiva    (1000)      572 2024-04-16 12:56:26.000000 climsight-0.2.0/pyproject.toml
+-rw-rw-r--   0 mayiva    (1000) mayiva    (1000)       38 2024-04-16 12:56:38.341546 climsight-0.2.0/setup.cfg
+drwxrwxr-x   0 mayiva    (1000) mayiva    (1000)        0 2024-04-16 12:56:38.337546 climsight-0.2.0/src/
+drwxrwxr-x   0 mayiva    (1000) mayiva    (1000)        0 2024-04-16 12:56:38.341546 climsight-0.2.0/src/climsight/
+-rw-rw-r--   0 mayiva    (1000) mayiva    (1000)        0 2024-04-15 07:44:37.000000 climsight-0.2.0/src/climsight/__init__.py
+-rw-rw-r--   0 mayiva    (1000) mayiva    (1000)     4145 2024-04-15 09:48:20.000000 climsight-0.2.0/src/climsight/climate_functions.py
+-rw-rw-r--   0 mayiva    (1000) mayiva    (1000)    13082 2024-04-15 07:44:37.000000 climsight-0.2.0/src/climsight/climsight.py
+-rw-rw-r--   0 mayiva    (1000) mayiva    (1000)     8191 2024-04-15 07:44:37.000000 climsight-0.2.0/src/climsight/economic_functions.py
+-rw-rw-r--   0 mayiva    (1000) mayiva    (1000)     4419 2024-04-15 07:44:37.000000 climsight-0.2.0/src/climsight/environmental_functions.py
+-rw-rw-r--   0 mayiva    (1000) mayiva    (1000)    10546 2024-04-15 07:44:37.000000 climsight-0.2.0/src/climsight/geo_functions.py
+-rw-rw-r--   0 mayiva    (1000) mayiva    (1000)      709 2024-04-16 12:48:02.000000 climsight-0.2.0/src/climsight/launch.py
+drwxrwxr-x   0 mayiva    (1000) mayiva    (1000)        0 2024-04-16 12:56:38.341546 climsight-0.2.0/src/climsight.egg-info/
+-rw-r--r--   0 mayiva    (1000) mayiva    (1000)     4273 2024-04-16 12:56:38.000000 climsight-0.2.0/src/climsight.egg-info/PKG-INFO
+-rw-rw-r--   0 mayiva    (1000) mayiva    (1000)      476 2024-04-16 12:56:38.000000 climsight-0.2.0/src/climsight.egg-info/SOURCES.txt
+-rw-rw-r--   0 mayiva    (1000) mayiva    (1000)        1 2024-04-16 12:56:38.000000 climsight-0.2.0/src/climsight.egg-info/dependency_links.txt
+-rw-rw-r--   0 mayiva    (1000) mayiva    (1000)       64 2024-04-16 12:56:38.000000 climsight-0.2.0/src/climsight.egg-info/entry_points.txt
+-rw-rw-r--   0 mayiva    (1000) mayiva    (1000)      132 2024-04-16 12:56:38.000000 climsight-0.2.0/src/climsight.egg-info/requires.txt
+-rw-rw-r--   0 mayiva    (1000) mayiva    (1000)       10 2024-04-16 12:56:38.000000 climsight-0.2.0/src/climsight.egg-info/top_level.txt
```

### Comparing `climsight-0.0.1/LICENSE` & `climsight-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `climsight-0.0.1/README.md` & `climsight-0.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -37,14 +37,19 @@
 Then open `http://localhost:8501/` in your browser. If you don't want to add OpenAI key every time, you can expose it through:
 
 ```bash
 docker run -p 8501:8501 -e OPENAI_API_KEY=$OPENAI_API_KEY climsight
 ```
 where `$OPENAI_API_KEY` not necessarily should be environment variable, you can insert the key directly.
 
+If you do not have an OpenAI key but want to test Climsight without sending requests to OpenAI, you can run Climsight with the `skipLLMCall` argument:
+```bash
+docker run -p 8501:8501 -e STREAMLIT_ARGS="skipLLMCall" climsight
+```
+
 ## Installation
 
 The easiest way is to install it through conda or mamba. We recommend mamba, as it's faster. 
 
 [Install mamba](https://mamba.readthedocs.io/en/latest/mamba-installation.html#mamba-install) if you don't have it.
 
 ```bash
@@ -84,19 +89,25 @@
 
 ### Running 
 
 Change to the `climsight` folder:
 
 ```bash
 cd climsight
-streamlit run climsight.py
+streamlit run src/climsight/climsight.py
 ```
 
 The browser window should pop up, with the app running. Ask the questions and don't forget to press "Generate".
 
 <img width="800" alt="Screenshot 2023-09-26 at 15 26 51" src="https://github.com/koldunovn/climsight/assets/3407313/569a4c38-a601-4014-b10d-bd34c59b91bb">
 
+If you do not have an OpenAI key but want to test Climsight without sending requests to OpenAI, you can run Climsight with the `skipLLMCall` argument:
+```bash
+streamlit run src/climsight/climsight.py skipLLMCall
+```
+
+
 ## Citation
 
 If you use or refer to ClimSight in your work, please cite the following publication:
 
 Koldunov, N., Jung, T. Local climate services for all, courtesy of large language models. _Commun Earth Environ_ **5**, 13 (2024). https://doi.org/10.1038/s43247-023-01199-1
```

### Comparing `climsight-0.0.1/pyproject.toml` & `climsight-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "climsight"
-version = "0.0.1"
+version = "0.2.0"
+readme = "README.md"
 dependencies = [
-    "sys",
     "streamlit",
     "xarray",
     "geopy",
     "geopandas",
     "pyproj",
     "requests",
     "pandas",
@@ -20,14 +20,13 @@
     "openai==1.5.0",
 ]
 
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
-
 #[tool.setuptools.packages]
 #find = {}  # Scan the project directory with the default parameters
 
 
 [project.scripts]
-climsight = "climsight.launch:launch_streamlit"
+climsight = "climsight.launch:launch_streamlit"
```

### Comparing `climsight-0.0.1/src/climsight/climate_functions.py` & `climsight-0.2.0/src/climsight/climate_functions.py`

 * *Files identical despite different names*

### Comparing `climsight-0.0.1/src/climsight/climsight.py` & `climsight-0.2.0/src/climsight/climsight.py`

 * *Files 4% similar despite different names*

```diff
@@ -212,43 +212,14 @@
         biodiv = fetch_biodiversity(round(lat), round(lon))
 
         distance_to_coastline = closest_shore_distance(lat, lon, coastline_shapefile)
 
         # create pandas dataframe
         df, data_dict = extract_climate_data(lat, lon, hist, future)
 
-        # Plot the chart
-        st.text(
-            "Near surface temperature [source: AWI-CM-1-1-MR, historical, and SSP5-8.5]",
-        )
-        st.line_chart(
-            df,
-            x="Month",
-            y=["Present Day Temperature", "Future Temperature"],
-            color=["#d62728", "#2ca02c"],
-        )
-        st.text(
-            "Precipitation [source: AWI-CM-1-1-MR, historical, and SSP5-8.5]",
-        )
-        st.line_chart(
-            df,
-            x="Month",
-            y=["Present Day Precipitation", "Future Precipitation"],
-            color=["#d62728", "#2ca02c"],
-        )
-        st.text(
-            "Wind speed [source: AWI-CM-1-1-MR, historical, and SSP5-8.5]",
-        )
-        st.line_chart(
-            df,
-            x="Month",
-            y=["Present Day Wind Speed", "Future Wind Speed"],
-            color=["#d62728", "#2ca02c"],
-        )
-
         filtered_events_square, promt_hazard_data = filter_events_within_square(lat, lon, haz_path, distance_from_event)
 
         population = x_year_mean_population(pop_path, country, year_step=year_step, start_year=start_year, end_year=end_year)
 
         haz_fig = plot_disaster_counts(filtered_events_square)
         population_plot = plot_population(pop_path, country)
```

### Comparing `climsight-0.0.1/src/climsight/economic_functions.py` & `climsight-0.2.0/src/climsight/economic_functions.py`

 * *Files identical despite different names*

### Comparing `climsight-0.0.1/src/climsight/environmental_functions.py` & `climsight-0.2.0/src/climsight/environmental_functions.py`

 * *Files identical despite different names*

### Comparing `climsight-0.0.1/src/climsight/geo_functions.py` & `climsight-0.2.0/src/climsight/geo_functions.py`

 * *Files identical despite different names*

