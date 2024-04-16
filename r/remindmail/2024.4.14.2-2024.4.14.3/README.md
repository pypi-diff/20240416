# Comparing `tmp/remindmail-2024.4.14.2.tar.gz` & `tmp/remindmail-2024.4.14.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remindmail-2024.4.14.2.tar", last modified: Mon Apr 15 03:38:19 2024, max compression
+gzip compressed data, was "remindmail-2024.4.14.3.tar", last modified: Mon Apr 15 03:49:32 2024, max compression
```

## Comparing `remindmail-2024.4.14.2.tar` & `remindmail-2024.4.14.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-15 03:38:19.403641 remindmail-2024.4.14.2/
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1070 2023-12-29 22:36:09.000000 remindmail-2024.4.14.2/LICENSE.md
--rw-r--r--   0 tyler     (1000) tyler     (1000)     6523 2024-04-15 03:38:19.403641 remindmail-2024.4.14.2/PKG-INFO
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     6162 2024-04-15 03:34:36.000000 remindmail-2024.4.14.2/README.md
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)       98 2023-12-29 22:36:09.000000 remindmail-2024.4.14.2/pyproject.toml
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)      762 2024-04-15 03:38:19.403641 remindmail-2024.4.14.2/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-15 03:38:19.403641 remindmail-2024.4.14.2/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-15 03:38:19.403641 remindmail-2024.4.14.2/src/remind/
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-12-29 22:36:09.000000 remindmail-2024.4.14.2/src/remind/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     2537 2024-04-15 03:34:08.000000 remindmail-2024.4.14.2/src/remind/__main__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     1257 2024-04-15 03:34:08.000000 remindmail-2024.4.14.2/src/remind/error_handler.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    11268 2024-04-15 03:34:08.000000 remindmail-2024.4.14.2/src/remind/query_manager.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     9889 2024-04-15 03:34:08.000000 remindmail-2024.4.14.2/src/remind/reminder.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    23906 2024-04-15 03:34:08.000000 remindmail-2024.4.14.2/src/remind/reminder_confirmation.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    17715 2024-04-15 03:34:08.000000 remindmail-2024.4.14.2/src/remind/reminder_manager.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-15 03:38:19.403641 remindmail-2024.4.14.2/src/remindmail.egg-info/
--rw-r--r--   0 tyler     (1000) tyler     (1000)     6523 2024-04-15 03:38:19.000000 remindmail-2024.4.14.2/src/remindmail.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      430 2024-04-15 03:38:19.000000 remindmail-2024.4.14.2/src/remindmail.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2024-04-15 03:38:19.000000 remindmail-2024.4.14.2/src/remindmail.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       48 2024-04-15 03:38:19.000000 remindmail-2024.4.14.2/src/remindmail.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        7 2024-04-15 03:38:19.000000 remindmail-2024.4.14.2/src/remindmail.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-15 03:49:32.189559 remindmail-2024.4.14.3/
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1070 2023-12-29 22:36:09.000000 remindmail-2024.4.14.3/LICENSE.md
+-rw-r--r--   0 tyler     (1000) tyler     (1000)     6523 2024-04-15 03:49:32.189559 remindmail-2024.4.14.3/PKG-INFO
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     6162 2024-04-15 03:34:36.000000 remindmail-2024.4.14.3/README.md
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)       98 2023-12-29 22:36:09.000000 remindmail-2024.4.14.3/pyproject.toml
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)      762 2024-04-15 03:49:32.189559 remindmail-2024.4.14.3/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-15 03:49:32.185560 remindmail-2024.4.14.3/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-15 03:49:32.189559 remindmail-2024.4.14.3/src/remind/
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-12-29 22:36:09.000000 remindmail-2024.4.14.3/src/remind/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     2537 2024-04-15 03:34:08.000000 remindmail-2024.4.14.3/src/remind/__main__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1257 2024-04-15 03:34:08.000000 remindmail-2024.4.14.3/src/remind/error_handler.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    11268 2024-04-15 03:34:08.000000 remindmail-2024.4.14.3/src/remind/query_manager.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     9884 2024-04-15 03:45:52.000000 remindmail-2024.4.14.3/src/remind/reminder.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    23906 2024-04-15 03:34:08.000000 remindmail-2024.4.14.3/src/remind/reminder_confirmation.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    17715 2024-04-15 03:34:08.000000 remindmail-2024.4.14.3/src/remind/reminder_manager.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-15 03:49:32.189559 remindmail-2024.4.14.3/src/remindmail.egg-info/
+-rw-r--r--   0 tyler     (1000) tyler     (1000)     6523 2024-04-15 03:49:32.000000 remindmail-2024.4.14.3/src/remindmail.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      430 2024-04-15 03:49:32.000000 remindmail-2024.4.14.3/src/remindmail.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2024-04-15 03:49:32.000000 remindmail-2024.4.14.3/src/remindmail.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       48 2024-04-15 03:49:32.000000 remindmail-2024.4.14.3/src/remindmail.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        7 2024-04-15 03:49:32.000000 remindmail-2024.4.14.3/src/remindmail.egg-info/top_level.txt
```

### Comparing `remindmail-2024.4.14.2/LICENSE.md` & `remindmail-2024.4.14.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.14.2/PKG-INFO` & `remindmail-2024.4.14.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remindmail
-Version: 2024.4.14.2
+Version: 2024.4.14.3
 Summary: Easily schedule reminders to be emailed
 Home-page: https://github.com/tylerjwoodfin/remindmail
 Author: Tyler Woodfin
 Author-email: feedback-remindmail@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `remindmail-2024.4.14.2/README.md` & `remindmail-2024.4.14.3/README.md`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.14.2/setup.cfg` & `remindmail-2024.4.14.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = remindmail
-version = 2024.04.14.2
+version = 2024.04.14.3
 author = Tyler Woodfin
 author_email = feedback-remindmail@tyler.cloud
 description = Easily schedule reminders to be emailed
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tylerjwoodfin/remindmail
 project_urls =
```

### Comparing `remindmail-2024.4.14.2/src/remind/__main__.py` & `remindmail-2024.4.14.3/src/remind/__main__.py`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.14.2/src/remind/error_handler.py` & `remindmail-2024.4.14.3/src/remind/error_handler.py`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.14.2/src/remind/query_manager.py` & `remindmail-2024.4.14.3/src/remind/query_manager.py`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.14.2/src/remind/reminder.py` & `remindmail-2024.4.14.3/src/remind/reminder.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,12 +247,12 @@
 
         reminder_format = format_reminder()
 
         path_remind_file = self.path_remind_file or \
             self.cabinet.get('path', 'remindmail', 'file') or ""
         path_remind_folder = path_remind_file.replace("/remind.md", "")
 
-        self.cabinet.write_file(path_remind_file,
+        self.cabinet.write_file('remind.md',
                                 path_remind_folder,
                                 reminder_format,
                                 append=True,
                                 is_quiet=is_quiet)
```

### Comparing `remindmail-2024.4.14.2/src/remind/reminder_confirmation.py` & `remindmail-2024.4.14.3/src/remind/reminder_confirmation.py`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.14.2/src/remind/reminder_manager.py` & `remindmail-2024.4.14.3/src/remind/reminder_manager.py`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.14.2/src/remindmail.egg-info/PKG-INFO` & `remindmail-2024.4.14.3/src/remindmail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remindmail
-Version: 2024.4.14.2
+Version: 2024.4.14.3
 Summary: Easily schedule reminders to be emailed
 Home-page: https://github.com/tylerjwoodfin/remindmail
 Author: Tyler Woodfin
 Author-email: feedback-remindmail@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

