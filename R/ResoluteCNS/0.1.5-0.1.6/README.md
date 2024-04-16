# Comparing `tmp/resolutecns-0.1.5.tar.gz` & `tmp/resolutecns-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resolutecns-0.1.5.tar", last modified: Tue Apr 16 21:15:03 2024, max compression
+gzip compressed data, was "resolutecns-0.1.6.tar", last modified: Tue Apr 16 21:48:01 2024, max compression
```

## Comparing `resolutecns-0.1.5.tar` & `resolutecns-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 21:15:03.387386 resolutecns-0.1.5/
--rw-rw-rw-   0        0        0       31 2024-04-15 18:34:47.000000 resolutecns-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0      553 2024-04-16 21:15:03.382384 resolutecns-0.1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-16 21:15:03.336387 resolutecns-0.1.5/ResoluteCNS/
--rw-rw-rw-   0        0        0     5973 2024-04-16 21:14:51.000000 resolutecns-0.1.5/ResoluteCNS/ResoluteCNS.py
--rw-rw-rw-   0        0        0       35 2024-04-15 16:59:56.000000 resolutecns-0.1.5/ResoluteCNS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 21:15:03.373385 resolutecns-0.1.5/ResoluteCNS/bankruptcies/
--rw-rw-rw-   0        0        0       37 2024-04-15 20:45:24.000000 resolutecns-0.1.5/ResoluteCNS/bankruptcies/__init__.py
--rw-rw-rw-   0        0        0     1889 2024-04-16 19:15:21.000000 resolutecns-0.1.5/ResoluteCNS/bankruptcies/bankruptcies.py
--rw-rw-rw-   0        0        0  3834815 2024-02-29 20:00:53.000000 resolutecns-0.1.5/ResoluteCNS/uBlock0.xpi
-drwxrwxrwx   0        0        0        0 2024-04-16 21:15:03.378556 resolutecns-0.1.5/ResoluteCNS.egg-info/
--rw-rw-rw-   0        0        0      553 2024-04-16 21:15:03.000000 resolutecns-0.1.5/ResoluteCNS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2024-04-16 21:15:03.000000 resolutecns-0.1.5/ResoluteCNS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 21:15:03.000000 resolutecns-0.1.5/ResoluteCNS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-16 21:15:03.000000 resolutecns-0.1.5/ResoluteCNS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-16 21:15:03.000000 resolutecns-0.1.5/ResoluteCNS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 21:15:03.388386 resolutecns-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1146 2024-04-16 21:08:14.000000 resolutecns-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 21:48:01.532846 resolutecns-0.1.6/
+-rw-rw-rw-   0        0        0       31 2024-04-15 18:34:47.000000 resolutecns-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      553 2024-04-16 21:48:01.526842 resolutecns-0.1.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-16 21:48:01.471842 resolutecns-0.1.6/ResoluteCNS/
+-rw-rw-rw-   0        0        0     6139 2024-04-16 21:47:38.000000 resolutecns-0.1.6/ResoluteCNS/ResoluteCNS.py
+-rw-rw-rw-   0        0        0       35 2024-04-15 16:59:56.000000 resolutecns-0.1.6/ResoluteCNS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 21:48:01.513844 resolutecns-0.1.6/ResoluteCNS/bankruptcies/
+-rw-rw-rw-   0        0        0       37 2024-04-15 20:45:24.000000 resolutecns-0.1.6/ResoluteCNS/bankruptcies/__init__.py
+-rw-rw-rw-   0        0        0     1889 2024-04-16 19:15:21.000000 resolutecns-0.1.6/ResoluteCNS/bankruptcies/bankruptcies.py
+-rw-rw-rw-   0        0        0  3834815 2024-02-29 20:00:53.000000 resolutecns-0.1.6/ResoluteCNS/uBlock0.xpi
+drwxrwxrwx   0        0        0        0 2024-04-16 21:48:01.520963 resolutecns-0.1.6/ResoluteCNS.egg-info/
+-rw-rw-rw-   0        0        0      553 2024-04-16 21:48:01.000000 resolutecns-0.1.6/ResoluteCNS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2024-04-16 21:48:01.000000 resolutecns-0.1.6/ResoluteCNS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 21:48:01.000000 resolutecns-0.1.6/ResoluteCNS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-16 21:48:01.000000 resolutecns-0.1.6/ResoluteCNS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-16 21:48:01.000000 resolutecns-0.1.6/ResoluteCNS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 21:48:01.533846 resolutecns-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1146 2024-04-16 21:47:55.000000 resolutecns-0.1.6/setup.py
```

### Comparing `resolutecns-0.1.5/PKG-INFO` & `resolutecns-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResoluteCNS
-Version: 0.1.5
+Version: 0.1.6
 Summary: CNS Scraping Package
 Author: Ryan Detlaff
 Author-email: rdetlaff@resolutecommercial.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `resolutecns-0.1.5/ResoluteCNS/ResoluteCNS.py` & `resolutecns-0.1.6/ResoluteCNS/ResoluteCNS.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,14 +58,15 @@
         self.click_search()
         return self.download_excel()
     
     def setup_date_filters(self, from_date, to_date):
         from_date_field = self._driver.find_element(By.CLASS_NAME, 'datepicker')
         from_date_field.send_keys(from_date)
         
+        
     def setup_court_filters(self, in_courts):
 
         courts = self._driver.find_elements(By.XPATH, "//input[@name='BankoCourts']/following-sibling::label")
 
         for court in courts:
             if validate_court(in_courts, court):
                 court_check = self._driver.find_element(By.ID, court.get_attribute('for'))
@@ -97,24 +98,26 @@
             from_date = now.strftime("%m/%d/%Y")
         if not to_date:
             from_date = now.strftime("%m/%d/%Y")
 
         #URL of the website     
         url = self._baseurl + "SearchBeta/Complaints"
         self._driver.get(url)
+        time.sleep(1)
+        self.setup_date_filters(from_date, to_date)
 
         if states:
             self.set_state_filters(states)
         if counties:
             self.set_county_filters(counties)
         
         self.click_search_complaints()
 
         self.download_excel_complaints()
-        
+
 
     def download_excel_complaints(self):
         self._driver.set_page_load_timeout(10)
         try:
             download_excel = self._driver.find_elements(By.XPATH, "//a[@href='/SearchBeta/GetComplaintsExcel']/child::img")
             download_excel.click()
         except Exception as e:
@@ -135,19 +138,22 @@
         states = self._driver.find_elements(By.XPATH, "//input[@name='States']")
         in_states = list(in_counties.keys())
 
         for state in states:
             if validate_state(in_states, state):
                 state_name = state.get_attribute('id')
                 self._driver.find_element(By.XPATH, f"//div[contains(text(), '{state_name}')][@class='statealphabutton']").click()
+                time.sleep(2)
                 
                 for county in in_counties[state_name]:
                     self._driver.find_element(By.XPATH, f"//label[contains(text(), '{county}')]").click()
+                
+                self._driver.find_element(By.XPATH, f"//span[@onclick='ShowStates();']").click()
+                time.sleep(2)
         
-        self._driver.find_element(By.XPATH, f"//span[@onclick='ShowStates();']").click()
     
     def click_search_complaints(self):
         self._driver.find_element(By.ID, 'button_submittop').click()
 
 def download_folder(filename):
     home = os.path.expanduser("~")
     download_path = home + os.sep + "Downloads"
```

### Comparing `resolutecns-0.1.5/ResoluteCNS/bankruptcies/bankruptcies.py` & `resolutecns-0.1.6/ResoluteCNS/bankruptcies/bankruptcies.py`

 * *Files identical despite different names*

### Comparing `resolutecns-0.1.5/ResoluteCNS/uBlock0.xpi` & `resolutecns-0.1.6/ResoluteCNS/uBlock0.xpi`

 * *Files identical despite different names*

### Comparing `resolutecns-0.1.5/ResoluteCNS.egg-info/PKG-INFO` & `resolutecns-0.1.6/ResoluteCNS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResoluteCNS
-Version: 0.1.5
+Version: 0.1.6
 Summary: CNS Scraping Package
 Author: Ryan Detlaff
 Author-email: rdetlaff@resolutecommercial.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `resolutecns-0.1.5/setup.py` & `resolutecns-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.5' 
+VERSION = '0.1.6' 
 DESCRIPTION = 'CNS Scraping Package'
 LONG_DESCRIPTION = 'CNS Scraping Package'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="ResoluteCNS",
```
