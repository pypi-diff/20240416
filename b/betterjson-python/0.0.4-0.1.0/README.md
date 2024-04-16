# Comparing `tmp/betterjson_python-0.0.4.tar.gz` & `tmp/betterjson-python-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betterjson_python-0.0.4.tar", last modified: Tue Apr 16 16:42:48 2024, max compression
+gzip compressed data, was "betterjson_python-0.1.0.tar", last modified: Tue Apr 16 17:24:10 2024, max compression
```

## Comparing `betterjson_python-0.0.4.tar` & `betterjson-python-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 16:42:48.881219 betterjson_python-0.0.4/
--rw-rw-rw-   0        0        0     2126 2024-04-16 16:42:48.880221 betterjson_python-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1859 2024-04-16 16:42:30.000000 betterjson_python-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 16:42:48.879224 betterjson_python-0.0.4/betterjson_python.egg-info/
--rw-rw-rw-   0        0        0     2126 2024-04-16 16:42:48.000000 betterjson_python-0.0.4/betterjson_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2024-04-16 16:42:48.000000 betterjson_python-0.0.4/betterjson_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 16:42:48.000000 betterjson_python-0.0.4/betterjson_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-16 16:42:48.000000 betterjson_python-0.0.4/betterjson_python.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-16 16:42:48.878226 betterjson_python-0.0.4/modules/
--rw-rw-rw-   0        0        0      923 2024-04-16 14:21:41.000000 betterjson_python-0.0.4/modules/files.py
--rw-rw-rw-   0        0        0     1732 2024-04-16 14:38:57.000000 betterjson_python-0.0.4/modules/format.py
--rw-rw-rw-   0        0        0     5002 2024-04-16 14:13:13.000000 betterjson_python-0.0.4/modules/parse.py
--rw-rw-rw-   0        0        0       42 2024-04-16 16:42:48.881219 betterjson_python-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      544 2024-04-16 16:42:02.000000 betterjson_python-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 17:24:10.969923 betterjson_python-0.1.0/
+-rw-rw-rw-   0        0        0     2288 2024-04-16 17:24:10.967929 betterjson_python-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1754 2024-04-16 17:12:38.000000 betterjson_python-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 17:24:10.949976 betterjson_python-0.1.0/betterjson/
+-rw-rw-rw-   0        0        0      605 2024-04-16 16:46:27.000000 betterjson_python-0.1.0/betterjson/__version__.py
+-rw-rw-rw-   0        0        0     3095 2024-04-16 16:37:05.000000 betterjson_python-0.1.0/betterjson/betterjson.py
+drwxrwxrwx   0        0        0        0 2024-04-16 17:24:10.952969 betterjson_python-0.1.0/betterjson/modules/
+-rw-rw-rw-   0        0        0      923 2024-04-16 14:21:41.000000 betterjson_python-0.1.0/betterjson/modules/files.py
+-rw-rw-rw-   0        0        0     1732 2024-04-16 14:38:57.000000 betterjson_python-0.1.0/betterjson/modules/format.py
+-rw-rw-rw-   0        0        0     5002 2024-04-16 14:13:13.000000 betterjson_python-0.1.0/betterjson/modules/parse.py
+drwxrwxrwx   0        0        0        0 2024-04-16 17:24:10.966931 betterjson_python-0.1.0/betterjson_python.egg-info/
+-rw-rw-rw-   0        0        0     2288 2024-04-16 17:24:10.000000 betterjson_python-0.1.0/betterjson_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2024-04-16 17:24:10.000000 betterjson_python-0.1.0/betterjson_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 17:24:10.000000 betterjson_python-0.1.0/betterjson_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-16 17:24:10.000000 betterjson_python-0.1.0/betterjson_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 17:24:10.969923 betterjson_python-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      808 2024-04-16 17:22:59.000000 betterjson_python-0.1.0/setup.py
```

### Comparing `betterjson_python-0.0.4/PKG-INFO` & `betterjson_python-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 Metadata-Version: 2.1
 Name: betterjson-python
-Version: 0.0.4
+Version: 0.1.0
 Summary: BetterJSON is an enhanced version of the JSON data format
-Author: ruxixa
-License: MIT
-Project-URL: Source, https://github.com/ruxixa/BetterJSON/
+Home-page: https://github.com/ruxixa/BetterJSON
+Author: Jan Kowalski
+Author-email: a@a.com
+Project-URL: Source, https://github.com/ruxixa/BetterJSON
+Project-URL: Bug Reports, https://github.com/ruxixa/BetterJSON/issues
+Keywords: kilka,słów,kluczowych,opisujących,Twoją,bibliotekę
+Classifier: Programming Language :: Python
+Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 
 # betterjson-python
 `betterjson-python` is a Python library implementing an extension to the JSON format with additional features such as adding comments and mathematical operations.
 
 ## Installation
 You can install the library via pip:
 
 ```bash
 pip install betterjson-python
 ```
 
 ## Usage
+### Python
 ```python
 import betterjson-python as bj
 
 # Example usage
 data = {
     "name": "John",
     "age": 30,
@@ -36,32 +42,35 @@
 print(loaded_data)
 
 # Formatting a dictionary as a JSON string
 formatted_json = bj.format(data)
 print(formatted_json)
 ```
 
+### C++
+(comming soon)
+
 ## Features
 - Comment Support: BetterJSON allows you to include comments in your JSON files, making them more readable
 - Mathematical Operations: You can perform mathematical operations directly json file
 
 ## Example
 ### Normal json
-```json
+```cpp
 {
     "name": "Alice",
     "age": 25, 
     "--comment": "this is a comment",
     "salary": 50000,
     "--comment": "we need to calculate json inside the program",
     "bonus": 0
 }
 ```
 ### BetterJSON
-```json
+```cpp
 {
     "name": "Alice",
     "age": 25, // this is a comment
     "salary": 50000,
     "bonus": 50000 * 0.1 // calculating bonus as 10% of salary 
 }
 ```
@@ -76,12 +85,9 @@
 # Print loaded data
 print(data)
 
 # Format loaded data as JSON string
 formatted_json = bj
 ```
 
-## Repository
-For issue tracking, feature requests, and contributions, visit our (Github Repository)[https://github.com/ruxixa/BetterJSON/]
-
 ## License
-This project is licensed under the MIT License - see the (LICENSE.md)[https://github.com/ruxixa/BetterJSON/blob/main/LICENSE] file for details.
+This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/ruxixa/BetterJSON/blob/main/LICENSE) file for details.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `betterjson_python-0.0.4/README.md` & `betterjson_python-0.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 You can install the library via pip:
 
 ```bash
 pip install betterjson-python
 ```
 
 ## Usage
+### Python
 ```python
 import betterjson-python as bj
 
 # Example usage
 data = {
     "name": "John",
     "age": 30,
@@ -27,32 +28,35 @@
 print(loaded_data)
 
 # Formatting a dictionary as a JSON string
 formatted_json = bj.format(data)
 print(formatted_json)
 ```
 
+### C++
+(comming soon)
+
 ## Features
 - Comment Support: BetterJSON allows you to include comments in your JSON files, making them more readable
 - Mathematical Operations: You can perform mathematical operations directly json file
 
 ## Example
 ### Normal json
-```json
+```cpp
 {
     "name": "Alice",
     "age": 25, 
     "--comment": "this is a comment",
     "salary": 50000,
     "--comment": "we need to calculate json inside the program",
     "bonus": 0
 }
 ```
 ### BetterJSON
-```json
+```cpp
 {
     "name": "Alice",
     "age": 25, // this is a comment
     "salary": 50000,
     "bonus": 50000 * 0.1 // calculating bonus as 10% of salary 
 }
 ```
@@ -67,12 +71,9 @@
 # Print loaded data
 print(data)
 
 # Format loaded data as JSON string
 formatted_json = bj
 ```
 
-## Repository
-For issue tracking, feature requests, and contributions, visit our (Github Repository)[https://github.com/ruxixa/BetterJSON/]
-
 ## License
-This project is licensed under the MIT License - see the (LICENSE.md)[https://github.com/ruxixa/BetterJSON/blob/main/LICENSE] file for details.
+This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/ruxixa/BetterJSON/blob/main/LICENSE) file for details.
```

### Comparing `betterjson_python-0.0.4/betterjson_python.egg-info/PKG-INFO` & `betterjson_python-0.1.0/betterjson_python.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 Metadata-Version: 2.1
 Name: betterjson-python
-Version: 0.0.4
+Version: 0.1.0
 Summary: BetterJSON is an enhanced version of the JSON data format
-Author: ruxixa
-License: MIT
-Project-URL: Source, https://github.com/ruxixa/BetterJSON/
+Home-page: https://github.com/ruxixa/BetterJSON
+Author: Jan Kowalski
+Author-email: a@a.com
+Project-URL: Source, https://github.com/ruxixa/BetterJSON
+Project-URL: Bug Reports, https://github.com/ruxixa/BetterJSON/issues
+Keywords: kilka,słów,kluczowych,opisujących,Twoją,bibliotekę
+Classifier: Programming Language :: Python
+Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 
 # betterjson-python
 `betterjson-python` is a Python library implementing an extension to the JSON format with additional features such as adding comments and mathematical operations.
 
 ## Installation
 You can install the library via pip:
 
 ```bash
 pip install betterjson-python
 ```
 
 ## Usage
+### Python
 ```python
 import betterjson-python as bj
 
 # Example usage
 data = {
     "name": "John",
     "age": 30,
@@ -36,32 +42,35 @@
 print(loaded_data)
 
 # Formatting a dictionary as a JSON string
 formatted_json = bj.format(data)
 print(formatted_json)
 ```
 
+### C++
+(comming soon)
+
 ## Features
 - Comment Support: BetterJSON allows you to include comments in your JSON files, making them more readable
 - Mathematical Operations: You can perform mathematical operations directly json file
 
 ## Example
 ### Normal json
-```json
+```cpp
 {
     "name": "Alice",
     "age": 25, 
     "--comment": "this is a comment",
     "salary": 50000,
     "--comment": "we need to calculate json inside the program",
     "bonus": 0
 }
 ```
 ### BetterJSON
-```json
+```cpp
 {
     "name": "Alice",
     "age": 25, // this is a comment
     "salary": 50000,
     "bonus": 50000 * 0.1 // calculating bonus as 10% of salary 
 }
 ```
@@ -76,12 +85,9 @@
 # Print loaded data
 print(data)
 
 # Format loaded data as JSON string
 formatted_json = bj
 ```
 
-## Repository
-For issue tracking, feature requests, and contributions, visit our (Github Repository)[https://github.com/ruxixa/BetterJSON/]
-
 ## License
-This project is licensed under the MIT License - see the (LICENSE.md)[https://github.com/ruxixa/BetterJSON/blob/main/LICENSE] file for details.
+This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/ruxixa/BetterJSON/blob/main/LICENSE) file for details.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `betterjson_python-0.0.4/modules/files.py` & `betterjson_python-0.1.0/betterjson/modules/files.py`

 * *Files identical despite different names*

### Comparing `betterjson_python-0.0.4/modules/format.py` & `betterjson_python-0.1.0/betterjson/modules/format.py`

 * *Files identical despite different names*

### Comparing `betterjson_python-0.0.4/modules/parse.py` & `betterjson_python-0.1.0/betterjson/modules/parse.py`

 * *Files identical despite different names*

