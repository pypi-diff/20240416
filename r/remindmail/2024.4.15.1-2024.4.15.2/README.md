# Comparing `tmp/remindmail-2024.4.15.1.tar.gz` & `tmp/remindmail-2024.4.15.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remindmail-2024.4.15.1.tar", last modified: Tue Apr 16 03:49:35 2024, max compression
+gzip compressed data, was "remindmail-2024.4.15.2.tar", last modified: Tue Apr 16 04:08:51 2024, max compression
```

## Comparing `remindmail-2024.4.15.1.tar` & `remindmail-2024.4.15.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-16 03:49:35.475697 remindmail-2024.4.15.1/
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1070 2023-12-29 22:36:09.000000 remindmail-2024.4.15.1/LICENSE.md
--rw-r--r--   0 tyler     (1000) tyler     (1000)     6600 2024-04-16 03:49:35.475697 remindmail-2024.4.15.1/PKG-INFO
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     6239 2024-04-16 03:47:36.000000 remindmail-2024.4.15.1/README.md
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)       98 2023-12-29 22:36:09.000000 remindmail-2024.4.15.1/pyproject.toml
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)      762 2024-04-16 03:49:35.475697 remindmail-2024.4.15.1/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-16 03:49:35.471697 remindmail-2024.4.15.1/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-16 03:49:35.475697 remindmail-2024.4.15.1/src/remind/
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-12-29 22:36:09.000000 remindmail-2024.4.15.1/src/remind/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     2537 2024-04-15 23:49:35.000000 remindmail-2024.4.15.1/src/remind/__main__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     1257 2024-04-15 23:49:35.000000 remindmail-2024.4.15.1/src/remind/error_handler.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    11366 2024-04-16 03:46:02.000000 remindmail-2024.4.15.1/src/remind/query_manager.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     9884 2024-04-16 02:55:43.000000 remindmail-2024.4.15.1/src/remind/reminder.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    23872 2024-04-16 03:48:14.000000 remindmail-2024.4.15.1/src/remind/reminder_confirmation.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    17715 2024-04-15 23:49:35.000000 remindmail-2024.4.15.1/src/remind/reminder_manager.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-16 03:49:35.475697 remindmail-2024.4.15.1/src/remindmail.egg-info/
--rw-r--r--   0 tyler     (1000) tyler     (1000)     6600 2024-04-16 03:49:35.000000 remindmail-2024.4.15.1/src/remindmail.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      430 2024-04-16 03:49:35.000000 remindmail-2024.4.15.1/src/remindmail.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2024-04-16 03:49:35.000000 remindmail-2024.4.15.1/src/remindmail.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       48 2024-04-16 03:49:35.000000 remindmail-2024.4.15.1/src/remindmail.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        7 2024-04-16 03:49:35.000000 remindmail-2024.4.15.1/src/remindmail.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-16 04:08:51.917256 remindmail-2024.4.15.2/
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1070 2023-12-29 22:36:09.000000 remindmail-2024.4.15.2/LICENSE.md
+-rw-r--r--   0 tyler     (1000) tyler     (1000)     6600 2024-04-16 04:08:51.917256 remindmail-2024.4.15.2/PKG-INFO
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     6239 2024-04-16 03:57:58.000000 remindmail-2024.4.15.2/README.md
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)       98 2023-12-29 22:36:09.000000 remindmail-2024.4.15.2/pyproject.toml
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)      762 2024-04-16 04:08:51.921256 remindmail-2024.4.15.2/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-16 04:08:51.917256 remindmail-2024.4.15.2/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-16 04:08:51.917256 remindmail-2024.4.15.2/src/remind/
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-12-29 22:36:09.000000 remindmail-2024.4.15.2/src/remind/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     2698 2024-04-16 03:59:27.000000 remindmail-2024.4.15.2/src/remind/__main__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1257 2024-04-15 23:49:35.000000 remindmail-2024.4.15.2/src/remind/error_handler.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    11616 2024-04-16 04:02:46.000000 remindmail-2024.4.15.2/src/remind/query_manager.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     9884 2024-04-16 02:55:43.000000 remindmail-2024.4.15.2/src/remind/reminder.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    23904 2024-04-16 04:06:27.000000 remindmail-2024.4.15.2/src/remind/reminder_confirmation.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    17715 2024-04-15 23:49:35.000000 remindmail-2024.4.15.2/src/remind/reminder_manager.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-16 04:08:51.917256 remindmail-2024.4.15.2/src/remindmail.egg-info/
+-rw-r--r--   0 tyler     (1000) tyler     (1000)     6600 2024-04-16 04:08:51.000000 remindmail-2024.4.15.2/src/remindmail.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      430 2024-04-16 04:08:51.000000 remindmail-2024.4.15.2/src/remindmail.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2024-04-16 04:08:51.000000 remindmail-2024.4.15.2/src/remindmail.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       48 2024-04-16 04:08:51.000000 remindmail-2024.4.15.2/src/remindmail.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        7 2024-04-16 04:08:51.000000 remindmail-2024.4.15.2/src/remindmail.egg-info/top_level.txt
```

### Comparing `remindmail-2024.4.15.1/LICENSE.md` & `remindmail-2024.4.15.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.15.1/PKG-INFO` & `remindmail-2024.4.15.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remindmail
-Version: 2024.4.15.1
+Version: 2024.4.15.2
 Summary: Easily schedule reminders to be emailed
 Home-page: https://github.com/tylerjwoodfin/remindmail
 Author: Tyler Woodfin
 Author-email: feedback-remindmail@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `remindmail-2024.4.15.1/README.md` & `remindmail-2024.4.15.2/README.md`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.15.1/setup.cfg` & `remindmail-2024.4.15.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = remindmail
-version = 2024.04.15.1
+version = 2024.04.15.2
 author = Tyler Woodfin
 author_email = feedback-remindmail@tyler.cloud
 description = Easily schedule reminders to be emailed
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tylerjwoodfin/remindmail
 project_urls =
```

### Comparing `remindmail-2024.4.15.1/src/remind/__main__.py` & `remindmail-2024.4.15.2/src/remind/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,14 +40,20 @@
 
     parser.add_argument(
         "--later",
         action="store_true",
         help="show reminders scheduled for later"
     )
 
+    parser.add_argument(
+        "--save",
+        action="store_true",
+        help="save reminder without confirmation"
+    )
+
     # action arguments
     parser.add_argument(
         "--generate",
         "--g",
         action="store_true",
         help="generate reminders.",
     )
@@ -84,15 +90,16 @@
             manager_r.show_reminders_for_days(2)
         elif args.show_week:
             manager_r.show_reminders_for_days()
         else:
             manager_q.wizard_manual_reminder(
                 title=args.title,
                 when=args.when,
-                notes=args.notes
+                notes=args.notes,
+                save=args.save
             )
 
     except KeyboardInterrupt as exc:
         raise KeyboardInterrupt from exc
 
 def main():
     """
```

### Comparing `remindmail-2024.4.15.1/src/remind/error_handler.py` & `remindmail-2024.4.15.2/src/remind/error_handler.py`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.15.1/src/remind/query_manager.py` & `remindmail-2024.4.15.2/src/remind/query_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import re
 import sys
 from datetime import datetime, timedelta
 from dateutil.relativedelta import relativedelta, MO, TU, WE, TH, FR, SA, SU
 from remind.reminder import Reminder, ReminderKeyType
 from remind.reminder_confirmation import ReminderConfirmation
 from remind.reminder_manager import ReminderManager
+from prompt_toolkit import print_formatted_text, HTML
 from cabinet import Cabinet, Mail
 
 class QueryManager:
     """
     handles reminder requests
     """
 
@@ -219,15 +220,16 @@
                         offset=0,
                         cabinet=self.cabinet,
                         mail=self.mail,
                         path_remind_file=self.manager.path_remind_file)
 
     def wizard_manual_reminder(self, title: str | None = None,
                                when: str | None = None,
-                               notes: str | None = None) -> Reminder:
+                               notes: str | None = None,
+                               save: bool = False) -> Reminder:
         """
         Guides the user through the process of creating a new manual reminder
         by collecting necessary information
         through interactive prompts.
 
         Parameters:
             - title (str, optional): the reminder's title (email subject)
@@ -253,19 +255,22 @@
                 reminder.title = title
                 reminder.notes = notes
                 reminder_date_success = True
             except ValueError as e:
                 print(e)
                 when = None
 
-        # display confirmation form
-        try:
-            ReminderConfirmation(reminder).run()
-        except KeyboardInterrupt:
-            sys.exit(0)
+        # display confirmation form if not `--save`
+        if not save:
+            try:
+                ReminderConfirmation(reminder).run()
+            except KeyboardInterrupt:
+                sys.exit(0)
+        else:
+            print_formatted_text(HTML('<ansigreen><b>Done.</b></ansigreen>'))
 
         # 'x' placed by ReminderConfirmation if cancelled
         if 'x' in reminder.modifiers:
             return reminder
 
         if reminder.key == ReminderKeyType.NOW:
             reminder.send_email()
```

### Comparing `remindmail-2024.4.15.1/src/remind/reminder.py` & `remindmail-2024.4.15.2/src/remind/reminder.py`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.15.1/src/remind/reminder_confirmation.py` & `remindmail-2024.4.15.2/src/remind/reminder_confirmation.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,16 @@
             self.frequency_input,
             self.offset_input,
             HSplit(children=[
                 self.modifiers_input
             ], height=2),
             HSplit(children=[
                 self.notes_input
-            ], height=3, style="bg:ansiyellow"),
+            ], height=3,
+                   style="bg:ansiyellow fg:ansiblack"),
             Window(height=1),  # button separator
             HSplit([
                 Window(width=1)
             ], padding=1),
             self.save_button,
             self.cancel_button,
             Window(height=1),  # toolbar separator
```

### Comparing `remindmail-2024.4.15.1/src/remind/reminder_manager.py` & `remindmail-2024.4.15.2/src/remind/reminder_manager.py`

 * *Files identical despite different names*

### Comparing `remindmail-2024.4.15.1/src/remindmail.egg-info/PKG-INFO` & `remindmail-2024.4.15.2/src/remindmail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remindmail
-Version: 2024.4.15.1
+Version: 2024.4.15.2
 Summary: Easily schedule reminders to be emailed
 Home-page: https://github.com/tylerjwoodfin/remindmail
 Author: Tyler Woodfin
 Author-email: feedback-remindmail@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

