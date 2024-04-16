# Comparing `tmp/resolutecns-0.1.2.tar.gz` & `tmp/resolutecns-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resolutecns-0.1.2.tar", last modified: Tue Apr 16 18:24:08 2024, max compression
+gzip compressed data, was "resolutecns-0.1.3.tar", last modified: Tue Apr 16 20:57:18 2024, max compression
```

## Comparing `resolutecns-0.1.2.tar` & `resolutecns-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 18:24:08.563477 resolutecns-0.1.2/
--rw-rw-rw-   0        0        0       31 2024-04-15 18:34:47.000000 resolutecns-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0      553 2024-04-16 18:24:08.557478 resolutecns-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-16 18:24:08.508477 resolutecns-0.1.2/ResoluteCNS/
--rw-rw-rw-   0        0        0     3521 2024-04-16 18:23:29.000000 resolutecns-0.1.2/ResoluteCNS/ResoluteCNS.py
--rw-rw-rw-   0        0        0       35 2024-04-15 16:59:56.000000 resolutecns-0.1.2/ResoluteCNS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 18:24:08.546477 resolutecns-0.1.2/ResoluteCNS/bankruptcies/
--rw-rw-rw-   0        0        0       37 2024-04-15 20:45:24.000000 resolutecns-0.1.2/ResoluteCNS/bankruptcies/__init__.py
--rw-rw-rw-   0        0        0     1819 2024-04-16 18:19:44.000000 resolutecns-0.1.2/ResoluteCNS/bankruptcies/bankruptcies.py
--rw-rw-rw-   0        0        0  3834815 2024-02-29 20:00:53.000000 resolutecns-0.1.2/ResoluteCNS/uBlock0.xpi
-drwxrwxrwx   0        0        0        0 2024-04-16 18:24:08.552915 resolutecns-0.1.2/ResoluteCNS.egg-info/
--rw-rw-rw-   0        0        0      553 2024-04-16 18:24:08.000000 resolutecns-0.1.2/ResoluteCNS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2024-04-16 18:24:08.000000 resolutecns-0.1.2/ResoluteCNS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 18:24:08.000000 resolutecns-0.1.2/ResoluteCNS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-16 18:24:08.000000 resolutecns-0.1.2/ResoluteCNS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-16 18:24:08.000000 resolutecns-0.1.2/ResoluteCNS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 18:24:08.563477 resolutecns-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1146 2024-04-16 18:24:05.000000 resolutecns-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 20:57:18.533139 resolutecns-0.1.3/
+-rw-rw-rw-   0        0        0       31 2024-04-15 18:34:47.000000 resolutecns-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      553 2024-04-16 20:57:18.527141 resolutecns-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-16 20:57:18.478139 resolutecns-0.1.3/ResoluteCNS/
+-rw-rw-rw-   0        0        0     5240 2024-04-16 20:53:43.000000 resolutecns-0.1.3/ResoluteCNS/ResoluteCNS.py
+-rw-rw-rw-   0        0        0       35 2024-04-15 16:59:56.000000 resolutecns-0.1.3/ResoluteCNS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 20:57:18.513141 resolutecns-0.1.3/ResoluteCNS/bankruptcies/
+-rw-rw-rw-   0        0        0       37 2024-04-15 20:45:24.000000 resolutecns-0.1.3/ResoluteCNS/bankruptcies/__init__.py
+-rw-rw-rw-   0        0        0     1889 2024-04-16 19:15:21.000000 resolutecns-0.1.3/ResoluteCNS/bankruptcies/bankruptcies.py
+-rw-rw-rw-   0        0        0  3834815 2024-02-29 20:00:53.000000 resolutecns-0.1.3/ResoluteCNS/uBlock0.xpi
+drwxrwxrwx   0        0        0        0 2024-04-16 20:57:18.520139 resolutecns-0.1.3/ResoluteCNS.egg-info/
+-rw-rw-rw-   0        0        0      553 2024-04-16 20:57:18.000000 resolutecns-0.1.3/ResoluteCNS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2024-04-16 20:57:18.000000 resolutecns-0.1.3/ResoluteCNS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 20:57:18.000000 resolutecns-0.1.3/ResoluteCNS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-16 20:57:18.000000 resolutecns-0.1.3/ResoluteCNS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-16 20:57:18.000000 resolutecns-0.1.3/ResoluteCNS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 20:57:18.533139 resolutecns-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1146 2024-04-16 20:57:12.000000 resolutecns-0.1.3/setup.py
```

### Comparing `resolutecns-0.1.2/PKG-INFO` & `resolutecns-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResoluteCNS
-Version: 0.1.2
+Version: 0.1.3
 Summary: CNS Scraping Package
 Author: Ryan Detlaff
 Author-email: rdetlaff@resolutecommercial.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `resolutecns-0.1.2/ResoluteCNS/bankruptcies/bankruptcies.py` & `resolutecns-0.1.3/ResoluteCNS/bankruptcies/bankruptcies.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 from selenium.webdriver.common.by import By
+from ResoluteCNS import ResoluteCNS
 
 class Bankruptcies:
-    def __init__(self, driv):
-         self._driver = driv
-      
+    def __init__(self):
+      pass
+
     def get(self, courts, from_date, to_date):
-            if not self._logged_in:
-                self.login()
+            if not cns._logged_in:
+                cns.login()
 
             #URL of the website     
             url = self._baseurl + "SearchBeta/Bankruptcy"
-            self._selfer.get(url)
+            cns._driver.get(url)
             self.setup_date_filters(from_date, to_date)
             self.setup_court_filters(courts)
             self.click_search()
             return self.download_excel()
 
     def setup_date_filters(self, from_date, to_date):
-        from_date_field = self._driver.find_element(By.CLASS_NAME, 'datepicker')
+        from_date_field = ResoluteCNS.CNS._driver.find_element(By.CLASS_NAME, 'datepicker')
         from_date_field.send_keys(from_date)
         
     def setup_court_filters(self, in_courts):
 
-        courts = self._driver.find_elements(By.XPATH, "//input[@name='BankoCourts']/following-sibling::label")
+        courts = ResoluteCNS.CNS._driver.find_elements(By.XPATH, "//input[@name='BankoCourts']/following-sibling::label")
 
         for court in courts:
             if validate_court(in_courts, court):
-                court_check = self._driver.find_element(By.ID, court.get_attribute('for'))
+                court_check = ResoluteCNS.CNS._driver.find_element(By.ID, court.get_attribute('for'))
                 court_check.click()
 
 
     def click_search(self):
-        self._driver.find_element(By.ID, 'button_submitbanko').click()
+        ResoluteCNS.CNS._driver.find_element(By.ID, 'button_submitbanko').click()
         
 
     def download_excel(self):
-            self._driver.set_page_load_timeout(10)
+            ResoluteCNS.CNS._driver.set_page_load_timeout(10)
             try:
-                download_excel = self._driver.find_elements(By.XPATH, "//a[@href='/SearchBeta/GetBankoExcel']/child::img")
+                download_excel = ResoluteCNS.CNS._driver.find_elements(By.XPATH, "//a[@href='/SearchBeta/GetBankoExcel']/child::img")
                 download_excel.click()
             except Exception as e:
                 print(e)
             
             return True
```

### Comparing `resolutecns-0.1.2/ResoluteCNS/uBlock0.xpi` & `resolutecns-0.1.3/ResoluteCNS/uBlock0.xpi`

 * *Files identical despite different names*

### Comparing `resolutecns-0.1.2/ResoluteCNS.egg-info/PKG-INFO` & `resolutecns-0.1.3/ResoluteCNS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResoluteCNS
-Version: 0.1.2
+Version: 0.1.3
 Summary: CNS Scraping Package
 Author: Ryan Detlaff
 Author-email: rdetlaff@resolutecommercial.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `resolutecns-0.1.2/setup.py` & `resolutecns-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.2' 
+VERSION = '0.1.3' 
 DESCRIPTION = 'CNS Scraping Package'
 LONG_DESCRIPTION = 'CNS Scraping Package'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="ResoluteCNS",
```

