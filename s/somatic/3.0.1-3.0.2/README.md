# Comparing `tmp/somatic-3.0.1.tar.gz` & `tmp/somatic-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "somatic-3.0.1.tar", last modified: Thu Apr  4 23:19:36 2024, max compression
+gzip compressed data, was "somatic-3.0.2.tar", max compression
```

## Comparing `somatic-3.0.1.tar` & `somatic-3.0.2.tar`

### file list

```diff
@@ -1,52 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.597034 somatic-3.0.1/
--rw-r--r--   0 root         (0) root         (0)     3781 2024-04-04 23:19:36.597034 somatic-3.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1729 2024-04-04 23:19:05.000000 somatic-3.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     3316 2024-04-04 23:16:39.000000 somatic-3.0.1/readme.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 23:19:36.597034 somatic-3.0.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.589034 somatic-3.0.1/venues/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.589034 somatic-3.0.1/venues/stages/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.593034 somatic-3.0.1/venues/stages/somatic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.593034 somatic-3.0.1/venues/stages/somatic/___itinerary/
--rw-r--r--   0 root         (0) root         (0)      916 2024-04-04 23:15:15.000000 somatic-3.0.1/venues/stages/somatic/___itinerary/itinerary.S.HTML
--rw-rw-r--   0 root         (0) root         (0)      977 2024-04-04 21:52:53.000000 somatic-3.0.1/venues/stages/somatic/___itinerary/possibilities.S.HTML
--rw-r--r--   0 root         (0) root         (0)      368 2024-04-04 22:59:35.000000 somatic-3.0.1/venues/stages/somatic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.593034 somatic-3.0.1/venues/stages/somatic/__license/
--rw-r--r--   0 root         (0) root         (0)      362 2024-02-14 04:20:52.000000 somatic-3.0.1/venues/stages/somatic/__license/license.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.593034 somatic-3.0.1/venues/stages/somatic/__license/licenses/
--rw-r--r--   0 root         (0) root         (0)    37279 2023-12-01 20:51:04.000000 somatic-3.0.1/venues/stages/somatic/__license/licenses/gpl-3.0-standalone.html
--rw-r--r--   0 root         (0) root         (0)     2645 2024-04-04 23:16:16.000000 somatic-3.0.1/venues/stages/somatic/_clique.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.589034 somatic-3.0.1/venues/stages/somatic/_controls/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.593034 somatic-3.0.1/venues/stages/somatic/_controls/flask/
--rw-rw-r--   0 root         (0) root         (0)     2040 2024-04-04 22:08:21.000000 somatic-3.0.1/venues/stages/somatic/_controls/flask/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.593034 somatic-3.0.1/venues/stages/somatic/_controls/sanic/
--rw-rw-r--   0 root         (0) root         (0)     2848 2024-04-04 22:41:36.000000 somatic-3.0.1/venues/stages/somatic/_controls/sanic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.593034 somatic-3.0.1/venues/stages/somatic/_status/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.589034 somatic-3.0.1/venues/stages/somatic/_status/checks/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.593034 somatic-3.0.1/venues/stages/somatic/_status/checks/1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.593034 somatic-3.0.1/venues/stages/somatic/_status/checks/1/shares/
--rw-r--r--   0 root         (0) root         (0)       25 2024-02-14 04:20:52.000000 somatic-3.0.1/venues/stages/somatic/_status/checks/1/shares/shares 1.s.HTML
--rw-r--r--   0 root         (0) root         (0)       25 2024-02-14 04:20:52.000000 somatic-3.0.1/venues/stages/somatic/_status/checks/1/shares/shares 2.s.HTML
--rw-r--r--   0 root         (0) root         (0)      659 2024-04-04 20:52:44.000000 somatic-3.0.1/venues/stages/somatic/_status/checks/1/status_1.py
--rw-r--r--   0 root         (0) root         (0)     1205 2024-04-04 22:05:34.000000 somatic-3.0.1/venues/stages/somatic/_status/status.proc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.593034 somatic-3.0.1/venues/stages/somatic/climate/
--rw-rw-r--   0 root         (0) root         (0)      220 2024-02-14 04:20:52.000000 somatic-3.0.1/venues/stages/somatic/climate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2812 2024-03-15 01:31:11.000000 somatic-3.0.1/venues/stages/somatic/module.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.593034 somatic-3.0.1/venues/stages/somatic/modules/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.593034 somatic-3.0.1/venues/stages/somatic/modules/HTML/
--rw-rw-r--   0 root         (0) root         (0)     3550 2024-04-04 21:54:29.000000 somatic-3.0.1/venues/stages/somatic/modules/HTML/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      553 2024-04-04 20:53:54.000000 somatic-3.0.1/venues/stages/somatic/modules/add_glob_to_paths.py
--rw-rw-r--   0 root         (0) root         (0)      806 2024-02-14 04:20:52.000000 somatic-3.0.1/venues/stages/somatic/modules/parse_extensions.py
--rw-rw-r--   0 root         (0) root         (0)      270 2024-04-04 22:07:22.000000 somatic-3.0.1/venues/stages/somatic/modules/port_in_use.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.589034 somatic-3.0.1/venues/stages/somatic/modules_ES/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.593034 somatic-3.0.1/venues/stages/somatic/modules_ES/address/
--rw-r--r--   0 root         (0) root         (0)      524 2024-01-31 20:00:34.000000 somatic-3.0.1/venues/stages/somatic/modules_ES/address/address.s.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.593034 somatic-3.0.1/venues/stages/somatic/moves/
--rw-rw-r--   0 root         (0) root         (0)     2761 2024-04-04 23:13:56.000000 somatic-3.0.1/venues/stages/somatic/moves/start.py
--rw-rw-r--   0 root         (0) root         (0)      452 2024-02-14 04:20:52.000000 somatic-3.0.1/venues/stages/somatic/start.proc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:19:36.593034 somatic-3.0.1/venues/stages/somatic.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3781 2024-04-04 23:19:36.000000 somatic-3.0.1/venues/stages/somatic.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1303 2024-04-04 23:19:36.000000 somatic-3.0.1/venues/stages/somatic.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2024-04-04 23:19:36.000000 somatic-3.0.1/venues/stages/somatic.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       43 2024-04-04 23:19:36.000000 somatic-3.0.1/venues/stages/somatic.egg-info/entry_points.txt
--rw-rw-r--   0 root         (0) root         (0)       69 2024-04-04 23:19:36.000000 somatic-3.0.1/venues/stages/somatic.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)        8 2024-04-04 23:19:36.000000 somatic-3.0.1/venues/stages/somatic.egg-info/top_level.txt
+-rwxr-xr-x   0        0        0      112 2024-04-04 21:59:18.417086 somatic-3.0.2/license.S.HTML
+-rw-r--r--   0        0        0      773 2024-04-16 05:40:55.544010 somatic-3.0.2/pyproject.toml
+-rwxr-xr-x   0        0        0     3316 2024-04-04 23:16:39.855140 somatic-3.0.2/readme.md
+-rw-r--r--   0        0        0     1536 2024-04-16 05:47:53.994607 somatic-3.0.2/venue.S.HTML
+-rwxr-xr-x   0        0        0     1396 2024-04-12 17:02:14.756736 somatic-3.0.2/venues/stages/somatic/___itinerary/itinerary.S.HTML
+-rwxr-xr-x   0        0        0     1030 2024-04-12 17:13:10.513654 somatic-3.0.2/venues/stages/somatic/___itinerary/possibilities.S.HTML
+-rwxr-xr-x   0        0        0   511709 2024-02-09 00:27:36.294764 somatic-3.0.2/venues/stages/somatic/__book/neem--art-1163780_1920.png
+-rwxr-xr-x   0        0        0      368 2024-04-04 22:59:35.447869 somatic-3.0.2/venues/stages/somatic/__init__.py
+-rwxr-xr-x   0        0        0      362 2024-02-14 04:20:52.275079 somatic-3.0.2/venues/stages/somatic/__license/license.s.HTML
+-rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 somatic-3.0.2/venues/stages/somatic/__license/licenses/gpl-3.0-standalone.html
+-rwxr-xr-x   0        0        0      480 2024-04-04 22:12:45.971487 somatic-3.0.2/venues/stages/somatic/_bin/somatic_1
+-rwxr-xr-x   0        0        0     2645 2024-04-04 23:16:16.911414 somatic-3.0.2/venues/stages/somatic/_clique.py
+-rwxr-xr-x   0        0        0     2040 2024-04-04 22:08:21.454593 somatic-3.0.2/venues/stages/somatic/_controls/flask/__init__.py
+-rwxr-xr-x   0        0        0     2304 2024-04-04 22:09:02.994103 somatic-3.0.2/venues/stages/somatic/_controls/flask/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2848 2024-04-04 22:41:36.732076 somatic-3.0.2/venues/stages/somatic/_controls/sanic/__init__.py
+-rwxr-xr-x   0        0        0     2857 2024-04-04 22:41:38.576055 somatic-3.0.2/venues/stages/somatic/_controls/sanic/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      908 2024-04-16 05:45:15.872591 somatic-3.0.2/venues/stages/somatic/_status/checks/1/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0       25 2024-02-14 04:20:52.283079 somatic-3.0.2/venues/stages/somatic/_status/checks/1/shares/shares 1.s.HTML
+-rwxr-xr-x   0        0        0       25 2024-02-14 04:20:52.295079 somatic-3.0.2/venues/stages/somatic/_status/checks/1/shares/shares 2.s.HTML
+-rwxr-xr-x   0        0        0      659 2024-04-04 20:52:44.678935 somatic-3.0.2/venues/stages/somatic/_status/checks/1/status_1.py
+-rwxr-xr-x   0        0        0     1209 2024-04-16 05:45:35.040347 somatic-3.0.2/venues/stages/somatic/_status/status.proc.py
+-rwxr-xr-x   0        0        0      220 2024-02-14 04:20:52.371078 somatic-3.0.2/venues/stages/somatic/climate/__init__.py
+-rwxr-xr-x   0        0        0      478 2024-02-14 04:22:02.250468 somatic-3.0.2/venues/stages/somatic/climate/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3316 2024-04-04 23:16:01.643597 somatic-3.0.2/venues/stages/somatic/module.MD
+-rwxr-xr-x   0        0        0     2812 2024-03-15 01:31:11.882110 somatic-3.0.2/venues/stages/somatic/module.s.HTML
+-rwxr-xr-x   0        0        0     3550 2024-04-04 21:54:29.564673 somatic-3.0.2/venues/stages/somatic/modules/HTML/__init__.py
+-rwxr-xr-x   0        0        0     3802 2024-04-04 21:56:47.882938 somatic-3.0.2/venues/stages/somatic/modules/HTML/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      275 2024-04-12 16:57:23.456313 somatic-3.0.2/venues/stages/somatic/modules/HTML_templates/template_1.py
+-rwxr-xr-x   0        0        0      718 2024-04-04 20:53:57.226081 somatic-3.0.2/venues/stages/somatic/modules/__pycache__/add_glob_to_paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0      917 2024-02-14 04:22:02.250468 somatic-3.0.2/venues/stages/somatic/modules/__pycache__/parse_extensions.cpython-310.pyc
+-rwxr-xr-x   0        0        0      430 2024-04-04 22:08:04.646791 somatic-3.0.2/venues/stages/somatic/modules/__pycache__/port_in_use.cpython-310.pyc
+-rwxr-xr-x   0        0        0      553 2024-04-04 20:53:54.546112 somatic-3.0.2/venues/stages/somatic/modules/add_glob_to_paths.py
+-rwxr-xr-x   0        0        0      806 2024-02-14 04:20:52.459077 somatic-3.0.2/venues/stages/somatic/modules/parse_extensions.py
+-rwxr-xr-x   0        0        0      270 2024-04-04 22:07:22.315291 somatic-3.0.2/venues/stages/somatic/modules/port_in_use.py
+-rw-r--r--   0        0        0       27 2024-04-12 17:00:56.457658 somatic-3.0.2/venues/stages/somatic/modules/themes/themes.S.HTML
+-rwxr-xr-x   0        0        0      524 2024-01-31 20:00:34.470985 somatic-3.0.2/venues/stages/somatic/modules_ES/address/address.s.HTML
+-rwxr-xr-x   0        0        0     2630 2024-04-04 23:14:00.329057 somatic-3.0.2/venues/stages/somatic/moves/__pycache__/start.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2761 2024-04-04 23:13:56.253106 somatic-3.0.2/venues/stages/somatic/moves/start.py
+-rwxr-xr-x   0        0        0      452 2024-02-14 04:20:52.463077 somatic-3.0.2/venues/stages/somatic/start.proc.py
+-rw-r--r--   0        0        0     4220 1970-01-01 00:00:00.000000 somatic-3.0.2/PKG-INFO
```

### Comparing `somatic-3.0.1/PKG-INFO` & `somatic-3.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: somatic
-Version: 3.0.1
+Version: 3.0.2
 Summary: The best documentation framework every created.
-License: GPL 3.0
-Project-URL: GitLab, https://gitlab.com/offline-money/squash-1/somatic
+License: GPL-3.0-only
 Keywords: documentation
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: click (>=8.1.7,<9.0.0)
+Requires-Dist: factory-farm (>=1.2.3,<2.0.0)
+Requires-Dist: flask (>=3.0.3,<4.0.0)
+Requires-Dist: jsonschema (>=4.21.1,<5.0.0)
+Requires-Dist: law-dictionary (>=1.0.11,<2.0.0)
+Requires-Dist: mako (>=1.3.3,<2.0.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0)
+Requires-Dist: sanic (>=23.12.1,<24.0.0)
+Project-URL: GitLab, https://gitlab.com/offline-money/squash-1/somatic
 Description-Content-Type: text/markdown
-Requires-Dist: volts
-Requires-Dist: law_dictionary
-Requires-Dist: clique
-Requires-Dist: esprima
-Requires-Dist: flask
-Requires-Dist: jsonschema
-Requires-Dist: mako
-Requires-Dist: rich
-Requires-Dist: sanic
 
 
 
 
 ******
 
 Bravo!  You have received a Mercantilism Diploma in "somatic" from   
@@ -178,7 +183,8 @@
 ```
 
 ---
 
 ## contacts
 BGrace2468@pm.me
 
+
```

### Comparing `somatic-3.0.1/readme.md` & `somatic-3.0.2/readme.md`

 * *Files identical despite different names*

### Comparing `somatic-3.0.1/venues/stages/somatic/___itinerary/itinerary.S.HTML` & `somatic-3.0.2/venues/stages/somatic/___itinerary/itinerary.S.HTML`

 * *Files 19% similar despite different names*

```diff
@@ -9,14 +9,50 @@
 	<h1>itinerary</h1>
 		# agenda
 
 	<h2>ranked itinerary</h2>
 	
 		[ ] don't add .png and .jpeg to the select box
 	
+		[ ] themes
+				script:
+					//
+					//	this retrieves somatic theme #1
+					//
+					retrieve_theme ("1")
+				
+			
+		[ ] templates:
+				
+		
+				.stem.S.HTML
+				
+					( ) built with vue-vite-turbo instead of mako, etc.
+				
+				
+				
+				.vue.S.HTML
+				
+					[ ] allows a vue template to be used there?
+					
+						script:
+						
+						template:
+						
+						
+					[ ] dynamic imports:
+							from somatic modules					
+						
+							
+					
+				
+		[ ] wire
+		
+			wire ("")			
+		
 	
 		[ ] home page:
 		
 			possibility:
 				home.S.HTML
```

### Comparing `somatic-3.0.1/venues/stages/somatic/___itinerary/possibilities.S.HTML` & `somatic-3.0.2/venues/stages/somatic/___itinerary/possibilities.S.HTML`

 * *Files 22% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 			that could be like a submenu in the select box.
 			
 			
 		[ ] use a custom select box that has links, a tags, in it,
 			for the purposes of Elastic.co or similar SEO.	
 			
 			
-			
+		[ ] directory: room.S.HTML
+		
+				if directory then...
 			
 	<h2>uhh..</h2>
 
 		[ ] Another server for "somatic" treasures
 	
 			preconfig:
 				&lt;somatic treasures server: 2346&gt;
```

### Comparing `somatic-3.0.1/venues/stages/somatic/__license/licenses/gpl-3.0-standalone.html` & `somatic-3.0.2/venues/stages/somatic/__license/licenses/gpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `somatic-3.0.1/venues/stages/somatic/_clique.py` & `somatic-3.0.2/venues/stages/somatic/_clique.py`

 * *Files identical despite different names*

### Comparing `somatic-3.0.1/venues/stages/somatic/_controls/flask/__init__.py` & `somatic-3.0.2/venues/stages/somatic/_controls/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `somatic-3.0.1/venues/stages/somatic/_controls/sanic/__init__.py` & `somatic-3.0.2/venues/stages/somatic/_controls/sanic/__init__.py`

 * *Files identical despite different names*

### Comparing `somatic-3.0.1/venues/stages/somatic/_status/checks/1/status_1.py` & `somatic-3.0.2/venues/stages/somatic/_status/checks/1/status_1.py`

 * *Files identical despite different names*

### Comparing `somatic-3.0.1/venues/stages/somatic/module.s.HTML` & `somatic-3.0.2/venues/stages/somatic/module.s.HTML`

 * *Files identical despite different names*

### Comparing `somatic-3.0.1/venues/stages/somatic/modules/HTML/__init__.py` & `somatic-3.0.2/venues/stages/somatic/modules/HTML/__init__.py`

 * *Files identical despite different names*

### Comparing `somatic-3.0.1/venues/stages/somatic/modules/add_glob_to_paths.py` & `somatic-3.0.2/venues/stages/somatic/modules/add_glob_to_paths.py`

 * *Files identical despite different names*

### Comparing `somatic-3.0.1/venues/stages/somatic/modules/parse_extensions.py` & `somatic-3.0.2/venues/stages/somatic/modules/parse_extensions.py`

 * *Files identical despite different names*

### Comparing `somatic-3.0.1/venues/stages/somatic/modules_ES/address/address.s.HTML` & `somatic-3.0.2/venues/stages/somatic/modules_ES/address/address.s.HTML`

 * *Files identical despite different names*

### Comparing `somatic-3.0.1/venues/stages/somatic/moves/start.py` & `somatic-3.0.2/venues/stages/somatic/moves/start.py`

 * *Files identical despite different names*

