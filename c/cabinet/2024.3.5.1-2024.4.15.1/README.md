# Comparing `tmp/cabinet-2024.3.5.1.tar.gz` & `tmp/cabinet-2024.4.15.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cabinet-2024.3.5.1.tar", last modified: Wed Mar  6 03:20:43 2024, max compression
+gzip compressed data, was "cabinet-2024.4.15.1.tar", last modified: Tue Apr 16 00:28:01 2024, max compression
```

## Comparing `cabinet-2024.3.5.1.tar` & `cabinet-2024.4.15.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-03-06 03:20:43.912523 cabinet-2024.3.5.1/
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1090 2024-01-29 08:09:41.000000 cabinet-2024.3.5.1/LICENSE
--rw-r--r--   0 tyler     (1000) tyler     (1000)     7942 2024-03-06 03:20:43.912523 cabinet-2024.3.5.1/PKG-INFO
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     7591 2024-01-29 08:09:41.000000 cabinet-2024.3.5.1/README.md
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)       98 2024-01-29 08:09:41.000000 cabinet-2024.3.5.1/pyproject.toml
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)      750 2024-03-06 03:20:43.912523 cabinet-2024.3.5.1/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-03-06 03:20:43.908523 cabinet-2024.3.5.1/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-03-06 03:20:43.912523 cabinet-2024.3.5.1/src/cabinet/
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)       80 2024-01-29 08:09:41.000000 cabinet-2024.3.5.1/src/cabinet/__init__.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)       69 2024-01-29 08:09:41.000000 cabinet-2024.3.5.1/src/cabinet/__main__.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)    35482 2024-03-06 03:19:51.000000 cabinet-2024.3.5.1/src/cabinet/cabinet.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     2598 2024-01-29 08:09:41.000000 cabinet-2024.3.5.1/src/cabinet/constants.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     3687 2024-01-29 08:09:41.000000 cabinet-2024.3.5.1/src/cabinet/mail.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-03-06 03:20:43.912523 cabinet-2024.3.5.1/src/cabinet.egg-info/
--rw-r--r--   0 tyler     (1000) tyler     (1000)     7942 2024-03-06 03:20:43.000000 cabinet-2024.3.5.1/src/cabinet.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      358 2024-03-06 03:20:43.000000 cabinet-2024.3.5.1/src/cabinet.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2024-03-06 03:20:43.000000 cabinet-2024.3.5.1/src/cabinet.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2024-03-06 03:20:43.000000 cabinet-2024.3.5.1/src/cabinet.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2024-03-06 03:20:43.000000 cabinet-2024.3.5.1/src/cabinet.egg-info/top_level.txt
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-03-06 03:20:43.912523 cabinet-2024.3.5.1/test/
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1730 2024-01-29 08:09:41.000000 cabinet-2024.3.5.1/test/test___init__.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-16 00:28:01.044599 cabinet-2024.4.15.1/
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1090 2024-01-29 08:09:41.000000 cabinet-2024.4.15.1/LICENSE
+-rw-r--r--   0 tyler     (1000) tyler     (1000)     7946 2024-04-16 00:28:01.044599 cabinet-2024.4.15.1/PKG-INFO
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     7594 2024-03-25 03:38:11.000000 cabinet-2024.4.15.1/README.md
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)       98 2024-01-29 08:09:41.000000 cabinet-2024.4.15.1/pyproject.toml
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)      750 2024-04-16 00:28:01.044599 cabinet-2024.4.15.1/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-16 00:28:01.040599 cabinet-2024.4.15.1/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-16 00:28:01.044599 cabinet-2024.4.15.1/src/cabinet/
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)       80 2024-01-29 08:09:41.000000 cabinet-2024.4.15.1/src/cabinet/__init__.py
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)       69 2024-01-29 08:09:41.000000 cabinet-2024.4.15.1/src/cabinet/__main__.py
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)    37122 2024-04-16 00:09:36.000000 cabinet-2024.4.15.1/src/cabinet/cabinet.py
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     2596 2024-03-25 04:02:52.000000 cabinet-2024.4.15.1/src/cabinet/constants.py
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     4413 2024-04-16 00:26:57.000000 cabinet-2024.4.15.1/src/cabinet/mail.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-16 00:28:01.044599 cabinet-2024.4.15.1/src/cabinet.egg-info/
+-rw-r--r--   0 tyler     (1000) tyler     (1000)     7946 2024-04-16 00:28:01.000000 cabinet-2024.4.15.1/src/cabinet.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      358 2024-04-16 00:28:01.000000 cabinet-2024.4.15.1/src/cabinet.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2024-04-16 00:28:01.000000 cabinet-2024.4.15.1/src/cabinet.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2024-04-16 00:28:01.000000 cabinet-2024.4.15.1/src/cabinet.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2024-04-16 00:28:01.000000 cabinet-2024.4.15.1/src/cabinet.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-16 00:28:01.044599 cabinet-2024.4.15.1/test/
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1730 2024-01-29 08:09:41.000000 cabinet-2024.4.15.1/test/test___init__.py
```

### Comparing `cabinet-2024.3.5.1/LICENSE` & `cabinet-2024.4.15.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cabinet-2024.3.5.1/PKG-INFO` & `cabinet-2024.4.15.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2024.3.5.1
+Version: 2024.4.15.1
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -278,27 +278,24 @@
 python:
 ```
 from cabinet import Cabinet
 
 cab = Cabinet()
 
 # writes to a file named LOG_DAILY_YYYY-MM-DD in the default log folder (or cab.get('path', 'log')) inside a YYYY-MM-DD folder
-
 cab.log("Connection timed out") # defaults to 'info' if no level is set
 cab.log("This function hit a breakpoint", level="debug")
 cab.log("Looks like the server is on fire", level="critical")
 cab.log("This is fine", level="info")
 
 # writes to a file named LOG_TEMPERATURE
-
 cab.log("30", log_name="LOG_TEMPERATURE")
 
 # writes to a file named LOG_TEMPERATURE in /home/{username}/weather
-
-cab.log("30", log_name="LOG_TEMPERATURE", file_path="/home/{username}/weather")
+cab.log("30", log_name="LOG_TEMPERATURE", log_folder_path="/home/{username}/weather")
 
     # format
     # 2021-12-29 19:29:27,896 — INFO — 30
 
 ```
 
 terminal:
```

### Comparing `cabinet-2024.3.5.1/README.md` & `cabinet-2024.4.15.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -266,27 +266,24 @@
 python:
 ```
 from cabinet import Cabinet
 
 cab = Cabinet()
 
 # writes to a file named LOG_DAILY_YYYY-MM-DD in the default log folder (or cab.get('path', 'log')) inside a YYYY-MM-DD folder
-
 cab.log("Connection timed out") # defaults to 'info' if no level is set
 cab.log("This function hit a breakpoint", level="debug")
 cab.log("Looks like the server is on fire", level="critical")
 cab.log("This is fine", level="info")
 
 # writes to a file named LOG_TEMPERATURE
-
 cab.log("30", log_name="LOG_TEMPERATURE")
 
 # writes to a file named LOG_TEMPERATURE in /home/{username}/weather
-
-cab.log("30", log_name="LOG_TEMPERATURE", file_path="/home/{username}/weather")
+cab.log("30", log_name="LOG_TEMPERATURE", log_folder_path="/home/{username}/weather")
 
     # format
     # 2021-12-29 19:29:27,896 — INFO — 30
 
 ```
 
 terminal:
```

### Comparing `cabinet-2024.3.5.1/src/cabinet/cabinet.py` & `cabinet-2024.4.15.1/src/cabinet/cabinet.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,21 +51,22 @@
     """
 
     mongodb_username: str = ''
     mongodb_password: str = ''
     mongodb_cluster_name: str = ''
     mongodb_db_name: str = ''
     mongodb_uri = ""
-    client: MongoClient = None
+    client: MongoClient | None = None
     database = None
     new_setup: bool = False
-    path_config_file = str(pathlib.Path(
-        __file__).resolve().parent / "cabinet_config.json")
-    path_cabinet: str = None
-    path_log: str = None
+    path_config_dir = str(pathlib.Path(
+        __file__).resolve().parent)
+    path_config_file = f"{path_config_dir}/cabinet_config.json"
+    path_cabinet: str | None = None
+    path_log: str | None = None
 
     def _get_config(self, key=None):
         """
         Retrieves the value associated with the specified key from the configuration file.
 
         Args:
             key (str): The key to retrieve the corresponding value.
@@ -153,15 +154,15 @@
                     file.write('{}')
                 print("Done. Please try again.")
             else:
                 print(f"OK. Please fix {self.path_config_file} and try again.")
 
             sys.exit(-1)
 
-    def _put_config(self, key: str = None, value: str = None):
+    def _put_config(self, key: str | None = None, value: str | None = None) -> str | None:
         """
         Updates the internal configuration file with a new key-value pair.
 
         Args:
             key (str): The key for the configuration setting.
             value (str): The value for the configuration setting.
 
@@ -210,28 +211,29 @@
         except TypeError:
             if is_print:
                 print(json.dumps(message, indent=2))
         except json.JSONDecodeError:
             if is_print:
                 print(message)
             return message
-        
+
     def _expand_aliases(self, string):
         """
         Expands environment variables and user aliases in a string.
 
         Args:
             - string (str): the string to expand
 
         Returns:
             - The expanded string.
         """
-        return string.replace("$HOME", os.environ.get("HOME", "")).replace("~", os.environ.get("HOME", ""))
+        return string.replace("$HOME", os.environ.get("HOME",
+            "")).replace("~", os.environ.get("HOME", ""))
 
-    def __init__(self, path_cabinet: str = None):
+    def __init__(self, path_cabinet: str | None = None):
         """
         Initializes the Cabinet instance with the provided or default configuration.
 
         Args:
             path_cabinet (str, optional): The path to the cabinet directory. Defaults to None.
 
         Notes:
@@ -347,51 +349,57 @@
                 # macOS
                 subprocess.run(['open', self.path_config_file], check=True)
             elif sys.platform.startswith('linux'):
                 # Linux
                 subprocess.run(['xdg-open', self.path_config_file], check=True)
             else:
                 print(f"Please edit ${self.path_config_file} to configure.")
-                
-    def update_cache(self):
-        """
-        Writes all MongoDB data to a cache file for faster reads in most situations
+
+    def update_cache(self, path: str | None = None) -> str | None:
         """
+        Writes all MongoDB data to a cache file for faster reads in most situations.
+        Creates the cache file if it does not exist.
         
+        Args:
+            - path (str): full path, including filename, of cache.json
+        """
+
+        if path is None:
+            path = f"{self.path_config_dir}/cache.json"
+
         collection_data = self.database.cabinet.find()
         json_data = json.dumps(list(collection_data), indent=4, default=json_util.default)
 
-        temp_file_path = "cache.json"
-        
         try:
-            # Write the JSON data to cache
-            with open(temp_file_path, "w", encoding="utf-8") as temp_file:
+            # Ensure the directory exists and write the JSON data to cache
+            os.makedirs(os.path.dirname(path), exist_ok=True)
+            with open(path, "w", encoding="utf-8") as temp_file:
                 temp_file.write(json_data)
-        except Exception as e:
+        except OSError as e:
             self.log(f"Error updating cache: {e}", level="error")
-            return None  # Or handle the error as appropriate
+            return None
 
         return json_data
 
     def edit_db(self):
         """
         Opens the data in self.database.cabinet within a JSON file in Vim.
         When the file is closed, it replaces the data in this collection in MongoDB.
         """
-        
-        json_data = self.update_cache()
-        path_cache = "cache.json"
+
+        path_cache_file = f"{self.path_config_dir}/cache.json"
+        json_data = self.update_cache(path_cache_file)
 
         try:
 
             # Open the cache file in Vim
-            subprocess.run(["vim", path_cache], check=True)
+            subprocess.run(["vim", path_cache_file], check=True)
 
             # Read the modified JSON data from the cache
-            with open(path_cache, "r", encoding="utf-8") as file_cache:
+            with open(path_cache_file, "r", encoding="utf-8") as file_cache:
                 modified_json_data = file_cache.read()
 
             # Check if any changes were made
             if modified_json_data == json_data:
                 print("No changes.")
                 return
 
@@ -404,23 +412,25 @@
             self.database.cabinet.drop()  # Drop the existing collection
             self.database.cabinet.insert_many(
                 modified_data)  # Insert the modified data
 
             print("Data in the collection has been updated.")
 
         except FileNotFoundError:
-            print("Error: Temporary file not found.")
+            print("Error: Cache file not found.")
         except subprocess.CalledProcessError:
             print("Error: Failed to open the file in Vim.")
         except json.JSONDecodeError:
-            print("Error: Failed to parse the modified JSON data.")
+            self.log("Failed to parse the modified JSON data.", level="error")
+            self.log("Refreshing cache with original data.", level="info")
+            self.write_file('cache.json', self.path_config_dir, json_data)
         except Exception as error:  # pylint: disable=W0703
             print(f"Error: {str(error)}")
 
-    def edit_file(self, file_path: str = None, create_if_not_exist: bool = True) -> None:
+    def edit_file(self, file_path: str | None = None, create_if_not_exist: bool = True) -> None:
         """
         Edit and save a file in Vim.
 
         Args:
             - file_path (str, optional): The path to the file to edit.
                 Allows for shortcuts by setting paths in MongoDB -> path -> edit
 
@@ -454,14 +464,18 @@
             item = self.get("path", "edit", file_path)
             if not isinstance(item, dict) or "value" not in item.keys():
                 self.log(f"Could not use shortcut for {file_path} \
                     in getItem(path -> edit); should be a JSON object with value", level="warn")
             else:
                 file_path = item["value"]
 
+        if not file_path:
+            print("Error: No file_path")
+            return
+
         if not os.path.exists(file_path):
             if create_if_not_exist:
                 with open(file_path, "w", encoding="utf-8"):
                     pass
             else:
                 self.log("Could not find file to edit", level="error")
                 raise FileNotFoundError(f"File does not exist: {file_path}")
@@ -571,44 +585,56 @@
         using a cache file to improve performance.
 
         Args:
             - *attributes (str): a sequence of strings representing nested attributes
             - warn_missing (bool, optional): whether to warn if an attribute is missing
             - is_print (bool, optional): whether to print the return value
             - no_cache (bool, optional): whether to force a fresh MongoDB call
-                - by default, if cache is over 1 hour old, update will be called and cache will be updated
+                - by default, if cache is over 1 hour old,
+                    update will be called and cache will be updated
 
         Returns:
             - The value of the attribute if it exists in the cache or MongoDB, otherwise None.
 
         Usage:
             - get('person', 'tyler', 'salary') returns the value of person -> tyler -> salary
         """
 
-        cache_file_path = "cache.json"
+        path_cache_file = f"{self.path_config_dir}/cache.json"
         cache_update_needed = no_cache
 
         # Check if cache file exists and is less than 1 hour old
-        if os.path.exists(cache_file_path):
-            last_modified = os.path.getmtime(cache_file_path)
-            if (time.time() - last_modified) / 3600 > 1:  # Cache older than 1 hour
+        if os.path.exists(path_cache_file):
+            last_modified = os.path.getmtime(path_cache_file)
+            if (time.time() - last_modified) / 3600 > 1:
                 cache_update_needed = True
         else:
             cache_update_needed = True
 
         if cache_update_needed:
             self.update_cache()  # Update the cache file
 
         # Read from cache
         try:
-            with open(cache_file_path, "r", encoding="utf-8") as file:
+            with open(path_cache_file, "r", encoding="utf-8") as file:
                 cached_data = json.load(file)
         except FileNotFoundError:
-            self.log("Cache file not found", level="warn")
+            self.log(f"Cache file not found at {path_cache_file}", level="warn")
             return None
+        except json.decoder.JSONDecodeError:
+            self.log(f"Could not read Cabinet cache at {path_cache_file}. Clearing.",
+                     level="warn")
+            try:
+                os.remove(path_cache_file)
+                print(f"File removed successfully: {path_cache_file}")
+                print("Please retry your last command.")
+                sys.exit(0)
+            except PermissionError:
+                self.log(f"Permission denied: Unable to delete the file at {path_cache_file}",
+                         level="critical")
 
         # Process the cached data
         for document in cached_data:
             result = document
             for attribute in attributes:
                 if isinstance(result, dict) and attribute in result:
                     result = result[attribute]
@@ -654,86 +680,93 @@
 
         result = self.database.cabinet.update_many(custom_filter, update)
 
         if is_print:
             print(f"Modified {result.modified_count} item(s)")
             print(f"{' -> '.join(attribute)} removed\n")
 
-    def log(self, message: str = '', log_name: str = None, level: str = None,
-            file_path: str = None, is_quiet: bool = False) -> None:
+    def log(self, message: str = '', log_name: str | None = None, level: str | None = None,
+            log_folder_path: str | None = None, is_quiet: bool = False) -> None:
         """
         Logs a message using the specified log level
         and writes it to a file if a file path is provided.
 
         Args:
             message (str, optional): The message to log. Defaults to ''.
             log_name (str, optional): The name of the logger to use. Defaults to None.
             level (str, optional): The log level to use.
                 Must be one of 'debug', 'info', 'warning', 'error', or 'critical'.
                 Defaults to 'info'.
-            file_path (str, optional): The path to the log file.
+            log_folder_path (str, optional): The path to the log file.
                 If not provided, logs will be saved to MongoDB -> path -> log.
                 Defaults to None.
             is_quiet (bool, optional): If True, logging output will be silenced. Defaults to False.
 
         Raises:
             ValueError: If an invalid log level is provided.
 
         Returns:
             None
         """
 
-        def _get_logger(log_name: str = None, level: int = logging.INFO,
-                        file_path: str = None, is_quiet: bool = False) -> logging.Logger:
+        def _get_logger(log_name: str | None = None,
+                        level: int = logging.INFO,
+                        log_folder_path: str | None = None,
+                        is_quiet: bool = False) -> logging.Logger:
             """
-            A helper function for log()
-
             Returns a customized logger object with the specified name and level,
             and optionally logs to a file.
 
             Args:
             - log_name (str): the name of the logger (defaults to 'root')
             - level (int): the logging level to use (defaults to logging.INFO)
-            - file_path (str): the path to a file to log to
+            - log_folder_path (str): the path to a file to log to
                 (defaults to None, meaning log only to console)
             - is_quiet (bool): if True, only logs to file and not to console (defaults to False)
 
             Returns:
             - logger (Logger): the configured logger object
             """
 
             today = str(date.today())
 
-            if file_path is None:
-                file_path = f"{self.path_log or self.path_cabinet + '/log/'}{today}"
+            if not self.path_cabinet:
+                raise ValueError("_get_logger: self.path_cabinet not available")
+
+            if log_folder_path is None:
+                log_folder_path = f"{self.path_log or self.path_cabinet + '/log/'}{today}"
+            else:
+                log_folder_path = os.path.expanduser(log_folder_path)
+
             if log_name is None:
                 log_name = f"LOG_DAILY_{today}"
 
             # create path if necessary
-            if not os.path.exists(file_path):
-                self._ifprint(f"Creating {file_path}", self.new_setup is True)
-                os.makedirs(file_path)
+            if not os.path.exists(log_folder_path):
+                self._ifprint(f"Creating {log_folder_path}", self.new_setup is True)
+                os.makedirs(log_folder_path)
 
             logger = logging.getLogger(log_name)
 
             logger.setLevel(level)
 
             if logger.handlers:
                 logger.handlers = []
 
             format_string = "%(asctime)s — %(levelname)s — %(message)s"
             log_format = logging.Formatter(format_string)
 
+            # only add console handler if not is_quiet
             if not is_quiet:
                 console_handler = logging.StreamHandler(sys.stdout)
                 console_handler.setFormatter(log_format)
                 logger.addHandler(console_handler)
 
             file_handler = logging.FileHandler(
-                f"{file_path}/{log_name}.log", mode='a')
+                os.path.join(log_folder_path, f"{log_name}.log"), mode='a')
             file_handler.setFormatter(log_format)
 
             logger.addHandler(file_handler)
             return logger
 
         if level is None:
             level = 'info'
@@ -743,28 +776,27 @@
                         'warning', 'error', 'critical'}
         if level.lower() not in valid_levels:
             raise ValueError(
                 f"Invalid log level: {level}. Must be one of {', '.join(valid_levels)}.")
 
         # get logger instance
         logger = _get_logger(log_name=log_name, level=level.upper(),
-                             file_path=file_path, is_quiet=is_quiet)
+                             log_folder_path=log_folder_path, is_quiet=is_quiet)
 
-        # Log message
-        if not is_quiet:
-            getattr(logger, level.lower())(message)
+        # log message
+        getattr(logger, level.lower())(message)
 
-    def get_file_as_array(self, item: str, file_path=None, strip: bool = True,
+    def get_file_as_array(self, file_name: str, file_path=None, strip: bool = True,
                           ignore_not_found: bool = False):
         """
         Reads a file and returns its contents as a list of lines.
         The file is assumed to be encoded in UTF-8.
 
         Args:
-            - item (str): The filename to read.
+            - file_name (str): The filename to read.
             - file_path (str, optional): The path to the directory containing the file.
                 If None, the default path is used.
             - strip (bool, optional): Whether to strip the lines of whitespace characters
                 On by default.
             - ignore_not_found (bool, optional): Whether to return None when the file is not found.
                 False by default.
 
@@ -777,15 +809,15 @@
         elif file_path == "notes":
             file_path = self.get('path', 'notes')
 
         if not file_path[-1] == '/':
             file_path += '/'
 
         try:
-            content = open(file_path + item, "r", encoding="utf8").read()
+            content = open(file_path + file_name, "r", encoding="utf8").read()
 
             if strip:
                 content = content.strip()
 
             return content.split('\n')
         except FileNotFoundError as error:
             if not ignore_not_found:
@@ -873,16 +905,16 @@
     class ValidatePutArgs(argparse.Action):
         """
         Custom argparse action to validate the number of arguments for the --put option.
         Ensures that a minimum of 2 arguments are provided.
         """
 
         def __call__(self, parser, namespace, values, option_string=None):
-            if len(values) < 2:
-                if len(values) == 1 and values[0] == 'ut':
+            if not values or len(values) < 2:
+                if values and len(values) == 1 and values[0] == 'ut':
                     print("I think you meant to use '--put' or '-p'.\n")
                 parser.error(
                     f"At least 2 arguments are required for {option_string}")
             setattr(namespace, self.dest, values)
 
     parser = argparse.ArgumentParser(
         description=f"Cabinet ({version})")
@@ -942,15 +974,15 @@
     elif args.put:
         attribute_values = args.put
         cab.put(*attribute_values, is_print=True)
     elif args.remove:
         attribute_values = args.remove
         cab.remove(*attribute_values, is_print=True)
     elif args.get_file:
-        cab.get_file_as_array(item=args.get_file,
+        cab.get_file_as_array(file_name=args.get_file,
                               file_path=None, strip=args.strip)
     elif args.log:
         cab.log(message=args.log, level=args.log_level)
     elif args.export:
         cab.export()
     elif args.mail:
         to_addr = None
```

### Comparing `cabinet-2024.3.5.1/src/cabinet/constants.py` & `cabinet-2024.4.15.1/src/cabinet/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,16 +48,16 @@
 Enter the full path where you would like to store Cabinet data,
 such as logs and settings.
 
 \n
 Default: {pathlib.Path.home().resolve()}/.cabinet
 """
 
-EDIT_FILE_DEFAULT = f"""
-"Enter the path of the file you want to edit.
+EDIT_FILE_DEFAULT = """
+Enter the path of the file you want to edit.
 (default: edit Cabinet's MongoDB collection):\n
 """
 
 ERROR_CONFIG_FILE_INVALID = """
 Cabinet could not initialize properly.
 
 Please check that all values in the configuration file are correct:
```

### Comparing `cabinet-2024.3.5.1/src/cabinet/mail.py` & `cabinet-2024.4.15.1/src/cabinet/mail.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 Provides functionality for sending email using SMTP and MIMEText.
 Does not support Gmail.
 
 A throwaway email is highly recommended.
 """
 
 import smtplib
-from typing import List
 from urllib.parse import unquote
 import sys
 import pwd
 import os
 from email.mime.text import MIMEText
 from email.mime.multipart import MIMEMultipart
 import cabinet
@@ -25,22 +24,29 @@
     """
 
     def __init__(self):
         self.user_dir = pwd.getpwuid(os.getuid())[0]
         self.cab = cabinet.Cabinet()
 
         # parameters
+        # port should be int; TODO update Cabinet to support type casting
         self.port = self.cab.get("email", "port")
-        self.smtp_server = self.cab.get("email", "smtp_server")
-        self.imap_server = self.cab.get("email", "imap_server")
+
+        self.smtp_server: str | None = self.cab.get("email", "smtp_server")
+        self.imap_server: str | None = self.cab.get("email", "imap_server")
         self.username = self.cab.get("email", "from")
         self.password = self.cab.get("email", "from_pw")
 
-    def send(self, subject: str, body: str, signature: str = '', to_addr: List[str] = None,
-             from_name: str = None, logging_enabled: bool = True, is_quiet: bool = False) -> None:
+    def send(self, subject: str,
+             body: str,
+             signature: str = '',
+             to_addr = None, # should be List[str]; TODO update Cabinet to support type casting
+             from_name: str | None = None,
+             logging_enabled: bool = True,
+             is_quiet: bool = False) -> None:
         """
         Sends an email with the given subject and body to the specified recipients.
 
         Args:
         - subject (str): The subject of the email.
         - body (str): The body of the email.
         - signature (str): The signature to include at the end of the email.
@@ -79,18 +85,34 @@
         # Create the message object.
         message = MIMEMultipart()
         message["Subject"] = unquote(subject)
         message["From"] = from_name
         message["To"] = (', ').join(to_addr)
         message.attach(MIMEText(unquote(body), "html"))
 
+        if not self.smtp_server:
+            self.cab.log("No SMTP Server set", level="error")
+            return
+
+        if not self.port:
+            self.cab.log("No port set", level="error")
+            return
+
+        if not isinstance(self.port, int):
+            self.cab.log(f"Port is not an integer (received '{self.port}')", level="error")
+            return
+
         # Send the email.
         server = smtplib.SMTP_SSL(self.smtp_server, self.port)
 
         try:
+
+            if not self.username or not self.password:
+                self.cab.log("Username/password not set", level="error")
+                return
             server.login(self.username, self.password)
 
             server.send_message(message)
 
             if logging_enabled:
                 self.cab.log(
                     f"Sent Email to {message['To']} as {message['From']}: {subject}",
```

### Comparing `cabinet-2024.3.5.1/src/cabinet.egg-info/PKG-INFO` & `cabinet-2024.4.15.1/src/cabinet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2024.3.5.1
+Version: 2024.4.15.1
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -278,27 +278,24 @@
 python:
 ```
 from cabinet import Cabinet
 
 cab = Cabinet()
 
 # writes to a file named LOG_DAILY_YYYY-MM-DD in the default log folder (or cab.get('path', 'log')) inside a YYYY-MM-DD folder
-
 cab.log("Connection timed out") # defaults to 'info' if no level is set
 cab.log("This function hit a breakpoint", level="debug")
 cab.log("Looks like the server is on fire", level="critical")
 cab.log("This is fine", level="info")
 
 # writes to a file named LOG_TEMPERATURE
-
 cab.log("30", log_name="LOG_TEMPERATURE")
 
 # writes to a file named LOG_TEMPERATURE in /home/{username}/weather
-
-cab.log("30", log_name="LOG_TEMPERATURE", file_path="/home/{username}/weather")
+cab.log("30", log_name="LOG_TEMPERATURE", log_folder_path="/home/{username}/weather")
 
     # format
     # 2021-12-29 19:29:27,896 — INFO — 30
 
 ```
 
 terminal:
```

### Comparing `cabinet-2024.3.5.1/test/test___init__.py` & `cabinet-2024.4.15.1/test/test___init__.py`

 * *Files identical despite different names*

