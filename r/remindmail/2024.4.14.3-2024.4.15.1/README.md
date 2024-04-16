# Comparing `tmp/remindmail-2024.4.14.3.tar.gz` & `tmp/remindmail-2024.4.15.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remindmail-2024.4.14.3.tar", last modified: Mon Apr 15 03:49:32 2024, max compression
+gzip compressed data, was "remindmail-2024.4.15.1.tar", last modified: Tue Apr 16 03:49:35 2024, max compression
```

## Comparing `remindmail-2024.4.14.3.tar` & `remindmail-2024.4.15.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-15 03:49:32.189559 remindmail-2024.4.14.3/
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1070 2023-12-29 22:36:09.000000 remindmail-2024.4.14.3/LICENSE.md
--rw-r--r--   0 tyler     (1000) tyler     (1000)     6523 2024-04-15 03:49:32.189559 remindmail-2024.4.14.3/PKG-INFO
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     6162 2024-04-15 03:34:36.000000 remindmail-2024.4.14.3/README.md
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)       98 2023-12-29 22:36:09.000000 remindmail-2024.4.14.3/pyproject.toml
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)      762 2024-04-15 03:49:32.189559 remindmail-2024.4.14.3/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-15 03:49:32.185560 remindmail-2024.4.14.3/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-15 03:49:32.189559 remindmail-2024.4.14.3/src/remind/
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-12-29 22:36:09.000000 remindmail-2024.4.14.3/src/remind/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     2537 2024-04-15 03:34:08.000000 remindmail-2024.4.14.3/src/remind/__main__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     1257 2024-04-15 03:34:08.000000 remindmail-2024.4.14.3/src/remind/error_handler.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    11268 2024-04-15 03:34:08.000000 remindmail-2024.4.14.3/src/remind/query_manager.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     9884 2024-04-15 03:45:52.000000 remindmail-2024.4.14.3/src/remind/reminder.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    23906 2024-04-15 03:34:08.000000 remindmail-2024.4.14.3/src/remind/reminder_confirmation.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    17715 2024-04-15 03:34:08.000000 remindmail-2024.4.14.3/src/remind/reminder_manager.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-15 03:49:32.189559 remindmail-2024.4.14.3/src/remindmail.egg-info/
--rw-r--r--   0 tyler     (1000) tyler     (1000)     6523 2024-04-15 03:49:32.000000 remindmail-2024.4.14.3/src/remindmail.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      430 2024-04-15 03:49:32.000000 remindmail-2024.4.14.3/src/remindmail.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2024-04-15 03:49:32.000000 remindmail-2024.4.14.3/src/remindmail.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       48 2024-04-15 03:49:32.000000 remindmail-2024.4.14.3/src/remindmail.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        7 2024-04-15 03:49:32.000000 remindmail-2024.4.14.3/src/remindmail.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-16 03:49:35.475697 remindmail-2024.4.15.1/
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1070 2023-12-29 22:36:09.000000 remindmail-2024.4.15.1/LICENSE.md
+-rw-r--r--   0 tyler     (1000) tyler     (1000)     6600 2024-04-16 03:49:35.475697 remindmail-2024.4.15.1/PKG-INFO
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     6239 2024-04-16 03:47:36.000000 remindmail-2024.4.15.1/README.md
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)       98 2023-12-29 22:36:09.000000 remindmail-2024.4.15.1/pyproject.toml
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)      762 2024-04-16 03:49:35.475697 remindmail-2024.4.15.1/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-16 03:49:35.471697 remindmail-2024.4.15.1/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-16 03:49:35.475697 remindmail-2024.4.15.1/src/remind/
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-12-29 22:36:09.000000 remindmail-2024.4.15.1/src/remind/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     2537 2024-04-15 23:49:35.000000 remindmail-2024.4.15.1/src/remind/__main__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1257 2024-04-15 23:49:35.000000 remindmail-2024.4.15.1/src/remind/error_handler.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    11366 2024-04-16 03:46:02.000000 remindmail-2024.4.15.1/src/remind/query_manager.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     9884 2024-04-16 02:55:43.000000 remindmail-2024.4.15.1/src/remind/reminder.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    23872 2024-04-16 03:48:14.000000 remindmail-2024.4.15.1/src/remind/reminder_confirmation.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    17715 2024-04-15 23:49:35.000000 remindmail-2024.4.15.1/src/remind/reminder_manager.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-16 03:49:35.475697 remindmail-2024.4.15.1/src/remindmail.egg-info/
+-rw-r--r--   0 tyler     (1000) tyler     (1000)     6600 2024-04-16 03:49:35.000000 remindmail-2024.4.15.1/src/remindmail.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      430 2024-04-16 03:49:35.000000 remindmail-2024.4.15.1/src/remindmail.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2024-04-16 03:49:35.000000 remindmail-2024.4.15.1/src/remindmail.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       48 2024-04-16 03:49:35.000000 remindmail-2024.4.15.1/src/remindmail.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        7 2024-04-16 03:49:35.000000 remindmail-2024.4.15.1/src/remindmail.egg-info/top_level.txt
```

### Comparing `remindmail-2024.4.14.3/LICENSE.md` & `remindmail-2024.4.15.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.14.3/PKG-INFO` & `remindmail-2024.4.15.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remindmail
-Version: 2024.4.14.3
+Version: 2024.4.15.1
 Summary: Easily schedule reminders to be emailed
 Home-page: https://github.com/tylerjwoodfin/remindmail
 Author: Tyler Woodfin
 Author-email: feedback-remindmail@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -91,14 +91,15 @@
 
 - `remind`: Schedule a new reminder interactively
 - `remind --title 'reminder title' --when 'june 20'`: Schedule a new reminder programatically
 - `remind --title 'reminder title' --when '2024-06-20'`: Schedule a new reminder programatically
 - `remind --title 'reminder title' --when 'every 3 weeks'`: Schedule a new reminder programatically
 - `remind --title 'reminder title' --when 'friday'`: Schedule a new reminder programatically
 - `remind --title 'reminder title' --when 'every 2 Mondays'`: Schedule a new reminder programatically
+- `remind --title 'reminder title' --when 'now'`: Sends an email immediately
 - `remind -h` (or `--help`): Displays usage information.
 - `remind -g` (or `--generate`): Generates all reminders scheduled for today. 
   - I recommend setting up a crontab.
 - `remind --later`: Emails reminders that are marked with `[later]`
 - `remind --st` (or `--show-tomorrow`): Lists reminders in remind.md that target tomorrow's date
 - `remind --sw` (or `--show-week`): Lists reminders for the next 7 days
 - `remind -e` (or `--edit`): Opens `remind.md` in vim
```

### Comparing `remindmail-2024.4.14.3/README.md` & `remindmail-2024.4.15.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,15 @@
 
 - `remind`: Schedule a new reminder interactively
 - `remind --title 'reminder title' --when 'june 20'`: Schedule a new reminder programatically
 - `remind --title 'reminder title' --when '2024-06-20'`: Schedule a new reminder programatically
 - `remind --title 'reminder title' --when 'every 3 weeks'`: Schedule a new reminder programatically
 - `remind --title 'reminder title' --when 'friday'`: Schedule a new reminder programatically
 - `remind --title 'reminder title' --when 'every 2 Mondays'`: Schedule a new reminder programatically
+- `remind --title 'reminder title' --when 'now'`: Sends an email immediately
 - `remind -h` (or `--help`): Displays usage information.
 - `remind -g` (or `--generate`): Generates all reminders scheduled for today. 
   - I recommend setting up a crontab.
 - `remind --later`: Emails reminders that are marked with `[later]`
 - `remind --st` (or `--show-tomorrow`): Lists reminders in remind.md that target tomorrow's date
 - `remind --sw` (or `--show-week`): Lists reminders for the next 7 days
 - `remind -e` (or `--edit`): Opens `remind.md` in vim
```

### Comparing `remindmail-2024.4.14.3/setup.cfg` & `remindmail-2024.4.15.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = remindmail
-version = 2024.04.14.3
+version = 2024.04.15.1
 author = Tyler Woodfin
 author_email = feedback-remindmail@tyler.cloud
 description = Easily schedule reminders to be emailed
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tylerjwoodfin/remindmail
 project_urls =
```

### Comparing `remindmail-2024.4.14.3/src/remind/__main__.py` & `remindmail-2024.4.15.1/src/remind/__main__.py`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.14.3/src/remind/error_handler.py` & `remindmail-2024.4.15.1/src/remind/error_handler.py`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.14.3/src/remind/query_manager.py` & `remindmail-2024.4.15.1/src/remind/query_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,14 +153,18 @@
                 value = date_formatted.strftime('%Y-%m-%d')
 
             # tomorrow
             elif input_str == 'tomorrow':
                 key = ReminderKeyType.DATE
                 value = start_date.strftime('%Y-%m-%d')
 
+            # now
+            elif input_str == 'now':
+                key = ReminderKeyType.NOW
+
         else:
             # 'every'
             modifiers = ''
 
             # every n days
             if match := regex_patterns['every_n_days'].match(input_str):
                 key = ReminderKeyType.DAY
```

### Comparing `remindmail-2024.4.14.3/src/remind/reminder.py` & `remindmail-2024.4.15.1/src/remind/reminder.py`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.14.3/src/remind/reminder_confirmation.py` & `remindmail-2024.4.15.1/src/remind/reminder_confirmation.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,21 +157,21 @@
         self.notes_input = TextArea(text=self.reminder.notes or "",
                                     multiline=True, prompt='Notes: ')
 
         # save
         self.save_button = TextArea(text='Save',
                                     read_only=True,
                                     multiline=False,
-                                    style='fg:ansigreen bold blink')
+                                    style='fg:ansigreen')
 
         # cancel
         self.cancel_button = TextArea(text='Cancel',
                                     read_only=True,
                                     multiline=False,
-                                    style='fg:ansired bold blink')
+                                    style='fg:ansired')
 
         # toolbar
         self.toolbar = Box(
             body=Label(text=lambda: self.toolbar_text, align=WindowAlign.LEFT),
             style="reverse",
             height=1,
             padding_left=1,
@@ -364,21 +364,21 @@
 
         if current_index is None:
             # handle the case where the current type is not found
             # (should not happen in normal circumstances)
             return
 
         # calculate the new index cyclically
-        new_index = (current_index + direction) % len(self.reminder_types)
+        new_index: int = (current_index + direction) % len(self.reminder_types)
 
         # set cache
         self.key_value_cache[self.reminder.key.label] = self.value_text_area.text
 
         # update the reminder's type with the new type
-        self.reminder.key: ReminderKeyType = self.reminder_types[new_index]
+        self.reminder.key = self.reminder_types[new_index]
 
         # update the text area with the new type label
         self.type_input.text = self.reminder.key.label
 
         self.update_toolbar_text()
 
         # get cache
```

### Comparing `remindmail-2024.4.14.3/src/remind/reminder_manager.py` & `remindmail-2024.4.15.1/src/remind/reminder_manager.py`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.14.3/src/remindmail.egg-info/PKG-INFO` & `remindmail-2024.4.15.1/src/remindmail.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remindmail
-Version: 2024.4.14.3
+Version: 2024.4.15.1
 Summary: Easily schedule reminders to be emailed
 Home-page: https://github.com/tylerjwoodfin/remindmail
 Author: Tyler Woodfin
 Author-email: feedback-remindmail@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -91,14 +91,15 @@
 
 - `remind`: Schedule a new reminder interactively
 - `remind --title 'reminder title' --when 'june 20'`: Schedule a new reminder programatically
 - `remind --title 'reminder title' --when '2024-06-20'`: Schedule a new reminder programatically
 - `remind --title 'reminder title' --when 'every 3 weeks'`: Schedule a new reminder programatically
 - `remind --title 'reminder title' --when 'friday'`: Schedule a new reminder programatically
 - `remind --title 'reminder title' --when 'every 2 Mondays'`: Schedule a new reminder programatically
+- `remind --title 'reminder title' --when 'now'`: Sends an email immediately
 - `remind -h` (or `--help`): Displays usage information.
 - `remind -g` (or `--generate`): Generates all reminders scheduled for today. 
   - I recommend setting up a crontab.
 - `remind --later`: Emails reminders that are marked with `[later]`
 - `remind --st` (or `--show-tomorrow`): Lists reminders in remind.md that target tomorrow's date
 - `remind --sw` (or `--show-week`): Lists reminders for the next 7 days
 - `remind -e` (or `--edit`): Opens `remind.md` in vim
```

