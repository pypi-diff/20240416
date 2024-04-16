# Comparing `tmp/pyweatherfr-5.2.1.tar.gz` & `tmp/pyweatherfr-5.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyweatherfr-5.2.1.tar", last modified: Mon Apr 15 18:28:21 2024, max compression
+gzip compressed data, was "pyweatherfr-5.2.2.tar", last modified: Mon Apr 15 20:41:39 2024, max compression
```

## Comparing `pyweatherfr-5.2.1.tar` & `pyweatherfr-5.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:28:21.285866 pyweatherfr-5.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-15 18:27:38.000000 pyweatherfr-5.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-15 18:28:21.281866 pyweatherfr-5.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-15 18:27:38.000000 pyweatherfr-5.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-15 18:27:38.000000 pyweatherfr-5.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:28:21.281866 pyweatherfr-5.2.1/pyweatherfr/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-15 18:27:38.000000 pyweatherfr-5.2.1/pyweatherfr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-04-15 18:27:38.000000 pyweatherfr-5.2.1/pyweatherfr/args.py
--rw-r--r--   0 runner    (1001) docker     (127)    43111 2024-04-15 18:27:38.000000 pyweatherfr-5.2.1/pyweatherfr/pyweatherfr.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-15 18:27:38.000000 pyweatherfr-5.2.1/pyweatherfr/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:28:21.281866 pyweatherfr-5.2.1/pyweatherfr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-15 18:28:21.000000 pyweatherfr-5.2.1/pyweatherfr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-15 18:28:21.000000 pyweatherfr-5.2.1/pyweatherfr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 18:28:21.000000 pyweatherfr-5.2.1/pyweatherfr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-15 18:28:21.000000 pyweatherfr-5.2.1/pyweatherfr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 18:27:43.000000 pyweatherfr-5.2.1/pyweatherfr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-15 18:28:21.000000 pyweatherfr-5.2.1/pyweatherfr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-15 18:28:21.000000 pyweatherfr-5.2.1/pyweatherfr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 18:28:21.285866 pyweatherfr-5.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-15 18:27:38.000000 pyweatherfr-5.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:41:39.195191 pyweatherfr-5.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-15 20:40:55.000000 pyweatherfr-5.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-15 20:41:39.195191 pyweatherfr-5.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-15 20:40:55.000000 pyweatherfr-5.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-15 20:40:55.000000 pyweatherfr-5.2.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:41:39.191192 pyweatherfr-5.2.2/pyweatherfr/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-15 20:40:55.000000 pyweatherfr-5.2.2/pyweatherfr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-04-15 20:40:55.000000 pyweatherfr-5.2.2/pyweatherfr/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44284 2024-04-15 20:40:55.000000 pyweatherfr-5.2.2/pyweatherfr/pyweatherfr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-15 20:40:55.000000 pyweatherfr-5.2.2/pyweatherfr/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:41:39.191192 pyweatherfr-5.2.2/pyweatherfr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-15 20:41:39.000000 pyweatherfr-5.2.2/pyweatherfr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-15 20:41:39.000000 pyweatherfr-5.2.2/pyweatherfr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 20:41:39.000000 pyweatherfr-5.2.2/pyweatherfr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-15 20:41:39.000000 pyweatherfr-5.2.2/pyweatherfr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 20:40:59.000000 pyweatherfr-5.2.2/pyweatherfr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-15 20:41:39.000000 pyweatherfr-5.2.2/pyweatherfr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-15 20:41:39.000000 pyweatherfr-5.2.2/pyweatherfr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 20:41:39.195191 pyweatherfr-5.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-15 20:40:55.000000 pyweatherfr-5.2.2/setup.py
```

### Comparing `pyweatherfr-5.2.1/LICENSE.txt` & `pyweatherfr-5.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyweatherfr-5.2.1/PKG-INFO` & `pyweatherfr-5.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 5.2.1
+Version: 5.2.2
 Summary: pyweatherfr displays weather forecast for a given town in world (with high accuracy for France)
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-5.2.1/README.md` & `pyweatherfr-5.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
   - ``-u/--update``  update pyweatherfr
   - ``-c/--condensate``  condense la sortie
   - ``--nocolor``  désactive les couleurs et les emojis en sortie
   - ``-v/--verbose``  mode verbeux
   - ``--nocache``  supprime le cache de l'api meteo france avant l'appel
   - ``--utc``    utilise l'heure utc dans les previsions au lieu de l'heure locale de la ville
   - ``--pc``    utilise l'heure du pc dans les previsions au lieu de l'heure locale de la ville
-  - ``--lang` recherche (puis affiche) les villes avec leurs noms locaux
+  - ``-l/--lang` recherche (puis affiche) les villes avec leurs noms locaux
   
 # Démo
 
 ![image](./demo_01.png)
 
 ![image](./demo_02.png)
```

### Comparing `pyweatherfr-5.2.1/pyweatherfr/args.py` & `pyweatherfr-5.2.2/pyweatherfr/args.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,14 +105,15 @@
     my_parser.add_argument(
         "-w",
         "--world",
         action="store_true",
         help="activer la recherche hors France",
     )
     my_parser.add_argument(
+        "-l",
         "--lang",
         action="store_true",
         help="recherche (puis affiche) les villes avec leurs noms locaux",
     )     
     group = my_parser.add_mutually_exclusive_group()
     group.add_argument(
         "--pc",
```

### Comparing `pyweatherfr-5.2.1/pyweatherfr/pyweatherfr.py` & `pyweatherfr-5.2.2/pyweatherfr/pyweatherfr.py`

 * *Files 2% similar despite different names*

```diff
@@ -792,39 +792,39 @@
     others = ','.join(parties[1:])
     print_debug(town)
     print_debug(others)
     ctx = ssl.create_default_context(cafile=certifi.where())
     geopy.geocoders.options.default_ssl_context = ctx
     geolocator = geopy.geocoders.Nominatim(user_agent="my_geocoder")
     if compute_args().lang:
-        locations = geolocator.geocode(town+","+others,exactly_one=False,addressdetails=True,limit=9999)
+        locations = geolocator.geocode(town+","+others,featuretype="city",exactly_one=False,addressdetails=True,limit=9999)
     else:
-        locations = geolocator.geocode(town+","+others,exactly_one=False,addressdetails=True,language="fr",limit=9999)    
+        locations = geolocator.geocode(town+","+others,featuretype="city",exactly_one=False,addressdetails=True,language="fr",limit=9999)    
     choix = []
     if locations is None:
         print(my_colored("erreur : aucune ville trouvée", "red"))
         exit(1)  
     world=False
     print_debug(str(len(locations)) +" villes trouvées")    
     for location in locations:
-        #print_debug(json.dumps(location.raw, indent=4,ensure_ascii=False))
-        if ((location.raw.get("addresstype")=="postcode" and location.raw.get("address").get("country")=="France") or location.raw.get("addresstype")=="hamlet" or location.raw.get("addresstype")=="town" or location.raw.get("addresstype")=="city" or location.raw.get("addresstype")=="municipality" or location.raw.get("addresstype")=="village"):
-            
-            
+        print_debug(json.dumps(location.raw, indent=4,ensure_ascii=False))
+        if ((location.raw.get("addresstype")=="postcode" and location.raw.get("address").get("country")=="France") or location.raw.get("addresstype")=="hamlet" or location.raw.get("addresstype")=="town" or location.raw.get("addresstype")=="city" or location.raw.get("addresstype")=="municipality" or location.raw.get("addresstype")=="village" or location.raw.get("addresstype")=="province"):   
             ville = None
-            if ville is None or (location.raw.get("address").get("hamlet") is not None and (clean_string(location.raw.get("address").get("hamlet").lower())==clean_string(town.lower()))):
-                ville = location.raw.get("address").get("hamlet")
-            if ville is None or (location.raw.get("address").get("village") is not None and (clean_string(location.raw.get("address").get("village").lower())==clean_string(town.lower()))):
-                ville = location.raw.get("address").get("village")
-            if ville is None or (location.raw.get("address").get("municipality") is not None and (clean_string(location.raw.get("address").get("municipality").lower())==clean_string(town.lower()))):
-                ville = location.raw.get("address").get("municipality")
-            if ville is None or (location.raw.get("address").get("town") is not None and (clean_string(location.raw.get("address").get("town").lower())==clean_string(town.lower()))):
-                ville = location.raw.get("address").get("town")               
-            if ville is None or (location.raw.get("address").get("city") is not None and (clean_string(location.raw.get("address").get("city").lower())==clean_string(town.lower()))):
+            if ville is None and (location.raw.get("address").get("province") is not None and (clean_string(location.raw.get("address").get("province").lower())==clean_string(town.lower()))):
+                ville = location.raw.get("address").get("province")                 
+            if ville is None and (location.raw.get("address").get("city") is not None and (clean_string(location.raw.get("address").get("city").lower())==clean_string(town.lower()))):
                 ville = location.raw.get("address").get("city") 
+            if ville is None and (location.raw.get("address").get("town") is not None and (clean_string(location.raw.get("address").get("town").lower())==clean_string(town.lower()))):
+                ville = location.raw.get("address").get("town")               
+            if ville is None and (location.raw.get("address").get("municipality") is not None and (clean_string(location.raw.get("address").get("municipality").lower())==clean_string(town.lower()))):
+                ville = location.raw.get("address").get("municipality")
+            if ville is None and (location.raw.get("address").get("village") is not None and (clean_string(location.raw.get("address").get("village").lower())==clean_string(town.lower()))):
+                ville = location.raw.get("address").get("village")
+            if ville is None and (location.raw.get("address").get("hamlet") is not None and (clean_string(location.raw.get("address").get("hamlet").lower())==clean_string(town.lower()))):
+                ville = location.raw.get("address").get("hamlet")
             dpt = ""
             if location.raw.get("address").get("county") is not None:        
                 dpt = location.raw.get("address").get("county")
             if location.raw.get("address").get("state") is not None:
                 if dpt =="":
                     dpt = location.raw.get("address").get("state")  
                 else:
@@ -832,30 +832,39 @@
             if compute_args().world:
                 if dpt =="":                       
                     dpt= location.raw.get("address").get("country")
                 else:
                     dpt= dpt + ", "+location.raw.get("address").get("country")
 
             country = location.raw.get("address").get("country")
-            if country == "France":
+            if country == "France" and location.raw.get("addresstype")=="postcode":
                 cp = location.raw.get("address").get("postcode")
+                if ville is None and (location.raw.get("address").get("village") is not None):
+                    ville = location.raw.get("address").get("village")              
+                if ville is None and (location.raw.get("address").get("municipality") is not None):
+                    ville = location.raw.get("address").get("municipality")
+                if ville is None and (location.raw.get("address").get("town") is not None):
+                    ville = location.raw.get("address").get("town")               
+                if ville is None and (location.raw.get("address").get("city") is not None):
+                    ville = location.raw.get("address").get("city")                 
             else:
                 cp = ""
             lat = location.raw.get("lat")
             long = location.raw.get("lon")
-            print_debug(ville+"-"+dpt+"-"+lat+"-"+long+"-"+country)
-            if (clean_string(ville.lower()) == clean_string(town.lower()) or cp.lower() == town.lower()):
-                if ville+"-"+dpt not in [item[0] for item in choix]:  
-                    if country=="France":
-                        choix.append([ville+"-"+dpt, ville, dpt, country,lat, long])
-                    else:
-                        if compute_args().world:
+            if ville is not None:
+                print_debug(ville+"-"+dpt+"-"+lat+"-"+long+"-"+country)
+                if (clean_string(ville.lower()) == clean_string(town.lower()) or cp.lower() == town.lower()):
+                    if ville+"-"+dpt not in [item[0] for item in choix]:  
+                        if country=="France":
                             choix.append([ville+"-"+dpt, ville, dpt, country,lat, long])
                         else:
-                            world=True    
+                            if compute_args().world:
+                                choix.append([ville+"-"+dpt, ville, dpt, country,lat, long])
+                            else:
+                                world=True    
     if not compute_args().world and world:
         print("")
         print(my_colored("warning : il existe des villes hors France disponibles pour wotre recherche. Relancez la avec --world pour y acceder", "yellow"))
     if len(choix)==1:
         choice = choix[0]
         ville = choice[1]
         dpt = choice[2]
```

### Comparing `pyweatherfr-5.2.1/pyweatherfr.egg-info/PKG-INFO` & `pyweatherfr-5.2.2/pyweatherfr.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 5.2.1
+Version: 5.2.2
 Summary: pyweatherfr displays weather forecast for a given town in world (with high accuracy for France)
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-5.2.1/setup.py` & `pyweatherfr-5.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name="pyweatherfr",
-    version="5.2.1",
+    version="5.2.2",
     description="pyweatherfr displays weather forecast for a given town in world (with high accuracy for France)",
     long_description="The complete description/installation/use/FAQ is available at : https://github.com/thib1984/pyweatherfr#readme",
     url="https://github.com/thib1984/pyweatherfr",
     author="thib1984",
     author_email="thibault.garcon@gmail.com",
     license="MIT",
     packages=["pyweatherfr"],
```

