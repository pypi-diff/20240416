# Comparing `tmp/unbirthday-1.0.3.tar.gz` & `tmp/unbirthday-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unbirthday-1.0.3.tar", last modified: Wed Apr 10 02:19:26 2024, max compression
+gzip compressed data, was "unbirthday-1.0.4.tar", last modified: Tue Apr 16 11:24:04 2024, max compression
```

## Comparing `unbirthday-1.0.3.tar` & `unbirthday-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 02:19:26.560007 unbirthday-1.0.3/
--rw-rw-rw-   0        0        0     8141 2024-04-10 02:19:26.560007 unbirthday-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     7876 2024-04-09 07:05:19.000000 unbirthday-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-10 02:19:26.560007 unbirthday-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      521 2024-04-10 02:15:33.000000 unbirthday-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 02:19:26.544382 unbirthday-1.0.3/unbirthday/
--rw-rw-rw-   0        0        0      177 2024-04-09 06:02:18.000000 unbirthday-1.0.3/unbirthday/__init__.py
--rw-rw-rw-   0        0        0     6909 2024-04-10 02:12:03.000000 unbirthday-1.0.3/unbirthday/unbirthday.py
-drwxrwxrwx   0        0        0        0 2024-04-10 02:19:26.560007 unbirthday-1.0.3/unbirthday.egg-info/
--rw-rw-rw-   0        0        0     8141 2024-04-10 02:19:26.000000 unbirthday-1.0.3/unbirthday.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-04-10 02:19:26.000000 unbirthday-1.0.3/unbirthday.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 02:19:26.000000 unbirthday-1.0.3/unbirthday.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-10 02:19:26.000000 unbirthday-1.0.3/unbirthday.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 11:24:04.822162 unbirthday-1.0.4/
+-rw-rw-rw-   0        0        0     8141 2024-04-16 11:24:04.821162 unbirthday-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     7876 2024-04-09 07:05:19.000000 unbirthday-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-16 11:24:04.822162 unbirthday-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      521 2024-04-16 11:15:39.000000 unbirthday-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 11:24:04.816162 unbirthday-1.0.4/unbirthday/
+-rw-rw-rw-   0        0        0      177 2024-04-09 06:02:18.000000 unbirthday-1.0.4/unbirthday/__init__.py
+-rw-rw-rw-   0        0        0     7066 2024-04-16 11:16:11.000000 unbirthday-1.0.4/unbirthday/unbirthday.py
+drwxrwxrwx   0        0        0        0 2024-04-16 11:24:04.821162 unbirthday-1.0.4/unbirthday.egg-info/
+-rw-rw-rw-   0        0        0     8141 2024-04-16 11:24:04.000000 unbirthday-1.0.4/unbirthday.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2024-04-16 11:24:04.000000 unbirthday-1.0.4/unbirthday.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 11:24:04.000000 unbirthday-1.0.4/unbirthday.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-16 11:24:04.000000 unbirthday-1.0.4/unbirthday.egg-info/top_level.txt
```

### Comparing `unbirthday-1.0.3/PKG-INFO` & `unbirthday-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unbirthday
-Version: 1.0.3
+Version: 1.0.4
 Summary: Unbirthday is a Python module that provides functions to calculate and manage "unbirthdays," which are days celebrated as not being a person's birthday.
 Description-Content-Type: text/markdown
 
 # Unbirthday (Calculator)
 
 ## Introduction
```

### Comparing `unbirthday-1.0.3/README.md` & `unbirthday-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `unbirthday-1.0.3/setup.py` & `unbirthday-1.0.4/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name="unbirthday",
-    version="1.0.3",
+    version="1.0.4",
     description="Unbirthday is a Python module that provides functions to calculate and manage \"unbirthdays,\" which are days celebrated as not being a person's birthday.",
     packages=find_packages(),
     install_requires=[
         #no packages needed
     ],
     long_description=description,
     long_description_content_type="text/markdown",
```

### Comparing `unbirthday-1.0.3/unbirthday/unbirthday.py` & `unbirthday-1.0.4/unbirthday/unbirthday.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from datetime import datetime, timedelta
 import math
 
-def add_ordinal_indicator(num):
+def add_ordinal_indicator(num: int) -> str:
     '''Adds the ordinal indicator (e.g., "st", "nd", "rd", "th") to a given number.'''
     if 10 <= num % 100 <= 20:
         suffix = 'th'
     else:
         suffix = {1: 'st', 2: 'nd', 3: 'rd'}.get(num % 10, 'th')
     return str(num) + suffix
 
-def get_todays_date():
+def get_todays_date() -> str:
     '''Gets the current date in the format "YYYY-MM-DD".'''
     return datetime.today().strftime('%Y-%m-%d')
 
-def is_leap_year(year):
+def is_leap_year(year: int):
     return year % 4 == 0 and (year % 100 != 0 or year % 400 == 0)
 
-def years_passed(start_date, end_date=None):
+def years_passed(start_date: str, end_date: str = None) -> int:
     '''Calculates the number of years passed between two dates.'''
     if end_date == None:
         end_date = get_todays_date()
 
     start_year, start_month, start_day = map(int, start_date.split('-'))
     end_year, end_month, end_day = map(int, end_date.split('-'))
     
@@ -35,15 +35,15 @@
         if is_leap_year(start_year) and start_month == 2 and start_day == 29:
             # If start_date is Feb 29th of a leap year, check if end_date's year is a leap year
             if not is_leap_year(end_year):
                 years_diff -= 1
     
     return years_diff
 
-def your_current_day_on_earth(start_date, end_date=None):
+def your_current_day_on_earth(start_date: str, end_date: str = None) -> int:
     '''Calculates the number of days between two dates.'''
     if end_date == None:
         end_date = get_todays_date()
 
     # Convert the string dates to datetime objects
     d1 = datetime.strptime(start_date, "%Y-%m-%d")
     d2 = datetime.strptime(end_date, "%Y-%m-%d")
@@ -51,15 +51,15 @@
     # Calculate the difference between the two dates
     delta = abs(d2 - d1).days + 1
 
     # Return the difference in days
     return delta
 
 
-def calculate_unbirthday(start_date, end_date=None):
+def calculate_unbirthday(start_date: str, end_date: str = None) -> int:
     '''Calculates the current unbirthday based on the provided start and end dates.'''
     if end_date == None:
         end_date = get_todays_date()
 
     # How to calculate unbirthdays
 
     # 1. Take your current day on earth
@@ -80,15 +80,15 @@
 
 
     # There you go! Your current unbirthday!
     return unbirthday
 
 
 
-def unbirthday_enddate_to_years(amount_of_days, end_date):
+def unbirthday_enddate_to_years(amount_of_days: int, end_date: str):
     end_date = datetime.strptime(end_date, '%Y-%m-%d')
     amount_of_days = amount_of_days - 1
     years_back = 0
 
     while amount_of_days >= 365:
         if is_leap_year(end_date.year - 1):
             # If the previous year was a leap year, subtract 366 days
@@ -102,27 +102,27 @@
         # Add one day to the remaining amount of days
         amount_of_days += 1
         # Increment the count of years gone back
         years_back += 1
 
     return years_back
 
-def count_back_past_date(days, input_date):
+def count_back_past_date(days: int, input_date: str):
     # Convert the input date string to a datetime object
     days = days - 1
     date_format = "%Y-%m-%d"
     current_date = datetime.strptime(input_date, date_format)
     
     # Calculate the new date by subtracting the days
     new_date = current_date - timedelta(days=days)
     
     # Convert the new date back to a string and return it
     return new_date.strftime(date_format)
 
-def find_startdate_unbirthday(unbirthday, end_date=None):
+def find_startdate_unbirthday(unbirthday: int, end_date: str = None) -> str:
     '''Calculates the start date (birth date) based on the provided unbirthday and end dates.'''
     if end_date == None:
         end_date = get_todays_date()
     
     # Assume how many birthdays has passed based on the amount of unbirthdays
     birthdays = unbirthday_enddate_to_years(unbirthday, end_date)
 
@@ -136,15 +136,15 @@
     # Count backwards the amount of days
     reverse_unbirthday = count_back_past_date(reverse_your_current_day_on_earth, end_date)
 
     return reverse_unbirthday
 
 
 
-def unbirthday_startdate_to_years(amount_of_days, start_date):
+def unbirthday_startdate_to_years(amount_of_days: int, start_date: str):
     start_date = datetime.strptime(start_date, '%Y-%m-%d')
     amount_of_days = amount_of_days - 1
     years_forward = 0
 
     while amount_of_days >= 365:
         if is_leap_year(start_date.year + 1):
             # If the current year is a leap year, add 366 days
@@ -158,28 +158,28 @@
         # Add one day to the remaining amount of days
         amount_of_days += 1
         # Increment the count of years gone forward
         years_forward += 1
 
     return years_forward
 
-def count_forward_future_date(days, input_date):
+def count_forward_future_date(days: int, input_date: str):
     days = days - 1
 
     # Convert the input date string to a datetime object
     date_format = "%Y-%m-%d"
     current_date = datetime.strptime(input_date, date_format)
     
     # Calculate the new date by adding the days
     new_date = current_date + timedelta(days=days)
     
     # Convert the new date back to a string and return it
     return new_date.strftime(date_format)
 
-def find_enddate_unbirthday(unbirthday, start_date):
+def find_enddate_unbirthday(unbirthday: int, start_date: str) -> str:
     '''Calculates the end date (current date) based on the provided unbirthday and start dates.'''
     # Assume how many birthdays will pass based on the amount of unbirthdays
     birthdays = unbirthday_startdate_to_years(unbirthday, start_date)
 
     # To reverse the unbirthday:
     # Add one because the day you were born
     reverse_your_current_day_on_earth = unbirthday + 1
```

### Comparing `unbirthday-1.0.3/unbirthday.egg-info/PKG-INFO` & `unbirthday-1.0.4/unbirthday.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unbirthday
-Version: 1.0.3
+Version: 1.0.4
 Summary: Unbirthday is a Python module that provides functions to calculate and manage "unbirthdays," which are days celebrated as not being a person's birthday.
 Description-Content-Type: text/markdown
 
 # Unbirthday (Calculator)
 
 ## Introduction
```

