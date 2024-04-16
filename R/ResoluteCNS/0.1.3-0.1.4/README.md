# Comparing `tmp/resolutecns-0.1.3.tar.gz` & `tmp/resolutecns-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resolutecns-0.1.3.tar", last modified: Tue Apr 16 20:57:18 2024, max compression
+gzip compressed data, was "resolutecns-0.1.4.tar", last modified: Tue Apr 16 21:04:35 2024, max compression
```

## Comparing `resolutecns-0.1.3.tar` & `resolutecns-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 20:57:18.533139 resolutecns-0.1.3/
--rw-rw-rw-   0        0        0       31 2024-04-15 18:34:47.000000 resolutecns-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0      553 2024-04-16 20:57:18.527141 resolutecns-0.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-16 20:57:18.478139 resolutecns-0.1.3/ResoluteCNS/
--rw-rw-rw-   0        0        0     5240 2024-04-16 20:53:43.000000 resolutecns-0.1.3/ResoluteCNS/ResoluteCNS.py
--rw-rw-rw-   0        0        0       35 2024-04-15 16:59:56.000000 resolutecns-0.1.3/ResoluteCNS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 20:57:18.513141 resolutecns-0.1.3/ResoluteCNS/bankruptcies/
--rw-rw-rw-   0        0        0       37 2024-04-15 20:45:24.000000 resolutecns-0.1.3/ResoluteCNS/bankruptcies/__init__.py
--rw-rw-rw-   0        0        0     1889 2024-04-16 19:15:21.000000 resolutecns-0.1.3/ResoluteCNS/bankruptcies/bankruptcies.py
--rw-rw-rw-   0        0        0  3834815 2024-02-29 20:00:53.000000 resolutecns-0.1.3/ResoluteCNS/uBlock0.xpi
-drwxrwxrwx   0        0        0        0 2024-04-16 20:57:18.520139 resolutecns-0.1.3/ResoluteCNS.egg-info/
--rw-rw-rw-   0        0        0      553 2024-04-16 20:57:18.000000 resolutecns-0.1.3/ResoluteCNS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2024-04-16 20:57:18.000000 resolutecns-0.1.3/ResoluteCNS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 20:57:18.000000 resolutecns-0.1.3/ResoluteCNS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-16 20:57:18.000000 resolutecns-0.1.3/ResoluteCNS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-16 20:57:18.000000 resolutecns-0.1.3/ResoluteCNS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 20:57:18.533139 resolutecns-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1146 2024-04-16 20:57:12.000000 resolutecns-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 21:04:35.013610 resolutecns-0.1.4/
+-rw-rw-rw-   0        0        0       31 2024-04-15 18:34:47.000000 resolutecns-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      553 2024-04-16 21:04:35.005604 resolutecns-0.1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-16 21:04:34.951294 resolutecns-0.1.4/ResoluteCNS/
+-rw-rw-rw-   0        0        0     5301 2024-04-16 21:04:20.000000 resolutecns-0.1.4/ResoluteCNS/ResoluteCNS.py
+-rw-rw-rw-   0        0        0       35 2024-04-15 16:59:56.000000 resolutecns-0.1.4/ResoluteCNS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 21:04:34.994608 resolutecns-0.1.4/ResoluteCNS/bankruptcies/
+-rw-rw-rw-   0        0        0       37 2024-04-15 20:45:24.000000 resolutecns-0.1.4/ResoluteCNS/bankruptcies/__init__.py
+-rw-rw-rw-   0        0        0     1889 2024-04-16 19:15:21.000000 resolutecns-0.1.4/ResoluteCNS/bankruptcies/bankruptcies.py
+-rw-rw-rw-   0        0        0  3834815 2024-02-29 20:00:53.000000 resolutecns-0.1.4/ResoluteCNS/uBlock0.xpi
+drwxrwxrwx   0        0        0        0 2024-04-16 21:04:35.001620 resolutecns-0.1.4/ResoluteCNS.egg-info/
+-rw-rw-rw-   0        0        0      553 2024-04-16 21:04:34.000000 resolutecns-0.1.4/ResoluteCNS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2024-04-16 21:04:34.000000 resolutecns-0.1.4/ResoluteCNS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 21:04:34.000000 resolutecns-0.1.4/ResoluteCNS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-16 21:04:34.000000 resolutecns-0.1.4/ResoluteCNS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-16 21:04:34.000000 resolutecns-0.1.4/ResoluteCNS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 21:04:35.013610 resolutecns-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1146 2024-04-16 21:02:17.000000 resolutecns-0.1.4/setup.py
```

### Comparing `resolutecns-0.1.3/PKG-INFO` & `resolutecns-0.1.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResoluteCNS
-Version: 0.1.3
+Version: 0.1.4
 Summary: CNS Scraping Package
 Author: Ryan Detlaff
 Author-email: rdetlaff@resolutecommercial.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `resolutecns-0.1.3/ResoluteCNS/ResoluteCNS.py` & `resolutecns-0.1.4/ResoluteCNS/ResoluteCNS.py`

 * *Files 7% similar despite different names*

```diff
@@ -117,15 +117,16 @@
     
     def set_county_filters(self, in_counties):
         states = self._driver.find_elements(By.XPATH, "//input[@name='States']")
         in_states = list(in_counties.keys())
 
         for state in states:
             if validate_state(in_states, state):
-                self._driver.find_element(By.XPATH, f"//div[contains(text(), '{state}')][@class='statealphabutton']").click()
+                state_name = state.get_attribute('id')
+                self._driver.find_element(By.XPATH, f"//div[contains(text(), '{state_name}')][@class='statealphabutton']").click()
                 
                 for county in in_counties[state]:
                     self._driver.find_element(By.XPATH, f"//label[contains(text(), {county})]").click()
         
         self._driver.find_element(By.XPATH, f"//span[@onclick='ShowStates();']").click()
```

### Comparing `resolutecns-0.1.3/ResoluteCNS/bankruptcies/bankruptcies.py` & `resolutecns-0.1.4/ResoluteCNS/bankruptcies/bankruptcies.py`

 * *Files identical despite different names*

### Comparing `resolutecns-0.1.3/ResoluteCNS/uBlock0.xpi` & `resolutecns-0.1.4/ResoluteCNS/uBlock0.xpi`

 * *Files identical despite different names*

### Comparing `resolutecns-0.1.3/ResoluteCNS.egg-info/PKG-INFO` & `resolutecns-0.1.4/ResoluteCNS.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResoluteCNS
-Version: 0.1.3
+Version: 0.1.4
 Summary: CNS Scraping Package
 Author: Ryan Detlaff
 Author-email: rdetlaff@resolutecommercial.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `resolutecns-0.1.3/setup.py` & `resolutecns-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.3' 
+VERSION = '0.1.4' 
 DESCRIPTION = 'CNS Scraping Package'
 LONG_DESCRIPTION = 'CNS Scraping Package'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="ResoluteCNS",
```

