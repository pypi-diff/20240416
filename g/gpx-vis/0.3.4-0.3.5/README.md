# Comparing `tmp/gpx_vis-0.3.4.tar.gz` & `tmp/gpx_vis-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpx_vis-0.3.4.tar", last modified: Wed Apr 10 13:07:53 2024, max compression
+gzip compressed data, was "gpx_vis-0.3.5.tar", last modified: Tue Apr 16 14:41:17 2024, max compression
```

## Comparing `gpx_vis-0.3.4.tar` & `gpx_vis-0.3.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-10 13:07:53.899475 gpx_vis-0.3.4/
--rw-r--r--   0 jwt        (501) staff       (20)     1514 2024-04-05 12:16:08.000000 gpx_vis-0.3.4/LICENSE
--rw-r--r--   0 jwt        (501) staff       (20)     3497 2024-04-10 13:07:53.898366 gpx_vis-0.3.4/PKG-INFO
--rw-r--r--   0 jwt        (501) staff       (20)     2944 2024-04-08 10:34:50.000000 gpx_vis-0.3.4/README.md
--rw-r--r--   0 jwt        (501) staff       (20)      593 2024-04-10 13:05:42.000000 gpx_vis-0.3.4/pyproject.toml
--rw-r--r--   0 jwt        (501) staff       (20)       38 2024-04-10 13:07:53.899723 gpx_vis-0.3.4/setup.cfg
-drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-10 13:07:53.891637 gpx_vis-0.3.4/src/
--rw-r--r--   0 jwt        (501) staff       (20)      113 2024-04-07 22:23:57.000000 gpx_vis-0.3.4/src/__init__.py
-drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-10 13:07:53.896837 gpx_vis-0.3.4/src/gpx_vis.egg-info/
--rw-r--r--   0 jwt        (501) staff       (20)     3497 2024-04-10 13:07:51.000000 gpx_vis-0.3.4/src/gpx_vis.egg-info/PKG-INFO
--rw-r--r--   0 jwt        (501) staff       (20)      237 2024-04-10 13:07:51.000000 gpx_vis-0.3.4/src/gpx_vis.egg-info/SOURCES.txt
--rw-r--r--   0 jwt        (501) staff       (20)        1 2024-04-10 13:07:51.000000 gpx_vis-0.3.4/src/gpx_vis.egg-info/dependency_links.txt
--rw-r--r--   0 jwt        (501) staff       (20)       83 2024-04-10 13:07:51.000000 gpx_vis-0.3.4/src/gpx_vis.egg-info/requires.txt
--rw-r--r--   0 jwt        (501) staff       (20)       17 2024-04-10 13:07:51.000000 gpx_vis-0.3.4/src/gpx_vis.egg-info/top_level.txt
--rw-r--r--   0 jwt        (501) staff       (20)    20247 2024-04-10 13:02:53.000000 gpx_vis-0.3.4/src/gpx_vis.py
+drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-16 14:41:17.067264 gpx_vis-0.3.5/
+-rw-r--r--   0 jwt        (501) staff       (20)     1514 2024-04-05 12:16:08.000000 gpx_vis-0.3.5/LICENSE
+-rw-r--r--   0 jwt        (501) staff       (20)     5178 2024-04-16 14:41:17.067036 gpx_vis-0.3.5/PKG-INFO
+-rw-r--r--   0 jwt        (501) staff       (20)     4628 2024-04-16 14:29:36.000000 gpx_vis-0.3.5/README.md
+-rw-r--r--   0 jwt        (501) staff       (20)      590 2024-04-16 14:40:07.000000 gpx_vis-0.3.5/pyproject.toml
+-rw-r--r--   0 jwt        (501) staff       (20)       38 2024-04-16 14:41:17.067325 gpx_vis-0.3.5/setup.cfg
+drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-16 14:41:17.064998 gpx_vis-0.3.5/src/
+-rw-r--r--   0 jwt        (501) staff       (20)      113 2024-04-07 22:23:57.000000 gpx_vis-0.3.5/src/__init__.py
+drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-16 14:41:17.066720 gpx_vis-0.3.5/src/gpx_vis.egg-info/
+-rw-r--r--   0 jwt        (501) staff       (20)     5178 2024-04-16 14:41:17.000000 gpx_vis-0.3.5/src/gpx_vis.egg-info/PKG-INFO
+-rw-r--r--   0 jwt        (501) staff       (20)      237 2024-04-16 14:41:17.000000 gpx_vis-0.3.5/src/gpx_vis.egg-info/SOURCES.txt
+-rw-r--r--   0 jwt        (501) staff       (20)        1 2024-04-16 14:41:17.000000 gpx_vis-0.3.5/src/gpx_vis.egg-info/dependency_links.txt
+-rw-r--r--   0 jwt        (501) staff       (20)       83 2024-04-16 14:41:17.000000 gpx_vis-0.3.5/src/gpx_vis.egg-info/requires.txt
+-rw-r--r--   0 jwt        (501) staff       (20)       17 2024-04-16 14:41:17.000000 gpx_vis-0.3.5/src/gpx_vis.egg-info/top_level.txt
+-rw-r--r--   0 jwt        (501) staff       (20)    20778 2024-04-16 13:35:51.000000 gpx_vis-0.3.5/src/gpx_vis.py
```

### Comparing `gpx_vis-0.3.4/LICENSE` & `gpx_vis-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gpx_vis-0.3.4/pyproject.toml` & `gpx_vis-0.3.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools >= 61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gpx_vis"
-version = "0.3.4"
+version = "0.3.5"
 authors = [
   { name="Jia Wei Teh", email="jiaweiteh.astro@gmail.com" },
 ]
-description = "Visualising your completed Komoot tours"
+description = "Visualising your Komoot/Strava tours"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 dependencies = [
```

### Comparing `gpx_vis-0.3.4/src/gpx_vis.py` & `gpx_vis-0.3.5/src/gpx_vis.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 import math
 import branca
 import folium
 import numpy as np
 import pandas as pd
 import altair as alt
 import humanfriendly
-from time import time
 import reverse_geocode
-from datetime import timedelta
-from folium.plugins import MarkerCluster, MiniMap
 
+from time import time
 from vincenty import vincenty
+from datetime import timedelta
+from folium.plugins import MarkerCluster, MiniMap
 
 class Track:
     """
     Instance used to process .gpx files.
     """
     
     # =============================================================================
@@ -46,18 +46,14 @@
         self.y = []
         # time
         self.t = []
         # elevation
         self.z = []
         # name
         self.name = []
-        # start timer
-        global _timer
-        _timer = Timer()
-        _timer.begin()
         print('Reading data...')
         # if pathname is a folder
         # loop through file.
         if os.path.isdir(pathname):
             for fname in os.listdir(pathname):
                 if fname.endswith('.gpx'):
                     with open(os.path.join(pathname, fname), 'r') as file:
@@ -92,15 +88,15 @@
                     self.z = np.concatenate((self.z, [pt.elevation]))
                     self.t = np.concatenate((self.t, [pt.time]))
                     self.name = np.concatenate((self.name, [trk.name]))
                     
     @property
     def header(self):
         # some column name here. TBD cause headers not finalised.
-        return
+        return self.data.columns.values
     
     @property
     def data(self):
         """
         Shows pd.DataFrame object from input gpx file.
         """
         # some pandas library here. Set column names
@@ -114,17 +110,17 @@
                 col_names[4]: self.t,
                 }
         # create dataframe
         df = pd.DataFrame(data = data)
         # return
         return df
     
-    # @property
-    # def help(self):
-    #     return "Documentations TBD"
+    @property
+    def help(self):
+        return print('Check out https://github.com/JiaWeiTeh/gpx_vis .')
             
     # =============================================================================
     # Here we deal with cities we have been in the tour.
     # =============================================================================
 
     class City:
         """
@@ -172,15 +168,15 @@
         unique_city_list = list(set(city_list))
         # add frequency of appearance of city in tour
         for ii, unique_city in enumerate(unique_city_list):
             counts = city_list.count(unique_city)
             # update attribute
             setattr(unique_city_list[ii], 'frequency', counts)
         # return full list of cities, sorted by country then by name
-        print('Here are the cities you have been in.')
+        print('Here are the cities you passed through on your journey.')
         return sorted(unique_city_list)
     
     # =============================================================================
     # Track handling
     # =============================================================================
     
     @staticmethod
@@ -237,14 +233,18 @@
     # Plotting on maps
     # =============================================================================
     
     def create_map(self, filename, lite = False, **kwargs):
         """
         Map out your tour on an interactive streetmaps.
         """
+        # start timer
+        _timer = Timer()
+        _timer.begin()
+        print('Mapping data...')
         # find optimal center for map display.
         map_center = self.data[['latitude', 'longitude']].mean().values.tolist()
         # southwest (minimums) and northeast (maximums) boundary.
         map_sw = self.data[['latitude', 'longitude']].min().values.tolist()
         map_ne = self.data[['latitude', 'longitude']].max().values.tolist()
         # create Map.
         main_map = folium.Map(location = map_center)
@@ -261,48 +261,51 @@
             
         # clusters
         cluster = MarkerCluster().add_to(main_map)
         # add group to map
         lineGroup.add_to(cluster)
         
         # add different backgrounds
-        _tilesList = ['openstreetmap', 'CartoDB Voyager', 'Cartodb dark_matter', 'cartodbpositron']
-        for tiles in _tilesList:
-            folium.TileLayer(tiles).add_to(main_map)
+        _tilesList = ['cartodbpositron', 'Cartodb dark_matter', 'CartoDB Voyager' ]
+        _tileName = ['Plain', 'Dark mode', 'Plain (heirarchical)']
+        for ii, tiles in enumerate(_tilesList):
+            folium.raster_layers.TileLayer(tiles, name = _tileName[ii]).add_to(main_map)
         # add layer control
         folium.LayerControl(position='bottomright').add_to(main_map)
         # add minimap 
         MiniMap(toggle_display = True, zoom_level_offset = -4,
                 witdh = 400, height = 200,
                 position = 'topright',
                 ).add_to(main_map)
         
         # save
         if not filename.endswith(".html"):
             filename += '.html'
         main_map.save(filename)
-        
         # show time
-        global _timer
         _timer.end()
         return print(f"File saved as {filename}.")
     
     @staticmethod
     def _addTracksOnMap(self, group, selected_idx, lite, **kwargs):
         """
         This function adds individual tracks onto create_map().
         group: FeatureGroup this track belongs to.
         selected_idx: index range of this particular track.
         """
         ii, jj = selected_idx
+        # sanity check
+        assert lite in [True, False], "'lite' accepts only 'True' or 'False'."
         # limit number of points shown to reduce runtime, if lite is enabled.
         if kwargs.get('nlite') is not None:
+            assert (kwargs.get('nlite') >= 10), "minimum value of 'nlite' is 10."
             max_nPoints = kwargs.get('nlite')
         else:
             max_nPoints = 50
+        # calculate the actual index interval for desired points
         if (jj-ii) < max_nPoints or lite == False:
             nPoints = 1 #basically means plot every single point
         else:
             nPoints = int((jj-ii)/max_nPoints)
         
             
         track_coords = list(zip(self.y[ii:jj:nPoints], self.x[ii:jj:nPoints]))
@@ -318,15 +321,15 @@
         # add to group
         # since elevation sometimes differ widly, perhaps it is better to use 
         # log-scale as a simple fix. (as long as there aren't zero entries)
         # Right now, I am using individual tracks for individual colorbar min/max. Can of course
         # switch to map-wide colorbar by removing [ii:jj]
         folium.ColorLine(track_coords,
                         colors = self.z[ii:jj:nPoints],
-                        colormap = branca.colormap.linear.viridis.scale(min(self.z[ii:jj:nPoints]),max(self.z[ii:jj:nPoints])),
+                        colormap = branca.colormap.linear.plasma.scale(min(self.z[ii:jj:nPoints]),max(self.z[ii:jj:nPoints])),
                         tooltip = tooltip,
                         weight = 4,
                         ).add_to(group)
         
         # add start/finish points
         folium.CircleMarker(location = track_coords[0],
                             radius = 5,
@@ -419,20 +422,23 @@
         # plot
         lineplot = alt.Chart(self.data[['time', 'elevation']][ii:jj:nPoints],
                                  title = alt.Title(  title, 
                                                      subtitle = [subtitle1, subtitle2, subtitle3])
                                                    )\
                             .mark_line()\
                             .encode(
-                                 alt.X('time', axis = alt.Axis(tickCount = 6)).title('Time (Local)'),\
-                                 alt.Y('elevation', axis = alt.Axis(tickMinStep=20)).scale(domain=(min(self.z[ii:jj:nPoints]-50), max(self.z[ii:jj:nPoints]+50))).title('Elevation (m)'),\
+                                 x = alt.X('time:T', axis = alt.Axis(tickCount = 6)).title('Time (Local)'),\
+                                 y = alt.Y('elevation:Q', axis = alt.Axis(tickMinStep=20)).scale(domain=(min(self.z[ii:jj:nPoints]-50), max(self.z[ii:jj:nPoints]+50))).title('Elevation (m)'),\
                                  )\
                             .properties(
                                 width = 300, height = 300,
+                                )\
+                            .add_params(
                                 )
+                            
         # turn into vega
         elevation_graph = folium.VegaLite(
                             lineplot,
                             width=300,
                             height=300,
                             )
         return elevation_graph
@@ -511,25 +517,25 @@
         # record the beginning time
         self.start = time()
 
     # sets end of timer
     def end(self):
         # make sure start is evoked:
         if self.start == None:
-            raise InvalidCall('_timer.end() called, but .begin() not detected.')
+            raise InvalidTimerCall('_timer.end() called, but .begin() not detected.')
         # record the end time
         self.stop = time()
         # then, print out time elapsed.
         time_str = self.secs2str()
         print('~'*(len(time_str)+14))
         print(f'Time elapsed: {time_str}.')
         print('~'*(len(time_str)+14))
         # reset
         self.start = None
         self.stop = None
 
-class InvalidCall(Exception):
+class InvalidTimerCall(Exception):
     """
     Raised when timer call is invalid. 
 
     For example: calling _timer.end() without explicitly calling _timer.begin().
     """
```

