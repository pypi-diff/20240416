# Comparing `tmp/datewise-0.1.6.tar.gz` & `tmp/datewise-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datewise-0.1.6.tar", last modified: Sat Apr  6 12:11:49 2024, max compression
+gzip compressed data, was "datewise-0.2.0.tar", last modified: Tue Apr 16 11:28:40 2024, max compression
```

## Comparing `datewise-0.1.6.tar` & `datewise-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:11:49.083352 datewise-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-06 12:11:49.083352 datewise-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-06 12:11:22.000000 datewise-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:11:49.079352 datewise-0.1.6/datewise/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-06 12:11:22.000000 datewise-0.1.6/datewise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19464 2024-04-06 12:11:22.000000 datewise-0.1.6/datewise/datewise.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:11:49.079352 datewise-0.1.6/datewise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-06 12:11:49.000000 datewise-0.1.6/datewise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-06 12:11:49.000000 datewise-0.1.6/datewise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 12:11:49.000000 datewise-0.1.6/datewise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-06 12:11:49.000000 datewise-0.1.6/datewise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-06 12:11:49.000000 datewise-0.1.6/datewise.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 12:11:49.083352 datewise-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-06 12:11:22.000000 datewise-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:11:49.079352 datewise-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    27284 2024-04-06 12:11:22.000000 datewise-0.1.6/tests/test_functionality.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:28:40.652130 datewise-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-16 11:28:40.652130 datewise-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-16 11:28:23.000000 datewise-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:28:40.648130 datewise-0.2.0/datewise/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-16 11:28:23.000000 datewise-0.2.0/datewise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20958 2024-04-16 11:28:23.000000 datewise-0.2.0/datewise/datewise.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:28:40.652130 datewise-0.2.0/datewise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-16 11:28:40.000000 datewise-0.2.0/datewise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-16 11:28:40.000000 datewise-0.2.0/datewise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 11:28:40.000000 datewise-0.2.0/datewise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-16 11:28:40.000000 datewise-0.2.0/datewise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 11:28:40.000000 datewise-0.2.0/datewise.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 11:28:40.652130 datewise-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-16 11:28:23.000000 datewise-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:28:40.652130 datewise-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    29294 2024-04-16 11:28:23.000000 datewise-0.2.0/tests/test_functionality.py
```

### Comparing `datewise-0.1.6/PKG-INFO` & `datewise-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datewise
-Version: 0.1.6
+Version: 0.2.0
 Summary: Thesis Library
 Home-page: https://datewise.readthedocs.io/
 Author: Sebastian Gontkovic
 Author-email: sebascngont@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `datewise-0.1.6/datewise/datewise.py` & `datewise-0.2.0/datewise/datewise.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from datetime import datetime, timedelta
 from typing import Union
 import pandas as pd
 
+operations = ['+', '-']
+comparison = ['==', '<=', '<', '>', '>=']
+
 def identify_date_format(date: Union[str, datetime, pd._libs.tslibs.timestamps.Timestamp]) -> str:
 
     """
     Identify date format of input date based on pre-determined widely used formats.
 
     :param date: The date given by a user to identify it's format 
     :type date: str, datetime, pd._libs.tslibs.timestamps.Timestamp
@@ -66,15 +69,15 @@
         return "Pandas Timestamp type, no specific format"
     elif isinstance(date, datetime):
         return "Datetime type, no specific format"
     else:
         raise ValueError("Unknow data type of date variable")
 
  
-def date_comparison(date_1= Union[str, datetime, pd._libs.tslibs.timestamps.Timestamp], date_2= Union[str, datetime, pd._libs.tslibs.timestamps.Timestamp], operation=str) -> bool:
+def date_comparison(date_1: Union[str, datetime, pd._libs.tslibs.timestamps.Timestamp], date_2: Union[str, datetime, pd._libs.tslibs.timestamps.Timestamp], operation: str) -> bool:
 
     """
     Compare two dates given by a surer based on chosen comparison operator
 
     :param date1: Date no. 1 given by a user to be compared
     :type date1: str, datetime, pd._libs.tslibs.timestamps.Timestamp
 
@@ -82,20 +85,21 @@
     :type date2: str, datetime, pd._libs.tslibs.timestamps.Timestamp
 
     :param operation: Any valid comparison sign in string format
     :type operation: str 
     
     :return: True or False value based on a result
     :rtype: bool
-
     """
 
-    
-    if date_1 and date_2 and operation:
 
+    global comparison 
+
+    if isinstance(operation, str) and operation in comparison and isinstance(date_1, (str, pd._libs.tslibs.timestamps.Timestamp, datetime)) and isinstance(date_2, (str, pd._libs.tslibs.timestamps.Timestamp, datetime)):
+        
         if isinstance(date_1, str) and isinstance(date_2, str): 
 
             date1_comparison = datetime.strptime(date_1, identify_date_format(date=date_1)) 
             date2_comparison = datetime.strptime(date_2, identify_date_format(date=date_2)) 
 
             if operation == "==":
 
@@ -126,23 +130,22 @@
 
                 date_1 = date_convert(date_1, 'str', '%Y-%m-%d')
 
             elif date_2_type != str:
 
                 date_2 = date_convert(date_2, 'str', '%Y-%m-%d')
 
-            return date_comparison(date_1, date_2, operation)        
-        else:
+            return date_comparison(date_1, date_2, operation) 
             
-            raise ValueError("Provided inputs are uncomperable"  )
+        else:
+            raise ValueError("Unable to complete such request. Check input variables.")
+    
+    else:
+        raise ValueError('Incorrect data type or value in an input parameter')
     
-    else: 
-
-        raise ValueError('Missing variable')
-
 
 def week_start(date: Union[str, datetime, pd._libs.tslibs.timestamps.Timestamp]) -> str:
  
     """
     Find the start of the specific week based on a given date
 
     :param date: The date given by a user to identify start of the week that the date is in 
@@ -160,26 +163,29 @@
         if fmt:
 
             weekday = datetime.strptime(date, fmt).weekday()
 
             date_start = (datetime.strptime(date, fmt) - timedelta(days=weekday)).strftime(fmt)
 
             return date_start
+        
+        else:
+            return ValueError("Unable to find start of the week for a date with such format.")
     
     elif isinstance(date, (pd._libs.tslibs.timestamps.Timestamp, datetime)):
 
         converted_date = date_convert(date, 'str', '%Y-%m-%d')
 
         return week_start(converted_date)
     
     else:
         raise ValueError("Unknow data type of date variable")
     
     
-def week_end(date: Union[str, datetime, pd._libs.tslibs.timestamps.Timestamp], weekend:bool) -> str:
+def week_end(date: Union[str, datetime, pd._libs.tslibs.timestamps.Timestamp], weekend: bool) -> str:
 
     """
     Find the end of the specific week based on a given date for either week as a whole or business week
 
     :param date: The date given by a user to identify end of the week that the date is in 
     :type date: str, datetime, pd._libs.tslibs.timestamps.Timestamp
 
@@ -187,15 +193,15 @@
     :type weekend: bool
 
     :return: Date representing end of the full or business week
     :rtype: str
     """
 
 
-    if isinstance(date, str):
+    if isinstance(date, str) and isinstance(weekend, bool):
 
         fmt = identify_date_format(date)
 
         if fmt:
 
             weekday = datetime.strptime(date, fmt).weekday()
 
@@ -225,26 +231,26 @@
 
                     return('Today is the end of the full week.')
                 
         else:
 
             raise ValueError("Couldn't process such date format.")
     
-    elif isinstance(date, (pd._libs.tslibs.timestamps.Timestamp, datetime)):
+    elif isinstance(date, (pd._libs.tslibs.timestamps.Timestamp, datetime)) and isinstance(weekend, bool):
 
         converted_date = date_convert(date, 'str', '%Y-%m-%d')
 
         return week_end(converted_date, weekend)
     
     else:
 
-        raise ValueError("Unknow data type of date variable")
+        raise ValueError("Unknow data type of input variable")
 
 
-def date_operations(date: Union[str, datetime, pd._libs.tslibs.timestamps.Timestamp], operation:str, frequency:str, range:int, weekend:bool) -> str:
+def date_operations(date: Union[str, datetime, pd._libs.tslibs.timestamps.Timestamp], operation: str, frequency: str, range: int, weekend: bool) -> str:
 
     """
     Adding or subtracting date for chosen frequency in specific range for either standard or business week
 
     :param date: date from which subtraction or addition will be calculated
     :type date: str, datetime, pd._libs.tslibs.timestamps.Timestamp
 
@@ -261,15 +267,17 @@
     :type weekend: bool
 
     :return: New day after subtraction or addition
     :rtype: str
     """
 
 
-    if date and operation and frequency and range:
+    global operations 
+
+    if operation in operations and isinstance(frequency, str) and isinstance(range, int) and isinstance(weekend, bool) and isinstance(date, (str, pd._libs.tslibs.timestamps.Timestamp, datetime)): 
 
         if isinstance(date, str):
 
             fmt = identify_date_format(date)
 
             weekday = datetime.strptime(date, fmt).weekday()
 
@@ -380,28 +388,32 @@
                 elif operation == '-':
 
                     year -= range
                     
                     date = datetime(year=year, month=month, day=day)
 
                     return(f'Subtracted date: {date.strftime(fmt)}')  
+                
+            else:
+                raise ValueError('No such frequency')
 
         elif isinstance(date, (pd._libs.tslibs.timestamps.Timestamp, datetime)):
 
             converted_date = date_convert(date, 'str', '%Y-%m-%d')
 
             return date_operations(converted_date, operation, frequency, range, weekend)
         
         else:
-            raise ValueError("Unknow data type of date variable")   
-    else: 
-        raise ValueError('Missing mandatory variable.')               
+            raise ValueError("Unknow data type of date variable") 
 
+    else:
+        raise ValueError('Incorrect data type or value in an input parameter')  
+             
 
-def range_calculation(start: Union[str, datetime, pd._libs.tslibs.timestamps.Timestamp], end: Union[str, datetime, pd._libs.tslibs.timestamps.Timestamp], weekend:bool, frequency:str) -> list:
+def range_calculation(start: Union[str, datetime, pd._libs.tslibs.timestamps.Timestamp], end: Union[str, datetime, pd._libs.tslibs.timestamps.Timestamp], weekend: bool, frequency: str) -> list:
 
     """
     Calculate range between two dates for standard or business week in different frquencies
     
     :param start: start of the period
     :type start: str, datetime, pd._libs.tslibs.timestamps.Timestamp
 
@@ -415,30 +427,30 @@
     :type frequency: str
 
     :return: Range of days/months/year between two given dates
     :rtype: list
     """
 
 
-    if start and end and frequency and range: 
-
+    if isinstance(start, (str, pd._libs.tslibs.timestamps.Timestamp, datetime)) and isinstance(end, (str, pd._libs.tslibs.timestamps.Timestamp, datetime)) and isinstance(weekend, bool) and isinstance(frequency, str):
+        
         if isinstance(start, str) and isinstance(end, str): 
 
             if date_comparison(end, start, '>'):
                 max_date = end
                 min_date = start
             else:
                 max_date = start
                 min_date = end
 
             max_format = identify_date_format(start)
-            max_date = datetime.strptime(end, max_format)
+            max_date = datetime.strptime(max_date, max_format)
 
             min_format = identify_date_format(end)
-            min_date = datetime.strptime(start, min_format)
+            min_date = datetime.strptime(min_date, min_format)
 
             days_between = []
 
             if weekend:
 
                 while max_date != min_date + timedelta(days=1):
 
@@ -509,14 +521,17 @@
 
                 if type(year_difference) != int:
 
                     years = int(year_difference)
                     days = len(days_between) % 365
 
                 return f"Difference between two dates is {years} year(s) and {days} days. If you want to see specific dates, switch to format='day'"
+            
+            else:
+                raise ValueError('No such frequency')
         
         elif isinstance(start, (pd._libs.tslibs.timestamps.Timestamp, datetime)) or isinstance(end, (pd._libs.tslibs.timestamps.Timestamp, datetime)):
 
             start_type = type(start)
             end_type = type(end)
 
             if start_type != str and end_type != str:
@@ -533,20 +548,20 @@
                 end = date_convert(end, 'str', '%Y-%m-%d')
 
             return range_calculation(start, end, weekend, frequency)
         
         else:
             
             raise ValueError( "Unknow data type of date variable")  
+        
     else:
-
-        raise ValueError('Missing mandatory variable')
+        raise ValueError('Incorrect data type or value in an input parameter')
 
 
-def date_convert(date: Union[str, datetime, pd._libs.tslibs.timestamps.Timestamp], desired_type:str, format:str):
+def date_convert(date: Union[str, datetime, pd._libs.tslibs.timestamps.Timestamp], desired_type: str, format: str):
 
     """
     Date conversion based on specified format according do tright party library options
 
     :param date: date for conversion 
     :type date: str, datetime, pd._libs.tslibs.timestamps.Timestamp
 
@@ -557,34 +572,40 @@
     :type format: str
 
     :return: Converted date
     :rtype: str, datetime, pd._libs.tslibs.timestamps.Timestamp
     """
     
 
-    date_type = str(type(date)).split("'")[1]
+    if isinstance(date, (str, pd._libs.tslibs.timestamps.Timestamp, datetime)) and isinstance(desired_type, (str)) and isinstance(format, (str)):
+        date_type = str(type(date)).split("'")[1]
 
-    conversions = {
-        'pandas._libs.tslibs.timestamps.Timestamp'  : 'pandas', 
-        'datetime.datetime'                         : 'datetime', 
-        'str'                                       : 'str'
-    }
-
-    desired_result = conversions[date_type] + '-' + desired_type
-
-    conversions = {
-        'str-pandas'                 : pd.to_datetime(date) if isinstance(date, str) else None, 
-        'str-datetime'               : datetime.strptime(date, format) if isinstance(date, str) else None,
-        'pandas-str'                 : date.strftime(format) if isinstance(date, pd._libs.tslibs.timestamps.Timestamp) else None,
-        'pandas-datetime'            : date.to_pydatetime(date) if isinstance(date, pd._libs.tslibs.timestamps.Timestamp) else None,
-        'datetime-str'               : date.strftime(format) if isinstance(date, datetime) else None,
-        'datetime-pandas'            : pd.Timestamp(date) if isinstance(date, datetime) else None
-    }
+        conversions = {
+            'pandas._libs.tslibs.timestamps.Timestamp'  : 'pandas', 
+            'datetime.datetime'                         : 'datetime', 
+            'str'                                       : 'str'
+        }
 
-    if date_type == desired_type:
-        return 'Your date is in desired format'
-    
-    elif isinstance(date, (pd._libs.tslibs.timestamps.Timestamp, datetime, str)):
-        return conversions[desired_result]
-    
+        desired_result = conversions[date_type] + '-' + desired_type
+
+        if date_type == desired_type:
+            return ValueError('Your date is in desired format')
+        
+        elif isinstance(date, (pd._libs.tslibs.timestamps.Timestamp, datetime, str)):
+
+            try:
+                conversions = {
+                'str-pandas'                 : pd.to_datetime(date) if isinstance(date, str) else None, 
+                'str-datetime'               : datetime.strptime(date, format) if isinstance(date, str) else None,
+                'pandas-str'                 : date.strftime(format) if isinstance(date, pd._libs.tslibs.timestamps.Timestamp) else None,
+                'pandas-datetime'            : date.to_pydatetime(date) if isinstance(date, pd._libs.tslibs.timestamps.Timestamp) else None,
+                'datetime-str'               : date.strftime(format) if isinstance(date, datetime) else None,
+                'datetime-pandas'            : pd.Timestamp(date) if isinstance(date, datetime) else None
+                }
+
+                return conversions[desired_result]
+            except:
+                raise ValueError("Unable to complete such request") 
+        
     else:
-        raise ValueError("Unknow data type of date variable")  
+        raise ValueError("Unknow data type of input variable")  
+
```

### Comparing `datewise-0.1.6/datewise.egg-info/PKG-INFO` & `datewise-0.2.0/datewise.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datewise
-Version: 0.1.6
+Version: 0.2.0
 Summary: Thesis Library
 Home-page: https://datewise.readthedocs.io/
 Author: Sebastian Gontkovic
 Author-email: sebascngont@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `datewise-0.1.6/setup.py` & `datewise-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="datewise",
-    version="0.1.6",
+    version="0.2.0",
     description="Thesis Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://datewise.readthedocs.io/",
     author="Sebastian Gontkovic",
     author_email="sebascngont@gmail.com",
     license="MIT",
```

### Comparing `datewise-0.1.6/tests/test_functionality.py` & `datewise-0.2.0/tests/test_functionality.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,25 @@
 
     date1 = '2024-03-17'
     date2 = (datetime.now() - timedelta(days=1))
 
     assert date_comparison(date_1=date1, date_2=date2, operation='<') == True
 
 
+def test_7_date_comparison_different_data_types_missing_variable():
+
+    date1 = '2024-03-17'
+    date2 = (datetime.now() - timedelta(days=1))
+
+    with pytest.raises(TypeError) as exc_info:
+        date_comparison(date_1=date1, date_2=date2)
+
+    assert str(exc_info.value) == "date_comparison() missing 1 required positional argument: 'operation'"
+
+
 # week_start
 
 def test1_week_start_date_as_string():
 
     date = '2024-03-19'
 
     assert week_start(date) == '2024-03-18'
@@ -199,14 +210,24 @@
 
     with pytest.raises(ValueError) as exc_info:
         week_end(date, True)
 
     assert str(exc_info.value) == "Couldn't process such date format."
 
 
+def test10_week_end_date_as_string_weekend_true_date_unknown_data_type():
+
+    date = 123
+
+    with pytest.raises(ValueError) as exc_info:
+        week_end(date, True)
+
+    assert str(exc_info.value) == "Unknow data type of input variable"
+
+
 # date_operations
     
 def test1_date_operations_date_string_operation_addition_frequency_day_weekend_false():
 
     date = '2024-03-19'
     range = 5
 
@@ -488,14 +509,24 @@
 def test36_date_operations_date_datetime_operation_addition_frequency_year_weekend_true():
 
     date = datetime(year=2024, month=3, day=19)
     range = 3
 
     assert date_operations(date=date, operation='-', frequency='year', range=range, weekend=True) == 'Subtracted date: 2021-03-19'
 
+def test37_date_operations_date_datetime_operation_incorrect_frequency_year_weekend_true():
+
+    date = datetime(year=2024, month=3, day=19)
+    range = 3
+
+    with pytest.raises(ValueError) as exc_info:
+        date_operations(date=date, operation='>', frequency='year', range=range, weekend=True)
+
+    assert str(exc_info.value) == "Incorrect data type or value in an input parameter"
+
 
 # range_calculation
     
 def test1_date1_string_date2_string_range_calculation_weekend_false_frequncy_day():
 
     start = '2024-03-19'
     end = '2024-04-02'
@@ -731,14 +762,36 @@
 
     start = pd.Timestamp('2024-03-19 12:30:00')
     end = datetime(year=2024, month=4, day=2)
 
     assert range_calculation(start=start, end=end, weekend=True, frequency='year') == "Difference between two dates is 0 year(s) and 9 days. If you want to see specific dates, switch to format='day'"
 
 
+def test31_date1_timestamp_date2_datetime_range_calculation_weekend_true_frequncy_unknown():
+
+    start = pd.Timestamp('2024-03-19 12:30:00')
+    end = datetime(year=2024, month=4, day=2)
+
+    with pytest.raises(ValueError) as exc_info:
+        range_calculation(start=start, end=end, weekend=True, frequency='unknown')
+
+    assert str(exc_info.value) == "No such frequency"
+
+
+def test32_date1_incorrect_data_type_date2_datetime_range_calculation_weekend_true_frequncy_year():
+
+    start = 1
+    end = datetime(year=2024, month=4, day=2)
+
+    with pytest.raises(ValueError) as exc_info:
+        range_calculation(start=start, end=end, weekend=True, frequency='year')
+
+    assert str(exc_info.value) == "Incorrect data type or value in an input parameter"
+
+
 # date_convert
     
 def test1_date_convert_from_str_to_pandas():
 
     date = '2024-03-19'
 
     assert date_convert(date=date, desired_type='pandas', format='%Y-%m-%d') == pd.Timestamp('2024-03-19 00:00:00')
@@ -775,11 +828,18 @@
 def test6_date_convert_from_datetime_to_pandas():
 
     date = datetime(2024, 3, 19, 0, 0)
 
     assert date_convert(date=date, desired_type='pandas', format='%Y-%m-%d') == pd.Timestamp('2024-03-19 00:00:00')
 
 
+def test7_date_convert_from_datetime_to_not_available_format():
+
+    date = 1
+
+    with pytest.raises(ValueError) as exc_info:
+        date_convert(date=date, desired_type='numpy', format='%Y-%m-%d')
 
+    assert str(exc_info.value) == "Unknow data type of input variable"
```

